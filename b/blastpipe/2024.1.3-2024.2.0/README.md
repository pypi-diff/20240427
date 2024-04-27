# Comparing `tmp/blastpipe-2024.1.3.tar.gz` & `tmp/blastpipe-2024.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blastpipe-2024.1.3.tar", last modified: Fri Apr 26 17:18:23 2024, max compression
+gzip compressed data, was "blastpipe-2024.2.0.tar", last modified: Sat Apr 27 21:36:06 2024, max compression
```

## Comparing `blastpipe-2024.1.3.tar` & `blastpipe-2024.2.0.tar`

### file list

```diff
@@ -1,60 +1,305 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:18:23.549308 blastpipe-2024.1.3/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     5868 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.github/workflows/ozi.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.github/workflows/scorecards.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/.pre-commit-config.yaml
--rw-rw-r--   0 runner    (1001) docker     (127)    83194 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/LICENSE.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-26 17:18:23.549308 blastpipe-2024.1.3/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/README.rst
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/
--rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/__init__.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/backports.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/buffer.py
--rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/buffer.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/loop.py
--rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/loop.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/malloc.py
--rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/malloc.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1235 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/mixin.py
--rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/mixin.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/sequence.py
--rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/sequence.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/tailcall.py
--rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/blastpipe/tailcall.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3291 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4520 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     8329 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/LICENSE.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/_static/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/_static/css/
--rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/_static/css/custom.css
--rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/_static/css/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/_static/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/_templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/_templates/layout.html
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/_templates/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/conf.cfg
--rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/index.rst
--rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/docs/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      121 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/subprojects/ozi.wrap
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/tests/test_backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/tests/test_fuzz.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-26 17:12:48.000000 blastpipe-2024.1.3/tests/test_tailcall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:36:06.435307 blastpipe-2024.2.0/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     5868 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/.github/workflows/ozi.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/.github/workflows/scorecards.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/.pre-commit-config.yaml
+-rw-rw-r--   0 runner    (1001) docker     (127)    84029 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/LICENSE.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-27 21:36:06.435307 blastpipe-2024.2.0/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/README.rst
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/__init__.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/backports.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/buffer.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/buffer.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/loop.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/loop.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/malloc.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/malloc.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1250 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/mixin.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/mixin.pyi
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)      359 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/.gitignore.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      212 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/CHANGELOG.md.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      342 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/LICENSE.txt.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      112 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/PKG-INFO.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      618 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/README.rst.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     1859 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      269 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/bandit.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      267 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/bandit.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      266 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/black.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      228 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/black.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      627 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/coverage.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      220 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/doc8.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      124 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/doc8.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2798 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/filter.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      385 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/flake8.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      432 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/flake8.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/github_workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1648 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/github_workflows/checkpoint.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      804 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/github_workflows/generate_provenance.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      542 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/github_workflows/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      602 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/github_workflows/ozi.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      757 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/github_workflows/publish.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     1375 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/github_workflows/release.yml.j2
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/gitlab_workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)      335 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/gitlab_workflows/ozi.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      349 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/isort.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      283 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/isort.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/cc0-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      343 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/agpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/agpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/apache-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/artistic-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/bsd-3-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    18660 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/cc-by-4.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    20141 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/cc-by-sa-4.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/epl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/gpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/gpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/isc.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/lgpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      835 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/mit.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/ofl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      485 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/wtfpl.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/DFSG_approved/zlib.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/
+-rw-rw-r--   0 runner    (1001) docker     (127)    11067 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      359 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ncsa.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    10315 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      357 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/apache-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      360 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)    19765 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    20209 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    19902 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    21198 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      419 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/artistic-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      362 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      710 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/0bsd.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1346 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1713 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      457 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1340 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      357 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    22960 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      360 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/epl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      357 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    14199 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      357 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    13154 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      358 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    13831 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      358 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      393 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/agpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      367 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      393 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      443 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      391 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      366 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      391 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      366 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      393 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      397 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      393 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      367 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      447 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/isc.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      353 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      353 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/mit.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      355 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      952 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      357 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       88 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/mpl-2.0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      463 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     9269 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      442 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    10302 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      360 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      442 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/ofl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1639 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/zlib.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/Public_Domain/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/Public_Domain/cc0-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/Public_Domain/licenseref-public-domain.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/Public_Domain/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1213 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/Public_Domain/unlicense.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    34525 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/agpl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    11359 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/apache-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     8896 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/artistic-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1544 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/bsd-3-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7050 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/cc0-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    11587 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/epl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    22965 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/gfdl-1.3.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    18094 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/gpl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    35151 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/gpl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      788 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/isc.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    25381 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/lgpl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    26528 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/lgpl-2.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7654 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/lgpl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1192 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1114 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/mit.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      260 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/ofl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)      901 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/license/zlib.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1844 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      418 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/meson.build.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      883 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/meson.options.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      168 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/mypy.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/mypy.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1151 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/new_child.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      353 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/ozi.wrap.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     2503 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/project.PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     1138 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/project.array.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      621 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/project.feature.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      544 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/project.integer.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     3602 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/project.meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/project.name/
+-rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/project.name/__init__.py.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      289 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/project.name/__init__.pyi.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      442 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/project.name/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      755 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/project.name/meson.build.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/project.name/new_module.py.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      129 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/project.name/py.typed.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      129 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/project.ozi.wrap.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/pydocstyle.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/pylint.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      600 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/pyproject.toml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      231 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/pyright.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      245 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/pyright.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      392 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/pytest.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      422 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/pytest.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      150 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/requirements.in.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      229 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/restructuredtext-lint.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     1224 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/root.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1126 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/ruff.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1124 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/semantic_release.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      341 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/setuptools_scm.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      359 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/tests/meson.build.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      260 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/tests/new_test.py.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     1427 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/ozi_templates/tox.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/sequence.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/sequence.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/tailcall.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/blastpipe/tailcall.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3291 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4520 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     8329 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)       33 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/subprojects/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/subprojects/docs/
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/subprojects/docs/LICENSE.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/subprojects/docs/_static/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/subprojects/docs/_static/css/
+-rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/subprojects/docs/_static/css/custom.css
+-rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/subprojects/docs/_static/css/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/subprojects/docs/_static/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/subprojects/docs/_templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/subprojects/docs/_templates/layout.html
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/subprojects/docs/_templates/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/subprojects/docs/conf.cfg
+-rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/subprojects/docs/index.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/subprojects/docs/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/subprojects/docs/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      121 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/subprojects/ozi.wrap
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      832 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/tests/test_backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1072 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/tests/test_filter.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/tests/test_fuzz.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-27 21:30:09.000000 blastpipe-2024.2.0/tests/test_tailcall.py
```

### Comparing `blastpipe-2024.1.3/.github/workflows/codeql.yml` & `blastpipe-2024.2.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/.github/workflows/dependency-review.yml` & `blastpipe-2024.2.0/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/.github/workflows/ozi.yml` & `blastpipe-2024.2.0/.github/workflows/ozi.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/.github/workflows/scorecards.yml` & `blastpipe-2024.2.0/.github/workflows/scorecards.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/.gitignore` & `blastpipe-2024.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/CHANGELOG.md` & `blastpipe-2024.2.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,36 @@
 # CHANGELOG
 
 
 
