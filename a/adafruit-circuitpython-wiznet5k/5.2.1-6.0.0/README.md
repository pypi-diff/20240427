# Comparing `tmp/adafruit_circuitpython_wiznet5k-5.2.1.tar.gz` & `tmp/adafruit_circuitpython_wiznet5k-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit_circuitpython_wiznet5k-5.2.1.tar", last modified: Mon Apr 22 22:38:29 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_wiznet5k-6.0.0.tar", last modified: Sat Apr 27 13:58:59 2024, max compression
```

## Comparing `adafruit_circuitpython_wiznet5k-5.2.1.tar` & `adafruit_circuitpython_wiznet5k-6.0.0.tar`

### file list

```diff
@@ -1,61 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:38:29.540271 adafruit_circuitpython_wiznet5k-5.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:38:29.528271 adafruit_circuitpython_wiznet5k-5.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:38:29.532271 adafruit_circuitpython_wiznet5k-5.2.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:38:29.532271 adafruit_circuitpython_wiznet5k-5.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:38:29.532271 adafruit_circuitpython_wiznet5k-5.2.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-04-22 22:38:29.540271 adafruit_circuitpython_wiznet5k-5.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:38:29.540271 adafruit_circuitpython_wiznet5k-5.2.1/adafruit_circuitpython_wiznet5k.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-04-22 22:38:29.000000 adafruit_circuitpython_wiznet5k-5.2.1/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-22 22:38:29.000000 adafruit_circuitpython_wiznet5k-5.2.1/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:38:29.000000 adafruit_circuitpython_wiznet5k-5.2.1/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-22 22:38:29.000000 adafruit_circuitpython_wiznet5k-5.2.1/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 22:38:29.000000 adafruit_circuitpython_wiznet5k-5.2.1/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:38:29.536271 adafruit_circuitpython_wiznet5k-5.2.1/adafruit_wiznet5k/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 22:38:27.000000 adafruit_circuitpython_wiznet5k-5.2.1/adafruit_wiznet5k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51779 2024-04-22 22:38:27.000000 adafruit_circuitpython_wiznet5k-5.2.1/adafruit_wiznet5k/adafruit_wiznet5k.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-22 22:38:27.000000 adafruit_circuitpython_wiznet5k-5.2.1/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    26273 2024-04-22 22:38:27.000000 adafruit_circuitpython_wiznet5k-5.2.1/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11431 2024-04-22 22:38:27.000000 adafruit_circuitpython_wiznet5k-5.2.1/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
--rw-r--r--   0 runner    (1001) docker     (127)    29955 2024-04-22 22:38:27.000000 adafruit_circuitpython_wiznet5k-5.2.1/adafruit_wiznet5k/adafruit_wiznet5k_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-04-22 22:38:27.000000 adafruit_circuitpython_wiznet5k-5.2.1/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:38:29.536271 adafruit_circuitpython_wiznet5k-5.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:38:29.536271 adafruit_circuitpython_wiznet5k-5.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:38:29.540271 adafruit_circuitpython_wiznet5k-5.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-22 22:38:27.000000 adafruit_circuitpython_wiznet5k-5.2.1/examples/wiznet5k_aio_post.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2159 2024-04-22 22:38:27.000000 adafruit_circuitpython_wiznet5k-5.2.1/examples/wiznet5k_cheerlights.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1085 2024-04-22 22:38:27.000000 adafruit_circuitpython_wiznet5k-5.2.1/examples/wiznet5k_cpython_client_for_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-22 22:38:27.000000 adafruit_circuitpython_wiznet5k-5.2.1/examples/wiznet5k_httpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-22 22:38:27.000000 adafruit_circuitpython_wiznet5k-5.2.1/examples/wiznet5k_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-22 22:38:27.000000 adafruit_circuitpython_wiznet5k-5.2.1/examples/wiznet5k_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-22 22:38:27.000000 adafruit_circuitpython_wiznet5k-5.2.1/examples/wiznet5k_simpletest_manual_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-22 22:38:27.000000 adafruit_circuitpython_wiznet5k-5.2.1/examples/wiznet5k_wsgiserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-22 22:38:27.000000 adafruit_circuitpython_wiznet5k-5.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-22 22:38:20.000000 adafruit_circuitpython_wiznet5k-5.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:38:29.540271 adafruit_circuitpython_wiznet5k-5.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.212026 adafruit_circuitpython_wiznet5k-6.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.204026 adafruit_circuitpython_wiznet5k-6.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.208026 adafruit_circuitpython_wiznet5k-6.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.208026 adafruit_circuitpython_wiznet5k-6.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.208026 adafruit_circuitpython_wiznet5k-6.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-27 13:58:59.212026 adafruit_circuitpython_wiznet5k-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.212026 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_circuitpython_wiznet5k.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-27 13:58:59.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-27 13:58:59.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 13:58:59.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-27 13:58:59.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 13:58:59.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.212026 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51779 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26273 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11431 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29999 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k_socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.212026 adafruit_circuitpython_wiznet5k-6.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.212026 adafruit_circuitpython_wiznet5k-6.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.212026 adafruit_circuitpython_wiznet5k-6.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_aio_post.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2159 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_cheerlights.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1085 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_cpython_client_for_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_httpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_simpletest_manual_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 13:58:59.212026 adafruit_circuitpython_wiznet5k-6.0.0/setup.cfg
```

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_wiznet5k-6.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/.gitignore` & `adafruit_circuitpython_wiznet5k-6.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/.pre-commit-config.yaml` & `adafruit_circuitpython_wiznet5k-6.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/.pylintrc` & `adafruit_circuitpython_wiznet5k-6.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_wiznet5k-6.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/LICENSE` & `adafruit_circuitpython_wiznet5k-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_wiznet5k-6.0.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/LICENSES/MIT.txt` & `adafruit_circuitpython_wiznet5k-6.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/LICENSES/Unlicense.txt` & `adafruit_circuitpython_wiznet5k-6.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/PKG-INFO` & `adafruit_circuitpython_wiznet5k-6.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wiznet5k
-Version: 5.2.1
+Version: 6.0.0
 Summary: Pure-Python interface for WIZNET 5k ethernet modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
 Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -125,78 +125,14 @@
     print('-'*40)
     print(r.json())
     print('-'*40)
     r.close()
 
     print("Done!")
 
-This example demonstrates a simple web server that allows setting the Neopixel color.
-
-.. code-block:: python
-
-    import board
-    import busio
-    import digitalio
-    import neopixel
-
-    from adafruit_wiznet5k.adafruit_wiznet5k import WIZNET5K
-    import adafruit_wiznet5k.adafruit_wiznet5k_wsgiserver as server
-    from adafruit_wsgi.wsgi_app import WSGIApp
-
-    print("Wiznet5k Web Server Test")
-
-    # Status LED
-    led = neopixel.NeoPixel(board.NEOPIXEL, 1)
-    led.brightness = 0.3
-    led[0] = (0, 0, 255)
-
-    # W5500 connections
-    cs = digitalio.DigitalInOut(board.D10)
-    spi_bus = busio.SPI(board.SCK, MOSI=board.MOSI, MISO=board.MISO)
-
-    # Initialize Ethernet interface with DHCP
-    eth = WIZNET5K(spi_bus, cs)
-
-    # Here we create our application, registering the
-    # following functions to be called on specific HTTP GET requests routes
-
-    web_app = WSGIApp()
-
-    @web_app.route("/led/<r>/<g>/<b>")
-    def led_on(request, r, g, b):
-        print("LED handler")
-        led.fill((int(r), int(g), int(b)))
-        return ("200 OK", [], ["LED set!"])
-
-    @web_app.route("/")
-    def root(request):
-        print("Root handler")
-        return ("200 OK", [], ["Root document"])
-
-    @web_app.route("/large")
-    def large(request):
-        print("Large pattern handler")
-        return ("200 OK", [], ["*-.-" * 2000])
-
-
-    # Here we setup our server, passing in our web_app as the application
-    server.set_interface(eth)
-    wsgiServer = server.WSGIServer(80, application=web_app)
-
-    print("Open this IP in your browser: ", eth.pretty_ip(eth.ip_address))
-
-    # Start the server
-    wsgiServer.start()
-    while True:
-        # Our main loop where we have the server poll for incoming requests
-        wsgiServer.update_poll()
-        # Maintain DHCP lease
-        eth.maintain_dhcp_lease()
-        # Could do any other background tasks here, like reading sensors
-
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/wiznet5k/en/latest/>`_.
 
 For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/README.rst` & `adafruit_circuitpython_wiznet5k-6.0.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: adafruit-circuitpython-wiznet5k
