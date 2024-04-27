# Comparing `tmp/yes_chef-0.9.3.tar.gz` & `tmp/yes_chef-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yes_chef-0.9.3.tar", last modified: Sat Apr 27 07:47:27 2024, max compression
+gzip compressed data, was "yes_chef-0.9.4.tar", last modified: Sat Apr 27 07:53:52 2024, max compression
```

## Comparing `yes_chef-0.9.3.tar` & `yes_chef-0.9.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:47:27.751280 yes_chef-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-27 07:47:27.751280 yes_chef-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-27 07:47:17.000000 yes_chef-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-27 07:47:18.000000 yes_chef-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 07:47:27.751280 yes_chef-0.9.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:47:27.743280 yes_chef-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:47:27.747280 yes_chef-0.9.3/src/api/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 07:47:18.000000 yes_chef-0.9.3/src/api/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/ingredient.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/initialise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:47:27.747280 yes_chef-0.9.3/src/api/recipe/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/recipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/recipe/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/recipe/recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/recipe/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/recipe/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/shopping_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:47:27.747280 yes_chef-0.9.3/src/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/cli/new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:47:27.747280 yes_chef-0.9.3/src/cli/routines/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/cli/routines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/cli/routines/export_recipes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/cli/routines/plan_recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/cli/routines/recipe_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-27 07:47:17.000000 yes_chef-0.9.3/src/cli/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:47:27.751280 yes_chef-0.9.3/yes_chef.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-27 07:47:27.000000 yes_chef-0.9.3/yes_chef.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-27 07:47:27.000000 yes_chef-0.9.3/yes_chef.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 07:47:27.000000 yes_chef-0.9.3/yes_chef.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-27 07:47:27.000000 yes_chef-0.9.3/yes_chef.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-27 07:47:27.000000 yes_chef-0.9.3/yes_chef.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-27 07:47:27.000000 yes_chef-0.9.3/yes_chef.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:53:52.796241 yes_chef-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-27 07:53:52.796241 yes_chef-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-27 07:53:40.000000 yes_chef-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-27 07:53:41.000000 yes_chef-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 07:53:52.796241 yes_chef-0.9.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:53:52.788241 yes_chef-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:53:52.788241 yes_chef-0.9.4/src/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 07:53:41.000000 yes_chef-0.9.4/src/api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/api/ingredient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/api/initialise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/api/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:53:52.792241 yes_chef-0.9.4/src/api/recipe/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/api/recipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/api/recipe/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/api/recipe/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/api/recipe/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/api/recipe/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/api/shopping_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/api/unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:53:52.792241 yes_chef-0.9.4/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/cli/new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:53:52.792241 yes_chef-0.9.4/src/cli/routines/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/cli/routines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/cli/routines/export_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/cli/routines/plan_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/cli/routines/recipe_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-27 07:53:40.000000 yes_chef-0.9.4/src/cli/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:53:52.792241 yes_chef-0.9.4/yes_chef.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-27 07:53:52.000000 yes_chef-0.9.4/yes_chef.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-27 07:53:52.000000 yes_chef-0.9.4/yes_chef.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 07:53:52.000000 yes_chef-0.9.4/yes_chef.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-27 07:53:52.000000 yes_chef-0.9.4/yes_chef.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-27 07:53:52.000000 yes_chef-0.9.4/yes_chef.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-27 07:53:52.000000 yes_chef-0.9.4/yes_chef.egg-info/top_level.txt
```

### Comparing `yes_chef-0.9.3/PKG-INFO` & `yes_chef-0.9.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: yes-chef
-Version: 0.9.3
+Version: 0.9.4
 Summary: A command-line tool for managing recipes and making shopping lists.
 Author-email: Robin Neville <robin.m.neville@gmail.com>
 Maintainer-email: Robin Neville <robin.m.neville@gmail.com>
 Project-URL: Repository, https://github.com/binnev/yes-chef
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: typer>=0.9
 Requires-Dist: colorama>=0.4
 Requires-Dist: rich>=13.7
 Requires-Dist: shellingham>=1.5
 Requires-Dist: pydantic>=2.6
 Requires-Dist: pydantic-settings>=2.2
 Requires-Dist: aiofiles>=23.2
 Requires-Dist: inquirer>=3.2
+Requires-Dist: pyyaml>=6.0.1
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: responses; extra == "dev"
 Requires-Dist: pyinstaller; extra == "dev"
```

### Comparing `yes_chef-0.9.3/README.md` & `yes_chef-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.3/pyproject.toml` & `yes_chef-0.9.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "yes-chef"
 description = "A command-line tool for managing recipes and making shopping lists."
