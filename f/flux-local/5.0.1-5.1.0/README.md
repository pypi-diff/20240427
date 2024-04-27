# Comparing `tmp/flux_local-5.0.1.tar.gz` & `tmp/flux_local-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux_local-5.0.1.tar", last modified: Sun Apr 21 14:19:07 2024, max compression
+gzip compressed data, was "flux_local-5.1.0.tar", last modified: Sat Apr 27 13:38:37 2024, max compression
```

## Comparing `flux_local-5.0.1.tar` & `flux_local-5.1.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:19:07.105002 flux_local-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-21 14:19:02.000000 flux_local-5.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-04-21 14:19:07.105002 flux_local-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-04-21 14:19:02.000000 flux_local-5.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:19:07.101002 flux_local-5.0.1/flux_local/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/command.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27320 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7353 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     9552 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/kustomize.py
--rw-r--r--   0 runner    (1001) docker     (127)    22281 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:19:07.101002 flux_local-5.0.1/flux_local/tool/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/tool/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/tool/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    16733 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/tool/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/tool/flux_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/tool/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/tool/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/tool/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/tool/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/tool/visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-04-21 14:19:02.000000 flux_local-5.0.1/flux_local/values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:19:07.105002 flux_local-5.0.1/flux_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-04-21 14:19:07.000000 flux_local-5.0.1/flux_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-21 14:19:07.000000 flux_local-5.0.1/flux_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 14:19:07.000000 flux_local-5.0.1/flux_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-21 14:19:07.000000 flux_local-5.0.1/flux_local.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-21 14:19:07.000000 flux_local-5.0.1/flux_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-21 14:19:07.000000 flux_local-5.0.1/flux_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-21 14:19:07.105002 flux_local-5.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-21 14:19:02.000000 flux_local-5.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:19:07.105002 flux_local-5.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-21 14:19:02.000000 flux_local-5.0.1/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-04-21 14:19:02.000000 flux_local-5.0.1/tests/test_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-21 14:19:02.000000 flux_local-5.0.1/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-21 14:19:02.000000 flux_local-5.0.1/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-21 14:19:02.000000 flux_local-5.0.1/tests/test_kustomize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-21 14:19:02.000000 flux_local-5.0.1/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    16462 2024-04-21 14:19:02.000000 flux_local-5.0.1/tests/test_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:19:07.105002 flux_local-5.0.1/tests/tool/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-21 14:19:02.000000 flux_local-5.0.1/tests/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-21 14:19:02.000000 flux_local-5.0.1/tests/tool/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-21 14:19:02.000000 flux_local-5.0.1/tests/tool/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-21 14:19:02.000000 flux_local-5.0.1/tests/tool/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-21 14:19:02.000000 flux_local-5.0.1/tests/tool/test_diff_hr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-21 14:19:02.000000 flux_local-5.0.1/tests/tool/test_diff_ks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-21 14:19:02.000000 flux_local-5.0.1/tests/tool/test_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-21 14:19:02.000000 flux_local-5.0.1/tests/tool/test_get_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-21 14:19:02.000000 flux_local-5.0.1/tests/tool/test_get_hr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-21 14:19:02.000000 flux_local-5.0.1/tests/tool/test_get_ks.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-21 14:19:02.000000 flux_local-5.0.1/tests/tool/test_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:38:37.293294 flux_local-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 13:38:33.000000 flux_local-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-04-27 13:38:37.293294 flux_local-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-04-27 13:38:33.000000 flux_local-5.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:38:37.285294 flux_local-5.1.0/flux_local/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27320 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9552 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22676 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:38:37.289294 flux_local-5.1.0/flux_local/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16733 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/flux_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/tool/visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-04-27 13:38:33.000000 flux_local-5.1.0/flux_local/values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:38:37.293294 flux_local-5.1.0/flux_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-04-27 13:38:37.000000 flux_local-5.1.0/flux_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-27 13:38:37.000000 flux_local-5.1.0/flux_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 13:38:37.000000 flux_local-5.1.0/flux_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-27 13:38:37.000000 flux_local-5.1.0/flux_local.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-27 13:38:37.000000 flux_local-5.1.0/flux_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-27 13:38:37.000000 flux_local-5.1.0/flux_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-27 13:38:37.293294 flux_local-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-27 13:38:33.000000 flux_local-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:38:37.289294 flux_local-5.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/test_kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16462 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/test_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:38:37.293294 flux_local-5.1.0/tests/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_diff_hr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_diff_ks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_get_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_get_hr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_get_ks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-27 13:38:33.000000 flux_local-5.1.0/tests/tool/test_test.py
```

### Comparing `flux_local-5.0.1/LICENSE` & `flux_local-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/PKG-INFO` & `flux_local-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 5.0.1
+Version: 5.1.0
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
```

### Comparing `flux_local-5.0.1/README.md` & `flux_local-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/flux_local/command.py` & `flux_local-5.1.0/flux_local/command.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/flux_local/context.py` & `flux_local-5.1.0/flux_local/context.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/flux_local/exceptions.py` & `flux_local-5.1.0/flux_local/exceptions.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/flux_local/git_repo.py` & `flux_local-5.1.0/flux_local/git_repo.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/flux_local/helm.py` & `flux_local-5.1.0/flux_local/helm.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,33 +45,43 @@
 from .kustomize import Kustomize
 from .manifest import (
     HelmRelease,
     HelmRepository,
     CRD_KIND,
     SECRET_KIND,
     REPO_TYPE_OCI,
+    HELM_REPOSITORY,
+    GIT_REPOSITORY
 )
 from .exceptions import HelmException
 
 __all__ = [
     "Helm",
     "Options",
 ]
 
 _LOGGER = logging.getLogger(__name__)
 
 
 HELM_BIN = "helm"
 
 
