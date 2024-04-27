# Comparing `tmp/data_prep_lab_kfp-0.1.5.tar.gz` & `tmp/data_prep_lab_kfp-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_prep_lab_kfp-0.1.5.tar", last modified: Fri Apr 26 06:50:20 2024, max compression
+gzip compressed data, was "data_prep_lab_kfp-0.1.6.tar", last modified: Sat Apr 27 18:12:39 2024, max compression
```

## Comparing `data_prep_lab_kfp-0.1.5.tar` & `data_prep_lab_kfp-0.1.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:50:20.153985 data_prep_lab_kfp-0.1.5/
--rw-r--r--   0 boris      (501) staff       (20)     2466 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/Makefile
--rw-r--r--   0 boris      (501) staff       (20)     2695 2024-04-26 06:50:20.153047 data_prep_lab_kfp-0.1.5/PKG-INFO
--rw-r--r--   0 boris      (501) staff       (20)     1889 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/README.md
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:50:20.131223 data_prep_lab_kfp-0.1.5/doc/
--rw-r--r--   0 boris      (501) staff       (20)      452 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/doc/kfp_support_library.md
--rw-r--r--   0 boris      (501) staff       (20)     1210 2024-04-26 06:49:00.000000 data_prep_lab_kfp-0.1.5/pyproject.toml
--rw-r--r--   0 boris      (501) staff       (20)       38 2024-04-26 06:50:20.154122 data_prep_lab_kfp-0.1.5/setup.cfg
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:50:20.128501 data_prep_lab_kfp-0.1.5/src/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:50:20.150835 data_prep_lab_kfp-0.1.5/src/data_prep_lab_kfp.egg-info/
--rw-r--r--   0 boris      (501) staff       (20)     2695 2024-04-26 06:50:19.000000 data_prep_lab_kfp-0.1.5/src/data_prep_lab_kfp.egg-info/PKG-INFO
--rw-r--r--   0 boris      (501) staff       (20)     1142 2024-04-26 06:50:20.000000 data_prep_lab_kfp-0.1.5/src/data_prep_lab_kfp.egg-info/SOURCES.txt
--rw-r--r--   0 boris      (501) staff       (20)        1 2024-04-26 06:50:19.000000 data_prep_lab_kfp-0.1.5/src/data_prep_lab_kfp.egg-info/dependency_links.txt
--rw-r--r--   0 boris      (501) staff       (20)      164 2024-04-26 06:50:19.000000 data_prep_lab_kfp-0.1.5/src/data_prep_lab_kfp.egg-info/requires.txt
--rw-r--r--   0 boris      (501) staff       (20)       12 2024-04-26 06:50:19.000000 data_prep_lab_kfp-0.1.5/src/data_prep_lab_kfp.egg-info/top_level.txt
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:50:20.129171 data_prep_lab_kfp-0.1.5/src/kfp_support/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:50:20.135510 data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/
--rw-r--r--   0 boris      (501) staff       (20)      238 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/README.md
--rw-r--r--   0 boris      (501) staff       (20)       67 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)    26996 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/kuberay_apis.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:50:20.142012 data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/params/
--rw-r--r--   0 boris      (501) staff       (20)     1259 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/params/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)    11445 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/params/cluster.py
--rw-r--r--   0 boris      (501) staff       (20)     5390 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/params/environmentvariables.py
--rw-r--r--   0 boris      (501) staff       (20)     7528 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/params/headnode.py
--rw-r--r--   0 boris      (501) staff       (20)     6367 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/params/jobsubmission.py
--rw-r--r--   0 boris      (501) staff       (20)     7491 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/params/templates.py
--rw-r--r--   0 boris      (501) staff       (20)    14921 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/params/volumes.py
--rw-r--r--   0 boris      (501) staff       (20)     7884 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/params/workernode.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:50:20.142947 data_prep_lab_kfp-0.1.5/src/kfp_support/workflow_support/
--rw-r--r--   0 boris      (501) staff       (20)     2698 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/src/kfp_support/workflow_support/README.md
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:50:20.144581 data_prep_lab_kfp-0.1.5/src/kfp_support/workflow_support/utils/
--rw-r--r--   0 boris      (501) staff       (20)      192 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/src/kfp_support/workflow_support/utils/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)    27875 2024-04-24 20:35:43.000000 data_prep_lab_kfp-0.1.5/src/kfp_support/workflow_support/utils/workflow_utils.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-26 06:50:20.149662 data_prep_lab_kfp-0.1.5/test/
--rw-r--r--   0 boris      (501) staff       (20)    14416 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/test/api_params_test.py
--rw-r--r--   0 boris      (501) staff       (20)     2319 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/test/configmaps.py
--rw-r--r--   0 boris      (501) staff       (20)     9967 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/test/kuberay_api_test.py
--rw-r--r--   0 boris      (501) staff       (20)     1401 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/test/pipeline_utils_test.py
--rw-r--r--   0 boris      (501) staff       (20)     3154 2024-04-23 18:07:37.000000 data_prep_lab_kfp-0.1.5/test/ray_remote_jobs_test.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:12:39.899076 data_prep_lab_kfp-0.1.6/
+-rw-r--r--   0 boris      (501) staff       (20)     2470 2024-04-27 18:08:10.000000 data_prep_lab_kfp-0.1.6/Makefile
+-rw-r--r--   0 boris      (501) staff       (20)     2695 2024-04-27 18:12:39.898529 data_prep_lab_kfp-0.1.6/PKG-INFO
+-rw-r--r--   0 boris      (501) staff       (20)     1889 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/README.md
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:12:39.880089 data_prep_lab_kfp-0.1.6/doc/
+-rw-r--r--   0 boris      (501) staff       (20)      452 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/doc/kfp_support_library.md
+-rw-r--r--   0 boris      (501) staff       (20)     1210 2024-04-27 18:11:08.000000 data_prep_lab_kfp-0.1.6/pyproject.toml
+-rw-r--r--   0 boris      (501) staff       (20)       38 2024-04-27 18:12:39.899196 data_prep_lab_kfp-0.1.6/setup.cfg
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:12:39.876739 data_prep_lab_kfp-0.1.6/src/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:12:39.896630 data_prep_lab_kfp-0.1.6/src/data_prep_lab_kfp.egg-info/
+-rw-r--r--   0 boris      (501) staff       (20)     2695 2024-04-27 18:12:39.000000 data_prep_lab_kfp-0.1.6/src/data_prep_lab_kfp.egg-info/PKG-INFO
+-rw-r--r--   0 boris      (501) staff       (20)     1142 2024-04-27 18:12:39.000000 data_prep_lab_kfp-0.1.6/src/data_prep_lab_kfp.egg-info/SOURCES.txt
+-rw-r--r--   0 boris      (501) staff       (20)        1 2024-04-27 18:12:39.000000 data_prep_lab_kfp-0.1.6/src/data_prep_lab_kfp.egg-info/dependency_links.txt
+-rw-r--r--   0 boris      (501) staff       (20)      164 2024-04-27 18:12:39.000000 data_prep_lab_kfp-0.1.6/src/data_prep_lab_kfp.egg-info/requires.txt
+-rw-r--r--   0 boris      (501) staff       (20)       12 2024-04-27 18:12:39.000000 data_prep_lab_kfp-0.1.6/src/data_prep_lab_kfp.egg-info/top_level.txt
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:12:39.877678 data_prep_lab_kfp-0.1.6/src/kfp_support/
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:12:39.884377 data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/
+-rw-r--r--   0 boris      (501) staff       (20)      238 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/README.md
+-rw-r--r--   0 boris      (501) staff       (20)       67 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)    26996 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/kuberay_apis.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:12:39.888452 data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/params/
+-rw-r--r--   0 boris      (501) staff       (20)     1259 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/params/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)    11445 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/params/cluster.py
+-rw-r--r--   0 boris      (501) staff       (20)     5390 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/params/environmentvariables.py
+-rw-r--r--   0 boris      (501) staff       (20)     7528 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/params/headnode.py
+-rw-r--r--   0 boris      (501) staff       (20)     6367 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/params/jobsubmission.py
+-rw-r--r--   0 boris      (501) staff       (20)     7491 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/params/templates.py
+-rw-r--r--   0 boris      (501) staff       (20)    14921 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/params/volumes.py
+-rw-r--r--   0 boris      (501) staff       (20)     7884 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/params/workernode.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:12:39.888929 data_prep_lab_kfp-0.1.6/src/kfp_support/workflow_support/
+-rw-r--r--   0 boris      (501) staff       (20)     2698 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/src/kfp_support/workflow_support/README.md
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:12:39.890340 data_prep_lab_kfp-0.1.6/src/kfp_support/workflow_support/utils/
+-rw-r--r--   0 boris      (501) staff       (20)      192 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/src/kfp_support/workflow_support/utils/__init__.py
+-rw-r--r--   0 boris      (501) staff       (20)    28030 2024-04-25 20:21:15.000000 data_prep_lab_kfp-0.1.6/src/kfp_support/workflow_support/utils/workflow_utils.py
+drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-04-27 18:12:39.895526 data_prep_lab_kfp-0.1.6/test/
+-rw-r--r--   0 boris      (501) staff       (20)    14416 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/test/api_params_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     2319 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/test/configmaps.py
+-rw-r--r--   0 boris      (501) staff       (20)     9967 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/test/kuberay_api_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     1401 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/test/pipeline_utils_test.py
+-rw-r--r--   0 boris      (501) staff       (20)     3154 2024-04-25 06:38:08.000000 data_prep_lab_kfp-0.1.6/test/ray_remote_jobs_test.py
```

### Comparing `data_prep_lab_kfp-0.1.5/Makefile` & `data_prep_lab_kfp-0.1.6/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 	$(PYTHON) -m venv venv
 	. ${VENV_ACTIVATE};     \
         pip install -r ../kfp_ray_components/requirements.txt ;\
 	pip install -e .;		\
 	pip install ray==${RAY} \
 	pip install pytest pytest-cov 
 
