# Comparing `tmp/shared_helpers-0.0.4.tar.gz` & `tmp/shared_helpers-0.0.5.tar.gz`

## Comparing `shared_helpers-0.0.4.tar` & `shared_helpers-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/requirements.txt
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/setup.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/__init__.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/functions.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/main.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/variables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/lm/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/lm/sbbid/__init__.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/lm/sbbid/sbbid_helper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/yandex/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/yandex/iam/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/yandex/organization/__init__.py
--rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/yandex/organization/organization_helper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/yandex/tracker/__init__.py
--rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/src/shared_helpers/yandex/tracker/tracker_helper.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/README.md
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 shared_helpers-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/setup.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/src/shared_helpers/__init__.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/src/shared_helpers/functions.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/src/shared_helpers/main.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/src/shared_helpers/variables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/src/shared_helpers/lm/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/src/shared_helpers/lm/sbbid/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/src/shared_helpers/lm/sbbid/sbbid_helper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/src/shared_helpers/yandex/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/src/shared_helpers/yandex/iam/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/src/shared_helpers/yandex/organization/__init__.py
+-rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/src/shared_helpers/yandex/organization/organization_helper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/src/shared_helpers/yandex/tracker/__init__.py
+-rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/src/shared_helpers/yandex/tracker/tracker_helper.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/README.md
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 shared_helpers-0.0.5/PKG-INFO
```

### Comparing `shared_helpers-0.0.4/src/shared_helpers/functions.py` & `shared_helpers-0.0.5/src/shared_helpers/functions.py`

 * *Files identical despite different names*

### Comparing `shared_helpers-0.0.4/src/shared_helpers/main.py` & `shared_helpers-0.0.5/src/shared_helpers/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,18 +10,21 @@
     """Fetch a valid IAM token or return None."""
     token = None
     if (
         variables.SA01_IAM_TOKEN and
         variables.SA01_IAM_TOKEN_EXPIRY and
         int(variables.SA01_IAM_TOKEN_EXPIRY) <300
     ):
+        print('using token from env')
         token = variables.SA01_IAM_TOKEN
     elif (variables.SA01_API_KEY and variables.SA01_CF_ENDPOINT_URL):
+        print('using token from endpoint')
         token = token_helper.get_iam_token_from_endpoint(api_key=variables.SA01_API_KEY, endpoint_url=variables.SA01_CF_ENDPOINT_URL)
     elif token_helper.file_exists(json_file_path=variables.SA01_JSON_FILE_PATH):
+        print('using token from file')
         token = token_helper.get_iam_token_from_file(json_file_path=variables.SA01_JSON_FILE_PATH)
     return token
 
 if token := fetch_current_iam_token():
     cloud_client = CloudHelper(token)
     tracker_client = TrackerHelper(token)
 sbbid_client = SbbIdHelper(x_api_key=variables.SBBID_X_API_KEY, environment = variables.SBBID_ENVIRONMENT)
```

### Comparing `shared_helpers-0.0.4/src/shared_helpers/lm/sbbid/sbbid_helper.py` & `shared_helpers-0.0.5/src/shared_helpers/lm/sbbid/sbbid_helper.py`

 * *Files identical despite different names*

### Comparing `shared_helpers-0.0.4/src/shared_helpers/yandex/organization/organization_helper.py` & `shared_helpers-0.0.5/src/shared_helpers/yandex/organization/organization_helper.py`

 * *Files identical despite different names*

### Comparing `shared_helpers-0.0.4/src/shared_helpers/yandex/tracker/tracker_helper.py` & `shared_helpers-0.0.5/src/shared_helpers/yandex/tracker/tracker_helper.py`

 * *Files identical despite different names*

### Comparing `shared_helpers-0.0.4/.gitignore` & `shared_helpers-0.0.5/.gitignore`

 * *Files identical despite different names*

