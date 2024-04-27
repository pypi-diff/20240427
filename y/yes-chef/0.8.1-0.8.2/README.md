# Comparing `tmp/yes-chef-0.8.1.tar.gz` & `tmp/yes_chef-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yes-chef-0.8.1.tar", last modified: Wed Apr  3 18:27:23 2024, max compression
+gzip compressed data, was "yes_chef-0.8.2.tar", last modified: Sat Apr 27 07:17:35 2024, max compression
```

## Comparing `yes-chef-0.8.1.tar` & `yes_chef-0.8.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:27:23.024263 yes-chef-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-03 18:27:23.024263 yes-chef-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-03 18:27:12.000000 yes-chef-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-03 18:27:12.000000 yes-chef-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:27:23.024263 yes-chef-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:27:23.020263 yes-chef-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:27:23.020263 yes-chef-0.8.1/src/api/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/api/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/api/ingredient.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/api/initialise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/api/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:27:23.020263 yes-chef-0.8.1/src/api/recipe/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/api/recipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/api/recipe/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/api/recipe/recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/api/recipe/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/api/recipe/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/api/shopping_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/api/unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:27:23.024263 yes-chef-0.8.1/src/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/cli/new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:27:23.024263 yes-chef-0.8.1/src/cli/routines/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/cli/routines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/cli/routines/export_recipes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/cli/routines/plan_recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/cli/routines/recipe_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-03 18:27:12.000000 yes-chef-0.8.1/src/cli/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:27:23.024263 yes-chef-0.8.1/yes_chef.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-03 18:27:23.000000 yes-chef-0.8.1/yes_chef.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-03 18:27:23.000000 yes-chef-0.8.1/yes_chef.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:27:23.000000 yes-chef-0.8.1/yes_chef.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-03 18:27:23.000000 yes-chef-0.8.1/yes_chef.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 18:27:23.000000 yes-chef-0.8.1/yes_chef.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:17:35.899663 yes_chef-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-27 07:17:35.899663 yes_chef-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-27 07:17:23.000000 yes_chef-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-27 07:17:24.000000 yes_chef-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 07:17:35.899663 yes_chef-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:17:35.891663 yes_chef-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:17:35.895663 yes_chef-0.8.2/src/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 07:17:24.000000 yes_chef-0.8.2/src/api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/api/ingredient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/api/initialise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/api/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:17:35.895663 yes_chef-0.8.2/src/api/recipe/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/api/recipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/api/recipe/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/api/recipe/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/api/recipe/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/api/recipe/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/api/shopping_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/api/unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:17:35.895663 yes_chef-0.8.2/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/cli/new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:17:35.895663 yes_chef-0.8.2/src/cli/routines/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/cli/routines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/cli/routines/export_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/cli/routines/plan_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/cli/routines/recipe_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-27 07:17:23.000000 yes_chef-0.8.2/src/cli/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 07:17:35.899663 yes_chef-0.8.2/yes_chef.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-27 07:17:35.000000 yes_chef-0.8.2/yes_chef.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-27 07:17:35.000000 yes_chef-0.8.2/yes_chef.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 07:17:35.000000 yes_chef-0.8.2/yes_chef.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-27 07:17:35.000000 yes_chef-0.8.2/yes_chef.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-27 07:17:35.000000 yes_chef-0.8.2/yes_chef.egg-info/top_level.txt
```

### Comparing `yes-chef-0.8.1/PKG-INFO` & `yes_chef-0.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yes-chef
-Version: 0.8.1
+Version: 0.8.2
 Summary: A command-line tool for managing recipes and making shopping lists.
 Author-email: Robin Neville <robin.m.neville@gmail.com>
 Maintainer-email: Robin Neville <robin.m.neville@gmail.com>
 Project-URL: Repository, https://github.com/binnev/yes-chef
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: typer>=0.9
```

### Comparing `yes-chef-0.8.1/README.md` & `yes_chef-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `yes-chef-0.8.1/pyproject.toml` & `yes_chef-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "yes-chef"
 description = "A command-line tool for managing recipes and making shopping lists."
-version = "0.8.1"
+version = "0.8.2"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
     { name = "Robin Neville", email = "robin.m.neville@gmail.com" },
 ]
 maintainers = [
     { name = "Robin Neville", email = "robin.m.neville@gmail.com" },
```

### Comparing `yes-chef-0.8.1/src/api/ingredient.py` & `yes_chef-0.8.2/src/api/ingredient.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.8.1/src/api/initialise.py` & `yes_chef-0.8.2/src/api/initialise.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.8.1/src/api/plan.py` & `yes_chef-0.8.2/src/api/plan.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.8.1/src/api/recipe/formats.py` & `yes_chef-0.8.2/src/api/recipe/formats.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.8.1/src/api/recipe/recipe.py` & `yes_chef-0.8.2/src/api/recipe/recipe.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.8.1/src/api/recipe/serializer.py` & `yes_chef-0.8.2/src/api/recipe/serializer.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.8.1/src/api/recipe/utils.py` & `yes_chef-0.8.2/src/api/recipe/utils.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.8.1/src/api/settings.py` & `yes_chef-0.8.2/src/api/settings.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.8.1/src/api/shopping_list.py` & `yes_chef-0.8.2/src/api/shopping_list.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.8.1/src/api/unit.py` & `yes_chef-0.8.2/src/api/unit.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.8.1/src/api/utils.py` & `yes_chef-0.8.2/src/api/utils.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.8.1/src/cli/__init__.py` & `yes_chef-0.8.2/src/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.8.1/src/cli/new.py` & `yes_chef-0.8.2/src/cli/new.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.8.1/src/cli/routines/export_recipes.py` & `yes_chef-0.8.2/src/cli/routines/export_recipes.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.8.1/src/cli/routines/plan_recipe.py` & `yes_chef-0.8.2/src/cli/routines/plan_recipe.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.8.1/src/cli/routines/recipe_wizard.py` & `yes_chef-0.8.2/src/cli/routines/recipe_wizard.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     if expected_type != str:
         s += f" ({expected_type.__name__})"
     if default is not NOT_SET:
         s += f" [{default}]"
     s += ": "
 
     while True:
-        raw = input(s)
+        raw = input(s).strip()
         if not raw:
             if default is NOT_SET:
                 return expected_type()
             else:
                 return default
 
         try:
```

### Comparing `yes-chef-0.8.1/src/cli/utils.py` & `yes_chef-0.8.2/src/cli/utils.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.8.1/src/cli/view.py` & `yes_chef-0.8.2/src/cli/view.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.8.1/yes_chef.egg-info/PKG-INFO` & `yes_chef-0.8.2/yes_chef.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yes-chef
-Version: 0.8.1
+Version: 0.8.2
 Summary: A command-line tool for managing recipes and making shopping lists.
 Author-email: Robin Neville <robin.m.neville@gmail.com>
 Maintainer-email: Robin Neville <robin.m.neville@gmail.com>
 Project-URL: Repository, https://github.com/binnev/yes-chef
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: typer>=0.9
```

### Comparing `yes-chef-0.8.1/yes_chef.egg-info/SOURCES.txt` & `yes_chef-0.8.2/yes_chef.egg-info/SOURCES.txt`

 * *Files identical despite different names*

