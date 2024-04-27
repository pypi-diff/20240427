# Comparing `tmp/OZI-1.1.5.tar.gz` & `tmp/OZI-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OZI-1.1.5.tar", last modified: Wed Apr 24 19:47:02 2024, max compression
+gzip compressed data, was "OZI-1.1.6.tar", last modified: Sat Apr 27 00:24:36 2024, max compression
```

## Comparing `OZI-1.1.5.tar` & `OZI-1.1.6.tar`

### file list

```diff
@@ -1,377 +1,377 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:47:02.133451 OZI-1.1.5/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-04-24 19:41:10.000000 OZI-1.1.5/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-04-24 19:41:10.000000 OZI-1.1.5/.github/CODEOWNERS
--rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-04-24 19:41:10.000000 OZI-1.1.5/.github/CODE_OF_CONDUCT.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-04-24 19:41:10.000000 OZI-1.1.5/.github/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-04-24 19:41:10.000000 OZI-1.1.5/.github/FUNDING.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-04-24 19:41:10.000000 OZI-1.1.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-04-24 19:41:10.000000 OZI-1.1.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-24 19:41:10.000000 OZI-1.1.5/.github/SECURITY.md
--rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-04-24 19:41:10.000000 OZI-1.1.5/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-04-24 19:41:10.000000 OZI-1.1.5/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-04-24 19:41:10.000000 OZI-1.1.5/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     2900 2024-04-24 19:41:10.000000 OZI-1.1.5/.github/workflows/dev-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     5873 2024-04-24 19:41:10.000000 OZI-1.1.5/.github/workflows/dist-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3544 2024-04-24 19:41:10.000000 OZI-1.1.5/.github/workflows/scorecard.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-04-24 19:41:10.000000 OZI-1.1.5/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)   284160 2024-04-24 19:41:10.000000 OZI-1.1.5/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-04-24 19:41:10.000000 OZI-1.1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-04-24 19:47:02.133451 OZI-1.1.5/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     6937 2024-04-24 19:41:10.000000 OZI-1.1.5/README.rst
--rw-rw-r--   0 runner    (1001) docker     (127)    16576 2024-04-24 19:41:10.000000 OZI-1.1.5/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     7664 2024-04-24 19:41:10.000000 OZI-1.1.5/meson.options
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/
--rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/actions.py
--rw-rw-r--   0 runner    (1001) docker     (127)     5811 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/comment.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/dist/
--rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/dist/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/dist/semantic_release/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/dist/semantic_release/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/dist/semantic_release/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/dist/sigstore/
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/dist/sigstore/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/dist/sigstore/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)     3368 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/filter.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/fix/
--rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/fix/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2367 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/fix/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4061 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/fix/build_definition.py
--rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/fix/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6265 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/fix/missing.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3612 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/fix/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7877 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/fix/rewrite_command.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/bandit/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/bandit/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/bandit/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/black/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/black/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/black/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/flake8/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/flake8/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/flake8/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/isort/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/isort/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/isort/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/mypy/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/mypy/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/mypy/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/pyright/
--rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/pyright/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/pyright/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/restructuredtext-lint/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/restructuredtext-lint/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       21 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/lint/restructuredtext-lint/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      842 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/meson.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/new/
--rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/new/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4731 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/new/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/new/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6436 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/new/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/new/validate.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/pkg_extra.py
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     6193 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/render.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/scripts/
--rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/scripts/core_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/scripts/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2044 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/scripts/meson_dist_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/scripts/meson_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/scripts/render_requirements.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/scripts/replace_ruff_target_version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/scripts/scm_version_snip.py
--rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/scripts/to_distribution_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/scripts/version_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/spdx.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/spec/
--rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/spec/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/spec/_license.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1687 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/spec/_spec.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/spec/base.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6070 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/spec/ci.py
--rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/spec/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/spec/pkg.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/spec/project.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6347 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/spec/python.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4572 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/spec/src.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/tap.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/
--rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/.gitignore.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      212 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/CHANGELOG.md.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      487 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/LICENSE.txt.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      257 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/PKG-INFO.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      763 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/README.rst.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      414 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/bandit.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/bandit.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/black.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      373 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/black.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      772 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/coverage.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/doc8.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      269 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/doc8.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      530 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/flake8.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      577 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/flake8.pyproject.toml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/github_workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     1793 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/github_workflows/checkpoint.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      804 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/github_workflows/generate_provenance.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      687 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/github_workflows/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      747 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/github_workflows/ozi.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      991 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/github_workflows/publish.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     1518 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/github_workflows/release.yml.j2
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/gitlab_workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)      480 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/gitlab_workflows/ozi.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      494 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/isort.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      428 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/isort.pyproject.toml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/cc0-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      490 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/agpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/agpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/apache-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/artistic-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/bsd-3-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    18660 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/cc-by-4.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    20141 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/cc-by-sa-4.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/epl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/gpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/gpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/isc.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/lgpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/lgpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/lgpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/mit.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/ofl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      485 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/wtfpl.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/DFSG_approved/zlib.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/Free_To_Use_But_Restricted/
--rw-rw-r--   0 runner    (1001) docker     (127)    11067 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      506 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/Free_To_Use_But_Restricted/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/Free_To_Use_But_Restricted/ncsa.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Academic_Free_License__AFL_/
--rw-rw-r--   0 runner    (1001) docker     (127)    10315 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Academic_Free_License__AFL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Apache_Software_License/
--rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Apache_Software_License/apache-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      507 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Apache_Software_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/
--rw-rw-r--   0 runner    (1001) docker     (127)    19765 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    20209 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    19902 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    21198 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      566 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Artistic_License/
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Artistic_License/artistic-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      509 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Artistic_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/BSD_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      710 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/BSD_License/0bsd.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1346 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/BSD_License/bsd-3-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1713 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      604 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/BSD_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)     1340 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/
--rw-rw-r--   0 runner    (1001) docker     (127)    22960 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      507 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/epl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)    14199 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/
--rw-rw-r--   0 runner    (1001) docker     (127)    13154 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      505 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/
--rw-rw-r--   0 runner    (1001) docker     (127)    13831 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      505 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      540 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/agpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      540 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      590 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      513 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      513 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      540 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      544 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      540 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      594 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/ISC_License__ISCL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/ISC_License__ISCL_/isc.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      500 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/ISC_License__ISCL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/MIT_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      500 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/MIT_License/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/MIT_License/mit.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      952 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       88 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/mpl-2.0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      610 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     9269 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    10302 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/PostgreSQL_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      507 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/PostgreSQL_License/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/ofl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1784 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/zlib_libpng_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/zlib_libpng_License/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/OSI_Approved/zlib_libpng_License/zlib.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/Public_Domain/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/Public_Domain/cc0-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/Public_Domain/licenseref-public-domain.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      547 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/Public_Domain/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1213 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/Public_Domain/unlicense.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    34525 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/agpl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    11359 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/apache-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     8896 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/artistic-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1544 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/bsd-3-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7050 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/cc0-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    11587 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/epl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    22965 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/gfdl-1.3.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    18094 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/gpl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    35151 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/gpl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      788 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/isc.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    25381 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/lgpl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    26528 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/lgpl-2.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7654 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/lgpl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1106 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1114 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/mit.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      260 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/ofl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      901 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/license/zlib.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1898 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      563 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/meson.build.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     1028 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/meson.options.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      313 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/mypy.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      391 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/mypy.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     1296 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/new_child.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      498 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/ozi.wrap.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     2648 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/project.PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     1283 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/project.array.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      766 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/project.feature.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      689 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/project.integer.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     3684 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/project.meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/project.name/
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/project.name/__init__.py.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/project.name/__init__.pyi.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/project.name/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      900 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/project.name/meson.build.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      394 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/project.name/new_module.py.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      274 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/project.name/py.typed.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      129 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/project.ozi.wrap.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      396 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/pydocstyle.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/pylint.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      600 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/pyproject.toml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      376 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/pyright.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      390 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/pyright.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      537 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/pytest.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/pytest.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/requirements.in.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      374 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/restructuredtext-lint.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     1369 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/root.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     1271 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/ruff.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     1269 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/semantic_release.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      486 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/setuptools_scm.pyproject.toml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      866 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/tests/meson.build.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/tests/new_test.py.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     1572 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/templates/tox.pyproject.toml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/test/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/test/coverage/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/test/coverage/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/test/coverage/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/test/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/test/pytest/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/test/pytest/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/test/pytest/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/trove.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/vendor/
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/vendor/__init__.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/vendor/email_validator/
--rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/vendor/email_validator/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/vendor/email_validator/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/vendor/email_validator/deliverability.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/vendor/email_validator/exceptions_types.py
--rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/vendor/email_validator/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/vendor/email_validator/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/vendor/email_validator/rfc_constants.py
--rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/vendor/email_validator/syntax.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/vendor/email_validator/validate_email.py
--rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/vendor/email_validator/version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-04-24 19:41:10.000000 OZI-1.1.5/ozi/vendor/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    10639 2024-04-24 19:41:10.000000 OZI-1.1.5/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      170 2024-04-24 19:41:10.000000 OZI-1.1.5/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/subprojects/
--rw-rw-r--   0 runner    (1001) docker     (127)      342 2024-04-24 19:41:10.000000 OZI-1.1.5/subprojects/blastpipe.wrap
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-04-24 19:41:10.000000 OZI-1.1.5/templates/CHANGELOG.md.j2
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:41:10.000000 OZI-1.1.5/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-04-24 19:41:10.000000 OZI-1.1.5/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    11040 2024-04-24 19:41:10.000000 OZI-1.1.5/tests/test_ozi_fix.py
--rw-rw-r--   0 runner    (1001) docker     (127)    13823 2024-04-24 19:41:10.000000 OZI-1.1.5/tests/test_ozi_new.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-04-24 19:41:10.000000 OZI-1.1.5/tests/test_tap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:24:36.905987 OZI-1.1.6/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-04-27 00:18:52.000000 OZI-1.1.6/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-04-27 00:18:52.000000 OZI-1.1.6/.github/CODEOWNERS
+-rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-04-27 00:18:52.000000 OZI-1.1.6/.github/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-04-27 00:18:52.000000 OZI-1.1.6/.github/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-04-27 00:18:52.000000 OZI-1.1.6/.github/FUNDING.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-04-27 00:18:52.000000 OZI-1.1.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-04-27 00:18:52.000000 OZI-1.1.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-27 00:18:52.000000 OZI-1.1.6/.github/SECURITY.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-04-27 00:18:52.000000 OZI-1.1.6/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-04-27 00:18:52.000000 OZI-1.1.6/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-04-27 00:18:52.000000 OZI-1.1.6/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2900 2024-04-27 00:18:52.000000 OZI-1.1.6/.github/workflows/dev-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     5873 2024-04-27 00:18:52.000000 OZI-1.1.6/.github/workflows/dist-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3544 2024-04-27 00:18:52.000000 OZI-1.1.6/.github/workflows/scorecard.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-04-27 00:18:52.000000 OZI-1.1.6/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)   286340 2024-04-27 00:18:52.000000 OZI-1.1.6/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-04-27 00:18:52.000000 OZI-1.1.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-04-27 00:24:36.905987 OZI-1.1.6/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     6937 2024-04-27 00:18:52.000000 OZI-1.1.6/README.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)    16576 2024-04-27 00:18:52.000000 OZI-1.1.6/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     7664 2024-04-27 00:18:52.000000 OZI-1.1.6/meson.options
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/
+-rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/actions.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     5811 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/comment.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/dist/
+-rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/dist/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/dist/semantic_release/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/dist/semantic_release/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/dist/semantic_release/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/dist/sigstore/
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/dist/sigstore/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/dist/sigstore/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     3368 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/filter.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/fix/
+-rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/fix/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2416 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/fix/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4061 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/fix/build_definition.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/fix/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6265 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/fix/missing.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3612 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/fix/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7877 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/fix/rewrite_command.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/bandit/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/bandit/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/bandit/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/black/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/black/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/black/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/flake8/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/flake8/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/flake8/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/isort/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/isort/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/isort/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/mypy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/mypy/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/mypy/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/pyright/
+-rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/pyright/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/pyright/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/restructuredtext-lint/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/restructuredtext-lint/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       21 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/lint/restructuredtext-lint/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      842 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/meson.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/new/
+-rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/new/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4800 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/new/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/new/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6436 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/new/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/new/validate.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/pkg_extra.py
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     6222 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/render.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/scripts/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/scripts/core_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/scripts/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2044 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/scripts/meson_dist_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/scripts/meson_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/scripts/render_requirements.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/scripts/replace_ruff_target_version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/scripts/scm_version_snip.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/scripts/to_distribution_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/scripts/version_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/spdx.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/spec/
+-rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/spec/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/spec/_license.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1687 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/spec/_spec.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/spec/base.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6070 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/spec/ci.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/spec/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/spec/pkg.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/spec/project.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6347 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/spec/python.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4572 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/spec/src.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/tap.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/.gitignore.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      212 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/CHANGELOG.md.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      487 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/LICENSE.txt.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      257 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/PKG-INFO.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      763 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/README.rst.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      414 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/bandit.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/bandit.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/black.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      373 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/black.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      772 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/coverage.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/doc8.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      269 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/doc8.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      530 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/flake8.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      577 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/flake8.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/github_workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1793 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/github_workflows/checkpoint.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      804 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/github_workflows/generate_provenance.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      687 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/github_workflows/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      747 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/github_workflows/ozi.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      991 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/github_workflows/publish.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     1518 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/github_workflows/release.yml.j2
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/gitlab_workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)      480 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/gitlab_workflows/ozi.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      494 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/isort.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      428 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/isort.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/cc0-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      490 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/agpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/agpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/apache-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/artistic-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/bsd-3-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    18660 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/cc-by-4.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    20141 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/cc-by-sa-4.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/epl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/gpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/gpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/isc.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/lgpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/lgpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/lgpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/mit.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/ofl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      485 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/wtfpl.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/DFSG_approved/zlib.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/Free_To_Use_But_Restricted/
+-rw-rw-r--   0 runner    (1001) docker     (127)    11067 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      506 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/Free_To_Use_But_Restricted/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/Free_To_Use_But_Restricted/ncsa.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Academic_Free_License__AFL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    10315 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Academic_Free_License__AFL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Apache_Software_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Apache_Software_License/apache-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      507 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Apache_Software_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)    19765 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    20209 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    19902 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    21198 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      566 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Artistic_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Artistic_License/artistic-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      509 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Artistic_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/BSD_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      710 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/BSD_License/0bsd.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1346 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/BSD_License/bsd-3-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1713 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      604 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/BSD_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1340 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    22960 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      507 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/epl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    14199 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    13154 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      505 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    13831 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      505 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      540 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/agpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      540 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      590 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      513 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      513 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      540 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      544 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      540 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      594 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/ISC_License__ISCL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/ISC_License__ISCL_/isc.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      500 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/ISC_License__ISCL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/MIT_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      500 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/MIT_License/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/MIT_License/mit.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      952 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       88 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/mpl-2.0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      610 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     9269 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    10302 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/PostgreSQL_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      507 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/PostgreSQL_License/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/ofl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1784 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/zlib_libpng_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/zlib_libpng_License/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/OSI_Approved/zlib_libpng_License/zlib.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/Public_Domain/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/Public_Domain/cc0-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/Public_Domain/licenseref-public-domain.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      547 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/Public_Domain/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1213 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/Public_Domain/unlicense.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    34525 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/agpl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    11359 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/apache-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     8896 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/artistic-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1544 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/bsd-3-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7050 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/cc0-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    11587 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/epl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    22965 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/gfdl-1.3.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    18094 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/gpl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    35151 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/gpl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      788 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/isc.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    25381 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/lgpl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    26528 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/lgpl-2.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7654 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/lgpl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1106 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1114 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/mit.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      260 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/ofl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      901 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/license/zlib.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1898 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      563 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/meson.build.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     1028 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/meson.options.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      313 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/mypy.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      391 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/mypy.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1296 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/new_child.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      498 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/ozi.wrap.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     2648 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/project.PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     1283 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/project.array.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      766 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/project.feature.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      689 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/project.integer.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     3684 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/project.meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/project.name/
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/project.name/__init__.py.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/project.name/__init__.pyi.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/project.name/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      900 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/project.name/meson.build.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      394 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/project.name/new_module.py.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      274 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/project.name/py.typed.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      129 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/project.ozi.wrap.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      396 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/pydocstyle.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/pylint.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      600 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/pyproject.toml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      376 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/pyright.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      390 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/pyright.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      537 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/pytest.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/pytest.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/requirements.in.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      374 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/restructuredtext-lint.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     1369 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/root.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1271 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/ruff.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1269 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/semantic_release.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      486 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/setuptools_scm.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      866 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/tests/meson.build.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/tests/new_test.py.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     1572 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/templates/tox.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/test/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/test/coverage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/test/coverage/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/test/coverage/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/test/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/test/pytest/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/test/pytest/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/test/pytest/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/trove.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/vendor/
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/vendor/__init__.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/vendor/email_validator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/vendor/email_validator/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/vendor/email_validator/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/vendor/email_validator/deliverability.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/vendor/email_validator/exceptions_types.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/vendor/email_validator/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/vendor/email_validator/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/vendor/email_validator/rfc_constants.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/vendor/email_validator/syntax.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/vendor/email_validator/validate_email.py
+-rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/vendor/email_validator/version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-04-27 00:18:52.000000 OZI-1.1.6/ozi/vendor/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    10639 2024-04-27 00:18:52.000000 OZI-1.1.6/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      170 2024-04-27 00:18:52.000000 OZI-1.1.6/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/subprojects/
+-rw-rw-r--   0 runner    (1001) docker     (127)      342 2024-04-27 00:18:52.000000 OZI-1.1.6/subprojects/blastpipe.wrap
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-04-27 00:18:52.000000 OZI-1.1.6/templates/CHANGELOG.md.j2
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:18:52.000000 OZI-1.1.6/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-04-27 00:18:52.000000 OZI-1.1.6/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    11059 2024-04-27 00:18:52.000000 OZI-1.1.6/tests/test_ozi_fix.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    14151 2024-04-27 00:18:52.000000 OZI-1.1.6/tests/test_ozi_new.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-04-27 00:18:52.000000 OZI-1.1.6/tests/test_tap.py
```

### Comparing `OZI-1.1.5/.github/CODEOWNERS` & `OZI-1.1.6/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/.github/CODE_OF_CONDUCT.md` & `OZI-1.1.6/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/.github/CONTRIBUTING.md` & `OZI-1.1.6/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/.github/ISSUE_TEMPLATE/bug_report.md` & `OZI-1.1.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/.github/ISSUE_TEMPLATE/feature_request.md` & `OZI-1.1.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/.github/SECURITY.md` & `OZI-1.1.6/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/.github/workflows/codeql.yml` & `OZI-1.1.6/.github/workflows/codeql.yml`

 * *Files 14% similar despite different names*

```diff
@@ -48,37 +48,37 @@
           allowed-endpoints: >
             api.github.com:443
             github.com:443
             objects.githubusercontent.com:443
             uploads.github.com:443
 
       - name: Checkout repository
