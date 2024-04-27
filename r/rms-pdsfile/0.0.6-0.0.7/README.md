# Comparing `tmp/rms_pdsfile-0.0.6.tar.gz` & `tmp/rms_pdsfile-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms_pdsfile-0.0.6.tar", last modified: Tue Apr 23 21:46:19 2024, max compression
+gzip compressed data, was "rms_pdsfile-0.0.7.tar", last modified: Sat Apr 27 17:57:28 2024, max compression
```

## Comparing `rms_pdsfile-0.0.6.tar` & `rms_pdsfile-0.0.7.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:46:19.287792 rms_pdsfile-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:46:19.271792 rms_pdsfile-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:46:19.275792 rms_pdsfile-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/.github/workflows/run-tests-and-opus.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-23 21:46:19.287792 rms_pdsfile-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:46:19.275792 rms_pdsfile-0.0.6/pdsfile/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-23 21:46:19.000000 rms_pdsfile-0.0.6/pdsfile/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:46:19.275792 rms_pdsfile-0.0.6/pdsfile/pds3file/
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:46:19.283792 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1513 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/ASTROM_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    61669 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/COCIRS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    46937 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/COISS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51098 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/CORSS_8xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2378 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/COSP_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25774 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/COUVIS_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22138 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/COUVIS_8xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    43611 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/COVIMS_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/COVIMS_8xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20096 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/EBROCC_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    77854 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/GO_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21822 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/HSTxx_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9721 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/JNOJIR_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7790 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/JNOJNC_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/JNOSP_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2380 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/NHSP_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    53813 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/NHxxxx_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1078 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/RES_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12928 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/RPX_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2523 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/VGIRIS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    64913 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/VGISS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12074 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/VG_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2483 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/VG_20xx.py
--rw-r--r--   0 runner    (1001) docker     (127)   129879 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/VG_28xx.py
--rw-r--r--   0 runner    (1001) docker     (127)    36492 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4823 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/rules/pytest_support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:46:19.283792 rms_pdsfile-0.0.6/pdsfile/pds3file/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    89512 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/tests/test_pds3file_blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    30950 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py
--rw-r--r--   0 runner    (1001) docker     (127)    35786 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/tests/test_pds3file_whitebox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:46:19.283792 rms_pdsfile-0.0.6/pdsfile/pds4file/
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds4file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:46:19.283792 rms_pdsfile-0.0.6/pdsfile/pds4file/rules/
--rw-r--r--   0 runner    (1001) docker     (127)    36279 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds4file/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23705 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds4file/rules/cassini_iss.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24866 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds4file/rules/cassini_vims.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4872 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds4file/rules/pytest_support.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    65261 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds4file/rules/uranus_occs_earthbased.py
--rw-r--r--   0 runner    (1001) docker     (127)   101120 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds4file/rules/uranus_occs_earthbased_primary_filespec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:46:19.283792 rms_pdsfile-0.0.6/pdsfile/pds4file/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds4file/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds4file/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    38184 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pds4file/tests/test_pds4file_blackbox.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    34894 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pdscache.py
--rw-r--r--   0 runner    (1001) docker     (127)   230983 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pdsfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19658 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/pdsviewable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pdsfile/preload_and_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:46:19.287792 rms_pdsfile-0.0.6/rms_pdsfile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-23 21:46:19.000000 rms_pdsfile-0.0.6/rms_pdsfile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-23 21:46:19.000000 rms_pdsfile-0.0.6/rms_pdsfile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 21:46:19.000000 rms_pdsfile-0.0.6/rms_pdsfile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 21:46:19.000000 rms_pdsfile-0.0.6/rms_pdsfile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 21:46:19.000000 rms_pdsfile-0.0.6/rms_pdsfile.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      761 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/run_tests_coverage.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:46:19.271792 rms_pdsfile-0.0.6/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:46:19.287792 rms_pdsfile-0.0.6/scripts/automated_tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1714 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/scripts/automated_tests/pdsfile_main_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 21:46:19.287792 rms_pdsfile-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:46:19.287792 rms_pdsfile-0.0.6/validation/
--rwxr-xr-x   0 runner    (1001) docker     (127)    18175 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/validation/pdsarchives.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31377 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/validation/pdschecksums.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3230 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/validation/pdsdata-sync.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    34502 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/validation/pdsdependency.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17150 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/validation/pdsindexshelf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31801 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/validation/pdsinfoshelf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    73841 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/validation/pdslinkshelf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29426 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/validation/re-validate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-04-23 21:46:15.000000 rms_pdsfile-0.0.6/validation/shelf-consistency-check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:57:28.583258 rms_pdsfile-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:57:28.567258 rms_pdsfile-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:57:28.571258 rms_pdsfile-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/.github/workflows/run-tests-and-opus.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-27 17:57:28.583258 rms_pdsfile-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:57:28.571258 rms_pdsfile-0.0.7/pdsfile/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 17:57:28.000000 rms_pdsfile-0.0.7/pdsfile/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:57:28.571258 rms_pdsfile-0.0.7/pdsfile/pds3file/
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:57:28.579258 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1513 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/ASTROM_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    61669 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/COCIRS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46937 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/COISS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51098 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/CORSS_8xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2378 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/COSP_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25774 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/COUVIS_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22138 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/COUVIS_8xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43611 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/COVIMS_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/COVIMS_8xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20096 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/EBROCC_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    77854 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/GO_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21822 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/HSTxx_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9721 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/JNOJIR_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7790 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/JNOJNC_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/JNOSP_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2380 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/NHSP_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53813 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/NHxxxx_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1078 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/RES_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12928 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/RPX_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2523 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/VGIRIS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    64913 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/VGISS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12074 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/VG_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2483 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/VG_20xx.py
+-rw-r--r--   0 runner    (1001) docker     (127)   129879 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/VG_28xx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36492 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4823 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/rules/pytest_support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:57:28.579258 rms_pdsfile-0.0.7/pdsfile/pds3file/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/tests/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    89512 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/tests/test_pds3file_blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30950 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35786 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/tests/test_pds3file_whitebox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:57:28.579258 rms_pdsfile-0.0.7/pdsfile/pds4file/
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds4file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:57:28.579258 rms_pdsfile-0.0.7/pdsfile/pds4file/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)    36279 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds4file/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23705 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds4file/rules/cassini_iss.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24866 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds4file/rules/cassini_vims.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4872 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds4file/rules/pytest_support.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    65123 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds4file/rules/uranus_occs_earthbased.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98630 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds4file/rules/uranus_occs_earthbased_primary_filespec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:57:28.579258 rms_pdsfile-0.0.7/pdsfile/pds4file/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds4file/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds4file/tests/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38081 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pds4file/tests/test_pds4file_blackbox.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34894 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pdscache.py
+-rw-r--r--   0 runner    (1001) docker     (127)   230983 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pdsfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19658 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/pdsviewable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pdsfile/preload_and_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:57:28.583258 rms_pdsfile-0.0.7/rms_pdsfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-27 17:57:28.000000 rms_pdsfile-0.0.7/rms_pdsfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-27 17:57:28.000000 rms_pdsfile-0.0.7/rms_pdsfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:57:28.000000 rms_pdsfile-0.0.7/rms_pdsfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-27 17:57:28.000000 rms_pdsfile-0.0.7/rms_pdsfile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-27 17:57:28.000000 rms_pdsfile-0.0.7/rms_pdsfile.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      761 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/run_tests_coverage.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:57:28.567258 rms_pdsfile-0.0.7/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:57:28.583258 rms_pdsfile-0.0.7/scripts/automated_tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1714 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/scripts/automated_tests/pdsfile_main_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-27 17:57:28.583258 rms_pdsfile-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:57:28.583258 rms_pdsfile-0.0.7/validation/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18175 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/validation/pdsarchives.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31377 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/validation/pdschecksums.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3230 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/validation/pdsdata-sync.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34502 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/validation/pdsdependency.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17150 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/validation/pdsindexshelf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31801 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/validation/pdsinfoshelf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    73841 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/validation/pdslinkshelf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29426 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/validation/re-validate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-04-27 17:57:24.000000 rms_pdsfile-0.0.7/validation/shelf-consistency-check.py
```

### Comparing `rms_pdsfile-0.0.6/.github/workflows/publish_to_pypi.yml` & `rms_pdsfile-0.0.7/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/.github/workflows/publish_to_test_pypi.yml` & `rms_pdsfile-0.0.7/.github/workflows/publish_to_test_pypi.yml`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/.github/workflows/run-tests-and-opus.yml` & `rms_pdsfile-0.0.7/.github/workflows/run-tests-and-opus.yml`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/.github/workflows/run-tests.yml` & `rms_pdsfile-0.0.7/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/.gitignore` & `rms_pdsfile-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/CODE_OF_CONDUCT.md` & `rms_pdsfile-0.0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/CONTRIBUTING.md` & `rms_pdsfile-0.0.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/LICENSE` & `rms_pdsfile-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/PKG-INFO` & `rms_pdsfile-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rms-pdsfile
-Version: 0.0.6
+Version: 0.0.7
 Summary: pdsfile
 Maintainer-email: "Robert S. French" <rfrench@seti.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/SETI/rms-pdsfile
 Project-URL: Repository, https://github.com/SETI/rms-pdsfile
 Project-URL: Source, https://github.com/SETI/rms-pdsfile
 Project-URL: Issues, https://github.com/SETI/rms-pdsfile/issues
