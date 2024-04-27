# Comparing `tmp/napatrackmater-5.1.1.tar.gz` & `tmp/napatrackmater-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napatrackmater-5.1.1.tar", last modified: Sun Apr 14 18:23:26 2024, max compression
+gzip compressed data, was "napatrackmater-5.1.2.tar", last modified: Sat Apr 27 17:10:19 2024, max compression
```

## Comparing `napatrackmater-5.1.1.tar` & `napatrackmater-5.1.2.tar`

### file list

```diff
@@ -1,281 +1,281 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.252231 napatrackmater-5.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.212231 napatrackmater-5.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.224231 napatrackmater-5.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/MASTER.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.224231 napatrackmater-5.1.1/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/Notebooks/Track_vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-14 18:23:26.252231 napatrackmater-5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.224231 napatrackmater-5.1.1/_build/.doctrees/
--rw-r--r--   0 runner    (1001) docker     (127)    33531 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/.doctrees/MASTER.doctree
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.224231 napatrackmater-5.1.1/_build/.doctrees/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    29083 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/.doctrees/Notebooks/Track_vector.doctree
--rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/.doctrees/README.doctree
--rw-r--r--   0 runner    (1001) docker     (127)    36454 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/.doctrees/environment.pickle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.228231 napatrackmater-5.1.1/_build/html/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/.buildinfo
--rw-r--r--   0 runner    (1001) docker     (127)    29915 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/MASTER.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.228231 napatrackmater-5.1.1/_build/html/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    66062 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/Notebooks/Track_vector.html
--rw-r--r--   0 runner    (1001) docker     (127)    18885 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/README.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.228231 napatrackmater-5.1.1/_build/html/_images/
--rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_images/ClusterDistributionPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_images/ClusterNearnessPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_images/ClusterPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_images/FeatureMatrixPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_images/QuadrantDistributionPlot_time_point_97.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.228231 napatrackmater-5.1.1/_build/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_sources/MASTER.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.228231 napatrackmater-5.1.1/_build/html/_sources/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_sources/Notebooks/Track_vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_sources/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.228231 napatrackmater-5.1.1/_build/html/_sphinx_design_static/
--rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_sphinx_design_static/design-tabs.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    14692 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/check-solid.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/copy-button.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/copybutton.css
--rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/copybutton.js
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/copybutton_funcs.js
--rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/design-tabs.js
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/file.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/images/logo_binder.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/images/logo_colab.png
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/images/logo_deepnote.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/images/logo_jupyterhub.svg
--rw-r--r--   0 runner    (1001) docker     (127)   287630 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 runner    (1001) docker     (127)    89476 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/kapoorlablogo.png
--rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/language_data.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/_build/html/_static/locales/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.212231 napatrackmater-5.1.1/_build/html/_static/locales/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.212231 napatrackmater-5.1.1/_build/html/_static/locales/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.212231 napatrackmater-5.1.1/_build/html/_static/locales/bn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/bn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.212231 napatrackmater-5.1.1/_build/html/_static/locales/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.212231 napatrackmater-5.1.1/_build/html/_static/locales/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.212231 napatrackmater-5.1.1/_build/html/_static/locales/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.212231 napatrackmater-5.1.1/_build/html/_static/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.212231 napatrackmater-5.1.1/_build/html/_static/locales/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.212231 napatrackmater-5.1.1/_build/html/_static/locales/eo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.212231 napatrackmater-5.1.1/_build/html/_static/locales/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.212231 napatrackmater-5.1.1/_build/html/_static/locales/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/id/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/iw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/iw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/lv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.236231 napatrackmater-5.1.1/_build/html/_static/locales/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/ml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/ml/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/mr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/mr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/ms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/ms/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/no/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.216231 napatrackmater-5.1.1/_build/html/_static/locales/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/_build/html/_static/locales/sl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/_build/html/_static/locales/sr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/_build/html/_static/locales/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/_build/html/_static/locales/ta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/ta/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/_build/html/_static/locales/te/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/te/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/_build/html/_static/locales/tg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/tg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/_build/html/_static/locales/th/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/_build/html/_static/locales/tl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/tl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/_build/html/_static/locales/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/_build/html/_static/locales/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/_build/html/_static/locales/ur/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/ur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/_build/html/_static/locales/vi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/vi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/_build/html/_static/locales/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/_build/html/_static/locales/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.240231 napatrackmater-5.1.1/_build/html/_static/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)    39364 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)    12757 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/sbt-webpack-macros.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.244231 napatrackmater-5.1.1/_build/html/_static/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)    80813 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/scripts/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/scripts/bootstrap.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   335757 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/scripts/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (127)    19648 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/scripts/pydata-sphinx-theme.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/scripts/sphinx-book-theme.js
--rw-r--r--   0 runner    (1001) docker     (127)    13066 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/scripts/sphinx-book-theme.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    16634 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/sphinx-thebe.css
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/sphinx-thebe.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.244231 napatrackmater-5.1.1/_build/html/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (127)   176654 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/styles/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)    63341 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/styles/sphinx-book-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/styles/theme.css
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/togglebutton.css
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/togglebutton.js
--rw-r--r--   0 runner    (1001) docker     (127)    68420 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/underscore.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/_build/html/_static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.244231 napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.244231 napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/css/
--rw-r--r--   0 runner    (1001) docker     (127)   101691 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.248231 napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/
--rw-r--r--   0 runner    (1001) docker     (127)   181264 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   105112 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    60236 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    24028 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   389948 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   154840 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/_static/webpack-macros.html
--rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/objects.inv
--rw-r--r--   0 runner    (1001) docker     (127)    12010 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/search.html
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/html/searchindex.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/_build/jupyter_execute/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.248231 napatrackmater-5.1.1/_build/jupyter_execute/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    17500 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_build/jupyter_execute/Notebooks/Track_vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.248231 napatrackmater-5.1.1/images/
--rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/images/ClusterDistributionPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/images/ClusterNearnessPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/images/ClusterPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/images/FeatureMatrixPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/images/QuadrantDistributionPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/images/kapoorlablogo.png
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/images/kapoorlogo.png
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-14 18:23:26.252231 napatrackmater-5.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.220231 napatrackmater-5.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.252231 napatrackmater-5.1.1/src/napatrackmater/
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/src/napatrackmater/CloudAutoEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/src/napatrackmater/DeepEmbeddedClustering.py
--rw-r--r--   0 runner    (1001) docker     (127)   133752 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/src/napatrackmater/Trackmate.py
--rw-r--r--   0 runner    (1001) docker     (127)   111039 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/src/napatrackmater/Trackvector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/src/napatrackmater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/src/napatrackmater/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    24558 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/src/napatrackmater/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/src/napatrackmater/fast_radius_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/src/napatrackmater/fate_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/src/napatrackmater/pretrained.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:23:26.252231 napatrackmater-5.1.1/src/napatrackmater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-14 18:23:26.000000 napatrackmater-5.1.1/src/napatrackmater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-14 18:23:26.000000 napatrackmater-5.1.1/src/napatrackmater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 18:23:26.000000 napatrackmater-5.1.1/src/napatrackmater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-14 18:23:26.000000 napatrackmater-5.1.1/src/napatrackmater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 18:23:26.000000 napatrackmater-5.1.1/src/napatrackmater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-14 18:23:12.000000 napatrackmater-5.1.1/update_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.196041 napatrackmater-5.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.148040 napatrackmater-5.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.164040 napatrackmater-5.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/MASTER.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.164040 napatrackmater-5.1.2/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/Notebooks/Track_vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-27 17:10:19.196041 napatrackmater-5.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.160040 napatrackmater-5.1.2/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.164040 napatrackmater-5.1.2/_build/.doctrees/
+-rw-r--r--   0 runner    (1001) docker     (127)    33531 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/.doctrees/MASTER.doctree
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.164040 napatrackmater-5.1.2/_build/.doctrees/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    29083 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/.doctrees/Notebooks/Track_vector.doctree
+-rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/.doctrees/README.doctree
+-rw-r--r--   0 runner    (1001) docker     (127)    36454 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/.doctrees/environment.pickle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.164040 napatrackmater-5.1.2/_build/html/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/.buildinfo
+-rw-r--r--   0 runner    (1001) docker     (127)    29915 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/MASTER.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.164040 napatrackmater-5.1.2/_build/html/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    66062 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/Notebooks/Track_vector.html
+-rw-r--r--   0 runner    (1001) docker     (127)    18885 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/README.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.168041 napatrackmater-5.1.2/_build/html/_images/
+-rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_images/ClusterDistributionPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_images/ClusterNearnessPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_images/ClusterPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_images/FeatureMatrixPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_images/QuadrantDistributionPlot_time_point_97.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.168041 napatrackmater-5.1.2/_build/html/_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_sources/MASTER.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.168041 napatrackmater-5.1.2/_build/html/_sources/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_sources/Notebooks/Track_vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_sources/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.168041 napatrackmater-5.1.2/_build/html/_sphinx_design_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_sphinx_design_static/design-tabs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.176041 napatrackmater-5.1.2/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14692 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/check-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/copy-button.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/copybutton.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/copybutton.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/copybutton_funcs.js
+-rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/design-tabs.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/file.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.176041 napatrackmater-5.1.2/_build/html/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/images/logo_binder.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/images/logo_colab.png
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/images/logo_deepnote.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/images/logo_jupyterhub.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   287630 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    89476 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/kapoorlablogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/language_data.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.156041 napatrackmater-5.1.2/_build/html/_static/locales/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.148040 napatrackmater-5.1.2/_build/html/_static/locales/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.176041 napatrackmater-5.1.2/_build/html/_static/locales/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.148040 napatrackmater-5.1.2/_build/html/_static/locales/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.176041 napatrackmater-5.1.2/_build/html/_static/locales/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.148040 napatrackmater-5.1.2/_build/html/_static/locales/bn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.176041 napatrackmater-5.1.2/_build/html/_static/locales/bn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.148040 napatrackmater-5.1.2/_build/html/_static/locales/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.176041 napatrackmater-5.1.2/_build/html/_static/locales/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.148040 napatrackmater-5.1.2/_build/html/_static/locales/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.176041 napatrackmater-5.1.2/_build/html/_static/locales/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.148040 napatrackmater-5.1.2/_build/html/_static/locales/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.176041 napatrackmater-5.1.2/_build/html/_static/locales/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.148040 napatrackmater-5.1.2/_build/html/_static/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.176041 napatrackmater-5.1.2/_build/html/_static/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.148040 napatrackmater-5.1.2/_build/html/_static/locales/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.176041 napatrackmater-5.1.2/_build/html/_static/locales/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.148040 napatrackmater-5.1.2/_build/html/_static/locales/eo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.176041 napatrackmater-5.1.2/_build/html/_static/locales/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.152040 napatrackmater-5.1.2/_build/html/_static/locales/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.176041 napatrackmater-5.1.2/_build/html/_static/locales/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.152040 napatrackmater-5.1.2/_build/html/_static/locales/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.176041 napatrackmater-5.1.2/_build/html/_static/locales/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.152040 napatrackmater-5.1.2/_build/html/_static/locales/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.176041 napatrackmater-5.1.2/_build/html/_static/locales/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.152040 napatrackmater-5.1.2/_build/html/_static/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.176041 napatrackmater-5.1.2/_build/html/_static/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.152040 napatrackmater-5.1.2/_build/html/_static/locales/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.176041 napatrackmater-5.1.2/_build/html/_static/locales/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.152040 napatrackmater-5.1.2/_build/html/_static/locales/id/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.176041 napatrackmater-5.1.2/_build/html/_static/locales/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.152040 napatrackmater-5.1.2/_build/html/_static/locales/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.152040 napatrackmater-5.1.2/_build/html/_static/locales/iw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/iw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.152040 napatrackmater-5.1.2/_build/html/_static/locales/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.152040 napatrackmater-5.1.2/_build/html/_static/locales/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.152040 napatrackmater-5.1.2/_build/html/_static/locales/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.152040 napatrackmater-5.1.2/_build/html/_static/locales/lv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.152040 napatrackmater-5.1.2/_build/html/_static/locales/ml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/ml/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.152040 napatrackmater-5.1.2/_build/html/_static/locales/mr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/mr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.152040 napatrackmater-5.1.2/_build/html/_static/locales/ms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/ms/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.152040 napatrackmater-5.1.2/_build/html/_static/locales/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.152040 napatrackmater-5.1.2/_build/html/_static/locales/no/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.152040 napatrackmater-5.1.2/_build/html/_static/locales/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.156041 napatrackmater-5.1.2/_build/html/_static/locales/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.156041 napatrackmater-5.1.2/_build/html/_static/locales/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.156041 napatrackmater-5.1.2/_build/html/_static/locales/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.156041 napatrackmater-5.1.2/_build/html/_static/locales/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.156041 napatrackmater-5.1.2/_build/html/_static/locales/sl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.156041 napatrackmater-5.1.2/_build/html/_static/locales/sr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.156041 napatrackmater-5.1.2/_build/html/_static/locales/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.156041 napatrackmater-5.1.2/_build/html/_static/locales/ta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/ta/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.156041 napatrackmater-5.1.2/_build/html/_static/locales/te/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/te/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.156041 napatrackmater-5.1.2/_build/html/_static/locales/tg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.180041 napatrackmater-5.1.2/_build/html/_static/locales/tg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.156041 napatrackmater-5.1.2/_build/html/_static/locales/th/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.184041 napatrackmater-5.1.2/_build/html/_static/locales/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.156041 napatrackmater-5.1.2/_build/html/_static/locales/tl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.184041 napatrackmater-5.1.2/_build/html/_static/locales/tl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.156041 napatrackmater-5.1.2/_build/html/_static/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.184041 napatrackmater-5.1.2/_build/html/_static/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.156041 napatrackmater-5.1.2/_build/html/_static/locales/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.184041 napatrackmater-5.1.2/_build/html/_static/locales/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.156041 napatrackmater-5.1.2/_build/html/_static/locales/ur/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.184041 napatrackmater-5.1.2/_build/html/_static/locales/ur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.156041 napatrackmater-5.1.2/_build/html/_static/locales/vi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.184041 napatrackmater-5.1.2/_build/html/_static/locales/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.156041 napatrackmater-5.1.2/_build/html/_static/locales/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.184041 napatrackmater-5.1.2/_build/html/_static/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.156041 napatrackmater-5.1.2/_build/html/_static/locales/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.184041 napatrackmater-5.1.2/_build/html/_static/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39364 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12757 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/sbt-webpack-macros.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.184041 napatrackmater-5.1.2/_build/html/_static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)    80813 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/scripts/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/scripts/bootstrap.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   335757 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/scripts/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19648 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/scripts/pydata-sphinx-theme.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/scripts/sphinx-book-theme.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13066 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/scripts/sphinx-book-theme.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    16634 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/sphinx-thebe.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/sphinx-thebe.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.188041 napatrackmater-5.1.2/_build/html/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)   176654 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/styles/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)    63341 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/styles/sphinx-book-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/styles/theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/togglebutton.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/togglebutton.js
+-rw-r--r--   0 runner    (1001) docker     (127)    68420 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/underscore.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.160040 napatrackmater-5.1.2/_build/html/_static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.160040 napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.188041 napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.188041 napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   101691 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.192041 napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   181264 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   105112 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    60236 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    24028 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   389948 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   154840 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/_static/webpack-macros.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (127)    12010 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/html/searchindex.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.160040 napatrackmater-5.1.2/_build/jupyter_execute/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.192041 napatrackmater-5.1.2/_build/jupyter_execute/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    17500 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_build/jupyter_execute/Notebooks/Track_vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.192041 napatrackmater-5.1.2/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/images/ClusterDistributionPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/images/ClusterNearnessPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/images/ClusterPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/images/FeatureMatrixPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/images/QuadrantDistributionPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/images/kapoorlablogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/images/kapoorlogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-27 17:10:19.196041 napatrackmater-5.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.160040 napatrackmater-5.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.196041 napatrackmater-5.1.2/src/napatrackmater/
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/src/napatrackmater/CloudAutoEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/src/napatrackmater/DeepEmbeddedClustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)   143204 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/src/napatrackmater/Trackmate.py
+-rw-r--r--   0 runner    (1001) docker     (127)   111329 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/src/napatrackmater/Trackvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/src/napatrackmater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/src/napatrackmater/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24585 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/src/napatrackmater/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/src/napatrackmater/fast_radius_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/src/napatrackmater/fate_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/src/napatrackmater/pretrained.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:19.196041 napatrackmater-5.1.2/src/napatrackmater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-27 17:10:19.000000 napatrackmater-5.1.2/src/napatrackmater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-27 17:10:19.000000 napatrackmater-5.1.2/src/napatrackmater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:10:19.000000 napatrackmater-5.1.2/src/napatrackmater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-27 17:10:19.000000 napatrackmater-5.1.2/src/napatrackmater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-27 17:10:19.000000 napatrackmater-5.1.2/src/napatrackmater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-27 17:10:02.000000 napatrackmater-5.1.2/update_version.py
```

### Comparing `napatrackmater-5.1.1/.github/workflows/deploy.yml` & `napatrackmater-5.1.2/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/.github/workflows/test_and_deploy.yml` & `napatrackmater-5.1.2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/.gitignore` & `napatrackmater-5.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/.pre-commit-config.yaml` & `napatrackmater-5.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/.travis.yml` & `napatrackmater-5.1.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/Dockerfile` & `napatrackmater-5.1.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/LICENSE` & `napatrackmater-5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/MASTER.md` & `napatrackmater-5.1.2/MASTER.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/Notebooks/Track_vector.ipynb` & `napatrackmater-5.1.2/Notebooks/Track_vector.ipynb`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/PKG-INFO` & `napatrackmater-5.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 5.1.1
+Version: 5.1.2
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/Kapoorlabs-CAPED/napatrackmater
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/napatrackmater/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/napatrackmater#README.md
```

