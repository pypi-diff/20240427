# Comparing `tmp/silverback-0.3.2.tar.gz` & `tmp/silverback-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silverback-0.3.2.tar", last modified: Wed Apr 17 00:47:13 2024, max compression
+gzip compressed data, was "silverback-0.3.3.tar", last modified: Sat Apr 27 18:07:03 2024, max compression
```

## Comparing `silverback-0.3.2.tar` & `silverback-0.3.3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.643592 silverback-0.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.639592 silverback-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.639592 silverback-0.3.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.639592 silverback-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-17 00:46:12.000000 silverback-0.3.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-17 00:46:12.000000 silverback-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-17 00:46:12.000000 silverback-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-17 00:46:12.000000 silverback-0.3.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-17 00:46:12.000000 silverback-0.3.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-17 00:46:12.000000 silverback-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-17 00:47:13.643592 silverback-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-17 00:46:12.000000 silverback-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-17 00:46:12.000000 silverback-0.3.2/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.639592 silverback-0.3.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.639592 silverback-0.3.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.639592 silverback-0.3.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.639592 silverback-0.3.2/docs/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/commands/run.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.639592 silverback-0.3.2/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/methoddocs/application.md
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/methoddocs/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/methoddocs/middlewares.md
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/methoddocs/runner.md
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/methoddocs/subscriptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.643592 silverback-0.3.2/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/userguides/development.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 00:46:12.000000 silverback-0.3.2/docs/userguides/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-17 00:46:12.000000 silverback-0.3.2/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-17 00:46:12.000000 silverback-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-17 00:47:13.643592 silverback-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-17 00:46:12.000000 silverback-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.643592 silverback-0.3.2/silverback/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-17 00:46:12.000000 silverback-0.3.2/silverback/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 00:47:13.000000 silverback-0.3.2/silverback/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.643592 silverback-0.3.2/silverback.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-17 00:47:13.000000 silverback-0.3.2/silverback.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-17 00:47:13.000000 silverback-0.3.2/silverback.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 00:47:13.000000 silverback-0.3.2/silverback.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-17 00:47:13.000000 silverback-0.3.2/silverback.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 00:47:13.000000 silverback-0.3.2/silverback.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-17 00:47:13.000000 silverback-0.3.2/silverback.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-17 00:47:13.000000 silverback-0.3.2/silverback.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:47:13.643592 silverback-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:46:12.000000 silverback-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-17 00:46:12.000000 silverback-0.3.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-17 00:46:12.000000 silverback-0.3.2/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.886002 silverback-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.878003 silverback-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.878003 silverback-0.3.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.878003 silverback-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-27 18:06:08.000000 silverback-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-27 18:06:08.000000 silverback-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-27 18:06:08.000000 silverback-0.3.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-27 18:06:08.000000 silverback-0.3.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-27 18:06:08.000000 silverback-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-27 18:07:03.886002 silverback-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-27 18:06:08.000000 silverback-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-27 18:06:08.000000 silverback-0.3.3/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.878003 silverback-0.3.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.878003 silverback-0.3.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.878003 silverback-0.3.3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.878003 silverback-0.3.3/docs/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/commands/run.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.882002 silverback-0.3.3/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/methoddocs/application.md
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/methoddocs/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/methoddocs/middlewares.md
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/methoddocs/runner.md
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/methoddocs/subscriptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.882002 silverback-0.3.3/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/userguides/development.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/userguides/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-27 18:06:08.000000 silverback-0.3.3/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-27 18:06:08.000000 silverback-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-27 18:07:03.886002 silverback-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-27 18:06:08.000000 silverback-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.882002 silverback-0.3.3/silverback/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 18:07:03.000000 silverback-0.3.3/silverback/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.882002 silverback-0.3.3/silverback.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-27 18:07:03.000000 silverback-0.3.3/silverback.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-27 18:07:03.000000 silverback-0.3.3/silverback.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 18:07:03.000000 silverback-0.3.3/silverback.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-27 18:07:03.000000 silverback-0.3.3/silverback.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 18:07:03.000000 silverback-0.3.3/silverback.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-27 18:07:03.000000 silverback-0.3.3/silverback.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 18:07:03.000000 silverback-0.3.3/silverback.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.886002 silverback-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 18:06:08.000000 silverback-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-27 18:06:08.000000 silverback-0.3.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-27 18:06:08.000000 silverback-0.3.3/tests/test_cli.py
```

### Comparing `silverback-0.3.2/.github/ISSUE_TEMPLATE/bug.md` & `silverback-0.3.3/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/.github/ISSUE_TEMPLATE/feature.md` & `silverback-0.3.3/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/.github/ISSUE_TEMPLATE/work-item.md` & `silverback-0.3.3/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/.github/release-drafter.yml` & `silverback-0.3.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/.github/workflows/codeql.yaml` & `silverback-0.3.3/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/.github/workflows/commitlint.yaml` & `silverback-0.3.3/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/.github/workflows/docs.yaml` & `silverback-0.3.3/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/.github/workflows/prtitle.yaml` & `silverback-0.3.3/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/.github/workflows/publish.yaml` & `silverback-0.3.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/.github/workflows/test.yaml` & `silverback-0.3.3/.github/workflows/test.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -58,15 +58,17 @@
           run: mypy .
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
-                os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
+                # TODO: Replace with macos-latest when works again.
+                #   https://github.com/actions/setup-python/issues/808
+                os: [ubuntu-latest, macos-12]   # eventually add `windows-latest`
                 python-version: [3.8, 3.9, "3.10", "3.11"]
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
```

### Comparing `silverback-0.3.2/.gitignore` & `silverback-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/.pre-commit-config.yaml` & `silverback-0.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/CONTRIBUTING.md` & `silverback-0.3.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/Dockerfile` & `silverback-0.3.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/LICENSE` & `silverback-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/PKG-INFO` & `silverback-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.3.2
+Version: 0.3.3
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/ApeWorX/silverback
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `silverback-0.3.2/README.md` & `silverback-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/build_docs.py` & `silverback-0.3.3/build_docs.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/docs/_static/custom.css` & `silverback-0.3.3/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/docs/_static/custom.js` & `silverback-0.3.3/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/docs/_templates/layout.html` & `silverback-0.3.3/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/docs/conf.py` & `silverback-0.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/docs/favicon.ico` & `silverback-0.3.3/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/docs/logo.gif` & `silverback-0.3.3/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/docs/userguides/development.md` & `silverback-0.3.3/docs/userguides/development.md`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/example.py` & `silverback-0.3.3/example.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/pyproject.toml` & `silverback-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/setup.py` & `silverback-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/silverback",
     include_package_data=True,
     install_requires=[
         "click",  # Use same version as eth-ape
         "eth-ape>=0.7.0,<1.0",
+        "ethpm-types>=0.6.10",  # lower pin only, `eth-ape` governs upper pin
         "eth-pydantic-types",  # Use same version as eth-ape
         "pydantic_settings",  # Use same version as eth-ape
         "taskiq[metrics]>=0.10.4,<0.11.0",
     ],
     entry_points={
         "console_scripts": ["silverback=silverback._cli:cli"],
     },
