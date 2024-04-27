# Comparing `tmp/arctix-0.0.2a17.tar.gz` & `tmp/arctix-0.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arctix-0.0.2a17.tar", max compression
+gzip compressed data, was "arctix-0.0.3a0.tar", max compression
```

## Comparing `arctix-0.0.2a17.tar` & `arctix-0.0.3a0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0     1501 2023-07-21 06:43:48.913849 arctix-0.0.2a17/LICENSE
--rw-r--r--   0        0        0     5494 2023-07-21 06:43:48.913849 arctix-0.0.2a17/README.md
--rw-r--r--   0        0        0     4115 2023-07-21 06:43:48.913849 arctix-0.0.2a17/pyproject.toml
--rw-r--r--   0        0        0      346 2023-07-21 06:43:48.913849 arctix-0.0.2a17/src/arctix/__init__.py
--rw-r--r--   0        0        0      459 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/formatters/__init__.py
--rw-r--r--   0        0        0     3404 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/formatters/base.py
--rw-r--r--   0        0        0    10448 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/formatters/default.py
--rw-r--r--   0        0        0     3174 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/formatters/numpy_.py
--rw-r--r--   0        0        0     3182 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/formatters/torch_.py
--rw-r--r--   0        0        0      446 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/reducers/__init__.py
--rw-r--r--   0        0        0     8728 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/reducers/base.py
--rw-r--r--   0        0        0     1253 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/reducers/basic.py
--rw-r--r--   0        0        0     1842 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/reducers/numpy_.py
--rw-r--r--   0        0        0     2904 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/reducers/registry.py
--rw-r--r--   0        0        0     1929 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/reducers/torch_.py
--rw-r--r--   0        0        0     1893 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/reduction.py
--rw-r--r--   0        0        0      333 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/stats/__init__.py
--rw-r--r--   0        0        0     1170 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/stats/base.py
--rw-r--r--   0        0        0    11055 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/stats/continuous.py
--rw-r--r--   0        0        0     4087 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/stats/discrete.py
--rw-r--r--   0        0        0      459 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/stats/noop.py
--rw-r--r--   0        0        0     1647 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/summarization.py
--rw-r--r--   0        0        0      276 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/summarizers/__init__.py
--rw-r--r--   0        0        0     1794 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/summarizers/base.py
--rw-r--r--   0        0        0    12075 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/summarizers/summarizer.py
--rw-r--r--   0        0        0      507 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/testing.py
--rw-r--r--   0        0        0        0 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/utils/__init__.py
--rw-r--r--   0        0        0     3399 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/utils/format.py
--rw-r--r--   0        0        0     6555 1970-01-01 00:00:00.000000 arctix-0.0.2a17/PKG-INFO
+-rw-r--r--   0        0        0     1501 2024-04-27 06:38:39.118699 arctix-0.0.3a0/LICENSE
+-rw-r--r--   0        0        0     4493 2024-04-27 06:38:39.118699 arctix-0.0.3a0/README.md
+-rw-r--r--   0        0        0     6569 2024-04-27 06:38:39.122699 arctix-0.0.3a0/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/dataset/__init__.py
+-rw-r--r--   0        0        0    16839 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/dataset/breakfast.py
+-rw-r--r--   0        0        0    22011 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/dataset/multithumos.py
+-rw-r--r--   0        0        0      247 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/testing/__init__.py
+-rw-r--r--   0        0        0      538 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/testing/fixtures.py
+-rw-r--r--   0        0        0       29 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/__init__.py
+-rw-r--r--   0        0        0     2165 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/dataframe/__init__.py
+-rw-r--r--   0        0        0     6978 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/dataframe/base.py
+-rw-r--r--   0        0        0     3265 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/dataframe/casting.py
+-rw-r--r--   0        0        0     2107 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/dataframe/function.py
+-rw-r--r--   0        0        0     2914 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/dataframe/replace.py
+-rw-r--r--   0        0        0     3809 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/dataframe/sequential.py
+-rw-r--r--   0        0        0     2413 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/dataframe/sorting.py
+-rw-r--r--   0        0        0     3185 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/dataframe/string.py
+-rw-r--r--   0        0        0     4581 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/transformer/dataframe/vocab.py
+-rw-r--r--   0        0        0       34 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/__init__.py
+-rw-r--r--   0        0        0      276 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/dataframe/__init__.py
+-rw-r--r--   0        0        0     1618 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/dataframe/removing.py
+-rw-r--r--   0        0        0     1618 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/dataframe/vocab.py
+-rw-r--r--   0        0        0     3334 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/download.py
+-rw-r--r--   0        0        0     7145 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/imports.py
+-rw-r--r--   0        0        0      190 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/iter/__init__.py
+-rw-r--r--   0        0        0     3543 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/iter/path.py
+-rw-r--r--   0        0        0     1324 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/mapping.py
+-rw-r--r--   0        0        0     3234 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/masking.py
+-rw-r--r--   0        0        0    12749 2024-04-27 06:38:39.122699 arctix-0.0.3a0/src/arctix/utils/vocab.py
+-rw-r--r--   0        0        0     5798 1970-01-01 00:00:00.000000 arctix-0.0.3a0/PKG-INFO
```

### Comparing `arctix-0.0.2a17/LICENSE` & `arctix-0.0.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `arctix-0.0.2a17/PKG-INFO` & `arctix-0.0.3a0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,135 +1,116 @@
 Metadata-Version: 2.1
 Name: arctix
-Version: 0.0.2a17
-Summary: A library to compute a string representation of nested objects
+Version: 0.0.3a0
+Summary: 
 Home-page: https://github.com/durandtibo/arctix
 License: BSD-3-Clause
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Provides-Extra: all
-Requires-Dist: coola (>=0.0.13,<1.0)
-Requires-Dist: numpy (>=1.20,<2.0) ; extra == "all"
-Requires-Dist: torch (>=1.10,<3.0) ; extra == "all"
+Requires-Dist: batcharray (>=0.0.2,<0.1)
+Requires-Dist: coola (>=0.6,<1.0)
+Requires-Dist: gdown (>=5.0,<6.0) ; extra == "all"
+Requires-Dist: iden (>=0.0.3,<1.0)
+Requires-Dist: matplotlib (>=3.6,<4.0) ; extra == "all"
+Requires-Dist: numpy (>=1.21,<2.0)
+Requires-Dist: polars (>=0.20.0,<1.0)
+Requires-Dist: requests (>=2.20,<3.0) ; extra == "all"
+Requires-Dist: tqdm (>=4.65,<5.0) ; extra == "all"
 Project-URL: Repository, https://github.com/durandtibo/arctix
 Description-Content-Type: text/markdown
 
 # arctix
 
 <p align="center">
     <a href="https://github.com/durandtibo/arctix/actions">
-        <img alt="CI" src="https://github.com/durandtibo/arctix/workflows/CI/badge.svg?event=push&branch=main">
+        <img alt="CI" src="https://github.com/durandtibo/arctix/workflows/CI/badge.svg">
+    </a>
+    <a href="https://github.com/durandtibo/arctix/actions">
+        <img alt="Nightly Tests" src="https://github.com/durandtibo/arctix/workflows/Nightly%20Tests/badge.svg">
+    </a>
+    <a href="https://github.com/durandtibo/arctix/actions">
+        <img alt="Nightly Package Tests" src="https://github.com/durandtibo/arctix/workflows/Nightly%20Package%20Tests/badge.svg">
+    </a>
+    <br/>
+    <a href="https://durandtibo.github.io/arctix/">
+        <img alt="Documentation" src="https://github.com/durandtibo/arctix/workflows/Documentation%20(stable)/badge.svg">
     </a>
     <a href="https://durandtibo.github.io/arctix/">
-        <img alt="CI" src="https://github.com/durandtibo/arctix/workflows/Documentation/badge.svg?event=push&branch=main">
+        <img alt="Documentation" src="https://github.com/durandtibo/arctix/workflows/Documentation%20(unstable)/badge.svg">
     </a>
+    <br/>
     <a href="https://codecov.io/gh/durandtibo/arctix">
         <img alt="Codecov" src="https://codecov.io/gh/durandtibo/arctix/branch/main/graph/badge.svg">
     </a>
     <a href="https://codeclimate.com/github/durandtibo/arctix/maintainability">
         <img src="https://api.codeclimate.com/v1/badges/61b8574ea18ecf106dce/maintainability" />
     </a>
     <a href="https://codeclimate.com/github/durandtibo/arctix/test_coverage">
         <img src="https://api.codeclimate.com/v1/badges/61b8574ea18ecf106dce/test_coverage" />
     </a>
     <br/>
+    <a href="https://github.com/psf/black">
+        <img  alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
+    </a>
+    <a href="https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings">
+        <img  alt="Doc style: google" src="https://img.shields.io/badge/%20style-google-3666d6.svg">
+    </a>
+    <a href="https://github.com/astral-sh/ruff">
+        <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json" alt="Ruff" style="max-width:100%;">
+    </a>
+    <a href="https://github.com/guilatrova/tryceratops">
+        <img  alt="Doc style: google" src="https://img.shields.io/badge/try%2Fexcept%20style-tryceratops%20%F0%9F%A6%96%E2%9C%A8-black">
+    </a>
+    <br/>
     <a href="https://pypi.org/project/arctix/">
         <img alt="PYPI version" src="https://img.shields.io/pypi/v/arctix">
     </a>
     <a href="https://pypi.org/project/arctix/">
         <img alt="Python" src="https://img.shields.io/pypi/pyversions/arctix.svg">
     </a>
     <a href="https://opensource.org/licenses/BSD-3-Clause">
         <img alt="BSD-3-Clause" src="https://img.shields.io/pypi/l/arctix">
     </a>
-    <a href="https://github.com/psf/black">
-        <img  alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
-    </a>
-    <a href="https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings">
-        <img  alt="Doc style: google" src="https://img.shields.io/badge/%20style-google-3666d6.svg">
-    </a>
     <br/>
     <a href="https://pepy.tech/project/arctix">
         <img  alt="Downloads" src="https://static.pepy.tech/badge/arctix">
     </a>
     <a href="https://pepy.tech/project/arctix">
         <img  alt="Monthly downloads" src="https://static.pepy.tech/badge/arctix/month">
     </a>
     <br/>
 </p>
 
 ## Overview
 
-`arctix` is a Python library to compute a string representation of complex/nested objects.
-`arctix` was initially designed to work
-with [PyTorch `Tensor`s](https://pytorch.org/docs/stable/tensors.html)
-and [NumPy `ndarray`](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html), but it
-is possible to extend it
-to [support other data structures](https://durandtibo.github.io/arctix/customization).
+TODO
 
 - [Motivation](#motivation)
 - [Documentation](https://durandtibo.github.io/arctix/)
 - [Installation](#installation)
 - [Contributing](#contributing)
 - [API stability](#api-stability)
 - [License](#license)
 
 ## Motivation
 
-Let's imagine you have the following dictionaries that contain both a PyTorch `Tensor` and a
-NumPy `ndarray`.
-You want to compute a string representation of it.
-By default, Python tries to show the values of all the tensor/array.
-The `arctix` library was developed to easily compute structured string representation of nested
-objects.
-`arctix` provides a function `summary` that can indicate if two complex/nested objects are equal or
-not.
-
-```pycon
->>> import numpy
->>> import torch
->>> from arctix import summary
->>> print(summary({"torch": torch.ones(2, 3), "numpy": numpy.zeros((2, 3))}))
-<class 'dict'> (length=2)
-  (torch): <class 'torch.Tensor'> | shape=torch.Size([2, 3]) | dtype=torch.float32 | device=cpu
-  (numpy): <class 'numpy.ndarray'> | shape=(2, 3) | dtype=float64
->>> print(
-...     summary(
-...         {
-...             "torch": [torch.ones(2, 3), torch.zeros(6)],
-...             "numpy": numpy.zeros((2, 3)),
-...             "other": [42, 4.2, "abc"],
-...         },
-...         max_depth=3,
-...     )
-... )
-<class 'dict'> (length=3)
-  (torch): <class 'list'> (length=2)
-      (0): <class 'torch.Tensor'> | shape=torch.Size([2, 3]) | dtype=torch.float32 | device=cpu
-      (1): <class 'torch.Tensor'> | shape=torch.Size([6]) | dtype=torch.float32 | device=cpu
-  (numpy): <class 'numpy.ndarray'> | shape=(2, 3) | dtype=float64
-  (other): <class 'list'> (length=3)
-      (0): <class 'int'> 42
-      (1): <class 'float'> 4.2
-      (2): <class 'str'> abc
-```
-
-Please check the [quickstart page](https://durandtibo.github.io/arctix/quickstart) to learn more on
-how to use `arctix`.
+TODO
 
 ## Installation
 
 We highly recommend installing
 a [virtual environment](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/).
 `arctix` can be installed from pip using the following command:
```