### Comparing `napatrackmater-5.1.1/README.md` & `napatrackmater-5.1.2/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/.doctrees/MASTER.doctree` & `napatrackmater-5.1.2/_build/.doctrees/MASTER.doctree`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/.doctrees/Notebooks/Track_vector.doctree` & `napatrackmater-5.1.2/_build/.doctrees/Notebooks/Track_vector.doctree`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/.doctrees/README.doctree` & `napatrackmater-5.1.2/_build/.doctrees/README.doctree`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/.doctrees/environment.pickle` & `napatrackmater-5.1.2/_build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/MASTER.html` & `napatrackmater-5.1.2/_build/html/MASTER.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/Notebooks/Track_vector.html` & `napatrackmater-5.1.2/_build/html/Notebooks/Track_vector.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/README.html` & `napatrackmater-5.1.2/_build/html/README.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_images/ClusterDistributionPlot_time_point_97.png` & `napatrackmater-5.1.2/_build/html/_images/ClusterDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_images/ClusterNearnessPlot_time_point_97.png` & `napatrackmater-5.1.2/_build/html/_images/ClusterNearnessPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_images/ClusterPlot_time_point_97.png` & `napatrackmater-5.1.2/_build/html/_images/ClusterPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_images/FeatureMatrixPlot_time_point_97.png` & `napatrackmater-5.1.2/_build/html/_images/FeatureMatrixPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_images/QuadrantDistributionPlot_time_point_97.png` & `napatrackmater-5.1.2/_build/html/_images/QuadrantDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_sources/MASTER.md` & `napatrackmater-5.1.2/_build/html/_sources/MASTER.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_sources/Notebooks/Track_vector.ipynb` & `napatrackmater-5.1.2/_build/html/_sources/Notebooks/Track_vector.ipynb`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_sources/README.md` & `napatrackmater-5.1.2/_build/html/_sources/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css` & `napatrackmater-5.1.2/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_sphinx_design_static/design-tabs.js` & `napatrackmater-5.1.2/_build/html/_sphinx_design_static/design-tabs.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/basic.css` & `napatrackmater-5.1.2/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/clipboard.min.js` & `napatrackmater-5.1.2/_build/html/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/copybutton.css` & `napatrackmater-5.1.2/_build/html/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/copybutton.js` & `napatrackmater-5.1.2/_build/html/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/copybutton_funcs.js` & `napatrackmater-5.1.2/_build/html/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css` & `napatrackmater-5.1.2/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/design-tabs.js` & `napatrackmater-5.1.2/_build/html/_static/design-tabs.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/doctools.js` & `napatrackmater-5.1.2/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/images/logo_binder.svg` & `napatrackmater-5.1.2/_build/html/_static/images/logo_binder.svg`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/images/logo_colab.png` & `napatrackmater-5.1.2/_build/html/_static/images/logo_colab.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/images/logo_deepnote.svg` & `napatrackmater-5.1.2/_build/html/_static/images/logo_deepnote.svg`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/images/logo_jupyterhub.svg` & `napatrackmater-5.1.2/_build/html/_static/images/logo_jupyterhub.svg`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/jquery-3.5.1.js` & `napatrackmater-5.1.2/_build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/jquery.js` & `napatrackmater-5.1.2/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/kapoorlablogo.png` & `napatrackmater-5.1.2/_build/html/_static/kapoorlablogo.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/language_data.js` & `napatrackmater-5.1.2/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po` & `napatrackmater-5.1.2/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css` & `napatrackmater-5.1.2/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/pygments.css` & `napatrackmater-5.1.2/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/scripts/bootstrap.js` & `napatrackmater-5.1.2/_build/html/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/scripts/bootstrap.js.map` & `napatrackmater-5.1.2/_build/html/_static/scripts/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/scripts/pydata-sphinx-theme.js` & `napatrackmater-5.1.2/_build/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/scripts/pydata-sphinx-theme.js.map` & `napatrackmater-5.1.2/_build/html/_static/scripts/pydata-sphinx-theme.js.map`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/scripts/sphinx-book-theme.js` & `napatrackmater-5.1.2/_build/html/_static/scripts/sphinx-book-theme.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/scripts/sphinx-book-theme.js.map` & `napatrackmater-5.1.2/_build/html/_static/scripts/sphinx-book-theme.js.map`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/searchtools.js` & `napatrackmater-5.1.2/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/sphinx-thebe.css` & `napatrackmater-5.1.2/_build/html/_static/sphinx-thebe.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/sphinx-thebe.js` & `napatrackmater-5.1.2/_build/html/_static/sphinx-thebe.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/styles/bootstrap.css` & `napatrackmater-5.1.2/_build/html/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/styles/pydata-sphinx-theme.css` & `napatrackmater-5.1.2/_build/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/styles/sphinx-book-theme.css` & `napatrackmater-5.1.2/_build/html/_static/styles/sphinx-book-theme.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/togglebutton.css` & `napatrackmater-5.1.2/_build/html/_static/togglebutton.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/togglebutton.js` & `napatrackmater-5.1.2/_build/html/_static/togglebutton.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/underscore-1.13.1.js` & `napatrackmater-5.1.2/_build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/underscore.js` & `napatrackmater-5.1.2/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt` & `napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css` & `napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf` & `napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2` & `napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf` & `napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2` & `napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf` & `napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2` & `napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf` & `napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2` & `napatrackmater-5.1.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/_static/webpack-macros.html` & `napatrackmater-5.1.2/_build/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/genindex.html` & `napatrackmater-5.1.2/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/search.html` & `napatrackmater-5.1.2/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/html/searchindex.js` & `napatrackmater-5.1.2/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_build/jupyter_execute/Notebooks/Track_vector.ipynb` & `napatrackmater-5.1.2/_build/jupyter_execute/Notebooks/Track_vector.ipynb`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/_config.yml` & `napatrackmater-5.1.2/_config.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/images/ClusterDistributionPlot_time_point_97.png` & `napatrackmater-5.1.2/images/ClusterDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/images/ClusterNearnessPlot_time_point_97.png` & `napatrackmater-5.1.2/images/ClusterNearnessPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/images/ClusterPlot_time_point_97.png` & `napatrackmater-5.1.2/images/ClusterPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/images/FeatureMatrixPlot_time_point_97.png` & `napatrackmater-5.1.2/images/FeatureMatrixPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/images/QuadrantDistributionPlot_time_point_97.png` & `napatrackmater-5.1.2/images/QuadrantDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/images/kapoorlablogo.png` & `napatrackmater-5.1.2/images/kapoorlablogo.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/images/kapoorlogo.png` & `napatrackmater-5.1.2/images/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/setup.cfg` & `napatrackmater-5.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/src/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-5.1.2/src/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/src/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-5.1.2/src/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/src/napatrackmater/Trackmate.py` & `napatrackmater-5.1.2/src/napatrackmater/Trackmate.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,27 +42,33 @@
         image: np.ndarray = None,
         mask: np.ndarray = None,
         fourier=True,
         autoencoder_model=None,
         num_points=2048,
         batch_size=1,
         compute_with_autoencoder=True,