```

### Comparing `rms_pdsfile-0.0.6/README.md` & `rms_pdsfile-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/conftest.py` & `rms_pdsfile-0.0.7/conftest.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/__init__.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/__init__.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/ASTROM_xxxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/ASTROM_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/COCIRS_xxxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/COCIRS_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/COISS_xxxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/COISS_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/CORSS_8xxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/CORSS_8xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/COSP_xxxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/COSP_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/COUVIS_0xxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/COUVIS_0xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/COUVIS_8xxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/COUVIS_8xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/COVIMS_0xxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/COVIMS_0xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/COVIMS_8xxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/COVIMS_8xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/EBROCC_xxxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/EBROCC_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/GO_0xxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/GO_0xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/HSTxx_xxxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/HSTxx_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/JNOJIR_xxxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/JNOJIR_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/JNOJNC_xxxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/JNOJNC_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/JNOSP_xxxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/JNOSP_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/NHSP_xxxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/NHSP_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/NHxxxx_xxxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/NHxxxx_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/RES_xxxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/RES_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/RPX_xxxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/RPX_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/VGIRIS_xxxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/VGIRIS_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/VGISS_xxxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/VGISS_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/VG_0xxx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/VG_0xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/VG_20xx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/VG_20xx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/VG_28xx.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/VG_28xx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/__init__.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/rules/pytest_support.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/rules/pytest_support.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/tests/helper.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/tests/helper.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/tests/test_pds3file_blackbox.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/tests/test_pds3file_blackbox.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/tests/test_pds3file_whitebox.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/tests/test_pds3file_whitebox.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py` & `rms_pdsfile-0.0.7/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds4file/__init__.py` & `rms_pdsfile-0.0.7/pdsfile/pds4file/__init__.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds4file/rules/__init__.py` & `rms_pdsfile-0.0.7/pdsfile/pds4file/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds4file/rules/cassini_iss.py` & `rms_pdsfile-0.0.7/pdsfile/pds4file/rules/cassini_iss.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds4file/rules/cassini_vims.py` & `rms_pdsfile-0.0.7/pdsfile/pds4file/rules/cassini_vims.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds4file/rules/pytest_support.py` & `rms_pdsfile-0.0.7/pdsfile/pds4file/rules/pytest_support.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds4file/rules/uranus_occs_earthbased.py` & `rms_pdsfile-0.0.7/pdsfile/pds4file/rules/uranus_occs_earthbased.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,14 @@
     ('u0_kao_91cm',         'kao0m91-vis-occ-1977-069-u0',       None,                               None),
     ('u0201_palomar_508cm', 'pal5m08-insb-occ-2002-210-u0201',   None,                               None),
     ('u2_teide_155cm',      'tei1m55-ir-occ-1977-357-u2',        None,                               None),
     ('u5_lco_250cm',        'lascam2m5-insb-occ-1978-100-u5',    None,                               None),
     ('u9_lco_250cm',        'lascam2m5-insb-occ-1979-161-u9',    None,                               None),
     ('u11_ctio_400cm',      'ctio4m0-insb-occ-1980-080-u11',     None,                               None),
     ('u12_ctio_400cm',      'ctio4m0-insb-occ-1980-229-u12',     'ctio4m0-insb-occ-1980-228-u12',    'ctio4m0-insb-occ-1980-228-u12'),
