# Comparing `tmp/helios_ml-0.1.4.tar.gz` & `tmp/helios_ml-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios_ml-0.1.4.tar", last modified: Thu Apr 25 04:43:03 2024, max compression
+gzip compressed data, was "helios_ml-0.1.5.tar", last modified: Fri Apr 26 01:20:58 2024, max compression
```

## Comparing `helios_ml-0.1.4.tar` & `helios_ml-0.1.5.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.459531 helios_ml-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.443530 helios_ml-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.447531 helios_ml-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-25 04:41:59.000000 helios_ml-0.1.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-25 04:41:59.000000 helios_ml-0.1.4/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-25 04:41:59.000000 helios_ml-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-25 04:41:59.000000 helios_ml-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-25 04:41:59.000000 helios_ml-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-25 04:43:03.459531 helios_ml-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-25 04:41:59.000000 helios_ml-0.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.443530 helios_ml-0.1.4/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.447531 helios_ml-0.1.4/data/logo/
--rw-r--r--   0 runner    (1001) docker     (127)    20058 2024-04-25 04:41:59.000000 helios_ml-0.1.4/data/logo/logo-background.png
--rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-04-25 04:41:59.000000 helios_ml-0.1.4/data/logo/logo-transparent.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.443530 helios_ml-0.1.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.447531 helios_ml-0.1.4/examples/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-04-25 04:41:59.000000 helios_ml-0.1.4/examples/cifar10/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-25 04:41:59.000000 helios_ml-0.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.447531 helios_ml-0.1.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-25 04:41:59.000000 helios_ml-0.1.4/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-25 04:41:59.000000 helios_ml-0.1.4/requirements/default.txt
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-25 04:41:59.000000 helios_ml-0.1.4/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 04:43:03.459531 helios_ml-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.443530 helios_ml-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.447531 helios_ml-0.1.4/src/helios/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.447531 helios_ml-0.1.4/src/helios/core/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/core/cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/core/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    17255 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/core/rng.py
--rw-r--r--   0 runner    (1001) docker     (127)    13539 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.451531 helios_ml-0.1.4/src/helios/data/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/data/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/data/samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/data/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.451531 helios_ml-0.1.4/src/helios/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/losses/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/losses/weighted_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.451531 helios_ml-0.1.4/src/helios/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/metrics/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.451531 helios_ml-0.1.4/src/helios/model/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.451531 helios_ml-0.1.4/src/helios/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/nn/swa_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/nn/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.451531 helios_ml-0.1.4/src/helios/optim/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/optim/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.451531 helios_ml-0.1.4/src/helios/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/scheduler/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/scheduler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    35631 2024-04-25 04:41:59.000000 helios_ml-0.1.4/src/helios/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.455531 helios_ml-0.1.4/src/helios_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-25 04:43:03.000000 helios_ml-0.1.4/src/helios_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-25 04:43:03.000000 helios_ml-0.1.4/src/helios_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 04:43:03.000000 helios_ml-0.1.4/src/helios_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-25 04:43:03.000000 helios_ml-0.1.4/src/helios_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 04:43:03.000000 helios_ml-0.1.4/src/helios_ml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.455531 helios_ml-0.1.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.455531 helios_ml-0.1.4/test/registry_test/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/registry_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/registry_test/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/registry_test/foo.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/registry_test/func_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.455531 helios_ml-0.1.4/test/registry_test/nested/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/registry_test/nested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/registry_test/nested/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/registry_test/nested/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/registry_test/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/test_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/test_optim.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-25 04:41:59.000000 helios_ml-0.1.4/test/test_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:43:03.455531 helios_ml-0.1.4/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-25 04:41:59.000000 helios_ml-0.1.4/tools/generate_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.170892 helios_ml-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.154892 helios_ml-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.158892 helios_ml-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-26 01:20:25.000000 helios_ml-0.1.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-26 01:20:25.000000 helios_ml-0.1.5/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-26 01:20:25.000000 helios_ml-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-26 01:20:25.000000 helios_ml-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-26 01:20:25.000000 helios_ml-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-26 01:20:58.170892 helios_ml-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-26 01:20:25.000000 helios_ml-0.1.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.154892 helios_ml-0.1.5/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.158892 helios_ml-0.1.5/data/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)    20058 2024-04-26 01:20:25.000000 helios_ml-0.1.5/data/logo/logo-background.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-04-26 01:20:25.000000 helios_ml-0.1.5/data/logo/logo-transparent.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.154892 helios_ml-0.1.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.158892 helios_ml-0.1.5/examples/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-04-26 01:20:25.000000 helios_ml-0.1.5/examples/cifar10/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-26 01:20:25.000000 helios_ml-0.1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.158892 helios_ml-0.1.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-26 01:20:25.000000 helios_ml-0.1.5/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-26 01:20:25.000000 helios_ml-0.1.5/requirements/default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-26 01:20:25.000000 helios_ml-0.1.5/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 01:20:58.170892 helios_ml-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.154892 helios_ml-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.158892 helios_ml-0.1.5/src/helios/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.158892 helios_ml-0.1.5/src/helios/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/core/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/core/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17255 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/core/rng.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13539 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.162892 helios_ml-0.1.5/src/helios/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/data/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/data/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/data/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.162892 helios_ml-0.1.5/src/helios/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/losses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/losses/weighted_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.162892 helios_ml-0.1.5/src/helios/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/metrics/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.162892 helios_ml-0.1.5/src/helios/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.162892 helios_ml-0.1.5/src/helios/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/nn/swa_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/nn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.162892 helios_ml-0.1.5/src/helios/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/optim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.162892 helios_ml-0.1.5/src/helios/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/scheduler/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/scheduler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35763 2024-04-26 01:20:25.000000 helios_ml-0.1.5/src/helios/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.166892 helios_ml-0.1.5/src/helios_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-26 01:20:58.000000 helios_ml-0.1.5/src/helios_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-26 01:20:58.000000 helios_ml-0.1.5/src/helios_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 01:20:58.000000 helios_ml-0.1.5/src/helios_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-26 01:20:58.000000 helios_ml-0.1.5/src/helios_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 01:20:58.000000 helios_ml-0.1.5/src/helios_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.166892 helios_ml-0.1.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.166892 helios_ml-0.1.5/test/registry_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/registry_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/registry_test/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/registry_test/foo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/registry_test/func_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.166892 helios_ml-0.1.5/test/registry_test/nested/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/registry_test/nested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/registry_test/nested/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/registry_test/nested/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/registry_test/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/test_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/test_optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-26 01:20:25.000000 helios_ml-0.1.5/test/test_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:20:58.166892 helios_ml-0.1.5/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-26 01:20:25.000000 helios_ml-0.1.5/tools/generate_requirements.py
```

### Comparing `helios_ml-0.1.4/.github/workflows/publish.yml` & `helios_ml-0.1.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/.github/workflows/tests.yml` & `helios_ml-0.1.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/.pre-commit-config.yaml` & `helios_ml-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/LICENSE` & `helios_ml-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/PKG-INFO` & `helios_ml-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-ml
-Version: 0.1.4
+Version: 0.1.5
 Summary: A light-weight system for training AI networks using PyTorch
 Author-email: "Mauricio A. Rovira Galvez" <maroviragalvez@outlook.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/marovira/helios-ml
 Project-URL: source, https://github.com/marovira/helios-ml
 Project-URL: issues, https://github.com/marovira/helios-ml/issues
 Project-URL: release notes, https://github.com/marovira/helios-ml/releases