+        variable_t_calibration: dict = None,
+        oneat_csv_file: str = None,
+        oneat_threshold_cutoff: int = 0.5,
     ):
 
         self.xml_path = xml_path
         self.master_xml_path = master_xml_path
         self.spot_csv_path = spot_csv_path
         self.track_csv_path = track_csv_path
         self.edges_csv_path = edges_csv_path
         self.accelerator = accelerator
         self.devices = devices
         self.scale_z = scale_z
         self.scale_xy = scale_xy
         self.center = center
         self.compute_with_autoencoder = compute_with_autoencoder
+        self.variable_t_calibration = variable_t_calibration
+        self.oneat_csv_file = oneat_csv_file
+        self.oneat_threshold_cutoff = oneat_threshold_cutoff
         self.latent_features = latent_features
         self.pretrainer = Trainer(accelerator=self.accelerator, devices=self.devices)
         if image is not None:
             self.image = image.astype(np.uint8)
         else:
             self.image = image
         if mask is not None:
@@ -188,14 +194,15 @@
         self.surface_area_key = "cloud_surfacearea"
         self.radial_angle_z_key = "radial_angle_z_key"
         self.radial_angle_y_key = "radial_angle_y_key"
         self.radial_angle_x_key = "radial_angle_x_key"
         self.motion_angle_z_key = "motion_angle_z"
         self.motion_angle_y_key = "motion_angle_y"
         self.motion_angle_x_key = "motion_angle_x"
