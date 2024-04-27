# Comparing `tmp/eastmoneypy-0.1.4.tar.gz` & `tmp/eastmoneypy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eastmoneypy-0.1.4.tar", last modified: Mon Apr  8 12:27:52 2024, max compression
+gzip compressed data, was "eastmoneypy-0.1.5.tar", last modified: Sat Apr 27 15:02:55 2024, max compression
```

## Comparing `eastmoneypy-0.1.4.tar` & `eastmoneypy-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:27:52.770866 eastmoneypy-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-08 12:27:39.000000 eastmoneypy-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-08 12:27:39.000000 eastmoneypy-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-08 12:27:52.770866 eastmoneypy-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-08 12:27:39.000000 eastmoneypy-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:27:52.766866 eastmoneypy-0.1.4/eastmoneypy/
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-08 12:27:39.000000 eastmoneypy-0.1.4/eastmoneypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-08 12:27:39.000000 eastmoneypy-0.1.4/eastmoneypy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 12:27:39.000000 eastmoneypy-0.1.4/eastmoneypy/config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:27:52.770866 eastmoneypy-0.1.4/eastmoneypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-08 12:27:52.000000 eastmoneypy-0.1.4/eastmoneypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-08 12:27:52.000000 eastmoneypy-0.1.4/eastmoneypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:27:52.000000 eastmoneypy-0.1.4/eastmoneypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 12:27:52.000000 eastmoneypy-0.1.4/eastmoneypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 12:27:52.000000 eastmoneypy-0.1.4/eastmoneypy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 12:27:52.770866 eastmoneypy-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-04-08 12:27:39.000000 eastmoneypy-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:27:52.770866 eastmoneypy-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-08 12:27:39.000000 eastmoneypy-0.1.4/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:02:55.818216 eastmoneypy-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-27 15:02:49.000000 eastmoneypy-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-27 15:02:49.000000 eastmoneypy-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-27 15:02:55.818216 eastmoneypy-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-27 15:02:49.000000 eastmoneypy-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:02:55.818216 eastmoneypy-0.1.5/eastmoneypy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-27 15:02:49.000000 eastmoneypy-0.1.5/eastmoneypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-04-27 15:02:49.000000 eastmoneypy-0.1.5/eastmoneypy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-27 15:02:49.000000 eastmoneypy-0.1.5/eastmoneypy/config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:02:55.818216 eastmoneypy-0.1.5/eastmoneypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-27 15:02:55.000000 eastmoneypy-0.1.5/eastmoneypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-27 15:02:55.000000 eastmoneypy-0.1.5/eastmoneypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 15:02:55.000000 eastmoneypy-0.1.5/eastmoneypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-27 15:02:55.000000 eastmoneypy-0.1.5/eastmoneypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 15:02:55.000000 eastmoneypy-0.1.5/eastmoneypy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 15:02:55.818216 eastmoneypy-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-04-27 15:02:49.000000 eastmoneypy-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 15:02:55.818216 eastmoneypy-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-27 15:02:49.000000 eastmoneypy-0.1.5/tests/test_api.py
```

### Comparing `eastmoneypy-0.1.4/LICENSE` & `eastmoneypy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eastmoneypy-0.1.4/PKG-INFO` & `eastmoneypy-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eastmoneypy
-Version: 0.1.4
+Version: 0.1.5
 Summary: python lib for operating eastmoney
 Home-page: https://github.com/zvtvz/eastmoneypy
 Author: foolcage
 Author-email: 5533061@qq.com
 Project-URL: Bug Reports, https://github.com/zvtvz/eastmoneypy/issues
 Project-URL: Funding, https://www.foolcage.com
 Project-URL: Say Thanks!, https://saythanks.io/to/foolcage
```

### Comparing `eastmoneypy-0.1.4/README.md` & `eastmoneypy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `eastmoneypy-0.1.4/eastmoneypy/__init__.py` & `eastmoneypy-0.1.5/eastmoneypy/__init__.py`

 * *Files identical despite different names*

### Comparing `eastmoneypy-0.1.4/eastmoneypy/api.py` & `eastmoneypy-0.1.5/eastmoneypy/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 import demjson3
 import requests
-from requests import Response
+from requests import Response, Session
 
 from eastmoneypy import my_env
 import time
 
 logger = logging.getLogger(__name__)
 
 
@@ -50,95 +50,119 @@
     logger.info(f"ret:{ret}")
     data = ret.get("data")
     if data and key:
         result_value = data.get(key)
     else:
         result_value = data
 
+    resp.close()
     return ret["state"], result_value
 
 
-def create_group(group_name):
+def create_group(group_name, session: Session = None):
     ts = current_timestamp()
     url = f"http://myfavor.eastmoney.com/v4/webouter/ag?appkey={APIKEY}&cb=jQuery112404771026622113468_{ts - 10}&gn={group_name}&_={ts}"
-    resp = requests.get(url, headers=HEADER)
+
+    if session:
+        resp = session.get(url, headers=HEADER)
+    else:
+        resp = requests.get(url, headers=HEADER)
 
     _, group = parse_resp(resp)
     return group
 
 
