# Comparing `tmp/streamlit-shortcuts-0.1.1.tar.gz` & `tmp/streamlit-shortcuts-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-shortcuts-0.1.1.tar", last modified: Tue Nov 28 22:00:35 2023, max compression
+gzip compressed data, was "streamlit-shortcuts-0.1.2.tar", last modified: Sat Apr 27 21:22:17 2024, max compression
```

## Comparing `streamlit-shortcuts-0.1.1.tar` & `streamlit-shortcuts-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrian     (501) staff       (20)        0 2023-11-28 22:00:35.396640 streamlit-shortcuts-0.1.1/
--rw-r--r--   0 adrian     (501) staff       (20)     1063 2023-11-28 21:52:39.000000 streamlit-shortcuts-0.1.1/LICENSE
--rw-r--r--   0 adrian     (501) staff       (20)     1411 2023-11-28 22:00:35.396440 streamlit-shortcuts-0.1.1/PKG-INFO
--rw-r--r--   0 adrian     (501) staff       (20)     1058 2023-11-28 21:46:42.000000 streamlit-shortcuts-0.1.1/README.md
--rw-r--r--   0 adrian     (501) staff       (20)       38 2023-11-28 22:00:35.396686 streamlit-shortcuts-0.1.1/setup.cfg
--rw-r--r--   0 adrian     (501) staff       (20)      556 2023-11-28 22:00:17.000000 streamlit-shortcuts-0.1.1/setup.py
-drwxr-xr-x   0 adrian     (501) staff       (20)        0 2023-11-28 22:00:35.394944 streamlit-shortcuts-0.1.1/src/
-drwxr-xr-x   0 adrian     (501) staff       (20)        0 2023-11-28 22:00:35.395525 streamlit-shortcuts-0.1.1/src/streamlit_shortcuts/
--rw-r--r--   0 adrian     (501) staff       (20)       56 2023-11-28 21:59:10.000000 streamlit-shortcuts-0.1.1/src/streamlit_shortcuts/__init__.py
--rw-r--r--   0 adrian     (501) staff       (20)     1518 2023-11-28 21:40:34.000000 streamlit-shortcuts-0.1.1/src/streamlit_shortcuts/streamlit_shortcuts.py
-drwxr-xr-x   0 adrian     (501) staff       (20)        0 2023-11-28 22:00:35.396226 streamlit-shortcuts-0.1.1/src/streamlit_shortcuts.egg-info/
--rw-r--r--   0 adrian     (501) staff       (20)     1411 2023-11-28 22:00:35.000000 streamlit-shortcuts-0.1.1/src/streamlit_shortcuts.egg-info/PKG-INFO
--rw-r--r--   0 adrian     (501) staff       (20)      343 2023-11-28 22:00:35.000000 streamlit-shortcuts-0.1.1/src/streamlit_shortcuts.egg-info/SOURCES.txt
--rw-r--r--   0 adrian     (501) staff       (20)        1 2023-11-28 22:00:35.000000 streamlit-shortcuts-0.1.1/src/streamlit_shortcuts.egg-info/dependency_links.txt
--rw-r--r--   0 adrian     (501) staff       (20)       10 2023-11-28 22:00:35.000000 streamlit-shortcuts-0.1.1/src/streamlit_shortcuts.egg-info/requires.txt
--rw-r--r--   0 adrian     (501) staff       (20)       20 2023-11-28 22:00:35.000000 streamlit-shortcuts-0.1.1/src/streamlit_shortcuts.egg-info/top_level.txt
+drwxr-xr-x   0 adrian     (501) staff       (20)        0 2024-04-27 21:22:17.501723 streamlit-shortcuts-0.1.2/
+-rw-r--r--   0 adrian     (501) staff       (20)     1063 2023-11-28 21:52:39.000000 streamlit-shortcuts-0.1.2/LICENSE
+-rw-r--r--   0 adrian     (501) staff       (20)     2014 2024-04-27 21:22:17.501504 streamlit-shortcuts-0.1.2/PKG-INFO
+-rw-r--r--   0 adrian     (501) staff       (20)     1661 2024-04-27 21:20:50.000000 streamlit-shortcuts-0.1.2/README.md
+-rw-r--r--   0 adrian     (501) staff       (20)       38 2024-04-27 21:22:17.501763 streamlit-shortcuts-0.1.2/setup.cfg
+-rw-r--r--   0 adrian     (501) staff       (20)      556 2024-04-27 21:22:13.000000 streamlit-shortcuts-0.1.2/setup.py
+drwxr-xr-x   0 adrian     (501) staff       (20)        0 2024-04-27 21:22:17.499984 streamlit-shortcuts-0.1.2/src/
+drwxr-xr-x   0 adrian     (501) staff       (20)        0 2024-04-27 21:22:17.500599 streamlit-shortcuts-0.1.2/src/streamlit_shortcuts/
+-rw-r--r--   0 adrian     (501) staff       (20)       65 2024-04-27 21:06:01.000000 streamlit-shortcuts-0.1.2/src/streamlit_shortcuts/__init__.py
+-rw-r--r--   0 adrian     (501) staff       (20)     1932 2024-04-27 21:10:49.000000 streamlit-shortcuts-0.1.2/src/streamlit_shortcuts/streamlit_shortcuts.py
+drwxr-xr-x   0 adrian     (501) staff       (20)        0 2024-04-27 21:22:17.501320 streamlit-shortcuts-0.1.2/src/streamlit_shortcuts.egg-info/
+-rw-r--r--   0 adrian     (501) staff       (20)     2014 2024-04-27 21:22:17.000000 streamlit-shortcuts-0.1.2/src/streamlit_shortcuts.egg-info/PKG-INFO
+-rw-r--r--   0 adrian     (501) staff       (20)      343 2024-04-27 21:22:17.000000 streamlit-shortcuts-0.1.2/src/streamlit_shortcuts.egg-info/SOURCES.txt
+-rw-r--r--   0 adrian     (501) staff       (20)        1 2024-04-27 21:22:17.000000 streamlit-shortcuts-0.1.2/src/streamlit_shortcuts.egg-info/dependency_links.txt
+-rw-r--r--   0 adrian     (501) staff       (20)       10 2024-04-27 21:22:17.000000 streamlit-shortcuts-0.1.2/src/streamlit_shortcuts.egg-info/requires.txt
+-rw-r--r--   0 adrian     (501) staff       (20)       20 2024-04-27 21:22:17.000000 streamlit-shortcuts-0.1.2/src/streamlit_shortcuts.egg-info/top_level.txt
```

### Comparing `streamlit-shortcuts-0.1.1/LICENSE` & `streamlit-shortcuts-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-shortcuts-0.1.1/PKG-INFO` & `streamlit-shortcuts-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,50 @@
-Metadata-Version: 2.1
-Name: streamlit-shortcuts
-Version: 0.1.1
-Summary: Streamlit keyboard shortcuts for your buttons.
-Home-page: https://github.com/adriangalilea/streamlit-shortcuts
-Author: Adrian Galilea Delgado
-Author-email: adriangalilea@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: streamlit
-
 
 # Streamlit Shortcuts
 
 Streamlit Shortcuts allows you to easily add keyboard shortcuts to your Streamlit buttons.
 
 ## Installation
 
 ```bash
 pip install streamlit-shortcuts
 ```
 
 ## Example
 
