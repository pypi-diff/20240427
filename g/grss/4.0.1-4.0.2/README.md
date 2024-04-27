# Comparing `tmp/grss-4.0.1.tar.gz` & `tmp/grss-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grss-4.0.1.tar", last modified: Thu Apr 25 18:14:55 2024, max compression
+gzip compressed data, was "grss-4.0.2.tar", last modified: Sat Apr 27 18:54:56 2024, max compression
```

## Comparing `grss-4.0.1.tar` & `grss-4.0.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.227516 grss-4.0.1/
--rw-r--r--   0 runner     (501) staff       (20)     1909 2024-04-25 18:14:08.000000 grss-4.0.1/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     1070 2024-04-25 18:14:08.000000 grss-4.0.1/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      192 2024-04-25 18:14:08.000000 grss-4.0.1/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     7681 2024-04-25 18:14:55.227242 grss-4.0.1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     4744 2024-04-25 18:14:08.000000 grss-4.0.1/README.md
--rwxr-xr-x   0 runner     (501) staff       (20)      590 2024-04-25 18:14:08.000000 grss-4.0.1/build_cpp.sh
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.184273 grss-4.0.1/docs/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.187110 grss-4.0.1/docs/source/
--rw-r--r--   0 runner     (501) staff       (20)     3688 2024-04-25 18:14:08.000000 grss-4.0.1/docs/source/conf.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.187552 grss-4.0.1/extern/
--rw-r--r--   0 runner     (501) staff       (20)    12707 2024-04-25 18:14:08.000000 grss-4.0.1/extern/get_cspice.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.188795 grss-4.0.1/grss/
--rw-r--r--   0 runner     (501) staff       (20)      249 2024-04-25 18:14:08.000000 grss-4.0.1/grss/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.189616 grss-4.0.1/grss/debias/
--rw-r--r--   0 runner     (501) staff       (20)     1589 2024-04-25 18:14:08.000000 grss-4.0.1/grss/debias/get_debiasing_data.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.192958 grss-4.0.1/grss/fit/
--rw-r--r--   0 runner     (501) staff       (20)      259 2024-04-25 18:14:08.000000 grss-4.0.1/grss/fit/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3211 2024-04-25 18:14:08.000000 grss-4.0.1/grss/fit/fit_ades.py
--rw-r--r--   0 runner     (501) staff       (20)    38604 2024-04-25 18:14:08.000000 grss-4.0.1/grss/fit/fit_optical.py
--rw-r--r--   0 runner     (501) staff       (20)     4085 2024-04-25 18:14:08.000000 grss-4.0.1/grss/fit/fit_radar.py
--rw-r--r--   0 runner     (501) staff       (20)    85476 2024-04-25 18:14:08.000000 grss-4.0.1/grss/fit/fit_simulation.py
--rw-r--r--   0 runner     (501) staff       (20)    19123 2024-04-25 18:14:08.000000 grss-4.0.1/grss/fit/fit_utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.193315 grss-4.0.1/grss/kernels/
--rw-r--r--   0 runner     (501) staff       (20)     3121 2024-04-25 18:14:08.000000 grss-4.0.1/grss/kernels/get_kernels.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.194553 grss-4.0.1/grss/prop/
--rw-r--r--   0 runner     (501) staff       (20)      156 2024-04-25 18:14:08.000000 grss-4.0.1/grss/prop/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    13716 2024-04-25 18:14:08.000000 grss-4.0.1/grss/prop/prop_parallel.py
--rw-r--r--   0 runner     (501) staff       (20)     6076 2024-04-25 18:14:08.000000 grss-4.0.1/grss/prop/prop_unscented.py
--rw-r--r--   0 runner     (501) staff       (20)    34546 2024-04-25 18:14:08.000000 grss-4.0.1/grss/prop/prop_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2612 2024-04-25 18:14:08.000000 grss-4.0.1/grss/utils.py
--rw-r--r--   0 runner     (501) staff       (20)        5 2024-04-25 18:14:08.000000 grss-4.0.1/grss/version.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.226914 grss-4.0.1/grss.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     7681 2024-04-25 18:14:55.000000 grss-4.0.1/grss.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1499 2024-04-25 18:14:55.000000 grss-4.0.1/grss.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-25 18:14:55.000000 grss-4.0.1/grss.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)      163 2024-04-25 18:14:55.000000 grss-4.0.1/grss.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       53 2024-04-25 18:14:55.000000 grss-4.0.1/grss.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.198768 grss-4.0.1/include/
--rw-r--r--   0 runner     (501) staff       (20)     1502 2024-04-25 18:14:08.000000 grss-4.0.1/include/approach.h
--rw-r--r--   0 runner     (501) staff       (20)     3334 2024-04-25 18:14:08.000000 grss-4.0.1/include/elements.h
--rw-r--r--   0 runner     (501) staff       (20)     1669 2024-04-25 18:14:08.000000 grss-4.0.1/include/force.h
--rw-r--r--   0 runner     (501) staff       (20)     4577 2024-04-25 18:14:08.000000 grss-4.0.1/include/gr15.h
--rw-r--r--   0 runner     (501) staff       (20)     1464 2024-04-25 18:14:08.000000 grss-4.0.1/include/grss.h
--rw-r--r--   0 runner     (501) staff       (20)     6190 2024-04-25 18:14:08.000000 grss-4.0.1/include/interpolate.h
--rw-r--r--   0 runner     (501) staff       (20)      356 2024-04-25 18:14:08.000000 grss-4.0.1/include/parallel.h
--rw-r--r--   0 runner     (501) staff       (20)     2714 2024-04-25 18:14:08.000000 grss-4.0.1/include/pck.h
--rw-r--r--   0 runner     (501) staff       (20)    19128 2024-04-25 18:14:08.000000 grss-4.0.1/include/simulation.h
--rw-r--r--   0 runner     (501) staff       (20)     3804 2024-04-25 18:14:08.000000 grss-4.0.1/include/spk.h
--rw-r--r--   0 runner     (501) staff       (20)     2685 2024-04-25 18:14:08.000000 grss-4.0.1/include/stm.h
--rw-r--r--   0 runner     (501) staff       (20)     1812 2024-04-25 18:14:08.000000 grss-4.0.1/include/timeconvert.h
--rw-r--r--   0 runner     (501) staff       (20)     5462 2024-04-25 18:14:08.000000 grss-4.0.1/include/utilities.h
--rw-r--r--   0 runner     (501) staff       (20)     2114 2024-04-25 18:14:08.000000 grss-4.0.1/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)      163 2024-04-25 18:14:08.000000 grss-4.0.1/requirements.txt
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-25 18:14:55.227557 grss-4.0.1/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1740 2024-04-25 18:14:08.000000 grss-4.0.1/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.207184 grss-4.0.1/src/
--rw-r--r--   0 runner     (501) staff       (20)      283 2024-04-25 18:14:08.000000 grss-4.0.1/src/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    31500 2024-04-25 18:14:08.000000 grss-4.0.1/src/approach.cpp
--rw-r--r--   0 runner     (501) staff       (20)    26087 2024-04-25 18:14:08.000000 grss-4.0.1/src/elements.cpp
--rw-r--r--   0 runner     (501) staff       (20)    29546 2024-04-25 18:14:08.000000 grss-4.0.1/src/force.cpp
--rw-r--r--   0 runner     (501) staff       (20)    20530 2024-04-25 18:14:08.000000 grss-4.0.1/src/gr15.cpp
--rw-r--r--   0 runner     (501) staff       (20)    45888 2024-04-25 18:14:08.000000 grss-4.0.1/src/grss.cpp
--rw-r--r--   0 runner     (501) staff       (20)    44803 2024-04-25 18:14:08.000000 grss-4.0.1/src/interpolate.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2722 2024-04-25 18:14:08.000000 grss-4.0.1/src/parallel.cpp
--rw-r--r--   0 runner     (501) staff       (20)    35824 2024-04-25 18:14:08.000000 grss-4.0.1/src/pck.cpp
--rw-r--r--   0 runner     (501) staff       (20)    68054 2024-04-25 18:14:08.000000 grss-4.0.1/src/simulation.cpp
--rw-r--r--   0 runner     (501) staff       (20)    15260 2024-04-25 18:14:08.000000 grss-4.0.1/src/spk.cpp
--rw-r--r--   0 runner     (501) staff       (20)    24181 2024-04-25 18:14:08.000000 grss-4.0.1/src/stm.cpp
--rw-r--r--   0 runner     (501) staff       (20)     6951 2024-04-25 18:14:08.000000 grss-4.0.1/src/timeconvert.cpp
--rw-r--r--   0 runner     (501) staff       (20)    12536 2024-04-25 18:14:08.000000 grss-4.0.1/src/utilities.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.185328 grss-4.0.1/tests/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.185257 grss-4.0.1/tests/cpp/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.209187 grss-4.0.1/tests/cpp/prop/
--rw-r--r--   0 runner     (501) staff       (20)      797 2024-04-25 18:14:08.000000 grss-4.0.1/tests/cpp/prop/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     3725 2024-04-25 18:14:08.000000 grss-4.0.1/tests/cpp/prop/apophis.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5981 2024-04-25 18:14:08.000000 grss-4.0.1/tests/cpp/prop/didymos.cpp
--rw-r--r--   0 runner     (501) staff       (20)     3449 2024-04-25 18:14:08.000000 grss-4.0.1/tests/cpp/prop/pck_map.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5917 2024-04-25 18:14:08.000000 grss-4.0.1/tests/cpp/prop/spk_map.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.209459 grss-4.0.1/tests/python/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.219120 grss-4.0.1/tests/python/fit/
--rw-r--r--   0 runner     (501) staff       (20)   743881 2024-04-25 18:14:08.000000 grss-4.0.1/tests/python/fit/chesley.ipynb
--rw-r--r--   0 runner     (501) staff       (20)   701963 2024-04-25 18:14:08.000000 grss-4.0.1/tests/python/fit/eggl.ipynb
--rw-r--r--   0 runner     (501) staff       (20)   635614 2024-04-25 18:14:08.000000 grss-4.0.1/tests/python/fit/farnocchia.ipynb
--rw-r--r--   0 runner     (501) staff       (20)   666353 2024-04-25 18:14:08.000000 grss-4.0.1/tests/python/fit/shantanunaidu.ipynb
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.226000 grss-4.0.1/tests/python/prop/
--rw-r--r--   0 runner     (501) staff       (20)   104846 2024-04-25 18:14:08.000000 grss-4.0.1/tests/python/prop/apophis.ipynb
--rw-r--r--   0 runner     (501) staff       (20)   102230 2024-04-25 18:14:08.000000 grss-4.0.1/tests/python/prop/didymos.ipynb
--rw-r--r--   0 runner     (501) staff       (20)   116221 2024-04-25 18:14:08.000000 grss-4.0.1/tests/python/prop/icarus.ipynb
--rw-r--r--   0 runner     (501) staff       (20)    77629 2024-04-25 18:14:08.000000 grss-4.0.1/tests/python/prop/moshup.ipynb
--rwxr-xr-x   0 runner     (501) staff       (20)      269 2024-04-25 18:14:08.000000 grss-4.0.1/tests/python/run_tests.sh
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-27 18:54:56.402985 grss-4.0.2/
+-rw-r--r--   0 runner     (501) staff       (20)     1909 2024-04-27 18:54:04.000000 grss-4.0.2/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1070 2024-04-27 18:54:04.000000 grss-4.0.2/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      192 2024-04-27 18:54:04.000000 grss-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     7681 2024-04-27 18:54:56.402575 grss-4.0.2/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     4744 2024-04-27 18:54:04.000000 grss-4.0.2/README.md
+-rwxr-xr-x   0 runner     (501) staff       (20)      590 2024-04-27 18:54:04.000000 grss-4.0.2/build_cpp.sh
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-27 18:54:56.269238 grss-4.0.2/docs/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-27 18:54:56.306926 grss-4.0.2/docs/source/
+-rw-r--r--   0 runner     (501) staff       (20)     3688 2024-04-27 18:54:04.000000 grss-4.0.2/docs/source/conf.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-27 18:54:56.307082 grss-4.0.2/extern/
+-rw-r--r--   0 runner     (501) staff       (20)    12707 2024-04-27 18:54:04.000000 grss-4.0.2/extern/get_cspice.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-27 18:54:56.307834 grss-4.0.2/grss/
+-rw-r--r--   0 runner     (501) staff       (20)      249 2024-04-27 18:54:04.000000 grss-4.0.2/grss/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-27 18:54:56.308837 grss-4.0.2/grss/debias/
+-rw-r--r--   0 runner     (501) staff       (20)     1589 2024-04-27 18:54:04.000000 grss-4.0.2/grss/debias/get_debiasing_data.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-27 18:54:56.310174 grss-4.0.2/grss/fit/
+-rw-r--r--   0 runner     (501) staff       (20)      259 2024-04-27 18:54:04.000000 grss-4.0.2/grss/fit/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3211 2024-04-27 18:54:04.000000 grss-4.0.2/grss/fit/fit_ades.py
+-rw-r--r--   0 runner     (501) staff       (20)    38897 2024-04-27 18:54:04.000000 grss-4.0.2/grss/fit/fit_optical.py
+-rw-r--r--   0 runner     (501) staff       (20)     4085 2024-04-27 18:54:04.000000 grss-4.0.2/grss/fit/fit_radar.py
+-rw-r--r--   0 runner     (501) staff       (20)    86272 2024-04-27 18:54:04.000000 grss-4.0.2/grss/fit/fit_simulation.py
+-rw-r--r--   0 runner     (501) staff       (20)    19123 2024-04-27 18:54:04.000000 grss-4.0.2/grss/fit/fit_utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-27 18:54:56.310518 grss-4.0.2/grss/kernels/
+-rw-r--r--   0 runner     (501) staff       (20)     3121 2024-04-27 18:54:04.000000 grss-4.0.2/grss/kernels/get_kernels.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-27 18:54:56.311267 grss-4.0.2/grss/prop/
+-rw-r--r--   0 runner     (501) staff       (20)      156 2024-04-27 18:54:04.000000 grss-4.0.2/grss/prop/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    13930 2024-04-27 18:54:04.000000 grss-4.0.2/grss/prop/prop_parallel.py
+-rw-r--r--   0 runner     (501) staff       (20)     6076 2024-04-27 18:54:04.000000 grss-4.0.2/grss/prop/prop_unscented.py
+-rw-r--r--   0 runner     (501) staff       (20)    34692 2024-04-27 18:54:04.000000 grss-4.0.2/grss/prop/prop_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2612 2024-04-27 18:54:04.000000 grss-4.0.2/grss/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)        5 2024-04-27 18:54:04.000000 grss-4.0.2/grss/version.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-27 18:54:56.402002 grss-4.0.2/grss.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     7681 2024-04-27 18:54:56.000000 grss-4.0.2/grss.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1499 2024-04-27 18:54:56.000000 grss-4.0.2/grss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-27 18:54:56.000000 grss-4.0.2/grss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)      163 2024-04-27 18:54:56.000000 grss-4.0.2/grss.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       53 2024-04-27 18:54:56.000000 grss-4.0.2/grss.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-27 18:54:56.313821 grss-4.0.2/include/
+-rw-r--r--   0 runner     (501) staff       (20)     1502 2024-04-27 18:54:04.000000 grss-4.0.2/include/approach.h
+-rw-r--r--   0 runner     (501) staff       (20)     3334 2024-04-27 18:54:04.000000 grss-4.0.2/include/elements.h
+-rw-r--r--   0 runner     (501) staff       (20)     1669 2024-04-27 18:54:04.000000 grss-4.0.2/include/force.h
+-rw-r--r--   0 runner     (501) staff       (20)     4577 2024-04-27 18:54:04.000000 grss-4.0.2/include/gr15.h
+-rw-r--r--   0 runner     (501) staff       (20)     1464 2024-04-27 18:54:04.000000 grss-4.0.2/include/grss.h
+-rw-r--r--   0 runner     (501) staff       (20)     6190 2024-04-27 18:54:04.000000 grss-4.0.2/include/interpolate.h
+-rw-r--r--   0 runner     (501) staff       (20)      356 2024-04-27 18:54:04.000000 grss-4.0.2/include/parallel.h
+-rw-r--r--   0 runner     (501) staff       (20)     2714 2024-04-27 18:54:04.000000 grss-4.0.2/include/pck.h
+-rw-r--r--   0 runner     (501) staff       (20)    19431 2024-04-27 18:54:04.000000 grss-4.0.2/include/simulation.h
+-rw-r--r--   0 runner     (501) staff       (20)     3804 2024-04-27 18:54:04.000000 grss-4.0.2/include/spk.h
+-rw-r--r--   0 runner     (501) staff       (20)     2685 2024-04-27 18:54:04.000000 grss-4.0.2/include/stm.h
+-rw-r--r--   0 runner     (501) staff       (20)     1812 2024-04-27 18:54:04.000000 grss-4.0.2/include/timeconvert.h
+-rw-r--r--   0 runner     (501) staff       (20)     5462 2024-04-27 18:54:04.000000 grss-4.0.2/include/utilities.h
+-rw-r--r--   0 runner     (501) staff       (20)     2114 2024-04-27 18:54:04.000000 grss-4.0.2/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)      163 2024-04-27 18:54:04.000000 grss-4.0.2/requirements.txt
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-27 18:54:56.403235 grss-4.0.2/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1740 2024-04-27 18:54:04.000000 grss-4.0.2/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-27 18:54:56.317130 grss-4.0.2/src/
+-rw-r--r--   0 runner     (501) staff       (20)      283 2024-04-27 18:54:04.000000 grss-4.0.2/src/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    32165 2024-04-27 18:54:04.000000 grss-4.0.2/src/approach.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    26087 2024-04-27 18:54:04.000000 grss-4.0.2/src/elements.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    29546 2024-04-27 18:54:04.000000 grss-4.0.2/src/force.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    20530 2024-04-27 18:54:04.000000 grss-4.0.2/src/gr15.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    45888 2024-04-27 18:54:04.000000 grss-4.0.2/src/grss.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    44803 2024-04-27 18:54:04.000000 grss-4.0.2/src/interpolate.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2722 2024-04-27 18:54:04.000000 grss-4.0.2/src/parallel.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    35824 2024-04-27 18:54:04.000000 grss-4.0.2/src/pck.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    68054 2024-04-27 18:54:04.000000 grss-4.0.2/src/simulation.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    15260 2024-04-27 18:54:04.000000 grss-4.0.2/src/spk.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    24181 2024-04-27 18:54:04.000000 grss-4.0.2/src/stm.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     6951 2024-04-27 18:54:04.000000 grss-4.0.2/src/timeconvert.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    12536 2024-04-27 18:54:04.000000 grss-4.0.2/src/utilities.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-27 18:54:56.270163 grss-4.0.2/tests/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-27 18:54:56.270072 grss-4.0.2/tests/cpp/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-27 18:54:56.317798 grss-4.0.2/tests/cpp/prop/
+-rw-r--r--   0 runner     (501) staff       (20)      797 2024-04-27 18:54:04.000000 grss-4.0.2/tests/cpp/prop/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     3725 2024-04-27 18:54:04.000000 grss-4.0.2/tests/cpp/prop/apophis.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     5981 2024-04-27 18:54:04.000000 grss-4.0.2/tests/cpp/prop/didymos.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     3449 2024-04-27 18:54:04.000000 grss-4.0.2/tests/cpp/prop/pck_map.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     5917 2024-04-27 18:54:04.000000 grss-4.0.2/tests/cpp/prop/spk_map.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-27 18:54:56.317931 grss-4.0.2/tests/python/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-27 18:54:56.327008 grss-4.0.2/tests/python/fit/
+-rw-r--r--   0 runner     (501) staff       (20)   743881 2024-04-27 18:54:04.000000 grss-4.0.2/tests/python/fit/chesley.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)   701963 2024-04-27 18:54:04.000000 grss-4.0.2/tests/python/fit/eggl.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)   635614 2024-04-27 18:54:04.000000 grss-4.0.2/tests/python/fit/farnocchia.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)   666353 2024-04-27 18:54:04.000000 grss-4.0.2/tests/python/fit/shantanunaidu.ipynb
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-27 18:54:56.400699 grss-4.0.2/tests/python/prop/
+-rw-r--r--   0 runner     (501) staff       (20)   104846 2024-04-27 18:54:04.000000 grss-4.0.2/tests/python/prop/apophis.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)   102230 2024-04-27 18:54:04.000000 grss-4.0.2/tests/python/prop/didymos.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)   116221 2024-04-27 18:54:04.000000 grss-4.0.2/tests/python/prop/icarus.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)    77629 2024-04-27 18:54:04.000000 grss-4.0.2/tests/python/prop/moshup.ipynb
+-rwxr-xr-x   0 runner     (501) staff       (20)      269 2024-04-27 18:54:04.000000 grss-4.0.2/tests/python/run_tests.sh
```

### Comparing `grss-4.0.1/CMakeLists.txt` & `grss-4.0.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/LICENSE` & `grss-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/PKG-INFO` & `grss-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grss
-Version: 4.0.1
+Version: 4.0.2
 Summary: GRSS: Gauss-Radau Small-body Simulator
 Author: Rahil Makadia
 Author-email: makadia2@illinois.edu
 Maintainer: Rahil Makadia
 Maintainer-email: makadia2@illinois.edu
 License: MIT License
