# Comparing `tmp/geojp-0.0.3.tar.gz` & `tmp/geojp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geojp-0.0.3.tar", last modified: Fri Mar  1 04:27:58 2024, max compression
+gzip compressed data, was "geojp-0.0.4.tar", last modified: Sat Apr 27 02:19:20 2024, max compression
```

## Comparing `geojp-0.0.3.tar` & `geojp-0.0.4.tar`

### file list

```diff
@@ -1,57 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:27:58.653726 geojp-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-01 04:27:47.000000 geojp-0.0.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:27:58.645726 geojp-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:27:58.649726 geojp-0.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-01 04:27:47.000000 geojp-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-01 04:27:47.000000 geojp-0.0.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-01 04:27:47.000000 geojp-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:27:58.649726 geojp-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-03-01 04:27:47.000000 geojp-0.0.3/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-01 04:27:47.000000 geojp-0.0.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-01 04:27:47.000000 geojp-0.0.3/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-01 04:27:47.000000 geojp-0.0.3/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-01 04:27:47.000000 geojp-0.0.3/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-03-01 04:27:47.000000 geojp-0.0.3/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-01 04:27:47.000000 geojp-0.0.3/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-01 04:27:47.000000 geojp-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 04:27:47.000000 geojp-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-01 04:27:47.000000 geojp-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-01 04:27:58.653726 geojp-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-01 04:27:47.000000 geojp-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:27:58.649726 geojp-0.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:27:58.649726 geojp-0.0.3/docs/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    33077 2024-03-01 04:27:47.000000 geojp-0.0.3/docs/Notebooks/lab4.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-01 04:27:47.000000 geojp-0.0.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-01 04:27:47.000000 geojp-0.0.3/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-03-01 04:27:47.000000 geojp-0.0.3/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:27:58.649726 geojp-0.0.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-01 04:27:47.000000 geojp-0.0.3/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-01 04:27:47.000000 geojp-0.0.3/docs/examples/random.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-01 04:27:47.000000 geojp-0.0.3/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-01 04:27:47.000000 geojp-0.0.3/docs/geojp.md
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-01 04:27:47.000000 geojp-0.0.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-01 04:27:47.000000 geojp-0.0.3/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:27:58.649726 geojp-0.0.3/docs/labs/
--rw-r--r--   0 runner    (1001) docker     (127)    33077 2024-03-01 04:27:47.000000 geojp-0.0.3/docs/labs/lab4.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:27:58.649726 geojp-0.0.3/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-01 04:27:47.000000 geojp-0.0.3/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-01 04:27:47.000000 geojp-0.0.3/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:27:58.653726 geojp-0.0.3/geojp/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-01 04:27:47.000000 geojp-0.0.3/geojp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-01 04:27:47.000000 geojp-0.0.3/geojp/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-01 04:27:47.000000 geojp-0.0.3/geojp/geojp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:27:58.653726 geojp-0.0.3/geojp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-01 04:27:58.000000 geojp-0.0.3/geojp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-01 04:27:58.000000 geojp-0.0.3/geojp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 04:27:58.000000 geojp-0.0.3/geojp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-01 04:27:58.000000 geojp-0.0.3/geojp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-01 04:27:58.000000 geojp-0.0.3/geojp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-01 04:27:58.000000 geojp-0.0.3/geojp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-03-01 04:27:47.000000 geojp-0.0.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-01 04:27:47.000000 geojp-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-01 04:27:47.000000 geojp-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-01 04:27:47.000000 geojp-0.0.3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 04:27:58.653726 geojp-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:27:58.653726 geojp-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-01 04:27:47.000000 geojp-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-01 04:27:47.000000 geojp-0.0.3/tests/test_geojp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:19:20.280889 geojp-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-27 02:19:05.000000 geojp-0.0.4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:19:20.264889 geojp-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:19:20.268889 geojp-0.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-27 02:19:05.000000 geojp-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-27 02:19:05.000000 geojp-0.0.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-27 02:19:05.000000 geojp-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:19:20.268889 geojp-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-27 02:19:05.000000 geojp-0.0.4/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-27 02:19:05.000000 geojp-0.0.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-27 02:19:05.000000 geojp-0.0.4/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-27 02:19:05.000000 geojp-0.0.4/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-27 02:19:05.000000 geojp-0.0.4/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-27 02:19:05.000000 geojp-0.0.4/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-27 02:19:05.000000 geojp-0.0.4/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-27 02:19:05.000000 geojp-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 02:19:05.000000 geojp-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-27 02:19:05.000000 geojp-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-27 02:19:20.280889 geojp-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-27 02:19:05.000000 geojp-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:19:20.272889 geojp-0.0.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:19:20.272889 geojp-0.0.4/docs/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/Notebooks/cats.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/Notebooks/dogs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/Notebooks/guest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/Notebooks/guest_book.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   781385 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/Notebooks/gutenberg_file.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    33077 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/Notebooks/lab4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    55075 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/Notebooks/lab5.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/Notebooks/learning_python.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/Notebooks/poll_responses.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:19:20.276889 geojp-0.0.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/examples/csv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/examples/image.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/examples/ipyleaflet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/examples/map.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/examples/random.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/examples/raster.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/geojp.md
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:19:20.276889 geojp-0.0.4/docs/labs/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/labs/cats.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/labs/dogs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/labs/guest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/labs/guest_book.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   781385 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/labs/gutenberg_file.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    33077 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/labs/lab4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    55075 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/labs/lab5.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/labs/learning_python.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/labs/poll_responses.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:19:20.276889 geojp-0.0.4/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-27 02:19:05.000000 geojp-0.0.4/docs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:19:20.276889 geojp-0.0.4/geojp/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-27 02:19:05.000000 geojp-0.0.4/geojp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-27 02:19:05.000000 geojp-0.0.4/geojp/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-27 02:19:05.000000 geojp-0.0.4/geojp/foliumap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-27 02:19:05.000000 geojp-0.0.4/geojp/geojp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-27 02:19:05.000000 geojp-0.0.4/geojp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:19:20.280889 geojp-0.0.4/geojp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-27 02:19:20.000000 geojp-0.0.4/geojp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-27 02:19:20.000000 geojp-0.0.4/geojp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 02:19:20.000000 geojp-0.0.4/geojp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-27 02:19:20.000000 geojp-0.0.4/geojp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-27 02:19:20.000000 geojp-0.0.4/geojp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-27 02:19:20.000000 geojp-0.0.4/geojp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-27 02:19:05.000000 geojp-0.0.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-27 02:19:05.000000 geojp-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-27 02:19:05.000000 geojp-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-27 02:19:05.000000 geojp-0.0.4/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 02:19:20.280889 geojp-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 02:19:20.280889 geojp-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-27 02:19:05.000000 geojp-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-27 02:19:05.000000 geojp-0.0.4/tests/test_geojp.py
```

### Comparing `geojp-0.0.3/.github/workflows/docs-build.yml` & `geojp-0.0.4/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `geojp-0.0.3/.github/workflows/docs.yml` & `geojp-0.0.4/.github/workflows/macos.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,40 @@
-name: docs
 on:
     push:
         branches:
             - main
+    pull_request:
+        branches:
+            - main
+
+name: macOS build
 jobs:
-    deploy:
-        runs-on: ubuntu-latest
-        steps:
-            - uses: actions/checkout@v4
-            - uses: actions/setup-python@v5
-              with:
-                  python-version: "3.11"
+    test-macOS:
+        runs-on: ${{ matrix.os }}
+        name: ${{ matrix.os }} (${{ matrix.python-version}})
 
-            - name: Install dependencies
-              run: |
-                  python -m pip install --upgrade pip
-                  pip install --user --no-cache-dir Cython
-                  pip install --user -r requirements.txt -r requirements_dev.txt
-                  pip install .
-            - name: Discover typos with codespell
-              run: |
-                  codespell --skip="*.csv,*.geojson,*.json,*.js,*.html,*cff,./.git" --ignore-words-list="aci,hist"
-            - name: PKG-TEST
-              run: |
-                  python -m unittest discover tests/
-            - run: mkdocs gh-deploy --force
+        strategy:
+            fail-fast: false
+            matrix:
+              os: ["macOS-latest"]
+              python-version: ["3.11"]
 
+        steps:
+          - name: Checkout code
+            uses: actions/checkout@v4
+      
+          - name: Set up Python
+            uses: actions/setup-python@v5
+            with:
+              python-version: ${{ matrix.python-version}}
+          - name: Install GDAL
+            run: |
+              brew install gdal
+          - name: Test GDAL installation
+            run: |
+              gdalinfo --version
+          - name: Install dependencies
+            run: |
+                python -m pip install --upgrade pip
+                pip install --no-cache-dir Cython
+                pip install -r requirements.txt
+                pip install .
```

