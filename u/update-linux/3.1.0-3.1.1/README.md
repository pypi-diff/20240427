# Comparing `tmp/update-linux-3.1.0.tar.gz` & `tmp/update_linux-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "update-linux-3.1.0.tar", last modified: Wed Nov  8 21:26:56 2023, max compression
+gzip compressed data, was "update_linux-3.1.1.tar", last modified: Sat Apr 27 19:42:47 2024, max compression
```

## Comparing `update-linux-3.1.0.tar` & `update_linux-3.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-11-08 21:26:56.155924 update-linux-3.1.0/
--rw-r--r--   0 barry     (1000) barry     (1000)    11357 2023-07-31 10:07:15.000000 update-linux-3.1.0/LICENSE
--rw-r--r--   0 barry     (1000) barry     (1000)     6612 2023-11-08 21:26:56.155924 update-linux-3.1.0/PKG-INFO
--rw-r--r--   0 barry     (1000) barry     (1000)     5894 2023-08-06 10:10:09.000000 update-linux-3.1.0/README.md
--rw-r--r--   0 barry     (1000) barry     (1000)      992 2023-10-03 19:03:41.000000 update-linux-3.1.0/pyproject.toml
--rw-r--r--   0 barry     (1000) barry     (1000)       33 2023-07-31 10:33:16.000000 update-linux-3.1.0/requirements.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       38 2023-11-08 21:26:56.155924 update-linux-3.1.0/setup.cfg
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-11-08 21:26:56.154924 update-linux-3.1.0/src/
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-11-08 21:26:56.154924 update-linux-3.1.0/src/update_linux/
--rwxr-xr-x   0 barry     (1000) barry     (1000)    27311 2023-11-08 21:23:33.000000 update-linux-3.1.0/src/update_linux/__init__.py
--rw-r--r--   0 barry     (1000) barry     (1000)      144 2023-04-15 15:36:02.000000 update-linux-3.1.0/src/update_linux/__main__.py
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-11-08 21:26:56.155924 update-linux-3.1.0/src/update_linux.egg-info/
--rw-r--r--   0 barry     (1000) barry     (1000)     6612 2023-11-08 21:26:56.000000 update-linux-3.1.0/src/update_linux.egg-info/PKG-INFO
--rw-r--r--   0 barry     (1000) barry     (1000)      349 2023-11-08 21:26:56.000000 update-linux-3.1.0/src/update_linux.egg-info/SOURCES.txt
--rw-r--r--   0 barry     (1000) barry     (1000)        1 2023-11-08 21:26:56.000000 update-linux-3.1.0/src/update_linux.egg-info/dependency_links.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       60 2023-11-08 21:26:56.000000 update-linux-3.1.0/src/update_linux.egg-info/entry_points.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       33 2023-11-08 21:26:56.000000 update-linux-3.1.0/src/update_linux.egg-info/requires.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       13 2023-11-08 21:26:56.000000 update-linux-3.1.0/src/update_linux.egg-info/top_level.txt
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2024-04-27 19:42:47.929817 update_linux-3.1.1/
+-rw-r--r--   0 barry     (1000) barry     (1000)    11357 2023-07-31 10:07:15.000000 update_linux-3.1.1/LICENSE
+-rw-r--r--   0 barry     (1000) barry     (1000)     6612 2024-04-27 19:42:47.929817 update_linux-3.1.1/PKG-INFO
+-rw-r--r--   0 barry     (1000) barry     (1000)     5894 2023-08-06 10:10:09.000000 update_linux-3.1.1/README.md
+-rw-r--r--   0 barry     (1000) barry     (1000)      993 2024-04-27 19:41:50.000000 update_linux-3.1.1/pyproject.toml
+-rw-r--r--   0 barry     (1000) barry     (1000)       33 2023-07-31 10:33:16.000000 update_linux-3.1.1/requirements.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       38 2024-04-27 19:42:47.929817 update_linux-3.1.1/setup.cfg
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2024-04-27 19:42:47.928817 update_linux-3.1.1/src/
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2024-04-27 19:42:47.929817 update_linux-3.1.1/src/update_linux/
+-rwxr-xr-x   0 barry     (1000) barry     (1000)    28008 2024-04-27 19:41:50.000000 update_linux-3.1.1/src/update_linux/__init__.py
+-rw-r--r--   0 barry     (1000) barry     (1000)      144 2023-04-15 15:36:02.000000 update_linux-3.1.1/src/update_linux/__main__.py
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2024-04-27 19:42:47.929817 update_linux-3.1.1/src/update_linux.egg-info/
+-rw-r--r--   0 barry     (1000) barry     (1000)     6612 2024-04-27 19:42:47.000000 update_linux-3.1.1/src/update_linux.egg-info/PKG-INFO
+-rw-r--r--   0 barry     (1000) barry     (1000)      349 2024-04-27 19:42:47.000000 update_linux-3.1.1/src/update_linux.egg-info/SOURCES.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)        1 2024-04-27 19:42:47.000000 update_linux-3.1.1/src/update_linux.egg-info/dependency_links.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       60 2024-04-27 19:42:47.000000 update_linux-3.1.1/src/update_linux.egg-info/entry_points.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       33 2024-04-27 19:42:47.000000 update_linux-3.1.1/src/update_linux.egg-info/requires.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       13 2024-04-27 19:42:47.000000 update_linux-3.1.1/src/update_linux.egg-info/top_level.txt
```

### Comparing `update-linux-3.1.0/LICENSE` & `update_linux-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `update-linux-3.1.0/PKG-INFO` & `update_linux-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: update-linux
-Version: 3.1.0
+Version: 3.1.1
 Summary: Command to automate the routine updating of packages and system upgrading for Unix systems.
 Author-email: Barry Scott <barry@barrys-emacs.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/barry-scott/CLI-tools
 Project-URL: Bug Tracker, https://github.com/barry-scott/CLI-tools/issues
 Keywords: development
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `update-linux-3.1.0/README.md` & `update_linux-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `update-linux-3.1.0/pyproject.toml` & `update_linux-3.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "update-linux"
 authors = [
     {name = "Barry Scott", email = "barry@barrys-emacs.org"},
 ]
 description = "Command to automate the routine updating of packages and system upgrading for Unix systems."
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">= 3.10"
 license = {text = "Apache-2.0"}
 keywords = [ "development" ]
 classifiers = [
     "Intended Audience :: End Users/Desktop",
     "Topic :: Utilities",
     "Environment :: Console",
     "Programming Language :: Python :: 3",
```

