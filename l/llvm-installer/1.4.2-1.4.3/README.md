# Comparing `tmp/llvm_installer-1.4.2.tar.gz` & `tmp/llvm_installer-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llvm_installer-1.4.2.tar", last modified: Tue Apr 16 00:32:37 2024, max compression
+gzip compressed data, was "llvm_installer-1.4.3.tar", last modified: Fri Apr 26 22:33:22 2024, max compression
```

## Comparing `llvm_installer-1.4.2.tar` & `llvm_installer-1.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-04-16 00:32:37.843134 llvm_installer-1.4.2/
--rw-r--r--   0 mikhail    (503) staff       (20)    11358 2022-05-26 15:06:09.000000 llvm_installer-1.4.2/LICENSE
--rw-r--r--   0 mikhail    (503) staff       (20)     1268 2024-04-16 00:32:37.842871 llvm_installer-1.4.2/PKG-INFO
--rw-r--r--   0 mikhail    (503) staff       (20)      643 2022-07-07 03:18:16.000000 llvm_installer-1.4.2/README.md
--rw-r--r--   0 mikhail    (503) staff       (20)       38 2024-04-16 00:32:37.843196 llvm_installer-1.4.2/setup.cfg
--rw-r--r--   0 mikhail    (503) staff       (20)     2235 2024-04-16 00:23:06.000000 llvm_installer-1.4.2/setup.py
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-04-16 00:32:37.839516 llvm_installer-1.4.2/src/
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-04-16 00:32:37.840700 llvm_installer-1.4.2/src/llvm_installer/
--rw-r--r--   0 mikhail    (503) staff       (20)    11455 2022-08-17 05:24:37.000000 llvm_installer-1.4.2/src/llvm_installer/__init__.py
--rw-r--r--   0 mikhail    (503) staff       (20)     5477 2023-08-24 20:40:18.000000 llvm_installer-1.4.2/src/llvm_installer/__main__.py
--rw-r--r--   0 mikhail    (503) staff       (20)        0 2022-05-26 15:06:09.000000 llvm_installer-1.4.2/src/llvm_installer/py.typed
--rw-r--r--   0 mikhail    (503) staff       (20)   144169 2024-04-16 00:19:40.000000 llvm_installer-1.4.2/src/llvm_installer/release_tags.json
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-04-16 00:32:37.842227 llvm_installer-1.4.2/src/llvm_installer.egg-info/
--rw-r--r--   0 mikhail    (503) staff       (20)     1268 2024-04-16 00:32:37.000000 llvm_installer-1.4.2/src/llvm_installer.egg-info/PKG-INFO
--rw-r--r--   0 mikhail    (503) staff       (20)      407 2024-04-16 00:32:37.000000 llvm_installer-1.4.2/src/llvm_installer.egg-info/SOURCES.txt
--rw-r--r--   0 mikhail    (503) staff       (20)        1 2024-04-16 00:32:37.000000 llvm_installer-1.4.2/src/llvm_installer.egg-info/dependency_links.txt
--rw-r--r--   0 mikhail    (503) staff       (20)       64 2024-04-16 00:32:37.000000 llvm_installer-1.4.2/src/llvm_installer.egg-info/entry_points.txt
--rw-r--r--   0 mikhail    (503) staff       (20)       86 2024-04-16 00:32:37.000000 llvm_installer-1.4.2/src/llvm_installer.egg-info/requires.txt
--rw-r--r--   0 mikhail    (503) staff       (20)       15 2024-04-16 00:32:37.000000 llvm_installer-1.4.2/src/llvm_installer.egg-info/top_level.txt
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-04-26 22:33:22.381458 llvm_installer-1.4.3/
+-rw-r--r--   0 mikhail    (503) staff       (20)    11358 2022-05-26 15:06:09.000000 llvm_installer-1.4.3/LICENSE
+-rw-r--r--   0 mikhail    (503) staff       (20)     1268 2024-04-26 22:33:22.381199 llvm_installer-1.4.3/PKG-INFO
+-rw-r--r--   0 mikhail    (503) staff       (20)      643 2022-07-07 03:18:16.000000 llvm_installer-1.4.3/README.md
+-rw-r--r--   0 mikhail    (503) staff       (20)       38 2024-04-26 22:33:22.381522 llvm_installer-1.4.3/setup.cfg
+-rw-r--r--   0 mikhail    (503) staff       (20)     2235 2024-04-26 22:02:31.000000 llvm_installer-1.4.3/setup.py
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-04-26 22:33:22.376157 llvm_installer-1.4.3/src/
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-04-26 22:33:22.377253 llvm_installer-1.4.3/src/llvm_installer/
+-rw-r--r--   0 mikhail    (503) staff       (20)    11455 2022-08-17 05:24:37.000000 llvm_installer-1.4.3/src/llvm_installer/__init__.py
+-rw-r--r--   0 mikhail    (503) staff       (20)     5477 2023-08-24 20:40:18.000000 llvm_installer-1.4.3/src/llvm_installer/__main__.py
+-rw-r--r--   0 mikhail    (503) staff       (20)        0 2022-05-26 15:06:09.000000 llvm_installer-1.4.3/src/llvm_installer/py.typed
+-rw-r--r--   0 mikhail    (503) staff       (20)   149874 2024-04-26 21:59:25.000000 llvm_installer-1.4.3/src/llvm_installer/release_tags.json
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-04-26 22:33:22.380569 llvm_installer-1.4.3/src/llvm_installer.egg-info/
+-rw-r--r--   0 mikhail    (503) staff       (20)     1268 2024-04-26 22:33:22.000000 llvm_installer-1.4.3/src/llvm_installer.egg-info/PKG-INFO
+-rw-r--r--   0 mikhail    (503) staff       (20)      407 2024-04-26 22:33:22.000000 llvm_installer-1.4.3/src/llvm_installer.egg-info/SOURCES.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)        1 2024-04-26 22:33:22.000000 llvm_installer-1.4.3/src/llvm_installer.egg-info/dependency_links.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)       64 2024-04-26 22:33:22.000000 llvm_installer-1.4.3/src/llvm_installer.egg-info/entry_points.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)       86 2024-04-26 22:33:22.000000 llvm_installer-1.4.3/src/llvm_installer.egg-info/requires.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)       15 2024-04-26 22:33:22.000000 llvm_installer-1.4.3/src/llvm_installer.egg-info/top_level.txt
```

### Comparing `llvm_installer-1.4.2/LICENSE` & `llvm_installer-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llvm_installer-1.4.2/PKG-INFO` & `llvm_installer-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llvm-installer
-Version: 1.4.2
+Version: 1.4.3
 Summary: Allows installing pre-built LLVM packages for various operating systems
 Home-page: https://github.com/yugabyte/llvm-installer
 Author: Mikhail Bautin
 Author-email: mbautin@users.noreply.github.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: packaging