### Comparing `geojp-0.0.3/.github/workflows/installation.yml` & `geojp-0.0.4/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `geojp-0.0.3/.github/workflows/macos.yml` & `geojp-0.0.4/.github/workflows/ubuntu.yml`

 * *Files 24% similar despite different names*

```diff
@@ -2,39 +2,44 @@
     push:
         branches:
             - main
     pull_request:
         branches:
             - main
 
-name: macOS build
+name: Linux build
 jobs:
-    test-macOS:
-        runs-on: ${{ matrix.os }}
-        name: ${{ matrix.os }} (${{ matrix.python-version}})
-
+    py-check:
+        runs-on: ${{ matrix.config.os }}
+        name: ${{ matrix.config.os }} (${{ matrix.config.py }})
         strategy:
             fail-fast: false
             matrix:
-              os: ["macOS-latest"]
-              python-version: ["3.11"]
-
+                config:
+                    - { os: ubuntu-latest, py: "3.8" }
+                    - { os: ubuntu-latest, py: "3.9" }
+                    - { os: ubuntu-latest, py: "3.10" }
+                    - { os: ubuntu-latest, py: "3.11" }
         steps:
-          - name: Checkout code
-            uses: actions/checkout@v4
-      
-          - name: Set up Python
-            uses: actions/setup-python@v5
-            with:
-              python-version: ${{ matrix.python-version}}
-          - name: Install GDAL
-            run: |
-              brew install gdal
-          - name: Test GDAL installation
-            run: |
-              gdalinfo --version
-          - name: Install dependencies
-            run: |
-                python -m pip install --upgrade pip
-                pip install --no-cache-dir Cython
-                pip install -r requirements.txt
-                pip install .
+            - name: Checkout Code
+              uses: actions/checkout@v4
+            - name: Setup Python
+              uses: actions/setup-python@v5
+              with:
+                  python-version: ${{ matrix.config.py }}
+            - name: Install GDAL
+              run: |
+                  python -m pip install --upgrade pip
+                  pip install --no-cache-dir Cython
+                  pip install --find-links=https://girder.github.io/large_image_wheels --no-cache GDAL
+            - name: Test GDAL installation
+              run: |
+                  python -c "from osgeo import gdal"
+                  gdalinfo --version
+            - name: Install dependencies
+              run: |
+                  pip install --user -r requirements.txt
+                  pip install .
+            - name: PKG-TEST
+              run: |
+                  python -m unittest discover tests/
+
```