+        self.local_cell_density_key = "local_density"
         self.latent_shape_features_key = "latent_shape_features"
 
         self.mean_intensity_ch1_key = self.track_analysis_spot_keys[
             "mean_intensity_ch1"
         ]
         self.mean_intensity_ch2_key = self.track_analysis_spot_keys[
             "mean_intensity_ch2"
@@ -234,26 +241,30 @@
         self.unique_track_properties = {}
         self.unique_fft_properties = {}
         self.unique_cluster_properties = {}
         self.unique_shape_properties = {}
         self.unique_dynamic_properties = {}
         self.unique_spot_properties = {}
         self.unique_spot_centroid = {}
+        self.unique_oneat_spot_centroid = {}
         self.unique_track_centroid = {}
+
         self.root_spots = {}
         self.all_current_cell_ids = {}
         self.channel_unique_spot_properties = {}
         self.edge_target_lookup = {}
         self.edge_source_lookup = {}
         self.generation_dict = {}
         self.tracklet_dict = {}
         self.graph_split = {}
         self.graph_tracks = {}
         self._timed_centroid = {}
+        self.oneat_dividing_tracks = {}
         self.count = 0
+        self.cell_veto_box = 0
         xml_parser = et.XMLParser(huge_tree=True)
         if self.master_xml_path is None:
             self.master_xml_path = Path(".")
 
         if self.master_xml_path.is_dir() and self.xml_path is not None:
             print("Reading XML")
             self.xml_content = et.fromstring(
@@ -374,14 +385,21 @@
             self.edges_dataset,
             self.edges_dataset_index,
             self.track_analysis_spot_keys,
             self.track_analysis_edges_keys,
         )
         print("obtained edge attributes")
 
+    def _get_cell_sizes(self):
+
+        print("Getting largest cell size")
+        if self.seg_image is not None:
+            self.timed_cell_size = get_largest_size(compute_cell_size(self.seg_image))
+        self.cell_veto_box = 4 * self.timed_cell_size
+
     def _get_boundary_points(self):
 
         print("Computing boundary points")
         if self.mask is not None:
 
             if self.channel_seg_image is not None:
 
@@ -452,14 +470,15 @@
         return all_source_ids, all_target_ids
 
     def _create_generations(self, all_source_ids: list):
 
         root_leaf = []
         root_root = []
         root_splits = []
+
         # Get the root id
         for source_id in all_source_ids:
             if source_id in self.edge_source_lookup:
                 source_target_id = self.edge_source_lookup[source_id]
             else:
                 source_target_id = None
             target_target_id = self.edge_target_lookup[source_id]
@@ -468,14 +487,19 @@
                     root_root.append(source_id)
             if len(target_target_id) > 1:
                 if source_id not in root_splits:
                     root_splits.append(source_id)
             if target_target_id[0] not in self.edge_target_lookup:
                 root_leaf.append(target_target_id[0])
 
+        if len(list(self.oneat_dividing_tracks.keys())) > 1:
+            for cell_id in list(self.oneat_dividing_tracks.keys()):
+                if cell_id in all_source_ids:
+                    root_splits.append(cell_id)
+
         return root_root, root_splits, root_leaf
 
     def _sort_dividing_cells(self, root_splits):
         cell_id_times = []
         split_cell_ids = []
         for root_split in root_splits:
             split_cell_id_time = self.unique_spot_properties[root_split][
@@ -647,21 +671,40 @@
             self._unique_tracklet_count(tracklet_count_taken, tracklet_count)
         return tracklet_count
 
     def _iterate_split_down(self, root_root, root_leaf, root_splits):
 
         self._iterate_dividing(root_root, root_leaf, root_splits)
 
+    def _get_label_density(self, frame, test_location):
+
+        current_frame_image = self.seg_image[int(float(frame)), :]
+        z_test, y_test, x_test = test_location
+
+        min_z = max(0, int(z_test - self.cell_veto_box))
+        max_z = min(current_frame_image.shape[0] - 1, int(z_test + self.cell_veto_box))
+        min_y = max(0, int(y_test - self.cell_veto_box))
+        max_y = min(current_frame_image.shape[1] - 1, int(y_test + self.cell_veto_box))
+        min_x = max(0, int(x_test - self.cell_veto_box))
+        max_x = min(current_frame_image.shape[2] - 1, int(x_test + self.cell_veto_box))
+
+        subvolume = current_frame_image[
+            min_z : max_z + 1, min_y : max_y + 1, min_x : max_x + 1
+        ]
+        unique_labels = np.unique(subvolume)
+        local_cell_density = len(unique_labels)
+
+        return local_cell_density
+
     def _get_boundary_dist(self, frame, testlocation):
 
         if self.mask is not None:
 
             tree, indices, maskcentroid = self.timed_mask[str(int(float(frame)))]
 
-            # Get the location and distance to the nearest boundary point
             distance_cell_mask, locationindex = tree.query(testlocation)
             distance_cell_mask = max(0, distance_cell_mask)
 
         else:
             distance_cell_mask = 0
             maskcentroid = (1, 1, 1)
 
@@ -843,16 +886,16 @@
             frame_spot_centroid = (
                 t,
                 round(z) / self.zcalibration,
                 round(y) / self.ycalibration,
                 round(x) / self.xcalibration,
             )
 
-            self.unique_spot_centroid[frame_spot_centroid] = k
             self.unique_track_centroid[frame_spot_centroid] = track_id
+            self.unique_spot_centroid[frame_spot_centroid] = k
 
             if str(t) in self._timed_centroid:
                 tree, spot_centroids = self._timed_centroid[str(t)]
                 spot_centroids.append(spot_centroid)
                 tree = spatial.cKDTree(spot_centroids)
                 self._timed_centroid[str(t)] = tree, spot_centroids
             else:
@@ -1102,14 +1145,15 @@
         radial_angle_x = float(all_dict_values[self.radial_angle_x_key])
 
         radius = float(all_dict_values[self.radius_key])
         radius_pixel = int(float(all_dict_values[self.quality_key]))
         total_intensity = float(all_dict_values[self.total_intensity_key])
 
         distance_cell_mask = float(all_dict_values[self.distance_cell_mask_key])
+        local_cell_density = float(all_dict_values[self.local_cell_density_key])
 
         track_displacement = float(all_dict_values[self.displacement_key])
         total_track_distance = float(all_dict_values[self.total_track_distance_key])
         max_track_distance = float(all_dict_values[self.max_distance_traveled_key])
         track_duration = float(all_dict_values[self.track_duration_key])
 
         if self.latent_shape_features_key in all_dict_values.keys():
@@ -1183,14 +1227,15 @@
                 total_intensity,
                 speed,
                 motion_angle_z,
                 motion_angle_y,
                 motion_angle_x,
                 acceleration,
                 distance_cell_mask,
+                local_cell_density,
                 radial_angle_z,
                 radial_angle_y,
                 radial_angle_x,
                 cell_axis_z,
                 cell_axis_y,
                 cell_axis_x,
                 track_displacement,
@@ -1241,14 +1286,15 @@
                 total_intensity,
                 speed,
                 motion_angle_z,
                 motion_angle_y,
                 motion_angle_x,
                 acceleration,
                 distance_cell_mask,
+                local_cell_density,
                 radial_angle_z,
                 radial_angle_y,
                 radial_angle_x,
                 cell_axis_z,
                 cell_axis_y,
                 cell_axis_x,
                 track_displacement,
@@ -1288,14 +1334,17 @@
                     self.total_intensity_key: total_intensity,
                     self.mean_intensity_key: mean_intensity,
                     self.radius_key: radius,
                     self.quality_key: quality,
                     self.distance_cell_mask_key: (
                         float(Spotobject.get(self.distance_cell_mask_key))
                     ),
+                    self.local_cell_density_key: (
+                        float(Spotobject.get(self.local_cell_density_key))
+                    ),
                     self.uniqueid_key: str(Spotobject.get(self.uniqueid_key)),
                     self.trackletid_key: str(Spotobject.get(self.trackletid_key)),
                     self.generationid_key: str(Spotobject.get(self.generationid_key)),
                     self.trackid_key: str(Spotobject.get(self.trackid_key)),
                     self.motion_angle_z_key: (
                         float(Spotobject.get(self.motion_angle_z_key))
                     ),
@@ -1403,30 +1452,41 @@
                 float(Spotobject.get(self.xposid_key)),
             )
             frame = Spotobject.get(self.frameid_key)
             distance_cell_mask, maskcentroid = self._get_boundary_dist(
                 frame, testlocation
             )
 
+            local_cell_density = self._get_label_density(frame, testlocation)
+
             self.unique_spot_properties[cell_id] = {
                 self.cellid_key: int(cell_id),
                 self.frameid_key: int(float(Spotobject.get(self.frameid_key))),
                 self.zposid_key: float(Spotobject.get(self.zposid_key)),
                 self.yposid_key: float(Spotobject.get(self.yposid_key)),
                 self.xposid_key: float(Spotobject.get(self.xposid_key)),
                 self.total_intensity_key: TOTAL_INTENSITY,
                 self.mean_intensity_key: MEAN_INTENSITY,
                 self.radius_key: RADIUS,
                 self.quality_key: QUALITY,
                 self.distance_cell_mask_key: float(distance_cell_mask),
                 self.maskcentroid_z_key: float(maskcentroid[0]),
                 self.maskcentroid_y_key: float(maskcentroid[1]),
                 self.maskcentroid_x_key: float(maskcentroid[2]),
+                self.local_cell_density_key: float(local_cell_density),
             }
 
+            frame_spot_centroid = (
+                int(float(Spotobject.get(self.frameid_key))),
+                float(Spotobject.get(self.zposid_key)) / self.zcalibration,
+                float(Spotobject.get(self.yposid_key)) / self.ycalibration,
+                float(Spotobject.get(self.xposid_key)) / self.xcalibration,
+            )
+            self.unique_oneat_spot_centroid[frame_spot_centroid] = cell_id
+
     def _get_master_xml_data(self):
         if self.channel_seg_image is not None:
             self.channel_xml_content = self.xml_content
             self.xml_tree = et.parse(self.xml_path)
             self.xml_root = self.xml_tree.getroot()
             base_name = os.path.splitext(os.path.basename(self.xml_path))[0]
             if "nuclei" in base_name:
@@ -1591,23 +1651,28 @@
                 new_quality = self.channel_unique_spot_properties[cell_id][
                     self.quality_key
                 ]
                 new_distance_cell_mask = self.channel_unique_spot_properties[cell_id][
                     self.distance_cell_mask_key
                 ]
 
+                new_local_density = self.channel_unique_spot_properties[cell_id][
+                    self.local_cell_density_key
+                ]
+
                 Spotobject.set(self.xposid_key, str(new_positionx))
                 Spotobject.set(self.yposid_key, str(new_positiony))
                 Spotobject.set(self.zposid_key, str(new_positionz))
 
                 Spotobject.set(self.total_intensity_key, str(new_total_intensity))
                 Spotobject.set(self.mean_intensity_key, str(new_mean_intensity))
                 Spotobject.set(self.radius_key, str(new_radius))
                 Spotobject.set(self.quality_key, str(new_quality))
                 Spotobject.set(self.distance_cell_mask_key, str(new_distance_cell_mask))
+                Spotobject.set(self.local_cell_density_key, str(new_local_density))
                 track_id = self.channel_unique_spot_properties[int(cell_id)][
                     self.trackid_key
                 ]
                 channel_filtered_tracks.append(track_id)
 
         self.xml_tree.write(os.path.join(self.channel_xml_path, self.channel_xml_name))
 
@@ -1674,15 +1739,17 @@
             "DetectorSettings"
         )
         self.basicsettings = self.xml_content.find("Settings").find("BasicSettings")
         self.detectorchannel = int(float(self.detectorsettings.get("TARGET_CHANNEL")))
         self.tstart = int(float(self.basicsettings.get("tstart")))
         self.tend = int(float(self.basicsettings.get("tend")))
         self._get_boundary_points()