### Comparing `update-linux-3.1.0/src/update_linux/__init__.py` & `update_linux-3.1.1/src/update_linux/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import time
 import socket
 import platform
 import tempfile
 import json
 from config_path import ConfigPath  # type: ignore
 
-VERSION = '3.1.0'
+VERSION = '3.1.1'
 
 default_json_config_template = u'''{
     "group":
         {"all": []},
     "logdir":   "%(logdir)s"
 }
 '''
@@ -414,19 +414,30 @@
                 return os_id, os_main_id, os_version_id
 
         return None, os_main_id, os_version_id
 
     def reboot( self, host, cmd, wait_limit=600 ):
         while True:
             rc, stdout = self.runAndLog( host, cmd )
-            if len(stdout) == 0:
+            # filter out warning/info messages before checking for success
+            filtered_stdout = []
+            for line in stdout:
+                if line.startswith(
+                        ('Warning: '
+                        ,'Offending key for '
+                        ,'Matching host key in ')):
+                    continue
+                filtered_stdout.append(line)
+
+            if len(filtered_stdout) == 0:
                 # no messages assume ok
                 break
 
-            if stdout[0] == ('Connection to %s closed by remote host.\r\n' % (host,)):
+            if( filtered_stdout[0].startswith('Connection to ')
+            and filtered_stdout[0].endswith('closed by remote host.\r\n') ):
                 # this is success
                 break
 
             self.error( host, 'reboot stdout: %r' % (stdout,) )
 
             self.info( host, 'Retry reboot in 10s' )
             time.sleep( 10 )
@@ -658,15 +669,23 @@
         if self.app.reboot( host, ['dnf', 'system-upgrade', 'reboot'], wait_limit=45*60 ):
             self.app.checkServices( host, upgrade_log_name )
 
         self.app.info( host, 'Now running release %d' % (self.releaseInfo( host ),) )
 
     def releaseInfo( self, host ):
         cmd = ['cat', '/etc/system-release-cpe']
-        rc, stdout = self.app.runAndLog( host, cmd, log=False )
+        # first boot after a system upgrade seen to block this access
+        log = False
+        for _ in range(10):
+            rc, stdout = self.app.runAndLog( host, cmd, log=log )
+            if 'System is booting up' not in stdout[0]:
+                break
+            log = True
+            time.sleep(5)
+
         cpe_parts = stdout[0].strip().split( ':' )
         if len(cpe_parts) >= 4:
             return int( cpe_parts[4] )
 
         self.app.error( host, 'Not enough fields in /etc/system-release-cpe - %r' % (cpe_parts,) )
         return 0
```

### Comparing `update-linux-3.1.0/src/update_linux.egg-info/PKG-INFO` & `update_linux-3.1.1/src/update_linux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: update-linux
-Version: 3.1.0
+Version: 3.1.1
 Summary: Command to automate the routine updating of packages and system upgrading for Unix systems.
 Author-email: Barry Scott <barry@barrys-emacs.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/barry-scott/CLI-tools
 Project-URL: Bug Tracker, https://github.com/barry-scott/CLI-tools/issues
 Keywords: development
 Classifier: Intended Audience :: End Users/Desktop
```

