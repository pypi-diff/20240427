# Comparing `tmp/ffit-0.0.1.tar.gz` & `tmp/ffit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffit-0.0.1.tar", last modified: Wed Mar 27 13:07:56 2024, max compression
+gzip compressed data, was "ffit-0.1.0.tar", last modified: Sat Apr 27 19:08:00 2024, max compression
```

## Comparing `ffit-0.0.1.tar` & `ffit-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:07:56.645480 ffit-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-03-27 13:07:44.000000 ffit-0.0.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-27 13:07:44.000000 ffit-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-27 13:07:56.645480 ffit-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-27 13:07:44.000000 ffit-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:07:56.641480 ffit-0.0.1/ffit/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-27 13:07:44.000000 ffit-0.0.1/ffit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-27 13:07:44.000000 ffit-0.0.1/ffit/fit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:07:56.641480 ffit-0.0.1/ffit/funcs/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-27 13:07:44.000000 ffit-0.0.1/ffit/funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-27 13:07:44.000000 ffit-0.0.1/ffit/funcs/lorentzianFunc.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-27 13:07:44.000000 ffit-0.0.1/ffit/funcs/polyFunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-03-27 13:07:44.000000 ffit-0.0.1/ffit/funcs/sinFunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-03-27 13:07:44.000000 ffit-0.0.1/ffit/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:07:56.641480 ffit-0.0.1/ffit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-27 13:07:56.000000 ffit-0.0.1/ffit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-27 13:07:56.000000 ffit-0.0.1/ffit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 13:07:56.000000 ffit-0.0.1/ffit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-27 13:07:56.000000 ffit-0.0.1/ffit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-27 13:07:56.000000 ffit-0.0.1/ffit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-27 13:07:44.000000 ffit-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 13:07:56.645480 ffit-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-27 13:07:44.000000 ffit-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:07:56.641480 ffit-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-27 13:07:44.000000 ffit-0.0.1/tests/test_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:08:00.887256 ffit-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-04-27 19:07:52.000000 ffit-0.1.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-27 19:07:52.000000 ffit-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-27 19:08:00.887256 ffit-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 19:07:52.000000 ffit-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:08:00.879257 ffit-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-27 19:07:52.000000 ffit-0.1.0/docs/about.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:08:00.879257 ffit-0.1.0/docs/develop/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-27 19:07:52.000000 ffit-0.1.0/docs/develop/custom_function.md
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-27 19:07:52.000000 ffit-0.1.0/docs/develop/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-27 19:07:52.000000 ffit-0.1.0/docs/fit_result.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:08:00.879257 ffit-0.1.0/docs/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-27 19:07:52.000000 ffit-0.1.0/docs/functions/cos.md
+-rw-r--r--   0 runner    (1001) docker     (127)    74982 2024-04-27 19:07:52.000000 ffit-0.1.0/docs/functions/create_images.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-27 19:07:52.000000 ffit-0.1.0/docs/functions/exp.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-27 19:07:52.000000 ffit-0.1.0/docs/functions/hyperbola.md
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-27 19:07:52.000000 ffit-0.1.0/docs/functions/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-27 19:07:52.000000 ffit-0.1.0/docs/functions/line.md
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-27 19:07:52.000000 ffit-0.1.0/docs/functions/log.md
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-27 19:07:52.000000 ffit-0.1.0/docs/functions/lorentzian.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-27 19:07:52.000000 ffit-0.1.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:08:00.879257 ffit-0.1.0/docs/releases/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-27 19:07:52.000000 ffit-0.1.0/docs/releases/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:08:00.879257 ffit-0.1.0/docs/starting_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-27 19:07:52.000000 ffit-0.1.0/docs/starting_guide/first_steps.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-27 19:07:52.000000 ffit-0.1.0/docs/starting_guide/install.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:08:00.883257 ffit-0.1.0/ffit/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/__config__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:08:00.883257 ffit-0.1.0/ffit/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/backends/jax_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/backends/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/backends/scipy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8957 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/fit_logic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/fit_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/fit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/front.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:08:00.887256 ffit-0.1.0/ffit/funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/funcs/complex_spiral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/funcs/func_cos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/funcs/func_exp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/funcs/func_hyperbola.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/funcs/func_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/funcs/func_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/funcs/func_lorentzian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/funcs/func_lorentzian_complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/funcs/func_polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-04-27 19:07:52.000000 ffit-0.1.0/ffit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 19:08:00.887256 ffit-0.1.0/ffit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-27 19:08:00.000000 ffit-0.1.0/ffit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-27 19:08:00.000000 ffit-0.1.0/ffit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 19:08:00.000000 ffit-0.1.0/ffit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 19:08:00.000000 ffit-0.1.0/ffit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-27 19:08:00.000000 ffit-0.1.0/ffit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-27 19:07:52.000000 ffit-0.1.0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 19:07:52.000000 ffit-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 19:08:00.887256 ffit-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-27 19:07:52.000000 ffit-0.1.0/setup.py
```

### Comparing `ffit-0.0.1/LICENCE` & `ffit-0.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ffit-0.0.1/setup.py` & `ffit-0.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 import setuptools
 
+NAME = "ffit"
+AUTHOR = "kyrylo.gr"
+AUTHOR_EMAIL = "git@kyrylo.gr"
+DESCRIPTION = "FastFit python library"
+
+
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+
+def get_version() -> str:
+    with open(f"{NAME}/__config__.py", "r", encoding="utf-8") as file:
+        for line in file.readlines():
+            if line.startswith("__version__"):
+                return line.split("=")[1].strip().strip('"').strip("'")
+    raise ValueError("Version not found")
+
+
 setuptools.setup(
-    name="ffit",
-    version="0.0.1",
-    author="kyrylo.gr",
-    author_email="git@kyrylo.gr",
-    description="FastFit python library",
+    name=NAME,
+    version=get_version(),
+    author=AUTHOR,
+    author_email=AUTHOR_EMAIL,
+    description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/kyrylo-gr/ffit",
-    packages=setuptools.find_packages(exclude=["tests", "tests.*"]),
+    url=f"https://github.com/kyrylo-gr/{NAME}",
+    packages=setuptools.find_packages(exclude=["tests", "tests.*", "docs", "docs.*"]),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.8",
-    install_requires=[
-        "numpy",
-    ],
+    install_requires=["numpy", "scipy"],
 )
```