+        self._get_cell_sizes()
         print("Iterating over spots in frame")
+
         self.count = 0
         futures = []
 
         with concurrent.futures.ThreadPoolExecutor(
             max_workers=os.cpu_count()
         ) as executor:
 
@@ -1698,14 +1765,16 @@
                 self.progress_bar.show()
 
             for r in concurrent.futures.as_completed(futures):
                 self.count = self.count + 1
                 if self.progress_bar is not None:
                     self.progress_bar.value = self.count
                 r.result()
+
+        self._correct_track_status()
         print(f"Iterating over tracks {len(self.filtered_track_ids)}")
         self.count = 0
         if self.progress_bar is not None:
             self.progress_bar.label = "Collecting Tracks"
             self.progress_bar.range = (0, len(self.filtered_track_ids))
             self.progress_bar.show()
 
@@ -1767,14 +1836,34 @@
             track = self.filtered_tracks[index]
             self._final_tracks(track_id)
 
         print("computing Phenotypes")
         self._compute_phenotypes()
         self._temporal_plots_trackmate()
 
+    def _correct_track_status(self):
+
+        if self.oneat_csv_file is not None:
+            print("Improving mitosis track classification using Oneat")
+            detections = pd.read_csv(self.oneat_csv_file, delimiter=",")
+            cutoff_score = self.oneat_threshold_cutoff
+            filtered_detections = detections[detections["Score"] > cutoff_score]
+
+            for index, row in filtered_detections.iterrows():
+                t = int(row["T"])
+                z = round(row["Z"])
+                y = round(row["Y"])
+                x = round(row["X"])
+
+                spot = (t, z, y, x)
+
+                spot_id = find_closest_key(spot, self.unique_oneat_spot_centroid, 0, 5)
+                if spot_id is not None:
+                    self.oneat_dividing_tracks[spot_id] = spot
+
     def _create_master_xml(self):
 
         for Spotobject in self.master_xml_root.iter("Spot"):
             cell_id = int(Spotobject.get(self.spotid_key))
             if cell_id in self.unique_spot_properties.keys():
 
                 for k in self.unique_spot_properties[cell_id].keys():
@@ -2063,33 +2152,34 @@
 
             motion_angle_z = tracklet_properties[:, 11]
             motion_angle_y = tracklet_properties[:, 12]
             motion_angle_x = tracklet_properties[:, 13]
 
             acceleration = tracklet_properties[:, 14]
             distance_cell_mask = tracklet_properties[:, 15]
+            local_density = tracklet_properties[:, 16]
 
-            radial_angle_z = tracklet_properties[:, 16]
-            radial_angle_y = tracklet_properties[:, 17]
-            radial_angle_x = tracklet_properties[:, 18]
+            radial_angle_z = tracklet_properties[:, 17]
+            radial_angle_y = tracklet_properties[:, 18]
+            radial_angle_x = tracklet_properties[:, 19]
 
-            cell_axis_z = tracklet_properties[:, 19]
-            cell_axis_y = tracklet_properties[:, 20]
-            cell_axis_x = tracklet_properties[:, 21]
+            cell_axis_z = tracklet_properties[:, 20]
+            cell_axis_y = tracklet_properties[:, 21]
+            cell_axis_x = tracklet_properties[:, 22]
 
-            track_displacement = tracklet_properties[:, 22]
+            track_displacement = tracklet_properties[:, 23]
 
-            total_track_distance = tracklet_properties[:, 23]
+            total_track_distance = tracklet_properties[:, 24]
 
-            max_track_distance = tracklet_properties[:, 24]
+            max_track_distance = tracklet_properties[:, 25]
 
-            track_duration = tracklet_properties[:, 25]
+            track_duration = tracklet_properties[:, 26]
 
-            if tracklet_properties.shape[1] > 25:
-                latent_shape_features = tracklet_properties[:, 26:]
+            if tracklet_properties.shape[1] > 26:
+                latent_shape_features = tracklet_properties[:, 27:]
             else:
                 latent_shape_features = []
 
             unique_fft_properties_tracklet = {}
             unique_cluster_properties_tracklet = {}
             self.unique_fft_properties[track_id] = {}
             self.unique_cluster_properties[track_id] = {}
@@ -2116,14 +2206,15 @@
                 current_speed = []
                 current_motion_angle_z = []
                 current_motion_angle_y = []
                 current_motion_angle_x = []
 
                 current_acceleration = []
                 current_distance_cell_mask = []
+                current_local_density = []
                 current_eccentricity_comp_first = []
                 current_eccentricity_comp_second = []
                 current_eccentricity_comp_third = []
                 current_surface_area = []
                 current_latent_shape_features = []
                 current_radial_angle_z = []
                 current_radial_angle_y = []
@@ -2149,14 +2240,15 @@
                         current_speed.append(speed[j])
                         current_motion_angle_z.append(motion_angle_z[j])
                         current_motion_angle_y.append(motion_angle_y[j])
                         current_motion_angle_x.append(motion_angle_x[j])
 
                         current_acceleration.append(acceleration[j])
                         current_distance_cell_mask.append(distance_cell_mask[j])
