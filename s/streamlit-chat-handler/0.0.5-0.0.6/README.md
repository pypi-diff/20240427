# Comparing `tmp/streamlit_chat_handler-0.0.5.tar.gz` & `tmp/streamlit_chat_handler-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_chat_handler-0.0.5.tar", last modified: Fri Apr 26 01:31:38 2024, max compression
+gzip compressed data, was "streamlit_chat_handler-0.0.6.tar", last modified: Fri Apr 26 17:56:42 2024, max compression
```

## Comparing `streamlit_chat_handler-0.0.5.tar` & `streamlit_chat_handler-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-26 01:31:38.672776 streamlit_chat_handler-0.0.5/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.0.5/LICENSE
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2024-04-26 01:31:38.672776 streamlit_chat_handler-0.0.5/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.0.5/README.md
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-26 01:31:38.672776 streamlit_chat_handler-0.0.5/examples/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      690 2024-04-23 03:41:26.000000 streamlit_chat_handler-0.0.5/examples/template.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1308 2024-04-26 01:31:13.000000 streamlit_chat_handler-0.0.5/pyproject.toml
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      363 2024-04-25 04:44:43.000000 streamlit_chat_handler-0.0.5/requirements.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-26 01:31:38.672776 streamlit_chat_handler-0.0.5/setup.cfg
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-26 01:31:38.672776 streamlit_chat_handler-0.0.5/streamlit_chat_handler/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.0.5/streamlit_chat_handler/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7672 2024-04-26 01:30:23.000000 streamlit_chat_handler-0.0.5/streamlit_chat_handler/_handler.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2056 2024-04-23 03:47:04.000000 streamlit_chat_handler-0.0.5/streamlit_chat_handler/types.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-26 01:31:38.672776 streamlit_chat_handler-0.0.5/streamlit_chat_handler.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2024-04-26 01:31:38.000000 streamlit_chat_handler-0.0.5/streamlit_chat_handler.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      401 2024-04-26 01:31:38.000000 streamlit_chat_handler-0.0.5/streamlit_chat_handler.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-26 01:31:38.000000 streamlit_chat_handler-0.0.5/streamlit_chat_handler.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      279 2024-04-26 01:31:38.000000 streamlit_chat_handler-0.0.5/streamlit_chat_handler.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-26 01:31:38.000000 streamlit_chat_handler-0.0.5/streamlit_chat_handler.egg-info/top_level.txt
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-26 17:56:42.623819 streamlit_chat_handler-0.0.6/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.0.6/LICENSE
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2024-04-26 17:56:42.623819 streamlit_chat_handler-0.0.6/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.0.6/README.md
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-26 17:56:42.619819 streamlit_chat_handler-0.0.6/examples/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      690 2024-04-23 03:41:26.000000 streamlit_chat_handler-0.0.6/examples/template.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1308 2024-04-26 17:55:03.000000 streamlit_chat_handler-0.0.6/pyproject.toml
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      363 2024-04-25 04:44:43.000000 streamlit_chat_handler-0.0.6/requirements.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-26 17:56:42.623819 streamlit_chat_handler-0.0.6/setup.cfg
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-26 17:56:42.619819 streamlit_chat_handler-0.0.6/streamlit_chat_handler/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.0.6/streamlit_chat_handler/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     7788 2024-04-26 17:54:23.000000 streamlit_chat_handler-0.0.6/streamlit_chat_handler/_handler.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2056 2024-04-23 03:47:04.000000 streamlit_chat_handler-0.0.6/streamlit_chat_handler/types.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-26 17:56:42.619819 streamlit_chat_handler-0.0.6/streamlit_chat_handler.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2024-04-26 17:56:42.000000 streamlit_chat_handler-0.0.6/streamlit_chat_handler.egg-info/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      401 2024-04-26 17:56:42.000000 streamlit_chat_handler-0.0.6/streamlit_chat_handler.egg-info/SOURCES.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-26 17:56:42.000000 streamlit_chat_handler-0.0.6/streamlit_chat_handler.egg-info/dependency_links.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      279 2024-04-26 17:56:42.000000 streamlit_chat_handler-0.0.6/streamlit_chat_handler.egg-info/requires.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-26 17:56:42.000000 streamlit_chat_handler-0.0.6/streamlit_chat_handler.egg-info/top_level.txt
```

### Comparing `streamlit_chat_handler-0.0.5/LICENSE` & `streamlit_chat_handler-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.0.5/PKG-INFO` & `streamlit_chat_handler-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.0.5
+Version: 0.0.6
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```

### Comparing `streamlit_chat_handler-0.0.5/README.md` & `streamlit_chat_handler-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.0.5/examples/template.py` & `streamlit_chat_handler-0.0.6/examples/template.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.0.5/pyproject.toml` & `streamlit_chat_handler-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]
 authors = [
   {name = "Eduardo Messias de Morais", email = "emdemor415@gmail.com" },
 ]
-version = "0.0.5"
+version = "0.0.6"
 dynamic = ["dependencies"]
 
 [project.optional-dependencies]
 lint = [
     "black==23.7.0",
     "flake8==6.1.0",
     "Flake8-pyproject==1.2.3",
```

### Comparing `streamlit_chat_handler-0.0.5/streamlit_chat_handler/_handler.py` & `streamlit_chat_handler-0.0.6/streamlit_chat_handler/_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     def append(
         self,
         role: Literal["user", "assistant"],
         type: str,
         content: Any,
         index: str | None = None,
         render: bool = False,
+        chat_element: StreamlitChatElement | None = None,
         *args,
         **kwargs
     ) -> Any | None:
         """Append a new chat element to the session state.
 
         Args:
             role: The role of the message ('user' or 'assistant').
@@ -85,21 +86,23 @@
 
         Raises:
             ValueError: If an unsupported type is provided.
         """
         if index is None:
             index = uuid.uuid4().hex
 
-        chat_element = StreamlitChatElement(
-            role=role,
-            type=type,
-            content=content,
-            args=args,
-            kwargs=kwargs,
-        )
+
+        if not chat_element:
+            chat_element = StreamlitChatElement(
+                role=role,
+                type=type,
+                content=content,
+                args=args,
+                kwargs=kwargs,
+            )
 
         self.session_state[self.elements_label][index] = chat_element
 
         if render:
             return chat_element.render()
         return self
```

### Comparing `streamlit_chat_handler-0.0.5/streamlit_chat_handler/types.py` & `streamlit_chat_handler-0.0.6/streamlit_chat_handler/types.py`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.0.5/streamlit_chat_handler.egg-info/PKG-INFO` & `streamlit_chat_handler-0.0.6/streamlit_chat_handler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.0.5
+Version: 0.0.6
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```

