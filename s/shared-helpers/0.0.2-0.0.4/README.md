# Comparing `tmp/shared_helpers-0.0.2.tar.gz` & `tmp/shared_helpers-0.0.4.tar.gz`

## Comparing `shared_helpers-0.0.2.tar` & `shared_helpers-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,21 @@
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 shared_helpers-0.0.2/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.2/README.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 shared_helpers-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 shared_helpers-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/setup.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/__init__.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/functions.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/main.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/variables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/lm/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/lm/sbbid/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/lm/sbbid/sbbid_helper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/yandex/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/yandex/iam/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/yandex/organization/__init__.py
+-rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/yandex/organization/organization_helper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/yandex/tracker/__init__.py
+-rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/yandex/tracker/tracker_helper.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/README.md
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/PKG-INFO
```

### Comparing `shared_helpers-0.0.2/.gitignore` & `shared_helpers-0.0.4/.gitignore`

 * *Files identical despite different names*

