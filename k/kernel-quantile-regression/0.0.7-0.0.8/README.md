# Comparing `tmp/kernel_quantile_regression-0.0.7.tar.gz` & `tmp/kernel_quantile_regression-0.0.8.tar.gz`

## Comparing `kernel_quantile_regression-0.0.7.tar` & `kernel_quantile_regression-0.0.8.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.7/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.7/LICENSE
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.7/README.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.8/krn/__init__.py
+-rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.8/krn/kqr.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.8/README.md
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.8/PKG-INFO
```

### Comparing `kernel_quantile_regression-0.0.7/LICENSE` & `kernel_quantile_regression-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kernel_quantile_regression-0.0.7/README.md` & `kernel_quantile_regression-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `kernel_quantile_regression-0.0.7/pyproject.toml` & `kernel_quantile_regression-0.0.8/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["hatchling","cvxopt","matplotlib","numpy","pandas","scipy","scikit-learn","tqdm"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "kernel_quantile_regression"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Luca Pernigo", email="luca.pernigo@usi.ch" },
 ]
 description = "Kernel quantile regression"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.hatch.build]
-include = ['kernel_quantile_regression/*']
+include = ['krn/*']
 
 
 [project.urls]
 Homepage = "https://github.com/luca-pernigo/kernel_quantile_regression"
```

### Comparing `kernel_quantile_regression-0.0.7/PKG-INFO` & `kernel_quantile_regression-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kernel_quantile_regression
-Version: 0.0.7
+Version: 0.0.8
 Summary: Kernel quantile regression
 Project-URL: Homepage, https://github.com/luca-pernigo/kernel_quantile_regression
 Author-email: Luca Pernigo <luca.pernigo@usi.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

