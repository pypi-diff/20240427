# Comparing `tmp/hanoikovoiduocdau-0.0.2.tar.gz` & `tmp/hanoikovoiduocdau-0.0.3.tar.gz`

## Comparing `hanoikovoiduocdau-0.0.2.tar` & `hanoikovoiduocdau-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.2/src/hanoikovoidcdau/__init__.py
--rw-r--r--   0        0        0    87256 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.2/src/hanoikovoidcdau/data.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.2/src/hanoikovoidcdau/standardize.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.2/tests/main.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.2/LICENSE
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.2/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.3/src/hanoikovoidcdau/__init__.py
+-rw-r--r--   0        0        0    89167 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.3/src/hanoikovoidcdau/standardize.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.3/tests/main.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.3/LICENSE
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.3/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 hanoikovoiduocdau-0.0.3/PKG-INFO
```

### Comparing `hanoikovoiduocdau-0.0.2/src/hanoikovoidcdau/data.py` & `hanoikovoiduocdau-0.0.3/src/hanoikovoidcdau/standardize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,74 @@
+import difflib
+
+useless_street_keywords = ["Phố", "Đường"]
+useless_ward_keywords = ["Phường", "Quận", "Huyện"]
+
+
+def get_all_streets(standard_data):
+    all_streets = []
+    for district in standard_data["district"]:
+        for street in district["streets"]:
+            street = remove_keywords(useless_street_keywords, street)
+            all_streets.append(street)
+    return all_streets
+
+
+def get_all_wards(standard_data):
+    all_wards = []
+    for district in standard_data["district"]:
+        for ward in district["wards"]:
+            ward = remove_keywords(useless_ward_keywords, ward)
+            all_wards.append(ward)
+    return all_wards
+
+
+def get_all_district(standard_data):
+    all_districts = []
+    for district in standard_data["district"]:
+        all_districts.append(district["name"])
+
+    print(all_districts)
+    return all_districts
+
+
+def find_closest_match(input_street, standard_data):
+    closest_match = difflib.get_close_matches(input_street, standard_data)
+    if closest_match:
+        return closest_match[0]
+
+    return input_street
+
+
+def standardize_street_name(street: str) -> str:
+    street = remove_keywords(useless_street_keywords, street)
+    all_streets = get_all_streets(data)
+    ans = find_closest_match(street, all_streets)
+    return ans
+
+
+def standardize_ward_name(ward: str) -> str:
+    ward = remove_keywords(useless_ward_keywords, ward)
+    all_wards = get_all_wards(data)
+    ans = find_closest_match(ward, all_wards)
+    return ans
+
+
+def standardize_district_name(district: str) -> str:
+    all_districts = get_all_district(data)
+    ans = find_closest_match(district, all_districts)
+    return ans
+
+
+def remove_keywords(useless_keywords: list, street: str) -> str:
+    for keyword in useless_keywords:
+        street = street.replace(keyword, "").strip()
+    return street
+
+
 data = {
     "district": [
         {
             "date": "2024-04-27 00:07:43",
             "name": "Gia Lâm",
             "wards": [
                     "Trâu quỳ",
```

### Comparing `hanoikovoiduocdau-0.0.2/LICENSE` & `hanoikovoiduocdau-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hanoikovoiduocdau-0.0.2/pyproject.toml` & `hanoikovoiduocdau-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/hanoikovoidcdau"]
 
 [project]
 name = "hanoikovoiduocdau"
-version = "0.0.2"
+version = "0.0.3"
 authors = [{ name = "betty2310", email = "huynhduongsh1@gmail.com" }]
 description = "A package for standardize Hanoi's address"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `hanoikovoiduocdau-0.0.2/PKG-INFO` & `hanoikovoiduocdau-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hanoikovoiduocdau
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for standardize Hanoi's address
 Project-URL: Homepage, https://github.com/betty2310/hanoikovoiduocdau
 Project-URL: Issues, https://github.com/betty2310/hanoikovoiduocdau/issues
 Author-email: betty2310 <huynhduongsh1@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