-    ('u12_eso_104cm',       'esosil1m04-insb-occ-1980-229-u12',  'esosil1m04-insb-occ-1980-228-u12', 'esosil1m04-insb-occ-1980-229-u12'),
     ('u12_eso_360cm',       'esosil3m6-insb-occ-1980-229-u12',   'esosil3m6-insb-occ-1980-228-u12',  'esosil3m6-insb-occ-1980-229-u12'),
     ('u12_lco_250cm',       'lascam2m5-insb-occ-1980-229-u12',   'lascam2m5-insb-occ-1980-228-u12',  None),
     ('u13_sso_390cm',       'sso3m9-insb-occ-1981-116-u13',      None,                               None),
     ('u14_ctio_150cm',      'ctio1m50-insb-occ-1982-112-u14',    None,                               None),
     ('u14_ctio_400cm',      'ctio4m0-ir-occ-1982-112-u14',       None,                               None),
     ('u14_eso_104cm',       'esosil1m04-insb-occ-1982-112-u14',  None,                               None),
     ('u14_lco_100cm',       'lascam1m0-ir-occ-1982-112-u14',     None,                               None),
```

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds4file/rules/uranus_occs_earthbased_primary_filespec.py` & `rms_pdsfile-0.0.7/pdsfile/pds4file/rules/uranus_occs_earthbased_primary_filespec.py`

 * *Files 4% similar despite different names*