```

### Comparing `grss-4.0.1/README.md` & `grss-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/build_cpp.sh` & `grss-4.0.2/build_cpp.sh`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/docs/source/conf.py` & `grss-4.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/extern/get_cspice.py` & `grss-4.0.2/extern/get_cspice.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/grss/debias/get_debiasing_data.py` & `grss-4.0.2/grss/debias/get_debiasing_data.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/grss/fit/fit_ades.py` & `grss-4.0.2/grss/fit/fit_ades.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/grss/fit/fit_optical.py` & `grss-4.0.2/grss/fit/fit_optical.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Optical observation handling for the GRSS orbit determination code"""
 import os
+from io import StringIO
 from astropy.time import Time
 import requests
 from astroquery.gaia import Gaia
 import healpy as hp
 import numpy as np
 import pandas as pd
 
@@ -32,15 +33,15 @@
     response = requests.get("https://data.minorplanetcenter.net/api/get-obs",
                             json={"desigs": [f"{tdes}"], "output_format":["XML"]},
                             timeout=30)
     if response.ok:
         obs_data = response.json()[0]["XML"]
     else:
         print("Error getting MPC XML data: ", response.status_code, response.content)
-    return obs_data
+    return StringIO(obs_data)
 
 def _ades_mode_check(df):
     """
     Check the mode values in the ADES data frame.
 
     Parameters
     ----------
@@ -133,28 +134,31 @@
     else:
         obs_data = optical_obs_file
         if not os.path.exists(obs_data):
             raise FileNotFoundError(f"File {obs_data} does not exist.")
     # read in the data and add extra columns if not present
     obs_df = (
         pd.read_xml(obs_data, dtype=ades_column_types)
-        # add columns if they are not present
-        .reindex(columns=ades_column_types.keys(), fill_value=np.nan)
         # compute the obsTimeMJD time from obsTime
         .assign(obsTimeMJD=lambda x:Time(x['obsTime'].to_list(),format='isot',scale='utc').utc.mjd)
     )
+    # add columns if they are not present
+    str_cols = ['trx', 'rcv', 'sys', 'selAst']
+    for col in str_cols:
+        if col not in obs_df:
+            obs_df[col] = str(np.nan)
+    for col in ades_column_types:
+        if col not in obs_df:
+            obs_df[col] = np.nan
     if verbose:
         print(f"Read in {len(obs_df)} observations from the MPC.")
     _ades_mode_check(obs_df)
     _ades_ast_cat_check(obs_df)
     # filter the data based on the time range
     obs_df.query(f"{t_min_utc} <= obsTimeMJD <= {t_max_utc}", inplace=True)
-    # # filter the data based on the observation station
-    # stn_to_remove = ('247', '270') # roving observatories
-    # obs_df.query(f"stn not in {stn_to_remove}", inplace=True)
     # reindex the data frame
     obs_df.reset_index(drop=True, inplace=True)
     # for all indices with OCC mode compute ra and dec as raStar+deltaRA and decStar+deltaDec
     occ_idx = obs_df.query("mode == 'OCC'").index
     obs_df.loc[occ_idx, 'dec'] = obs_df.loc[occ_idx, 'decStar']
     obs_df.loc[occ_idx, 'dec'] += obs_df.loc[occ_idx, 'deltaDec']/3600
     obs_df['cosDec'] = np.cos(obs_df['dec']*np.pi/180)
@@ -954,15 +958,21 @@
     if eliminate and deweight:
         raise ValueError('Cannot deweight and eliminate observations at the same time.')
     if not eliminate and not deweight:
         print("WARNING: No deweighting or elimination scheme applied",
                 "for observations during the same night.")
     obs_df = create_optical_obs_df(body_id, optical_obs_file,
                                     t_min_tdb, t_max_tdb, verbose)
-    obs_df = apply_debiasing_scheme(obs_df, debias_lowres, verbose)
+    if debias_lowres is not None:
+        obs_df = apply_debiasing_scheme(obs_df, debias_lowres, verbose)
+    else:
+        print("WARNING: No debiasing scheme applied to the observations.",
+                "Setting biases to zero.")
+        opt_idx = obs_df.query("mode != 'RAD'").index
+        obs_df.loc[opt_idx, ['biasRA', 'biasDec']] = 0.0
     obs_df = apply_weighting_scheme(obs_df, verbose)
     if deweight:
         obs_df = deweight_obs(obs_df, num_obs_per_night, verbose)
     elif eliminate:
         obs_df = eliminate_obs(obs_df, num_obs_per_night, verbose)
     # obs_df.sort_values(by='obsTimeMJD', inplace=True, ignore_index=True)
     return obs_df
```