-def _chart_name(repo: HelmRepository, release: HelmRelease) -> str:
+def _chart_name(release: HelmRelease, repo: HelmRepository | None) -> str:
     """Return the helm chart name used for the helm template command."""
-    if repo.repo_type == REPO_TYPE_OCI:
-        return f"{repo.url}/{release.chart.name}"
-    return release.chart.chart_name
+    if release.chart.repo_kind == HELM_REPOSITORY:
+        if repo.repo_type == REPO_TYPE_OCI:
+            return f"{repo.url}/{release.chart.name}"
+        return release.chart.chart_name
+    elif release.chart.repo_kind == GIT_REPOSITORY:
+        return release.chart.name
+    raise HelmException(
+        f"Unable to find chart source for chart {release.chart.chart_name} "
+        f"kind {release.chart.repo_kind} for HelmRelease {release.name}"
+    )
+
 
 
 class RepositoryConfig:
     """Generates a helm repository configuration from flux HelmRepository objects."""
 
     def __init__(self, repos: list[HelmRepository]) -> None:
         """Initialize RepositoryConfig."""
@@ -197,25 +207,27 @@
         """
         if options is None:
             options = Options()
         repo = next(
             iter([repo for repo in self._repos if repo.repo_name == release.repo_name]),
             None,
         )
-        if not repo:
+        # We'll attempt to make a chart name for a GitRepository below and it will
+        # be somewhat best effort.
+        if not repo and release.chart.repo_kind == HELM_REPOSITORY:
             raise HelmException(
                 f"Unable to find HelmRepository for {release.chart.chart_name} for "
                 f"HelmRelease {release.name} "
                 f"({len(self._repos)} other HelmRepositories in --path)"
             )
         args: list[str] = [
             HELM_BIN,
             "template",
             release.name,
-            _chart_name(repo, release),
+            _chart_name(release, repo),
             "--namespace",
             release.namespace,
         ]
         args.extend(options.template_args)
         if release.chart.version:
             args.extend(
                 [
```

### Comparing `flux_local-5.0.1/flux_local/image.py` & `flux_local-5.1.0/flux_local/image.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/flux_local/kustomize.py` & `flux_local-5.1.0/flux_local/kustomize.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/flux_local/manifest.py` & `flux_local-5.1.0/flux_local/manifest.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 CLUSTER_POLICY_DOMAIN = "kyverno.io"
 CRD_KIND = "CustomResourceDefinition"
 SECRET_KIND = "Secret"
 CONFIG_MAP_KIND = "ConfigMap"
 DEFAULT_NAMESPACE = "flux-system"
 VALUE_PLACEHOLDER = "!!PLACEHOLDER!!"
 VALUE_B64_PLACEHOLDER = base64.b64encode(VALUE_PLACEHOLDER.encode())
+HELM_REPOSITORY = "HelmRepository"
+GIT_REPOSITORY = "GitRepository"
 
 REPO_TYPE_DEFAULT = "default"
 REPO_TYPE_OCI = "oci"
 
 
 def _check_version(doc: dict[str, Any], version: str) -> None:
     """Assert that the resource has the specified version."""
@@ -89,22 +91,25 @@
 @dataclass
 class HelmChart(BaseManifest):
     """A representation of an instantiation of a chart for a HelmRelease."""
 
     name: str
     """The name of the chart within the HelmRepository."""
 
-    version: Optional[str] = field(metadata={"serialize":"omit"})
+    version: Optional[str] = field(metadata={"serialize": "omit"})
     """The version of the chart."""
 
     repo_name: str
-    """The short name of the HelmRepository."""
+    """The short name of the repository."""
 
     repo_namespace: str
-    """The namespace of the HelmRepository."""
+    """The namespace of the repository."""
+
+    repo_kind: str = HELM_REPOSITORY
+    """The kind of the soruceRef of the repository (e.g. HelmRepository, GitRepository)."""
 
     @classmethod
     def parse_doc(cls, doc: dict[str, Any], default_namespace: str) -> "HelmChart":
         """Parse a HelmChart from a HelmRelease resource object."""
         _check_version(doc, HELM_RELEASE_DOMAIN)
         if not (spec := doc.get("spec")):
             raise InputException(f"Invalid {cls} missing spec: {doc}")
@@ -122,14 +127,15 @@
         if "name" not in source_ref:
             raise InputException(f"Invalid {cls} missing sourceRef fields: {doc}")
         return cls(
             name=chart,
             version=version,
             repo_name=source_ref["name"],
             repo_namespace=source_ref.get("namespace", default_namespace),
+            repo_kind=source_ref.get("kind", HELM_REPOSITORY),
         )
 
     @property
     def repo_full_name(self) -> str:
         """Identifier for the HelmRepository."""
         return f"{self.repo_namespace}-{self.repo_name}"
 
@@ -145,40 +151,45 @@
 
     kind: str
     """The kind of resource."""
 
     name: str
     """The name of the resource."""
 
-    values_key: str = field(metadata=field_options(alias="valuesKey"), default="values.yaml")
+    values_key: str = field(
+        metadata=field_options(alias="valuesKey"), default="values.yaml"
+    )
     """The key in the resource that contains the values."""
 
-    target_path: Optional[str] = field(metadata=field_options(alias="targetPath"), default=None)
+    target_path: Optional[str] = field(
+        metadata=field_options(alias="targetPath"), default=None
+    )
     """The path in the HelmRelease values to store the values."""
 
     optional: bool = False
     """Whether the reference is optional."""
 
+
 @dataclass
 class HelmRelease(BaseManifest):
     """A representation of a Flux HelmRelease."""
 
     name: str
     """The name of the HelmRelease."""
 
     namespace: str
     """The namespace that owns the HelmRelease."""
 
     chart: HelmChart
     """A mapping to a specific helm chart for this HelmRelease."""
 
-    values: Optional[dict[str, Any]] = field(metadata={"serialize":"omit"})
+    values: Optional[dict[str, Any]] = field(metadata={"serialize": "omit"})
     """The values to install in the chart."""
 
-    values_from: Optional[list[ValuesReference]] = field(metadata={"serialize":"omit"})
+    values_from: Optional[list[ValuesReference]] = field(metadata={"serialize": "omit"})
     """A list of values to reference from an ConfigMap or Secret."""
 
     images: list[str] | None = field(default=None)
     """The list of images referenced in the HelmRelease."""
 
     @classmethod
     def parse_doc(cls, doc: dict[str, Any]) -> "HelmRelease":
@@ -190,15 +201,17 @@
             raise InputException(f"Invalid {cls} missing metadata.name: {doc}")
         if not (namespace := metadata.get("namespace")):
             raise InputException(f"Invalid {cls} missing metadata.namespace: {doc}")
         chart = HelmChart.parse_doc(doc, namespace)
         spec = doc["spec"]
         values_from: list[ValuesReference] | None = None
         if values_from_dict := spec.get("valuesFrom"):
-            values_from = [ValuesReference.from_dict(subdoc) for subdoc in values_from_dict]
+            values_from = [
+                ValuesReference.from_dict(subdoc) for subdoc in values_from_dict
+            ]
         return HelmRelease(
             name=name,
             namespace=namespace,
             chart=chart,
             values=spec.get("values"),
             values_from=values_from,
         )
@@ -268,15 +281,15 @@
 
     name: str
     """The name of the kustomization."""
 
     namespace: str | None = None
     """The namespace of the kustomization."""
 
-    doc: dict[str, Any] | None = field(metadata={"serialize":"omit"}, default=None)
+    doc: dict[str, Any] | None = field(metadata={"serialize": "omit"}, default=None)
     """The raw ClusterPolicy document."""
 
     @classmethod
     def parse_doc(cls, doc: dict[str, Any]) -> "ClusterPolicy":
         """Parse a cluster policy object from a kubernetes resource."""
         _check_version(doc, CLUSTER_POLICY_DOMAIN)
         if not (metadata := doc.get("metadata")):
@@ -295,18 +308,20 @@
 
     name: str
     """The name of the kustomization."""
 
     namespace: str | None = None
     """The namespace of the kustomization."""
 
-    data: dict[str, Any] | None = field(metadata={"serialize":"omit"}, default=None)
+    data: dict[str, Any] | None = field(metadata={"serialize": "omit"}, default=None)
     """The data in the ConfigMap."""
 
-    binary_data: dict[str, Any] | None = field(metadata={"serialize":"omit"}, default=None)
+    binary_data: dict[str, Any] | None = field(
+        metadata={"serialize": "omit"}, default=None
+    )
     """The binary data in the ConfigMap."""
 
     @classmethod
     def parse_doc(cls, doc: dict[str, Any]) -> "ConfigMap":
         """Parse a config map object from a kubernetes resource."""
         _check_version(doc, "v1")
         if not (metadata := doc.get("metadata")):
@@ -328,18 +343,20 @@
 
     name: str
     """The name of the kustomization."""
 
     namespace: str | None = None
     """The namespace of the kustomization."""
 
-    data: dict[str, Any] | None = field(metadata={"serialize":"omit"}, default=None)
+    data: dict[str, Any] | None = field(metadata={"serialize": "omit"}, default=None)
     """The data in the Secret."""
 
-    string_data: dict[str, Any] | None = field(metadata={"serialize":"omit"}, default=None)
+    string_data: dict[str, Any] | None = field(
+        metadata={"serialize": "omit"}, default=None
+    )
     """The string data in the Secret."""
 
     @classmethod
     def parse_doc(cls, doc: dict[str, Any]) -> "Secret":
         """Parse a secret object from a kubernetes resource."""
         _check_version(doc, "v1")
         if not (metadata := doc.get("metadata")):
@@ -369,14 +386,15 @@
 
     name: str
     """The name of the resource."""
 
     optional: bool = False
     """Whether the reference is optional."""
 
+
 @dataclass
 class Kustomization(BaseManifest):
     """A Kustomization is a set of declared cluster artifacts.
 
     This represents a flux Kustomization that points to a path that
     contains typical `kustomize` Kustomizations on local disk that
     may be flat or contain overlays.