-version = "0.9.3"
+version = "0.9.4"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
     { name = "Robin Neville", email = "robin.m.neville@gmail.com" },
 ]
 maintainers = [
     { name = "Robin Neville", email = "robin.m.neville@gmail.com" },
@@ -17,14 +17,15 @@
     "colorama>=0.4",
     "rich>=13.7",
     "shellingham>=1.5",
     "pydantic>=2.6",
     "pydantic-settings>=2.2",
     "aiofiles>=23.2",
     "inquirer>=3.2",
+    "pyyaml>=6.0.1",
 ]
 
 [project.optional-dependencies]
 dev = [
     "ruff",
     "pytest",
     "pytest-asyncio",
@@ -44,23 +45,22 @@
 [project.scripts]
 chef = "src.cli:app"
 
 [tool.setuptools.packages.find]
 include = ["src*"]
 
 [tool.pytest.ini_options]
-#addopts = "-p no:cacheprovider --cov --cov-fail-under=70 --cov-report term-missing:skip-covered"
+addopts = "-p no:cacheprovider --cov --cov-fail-under=70 --cov-report term-missing:skip-covered"
 testpaths = ["tests"]
 markers = [
     "allow_settings_save: by default, Settings.save is mocked, so we don't create real files when running tests.",
     "allow_settings_load: ditto",
     "allow_path_mkdir",
     "allow_path_touch",
     "allow_path_glob",
-
 ]
 
 [tool.coverage.run]
 omit = ["*/__init__.py"]
 
 
 [tool.ruff]
```

### Comparing `yes_chef-0.9.3/src/api/ingredient.py` & `yes_chef-0.9.4/src/api/ingredient.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.3/src/api/initialise.py` & `yes_chef-0.9.4/src/api/initialise.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.3/src/api/plan.py` & `yes_chef-0.9.4/src/api/plan.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.3/src/api/recipe/formats.py` & `yes_chef-0.9.4/src/api/recipe/formats.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.3/src/api/recipe/recipe.py` & `yes_chef-0.9.4/src/api/recipe/recipe.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.3/src/api/recipe/serializer.py` & `yes_chef-0.9.4/src/api/recipe/serializer.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.3/src/api/recipe/utils.py` & `yes_chef-0.9.4/src/api/recipe/utils.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.3/src/api/settings.py` & `yes_chef-0.9.4/src/api/settings.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.3/src/api/shopping_list.py` & `yes_chef-0.9.4/src/api/shopping_list.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.3/src/api/unit.py` & `yes_chef-0.9.4/src/api/unit.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.3/src/api/utils.py` & `yes_chef-0.9.4/src/api/utils.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.3/src/cli/__init__.py` & `yes_chef-0.9.4/src/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.3/src/cli/new.py` & `yes_chef-0.9.4/src/cli/new.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.3/src/cli/routines/export_recipes.py` & `yes_chef-0.9.4/src/cli/routines/export_recipes.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.3/src/cli/routines/plan_recipe.py` & `yes_chef-0.9.4/src/cli/routines/plan_recipe.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.3/src/cli/routines/recipe_wizard.py` & `yes_chef-0.9.4/src/cli/routines/recipe_wizard.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.3/src/cli/utils.py` & `yes_chef-0.9.4/src/cli/utils.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.3/src/cli/view.py` & `yes_chef-0.9.4/src/cli/view.py`

 * *Files identical despite different names*

### Comparing `yes_chef-0.9.3/yes_chef.egg-info/PKG-INFO` & `yes_chef-0.9.4/yes_chef.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: yes-chef
-Version: 0.9.3
+Version: 0.9.4
 Summary: A command-line tool for managing recipes and making shopping lists.
 Author-email: Robin Neville <robin.m.neville@gmail.com>
 Maintainer-email: Robin Neville <robin.m.neville@gmail.com>
 Project-URL: Repository, https://github.com/binnev/yes-chef
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: typer>=0.9
 Requires-Dist: colorama>=0.4
 Requires-Dist: rich>=13.7
 Requires-Dist: shellingham>=1.5
 Requires-Dist: pydantic>=2.6
 Requires-Dist: pydantic-settings>=2.2
 Requires-Dist: aiofiles>=23.2
 Requires-Dist: inquirer>=3.2
+Requires-Dist: pyyaml>=6.0.1
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: responses; extra == "dev"
 Requires-Dist: pyinstaller; extra == "dev"
```

### Comparing `yes_chef-0.9.3/yes_chef.egg-info/SOURCES.txt` & `yes_chef-0.9.4/yes_chef.egg-info/SOURCES.txt`

 * *Files identical despite different names*

