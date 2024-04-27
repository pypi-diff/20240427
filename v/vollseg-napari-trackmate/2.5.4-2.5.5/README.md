# Comparing `tmp/vollseg-napari-trackmate-2.5.4.tar.gz` & `tmp/vollseg_napari_trackmate-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vollseg-napari-trackmate-2.5.4.tar", last modified: Fri Apr  5 21:40:00 2024, max compression
+gzip compressed data, was "vollseg_napari_trackmate-2.5.5.tar", last modified: Sat Apr 27 17:09:23 2024, max compression
```

## Comparing `vollseg-napari-trackmate-2.5.4.tar` & `vollseg_napari_trackmate-2.5.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.744773 vollseg-napari-trackmate-2.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.736773 vollseg-napari-trackmate-2.5.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.740773 vollseg-napari-trackmate-2.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/.github/workflows/napari-hub-preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.740773 vollseg-napari-trackmate-2.5.4/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/ALGORITHM.md
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/MITOSIS.md
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-05 21:40:00.744773 vollseg-napari-trackmate-2.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/RADIAL_ANGLE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.740773 vollseg-napari-trackmate-2.5.4/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/examples/annotate_oneat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/examples/apply_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/examples/create_oneat_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/examples/train_oneat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/examples/visualize_point_clouds.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-05 21:40:00.748772 vollseg-napari-trackmate-2.5.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.736773 vollseg-napari-trackmate-2.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.744773 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_temporal_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.744773 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_tests/test_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    91994 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.744773 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/resources/kapoorlogo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:40:00.744773 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-05 21:40:00.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-05 21:40:00.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:40:00.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 21:40:00.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-05 21:40:00.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 21:40:00.000000 vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-05 21:39:42.000000 vollseg-napari-trackmate-2.5.4/update_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.703421 vollseg_napari_trackmate-2.5.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.695421 vollseg_napari_trackmate-2.5.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.699421 vollseg_napari_trackmate-2.5.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/.github/workflows/napari-hub-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.699421 vollseg_napari_trackmate-2.5.5/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/ALGORITHM.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/MITOSIS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-27 17:09:23.703421 vollseg_napari_trackmate-2.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/RADIAL_ANGLE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.699421 vollseg_napari_trackmate-2.5.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/examples/annotate_oneat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/examples/apply_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/examples/create_oneat_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/examples/train_oneat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/examples/visualize_point_clouds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-27 17:09:23.703421 vollseg_napari_trackmate-2.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.695421 vollseg_napari_trackmate-2.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.699421 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_temporal_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.703421 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_tests/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95277 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.703421 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/resources/kapoorlogo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:09:23.703421 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-27 17:09:23.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-27 17:09:23.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:09:23.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-27 17:09:23.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-27 17:09:23.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-27 17:09:23.000000 vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-27 17:09:10.000000 vollseg_napari_trackmate-2.5.5/update_version.py
```

### Comparing `vollseg-napari-trackmate-2.5.4/.github/workflows/deploy.yml` & `vollseg_napari_trackmate-2.5.5/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/.github/workflows/napari-hub-preview.yml` & `vollseg_napari_trackmate-2.5.5/.github/workflows/napari-hub-preview.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/.github/workflows/test_and_deploy.yml` & `vollseg_napari_trackmate-2.5.5/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/.gitignore` & `vollseg_napari_trackmate-2.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/.napari-hub/DESCRIPTION.md` & `vollseg_napari_trackmate-2.5.5/.napari-hub/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/.napari-hub/config.yml` & `vollseg_napari_trackmate-2.5.5/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/.pre-commit-config.yaml` & `vollseg_napari_trackmate-2.5.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/ALGORITHM.md` & `vollseg_napari_trackmate-2.5.5/ALGORITHM.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/LICENSE` & `vollseg_napari_trackmate-2.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/MITOSIS.md` & `vollseg_napari_trackmate-2.5.5/MITOSIS.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/PKG-INFO` & `vollseg_napari_trackmate-2.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.5.4
+Version: 2.5.5
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg-napari-trackmate-2.5.4/README.md` & `vollseg_napari_trackmate-2.5.5/README.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/_config.yml` & `vollseg_napari_trackmate-2.5.5/_config.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/examples/apply_autoencoder.py` & `vollseg_napari_trackmate-2.5.5/examples/apply_autoencoder.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/examples/create_oneat_patches.py` & `vollseg_napari_trackmate-2.5.5/examples/create_oneat_patches.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/examples/train_oneat.py` & `vollseg_napari_trackmate-2.5.5/examples/train_oneat.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/examples/visualize_point_clouds.py` & `vollseg_napari_trackmate-2.5.5/examples/visualize_point_clouds.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/setup.cfg` & `vollseg_napari_trackmate-2.5.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_data_model.py` & `vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_data_model.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_temporal_plots.py` & `vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_temporal_plots.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_tests/test_widget.py` & `vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/_widget.py` & `vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -873,14 +873,15 @@
                             cluster_time,
                             cluster_speed,
                             cluster_motion_angle_z,
                             cluster_motion_angle_y,
                             cluster_motion_angle_x,
                             cluster_acceleration,
                             cluster_distance_cell_mask,
