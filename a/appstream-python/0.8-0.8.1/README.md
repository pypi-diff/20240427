# Comparing `tmp/appstream-python-0.8.tar.gz` & `tmp/appstream_python-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appstream-python-0.8.tar", last modified: Sat Mar 30 16:30:23 2024, max compression
+gzip compressed data, was "appstream_python-0.8.1.tar", last modified: Sat Apr 27 20:23:56 2024, max compression
```

## Comparing `appstream-python-0.8.tar` & `appstream_python-0.8.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 16:30:23.468993 appstream-python-0.8/
--rw-r--r--   0 root         (0) root         (0)     1318 2024-03-30 16:29:58.000000 appstream-python-0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       71 2024-03-30 16:29:58.000000 appstream-python-0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1328 2024-03-30 16:30:23.468993 appstream-python-0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      112 2024-03-30 16:29:58.000000 appstream-python-0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 16:30:23.468993 appstream-python-0.8/appstream_python/
--rw-r--r--   0 root         (0) root         (0)     2777 2024-03-30 16:29:58.000000 appstream-python-0.8/appstream_python/Collection.py
--rw-r--r--   0 root         (0) root         (0)    24219 2024-03-30 16:29:58.000000 appstream-python-0.8/appstream_python/Component.py
--rw-r--r--   0 root         (0) root         (0)     5409 2024-03-30 16:29:58.000000 appstream-python-0.8/appstream_python/Release.py
--rw-r--r--   0 root         (0) root         (0)    13959 2024-03-30 16:29:58.000000 appstream-python-0.8/appstream_python/Shared.py
--rw-r--r--   0 root         (0) root         (0)     2376 2024-03-30 16:29:58.000000 appstream-python-0.8/appstream_python/StandardConstants.py
--rw-r--r--   0 root         (0) root         (0)      212 2024-03-30 16:29:58.000000 appstream-python-0.8/appstream_python/__init__.py
--rw-r--r--   0 root         (0) root         (0)      326 2024-03-30 16:29:58.000000 appstream-python-0.8/appstream_python/_helper.py
--rw-r--r--   0 root         (0) root         (0)        4 2024-03-30 16:29:58.000000 appstream-python-0.8/appstream_python/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 16:30:23.468993 appstream-python-0.8/appstream_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1328 2024-03-30 16:30:23.000000 appstream-python-0.8/appstream_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      590 2024-03-30 16:30:23.000000 appstream-python-0.8/appstream_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-30 16:30:23.000000 appstream-python-0.8/appstream_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-03-30 16:30:23.000000 appstream-python-0.8/appstream_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-30 16:30:23.000000 appstream-python-0.8/appstream_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1520 2024-03-30 16:29:58.000000 appstream-python-0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-30 16:30:23.468993 appstream-python-0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 16:30:23.468993 appstream-python-0.8/tests/
--rw-r--r--   0 root         (0) root         (0)     3014 2024-03-30 16:29:58.000000 appstream-python-0.8/tests/test_appstream_data.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-03-30 16:29:58.000000 appstream-python-0.8/tests/test_description.py
--rw-r--r--   0 root         (0) root         (0)     2982 2024-03-30 16:29:58.000000 appstream-python-0.8/tests/test_display_length.py
--rw-r--r--   0 root         (0) root         (0)     3799 2024-03-30 16:29:58.000000 appstream-python-0.8/tests/test_releases.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:23:56.014913 appstream_python-0.8.1/
+-rw-r--r--   0 root         (0) root         (0)     1318 2024-04-27 20:22:19.000000 appstream_python-0.8.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       71 2024-04-27 20:22:19.000000 appstream_python-0.8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1330 2024-04-27 20:23:56.014913 appstream_python-0.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      112 2024-04-27 20:22:19.000000 appstream_python-0.8.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:23:56.010913 appstream_python-0.8.1/appstream_python/
+-rw-r--r--   0 root         (0) root         (0)     3472 2024-04-27 20:22:19.000000 appstream_python-0.8.1/appstream_python/Collection.py
+-rw-r--r--   0 root         (0) root         (0)    24302 2024-04-27 20:22:19.000000 appstream_python-0.8.1/appstream_python/Component.py
+-rw-r--r--   0 root         (0) root         (0)     5409 2024-04-27 20:22:19.000000 appstream_python-0.8.1/appstream_python/Release.py
+-rw-r--r--   0 root         (0) root         (0)    13959 2024-04-27 20:22:19.000000 appstream_python-0.8.1/appstream_python/Shared.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2024-04-27 20:22:19.000000 appstream_python-0.8.1/appstream_python/StandardConstants.py
+-rw-r--r--   0 root         (0) root         (0)      212 2024-04-27 20:22:19.000000 appstream_python-0.8.1/appstream_python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      326 2024-04-27 20:22:19.000000 appstream_python-0.8.1/appstream_python/_helper.py
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-27 20:22:19.000000 appstream_python-0.8.1/appstream_python/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:23:56.014913 appstream_python-0.8.1/appstream_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1330 2024-04-27 20:23:56.000000 appstream_python-0.8.1/appstream_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      615 2024-04-27 20:23:56.000000 appstream_python-0.8.1/appstream_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 20:23:56.000000 appstream_python-0.8.1/appstream_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-27 20:23:56.000000 appstream_python-0.8.1/appstream_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-27 20:23:56.000000 appstream_python-0.8.1/appstream_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1520 2024-04-27 20:22:19.000000 appstream_python-0.8.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 20:23:56.014913 appstream_python-0.8.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 20:23:56.014913 appstream_python-0.8.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     3072 2024-04-27 20:22:19.000000 appstream_python-0.8.1/tests/test_appstream_data.py
+-rw-r--r--   0 root         (0) root         (0)     3594 2024-04-27 20:22:19.000000 appstream_python-0.8.1/tests/test_collection.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-04-27 20:22:19.000000 appstream_python-0.8.1/tests/test_description.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2024-04-27 20:22:19.000000 appstream_python-0.8.1/tests/test_display_length.py
+-rw-r--r--   0 root         (0) root         (0)     3799 2024-04-27 20:22:19.000000 appstream_python-0.8.1/tests/test_releases.py
```

### Comparing `appstream-python-0.8/LICENSE` & `appstream_python-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `appstream-python-0.8/PKG-INFO` & `appstream_python-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appstream-python
-Version: 0.8
+Version: 0.8.1
 Summary: A library for dealing with Freedesktop Appstream data
 Author-email: JakobDev <jakobdev@gmx.de>
 License: BSD-2-Clause
 Project-URL: Documentation, https://appstream-python.readthedocs.io
 Project-URL: Issues, https://codeberg.org/JakobDev/appstream-python/issues
 Project-URL: Source, https://codeberg.org/JakobDev/appstream-python
 Project-URL: Donation, https://ko-fi.com/jakobdev
```

