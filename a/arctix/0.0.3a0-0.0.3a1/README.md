# Comparing `tmp/arctix-0.0.3a0.tar.gz` & `tmp/arctix-0.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arctix-0.0.3a0.tar", max compression
+gzip compressed data, was "arctix-0.0.3a1.tar", max compression
```

## Comparing `arctix-0.0.3a0.tar` & `arctix-0.0.3a1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1501 2024-04-27 06:38:39.118699 arctix-0.0.3a0/LICENSE
--rw-r--r--   0        0        0     4493 2024-04-27 06:38:39.118699 arctix-0.0.3a0/README.md
--rw-r--r--   0        0        0     6569 2024-04-27 06:38:39.122699 arctix-0.0.3a0/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/__init__.py
--rw-r--r--   0        0        0       43 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/dataset/__init__.py
--rw-r--r--   0        0        0    16839 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/dataset/breakfast.py
--rw-r--r--   0        0        0    22011 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/dataset/multithumos.py
--rw-r--r--   0        0        0      247 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/testing/__init__.py
--rw-r--r--   0        0        0      538 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/testing/fixtures.py
--rw-r--r--   0        0        0       29 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/__init__.py
--rw-r--r--   0        0        0     2165 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/dataframe/__init__.py
--rw-r--r--   0        0        0     6978 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/dataframe/base.py
--rw-r--r--   0        0        0     3265 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/dataframe/casting.py
--rw-r--r--   0        0        0     2107 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/dataframe/function.py
--rw-r--r--   0        0        0     2914 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/dataframe/replace.py
--rw-r--r--   0        0        0     3809 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/dataframe/sequential.py
--rw-r--r--   0        0        0     2413 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/dataframe/sorting.py
--rw-r--r--   0        0        0     3185 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/dataframe/string.py
--rw-r--r--   0        0        0     4581 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/dataframe/vocab.py
--rw-r--r--   0        0        0       34 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/__init__.py
--rw-r--r--   0        0        0      276 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/dataframe/__init__.py
--rw-r--r--   0        0        0     1618 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/dataframe/removing.py
--rw-r--r--   0        0        0     1618 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/dataframe/vocab.py
--rw-r--r--   0        0        0     3334 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/download.py
--rw-r--r--   0        0        0     7145 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/imports.py
--rw-r--r--   0        0        0      190 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/iter/__init__.py
--rw-r--r--   0        0        0     3543 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/iter/path.py
--rw-r--r--   0        0        0     1324 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/mapping.py
--rw-r--r--   0        0        0     3234 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/masking.py
--rw-r--r--   0        0        0    12749 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/vocab.py
--rw-r--r--   0        0        0     5798 1970-01-01 00:00:00.000000 arctix-0.0.3a0/PKG-INFO
+-rw-r--r--   0        0        0     1501 2024-04-27 06:41:51.236513 arctix-0.0.3a1/LICENSE
+-rw-r--r--   0        0        0     4493 2024-04-27 06:41:51.236513 arctix-0.0.3a1/README.md
+-rw-r--r--   0        0        0     6569 2024-04-27 06:41:51.240513 arctix-0.0.3a1/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/dataset/__init__.py
+-rw-r--r--   0        0        0    16839 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/dataset/breakfast.py
+-rw-r--r--   0        0        0    22011 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/dataset/multithumos.py
+-rw-r--r--   0        0        0      247 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/testing/__init__.py
+-rw-r--r--   0        0        0      538 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/testing/fixtures.py
+-rw-r--r--   0        0        0       29 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/__init__.py
+-rw-r--r--   0        0        0     2165 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/dataframe/__init__.py
+-rw-r--r--   0        0        0     6978 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/dataframe/base.py
+-rw-r--r--   0        0        0     3265 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/dataframe/casting.py
+-rw-r--r--   0        0        0     2107 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/dataframe/function.py
+-rw-r--r--   0        0        0     2914 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/dataframe/replace.py
+-rw-r--r--   0        0        0     3809 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/dataframe/sequential.py
+-rw-r--r--   0        0        0     2413 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/dataframe/sorting.py
+-rw-r--r--   0        0        0     3185 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/dataframe/string.py
+-rw-r--r--   0        0        0     4581 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/transformer/dataframe/vocab.py
+-rw-r--r--   0        0        0       34 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/__init__.py
+-rw-r--r--   0        0        0      276 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/dataframe/__init__.py
+-rw-r--r--   0        0        0     1618 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/dataframe/removing.py
+-rw-r--r--   0        0        0     1618 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/dataframe/vocab.py
+-rw-r--r--   0        0        0     3334 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/download.py
+-rw-r--r--   0        0        0     7145 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/imports.py
+-rw-r--r--   0        0        0      190 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/iter/__init__.py
+-rw-r--r--   0        0        0     3543 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/iter/path.py
+-rw-r--r--   0        0        0     1324 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/mapping.py
+-rw-r--r--   0        0        0     3234 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/masking.py
+-rw-r--r--   0        0        0    12749 2024-04-27 06:41:51.240513 arctix-0.0.3a1/src/arctix/utils/vocab.py
+-rw-r--r--   0        0        0     5798 1970-01-01 00:00:00.000000 arctix-0.0.3a1/PKG-INFO
```

### Comparing `arctix-0.0.3a0/LICENSE` & `arctix-0.0.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/README.md` & `arctix-0.0.3a1/README.md`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/pyproject.toml` & `arctix-0.0.3a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arctix"
-version = "0.0.3a0"
+version = "0.0.3a1"
 description = ""
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/arctix"
 repository = "https://github.com/durandtibo/arctix"
 keywords = []
 license = "BSD-3-Clause"
@@ -27,15 +27,15 @@
 ]
 
 [tool.poetry.dependencies]
 # Core dependencies
 batcharray = ">=0.0.2,<0.1"
 coola = ">=0.6,<1.0"
 iden = ">=0.0.3,<1.0"
-numpy = ">=1.21,<2.0"
+numpy = ">=1.22,<2.0"
 polars = ">=0.20.0,<1.0"
 python = ">=3.9,<3.13"
 
 # Optional dependencies
 gdown = { version = ">=5.0,<6.0", optional = true }
 matplotlib = { version = ">=3.6,<4.0", optional = true }
 requests = { version = ">=2.20,<3.0", optional = true }
```