@@ -402,42 +420,48 @@
 
     config_maps: list[ConfigMap] = field(default_factory=list)
     """The list of config maps referenced in the kustomization."""
 
     secrets: list[Secret] = field(default_factory=list)
     """The list of secrets referenced in the kustomization."""
 
-    source_path: str | None = field(metadata={"serialize":"omit"}, default=None)
+    source_path: str | None = field(metadata={"serialize": "omit"}, default=None)
     """Optional source path for this Kustomization, relative to the build path."""
 
-    source_kind: str | None = field(metadata={"serialize":"omit"}, default=None)
+    source_kind: str | None = field(metadata={"serialize": "omit"}, default=None)
     """The sourceRef kind that provides this Kustomization e.g. GitRepository etc."""
 
-    source_name: str | None = field(metadata={"serialize":"omit"}, default=None)
+    source_name: str | None = field(metadata={"serialize": "omit"}, default=None)
     """The name of the sourceRef that provides this Kustomization."""
 
-    source_namespace: str | None = field(metadata={"serialize":"omit"}, default=None)
+    source_namespace: str | None = field(metadata={"serialize": "omit"}, default=None)
     """The namespace of the sourceRef that provides this Kustomization."""
 
-    target_namespace: str | None = field(metadata={"serialize":"omit"}, default=None)
+    target_namespace: str | None = field(metadata={"serialize": "omit"}, default=None)
     """The namespace to target when performing the operation."""
 