```

### Comparing `silverback-0.3.2/silverback/_cli.py` & `silverback-0.3.3/silverback/_cli.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/silverback/_importer.py` & `silverback-0.3.3/silverback/_importer.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/silverback/application.py` & `silverback-0.3.3/silverback/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,18 +114,26 @@
                 and container is not None
             )
         ):
             raise ContainerTypeMismatchError(task_type, container)
 
         # Register user function as task handler with our broker
         def add_taskiq_task(handler: Callable) -> AsyncTaskiqDecoratedTask:
+            labels = {"task_type": str(task_type)}
+
+            if container and isinstance(container, ContractEvent):
+                # Address is almost a certainty if the container is being used as a filter here.
+                if contract_address := getattr(container.contract, "address", None):
+                    labels["contract_address"] = contract_address
+                labels["event_signature"] = container.abi.signature
+
             broker_task = self.broker.register_task(
                 handler,
                 task_name=handler.__name__,
-                task_type=str(task_type),
+                **labels,
             )
 
             self.tasks[task_type].append(TaskData(container=container, handler=broker_task))
             return broker_task
 
         return add_taskiq_task
```

### Comparing `silverback-0.3.2/silverback/exceptions.py` & `silverback-0.3.3/silverback/exceptions.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/silverback/middlewares.py` & `silverback-0.3.3/silverback/middlewares.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,19 @@
         if labels_str := ",".join(f"{k}={v}" for k, v in message.labels.items()):
             return f"{message.task_name}[{labels_str}]"
 
         else:
             return message.task_name
 
     def pre_execute(self, message: TaskiqMessage) -> TaskiqMessage:
-        if not (task_type := message.labels.pop("task_type")):
+        if "task_type" not in message.labels:
             return message  # Not a silverback task
 
+        task_type = message.labels.pop("task_type")
+
         try:
             task_type = TaskType(task_type)
         except ValueError:
             return message  # Not a silverback task
 
         # Add extra labels for our task to see what their source was
         if task_type is TaskType.NEW_BLOCKS:
```

### Comparing `silverback-0.3.2/silverback/persistence.py` & `silverback-0.3.3/silverback/persistence.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/silverback/runner.py` & `silverback-0.3.3/silverback/runner.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/silverback/settings.py` & `silverback-0.3.3/silverback/settings.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/silverback/subscriptions.py` & `silverback-0.3.3/silverback/subscriptions.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/silverback/types.py` & `silverback-0.3.3/silverback/types.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/silverback/utils.py` & `silverback-0.3.3/silverback/utils.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/silverback.egg-info/PKG-INFO` & `silverback-0.3.3/silverback.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.3.2
+Version: 0.3.3
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/ApeWorX/silverback
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `silverback-0.3.2/silverback.egg-info/SOURCES.txt` & `silverback-0.3.3/silverback.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `silverback-0.3.2/silverback.egg-info/requires.txt` & `silverback-0.3.3/silverback.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 click
 eth-ape<1.0,>=0.7.0
+ethpm-types>=0.6.10
 eth-pydantic-types
 pydantic_settings
 taskiq[metrics]<0.11.0,>=0.10.4
 
 [dev]
 pytest>=6.0
 pytest-xdist
```