```diff
@@ -399,34 +399,14 @@
     'bundles/uranus_occs_earthbased/uranus_occ_u34_irtf_320cm/data/rings/u34_irtf_320cm_2200nm_radius_five_egress_100m.xml',
     'bundles/uranus_occs_earthbased/uranus_occ_u34_irtf_320cm/data/rings/u34_irtf_320cm_2200nm_radius_four_ingress_100m.xml',
     'bundles/uranus_occs_earthbased/uranus_occ_u34_irtf_320cm/data/rings/u34_irtf_320cm_2200nm_radius_epsilon_egress_100m.xml',
     'bundles/uranus_occs_earthbased/uranus_occ_u34_irtf_320cm/data/rings/u34_irtf_320cm_2200nm_radius_alpha_ingress_100m.xml',
     'bundles/uranus_occs_earthbased/uranus_occ_u34_irtf_320cm/data/rings/u34_irtf_320cm_2200nm_radius_gamma_ingress_100m.xml',
     'bundles/uranus_occs_earthbased/uranus_occ_u34_irtf_320cm/data/global/u34_irtf_320cm_2200nm_radius_equator_ingress_100m.xml',
     'bundles/uranus_occs_earthbased/uranus_occ_u34_irtf_320cm/data/global/u34_irtf_320cm_2200nm_radius_equator_egress_100m.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/atmosphere/u12_eso_104cm_2200nm_counts-v-time_atmos_egress.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/rings/u12_eso_104cm_2200nm_radius_six_egress_100m.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/rings/u12_eso_104cm_2200nm_radius_eta_ingress_100m.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/rings/u12_eso_104cm_2200nm_radius_four_ingress_100m.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/rings/u12_eso_104cm_2200nm_radius_six_ingress_100m.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/rings/u12_eso_104cm_2200nm_radius_beta_ingress_100m.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/rings/u12_eso_104cm_2200nm_radius_five_egress_100m.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/rings/u12_eso_104cm_2200nm_radius_alpha_ingress_100m.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/rings/u12_eso_104cm_2200nm_radius_gamma_ingress_100m.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/rings/u12_eso_104cm_2200nm_radius_beta_egress_100m.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/rings/u12_eso_104cm_2200nm_radius_gamma_egress_100m.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/rings/u12_eso_104cm_2200nm_radius_delta_ingress_100m.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/rings/u12_eso_104cm_2200nm_radius_five_ingress_100m.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/rings/u12_eso_104cm_2200nm_radius_epsilon_egress_100m.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/rings/u12_eso_104cm_2200nm_radius_eta_egress_100m.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/rings/u12_eso_104cm_2200nm_radius_delta_egress_100m.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/rings/u12_eso_104cm_2200nm_radius_four_egress_100m.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/rings/u12_eso_104cm_2200nm_radius_alpha_egress_100m.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/global/u12_eso_104cm_2200nm_radius_equator_ingress_100m.xml',
-    'bundles/uranus_occs_earthbased/uranus_occ_u12_eso_104cm/data/global/u12_eso_104cm_2200nm_radius_equator_egress_100m.xml',
     'bundles/uranus_occs_earthbased/uranus_occ_u36_maunakea_380cm/data/rings/u36_maunakea_380cm_2200nm_radius_epsilon_egress_100m.xml',
     'bundles/uranus_occs_earthbased/uranus_occ_u36_maunakea_380cm/data/rings/u36_maunakea_380cm_2200nm_radius_eta_ingress_100m.xml',
     'bundles/uranus_occs_earthbased/uranus_occ_u36_maunakea_380cm/data/rings/u36_maunakea_380cm_2200nm_radius_delta_egress_100m.xml',
     'bundles/uranus_occs_earthbased/uranus_occ_u36_maunakea_380cm/data/rings/u36_maunakea_380cm_2200nm_radius_gamma_egress_100m.xml',
     'bundles/uranus_occs_earthbased/uranus_occ_u36_maunakea_380cm/data/rings/u36_maunakea_380cm_2200nm_radius_gamma_ingress_100m.xml',
     'bundles/uranus_occs_earthbased/uranus_occ_u36_maunakea_380cm/data/rings/u36_maunakea_380cm_2200nm_radius_beta_ingress_100m.xml',
     'bundles/uranus_occs_earthbased/uranus_occ_u36_maunakea_380cm/data/rings/u36_maunakea_380cm_2200nm_radius_delta_ingress_100m.xml',
```

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds4file/tests/helper.py` & `rms_pdsfile-0.0.7/pdsfile/pds4file/tests/helper.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pds4file/tests/test_pds4file_blackbox.py` & `rms_pdsfile-0.0.7/pdsfile/pds4file/tests/test_pds4file_blackbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,16 @@
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             # expected bundles for uranus are coming from staging server
             # /volumes/pdsdata-admin/pds4-holdings/bundles/uranus_occs_earthbased
             ('uranus_occs_earthbased/',
              ['checksums_uranus_occs_earthbased',
-              'known-errors.txt',
+              'superseded',
+              'uranus_occ_support',
               'uranus_occ_u11_ctio_400cm',
               'uranus_occ_u23_ctio_400cm',
               'uranus_occ_u149_lowell_180cm',
               'uranus_occ_u138_palomar_508cm',
               'uranus_occ_u36_sso_390cm',
               'uranus_occ_u12_eso_360cm',
               'uranus_occ_u15_mso_190cm',
@@ -407,16 +408,14 @@
               'uranus_occ_u9539_ctio_400cm',
               'uranus_occ_u14_lco_250cm',
               'uranus_occ_u14_lco_100cm',
               'uranus_occ_u103_eso_220cm',
               'uranus_occ_u14_opmt_200cm',
               'uranus_occ_u14_opmt_106cm',
               'uranus_occ_u5_lco_250cm',
-              'uranus_occ_u12_eso_104cm',
-              'uranus_occ_support',
               'uranus_occ_u13_sso_390cm',
               'uranus_occ_u2_teide_155cm',
               'uranus_occ_u9_lco_250cm',
               'uranus_occ_u103_palomar_508cm',
               'uranus_occ_u23_mcdonald_270cm',
               'uranus_occ_u25_ctio_400cm',
               'uranus_occ_u83_irtf_320cm',
@@ -435,15 +434,14 @@
               'uranus_occ_u0201_palomar_508cm',
               'uranus_occ_u1052_irtf_320cm',
               'uranus_occ_u36_ctio_400cm',
               'uranus_occ_u134_saao_188cm',
               'uranus_occ_u144_caha_123cm',
               'uranus_occ_u17b_saao_188cm',
               'uranus_occ_u137_hst_fos',
-              'bundleset_index.csv',
               'uranus_occ_u14_ctio_150cm',
               'uranus_occ_u144_saao_188cm',
               'uranus_occ_u102b_irtf_320cm',
               'uranus_occ_u84_irtf_320cm']),
             ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/bundle.xml',
              []),
             ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml',