+                            cluster_local_cell_density,
                             cluster_radial_angle_z,
                             cluster_radial_angle_y,
                             cluster_radial_angle_x,
                             cluster_cell_axis_z,
                             cluster_cell_axis_y,
                             cluster_cell_axis_x,
                             _,
@@ -893,14 +894,15 @@
                                 cluster_time,
                                 cluster_speed,
                                 cluster_motion_angle_z,
                                 cluster_motion_angle_y,
                                 cluster_motion_angle_x,
                                 cluster_acceleration,
                                 cluster_distance_cell_mask,
+                                cluster_local_cell_density,
                                 cluster_radial_angle_z,
                                 cluster_radial_angle_y,
                                 cluster_radial_angle_x,
                                 cluster_cell_axis_z,
                                 cluster_cell_axis_y,
                                 cluster_cell_axis_x,
                                 countk + 1,
@@ -945,39 +947,45 @@
                                 4
                             ]
 
                             cluster_acceleration = current_unique_dynamic_properties[5]
                             cluster_distance_cell_mask = (
                                 current_unique_dynamic_properties[6]
                             )
+
+                            cluster_local_cell_density = (
+                                current_unique_dynamic_properties[7]
+                            )
+
                             cluster_radial_angle_z = current_unique_dynamic_properties[
-                                7
+                                8
                             ]
                             cluster_radial_angle_y = current_unique_dynamic_properties[
-                                8
+                                9
                             ]
                             cluster_radial_angle_x = current_unique_dynamic_properties[
-                                9
+                                10
                             ]
 