-        uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f # v4.1.3
+        uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
 
       # Initializes the CodeQL tools for scanning.
       - name: Initialize CodeQL
-        uses: github/codeql-action/init@8f596b4ae3cb3c588a5c46780b86dd53fef16c52 # v3.25.2
+        uses: github/codeql-action/init@d39d31e687223d841ef683f52467bd88e9b21c14 # v3.25.3
         with:
           languages: ${{ matrix.language }}
           # If you wish to specify custom queries, you can do so here or in a config file.
           # By default, queries listed here will override any specified in a config file.
           # Prefix the list here with "+" to use these queries and those in the config file.
 
       # Autobuild attempts to build any compiled languages  (C/C++, C#, or Java).
       # If this step fails, then you should remove it and run the build manually (see below)
       - name: Autobuild
-        uses: github/codeql-action/autobuild@8f596b4ae3cb3c588a5c46780b86dd53fef16c52 # v3.25.2
+        uses: github/codeql-action/autobuild@d39d31e687223d841ef683f52467bd88e9b21c14 # v3.25.3
 
       # ℹ️ Command-line programs to run using the OS shell.
       # 📚 See https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#jobsjob_idstepsrun
 
       #   If the Autobuild fails above, remove it and uncomment the following three lines.
       #   modify them (or add more) to build your code if your project, please refer to the EXAMPLE below for guidance.
 
       # - run: |
       #   echo "Run, Build Application using script"
       #   ./location_of_script_within_repo/buildscript.sh
 
       - name: Perform CodeQL Analysis
