# Comparing `tmp/jax-relax-0.2.6.tar.gz` & `tmp/jax-relax-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-relax-0.2.6.tar", last modified: Thu Apr  4 15:25:57 2024, max compression
+gzip compressed data, was "jax-relax-0.2.7.tar", last modified: Sat Apr 27 19:15:13 2024, max compression
```

## Comparing `jax-relax-0.2.6.tar` & `jax-relax-0.2.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2024-04-04 15:25:57.171337 jax-relax-0.2.6/
--rw-r--r--   0 birk      (1000) birk      (1000)     2381 2023-09-10 14:18:49.000000 jax-relax-0.2.6/CONTRIBUTING.md
--rw-r--r--   0 birk      (1000) birk      (1000)    11538 2023-09-10 14:18:49.000000 jax-relax-0.2.6/LICENSE
--rw-r--r--   0 birk      (1000) birk      (1000)      116 2023-09-10 14:18:49.000000 jax-relax-0.2.6/MANIFEST.in
--rw-r--r--   0 birk      (1000) birk      (1000)     8880 2024-04-04 15:25:57.171337 jax-relax-0.2.6/PKG-INFO
--rw-r--r--   0 birk      (1000) birk      (1000)     8099 2024-01-16 16:50:43.000000 jax-relax-0.2.6/README.md
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2024-04-04 15:25:57.171337 jax-relax-0.2.6/jax_relax.egg-info/
--rw-r--r--   0 birk      (1000) birk      (1000)     8880 2024-04-04 15:25:57.000000 jax-relax-0.2.6/jax_relax.egg-info/PKG-INFO
--rw-r--r--   0 birk      (1000) birk      (1000)     1059 2024-04-04 15:25:57.000000 jax-relax-0.2.6/jax_relax.egg-info/SOURCES.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        1 2024-04-04 15:25:57.000000 jax-relax-0.2.6/jax_relax.egg-info/dependency_links.txt
--rw-r--r--   0 birk      (1000) birk      (1000)       32 2024-04-04 15:25:57.000000 jax-relax-0.2.6/jax_relax.egg-info/entry_points.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-09-10 15:15:42.000000 jax-relax-0.2.6/jax_relax.egg-info/not-zip-safe
--rw-r--r--   0 birk      (1000) birk      (1000)      199 2024-04-04 15:25:57.000000 jax-relax-0.2.6/jax_relax.egg-info/requires.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        6 2024-04-04 15:25:57.000000 jax-relax-0.2.6/jax_relax.egg-info/top_level.txt
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2024-04-04 15:25:57.171337 jax-relax-0.2.6/relax/
--rw-r--r--   0 birk      (1000) birk      (1000)      301 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)   115942 2024-04-04 15:15:48.000000 jax-relax-0.2.6/relax/_modidx.py
--rw-r--r--   0 birk      (1000) birk      (1000)     2110 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/base.py
--rw-r--r--   0 birk      (1000) birk      (1000)    19574 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/data_module.py
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2024-04-04 15:25:57.171337 jax-relax-0.2.6/relax/data_utils/
--rw-r--r--   0 birk      (1000) birk      (1000)       82 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/data_utils/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)    12617 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/data_utils/features.py
--rw-r--r--   0 birk      (1000) birk      (1000)     5140 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/data_utils/preprocessing.py
--rw-r--r--   0 birk      (1000) birk      (1000)     6755 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/data_utils/transforms.py
--rw-r--r--   0 birk      (1000) birk      (1000)     7257 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/docs.py
--rw-r--r--   0 birk      (1000) birk      (1000)     9513 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/evaluate.py
--rw-r--r--   0 birk      (1000) birk      (1000)     9500 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/explain.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1435 2023-11-28 15:29:08.000000 jax-relax-0.2.6/relax/import_essentials.py
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2024-04-04 15:25:57.171337 jax-relax-0.2.6/relax/legacy/
--rw-r--r--   0 birk      (1000) birk      (1000)        0 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/legacy/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)     3895 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/legacy/ckpt_manager.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1425 2023-11-28 15:29:08.000000 jax-relax-0.2.6/relax/legacy/import_essentials.py
--rw-r--r--   0 birk      (1000) birk      (1000)     2121 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/legacy/logger.py
--rw-r--r--   0 birk      (1000) birk      (1000)     8054 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/legacy/module.py
--rw-r--r--   0 birk      (1000) birk      (1000)     5358 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/legacy/trainer.py
--rw-r--r--   0 birk      (1000) birk      (1000)     5883 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/legacy/utils.py
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2024-04-04 15:25:57.171337 jax-relax-0.2.6/relax/methods/
--rw-r--r--   0 birk      (1000) birk      (1000)      435 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)     2640 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/base.py
--rw-r--r--   0 birk      (1000) birk      (1000)     9283 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/cchvae.py
--rw-r--r--   0 birk      (1000) birk      (1000)    10667 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/clue.py
--rw-r--r--   0 birk      (1000) birk      (1000)    12317 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/counternet.py
--rw-r--r--   0 birk      (1000) birk      (1000)     5585 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/dice.py
--rw-r--r--   0 birk      (1000) birk      (1000)    15559 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/l2c.py
--rw-r--r--   0 birk      (1000) birk      (1000)     7013 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/proto.py
--rw-r--r--   0 birk      (1000) birk      (1000)    12201 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/sphere.py
--rw-r--r--   0 birk      (1000) birk      (1000)     9542 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/vaecf.py
--rw-r--r--   0 birk      (1000) birk      (1000)     4096 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/vanilla.py
--rw-r--r--   0 birk      (1000) birk      (1000)     7822 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/ml_model.py
--rw-r--r--   0 birk      (1000) birk      (1000)     8089 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/strategy.py
--rw-r--r--   0 birk      (1000) birk      (1000)     6600 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/utils.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1162 2024-04-03 13:49:44.000000 jax-relax-0.2.6/settings.ini
--rw-r--r--   0 birk      (1000) birk      (1000)       38 2024-04-04 15:25:57.171337 jax-relax-0.2.6/setup.cfg
--rw-r--r--   0 birk      (1000) birk      (1000)     2658 2023-11-26 18:26:06.000000 jax-relax-0.2.6/setup.py
+drwxr-xr-x   0 birk       (501) staff       (20)        0 2024-04-27 19:15:13.905958 jax-relax-0.2.7/
+-rw-r--r--   0 birk       (501) staff       (20)     2348 2024-04-01 17:06:03.000000 jax-relax-0.2.7/CONTRIBUTING.md
+-rw-r--r--   0 birk       (501) staff       (20)    11337 2024-04-01 17:06:03.000000 jax-relax-0.2.7/LICENSE
+-rw-r--r--   0 birk       (501) staff       (20)      111 2024-04-01 17:06:03.000000 jax-relax-0.2.7/MANIFEST.in
+-rw-r--r--   0 birk       (501) staff       (20)     8880 2024-04-27 19:15:13.905697 jax-relax-0.2.7/PKG-INFO
+-rw-r--r--   0 birk       (501) staff       (20)     8099 2024-04-01 17:06:03.000000 jax-relax-0.2.7/README.md
+drwxr-xr-x   0 birk       (501) staff       (20)        0 2024-04-27 19:15:13.899983 jax-relax-0.2.7/jax_relax.egg-info/
+-rw-r--r--   0 birk       (501) staff       (20)     8880 2024-04-27 19:15:13.000000 jax-relax-0.2.7/jax_relax.egg-info/PKG-INFO
+-rw-r--r--   0 birk       (501) staff       (20)     1059 2024-04-27 19:15:13.000000 jax-relax-0.2.7/jax_relax.egg-info/SOURCES.txt
+-rw-r--r--   0 birk       (501) staff       (20)        1 2024-04-27 19:15:13.000000 jax-relax-0.2.7/jax_relax.egg-info/dependency_links.txt
+-rw-r--r--   0 birk       (501) staff       (20)       32 2024-04-27 19:15:13.000000 jax-relax-0.2.7/jax_relax.egg-info/entry_points.txt
+-rw-r--r--   0 birk       (501) staff       (20)        1 2024-04-27 19:15:03.000000 jax-relax-0.2.7/jax_relax.egg-info/not-zip-safe
+-rw-r--r--   0 birk       (501) staff       (20)      199 2024-04-27 19:15:13.000000 jax-relax-0.2.7/jax_relax.egg-info/requires.txt
+-rw-r--r--   0 birk       (501) staff       (20)        6 2024-04-27 19:15:13.000000 jax-relax-0.2.7/jax_relax.egg-info/top_level.txt
+drwxr-xr-x   0 birk       (501) staff       (20)        0 2024-04-27 19:15:13.901790 jax-relax-0.2.7/relax/
+-rw-r--r--   0 birk       (501) staff       (20)      301 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/__init__.py
+-rw-r--r--   0 birk       (501) staff       (20)   115942 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/_modidx.py
+-rw-r--r--   0 birk       (501) staff       (20)     2110 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/base.py
+-rw-r--r--   0 birk       (501) staff       (20)    19574 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/data_module.py
+drwxr-xr-x   0 birk       (501) staff       (20)        0 2024-04-27 19:15:13.902484 jax-relax-0.2.7/relax/data_utils/
+-rw-r--r--   0 birk       (501) staff       (20)       79 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/data_utils/__init__.py
+-rw-r--r--   0 birk       (501) staff       (20)    12617 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/data_utils/features.py
+-rw-r--r--   0 birk       (501) staff       (20)     5140 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/data_utils/preprocessing.py
+-rw-r--r--   0 birk       (501) staff       (20)     6755 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/data_utils/transforms.py
+-rw-r--r--   0 birk       (501) staff       (20)     7257 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/docs.py
+-rw-r--r--   0 birk       (501) staff       (20)     9513 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/evaluate.py
+-rw-r--r--   0 birk       (501) staff       (20)     9500 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/explain.py
+-rw-r--r--   0 birk       (501) staff       (20)     1394 2024-04-01 17:06:03.000000 jax-relax-0.2.7/relax/import_essentials.py
+drwxr-xr-x   0 birk       (501) staff       (20)        0 2024-04-27 19:15:13.903554 jax-relax-0.2.7/relax/legacy/
+-rw-r--r--   0 birk       (501) staff       (20)        0 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/legacy/__init__.py
+-rw-r--r--   0 birk       (501) staff       (20)     3895 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/legacy/ckpt_manager.py
+-rw-r--r--   0 birk       (501) staff       (20)     1384 2024-04-01 17:06:03.000000 jax-relax-0.2.7/relax/legacy/import_essentials.py
+-rw-r--r--   0 birk       (501) staff       (20)     2121 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/legacy/logger.py
+-rw-r--r--   0 birk       (501) staff       (20)     8054 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/legacy/module.py
+-rw-r--r--   0 birk       (501) staff       (20)     5358 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/legacy/trainer.py
+-rw-r--r--   0 birk       (501) staff       (20)     5883 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/legacy/utils.py
+drwxr-xr-x   0 birk       (501) staff       (20)        0 2024-04-27 19:15:13.905502 jax-relax-0.2.7/relax/methods/
+-rw-r--r--   0 birk       (501) staff       (20)      425 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/methods/__init__.py
+-rw-r--r--   0 birk       (501) staff       (20)     2640 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/methods/base.py
+-rw-r--r--   0 birk       (501) staff       (20)     9283 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/methods/cchvae.py
+-rw-r--r--   0 birk       (501) staff       (20)    10667 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/methods/clue.py
+-rw-r--r--   0 birk       (501) staff       (20)    12317 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/methods/counternet.py
+-rw-r--r--   0 birk       (501) staff       (20)     5585 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/methods/dice.py
+-rw-r--r--   0 birk       (501) staff       (20)    15559 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/methods/l2c.py
+-rw-r--r--   0 birk       (501) staff       (20)     7013 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/methods/proto.py
+-rw-r--r--   0 birk       (501) staff       (20)    12203 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/methods/sphere.py
+-rw-r--r--   0 birk       (501) staff       (20)     9542 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/methods/vaecf.py
+-rw-r--r--   0 birk       (501) staff       (20)     4096 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/methods/vanilla.py
+-rw-r--r--   0 birk       (501) staff       (20)     7822 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/ml_model.py
+-rw-r--r--   0 birk       (501) staff       (20)     8089 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/strategy.py
+-rw-r--r--   0 birk       (501) staff       (20)     6600 2024-04-27 19:08:00.000000 jax-relax-0.2.7/relax/utils.py
+-rw-r--r--   0 birk       (501) staff       (20)     1124 2024-04-27 18:47:15.000000 jax-relax-0.2.7/settings.ini
+-rw-r--r--   0 birk       (501) staff       (20)       38 2024-04-27 19:15:13.906003 jax-relax-0.2.7/setup.cfg
+-rw-r--r--   0 birk       (501) staff       (20)     2601 2024-04-01 17:06:03.000000 jax-relax-0.2.7/setup.py
```

### Comparing `jax-relax-0.2.6/CONTRIBUTING.md` & `jax-relax-0.2.7/CONTRIBUTING.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# How to contribute
-
-## How to get started
-
-Before anything else, please install the git hooks that run automatic scripts during each commit and merge to strip the notebooks of superfluous metadata (and avoid merge conflicts). After cloning the repository, run the following command inside it:
-```
-nbdev_install_git_hooks
-```
-
-## Did you find a bug?
-
-* Ensure the bug was not already reported by searching on GitHub under Issues.
-* If you're unable to find an open issue addressing the problem, open a new one. Be sure to include a title and clear description, as much relevant information as possible, and a code sample or an executable test case demonstrating the expected behavior that is not occurring.
-* Be sure to add the complete error messages.
-
-#### Did you write a patch that fixes a bug?
-
-* Open a new GitHub pull request with the patch.
-* Ensure that your PR includes a test that fails without your patch, and pass with it.
-* Ensure the PR description clearly describes the problem and solution. Include the relevant issue number if applicable.
-
-## PR submission guidelines
-
-* Keep each PR focused. While it's more convenient, do not combine several unrelated fixes together. Create as many branches as needing to keep each PR focused.
-* Do not mix style changes/fixes with "functional" changes. It's very difficult to review such PRs and it most likely get rejected.
-* Do not add/remove vertical whitespace. Preserve the original style of the file you edit as much as you can.
-* Do not turn an already submitted PR into your development playground. If after you submitted PR, you discovered that more work is needed - close the PR, do the required work and then submit a new PR. Otherwise each of your commits requires attention from maintainers of the project.
-* If, however, you submitted a PR and received a request for changes, you should proceed with commits inside that PR, so that the maintainer can see the incremental fixes and won't need to review the whole PR again. In the exception case where you realize it'll take many many commits to complete the requests, then it's probably best to close the PR, do the work and then submit it again. Use common sense where you'd choose one way over another.
-
-## Do you want to contribute to the documentation?
-
-* Docs are automatically created from the notebooks in the nbs folder.
-
+# How to contribute
+
+## How to get started
+
+Before anything else, please install the git hooks that run automatic scripts during each commit and merge to strip the notebooks of superfluous metadata (and avoid merge conflicts). After cloning the repository, run the following command inside it:
+```
+nbdev_install_git_hooks
+```
+
+## Did you find a bug?
+
+* Ensure the bug was not already reported by searching on GitHub under Issues.
+* If you're unable to find an open issue addressing the problem, open a new one. Be sure to include a title and clear description, as much relevant information as possible, and a code sample or an executable test case demonstrating the expected behavior that is not occurring.
+* Be sure to add the complete error messages.
+
+#### Did you write a patch that fixes a bug?
+
+* Open a new GitHub pull request with the patch.
+* Ensure that your PR includes a test that fails without your patch, and pass with it.
+* Ensure the PR description clearly describes the problem and solution. Include the relevant issue number if applicable.
+
+## PR submission guidelines
+
+* Keep each PR focused. While it's more convenient, do not combine several unrelated fixes together. Create as many branches as needing to keep each PR focused.
+* Do not mix style changes/fixes with "functional" changes. It's very difficult to review such PRs and it most likely get rejected.
+* Do not add/remove vertical whitespace. Preserve the original style of the file you edit as much as you can.
+* Do not turn an already submitted PR into your development playground. If after you submitted PR, you discovered that more work is needed - close the PR, do the required work and then submit a new PR. Otherwise each of your commits requires attention from maintainers of the project.
+* If, however, you submitted a PR and received a request for changes, you should proceed with commits inside that PR, so that the maintainer can see the incremental fixes and won't need to review the whole PR again. In the exception case where you realize it'll take many many commits to complete the requests, then it's probably best to close the PR, do the work and then submit it again. Use common sense where you'd choose one way over another.
+
+## Do you want to contribute to the documentation?
+
+* Docs are automatically created from the notebooks in the nbs folder.
+
```

### Comparing `jax-relax-0.2.6/LICENSE` & `jax-relax-0.2.7/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2022, fastai
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2022, fastai
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `jax-relax-0.2.6/PKG-INFO` & `jax-relax-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-relax
-Version: 0.2.6
+Version: 0.2.7
 Summary: JAX-based Recourse Explanation Library
 Home-page: https://github.com/birkhoffg/jax-relax
 Author: BirkhoffG
 Author-email: 26811230+BirkhoffG@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: JAX,Recourse,Explanation,Interpretability,Machine Learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jax-relax-0.2.6/README.md` & `jax-relax-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/jax_relax.egg-info/PKG-INFO` & `jax-relax-0.2.7/jax_relax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-relax
-Version: 0.2.6
+Version: 0.2.7
 Summary: JAX-based Recourse Explanation Library
 Home-page: https://github.com/birkhoffg/jax-relax
 Author: BirkhoffG
 Author-email: 26811230+BirkhoffG@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: JAX,Recourse,Explanation,Interpretability,Machine Learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jax-relax-0.2.6/jax_relax.egg-info/SOURCES.txt` & `jax-relax-0.2.7/jax_relax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/_modidx.py` & `jax-relax-0.2.7/relax/_modidx.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/base.py` & `jax-relax-0.2.7/relax/base.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/data_module.py` & `jax-relax-0.2.7/relax/data_module.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/data_utils/features.py` & `jax-relax-0.2.7/relax/data_utils/features.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/data_utils/preprocessing.py` & `jax-relax-0.2.7/relax/data_utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/data_utils/transforms.py` & `jax-relax-0.2.7/relax/data_utils/transforms.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/docs.py` & `jax-relax-0.2.7/relax/docs.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/evaluate.py` & `jax-relax-0.2.7/relax/evaluate.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/explain.py` & `jax-relax-0.2.7/relax/explain.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/import_essentials.py` & `jax-relax-0.2.7/relax/legacy/import_essentials.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-# Cell
-# https://github.com/fastai/fastai/blob/master/fastai/imports.py
-from __future__ import annotations
-import matplotlib.pyplot as plt,numpy as np,pandas as pd,scipy
-from typing import Union,Optional,Dict,List,Tuple,Sequence,Mapping,Callable,Iterable,Any,NamedTuple,Literal
-import io,operator,sys,os,re,mimetypes,csv,itertools,json,shutil,glob,pickle,tarfile,collections
-import hashlib,itertools,types,inspect,functools,time,math,bz2,typing,numbers,string
-import multiprocessing,threading,urllib,tempfile,concurrent.futures,matplotlib,warnings,zipfile
-
-# import sklearn
-# from sklearn.utils import shuffle
-# from sklearn.model_selection import train_test_split, GridSearchCV, cross_validate
-
-# misc.
-from pprint import pprint
-import logging
-from joblib import Parallel, delayed
-from tqdm import tqdm
-from pathlib import Path
-from fastcore.utils import in_jupyter
-from dataclasses import dataclass
-from abc import ABC, abstractmethod
-from pydantic import BaseModel as BaseParser, validator, ValidationError, Field
-import functools as ft
-from functools import partial
-
-# jax related
-import jax
-from jax import pmap, vmap, random, device_put, lax, jit, Array
-import jax.numpy as jnp, jax.random as jrand
-from jax_tqdm import loop_tqdm, scan_tqdm
-import optax
-import chex
-
-# keras
-os.environ['KERAS_BACKEND'] = 'jax'
-# import keras_core as keras
-import keras
-
-# nn related
-# import haiku as hk
+# Cell
+# https://github.com/fastai/fastai/blob/master/fastai/imports.py
+from __future__ import annotations
+import matplotlib.pyplot as plt,numpy as np,pandas as pd,scipy
+from typing import Union,Optional,Dict,List,Tuple,Sequence,Mapping,Callable,Iterable,Any,NamedTuple
+import io,operator,sys,os,re,mimetypes,csv,itertools,json,shutil,glob,pickle,tarfile,collections
+import hashlib,itertools,types,inspect,functools,time,math,bz2,typing,numbers,string
+import multiprocessing,threading,urllib,tempfile,concurrent.futures,matplotlib,warnings,zipfile
+
+# import sklearn
+# from sklearn.utils import shuffle
+# from sklearn.model_selection import train_test_split, GridSearchCV, cross_validate
+
+# misc.
+from pprint import pprint
+import logging
+from joblib import Parallel, delayed
+from tqdm import tqdm
+from pathlib import Path
+from fastcore.utils import in_jupyter
+from dataclasses import dataclass
+from abc import ABC, abstractmethod
+from pydantic import BaseModel as BaseParser, validator, ValidationError, Field
+import functools as ft
+from functools import partial
+
+# jax related
+import jax
+from jax import pmap, vmap, random, device_put, lax, jit, Array
+import jax.numpy as jnp, jax.random as jrand
+from jax_tqdm import loop_tqdm, scan_tqdm
+import optax
+import chex
+
+# keras
+os.environ['KERAS_BACKEND'] = 'jax'
+# import keras_core as keras
+import keras
+
+# nn related
+import haiku as hk
```