### Comparing `arctix-0.0.3a0/src/arctix/dataset/breakfast.py` & `arctix-0.0.3a1/src/arctix/dataset/breakfast.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/src/arctix/dataset/multithumos.py` & `arctix-0.0.3a1/src/arctix/dataset/multithumos.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/src/arctix/testing/fixtures.py` & `arctix-0.0.3a1/src/arctix/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/src/arctix/transformer/dataframe/__init__.py` & `arctix-0.0.3a1/src/arctix/transformer/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/src/arctix/transformer/dataframe/base.py` & `arctix-0.0.3a1/src/arctix/transformer/dataframe/base.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/src/arctix/transformer/dataframe/casting.py` & `arctix-0.0.3a1/src/arctix/transformer/dataframe/casting.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/src/arctix/transformer/dataframe/function.py` & `arctix-0.0.3a1/src/arctix/transformer/dataframe/function.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/src/arctix/transformer/dataframe/replace.py` & `arctix-0.0.3a1/src/arctix/transformer/dataframe/replace.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/src/arctix/transformer/dataframe/sequential.py` & `arctix-0.0.3a1/src/arctix/transformer/dataframe/sequential.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/src/arctix/transformer/dataframe/sorting.py` & `arctix-0.0.3a1/src/arctix/transformer/dataframe/sorting.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/src/arctix/transformer/dataframe/string.py` & `arctix-0.0.3a1/src/arctix/transformer/dataframe/string.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/src/arctix/transformer/dataframe/vocab.py` & `arctix-0.0.3a1/src/arctix/transformer/dataframe/vocab.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/src/arctix/utils/dataframe/removing.py` & `arctix-0.0.3a1/src/arctix/utils/dataframe/removing.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/src/arctix/utils/dataframe/vocab.py` & `arctix-0.0.3a1/src/arctix/utils/dataframe/vocab.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/src/arctix/utils/download.py` & `arctix-0.0.3a1/src/arctix/utils/download.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/src/arctix/utils/imports.py` & `arctix-0.0.3a1/src/arctix/utils/imports.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/src/arctix/utils/iter/path.py` & `arctix-0.0.3a1/src/arctix/utils/iter/path.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/src/arctix/utils/mapping.py` & `arctix-0.0.3a1/src/arctix/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/src/arctix/utils/masking.py` & `arctix-0.0.3a1/src/arctix/utils/masking.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/src/arctix/utils/vocab.py` & `arctix-0.0.3a1/src/arctix/utils/vocab.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.3a0/PKG-INFO` & `arctix-0.0.3a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arctix
-Version: 0.0.3a0
+Version: 0.0.3a1
 Summary: 
 Home-page: https://github.com/durandtibo/arctix
 License: BSD-3-Clause
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -20,15 +20,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Provides-Extra: all
 Requires-Dist: batcharray (>=0.0.2,<0.1)
 Requires-Dist: coola (>=0.6,<1.0)
 Requires-Dist: gdown (>=5.0,<6.0) ; extra == "all"
 Requires-Dist: iden (>=0.0.3,<1.0)
 Requires-Dist: matplotlib (>=3.6,<4.0) ; extra == "all"