+Version: 6.0.0
+Summary: Pure-Python interface for WIZNET 5k ethernet modules.
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
+License: MIT
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
+Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
+Classifier: Topic :: System :: Hardware
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: Adafruit-Blinka
+Requires-Dist: adafruit-circuitpython-busdevice
+Requires-Dist: adafruit-circuitpython-ticks
+Provides-Extra: optional
+
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/wiznet5k/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/wiznet5k/en/latest/
     :alt: Documentation Status
 
@@ -104,78 +125,14 @@
     print('-'*40)
     print(r.json())
     print('-'*40)
     r.close()
 
     print("Done!")
 
-This example demonstrates a simple web server that allows setting the Neopixel color.
-
-.. code-block:: python
-
-    import board
-    import busio
-    import digitalio
-    import neopixel
-
-    from adafruit_wiznet5k.adafruit_wiznet5k import WIZNET5K
-    import adafruit_wiznet5k.adafruit_wiznet5k_wsgiserver as server
-    from adafruit_wsgi.wsgi_app import WSGIApp
-
-    print("Wiznet5k Web Server Test")
-
-    # Status LED
-    led = neopixel.NeoPixel(board.NEOPIXEL, 1)
-    led.brightness = 0.3
-    led[0] = (0, 0, 255)
-
-    # W5500 connections
-    cs = digitalio.DigitalInOut(board.D10)
-    spi_bus = busio.SPI(board.SCK, MOSI=board.MOSI, MISO=board.MISO)
-
-    # Initialize Ethernet interface with DHCP
-    eth = WIZNET5K(spi_bus, cs)
-
-    # Here we create our application, registering the
-    # following functions to be called on specific HTTP GET requests routes
-
-    web_app = WSGIApp()
-
-    @web_app.route("/led/<r>/<g>/<b>")
-    def led_on(request, r, g, b):
-        print("LED handler")
-        led.fill((int(r), int(g), int(b)))
-        return ("200 OK", [], ["LED set!"])
-
-    @web_app.route("/")
-    def root(request):
-        print("Root handler")
-        return ("200 OK", [], ["Root document"])
-
-    @web_app.route("/large")
-    def large(request):
-        print("Large pattern handler")
-        return ("200 OK", [], ["*-.-" * 2000])
-
-
-    # Here we setup our server, passing in our web_app as the application
-    server.set_interface(eth)
-    wsgiServer = server.WSGIServer(80, application=web_app)
-
-    print("Open this IP in your browser: ", eth.pretty_ip(eth.ip_address))
-
-    # Start the server
-    wsgiServer.start()
-    while True:
-        # Our main loop where we have the server poll for incoming requests
-        wsgiServer.update_poll()
-        # Maintain DHCP lease
-        eth.maintain_dhcp_lease()
-        # Could do any other background tasks here, like reading sensors
-
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/wiznet5k/en/latest/>`_.
 
 For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt` & `adafruit_circuitpython_wiznet5k-6.0.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
 adafruit_wiznet5k/__init__.py
 adafruit_wiznet5k/adafruit_wiznet5k.py
 adafruit_wiznet5k/adafruit_wiznet5k_debug.py
 adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
 adafruit_wiznet5k/adafruit_wiznet5k_dns.py
 adafruit_wiznet5k/adafruit_wiznet5k_socket.py
-adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py
 docs/api.rst
 docs/api.rst.license
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
@@ -41,9 +40,8 @@
 docs/_static/favicon.ico.license
 examples/wiznet5k_aio_post.py
 examples/wiznet5k_cheerlights.py
 examples/wiznet5k_cpython_client_for_simpleserver.py
 examples/wiznet5k_httpserver.py
 examples/wiznet5k_simpleserver.py
 examples/wiznet5k_simpletest.py
-examples/wiznet5k_simpletest_manual_network.py
-examples/wiznet5k_wsgiserver.py
+examples/wiznet5k_simpletest_manual_network.py
```

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/adafruit_wiznet5k/adafruit_wiznet5k.py` & `adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         import digitalio
 
         IpAddress4Raw = Union[bytes, Tuple[int, int, int, int]]
         MacAddressRaw = Union[bytes, Tuple[int, int, int, int, int, int]]
 except ImportError:
     pass
 