### Comparing `jax-relax-0.2.6/relax/legacy/ckpt_manager.py` & `jax-relax-0.2.7/relax/legacy/ckpt_manager.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/legacy/logger.py` & `jax-relax-0.2.7/relax/legacy/logger.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/legacy/module.py` & `jax-relax-0.2.7/relax/legacy/module.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/legacy/trainer.py` & `jax-relax-0.2.7/relax/legacy/trainer.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/legacy/utils.py` & `jax-relax-0.2.7/relax/legacy/utils.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/methods/base.py` & `jax-relax-0.2.7/relax/methods/base.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/methods/cchvae.py` & `jax-relax-0.2.7/relax/methods/cchvae.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/methods/clue.py` & `jax-relax-0.2.7/relax/methods/clue.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/methods/counternet.py` & `jax-relax-0.2.7/relax/methods/counternet.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/methods/dice.py` & `jax-relax-0.2.7/relax/methods/dice.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/methods/l2c.py` & `jax-relax-0.2.7/relax/methods/l2c.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/methods/proto.py` & `jax-relax-0.2.7/relax/methods/proto.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/methods/sphere.py` & `jax-relax-0.2.7/relax/methods/sphere.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,15 @@
                 self.perturb_fn = ft.partial(
                     perturb_function_with_features, 
                     cont_masks=cont_masks,
                     immut_masks=immut_masks,
                     num_categories=num_categories,
                     cat_perturb_fn=perturb_fn
                 )