+⭐ NEW! thanks to @quantum-ernest 
+```
+import streamlit as st
+from streamlit_shortcuts import button
+
+def delete_callback():
+    st.write("DELETED!")
+
+streamlit_shortcuts.button("delete", on_click=delete_callback, shortcut,="Ctrl+Shift+X")
+```
+
+🥱 Old 
 ```python
 import streamlit as st
 from streamlit_shortcuts import add_keyboard_shortcuts
 
 def delete_callback():
     st.write("DELETED!")
 
 st.button("delete", on_click=delete_callback)
 
 add_keyboard_shortcuts({
     'Ctrl+Shift+X': 'delete',
-    # Add more key-button mappings here
 })
 ```
 
 The 'Ctrl+Shift+X' combination will trigger "Another Button".
 
 ## Keys
-- Modifiers: 'Control', 'Shift', 'Alt'
+- Modifiers: 'Control', 'Shift', 'Alt', 'Meta' ('Cmd' on Mac or 'Win' on Windows, thanks to @toolittlecakes)  
 - Common Keys: 'Enter', 'Escape', 'Space'
 - Arrow Keys: 'ArrowLeft', 'ArrowRight', 'ArrowUp', 'ArrowDown'
 
 Examples of Key Combinations:
 - 'Control+Enter'
 - 'Shift+ArrowUp'
 - 'Alt+Space'
@@ -53,7 +52,23 @@
 For a complete list of key values, refer to:
 https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/key/Key_Values
 
 
 ## Contributing
 
 Contributions are welcome! If you have suggestions for improvements or bug fixes, please feel free to make a pull request or open an issue.
