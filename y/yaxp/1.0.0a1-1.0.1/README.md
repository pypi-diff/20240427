# Comparing `tmp/yaxp-1.0.0a1.tar.gz` & `tmp/yaxp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaxp-1.0.0a1.tar", last modified: Tue Oct 24 11:50:20 2023, max compression
+gzip compressed data, was "yaxp-1.0.1.tar", last modified: Sat Apr 27 12:40:49 2024, max compression
```

## Comparing `yaxp-1.0.0a1.tar` & `yaxp-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:50:20.139487 yaxp-1.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2023-10-24 11:50:20.139487 yaxp-1.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2023-10-24 11:50:12.000000 yaxp-1.0.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-10-24 11:50:12.000000 yaxp-1.0.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      521 2023-10-24 11:50:20.143487 yaxp-1.0.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:50:20.139487 yaxp-1.0.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:50:20.139487 yaxp-1.0.0a1/src/yaxp/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-10-24 11:50:12.000000 yaxp-1.0.0a1/src/yaxp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2023-10-24 11:50:12.000000 yaxp-1.0.0a1/src/yaxp/_xpath.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:50:20.139487 yaxp-1.0.0a1/src/yaxp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2023-10-24 11:50:20.000000 yaxp-1.0.0a1/src/yaxp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-10-24 11:50:20.000000 yaxp-1.0.0a1/src/yaxp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-24 11:50:20.000000 yaxp-1.0.0a1/src/yaxp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-24 11:50:20.000000 yaxp-1.0.0a1/src/yaxp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 11:50:20.139487 yaxp-1.0.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2023-10-24 11:50:12.000000 yaxp-1.0.0a1/tests/test_xpath.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:40:49.935485 yaxp-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-27 12:40:49.935485 yaxp-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-27 12:40:44.000000 yaxp-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-27 12:40:44.000000 yaxp-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-27 12:40:49.939485 yaxp-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:40:49.935485 yaxp-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:40:49.935485 yaxp-1.0.1/src/yaxp/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-27 12:40:44.000000 yaxp-1.0.1/src/yaxp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-27 12:40:44.000000 yaxp-1.0.1/src/yaxp/_xpath.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:40:49.935485 yaxp-1.0.1/src/yaxp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-27 12:40:49.000000 yaxp-1.0.1/src/yaxp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-27 12:40:49.000000 yaxp-1.0.1/src/yaxp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 12:40:49.000000 yaxp-1.0.1/src/yaxp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-27 12:40:49.000000 yaxp-1.0.1/src/yaxp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:40:49.935485 yaxp-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-27 12:40:44.000000 yaxp-1.0.1/tests/test_xpath.py
```

### Comparing `yaxp-1.0.0a1/PKG-INFO` & `yaxp-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaxp
-Version: 1.0.0a1
+Version: 1.0.1
 Summary: intuitive xpath generator
 Project-URL: Homepage, https://github.com/realtimeprojects/yaxp
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/yaxp/issues
 Keywords: xpath,selenium,xml
 Description-Content-Type: text/markdown
 
 # yet another xpath generator
```

### Comparing `yaxp-1.0.0a1/README.md` & `yaxp-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `yaxp-1.0.0a1/setup.cfg` & `yaxp-1.0.1/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = yaxp
-version = 1.0.0a1
+version = 1.0.1
 description = intuitive xpath generator
 keywords = xpath, selenium, xml
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
 	Homepage = https://github.com/realtimeprojects/yaxp
 	Bug Tracker = https://github.com/realtimeprojects/yaxp/issues
```

### Comparing `yaxp-1.0.0a1/src/yaxp/_xpath.py` & `yaxp-1.0.1/src/yaxp/_xpath.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,21 +72,24 @@
                 arg = f"@{arg}"
             if not values:
                 continue
             if not isinstance(values, list):
                 values = [values]
             for value in values:
                 if wildcard:
-                    filter += f'[contains({arg}, "{value}")]'
+                    filter += f'[contains({arg}, {_quote(value)})]'
                 elif value[0] == "*":
-                    filter += f'[{arg}[contains(., "{value[1:]}")]]'
+                    if arg == ".":
+                        filter += f'[contains(., {_quote(value[1:])})]'
+                    else:
+                        filter += f'[{arg}[contains(., {_quote(value[1:])})]]'
                 elif value[0] == "#":
