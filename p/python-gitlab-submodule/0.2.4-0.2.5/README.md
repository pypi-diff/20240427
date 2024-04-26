# Comparing `tmp/python-gitlab-submodule-0.2.4.tar.gz` & `tmp/python_gitlab_submodule-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-gitlab-submodule-0.2.4.tar", last modified: Mon Sep 11 05:23:12 2023, max compression
+gzip compressed data, was "python_gitlab_submodule-0.2.5.tar", last modified: Fri Apr 26 22:32:14 2024, max compression
```

## Comparing `python-gitlab-submodule-0.2.4.tar` & `python_gitlab_submodule-0.2.5.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 05:23:12.061669 python-gitlab-submodule-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-09-11 05:22:58.000000 python-gitlab-submodule-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14245 2023-09-11 05:23:12.061669 python-gitlab-submodule-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14072 2023-09-11 05:22:58.000000 python-gitlab-submodule-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 05:23:12.053669 python-gitlab-submodule-0.2.4/gitlab_submodule/
--rw-r--r--   0 runner    (1001) docker     (127)      786 2023-09-11 05:22:58.000000 python-gitlab-submodule-0.2.4/gitlab_submodule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-11 05:22:58.000000 python-gitlab-submodule-0.2.4/gitlab_submodule/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2023-09-11 05:22:58.000000 python-gitlab-submodule-0.2.4/gitlab_submodule/gitlab_submodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2023-09-11 05:22:58.000000 python-gitlab-submodule-0.2.4/gitlab_submodule/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2023-09-11 05:22:58.000000 python-gitlab-submodule-0.2.4/gitlab_submodule/read_gitmodules.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-09-11 05:22:58.000000 python-gitlab-submodule-0.2.4/gitlab_submodule/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2023-09-11 05:22:58.000000 python-gitlab-submodule-0.2.4/gitlab_submodule/submodule_commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2023-09-11 05:22:58.000000 python-gitlab-submodule-0.2.4/gitlab_submodule/submodule_to_project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 05:23:12.057669 python-gitlab-submodule-0.2.4/python_gitlab_submodule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14245 2023-09-11 05:23:11.000000 python-gitlab-submodule-0.2.4/python_gitlab_submodule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      710 2023-09-11 05:23:12.000000 python-gitlab-submodule-0.2.4/python_gitlab_submodule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-11 05:23:11.000000 python-gitlab-submodule-0.2.4/python_gitlab_submodule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-09-11 05:23:11.000000 python-gitlab-submodule-0.2.4/python_gitlab_submodule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-09-11 05:23:11.000000 python-gitlab-submodule-0.2.4/python_gitlab_submodule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-11 05:23:12.061669 python-gitlab-submodule-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      953 2023-09-11 05:22:58.000000 python-gitlab-submodule-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 05:23:12.057669 python-gitlab-submodule-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2023-09-11 05:22:58.000000 python-gitlab-submodule-0.2.4/tests/test_gitlab_submodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2023-09-11 05:22:58.000000 python-gitlab-submodule-0.2.4/tests/test_gitmodules_to_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2023-09-11 05:22:58.000000 python-gitlab-submodule-0.2.4/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2023-09-11 05:22:58.000000 python-gitlab-submodule-0.2.4/tests/test_read_gitmodules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-09-11 05:22:58.000000 python-gitlab-submodule-0.2.4/tests/test_string_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2023-09-11 05:22:58.000000 python-gitlab-submodule-0.2.4/tests/test_submodule_commit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:32:14.011055 python_gitlab_submodule-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 22:32:05.000000 python_gitlab_submodule-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-04-26 22:32:14.011055 python_gitlab_submodule-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14072 2024-04-26 22:32:05.000000 python_gitlab_submodule-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:32:14.011055 python_gitlab_submodule-0.2.5/gitlab_submodule/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-26 22:32:05.000000 python_gitlab_submodule-0.2.5/gitlab_submodule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 22:32:05.000000 python_gitlab_submodule-0.2.5/gitlab_submodule/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-26 22:32:05.000000 python_gitlab_submodule-0.2.5/gitlab_submodule/gitlab_submodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-26 22:32:05.000000 python_gitlab_submodule-0.2.5/gitlab_submodule/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-26 22:32:05.000000 python_gitlab_submodule-0.2.5/gitlab_submodule/read_gitmodules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-26 22:32:05.000000 python_gitlab_submodule-0.2.5/gitlab_submodule/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-26 22:32:05.000000 python_gitlab_submodule-0.2.5/gitlab_submodule/submodule_commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-26 22:32:05.000000 python_gitlab_submodule-0.2.5/gitlab_submodule/submodule_to_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:32:14.011055 python_gitlab_submodule-0.2.5/python_gitlab_submodule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-04-26 22:32:13.000000 python_gitlab_submodule-0.2.5/python_gitlab_submodule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-26 22:32:13.000000 python_gitlab_submodule-0.2.5/python_gitlab_submodule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 22:32:13.000000 python_gitlab_submodule-0.2.5/python_gitlab_submodule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-26 22:32:13.000000 python_gitlab_submodule-0.2.5/python_gitlab_submodule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-26 22:32:13.000000 python_gitlab_submodule-0.2.5/python_gitlab_submodule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 22:32:14.011055 python_gitlab_submodule-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-26 22:32:05.000000 python_gitlab_submodule-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:32:14.011055 python_gitlab_submodule-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-04-26 22:32:05.000000 python_gitlab_submodule-0.2.5/tests/test_gitlab_submodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-26 22:32:05.000000 python_gitlab_submodule-0.2.5/tests/test_gitmodules_to_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-26 22:32:05.000000 python_gitlab_submodule-0.2.5/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-26 22:32:05.000000 python_gitlab_submodule-0.2.5/tests/test_read_gitmodules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-26 22:32:05.000000 python_gitlab_submodule-0.2.5/tests/test_string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-26 22:32:05.000000 python_gitlab_submodule-0.2.5/tests/test_submodule_commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-26 22:32:05.000000 python_gitlab_submodule-0.2.5/tests/test_submodule_to_project.py
```

### Comparing `python-gitlab-submodule-0.2.4/LICENSE` & `python_gitlab_submodule-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-gitlab-submodule-0.2.4/PKG-INFO` & `python_gitlab_submodule-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: python-gitlab-submodule
-Version: 0.2.4
+Version: 0.2.5
 Summary: python-gitlab-submodule : List project submodules and get the commits they point to with python-gitlab.
 Home-page: https://github.com/ValentinFrancois/python-gitlab-submodule
 Author: Valentin François
 Maintainer: Valentin François
 License: Apache License 2.0
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-gitlab>=3.0.0
 Requires-Dist: giturlparse>=0.10.0
 