+                        current_local_density.append(local_density[j])
                         current_eccentricity_comp_first.append(
                             eccentricity_comp_first[j]
                         )
                         current_eccentricity_comp_second.append(
                             eccentricity_comp_second[j]
                         )
                         current_eccentricity_comp_third.append(
@@ -2217,14 +2309,18 @@
                 )
                 current_acceleration = np.asarray(
                     current_acceleration, dtype=np.float32
                 )
                 current_distance_cell_mask = np.asarray(
                     current_distance_cell_mask, dtype=np.float32
                 )
+
+                current_local_density = np.asarray(
+                    current_local_density, dtype=np.float32
+                )
                 current_radial_angle_z = np.asarray(
                     current_radial_angle_z, dtype=np.float32
                 )
                 current_radial_angle_y = np.asarray(
                     current_radial_angle_y, dtype=np.float32
                 )
                 current_radial_angle_x = np.asarray(
@@ -2279,14 +2375,15 @@
                     current_time,
                     current_speed,
                     current_motion_angle_z,
                     current_motion_angle_y,
                     current_motion_angle_x,
                     current_acceleration,
                     current_distance_cell_mask,
+                    current_local_density,
                     current_radial_angle_z,
                     current_radial_angle_y,
                     current_radial_angle_x,
                     current_cell_axis_z,
                     current_cell_axis_y,
                     current_cell_axis_x,
                     current_track_displacement,
@@ -2353,27 +2450,29 @@
         QUALITY = math.pow(volume[index], 1.0 / 3.0)
         RADIUS = math.pow(
             volume[index] * self.xcalibration * self.ycalibration * self.zcalibration,
             1.0 / 3.0,
         )
 
         distance_cell_mask, maskcentroid = self._get_boundary_dist(frame, location)
+        local_density = self._get_label_density(frame, location)
         if dist <= 2 * veto_radius:
             self.channel_unique_spot_properties[cell_id] = {
                 self.cellid_key: int(cell_id),
                 self.frameid_key: int(frame),
                 self.zposid_key: float(centroids[index][0] * self.zcalibration),
                 self.yposid_key: float(centroids[index][1] * self.ycalibration),
                 self.xposid_key: float(centroids[index][2] * self.xcalibration),
                 self.trackid_key: int(track_id),
                 self.total_intensity_key: (float(intensity_total[index])),
                 self.mean_intensity_key: (float(intensity_mean[index])),
                 self.radius_key: (float(RADIUS)),
                 self.quality_key: (float(QUALITY)),
                 self.distance_cell_mask_key: float(distance_cell_mask),
+                self.local_cell_density_key: float(local_density),
                 self.maskcentroid_z_key: float(maskcentroid[0]),
                 self.maskcentroid_y_key: float(maskcentroid[1]),
                 self.maskcentroid_x_key: float(maskcentroid[2]),
             }
         else:
             self.channel_unique_spot_properties[cell_id] = self.unique_spot_properties[
                 cell_id
@@ -2383,23 +2482,34 @@
             )
             self.channel_unique_spot_properties[cell_id].update(
                 {self.mean_intensity_key: -1}
             )
             self.channel_unique_spot_properties[cell_id].update({self.radius_key: -1})
             self.channel_unique_spot_properties[cell_id].update({self.quality_key: -1})
 
+    def _get_cal(self, frame):
+
+        frame = int(float(frame))
+
+        if self.variable_t_calibration is not None:
+
+            for key_time in sorted(self.variable_t_calibration.keys()):
+                key_time = int(float(key_time))
+                if frame <= key_time:
+                    self.tcalibration = float(self.variable_t_calibration[key_time])
+                    return
+
     def _dict_update(
         self,
         unique_tracklet_ids: List,
         cell_id: int,
         track_id: int,
         source_id: int,
         target_id: int,
     ):
-
         generation_id = self.generation_dict[cell_id]
         tracklet_id = self.tracklet_dict[cell_id]
 
         unique_id = str(track_id) + str(generation_id) + str(tracklet_id)
 
         vec_cell = [
             float(self.unique_spot_properties[int(cell_id)][self.xposid_key]),
@@ -2459,15 +2569,36 @@
                 float(self.unique_spot_properties[int(cell_id)][self.xposid_key])
                 - float(self.unique_spot_properties[int(source_id)][self.xposid_key]),
                 float(self.unique_spot_properties[int(cell_id)][self.yposid_key])
                 - float(self.unique_spot_properties[int(source_id)][self.yposid_key]),
                 float(self.unique_spot_properties[int(cell_id)][self.zposid_key])
                 - float(self.unique_spot_properties[int(source_id)][self.zposid_key]),
             ]
-            speed = np.sqrt(np.dot(vec_1, vec_1)) / self.tcalibration
+
+            time_vec_1 = max(
+                1,
+                abs(
+                    int(
+                        float(
+                            self.unique_spot_properties[int(cell_id)][self.frameid_key]
+                        )
+                        - float(
+                            self.unique_spot_properties[int(source_id)][
+                                self.frameid_key
+                            ]
+                        )
+                    )
+                ),
+            )
+            frame = int(
+                float(self.unique_spot_properties[int(cell_id)][self.frameid_key])
+            )
+            self._get_cal(frame)
+
+            speed = np.sqrt(np.dot(vec_1, vec_1)) / (time_vec_1 * self.tcalibration)
             self.unique_spot_properties[int(cell_id)].update({self.speed_key: speed})
 
             motion_angle_x = cell_angular_change_x(vec_1)
             motion_angle_y = cell_angular_change_y(vec_1)
             motion_angle_z = cell_angular_change_z(vec_1)
 
             self.unique_spot_properties[int(cell_id)].update(
@@ -2507,15 +2638,34 @@
                     * float(
                         self.unique_spot_properties[int(source_id)][self.zposid_key]
                     )
                     + float(
                         self.unique_spot_properties[int(pre_source_id)][self.zposid_key]
                     ),
                 ]
-                acc = np.sqrt(np.dot(vec_2, vec_2)) / self.tcalibration
+
+                time_vec_2 = max(
+                    1,
+                    abs(
+                        int(
+                            float(
+                                self.unique_spot_properties[int(cell_id)][
+                                    self.frameid_key
+                                ]
+                            )
+                            - float(
+                                self.unique_spot_properties[int(pre_source_id)][
+                                    self.frameid_key
+                                ]
+                            )
+                        )
+                    ),
+                )
+
+                acc = np.sqrt(np.dot(vec_2, vec_2)) / (time_vec_2 * self.tcalibration)
 
                 self.unique_spot_properties[int(cell_id)].update(
                     {self.acceleration_key: acc}
                 )
         elif source_id is None:
             self.unique_spot_properties[int(cell_id)].update({self.beforeid_key: None})
 
@@ -2561,14 +2711,17 @@
 
         self.mitotic_mean_directional_change_x = []
         self.mitotic_var_directional_change_x = []
 
         self.mitotic_mean_distance_cell_mask = []
         self.mitotic_var_distance_cell_mask = []
 
+        self.mitotic_mean_local_cell_density = []
+        self.mitotic_var_local_cell_density = []
+
         self.non_mitotic_mean_disp_z = []
         self.non_mitotic_var_disp_z = []
 
         self.non_mitotic_mean_disp_y = []
         self.non_mitotic_var_disp_y = []
 
         self.non_mitotic_mean_disp_x = []
@@ -2591,14 +2744,17 @@
 
         self.non_mitotic_mean_directional_change_x = []
         self.non_mitotic_var_directional_change_x = []
 
         self.non_mitotic_mean_distance_cell_mask = []
         self.non_mitotic_var_distance_cell_mask = []
 
+        self.non_mitotic_mean_local_cell_density = []
+        self.non_mitotic_var_local_cell_density = []
+
         self.all_mean_disp_z = []
         self.all_var_disp_z = []
 
         self.all_mean_disp_y = []
         self.all_var_disp_y = []
 
         self.all_mean_disp_x = []
@@ -2621,14 +2777,23 @@
 
         self.all_mean_directional_change_x = []
         self.all_var_directional_change_x = []
 
         self.all_mean_distance_cell_mask = []
         self.all_var_distance_cell_mask = []
 
+        self.all_mean_distance_cell_mask = []
+        self.all_var_distance_cell_mask = []
+
+        self.all_mean_local_cell_density = []
+        self.all_var_local_cell_density = []
+
+        self.all_mean_local_cell_density = []
+        self.all_var_local_cell_density = []
+
         all_spots_tracks = {}
         for (k, v) in self.unique_spot_properties.items():
 
             all_spots = self.unique_spot_properties[k]
             if self.trackid_key in all_spots:
                 all_spots_tracks[k] = all_spots
 
@@ -2652,43 +2817,48 @@
         mitotic_radius = []
         mitotic_speed = []
         mitotic_acc = []
         mitotic_directional_change_z = []
         mitotic_directional_change_y = []
         mitotic_directional_change_x = []
         mitotic_distance_cell_mask = []
+        mitotic_local_cell_density = []
 
         non_mitotic_disp_z = []
         non_mitotic_disp_y = []
         non_mitotic_disp_x = []
         non_mitotic_radius = []
         non_mitotic_speed = []
         non_mitotic_acc = []
         non_mitotic_directional_change_z = []
         non_mitotic_directional_change_y = []
         non_mitotic_directional_change_x = []
         non_mitotic_distance_cell_mask = []
+        non_mitotic_local_cell_density = []
 
         all_disp_z = []
         all_disp_y = []
         all_disp_x = []
         all_radius = []
         all_speed = []
         all_acc = []
         all_directional_change_z = []
         all_directional_change_y = []
         all_directional_change_x = []
         all_distance_cell_mask = []
+        all_local_cell_density = []
 
         for (k, v) in all_spots_tracks.items():
 
             current_time = all_spots_tracks[k][self.frameid_key]
             mitotic = all_spots_tracks[k][self.dividing_key]
 
             if i == int(current_time):
+
+                self._get_cal(current_time)
                 if mitotic:
                     mitotic_disp_z.append(all_spots_tracks[k][self.zposid_key])
                     mitotic_disp_y.append(all_spots_tracks[k][self.yposid_key])
                     mitotic_disp_x.append(all_spots_tracks[k][self.xposid_key])
                     if all_spots_tracks[k][self.radius_key] > 0:
                         mitotic_radius.append(all_spots_tracks[k][self.radius_key])
                     else:
@@ -2703,14 +2873,17 @@
                     )
                     mitotic_directional_change_x.append(
                         all_spots_tracks[k][self.motion_angle_x_key]
                     )
                     mitotic_distance_cell_mask.append(
                         all_spots_tracks[k][self.distance_cell_mask_key]
                     )