### Comparing `geojp-0.0.3/.github/workflows/pypi.yml` & `geojp-0.0.4/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `geojp-0.0.3/.github/workflows/windows.yml` & `geojp-0.0.4/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `geojp-0.0.3/.gitignore` & `geojp-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `geojp-0.0.3/PKG-INFO` & `geojp-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geojp
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package for my Geospacial Analysis class
 Author-email: Brycen Harris <bharri94@vols.utk.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/BrycenHarris/geojp
 Keywords: geojp
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
+Requires-Dist: ipyleaflet
 Provides-Extra: all
 Requires-Dist: geojp[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # Welcome to geojp
 ![](https://oyster.ignimgs.com/wordpress/stg.ign.com/2013/04/JurassicPark_040413_1600.jpg?width=1920)
```

### Comparing `geojp-0.0.3/README.md` & `geojp-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `geojp-0.0.3/docs/Notebooks/lab4.ipynb` & `geojp-0.0.4/docs/Notebooks/lab4.ipynb`

 * *Files identical despite different names*

### Comparing `geojp-0.0.3/docs/contributing.md` & `geojp-0.0.4/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `geojp-0.0.3/docs/examples/random.ipynb` & `geojp-0.0.4/docs/examples/random.ipynb`

 * *Files identical despite different names*

### Comparing `geojp-0.0.3/docs/installation.md` & `geojp-0.0.4/docs/installation.md`

 * *Files identical despite different names*

### Comparing `geojp-0.0.3/docs/labs/lab4.ipynb` & `geojp-0.0.4/docs/labs/lab4.ipynb`

 * *Files identical despite different names*

### Comparing `geojp-0.0.3/geojp.egg-info/PKG-INFO` & `geojp-0.0.4/geojp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geojp
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package for my Geospacial Analysis class
 Author-email: Brycen Harris <bharri94@vols.utk.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/BrycenHarris/geojp
 Keywords: geojp
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
+Requires-Dist: ipyleaflet
 Provides-Extra: all
 Requires-Dist: geojp[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # Welcome to geojp
 ![](https://oyster.ignimgs.com/wordpress/stg.ign.com/2013/04/JurassicPark_040413_1600.jpg?width=1920)
```

### Comparing `geojp-0.0.3/mkdocs.yml` & `geojp-0.0.4/mkdocs.yml`

 * *Files 23% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     - git-revision-date-localized:
           enable_creation_date: true
           type: timeago
     # - pdf-export
     - mkdocs-jupyter:
           include_source: True
           ignore_h1_titles: True
-          execute: True
+          execute: false
           allow_errors: false
           ignore: ["conf.py"]
           execute_ignore: ["*ignore.ipynb"]
           
 markdown_extensions:
     - admonition
     - abbr
@@ -77,13 +77,25 @@
     - Usage: usage.md
     - Contributing: contributing.md
     - FAQ: faq.md
     - Changelog: changelog.md
     - Report Issues: https://github.com/BrycenHarris/geojp/issues
     - Examples:
         - examples/intro.ipynb
+        - examples/random.ipynb
+        - examples/ipyleaflet.ipynb
+        - examples/csv.ipynb
+        - examples/raster.ipynb
+        - examples/image.ipynb
+        - examples/map.ipynb
+
     - Notebooks:
-        - notebooks/colab.ipynb
-        - notebooks/lab4.ipynb
+        - Notebooks/lab4.ipynb
+        - Notebooks/lab5.ipynb
+
     - API Reference:
           - geojp module: geojp.md
           - common module: common.md
+          - utils module: utils.md
+    - labs:
+        - labs/lab4.ipynb
+        - labs/lab5.ipynb
```

### Comparing `geojp-0.0.3/pyproject.toml` & `geojp-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "geojp"
-version = "0.0.3"
+version = "0.0.4"
 dynamic = [
     "dependencies",
 ]
 description = "A python package for my Geospacial Analysis class"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.3"
+current_version = "0.0.4"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