-def get_groups():
+def get_groups(session: Session = None):
     ts = current_timestamp()
     url = f"http://myfavor.eastmoney.com/v4/webouter/ggdefstkindexinfos?appkey={APIKEY}&cb=jQuery112407703233916827181_{ts - 10}&g=1&_={ts}"
 
-    resp = requests.get(url, headers=HEADER)
+    if session:
+        resp = session.get(url, headers=HEADER)
+    else:
+        resp = requests.get(url, headers=HEADER)
 
     _, value = parse_resp(resp, key="ginfolist")
     return value
 
 
-def rename_group(group_id, group_name):
+def rename_group(group_id, group_name, session: Session = None):
     ts = current_timestamp()
     url = f"http://myfavor.eastmoney.com/v4/webouter/mg?appkey={APIKEY}&cb=jQuery112406922055532444666_{ts - 10}&g={group_id}&gn={group_name}&_={ts}"
 
-    resp = requests.get(url, headers=HEADER)
+    if session:
+        resp = session.get(url, headers=HEADER)
+    else:
+        resp = requests.get(url, headers=HEADER)
 
     ret, _ = parse_resp(resp)
     return ret
 
 
-def del_group(group_name=None, group_id=None):
+def del_group(group_name=None, group_id=None, session: Session = None):
     if not group_id:
         assert group_name is not None
         group_id = get_group_id(group_name)
         if not group_id:
             raise Exception(f"could not find group:{group_name}")
 
     ts = current_timestamp()
     url = f"http://myfavor.eastmoney.com/v4/webouter/dg?appkey={APIKEY}&cb=jQuery1124005355240135242356_{ts - 10}&g={group_id}&_={ts}"
 
-    resp = requests.get(url, headers=HEADER)
+    if session:
+        resp = session.get(url, headers=HEADER)
+    else:
+        resp = requests.get(url, headers=HEADER)
 
     ret, _ = parse_resp(resp, key=None)
     return ret
 
 
 def get_group_id(group_name):
     groups = get_groups()
     groups = [group for group in groups if group["gname"] == group_name]
     if groups:
         return groups[0]["gid"]
     return None
 
 
-def list_entities(group_name=None, group_id=None):
+def list_entities(group_name=None, group_id=None, session: Session = None):
     if not group_id:
         assert group_name is not None
         group_id = get_group_id(group_name)
         if not group_id:
             raise Exception(f"could not find group:{group_name}")
     ts = current_timestamp()
     url = f"https://myfavor.eastmoney.com/v4/webouter/gstkinfos?appkey={APIKEY}&cb=jQuery112404771026622113468_{ts - 10}&g={group_id}&_={ts}"
-    resp = requests.get(url, headers=HEADER)
+
+    if session:
+        resp = session.get(url, headers=HEADER)
+    else:
+        resp = requests.get(url, headers=HEADER)
 
     _, result = parse_resp(resp)
     datas = result["stkinfolist"]
     return [data["security"].split("$")[1] for data in datas]
 
 
-def add_to_group(code, entity_type="stock", group_name=None, group_id=None):
+def add_to_group(
+    code, entity_type="stock", group_name=None, group_id=None, session: Session = None
+):
     if not group_id:
         assert group_name is not None
         group_id = get_group_id(group_name)
         if not group_id:
             raise Exception(f"could not find group:{group_name}")
     code = to_eastmoney_code(code, entity_type=entity_type)
     ts = current_timestamp()
     url = f"http://myfavor.eastmoney.com/v4/webouter/as?appkey={APIKEY}&cb=jQuery112404771026622113468_{ts - 10}&g={group_id}&sc={code}&_={ts}"
-    resp = requests.get(url, headers=HEADER)
+
+    if session:
+        resp = session.get(url, headers=HEADER)
+    else:
+        resp = requests.get(url, headers=HEADER)
 
     return parse_resp(resp)
 
 
 def to_eastmoney_code(code, entity_type="stock"):
     if entity_type == "stock":
         code_ = int(code)
@@ -170,8 +194,9 @@
 if __name__ == "__main__":
     # print(get_groups())
     # create_group("111")
     # print(add_to_group("MSFT", group_name="111", entity_type="stockus"))
     # del_group("111")
 
     # print(add_to_group("430047", group_name="111", entity_type="stock"))
-    print(list_entities(group_name="自选股"))
+    session = requests.Session()
+    print(list_entities(group_name="自选股", session=session))
```

### Comparing `eastmoneypy-0.1.4/eastmoneypy.egg-info/PKG-INFO` & `eastmoneypy-0.1.5/eastmoneypy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eastmoneypy
-Version: 0.1.4
+Version: 0.1.5
 Summary: python lib for operating eastmoney
 Home-page: https://github.com/zvtvz/eastmoneypy
 Author: foolcage
 Author-email: 5533061@qq.com
 Project-URL: Bug Reports, https://github.com/zvtvz/eastmoneypy/issues
 Project-URL: Funding, https://www.foolcage.com
 Project-URL: Say Thanks!, https://saythanks.io/to/foolcage
```

### Comparing `eastmoneypy-0.1.4/setup.py` & `eastmoneypy-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.1.4',  # Required
+    version='0.1.5',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='python lib for operating eastmoney',  # Required
 
     # This is an optional longer description of your project that represents
```

