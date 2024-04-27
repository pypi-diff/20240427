# Comparing `tmp/github-provenance-demo-0.0.8.tar.gz` & `tmp/github-provenance-demo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github-provenance-demo-0.0.8.tar", last modified: Tue Apr  9 14:07:25 2024, max compression
+gzip compressed data, was "github-provenance-demo-0.0.9.tar", last modified: Tue Apr  9 17:18:20 2024, max compression
```

## Comparing `github-provenance-demo-0.0.8.tar` & `github-provenance-demo-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:07:25.103007 github-provenance-demo-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 14:07:25.103007 github-provenance-demo-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 14:07:20.000000 github-provenance-demo-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:07:25.103007 github-provenance-demo-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:07:25.103007 github-provenance-demo-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:07:25.103007 github-provenance-demo-0.0.8/src/github-provenance-demo/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 14:07:20.000000 github-provenance-demo-0.0.8/src/github-provenance-demo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:07:25.103007 github-provenance-demo-0.0.8/src/github_provenance_demo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 14:07:25.000000 github-provenance-demo-0.0.8/src/github_provenance_demo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 14:07:25.000000 github-provenance-demo-0.0.8/src/github_provenance_demo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:07:25.000000 github-provenance-demo-0.0.8/src/github_provenance_demo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 14:07:25.000000 github-provenance-demo-0.0.8/src/github_provenance_demo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:18:20.881013 github-provenance-demo-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 17:18:20.877013 github-provenance-demo-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 17:18:16.000000 github-provenance-demo-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:18:20.881013 github-provenance-demo-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:18:20.877013 github-provenance-demo-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:18:20.877013 github-provenance-demo-0.0.9/src/github-provenance-demo/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 17:18:16.000000 github-provenance-demo-0.0.9/src/github-provenance-demo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:18:20.877013 github-provenance-demo-0.0.9/src/github_provenance_demo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 17:18:20.000000 github-provenance-demo-0.0.9/src/github_provenance_demo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 17:18:20.000000 github-provenance-demo-0.0.9/src/github_provenance_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:18:20.000000 github-provenance-demo-0.0.9/src/github_provenance_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 17:18:20.000000 github-provenance-demo-0.0.9/src/github_provenance_demo.egg-info/top_level.txt
```

