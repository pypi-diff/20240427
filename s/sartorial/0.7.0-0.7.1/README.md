# Comparing `tmp/sartorial-0.7.0.tar.gz` & `tmp/sartorial-0.7.1.tar.gz`

## Comparing `sartorial-0.7.0.tar` & `sartorial-0.7.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 sartorial-0.7.0/sartorial/__init__.py
--rw-r--r--   0        0        0    10483 2020-02-02 00:00:00.000000 sartorial-0.7.0/sartorial/schema.py
--rw-r--r--   0        0        0     4802 2020-02-02 00:00:00.000000 sartorial-0.7.0/sartorial/serialization.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 sartorial-0.7.0/sartorial/types.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sartorial-0.7.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 sartorial-0.7.0/LICENSE
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 sartorial-0.7.0/README.md
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 sartorial-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 sartorial-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 sartorial-0.7.1/sartorial/__init__.py
+-rw-r--r--   0        0        0    10483 2020-02-02 00:00:00.000000 sartorial-0.7.1/sartorial/schema.py
+-rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 sartorial-0.7.1/sartorial/serialization.py
+-rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 sartorial-0.7.1/sartorial/types.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sartorial-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 sartorial-0.7.1/LICENSE
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 sartorial-0.7.1/README.md
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 sartorial-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 sartorial-0.7.1/PKG-INFO
```

### Comparing `sartorial-0.7.0/sartorial/schema.py` & `sartorial-0.7.1/sartorial/schema.py`

 * *Files identical despite different names*

### Comparing `sartorial-0.7.0/sartorial/serialization.py` & `sartorial-0.7.1/sartorial/serialization.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,14 +98,23 @@
         return datetime.time(0)
     elif isinstance(t, datetime.time):
         return t
     else:
         return date_parse(t).time()
 
 
+def any_to_decimal(d):
+    if isinstance(d, Decimal):
+        return d
+    elif isinstance(d, str):
+        return Decimal(d)
+    else:
+        return Decimal(str(d))
+
+
 def any_to_uuid(u):
     if isinstance(u, UUID):
         return u
     else:
         return UUID(u)
 
 
@@ -117,15 +126,15 @@
 
 
 DECODERS_BY_TYPE: Dict[Type[Any], Callable[[Any], Any]] = {
     datetime.date: any_to_date,
     datetime.datetime: any_to_datetime,
     datetime.time: any_to_time,
     datetime.timedelta: timedelta_parse,
-    Decimal: Decimal,
+    Decimal: any_to_decimal,
     IPv4Address: IPv4Address,
     IPv4Interface: IPv4Interface,
     IPv4Network: IPv4Network,
     IPv6Address: IPv6Address,
     IPv6Interface: IPv6Interface,
     IPv6Network: IPv6Network,
     UUID: any_to_uuid,
```

### Comparing `sartorial-0.7.0/sartorial/types.py` & `sartorial-0.7.1/sartorial/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         if "python_type" not in cls.__dict__:
             cls.python_type = cls
         if not cls.schema_format:
             raise ValueError("schema_format is required")
         if "schema_format" not in cls.__dict__ and (
-            not hasattr(".__pydantic_generic_metadata__")
+            not hasattr(cls, ".__pydantic_generic_metadata__")
             or not cls.__pydantic_generic_metadata__.get("origin")
         ):
             raise ValueError("schema_format is required for generic base classes")
         cls.register(cls.python_type, cls.schema_type, cls.schema_format)
 
     @classmethod
     def get_type(
```

### Comparing `sartorial-0.7.0/.gitignore` & `sartorial-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sartorial-0.7.0/LICENSE` & `sartorial-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sartorial-0.7.0/pyproject.toml` & `sartorial-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [bumpver]
-current_version = "0.7.0"
+current_version = "0.7.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version: {old_version} → {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = false
```

### Comparing `sartorial-0.7.0/PKG-INFO` & `sartorial-0.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sartorial
-Version: 0.7.0
+Version: 0.7.1
 Summary: Pydantic model base classes and custom type handling, JSON schema generation, etc. covering a variety of common scenarios without much config
 Project-URL: Homepage, https://github.com/goodcleanfun/sartorial
 Project-URL: Repository, https://github.com/goodcleanfun/sartorial
 Author: Al Barrentine
 License-Expression: MIT
 License-File: LICENSE
 Keywords: json-schema,model,pydantic,sartorial,schema
```