-__version__ = "5.2.1"
+__version__ = "6.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k.git"
 
 from random import randint
 import time
 import gc
 from micropython import const
 from adafruit_ticks import ticks_ms, ticks_diff
```

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/adafruit_wiznet5k/adafruit_wiznet5k_debug.py` & `adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py` & `adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/adafruit_wiznet5k/adafruit_wiznet5k_dns.py` & `adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/adafruit_wiznet5k/adafruit_wiznet5k_socket.py` & `adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k_socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,15 @@
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         _the_interface.release_socket(self._socknum)
         if self._sock_type == SOCK_STREAM:
             _the_interface.write_snir(
-                self._socknum, 0xFF
+                self._socknum, 0xFF & (~wiznet5k.adafruit_wiznet5k.SNIR_DISCON)
             )  # Reset socket interrupt register.
             _the_interface.socket_disconnect(self._socknum)
             mask = (
                 wiznet5k.adafruit_wiznet5k.SNIR_TIMEOUT
                 | wiznet5k.adafruit_wiznet5k.SNIR_DISCON
             )
             while not _the_interface.read_snir(self._socknum) & mask:
```

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/docs/_static/favicon.ico` & `adafruit_circuitpython_wiznet5k-6.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/docs/conf.py` & `adafruit_circuitpython_wiznet5k-6.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/docs/index.rst` & `adafruit_circuitpython_wiznet5k-6.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/examples/wiznet5k_aio_post.py` & `adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/examples/wiznet5k_cheerlights.py` & `adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/examples/wiznet5k_cpython_client_for_simpleserver.py` & `adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_cpython_client_for_simpleserver.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/examples/wiznet5k_httpserver.py` & `adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_httpserver.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/examples/wiznet5k_simpleserver.py` & `adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_simpleserver.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/examples/wiznet5k_simpletest.py` & `adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/examples/wiznet5k_simpletest_manual_network.py` & `adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_simpletest_manual_network.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-5.2.1/pyproject.toml` & `adafruit_circuitpython_wiznet5k-6.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-wiznet5k"
 description = "Pure-Python interface for WIZNET 5k ethernet modules."
-version = "5.2.1"
+version = "6.0.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k"}
 keywords = [
     "adafruit",
```