-test:: 	
+test:: 	venv
 	@# Help: Use the already-built virtual environment to run pytest on the test directory.
 	. ${VENV_ACTIVATE}; export PYTHONPATH=../src; cd test;  $(PYTEST) api_params_test.py;
-	. ${VENV_ACTIVATE}; export PYTHONPATH=../src; cd test;  $(PYTEST) kuberay_api_test.py;
 ifeq ($(DEPLOY_KUBEFLOW),1)
+	. ${VENV_ACTIVATE}; export PYTHONPATH=../src; cd test;  $(PYTEST) kuberay_api_test.py;
 	. ${VENV_ACTIVATE}; export PYTHONPATH=../src; cd test;  $(PYTEST) ray_remote_jobs_test.py;
 	. ${VENV_ACTIVATE}; export PYTHONPATH=../src; cd test;  $(PYTEST) pipeline_utils_test.py;
 endif
```

### Comparing `data_prep_lab_kfp-0.1.5/PKG-INFO` & `data_prep_lab_kfp-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: data_prep_lab_kfp
-Version: 0.1.5
+Version: 0.1.6
 Summary: Data Preparation Laboratory Library. KFP support
 Author-email: Boris Lublinsky <blublinsky@ibm.com>, Alexey Roytman <roytman@il.ibm.com>, Mohammad Nassar <Mohammad.Nassar@ibm.com>, Revital Eres <eres@il.ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kfp==1.8.22
 Requires-Dist: requests