-                            cluster_cell_axis_z = current_unique_dynamic_properties[10]
-                            cluster_cell_axis_y = current_unique_dynamic_properties[11]
-                            cluster_cell_axis_x = current_unique_dynamic_properties[12]
+                            cluster_cell_axis_z = current_unique_dynamic_properties[11]
+                            cluster_cell_axis_y = current_unique_dynamic_properties[12]
+                            cluster_cell_axis_x = current_unique_dynamic_properties[13]
 
                             cluster_id = current_unique_dynamic_properties[-1]
 
                             data_dynamic_cluster_plot = pd.DataFrame(
                                 {
                                     "Time": cluster_time,
                                     "Speed": cluster_speed,
                                     "Motion_Angle_Z": cluster_motion_angle_z,
                                     "Motion_Angle_Y": cluster_motion_angle_y,
                                     "Motion_Angle_X": cluster_motion_angle_x,
                                     "Acceleration": cluster_acceleration,
                                     "Distance_cell_to_tissue": cluster_distance_cell_mask,
+                                    "Local_Cell_Density": cluster_local_cell_density,
                                     "Radial_Angle_Z": cluster_radial_angle_z,
                                     "Radial_Angle_Y": cluster_radial_angle_y,
                                     "Radial_Angle_X": cluster_radial_angle_x,
                                     "Cell_Axis_Z": cluster_cell_axis_z,
                                     "Cell_Axis_Y": cluster_cell_axis_y,
                                     "Cell_Axis_X": cluster_cell_axis_x,
                                     "id": cluster_id,
@@ -1049,255 +1057,270 @@
                     y="Speed",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
                 plot_ax.set_title("Speed")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Motion_Angle_Z",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
                 plot_ax.set_title("Motion Angle Z")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Radial_Angle_Z",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
                 plot_ax.set_title("Radial Angle Z")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Motion_Angle_Y",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
                 plot_ax.set_title("Motion Angle Y")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Radial_Angle_Y",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
                 plot_ax.set_title("Radial Angle Y")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Motion_Angle_X",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
                 plot_ax.set_title("Motion Angle X")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Radial_Angle_X",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
                 plot_ax.set_title("Radial Angle X")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Acceleration",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
                 plot_ax.set_title("Acceleration")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Distance_cell_to_tissue",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
                 plot_ax.set_title("Distance cell to tissue")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
+
+                phenotype_plot_class._repeat_after_plot()
+                plot_ax = phenotype_plot_class.plot_ax
+                sns.set_palette(flatui)
+                sns.lineplot(
+                    global_data_dynamic_cluster_plot,
+                    x="Time",
+                    y="Local_Cell_Density",
+                    hue="id",
+                    ax=plot_ax,
+                    legend=False,
+                )
+
+                plot_ax.set_title("Local Cell Density")
+                plot_ax.set_xlabel("Time (sec)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Cell_Axis_Z",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
                 plot_ax.set_title("Cell Axis Z")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
-                    y="Aell_Axis_Y",
+                    y="Cell_Axis_Y",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
                 plot_ax.set_title("Cell Axis Y")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_dynamic_cluster_plot,
                     x="Time",
                     y="Cell_Axis_X",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
                 plot_ax.set_title("Cell Axis X")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Radius",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
                 plot_ax.set_title("Radius")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
-                    y="Radius_pixel",
+                    y="Radius_Pixel",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
-                plot_ax.set_title("Radius_pixel")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_title("Radius_Pixel")
+                plot_ax.set_xlabel("Time (sec)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Surface_Area",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
                 plot_ax.set_title("Surface_Area")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Eccentricity_Comp_First",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
                 plot_ax.set_title("Eccentricity Comp First")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
                     y="Eccentricity_Comp_Second",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
                 plot_ax.set_title("Eccentricity Comp Second")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
@@ -1307,15 +1330,15 @@
                     y="Eccentricity_Comp_Third",
                     hue="id",
                     ax=plot_ax,
                     legend=False,
                 )
 
                 plot_ax.set_title("Eccentricity Comp Third")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
             summed_amplitude = []
             for i in range(len(unique_fft_properties)):
                 summed_amplitude.append(unique_fft_properties[i][3] ** 2)
             summed_amplitude = np.sum(summed_amplitude, axis=0)
@@ -1336,15 +1359,15 @@
                     "Intensity": summed_intesity,
                 }
             )
 
             sns.set_palette(flatui)
             sns.lineplot(data_time_plot, x="Time", y="Intensity", ax=plot_ax)
             plot_ax.set_title("Cell Intensity")
-            plot_ax.set_xlabel("Time (min)")
+            plot_ax.set_xlabel("Time (sec)")
             plot_ax.set_ylabel("Amplitude")
 
             phenotype_plot_class._repeat_after_plot()
             plot_ax = phenotype_plot_class.plot_ax
 
             sns.set_palette(flatui)
             sns.lineplot(data_fft_plot, x="Frequ", y="Amplitude", ax=plot_ax)
@@ -1525,31 +1548,47 @@
                     _trackmate_objects.mitotic_var_distance_cell_mask,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Cell-tissue distance")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
+                    _trackmate_objects.mitotic_mean_local_cell_density,
+                    _trackmate_objects.mitotic_var_local_cell_density,
+                    linestyle="None",
+                    marker=".",
+                    mfc="green",
+                    ecolor="green",
+                )
+                plot_ax.set_title("Local Cell Density")
+                plot_ax.set_xlabel("Time (sec)")
+                plot_ax.set_ylabel("Density")
+
+                stat_plot_class._repeat_after_plot()
+                plot_ax = stat_plot_class.plot_ax
+
+                plot_ax.errorbar(
+                    _trackmate_objects.time,
                     _trackmate_objects.mitotic_mean_directional_change_z,
                     _trackmate_objects.mitotic_var_directional_change_z,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Instantaneous Directional change in Z")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("angle (degrees)")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1557,15 +1596,15 @@
                     _trackmate_objects.mitotic_var_directional_change_y,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Instantaneous Directional change in Y")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("angle (degrees)")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1573,15 +1612,15 @@
                     _trackmate_objects.mitotic_var_directional_change_x,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Instantaneous Directional change in X")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("angle (degrees)")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1589,15 +1628,15 @@
                     _trackmate_objects.mitotic_var_speed,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Speed")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um/min")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1605,15 +1644,15 @@
                     _trackmate_objects.mitotic_var_acc,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Acceleration")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um/min")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1621,15 +1660,15 @@
                     _trackmate_objects.mitotic_var_radius,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Radius")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1638,15 +1677,15 @@
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
 
                 plot_ax.set_title("Displacement in Z")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1655,15 +1694,15 @@
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
 
                 plot_ax.set_title("Displacement in Y")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1672,15 +1711,15 @@
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
 
                 plot_ax.set_title("Displacement in X")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um")
 
             if key == track_model_type_dict[1]:
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
                 plot_ax.cla()