-    contents: dict[str, Any] | None = field(metadata={"serialize":"omit"}, default=None)
+    contents: dict[str, Any] | None = field(
+        metadata={"serialize": "omit"}, default=None
+    )
     """Contents of the raw Kustomization document."""
 
     images: list[str] | None = field(default=None)
     """The list of images referenced in the kustomization."""
 
-    postbuild_substitute: Optional[dict[str, Any]] = field(metadata={"serialize":"omit"}, default=None)
+    postbuild_substitute: Optional[dict[str, Any]] = field(
+        metadata={"serialize": "omit"}, default=None
+    )
     """A map of key/value pairs to substitute into the final YAML manifest, after building."""
 
-    postbuild_substitute_from: Optional[list[SubstituteReference]] = field(metadata={"serialize":"omit"}, default=None)
+    postbuild_substitute_from: Optional[list[SubstituteReference]] = field(
+        metadata={"serialize": "omit"}, default=None
+    )
     """A list of substitutions to reference from an ConfigMap or Secret."""
 
-    depends_on: list[str] | None = field(metadata={"serialize":"omit"}, default=None)
+    depends_on: list[str] | None = field(metadata={"serialize": "omit"}, default=None)
     """A list of namespaced names that this Kustomization depends on."""
 
     @classmethod
     def parse_doc(cls, doc: dict[str, Any]) -> "Kustomization":
         """Parse a partial Kustomization from a kubernetes resource."""
         _check_version(doc, FLUXTOMIZE_DOMAIN)
         if not (metadata := doc.get("metadata")):