### Comparing `appstream-python-0.8/appstream_python/Collection.py` & `appstream_python-0.8.1/appstream_python/Collection.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,21 +8,32 @@
     def __init__(self) -> None:
         self._components: dict[str, AppstreamComponent] = {}
         self._categories: dict[str, list[str]] = {}
 
     def _add_appstream_tag(self, tag: etree.Element) -> None:
         component_data = AppstreamComponent()
         component_data.parse_component_tag(tag)
+        self.add_component(component_data)
 
-        self._components[component_data.id] = component_data
+    def add_component(self, component: AppstreamComponent) -> None:
+        "Adds a AppstreamComponent to the collection"
+        self._components[component.id] = component
 
-        for i in component_data.categories:
+        for i in component.categories:
             if i not in self._categories:
                 self._categories[i] = []
-            self._categories[i].append(component_data.id)
+            self._categories[i].append(component.id)
+
+    def load_uncompressed_appstream_collection(self, path: str) -> None:
+        "Loads a uncompressed collection"
+        with open(path, "rb") as f:
+            root = etree.fromstring(f.read())
+
+        for i in root.findall("component"):
+            self._add_appstream_tag(i)
 
     def load_compressed_appstream_collection(self, path: str) -> None:
         "Loads a GZIP compressed collection"
         with gzip.open(path, "rb") as f:
             root = etree.fromstring(f.read())
 
         for i in root.findall("component"):
@@ -68,9 +79,14 @@
         return components_tag
 
     def write_uncompressed_file(self, path: str) -> None:
         "Writes a Uncompressed collection file"
         with open(path, "w", encoding="utf-8") as f:
             f.write(etree.tostring(self.get_collection_tag(), pretty_print=True, xml_declaration=True, encoding="utf-8").decode("utf-8"))
 
+    def write_compressed_file(self, path: str) -> None:
+        "Writes a Uncompressed collection file"
+        with gzip.open(path, "wb") as f:
+            f.write(etree.tostring(self.get_collection_tag(), pretty_print=True, xml_declaration=True, encoding="utf-8"))
+
     def __len__(self) -> int:
         return len(self._components)