-        uses: github/codeql-action/analyze@8f596b4ae3cb3c588a5c46780b86dd53fef16c52 # v3.25.2
+        uses: github/codeql-action/analyze@d39d31e687223d841ef683f52467bd88e9b21c14 # v3.25.3
         with:
           category: "/language:${{matrix.language}}"
```

### Comparing `OZI-1.1.5/.github/workflows/dependency-review.yml` & `OZI-1.1.6/.github/workflows/dependency-review.yml`

 * *Files 7% similar despite different names*

```diff
@@ -23,12 +23,12 @@
     steps:
       - name: Harden Runner
         uses: step-security/harden-runner@63c24ba6bd7ba022e95695ff85de572c04a18142 # v2.7.0
         with:
           egress-policy: audit
 
       - name: 'Checkout Repository'
-        uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f # v4.1.3
+        uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
       - name: 'Dependency Review'
         uses: actions/dependency-review-action@5bbc3ba658137598168acb2ab73b21c432dd411b # v4.2.5
         with:
           head-ref: main
```

### Comparing `OZI-1.1.5/.github/workflows/dev-workflow.yml` & `OZI-1.1.6/.github/workflows/dev-workflow.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/.github/workflows/dist-workflow.yml` & `OZI-1.1.6/.github/workflows/dist-workflow.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/.github/workflows/scorecard.yml` & `OZI-1.1.6/.github/workflows/scorecard.yml`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             github.com:443
             oss-fuzz-build-logs.storage.googleapis.com:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
             www.bestpractices.dev:443
 
       - name: "Checkout code"
-        uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f # v4.1.3
+        uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
         with:
           persist-credentials: false
 
       - name: "Run analysis"
         uses: ossf/scorecard-action@0864cf19026789058feabb7e87baa5f140aac736 # v2.3.1
         with:
           results_file: results.sarif
@@ -79,10 +79,10 @@
         with:
           name: SARIF file
           path: results.sarif
           retention-days: 5
 
       # Upload the results to GitHub's code scanning dashboard.
       - name: "Upload to code-scanning"
-        uses: github/codeql-action/upload-sarif@8f596b4ae3cb3c588a5c46780b86dd53fef16c52 # v3.25.2
+        uses: github/codeql-action/upload-sarif@d39d31e687223d841ef683f52467bd88e9b21c14 # v3.25.3
         with:
           sarif_file: results.sarif
```