@@ -484,38 +508,38 @@
         return f"{self.path}"
 
     @property
     def namespaced_name(self) -> str:
         """Return the namespace and name concatenated as an id."""
         return f"{self.namespace}/{self.name}"
 
-
     def validate_depends_on(self, all_ks: set[str]) -> None:
         """Validate depends_on values are all correct given the list of Kustomizations."""
         depends_on = set(self.depends_on or {})
         if missing := (depends_on - all_ks):
             _LOGGER.warning(
                 "Kustomization %s has dependsOn with invalid names: %s",
                 self.namespaced_name,
                 missing,
             )
             self.depends_on = list(depends_on - missing)
-    
+
     def update_postbuild_substitutions(self, substitutions: dict[str, Any]) -> None:
         """Update the postBuild.substitutions in the extracted values and raw doc contents."""
         if self.postbuild_substitute is None:
             self.postbuild_substitute = {}
         self.postbuild_substitute.update(substitutions)
         if self.contents:
             post_build = self.contents["spec"]["postBuild"]
             if (substitute := post_build.get("substitute")) is None:
                 substitute = {}
                 post_build["substitute"] = substitute
             substitute.update(substitutions)
 
+
 @dataclass
 class Cluster(BaseManifest):
     """A set of nodes that run containerized applications.
 
     Many flux git repos will only have a single flux cluster, though
     a repo may also contain multiple (e.g. dev an prod).
     """
@@ -563,15 +587,14 @@
 class Manifest(BaseManifest):
     """Holds information about cluster and applications contained in a repo."""
 
     clusters: list[Cluster]
     """A list of Clusters represented in the repo."""
 
 
-
 async def read_manifest(manifest_path: Path) -> Manifest:
     """Return the contents of a serialized manifest file.
 
     A manifest file is typically created by `flux-local get cluster -o yaml` or
     similar command.
     """
     async with aiofiles.open(str(manifest_path)) as manifest_file:
```

### Comparing `flux_local-5.0.1/flux_local/tool/build.py` & `flux_local-5.1.0/flux_local/tool/build.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/flux_local/tool/diagnostics.py` & `flux_local-5.1.0/flux_local/tool/diagnostics.py`

 * *Files 21% similar despite different names*

```diff
@@ -43,16 +43,30 @@
     async def run(  # type: ignore[no-untyped-def]
         self,
         **kwargs,  # pylint: disable=unused-argument
     ) -> None:
         """Async Action implementation."""
         path = kwargs.get("path") or "."
 
+        # Parse directories to ignore from `.krmignore`
+        krmignore = pathlib.Path(path) / ".krmignore"
+        ignoredirs = []
+        if krmignore.exists():
+            with krmignore.open() as fd:
+                ignoredirs = [
+                    str(pathlib.Path(line.strip())) for line in fd.readlines()
+                ]
+
         errors = []
         for root, dirs, files in os.walk(str(path)):
+            # Ignore any directories that we should not walk
+            rootpath = str(pathlib.Path(root))
+            if any([rootpath.startswith(i) for i in ignoredirs]):
+                continue
+
             for file in files:
                 if not (file.endswith(".yaml") or file.endswith(".yml")):
                     continue
 
                 full_path = pathlib.Path(root) / file
                 try:
                     doc = list(yaml.safe_load_all(full_path.read_text()))
```

### Comparing `flux_local-5.0.1/flux_local/tool/diff.py` & `flux_local-5.1.0/flux_local/tool/diff.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/flux_local/tool/flux_local.py` & `flux_local-5.1.0/flux_local/tool/flux_local.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/flux_local/tool/format.py` & `flux_local-5.1.0/flux_local/tool/format.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/flux_local/tool/get.py` & `flux_local-5.1.0/flux_local/tool/get.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/flux_local/tool/selector.py` & `flux_local-5.1.0/flux_local/tool/selector.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/flux_local/tool/test.py` & `flux_local-5.1.0/flux_local/tool/test.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/flux_local/tool/visitor.py` & `flux_local-5.1.0/flux_local/tool/visitor.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/flux_local/values.py` & `flux_local-5.1.0/flux_local/values.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/flux_local.egg-info/PKG-INFO` & `flux_local-5.1.0/flux_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 5.0.1
+Version: 5.1.0
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
```

### Comparing `flux_local-5.0.1/flux_local.egg-info/SOURCES.txt` & `flux_local-5.1.0/flux_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/setup.cfg` & `flux_local-5.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flux-local
-version = 5.0.1
+version = 5.1.0
 description = flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 long_description = file: README.md
 long_description_content_type = text/markdown
 prodid = github.com/allenporter/flux-local
 url = https://github.com/allenporter/flux-local
 author = Allen Porter
 author_email = allen.porter@gmail.com
```

### Comparing `flux_local-5.0.1/tests/test_command.py` & `flux_local-5.1.0/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/tests/test_git_repo.py` & `flux_local-5.1.0/tests/test_git_repo.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/tests/test_helm.py` & `flux_local-5.1.0/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/tests/test_image.py` & `flux_local-5.1.0/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/tests/test_kustomize.py` & `flux_local-5.1.0/tests/test_kustomize.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/tests/test_manifest.py` & `flux_local-5.1.0/tests/test_manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     )
     print(release)
     assert release.compact_dict() == {
         "name": "metallb",
         "namespace": "metallb",
         "chart": {
             "name": "metallb",
+            "repo_kind": "HelmRepository",
             "repo_name": "bitnami",
             "repo_namespace": "flux-system",
         },
     }
 
 
 def test_parse_helm_repository() -> None:
```

### Comparing `flux_local-5.0.1/tests/test_values.py` & `flux_local-5.1.0/tests/test_values.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/tests/tool/test_build.py` & `flux_local-5.1.0/tests/tool/test_build.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,22 +21,24 @@
                 "--skip-crds",
                 "tests/testdata/cluster6/",
                 "-a",
                 "batch/v1/CronJob",
             ]
         ),
         (["--enable-helm", "--no-skip-secrets", "tests/testdata/cluster8/"]),
+        (["--enable-helm", "--no-skip-secrets", "tests/testdata/cluster9/clusters/dev"]),
     ],
     ids=[
         "build",
         "build-cluster2",
         "build-cluster3",
         "build-cluster6",
         "build-helm-cluster",
         "build-helm-cluster6",
-        "build-helm-cluster8-valuesFrom"
+        "build-helm-cluster8-valuesFrom",
+        "build-helm-cluster9",
     ],
 )
 async def test_build(args: list[str], snapshot: SnapshotAssertion) -> None:
     """Test build commands."""
     result = await run_command(["build"] + args)
     assert result == snapshot