+
+## Contributors
+@toolittlecakes - Added 'Meta' modifier
+@quantum-ernest - Improved usage ergonomics
+
+## Credits
+Solution seen on:
+https://github.com/streamlit/streamlit/issues/1291
+
+https://gist.github.com/brunomsantiago/e0ab366fc0dbc092c1a5946b30caa9a0
+
+@brunomsantiago
+
+@TomJohnH
+
+And wrapped for comfier usage.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `streamlit-shortcuts-0.1.1/setup.py` & `streamlit-shortcuts-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='streamlit-shortcuts',
-    version='0.1.1',
+    version='0.1.2',
     author='Adrian Galilea Delgado',
     author_email='adriangalilea@gmail.com',
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     url='https://github.com/adriangalilea/streamlit-shortcuts',
     license='MIT',
     description='Streamlit keyboard shortcuts for your buttons.',
```

### Comparing `streamlit-shortcuts-0.1.1/src/streamlit_shortcuts/streamlit_shortcuts.py` & `streamlit-shortcuts-0.1.2/src/streamlit_shortcuts/streamlit_shortcuts.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,16 @@
+from typing import Callable
+
 import streamlit.components.v1 as components
+import streamlit as st
+
 
+# TODO bump to v0.1.2 for 'Meta modifier' and 'Usage ergonomics'
+# TODO add keyboard tooltip to button (streamlit-extras)
+# https://arnaudmiribel.github.io/streamlit-extras/extras/keyboard_text/
 
 def add_keyboard_shortcuts(key_combinations: dict[str, str]):
     """
     Add keyboard shortcuts to trigger Streamlit buttons.
 
     Keys:
     - Modifiers: 'Control', 'Shift', 'Alt'
@@ -45,7 +52,12 @@
 
     js_code += """
     });
     </script>
     """
 
     components.html(js_code, height=0, width=0)
+
+
+def button(label: str, shortcut: dict[str, str], on_click: Callable[..., None]):
+    st.button(label=label, on_click=on_click)
+    add_keyboard_shortcuts(shortcut)
```

### Comparing `streamlit-shortcuts-0.1.1/src/streamlit_shortcuts.egg-info/PKG-INFO` & `streamlit-shortcuts-0.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-shortcuts
-Version: 0.1.1
+Version: 0.1.2
 Summary: Streamlit keyboard shortcuts for your buttons.
 Home-page: https://github.com/adriangalilea/streamlit-shortcuts
 Author: Adrian Galilea Delgado
 Author-email: adriangalilea@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -19,33 +19,44 @@
 
 ```bash
 pip install streamlit-shortcuts
 ```
 
 ## Example
 
+⭐ NEW! thanks to @quantum-ernest 
+```
+import streamlit as st
+from streamlit_shortcuts import button
+
+def delete_callback():
+    st.write("DELETED!")
+
+streamlit_shortcuts.button("delete", on_click=delete_callback, shortcut,="Ctrl+Shift+X")
+```
+
+🥱 Old 
 ```python
 import streamlit as st
 from streamlit_shortcuts import add_keyboard_shortcuts
 
 def delete_callback():
     st.write("DELETED!")
 
 st.button("delete", on_click=delete_callback)
 
 add_keyboard_shortcuts({
     'Ctrl+Shift+X': 'delete',
-    # Add more key-button mappings here
 })
 ```
 
 The 'Ctrl+Shift+X' combination will trigger "Another Button".
 
 ## Keys
-- Modifiers: 'Control', 'Shift', 'Alt'
+- Modifiers: 'Control', 'Shift', 'Alt', 'Meta' ('Cmd' on Mac or 'Win' on Windows, thanks to @toolittlecakes)  
 - Common Keys: 'Enter', 'Escape', 'Space'
 - Arrow Keys: 'ArrowLeft', 'ArrowRight', 'ArrowUp', 'ArrowDown'
 
 Examples of Key Combinations:
 - 'Control+Enter'
 - 'Shift+ArrowUp'
 - 'Alt+Space'
@@ -53,7 +64,23 @@
 For a complete list of key values, refer to:
 https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/key/Key_Values
 
 
 ## Contributing
 
 Contributions are welcome! If you have suggestions for improvements or bug fixes, please feel free to make a pull request or open an issue.
+
+## Contributors
+@toolittlecakes - Added 'Meta' modifier
+@quantum-ernest - Improved usage ergonomics
+
+## Credits
+Solution seen on:
+https://github.com/streamlit/streamlit/issues/1291
+
+https://gist.github.com/brunomsantiago/e0ab366fc0dbc092c1a5946b30caa9a0
+
+@brunomsantiago
+
+@TomJohnH
+
+And wrapped for comfier usage.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