```

### Comparing `llvm_installer-1.4.2/README.md` & `llvm_installer-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `llvm_installer-1.4.2/setup.py` & `llvm_installer-1.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     from os import path
     this_directory = path.abspath(path.dirname(__file__))
     with open(path.join(this_directory, 'README.md'), encoding='utf-8') as readme_file:
         long_description = readme_file.read()
 
     setup(
         name='llvm-installer',
-        version='1.4.2',
+        version='1.4.3',
         url='https://github.com/yugabyte/llvm-installer',
         author='Mikhail Bautin',
         author_email='mbautin@users.noreply.github.com',
         description='Allows installing pre-built LLVM packages for various operating systems',
         packages=find_packages(where='src'),
         package_dir={"": "src"},
         package_data={'llvm_installer': ['py.typed', 'release_tags.json']},
```

### Comparing `llvm_installer-1.4.2/src/llvm_installer/__init__.py` & `llvm_installer-1.4.3/src/llvm_installer/__init__.py`

 * *Files identical despite different names*

### Comparing `llvm_installer-1.4.2/src/llvm_installer/__main__.py` & `llvm_installer-1.4.3/src/llvm_installer/__main__.py`

 * *Files identical despite different names*

### Comparing `llvm_installer-1.4.2/src/llvm_installer/release_tags.json` & `llvm_installer-1.4.3/src/llvm_installer/release_tags.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9809384164222874%*

 * *Differences: {"'parsed_tags'": "{insert: [(271, OrderedDict([('architecture', 'aarch64'), "*

 * *                  "('is_old_tag_without_os_and_arch', False), ('major_version', 17), "*

 * *                  "('minor_version', 0), ('patch_version', 6), ('sha1_prefix', '9b881774'), "*

 * *                  "('short_os_name_and_version', 'amzn2'), ('tag', "*

 * *                  "'v17.0.6-yb-1-1714076298-9b881774-amzn2-aarch64'), ('timestamp', '1714076298'), "*

 * *                  "('version', '17.0.6'), ('version_suffix', 'yb-1'), ('yb_suffix_ […]*

```diff
@@ -3795,14 +3795,42 @@
             "yb_suffix_version": 1
         },
         {
             "architecture": "aarch64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 17,
             "minor_version": 0,
+            "patch_version": 6,
+            "sha1_prefix": "9b881774",
+            "short_os_name_and_version": "amzn2",
+            "tag": "v17.0.6-yb-1-1714076298-9b881774-amzn2-aarch64",
+            "timestamp": "1714076298",
+            "version": "17.0.6",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 17,
+            "minor_version": 0,
+            "patch_version": 6,
+            "sha1_prefix": "9b881774",
+            "short_os_name_and_version": "amzn2",
+            "tag": "v17.0.6-yb-1-1714070589-9b881774-amzn2-x86_64",
+            "timestamp": "1714070589",
+            "version": "17.0.6",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 17,
+            "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "ff047e99",
             "short_os_name_and_version": "centos7",
             "tag": "v17.0.0-rc3-yb-1-1692919510-ff047e99-centos7-aarch64",
             "timestamp": "1692919510",
             "version": "17.0.0",
             "version_suffix": "rc3-yb-1",
@@ -4407,14 +4435,28 @@
             "tag": "v18.1.2-yb-1-1711588306-53fdd023-almalinux8-aarch64",
             "timestamp": "1711588306",
             "version": "18.1.2",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 18,
+            "minor_version": 1,
+            "patch_version": 3,
+            "sha1_prefix": "317a1841",
+            "short_os_name_and_version": "almalinux8",
+            "tag": "v18.1.3-yb-1-1713354410-317a1841-almalinux8-aarch64",
+            "timestamp": "1713354410",
+            "version": "18.1.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 18,
             "minor_version": 1,
             "patch_version": 0,
             "sha1_prefix": "1d6270bf",
             "short_os_name_and_version": "almalinux8",
@@ -4435,28 +4477,70 @@
             "tag": "v18.1.2-yb-1-1711487585-53fdd023-almalinux8-x86_64",
             "timestamp": "1711487585",
             "version": "18.1.2",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 18,
+            "minor_version": 1,
+            "patch_version": 3,
+            "sha1_prefix": "317a1841",
+            "short_os_name_and_version": "almalinux8",
+            "tag": "v18.1.3-yb-1-1713309539-317a1841-almalinux8-x86_64",
+            "timestamp": "1713309539",
+            "version": "18.1.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 18,
+            "minor_version": 1,
+            "patch_version": 3,
+            "sha1_prefix": "317a1841",
+            "short_os_name_and_version": "almalinux8",
+            "tag": "v18.1.3-yb-1-1713309567-317a1841-almalinux8-x86_64",
+            "timestamp": "1713309567",
+            "version": "18.1.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "aarch64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 18,
             "minor_version": 1,
             "patch_version": 2,
             "sha1_prefix": "53fdd023",
             "short_os_name_and_version": "almalinux9",
             "tag": "v18.1.2-yb-1-1711597954-53fdd023-almalinux9-aarch64",
             "timestamp": "1711597954",
             "version": "18.1.2",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 18,
+            "minor_version": 1,
+            "patch_version": 3,
+            "sha1_prefix": "317a1841",
+            "short_os_name_and_version": "almalinux9",
+            "tag": "v18.1.3-yb-1-1713364232-317a1841-almalinux9-aarch64",
+            "timestamp": "1713364232",
+            "version": "18.1.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 18,
             "minor_version": 1,
             "patch_version": 0,
             "sha1_prefix": "1d6270bf",
             "short_os_name_and_version": "almalinux9",
@@ -4477,28 +4561,84 @@
             "tag": "v18.1.2-yb-1-1711492549-53fdd023-almalinux9-x86_64",
             "timestamp": "1711492549",
             "version": "18.1.2",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 18,
+            "minor_version": 1,
+            "patch_version": 3,
+            "sha1_prefix": "317a1841",
+            "short_os_name_and_version": "almalinux9",
+            "tag": "v18.1.3-yb-1-1713315838-317a1841-almalinux9-x86_64",
+            "timestamp": "1713315838",
+            "version": "18.1.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 18,
+            "minor_version": 1,
+            "patch_version": 3,
+            "sha1_prefix": "317a1841",
+            "short_os_name_and_version": "amzn2",
+            "tag": "v18.1.3-yb-1-1714085750-317a1841-amzn2-aarch64",
+            "timestamp": "1714085750",
+            "version": "18.1.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 18,
+            "minor_version": 1,
+            "patch_version": 3,
+            "sha1_prefix": "317a1841",
+            "short_os_name_and_version": "amzn2",
+            "tag": "v18.1.3-yb-1-1714074888-317a1841-amzn2-x86_64",
+            "timestamp": "1714074888",
+            "version": "18.1.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "aarch64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 18,
             "minor_version": 1,
             "patch_version": 2,
             "sha1_prefix": "53fdd023",
             "short_os_name_and_version": "centos7",
             "tag": "v18.1.2-yb-1-1711578240-53fdd023-centos7-aarch64",
             "timestamp": "1711578240",
             "version": "18.1.2",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 18,
+            "minor_version": 1,
+            "patch_version": 3,
+            "sha1_prefix": "317a1841",
+            "short_os_name_and_version": "centos7",
+            "tag": "v18.1.3-yb-1-1713344086-317a1841-centos7-aarch64",
+            "timestamp": "1713344086",
+            "version": "18.1.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 18,
             "minor_version": 1,
             "patch_version": 0,
             "sha1_prefix": "1d6270bf",
             "short_os_name_and_version": "centos7",
@@ -4533,14 +4673,28 @@
             "tag": "v18.1.2-yb-1-1711607838-53fdd023-ubuntu22.04-aarch64",
             "timestamp": "1711607838",
             "version": "18.1.2",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 18,
+            "minor_version": 1,
+            "patch_version": 3,
+            "sha1_prefix": "317a1841",
+            "short_os_name_and_version": "ubuntu22.04",
+            "tag": "v18.1.3-yb-1-1713374229-317a1841-ubuntu22.04-aarch64",
+            "timestamp": "1713374229",
+            "version": "18.1.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 18,
             "minor_version": 1,
             "patch_version": 0,
             "sha1_prefix": "1d6270bf",
             "short_os_name_and_version": "ubuntu22.04",
@@ -4565,14 +4719,28 @@
             "yb_suffix_version": 1
         },
         {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 18,
             "minor_version": 1,
+            "patch_version": 3,
+            "sha1_prefix": "317a1841",
+            "short_os_name_and_version": "ubuntu22.04",
+            "tag": "v18.1.3-yb-1-1713320479-317a1841-ubuntu22.04-x86_64",
+            "timestamp": "1713320479",
+            "version": "18.1.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 18,
+            "minor_version": 1,
             "patch_version": 0,
             "sha1_prefix": "1d6270bf",
             "short_os_name_and_version": "ubuntu23.04",
             "tag": "v18.1.0-rc2-yb-1-1708032174-1d6270bf-ubuntu23.04-x86_64",
             "timestamp": "1708032174",
             "version": "18.1.0",
             "version_suffix": "rc2-yb-1",
@@ -4587,10 +4755,24 @@
             "sha1_prefix": "53fdd023",
             "short_os_name_and_version": "ubuntu23.04",
             "tag": "v18.1.2-yb-1-1711501883-53fdd023-ubuntu23.04-x86_64",
             "timestamp": "1711501883",
             "version": "18.1.2",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
+        },
+        {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 18,
+            "minor_version": 1,
+            "patch_version": 3,
+            "sha1_prefix": "317a1841",
+            "short_os_name_and_version": "ubuntu23.04",
+            "tag": "v18.1.3-yb-1-1713325031-317a1841-ubuntu23.04-x86_64",
+            "timestamp": "1713325031",
+            "version": "18.1.3",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
         }
     ]
 }
```

### Comparing `llvm_installer-1.4.2/src/llvm_installer.egg-info/PKG-INFO` & `llvm_installer-1.4.3/src/llvm_installer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llvm-installer
-Version: 1.4.2
+Version: 1.4.3
 Summary: Allows installing pre-built LLVM packages for various operating systems
 Home-page: https://github.com/yugabyte/llvm-installer
 Author: Mikhail Bautin
 Author-email: mbautin@users.noreply.github.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: packaging
```