```

### Comparing `helios_ml-0.1.4/README.rst` & `helios_ml-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/data/logo/logo-background.png` & `helios_ml-0.1.5/data/logo/logo-background.png`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/data/logo/logo-transparent.png` & `helios_ml-0.1.5/data/logo/logo-transparent.png`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/examples/cifar10/cifar10.py` & `helios_ml-0.1.5/examples/cifar10/cifar10.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/pyproject.toml` & `helios_ml-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/core/cuda.py` & `helios_ml-0.1.5/src/helios/core/cuda.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/core/distributed.py` & `helios_ml-0.1.5/src/helios/core/distributed.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/core/logging.py` & `helios_ml-0.1.5/src/helios/core/logging.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/core/rng.py` & `helios_ml-0.1.5/src/helios/core/rng.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/core/utils.py` & `helios_ml-0.1.5/src/helios/core/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/data/__init__.py` & `helios_ml-0.1.5/src/helios/data/__init__.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/data/datamodule.py` & `helios_ml-0.1.5/src/helios/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/data/functional.py` & `helios_ml-0.1.5/src/helios/data/functional.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/data/samplers.py` & `helios_ml-0.1.5/src/helios/data/samplers.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/data/transforms.py` & `helios_ml-0.1.5/src/helios/data/transforms.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/losses/utils.py` & `helios_ml-0.1.5/src/helios/losses/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/losses/weighted_loss.py` & `helios_ml-0.1.5/src/helios/losses/weighted_loss.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/metrics/functional.py` & `helios_ml-0.1.5/src/helios/metrics/functional.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/metrics/metrics.py` & `helios_ml-0.1.5/src/helios/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/model/model.py` & `helios_ml-0.1.5/src/helios/model/model.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/model/utils.py` & `helios_ml-0.1.5/src/helios/model/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/nn/swa_utils.py` & `helios_ml-0.1.5/src/helios/nn/swa_utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/nn/utils.py` & `helios_ml-0.1.5/src/helios/nn/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/onnx.py` & `helios_ml-0.1.5/src/helios/onnx.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/optim/utils.py` & `helios_ml-0.1.5/src/helios/optim/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/scheduler/schedulers.py` & `helios_ml-0.1.5/src/helios/scheduler/schedulers.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/scheduler/utils.py` & `helios_ml-0.1.5/src/helios/scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/src/helios/trainer.py` & `helios_ml-0.1.5/src/helios/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -748,15 +748,15 @@
         save_freq = self._chkpt_frequency
         val_freq = self._valid_frequency
         print_freq = self._print_frequency
         accumulation_steps = self._accumulation_steps
         enable_progress_bar = self._enable_progress_bar
         early_stop_cycles = self._early_stop_cycles
 
