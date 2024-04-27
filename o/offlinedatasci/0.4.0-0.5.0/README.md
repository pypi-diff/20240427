# Comparing `tmp/offlinedatasci-0.4.0.tar.gz` & `tmp/offlinedatasci-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offlinedatasci-0.4.0.tar", last modified: Fri Feb  2 13:03:28 2024, max compression
+gzip compressed data, was "offlinedatasci-0.5.0.tar", last modified: Sat Apr 27 18:04:59 2024, max compression
```

## Comparing `offlinedatasci-0.4.0.tar` & `offlinedatasci-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2024-02-02 13:03:28.519928 offlinedatasci-0.4.0/
--rw-rw-r--   0 ethan     (1000) ethan     (1000)     1071 2023-03-08 01:31:34.000000 offlinedatasci-0.4.0/LICENSE
--rw-rw-r--   0 ethan     (1000) ethan     (1000)       52 2023-03-08 01:31:34.000000 offlinedatasci-0.4.0/MANIFEST.in
--rw-r--r--   0 ethan     (1000) ethan     (1000)     4413 2024-02-02 13:03:28.519928 offlinedatasci-0.4.0/PKG-INFO
--rw-rw-r--   0 ethan     (1000) ethan     (1000)     2669 2024-02-02 12:52:54.000000 offlinedatasci-0.4.0/README.md
-drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2024-02-02 13:03:28.519928 offlinedatasci-0.4.0/docs/
--rw-rw-r--   0 ethan     (1000) ethan     (1000)     1202 2024-02-02 12:49:40.000000 offlinedatasci-0.4.0/docs/conf.py
-drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2024-02-02 13:03:28.519928 offlinedatasci-0.4.0/offlinedatasci/
--rw-rw-r--   0 ethan     (1000) ethan     (1000)       62 2024-02-02 12:49:20.000000 offlinedatasci-0.4.0/offlinedatasci/__init__.py
--rw-rw-r--   0 ethan     (1000) ethan     (1000)     2363 2024-01-25 01:33:30.000000 offlinedatasci-0.4.0/offlinedatasci/cli.py
--rw-rw-r--   0 ethan     (1000) ethan     (1000)    15427 2024-02-02 12:51:01.000000 offlinedatasci-0.4.0/offlinedatasci/main.py
--rw-rw-r--   0 ethan     (1000) ethan     (1000)     1847 2024-02-02 12:51:01.000000 offlinedatasci-0.4.0/offlinedatasci/miniCran.R
-drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2024-02-02 13:03:28.519928 offlinedatasci-0.4.0/offlinedatasci.egg-info/
--rw-r--r--   0 ethan     (1000) ethan     (1000)     4413 2024-02-02 13:03:28.000000 offlinedatasci-0.4.0/offlinedatasci.egg-info/PKG-INFO
--rw-rw-r--   0 ethan     (1000) ethan     (1000)      413 2024-02-02 13:03:28.000000 offlinedatasci-0.4.0/offlinedatasci.egg-info/SOURCES.txt
--rw-rw-r--   0 ethan     (1000) ethan     (1000)        1 2024-02-02 13:03:28.000000 offlinedatasci-0.4.0/offlinedatasci.egg-info/dependency_links.txt
--rw-rw-r--   0 ethan     (1000) ethan     (1000)       59 2024-02-02 13:03:28.000000 offlinedatasci-0.4.0/offlinedatasci.egg-info/entry_points.txt
--rw-rw-r--   0 ethan     (1000) ethan     (1000)       77 2024-02-02 13:03:28.000000 offlinedatasci-0.4.0/offlinedatasci.egg-info/requires.txt
--rw-rw-r--   0 ethan     (1000) ethan     (1000)       30 2024-02-02 13:03:28.000000 offlinedatasci-0.4.0/offlinedatasci.egg-info/top_level.txt
--rw-rw-r--   0 ethan     (1000) ethan     (1000)     1860 2024-02-02 12:49:14.000000 offlinedatasci-0.4.0/pyproject.toml
--rw-rw-r--   0 ethan     (1000) ethan     (1000)       38 2024-02-02 13:03:28.519928 offlinedatasci-0.4.0/setup.cfg
-drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2024-02-02 13:03:28.519928 offlinedatasci-0.4.0/test/
--rw-rw-r--   0 ethan     (1000) ethan     (1000)     1025 2024-02-02 12:51:01.000000 offlinedatasci-0.4.0/test/test_offlinedatasci.py
+drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2024-04-27 18:04:59.688532 offlinedatasci-0.5.0/
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)     1071 2023-03-08 01:31:34.000000 offlinedatasci-0.5.0/LICENSE
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)       52 2023-03-08 01:31:34.000000 offlinedatasci-0.5.0/MANIFEST.in
+-rw-r--r--   0 ethan     (1000) ethan     (1000)     4437 2024-04-27 18:04:59.688532 offlinedatasci-0.5.0/PKG-INFO
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)     2669 2024-03-07 12:18:01.000000 offlinedatasci-0.5.0/README.md
+drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2024-04-27 18:04:59.684532 offlinedatasci-0.5.0/docs/
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)     1202 2024-04-27 18:03:53.000000 offlinedatasci-0.5.0/docs/conf.py
+drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2024-04-27 18:04:59.684532 offlinedatasci-0.5.0/offlinedatasci/
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)       62 2024-04-27 18:03:53.000000 offlinedatasci-0.5.0/offlinedatasci/__init__.py
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)     2180 2024-03-07 12:18:15.000000 offlinedatasci-0.5.0/offlinedatasci/cli.py
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)    16933 2024-04-27 17:57:58.000000 offlinedatasci-0.5.0/offlinedatasci/main.py
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)     1847 2024-03-07 12:18:01.000000 offlinedatasci-0.5.0/offlinedatasci/miniCran.R
+drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2024-04-27 18:04:59.688532 offlinedatasci-0.5.0/offlinedatasci.egg-info/
+-rw-r--r--   0 ethan     (1000) ethan     (1000)     4437 2024-04-27 18:04:59.000000 offlinedatasci-0.5.0/offlinedatasci.egg-info/PKG-INFO
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)      413 2024-04-27 18:04:59.000000 offlinedatasci-0.5.0/offlinedatasci.egg-info/SOURCES.txt
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)        1 2024-04-27 18:04:59.000000 offlinedatasci-0.5.0/offlinedatasci.egg-info/dependency_links.txt
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)       59 2024-04-27 18:04:59.000000 offlinedatasci-0.5.0/offlinedatasci.egg-info/entry_points.txt
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)       86 2024-04-27 18:04:59.000000 offlinedatasci-0.5.0/offlinedatasci.egg-info/requires.txt
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)       36 2024-04-27 18:04:59.000000 offlinedatasci-0.5.0/offlinedatasci.egg-info/top_level.txt
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)     1874 2024-04-27 18:03:53.000000 offlinedatasci-0.5.0/pyproject.toml
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)       38 2024-04-27 18:04:59.688532 offlinedatasci-0.5.0/setup.cfg
+drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2024-04-27 18:04:59.688532 offlinedatasci-0.5.0/test/
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)     1361 2024-04-27 17:12:23.000000 offlinedatasci-0.5.0/test/test_offlinedatasci.py
```

### Comparing `offlinedatasci-0.4.0/LICENSE` & `offlinedatasci-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `offlinedatasci-0.4.0/PKG-INFO` & `offlinedatasci-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offlinedatasci
-Version: 0.4.0
+Version: 0.5.0
 Summary: Download and configure common tools for teaching and doing data science without an internet connection
 Author: Virnaliz Cruz, Colin Sauze, Jannetta Steyn, Abhishek Dasgupta, Ethan P. White
 Project-URL: Carpentries Offline Website, https://carpentriesoffline.github.io/
 Project-URL: Documentation, https://github.com/carpentriesoffline/offlinedatasci/#readme
 Project-URL: CI, https://github.com/carpentriesoffline/offlinedatasci/actions
 Project-URL: Source, https://github.com/carpentriesoffline/offlinedatasci
 Project-URL: Tracker, https://github.com/carpentriesoffline/offlinedatasci/issues
@@ -30,14 +30,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: airium
 Requires-Dist: beautifulsoup4
 Requires-Dist: importlib_resources
 Requires-Dist: lxml
 Requires-Dist: python-pypi-mirror
+Requires-Dist: requests
 Requires-Dist: setuptools
 
 [![Build Check](https://github.com/carpentriesoffline/offlinedatasci/actions/workflows/package-check.yml/badge.svg)](https://github.com/carpentriesoffline/offlinedatasci/actions/workflows/package-check.yml)
 [![Documentation Status](https://readthedocs.org/projects/offlinedatasci/badge/?version=latest)](https://offlinedatasci.readthedocs.io/en/latest/?badge=latest)
 
 # OfflineDataSci
```