-Requires-Dist: numpy (>=1.21,<2.0)
+Requires-Dist: numpy (>=1.22,<2.0)
 Requires-Dist: polars (>=0.20.0,<1.0)
 Requires-Dist: requests (>=2.20,<3.0) ; extra == "all"
 Requires-Dist: tqdm (>=4.65,<5.0) ; extra == "all"
 Project-URL: Repository, https://github.com/durandtibo/arctix
 Description-Content-Type: text/markdown
 
 # arctix
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: arctix Version: 0.0.3a0 Summary: Home-page: https:/
+Metadata-Version: 2.1 Name: arctix Version: 0.0.3a1 Summary: Home-page: https:/
 /github.com/durandtibo/arctix License: BSD-3-Clause Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com Requires-Python: >=3.9,<3.13 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Provides-Extra: all Requires-Dist: batcharray
 (>=0.0.2,<0.1) Requires-Dist: coola (>=0.6,<1.0) Requires-Dist: gdown
 (>=5.0,<6.0) ; extra == "all" Requires-Dist: iden (>=0.0.3,<1.0) Requires-Dist:
-matplotlib (>=3.6,<4.0) ; extra == "all" Requires-Dist: numpy (>=1.21,<2.0)
+matplotlib (>=3.6,<4.0) ; extra == "all" Requires-Dist: numpy (>=1.22,<2.0)
 Requires-Dist: polars (>=0.20.0,<1.0) Requires-Dist: requests (>=2.20,<3.0) ;
 extra == "all" Requires-Dist: tqdm (>=4.65,<5.0) ; extra == "all" Project-URL:
 Repository, https://github.com/durandtibo/arctix Description-Content-Type:
 text/markdown # arctix
                   _[_C_I_]_[_N_i_g_h_t_l_y_ _T_e_s_t_s_]_[_N_i_g_h_t_l_y_ _P_a_c_k_a_g_e_ _T_e_s_t_s_]
                         _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]
      _[_C_o_d_e_c_o_v_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_6_1_b_8_5_7_4_e_a_1_8_e_c_f_1_0_6_d_c_e_/
```