@@ -1691,31 +1730,47 @@
                     _trackmate_objects.non_mitotic_var_distance_cell_mask,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Cell-tissue distance")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
+                    _trackmate_objects.non_mitotic_mean_local_cell_density,
+                    _trackmate_objects.non_mitotic_var_local_cell_density,
+                    linestyle="None",
+                    marker=".",
+                    mfc="green",
+                    ecolor="green",
+                )
+                plot_ax.set_title("Local Cell Density")
+                plot_ax.set_xlabel("Time (sec)")
+                plot_ax.set_ylabel("Density")
+
+                stat_plot_class._repeat_after_plot()
+                plot_ax = stat_plot_class.plot_ax
+
+                plot_ax.errorbar(
+                    _trackmate_objects.time,
                     _trackmate_objects.non_mitotic_mean_directional_change_z,
                     _trackmate_objects.non_mitotic_var_directional_change_z,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Instantaneous Directional change in Z")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("angle (degrees)")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1723,15 +1778,15 @@
                     _trackmate_objects.non_mitotic_var_directional_change_y,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Instantaneous Directional change in Y")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("angle (degrees)")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1739,15 +1794,15 @@
                     _trackmate_objects.non_mitotic_var_directional_change_x,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Instantaneous Directional change in X")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("angle (degrees)")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1755,15 +1810,15 @@
                     _trackmate_objects.non_mitotic_var_speed,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Instantaneous Speed")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um/min")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1771,15 +1826,15 @@
                     _trackmate_objects.mitotic_var_acc,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Acceleration")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um/min")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1787,15 +1842,15 @@
                     _trackmate_objects.non_mitotic_var_radius,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Radius")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1804,15 +1859,15 @@
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
 
                 plot_ax.set_title("Displacement in Z")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1821,15 +1876,15 @@
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
 
                 plot_ax.set_title("Displacement in Y")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1838,15 +1893,15 @@
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
 
                 plot_ax.set_title("Displacement in X")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um")
 
             if key == track_model_type_dict[2]:
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
                 plot_ax.cla()
@@ -1857,31 +1912,47 @@
                     _trackmate_objects.all_var_distance_cell_mask,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Cell-tissue distance")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
+                    _trackmate_objects.all_mean_local_cell_density,
+                    _trackmate_objects.all_var_local_cell_density,
+                    linestyle="None",
+                    marker=".",
+                    mfc="green",
+                    ecolor="green",
+                )
+                plot_ax.set_title("Local Cell Density")
+                plot_ax.set_xlabel("Time (sec)")
+                plot_ax.set_ylabel("Density")
+
+                stat_plot_class._repeat_after_plot()
+                plot_ax = stat_plot_class.plot_ax
+
+                plot_ax.errorbar(
+                    _trackmate_objects.time,
                     _trackmate_objects.all_mean_directional_change_z,
                     _trackmate_objects.all_var_directional_change_z,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Instantaneous Directional change in Z")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("angle (degrees)")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1889,15 +1960,15 @@
                     _trackmate_objects.all_var_directional_change_y,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Instantaneous Directional change in Y")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("angle (degrees)")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1905,15 +1976,15 @@
                     _trackmate_objects.all_var_directional_change_x,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Instantaneous Directional change in X")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("angle (degrees)")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1921,15 +1992,15 @@
                     _trackmate_objects.non_mitotic_var_speed,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Instantaneous  Speed")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um/min")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1937,15 +2008,15 @@
                     _trackmate_objects.mitotic_var_acc,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Acceleration")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um/min")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1953,15 +2024,15 @@
                     _trackmate_objects.non_mitotic_var_radius,
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
                 plot_ax.set_title("Radius")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1970,15 +2041,15 @@
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
 
                 plot_ax.set_title("Displacement in Z")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -1987,15 +2058,15 @@
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
 
                 plot_ax.set_title("Displacement in Y")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um")
 
                 stat_plot_class._repeat_after_plot()
                 plot_ax = stat_plot_class.plot_ax
 
                 plot_ax.errorbar(
                     _trackmate_objects.time,
@@ -2004,15 +2075,15 @@
                     linestyle="None",
                     marker=".",
                     mfc="green",
                     ecolor="green",
                 )
 
                 plot_ax.set_title("Displacement in X")