### Comparing `offlinedatasci-0.4.0/README.md` & `offlinedatasci-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `offlinedatasci-0.4.0/docs/conf.py` & `offlinedatasci-0.5.0/docs/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'offlinedatasci'
 copyright = '2023, Virnaliz Cruz, Abhishek Dasgupta, Colin Sauze, Jannetta Steyn, Ethan P. White'
 author = 'Virnaliz Cruz, Abhishek Dasgupta, Colin Sauze, Jannetta Steyn, Ethan P. White'
-release = 'v0.4.0'
+release = 'v0.5.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['myst_parser',
               'sphinx.ext.autodoc',
               'sphinx_rtd_theme']
```

### Comparing `offlinedatasci-0.4.0/offlinedatasci/cli.py` & `offlinedatasci-0.5.0/offlinedatasci/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import argparse
 from secrets import choice
 import sys
 from offlinedatasci import *
 
-function_list = [download_r,download_rstudio,download_minicran,
-                 download_lessons,download_python,
-                 download_python_libraries]
-def get_installer_functions(selection, ods_dir):
+def get_installer_function(selection, ods_dir):
     if selection == "all":
-        try_except_functions(ods_dir, function_list)
+        download_all(ods_dir)
     elif selection == "rstudio":
         try_except_functions(ods_dir, download_rstudio)
     elif selection == "python":
         try_except_functions(ods_dir, download_python)
     else:
         try:
             download_function = f"download_{selection}"
             getattr(sys.modules[__name__], download_function)(ods_dir)
         except Exception:
             print(f'method does not exist for selection: {selection}')
