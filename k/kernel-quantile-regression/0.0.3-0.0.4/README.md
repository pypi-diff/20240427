# Comparing `tmp/kernel_quantile_regression-0.0.3.tar.gz` & `tmp/kernel_quantile_regression-0.0.4.tar.gz`

## Comparing `kernel_quantile_regression-0.0.3.tar` & `kernel_quantile_regression-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.3/src/kernel_quantile_regression/__init__.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.3/src/kernel_quantile_regression/kqr.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.3/LICENSE
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.3/README.md
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.4/src/kernel_quantile_regression/__init__.py
+-rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.4/src/kernel_quantile_regression/kqr.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.4/README.md
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 kernel_quantile_regression-0.0.4/PKG-INFO
```

### Comparing `kernel_quantile_regression-0.0.3/LICENSE` & `kernel_quantile_regression-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kernel_quantile_regression-0.0.3/pyproject.toml` & `kernel_quantile_regression-0.0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling","cvxopt","matplotlib","numpy","pandas","scipy","scikit-learn","tqdm"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "kernel_quantile_regression"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Luca Pernigo", email="luca.pernigo@usi.ch" },
 ]
 description = "Kernel quantile regression"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

