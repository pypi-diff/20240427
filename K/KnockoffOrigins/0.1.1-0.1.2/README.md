# Comparing `tmp/knockofforigins-0.1.1.tar.gz` & `tmp/knockofforigins-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knockofforigins-0.1.1.tar", max compression
+gzip compressed data, was "knockofforigins-0.1.2.tar", max compression
```

## Comparing `knockofforigins-0.1.1.tar` & `knockofforigins-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2024-04-26 20:50:14.680887 knockofforigins-0.1.1/LICENSE
--rw-r--r--   0        0        0     3669 2024-04-26 20:46:06.696480 knockofforigins-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-26 21:46:15.138438 knockofforigins-0.1.1/knockofforigins/__init__.py
--rw-r--r--   0        0        0     3555 2024-04-26 21:46:15.138438 knockofforigins-0.1.1/knockofforigins/data_gen.py
--rw-r--r--   0        0        0     2829 2024-04-26 21:46:15.138438 knockofforigins-0.1.1/knockofforigins/decompose.py
--rw-r--r--   0        0        0        0 2024-04-26 21:46:15.138438 knockofforigins-0.1.1/knockofforigins/evaluation.py
--rw-r--r--   0        0        0     1267 2024-04-26 21:46:15.138438 knockofforigins-0.1.1/knockofforigins/gram_matrix.py
--rw-r--r--   0        0        0        0 2024-04-26 21:46:15.139438 knockofforigins-0.1.1/knockofforigins/knockoff.py
--rw-r--r--   0        0        0     2659 2024-04-26 21:48:10.588247 knockofforigins-0.1.1/knockofforigins/knockoff_construct.py
--rw-r--r--   0        0        0     1499 2024-04-26 21:46:15.139438 knockofforigins-0.1.1/knockofforigins/lasso.py
--rw-r--r--   0        0        0        0 2024-04-26 21:46:15.139438 knockofforigins-0.1.1/knockofforigins/plots.py
--rw-r--r--   0        0        0        0 2024-04-26 21:46:15.139438 knockofforigins-0.1.1/knockofforigins/testatistics.py
--rw-r--r--   0        0        0        0 2024-04-26 21:46:15.139438 knockofforigins-0.1.1/knockofforigins/utils.py
--rw-r--r--   0        0        0      965 2024-04-26 22:07:04.893770 knockofforigins-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4855 1970-01-01 00:00:00.000000 knockofforigins-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-26 23:43:18.726204 knockofforigins-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5248 2024-04-26 23:43:18.726204 knockofforigins-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-26 23:43:18.726204 knockofforigins-0.1.2/knockofforigins/__init__.py
+-rw-r--r--   0        0        0     3555 2024-04-26 23:43:18.726204 knockofforigins-0.1.2/knockofforigins/data_gen.py
+-rw-r--r--   0        0        0     2829 2024-04-26 23:43:18.726204 knockofforigins-0.1.2/knockofforigins/decompose.py
+-rw-r--r--   0        0        0        0 2024-04-26 23:43:18.726204 knockofforigins-0.1.2/knockofforigins/evaluation.py
+-rw-r--r--   0        0        0     1267 2024-04-26 23:43:18.726204 knockofforigins-0.1.2/knockofforigins/gram_matrix.py
+-rw-r--r--   0        0        0        0 2024-04-26 23:43:18.726204 knockofforigins-0.1.2/knockofforigins/knockoff.py
+-rw-r--r--   0        0        0     2659 2024-04-26 23:43:18.726204 knockofforigins-0.1.2/knockofforigins/knockoff_construct.py
+-rw-r--r--   0        0        0     1499 2024-04-26 23:43:18.730204 knockofforigins-0.1.2/knockofforigins/lasso.py
+-rw-r--r--   0        0        0        0 2024-04-26 23:43:18.730204 knockofforigins-0.1.2/knockofforigins/plots.py
+-rw-r--r--   0        0        0        0 2024-04-26 23:43:18.730204 knockofforigins-0.1.2/knockofforigins/testatistics.py
+-rw-r--r--   0        0        0        0 2024-04-26 23:43:18.730204 knockofforigins-0.1.2/knockofforigins/utils.py
+-rw-r--r--   0        0        0      965 2024-04-26 23:43:18.730204 knockofforigins-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6485 1970-01-01 00:00:00.000000 knockofforigins-0.1.2/PKG-INFO
```

### Comparing `knockofforigins-0.1.1/LICENSE` & `knockofforigins-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `knockofforigins-0.1.1/knockofforigins/data_gen.py` & `knockofforigins-0.1.2/knockofforigins/data_gen.py`

 * *Files identical despite different names*

### Comparing `knockofforigins-0.1.1/knockofforigins/decompose.py` & `knockofforigins-0.1.2/knockofforigins/decompose.py`

 * *Files identical despite different names*

### Comparing `knockofforigins-0.1.1/knockofforigins/gram_matrix.py` & `knockofforigins-0.1.2/knockofforigins/gram_matrix.py`

 * *Files identical despite different names*

### Comparing `knockofforigins-0.1.1/knockofforigins/knockoff_construct.py` & `knockofforigins-0.1.2/knockofforigins/knockoff_construct.py`

 * *Files identical despite different names*

### Comparing `knockofforigins-0.1.1/knockofforigins/lasso.py` & `knockofforigins-0.1.2/knockofforigins/lasso.py`

 * *Files identical despite different names*