+## v2024.2.0 (2024-04-27)
+
+### :heavy_plus_sign:
+
+* :heavy_plus_sign: add deps jinja2, requests, types-requests.
+
+Signed-off-by: rjdbcm &lt;rjdbcm@outlook.com&gt; ([`2d566c8`](https://github.com/OZI-Project/blastpipe/commit/2d566c835be404bb95ed465d680416c5adda2575))
+
+### :pencil2:
+
+* :pencil2: fix missing source children. ([`0574d2f`](https://github.com/OZI-Project/blastpipe/commit/0574d2f0ac75fc6ddbf18553fb8ed30a2d52f66c))
+
+### :sparkles:
+
+* :sparkles: add ozi_templates subdir.
+
+Signed-off-by: rjdbcm &lt;rjdbcm@outlook.com&gt; ([`08869d3`](https://github.com/OZI-Project/blastpipe/commit/08869d31b561c5eabe445548cd84c7f8391d14f8))
+
+### Other
+
+* :rotating_light: run isort
+
+Signed-off-by: rjdbcm &lt;rjdbcm@outlook.com&gt; ([`d0ade4a`](https://github.com/OZI-Project/blastpipe/commit/d0ade4a18dfa0429e6f38771278d828319e33b74))
+
+
 ## v2024.1.3 (2024-04-26)
 
 ### :arrow_up:
 
 * :arrow_up: Bump github/codeql-action from 3.25.2 to 3.25.3
 
 Bumps [github/codeql-action](https://github.com/github/codeql-action) from 3.25.2 to 3.25.3.
```

### Comparing `blastpipe-2024.1.3/LICENSE.txt` & `blastpipe-2024.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/NOTICE.md` & `blastpipe-2024.2.0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/PKG-INFO` & `blastpipe-2024.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: blastpipe
-Version: 2024.1.3
+Version: 2024.2.0
 Summary: OZI integrated test library.
 Home-page: https://oziproject.dev
 Author: Eden Ross Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
-Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.1.3.tar.gz
+Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.2.0.tar.gz
 Requires-Python: >=3.10, <3.13
 Keywords: ozi,meson
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Other Audience
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Classifier: Environment :: Other Environment
 Description-Content-Type: text/x-rst
-
+Requires-Dist: jinja2>3
+Requires-Dist: requests
+Requires-Dist: types-requests
 
 .. OZI
   Classifier: License-Expression :: Apache-2.0 WITH LLVM-exception
   Classifier: License-File :: LICENSE.txt
 
 .. README.rst
    Part of the OZI Project, under the Apache License v2.0 with LLVM Exceptions.
```

### Comparing `blastpipe-2024.1.3/README.rst` & `blastpipe-2024.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/blastpipe/__init__.py` & `blastpipe-2024.2.0/blastpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/blastpipe/backports.py` & `blastpipe-2024.2.0/blastpipe/backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/blastpipe/backports.pyi` & `blastpipe-2024.2.0/blastpipe/backports.pyi`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/blastpipe/buffer.py` & `blastpipe-2024.2.0/blastpipe/buffer.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/blastpipe/loop.py` & `blastpipe-2024.2.0/blastpipe/loop.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/blastpipe/malloc.py` & `blastpipe-2024.2.0/blastpipe/malloc.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/blastpipe/meson.build` & `blastpipe-2024.2.0/blastpipe/meson.build`

 * *Files 9% similar despite different names*

```diff
@@ -33,11 +33,11 @@
 ]
 foreach file: source_files
     fs.copyfile(file)
     if not meson.is_subproject() or get_option('install-subprojects').enabled()
         python.install_sources(file, subdir: project_name)
     endif
 endforeach
-source_children = []
+source_children = ['ozi_templates']
 foreach child: source_children
     subdir(child)
 endforeach
```

### Comparing `blastpipe-2024.1.3/blastpipe/mixin.py` & `blastpipe-2024.2.0/blastpipe/mixin.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/blastpipe/sequence.py` & `blastpipe-2024.2.0/blastpipe/sequence.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/blastpipe/tailcall.py` & `blastpipe-2024.2.0/blastpipe/tailcall.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/meson.build` & `blastpipe-2024.2.0/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/meson.options` & `blastpipe-2024.2.0/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/pyproject.toml` & `blastpipe-2024.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/subprojects/docs/LICENSE.txt` & `blastpipe-2024.2.0/subprojects/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/subprojects/docs/_static/css/custom.css` & `blastpipe-2024.2.0/subprojects/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/subprojects/docs/_static/css/meson.build` & `blastpipe-2024.2.0/subprojects/docs/_static/css/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/subprojects/docs/_static/meson.build` & `blastpipe-2024.2.0/subprojects/docs/_static/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/subprojects/docs/_templates/layout.html` & `blastpipe-2024.2.0/subprojects/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/subprojects/docs/_templates/meson.build` & `blastpipe-2024.2.0/subprojects/docs/_templates/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/subprojects/docs/conf.cfg` & `blastpipe-2024.2.0/subprojects/docs/conf.cfg`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/subprojects/docs/index.rst` & `blastpipe-2024.2.0/subprojects/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/subprojects/docs/meson.build` & `blastpipe-2024.2.0/subprojects/docs/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/subprojects/docs/meson.options` & `blastpipe-2024.2.0/subprojects/docs/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/tests/meson.build` & `blastpipe-2024.2.0/tests/meson.build`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 test_files = [
  'test_backports.py',
+ 'test_filter.py',
  'test_fuzz.py',
  'test_tailcall.py',
 ]
 foreach file: test_files
   fs.copyfile(file)
   python.install_sources(file, subdir: project_name/'tests')
 endforeach
```

### Comparing `blastpipe-2024.1.3/tests/test_backports.py` & `blastpipe-2024.2.0/tests/test_backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/tests/test_fuzz.py` & `blastpipe-2024.2.0/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.3/tests/test_tailcall.py` & `blastpipe-2024.2.0/tests/test_tailcall.py`

 * *Files identical despite different names*