### Comparing `grss-4.0.1/grss/fit/fit_radar.py` & `grss-4.0.2/grss/fit/fit_radar.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/grss/fit/fit_simulation.py` & `grss-4.0.2/grss/fit/fit_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import datetime
 import numpy as np
 import matplotlib.pyplot as plt
 from astropy.time import Time
 
 from .. import libgrss
 from ..utils import default_kernel_path, grss_path
-from .fit_utils import get_observer_info
+from .fit_utils import get_observer_info, get_similarity_stats
 
 __all__ = [ 'FitSimulation',
 ]
 
 class IterationParams:
     """
     Class for storing the iteration parameters for a single iteration of the
@@ -708,15 +708,16 @@
 
         Returns
         -------
         None : NoneType
             None
         """
         self.obs = obs_df
-        self.obs['selAst'].fillna('A', inplace=True)
+        sel_ast_map = {'': 'A', ' ': 'A', np.nan: 'A', 'nan': 'A'}
+        self.obs['selAst'] = self.obs['selAst'].replace(sel_ast_map)
         if self.simulated_obs is not None:
             self._add_simulated_obs()
         self.obs.sort_values(by='obsTimeMJD', inplace=True, ignore_index=True)
         self.observer_info = get_observer_info(self.obs)
         self.optical_idx = []
         self.delay_idx = []
         self.doppler_idx = []
