# Comparing `tmp/smtp_proxy-0.1.1.tar.gz` & `tmp/smtp_proxy-0.1.2.tar.gz`

## Comparing `smtp_proxy-0.1.1.tar` & `smtp_proxy-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 smtp_proxy-0.1.1/CHANGES.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smtp_proxy-0.1.1/src/smtp_proxy/__init__.py
--rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 smtp_proxy-0.1.1/src/smtp_proxy/smtp_proxy.py
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 smtp_proxy-0.1.1/tests/test_smtp_proxy.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 smtp_proxy-0.1.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 smtp_proxy-0.1.1/LICENSE
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 smtp_proxy-0.1.1/README.md
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 smtp_proxy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 smtp_proxy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 smtp_proxy-0.1.2/CHANGES.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smtp_proxy-0.1.2/src/smtp_proxy/__init__.py
+-rw-r--r--   0        0        0     7184 2020-02-02 00:00:00.000000 smtp_proxy-0.1.2/src/smtp_proxy/smtp_proxy.py
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 smtp_proxy-0.1.2/tests/test_smtp_proxy.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 smtp_proxy-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 smtp_proxy-0.1.2/LICENSE
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 smtp_proxy-0.1.2/README.md
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 smtp_proxy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 smtp_proxy-0.1.2/PKG-INFO
```

### Comparing `smtp_proxy-0.1.1/src/smtp_proxy/smtp_proxy.py` & `smtp_proxy-0.1.2/src/smtp_proxy/smtp_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import click
 import logging
 import asyncio
 import email.message
 import email.parser
 import signal
+import os
 
 from aiosmtpd.controller import Controller
 from aiosmtpd.smtp import Envelope
 from async_sendgrid import SendgridAPI
 from sendgrid import SendGridAPIClient
 from sendgrid.helpers.mail import Mail
 
@@ -80,30 +81,31 @@
                     response = await self.sendMail(payload)
 
                     # TODO: Adapt to MS Graph response value + add wait until support
                     if response.status_code < 400:
                         log.debug(f"Payload Sent!")
                         break
                     else:
-                        raise Exception(f"[{response.status_code}: {response.body}]")
+                        raise Exception(f"[{response.status_code}: {response.text}]")
                 except Exception as err:
                     retries += 1
                     errorMsg = f"Could not process your {className} message {mailArgs['subject']} to {mailArgs['rcpt_tos']}: {err}"
                     log.debug(err)
                     if retries == MAX_RETRIES:
                         log.error(f"Retry limit reached, giving up on {errorMsg}!")
                     else:
                         log.warning(f"Retry attempt {retries}: {errorMsg}")
                         await asyncio.sleep(1 * retries)
             self.queue.task_done()
 
 
 class SendgridHandler(BaseHandler):
     def getClient(self, **kwargs):
-        return SendgridAPI(kwargs["sendgrid_api_key"])
+        environKey = os.environ.get("SENDGRID_API_KEY")
+        return SendgridAPI(kwargs.get("sendgrid_api_key", environKey))
 
     def processPayload(self, mailArgs):
         sg_msg = Mail(
             from_email=mailArgs["mail_from"],
             to_emails=mailArgs["rcpt_tos"],
             subject=mailArgs["subject"],
             html_content=mailArgs["body"],
```

### Comparing `smtp_proxy-0.1.1/tests/test_smtp_proxy.py` & `smtp_proxy-0.1.2/tests/test_smtp_proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,42 @@
 import pytest
+import os
 from smtp_proxy.smtp_proxy import SmtpProxyServer, SendgridHandler
 
 from unittest import mock
 from async_sendgrid import SendgridAPI
 from aiosmtpd.smtp import Envelope
 
 
 def test_smtp_proxy_sendgrid_start():
     server = SmtpProxyServer(
         hostname="localtest", port=42, max_concurrent_requests=5, sendgrid_api_key="test"
     )
 
+    assert server.handler.client.api_key == "test"
+
+    # Don't keep the server alive, just initialize it
+    server.controller.start = mock.Mock()
+    server.handler.continueLoop = False
+
+    server.start()
+
+    # Server is initialized with the correct handler, client, and number of tasks
+    assert len(server.asyncTasks) == 5
+    assert isinstance(server.controller.handler, SendgridHandler)
+    assert isinstance(server.handler.client, SendgridAPI)
+
+def test_smtp_proxy_sendgrid_start_env_var():
+    os.environ['SENDGRID_API_KEY'] = "envTest"
+    server = SmtpProxyServer(
+        hostname="localtest", port=42, max_concurrent_requests=5
+    )
+
+    assert server.handler.client.api_key == "envTest"
+
     # Don't keep the server alive, just initialize it
     server.controller.start = mock.Mock()
     server.handler.continueLoop = False
 
     server.start()
 
     # Server is initialized with the correct handler, client, and number of tasks
```

### Comparing `smtp_proxy-0.1.1/LICENSE` & `smtp_proxy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smtp_proxy-0.1.1/pyproject.toml` & `smtp_proxy-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "smtp-proxy"
-version = "0.1.1"
+version = "0.1.2"
 description = "SMTP server meant to redirect SMTP requests to a third-party email provider"
 readme = "README.md"
 requires-python = ">=3"
 keywords = ["smtp", "email", "proxy"]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `smtp_proxy-0.1.1/PKG-INFO` & `smtp_proxy-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smtp-proxy
-Version: 0.1.1
+Version: 0.1.2
 Summary: SMTP server meant to redirect SMTP requests to a third-party email provider
 License-File: LICENSE
 Keywords: email,proxy,smtp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