### Comparing `OZI-1.1.5/.gitignore` & `OZI-1.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/CHANGELOG.md` & `OZI-1.1.6/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,62 @@
 # CHANGELOG
+## 1.1.6 (2024-04-27)
+
+### :alembic:
+
+* :alembic:(``ozi.render.load_environment``): Add globals dict argument.
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`eaac863`](https://github.com/OZI-Project/OZI/commit/eaac8633e08b2f345333e4a4bfdf0b350ce7966d))
+
+### :arrow_up:
+
+* :arrow_up: Bump github/codeql-action from 3.25.2 to 3.25.3
+
+Bumps [github/codeql-action](https://github.com/github/codeql-action) from 3.25.2 to 3.25.3.
+- [Release notes](https://github.com/github/codeql-action/releases)
+- [Changelog](https://github.com/github/codeql-action/blob/main/CHANGELOG.md)
+- [Commits](https://github.com/github/codeql-action/compare/8f596b4ae3cb3c588a5c46780b86dd53fef16c52...d39d31e687223d841ef683f52467bd88e9b21c14)
+
+---
+updated-dependencies:
+- dependency-name: github/codeql-action
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`e7888b0`](https://github.com/OZI-Project/OZI/commit/e7888b059f9223008680a7d9dfd28e01a07205ba))
+
+* :arrow_up: Bump actions/checkout from 4.1.3 to 4.1.4
+
+Bumps [actions/checkout](https://github.com/actions/checkout) from 4.1.3 to 4.1.4.
+- [Release notes](https://github.com/actions/checkout/releases)
+- [Changelog](https://github.com/actions/checkout/blob/main/CHANGELOG.md)
+- [Commits](https://github.com/actions/checkout/compare/1d96c772d19495a3b5c517cd2bc0cb401ea0529f...0ad4b8fadaa221de15dcec353f45205ec38ea70b)
+
+---
+updated-dependencies:
+- dependency-name: actions/checkout
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`41251c9`](https://github.com/OZI-Project/OZI/commit/41251c94d744593a3931d1d5acd70ac18f2838e5))
+
+### :bug:
+
+* :bug: exclude double quotes from fuzzer input.
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`361a75a`](https://github.com/OZI-Project/OZI/commit/361a75a9e1b63dc6ad12b24cf85f9762a213c8a7))
+
+### Other
+
+* :rotating_light: run ``black -S tests``
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`fdd8fe2`](https://github.com/OZI-Project/OZI/commit/fdd8fe2fdbe6b7941972efc33aa77ee1707dae5a))
+
 ## 1.1.5 (2024-04-24)
 
 ### :arrow_up:
 
 * :arrow_up: Bump release to 0.1.17
 
 Signed-off-by: Eden Rose, MSc &lt;ozi.project@outlook.com&gt; ([`eca9b71`](https://github.com/OZI-Project/OZI/commit/eca9b713ea773157c3912eca2fb4d87ff38d0ef5))
```

### Comparing `OZI-1.1.5/LICENSE.txt` & `OZI-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/PKG-INFO` & `OZI-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: OZI
-Version: 1.1.5
+Version: 1.1.6
 Summary: Packager for Python projects using Meson.
-Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.1.5.tar.gz
+Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.1.6.tar.gz
 Home-page: https://oziproject.dev/
 Author: Eden Rose Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
 Keywords: meson,packaging,wheel
 Project-URL: Bug Tracker, https://github.com/rjdbcm/ozi/issues
 Project-URL: Community, https://github.com/orgs/OZI-Project/discussions
```

### Comparing `OZI-1.1.5/README.rst` & `OZI-1.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/meson.build` & `OZI-1.1.6/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/meson.options` & `OZI-1.1.6/meson.options`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/__main__.py` & `OZI-1.1.6/ozi/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/actions.py` & `OZI-1.1.6/ozi/actions.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/comment.py` & `OZI-1.1.6/ozi/comment.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/filter.py` & `OZI-1.1.6/ozi/filter.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/fix/__main__.py` & `OZI-1.1.6/ozi/fix/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from typing import NoReturn
 
 from ozi.filter import underscorify
 from ozi.fix.missing import report
 from ozi.fix.parser import parser
 from ozi.fix.rewrite_command import Rewriter
 from ozi.render import load_environment
+from ozi.spec import METADATA
 from ozi.tap import TAP
 
 
 def main() -> NoReturn:  # pragma: no cover
     """Main ozi.fix entrypoint."""
     project = parser.parse_args()
     project.missing = project.fix == 'missing' or project.fix == 'm'
@@ -27,15 +28,15 @@
         TAP.bail_out(f'target: {project.target} does not exist.')
     elif not project.target.is_dir():
         TAP.bail_out(f'target: {project.target} is not a directory.')
     project.add.remove('ozi.phony')
     project.add = list(set(project.add))
     project.remove.remove('ozi.phony')
     project.remove = list(set(project.remove))
-    env = load_environment(vars(project))
+    env = load_environment(vars(project), METADATA.asdict())
 
     match [project.missing, project.strict]:
         case [True, False]:
             name, *_ = report(project.target)
             TAP.end()
         case [False, _]:
             with TAP.suppress():
```

### Comparing `OZI-1.1.5/ozi/fix/build_definition.py` & `OZI-1.1.6/ozi/fix/build_definition.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/fix/meson.build` & `OZI-1.1.6/ozi/fix/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/fix/missing.py` & `OZI-1.1.6/ozi/fix/missing.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/fix/parser.py` & `OZI-1.1.6/ozi/fix/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/fix/rewrite_command.py` & `OZI-1.1.6/ozi/fix/rewrite_command.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/lint/meson.build` & `OZI-1.1.6/ozi/lint/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/lint/pyright/meson.build` & `OZI-1.1.6/ozi/lint/pyright/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/meson.build` & `OZI-1.1.6/ozi/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/meson.py` & `OZI-1.1.6/ozi/meson.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/new/__main__.py` & `OZI-1.1.6/ozi/new/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 import re
 import shlex
 import sys
 from pathlib import Path
 from typing import TYPE_CHECKING
 
+from ozi.spec import METADATA
+
 if TYPE_CHECKING:
     from argparse import Namespace
     from typing import Callable
     from typing import TypeAlias
 
     from jinja2 import Environment
 
@@ -107,21 +109,21 @@
 
 
 def project(project: Namespace) -> None:
     """Create a new project in a target directory."""
     project = postprocess_arguments(preprocess_arguments(project))
     create_project_files(
         project=project,
-        env=load_environment(vars(project)),
+        env=load_environment(vars(project), METADATA.asdict()),
     )
 
 
 def wrap(project: Namespace) -> None:  # pragma: no cover
     """Create a new wrap file for publishing. Not a public function."""
-    env = load_environment(vars(project))
+    env = load_environment(vars(project), METADATA.asdict())
     template = env.get_template('ozi.wrap.j2')
     with open('ozi.wrap', 'w') as f:
         f.write(template.render())
 
 
 def main() -> None:  # pragma: no cover
     """Main ozi.new entrypoint."""
```

### Comparing `OZI-1.1.5/ozi/new/meson.build` & `OZI-1.1.6/ozi/new/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/new/parser.py` & `OZI-1.1.6/ozi/new/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/new/validate.py` & `OZI-1.1.6/ozi/new/validate.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/pkg_extra.py` & `OZI-1.1.6/ozi/pkg_extra.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/render.py` & `OZI-1.1.6/ozi/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # ozi/render.py
 # Part of the OZI Project, under the Apache License v2.0 with LLVM Exceptions.
 # See LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 """Rendering utilities for the OZI project templates."""
 from functools import _lru_cache_wrapper
-from functools import lru_cache
 from pathlib import Path
 from types import FunctionType
+from typing import Any
 from warnings import warn
 
 from git import InvalidGitRepositoryError
 from git import Repo
 from jinja2 import Environment
 from jinja2 import PackageLoader
 from jinja2 import TemplateNotFound
@@ -32,16 +32,15 @@
     zip,
     sha256sum,
     wheel_repr,
     current_date,
 )
 
 
-@lru_cache
-def _init_environment() -> Environment:
+def _init_environment(_globals: dict[str, Any]) -> Environment:
     """Initialize the rendering environment, set filters, and set global metadata."""
     env = Environment(
         loader=PackageLoader('ozi'),
         autoescape=select_autoescape(),
         enable_async=True,
         auto_reload=False,
     )
@@ -49,25 +48,25 @@
         match f:
             case type():
                 env.filters.setdefault(f.__name__, f)
             case FunctionType():
                 env.filters.setdefault(f.__name__, f)
             case _lru_cache_wrapper():  # pragma: defer to pyright,mypy
                 env.filters.setdefault(f.__wrapped__.__name__, f)
-    env.globals = env.globals | METADATA.asdict()
+    env.globals = env.globals | _globals
     return env
 
 
-def load_environment(project: dict[str, str]) -> Environment:
+def load_environment(project: dict[str, str], _globals: dict[str, Any]) -> Environment:
     """Load the rendering environment for templates.
 
     :return: jinja2 rendering environment for OZI
     :rtype: Environment
     """
-    env = _init_environment()
+    env = _init_environment(_globals)
     env.globals = env.globals | {'project': project}
     return env
 
 
 def find_user_template(target: str, file: str, fix: str) -> str | None:
     """Find a user-defined project template file e.g. :file:`{target}/templates/{fix}/{file}`.
```

### Comparing `OZI-1.1.5/ozi/scripts/core_metadata_template.py` & `OZI-1.1.6/ozi/scripts/core_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/scripts/meson.build` & `OZI-1.1.6/ozi/scripts/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/scripts/meson_dist_setuptools_scm.py` & `OZI-1.1.6/ozi/scripts/meson_dist_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/scripts/meson_setuptools_scm.py` & `OZI-1.1.6/ozi/scripts/meson_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/scripts/render_requirements.py` & `OZI-1.1.6/ozi/scripts/render_requirements.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/scripts/replace_ruff_target_version.py` & `OZI-1.1.6/ozi/scripts/replace_ruff_target_version.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/scripts/scm_version_snip.py` & `OZI-1.1.6/ozi/scripts/scm_version_snip.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/scripts/to_distribution_template.py` & `OZI-1.1.6/ozi/scripts/to_distribution_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/scripts/version_metadata_template.py` & `OZI-1.1.6/ozi/scripts/version_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/spdx.py` & `OZI-1.1.6/ozi/spdx.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/spec/_license.py` & `OZI-1.1.6/ozi/spec/_license.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/spec/_spec.py` & `OZI-1.1.6/ozi/spec/_spec.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/spec/base.py` & `OZI-1.1.6/ozi/spec/base.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/spec/ci.py` & `OZI-1.1.6/ozi/spec/ci.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/spec/meson.build` & `OZI-1.1.6/ozi/spec/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/spec/pkg.py` & `OZI-1.1.6/ozi/spec/pkg.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/spec/project.py` & `OZI-1.1.6/ozi/spec/project.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/spec/python.py` & `OZI-1.1.6/ozi/spec/python.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/spec/src.py` & `OZI-1.1.6/ozi/spec/src.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/tap.py` & `OZI-1.1.6/ozi/tap.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/README.rst.j2` & `OZI-1.1.6/ozi/templates/README.rst.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/coverage.pyproject.toml` & `OZI-1.1.6/ozi/templates/coverage.pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/flake8.meson.options` & `OZI-1.1.6/ozi/templates/flake8.meson.options`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/flake8.pyproject.toml` & `OZI-1.1.6/ozi/templates/flake8.pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/github_workflows/checkpoint.yml.j2` & `OZI-1.1.6/ozi/templates/github_workflows/checkpoint.yml.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/github_workflows/generate_provenance.yml.j2` & `OZI-1.1.6/ozi/templates/github_workflows/generate_provenance.yml.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/github_workflows/meson.build` & `OZI-1.1.6/ozi/templates/github_workflows/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/github_workflows/ozi.yml.j2` & `OZI-1.1.6/ozi/templates/github_workflows/ozi.yml.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/github_workflows/publish.yml.j2` & `OZI-1.1.6/ozi/templates/github_workflows/publish.yml.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/github_workflows/release.yml.j2` & `OZI-1.1.6/ozi/templates/github_workflows/release.yml.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/DFSG_approved/cc-by-4.0.txt` & `OZI-1.1.6/ozi/templates/license/DFSG_approved/cc-by-4.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/DFSG_approved/cc-by-sa-4.0.txt` & `OZI-1.1.6/ozi/templates/license/DFSG_approved/cc-by-sa-4.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/DFSG_approved/meson.build` & `OZI-1.1.6/ozi/templates/license/DFSG_approved/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt` & `OZI-1.1.6/ozi/templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/Free_To_Use_But_Restricted/ncsa.txt` & `OZI-1.1.6/ozi/templates/license/Free_To_Use_But_Restricted/ncsa.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/BSD_License/0bsd.txt` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/BSD_License/0bsd.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/BSD_License/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/BSD_License/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/OSI_Approved/zlib_libpng_License/meson.build` & `OZI-1.1.6/ozi/templates/license/OSI_Approved/zlib_libpng_License/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/Public_Domain/meson.build` & `OZI-1.1.6/ozi/templates/license/Public_Domain/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/Public_Domain/unlicense.txt` & `OZI-1.1.6/ozi/templates/license/Public_Domain/unlicense.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/agpl-3.0.txt` & `OZI-1.1.6/ozi/templates/license/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/apache-2.0.txt` & `OZI-1.1.6/ozi/templates/license/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/artistic-2.0.txt` & `OZI-1.1.6/ozi/templates/license/artistic-2.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/bsd-3-clause.txt` & `OZI-1.1.6/ozi/templates/license/bsd-3-clause.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/cc0-1.0.txt` & `OZI-1.1.6/ozi/templates/license/cc0-1.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/epl-1.0.txt` & `OZI-1.1.6/ozi/templates/license/epl-1.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/gfdl-1.3.txt` & `OZI-1.1.6/ozi/templates/license/gfdl-1.3.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/gpl-2.0.txt` & `OZI-1.1.6/ozi/templates/license/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/gpl-3.0.txt` & `OZI-1.1.6/ozi/templates/license/gpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/isc.txt` & `OZI-1.1.6/ozi/templates/license/isc.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/lgpl-2.0.txt` & `OZI-1.1.6/ozi/templates/license/lgpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/lgpl-2.1.txt` & `OZI-1.1.6/ozi/templates/license/lgpl-2.1.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/lgpl-3.0.txt` & `OZI-1.1.6/ozi/templates/license/lgpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/meson.build` & `OZI-1.1.6/ozi/templates/license/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/mit.txt` & `OZI-1.1.6/ozi/templates/license/mit.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/license/zlib.txt` & `OZI-1.1.6/ozi/templates/license/zlib.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/meson.build` & `OZI-1.1.6/ozi/templates/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/meson.build.j2` & `OZI-1.1.6/ozi/templates/meson.build.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/meson.options.j2` & `OZI-1.1.6/ozi/templates/meson.options.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/new_child.j2` & `OZI-1.1.6/ozi/templates/new_child.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/project.PKG-INFO` & `OZI-1.1.6/ozi/templates/project.PKG-INFO`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/project.array.meson.options` & `OZI-1.1.6/ozi/templates/project.array.meson.options`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/project.feature.meson.options` & `OZI-1.1.6/ozi/templates/project.feature.meson.options`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/project.integer.meson.options` & `OZI-1.1.6/ozi/templates/project.integer.meson.options`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/project.meson.build` & `OZI-1.1.6/ozi/templates/project.meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/project.name/meson.build` & `OZI-1.1.6/ozi/templates/project.name/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/project.name/meson.build.j2` & `OZI-1.1.6/ozi/templates/project.name/meson.build.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/pyproject.toml.j2` & `OZI-1.1.6/ozi/templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/pytest.meson.options` & `OZI-1.1.6/ozi/templates/pytest.meson.options`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/pytest.pyproject.toml` & `OZI-1.1.6/ozi/templates/pytest.pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/root.pyproject.toml` & `OZI-1.1.6/ozi/templates/root.pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/ruff.pyproject.toml` & `OZI-1.1.6/ozi/templates/ruff.pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/semantic_release.pyproject.toml` & `OZI-1.1.6/ozi/templates/semantic_release.pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/tests/meson.build.j2` & `OZI-1.1.6/ozi/templates/tests/meson.build.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/templates/tox.pyproject.toml` & `OZI-1.1.6/ozi/templates/tox.pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/trove.py` & `OZI-1.1.6/ozi/trove.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/vendor/email_validator/__init__.py` & `OZI-1.1.6/ozi/vendor/email_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/vendor/email_validator/__main__.py` & `OZI-1.1.6/ozi/vendor/email_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/vendor/email_validator/deliverability.py` & `OZI-1.1.6/ozi/vendor/email_validator/deliverability.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/vendor/email_validator/exceptions_types.py` & `OZI-1.1.6/ozi/vendor/email_validator/exceptions_types.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/vendor/email_validator/meson.build` & `OZI-1.1.6/ozi/vendor/email_validator/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/vendor/email_validator/rfc_constants.py` & `OZI-1.1.6/ozi/vendor/email_validator/rfc_constants.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/vendor/email_validator/syntax.py` & `OZI-1.1.6/ozi/vendor/email_validator/syntax.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/vendor/email_validator/validate_email.py` & `OZI-1.1.6/ozi/vendor/email_validator/validate_email.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/ozi/vendor/meson.build` & `OZI-1.1.6/ozi/vendor/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/pyproject.toml` & `OZI-1.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/templates/CHANGELOG.md.j2` & `OZI-1.1.6/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/tests/meson.build` & `OZI-1.1.6/tests/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.5/tests/test_ozi_fix.py` & `OZI-1.1.6/tests/test_ozi_fix.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     add=['ozi.phony'],
     remove=['ozi.phony'],
     dist_requires=[],
     allow_file=[],
     missing=True,
 )
 
-env = load_environment(vars(bad_namespace))
+env = load_environment(vars(bad_namespace), METADATA.asdict())
 
 
 @pytest.fixture
 def bad_project(tmp_path_factory: pytest.TempPathFactory) -> pathlib.Path:
     """Fixture to wrap the ``ozi-new project`` functionality."""
     fn = tmp_path_factory.mktemp('project_')
     namespace = deepcopy(bad_namespace)
```

### Comparing `OZI-1.1.5/tests/test_ozi_new.py` & `OZI-1.1.6/tests/test_ozi_new.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,42 +36,53 @@
             'keywords': st.from_regex(r'^(([a-z_]*[a-z0-9],)*){2,650}$', fullmatch=True),
             'ci_provider': st.just('github'),
             'name': st.from_regex(
                 r'^([A-Za-z]|[A-Za-z][A-Za-z0-9._-]*[A-Za-z0-9]){1,80}$',
                 fullmatch=True,
             ),
             'author': st.lists(
-                st.text(st.characters(exclude_categories=['C']), min_size=1, max_size=16),
+                st.text(
+                    st.characters(exclude_categories=['C'], exclude_characters='\\"'),
+                    min_size=1,
+                    max_size=16,
+                ),
                 min_size=1,
                 max_size=8,
                 unique=True,
             ),
             'author_email': st.lists(
                 st.emails(domains=st.just('phony1.oziproject.dev')),
                 min_size=1,
                 max_size=8,
             ),
             'maintainer': st.lists(
-                st.text(st.characters(exclude_categories=['C']), min_size=1, max_size=16),
+                st.text(
+                    st.characters(exclude_categories=['C'], exclude_characters='\\"'),
+                    min_size=1,
+                    max_size=16,
+                ),
                 min_size=1,
                 max_size=8,
                 unique=True,
             ),
             'maintainer_email': st.lists(
                 st.emails(domains=st.just('phony2.oziproject.dev')),
                 max_size=8,
             ),
             'home_page': st.one_of(st.just('https://oziproject.dev/')),
             'project_url': st.lists(
                 st.just('A, https://oziproject.dev'),
                 max_size=1,
             ),
-            'summary': st.text(st.characters(exclude_categories=['C']), max_size=255),
+            'summary': st.text(
+                st.characters(exclude_categories=['C'], exclude_characters='\\"'),
+                max_size=255,
+            ),
             'copyright_head': st.text(
-                st.characters(exclude_categories=['C']),
+                st.characters(exclude_categories=['C'], exclude_characters='\\"'),
                 max_size=255,
             ),
             'license_file': st.just('LICENSE.txt'),
             'license_exception_id': st.one_of(
                 list(map(st.just, ozi.actions.ExactMatch().license_exception_id)),  # type: ignore
             ),
             'topic': st.lists(st.sampled_from(list(map(st.just, ozi.actions.ExactMatch().topic)))),  # type: ignore
@@ -118,15 +129,15 @@
     )
     project['license_expression'] = license_expression.draw(st.just(project['license_id']))
     namespace = argparse.Namespace(**project)
     preprocessed = ozi.new.__main__.preprocess_arguments(namespace)
     postprocessed = ozi.new.__main__.postprocess_arguments(preprocessed)
     ozi.new.__main__.create_project_files(
         postprocessed,
-        env=load_environment(vars(postprocessed)),
+        env=load_environment(vars(postprocessed), METADATA.asdict()),
     )
     name, _ = required_pkg_info(postprocessed.target)
     required_files('root', postprocessed.target, postprocessed.name)
     required_files('test', postprocessed.target, postprocessed.name)
     required_files(
         'source',
         postprocessed.target,
```

### Comparing `OZI-1.1.5/tests/test_tap.py` & `OZI-1.1.6/tests/test_tap.py`

 * *Files identical despite different names*