@@ -1889,26 +1890,24 @@
             f.write(f'{f"RA[as]/Del[{chr(0x00b5)}s]".center(widths["resRA"])}')
             f.write(f'{"Dec[as]/Dop[Hz]".center(widths["resDec"])}')
             f.write("\n")
             for i, obs in self.obs[::-1].iterrows():
                 f.write(f'{obs["selAst"]+obs["obsTime"]:<{widths["obsTime"]}}')
                 if obs['mode'] in {'RAD', 'SIM_RAD_DEL', 'SIM_RAD_DOP'}:
                     f.write(f'{obs["trx"]+"/"+obs["rcv"]:^{widths["stn"]}}')
-                    f.write(f'{obs["delay"]:^{widths["ra"]}.9f}')
-                    sign = "+" if obs["doppler"] >= 0 else ""
-                    f.write(f'{sign+str(obs["doppler"]):^{widths["dec"]}}')
+                    f.write(f'{obs["delay"]:^{widths["ra"]}.13g}')
+                    f.write(f'{obs["doppler"]:^+{widths["dec"]}.12g}')
                     f.write(f'{obs["sigDelay"]:^{widths["sigRA"]}.4f}')
                     f.write(f'{obs["sigDoppler"]:^{widths["sigDec"]}.4f}')
                     f.write(f'{obs["resDelay"]:^+{widths["resRA"]}.7f}')
                     f.write(f'{obs["resDoppler"]:^+{widths["resDec"]}.7f}')
                 else:
                     f.write(f'{obs["stn"]:^{widths["stn"]}}')
-                    f.write(f'{obs["ra"]:^{widths["ra"]}}')
-                    sign = "+" if obs["dec"] >= 0 else ""
-                    f.write(f'{sign+str(obs["dec"]):^{widths["dec"]}}')
+                    f.write(f'{obs["ra"]:^{widths["ra"]}.13g}')
+                    f.write(f'{obs["dec"]:^+{widths["dec"]}.12g}')
                     f.write(f'{obs["sigRA"]:^{widths["sigRA"]}.4f}')
                     f.write(f'{obs["sigDec"]:^{widths["sigDec"]}.4f}')
                     f.write(f'{obs["resRA"]:^+{widths["resRA"]}.7f}')
                     f.write(f'{obs["resDec"]:^+{widths["resDec"]}.7f}')
                 f.write("\n")
             f.write("\n")
 
@@ -1947,11 +1946,26 @@
                         f.write(f'{final_unc:18.11e}{half_tab}')
                         f.write(f'{final_val-init_val:+18.11e}{half_tab}')
                         f.write(f'{(final_val-init_val)/init_unc:+10.3f}\n')
                 f.write("\n")
                 if itrn.iter_number != self.n_iter:
                     f.write(subsection_full + '\n')
 