-Requires-Dist: data-prep-lab==0.1.4
+Requires-Dist: data-prep-lab==0.1.5
 Provides-Extra: dev
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pytest>=7.3.2; extra == "dev"
 Requires-Dist: pytest-dotenv>=0.5.2; extra == "dev"
 Requires-Dist: pytest-env>=1.0.0; extra == "dev"
 Requires-Dist: pre-commit>=3.3.2; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
```

### Comparing `data_prep_lab_kfp-0.1.5/README.md` & `data_prep_lab_kfp-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.5/pyproject.toml` & `data_prep_lab_kfp-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [project]
 name = "data_prep_lab_kfp"
-version = "0.1.5"
+version = "0.1.6"
 requires-python = ">=3.10"
 description = "Data Preparation Laboratory Library. KFP support"
 license = {text = "Apache-2.0"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     { name = "Boris Lublinsky", email = "blublinsky@ibm.com" },
     { name = "Alexey Roytman", email = "roytman@il.ibm.com" },
     { name = "Mohammad Nassar", email = "Mohammad.Nassar@ibm.com" },
     { name = "Revital Eres", email = "eres@il.ibm.com" },
 ]
 dependencies = [
     "kfp==1.8.22",
     "requests",
-    "data-prep-lab==0.1.4",
+    "data-prep-lab==0.1.5",
 ]
 
 [build-system]
 requires = ["setuptools>=68.0.0", "wheel", "setuptools_scm[toml]>=7.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project.optional-dependencies]
```

### Comparing `data_prep_lab_kfp-0.1.5/src/data_prep_lab_kfp.egg-info/PKG-INFO` & `data_prep_lab_kfp-0.1.6/src/data_prep_lab_kfp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: data_prep_lab_kfp
-Version: 0.1.5
+Version: 0.1.6
 Summary: Data Preparation Laboratory Library. KFP support
 Author-email: Boris Lublinsky <blublinsky@ibm.com>, Alexey Roytman <roytman@il.ibm.com>, Mohammad Nassar <Mohammad.Nassar@ibm.com>, Revital Eres <eres@il.ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kfp==1.8.22
 Requires-Dist: requests
-Requires-Dist: data-prep-lab==0.1.4
+Requires-Dist: data-prep-lab==0.1.5
 Provides-Extra: dev
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pytest>=7.3.2; extra == "dev"
 Requires-Dist: pytest-dotenv>=0.5.2; extra == "dev"
 Requires-Dist: pytest-env>=1.0.0; extra == "dev"
 Requires-Dist: pre-commit>=3.3.2; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
```

### Comparing `data_prep_lab_kfp-0.1.5/src/data_prep_lab_kfp.egg-info/SOURCES.txt` & `data_prep_lab_kfp-0.1.6/src/data_prep_lab_kfp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/kuberay_apis.py` & `data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/kuberay_apis.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/params/__init__.py` & `data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/params/__init__.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/params/cluster.py` & `data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/params/cluster.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/params/environmentvariables.py` & `data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/params/environmentvariables.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/params/headnode.py` & `data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/params/headnode.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/params/jobsubmission.py` & `data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/params/jobsubmission.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/params/templates.py` & `data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/params/templates.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/params/volumes.py` & `data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/params/volumes.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.5/src/kfp_support/api_server_client/params/workernode.py` & `data_prep_lab_kfp-0.1.6/src/kfp_support/api_server_client/params/workernode.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.5/src/kfp_support/workflow_support/README.md` & `data_prep_lab_kfp-0.1.6/src/kfp_support/workflow_support/README.md`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.5/src/kfp_support/workflow_support/utils/workflow_utils.py` & `data_prep_lab_kfp-0.1.6/src/kfp_support/workflow_support/utils/workflow_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 class KFPUtils:
     """
     Helper utilities for KFP implementations
     """
 
     @staticmethod
     def credentials(
-        access_key: str = "S3_KEY", secret_key: str = "S3_SECRET", endpoint: str = "ENDPOINT"
+            access_key: str = "S3_KEY", secret_key: str = "S3_SECRET", endpoint: str = "ENDPOINT"
     ) -> tuple[str, str, str]:
         """
         Get credentials from the environment
         :param access_key: environment variable for access key
         :param secret_key: environment variable for secret key
         :param endpoint: environment variable for S3 endpoint
         :return:
@@ -140,18 +140,18 @@
         """
         Initialization
         :param host: host to connect to
         """
         self.kfp_client = Client(host=host)
 
     def start_pipeline(
-        self,
-        pipeline: models.api_pipeline.ApiPipeline,
-        experiment: models.api_experiment.ApiExperiment,
-        params: Optional[dict[str, Any]],
+            self,
+            pipeline: models.api_pipeline.ApiPipeline,
+            experiment: models.api_experiment.ApiExperiment,
+            params: Optional[dict[str, Any]],
     ) -> str:
         """
         Start a specified pipeline.
         :param pipeline: pipeline definition
         :param experiment: experiment to use
         :param params: pipeline parameters
         :return: the id of the run object
@@ -236,39 +236,39 @@
     """
     class supporting Ray remote jobs
     """
 
     ansi_escape = re.compile(r"\x1B\[[0-?]*[ -/]*[@-~]")
 
     def __init__(
-        self,
-        server_url: str = "http://kuberay-apiserver-service.kuberay.svc.cluster.local:8888",
-        default_image: str = "rayproject/ray:2.9.3-py310",
-        http_retries: int = 5,
-        wait_interval: int = 2,
+            self,
+            server_url: str = "http://kuberay-apiserver-service.kuberay.svc.cluster.local:8888",
+            default_image: str = "rayproject/ray:2.9.3-py310",
+            http_retries: int = 5,
+            wait_interval: int = 2,
     ):
         """
         Initialization
         :param server_url: API server URL. Default value is assuming running inside the cluster
         :param default_image - default Ray image
         :param wait_interval: wait interval
         :param http_retries: http retries
         """
         self.api_server_client = KubeRayAPIs(
             server_url=server_url, http_retries=http_retries, wait_interval=wait_interval
         )
         self.default_image = default_image
 
     def create_ray_cluster(
-        self,
-        name: str,
-        namespace: str,
-        head_node: dict[str, Any],
-        worker_nodes: list[dict[str, Any]],
-        wait_cluster_ready: int = -1,
+            self,
+            name: str,
+            namespace: str,
+            head_node: dict[str, Any],
+            worker_nodes: list[dict[str, Any]],
+            wait_cluster_ready: int = -1,
     ) -> tuple[int, str]:
         """
         Create Ray cluster
         :param name: name, _ are not allowed in the name
         :param namespace: namespace
         :param head_node: head node specification dictionary including the following:
             mandatory fields:
@@ -451,20 +451,20 @@
             if template.name.startswith(name):
                 status, error = self.api_server_client.delete_compute_template(ns=namespace, name=template.name)
                 if status != 200:
                     return status, error
         return status, error
 
     def submit_job(
-        self,
-        name: str,
-        namespace: str,
-        request: dict[str, Any],
-        runtime_env: str = None,
-        executor: str = "transformer_launcher.py",
+            self,
+            name: str,
+            namespace: str,
+            request: dict[str, Any],
+            runtime_env: str = None,
+            executor: str = "transformer_launcher.py",
     ) -> tuple[int, str, str]:
         """
         Submit job for execution
         :param name: cluster name
         :param namespace: cluster namespace
         :param request: dictionary of the remote job request
         :param runtime_env: runtime environment string
@@ -507,21 +507,21 @@
         """
         l_to_print = log[previous_log_len:]
         if len(l_to_print) > 0:
             l_to_print = RayRemoteJobs.ansi_escape.sub("", l_to_print)
             print(l_to_print)
 
     def follow_execution(
-        self,
-        name: str,
-        namespace: str,
-        submission_id: str,
-        data_access: DataAccess = None,
-        job_ready_timeout: int = 600,
-        print_timeout: int = 120,
+            self,
+            name: str,
+            namespace: str,
+            submission_id: str,
+            data_access: DataAccess = None,
+            job_ready_timeout: int = 600,
+            print_timeout: int = 120,
     ) -> None:
         """
         Follow remote job execution
         :param name: cluster name
         :param namespace: cluster namespace
         :param submission_id: job submission ID
         :param data_access - data access class
@@ -591,18 +591,18 @@
 class ComponentUtils:
     """
     Class containing methods supporting building pipelines
     """
 
     @staticmethod
     def add_settings_to_component(
-        component: dsl.ContainerOp,
-        timeout: int,
-        image_pull_policy: str = "Always",
-        cache_strategy: str = "P0D",
+            component: dsl.ContainerOp,
+            timeout: int,
+            image_pull_policy: str = "Always",
+            cache_strategy: str = "P0D",
     ) -> None:
         """
         Add settings to kfp component
         :param component: kfp component
         :param timeout: timeout to set to the component in seconds
         :param image_pull_policy: pull policy to set to the component
         :param cache_strategy: cache strategy
@@ -612,18 +612,18 @@
         # image pull policy
         component.container.set_image_pull_policy(image_pull_policy)
         # Set the timeout for the task
         component.set_timeout(timeout)
 
     @staticmethod
     def set_s3_env_vars_to_component(
-        component: dsl.ContainerOp,
-        secret: str,
-        env2key: dict[str, str] = {"S3_KEY": "s3-key", "S3_SECRET": "s3-secret", "ENDPOINT": "s3-endpoint"},
-        prefix: str = None,
+            component: dsl.ContainerOp,
+            secret: str,
+            env2key: dict[str, str] = {"S3_KEY": "s3-key", "S3_SECRET": "s3-secret", "ENDPOINT": "s3-endpoint"},
+            prefix: str = None,
     ) -> None:
         """
         Set S3 env variables to KFP component
         :param component: kfp component
         :param secret: secret name with the S3 credentials
         :param env2key: dict with mapping each env variable to a key in the secret
         :param prefix: prefix to add to env name
@@ -638,16 +638,16 @@
                         secret_key_ref=k8s_client.V1SecretKeySelector(name=secret, key=secret_key)
                     ),
                 )
             )
 
     @staticmethod
     def default_compute_execution_params(
-        worker_options: str,  # ray worker configuration
-        actor_options: str,  # cpus per actor
+            worker_options: str,  # ray worker configuration
+            actor_options: str,  # cpus per actor
     ) -> str:
         """
         This is the most simplistic transform execution parameters computation
         :param worker_options: configuration of ray workers
         :param actor_options: actor request requirements
         :return: number of actors
         """
@@ -681,8 +681,8 @@
                 f"Not enough cpu/gpu/memory to run transform, "
                 f"required cpu {a_options.get('num_cpus', .5)}, available {cluster_cpu}, "
                 f"required memory {a_options.get('memory', 1)}, available {cluster_mem}, "
                 f"required cpu {actor_gpu}, available {cluster_gpu}"
             )
             sys.exit(1)
 
-        return str(n_actors)
+        return str(n_actors)
```

### Comparing `data_prep_lab_kfp-0.1.5/test/api_params_test.py` & `data_prep_lab_kfp-0.1.6/test/api_params_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.5/test/configmaps.py` & `data_prep_lab_kfp-0.1.6/test/configmaps.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.5/test/kuberay_api_test.py` & `data_prep_lab_kfp-0.1.6/test/kuberay_api_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.5/test/pipeline_utils_test.py` & `data_prep_lab_kfp-0.1.6/test/pipeline_utils_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_lab_kfp-0.1.5/test/ray_remote_jobs_test.py` & `data_prep_lab_kfp-0.1.6/test/ray_remote_jobs_test.py`

 * *Files identical despite different names*