+                    mitotic_local_cell_density.append(
+                        all_spots_tracks[k][self.local_cell_density_key]
+                    )
 
                 if not mitotic:
                     non_mitotic_disp_z.append(all_spots_tracks[k][self.zposid_key])
                     non_mitotic_disp_y.append(all_spots_tracks[k][self.yposid_key])
                     non_mitotic_disp_x.append(all_spots_tracks[k][self.xposid_key])
                     if all_spots_tracks[k][self.radius_key] > 0:
                         non_mitotic_radius.append(all_spots_tracks[k][self.radius_key])
@@ -2726,14 +2899,17 @@
                     )
                     non_mitotic_directional_change_x.append(
                         all_spots_tracks[k][self.motion_angle_x_key]
                     )
                     non_mitotic_distance_cell_mask.append(
                         all_spots_tracks[k][self.distance_cell_mask_key]
                     )
+                    non_mitotic_local_cell_density.append(
+                        all_spots_tracks[k][self.local_cell_density_key]
+                    )
 
                 all_disp_z.append(all_spots_tracks[k][self.zposid_key])
                 all_disp_y.append(all_spots_tracks[k][self.yposid_key])
                 all_disp_x.append(all_spots_tracks[k][self.xposid_key])
                 if all_spots_tracks[k][self.radius_key] > 0:
                     all_radius.append(all_spots_tracks[k][self.radius_key])
                 else:
@@ -2748,14 +2924,17 @@
                 )
                 all_directional_change_x.append(
                     all_spots_tracks[k][self.motion_angle_x_key]
                 )
                 all_distance_cell_mask.append(
                     all_spots_tracks[k][self.distance_cell_mask_key]
                 )
+                all_local_cell_density.append(
+                    all_spots_tracks[k][self.local_cell_density_key]
+                )
 
         mitotic_disp_z = np.abs(np.diff(mitotic_disp_z))
         mitotic_disp_y = np.abs(np.diff(mitotic_disp_y))
         mitotic_disp_x = np.abs(np.diff(mitotic_disp_x))
 
         non_mitotic_disp_z = np.abs(np.diff(non_mitotic_disp_z))
         non_mitotic_disp_y = np.abs(np.diff(non_mitotic_disp_y))
@@ -2807,14 +2986,17 @@
         self.mitotic_var_directional_change_x.append(
             np.std(mitotic_directional_change_x)
         )
 
         self.mitotic_mean_distance_cell_mask.append(np.mean(mitotic_distance_cell_mask))
         self.mitotic_var_distance_cell_mask.append(np.std(mitotic_distance_cell_mask))
 
+        self.mitotic_mean_local_cell_density.append(np.mean(mitotic_local_cell_density))
+        self.mitotic_var_local_cell_density.append(np.std(mitotic_local_cell_density))
+
         self.non_mitotic_mean_disp_z.append(np.mean(non_mitotic_disp_z))
         self.non_mitotic_var_disp_z.append(np.std(non_mitotic_disp_z))
 
         self.non_mitotic_mean_disp_y.append(np.mean(non_mitotic_disp_y))
         self.non_mitotic_var_disp_y.append(np.std(non_mitotic_disp_y))
 
         self.non_mitotic_mean_disp_x.append(np.mean(non_mitotic_disp_x))
@@ -2855,14 +3037,21 @@
         self.non_mitotic_mean_distance_cell_mask.append(
             np.mean(non_mitotic_distance_cell_mask)
         )
         self.non_mitotic_var_distance_cell_mask.append(
             np.std(non_mitotic_distance_cell_mask)
         )
 
+        self.non_mitotic_mean_local_cell_density.append(
+            np.mean(non_mitotic_local_cell_density)
+        )
+        self.non_mitotic_var_local_cell_density.append(
+            np.std(non_mitotic_local_cell_density)
+        )
+
         self.all_mean_disp_z.append(np.mean(all_disp_z))
         self.all_var_disp_z.append(np.std(all_disp_z))
 
         self.all_mean_disp_y.append(np.mean(all_disp_y))
         self.all_var_disp_y.append(np.std(all_disp_y))
 
         self.all_mean_disp_x.append(np.mean(all_disp_x))
@@ -2887,14 +3076,41 @@
 
         self.all_mean_directional_change_x.append(np.mean(all_directional_change_x))
         self.all_var_directional_change_x.append(np.std(all_directional_change_x))
 
         self.all_mean_distance_cell_mask.append(np.mean(all_distance_cell_mask))
         self.all_var_distance_cell_mask.append(np.std(all_distance_cell_mask))
 
+        self.all_mean_local_cell_density.append(np.mean(all_local_cell_density))
+        self.all_var_local_cell_density.append(np.std(all_local_cell_density))
+
+
+def get_largest_size(timed_cell_size):
+    largest_size = max(timed_cell_size.values())
+    return largest_size
+
+
+def compute_cell_size(seg_image):
+
+    ndim = len(seg_image.shape)
+    timed_cell_size = {}
+    if ndim == 2:
+        props = measure.regionprops(seg_image)
+        largest_size = max(props, key=lambda prop: prop.feret_diameter_max)
+        timed_cell_size[str(0)] = float(largest_size.feret_diameter_max)
+
+    if ndim in (3, 4):
+        for i in tqdm(range(0, seg_image.shape[0], int(seg_image.shape[0] / 10))):
+
+            props = measure.regionprops(seg_image[i, :])
+            largest_size = max(props, key=lambda prop: prop.feret_diameter_max)
+            timed_cell_size[str(i)] = float(largest_size.feret_diameter_max)
+
+    return timed_cell_size
+
 
 def boundary_points(mask, xcalibration, ycalibration, zcalibration):
 
     ndim = len(mask.shape)
     timed_mask = {}
     mask = mask > 0
     mask = mask.astype("uint8")
@@ -3063,14 +3279,37 @@
     TrackAttributeids.append(TrackAttributeBoxname)
     for attributename in track_analysis_track_keys.keys():
         TrackAttributeids.append(attributename)
 
     return TrackAttributeids, AllTrackValues
 
 
+def find_closest_key(test_point, unique_dict, time_veto, space_veto):
+    closest_key = None
+    spot_id = None
+    min_distance = float("inf")
+
+    t_test, z_test, y_test, x_test = test_point
+    for key in unique_dict.keys():
+        t_key, z_key, y_key, x_key = key
+
+        time_distance = abs(t_key - t_test)
+        space_distance = np.sqrt(
+            (z_key - z_test) ** 2 + (y_key - y_test) ** 2 + (x_key - x_test) ** 2
+        )
+
+        if time_distance <= time_veto and space_distance <= space_veto:
+            if time_distance + space_distance < min_distance:
+                min_distance = time_distance + space_distance
+                closest_key = key
+    if closest_key is not None:
+        spot_id = unique_dict[closest_key]
+    return spot_id
+
+
 def get_edges_dataset(
     edges_dataset,
     edges_dataset_index,
     track_analysis_spot_keys,
     track_analysis_edges_keys,
 ):
 