-                self.apply_constraints = default_apply_constraints_fn
+                # self.apply_constraints = default_apply_constraints_fn
             else:
                 self.perturb_fn = default_perturb_function
         
     @auto_reshaping('x')
     def generate_cf(
         self,
         x: Array,  # `x` shape: (k,), where `k` is the number of features
```

### Comparing `jax-relax-0.2.6/relax/methods/vaecf.py` & `jax-relax-0.2.7/relax/methods/vaecf.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/methods/vanilla.py` & `jax-relax-0.2.7/relax/methods/vanilla.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/ml_model.py` & `jax-relax-0.2.7/relax/ml_model.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/strategy.py` & `jax-relax-0.2.7/relax/strategy.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/relax/utils.py` & `jax-relax-0.2.7/relax/utils.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.6/settings.ini` & `jax-relax-0.2.7/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-[DEFAULT]
-repo = jax-relax
-lib_name = jax-relax
-version = 0.2.6
-min_python = 3.9
-license = apache2
-black_formatting = False
-doc_path = _docs
-lib_path = relax
-nbs_path = nbs
-recursive = True
-tst_flags = slow
-put_version_in_init = True
-branch = master
-custom_sidebar = True
-doc_host = https://birkhoffg.github.io
-doc_baseurl = /jax-relax
-git_url = https://github.com/birkhoffg/jax-relax
-title = jax-relax
-renderer = relax.docs.CustomizedMarkdownRenderer
-audience = Developers
-author = BirkhoffG
-author_email = 26811230+BirkhoffG@users.noreply.github.com
-copyright = 2022 onwards, BirkhoffG
-description = JAX-based Recourse Explanation Library
-keywords = JAX, Recourse, Explanation, Interpretability, Machine Learning
-language = English
-status = 3
-user = birkhoffg
-requirements = scikit-learn>=1.0.2 pandas jax[cpu] tqdm optax pydantic>=1.9.0,<2 jax-tqdm einops keras>=3.0.3 matplotlib seaborn dm-haiku
-dev_requirements = torch>=1.7.0 causalgraphicalmodels pre-commit datasets nbdev jupyter
-readme_nb = index.ipynb
-allowed_metadata_keys = 
-allowed_cell_metadata_keys = 
-jupyter_hooks = True
-clean_ids = True
-clear_all = False
-
+[DEFAULT]
+repo = jax-relax
+lib_name = jax-relax
+version = 0.2.7
+min_python = 3.9
+license = apache2
+black_formatting = False
+doc_path = _docs
+lib_path = relax
+nbs_path = nbs
+recursive = True
+tst_flags = slow
+put_version_in_init = True
+branch = master
+custom_sidebar = True
+doc_host = https://birkhoffg.github.io
+doc_baseurl = /jax-relax
+git_url = https://github.com/birkhoffg/jax-relax
+title = jax-relax
+renderer = relax.docs.CustomizedMarkdownRenderer
+audience = Developers
+author = BirkhoffG
+author_email = 26811230+BirkhoffG@users.noreply.github.com
+copyright = 2022 onwards, BirkhoffG
+description = JAX-based Recourse Explanation Library
+keywords = JAX, Recourse, Explanation, Interpretability, Machine Learning
+language = English
+status = 3
+user = birkhoffg
+requirements = scikit-learn>=1.0.2 pandas jax[cpu] tqdm optax pydantic>=1.9.0,<2 jax-tqdm einops keras>=3.0.3 matplotlib seaborn dm-haiku
+dev_requirements = torch>=1.7.0 causalgraphicalmodels pre-commit datasets nbdev jupyter
+readme_nb = index.ipynb
+allowed_metadata_keys = 
+allowed_cell_metadata_keys = 
+jupyter_hooks = True
+clean_ids = True
+clear_all = False
+
```

### Comparing `jax-relax-0.2.6/setup.py` & `jax-relax-0.2.7/setup.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-from pkg_resources import parse_version
-from configparser import ConfigParser
-import setuptools, shlex
-assert parse_version(setuptools.__version__)>=parse_version('36.2')
-
-# note: all settings are in settings.ini; edit there, not here
-config = ConfigParser(delimiters=['='])
-config.read('settings.ini', encoding='utf-8')
-cfg = config['DEFAULT']
-
-cfg_keys = 'version description keywords author author_email'.split()
-expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
-for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
-setup_cfg = {o:cfg[o] for o in cfg_keys}
-
-licenses = {
-    'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
-    'mit': ('MIT License', 'OSI Approved :: MIT License'),
-    'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
-    'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
-    'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
-}
-statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
-    '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
-py_versions = '3.6 3.7 3.8 3.9 3.10 3.11'.split()
-
-requirements = shlex.split(cfg.get('requirements', ''))
-if cfg.get('pip_requirements'): requirements += shlex.split(cfg.get('pip_requirements', ''))
-min_python = cfg['min_python']
-lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
-dev_requirements = (cfg.get('dev_requirements') or '').split()
-
-setuptools.setup(
-    name = cfg['lib_name'],
-    license = lic[0],
-    classifiers = [
-        'Development Status :: ' + statuses[int(cfg['status'])],
-        'Intended Audience :: ' + cfg['audience'].title(),
-        'Natural Language :: ' + cfg['language'].title(),
-    ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
-    url = cfg['git_url'],
-    packages = setuptools.find_packages(),
-    include_package_data = True,
-    install_requires = requirements,
-    extras_require={ 'dev': dev_requirements },
-    dependency_links = cfg.get('dep_links','').split(),
-    python_requires  = '>=' + cfg['min_python'],
-    long_description = open('README.md', encoding='utf-8').read(),
-    long_description_content_type = 'text/markdown',
-    zip_safe = False,
-    entry_points = {
-        'console_scripts': cfg.get('console_scripts','').split(),
-        'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
-    },
-    **setup_cfg)
-
-
+from pkg_resources import parse_version
+from configparser import ConfigParser
+import setuptools, shlex
+assert parse_version(setuptools.__version__)>=parse_version('36.2')
+
+# note: all settings are in settings.ini; edit there, not here
+config = ConfigParser(delimiters=['='])
+config.read('settings.ini', encoding='utf-8')
+cfg = config['DEFAULT']
+
+cfg_keys = 'version description keywords author author_email'.split()
+expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
+for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
+setup_cfg = {o:cfg[o] for o in cfg_keys}
+
+licenses = {
+    'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
+    'mit': ('MIT License', 'OSI Approved :: MIT License'),
+    'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
+    'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
+    'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
+}
+statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
+    '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
+py_versions = '3.6 3.7 3.8 3.9 3.10 3.11'.split()
+
+requirements = shlex.split(cfg.get('requirements', ''))
+if cfg.get('pip_requirements'): requirements += shlex.split(cfg.get('pip_requirements', ''))
+min_python = cfg['min_python']
+lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
+dev_requirements = (cfg.get('dev_requirements') or '').split()
+
+setuptools.setup(
+    name = cfg['lib_name'],
+    license = lic[0],
+    classifiers = [
+        'Development Status :: ' + statuses[int(cfg['status'])],
+        'Intended Audience :: ' + cfg['audience'].title(),
+        'Natural Language :: ' + cfg['language'].title(),
+    ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
+    url = cfg['git_url'],
+    packages = setuptools.find_packages(),
+    include_package_data = True,
+    install_requires = requirements,
+    extras_require={ 'dev': dev_requirements },
+    dependency_links = cfg.get('dep_links','').split(),
+    python_requires  = '>=' + cfg['min_python'],
+    long_description = open('README.md', encoding='utf-8').read(),
+    long_description_content_type = 'text/markdown',
+    zip_safe = False,
+    entry_points = {
+        'console_scripts': cfg.get('console_scripts','').split(),
+        'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
+    },
+    **setup_cfg)
+
+
```