-        perform_validation: bool = True
+        current_iteration_changed: bool = True
         training_done: bool = False
         root_logger = logging.get_root_logger()
         iter_timer = core.AverageTimer()
 
         pbar_disabled = (
             self._is_distributed and self.rank != 0
         ) or not enable_progress_bar
@@ -783,17 +783,17 @@
             epoch_start = time.time()
 
             iter_timer.start()
             for batch in dataloader:
                 if state.global_iteration % accumulation_steps == 0:
                     state.current_iteration += 1
                     state.running_iter += 1
-                    perform_validation = True
+                    current_iteration_changed = True
                 else:
-                    perform_validation = False
+                    current_iteration_changed = False
 
                 state.global_iteration += 1
                 if state.current_iteration > total_steps:
                     training_done = True
                     break
 
                 self.model.on_training_batch_start(state)
@@ -802,39 +802,41 @@
                 state.average_iter_time = iter_timer.get_average_time()
                 self.model.on_training_batch_end(
                     state,
                     should_log=(
                         False
                         if print_freq is None
                         else state.current_iteration % print_freq == 0
+                        and current_iteration_changed
                     ),
                 )
                 # Depending on how fast the iteration loop is, it is possible that the
                 # progress bar isn't refreshed every tick, so make sure it gets re-drawn.
                 if state.global_iteration % accumulation_steps == 0 and not pbar.update():
                     pbar.refresh()
                 state.dataset_iter += 1
 
                 if (
                     val_freq is not None
                     and state.current_iteration % val_freq == 0
-                    and perform_validation
+                    and current_iteration_changed
                 ):
                     self._validate(state.validation_cycles)
                     state.validation_cycles += 1
                     state.running_iter = 0
                     if not self.model.have_metrics_improved():
                         state.early_stop_count += 1
                     else:
                         state.early_stop_count = 0
 
                 if (
                     save_freq is not None
                     and state.current_iteration % save_freq == 0
                     and self.rank == 0
+                    and current_iteration_changed
                 ):
                     self._save_checkpoint(state)
 
             state.dataset_iter = 0
             state.global_epoch += 1
 
             root_logger.info(
```

### Comparing `helios_ml-0.1.4/src/helios_ml.egg-info/PKG-INFO` & `helios_ml-0.1.5/src/helios_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-ml
-Version: 0.1.4
+Version: 0.1.5
 Summary: A light-weight system for training AI networks using PyTorch
 Author-email: "Mauricio A. Rovira Galvez" <maroviragalvez@outlook.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/marovira/helios-ml
 Project-URL: source, https://github.com/marovira/helios-ml
 Project-URL: issues, https://github.com/marovira/helios-ml/issues
 Project-URL: release notes, https://github.com/marovira/helios-ml/releases
```

### Comparing `helios_ml-0.1.4/src/helios_ml.egg-info/SOURCES.txt` & `helios_ml-0.1.5/src/helios_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/test/conftest.py` & `helios_ml-0.1.5/test/conftest.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/test/test_core.py` & `helios_ml-0.1.5/test/test_core.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/test/test_data.py` & `helios_ml-0.1.5/test/test_data.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/test/test_losses.py` & `helios_ml-0.1.5/test/test_losses.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/test/test_metrics.py` & `helios_ml-0.1.5/test/test_metrics.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/test/test_model.py` & `helios_ml-0.1.5/test/test_model.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/test/test_nn.py` & `helios_ml-0.1.5/test/test_nn.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/test/test_onnx.py` & `helios_ml-0.1.5/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/test/test_trainer.py` & `helios_ml-0.1.5/test/test_trainer.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.4/tools/generate_requirements.py` & `helios_ml-0.1.5/tools/generate_requirements.py`

 * *Files identical despite different names*