@@ -3191,30 +3430,33 @@
         "motion_angle_z": np.asarray(unique_tracks_properties, dtype="float16")[:, 11],
         "motion_angle_y": np.asarray(unique_tracks_properties, dtype="float16")[:, 12],
         "motion_angle_x": np.asarray(unique_tracks_properties, dtype="float16")[:, 13],
         "acceleration": np.asarray(unique_tracks_properties, dtype="float16")[:, 14],
         "distance_cell_mask": np.asarray(unique_tracks_properties, dtype="float16")[
             :, 15
         ],
-        "radial_angle_z": np.asarray(unique_tracks_properties, dtype="float16")[:, 16],
-        "radial_angle_y": np.asarray(unique_tracks_properties, dtype="float16")[:, 17],
-        "radial_angle_x": np.asarray(unique_tracks_properties, dtype="float16")[:, 18],
-        "cell_axis_z": np.asarray(unique_tracks_properties, dtype="float16")[:, 19],
-        "cell_axis_y": np.asarray(unique_tracks_properties, dtype="float16")[:, 20],
-        "cell_axis_x": np.asarray(unique_tracks_properties, dtype="float16")[:, 21],
+        "local_cell_density": np.asarray(unique_tracks_properties, dtype="float16")[
+            :, 16
+        ],
+        "radial_angle_z": np.asarray(unique_tracks_properties, dtype="float16")[:, 17],
+        "radial_angle_y": np.asarray(unique_tracks_properties, dtype="float16")[:, 18],
+        "radial_angle_x": np.asarray(unique_tracks_properties, dtype="float16")[:, 19],
+        "cell_axis_z": np.asarray(unique_tracks_properties, dtype="float16")[:, 20],
+        "cell_axis_y": np.asarray(unique_tracks_properties, dtype="float16")[:, 21],
+        "cell_axis_x": np.asarray(unique_tracks_properties, dtype="float16")[:, 22],
         "track_displacement": np.asarray(unique_tracks_properties, dtype="float16")[
-            :, 22
+            :, 23
         ],
         "total_track_distance": np.asarray(unique_tracks_properties, dtype="float16")[
-            :, 23
+            :, 24
         ],
         "max_track_distance": np.asarray(unique_tracks_properties, dtype="float16")[
-            :, 24
+            :, 25
         ],
-        "track_duration": np.asarray(unique_tracks_properties, dtype="float16")[:, 25],
+        "track_duration": np.asarray(unique_tracks_properties, dtype="float16")[:, 26],
     }
 
     return features
 
 
 def set_scale(dimensions, x_calibration, y_calibration, z_calibration):
```

### Comparing `napatrackmater-5.1.1/src/napatrackmater/Trackvector.py` & `napatrackmater-5.1.2/src/napatrackmater/Trackvector.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 SHAPE_FEATURES = [
     "Radius",
     "Radius_Pixel",
     "Eccentricity_Comp_First",
     "Eccentricity_Comp_Second",
     "Eccentricity_Comp_Third",
     "Surface_Area",
+    "Local_Cell_Density",
 ]
 
 DYNAMIC_FEATURES = [
     "Speed",
     "Motion_Angle_Z",
     "Motion_Angle_Y",
     "Motion_Angle_X",
@@ -307,14 +308,15 @@
                     current_y,
                     current_x,
                     radius,
                     radius_pixel,
                     eccentricity_comp_first,
                     eccentricity_comp_second,
                     eccentricity_comp_third,
+                    local_cell_density,
                     surface_area,
                     latent_features,
                 ) = unique_shape_properties_tracklet
 
                 track_id_array = np.ones(current_time.shape)
                 dividing_array = np.ones(current_time.shape)
                 number_dividing_array = np.ones(current_time.shape)
@@ -334,14 +336,15 @@
                         dividing_array,
                         number_dividing_array,
                         radius,
                         radius_pixel,
                         eccentricity_comp_first,
                         eccentricity_comp_second,
                         eccentricity_comp_third,
+                        local_cell_density,
                         surface_area,
                         speed,
                         motion_angle_z,
                         motion_angle_y,
                         motion_angle_x,
                         acceleration,
                         distance_cell_mask,
@@ -548,14 +551,15 @@
             unique_id = spot_properties[self.uniqueid_key]
             tracklet_id = spot_properties[self.trackletid_key]
             number_times_divided = spot_properties[self.number_dividing_key]
             surface_area = spot_properties[self.surface_area_key]
             eccentricity_comp_first = spot_properties[self.eccentricity_comp_firstkey]
             eccentricity_comp_second = spot_properties[self.eccentricity_comp_secondkey]
             eccentricity_comp_third = spot_properties[self.eccentricity_comp_thirdkey]
+            local_cell_density = spot_properties[self.local_cell_density_key]
             radius = spot_properties[self.radius_key]
             radius_pixel = spot_properties[self.quality_key]
             speed = spot_properties[self.speed_key]
 
             motion_angle_z = spot_properties[self.motion_angle_z_key]
             motion_angle_y = spot_properties[self.motion_angle_y_key]
             motion_angle_x = spot_properties[self.motion_angle_x_key]
@@ -573,14 +577,15 @@
                 "Unique_ID": unique_id,
                 "Tracklet_ID": tracklet_id,
                 "Number_Times_Divided": number_times_divided,
                 "Surface_Area": surface_area,
                 "Eccentricity_Comp_First": eccentricity_comp_first,
                 "Eccentricity_Comp_Second": eccentricity_comp_second,
                 "Eccentricity_Comp_Third": eccentricity_comp_third,
+                "Local_Cell_Density": local_cell_density,
                 "Radius": radius,
                 "Radius_Pixel": radius_pixel,
                 "Speed": speed,
                 "Motion_Angle_Z": motion_angle_z,
                 "Motion_Angle_Y": motion_angle_y,
                 "Motion_Angle_X": motion_angle_x,
                 "Acceleration": acceleration,
@@ -621,14 +626,15 @@
 
             cols_to_replace = [
                 "Radius",
                 "Radius_Pixel",
                 "Eccentricity_Comp_First",
                 "Eccentricity_Comp_Second",
                 "Eccentricity_Comp_Third",
+                "Local_Cell_Density",
                 "Surface_Area",
             ]
             shape_dynamic_dataframe[cols_to_replace] = shape_dynamic_dataframe[
                 cols_to_replace
             ].apply(lambda x: np.where(x < 0, np.nan, x))
             if len(latent_shape_features) > 0:
                 new_columns = [
```

### Comparing `napatrackmater-5.1.1/src/napatrackmater/__init__.py` & `napatrackmater-5.1.2/src/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/src/napatrackmater/clustering.py` & `napatrackmater-5.1.2/src/napatrackmater/clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         min_size: tuple = (2, 2, 2),
         progress_bar=None,
         batch_size=1,
         scale_z=1.0,
         scale_xy=1.0,
         center=True,
         compute_with_autoencoder=True,
+
     ):
 
         self.pretrainer = pretrainer
         self.accelerator = accelerator
         self.devices = devices
         self.label_image = label_image
         self.model = model
@@ -436,14 +437,15 @@
 
     output_labels = []
     output_cluster_centroid = []
     output_cloud_eccentricity = []
     output_cloud_surface_area = []
     output_eigenvectors = []
     output_eigenvalues = []
+    output_density = []
     output_dimensions = []
     dataset = PointCloudDataset(clouds, scale_z=scale_z, scale_xy=scale_xy)
     dataloader = DataLoader(dataset, batch_size=batch_size)
 
     output_cluster_centroid = output_cluster_centroid + [
         tuple(centroid_input) for centroid_input in centroids
     ]
```

### Comparing `napatrackmater-5.1.1/src/napatrackmater/fast_radius_regression.py` & `napatrackmater-5.1.2/src/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/src/napatrackmater/fate_mapping.py` & `napatrackmater-5.1.2/src/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/src/napatrackmater/pretrained.py` & `napatrackmater-5.1.2/src/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/src/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-5.1.2/src/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 5.1.1
+Version: 5.1.2
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/Kapoorlabs-CAPED/napatrackmater
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/napatrackmater/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/napatrackmater#README.md
```

### Comparing `napatrackmater-5.1.1/src/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-5.1.2/src/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.1/update_version.py` & `napatrackmater-5.1.2/update_version.py`

 * *Files identical despite different names*