### Comparing `knockofforigins-0.1.1/pyproject.toml` & `knockofforigins-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "KnockoffOrigins"
-version = "0.1.1"
+version = "0.1.2"
 description = "This repository is dedicated to implementing the methodologies from the 2015 paper \"False Discovery Rate via Knockoffs\". It provides code for generating knockoff features and applying selection procedures. The aim is to help users understand and apply the knockoff method for feature selection. Please refer to the original paper for a complete understanding."
 authors = ["Javad Razi <j.razi@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jrazi/KnockoffOrigins"
 
 [tool.poetry.dependencies]
```

### Comparing `knockofforigins-0.1.1/PKG-INFO` & `knockofforigins-0.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,12 @@
-Metadata-Version: 2.1
-Name: knockofforigins
-Version: 0.1.1
-Summary: This repository is dedicated to implementing the methodologies from the 2015 paper "False Discovery Rate via Knockoffs". It provides code for generating knockoff features and applying selection procedures. The aim is to help users understand and apply the knockoff method for feature selection. Please refer to the original paper for a complete understanding.
-Home-page: https://github.com/jrazi/KnockoffOrigins
-License: MIT
-Author: Javad Razi
-Author-email: j.razi@outlook.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
-Requires-Dist: pandas (>=2.2.2,<3.0.0)
-Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
-Requires-Dist: scipy (>=1.13.0,<2.0.0)
-Requires-Dist: seaborn (>=0.13.2,<0.14.0)
-Requires-Dist: statsmodels (>=0.14.2,<0.15.0)
-Project-URL: Repository, https://github.com/jrazi/KnockoffOrigins
-Description-Content-Type: text/markdown
-
 # 🔍 KnockoffOrigins: An Implementation of "CONTROLLING THE FALSE DISCOVERY RATE VIA KNOCKOFFS (2015)"
 
+[![Python package](https://github.com/jrazi/KnockoffOrigins/actions/workflows/python-package.yml/badge.svg?event=registry_package)](https://github.com/jrazi/KnockoffOrigins/actions/workflows/python-package.yml)
+
+
 This repository hosts the implementation of the knockoff filter method for controlled variable selection, based on the "Controlling the False Discovery Rate via Knockoffs" paper from 2015. The method is designed for high-dimensional data settings to effectively control the false discovery rate while preserving statistical power.
 
 **Note:** Much of this implementation was crafted either from scratch or without relying on high-level libraries. This approach was chosen primarily for educational purposes (mostly _self-educational_ purposes), allowing for a deeper understanding and exploration of the underlying algorithms. While this method involves some "reinventing the wheel," it might have some educational value. Future development may include the integration of more specialized libraries to enhance functionality and performance.
 
 ## Table of Content
 
 - [🔍 KnockoffOrigins: An Implementation of "CONTROLLING THE FALSE DISCOVERY RATE VIA KNOCKOFFS (2015)"](#-knockofforigins-an-implementation-of-controlling-the-false-discovery-rate-via-knockoffs-2015)
@@ -86,24 +66,66 @@
 git clone https://github.com/jrazi/KnockoffOrigins.git
 cd KnockoffOrigins
 poetry install
 ```
 
 ## Usage
 
-Here is a quick example of how to generate data and apply the knockoff filter:
+### Generating Knockoff Features
+
+To generate knockoff features based on your original data, you can use the `generate_knockoff_features` function from the `knockofforigins.knockoff_construct` module.
+
+```python
+import numpy as np
+from knockofforigins.knockoff_construct import generate_knockoff_features, choose_s_vector
+
+# Load your original feature matrix X (n x p)
+# ...
+
+# Choose the s vector for knockoff construction
+s = choose_s_vector(np.cov(X.T))
+
+# Generate knockoff features
+X_knockoff = generate_knockoff_features(X, s)
+```
+
+### Feature Selection with Lasso
+
+After generating knockoff features, you can perform feature selection using the Lasso regression model with the augmented design matrix (original and knockoff features concatenated).
 
 ```python
-from KnockOffOrigins.data_gen import SyntheticDataGenerator, GWASDataGenerator
+from knockofforigins.lasso import compute_feature_importance
+
+# Load your response vector y (n x 1)
+# ...
 
-# Initialize the data generator
-base_generator = SyntheticDataGenerator(n=10000, p=100, noise_variance=1.0)
+# Compute feature importance statistic W
+alpha = 0.1  # Regularization parameter for Lasso
+W = compute_feature_importance(X, X_knockoff, y, alpha)
 
-# Generate data and apply the knockoff filter
-X, y = base_generator.generate_data()
+# Select features based on W
+selected_features = np.argsort(-W)[:num_features_to_select]
+```
+
+### Generating Synthetic GWAS Data
+
+If you need to generate synthetic GWAS data for testing purposes, you can use the InfluentialFeatureGWASDataGenerator class.
+
+```python
+from KnockoffOrigins.knockoff_construct import generate_knockoff_features, choose_s_vector
+from KnockoffOrigins.gram_matrix import generate_gram_matrix
+
+# Calculate the covariance matrix Sigma of the original features X
+Sigma = generate_gram_matrix(X)
+
+# Choose the vector 's' for knockoff feature generation
+s = choose_s_vector(Sigma)
+
+# Generate knockoff features using the original features X
+X_knockoff = generate_knockoff_features(X, s)
 ```
 
 ## Contributing
 
 Contributions are welcome, and appreciated!
 
 ## License
@@ -116,8 +138,7 @@
 - [ ] Develop FDR control mechanisms as outlined in the original study.
 - [ ] Implement Lasso feature selection using lower-level libraries.
 - [ ] Address some of the bugs and implementation issues.
 - [ ] Create example notebooks demonstrating package usage.
 - [ ] Replicate experiments from the original 2015 knockoff paper.
 - [ ] Develop visualization methods for feature selection analysis.
 - [ ] Implement the KnockOff+ method for enhanced feature selection.
-
```