+            mean_0 = np.array(list(self.x_init.values()))
+            cov_0 = self.covariance_init
+            mean_f = np.array(list(self.x_nom.values()))
+            cov_f = self.covariance
+            md_f, md_0, b_dist, b_coeff = get_similarity_stats(mean_0, cov_0, mean_f, cov_f)
+            f.write(f'Mahalonobis distance between initial and final solution: {md_f:0.2f}')
+            f.write("\n")
+            f.write(f'Mahalonobis distance between final and initial solution: {md_0:0.2f}')
+            f.write("\n")
+            f.write(f'Bhattacharya distance between initial and final solution: {b_dist:0.4f}')
+            f.write("\n")
+            f.write(f'Bhattacharya coefficient between initial and final solution: {b_coeff:0.4f}')
+            f.write("\n")
+            f.write(subsection_full + '\n')
+
             f.write(section_full + '\n')
             f.write(f"{header_section_half} END OF FILE {header_section_half}" + '\n')
             f.write(section_full + '\n')
         return None
```

### Comparing `grss-4.0.1/grss/fit/fit_utils.py` & `grss-4.0.2/grss/fit/fit_utils.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/grss/kernels/get_kernels.py` & `grss-4.0.2/grss/kernels/get_kernels.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/grss/prop/prop_parallel.py` & `grss-4.0.2/grss/prop/prop_parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,14 +360,15 @@
 
     Returns
     -------
     all_clusters : tuple of list of libgrss.CloseApproachParameters objects
         A tuple of close approach clusters (each cluster is a list of
         close approaches).
     """
+    start_time = time.time()
     all_clusters = []
     full_list = [ca_or_impact for ca_or_impact in full_list
                     if ca_or_impact.centralBodySpiceId == central_body]
     if not full_list:
         return tuple(all_clusters)
     times = [ca_or_impact.t for ca_or_impact in full_list]
     bodies = [ca_or_impact.flybyBody for ca_or_impact in full_list]
@@ -383,8 +384,13 @@
             all_clusters.append(cluster)
             cluster = [full_list[idx]]
             cluster_bodies = [bodies[idx]]
         else:
             cluster.append(full_list[idx])
             cluster_bodies.append(bodies[idx])
     all_clusters.append(cluster)
+    end_time = time.time()
+    duration = end_time - start_time
+    mm = int(duration / 60)
+    ss = duration % 60
+    print(f'Clustering took {mm:02d} minute(s) and {ss:.6f} seconds')
     return tuple(all_clusters)
```

### Comparing `grss-4.0.1/grss/prop/prop_unscented.py` & `grss-4.0.2/grss/prop/prop_unscented.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/grss/prop/prop_utils.py` & `grss-4.0.2/grss/prop/prop_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -541,16 +541,21 @@
     scaled_x = np.array([approach.scaled.x*au2units for approach in ca_list])
     scaled_y = np.array([approach.scaled.y*au2units for approach in ca_list])
     scaled_nan = np.any(np.isnan(scaled_x)) or np.any(np.isnan(scaled_y))
     mtp_x = np.array([approach.mtp.x*au2units for approach in ca_list])
     mtp_y = np.array([approach.mtp.y*au2units for approach in ca_list])
     mtp_nan = np.any(np.isnan(mtp_x)) or np.any(np.isnan(mtp_y))
     focus_factor = np.nanmean([approach.gravFocusFactor for approach in ca_list])
-    impact_bool = np.array([approach.impact for approach in ca_list])
-    impact_any = np.any(impact_bool)
+    try:
+        lon = np.array([approach.lon for approach in ca_list])
+        lat = np.array([approach.lat for approach in ca_list])
+    except AttributeError:
+        lon = None
+        lat = None
+    impact_any = lon is not None and lat is not None
     if len(ca_list) >= 100 or sigma_points is not None:
         if not kizner_nan:
             kizner_data = data_to_ellipse(kizner_x, kizner_y, n_std, 'kizner',
                                             print_ellipse_params, units, sigma_points)
         else:
             kizner_data = None
         if not opik_nan:
```

### Comparing `grss-4.0.1/grss/utils.py` & `grss-4.0.2/grss/utils.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/grss.egg-info/PKG-INFO` & `grss-4.0.2/grss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grss
-Version: 4.0.1
+Version: 4.0.2
 Summary: GRSS: Gauss-Radau Small-body Simulator
 Author: Rahil Makadia
 Author-email: makadia2@illinois.edu
 Maintainer: Rahil Makadia
 Maintainer-email: makadia2@illinois.edu
 License: MIT License
```

### Comparing `grss-4.0.1/grss.egg-info/SOURCES.txt` & `grss-4.0.2/grss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/include/approach.h` & `grss-4.0.2/include/approach.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/include/elements.h` & `grss-4.0.2/include/elements.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/include/force.h` & `grss-4.0.2/include/force.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/include/gr15.h` & `grss-4.0.2/include/gr15.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/include/grss.h` & `grss-4.0.2/include/grss.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/include/interpolate.h` & `grss-4.0.2/include/interpolate.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/include/pck.h` & `grss-4.0.2/include/pck.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/include/simulation.h` & `grss-4.0.2/include/simulation.h`

 * *Files 0% similar despite different names*

```diff
@@ -170,28 +170,30 @@
     real r0_au = 2.808L;
 };
 
 /**
  * @brief Class for integrated bodies in a PropSimulation.
  * 
  * @param spiceId SPICE ID of the body.
+ * @param logCA Flag to indicate if close approaches are logged (default: true).
  * @param isCometary Flag to indicate if the body is initialized with a cometary state (as opposed to Cartesian state).
  * @param initState Initial state of the body.
  * @param isInteg Flag to indicate if the body is integrated.
  * @param isThrusting Flag to indicate if the body is thrusting.
  * @param ngParams Nongravitational parameters for the body.
  * @param n2Derivs Number of second derivatives for the body.
  * @param propStm Flag to indicate if the state transition matrix is propagated.
  * @param stm State transition matrix.
  * @param dCartdState Derivatives of initial Cartesian state with respect to initial state.
  */
 class IntegBody : public Body {
    private:
    public:
     int spiceId = -99999;
+    bool logCA = true;
     bool isCometary = false;
     std::vector<real> initState;
     std::vector<real> initCart;
     bool isInteg = true;
     bool isThrusting = false;
     NongravParameters ngParams;
     size_t n2Derivs = 3;
@@ -268,16 +270,18 @@
     std::vector<real> dx = std::vector<real>(6, std::numeric_limits<real>::quiet_NaN());
     std::vector<real> dy = std::vector<real>(6, std::numeric_limits<real>::quiet_NaN());
 };
 
 /**
  * @brief Class for close approach parameters in a PropSimulation.
  * 
- * @param t Time of the close approach.
- * @param xRel Relative state at the close approach.
+ * @param t Time of the close approach or impact (from child class).
+ * @param xRel Relative state at the close approach or impact (from child class).
+ * @param tCA Time of the close approach.
+ * @param xRelCA Relative state at the close approach.
  * @param tMap Time of the B-plane map.
  * @param xRelMap Relative state at the B-plane map time.
  * @param dist Distance at the close approach.
  * @param vel Relative velocity at the close approach.
  * @param vInf Hyperbolic excess velocity of the close approach.
  * @param flybyBody Name of the flyby body.
  * @param flybyBodyIdx Index of the flyby body in the PropSimulation.
@@ -298,14 +302,16 @@
  * @param dt Partial derivatives of the time of closest approach with respect to the state at the close approach.
  */
 class CloseApproachParameters {
    private:
    public:
     real t;
     std::vector<real> xRel;
+    real tCA;
+    std::vector<real> xRelCA;
     real tMap;
     std::vector<real> xRelMap;
     real dist;
     real vel;
     real vInf;
     std::string flybyBody;
     int flybyBodyIdx;
@@ -509,15 +515,15 @@
     void set_integration_parameters(
         real tf, std::vector<real> tEval = std::vector<real>(),
         bool tEvalUTC = false, bool evalApparentState = false,
         bool convergedLightTime = false,
         std::vector<std::vector<real>> observerInfo =
             std::vector<std::vector<real>>(),
         bool adaptiveTimestep = true, real dt0 = 0.0L, real dtMax = 21.0L,
-        real dtMin = 5.0e-3L, real dtChangeFactor = 0.25L,
+        real dtMin = 1.0e-4L, real dtChangeFactor = 0.25L,
         real tolInteg = 1.0e-11L, real tolPC = 1.0e-16L);
     /**
      * @brief Get the constants used in the simulation.
      */
     std::vector<real> get_sim_constants();
     /**
      * @brief Get the integration parameters used in the simulation.
```

### Comparing `grss-4.0.1/include/spk.h` & `grss-4.0.2/include/spk.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/include/stm.h` & `grss-4.0.2/include/stm.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/include/timeconvert.h` & `grss-4.0.2/include/timeconvert.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/include/utilities.h` & `grss-4.0.2/include/utilities.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/pyproject.toml` & `grss-4.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/setup.py` & `grss-4.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/src/approach.cpp` & `grss-4.0.2/src/approach.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,31 @@
 #include "approach.h"
 
 /**
+ * @brief Get the atmosphere thickness offset for the central body.
+ * 
+ * @param[in] centralBodySpiceId SPICE ID of the central body.
+ * @return atm_offset Offset for the atmosphere of the central body.
+ */
+static real get_atm_offset(const int &centralBodySpiceId){
+    real atm_offset = 0;
+    real au2km = 149597870.7;
+    switch (centralBodySpiceId)
+    {
+    case 399:
+        atm_offset = 100.0/au2km;
+        break;
+    default:
+        atm_offset = 0;
+        break;
+    }
+    return atm_offset;
+}
+
+/**
  * @param[inout] propSim PropSimulation object for the integration.
  * @param[in] tOld Time at the previous integrator epoch.
  * @param[in] xIntegOld State at the previous integrator epoch.
  * @param[in] t Time at the current integrator epoch.
  * @param[in] xInteg State at the current integrator epoch.
  */
 void check_ca_or_impact(PropSimulation *propSim, const real &tOld,
@@ -13,95 +34,88 @@
     // Check for close approach or impact
     // If a close approach is detected, the time of closest approach is
     // determined by root finding using Brent's method.
     // If an impact is detected, the simulation is terminated.
     const bool forwardProp = propSim->integParams.t0 < propSim->integParams.tf;
     const bool backwardProp = propSim->integParams.t0 > propSim->integParams.tf;
     size_t starti = 0;
-    real relPosOld[3], relPos[3], relVelOld[3], relVel[3];
     for (size_t i = 0; i < propSim->integParams.nInteg; i++) {
+        if (!propSim->integBodies[i].logCA) {
+            continue;
+        }
         const real flybyBodyRadius = propSim->integBodies[i].radius;
         real centralBodyRadius, caTol;
         size_t startj = 0;
         for (size_t j = 0; j < propSim->integParams.nTotal; j++) {
             if (i != j) {
-                real relDistOld, relDist;
+                real relPosOld[3], relPos[3], relVelOld[3], relVel[3];
                 if (j < propSim->integParams.nInteg) {
                     centralBodyRadius = propSim->integBodies[j].radius;
                     caTol = propSim->integBodies[j].caTol;
                     for (size_t k = 0; k < 3; k++) {
                         relPosOld[k] = xIntegOld[starti + k] - xIntegOld[startj + k];
                         relPos[k] = xInteg[starti + k] - xInteg[startj + k];
                         relVelOld[k] = xIntegOld[starti + 3 + k] - xIntegOld[startj + 3 + k];
                         relVel[k] = xInteg[starti + 3 + k] - xInteg[startj + 3 + k];
                     }
                 } else {
                     SpiceBody bodyj = propSim->spiceBodies[j - propSim->integParams.nInteg];
-                    centralBodyRadius = bodyj.radius;
+                    centralBodyRadius = bodyj.radius + get_atm_offset(bodyj.spiceId);
                     caTol = bodyj.caTol;
-                    const real atm_offset = 100.0e3/propSim->consts.du2m;
-                    centralBodyRadius += atm_offset;
                     double xSpice[9], xSpiceOld[9];
                     get_spk_state(bodyj.spiceId, t, propSim->spkEphem, xSpice);
                     get_spk_state(bodyj.spiceId, tOld, propSim->spkEphem, xSpiceOld);
                     for (size_t k = 0; k < 3; k++) {
                         relPosOld[k] = xIntegOld[starti + k] - xSpiceOld[k];
                         relPos[k] = xInteg[starti + k] - xSpice[k];
                         relVelOld[k] = xIntegOld[starti + 3 + k] - xSpiceOld[3 + k];
                         relVel[k] = xInteg[starti + 3 + k] - xSpice[3 + k];
                     }
                 }
-                relDistOld = sqrt(relPosOld[0] * relPosOld[0] +
-                                  relPosOld[1] * relPosOld[1] +
-                                  relPosOld[2] * relPosOld[2]);
-                relDist = sqrt(relPos[0] * relPos[0] + relPos[1] * relPos[1] +
-                               relPos[2] * relPos[2]);
-                // check impacts with spiceBodies first
-                if (j > propSim->integParams.nInteg &&
-                    relDist <= flybyBodyRadius + centralBodyRadius &&
-                    relDistOld > flybyBodyRadius + centralBodyRadius) {
-                    ImpactParameters impact;
-                    get_ca_or_impact_time(propSim, i, j, tOld, t, impact.t, impact_r_calc);
-                    impact.xRel = get_rel_state(propSim, i, j, impact.t);
-                    impact.flybyBodyIdx = i;
-                    impact.centralBodyIdx = j;
-                    impact.get_ca_parameters(propSim, impact.t);
-                    impact.get_impact_parameters(propSim);
-                    impact.impact = true;
-                    propSim->impactParams.push_back(impact);
-                    // std::cout << "Impact detected at MJD " << impact.t
-                    //             << " TDB. " << impact.flybyBody
-                    //             << " collided with " << impact.centralBody
-                    //             << "!" << std::endl;
-                }
+                const real relDistOld = sqrt(relPosOld[0] * relPosOld[0] +
+                                             relPosOld[1] * relPosOld[1] +
+                                             relPosOld[2] * relPosOld[2]);
+                const real relDist =
+                    sqrt(relPos[0] * relPos[0] + relPos[1] * relPos[1] +
+                         relPos[2] * relPos[2]);
                 // check close approach
-                real radialVel, radialVelOld;
-                radialVelOld =
+                const real radialVelOld =
                     (relPosOld[0] * relVelOld[0] + relPosOld[1] * relVelOld[1] +
                      relPosOld[2] * relVelOld[2]) /
                     relDistOld;
-                radialVel = (relPos[0] * relVel[0] + relPos[1] * relVel[1] +
-                             relPos[2] * relVel[2]) /
+                const real radialVel =
+                    (relPos[0] * relVel[0] + relPos[1] * relVel[1] +
+                     relPos[2] * relVel[2]) /
                     relDist;
                 const bool relDistMinimum = (forwardProp && radialVelOld < 0.0 && radialVel >= 0.0) ||
                                             (backwardProp && radialVelOld > 0.0 && radialVel <= 0.0);
-                if (j < propSim->integParams.nInteg) {
-                    caTol = propSim->integBodies[j].caTol;
-                } else {
-                    caTol = propSim->spiceBodies[j - propSim->integParams.nInteg].caTol;
-                }
                 const bool relDistWithinTol = relDist <= caTol || relDistOld <= caTol;
                 if (relDistMinimum && relDistWithinTol) {
                     CloseApproachParameters ca;
                     get_ca_or_impact_time(propSim, i, j, tOld, t, ca.t, ca_rdot_calc);
                     ca.xRel = get_rel_state(propSim, i, j, ca.t);
+                    ca.tCA = ca.t;
+                    ca.xRelCA = ca.xRel;
                     ca.flybyBodyIdx = i;
                     ca.centralBodyIdx = j;
                     ca.get_ca_parameters(propSim, ca.t);
                     propSim->caParams.push_back(ca);
+                    if (ca.impact){
+                        ImpactParameters impact;
+                        get_ca_or_impact_time(propSim, i, j, tOld-1, ca.t, impact.t, impact_r_calc);
+                        impact.xRel = get_rel_state(propSim, i, j, impact.t);
+                        impact.tCA = ca.t;
+                        impact.xRelCA = ca.xRel;
+                        impact.flybyBodyIdx = i;
+                        impact.centralBodyIdx = j;
+                        impact.get_ca_parameters(propSim, impact.t);
+                        impact.get_impact_parameters(propSim);
+                        propSim->impactParams.push_back(impact);
+                        propSim->integBodies[i].logCA = false;
+                    }
                 }
             }
             if (j < propSim->integParams.nInteg) {
                 startj += 2*propSim->integBodies[j].n2Derivs;
             }
         }
         starti += 2*propSim->integBodies[i].n2Derivs;
@@ -141,17 +155,16 @@
     real relDist =
         sqrt(xRel[0] * xRel[0] + xRel[1] * xRel[1] + xRel[2] * xRel[2]);
     real flybyBodyRadius, centralBodyRadius;
     flybyBodyRadius = propSim->integBodies[i].radius;
     if (j < propSim->integParams.nInteg) {
         centralBodyRadius = propSim->integBodies[j].radius;
     } else {
-        centralBodyRadius = propSim->spiceBodies[j - propSim->integParams.nInteg].radius;
-        const real atm_offset = 100.0e3/propSim->consts.du2m;
-        centralBodyRadius += atm_offset;
+        const SpiceBody bodyj = propSim->spiceBodies[j - propSim->integParams.nInteg];
+        centralBodyRadius = bodyj.radius + get_atm_offset(bodyj.spiceId);
     }
     r = relDist - flybyBodyRadius - centralBodyRadius;
 }
 
 /**
  * @param[in] propSim PropSimulation object for the integration.
  * @param[in] i Index of the first body.
@@ -203,29 +216,34 @@
                            const size_t &j, const real &x1, const real &x2,
                            real &tCA,
                            void (*zero_func)(PropSimulation *, const size_t &,
                                              const size_t &, const real &,
                                              real &)) {
     // Brent's method for root finding, from Numerical Recipes in C/C++, 3rd
     // edition, p. 454
+    // make sure x1 and x2 are not nan
+    if (std::isnan(x1) || std::isnan(x2)) {
+        std::cout << "x1: " << x1 << " x2: " << x2 << std::endl;
+        throw std::runtime_error("get_ca_or_impact_time: One of the interval points is nan.");
+    }
     const real tol = 1.0e-6 / 86400.0;  // 1 microsecond
     const size_t maxIter = 100;
     const real eps = std::numeric_limits<real>::epsilon();
     real a = x1;
     real b = x2;
     real c = x2;
     real d = 0.0;
     real e = 0.0;
     real min1, min2;
     real fa, fb, fc, p, q, r, s, tol1, xm;
     zero_func(propSim, i, j, a, fa);
     zero_func(propSim, i, j, b, fb);
     if ((fa > 0.0 && fb > 0.0) || (fa < 0.0 && fb < 0.0)) {
         std::cout << "t1: " << x1 << " t2: " << x2 << " f1: " << fa << " f2: " << fb << std::endl;
-        throw std::runtime_error("Root must be bracketed in get_ca_or_impact_time");
+        throw std::runtime_error("get_ca_or_impact_time: Root must be bracketed.");
     }
     fc = fb;
     size_t iter;
     for (iter = 0; iter < maxIter; ++iter) {
         if ((fb > 0.0 && fc > 0.0) || (fb < 0.0 && fc < 0.0)) {
             c = a;
             fc = fa;
@@ -279,15 +297,16 @@
             b += d;
         } else {
             b += (xm > 0.0 ? fabs(tol1) : -fabs(tol1));
         }
         zero_func(propSim, i, j, b, fb);
     }
     std::cout << "WARNING: Maximum number of iterations exceeded in "
-                 "get_ca_or_impact_time!!! Impact/CA time may not be accurate.";
+                 "get_ca_or_impact_time!!! Impact/CA time may not be accurate."
+                << std::endl;
 }
 
 /**
  * @param[in] propSim PropSimulation object.
  * @param[in] tMap Time of the B-plane map.
  */
 void CloseApproachParameters::get_ca_parameters(PropSimulation *propSim, const real &tMap) {
@@ -308,14 +327,15 @@
         this->centralBody =
             propSim->spiceBodies[j - propSim->integParams.nInteg].name;
         this->centralBodySpiceId =
             propSim->spiceBodies[j - propSim->integParams.nInteg].spiceId;
         mu = propSim->spiceBodies[j - propSim->integParams.nInteg].mass *
             propSim->consts.G;
         radius = propSim->spiceBodies[j - propSim->integParams.nInteg].radius;
+        radius += get_atm_offset(this->centralBodySpiceId);
     }
     // calculate B-plane parameters (Kizner B.R, B.T formulation)
     const real r = sqrt(xRelMap[0] * xRelMap[0] + xRelMap[1] * xRelMap[1] +
                         xRelMap[2] * xRelMap[2]);
     this->dist = r;
     const real v = sqrt(xRelMap[3] * xRelMap[3] + xRelMap[4] * xRelMap[4] +
                         xRelMap[5] * xRelMap[5]);
@@ -344,44 +364,50 @@
     }
     const real fac1 = 1 / e;
     const real fac2 = sqrt(e * e - 1);
     real sHat[3];
     for (size_t k = 0; k < 3; k++) {
         sHat[k] = fac1 * pHat[k] + fac1 * fac2 * qHat[k];
     }
-    real sHatCrossHVec[3], bVec[3], b;
+    real sHatCrossHVec[3], bVec[3];
     vcross(sHat, hVec, sHatCrossHVec);
     for (size_t k = 0; k < 3; k++) {
         bVec[k] = sHatCrossHVec[k] / vInf;
         this->bVec[k] = bVec[k];
     }
-    vnorm(bVec, 3, b);
-    this->bMag = b;
+    vnorm(bVec, 3, this->bMag);
     real vVec[3];
     vVec[0] = 0;
     vVec[1] = 0;
     vVec[2] = -1;
     real rHat[3], tHat[3], vCrossSHatVec[3];
     vcross(vVec, sHat, vCrossSHatVec);
     vunit(vCrossSHatVec, 3, tHat);
     vcross(sHat, tHat, rHat);
     vdot(bVec, rHat, 3, this->kizner.x);
     vdot(bVec, tHat, 3, this->kizner.y);
     vdot(bVec, sHat, 3, this->kizner.z);
     this->gravFocusFactor = sqrt(1.0 + 2 * mu / radius / vInf / vInf);
-    this->impact = b <= radius * this->gravFocusFactor;
+    this->impact = this->bMag <= radius * this->gravFocusFactor;
+    // if vInf is nan, compute distance at CA and check for impact
+    if (std::isnan(vInf)) {
+        const real distCA = sqrt(this->xRelCA[0] * this->xRelCA[0] +
+                                 this->xRelCA[1] * this->xRelCA[1] +
+                                 this->xRelCA[2] * this->xRelCA[2]);
+        this->impact = distCA <= radius;
+    }
     this->scaled.x = this->kizner.x / this->gravFocusFactor;
     this->scaled.y = this->kizner.y / this->gravFocusFactor;
     this->scaled.z = this->kizner.z / this->gravFocusFactor;
     real posDotVel;
     vdot(pos, vel, 3, posDotVel);
     const real sinhF = vInf*posDotVel/mu/e;
     const real F = asinh(sinhF); // or F = -log(2*r/a/e);
     const real n = sqrt(-mu / a / a / a);
-    this->tPeri = tMap + (F - e*sinhF)/n;
+    this->tPeri = tMap - (e*sinhF - F)/n;
     this->tLin = this->tPeri - log(e) / n;
     // calculate B-plane parameters (Öpik xi, zeta formulation)
     double xCentralBody[9];
     get_spk_state(this->centralBodySpiceId, tMap, propSim->spkEphem, xCentralBody);
     double xSun[9];
     get_spk_state(10, tMap, propSim->spkEphem, xSun);
     real vCentralBodyHelio[3];
@@ -395,30 +421,30 @@
     for (size_t k = 0; k < 3; k++) {
         zetaHat[k] *= -1;
     }
     vdot(bVec, xiHat, 3, this->opik.x);
     vdot(bVec, zetaHat, 3, this->opik.y);
     vdot(bVec, sHat, 3, this->opik.z);
     real posCA[3], velCA[3];
-    posCA[0] = this->xRel[0];
-    posCA[1] = this->xRel[1];
-    posCA[2] = this->xRel[2];
-    velCA[0] = this->xRel[3];
-    velCA[1] = this->xRel[4];
-    velCA[2] = this->xRel[5];
+    posCA[0] = this->xRelCA[0];
+    posCA[1] = this->xRelCA[1];
+    posCA[2] = this->xRelCA[2];
+    velCA[0] = this->xRelCA[3];
+    velCA[1] = this->xRelCA[4];
+    velCA[2] = this->xRelCA[5];
     real eHatX[3], eHatY[3], eHatZ[3], vVecCrosseHatZ[3];
     vunit(velCA, 3, eHatZ);
     vcross(vVec, eHatZ, vVecCrosseHatZ);
     vunit(vVecCrosseHatZ, 3, eHatY);
     vcross(eHatY, eHatZ, eHatX);
     vdot(posCA, eHatX, 3, this->mtp.x);
     vdot(posCA, eHatY, 3, this->mtp.y);
     vdot(posCA, eHatZ, 3, this->mtp.z);
 
-    if (tMap == this->t && propSim->integBodies[i].propStm == true){
+    if (tMap == this->tCA && propSim->integBodies[i].propStm == true){
         real **partial_r_vec = new real*[6];
         real **partial_v_vec = new real*[6];
         for (size_t k = 0; k < 6; k++) {
             partial_r_vec[k] = new real[3];
             partial_r_vec[k][0] = 0;
             partial_r_vec[k][1] = 0;
             partial_r_vec[k][2] = 0;
```

### Comparing `grss-4.0.1/src/elements.cpp` & `grss-4.0.2/src/elements.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/src/force.cpp` & `grss-4.0.2/src/force.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/src/gr15.cpp` & `grss-4.0.2/src/gr15.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/src/grss.cpp` & `grss-4.0.2/src/grss.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -927,15 +927,15 @@
         .def("set_integration_parameters",
              &PropSimulation::set_integration_parameters, py::arg("tf"),
              py::arg("tEval") = std::vector<real>(),
              py::arg("tEvalUTC") = false, py::arg("evalApparentState") = false,
              py::arg("convergedLightTims") = false,
              py::arg("observerInfo") = std::vector<std::vector<real>>(),
              py::arg("adaptiveTimestep") = true, py::arg("dt0") = 0.0L,
-             py::arg("dtMax") = 21.0L, py::arg("dtMin") = 5.0e-3L,
+             py::arg("dtMax") = 21.0L, py::arg("dtMin") = 1.0e-4L,
              py::arg("dtChangeFactor") = 0.25L, py::arg("tolInteg") = 1.0e-11L,
              py::arg("tolPC") = 1.0e-16L, R"mydelimiter(
             Sets the integration parameters.
 
             Parameters
             ----------
             tf : real
```

### Comparing `grss-4.0.1/src/interpolate.cpp` & `grss-4.0.2/src/interpolate.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -103,23 +103,23 @@
     size_t idx = 0;
     const bool forwardProp = this->integParams.t0 < this->integParams.tf;
     const bool backwardProp = this->integParams.t0 > this->integParams.tf;
     if (forwardProp) {
         if (t+this->tEvalMargin < this->integParams.t0 || t-this->tEvalMargin > this->integParams.tf) {
             throw std::runtime_error("The interpolation time is outside the integration time window");
         }
-        while (idx < this->interpParams.tStack.size()-1 &&
+        while (idx < this->interpParams.bStack.size()-1 &&
                this->interpParams.tStack[idx+1] < t) {
             idx++;
         }
     } else if (backwardProp) {
         if (t-this->tEvalMargin > this->integParams.t0 || t+this->tEvalMargin < this->integParams.tf) {
             throw std::runtime_error("The interpolation time is outside the integration time window");
         }
-        while (idx < this->interpParams.tStack.size()-1 &&
+        while (idx < this->interpParams.bStack.size()-1 &&
                this->interpParams.tStack[idx+1] > t) {
             idx++;
         }
     }
     const real t0 = this->interpParams.tStack[idx];
     real dt;
     if (idx == this->interpParams.tStack.size() - 1) {
```

### Comparing `grss-4.0.1/src/parallel.cpp` & `grss-4.0.2/src/parallel.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/src/pck.cpp` & `grss-4.0.2/src/pck.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/src/simulation.cpp` & `grss-4.0.2/src/simulation.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/src/spk.cpp` & `grss-4.0.2/src/spk.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/src/stm.cpp` & `grss-4.0.2/src/stm.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/src/timeconvert.cpp` & `grss-4.0.2/src/timeconvert.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/src/utilities.cpp` & `grss-4.0.2/src/utilities.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/tests/cpp/prop/CMakeLists.txt` & `grss-4.0.2/tests/cpp/prop/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/tests/cpp/prop/apophis.cpp` & `grss-4.0.2/tests/cpp/prop/apophis.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/tests/cpp/prop/didymos.cpp` & `grss-4.0.2/tests/cpp/prop/didymos.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/tests/cpp/prop/pck_map.cpp` & `grss-4.0.2/tests/cpp/prop/pck_map.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/tests/cpp/prop/spk_map.cpp` & `grss-4.0.2/tests/cpp/prop/spk_map.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/tests/python/fit/chesley.ipynb` & `grss-4.0.2/tests/python/fit/chesley.ipynb`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/tests/python/fit/eggl.ipynb` & `grss-4.0.2/tests/python/fit/eggl.ipynb`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/tests/python/fit/farnocchia.ipynb` & `grss-4.0.2/tests/python/fit/farnocchia.ipynb`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/tests/python/fit/shantanunaidu.ipynb` & `grss-4.0.2/tests/python/fit/shantanunaidu.ipynb`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/tests/python/prop/apophis.ipynb` & `grss-4.0.2/tests/python/prop/apophis.ipynb`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/tests/python/prop/didymos.ipynb` & `grss-4.0.2/tests/python/prop/didymos.ipynb`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/tests/python/prop/icarus.ipynb` & `grss-4.0.2/tests/python/prop/icarus.ipynb`

 * *Files identical despite different names*

### Comparing `grss-4.0.1/tests/python/prop/moshup.ipynb` & `grss-4.0.2/tests/python/prop/moshup.ipynb`

 * *Files identical despite different names*