+
 def main():
     parser = argparse.ArgumentParser(prog = 'offlinedatasci')
     subparsers = parser.add_subparsers(help = 'sub-command help', dest='command')
     INSTALL_OPTIONS = ["all", "lessons", "minicran", "python", "python_libraries", "r", "rstudio"]
 
     install_parser = subparsers.add_parser('install')
     install_parser.add_argument('item',
@@ -44,15 +42,15 @@
 
 
     args = parser.parse_args()
     ods_dir = get_ods_dir(args.path)
 
     if args.command == 'install':
         for i in args.item:
-            get_installer_functions(i, ods_dir)
+            get_installer_function(i, ods_dir)
 
     elif args.command == 'add-packages':
         packages_to_install = package_selection(args.language[0], args.libraries)
         if args.language[0] == "python":
             download_python_libraries(ods_dir, packages_to_install)
         elif args.language[0] == "r":
             download_minicran(ods_dir, packages_to_install)
```

### Comparing `offlinedatasci-0.4.0/offlinedatasci/main.py` & `offlinedatasci-0.5.0/offlinedatasci/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import bs4 as bs
 import os
 import re
 import subprocess
 import urllib.request, urllib.error, urllib.parse
 import importlib_resources
 import pypi_mirror
+import requests
 import shutil
 import sys
 import warnings
 
 def add_lesson_index_page(lesson_path):
     """Add a basic landing page for lessons
     
@@ -41,14 +42,52 @@
                         lesson_index = Path(Path(source), Path(lesson), Path("index.html"))
                         with a.a(href = lesson_index):
                             a(lesson.replace('-', ' ').title())
 
     with open(Path(Path(lesson_path), Path("index.html")), "w+") as index_file:
         index_file.writelines(str(a))
 
+def download_all(ods_dir):
+    """Download all installers, repositories, and lesson materials.
+
+    Each function will run even if others fail.
+
+    Keyword arguments:
+    ods_dir -- Directory to save installers and lesson materials
+    """
+    try:
+        download_r(ods_dir)
+    except Exception as e:
+        print(f"Error downloading R: {e}")
+
+    try:
+        download_rstudio(ods_dir)
+    except Exception as e:
+        print(f"Error downloading RStudio: {e}")
+
+    try:
+        download_minicran(ods_dir)
+    except Exception as e:
+        print(f"Error downloading R packages: {e}")
+
+    try:
+        download_lessons(ods_dir)
+    except Exception as e:
+        print(f"Error downloading lessons: {e}")
+
+    try:
+        download_python(ods_dir)
+    except Exception as e:
+        print(f"Error downloading Python: {e}")
+
+    try:
+        download_python_libraries(ods_dir)
+    except Exception as e:
+        print(f"Error downloading Python packages: {e}")
+
 def download_and_save_installer(latest_version_url, destination_path):
     """Download and save installer in user given path.
 
     Keyword arguments:
     latest_version_url -- Link to download installer
     destination_path -- Path to save installer
     """
@@ -147,16 +186,16 @@
 
 def download_rstudio(ods_dir):
     """Download RStudio installers"""
     baseurl = 'https://www.rstudio.com/products/rstudio/download/#download'
     destination_path = Path(Path(ods_dir), Path("rstudio"))
     if not os.path.isdir(destination_path):
         os.makedirs(destination_path)
-    fp = urllib.request.urlopen(baseurl)
-    web_content = fp.read()
+    fp = requests.get(baseurl)
+    web_content = fp.content
     soup = bs.BeautifulSoup(web_content, 'lxml')
     links = soup.find_all('a')
     for link in links:
         if link.has_attr('href') and (".exe" in link['href'] or ".dmg" in link['href']):
             url = str(link['href'])
             download_and_save_installer(url, Path(Path(destination_path), Path(os.path.basename(url))))
 
@@ -172,16 +211,16 @@
     hrefcolnum=0
     key="version"
 
     destination_path = Path(Path(ods_dir), Path("python"))
     if not os.path.isdir(destination_path):
         os.makedirs(destination_path)
     python_versions = {}
-    fp = urllib.request.urlopen(url)
-    web_content = fp.read()
+    fp = requests.get(url)
+    web_content = fp.content
     soup = bs.BeautifulSoup(web_content, 'lxml')
     r_studio_download_table = soup.find_all('table')[download_table_num]
     table_body = r_studio_download_table.find('tbody')
     python_versions = {}
     for row in table_body.find_all("tr"):
       os_data = table_parse_version_info(row,oscolnum,hrefcolnum)
       os_version = os_data[key] 
@@ -197,15 +236,15 @@
 def find_r_current_version(url):
     """Determine the most recent version of R from CRAN
 
     Keyword arguments:
     url -- CRAN r-project URL
     """
     version_regex = "(R\-\d+\.\d+\.\d)+\-(?:x86_64|arm64|win)\.(?:exe|pkg)"
-    urlfile = urllib.request.urlopen(url)
+    urlfile = requests.get(url)
     for line in urlfile:
         decoded = line.decode("utf-8") 
         match = re.findall(version_regex, decoded)
         if (match):
             r_current_version = match[0].strip(".exe").strip(".pkg")
             return r_current_version
     return None
@@ -255,22 +294,29 @@
         print("\nCreating ods folder in " + str(directory))
         Path.mkdir(folder_path, parents=True)
     return str(folder_path)
 
 def get_python_download_page():
     """Get download page from Python homepage."""
     base_url="https://www.python.org"
-    fp = urllib.request.urlopen(base_url)
-    web_content = fp.read()
+    fp = requests.get(base_url)
+    web_content = fp.content
     soup = bs.BeautifulSoup(web_content, "html.parser")
     release_a_tag = soup.find("a", href=lambda href: href and "release" in href)
     current_release_path = release_a_tag["href"]
     current_release_url = base_url + current_release_path
     return(current_release_url)
 
+def get_python_version():
+    """Determine the Python version from the Python homepage."""
+    python_download_page = get_python_download_page()
+    version_txt = python_download_page.split('-')[1][0:3]
+    version = version_txt[0] + "." + version_txt[1:3]
+    return version
+
 def table_parse_version_info(row,oscolnum,hrefcolnum):
     """Parse and return software information from table.
 
     Keyword arguments:
     row -- Row from HTML table
     oscolnum -- Number of column in which OS is found
     hrefcolnum -- Number of column in which HREFs are found
@@ -313,27 +359,36 @@
 
 def download_python_libraries(ods_dir,py_library_reqs = [ "matplotlib", "notebook","numpy", "pandas"] ):
     """Creating partial PyPI mirror of workshop libraries.
 
     Keyword arguments:
     ods_dir -- Directory to save partial Pypi mirror
     """
-    #workshop_needed_libraries = pandas, matplotlib, numpy
-    #python_included_libraries = math, random, glob, time, sys, pathlib
+    python_version = get_python_version()
     download_dir = Path(Path(ods_dir), Path("pythonlibraries"))
     pypi_dir = Path(Path(ods_dir), Path("pypi"))
     parameters = {
         'pip': 'pip3',
         'dest': download_dir,
         'pkgs': py_library_reqs,
-        'python_version': '3.11',
+        'python_version': python_version,
         'allow_binary': True
     }
-    pypi_mirror.download(platform = ['manylinux_2_17_x86_64'], **parameters)
-    pypi_mirror.download(platform = ['macosx_10_12_x86_64'], **parameters)
+    if sys.platform == 'win32':
+        # pip download does not currently work for other OSs on Windows
+        # Therefore we don't download mac and Linux packages on Windows
+        # See https://github.com/pypa/pip/issues/11664
+        warnings.warn("""Only mirroring Python packages for Windows
+                      
+        pip cannot currently download macos and Linux packages on Windows.
+        See https://github.com/pypa/pip/issues/11664
+        """)
+    else:
+        pypi_mirror.download(platform = ['manylinux_2_17_x86_64'], **parameters)
+        pypi_mirror.download(platform = ['macosx_10_12_x86_64'], **parameters)
     pypi_mirror.download(platform = ['win_amd64'], **parameters)
     mirror_creation_parameters = {
         'download_dir': download_dir,
         'mirror_dir': pypi_dir,
         'copy': True
     }
     pypi_mirror.create_mirror(**mirror_creation_parameters)
@@ -360,15 +415,12 @@
         if item in [*language_dictionary]:
             packages_to_download.extend(language_dictionary[item])
         else:
             packages_to_download.append(item)
     packages_to_download = list(set(packages_to_download))
     return packages_to_download
 
-def try_except_functions(input,functions):
-    if not isinstance(functions, list):
-        functions = [functions]
-    for function in functions:
-        try:
-            function(input)
-        except Exception as e:
-            print( f"Error in function: {function.__name__}. Error: {str(e)}")
+def try_except_functions(input, function):
+    try:
+        function(input)
+    except Exception as e:
+        print( f"Error in function: {function.__name__}. Error: {str(e)}")
```

### Comparing `offlinedatasci-0.4.0/offlinedatasci/miniCran.R` & `offlinedatasci-0.5.0/offlinedatasci/miniCran.R`

 * *Files identical despite different names*

### Comparing `offlinedatasci-0.4.0/offlinedatasci.egg-info/PKG-INFO` & `offlinedatasci-0.5.0/offlinedatasci.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offlinedatasci
-Version: 0.4.0
+Version: 0.5.0
 Summary: Download and configure common tools for teaching and doing data science without an internet connection
 Author: Virnaliz Cruz, Colin Sauze, Jannetta Steyn, Abhishek Dasgupta, Ethan P. White
 Project-URL: Carpentries Offline Website, https://carpentriesoffline.github.io/
 Project-URL: Documentation, https://github.com/carpentriesoffline/offlinedatasci/#readme
 Project-URL: CI, https://github.com/carpentriesoffline/offlinedatasci/actions
 Project-URL: Source, https://github.com/carpentriesoffline/offlinedatasci
 Project-URL: Tracker, https://github.com/carpentriesoffline/offlinedatasci/issues
@@ -30,14 +30,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: airium
 Requires-Dist: beautifulsoup4
 Requires-Dist: importlib_resources
 Requires-Dist: lxml
 Requires-Dist: python-pypi-mirror
+Requires-Dist: requests
 Requires-Dist: setuptools
 
 [![Build Check](https://github.com/carpentriesoffline/offlinedatasci/actions/workflows/package-check.yml/badge.svg)](https://github.com/carpentriesoffline/offlinedatasci/actions/workflows/package-check.yml)
 [![Documentation Status](https://readthedocs.org/projects/offlinedatasci/badge/?version=latest)](https://offlinedatasci.readthedocs.io/en/latest/?badge=latest)
 
 # OfflineDataSci
```

### Comparing `offlinedatasci-0.4.0/pyproject.toml` & `offlinedatasci-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "offlinedatasci"
 description = "Download and configure common tools for teaching and doing data science without an internet connection"
 readme = "README.md"
-version = "0.4.0"
+version = "0.5.0"
 
 authors = [
   { name="Virnaliz Cruz" },
   { name="Colin Sauze" },
   { name="Jannetta Steyn" },
   { name="Abhishek Dasgupta" },
   { name="Ethan P. White" },
@@ -39,14 +39,15 @@
 
 dependencies = [
   'airium',
   'beautifulsoup4',
   'importlib_resources',
   'lxml',
   'python-pypi-mirror',
+  'requests',
   'setuptools'
 ]
 
 requires-python = ">=3.6"
 
 [project.urls]
 "Carpentries Offline Website" = "https://carpentriesoffline.github.io/"
```