-                plot_ax.set_xlabel("Time (min)")
+                plot_ax.set_xlabel("Time (sec)")
                 plot_ax.set_ylabel("um")
 
             for layer in list(plugin.viewer.value.layers):
                 if isinstance(layer, napari.layers.Tracks):
                     table_tab.layer = layer
 
     def _refreshStatPlotData():
@@ -2048,20 +2119,21 @@
         _both_choices = _trackmate_objects.AllTrackIds
         _both_track_ids_analyze = _trackmate_objects.AllTrackIds.copy()
         if TrackidBox in _both_track_ids_analyze:
             _both_track_ids_analyze.remove(TrackidBox)
         if None in _both_track_ids_analyze:
             _both_track_ids_analyze.remove(None)
 
-        plugin_color_parameters.track_attributes.choices = (
-            _trackmate_objects.TrackAttributeids
-        )
-        plugin_color_parameters.spot_attributes.choices = (
-            _trackmate_objects.Attributeids
-        )
+        if hasattr(_trackmate_objects, "TrackAttributeids"):
+            plugin_color_parameters.track_attributes.choices = (
+                _trackmate_objects.TrackAttributeids
+            )
+            plugin_color_parameters.spot_attributes.choices = (
+                _trackmate_objects.Attributeids
+            )
         plugin.progress_bar.label = "Creating Table"
         plugin.progress_bar.range = (0, len(root_spots) - 1)
 
         v = next(iter(root_spots.values()))
         columns = [value for value in v.keys()]
         for count, (k, v) in enumerate(root_spots.items()):
 
@@ -2321,20 +2393,29 @@
                 scale_z = config["scale_z"]
                 scale_xy = config["scale_xy"]
 
         if plugin_data.device_type.value == "GPU":
             accelerator = "gpu"
         else:
             accelerator = "cpu"
+        spot_csv_path = plugin_data.spot_csv_path.value
+        track_csv_path = plugin_data.track_csv_path.value
+        edges_csv_path = plugin_data.edges_csv_path.value
+        if os.path.isdir(plugin_data.spot_csv_path.value):
+            spot_csv_path = None
+        if os.path.isdir(plugin_data.track_csv_path.value):
+            track_csv_path = None
+        if os.path.isdir(plugin_data.edges_csv_path.value):
+            edges_csv_path = None
 
         _trackmate_objects = TrackMate(
             plugin_data.xml_path.value,
-            plugin_data.spot_csv_path.value,
-            plugin_data.track_csv_path.value,
-            plugin_data.edges_csv_path.value,
+            spot_csv_path,
+            track_csv_path,
+            edges_csv_path,
             AttributeBoxname,
             TrackAttributeBoxname,
             TrackidBox,
             plugin_data.axes.value,
             master_xml_path=plugin_data.master_xml_path.value,
             channel_seg_image=x_channel_seg,
             seg_image=x_seg,
```

### Comparing `vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/napari.yaml` & `vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/napari.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate/resources/kapoorlogo.png` & `vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate/resources/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate.egg-info/PKG-INFO` & `vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.5.4
+Version: 2.5.5
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg-napari-trackmate-2.5.4/src/vollseg_napari_trackmate.egg-info/SOURCES.txt` & `vollseg_napari_trackmate-2.5.5/src/vollseg_napari_trackmate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/tox.ini` & `vollseg_napari_trackmate-2.5.5/tox.ini`

 * *Files identical despite different names*

### Comparing `vollseg-napari-trackmate-2.5.4/update_version.py` & `vollseg_napari_trackmate-2.5.5/update_version.py`

 * *Files identical despite different names*