-# python-gitlab-submodule <sub><sup>v0.2.4</sup></sub>
+# python-gitlab-submodule <sub><sup>v0.2.5</sup></sub>
 
 List project submodules and get the commits they point to with python-gitlab.
 
 
 The [Gitlab REST API V4](https://docs.gitlab.com/ee/api/api_resources.html) 
 doesn't implement anything for submodule inspection yet. The only thing we can 
 currently do is [updating a submodule to a new commit id](
```

### Comparing `python-gitlab-submodule-0.2.4/README.md` & `python_gitlab_submodule-0.2.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# python-gitlab-submodule <sub><sup>v0.2.4</sup></sub>
+# python-gitlab-submodule <sub><sup>v0.2.5</sup></sub>
 
 List project submodules and get the commits they point to with python-gitlab.
 
 
 The [Gitlab REST API V4](https://docs.gitlab.com/ee/api/api_resources.html) 
 doesn't implement anything for submodule inspection yet. The only thing we can 
 currently do is [updating a submodule to a new commit id](
```

### Comparing `python-gitlab-submodule-0.2.4/gitlab_submodule/__init__.py` & `python_gitlab_submodule-0.2.5/gitlab_submodule/__init__.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-submodule-0.2.4/gitlab_submodule/gitlab_submodule.py` & `python_gitlab_submodule-0.2.5/gitlab_submodule/gitlab_submodule.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-submodule-0.2.4/gitlab_submodule/objects.py` & `python_gitlab_submodule-0.2.5/gitlab_submodule/objects.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-submodule-0.2.4/gitlab_submodule/read_gitmodules.py` & `python_gitlab_submodule-0.2.5/gitlab_submodule/read_gitmodules.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-submodule-0.2.4/gitlab_submodule/submodule_commit.py` & `python_gitlab_submodule-0.2.5/gitlab_submodule/submodule_commit.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-submodule-0.2.4/gitlab_submodule/submodule_to_project.py` & `python_gitlab_submodule-0.2.5/gitlab_submodule/submodule_to_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+from typing import List, Optional, Union
+
 import logging
+import re
 from posixpath import join, normpath
-from typing import Optional
 
 from gitlab.exceptions import GitlabGetError
 from gitlab.v4.objects import Project, ProjectManager
 from giturlparse import GitUrlParsed, parse
 
 from gitlab_submodule.objects import Submodule
 from gitlab_submodule.string_utils import lstrip, rstrip
 
 logger = logging.getLogger(__name__)
 
 
 def submodule_to_project(
         submodule: Submodule,
         project_manager: ProjectManager,
-        self_managed_gitlab_host: Optional[str] = None) -> Optional[Project]:
+        self_managed_gitlab_host: Optional[Union[str, List[str]]] = None
+) -> Optional[Project]:
     submodule_project_path_with_namespace = \
         _submodule_url_to_path_with_namespace(submodule.url,
                                               submodule.parent_project,
                                               self_managed_gitlab_host)
     if not submodule_project_path_with_namespace:
         return None
     try:
@@ -33,15 +36,16 @@
             'the repo was deleted.'.format(submodule.url, submodule.path))
     return submodule_project
 
 
 def _submodule_url_to_path_with_namespace(
         url: str,
         parent_project: Project,
-        self_managed_gitlab_host: Optional[str] = None) -> Optional[str]:
+        self_managed_gitlab_host: Optional[Union[str, List[str]]] = None
+) -> Optional[str]:
     """Returns a path pointing to a Gitlab project, or None if the submodule
     is hosted elsewhere
     """
     # check if the submodule url is a relative path to the project path
     if url.startswith('./') or url.startswith('../'):
         # we build the path of the submodule project using the path of
         # the current project
@@ -55,21 +59,25 @@
         logger.warning(f'submodule git url does not seem to be valid: {url}')
         return None
 
     # even if the parent project is hosted on a self-managed gitlab host,
     # it can still use submodules hosted on gitlab.com
     gitlab_hosts = ['gitlab']
     if self_managed_gitlab_host:
-        gitlab_hosts.append(self_managed_gitlab_host)
+        if isinstance(self_managed_gitlab_host, str):
+            gitlab_hosts.append(self_managed_gitlab_host)
+        else:
+            gitlab_hosts.extend(self_managed_gitlab_host)
 
     # giturlparse.GitUrlParsed.platform is too permissive and will be set to
     # 'gitlab' for some non-gitlab urls, for instance:
     # https://opensource.ncsa.illinois.edu/bitbucket/scm/u3d/3dutilities.git
-    if (parsed.platform != 'gitlab'
-            or all([host not in parsed.host for host in gitlab_hosts])):
+    if (parsed.platform not in ('gitlab', 'base')
+            or not any([re.match(fr'^{host}(\.\w+)?$', parsed.host)
+                        for host in gitlab_hosts])):
         logger.warning(f'submodule git url is not hosted on gitlab: {url}')
         return None
 
     # Format to python-gitlab path_with_namespace:
     # rewrite to https format then split by host and keep & cut the right part.
     # I find it more robust than trying to rebuild the path from the different
     # attributes of giturlparse.GitUrlParsed objects
```

### Comparing `python-gitlab-submodule-0.2.4/python_gitlab_submodule.egg-info/PKG-INFO` & `python_gitlab_submodule-0.2.5/python_gitlab_submodule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: python-gitlab-submodule
-Version: 0.2.4
+Version: 0.2.5
 Summary: python-gitlab-submodule : List project submodules and get the commits they point to with python-gitlab.
 Home-page: https://github.com/ValentinFrancois/python-gitlab-submodule
 Author: Valentin François
 Maintainer: Valentin François
 License: Apache License 2.0
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-gitlab>=3.0.0
 Requires-Dist: giturlparse>=0.10.0
 
-# python-gitlab-submodule <sub><sup>v0.2.4</sup></sub>
+# python-gitlab-submodule <sub><sup>v0.2.5</sup></sub>
 
 List project submodules and get the commits they point to with python-gitlab.
 
 
 The [Gitlab REST API V4](https://docs.gitlab.com/ee/api/api_resources.html) 
 doesn't implement anything for submodule inspection yet. The only thing we can 
 currently do is [updating a submodule to a new commit id](
```

### Comparing `python-gitlab-submodule-0.2.4/python_gitlab_submodule.egg-info/SOURCES.txt` & `python_gitlab_submodule-0.2.5/python_gitlab_submodule.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 python_gitlab_submodule.egg-info/requires.txt
 python_gitlab_submodule.egg-info/top_level.txt
 tests/test_gitlab_submodule.py
 tests/test_gitmodules_to_project.py
 tests/test_objects.py
 tests/test_read_gitmodules.py
 tests/test_string_utils.py
-tests/test_submodule_commit.py
+tests/test_submodule_commit.py
+tests/test_submodule_to_project.py
```

### Comparing `python-gitlab-submodule-0.2.4/setup.py` & `python_gitlab_submodule-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-submodule-0.2.4/tests/test_gitlab_submodule.py` & `python_gitlab_submodule-0.2.5/tests/test_gitlab_submodule.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-submodule-0.2.4/tests/test_gitmodules_to_project.py` & `python_gitlab_submodule-0.2.5/tests/test_gitmodules_to_project.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-submodule-0.2.4/tests/test_objects.py` & `python_gitlab_submodule-0.2.5/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-submodule-0.2.4/tests/test_read_gitmodules.py` & `python_gitlab_submodule-0.2.5/tests/test_read_gitmodules.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-submodule-0.2.4/tests/test_string_utils.py` & `python_gitlab_submodule-0.2.5/tests/test_string_utils.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-submodule-0.2.4/tests/test_submodule_commit.py` & `python_gitlab_submodule-0.2.5/tests/test_submodule_commit.py`

 * *Files identical despite different names*