#### html2text {}

```diff
@@ -1,71 +1,46 @@
-Metadata-Version: 2.1 Name: arctix Version: 0.0.2a17 Summary: A library to
-compute a string representation of nested objects Home-page: https://
-github.com/durandtibo/arctix License: BSD-3-Clause Author: Thibaut Durand
-Author-email: durand.tibo+gh@gmail.com Requires-Python: >=3.9,<4.0 Classifier:
+Metadata-Version: 2.1 Name: arctix Version: 0.0.3a0 Summary: Home-page: https:/
+/github.com/durandtibo/arctix License: BSD-3-Clause Author: Thibaut Durand
+Author-email: durand.tibo+gh@gmail.com Requires-Python: >=3.9,<3.13 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Provides-Extra: all Requires-
-Dist: coola (>=0.0.13,<1.0) Requires-Dist: numpy (>=1.20,<2.0) ; extra == "all"
-Requires-Dist: torch (>=1.10,<3.0) ; extra == "all" Project-URL: Repository,
-https://github.com/durandtibo/arctix Description-Content-Type: text/markdown #
-arctix
- _[_C_I_]_[_C_I_]_[_C_o_d_e_c_o_v_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_6_1_b_8_5_7_4_e_a_1_8_e_c_f_1_0_6_d_c_e_/
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Provides-Extra: all Requires-Dist: batcharray
+(>=0.0.2,<0.1) Requires-Dist: coola (>=0.6,<1.0) Requires-Dist: gdown
+(>=5.0,<6.0) ; extra == "all" Requires-Dist: iden (>=0.0.3,<1.0) Requires-Dist:
+matplotlib (>=3.6,<4.0) ; extra == "all" Requires-Dist: numpy (>=1.21,<2.0)
+Requires-Dist: polars (>=0.20.0,<1.0) Requires-Dist: requests (>=2.20,<3.0) ;
+extra == "all" Requires-Dist: tqdm (>=4.65,<5.0) ; extra == "all" Project-URL:
+Repository, https://github.com/durandtibo/arctix Description-Content-Type:
+text/markdown # arctix
+                  _[_C_I_]_[_N_i_g_h_t_l_y_ _T_e_s_t_s_]_[_N_i_g_h_t_l_y_ _P_a_c_k_a_g_e_ _T_e_s_t_s_]
+                        _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]
+     _[_C_o_d_e_c_o_v_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_6_1_b_8_5_7_4_e_a_1_8_e_c_f_1_0_6_d_c_e_/
  _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_6_1_b_8_5_7_4_e_a_1_8_e_c_f_1_0_6_d_c_e_/
                                 _t_e_s_t___c_o_v_e_r_a_g_e_]
-  _[_P_Y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_B_S_D_-_3_-_C_l_a_u_s_e_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_D_o_c_ _s_t_y_l_e_:_ _g_o_o_g_l_e_]
+        _[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_D_o_c_ _s_t_y_l_e_:_ _g_o_o_g_l_e_]_[_R_u_f_f_]_[_D_o_c_ _s_t_y_l_e_:_ _g_o_o_g_l_e_]
+                     _[_P_Y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_B_S_D_-_3_-_C_l_a_u_s_e_]
                         _[_D_o_w_n_l_o_a_d_s_]_[_M_o_n_t_h_l_y_ _d_o_w_n_l_o_a_d_s_]
-## Overview `arctix` is a Python library to compute a string representation of
-complex/nested objects. `arctix` was initially designed to work with [PyTorch
-`Tensor`s](https://pytorch.org/docs/stable/tensors.html) and [NumPy `ndarray`]
-(https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html), but it
-is possible to extend it to [support other data structures](https://
-durandtibo.github.io/arctix/customization). - [Motivation](#motivation) -
-[Documentation](https://durandtibo.github.io/arctix/) - [Installation]
-(#installation) - [Contributing](#contributing) - [API stability](#api-
-stability) - [License](#license) ## Motivation Let's imagine you have the
-following dictionaries that contain both a PyTorch `Tensor` and a NumPy
-`ndarray`. You want to compute a string representation of it. By default,
-Python tries to show the values of all the tensor/array. The `arctix` library
-was developed to easily compute structured string representation of nested
-objects. `arctix` provides a function `summary` that can indicate if two
-complex/nested objects are equal or not. ```pycon >>> import numpy >>> import
-torch >>> from arctix import summary >>> print(summary({"torch": torch.ones(2,
-3), "numpy": numpy.zeros((2, 3))}))
-dict'> (length=2) (torch):
-torch.Tensor'> | shape=torch.Size([2, 3]) | dtype=torch.float32 | device=cpu
-(numpy):
-numpy.ndarray'> | shape=(2, 3) | dtype=float64 >>> print( ... summary( ...
-{ ... "torch": [torch.ones(2, 3), torch.zeros(6)], ... "numpy": numpy.zeros((2,
-3)), ... "other": [42, 4.2, "abc"], ... }, ... max_depth=3, ... ) ... )
-dict'> (length=3) (torch):
-list'> (length=2) (0):
-torch.Tensor'> | shape=torch.Size([2, 3]) | dtype=torch.float32 | device=cpu
-(1):
-torch.Tensor'> | shape=torch.Size([6]) | dtype=torch.float32 | device=cpu
-(numpy):
-numpy.ndarray'> | shape=(2, 3) | dtype=float64 (other):
-list'> (length=3) (0):
-int'> 42 (1):
-float'> 4.2 (2):
-str'> abc ``` Please check the [quickstart page](https://durandtibo.github.io/
-arctix/quickstart) to learn more on how to use `arctix`. ## Installation We
-highly recommend installing a [virtual environment](https://
-packaging.python.org/guides/installing-using-pip-and-virtual-environments/).
-`arctix` can be installed from pip using the following command: ```shell pip
-install arctix ``` To make the package as slim as possible, only the minimal
-packages required to use `arctix` are installed. To include all the packages,
-you can use the following command: ```shell pip install arctix[all] ``` Please
-check the [get started page](https://durandtibo.github.io/arctix/get_started)
-to see how to install only some specific packages or other alternatives to
-install the library. ## Contributing Please check the instructions in
-[CONTRIBUTING.md](.github/CONTRIBUTING.md). ## API stability :warning: While
-`arctix` is in development stage, no API is guaranteed to be stable from one
-release to the next. In fact, it is very likely that the API will change
-multiple times before a stable 1.0.0 release. In practice, this means that
-upgrading `arctix` to a new version will possibly break any code that was using
-the old version of `arctix`. ## License `arctix` is licensed under BSD 3-Clause
-"New" or "Revised" license available in [LICENSE](LICENSE) file.
+## Overview TODO - [Motivation](#motivation) - [Documentation](https://
+durandtibo.github.io/arctix/) - [Installation](#installation) - [Contributing]
+(#contributing) - [API stability](#api-stability) - [License](#license) ##
+Motivation TODO ## Installation We highly recommend installing a [virtual
+environment](https://packaging.python.org/guides/installing-using-pip-and-
+virtual-environments/). `arctix` can be installed from pip using the following
+command: ```shell pip install arctix ``` To make the package as slim as
+possible, only the minimal packages required to use `arctix` are installed. To
+include all the packages, you can use the following command: ```shell pip
+install arctix[all] ``` Please check the [get started page](https://
+durandtibo.github.io/arctix/get_started) to see how to install only some
+specific packages or other alternatives to install the library. ## Contributing
+Please check the instructions in [CONTRIBUTING.md](.github/CONTRIBUTING.md). ##
+API stability :warning: While `arctix` is in development stage, no API is
+guaranteed to be stable from one release to the next. In fact, it is very
+likely that the API will change multiple times before a stable 1.0.0 release.
+In practice, this means that upgrading `arctix` to a new version will possibly
+break any code that was using the old version of `arctix`. ## License `arctix`
+is licensed under BSD 3-Clause "New" or "Revised" license available in
+[LICENSE](LICENSE) file.
```