-                    filter += f'[contains(concat(" ", normalize-space({arg}), " "), " {value[1:]} ")]'
+                    filter += f'[contains(concat(" ", normalize-space({arg}), " "), {_quote(" " + value[1:] + " ")})]'
                 else:
-                    filter += f'[{arg}="{value}"]'
+                    filter += f'[{arg}={_quote(value)}]'
         self._filter.append(filter)
 
     @staticmethod
     def _by_xpath(xpath):
         return XPG(role=xpath)
 
     @property
@@ -129,7 +132,15 @@
     def __getattr__(self, name):
         if name[0] == "_":
             name = name[1:]
         name = name.replace("_", ".")
         name = name.replace("..", "_")
 
         return XPG(name, parent=self)
+
+
+def _quote(value):
+    if '"' in value and "'" in value:
+        raise Exception("values containing `'` and `\"` are not supported")
+    if '"' in value:
+        return f"'{value}'"
+    return f'"{value}"'
```

### Comparing `yaxp-1.0.0a1/src/yaxp.egg-info/PKG-INFO` & `yaxp-1.0.1/src/yaxp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaxp
-Version: 1.0.0a1
+Version: 1.0.1
 Summary: intuitive xpath generator
 Project-URL: Homepage, https://github.com/realtimeprojects/yaxp
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/yaxp/issues
 Keywords: xpath,selenium,xml
 Description-Content-Type: text/markdown
 
 # yet another xpath generator
```

### Comparing `yaxp-1.0.0a1/tests/test_xpath.py` & `yaxp-1.0.1/tests/test_xpath.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,37 +13,38 @@
     # direct parent
     (xp.h2.by(_id="huhu", direct=True),        '/h2[@id="huhu"]'),
 
     # No role
     (xp.by(_id="huhu"),        '//*[@id="huhu"]'),
 
     # partial-match specification
-    (xp.span(_id="*huhu"),  '//span[contains(@id, "huhu")]'),
-    (xp.span.contains(_id="huhu"),  '//span[contains(@id, "huhu")]'),
+    (xp.span(_id="*huhu"),  '//span[@id[contains(., "huhu")]]'),
+    (xp.span.contains(_id="huhu"),  '//span[@id[contains(., "huhu")]]'),
 
     # text match exactly
     (xp.span(text="Hello"),  '//span[text()="Hello"]'),
 
     # text match exactly
-    (xp.span(text="*Hello3"),  '//span[contains(text(), "Hello3")]'),
+    (xp.span(text="*Hello3"),  '//span[text()[contains(., "Hello3")]]'),
 
     # text attribute match
     (xp.span(_text="Hello2"),  '//span[@text="Hello2"]'),
 
     # text attribute match
-    (xp.span(_text="*Hello4"),  '//span[contains(@text, "Hello4")]'),
+    (xp.span(_text="*Hello4"),  '//span[@text[contains(., "Hello4")]]'),
 
     # text match partial
     (xp.span(_="*World"),  '//span[contains(., "World")]'),
 
     # text match partial
     (xp.span(_="World"),  '//span[.="World"]'),
 
     # text match partial
-    (xp.span(_id="myid").contains(_="Hello", _class="myclass"),  '//span[@id="myid"][contains(., "Hello")][contains(@class, "myclass")]'),
+    (xp.span(_id="myid").contains(_="Hello", _class="myclass"),
+        '//span[@id="myid"][contains(., "Hello")][@class[contains(., "myclass")]]'),
 
     # word-match specification
     (xp.div(_class="#part"),   '//div[contains(concat(" ", normalize-space(@class), " "), " part ")]'),
 
     # convert _ to -
     (xp.span(test_id="huhu"), '//span[@test-id="huhu"]'),
 
@@ -83,13 +84,17 @@
     (xp.div.h1(_class="myclass"), '//div//h1[@class="myclass"]'),
 
     # roles containing "."
     (xp.Android_Container(_id="huhu"), '//Android.Container[@id="huhu"]'),
 
     # tags containing "_"
     (xp.Android__Container(_id="huhu"), '//Android_Container[@id="huhu"]'),
+
+    # values containing \"
+    (xp.span(test_id='hu"hu'), "//span[@test-id='hu\"hu']"),
+    (xp.span(_='*Wo"rld'),  "//span[contains(., 'Wo\"rld')]"),
 ]
 
 
 @pytest.mark.parametrize("xp,xpath", testdata)
 def test_xpath(xp, xpath):
     assert str(xp) == xpath
```