@@ -467,16 +465,15 @@
             # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/13089xxxxx/1308947235.xml',
             #  []),
         ]
     )
     def test_childnames(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.childnames
-        for child in res:
-            assert child in expected
+        assert res.sort() == expected.sort()
 
     @pytest.mark.parametrize(
     'input_path,expected',
         [
             # ('cassini_iss/cassini_iss_cruise',
             #  f'{PDS4_BUNDLES_DIR}/cassini_iss/cassini_iss_cruise'),
             # ('cassini_iss_cruise',
```

### Comparing `rms_pdsfile-0.0.6/pdsfile/pdscache.py` & `rms_pdsfile-0.0.7/pdsfile/pdscache.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pdsfile.py` & `rms_pdsfile-0.0.7/pdsfile/pdsfile.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/pdsviewable.py` & `rms_pdsfile-0.0.7/pdsfile/pdsviewable.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pdsfile/preload_and_cache.py` & `rms_pdsfile-0.0.7/pdsfile/preload_and_cache.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/pyproject.toml` & `rms_pdsfile-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/rms_pdsfile.egg-info/PKG-INFO` & `rms_pdsfile-0.0.7/rms_pdsfile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rms-pdsfile
-Version: 0.0.6
+Version: 0.0.7
 Summary: pdsfile
 Maintainer-email: "Robert S. French" <rfrench@seti.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/SETI/rms-pdsfile
 Project-URL: Repository, https://github.com/SETI/rms-pdsfile
 Project-URL: Source, https://github.com/SETI/rms-pdsfile
 Project-URL: Issues, https://github.com/SETI/rms-pdsfile/issues
```

### Comparing `rms_pdsfile-0.0.6/rms_pdsfile.egg-info/SOURCES.txt` & `rms_pdsfile-0.0.7/rms_pdsfile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/run_tests_coverage.sh` & `rms_pdsfile-0.0.7/run_tests_coverage.sh`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/scripts/automated_tests/pdsfile_main_test.sh` & `rms_pdsfile-0.0.7/scripts/automated_tests/pdsfile_main_test.sh`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/validation/pdsarchives.py` & `rms_pdsfile-0.0.7/validation/pdsarchives.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/validation/pdschecksums.py` & `rms_pdsfile-0.0.7/validation/pdschecksums.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/validation/pdsdata-sync.sh` & `rms_pdsfile-0.0.7/validation/pdsdata-sync.sh`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/validation/pdsdependency.py` & `rms_pdsfile-0.0.7/validation/pdsdependency.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/validation/pdsindexshelf.py` & `rms_pdsfile-0.0.7/validation/pdsindexshelf.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/validation/pdsinfoshelf.py` & `rms_pdsfile-0.0.7/validation/pdsinfoshelf.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/validation/pdslinkshelf.py` & `rms_pdsfile-0.0.7/validation/pdslinkshelf.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/validation/re-validate.py` & `rms_pdsfile-0.0.7/validation/re-validate.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.6/validation/shelf-consistency-check.py` & `rms_pdsfile-0.0.7/validation/shelf-consistency-check.py`

 * *Files identical despite different names*