```

### Comparing `appstream-python-0.8/appstream_python/Component.py` & `appstream_python-0.8.1/appstream_python/Component.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,15 +353,15 @@
             self.provides[i] = []
 
         for i in CONTROL_TYPES:
             self.controls[i] = None
 
     def get_available_languages(self) -> list[str]:
         "Returns a list with all available languages of the Component"
-        lang_list = self.name.get_available_languages() + self.summary.get_available_languages() + self.developer_name.get_available_languages()
+        lang_list = self.name.get_available_languages() + self.summary.get_available_languages() + self.developer.name.get_available_languages()
         return list(set(lang_list))
 
     def _parse_relation_tag(self, tag: etree.Element) -> None:
         "Parses a relation tag"
         relation = tag.tag
 
         for control_tag in tag.findall("control"):
@@ -405,19 +405,19 @@
         self.summary.load_tags(tag.findall("summary"))
 
         description_tag = tag.find("description")
         if description_tag is not None:
             self.description.load_tags(description_tag)
 
         metadata_license_tag = tag.find("metadata_license")
-        if metadata_license_tag is not None:
+        if metadata_license_tag is not None and metadata_license_tag.text is not None:
             self.metadata_license = metadata_license_tag.text.strip()
 
         project_license_tag = tag.find("project_license")
-        if project_license_tag is not None:
+        if project_license_tag is not None and project_license_tag.text is not None:
             self.project_license = project_license_tag.text.strip()
 
         categories_tag = tag.find("categories")
         if categories_tag is not None:
             for i in categories_tag.findall("category"):
                 self.categories.append(i.text.strip())
```

### Comparing `appstream-python-0.8/appstream_python/Release.py` & `appstream_python-0.8.1/appstream_python/Release.py`

 * *Files identical despite different names*

### Comparing `appstream-python-0.8/appstream_python/Shared.py` & `appstream_python-0.8.1/appstream_python/Shared.py`

 * *Files identical despite different names*

### Comparing `appstream-python-0.8/appstream_python/StandardConstants.py` & `appstream_python-0.8.1/appstream_python/StandardConstants.py`

 * *Files identical despite different names*

### Comparing `appstream-python-0.8/appstream_python.egg-info/PKG-INFO` & `appstream_python-0.8.1/appstream_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appstream-python
-Version: 0.8
+Version: 0.8.1
 Summary: A library for dealing with Freedesktop Appstream data
 Author-email: JakobDev <jakobdev@gmx.de>
 License: BSD-2-Clause
 Project-URL: Documentation, https://appstream-python.readthedocs.io
 Project-URL: Issues, https://codeberg.org/JakobDev/appstream-python/issues
 Project-URL: Source, https://codeberg.org/JakobDev/appstream-python
 Project-URL: Donation, https://ko-fi.com/jakobdev
```

### Comparing `appstream-python-0.8/appstream_python.egg-info/SOURCES.txt` & `appstream_python-0.8.1/appstream_python.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -12,10 +12,11 @@
 appstream_python/version.txt
 appstream_python.egg-info/PKG-INFO
 appstream_python.egg-info/SOURCES.txt
 appstream_python.egg-info/dependency_links.txt
 appstream_python.egg-info/requires.txt
 appstream_python.egg-info/top_level.txt
 tests/test_appstream_data.py
+tests/test_collection.py
 tests/test_description.py
 tests/test_display_length.py
 tests/test_releases.py
```

### Comparing `appstream-python-0.8/pyproject.toml` & `appstream_python-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `appstream-python-0.8/tests/test_appstream_data.py` & `appstream_python-0.8.1/tests/test_appstream_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     assert len(component.releases) == 25
     assert component.releases.type == "embedded"
     assert component.releases[0].version == "10.3"
 
     assert component.display_length["recommends"][0].px == 760
     assert component.display_length["recommends"][0].compare == "ge"
 
+    assert component.get_available_languages() == ["de"]
+
 
 def test_from_component_tag() -> None:
     root = etree.parse(JDTEXTEDIT_METAINFO)
     component = appstream_python.AppstreamComponent.from_component_tag(root)
     assert_component_jdtextedit(component)
```

### Comparing `appstream-python-0.8/tests/test_description.py` & `appstream_python-0.8.1/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `appstream-python-0.8/tests/test_display_length.py` & `appstream_python-0.8.1/tests/test_display_length.py`

 * *Files identical despite different names*

### Comparing `appstream-python-0.8/tests/test_releases.py` & `appstream_python-0.8.1/tests/test_releases.py`

 * *Files identical despite different names*