```

### Comparing `flux_local-5.0.1/tests/tool/test_diagnostics.py` & `flux_local-5.1.0/tests/tool/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/tests/tool/test_diff.py` & `flux_local-5.1.0/tests/tool/test_diff.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/tests/tool/test_diff_hr.py` & `flux_local-5.1.0/tests/tool/test_diff_hr.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/tests/tool/test_diff_ks.py` & `flux_local-5.1.0/tests/tool/test_diff_ks.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/tests/tool/test_format.py` & `flux_local-5.1.0/tests/tool/test_format.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/tests/tool/test_get_cluster.py` & `flux_local-5.1.0/tests/tool/test_get_cluster.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.0.1/tests/tool/test_get_hr.py` & `flux_local-5.1.0/tests/tool/test_get_hr.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,25 +24,27 @@
         ),
         (["-A", "--path", "tests/testdata/cluster4"]),
         (["-A", "--path", "tests/testdata/cluster5"]),
         (["-A", "--path", "tests/testdata/cluster6"]),
         (["-A", "--path", "tests/testdata/cluster7"]),
         (["metallb", "-A", "--path", "tests/testdata/cluster"]),
         (["-n", "metallb", "--path", "tests/testdata/cluster"]),
+        (["-A", "--path", "tests/testdata/cluster9/clusters/dev"]),
     ],
     ids=[
         "cluster",
         "cluster2",
         "cluster3-no-source",
         "cluster3",
         "cluster4",
         "cluster5",
         "cluster6",
         "cluster7",
         "all_namespace",
         "name",
+        "cluster9",
     ],
 )
 async def test_get_hr(args: list[str], snapshot: SnapshotAssertion) -> None:
     """Test test get hr commands."""
     result = await run_command(["get", "hr"] + args)
     assert result == snapshot
```

### Comparing `flux_local-5.0.1/tests/tool/test_get_ks.py` & `flux_local-5.1.0/tests/tool/test_get_ks.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,26 +25,28 @@
         (["--path", "tests/testdata/cluster5"]),
         (["--all", "--path", "tests/testdata/cluster5"]),
         (["--path", "tests/testdata/cluster6"]),
         (["--path", "tests/testdata/cluster7"]),
         (["--path", "./tests/testdata/cluster/clusters/prod"]),
         (["--path", "tests/testdata/cluster", "-o", "wide"]),
         (["--all-namespaces", "--path", "./tests/testdata/cluster/apps/prod"]),
+        (["--path", "tests/testdata/cluster9/clusters/dev"]),
     ],
     ids=[
         "cluster",
         "cluster2",
         "cluster3",
         "cluster4",
         "cluster5",
         "cluster5-all",
         "cluster6",
         "cluster7",
         "cluster_path",
         "wide",
         "ks_path",
+        "cluster9",
     ],
 )
 async def test_get_ks(args: list[str], snapshot: SnapshotAssertion) -> None:
     """Test test get ks commands."""
     result = await run_command(["get", "ks"] + args)
     assert result == snapshot
```

### Comparing `flux_local-5.0.1/tests/tool/test_test.py` & `flux_local-5.1.0/tests/tool/test_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     ("args"),
     [
         (["tests/testdata/cluster"]),
         (["tests/testdata/cluster2"]),
         (["--sources", "cluster=tests/testdata/cluster3", "tests/testdata/cluster3"]),
         (["--enable-kyverno", "tests/testdata/cluster"]),
         (["--enable-kyverno", "tests/testdata/cluster2"]),
+        (["tests/testdata/cluster9/clusters/dev"]),
     ],
-    ids=["cluster", "cluster2", "cluster3", "policy", "policy-cluster2"],
+    ids=["cluster", "cluster2", "cluster3", "policy", "policy-cluster2", "cluster9"],
 )
 async def test_test_hr(args: list[str]) -> None:
     """Test test helmrelease commands."""
     result = await run_command(["test", "--enable-helm"] + args)
     assert "passed" in result
```

