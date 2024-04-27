# Comparing `tmp/yes_chef-0.9.2.tar.gz` & `tmp/yes_chef-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yes_chef-0.9.2.tar", last modified: Sat Apr 27 07:43:12 2024, max compression
+gzip compressed data, was "yes_chef-0.9.3.tar", last modified: Sat Apr 27 07:47:27 2024, max compression
```

## Comparing `yes_chef-0.9.2.tar` & `yes_chef-0.9.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:43:12.825572 yes_chef-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-27 07:43:12.825572 yes_chef-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-27 07:43:02.000000 yes_chef-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-27 07:43:03.000000 yes_chef-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 07:43:12.825572 yes_chef-0.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:43:12.817572 yes_chef-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:43:12.817572 yes_chef-0.9.2/src/api/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 07:43:03.000000 yes_chef-0.9.2/src/api/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/api/ingredient.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/api/initialise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/api/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:43:12.821572 yes_chef-0.9.2/src/api/recipe/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/api/recipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/api/recipe/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/api/recipe/recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/api/recipe/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/api/recipe/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/api/shopping_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/api/unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:43:12.821572 yes_chef-0.9.2/src/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/cli/new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:43:12.821572 yes_chef-0.9.2/src/cli/routines/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/cli/routines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/cli/routines/export_recipes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/cli/routines/plan_recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/cli/routines/recipe_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-27 07:43:02.000000 yes_chef-0.9.2/src/cli/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:43:12.821572 yes_chef-0.9.2/yes_chef.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-27 07:43:12.000000 yes_chef-0.9.2/yes_chef.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-27 07:43:12.000000 yes_chef-0.9.2/yes_chef.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 07:43:12.000000 yes_chef-0.9.2/yes_chef.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-27 07:43:12.000000 yes_chef-0.9.2/yes_chef.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-27 07:43:12.000000 yes_chef-0.9.2/yes_chef.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-27 07:43:12.000000 yes_chef-0.9.2/yes_chef.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:47:27.751280 yes_chef-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-27 07:47:27.751280 yes_chef-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-27 07:47:17.000000 yes_chef-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-27 07:47:18.000000 yes_chef-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 07:47:27.751280 yes_chef-0.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:47:27.743280 yes_chef-0.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:47:27.747280 yes_chef-0.9.3/src/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 07:47:18.000000 yes_chef-0.9.3/src/api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/ingredient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/initialise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:47:27.747280 yes_chef-0.9.3/src/api/recipe/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/recipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/recipe/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/recipe/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/recipe/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/recipe/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/shopping_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:47:27.747280 yes_chef-0.9.3/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/cli/new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:47:27.747280 yes_chef-0.9.3/src/cli/routines/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/cli/routines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/cli/routines/export_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/cli/routines/plan_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/cli/routines/recipe_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/cli/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:47:27.751280 yes_chef-0.9.3/yes_chef.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-27 07:47:27.000000 yes_chef-0.9.3/yes_chef.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-27 07:47:27.000000 yes_chef-0.9.3/yes_chef.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 07:47:27.000000 yes_chef-0.9.3/yes_chef.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-27 07:47:27.000000 yes_chef-0.9.3/yes_chef.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-27 07:47:27.000000 yes_chef-0.9.3/yes_chef.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-27 07:47:27.000000 yes_chef-0.9.3/yes_chef.egg-info/top_level.txt
```

### Comparing `yes_chef-0.9.2/PKG-INFO` & `yes_chef-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yes-chef
-Version: 0.9.2
+Version: 0.9.3
 Summary: A command-line tool for managing recipes and making shopping lists.
 Author-email: Robin Neville <robin.m.neville@gmail.com>
 Maintainer-email: Robin Neville <robin.m.neville@gmail.com>
 Project-URL: Repository, https://github.com/binnev/yes-chef
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: typer>=0.9
```

### Comparing `yes_chef-0.9.2/README.md` & `yes_chef-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.2/pyproject.toml` & `yes_chef-0.9.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "yes-chef"
 description = "A command-line tool for managing recipes and making shopping lists."
-version = "0.9.2"
+version = "0.9.3"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
     { name = "Robin Neville", email = "robin.m.neville@gmail.com" },
 ]
 maintainers = [
     { name = "Robin Neville", email = "robin.m.neville@gmail.com" },
@@ -38,15 +38,15 @@
     "mike",
 ]
 
 [project.urls]
 Repository = "https://github.com/binnev/yes-chef"
 
 [project.scripts]
-chef = "entrypoint"
+chef = "src.cli:app"
 
 [tool.setuptools.packages.find]
 include = ["src*"]
 
 [tool.pytest.ini_options]
 #addopts = "-p no:cacheprovider --cov --cov-fail-under=70 --cov-report term-missing:skip-covered"
 testpaths = ["tests"]
```

### Comparing `yes_chef-0.9.2/src/api/ingredient.py` & `yes_chef-0.9.3/src/api/ingredient.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.2/src/api/initialise.py` & `yes_chef-0.9.3/src/api/initialise.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.2/src/api/plan.py` & `yes_chef-0.9.3/src/api/plan.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.2/src/api/recipe/formats.py` & `yes_chef-0.9.3/src/api/recipe/formats.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.2/src/api/recipe/recipe.py` & `yes_chef-0.9.3/src/api/recipe/recipe.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.2/src/api/recipe/serializer.py` & `yes_chef-0.9.3/src/api/recipe/serializer.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.2/src/api/recipe/utils.py` & `yes_chef-0.9.3/src/api/recipe/utils.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.2/src/api/settings.py` & `yes_chef-0.9.3/src/api/settings.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.2/src/api/shopping_list.py` & `yes_chef-0.9.3/src/api/shopping_list.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.2/src/api/unit.py` & `yes_chef-0.9.3/src/api/unit.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.2/src/api/utils.py` & `yes_chef-0.9.3/src/api/utils.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.2/src/cli/__init__.py` & `yes_chef-0.9.3/src/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.2/src/cli/new.py` & `yes_chef-0.9.3/src/cli/new.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.2/src/cli/routines/export_recipes.py` & `yes_chef-0.9.3/src/cli/routines/export_recipes.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.2/src/cli/routines/plan_recipe.py` & `yes_chef-0.9.3/src/cli/routines/plan_recipe.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.2/src/cli/routines/recipe_wizard.py` & `yes_chef-0.9.3/src/cli/routines/recipe_wizard.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.2/src/cli/utils.py` & `yes_chef-0.9.3/src/cli/utils.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.2/src/cli/view.py` & `yes_chef-0.9.3/src/cli/view.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.2/yes_chef.egg-info/PKG-INFO` & `yes_chef-0.9.3/yes_chef.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yes-chef
-Version: 0.9.2
+Version: 0.9.3
 Summary: A command-line tool for managing recipes and making shopping lists.
 Author-email: Robin Neville <robin.m.neville@gmail.com>
 Maintainer-email: Robin Neville <robin.m.neville@gmail.com>
 Project-URL: Repository, https://github.com/binnev/yes-chef
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: typer>=0.9
```

### Comparing `yes_chef-0.9.2/yes_chef.egg-info/SOURCES.txt` & `yes_chef-0.9.3/yes_chef.egg-info/SOURCES.txt`

 * *Files identical despite different names*

