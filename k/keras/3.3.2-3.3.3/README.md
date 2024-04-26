# Comparing `tmp/keras-3.3.2.tar.gz` & `tmp/keras-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-3.3.2.tar", last modified: Mon Apr 22 23:35:30 2024, max compression
+gzip compressed data, was "keras-3.3.3.tar", last modified: Fri Apr 26 23:19:33 2024, max compression
```

## Comparing `keras-3.3.2.tar` & `keras-3.3.3.tar`

### file list

```diff
@@ -1,697 +1,698 @@
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.300335 keras-3.3.2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5731 2024-04-22 23:35:30.300055 keras-3.3.2/PKG-INFO
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4789 2024-04-22 23:35:27.000000 keras-3.3.2/README.md
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.193068 keras-3.3.2/keras/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      828 2024-04-20 19:17:05.000000 keras-3.3.2/keras/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.194100 keras-3.3.2/keras/_tf_keras/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       34 2024-04-22 23:35:27.000000 keras-3.3.2/keras/_tf_keras/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.194255 keras-3.3.2/keras/_tf_keras/keras/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2331 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.194417 keras-3.3.2/keras/_tf_keras/keras/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1347 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.194580 keras-3.3.2/keras/_tf_keras/keras/applications/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3295 2024-04-22 23:09:51.000000 keras-3.3.2/keras/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.194743 keras-3.3.2/keras/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      535 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.194898 keras-3.3.2/keras/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      414 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.195058 keras-3.3.2/keras/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      758 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.195216 keras-3.3.2/keras/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      733 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.195369 keras-3.3.2/keras/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      258 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.195517 keras-3.3.2/keras/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      341 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.195687 keras-3.3.2/keras/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.195848 keras-3.3.2/keras/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.196003 keras-3.3.2/keras/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.196170 keras-3.3.2/keras/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      254 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.196320 keras-3.3.2/keras/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      351 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.196477 keras-3.3.2/keras/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      397 2024-04-22 23:09:43.000000 keras-3.3.2/keras/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.196647 keras-3.3.2/keras/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      293 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.196818 keras-3.3.2/keras/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      418 2024-04-22 23:09:55.000000 keras-3.3.2/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.196975 keras-3.3.2/keras/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.197138 keras-3.3.2/keras/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.197291 keras-3.3.2/keras/_tf_keras/keras/applications/xception/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      299 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.197456 keras-3.3.2/keras/_tf_keras/keras/backend/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6808 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.197639 keras-3.3.2/keras/_tf_keras/keras/callbacks/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1044 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.197798 keras-3.3.2/keras/_tf_keras/keras/config/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1143 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.197961 keras-3.3.2/keras/_tf_keras/keras/constraints/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      797 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.198115 keras-3.3.2/keras/_tf_keras/keras/datasets/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      454 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.198268 keras-3.3.2/keras/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.198428 keras-3.3.2/keras/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      182 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.198586 keras-3.3.2/keras/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      171 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.198756 keras-3.3.2/keras/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      172 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.198919 keras-3.3.2/keras/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.199087 keras-3.3.2/keras/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      219 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.199246 keras-3.3.2/keras/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      169 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.199400 keras-3.3.2/keras/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      280 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.199551 keras-3.3.2/keras/_tf_keras/keras/distribution/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      775 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.199723 keras-3.3.2/keras/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      536 2024-04-22 23:10:10.000000 keras-3.3.2/keras/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.199901 keras-3.3.2/keras/_tf_keras/keras/export/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      176 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.200075 keras-3.3.2/keras/_tf_keras/keras/initializers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2844 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.200246 keras-3.3.2/keras/_tf_keras/keras/layers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10285 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.200509 keras-3.3.2/keras/_tf_keras/keras/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      158 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.200709 keras-3.3.2/keras/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.200911 keras-3.3.2/keras/_tf_keras/keras/losses/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3352 2024-04-22 23:11:01.000000 keras-3.3.2/keras/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.201113 keras-3.3.2/keras/_tf_keras/keras/metrics/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5164 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.201321 keras-3.3.2/keras/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      636 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.201537 keras-3.3.2/keras/_tf_keras/keras/models/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      416 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.201742 keras-3.3.2/keras/_tf_keras/keras/ops/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8842 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.201950 keras-3.3.2/keras/_tf_keras/keras/ops/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      442 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.202123 keras-3.3.2/keras/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      556 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.202307 keras-3.3.2/keras/_tf_keras/keras/ops/nn/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1464 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.202482 keras-3.3.2/keras/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5687 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.202668 keras-3.3.2/keras/_tf_keras/keras/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      965 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.202845 keras-3.3.2/keras/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      516 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.203030 keras-3.3.2/keras/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      918 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.203201 keras-3.3.2/keras/_tf_keras/keras/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      765 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.203367 keras-3.3.2/keras/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1364 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.203551 keras-3.3.2/keras/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      509 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.203729 keras-3.3.2/keras/_tf_keras/keras/preprocessing/text/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      436 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/preprocessing/text/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.203907 keras-3.3.2/keras/_tf_keras/keras/quantizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      627 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.204079 keras-3.3.2/keras/_tf_keras/keras/random/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      628 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.204245 keras-3.3.2/keras/_tf_keras/keras/regularizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      819 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.204414 keras-3.3.2/keras/_tf_keras/keras/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      923 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.204591 keras-3.3.2/keras/_tf_keras/keras/tree/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      582 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.204763 keras-3.3.2/keras/_tf_keras/keras/utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2652 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.204931 keras-3.3.2/keras/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-22 23:09:19.000000 keras-3.3.2/keras/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.205112 keras-3.3.2/keras/api/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2057 2024-04-22 23:35:27.000000 keras-3.3.2/keras/api/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.205294 keras-3.3.2/keras/api/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1347 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/activations/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.205477 keras-3.3.2/keras/api/applications/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3295 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/applications/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.205646 keras-3.3.2/keras/api/applications/convnext/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      535 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/applications/convnext/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.205829 keras-3.3.2/keras/api/applications/densenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      414 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/applications/densenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.206012 keras-3.3.2/keras/api/applications/efficientnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      758 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/applications/efficientnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.206177 keras-3.3.2/keras/api/applications/efficientnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      733 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.206351 keras-3.3.2/keras/api/applications/imagenet_utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      258 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.206513 keras-3.3.2/keras/api/applications/inception_resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      341 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.206673 keras-3.3.2/keras/api/applications/inception_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/applications/inception_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.206838 keras-3.3.2/keras/api/applications/mobilenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/applications/mobilenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.207005 keras-3.3.2/keras/api/applications/mobilenet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.207167 keras-3.3.2/keras/api/applications/mobilenet_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      254 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.207328 keras-3.3.2/keras/api/applications/nasnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      351 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/applications/nasnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.207489 keras-3.3.2/keras/api/applications/resnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      397 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/applications/resnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.207652 keras-3.3.2/keras/api/applications/resnet50/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      293 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/applications/resnet50/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.207820 keras-3.3.2/keras/api/applications/resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      418 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.207984 keras-3.3.2/keras/api/applications/vgg16/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/applications/vgg16/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.208147 keras-3.3.2/keras/api/applications/vgg19/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/applications/vgg19/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.208737 keras-3.3.2/keras/api/applications/xception/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      299 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/applications/xception/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.210013 keras-3.3.2/keras/api/backend/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      883 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/backend/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.210315 keras-3.3.2/keras/api/callbacks/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1044 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/callbacks/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.210557 keras-3.3.2/keras/api/config/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1143 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/config/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.210806 keras-3.3.2/keras/api/constraints/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      797 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/constraints/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.211016 keras-3.3.2/keras/api/datasets/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      454 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/datasets/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.211203 keras-3.3.2/keras/api/datasets/boston_housing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.211384 keras-3.3.2/keras/api/datasets/california_housing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      182 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/datasets/california_housing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.211549 keras-3.3.2/keras/api/datasets/cifar10/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      171 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/datasets/cifar10/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.211758 keras-3.3.2/keras/api/datasets/cifar100/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      172 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/datasets/cifar100/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.212000 keras-3.3.2/keras/api/datasets/fashion_mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.212190 keras-3.3.2/keras/api/datasets/imdb/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      219 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/datasets/imdb/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.212389 keras-3.3.2/keras/api/datasets/mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      169 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/datasets/mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.212607 keras-3.3.2/keras/api/datasets/reuters/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      280 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/datasets/reuters/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.212797 keras-3.3.2/keras/api/distribution/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      775 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/distribution/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.212965 keras-3.3.2/keras/api/dtype_policies/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      536 2024-04-22 16:35:02.000000 keras-3.3.2/keras/api/dtype_policies/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.213167 keras-3.3.2/keras/api/export/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      176 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/export/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.213421 keras-3.3.2/keras/api/initializers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2844 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/initializers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.213619 keras-3.3.2/keras/api/layers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9963 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/layers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.213812 keras-3.3.2/keras/api/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      158 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.213977 keras-3.3.2/keras/api/legacy/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/legacy/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.214137 keras-3.3.2/keras/api/losses/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2381 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/losses/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.214300 keras-3.3.2/keras/api/metrics/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4239 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/metrics/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.214479 keras-3.3.2/keras/api/mixed_precision/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      636 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/mixed_precision/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.214637 keras-3.3.2/keras/api/models/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      416 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/models/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.214807 keras-3.3.2/keras/api/ops/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8842 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/ops/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.214983 keras-3.3.2/keras/api/ops/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      442 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/ops/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.215144 keras-3.3.2/keras/api/ops/linalg/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      556 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/ops/linalg/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.215311 keras-3.3.2/keras/api/ops/nn/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1464 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/ops/nn/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.215479 keras-3.3.2/keras/api/ops/numpy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5687 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/ops/numpy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.215645 keras-3.3.2/keras/api/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      965 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/optimizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.215811 keras-3.3.2/keras/api/optimizers/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      516 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/optimizers/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.215970 keras-3.3.2/keras/api/optimizers/schedules/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      918 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/optimizers/schedules/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.216121 keras-3.3.2/keras/api/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      453 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/preprocessing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.216283 keras-3.3.2/keras/api/preprocessing/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      379 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/preprocessing/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.216453 keras-3.3.2/keras/api/preprocessing/sequence/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      179 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.216606 keras-3.3.2/keras/api/quantizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      627 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/quantizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.216759 keras-3.3.2/keras/api/random/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      628 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/random/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.216917 keras-3.3.2/keras/api/regularizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      819 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/regularizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.217060 keras-3.3.2/keras/api/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      923 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.217211 keras-3.3.2/keras/api/tree/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      582 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/tree/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.217367 keras-3.3.2/keras/api/utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2652 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.217518 keras-3.3.2/keras/api/utils/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-20 19:17:05.000000 keras-3.3.2/keras/api/utils/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.217988 keras-3.3.2/keras/src/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      648 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.218495 keras-3.3.2/keras/src/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3540 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/activations/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12442 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/activations/activations.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1173 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/api_export.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.222908 keras-3.3.2/keras/src/applications/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/applications/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    24919 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/applications/convnext.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16848 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/applications/densenet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25274 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/applications/efficientnet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    40460 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16034 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14509 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15520 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/applications/inception_v3.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17168 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/applications/mobilenet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17934 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    23521 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    30694 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/applications/nasnet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19006 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/applications/resnet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6363 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/applications/resnet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9110 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/applications/vgg16.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9433 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/applications/vgg19.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12705 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/applications/xception.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.223550 keras-3.3.2/keras/src/backend/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1971 2024-04-20 18:16:39.000000 keras-3.3.2/keras/src/backend/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.225177 keras-3.3.2/keras/src/backend/common/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      583 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/common/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17099 2024-04-21 17:37:40.000000 keras-3.3.2/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9808 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/common/dtypes.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3412 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/common/global_state.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8974 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2545 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/common/name_scope.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3692 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    21446 2024-04-20 18:16:39.000000 keras-3.3.2/keras/src/backend/common/variables.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7139 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/config.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1056 2024-04-20 18:16:39.000000 keras-3.3.2/keras/src/backend/exports.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.228087 keras-3.3.2/keras/src/backend/jax/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1173 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/jax/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12765 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/jax/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9679 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14746 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/jax/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       25 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/jax/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1800 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/jax/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8757 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/jax/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26214 2024-04-22 16:38:23.000000 keras-3.3.2/keras/src/backend/jax/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    30833 2024-04-22 22:43:14.000000 keras-3.3.2/keras/src/backend/jax/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3856 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3594 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/jax/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7552 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/jax/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13804 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/jax/sparse.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    36259 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.230213 keras-3.3.2/keras/src/backend/numpy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1012 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6855 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/numpy/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13086 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/numpy/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       27 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/numpy/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1964 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10586 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/numpy/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18006 2024-04-20 18:16:39.000000 keras-3.3.2/keras/src/backend/numpy/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    28098 2024-04-22 22:43:14.000000 keras-3.3.2/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3961 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/numpy/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7652 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10738 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.233927 keras-3.3.2/keras/src/backend/tensorflow/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1458 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9444 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2747 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14197 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4639 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6161 2024-04-20 18:16:39.000000 keras-3.3.2/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11451 2024-04-20 18:16:39.000000 keras-3.3.2/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26595 2024-04-20 18:16:39.000000 keras-3.3.2/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    77771 2024-04-22 22:43:14.000000 keras-3.3.2/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9334 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6211 2024-04-20 18:16:39.000000 keras-3.3.2/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    34600 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    32268 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      170 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1993 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    33111 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.236661 keras-3.3.2/keras/src/backend/torch/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1892 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16162 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14001 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1865 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1801 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15073 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    24278 2024-04-20 18:16:39.000000 keras-3.3.2/keras/src/backend/torch/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    47434 2024-04-22 22:43:14.000000 keras-3.3.2/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.238633 keras-3.3.2/keras/src/backend/torch/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       78 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1672 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1041 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1889 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1483 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      150 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1041 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2421 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1803 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      783 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2053 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1175 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8292 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13704 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17577 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.241701 keras-3.3.2/keras/src/callbacks/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      922 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/callbacks/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7552 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9830 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/callbacks/callback.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5255 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/callbacks/callback_list.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3206 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8933 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1301 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/callbacks/history.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3441 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2965 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18488 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3104 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5339 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2727 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6843 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26393 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      669 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/callbacks/terminate_on_nan.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.242092 keras-3.3.2/keras/src/constraints/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1715 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/constraints/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7333 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/constraints/constraints.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.244007 keras-3.3.2/keras/src/datasets/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      383 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/datasets/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2644 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/datasets/boston_housing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3850 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/datasets/california_housing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      704 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/datasets/cifar.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3086 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/datasets/cifar10.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2914 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/datasets/cifar100.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2929 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7149 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/datasets/imdb.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2393 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/datasets/mnist.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7203 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/datasets/reuters.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.244393 keras-3.3.2/keras/src/distribution/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      718 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/distribution/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    31207 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/distribution/distribution_lib.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.244798 keras-3.3.2/keras/src/dtype_policies/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3506 2024-04-22 16:35:02.000000 keras-3.3.2/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12480 2024-04-22 16:35:02.000000 keras-3.3.2/keras/src/dtype_policies/dtype_policy.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.245211 keras-3.3.2/keras/src/export/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       54 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/export/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    32830 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/export/export_lib.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.246010 keras-3.3.2/keras/src/initializers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3958 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/initializers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4884 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2633 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/initializers/initializer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    23462 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/initializers/random_initializers.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.246779 keras-3.3.2/keras/src/layers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8848 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.248387 keras-3.3.2/keras/src/layers/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      272 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/activations/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1236 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/activations/activation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      809 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/activations/elu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1900 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3453 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/activations/prelu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2670 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/activations/relu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2258 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/activations/softmax.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.249307 keras-3.3.2/keras/src/layers/attention/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/attention/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4330 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11889 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/attention/attention.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17952 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    28353 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/attention/multi_head_attention.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.253928 keras-3.3.2/keras/src/layers/convolutional/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17263 2024-04-22 16:35:02.000000 keras-3.3.2/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10695 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11617 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12643 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7300 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5571 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5670 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5691 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5893 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5897 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5999 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6087 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6450 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6531 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/convolutional/separable_conv2d.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.255697 keras-3.3.2/keras/src/layers/core/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/core/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25345 2024-04-22 16:35:02.000000 keras-3.3.2/keras/src/layers/core/dense.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    42181 2024-04-22 16:35:02.000000 keras-3.3.2/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17364 2024-04-22 16:35:02.000000 keras-3.3.2/keras/src/layers/core/embedding.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      817 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/core/identity.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5107 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/core/input_layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8989 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2629 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/core/masking.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1535 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/core/wrapper.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9827 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/input_spec.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    63788 2024-04-20 18:16:39.000000 keras-3.3.2/keras/src/layers/layer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.257527 keras-3.3.2/keras/src/layers/merging/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/merging/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2150 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/merging/add.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2214 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/merging/average.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9249 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6586 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12807 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/merging/dot.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2214 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/merging/maximum.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2212 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/merging/minimum.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2211 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/merging/multiply.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2684 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.258510 keras-3.3.2/keras/src/layers/normalization/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13440 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8534 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9836 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4306 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1831 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/normalization/unit_normalization.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.260810 keras-3.3.2/keras/src/layers/pooling/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3344 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4150 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3235 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1460 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2425 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3131 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2469 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2603 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2357 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2451 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2585 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3343 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4125 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3225 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/pooling/max_pooling3d.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.265785 keras-3.3.2/keras/src/layers/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14572 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8705 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5489 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13145 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    29613 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8317 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10936 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    41399 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18458 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13920 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6463 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3814 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6315 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3805 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9645 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10614 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10820 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2177 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5349 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17734 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27820 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2133 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.266981 keras-3.3.2/keras/src/layers/regularization/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1198 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3594 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2978 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2041 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2089 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7300 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/regularization/spatial_dropout.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.269364 keras-3.3.2/keras/src/layers/reshaping/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2760 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9044 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11265 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3059 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2087 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1335 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2322 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1592 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5992 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4910 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2106 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4646 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5060 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/reshaping/zero_padding3d.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.271417 keras-3.3.2/keras/src/layers/rnn/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13203 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27242 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8294 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8379 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8287 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2132 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27701 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/rnn/gru.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26544 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19159 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17537 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4943 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4797 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/layers/rnn/time_distributed.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.272088 keras-3.3.2/keras/src/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/legacy/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    70241 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/legacy/backend.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8412 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/legacy/layers.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      523 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/legacy/losses.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.272784 keras-3.3.2/keras/src/legacy/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    65545 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11172 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11110 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.273803 keras-3.3.2/keras/src/legacy/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7296 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    22750 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      485 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9275 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    21808 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.274274 keras-3.3.2/keras/src/losses/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6363 2024-04-22 16:35:02.000000 keras-3.3.2/keras/src/losses/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5892 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/losses/loss.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    69132 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/losses/losses.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.276069 keras-3.3.2/keras/src/metrics/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7198 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/metrics/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15604 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    61579 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11743 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3255 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26976 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8186 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/metrics/metric.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26611 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10692 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7212 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19818 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/metrics/regression_metrics.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.277676 keras-3.3.2/keras/src/models/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      143 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/models/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11094 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/models/cloning.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    32453 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/models/functional.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    23789 2024-04-20 18:16:39.000000 keras-3.3.2/keras/src/models/model.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13013 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/models/sequential.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2164 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/models/variable_mapping.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.280199 keras-3.3.2/keras/src/ops/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      644 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/ops/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    22866 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/ops/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15334 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/ops/function.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    37256 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/ops/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18342 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/ops/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    30618 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/ops/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    64046 2024-04-20 18:16:39.000000 keras-3.3.2/keras/src/ops/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5583 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/ops/node.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)   195627 2024-04-22 22:43:14.000000 keras-3.3.2/keras/src/ops/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10732 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/ops/operation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13759 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/ops/operation_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1694 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/ops/symbolic_arguments.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.285011 keras-3.3.2/keras/src/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3931 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/optimizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4759 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/optimizers/adadelta.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7637 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/optimizers/adafactor.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3918 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/optimizers/adagrad.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5909 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/optimizers/adam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5083 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/optimizers/adamax.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3784 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/optimizers/adamw.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    40410 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9099 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/optimizers/ftrl.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4969 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/optimizers/lion.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11553 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5926 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/optimizers/nadam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      813 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/optimizers/optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6003 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/optimizers/rmsprop.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.285617 keras-3.3.2/keras/src/optimizers/schedules/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      546 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    35507 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4556 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/optimizers/sgd.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.286813 keras-3.3.2/keras/src/quantizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1784 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/quantizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4810 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/quantizers/quantizers.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.287481 keras-3.3.2/keras/src/random/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      420 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/random/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13438 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/random/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4905 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/random/seed_generator.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.288037 keras-3.3.2/keras/src/regularizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1731 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/regularizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11799 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/regularizers/regularizers.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.289345 keras-3.3.2/keras/src/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      614 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/saving/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7358 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/saving/object_registration.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9737 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/saving/saving_api.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27008 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/saving/saving_lib.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    29052 2024-04-20 18:16:39.000000 keras-3.3.2/keras/src/saving/serialization_lib.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.289954 keras-3.3.2/keras/src/testing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      266 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/testing/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27552 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/testing/test_case.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6197 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/testing/test_utils.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.290703 keras-3.3.2/keras/src/trainers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/trainers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25940 2024-04-22 17:46:41.000000 keras-3.3.2/keras/src/trainers/compile_utils.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.292790 keras-3.3.2/keras/src/trainers/data_adapters/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5423 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14323 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17071 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3101 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9717 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2863 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19412 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5224 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2643 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3923 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    46449 2024-04-20 18:16:39.000000 keras-3.3.2/keras/src/trainers/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.293589 keras-3.3.2/keras/src/tree/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      521 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/tree/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4970 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/tree/dmtree_impl.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11138 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/tree/optree_impl.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9397 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/tree/tree_api.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.299314 keras-3.3.2/keras/src/utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1423 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2876 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/argument_validation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14664 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4130 2024-04-20 18:16:39.000000 keras-3.3.2/keras/src/utils/backend_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1442 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/code_stats.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    28554 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1483 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/dtype_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16371 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/file_utils.py
--rwxr-xr-x   0 fchollet (337002) primarygroup (89939)    16538 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16544 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/image_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3491 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/io_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26570 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/jax_layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      263 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/jax_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15635 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/model_visualization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1276 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/module_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1776 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/naming.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4571 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/numerical_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10349 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/progbar.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4003 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/python_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1677 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/rng_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4714 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/sequence_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14512 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/summary_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10509 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4630 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/tf_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9842 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4991 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/torch_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8997 2024-04-20 16:30:07.000000 keras-3.3.2/keras/src/utils/traceback_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8980 2024-04-21 17:38:44.000000 keras-3.3.2/keras/src/utils/tracking.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      189 2024-04-22 23:35:27.000000 keras-3.3.2/keras/src/version.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 23:35:30.299646 keras-3.3.2/keras.egg-info/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5731 2024-04-22 23:35:30.000000 keras-3.3.2/keras.egg-info/PKG-INFO
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    20344 2024-04-22 23:35:30.000000 keras-3.3.2/keras.egg-info/SOURCES.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-22 23:35:30.000000 keras-3.3.2/keras.egg-info/dependency_links.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       47 2024-04-22 23:35:30.000000 keras-3.3.2/keras.egg-info/requires.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        6 2024-04-22 23:35:30.000000 keras-3.3.2/keras.egg-info/top_level.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       38 2024-04-22 23:35:30.300394 keras-3.3.2/setup.cfg
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1769 2024-04-22 23:35:27.000000 keras-3.3.2/setup.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.910323 keras-3.3.3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5731 2024-04-26 23:19:33.910041 keras-3.3.3/PKG-INFO
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4789 2024-04-26 23:19:29.000000 keras-3.3.3/README.md
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.819950 keras-3.3.3/keras/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      828 2024-04-26 23:13:01.000000 keras-3.3.3/keras/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.820858 keras-3.3.3/keras/_tf_keras/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       34 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.821004 keras-3.3.3/keras/_tf_keras/keras/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2088 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.821345 keras-3.3.3/keras/_tf_keras/keras/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1347 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.821581 keras-3.3.3/keras/_tf_keras/keras/applications/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3295 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.821765 keras-3.3.3/keras/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      535 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.821948 keras-3.3.3/keras/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      414 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.822124 keras-3.3.3/keras/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      758 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.822288 keras-3.3.3/keras/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      733 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.822449 keras-3.3.3/keras/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      258 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.822613 keras-3.3.3/keras/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      341 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.822773 keras-3.3.3/keras/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.822920 keras-3.3.3/keras/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.823077 keras-3.3.3/keras/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.823236 keras-3.3.3/keras/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      254 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.823397 keras-3.3.3/keras/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      351 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.823560 keras-3.3.3/keras/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      397 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.823722 keras-3.3.3/keras/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      293 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.823882 keras-3.3.3/keras/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      418 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.824036 keras-3.3.3/keras/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.824254 keras-3.3.3/keras/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.824421 keras-3.3.3/keras/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      299 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.824582 keras-3.3.3/keras/_tf_keras/keras/backend/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6684 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.824772 keras-3.3.3/keras/_tf_keras/keras/callbacks/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1044 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.824926 keras-3.3.3/keras/_tf_keras/keras/config/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1143 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.825092 keras-3.3.3/keras/_tf_keras/keras/constraints/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      797 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.825258 keras-3.3.3/keras/_tf_keras/keras/datasets/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      454 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.825412 keras-3.3.3/keras/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.825576 keras-3.3.3/keras/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      182 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.825721 keras-3.3.3/keras/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      171 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.825866 keras-3.3.3/keras/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      172 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.826016 keras-3.3.3/keras/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.826168 keras-3.3.3/keras/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      219 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.826331 keras-3.3.3/keras/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      169 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.826482 keras-3.3.3/keras/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      280 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.826642 keras-3.3.3/keras/_tf_keras/keras/distribution/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      775 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.826797 keras-3.3.3/keras/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      536 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.826944 keras-3.3.3/keras/_tf_keras/keras/export/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      176 2024-04-26 23:19:30.000000 keras-3.3.3/keras/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.827122 keras-3.3.3/keras/_tf_keras/keras/initializers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2844 2024-04-26 23:19:30.000000 keras-3.3.3/keras/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.827317 keras-3.3.3/keras/_tf_keras/keras/layers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10090 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.827508 keras-3.3.3/keras/_tf_keras/keras/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      158 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.827649 keras-3.3.3/keras/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.827790 keras-3.3.3/keras/_tf_keras/keras/losses/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2888 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.827958 keras-3.3.3/keras/_tf_keras/keras/metrics/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4700 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.828122 keras-3.3.3/keras/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      636 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.828290 keras-3.3.3/keras/_tf_keras/keras/models/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      416 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.828446 keras-3.3.3/keras/_tf_keras/keras/ops/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8916 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.828631 keras-3.3.3/keras/_tf_keras/keras/ops/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      442 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.828792 keras-3.3.3/keras/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      556 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.828948 keras-3.3.3/keras/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1498 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.829094 keras-3.3.3/keras/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5727 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.829253 keras-3.3.3/keras/_tf_keras/keras/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      965 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.829395 keras-3.3.3/keras/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      516 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.829551 keras-3.3.3/keras/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      918 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.829712 keras-3.3.3/keras/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      530 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.829881 keras-3.3.3/keras/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1240 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.830079 keras-3.3.3/keras/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      385 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.830259 keras-3.3.3/keras/_tf_keras/keras/preprocessing/text/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      436 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/preprocessing/text/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.830413 keras-3.3.3/keras/_tf_keras/keras/quantizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      627 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.830574 keras-3.3.3/keras/_tf_keras/keras/random/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      628 2024-04-26 23:19:30.000000 keras-3.3.3/keras/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.830746 keras-3.3.3/keras/_tf_keras/keras/regularizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      819 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.830900 keras-3.3.3/keras/_tf_keras/keras/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      923 2024-04-26 23:19:30.000000 keras-3.3.3/keras/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.831070 keras-3.3.3/keras/_tf_keras/keras/tree/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      582 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.831217 keras-3.3.3/keras/_tf_keras/keras/utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2652 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.831375 keras-3.3.3/keras/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-26 23:19:29.000000 keras-3.3.3/keras/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.831547 keras-3.3.3/keras/api/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2058 2024-04-26 23:19:29.000000 keras-3.3.3/keras/api/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.831715 keras-3.3.3/keras/api/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1347 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/activations/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.831870 keras-3.3.3/keras/api/applications/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3295 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/applications/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.832019 keras-3.3.3/keras/api/applications/convnext/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      535 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/applications/convnext/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.832165 keras-3.3.3/keras/api/applications/densenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      414 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/applications/densenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.832311 keras-3.3.3/keras/api/applications/efficientnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      758 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/applications/efficientnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.832458 keras-3.3.3/keras/api/applications/efficientnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      733 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.832606 keras-3.3.3/keras/api/applications/imagenet_utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      258 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.832756 keras-3.3.3/keras/api/applications/inception_resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      341 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.832909 keras-3.3.3/keras/api/applications/inception_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/applications/inception_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.833058 keras-3.3.3/keras/api/applications/mobilenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/applications/mobilenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.833222 keras-3.3.3/keras/api/applications/mobilenet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.833384 keras-3.3.3/keras/api/applications/mobilenet_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      254 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.833544 keras-3.3.3/keras/api/applications/nasnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      351 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/applications/nasnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.833708 keras-3.3.3/keras/api/applications/resnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      397 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/applications/resnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.833860 keras-3.3.3/keras/api/applications/resnet50/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      293 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/applications/resnet50/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.834022 keras-3.3.3/keras/api/applications/resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      418 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.834181 keras-3.3.3/keras/api/applications/vgg16/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/applications/vgg16/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.834332 keras-3.3.3/keras/api/applications/vgg19/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/applications/vgg19/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.834473 keras-3.3.3/keras/api/applications/xception/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      299 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/applications/xception/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.834621 keras-3.3.3/keras/api/backend/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      883 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/backend/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.834777 keras-3.3.3/keras/api/callbacks/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1044 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/callbacks/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.834929 keras-3.3.3/keras/api/config/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1143 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/config/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.835081 keras-3.3.3/keras/api/constraints/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      797 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/constraints/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.835230 keras-3.3.3/keras/api/datasets/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      454 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/datasets/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.835384 keras-3.3.3/keras/api/datasets/boston_housing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.835542 keras-3.3.3/keras/api/datasets/california_housing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      182 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/datasets/california_housing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.835705 keras-3.3.3/keras/api/datasets/cifar10/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      171 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/datasets/cifar10/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.835859 keras-3.3.3/keras/api/datasets/cifar100/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      172 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/datasets/cifar100/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.836026 keras-3.3.3/keras/api/datasets/fashion_mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.836322 keras-3.3.3/keras/api/datasets/imdb/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      219 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/datasets/imdb/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.836535 keras-3.3.3/keras/api/datasets/mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      169 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/datasets/mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.836730 keras-3.3.3/keras/api/datasets/reuters/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      280 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/datasets/reuters/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.836920 keras-3.3.3/keras/api/distribution/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      775 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/distribution/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.837112 keras-3.3.3/keras/api/dtype_policies/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      536 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/dtype_policies/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.837285 keras-3.3.3/keras/api/export/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      176 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/export/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.837460 keras-3.3.3/keras/api/initializers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2844 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/initializers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.837640 keras-3.3.3/keras/api/layers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9963 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/layers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.837855 keras-3.3.3/keras/api/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      158 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.838031 keras-3.3.3/keras/api/legacy/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/legacy/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.838203 keras-3.3.3/keras/api/losses/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2381 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/losses/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.838369 keras-3.3.3/keras/api/metrics/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4239 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/metrics/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.838554 keras-3.3.3/keras/api/mixed_precision/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      636 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/mixed_precision/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.838738 keras-3.3.3/keras/api/models/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      416 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/models/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.838941 keras-3.3.3/keras/api/ops/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8916 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/ops/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.839141 keras-3.3.3/keras/api/ops/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      442 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/ops/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.839297 keras-3.3.3/keras/api/ops/linalg/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      556 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/ops/linalg/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.839464 keras-3.3.3/keras/api/ops/nn/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1498 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/ops/nn/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.839631 keras-3.3.3/keras/api/ops/numpy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5727 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/ops/numpy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.839802 keras-3.3.3/keras/api/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      965 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/optimizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.839989 keras-3.3.3/keras/api/optimizers/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      516 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/optimizers/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.840197 keras-3.3.3/keras/api/optimizers/schedules/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      918 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/optimizers/schedules/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.840367 keras-3.3.3/keras/api/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      453 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/preprocessing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.840785 keras-3.3.3/keras/api/preprocessing/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      379 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/preprocessing/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.840937 keras-3.3.3/keras/api/preprocessing/sequence/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      179 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.841089 keras-3.3.3/keras/api/quantizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      627 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/quantizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.841237 keras-3.3.3/keras/api/random/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      628 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/random/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.841436 keras-3.3.3/keras/api/regularizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      819 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/regularizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.841632 keras-3.3.3/keras/api/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      923 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.841822 keras-3.3.3/keras/api/tree/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      582 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/tree/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.841979 keras-3.3.3/keras/api/utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2652 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.842148 keras-3.3.3/keras/api/utils/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-26 23:13:01.000000 keras-3.3.3/keras/api/utils/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.842771 keras-3.3.3/keras/src/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      648 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.843098 keras-3.3.3/keras/src/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3540 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/activations/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12442 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/activations/activations.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1173 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/api_export.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.846059 keras-3.3.3/keras/src/applications/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/applications/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    24919 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/applications/convnext.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16848 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/applications/densenet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25274 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/applications/efficientnet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    40460 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16034 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14509 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15520 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/applications/inception_v3.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17168 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/applications/mobilenet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17934 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    23521 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    30694 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/applications/nasnet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19006 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/applications/resnet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6363 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9110 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/applications/vgg16.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9433 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/applications/vgg19.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12705 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/applications/xception.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.846559 keras-3.3.3/keras/src/backend/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1971 2024-04-20 18:16:39.000000 keras-3.3.3/keras/src/backend/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.847766 keras-3.3.3/keras/src/backend/common/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      583 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/common/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17099 2024-04-21 17:37:40.000000 keras-3.3.3/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9808 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3412 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/common/global_state.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8974 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2545 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3692 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    21446 2024-04-20 18:16:39.000000 keras-3.3.3/keras/src/backend/common/variables.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7139 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/config.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1056 2024-04-20 18:16:39.000000 keras-3.3.3/keras/src/backend/exports.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.850761 keras-3.3.3/keras/src/backend/jax/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1173 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12765 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/jax/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9679 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14746 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/jax/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       25 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/jax/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2049 2024-04-26 15:27:00.000000 keras-3.3.3/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8757 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/jax/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    28924 2024-04-25 23:45:18.000000 keras-3.3.3/keras/src/backend/jax/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    30920 2024-04-24 20:44:40.000000 keras-3.3.3/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3856 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3594 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/jax/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7552 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13804 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    36259 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.852823 keras-3.3.3/keras/src/backend/numpy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1012 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6855 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/numpy/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13086 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/numpy/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       27 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1964 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10586 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/numpy/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    30646 2024-04-25 23:45:18.000000 keras-3.3.3/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    28155 2024-04-24 20:44:35.000000 keras-3.3.3/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3961 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/numpy/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7652 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10738 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.855701 keras-3.3.3/keras/src/backend/tensorflow/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1458 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9444 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2747 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14197 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4639 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6161 2024-04-20 18:16:39.000000 keras-3.3.3/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11451 2024-04-20 18:16:39.000000 keras-3.3.3/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27369 2024-04-25 23:45:18.000000 keras-3.3.3/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    77857 2024-04-24 20:44:28.000000 keras-3.3.3/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9334 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6211 2024-04-20 18:16:39.000000 keras-3.3.3/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    34600 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    32268 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      170 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1993 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    33111 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.857938 keras-3.3.3/keras/src/backend/torch/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1892 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16088 2024-04-25 23:45:23.000000 keras-3.3.3/keras/src/backend/torch/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14001 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1865 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1801 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15073 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27095 2024-04-25 23:45:18.000000 keras-3.3.3/keras/src/backend/torch/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    47523 2024-04-24 20:41:34.000000 keras-3.3.3/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.860048 keras-3.3.3/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       78 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1672 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1041 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1889 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1483 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      150 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1041 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2421 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1803 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      783 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2053 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1175 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8292 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13704 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17577 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.862737 keras-3.3.3/keras/src/callbacks/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      922 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/callbacks/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7552 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9830 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/callbacks/callback.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5255 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3206 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8932 2024-04-25 23:45:18.000000 keras-3.3.3/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1301 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/callbacks/history.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3441 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2965 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18488 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3104 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5339 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2727 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6843 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26393 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      669 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/callbacks/terminate_on_nan.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.863051 keras-3.3.3/keras/src/constraints/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1715 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/constraints/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7333 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/constraints/constraints.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.864610 keras-3.3.3/keras/src/datasets/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      383 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/datasets/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2644 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3850 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/datasets/california_housing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      704 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/datasets/cifar.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3086 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/datasets/cifar10.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2914 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/datasets/cifar100.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2929 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7201 2024-04-23 17:54:22.000000 keras-3.3.3/keras/src/datasets/imdb.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2393 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/datasets/mnist.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7203 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/datasets/reuters.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.864933 keras-3.3.3/keras/src/distribution/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      718 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/distribution/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    31207 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/distribution/distribution_lib.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.865280 keras-3.3.3/keras/src/dtype_policies/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3506 2024-04-22 16:35:02.000000 keras-3.3.3/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12480 2024-04-22 16:35:02.000000 keras-3.3.3/keras/src/dtype_policies/dtype_policy.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.865646 keras-3.3.3/keras/src/export/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       54 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/export/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    32830 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/export/export_lib.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.866315 keras-3.3.3/keras/src/initializers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3958 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/initializers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4884 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2633 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/initializers/initializer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    23462 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/initializers/random_initializers.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.866825 keras-3.3.3/keras/src/layers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8848 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.867930 keras-3.3.3/keras/src/layers/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      272 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1236 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/activations/activation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      809 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/activations/elu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1900 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3453 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2670 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/activations/relu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2258 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/activations/softmax.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.868764 keras-3.3.3/keras/src/layers/attention/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4330 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11889 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/attention/attention.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17952 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    28353 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/attention/multi_head_attention.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.871200 keras-3.3.3/keras/src/layers/convolutional/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17263 2024-04-22 16:35:02.000000 keras-3.3.3/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10695 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11617 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12643 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7300 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5571 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5670 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5691 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5893 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5897 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5999 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6087 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6450 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6531 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/convolutional/separable_conv2d.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.872673 keras-3.3.3/keras/src/layers/core/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/core/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25225 2024-04-24 18:01:17.000000 keras-3.3.3/keras/src/layers/core/dense.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    42009 2024-04-24 18:01:17.000000 keras-3.3.3/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17438 2024-04-24 18:01:17.000000 keras-3.3.3/keras/src/layers/core/embedding.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      817 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/core/identity.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5107 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8989 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2629 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/core/masking.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1535 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9827 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/input_spec.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    63910 2024-04-24 18:01:17.000000 keras-3.3.3/keras/src/layers/layer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.874348 keras-3.3.3/keras/src/layers/merging/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2150 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/merging/add.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2214 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/merging/average.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9249 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6586 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12807 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/merging/dot.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2214 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2212 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2211 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2684 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.875380 keras-3.3.3/keras/src/layers/normalization/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13440 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8534 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9836 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4306 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1831 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/normalization/unit_normalization.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.878003 keras-3.3.3/keras/src/layers/pooling/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3344 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4150 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3235 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1460 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2425 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3131 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2469 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2603 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2357 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2451 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2585 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3343 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4125 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3225 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/pooling/max_pooling3d.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.882453 keras-3.3.3/keras/src/layers/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14572 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8705 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5489 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13145 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    29613 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8317 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10936 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    41399 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18458 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13920 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6463 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3814 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6315 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3805 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9645 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10614 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10820 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2177 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5349 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17734 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27820 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2133 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.883613 keras-3.3.3/keras/src/layers/regularization/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1198 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3594 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2978 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2041 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2089 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7300 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/regularization/spatial_dropout.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.886254 keras-3.3.3/keras/src/layers/reshaping/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2760 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9044 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11265 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3059 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2087 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1335 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2322 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1592 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5992 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4910 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2106 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4646 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5060 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/reshaping/zero_padding3d.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.888525 keras-3.3.3/keras/src/layers/rnn/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13235 2024-04-26 18:29:16.000000 keras-3.3.3/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27242 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8294 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8379 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8287 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2132 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27701 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26544 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19159 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17537 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4943 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4797 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/layers/rnn/time_distributed.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.889162 keras-3.3.3/keras/src/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/legacy/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    70241 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/legacy/backend.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8412 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/legacy/layers.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      523 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/legacy/losses.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.889794 keras-3.3.3/keras/src/legacy/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    65545 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11172 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11110 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.890742 keras-3.3.3/keras/src/legacy/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7296 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    22750 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      485 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9275 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    21808 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.891229 keras-3.3.3/keras/src/losses/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6363 2024-04-22 16:35:02.000000 keras-3.3.3/keras/src/losses/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6013 2024-04-24 18:01:17.000000 keras-3.3.3/keras/src/losses/loss.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    69104 2024-04-25 23:45:18.000000 keras-3.3.3/keras/src/losses/losses.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.893122 keras-3.3.3/keras/src/metrics/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7198 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/metrics/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15604 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    61579 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11743 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3255 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26976 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8309 2024-04-24 18:01:17.000000 keras-3.3.3/keras/src/metrics/metric.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26611 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10692 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7212 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19818 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/metrics/regression_metrics.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.894102 keras-3.3.3/keras/src/models/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      143 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/models/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15386 2024-04-25 23:45:23.000000 keras-3.3.3/keras/src/models/cloning.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    32507 2024-04-24 18:01:17.000000 keras-3.3.3/keras/src/models/functional.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    22763 2024-04-24 18:46:18.000000 keras-3.3.3/keras/src/models/model.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13067 2024-04-24 18:01:17.000000 keras-3.3.3/keras/src/models/sequential.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2181 2024-04-24 19:06:31.000000 keras-3.3.3/keras/src/models/variable_mapping.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.896232 keras-3.3.3/keras/src/ops/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      644 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/ops/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    22866 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/ops/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15497 2024-04-25 23:45:23.000000 keras-3.3.3/keras/src/ops/function.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    37275 2024-04-26 21:48:49.000000 keras-3.3.3/keras/src/ops/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18342 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/ops/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    30618 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/ops/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    67520 2024-04-25 23:45:18.000000 keras-3.3.3/keras/src/ops/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5583 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/ops/node.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)   195656 2024-04-24 21:28:45.000000 keras-3.3.3/keras/src/ops/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10732 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/ops/operation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13759 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/ops/operation_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1694 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/ops/symbolic_arguments.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.898645 keras-3.3.3/keras/src/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3931 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/optimizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4759 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7637 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3918 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5909 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/optimizers/adam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5083 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/optimizers/adamax.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3784 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/optimizers/adamw.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    40536 2024-04-24 18:01:17.000000 keras-3.3.3/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9099 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4969 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/optimizers/lion.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11553 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5926 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/optimizers/nadam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      813 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6003 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/optimizers/rmsprop.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.898969 keras-3.3.3/keras/src/optimizers/schedules/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      546 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    35507 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4556 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/optimizers/sgd.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.899284 keras-3.3.3/keras/src/quantizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1784 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/quantizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4810 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/quantizers/quantizers.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.899771 keras-3.3.3/keras/src/random/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      420 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/random/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13438 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/random/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4905 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/random/seed_generator.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.900087 keras-3.3.3/keras/src/regularizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1731 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/regularizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11799 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/regularizers/regularizers.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.901148 keras-3.3.3/keras/src/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      614 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/saving/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1285 2024-04-24 18:08:42.000000 keras-3.3.3/keras/src/saving/keras_saveable.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7358 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/saving/object_registration.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9737 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/saving/saving_api.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26931 2024-04-24 18:46:38.000000 keras-3.3.3/keras/src/saving/saving_lib.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    29052 2024-04-20 18:16:39.000000 keras-3.3.3/keras/src/saving/serialization_lib.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.901670 keras-3.3.3/keras/src/testing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      266 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/testing/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27552 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/testing/test_case.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6197 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/testing/test_utils.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.902340 keras-3.3.3/keras/src/trainers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/trainers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25904 2024-04-26 23:02:57.000000 keras-3.3.3/keras/src/trainers/compile_utils.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.903919 keras-3.3.3/keras/src/trainers/data_adapters/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5767 2024-04-26 21:48:49.000000 keras-3.3.3/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14323 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17071 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3101 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9717 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2863 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    20637 2024-04-26 21:48:49.000000 keras-3.3.3/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5224 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2643 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3923 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    46449 2024-04-20 18:16:39.000000 keras-3.3.3/keras/src/trainers/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.904557 keras-3.3.3/keras/src/tree/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      521 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/tree/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4970 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/tree/dmtree_impl.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11138 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/tree/optree_impl.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9397 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/tree/tree_api.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.909304 keras-3.3.3/keras/src/utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1423 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2876 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/argument_validation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15102 2024-04-26 21:46:27.000000 keras-3.3.3/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4130 2024-04-20 18:16:39.000000 keras-3.3.3/keras/src/utils/backend_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1442 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/code_stats.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    28554 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1483 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16371 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/file_utils.py
+-rwxr-xr-x   0 fchollet (337002) primarygroup (89939)    16629 2024-04-26 21:47:39.000000 keras-3.3.3/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16544 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/image_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3491 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/io_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26570 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/jax_layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      263 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/jax_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15635 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/model_visualization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1276 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/module_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1776 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/naming.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4571 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10349 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/progbar.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4003 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/python_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1677 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/rng_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4714 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14512 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/summary_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10675 2024-04-26 21:47:10.000000 keras-3.3.3/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4630 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/tf_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9842 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4991 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/torch_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8997 2024-04-20 16:30:07.000000 keras-3.3.3/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8980 2024-04-21 17:38:44.000000 keras-3.3.3/keras/src/utils/tracking.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      189 2024-04-26 23:19:31.000000 keras-3.3.3/keras/src/version.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-26 23:19:33.909668 keras-3.3.3/keras.egg-info/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5731 2024-04-26 23:19:33.000000 keras-3.3.3/keras.egg-info/PKG-INFO
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    20379 2024-04-26 23:19:33.000000 keras-3.3.3/keras.egg-info/SOURCES.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-26 23:19:33.000000 keras-3.3.3/keras.egg-info/dependency_links.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       47 2024-04-26 23:19:33.000000 keras-3.3.3/keras.egg-info/requires.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        6 2024-04-26 23:19:33.000000 keras-3.3.3/keras.egg-info/top_level.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       38 2024-04-26 23:19:33.910374 keras-3.3.3/setup.cfg
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1769 2024-04-26 23:19:29.000000 keras-3.3.3/setup.py
```

### Comparing `keras-3.3.2/PKG-INFO` & `keras-3.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras
-Version: 3.3.2
+Version: 3.3.3
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-3.3.2/README.md` & `keras-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/__init__.py` & `keras-3.3.3/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,53 +11,43 @@
 from keras.api import constraints
 from keras.api import datasets
 from keras.api import distribution
 from keras.api import dtype_policies
 from keras.api import export
 from keras.api import initializers
 from keras.api import legacy
-from keras.api import metrics
 from keras.api import mixed_precision
 from keras.api import models
 from keras.api import ops
 from keras.api import optimizers
 from keras.api import quantizers
 from keras.api import random
 from keras.api import regularizers
 from keras.api import tree
 from keras.api import utils
+from keras._tf_keras.keras import backend
+from keras._tf_keras.keras import layers
+from keras._tf_keras.keras import losses
+from keras._tf_keras.keras import metrics
+from keras._tf_keras.keras import preprocessing
 from keras.src.backend.common.keras_tensor import KerasTensor
 from keras.src.backend.common.stateless_scope import StatelessScope
 from keras.src.backend.exports import Variable
 from keras.src.backend.exports import device
 from keras.src.backend.exports import name_scope
 from keras.src.dtype_policies.dtype_policy import DTypePolicy
 from keras.src.dtype_policies.dtype_policy import FloatDTypePolicy
-from keras.src.dtype_policies.dtype_policy import QuantizedDTypePolicy
 from keras.src.initializers.initializer import Initializer
 from keras.src.layers.core.input_layer import Input
 from keras.src.layers.input_spec import InputSpec
 from keras.src.layers.layer import Layer
 from keras.src.losses.loss import Loss
 from keras.src.metrics.metric import Metric
 from keras.src.models.model import Model
 from keras.src.models.sequential import Sequential
 from keras.src.ops.function import Function
 from keras.src.ops.operation import Operation
 from keras.src.optimizers.optimizer import Optimizer
-from keras.src.quantizers.quantizers import AbsMaxQuantizer
 from keras.src.quantizers.quantizers import Quantizer
 from keras.src.regularizers.regularizers import Regularizer
+from keras.src.version import __version__
 from keras.src.version import version
-
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-
-from keras._tf_keras.keras import backend
-from keras._tf_keras.keras import layers
-from keras._tf_keras.keras import losses
-from keras._tf_keras.keras import metrics
-from keras._tf_keras.keras import preprocessing
```

### Comparing `keras-3.3.2/keras/_tf_keras/keras/activations/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/applications/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/applications/convnext/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/backend/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/backend/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,14 @@
 from keras.src.backend.config import backend
 from keras.src.backend.config import epsilon
 from keras.src.backend.config import floatx
 from keras.src.backend.config import image_data_format
 from keras.src.backend.config import set_epsilon
 from keras.src.backend.config import set_floatx
 from keras.src.backend.config import set_image_data_format
-from keras.src.utils.naming import get_uid
-
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-
 from keras.src.legacy.backend import abs
 from keras.src.legacy.backend import all
 from keras.src.legacy.backend import any
 from keras.src.legacy.backend import arange
 from keras.src.legacy.backend import argmax
 from keras.src.legacy.backend import argmin
 from keras.src.legacy.backend import batch_dot
@@ -145,7 +136,8 @@
 from keras.src.legacy.backend import update
 from keras.src.legacy.backend import update_add
 from keras.src.legacy.backend import update_sub
 from keras.src.legacy.backend import var
 from keras.src.legacy.backend import variable
 from keras.src.legacy.backend import zeros
 from keras.src.legacy.backend import zeros_like
+from keras.src.utils.naming import get_uid
```

### Comparing `keras-3.3.2/keras/_tf_keras/keras/callbacks/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/config/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/constraints/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/distribution/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/dtype_policies/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/initializers/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/layers/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/layers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,14 @@
 from keras.src.layers.preprocessing.rescaling import Rescaling
 from keras.src.layers.preprocessing.resizing import Resizing
 from keras.src.layers.preprocessing.string_lookup import StringLookup
 from keras.src.layers.preprocessing.text_vectorization import TextVectorization
 from keras.src.layers.regularization.activity_regularization import (
     ActivityRegularization,
 )
-from keras.src.layers.regularization.alpha_dropout import AlphaDropout
 from keras.src.layers.regularization.dropout import Dropout
 from keras.src.layers.regularization.gaussian_dropout import GaussianDropout
 from keras.src.layers.regularization.gaussian_noise import GaussianNoise
 from keras.src.layers.regularization.spatial_dropout import SpatialDropout1D
 from keras.src.layers.regularization.spatial_dropout import SpatialDropout2D
 from keras.src.layers.regularization.spatial_dropout import SpatialDropout3D
 from keras.src.layers.reshaping.cropping1d import Cropping1D
@@ -186,22 +185,14 @@
 from keras.src.layers.rnn.lstm import LSTM
 from keras.src.layers.rnn.lstm import LSTMCell
 from keras.src.layers.rnn.rnn import RNN
 from keras.src.layers.rnn.simple_rnn import SimpleRNN
 from keras.src.layers.rnn.simple_rnn import SimpleRNNCell
 from keras.src.layers.rnn.stacked_rnn_cells import StackedRNNCells
 from keras.src.layers.rnn.time_distributed import TimeDistributed
-from keras.src.utils.jax_layer import FlaxLayer
-from keras.src.utils.jax_layer import JaxLayer
-from keras.src.utils.torch_utils import TorchModuleWrapper
-
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-
 from keras.src.legacy.layers import AlphaDropout
 from keras.src.legacy.layers import RandomHeight
 from keras.src.legacy.layers import RandomWidth
 from keras.src.legacy.layers import ThresholdedReLU
+from keras.src.utils.jax_layer import FlaxLayer
+from keras.src.utils.jax_layer import JaxLayer
+from keras.src.utils.torch_utils import TorchModuleWrapper
```

### Comparing `keras-3.3.2/keras/_tf_keras/keras/losses/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/losses/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
+from keras.src.legacy.losses import Reduction
 from keras.src.losses import deserialize
 from keras.src.losses import get
 from keras.src.losses import serialize
 from keras.src.losses.loss import Loss
+from keras.src.losses.losses import CTC
 from keras.src.losses.losses import BinaryCrossentropy
 from keras.src.losses.losses import BinaryFocalCrossentropy
-from keras.src.losses.losses import CTC
 from keras.src.losses.losses import CategoricalCrossentropy
 from keras.src.losses.losses import CategoricalFocalCrossentropy
 from keras.src.losses.losses import CategoricalHinge
 from keras.src.losses.losses import CosineSimilarity
 from keras.src.losses.losses import Dice
 from keras.src.losses.losses import Hinge
 from keras.src.losses.losses import Huber
@@ -34,38 +35,23 @@
 from keras.src.losses.losses import categorical_focal_crossentropy
 from keras.src.losses.losses import categorical_hinge
 from keras.src.losses.losses import cosine_similarity
 from keras.src.losses.losses import ctc
 from keras.src.losses.losses import dice
 from keras.src.losses.losses import hinge
 from keras.src.losses.losses import huber
-from keras.src.losses.losses import kl_divergence
-from keras.src.losses.losses import log_cosh
-from keras.src.losses.losses import mean_absolute_error
-from keras.src.losses.losses import mean_absolute_percentage_error
-from keras.src.losses.losses import mean_squared_error
-from keras.src.losses.losses import mean_squared_logarithmic_error
-from keras.src.losses.losses import poisson
-from keras.src.losses.losses import sparse_categorical_crossentropy
-from keras.src.losses.losses import squared_hinge
-from keras.src.losses.losses import tversky
-
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-
-from keras.src.legacy.losses import Reduction
 from keras.src.losses.losses import kl_divergence as KLD
 from keras.src.losses.losses import kl_divergence as kld
 from keras.src.losses.losses import kl_divergence as kullback_leibler_divergence
 from keras.src.losses.losses import log_cosh as logcosh
 from keras.src.losses.losses import mean_absolute_error as MAE
 from keras.src.losses.losses import mean_absolute_error as mae
 from keras.src.losses.losses import mean_absolute_percentage_error as MAPE
 from keras.src.losses.losses import mean_absolute_percentage_error as mape
 from keras.src.losses.losses import mean_squared_error as MSE
 from keras.src.losses.losses import mean_squared_error as mse
 from keras.src.losses.losses import mean_squared_logarithmic_error as MSLE
 from keras.src.losses.losses import mean_squared_logarithmic_error as msle
+from keras.src.losses.losses import poisson
+from keras.src.losses.losses import sparse_categorical_crossentropy
+from keras.src.losses.losses import squared_hinge
+from keras.src.losses.losses import tversky
```

### Comparing `keras-3.3.2/keras/_tf_keras/keras/metrics/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/metrics/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,26 @@
 from keras.src.losses.losses import binary_crossentropy
 from keras.src.losses.losses import binary_focal_crossentropy
 from keras.src.losses.losses import categorical_crossentropy
 from keras.src.losses.losses import categorical_focal_crossentropy
 from keras.src.losses.losses import categorical_hinge
 from keras.src.losses.losses import hinge
 from keras.src.losses.losses import huber
-from keras.src.losses.losses import kl_divergence
-from keras.src.losses.losses import log_cosh
-from keras.src.losses.losses import mean_absolute_error
-from keras.src.losses.losses import mean_absolute_percentage_error
-from keras.src.losses.losses import mean_squared_error
-from keras.src.losses.losses import mean_squared_logarithmic_error
+from keras.src.losses.losses import kl_divergence as KLD
+from keras.src.losses.losses import kl_divergence as kld
+from keras.src.losses.losses import kl_divergence as kullback_leibler_divergence
+from keras.src.losses.losses import log_cosh as logcosh
+from keras.src.losses.losses import mean_absolute_error as MAE
+from keras.src.losses.losses import mean_absolute_error as mae
+from keras.src.losses.losses import mean_absolute_percentage_error as MAPE
+from keras.src.losses.losses import mean_absolute_percentage_error as mape
+from keras.src.losses.losses import mean_squared_error as MSE
+from keras.src.losses.losses import mean_squared_error as mse
+from keras.src.losses.losses import mean_squared_logarithmic_error as MSLE
+from keras.src.losses.losses import mean_squared_logarithmic_error as msle
 from keras.src.losses.losses import poisson
 from keras.src.losses.losses import sparse_categorical_crossentropy
 from keras.src.losses.losses import squared_hinge
 from keras.src.metrics import deserialize
 from keras.src.metrics import get
 from keras.src.metrics import serialize
 from keras.src.metrics.accuracy_metrics import Accuracy
@@ -70,27 +76,7 @@
 from keras.src.metrics.regression_metrics import LogCoshError
 from keras.src.metrics.regression_metrics import MeanAbsoluteError
 from keras.src.metrics.regression_metrics import MeanAbsolutePercentageError
 from keras.src.metrics.regression_metrics import MeanSquaredError
 from keras.src.metrics.regression_metrics import MeanSquaredLogarithmicError
 from keras.src.metrics.regression_metrics import R2Score
 from keras.src.metrics.regression_metrics import RootMeanSquaredError
-
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-
-from keras.src.losses.losses import kl_divergence as KLD
-from keras.src.losses.losses import kl_divergence as kld
-from keras.src.losses.losses import kl_divergence as kullback_leibler_divergence
-from keras.src.losses.losses import log_cosh as logcosh
-from keras.src.losses.losses import mean_absolute_error as MAE
-from keras.src.losses.losses import mean_absolute_error as mae
-from keras.src.losses.losses import mean_absolute_percentage_error as MAPE
-from keras.src.losses.losses import mean_absolute_percentage_error as mape
-from keras.src.losses.losses import mean_squared_error as MSE
-from keras.src.losses.losses import mean_squared_error as mse
-from keras.src.losses.losses import mean_squared_logarithmic_error as MSLE
-from keras.src.losses.losses import mean_squared_logarithmic_error as msle
```

### Comparing `keras-3.3.2/keras/_tf_keras/keras/mixed_precision/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/ops/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/ops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 from keras.src.ops.nn import log_sigmoid
 from keras.src.ops.nn import log_softmax
 from keras.src.ops.nn import max_pool
 from keras.src.ops.nn import moments
 from keras.src.ops.nn import multi_hot
 from keras.src.ops.nn import normalize
 from keras.src.ops.nn import one_hot
+from keras.src.ops.nn import psnr
 from keras.src.ops.nn import relu
 from keras.src.ops.nn import relu6
 from keras.src.ops.nn import selu
 from keras.src.ops.nn import separable_conv
 from keras.src.ops.nn import sigmoid
 from keras.src.ops.nn import silu
 from keras.src.ops.nn import silu as swish
@@ -192,14 +193,15 @@
 from keras.src.ops.numpy import roll
 from keras.src.ops.numpy import round
 from keras.src.ops.numpy import select
 from keras.src.ops.numpy import sign
 from keras.src.ops.numpy import sin
 from keras.src.ops.numpy import sinh
 from keras.src.ops.numpy import size
+from keras.src.ops.numpy import slogdet
 from keras.src.ops.numpy import sort
 from keras.src.ops.numpy import split
 from keras.src.ops.numpy import sqrt
 from keras.src.ops.numpy import square
 from keras.src.ops.numpy import squeeze
 from keras.src.ops.numpy import stack
 from keras.src.ops.numpy import std
```

### Comparing `keras-3.3.2/keras/_tf_keras/keras/ops/linalg/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/ops/nn/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/ops/nn/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from keras.src.ops.nn import log_sigmoid
 from keras.src.ops.nn import log_softmax
 from keras.src.ops.nn import max_pool
 from keras.src.ops.nn import moments
 from keras.src.ops.nn import multi_hot
 from keras.src.ops.nn import normalize
 from keras.src.ops.nn import one_hot
+from keras.src.ops.nn import psnr
 from keras.src.ops.nn import relu
 from keras.src.ops.nn import relu6
 from keras.src.ops.nn import selu
 from keras.src.ops.nn import separable_conv
 from keras.src.ops.nn import sigmoid
 from keras.src.ops.nn import silu
 from keras.src.ops.nn import silu as swish
```

### Comparing `keras-3.3.2/keras/_tf_keras/keras/ops/numpy/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
 from keras.src.ops.numpy import roll
 from keras.src.ops.numpy import round
 from keras.src.ops.numpy import select
 from keras.src.ops.numpy import sign
 from keras.src.ops.numpy import sin
 from keras.src.ops.numpy import sinh
 from keras.src.ops.numpy import size
+from keras.src.ops.numpy import slogdet
 from keras.src.ops.numpy import sort
 from keras.src.ops.numpy import split
 from keras.src.ops.numpy import sqrt
 from keras.src.ops.numpy import square
 from keras.src.ops.numpy import squeeze
 from keras.src.ops.numpy import stack
 from keras.src.ops.numpy import std
```

### Comparing `keras-3.3.2/keras/_tf_keras/keras/optimizers/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/preprocessing/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/preprocessing/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,23 +2,13 @@
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
 from keras._tf_keras.keras.preprocessing import image
 from keras._tf_keras.keras.preprocessing import sequence
+from keras._tf_keras.keras.preprocessing import text
 from keras.src.utils.image_dataset_utils import image_dataset_from_directory
 from keras.src.utils.text_dataset_utils import text_dataset_from_directory
 from keras.src.utils.timeseries_dataset_utils import (
     timeseries_dataset_from_array,
 )
-
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-
-from keras._tf_keras.keras.preprocessing import image
-from keras._tf_keras.keras.preprocessing import sequence
-from keras._tf_keras.keras.preprocessing import text
```

### Comparing `keras-3.3.2/keras/_tf_keras/keras/preprocessing/image/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/preprocessing/image/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-from keras.src.utils.image_utils import array_to_img
-from keras.src.utils.image_utils import img_to_array
-from keras.src.utils.image_utils import load_img
-from keras.src.utils.image_utils import save_img
-from keras.src.utils.image_utils import smart_resize
-
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-
 from keras.src.legacy.preprocessing.image import DirectoryIterator
 from keras.src.legacy.preprocessing.image import ImageDataGenerator
 from keras.src.legacy.preprocessing.image import Iterator
 from keras.src.legacy.preprocessing.image import NumpyArrayIterator
 from keras.src.legacy.preprocessing.image import apply_affine_transform
 from keras.src.legacy.preprocessing.image import apply_brightness_shift
 from keras.src.legacy.preprocessing.image import apply_channel_shift
 from keras.src.legacy.preprocessing.image import random_brightness
 from keras.src.legacy.preprocessing.image import random_channel_shift
 from keras.src.legacy.preprocessing.image import random_rotation
 from keras.src.legacy.preprocessing.image import random_shear
 from keras.src.legacy.preprocessing.image import random_shift
 from keras.src.legacy.preprocessing.image import random_zoom
+from keras.src.utils.image_utils import array_to_img
+from keras.src.utils.image_utils import img_to_array
+from keras.src.utils.image_utils import load_img
+from keras.src.utils.image_utils import save_img
+from keras.src.utils.image_utils import smart_resize
```

### Comparing `keras-3.3.2/keras/_tf_keras/keras/quantizers/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/random/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/regularizers/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/saving/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/tree/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/_tf_keras/keras/utils/__init__.py` & `keras-3.3.3/keras/_tf_keras/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/__init__.py` & `keras-3.3.3/keras/api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
+
 from keras.api import activations
 from keras.api import applications
 from keras.api import backend
 from keras.api import callbacks
 from keras.api import config
 from keras.api import constraints
 from keras.api import datasets
```

### Comparing `keras-3.3.2/keras/api/activations/__init__.py` & `keras-3.3.3/keras/api/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/applications/__init__.py` & `keras-3.3.3/keras/api/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/applications/convnext/__init__.py` & `keras-3.3.3/keras/api/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/applications/efficientnet/__init__.py` & `keras-3.3.3/keras/api/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/applications/efficientnet_v2/__init__.py` & `keras-3.3.3/keras/api/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/backend/__init__.py` & `keras-3.3.3/keras/api/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/callbacks/__init__.py` & `keras-3.3.3/keras/api/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/config/__init__.py` & `keras-3.3.3/keras/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/constraints/__init__.py` & `keras-3.3.3/keras/api/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/distribution/__init__.py` & `keras-3.3.3/keras/api/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/dtype_policies/__init__.py` & `keras-3.3.3/keras/api/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/initializers/__init__.py` & `keras-3.3.3/keras/api/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/layers/__init__.py` & `keras-3.3.3/keras/api/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/losses/__init__.py` & `keras-3.3.3/keras/api/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/metrics/__init__.py` & `keras-3.3.3/keras/api/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/mixed_precision/__init__.py` & `keras-3.3.3/keras/api/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/ops/__init__.py` & `keras-3.3.3/keras/api/ops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 from keras.src.ops.nn import log_sigmoid
 from keras.src.ops.nn import log_softmax
 from keras.src.ops.nn import max_pool
 from keras.src.ops.nn import moments
 from keras.src.ops.nn import multi_hot
 from keras.src.ops.nn import normalize
 from keras.src.ops.nn import one_hot
+from keras.src.ops.nn import psnr
 from keras.src.ops.nn import relu
 from keras.src.ops.nn import relu6
 from keras.src.ops.nn import selu
 from keras.src.ops.nn import separable_conv
 from keras.src.ops.nn import sigmoid
 from keras.src.ops.nn import silu
 from keras.src.ops.nn import silu as swish
@@ -192,14 +193,15 @@
 from keras.src.ops.numpy import roll
 from keras.src.ops.numpy import round
 from keras.src.ops.numpy import select
 from keras.src.ops.numpy import sign
 from keras.src.ops.numpy import sin
 from keras.src.ops.numpy import sinh
 from keras.src.ops.numpy import size
+from keras.src.ops.numpy import slogdet
 from keras.src.ops.numpy import sort
 from keras.src.ops.numpy import split
 from keras.src.ops.numpy import sqrt
 from keras.src.ops.numpy import square
 from keras.src.ops.numpy import squeeze
 from keras.src.ops.numpy import stack
 from keras.src.ops.numpy import std
```

### Comparing `keras-3.3.2/keras/api/ops/linalg/__init__.py` & `keras-3.3.3/keras/api/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/ops/nn/__init__.py` & `keras-3.3.3/keras/api/ops/nn/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from keras.src.ops.nn import log_sigmoid
 from keras.src.ops.nn import log_softmax
 from keras.src.ops.nn import max_pool
 from keras.src.ops.nn import moments
 from keras.src.ops.nn import multi_hot
 from keras.src.ops.nn import normalize
 from keras.src.ops.nn import one_hot
+from keras.src.ops.nn import psnr
 from keras.src.ops.nn import relu
 from keras.src.ops.nn import relu6
 from keras.src.ops.nn import selu
 from keras.src.ops.nn import separable_conv
 from keras.src.ops.nn import sigmoid
 from keras.src.ops.nn import silu
 from keras.src.ops.nn import silu as swish
```

### Comparing `keras-3.3.2/keras/api/ops/numpy/__init__.py` & `keras-3.3.3/keras/api/ops/numpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
 from keras.src.ops.numpy import roll
 from keras.src.ops.numpy import round
 from keras.src.ops.numpy import select
 from keras.src.ops.numpy import sign
 from keras.src.ops.numpy import sin
 from keras.src.ops.numpy import sinh
 from keras.src.ops.numpy import size
+from keras.src.ops.numpy import slogdet
 from keras.src.ops.numpy import sort
 from keras.src.ops.numpy import split
 from keras.src.ops.numpy import sqrt
 from keras.src.ops.numpy import square
 from keras.src.ops.numpy import squeeze
 from keras.src.ops.numpy import stack
 from keras.src.ops.numpy import std
```

### Comparing `keras-3.3.2/keras/api/optimizers/__init__.py` & `keras-3.3.3/keras/api/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/optimizers/legacy/__init__.py` & `keras-3.3.3/keras/api/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/optimizers/schedules/__init__.py` & `keras-3.3.3/keras/api/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/quantizers/__init__.py` & `keras-3.3.3/keras/api/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/random/__init__.py` & `keras-3.3.3/keras/api/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/regularizers/__init__.py` & `keras-3.3.3/keras/api/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/saving/__init__.py` & `keras-3.3.3/keras/api/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/tree/__init__.py` & `keras-3.3.3/keras/api/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/api/utils/__init__.py` & `keras-3.3.3/keras/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/__init__.py` & `keras-3.3.3/keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/activations/__init__.py` & `keras-3.3.3/keras/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/activations/activations.py` & `keras-3.3.3/keras/src/activations/activations.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/api_export.py` & `keras-3.3.3/keras/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/applications/convnext.py` & `keras-3.3.3/keras/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/applications/densenet.py` & `keras-3.3.3/keras/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/applications/efficientnet.py` & `keras-3.3.3/keras/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/applications/efficientnet_v2.py` & `keras-3.3.3/keras/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/applications/imagenet_utils.py` & `keras-3.3.3/keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/applications/inception_resnet_v2.py` & `keras-3.3.3/keras/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/applications/inception_v3.py` & `keras-3.3.3/keras/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/applications/mobilenet.py` & `keras-3.3.3/keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/applications/mobilenet_v2.py` & `keras-3.3.3/keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/applications/mobilenet_v3.py` & `keras-3.3.3/keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/applications/nasnet.py` & `keras-3.3.3/keras/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/applications/resnet.py` & `keras-3.3.3/keras/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/applications/resnet_v2.py` & `keras-3.3.3/keras/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/applications/vgg16.py` & `keras-3.3.3/keras/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/applications/vgg19.py` & `keras-3.3.3/keras/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/applications/xception.py` & `keras-3.3.3/keras/src/applications/xception.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/__init__.py` & `keras-3.3.3/keras/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/common/__init__.py` & `keras-3.3.3/keras/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/common/backend_utils.py` & `keras-3.3.3/keras/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/common/dtypes.py` & `keras-3.3.3/keras/src/backend/common/dtypes.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/common/global_state.py` & `keras-3.3.3/keras/src/backend/common/global_state.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/common/keras_tensor.py` & `keras-3.3.3/keras/src/backend/common/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/common/name_scope.py` & `keras-3.3.3/keras/src/backend/common/name_scope.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/common/stateless_scope.py` & `keras-3.3.3/keras/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/common/variables.py` & `keras-3.3.3/keras/src/backend/common/variables.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/config.py` & `keras-3.3.3/keras/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/exports.py` & `keras-3.3.3/keras/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/jax/__init__.py` & `keras-3.3.3/keras/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/jax/core.py` & `keras-3.3.3/keras/src/backend/jax/core.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/jax/distribution_lib.py` & `keras-3.3.3/keras/src/backend/jax/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/jax/image.py` & `keras-3.3.3/keras/src/backend/jax/image.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/jax/linalg.py` & `keras-3.3.3/keras/src/backend/jax/linalg.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,19 +7,26 @@
 from keras.src.backend.common import dtypes
 from keras.src.backend.jax.core import cast
 from keras.src.backend.jax.core import convert_to_tensor
 
 
 def cholesky(a):
     out = jnp.linalg.cholesky(a)
-    if jnp.any(jnp.isnan(out)):
-        raise ValueError(
-            "Cholesky decomposition failed. "
-            "The input might not be a valid positive definite matrix."
-        )
+    try:
+        # In eager mode, raise for nan to
+        # achieve behavior consistency with numpy
+        if jnp.any(jnp.isnan(out)):
+            raise ValueError(
+                "Cholesky decomposition failed. "
+                "The input might not be a valid "
+                "positive definite matrix."
+            )
+    except jax.errors.TracerBoolConversionError:
+        # Cannot raise for nan in tracing mode
+        pass
     return out
 
 
 def det(a):
     return jnp.linalg.det(a)
```

### Comparing `keras-3.3.2/keras/src/backend/jax/math.py` & `keras-3.3.3/keras/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/jax/nn.py` & `keras-3.3.3/keras/src/backend/jax/nn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+import builtins
+import math
+
 import jax
 import jax.experimental.sparse as jax_sparse
 import jax.numpy as jnp
-import numpy as np
 from jax import lax
 from jax import nn as jnn
 
-from keras.src.backend import standardize_data_format
-from keras.src.backend import standardize_dtype
+from keras.src import backend
 from keras.src.backend.common.backend_utils import (
     compute_conv_transpose_padding_args_for_jax,
 )
-from keras.src.backend.config import epsilon
 from keras.src.backend.jax.core import cast
 from keras.src.backend.jax.core import convert_to_tensor
 
 
 def relu(x):
     x = convert_to_tensor(x)
     return jnn.relu(x)
@@ -153,15 +153,15 @@
 def max_pool(
     inputs,
     pool_size,
     strides=None,
     padding="valid",
     data_format=None,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     num_spatial_dims = inputs.ndim - 2
     pool_size = _convert_to_spatial_operand(
         pool_size, num_spatial_dims, data_format
     )
     strides = pool_size if strides is None else strides
     strides = _convert_to_spatial_operand(
         strides, num_spatial_dims, data_format
@@ -172,28 +172,28 @@
 def average_pool(
     inputs,
     pool_size,
     strides,
     padding,
     data_format=None,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     num_spatial_dims = inputs.ndim - 2
     pool_size = _convert_to_spatial_operand(
         pool_size, num_spatial_dims, data_format
     )
     strides = pool_size if strides is None else strides
     strides = _convert_to_spatial_operand(
         strides, num_spatial_dims, data_format
     )
 
     pooled = _pool(inputs, 0.0, lax.add, pool_size, strides, padding)
     if padding == "valid":
         # Avoid the extra reduce_window.
-        return pooled / np.prod(pool_size)
+        return pooled / math.prod(pool_size)
     else:
         # Count the number of valid entries at each input point, then use that
         # for computing average. Assumes that any two arrays of same shape will
         # be padded the same. Avoid broadcasting on axis where pooling is
         # skipped.
         shape = [
             (a if b != 1 else 1) for (a, b) in zip(inputs.shape, pool_size)
@@ -238,15 +238,15 @@
     inputs,
     kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     num_spatial_dims = inputs.ndim - 2
     dimension_numbers = _convert_to_lax_conv_dimension_numbers(
         num_spatial_dims,
         data_format,
         transpose=False,
     )
     strides = _convert_to_spatial_operand(
@@ -288,15 +288,15 @@
     inputs,
     kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     num_spatial_dims = inputs.ndim - 2
     dimension_numbers = _convert_to_lax_conv_dimension_numbers(
         num_spatial_dims,
         data_format,
         transpose=False,
     )
     strides = _convert_to_spatial_operand(
@@ -334,15 +334,15 @@
     depthwise_kernel,
     pointwise_kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     depthwise_conv_output = depthwise_conv(
         inputs,
         depthwise_kernel,
         strides,
         padding,
         data_format,
         dilation_rate,
@@ -362,15 +362,15 @@
     kernel,
     strides=1,
     padding="valid",
     output_padding=None,
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     num_spatial_dims = inputs.ndim - 2
     padding_values = compute_conv_transpose_padding_args_for_jax(
         input_shape=inputs.shape,
         kernel_shape=kernel.shape,
         strides=strides,
         padding=padding,
         output_padding=output_padding,
@@ -473,15 +473,15 @@
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
 
     if from_logits:
         log_prob = jax.nn.log_softmax(output, axis=axis)
     else:
         output = output / jnp.sum(output, axis, keepdims=True)
-        output = jnp.clip(output, epsilon(), 1.0 - epsilon())
+        output = jnp.clip(output, backend.epsilon(), 1.0 - backend.epsilon())
         log_prob = jnp.log(output)
     return -jnp.sum(target * log_prob, axis=axis)
 
 
 def sparse_categorical_crossentropy(target, output, from_logits=False, axis=-1):
     target = jnp.array(target, dtype="int32")
     output = jnp.array(output)
@@ -500,15 +500,15 @@
             "up until the last dimension: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
     if from_logits:
         log_prob = jax.nn.log_softmax(output, axis=axis)
     else:
         output = output / jnp.sum(output, axis, keepdims=True)
-        output = jnp.clip(output, epsilon(), 1.0 - epsilon())
+        output = jnp.clip(output, backend.epsilon(), 1.0 - backend.epsilon())
         log_prob = jnp.log(output)
     target = jnn.one_hot(target, output.shape[axis], axis=axis)
     return -jnp.sum(target * log_prob, axis=axis)
 
 
 def binary_crossentropy(target, output, from_logits=False):
     target = jnp.array(target)
@@ -522,30 +522,30 @@
         )
 
     if from_logits:
         log_logits = jax.nn.log_sigmoid(output)
         log_neg_logits = jax.nn.log_sigmoid(-output)
         return -1.0 * target * log_logits - (1.0 - target) * log_neg_logits
 
-    output = jnp.clip(output, epsilon(), 1.0 - epsilon())
+    output = jnp.clip(output, backend.epsilon(), 1.0 - backend.epsilon())
     bce = target * jnp.log(output)
     bce += (1.0 - target) * jnp.log(1.0 - output)
     return -bce
 
 
 def moments(x, axes, keepdims=False, synchronized=False):
     if synchronized:
         raise NotImplementedError(
             "Argument synchronized=True is not supported with JAX."
         )
     # The dynamic range of float16 is too limited for statistics. As a
     # workaround, we simply perform the operations on float32 and convert back
     # to float16
     need_cast = False
-    ori_dtype = standardize_dtype(x.dtype)
+    ori_dtype = backend.standardize_dtype(x.dtype)
     if ori_dtype in ("float16", "bfloat16"):
         need_cast = True
         x = cast(x, "float32")
 
     mean = jnp.mean(x, axes, keepdims=True)
     variance = jnp.var(x, axis=axes, keepdims=True)
 
@@ -582,137 +582,167 @@
     if offset is not None:
         offset = jnp.reshape(offset, shape)
         res = res + offset
 
     return jnp.add(x * inv, res)
 
 
-def ctc_loss(
-    target,
-    output,
-    target_length,
-    output_length,
-    mask_index=0,
-):
-    batch_size, _, _ = output.shape
-    batch_size, max_target_length = target.shape
+def ctc_loss(target, output, target_length, output_length, mask_index=0):
+    # Ref: https://github.com/google-deepmind/optax
+    # optax.ctc_loss_with_forward_probs
+    target = convert_to_tensor(target, dtype="int32")
+    output = convert_to_tensor(output)
+    target_length = convert_to_tensor(target_length, "int32")
+    output_length = convert_to_tensor(output_length, "int32")
+    batch_size, _, num_classes = output.shape
+    batch_size, max_label_length = target.shape
+    log_epsilon = -1e5
 
-    output = output.transpose((1, 0, 2))
-    target = target.transpose((1, 0)).astype("int32")
+    # Ensure that the dtype promotion behavior matchs that of `tf.nn.ctc_loss`
+    dtype = backend.result_type(output.dtype, "float32")
+    output = cast(output, dtype)
 
-    logits = jnn.log_softmax(output)
-    mgrid_t, mgrid_b = jnp.meshgrid(
-        jnp.arange(max_target_length), jnp.arange(batch_size)
-    )
-    logprobs_emit = logits[mgrid_t, mgrid_b, target[:, :, None]]
-    logprobs_mask = logits[:, :, mask_index]
+    def _lengths_to_paddings(lengths, max_length):
+        indices = jnp.arange(max_length).reshape(
+            (1,) * lengths.ndim + (max_length,)
+        )
+        lengths = jnp.expand_dims(lengths, axis=-1)
+        elem_valid = indices < lengths
+        return jnp.logical_not(elem_valid)
+
+    target_paddings = _lengths_to_paddings(target_length, max_label_length)
+    output_paddings = _lengths_to_paddings(output_length, max_label_length)
+    target_paddings = target_paddings.astype(output.dtype)
+    output_paddings = output_paddings.astype(output.dtype)
 
-    logit_paddings = jnp.array(
-        jnp.arange(max_target_length) < output_length[:, None],
-        dtype=jnp.float32,
+    logprobs = jnn.log_softmax(output)
+    label_lengths = max_label_length - jnp.sum(target_paddings, axis=1).astype(
+        jnp.int32
     )
 
-    repeat = jnp.array(target[1:] == target[:-1])
-    repeat = jnp.pad(repeat, ((0, 1), (0, 0))).transpose((1, 0))
+    # repeat[b, n] == 1.0 when label[b, n] == label[b, n+1].
+    repeat = (target[:, :-1] == target[:, 1:]).astype(jnp.float32)
+    repeat = jnp.pad(repeat, ((0, 0), (0, 1)))
 
-    _logepsilon = -100000.0
+    logprobs_phi = logprobs[:, :, mask_index : mask_index + 1]  # [B, T, 1]
+    logprobs_phi = jnp.transpose(logprobs_phi, (1, 0, 2))  # [T, B, 1]
 
-    def _iterate(prev, x):
-        prev_mask, prev_emit = prev
-        logprob_mask, logprob_emit, pad = x
+    _one_hot = jax.nn.one_hot(target, num_classes=num_classes)  # [B, N, K]
+    logprobs_emit = jnp.einsum("btk,bnk->btn", logprobs, _one_hot)
+    logprobs_emit = jnp.transpose(logprobs_emit, (1, 0, 2))  # [T, B, N]
 
-        prev_mask_orig = prev_mask
-        prev_mask = prev_mask.at[:, 1:].set(
-            jnp.logaddexp(prev_mask[:, 1:], prev_emit + _logepsilon * repeat),
-        )
-        emit = jnp.logaddexp(
-            prev_mask[:, :-1] + logprob_emit, prev_emit + logprob_emit
-        )
+    # [B, N]
+    logalpha_phi_init = (
+        jnp.ones((batch_size, max_label_length + 1), dtype=output.dtype)
+        * log_epsilon
+    )
+    logalpha_phi_init = logalpha_phi_init.at[:, 0].set(0.0)
+    logalpha_emit_init = (
+        jnp.ones((batch_size, max_label_length), dtype=output.dtype)
+        * log_epsilon
+    )
 
-        mask = prev_mask + logprob_mask[:, None]
-        mask = mask.at[:, 1:].set(
-            jnp.logaddexp(
-                mask[:, 1:],
-                prev_emit + logprob_mask[:, None] + _logepsilon * (1 - repeat),
-            )
+    def update_phi_score(phi, added_score):
+        # Update `phi[:, 1:]`` with adding `added_score` in log space.
+        return jnp.concatenate(
+            [phi[:, :1], jnp.logaddexp(phi[:, 1:], added_score)], axis=-1
         )
 
-        pad = pad[:, None]
-        emit = emit * pad + prev_emit * (1 - pad)
-        mask = mask * pad + prev_mask_orig * (1 - pad)
+    def loop_body(prev, x):
+        prev_phi, prev_emit = prev
+        # emit-to-phi epsilon transition, except if the next label is repetition
+        prev_phi_orig = prev_phi
+        prev_phi = update_phi_score(prev_phi, prev_emit + log_epsilon * repeat)
 
-        return (mask, emit), (mask, emit)
+        logprob_emit, logprob_phi, pad = x
 
-    mask_init = jnp.full((batch_size, max_target_length + 1), _logepsilon)
-    mask_init = mask_init.at[:, 0].set(0.0)
-    emit_init = jnp.full((batch_size, max_target_length), _logepsilon)
+        # phi-to-emit transition
+        next_emit = jnp.logaddexp(
+            prev_phi[:, :-1] + logprob_emit, prev_emit + logprob_emit
+        )
+        # self-loop transition
+        next_phi = prev_phi + logprob_phi
+        # emit-to-phi blank transition only when the next label is repetition
+        next_phi = update_phi_score(
+            next_phi, prev_emit + logprob_phi + log_epsilon * (1.0 - repeat)
+        )
 
-    _, (alphas_mask, alphas_emit) = lax.scan(
-        _iterate,
-        (mask_init, emit_init),
-        (logprobs_mask, logprobs_emit, logit_paddings.transpose()),
-    )
+        pad = pad.reshape((batch_size, 1))
+        next_emit = pad * prev_emit + (1.0 - pad) * next_emit
+        next_phi = pad * prev_phi_orig + (1.0 - pad) * next_phi
+
+        return (next_phi, next_emit), (next_phi, next_emit)
 
-    last_alpha_mask = (
-        alphas_mask[-1]
-        .at[:, 1:]
-        .set(jnp.logaddexp(alphas_mask[-1, :, 1:], alphas_emit[-1]))
+    xs = (logprobs_emit, logprobs_phi, output_paddings.transpose((1, 0)))
+    _, (logalpha_phi, logalpha_emit) = jax.lax.scan(
+        loop_body, (logalpha_phi_init, logalpha_emit_init), xs
     )
 
-    return -last_alpha_mask[jnp.arange(batch_size), target_length]
+    # last row needs to be updated with the last epsilon transition
+    logalpha_phi_last = update_phi_score(logalpha_phi[-1], logalpha_emit[-1])
+    logalpha_phi = logalpha_phi.at[-1].set(logalpha_phi_last)
 
+    # extract per_seq_loss
+    # [B, N+1]
+    _one_hot = jax.nn.one_hot(label_lengths, num_classes=max_label_length + 1)
+    per_seq_loss = -jnp.einsum("bn,bn->b", logalpha_phi_last, _one_hot)
+    return per_seq_loss
 
-def ctc_greedy_decode(
+
+def _ctc_greedy_decode(
     inputs,
     sequence_length,
     merge_repeated=True,
     mask_index=None,
 ):
-    inputs = jnp.array(inputs)
-    sequence_length = jnp.array(sequence_length, dtype=jnp.int32)
+    inputs = convert_to_tensor(inputs)
+    sequence_length = convert_to_tensor(sequence_length, dtype="int32")
+    batch_size, max_length, num_classes = inputs.shape
 
     if mask_index is None:
-        mask_index = inputs.shape[-1] - 1
+        mask_index = num_classes - 1
 
     indices = jnp.argmax(inputs, axis=-1)
     scores = jnp.max(inputs, axis=-1)
 
-    seqlen_mask = jnp.arange(inputs.shape[1])[None, :]
+    seqlen_mask = jnp.arange(max_length)[None, :]
     seqlen_mask = seqlen_mask >= sequence_length[:, None]
 
-    if merge_repeated:
-        repeat = indices[:, 1:] == indices[:, :-1]
-        repeat = jnp.pad(repeat, ((0, 0), (1, 0)))
-
-        indices = jnp.where(repeat, mask_index, indices)
-    else:
-        repeat = jnp.zeros_like(indices, dtype=bool)
-
     indices = jnp.where(seqlen_mask, mask_index, indices)
-    indices = [batch[batch != mask_index] for batch in indices]
-    max_len = max(len(batch) for batch in indices)
-    indices = jnp.array(
-        [jnp.pad(batch, (0, max_len - len(batch))) for batch in indices]
-    )
-
     scores = jnp.where(seqlen_mask, 0.0, scores)
-    scores = -jnp.sum(scores, axis=1)[:, None]
 
-    return [indices], scores
+    if merge_repeated:
+        repeat_mask = indices[:, 1:] == indices[:, :-1]
+        repeat_mask = jnp.pad(repeat_mask, ((0, 0), (1, 0)))
+        indices = jnp.where(repeat_mask, mask_index, indices)
+
+    # We rearrange the indices by moving `mask_index` to the end of the array
+    invalid_mask = indices == mask_index
+    order = jnp.expand_dims(jnp.arange(max_length), axis=0)  # [1, N]
+    order = jnp.tile(order, (batch_size, 1))  # [B, N]
+    order = jnp.where(invalid_mask, max_length, order)
+    order = jnp.argsort(order, axis=-1)
+    indices = jnp.take_along_axis(indices, order, axis=-1)
+
+    # We set to -1 for blank labels
+    indices = jnp.where(invalid_mask, -1, indices)
+    scores = -jnp.sum(scores, axis=1)[:, None]
+    indices = jnp.expand_dims(indices, axis=0)
+    return indices, scores
 
 
-def ctc_beam_search_decode(
+def _ctc_beam_search_decode(
     inputs,
     sequence_length,
     beam_width=100,
     top_paths=1,
     mask_index=None,
 ):
-    inputs = jnp.array(inputs)
-    sequence_length = jnp.array(sequence_length)
+    inputs = convert_to_tensor(inputs)
+    sequence_length = convert_to_tensor(sequence_length)
 
     batch_size, max_seq_len, num_classes = inputs.shape
     inputs = jnn.log_softmax(inputs)
     seqlen_mask = jnp.arange(max_seq_len)[None, :] >= sequence_length[:, None]
 
     if mask_index is None:
         mask_index = num_classes - 1
@@ -726,21 +756,21 @@
 
     _pad = -1
 
     init_paths = jnp.full(
         (batch_size, 2 * beam_width, max_seq_len), _pad, dtype=jnp.int32
     )
 
-    num_init_paths = jnp.min(jnp.array([num_classes, beam_width]))
+    num_init_paths = builtins.min(num_classes, beam_width)
     max_classes = jnp.argsort(inputs[:, 0], axis=1)[:, -num_init_paths:]
     init_classes = jnp.where(max_classes == mask_index, _pad, max_classes)
     init_paths = init_paths.at[:, :num_init_paths, 0].set(init_classes)
 
     init_scores = (
-        jnp.full((batch_size, 2 * beam_width), -jnp.inf)
+        jnp.full((batch_size, 2 * beam_width), -jnp.inf, dtype=inputs.dtype)
         .at[:, :num_init_paths]
         .set(jnp.take_along_axis(inputs[:, 0], max_classes, axis=1))
     )
     init_masked = init_paths[:, :, 0] == _pad
 
     def _extend_paths(paths, scores, masked, x):
         paths = jnp.repeat(paths, num_classes, axis=0)
@@ -855,42 +885,57 @@
 
     paths, scores = jax.vmap(_decode_batch)(
         init_paths, init_scores, init_masked, inputs, seqlen_mask
     )
 
     # convert classes back to the correct indices
     paths = jnp.where(paths == _pad, _pad, num_classes - paths - 1)
-
-    lengths = jnp.argmax(paths == _pad, axis=2)
-    lengths = jnp.max(lengths, axis=0)
-    paths = jnp.where(paths == _pad, 0, paths)
-
-    paths = paths.transpose((1, 0, 2))
-    paths = [path[:, :length] for path, length in zip(paths, lengths)]
-
+    paths = jnp.transpose(paths, [1, 0, 2])
     return paths, scores
 
 
 def ctc_decode(
     inputs,
     sequence_length,
-    strategy,
+    strategy="greedy",
     beam_width=100,
     top_paths=1,
     merge_repeated=True,
     mask_index=None,
 ):
+    inputs = convert_to_tensor(inputs)
+    dtype = backend.result_type(inputs.dtype, "float32")
+    inputs = cast(inputs, dtype)
+
     if strategy == "greedy":
-        return ctc_greedy_decode(
+        return _ctc_greedy_decode(
             inputs,
             sequence_length,
             merge_repeated=merge_repeated,
             mask_index=mask_index,
         )
-    else:
-        return ctc_beam_search_decode(
+    elif strategy == "beam_search":
+        return _ctc_beam_search_decode(
             inputs,
             sequence_length,
             beam_width=beam_width,
             top_paths=top_paths,
             mask_index=mask_index,
         )
+    else:
+        raise ValueError(
+            f"Invalid strategy {strategy}. Supported values are "
+            "'greedy' and 'beam_search'."
+        )
+
+
+def psnr(x1, x2, max_val):
+    if x1.shape != x2.shape:
+        raise ValueError(
+            f"Input shapes {x1.shape} and {x2.shape} must "
+            "match for PSNR calculation. "
+        )
+
+    max_val = convert_to_tensor(max_val, dtype=x2.dtype)
+    mse = jnp.mean(jnp.square(x1 - x2))
+    psnr = 20 * jnp.log10(max_val) - 10 * jnp.log10(mse)
+    return psnr
```

### Comparing `keras-3.3.2/keras/src/backend/jax/numpy.py` & `keras-3.3.3/keras/src/backend/jax/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1158,7 +1158,12 @@
     x1 = convert_to_tensor(x1)
     x2 = convert_to_tensor(x2)
     return jnp.correlate(x1, x2, mode)
 
 
 def select(condlist, choicelist, default=0):
     return jnp.select(condlist, choicelist, default=default)
+
+
+def slogdet(x):
+    x = convert_to_tensor(x)
+    return tuple(jnp.linalg.slogdet(x))
```

### Comparing `keras-3.3.2/keras/src/backend/jax/optimizer.py` & `keras-3.3.3/keras/src/backend/jax/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/jax/random.py` & `keras-3.3.3/keras/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/jax/rnn.py` & `keras-3.3.3/keras/src/backend/jax/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/jax/sparse.py` & `keras-3.3.3/keras/src/backend/jax/sparse.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/jax/trainer.py` & `keras-3.3.3/keras/src/backend/jax/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/numpy/__init__.py` & `keras-3.3.3/keras/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/numpy/core.py` & `keras-3.3.3/keras/src/backend/numpy/core.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/numpy/image.py` & `keras-3.3.3/keras/src/backend/numpy/image.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/numpy/linalg.py` & `keras-3.3.3/keras/src/backend/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/numpy/math.py` & `keras-3.3.3/keras/src/backend/numpy/math.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/numpy/nn.py` & `keras-3.3.3/keras/src/ops/linalg.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,631 +1,638 @@
-import jax
-import numpy as np
-from jax import lax
-from jax import numpy as jnp
-
-from keras.src.backend import standardize_data_format
-from keras.src.backend import standardize_dtype
-from keras.src.backend.common.backend_utils import (
-    compute_conv_transpose_padding_args_for_jax,
-)
-from keras.src.backend.config import epsilon
-from keras.src.backend.numpy.core import cast
-from keras.src.backend.numpy.core import convert_to_tensor
-from keras.src.backend.numpy.core import is_tensor
-from keras.src.utils.module_utils import scipy
+from keras.src import backend
+from keras.src.api_export import keras_export
+from keras.src.backend import KerasTensor
+from keras.src.backend import any_symbolic_tensors
+from keras.src.ops.operation import Operation
+from keras.src.ops.operation_utils import reduce_shape
+
+
+class Cholesky(Operation):
+    def __init__(self):
+        super().__init__()
+
+    def call(self, x):
+        return _cholesky(x)
+
+    def compute_output_spec(self, x):
+        _assert_2d(x)
+        _assert_square(x)
+        return KerasTensor(x.shape, x.dtype)
+
+
+@keras_export(["keras.ops.cholesky", "keras.ops.linalg.cholesky"])
+def cholesky(x):
+    """Computes the Cholesky decomposition of a positive semi-definite matrix.
 
+    Args:
+        x: Input tensor of shape `(..., M, M)`.
 
-def relu(x):
-    x = convert_to_tensor(x)
-    return np.maximum(x, np.array(0.0, x.dtype))
+    Returns:
+        A tensor of shape `(..., M, M)` representing the lower triangular
+        Cholesky factor of `x`.
 
+    """
+    if any_symbolic_tensors((x,)):
+        return Cholesky().symbolic_call(x)
+    return _cholesky(x)
 
-def relu6(x):
-    x = convert_to_tensor(x)
-    # np.clip incorrectly promote bfloat16 to float32, so we replace it with
-    # np.minimum and np.maximum here
-    return np.minimum(
-        np.maximum(x, np.array(0.0, x.dtype)), np.array(6.0, x.dtype)
-    )
 
+def _cholesky(x):
+    x = backend.convert_to_tensor(x)
+    _assert_2d(x)
+    _assert_square(x)
+    try:
+        return backend.linalg.cholesky(x)
+    except Exception as e:
+        raise ValueError(f"Cholesky decomposition failed: {e}")
 
-def sigmoid(x):
-    x = convert_to_tensor(x)
-    return np.array(1.0, x.dtype) / (np.array(1.0, x.dtype) + np.exp(-x))
 
+class Det(Operation):
 
-def tanh(x):
-    return np.tanh(x)
+    def __init__(self):
+        super().__init__()
 
+    def call(self, x):
+        return _det(x)
 
-def softplus(x):
-    x = convert_to_tensor(x)
-    return np.logaddexp(x, np.array(0.0, x.dtype))
+    def compute_output_spec(self, x):
+        _assert_2d(x)
+        _assert_square(x)
+        return KerasTensor(x.shape[:-2], x.dtype)
 
 
-def softsign(x):
-    x = convert_to_tensor(x)
-    return x / (np.array(1.0, x.dtype) + np.abs(x))
+@keras_export(["keras.ops.det", "keras.ops.linalg.det"])
+def det(x):
+    """Computes the determinant of a square tensor.
 
+    Args:
+        x: Input tensor of shape `(..., M, M)`.
 
-def silu(x):
-    x = convert_to_tensor(x)
-    return x * sigmoid(x)
+    Returns:
+        A tensor of shape `(...,)` represeting the determinant of `x`.
 
+    """
+    if any_symbolic_tensors((x,)):
+        return Det().symbolic_call(x)
+    return _det(x)
 
-def log_sigmoid(x):
-    x = convert_to_tensor(x)
-    return -softplus(-x)
 
+def _det(x):
+    x = backend.convert_to_tensor(x)
+    _assert_2d(x)
+    _assert_square(x)
+    return backend.linalg.det(x)
 
-def leaky_relu(x, negative_slope=0.2):
-    x = convert_to_tensor(x)
-    return np.maximum(x, np.array(negative_slope, x.dtype) * x)
 
+class Eig(Operation):
 
-def hard_sigmoid(x):
-    # python numbers will be promoted to float64 by np, so it's necessary to
-    # first convert the python numbers to np scalars
-    x = x / np.array(6.0, x.dtype) + np.array(0.5, x.dtype)
-    return np.where(
-        x <= 0.0,
-        np.array(0.0, x.dtype),
-        np.where(x >= 1.0, np.array(1.0, x.dtype), x),
-    )
+    def __init__(self):
+        super().__init__()
 
+    def call(self, x):
+        return _eig(x)
 
-def hard_silu(x):
-    return x * hard_sigmoid(x)
+    def compute_output_spec(self, x):
+        _assert_square(x)
+        _assert_2d(x)
+        return (
+            KerasTensor(x.shape[:-1], x.dtype),
+            KerasTensor(x.shape, x.dtype),
+        )
 
 
-def elu(x, alpha=1.0):
-    x = convert_to_tensor(x)
-    return np.where(
-        x >= np.array(0.0, x.dtype), x, np.array(alpha, x.dtype) * np.expm1(x)
-    )
+@keras_export(["keras.ops.eig", "keras.ops.linalg.eig"])
+def eig(x):
+    """Computes the eigenvalues and eigenvectors of a square matrix.
 
+    Args:
+        x: Input tensor of shape `(..., M, M)`.
 
-def selu(
-    x,
-    alpha=1.6732632423543772848170429916717,
-    scale=1.0507009873554804934193349852946,
-):
-    x = convert_to_tensor(x)
-    return np.array(scale, x.dtype) * elu(x, alpha)
+    Returns:
+        A tuple of two tensors: a tensor of shape `(..., M)` containing
+        eigenvalues and a tensor of shape `(..., M, M)` containing eigenvectors.
+    """
+    if any_symbolic_tensors((x,)):
+        return Eig().symbolic_call(x)
+    return _eig(x)
 
 
-def gelu(x, approximate=True):
-    x = convert_to_tensor(x)
-    # followed by JAX's implementation
-    if approximate:
-        sqrt_2_over_pi = np.sqrt(2 / np.pi).astype(x.dtype)
-        cdf = np.array(0.5, x.dtype) * (
-            np.array(1.0, x.dtype)
-            + np.tanh(
-                sqrt_2_over_pi
-                * (x + np.array(0.044715, x.dtype) * (x**3).astype(x.dtype))
-            )
-        )
-        return x * cdf
-    else:
-        sqrt_2 = np.sqrt(2).astype(x.dtype)
+def _eig(x):
+    x = backend.convert_to_tensor(x)
+    _assert_square(x)
+    _assert_2d(x)
+    return backend.linalg.eig(x)
+
+
+class Eigh(Operation):
+
+    def __init__(self):
+        super().__init__()
+
+    def call(self, x):
+        return _eigh(x)
+
+    def compute_output_spec(self, x):
+        _assert_square(x)
+        _assert_2d(x)
         return (
-            x
-            * (scipy.special.erf(x / sqrt_2) + 1).astype(x.dtype)
-            / np.array(2, x.dtype)
+            KerasTensor(x.shape[:-1], x.dtype),
+            KerasTensor(x.shape, x.dtype),
         )
 
 
-def softmax(x, axis=None):
-    exp_x = np.exp(x - np.max(x, axis=axis, keepdims=True))
-    return exp_x / np.sum(exp_x, axis=axis, keepdims=True)
-
-
-def log_softmax(x, axis=None):
-    max_x = np.max(x, axis=axis, keepdims=True)
-    logsumexp = np.log(np.exp(x - max_x).sum(axis=axis, keepdims=True))
-    return x - max_x - logsumexp
-
-
-def _convert_to_spatial_operand(
-    x,
-    num_spatial_dims,
-    data_format="channels_last",
-    include_batch_and_channels=True,
-):
-    # Helper function that converts an operand to a spatial operand.
-    x = (x,) * num_spatial_dims if isinstance(x, int) else x
-    if not include_batch_and_channels:
-        return x
-    if data_format == "channels_last":
-        x = (1,) + x + (1,)
-    else:
-        x = (1,) + (1,) + x
-    return x
-
-
-def _pool(
-    inputs,
-    initial_value,
-    reduce_fn,
-    pool_size,
-    strides=None,
-    padding="valid",
-):
-    """Helper function to define pooling functions.
-
-    Args:
-        inputs: input data of shape `N+2`.
-        initial_value: the initial value for the reduction.
-        reduce_fn: a reduce function of the form `(T, T) -> T`.
-        pool_size: a sequence of `N` integers, representing the window size to
-            reduce over.
-        strides: a sequence of `N` integers, representing the inter-window
-            strides (default: `(1, ..., 1)`).
-        padding: either the string `same` or `valid`.
-
-    Returns:
-        The output of the reduction for each window slice.
-    """
-    if padding not in ("same", "valid"):
-        raise ValueError(
-            f"Invalid padding '{padding}', must be 'same' or 'valid'."
-        )
-    padding = padding.upper()
-    return np.array(
-        lax.reduce_window(
-            inputs,
-            initial_value,
-            reduce_fn,
-            pool_size,
-            strides,
-            padding,
-        )
-    )
+@keras_export(["keras.ops.eigh", "keras.ops.linalg.eigh"])
+def eigh(x):
+    """Computes the eigenvalues and eigenvectors of a complex Hermitian.
 
+    Args:
+        x: Input tensor of shape `(..., M, M)`.
 
-def max_pool(
-    inputs,
-    pool_size,
-    strides=None,
-    padding="valid",
-    data_format=None,
-):
-    data_format = standardize_data_format(data_format)
-    num_spatial_dims = inputs.ndim - 2
-    pool_size = _convert_to_spatial_operand(
-        pool_size, num_spatial_dims, data_format
-    )
-    strides = pool_size if strides is None else strides
-    strides = _convert_to_spatial_operand(
-        strides, num_spatial_dims, data_format
-    )
-    return _pool(inputs, -jnp.inf, lax.max, pool_size, strides, padding)
-
-
-def average_pool(
-    inputs,
-    pool_size,
-    strides,
-    padding,
-    data_format=None,
-):
-    data_format = standardize_data_format(data_format)
-    num_spatial_dims = inputs.ndim - 2
-    pool_size = _convert_to_spatial_operand(
-        pool_size, num_spatial_dims, data_format
-    )
-    strides = pool_size if strides is None else strides
-    strides = _convert_to_spatial_operand(
-        strides, num_spatial_dims, data_format
-    )
-
-    pooled = _pool(inputs, 0.0, lax.add, pool_size, strides, padding)
-    if padding == "valid":
-        # Avoid the extra reduce_window.
-        return pooled / np.prod(pool_size)
-    else:
-        # Count the number of valid entries at each input point, then use that
-        # for computing average. Assumes that any two arrays of same shape will
-        # be padded the same. Avoid broadcasting on axis where pooling is
-        # skipped.
-        shape = [
-            (a if b != 1 else 1) for (a, b) in zip(inputs.shape, pool_size)
-        ]
-        window_counts = _pool(
-            jnp.ones(shape, inputs.dtype),
-            0.0,
-            lax.add,
-            pool_size,
-            strides,
-            padding,
-        )
-        return pooled / window_counts
+    Returns:
+        A tuple of two tensors: a tensor of shape `(..., M)` containing
+        eigenvalues and a tensor of shape `(..., M, M)` containing eigenvectors.
 
+    """
+    if any_symbolic_tensors((x,)):
+        return Eigh().symbolic_call(x)
+    return _eigh(x)
 
-def _convert_to_lax_conv_dimension_numbers(
-    num_spatial_dims,
-    data_format="channels_last",
-    transpose=False,
-):
-    """Create a `lax.ConvDimensionNumbers` for the given inputs."""
-    num_dims = num_spatial_dims + 2
-
-    if data_format == "channels_last":
-        spatial_dims = tuple(range(1, num_dims - 1))
-        inputs_dn = (0, num_dims - 1) + spatial_dims
-    else:
-        spatial_dims = tuple(range(2, num_dims))
-        inputs_dn = (0, 1) + spatial_dims
-
-    if transpose:
-        kernel_dn = (num_dims - 2, num_dims - 1) + tuple(range(num_dims - 2))
-    else:
-        kernel_dn = (num_dims - 1, num_dims - 2) + tuple(range(num_dims - 2))
-
-    return lax.ConvDimensionNumbers(
-        lhs_spec=inputs_dn, rhs_spec=kernel_dn, out_spec=inputs_dn
-    )
-
-
-def conv(
-    inputs,
-    kernel,
-    strides=1,
-    padding="valid",
-    data_format=None,
-    dilation_rate=1,
-):
-    data_format = standardize_data_format(data_format)
-    num_spatial_dims = inputs.ndim - 2
-    dimension_numbers = _convert_to_lax_conv_dimension_numbers(
-        num_spatial_dims,
-        data_format,
-        transpose=False,
-    )
-    strides = _convert_to_spatial_operand(
-        strides,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-    dilation_rate = _convert_to_spatial_operand(
-        dilation_rate,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-    if data_format == "channels_last":
-        channels = inputs.shape[-1]
-    else:
-        channels = inputs.shape[1]
-    kernel_in_channels = kernel.shape[-2]
-    if channels % kernel_in_channels > 0:
-        raise ValueError(
-            "The number of input channels must be evenly divisible by "
-            f"kernel's in_channels. Received input channels {channels} and "
-            f"kernel in_channels {kernel_in_channels}. "
-        )
-    feature_group_count = channels // kernel_in_channels
-    return np.array(
-        jax.lax.conv_general_dilated(
-            inputs,
-            kernel if is_tensor(kernel) else kernel.numpy(),
-            strides,
-            padding,
-            rhs_dilation=dilation_rate,
-            dimension_numbers=dimension_numbers,
-            feature_group_count=feature_group_count,
-        )
-    )
 
+def _eigh(x):
+    x = backend.convert_to_tensor(x)
+    _assert_square(x)
+    _assert_2d(x)
+    return backend.linalg.eigh(x)
 
-def depthwise_conv(
-    inputs,
-    kernel,
-    strides=1,
-    padding="valid",
-    data_format=None,
-    dilation_rate=1,
-):
-    data_format = standardize_data_format(data_format)
-    num_spatial_dims = inputs.ndim - 2
-    dimension_numbers = _convert_to_lax_conv_dimension_numbers(
-        num_spatial_dims,
-        data_format,
-        transpose=False,
-    )
-    strides = _convert_to_spatial_operand(
-        strides,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-    dilation_rate = _convert_to_spatial_operand(
-        dilation_rate,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-    feature_group_count = (
-        inputs.shape[-1] if data_format == "channels_last" else inputs.shape[1]
-    )
-    kernel = jnp.reshape(
-        kernel if is_tensor(kernel) else kernel.numpy(),
-        kernel.shape[:-2] + (1, feature_group_count * kernel.shape[-1]),
-    )
-    return np.array(
-        jax.lax.conv_general_dilated(
-            inputs,
-            kernel,
-            strides,
-            padding,
-            rhs_dilation=dilation_rate,
-            dimension_numbers=dimension_numbers,
-            feature_group_count=feature_group_count,
-        )
-    )
 
+class Inv(Operation):
 
-def separable_conv(
-    inputs,
-    depthwise_kernel,
-    pointwise_kernel,
-    strides=1,
-    padding="valid",
-    data_format=None,
-    dilation_rate=1,
-):
-    data_format = standardize_data_format(data_format)
-    depthwise_conv_output = depthwise_conv(
-        inputs,
-        depthwise_kernel,
-        strides,
-        padding,
-        data_format,
-        dilation_rate,
-    )
-    return conv(
-        depthwise_conv_output,
-        pointwise_kernel,
-        strides=1,
-        padding="valid",
-        data_format=data_format,
-        dilation_rate=dilation_rate,
-    )
-
-
-def conv_transpose(
-    inputs,
-    kernel,
-    strides=1,
-    padding="valid",
-    output_padding=None,
-    data_format=None,
-    dilation_rate=1,
-):
-    data_format = standardize_data_format(data_format)
-    num_spatial_dims = inputs.ndim - 2
-    padding_values = compute_conv_transpose_padding_args_for_jax(
-        input_shape=inputs.shape,
-        kernel_shape=kernel.shape,
-        strides=strides,
-        padding=padding,
-        output_padding=output_padding,
-        dilation_rate=dilation_rate,
-    )
-    dimension_numbers = _convert_to_lax_conv_dimension_numbers(
-        num_spatial_dims,
-        data_format,
-        transpose=False,
-    )
-    strides = _convert_to_spatial_operand(
-        strides,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-    dilation_rate = _convert_to_spatial_operand(
-        dilation_rate,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-
-    return np.array(
-        jax.lax.conv_transpose(
-            inputs,
-            kernel if is_tensor(kernel) else kernel.numpy(),
-            strides,
-            padding=padding_values,
-            rhs_dilation=dilation_rate,
-            dimension_numbers=dimension_numbers,
-            transpose_kernel=True,
-        )
-    )
+    def __init__(self):
+        super().__init__()
 
+    def call(self, x):
+        return _inv(x)
+
+    def compute_output_spec(self, x):
+        _assert_2d(x)
+        _assert_square(x)
+        return KerasTensor(x.shape, x.dtype)
 
-def one_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
-    if sparse:
-        raise ValueError("Unsupported value `sparse=True` with numpy backend")
-    x = convert_to_tensor(x)
-    input_shape = x.shape
-
-    # Shrink the last dimension if the shape is (..., 1).
-    if input_shape and input_shape[-1] == 1 and len(input_shape) > 1:
-        input_shape = tuple(input_shape[:-1])
-
-    x = x.reshape(-1)
-    if not num_classes:
-        num_classes = np.max(x) + 1
-
-    batch_size = x.shape[0]
-    categorical = np.zeros((batch_size, num_classes), dtype=dtype)
-    valid_indices = x >= 0
-    categorical[np.arange(batch_size)[valid_indices], x[valid_indices]] = 1
-
-    # First, reshape the array with the extra dimension at the end
-    output_shape = input_shape + (num_classes,)
-    categorical = np.reshape(categorical, output_shape)
-
-    # Then, move this new dimension to the right place (according to axis)
-    if axis != -1:
-        categorical = np.moveaxis(categorical, -1, axis)
-
-    return categorical
-
-
-def multi_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
-    if sparse:
-        raise ValueError("Unsupported value `sparse=True` with numpy backend")
-    x = convert_to_tensor(x)
-    reduction_axis = 1 if len(x.shape) > 1 else 0
-    outputs = np.max(
-        one_hot(cast(x, "int32"), num_classes, axis=axis, dtype=dtype),
-        axis=reduction_axis,
-    )
-    return outputs
-
-
-def categorical_crossentropy(target, output, from_logits=False, axis=-1):
-    target = np.array(target)
-    output = np.array(output)
-
-    if target.shape != output.shape:
-        raise ValueError(
-            "Arguments `target` and `output` must have the same shape. "
-            "Received: "
-            f"target.shape={target.shape}, output.shape={output.shape}"
-        )
-    if len(target.shape) < 1:
-        raise ValueError(
-            "Arguments `target` and `output` must be at least rank 1. "
-            "Received: "
-            f"target.shape={target.shape}, output.shape={output.shape}"
-        )
 
-    if from_logits:
-        log_prob = log_softmax(output, axis=axis)
-    else:
-        output = output / np.sum(output, axis, keepdims=True)
-        output = np.clip(output, epsilon(), 1.0 - epsilon())
-        log_prob = np.log(output)
-    return -np.sum(target * log_prob, axis=axis)
-
-
-def sparse_categorical_crossentropy(target, output, from_logits=False, axis=-1):
-    target = np.array(target, dtype="int32")
-    output = np.array(output)
-    if len(target.shape) == len(output.shape) and target.shape[-1] == 1:
-        target = np.squeeze(target, axis=-1)
-
-    if len(output.shape) < 1:
-        raise ValueError(
-            "Argument `output` must be at least rank 1. "
-            "Received: "
-            f"output.shape={output.shape}"
+@keras_export(["keras.ops.inv", "keras.ops.linalg.inv"])
+def inv(x):
+    """Computes the inverse of a square tensor.
+
+    Args:
+        x: Input tensor of shape `(..., M, M)`.
+
+    Returns:
+        A tensor of shape `(..., M, M)` representing the inverse of `x`.
+
+    """
+    if any_symbolic_tensors((x,)):
+        return Inv().symbolic_call(x)
+    return _inv(x)
+
+
+def _inv(x):
+    x = backend.convert_to_tensor(x)
+    _assert_2d(x)
+    _assert_square(x)
+    return backend.linalg.inv(x)
+
+
+class LuFactor(Operation):
+
+    def __init__(self):
+        super().__init__()
+
+    def call(self, x):
+        return _lu_factor(x)
+
+    def compute_output_spec(self, x):
+        _assert_2d(x)
+        batch_shape = x.shape[:-2]
+        m, n = x.shape[-2:]
+        k = min(m, n)
+        return (
+            KerasTensor(batch_shape + (m, n), x.dtype),
+            KerasTensor(batch_shape + (k,), x.dtype),
         )
-    if target.shape != output.shape[:-1]:
-        raise ValueError(
-            "Arguments `target` and `output` must have the same shape "
-            "up until the last dimension: "
-            f"target.shape={target.shape}, output.shape={output.shape}"
+
+
+@keras_export(["keras.ops.lu_factor", "keras.ops.linalg.lu_factor"])
+def lu_factor(x):
+    """Computes the lower-upper decomposition of a square matrix.
+
+    Args:
+        x: A tensor of shape `(..., M, M)`.
+
+    Returns:
+        A tuple of two tensors: a tensor of shape `(..., M, M)` containing the
+        lower and upper triangular matrices and a tensor of shape `(..., M)`
+        containing the pivots.
+
+    """
+    if any_symbolic_tensors((x,)):
+        return LuFactor().symbolic_call(x)
+    return _lu_factor(x)
+
+
+def _lu_factor(x):
+    x = backend.convert_to_tensor(x)
+    _assert_2d(x)
+    if backend.backend() == "tensorflow":
+        try:
+            _assert_square(x)
+        except ValueError as e:
+            raise ValueError(
+                f"LU decomposition failed: {e}. LU decomposition is only "
+                "supported for square matrices in Tensorflow."
+            )
+    return backend.linalg.lu_factor(x)
+
+
+class Norm(Operation):
+    def __init__(self, ord=None, axis=None, keepdims=False):
+        super().__init__()
+        if isinstance(ord, str):
+            if ord not in ("fro", "nuc"):
+                raise ValueError(
+                    "Invalid `ord` argument. "
+                    "Expected one of {'fro', 'nuc'} when using string. "
+                    f"Received: ord={ord}"
+                )
+        if isinstance(axis, int):
+            axis = [axis]
+        self.ord = ord
+        self.axis = axis
+        self.keepdims = keepdims
+
+    def compute_output_spec(self, x):
+        output_dtype = backend.standardize_dtype(x.dtype)
+        if "int" in output_dtype or output_dtype == "bool":
+            output_dtype = backend.floatx()
+        if self.axis is None:
+            axis = tuple(range(len(x.shape)))
+        else:
+            axis = self.axis
+        num_axes = len(axis)
+        if num_axes == 1 and isinstance(self.ord, str):
+            raise ValueError(
+                "Invalid `ord` argument for vector norm. "
+                f"Received: ord={self.ord}"
+            )
+        elif num_axes == 2 and self.ord not in (
+            None,
+            "fro",
+            "nuc",
+            float("inf"),
+            float("-inf"),
+            1,
+            -1,
+            2,
+            -2,
+        ):
+            raise ValueError(
+                "Invalid `ord` argument for matrix norm. "
+                f"Received: ord={self.ord}"
+            )
+        return KerasTensor(
+            reduce_shape(x.shape, axis=self.axis, keepdims=self.keepdims),
+            dtype=output_dtype,
         )
-    if from_logits:
-        log_prob = log_softmax(output, axis=axis)
-    else:
-        output = output / np.sum(output, axis, keepdims=True)
-        output = np.clip(output, epsilon(), 1.0 - epsilon())
-        log_prob = np.log(output)
-    target = one_hot(target, output.shape[axis], axis=axis)
-    return -np.sum(target * log_prob, axis=axis)
-
-
-def binary_crossentropy(target, output, from_logits=False):
-    target = np.array(target)
-    output = np.array(output)
-
-    if target.shape != output.shape:
-        raise ValueError(
-            "Arguments `target` and `output` must have the same shape. "
-            "Received: "
-            f"target.shape={target.shape}, output.shape={output.shape}"
+
+    def call(self, x):
+        x = backend.convert_to_tensor(x)
+        return backend.linalg.norm(
+            x, ord=self.ord, axis=self.axis, keepdims=self.keepdims
         )
 
-    if from_logits:
-        output = sigmoid(output)
 
-    output = np.clip(output, epsilon(), 1.0 - epsilon())
-    bce = target * np.log(output)
-    bce += (1.0 - target) * np.log(1.0 - output)
-    return -bce
+@keras_export(["keras.ops.norm", "keras.ops.linalg.norm"])
+def norm(x, ord=None, axis=None, keepdims=False):
+    """Matrix or vector norm.
 
+    This function is able to return one of eight different matrix norms, or one
+    of an infinite number of vector norms (described below), depending on the
+    value of the `ord` parameter.
 
-def moments(x, axes, keepdims=False, synchronized=False):
-    if synchronized:
-        raise NotImplementedError(
-            "Argument synchronized=True is not supported with NumPy."
-        )
-    axes = tuple(axes) if isinstance(axes, list) else axes
-    # The dynamic range of float16 is too limited for statistics. As a
-    # workaround, we simply perform the operations on float32 and convert back
-    # to float16
-    need_cast = False
-    ori_dtype = standardize_dtype(x.dtype)
-    if ori_dtype == "float16":
-        need_cast = True
-        x = cast(x, "float32")
-
-    mean = np.mean(x, axes, keepdims=True)
-
-    # The variance is computed using $Var = E[|x|^2] - |E[x]|^2$, It is faster
-    # but less numerically stable.
-    variance = np.mean(np.square(x), axis=axes, keepdims=True) - np.square(mean)
-
-    if not keepdims:
-        mean = np.squeeze(mean, axes)
-        variance = np.squeeze(variance, axes)
-    if need_cast:
-        # avoid overflow and underflow when casting from float16 to float32
-        mean = np.clip(mean, np.finfo(np.float16).min, np.finfo(np.float16).max)
-        variance = np.clip(
-            variance, np.finfo(np.float16).min, np.finfo(np.float16).max
+    Args:
+        x: Input tensor.
+        ord: Order of the norm (see table under Notes). The default is `None`.
+        axis: If `axis` is an integer, it specifies the axis of `x` along which
+            to compute the vector norms. If `axis` is a 2-tuple, it specifies
+            the axes that hold 2-D matrices, and the matrix norms of these
+            matrices are computed.
+        keepdims: If this is set to `True`, the axes which are reduced are left
+            in the result as dimensions with size one.
+
+    Note:
+        For values of `ord < 1`, the result is, strictly speaking, not a
+        mathematical 'norm', but it may still be useful for various numerical
+        purposes. The following norms can be calculated:
+        - For matrices:
+            - `ord=None`: Frobenius norm
+            - `ord="fro"`: Frobenius norm
+            - `ord="nuc"`: nuclear norm
+            - `ord=np.inf`: `max(sum(abs(x), axis=1))`
+            - `ord=-np.inf`: `min(sum(abs(x), axis=1))`
+            - `ord=0`: not supported
+            - `ord=1`: `max(sum(abs(x), axis=0))`
+            - `ord=-1`: `min(sum(abs(x), axis=0))`
+            - `ord=2`: 2-norm (largest sing. value)
+            - `ord=-2`: smallest singular value
+            - other: not supported
+        - For vectors:
+            - `ord=None`: 2-norm
+            - `ord="fro"`: not supported
+            - `ord="nuc"`: not supported
+            - `ord=np.inf`: `max(abs(x))`
+            - `ord=-np.inf`: `min(abs(x))`
+            - `ord=0`: `sum(x != 0)`
+            - `ord=1`: as below
+            - `ord=-1`: as below
+            - `ord=2`: as below
+            - `ord=-2`: as below
+            - other: `sum(abs(x)**ord)**(1./ord)`
+
+    Returns:
+        Norm of the matrix or vector(s).
+
+    Example:
+
+    >>> x = keras.ops.reshape(keras.ops.arange(9, dtype="float32") - 4, (3, 3))
+    >>> keras.ops.linalg.norm(x)
+    7.7459664
+    """
+    if any_symbolic_tensors((x,)):
+        return Norm(ord=ord, axis=axis, keepdims=keepdims).symbolic_call(x)
+    x = backend.convert_to_tensor(x)
+    return backend.linalg.norm(x, ord=ord, axis=axis, keepdims=keepdims)
+
+
+class Qr(Operation):
+    def __init__(self, mode="reduced"):
+        super().__init__()
+        if mode not in {"reduced", "complete"}:
+            raise ValueError(
+                "`mode` argument value not supported. "
+                "Expected one of {'reduced', 'complete'}. "
+                f"Received: mode={mode}"
+            )
+        self.mode = mode
+
+    def compute_output_spec(self, x):
+        if len(x.shape) < 2:
+            raise ValueError(
+                "Input should have rank >= 2. Received: "
+                f"input.shape = {x.shape}"
+            )
+        m = x.shape[-2]
+        n = x.shape[-1]
+        if m is None or n is None:
+            raise ValueError(
+                "Input should have its last 2 dimensions "
+                "fully-defined. Received: "
+                f"input.shape = {x.shape}"
+            )
+        k = min(m, n)
+        base = tuple(x.shape[:-2])
+        if self.mode == "reduced":
+            return (
+                KerasTensor(shape=base + (m, k), dtype=x.dtype),
+                KerasTensor(shape=base + (k, n), dtype=x.dtype),
+            )
+        # 'complete' mode.
+        return (
+            KerasTensor(shape=base + (m, m), dtype=x.dtype),
+            KerasTensor(shape=base + (m, n), dtype=x.dtype),
         )
-        mean = cast(mean, ori_dtype)
-        variance = cast(variance, ori_dtype)
-    return mean, variance
-
-
-def batch_normalization(
-    x, mean, variance, axis, offset=None, scale=None, epsilon=1e-3
-):
-    shape = [1] * len(x.shape)
-    shape[axis] = mean.shape[0]
-    mean = np.reshape(mean, shape)
-    variance = np.reshape(variance, shape)
-
-    inv = 1.0 / np.sqrt(variance + epsilon)
-    if scale is not None:
-        scale = np.reshape(scale, shape)
-        inv = inv * scale
-
-    res = -mean * inv
-    if offset is not None:
-        offset = np.reshape(offset, shape)
-        res = res + offset
-
-    return x * inv + res
-
-
-def ctc_decode(
-    inputs,
-    sequence_length,
-    strategy,
-    beam_width=100,
-    top_paths=1,
-    merge_repeated=True,
-    mask_index=None,
-):
-    raise NotImplementedError(
-        "NumPy backend does not yet support CTC decoding."
-    )
+
+    def call(self, x):
+        x = backend.convert_to_tensor(x)
+        return backend.linalg.qr(x, mode=self.mode)
+
+
+@keras_export(["keras.ops.qr", "keras.ops.linalg.qr"])
+def qr(x, mode="reduced"):
+    """Computes the QR decomposition of a tensor.
+
+    Args:
+        x: Input tensor of shape `(..., M, N)`.
+        mode: A string specifying the mode of the QR decomposition.
+            - 'reduced': Returns the reduced QR decomposition. (default)
+            - 'complete': Returns the complete QR decomposition.
+
+    Returns:
+        A tuple containing two tensors. The first tensor of shape `(..., M, K)`
+        is the orthogonal matrix `q` and the second tensor of shape
+        `(..., K, N)` is the upper triangular matrix `r`, where `K = min(M, N)`.
+
+    Example:
+
+    >>> x = keras.ops.convert_to_tensor([[1., 2.], [3., 4.], [5., 6.]])
+    >>> q, r = qr(x)
+    >>> print(q)
+    array([[-0.16903079  0.897085]
+           [-0.5070925   0.2760267 ]
+           [-0.8451542  -0.34503305]], shape=(3, 2), dtype=float32)
+    """
+    if any_symbolic_tensors((x,)):
+        return Qr(mode=mode).symbolic_call(x)
+    x = backend.convert_to_tensor(x)
+    return backend.linalg.qr(x, mode=mode)
+
+
+class Solve(Operation):
+
+    def __init__(self):
+        super().__init__()
+
+    def call(self, a, b):
+        return _solve(a, b)
+
+    def compute_output_spec(self, a, b):
+        _assert_2d(a)
+        _assert_square(a)
+        _assert_1d(b)
+        _assert_a_b_compat(a, b)
+        return KerasTensor(b.shape, b.dtype)
+
+
+@keras_export(["keras.ops.solve", "keras.ops.linalg.solve"])
+def solve(a, b):
+    """Solves a linear system of equations given by `a x = b`.
+
+    Args:
+        a: A tensor of shape `(..., M, M)` representing the coefficients matrix.
+        b: A tensor of shape `(..., M)` or `(..., M, N)` represeting the
+        right-hand side or "dependent variable" matrix.
+
+    Returns:
+        A tensor of shape `(..., M)` or `(..., M, N)` representing the solution
+        of the linear system. Returned shape is identical to `b`.
+
+    """
+    if any_symbolic_tensors((a, b)):
+        return Solve().symbolic_call(a, b)
+    return _solve(a, b)
+
+
+def _solve(a, b):
+    a = backend.convert_to_tensor(a)
+    b = backend.convert_to_tensor(b)
+    _assert_2d(a)
+    _assert_square(a)
+    _assert_1d(b)
+    _assert_a_b_compat(a, b)
+    return backend.linalg.solve(a, b)
+
+
+class SolveTriangular(Operation):
+
+    def __init__(self, lower=False):
+        super().__init__()
+        self.lower = lower
+
+    def call(self, a, b):
+        return _solve_triangular(a, b, self.lower)
+
+    def compute_output_spec(self, a, b):
+        _assert_2d(a)
+        _assert_square(a)
+        _assert_1d(b)
+        _assert_a_b_compat(a, b)
+        return KerasTensor(b.shape, b.dtype)
+
+
+@keras_export(
+    ["keras.ops.solve_triangular", "keras.ops.linalg.solve_triangular"]
+)
+def solve_triangular(a, b, lower=False):
+    """Solves a linear system of equations given by `a x = b`.
+
+    Args:
+        a: A tensor of shape `(..., M, M)` representing the coefficients matrix.
+        b: A tensor of shape `(..., M)` or `(..., M, N)` represeting the
+        right-hand side or "dependent variable" matrix.
+
+    Returns:
+        A tensor of shape `(..., M)` or `(..., M, N)` representing the solution
+        of the linear system. Returned shape is identical to `b`.
+
+    """
+    if any_symbolic_tensors((a, b)):
+        return SolveTriangular(lower).symbolic_call(a, b)
+    return _solve_triangular(a, b, lower)
+
+
+def _solve_triangular(a, b, lower=False):
+    a = backend.convert_to_tensor(a)
+    b = backend.convert_to_tensor(b)
+    _assert_2d(a)
+    _assert_square(a)
+    _assert_1d(b)
+    _assert_a_b_compat(a, b)
+    return backend.linalg.solve_triangular(a, b, lower)
+
+
+class SVD(Operation):
+
+    def __init__(self, full_matrices=True, compute_uv=True):
+        super().__init__()
+        self.full_matrices = full_matrices
+        self.compute_uv = compute_uv
+
+    def call(self, x):
+        return _svd(x, self.full_matrices, self.compute_uv)
+
+    def compute_output_spec(self, x):
+        _assert_2d(x)
+        rows, columns = x.shape[-2:]
+        batches = x.shape[:-2]
+        s_shape = batches + (min(rows, columns),)
+        if self.full_matrices:
+            u_shape = batches + (rows, rows)
+            v_shape = batches + (columns, columns)
+        else:
+            u_shape = batches + (rows, min(rows, columns))
+            v_shape = batches + (min(rows, columns), columns)
+
+        if self.compute_uv:
+            return (
+                KerasTensor(u_shape, x.dtype),
+                KerasTensor(s_shape, x.dtype),
+                KerasTensor(v_shape, x.dtype),
+            )
+        return KerasTensor(s_shape, x.dtype)
+
+
+@keras_export(["keras.ops.svd", "keras.ops.linalg.svd"])
+def svd(x, full_matrices=True, compute_uv=True):
+    """Computes the singular value decomposition of a matrix.
+
+    Args:
+        x: Input tensor of shape `(..., M, N)`.
+
+    Returns:
+        A tuple of three tensors: a tensor of shape `(..., M, M)` containing the
+        left singular vectors, a tensor of shape `(..., M, N)` containing the
+        singular values and a tensor of shape `(..., N, N)` containing the
+        right singular vectors.
+
+    """
+    if any_symbolic_tensors((x,)):
+        return SVD(full_matrices, compute_uv).symbolic_call(x)
+    return _svd(x, full_matrices, compute_uv)
+
+
+def _svd(x, full_matrices=True, compute_uv=True):
+    x = backend.convert_to_tensor(x)
+    _assert_2d(x)
+    return backend.linalg.svd(x, full_matrices, compute_uv)
+
+
+def _assert_1d(*arrays):
+    for a in arrays:
+        if a.ndim < 1:
+            raise ValueError(
+                "Expected input to have rank >= 1. "
+                "Received scalar input {a}."
+            )
+
+
+def _assert_2d(*arrays):
+    for a in arrays:
+        if a.ndim < 2:
+            raise ValueError(
+                "Expected input to have rank >= 2. "
+                "Received input with shape {a.shape}."
+            )
+
+
+def _assert_square(*arrays):
+    for a in arrays:
+        m, n = a.shape[-2:]
+        if m != n:
+            raise ValueError(
+                "Expected a square matrix. "
+                f"Received non-square input with shape {a.shape}"
+            )
+
+
+def _assert_a_b_compat(a, b):
+    if a.ndim == b.ndim:
+        if a.shape[-2] != b.shape[-2]:
+            raise ValueError(
+                "Incompatible shapes between `a` and `b`. "
+                "Expected `a.shape[-2] == b.shape[-2]`. "
+                f"Received: a.shape={a.shape}, b.shape={b.shape}"
+            )
+    elif a.ndim == b.ndim - 1:
+        if a.shape[-1] != b.shape[-1]:
+            raise ValueError(
+                "Incompatible shapes between `a` and `b`. "
+                "Expected `a.shape[-1] == b.shape[-1]`. "
+                f"Received: a.shape={a.shape}, b.shape={b.shape}"
+            )
```

### Comparing `keras-3.3.2/keras/src/backend/numpy/numpy.py` & `keras-3.3.3/keras/src/backend/numpy/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1094,7 +1094,11 @@
     x1 = convert_to_tensor(x1, dtype)
     x2 = convert_to_tensor(x2, dtype)
     return np.correlate(x1, x2, mode)
 
 
 def select(condlist, choicelist, default=0):
     return np.select(condlist, choicelist, default=default)
+
+
+def slogdet(x):
+    return tuple(np.linalg.slogdet(x))
```

### Comparing `keras-3.3.2/keras/src/backend/numpy/random.py` & `keras-3.3.3/keras/src/backend/numpy/random.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/numpy/rnn.py` & `keras-3.3.3/keras/src/backend/numpy/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/numpy/trainer.py` & `keras-3.3.3/keras/src/backend/numpy/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/tensorflow/__init__.py` & `keras-3.3.3/keras/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/tensorflow/core.py` & `keras-3.3.3/keras/src/backend/tensorflow/core.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/tensorflow/distribution_lib.py` & `keras-3.3.3/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/tensorflow/image.py` & `keras-3.3.3/keras/src/backend/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/tensorflow/layer.py` & `keras-3.3.3/keras/src/backend/tensorflow/layer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/tensorflow/linalg.py` & `keras-3.3.3/keras/src/backend/tensorflow/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/tensorflow/math.py` & `keras-3.3.3/keras/src/backend/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/tensorflow/nn.py` & `keras-3.3.3/keras/src/backend/tensorflow/nn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import math
 import warnings
 
 import tensorflow as tf
 
-from keras.src.backend import standardize_data_format
-from keras.src.backend import standardize_dtype
+from keras.src import backend
 from keras.src.backend.common.backend_utils import (
     compute_conv_transpose_output_shape,
 )
-from keras.src.backend.config import epsilon
 from keras.src.backend.tensorflow.core import cast
 from keras.src.backend.tensorflow.core import convert_to_tensor
 
 
 def relu(x):
     return tf.nn.relu(x)
 
@@ -71,38 +69,15 @@
 
 def selu(x):
     return tf.nn.selu(x)
 
 
 def gelu(x, approximate=True):
     x = convert_to_tensor(x)
-    # we need to explicitly implement gelu because bfloat16 will trigger
-    # DTypePromotionError when using enable_numpy_behavior()
-    if approximate:
-        coeff = tf.constant(0.044715, x.dtype)
-        return (
-            tf.constant(0.5, x.dtype)
-            * x
-            * (
-                tf.constant(1.0, x.dtype)
-                + tf.math.tanh(
-                    tf.constant(0.7978845608028654, x.dtype)
-                    * (x + coeff * tf.pow(x, 3))
-                )
-            )
-        )
-    else:
-        return (
-            tf.constant(0.5, x.dtype)
-            * x
-            * (
-                tf.constant(1.0, x.dtype)
-                + tf.math.erf(x / tf.constant(1.4142135623730951, x.dtype))
-            )
-        )
+    return tf.nn.gelu(x, approximate=approximate)
 
 
 def softmax(x, axis=-1):
     logits = x
     if axis is None:
         # Unlike numpy, tf will handle axis=None as axis=-1.
         # We need this workaround for the reduction on every dim.
@@ -158,15 +133,15 @@
 def max_pool(
     inputs,
     pool_size,
     strides=None,
     padding="valid",
     data_format=None,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     strides = pool_size if strides is None else strides
     padding = padding.upper()
     tf_data_format = _convert_data_format("channels_last", len(inputs.shape))
     if data_format == "channels_first":
         # Tensorflow pooling does not support `channels_first` format, so
         # we need to transpose to `channels_last` format.
         inputs = _transpose_spatial_inputs(inputs)
@@ -186,15 +161,15 @@
 def average_pool(
     inputs,
     pool_size,
     strides=None,
     padding="valid",
     data_format=None,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     strides = pool_size if strides is None else strides
     padding = padding.upper()
     tf_data_format = _convert_data_format("channels_last", len(inputs.shape))
     if data_format == "channels_first":
         # Tensorflow pooling does not support `channels_first` format, so
         # we need to transpose to `channels_last` format.
         inputs = _transpose_spatial_inputs(inputs)
@@ -264,15 +239,15 @@
 
     # Reason for making this function is in Tensorflow, `groups > 1` does not
     # work on CPU for `tf.nn.convolution`, but wrapping it by XLA works.
     @tf.function(jit_compile=True)
     def _conv_xla():
         return _conv()
 
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     if data_format == "channels_last":
         channels = inputs.shape[-1]
     else:
         channels = inputs.shape[1]
     if channels != kernel.shape[-2]:
         # If kernel's in_channel does not match input's channels,  it indicates
         # convolution is broken down into groups.
@@ -284,15 +259,15 @@
     inputs,
     kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     num_spatial_dims = len(inputs.shape) - 2
     if num_spatial_dims > 2:
         raise ValueError(
             "`inputs` rank must be 3 (1D conv) or 4 (2D conv). Received: "
             "{inputs.ndim}."
         )
     # Because we use `tf.nn.depthwise_conv2d` for both 1D and 2D convs, we set
@@ -347,15 +322,15 @@
     depthwise_kernel,
     pointwise_kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     num_spatial_dims = len(inputs.shape) - 2
     if num_spatial_dims > 2:
         raise ValueError(
             "`num_spatial_dims` must be 1 or 2. Received: "
             f"num_spatial_dims={num_spatial_dims}."
         )
     # Because we use `tf.nn.separable_conv2d` for both 1D and 2D convs, we set
@@ -410,15 +385,15 @@
     kernel,
     strides=1,
     padding="valid",
     output_padding=None,
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     tf_data_format = _convert_data_format(data_format, len(inputs.shape))
     kernel_size = kernel.shape[:-2]
     filters = kernel.shape[-2]
     input_shape = list(inputs.shape)
     symbolic_shape = tf.shape(inputs)
     for i, e in enumerate(input_shape):
         if e is None:
@@ -593,15 +568,17 @@
     # Adjust the predictions so that the probability of
     # each class for every sample adds up to 1
     # This is needed to ensure that the cross entropy is
     # computed correctly.
     output = output / tf.reduce_sum(output, axis, keepdims=True)
 
     # Compute cross entropy from probabilities.
-    output = tf.clip_by_value(output, epsilon(), 1.0 - epsilon())
+    output = tf.clip_by_value(
+        output, backend.epsilon(), 1.0 - backend.epsilon()
+    )
     return -tf.reduce_sum(target * tf.math.log(output), axis)
 
 
 def sparse_categorical_crossentropy(target, output, from_logits=False, axis=-1):
     """Categorical crossentropy with integer targets.
 
     Args:
@@ -649,15 +626,17 @@
             raise ValueError(
                 "Arguments `target` and `output` must have the same shape "
                 "up until the last dimension: "
                 f"target.shape={target.shape}, output.shape={output.shape}"
             )
 
     if not from_logits:
-        output = tf.clip_by_value(output, epsilon(), 1 - epsilon())
+        output = tf.clip_by_value(
+            output, backend.epsilon(), 1 - backend.epsilon()
+        )
         output = tf.math.log(output)
 
     result = tf.nn.sparse_softmax_cross_entropy_with_logits(
         labels=target, logits=output
     )
     return result
 
@@ -698,26 +677,28 @@
 
     if from_logits:
         return tf.nn.sigmoid_cross_entropy_with_logits(
             labels=target, logits=output
         )
 
     # Compute cross entropy from probabilities.
-    output = tf.clip_by_value(output, epsilon(), 1.0 - epsilon())
+    output = tf.clip_by_value(
+        output, backend.epsilon(), 1.0 - backend.epsilon()
+    )
     bce = target * tf.math.log(output)
     bce += (1 - target) * tf.math.log(1 - output)
     return -bce
 
 
 def moments(x, axes, keepdims=False, synchronized=False):
     # The dynamic range of float16 is too limited for statistics. As a
     # workaround, we simply perform the operations on float32 and convert back
     # to float16
     need_cast = False
-    ori_dtype = standardize_dtype(x.dtype)
+    ori_dtype = backend.standardize_dtype(x.dtype)
     if ori_dtype in ("float16", "bfloat16"):
         need_cast = True
         x = cast(x, "float32")
 
     if synchronized:
         mean, variance = _compute_moments_sync(x, axes, keepdims)
     else:
@@ -793,53 +774,90 @@
 def ctc_loss(
     target,
     output,
     target_length,
     output_length,
     mask_index=0,
 ):
-    target = tf.convert_to_tensor(target)
+    target = convert_to_tensor(target)
+    output = convert_to_tensor(output)
     target = tf.cast(target, dtype="int32")
-    output = tf.convert_to_tensor(output)
-    output = tf.cast(output, dtype="float32")
-    return tf.nn.ctc_loss(
+
+    # `tf.nn.ctc_loss` will internally cast to float32 when the input is float16
+    # or bfloat16. Additionally, it will raise an error when the input is
+    # float64. As a result, we perform the casting externally and add support
+    # for float64.
+    result_dtype = backend.result_type(output.dtype, "float32")
+    compute_dtype = "float32" if result_dtype == "float64" else result_dtype
+    output = tf.cast(output, compute_dtype)
+    loss = tf.nn.ctc_loss(
         labels=target,
         logits=output,
         label_length=target_length,
         logit_length=output_length,
         blank_index=mask_index,
         logits_time_major=False,
     )
+    return tf.cast(loss, result_dtype)
 
 
 def ctc_decode(
     inputs,
     sequence_length,
-    strategy,
+    strategy="greedy",
     beam_width=100,
     top_paths=1,
     merge_repeated=True,
     mask_index=None,
 ):
-    inputs = tf.convert_to_tensor(inputs)
+    inputs = convert_to_tensor(inputs)
+    input_shape = tf.shape(inputs)
+    num_samples, num_steps = input_shape[0], input_shape[1]
     inputs = tf.transpose(inputs, (1, 0, 2))
 
-    sequence_length = tf.convert_to_tensor(sequence_length, dtype="int32")
+    dtype = backend.result_type(inputs.dtype, "float32")
+    inputs = tf.cast(inputs, dtype)
+
+    sequence_length = convert_to_tensor(sequence_length, dtype="int32")
     if strategy == "greedy":
-        return tf.nn.ctc_greedy_decoder(
+        (decoded, scores) = tf.nn.ctc_greedy_decoder(
             inputs=inputs,
             sequence_length=sequence_length,
             merge_repeated=merge_repeated,
             blank_index=mask_index,
         )
     elif strategy == "beam_search":
-        return tf.nn.ctc_beam_search_decoder(
+        (decoded, scores) = tf.nn.ctc_beam_search_decoder(
             inputs=inputs,
             sequence_length=sequence_length,
             beam_width=beam_width,
             top_paths=top_paths,
         )
     else:
         raise ValueError(
             f"Invalid strategy {strategy}. Supported values are "
             "'greedy' and 'beam_search'."
         )
+
+    # Postprocess sparse tensor
+    decoded_dense = []
+    for st in decoded:
+        st = tf.SparseTensor(st.indices, st.values, (num_samples, num_steps))
+        decoded_dense.append(tf.sparse.to_dense(sp_input=st, default_value=-1))
+    decoded_dense = tf.stack(decoded_dense, axis=0)
+    decoded_dense = tf.cast(decoded_dense, "int32")
+    return decoded_dense, scores
+
+
+def psnr(x1, x2, max_val):
+    from keras.src.backend.tensorflow.numpy import log10
+
+    if x1.shape != x2.shape:
+        raise ValueError(
+            f"Input shapes {x1.shape} and {x2.shape} must "
+            "match for PSNR calculation. "
+        )
+
+    max_val = convert_to_tensor(max_val, dtype=x2.dtype)
+    mse = tf.reduce_mean(tf.square(x1 - x2))
+    psnr = 20 * log10(max_val) - 10 * log10(mse)
+    return psnr
```

### Comparing `keras-3.3.2/keras/src/backend/tensorflow/numpy.py` & `keras-3.3.3/keras/src/backend/tensorflow/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -2426,7 +2426,12 @@
     x2 = tf.reshape(x2, (x2_len, 1, 1))
 
     return tf.squeeze(tf.nn.conv1d(x1, x2, stride=1, padding=mode.upper()))
 
 
 def select(condlist, choicelist, default=0):
     return tf.experimental.numpy.select(condlist, choicelist, default=default)
+
+
+def slogdet(x):
+    x = convert_to_tensor(x)
+    return tuple(tf.linalg.slogdet(x))
```

### Comparing `keras-3.3.2/keras/src/backend/tensorflow/optimizer.py` & `keras-3.3.3/keras/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/tensorflow/random.py` & `keras-3.3.3/keras/src/backend/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/tensorflow/rnn.py` & `keras-3.3.3/keras/src/backend/tensorflow/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/tensorflow/sparse.py` & `keras-3.3.3/keras/src/backend/tensorflow/sparse.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/tensorflow/trackable.py` & `keras-3.3.3/keras/src/backend/tensorflow/trackable.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/tensorflow/trainer.py` & `keras-3.3.3/keras/src/backend/tensorflow/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/torch/__init__.py` & `keras-3.3.3/keras/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/torch/core.py` & `keras-3.3.3/keras/src/backend/torch/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import contextlib
-import os
 
 import ml_dtypes
 import numpy as np
 import torch
 
 from keras.src import tree
 from keras.src.backend.common import KerasVariable
@@ -15,18 +14,15 @@
 from keras.src.backend.config import floatx
 
 SUPPORTS_SPARSE_TENSORS = False
 
 # Some operators such as 'aten::_foreach_mul_.Scalar'
 # are not currently implemented for the MPS device.
 # check https://github.com/pytorch/pytorch/issues/77764.
-if (
-    torch.backends.mps.is_available()
-    and os.getenv("PYTORCH_ENABLE_MPS_FALLBACK") == "1"
-):
+if torch.backends.mps.is_available():
     DEFAULT_DEVICE = "mps"
 elif torch.cuda.is_available():
     DEFAULT_DEVICE = "cuda"
 else:
     DEFAULT_DEVICE = "cpu"
 
 TORCH_DTYPES = {
```

### Comparing `keras-3.3.2/keras/src/backend/torch/image.py` & `keras-3.3.3/keras/src/backend/torch/image.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/torch/layer.py` & `keras-3.3.3/keras/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/torch/linalg.py` & `keras-3.3.3/keras/src/backend/torch/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/torch/math.py` & `keras-3.3.3/keras/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/torch/nn.py` & `keras-3.3.3/keras/src/backend/torch/nn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import torch
 import torch.nn.functional as tnn
 
+from keras.src import backend
 from keras.src import tree
-from keras.src.backend import standardize_data_format
-from keras.src.backend import standardize_dtype
 from keras.src.backend.common.backend_utils import (
     compute_conv_transpose_padding_args_for_torch,
 )
-from keras.src.backend.config import epsilon
 from keras.src.backend.torch.core import cast
 from keras.src.backend.torch.core import convert_to_tensor
 from keras.src.backend.torch.core import get_device
 from keras.src.backend.torch.numpy import expand_dims
 from keras.src.backend.torch.numpy import maximum
 from keras.src.backend.torch.numpy import where
 from keras.src.utils.argument_validation import standardize_tuple
@@ -88,34 +86,40 @@
     if approximate:
         return tnn.gelu(x, approximate="tanh")
     return tnn.gelu(x)
 
 
 def softmax(x, axis=-1):
     x = convert_to_tensor(x)
-    dtype = standardize_dtype(x.dtype)
+    dtype = backend.standardize_dtype(x.dtype)
     # TODO: tnn.softmax doesn't support float16 using cpu
-    if get_device() == "cpu" and standardize_dtype(x.dtype) == "float16":
+    if (
+        get_device() == "cpu"
+        and backend.standardize_dtype(x.dtype) == "float16"
+    ):
         x = cast(x, "float32")
     if axis is None:
         # Unlike numpy, PyTorch will handle axis=None as axis=-1.
         # We need this workaround for the reduction on every dim.
         output = torch.reshape(x, [-1])
         output = tnn.softmax(output, dim=-1)
         output = torch.reshape(output, x.shape)
     else:
         output = tnn.softmax(x, dim=axis)
     return cast(output, dtype)
 
 
 def log_softmax(x, axis=-1):
     x = convert_to_tensor(x)
-    dtype = standardize_dtype(x.dtype)
+    dtype = backend.standardize_dtype(x.dtype)
     # TODO: tnn.log_softmax doesn't support float16 using cpu
-    if get_device() == "cpu" and standardize_dtype(x.dtype) == "float16":
+    if (
+        get_device() == "cpu"
+        and backend.standardize_dtype(x.dtype) == "float16"
+    ):
         x = cast(x, "float32")
     if axis is None:
         # Unlike numpy, PyTorch will handle axis=None as axis=-1.
         # We need this workaround for the reduction on every dim.
         output = torch.reshape(x, [-1])
         output = tnn.log_softmax(output, dim=-1)
         output = torch.reshape(output, x.shape)
@@ -236,15 +240,15 @@
     num_spatial_dims = inputs.ndim - 2
     pool_size = standardize_tuple(pool_size, num_spatial_dims, "pool_size")
     if strides is None:
         strides = pool_size
     else:
         strides = standardize_tuple(strides, num_spatial_dims, "strides")
 
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     if data_format == "channels_last":
         inputs = _transpose_spatial_inputs(inputs)
 
     if padding == "same":
         # Torch does not natively support `"same"` padding, we need to manually
         # apply the right amount of padding to `inputs`.
         inputs, padding = _apply_same_padding(
@@ -297,15 +301,15 @@
     num_spatial_dims = inputs.ndim - 2
     pool_size = standardize_tuple(pool_size, num_spatial_dims, "pool_size")
     if strides is None:
         strides = pool_size
     else:
         strides = standardize_tuple(strides, num_spatial_dims, "strides")
 
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     if data_format == "channels_last":
         inputs = _transpose_spatial_inputs(inputs)
     padding_value = 0
     if padding == "same":
         spatial_shape = inputs.shape[2:]
         num_spatial_dims = len(spatial_shape)
         padding_value = []
@@ -371,15 +375,15 @@
     dilation_rate=1,
 ):
     inputs = convert_to_tensor(inputs)
     kernel = convert_to_tensor(kernel)
     num_spatial_dims = inputs.ndim - 2
     strides = standardize_tuple(strides, num_spatial_dims, "strides")
 
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     if data_format == "channels_last":
         inputs = _transpose_spatial_inputs(inputs)
     # Transpose kernel from keras format to torch format.
     kernel = _transpose_conv_kernel(kernel)
     if padding == "same" and any(d != 1 for d in tree.flatten(strides)):
         # Torch does not support this case in conv2d().
         # Manually pad the tensor.
@@ -490,15 +494,15 @@
     dilation_rate=1,
 ):
     inputs = convert_to_tensor(inputs)
     kernel = convert_to_tensor(kernel)
     num_spatial_dims = inputs.ndim - 2
     strides = standardize_tuple(strides, num_spatial_dims, "strides")
 
-    data_format = standardize_data_format(data_format)
+    data_format = backend.standardize_data_format(data_format)
     (
         torch_padding,
         torch_output_padding,
     ) = compute_conv_transpose_padding_args_for_torch(
         input_shape=inputs.shape,
         kernel_shape=kernel.shape,
         strides=strides,
@@ -606,15 +610,15 @@
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
 
     if from_logits:
         log_prob = tnn.log_softmax(output, dim=axis)
     else:
         output = output / torch.sum(output, dim=axis, keepdim=True)
-        output = torch.clip(output, epsilon(), 1.0 - epsilon())
+        output = torch.clip(output, backend.epsilon(), 1.0 - backend.epsilon())
         log_prob = torch.log(output)
     return -torch.sum(target * log_prob, dim=axis)
 
 
 def sparse_categorical_crossentropy(target, output, from_logits=False, axis=-1):
     target = convert_to_tensor(target, dtype=torch.long)
     output = convert_to_tensor(output)
@@ -634,15 +638,15 @@
             "up until the last dimension: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
     if from_logits:
         log_prob = tnn.log_softmax(output, dim=axis)
     else:
         output = output / torch.sum(output, dim=axis, keepdim=True)
-        output = torch.clip(output, epsilon(), 1.0 - epsilon())
+        output = torch.clip(output, backend.epsilon(), 1.0 - backend.epsilon())
         log_prob = torch.log(output)
     target = one_hot(target, output.shape[axis], axis=axis)
     return -torch.sum(target * log_prob, dim=axis)
 
 
 def binary_crossentropy(target, output, from_logits=False):
     target = convert_to_tensor(target)
@@ -657,29 +661,29 @@
     # By default, PyTorch, does reduction of `sum` over all rows,
     # change reduction to `none` to keep dim
     if from_logits:
         return tnn.binary_cross_entropy_with_logits(
             output, target, reduction="none"
         )
     else:
-        output = torch.clip(output, epsilon(), 1.0 - epsilon())
+        output = torch.clip(output, backend.epsilon(), 1.0 - backend.epsilon())
         return tnn.binary_cross_entropy(output, target, reduction="none")
 
 
 def moments(x, axes, keepdims=False, synchronized=False):
     if synchronized:
         raise NotImplementedError(
             "Argument synchronized=True is not supported with PyTorch."
         )
     x = convert_to_tensor(x)
     # The dynamic range of float16 is too limited for statistics. As a
     # workaround, we simply perform the operations on float32 and convert back
     # to float16
     need_cast = False
-    ori_dtype = standardize_dtype(x.dtype)
+    ori_dtype = backend.standardize_dtype(x.dtype)
     if ori_dtype == "float16":
         need_cast = True
         x = cast(x, "float32")
 
     mean = torch.mean(x, dim=axes, keepdim=True)
 
     # The variance is computed using $Var = E[|x|^2] - |E[x]|^2$, It is faster
@@ -748,32 +752,116 @@
     mask_index=0,
 ):
     target = convert_to_tensor(target)
     output = convert_to_tensor(output)
     target_length = convert_to_tensor(target_length)
     output_length = convert_to_tensor(output_length)
 
+    # Ensure that the dtype promotion behavior matchs that of `tf.nn.ctc_loss`
+    dtype = backend.result_type(output.dtype, "float32")
+    output = cast(output, dtype)
+
     output = torch.transpose(output, 1, 0)
     logits = tnn.log_softmax(output, dim=-1)
-
-    return tnn.ctc_loss(
+    loss = tnn.ctc_loss(
         logits,
         target,
         output_length,
         target_length,
         blank=mask_index,
         reduction="none",
     )
+    return loss
+
+
+def _ctc_greedy_decode(
+    inputs,
+    sequence_length,
+    merge_repeated=True,
+    mask_index=None,
+):
+    inputs = convert_to_tensor(inputs)
+    sequence_length = convert_to_tensor(sequence_length, dtype="int32")
+    batch_size, max_length, num_classes = inputs.shape
+
+    if mask_index is None:
+        mask_index = num_classes - 1
+
+    indices = torch.argmax(inputs, axis=-1)
+    indices = cast(indices, "int32")
+    scores = torch.max(inputs, axis=-1)[0]
+
+    seqlen_mask = torch.arange(max_length, device=indices.device)[None, :]
+    seqlen_mask = seqlen_mask >= sequence_length[:, None]
+
+    indices = torch.where(seqlen_mask, mask_index, indices)
+    scores = torch.where(seqlen_mask, 0.0, scores)
+
+    if merge_repeated:
+        repeat = indices[:, 1:] == indices[:, :-1]
+        repeat = tnn.pad(repeat, (1, 0, 0, 0))
+        indices = torch.where(repeat, mask_index, indices)
+
+    # We rearrange the indices by moving `mask_index` to the end of the array
+    invalid_mask = indices == mask_index
+    order = torch.unsqueeze(
+        torch.arange(max_length, device=indices.device), dim=0
+    )  # [1, N]
+    order = torch.tile(order, (batch_size, 1))  # [B, N]
+    order = torch.where(invalid_mask, max_length, order)
+    order = torch.argsort(order, dim=-1)
+    indices = torch.take_along_dim(indices, order, dim=-1)
+
+    # We set to -1 for blank labels
+    indices = torch.where(invalid_mask, -1, indices)
+    scores = -torch.sum(scores, axis=1)[:, None]
+    indices = torch.unsqueeze(indices, dim=0)
+    return indices, scores
 
 
 def ctc_decode(
     inputs,
     sequence_length,
-    strategy,
+    strategy="greedy",
     beam_width=100,
     top_paths=1,
     merge_repeated=True,
     mask_index=None,
 ):
-    raise NotImplementedError(
-        "Torch backend does not yet support CTC decoding."
+    inputs = convert_to_tensor(inputs)
+    dtype = backend.result_type(inputs.dtype, "float32")
+    inputs = cast(inputs, dtype)
+
+    if strategy == "greedy":
+        return _ctc_greedy_decode(
+            inputs,
+            sequence_length,
+            merge_repeated=merge_repeated,
+            mask_index=mask_index,
+        )
+    elif strategy == "beam_search":
+        raise NotImplementedError(
+            "Torch backend doesn't yet support the beam search strategy for CTC"
+            "decoding."
+        )
+    else:
+        raise ValueError(
+            f"Invalid strategy {strategy}. Supported values are "
+            "'greedy' and 'beam_search'."
+        )
+
+
+def psnr(x1, x2, max_val):
+    if x1.shape != x2.shape:
+        raise ValueError(
+            f"Input shapes {x1.shape} and {x2.shape} must "
+            "match for PSNR calculation. "
+        )
+
+    x1, x2 = (
+        convert_to_tensor(x1),
+        convert_to_tensor(x2),
     )
+    max_val = convert_to_tensor(max_val, dtype=x1.dtype)
+    mse = torch.mean((x1 - x2) ** 2)
+    psnr = 20 * torch.log10(max_val) - 10 * torch.log10(mse)
+    return psnr
```

### Comparing `keras-3.3.2/keras/src/backend/torch/numpy.py` & `keras-3.3.3/keras/src/backend/torch/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1604,7 +1604,12 @@
 def select(condlist, choicelist, default=0):
     condlist = [convert_to_tensor(c) for c in condlist]
     choicelist = [convert_to_tensor(c) for c in choicelist]
     out = convert_to_tensor(default)
     for c, v in reversed(list(zip(condlist, choicelist))):
         out = torch.where(c, v, out)
     return out
+
+
+def slogdet(x):
+    x = convert_to_tensor(x)
+    return tuple(torch.linalg.slogdet(x))
```

### Comparing `keras-3.3.2/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras-3.3.3/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras-3.3.3/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/torch/optimizers/torch_adam.py` & `keras-3.3.3/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras-3.3.3/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/torch/optimizers/torch_lion.py` & `keras-3.3.3/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras-3.3.3/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras-3.3.3/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras-3.3.3/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras-3.3.3/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras-3.3.3/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/torch/random.py` & `keras-3.3.3/keras/src/backend/torch/random.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/torch/rnn.py` & `keras-3.3.3/keras/src/backend/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/backend/torch/trainer.py` & `keras-3.3.3/keras/src/backend/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/callbacks/__init__.py` & `keras-3.3.3/keras/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/callbacks/backup_and_restore.py` & `keras-3.3.3/keras/src/callbacks/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/callbacks/callback.py` & `keras-3.3.3/keras/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/callbacks/callback_list.py` & `keras-3.3.3/keras/src/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/callbacks/csv_logger.py` & `keras-3.3.3/keras/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/callbacks/early_stopping.py` & `keras-3.3.3/keras/src/callbacks/early_stopping.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
             for `patience` epochs and restore weights from the best epoch in
             that set. Defaults to `False`.
         start_from_epoch: Number of epochs to wait before starting to monitor
             improvement. This allows for a warm-up period in which no
             improvement is expected and thus training will not be stopped.
             Defaults to `0`.
 
-
     Example:
 
     >>> callback = keras.callbacks.EarlyStopping(monitor='loss',
     ...                                               patience=3)
     >>> # This callback will stop the training when there is no improvement in
     >>> # the loss for three consecutive epochs.
     >>> model = keras.models.Sequential([keras.layers.Dense(10)])
```

### Comparing `keras-3.3.2/keras/src/callbacks/history.py` & `keras-3.3.3/keras/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/callbacks/lambda_callback.py` & `keras-3.3.3/keras/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/callbacks/learning_rate_scheduler.py` & `keras-3.3.3/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/callbacks/model_checkpoint.py` & `keras-3.3.3/keras/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/callbacks/progbar_logger.py` & `keras-3.3.3/keras/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras-3.3.3/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/callbacks/remote_monitor.py` & `keras-3.3.3/keras/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/callbacks/swap_ema_weights.py` & `keras-3.3.3/keras/src/callbacks/swap_ema_weights.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/callbacks/tensorboard.py` & `keras-3.3.3/keras/src/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/callbacks/terminate_on_nan.py` & `keras-3.3.3/keras/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/constraints/__init__.py` & `keras-3.3.3/keras/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/constraints/constraints.py` & `keras-3.3.3/keras/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/datasets/boston_housing.py` & `keras-3.3.3/keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/datasets/california_housing.py` & `keras-3.3.3/keras/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/datasets/cifar.py` & `keras-3.3.3/keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/datasets/cifar10.py` & `keras-3.3.3/keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/datasets/cifar100.py` & `keras-3.3.3/keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/datasets/fashion_mnist.py` & `keras-3.3.3/keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/datasets/imdb.py` & `keras-3.3.3/keras/src/datasets/imdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,16 +131,16 @@
             [w if (skip_top <= w < num_words) else oov_char for w in x]
             for x in xs
         ]
     else:
         xs = [[w for w in x if skip_top <= w < num_words] for x in xs]
 
     idx = len(x_train)
-    x_train, y_train = xs[:idx], labels[:idx]
-    x_test, y_test = xs[idx:], labels[idx:]
+    x_train, y_train = np.array(xs[:idx], dtype="object"), labels[:idx]
+    x_test, y_test = np.array(xs[idx:], dtype="object"), labels[idx:]
     return (x_train, y_train), (x_test, y_test)
 
 
 @keras_export("keras.datasets.imdb.get_word_index")
 def get_word_index(path="imdb_word_index.json"):
     """Retrieves a dict mapping words to their index in the IMDB dataset.
```

### Comparing `keras-3.3.2/keras/src/datasets/mnist.py` & `keras-3.3.3/keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/datasets/reuters.py` & `keras-3.3.3/keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/distribution/__init__.py` & `keras-3.3.3/keras/src/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/distribution/distribution_lib.py` & `keras-3.3.3/keras/src/distribution/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/dtype_policies/__init__.py` & `keras-3.3.3/keras/src/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/dtype_policies/dtype_policy.py` & `keras-3.3.3/keras/src/dtype_policies/dtype_policy.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/export/export_lib.py` & `keras-3.3.3/keras/src/export/export_lib.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/initializers/__init__.py` & `keras-3.3.3/keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/initializers/constant_initializers.py` & `keras-3.3.3/keras/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/initializers/initializer.py` & `keras-3.3.3/keras/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/initializers/random_initializers.py` & `keras-3.3.3/keras/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/__init__.py` & `keras-3.3.3/keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/activations/activation.py` & `keras-3.3.3/keras/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/activations/elu.py` & `keras-3.3.3/keras/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/activations/leaky_relu.py` & `keras-3.3.3/keras/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/activations/prelu.py` & `keras-3.3.3/keras/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/activations/relu.py` & `keras-3.3.3/keras/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/activations/softmax.py` & `keras-3.3.3/keras/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/attention/additive_attention.py` & `keras-3.3.3/keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/attention/attention.py` & `keras-3.3.3/keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/attention/grouped_query_attention.py` & `keras-3.3.3/keras/src/layers/attention/grouped_query_attention.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/attention/multi_head_attention.py` & `keras-3.3.3/keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/convolutional/base_conv.py` & `keras-3.3.3/keras/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/convolutional/base_conv_transpose.py` & `keras-3.3.3/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras-3.3.3/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/convolutional/base_separable_conv.py` & `keras-3.3.3/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/convolutional/conv1d.py` & `keras-3.3.3/keras/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/convolutional/conv1d_transpose.py` & `keras-3.3.3/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/convolutional/conv2d.py` & `keras-3.3.3/keras/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/convolutional/conv2d_transpose.py` & `keras-3.3.3/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/convolutional/conv3d.py` & `keras-3.3.3/keras/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/convolutional/conv3d_transpose.py` & `keras-3.3.3/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras-3.3.3/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras-3.3.3/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/convolutional/separable_conv1d.py` & `keras-3.3.3/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/convolutional/separable_conv2d.py` & `keras-3.3.3/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/core/dense.py` & `keras-3.3.3/keras/src/layers/core/dense.py`

 * *Files 2% similar despite different names*

```diff
@@ -553,16 +553,14 @@
             quantized_dtype = f"{mode}_from_{self.dtype_policy.name}"
             # We set the internal `self._dtype_policy` instead of using the
             # setter to avoid double `quantize` call
             self._dtype_policy = dtype_policies.get(quantized_dtype)
 
         self._tracker.unlock()
         if mode == "int8":
-            # Configure `self.inputs_quantizer`
-            self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
             # Quantize `self._kernel` to int8 and compute corresponding scale
             kernel_value, kernel_scale = quantizers.abs_max_quantize(
                 self._kernel, axis=0
             )
             kernel_scale = ops.squeeze(kernel_scale, axis=0)
             self._untrack_variable(self._kernel)
             kernel_shape = self._kernel.shape
```

### Comparing `keras-3.3.2/keras/src/layers/core/einsum_dense.py` & `keras-3.3.3/keras/src/layers/core/einsum_dense.py`

 * *Files 0% similar despite different names*

```diff
@@ -680,18 +680,14 @@
                 self._input_expand_axes,
                 self._kernel_expand_axes,
                 self._input_squeeze_axes,
                 self._kernel_squeeze_axes,
                 self._custom_gradient_equation,
                 self._kernel_reverse_transpose_axes,
             ) = _analyze_quantization_info(self.equation, self.input_spec.ndim)
-            # Configure `self.inputs_quantizer`
-            self.inputs_quantizer = quantizers.AbsMaxQuantizer(
-                axis=self._input_reduced_axes
-            )
             # Quantize `self._kernel` to int8 and compute corresponding scale
             kernel_value, kernel_scale = quantizers.abs_max_quantize(
                 self._kernel, axis=self._kernel_reduced_axes
             )
             kernel_scale = ops.transpose(
                 kernel_scale, self._kernel_transpose_axes
             )
```

### Comparing `keras-3.3.2/keras/src/layers/core/embedding.py` & `keras-3.3.3/keras/src/layers/core/embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,25 +311,27 @@
             )
 
     def _int8_build(
         self,
         embeddings_initializer="zeros",
         embeddings_scale_initializer="ones",
     ):
-        self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
         self._embeddings = self.add_weight(
             name="embeddings",
             shape=(self.input_dim, self.output_dim),
             initializer=embeddings_initializer,
             dtype="int8",
             trainable=False,
         )
+        # We choose to reduce the axis of `output_dim` because, typically,
+        # `input_dim` is larger than `output_dim`. This reduces quantization
+        # error.
         self.embeddings_scale = self.add_weight(
             name="embeddings_scale",
-            shape=(self.output_dim,),
+            shape=(self.input_dim,),
             initializer=embeddings_scale_initializer,
             trainable=False,
         )
         self._is_quantized = True
 
     def quantized_call(self, inputs):
         if self.dtype_policy.quantization_mode == "int8":
@@ -341,19 +343,20 @@
             )
 
     def _int8_call(self, inputs):
         # We cannot update quantized self._embeddings, so the custom gradient is
         # not needed
         if backend.standardize_dtype(inputs.dtype) not in ("int32", "int64"):
             inputs = ops.cast(inputs, "int32")
+        embeddings_scale = ops.take(self.embeddings_scale, inputs, axis=0)
         outputs = ops.take(self._embeddings, inputs, axis=0)
         # De-scale outputs
-        outputs = ops.cast(outputs, self.compute_dtype)
         outputs = ops.divide(
-            outputs, ops.expand_dims(self.embeddings_scale, axis=0)
+            ops.cast(outputs, dtype=self.compute_dtype),
+            ops.expand_dims(embeddings_scale, axis=-1),
         )
         if self.lora_enabled:
             lora_outputs = ops.take(self.lora_embeddings_a, inputs, axis=0)
             lora_outputs = ops.matmul(lora_outputs, self.lora_embeddings_b)
             outputs = ops.add(outputs, lora_outputs)
         return outputs
 
@@ -375,22 +378,20 @@
             quantized_dtype = f"{mode}_from_{self.dtype_policy.name}"
             # We set the internal `self._dtype_policy` instead of using the
             # setter to avoid double `quantize` call
             self._dtype_policy = dtype_policies.get(quantized_dtype)
 
         self._tracker.unlock()
         if mode == "int8":
-            # Configure `self.inputs_quantizer`
-            self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
             # Quantize `self._embeddings` to int8 and compute corresponding
             # scale
             embeddings_value, embeddings_scale = quantizers.abs_max_quantize(
-                self._embeddings, axis=0
+                self._embeddings, axis=-1
             )
-            embeddings_scale = ops.squeeze(embeddings_scale, axis=0)
+            embeddings_scale = ops.squeeze(embeddings_scale, axis=-1)
             self._untrack_variable(self._embeddings)
             del self._embeddings
             # Utilize a lambda expression as an initializer to prevent adding a
             # large constant to the computation graph.
             self._int8_build(
                 lambda shape, dtype: embeddings_value,
                 lambda shape, dtype: embeddings_scale,
@@ -408,19 +409,19 @@
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
             embeddings_value = self._embeddings
             embeddings_scale = self.embeddings_scale
             if self.lora_enabled:
                 # Dequantize & quantize to merge lora weights into embeddings
                 # Note that this is a lossy compression
                 embeddings_value = ops.divide(
-                    embeddings_value, embeddings_scale
+                    embeddings_value, ops.expand_dims(embeddings_scale, axis=-1)
                 )
                 embeddings_value = ops.add(
                     embeddings_value,
                     ops.matmul(self.lora_embeddings_a, self.lora_embeddings_b),
                 )
                 embeddings_value, embeddings_scale = (
-                    quantizers.abs_max_quantize(embeddings_value, axis=0)
+                    quantizers.abs_max_quantize(embeddings_value, axis=-1)
                 )
-                embeddings_scale = ops.squeeze(embeddings_scale, axis=0)
+                embeddings_scale = ops.squeeze(embeddings_scale, axis=-1)
             return embeddings_value, embeddings_scale
         return self.embeddings, None
```

### Comparing `keras-3.3.2/keras/src/layers/core/identity.py` & `keras-3.3.3/keras/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/core/input_layer.py` & `keras-3.3.3/keras/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/core/lambda_layer.py` & `keras-3.3.3/keras/src/layers/core/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/core/masking.py` & `keras-3.3.3/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/core/wrapper.py` & `keras-3.3.3/keras/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/input_spec.py` & `keras-3.3.3/keras/src/layers/input_spec.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/layer.py` & `keras-3.3.3/keras/src/layers/layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from keras.src.backend import KerasTensor
 from keras.src.backend.common import global_state
 from keras.src.backend.common.name_scope import current_path
 from keras.src.distribution import distribution_lib
 from keras.src.layers import input_spec
 from keras.src.metrics.metric import Metric
 from keras.src.ops.operation import Operation
+from keras.src.saving.keras_saveable import KerasSaveable
 from keras.src.utils import python_utils
 from keras.src.utils import summary_utils
 from keras.src.utils import traceback_utils
 from keras.src.utils import tracking
 
 if backend.backend() == "tensorflow":
     from keras.src.backend.tensorflow.layer import TFLayer as BackendLayer
@@ -52,15 +53,15 @@
 else:
     raise RuntimeError(
         f"Backend '{backend.backend()}' must implement a layer mixin class."
     )
 
 
 @keras_export(["keras.Layer", "keras.layers.Layer"])
-class Layer(BackendLayer, Operation):
+class Layer(BackendLayer, Operation, KerasSaveable):
     """This is the class from which all layers inherit.
 
     A layer is a callable object that takes as input one or more tensors and
     that outputs one or more tensors. It involves *computation*, defined
     in the `call()` method, and a *state* (weight variables). State can be
     created:
 
@@ -418,14 +419,17 @@
         if config:
             if "input_shape" in config:
                 self.build(config["input_shape"])
             elif "shapes_dict" in config:
                 self.build(**config["shapes_dict"])
             self.built = True
 
+    def _obj_type(self):
+        return "Layer"
+
     def add_variable(
         self,
         shape,
         initializer,
         dtype=None,
         trainable=True,
         autocast=True,
```

### Comparing `keras-3.3.2/keras/src/layers/merging/add.py` & `keras-3.3.3/keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/merging/average.py` & `keras-3.3.3/keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/merging/base_merge.py` & `keras-3.3.3/keras/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/merging/concatenate.py` & `keras-3.3.3/keras/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/merging/dot.py` & `keras-3.3.3/keras/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/merging/maximum.py` & `keras-3.3.3/keras/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/merging/minimum.py` & `keras-3.3.3/keras/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/merging/multiply.py` & `keras-3.3.3/keras/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/merging/subtract.py` & `keras-3.3.3/keras/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/normalization/batch_normalization.py` & `keras-3.3.3/keras/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/normalization/group_normalization.py` & `keras-3.3.3/keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/normalization/layer_normalization.py` & `keras-3.3.3/keras/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/normalization/spectral_normalization.py` & `keras-3.3.3/keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/normalization/unit_normalization.py` & `keras-3.3.3/keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/pooling/average_pooling1d.py` & `keras-3.3.3/keras/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/pooling/average_pooling2d.py` & `keras-3.3.3/keras/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/pooling/average_pooling3d.py` & `keras-3.3.3/keras/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/pooling/base_global_pooling.py` & `keras-3.3.3/keras/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/pooling/base_pooling.py` & `keras-3.3.3/keras/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/pooling/global_average_pooling1d.py` & `keras-3.3.3/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/pooling/global_average_pooling2d.py` & `keras-3.3.3/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/pooling/global_average_pooling3d.py` & `keras-3.3.3/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/pooling/global_max_pooling1d.py` & `keras-3.3.3/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/pooling/global_max_pooling2d.py` & `keras-3.3.3/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/pooling/global_max_pooling3d.py` & `keras-3.3.3/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/pooling/max_pooling1d.py` & `keras-3.3.3/keras/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/pooling/max_pooling2d.py` & `keras-3.3.3/keras/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/pooling/max_pooling3d.py` & `keras-3.3.3/keras/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras-3.3.3/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/category_encoding.py` & `keras-3.3.3/keras/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/center_crop.py` & `keras-3.3.3/keras/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/discretization.py` & `keras-3.3.3/keras/src/layers/preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/feature_space.py` & `keras-3.3.3/keras/src/layers/preprocessing/feature_space.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/hashed_crossing.py` & `keras-3.3.3/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/hashing.py` & `keras-3.3.3/keras/src/layers/preprocessing/hashing.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/index_lookup.py` & `keras-3.3.3/keras/src/layers/preprocessing/index_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/integer_lookup.py` & `keras-3.3.3/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/normalization.py` & `keras-3.3.3/keras/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/random_brightness.py` & `keras-3.3.3/keras/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/random_contrast.py` & `keras-3.3.3/keras/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/random_crop.py` & `keras-3.3.3/keras/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/random_flip.py` & `keras-3.3.3/keras/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/random_rotation.py` & `keras-3.3.3/keras/src/layers/preprocessing/random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/random_translation.py` & `keras-3.3.3/keras/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/random_zoom.py` & `keras-3.3.3/keras/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/rescaling.py` & `keras-3.3.3/keras/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/resizing.py` & `keras-3.3.3/keras/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/string_lookup.py` & `keras-3.3.3/keras/src/layers/preprocessing/string_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/text_vectorization.py` & `keras-3.3.3/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/preprocessing/tf_data_layer.py` & `keras-3.3.3/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/regularization/activity_regularization.py` & `keras-3.3.3/keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/regularization/alpha_dropout.py` & `keras-3.3.3/keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/regularization/dropout.py` & `keras-3.3.3/keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/regularization/gaussian_dropout.py` & `keras-3.3.3/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/regularization/gaussian_noise.py` & `keras-3.3.3/keras/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/regularization/spatial_dropout.py` & `keras-3.3.3/keras/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/reshaping/cropping1d.py` & `keras-3.3.3/keras/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/reshaping/cropping2d.py` & `keras-3.3.3/keras/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/reshaping/cropping3d.py` & `keras-3.3.3/keras/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/reshaping/flatten.py` & `keras-3.3.3/keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/reshaping/permute.py` & `keras-3.3.3/keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/reshaping/repeat_vector.py` & `keras-3.3.3/keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/reshaping/reshape.py` & `keras-3.3.3/keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/reshaping/up_sampling1d.py` & `keras-3.3.3/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/reshaping/up_sampling2d.py` & `keras-3.3.3/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/reshaping/up_sampling3d.py` & `keras-3.3.3/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/reshaping/zero_padding1d.py` & `keras-3.3.3/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/reshaping/zero_padding2d.py` & `keras-3.3.3/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/reshaping/zero_padding3d.py` & `keras-3.3.3/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/rnn/bidirectional.py` & `keras-3.3.3/keras/src/layers/rnn/bidirectional.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import copy
 
 from keras.src import ops
 from keras.src import utils
 from keras.src.api_export import keras_export
-from keras.src.layers.core.wrapper import Wrapper
 from keras.src.layers.layer import Layer
 from keras.src.saving import serialization_lib
 
 
 @keras_export("keras.layers.Bidirectional")
-class Bidirectional(Wrapper):
+class Bidirectional(Layer):
     """Bidirectional wrapper for RNNs.
 
     Args:
         layer: `keras.layers.RNN` instance, such as
             `keras.layers.LSTM` or `keras.layers.GRU`.
             It could also be a `keras.layers.Layer` instance
             that meets the following criteria:
@@ -101,15 +100,15 @@
             )
         if merge_mode not in ["sum", "mul", "ave", "concat", None]:
             raise ValueError(
                 f"Invalid merge mode. Received: {merge_mode}. "
                 "Merge mode should be one of "
                 '{"sum", "mul", "ave", "concat", None}'
             )
-        super().__init__(layer, **kwargs)
+        super().__init__(**kwargs)
 
         # Recreate the forward layer from the original layer config, so that it
         # will not carry over any state from the layer.
         config = serialization_lib.serialize_keras_object(layer)
         config["config"]["name"] = "forward_" + utils.removeprefix(
             layer.name, "forward_"
         )
@@ -268,16 +267,18 @@
     @property
     def states(self):
         if self.forward_layer.states and self.backward_layer.states:
             return tuple(self.forward_layer.states + self.backward_layer.states)
         return None
 
     def build(self, sequences_shape, initial_state_shape=None):
-        self.forward_layer.build(sequences_shape)
-        self.backward_layer.build(sequences_shape)
+        if not self.forward_layer.built:
+            self.forward_layer.build(sequences_shape)
+        if not self.backward_layer.built:
+            self.backward_layer.build(sequences_shape)
         self.built = True
 
     def compute_mask(self, _, mask):
         if isinstance(mask, list):
             mask = mask[0]
         if self.return_sequences:
             if not self.merge_mode:
```

### Comparing `keras-3.3.2/keras/src/layers/rnn/conv_lstm.py` & `keras-3.3.3/keras/src/layers/rnn/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/rnn/conv_lstm1d.py` & `keras-3.3.3/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/rnn/conv_lstm2d.py` & `keras-3.3.3/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/rnn/conv_lstm3d.py` & `keras-3.3.3/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras-3.3.3/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/rnn/gru.py` & `keras-3.3.3/keras/src/layers/rnn/gru.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/rnn/lstm.py` & `keras-3.3.3/keras/src/layers/rnn/lstm.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/rnn/rnn.py` & `keras-3.3.3/keras/src/layers/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/rnn/simple_rnn.py` & `keras-3.3.3/keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras-3.3.3/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/layers/rnn/time_distributed.py` & `keras-3.3.3/keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/legacy/backend.py` & `keras-3.3.3/keras/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/legacy/layers.py` & `keras-3.3.3/keras/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/legacy/losses.py` & `keras-3.3.3/keras/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/legacy/preprocessing/image.py` & `keras-3.3.3/keras/src/legacy/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/legacy/preprocessing/sequence.py` & `keras-3.3.3/keras/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/legacy/preprocessing/text.py` & `keras-3.3.3/keras/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/legacy/saving/json_utils.py` & `keras-3.3.3/keras/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/legacy/saving/legacy_h5_format.py` & `keras-3.3.3/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/legacy/saving/saving_utils.py` & `keras-3.3.3/keras/src/legacy/saving/saving_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/legacy/saving/serialization.py` & `keras-3.3.3/keras/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/losses/__init__.py` & `keras-3.3.3/keras/src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/losses/loss.py` & `keras-3.3.3/keras/src/losses/loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from keras.src import backend
 from keras.src import ops
 from keras.src import tree
 from keras.src.api_export import keras_export
+from keras.src.saving.keras_saveable import KerasSaveable
 from keras.src.utils.naming import auto_name
 
 
 @keras_export(["keras.Loss", "keras.losses.Loss"])
-class Loss:
+class Loss(KerasSaveable):
     """Loss base class.
 
     To be implemented by subclasses:
 
     * `call()`: Contains the logic for loss calculation using `y_true`,
         `y_pred`.
 
@@ -65,14 +66,17 @@
     def get_config(self):
         return {"name": self.name, "reduction": self.reduction}
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
 
+    def _obj_type(self):
+        return "Loss"
+
 
 def standardize_reduction(reduction):
     allowed = {"sum_over_batch_size", "sum", None, "none"}
     if reduction not in allowed:
         raise ValueError(
             "Invalid value for argument `reduction`. "
             f"Expected one of {allowed}. Received: "
```

### Comparing `keras-3.3.2/keras/src/losses/losses.py` & `keras-3.3.3/keras/src/losses/losses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1889,15 +1889,15 @@
             containing logits (the output of your model).
             They should *not* be normalized via softmax.
     """
 
     def __init__(
         self,
         reduction="sum_over_batch_size",
-        name="sparse_categorical_crossentropy",
+        name="ctc",
     ):
         super().__init__(
             ctc,
             name=name,
             reduction=reduction,
         )
```

### Comparing `keras-3.3.2/keras/src/metrics/__init__.py` & `keras-3.3.3/keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/metrics/accuracy_metrics.py` & `keras-3.3.3/keras/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/metrics/confusion_metrics.py` & `keras-3.3.3/keras/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/metrics/f_score_metrics.py` & `keras-3.3.3/keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/metrics/hinge_metrics.py` & `keras-3.3.3/keras/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/metrics/iou_metrics.py` & `keras-3.3.3/keras/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/metrics/metric.py` & `keras-3.3.3/keras/src/metrics/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from keras.src import backend
 from keras.src import initializers
 from keras.src import ops
 from keras.src.api_export import keras_export
+from keras.src.saving.keras_saveable import KerasSaveable
 from keras.src.utils.naming import auto_name
 from keras.src.utils.tracking import Tracker
 
 
 @keras_export(["keras.Metric", "keras.metrics.Metric"])
-class Metric:
+class Metric(KerasSaveable):
     """Encapsulates metric logic and state.
 
     Args:
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
     Example:
@@ -175,14 +176,17 @@
                 metric_variables.append(v)
         return metric_variables
 
     @property
     def dtype(self):
         return self._dtype
 
+    def _obj_type(self):
+        return "Metric"
+
     def add_variable(
         self, shape, initializer, dtype=None, aggregation="sum", name=None
     ):
         self._check_super_called()
         with backend.name_scope(self.name.replace("/", ">"), caller=self):
             initializer = initializers.get(initializer)
             variable = backend.Variable(
```

### Comparing `keras-3.3.2/keras/src/metrics/metrics_utils.py` & `keras-3.3.3/keras/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/metrics/probabilistic_metrics.py` & `keras-3.3.3/keras/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/metrics/reduction_metrics.py` & `keras-3.3.3/keras/src/metrics/reduction_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/metrics/regression_metrics.py` & `keras-3.3.3/keras/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/models/cloning.py` & `keras-3.3.3/keras/src/models/cloning.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,15 +7,22 @@
 from keras.src.models.functional import Functional
 from keras.src.models.functional import functional_like_constructor
 from keras.src.models.sequential import Sequential
 from keras.src.saving import serialization_lib
 
 
 @keras_export("keras.models.clone_model")
-def clone_model(model, input_tensors=None, clone_function=None):
+def clone_model(
+    model,
+    input_tensors=None,
+    clone_function=None,
+    call_function=None,
+    recursive=False,
+    **kwargs,
+):
     """Clone a Functional or Sequential `Model` instance.
 
     Model cloning is similar to calling a model on new inputs,
     except that it creates new layers (and thus new weights) instead
     of sharing the weights of the existing layers.
 
     Note that
@@ -25,32 +32,52 @@
 
     Args:
         model: Instance of `Model`
             (could be a Functional model or a Sequential model).
         input_tensors: optional list of input tensors or InputLayer objects
             to build the model upon. If not provided,
             new `Input` objects will be created.
-        clone_function: Callable to be used to clone each layer in the target
+        clone_function: Callable with signature `fn(layer)`
+            to be used to clone each layer in the target
             model (except `Input` instances). It takes as argument the
             layer instance to be cloned, and returns the corresponding layer
             instance to be used in the model copy. If unspecified, this callable
-            becomes the following serialization/deserialization function:
+            defaults to the following serialization/deserialization function:
             `lambda layer: layer.__class__.from_config(layer.get_config())`.
             By passing a custom callable, you can customize your copy of the
             model, e.g. by wrapping certain layers of interest (you might want
             to replace all `LSTM` instances with equivalent
             `Bidirectional(LSTM(...))` instances, for example).
             Defaults to `None`.
+        call_function: Callable with signature
+            `fn(layer, *args, **kwargs)` to be used to call each
+            cloned layer and a set of inputs. It takes the layer instance,
+            the call arguments and keyword arguments, and returns the
+            call outputs. If unspecified, this callable defaults to
+            the regular `__call__()` method:
+            `def fn(layer, *args, **kwargs): return layer(*args, **kwargs)`.
+            By passing a custom callable, you can insert new layers before or
+            after a given layer. Note: this argument can only be used with
+            Functional models.
+        recursive: Boolean. Whether to recursively clone any Sequential
+            or Functional models encountered in the original
+            Sequential/Functional model. If `False`,
+            then inner models are cloned by calling `clone_function()`.
+            If `True`, then inner models are cloned by calling `clone_model()`
+            with the same `clone_function`, `call_function`, and `recursive`
+            arguments. Note that in this case, `call_function`
+            will not be propagated to any Sequential model
+            (since it is not applicable to Sequential models).
 
     Returns:
         An instance of `Model` reproducing the behavior
         of the original model, on top of new inputs tensors,
         using newly instantiated weights. The cloned model may behave
         differently from the original model if a custom `clone_function`
-        modifies the layer.
+        or `call_function` modifies a layer or layer call.
 
     Example:
 
     ```python
     # Create a test Sequential model.
     model = keras.Sequential([
         keras.layers.Input(shape=(728,)),
@@ -70,65 +97,166 @@
         if "seed" in config:
             config["seed"] = 1337
         return layer.__class__.from_config(config)
 
     new_model = clone_model(model)
     ```
 
+    Using a `call_function` to add a `Dropout` layer after each `Dense` layer
+    (without recreating new layers):
+
+    ```python
+    def call_function(layer, *args, **kwargs):
+        out = layer(*args, **kwargs)
+        if isinstance(layer, keras.layers.Dense):
+            out = keras.layers.Dropout(0.5)(out)
+        return out
+
+    new_model = clone_model(
+        model,
+        clone_function=lambda x: x,  # Reuse the same layers.
+        call_function=call_function,
+    )
+    ```
+
     Note that subclassed models cannot be cloned by default,
     since their internal layer structure is not known.
     To achieve equivalent functionality
     as `clone_model` in the case of a subclassed model, simply make sure
     that the model class implements `get_config()`
     (and optionally `from_config()`), and call:
 
     ```python
     new_model = model.__class__.from_config(model.get_config())
     ```
 
     In the case of a subclassed model, you cannot using a custom
     `clone_function`.
     """
+    cache = kwargs.pop("cache", None)
+    if kwargs:
+        raise ValueError(
+            f"Unexpected keyword argument(s): {tuple(kwargs.keys())}"
+        )
+
     if isinstance(model, Sequential):
+        # Wrap clone_function to handle recursiveness and layer sharing.
+        clone_function = _wrap_clone_function(
+            clone_function,
+            call_function=call_function,
+            recursive=recursive,
+            cache=cache,
+        )
+        if call_function is not None:
+            raise ValueError(
+                "`call_function` argument is not supported with Sequential "
+                "models.  In a Sequential model, layers aren't called "
+                "at model-construction time (they're merely listed). "
+                "Use `call_function` with Functional models only. "
+                "Received model of "
+                f"type '{model.__class__.__name__}', with "
+                f"call_function={clone_function}"
+            )
         return _clone_sequential_model(
-            model, input_tensors=input_tensors, clone_function=clone_function
+            model,
+            clone_function=clone_function,
+            input_tensors=input_tensors,
         )
     if isinstance(model, Functional):
+        # Wrap clone_function to handle recursiveness and layer sharing.
+        clone_function = _wrap_clone_function(
+            clone_function,
+            call_function=call_function,
+            recursive=recursive,
+            cache=cache,
+        )
+
         # If the get_config() method is the same as a regular Functional
         # model, we're safe to use _clone_functional_model (which relies
         # on a Functional constructor). In the case where the get_config
         # is custom, this may not necessarily work, but if clone_function
         # or input_tensors are passed, we attempt it anyway
         # in order to preserve backwards compatibility.
         if utils.is_default(model.get_config) or (
             clone_function or input_tensors
         ):
             return _clone_functional_model(
                 model,
-                input_tensors=input_tensors,
                 clone_function=clone_function,
+                call_function=call_function,
+                input_tensors=input_tensors,
             )
 
     # Case of a custom model class
     if clone_function or input_tensors:
         raise ValueError(
-            "Arguments clone_function and input_tensors "
+            "Arguments `clone_function` and `input_tensors` "
             "are only supported for Sequential models "
             "or Functional models. Received model of "
             f"type '{model.__class__.__name__}', with "
             f"clone_function={clone_function} and "
             f"input_tensors={input_tensors}"
         )
+    if call_function is not None:
+        raise ValueError(
+            "Argument `call_function` is only supported "
+            "for Functional models. Received model of "
+            f"type '{model.__class__.__name__}', with "
+            f"call_function={clone_function}"
+        )
     config = serialization_lib.serialize_keras_object(model)
     return serialization_lib.deserialize_keras_object(
         config, custom_objects={model.__class__.__name__: model.__class__}
     )
 
 
-def _clone_sequential_model(model, input_tensors=None, clone_function=None):
+def _wrap_clone_function(
+    clone_function, call_function=None, recursive=False, cache=None
+):
+    """Wrapper to handle recursiveness and layer sharing."""
+    if clone_function is None:
+
+        def _clone_layer(layer):
+            return layer.__class__.from_config(layer.get_config())
+
+        clone_function = _clone_layer
+
+    if cache is None:
+        cache = {}
+
+    def wrapped_clone_function(layer):
+        if id(layer) in cache:
+            return cache[id(layer)]
+        if recursive:
+            if isinstance(layer, Sequential):
+                # Note: Sequential doens't support call_function.
+                clone = clone_model(
+                    layer,
+                    clone_function=clone_function,
+                    cache=cache,
+                )
+                cache[id(layer)] = clone
+                return clone
+            elif isinstance(layer, Functional):
+                clone = clone_model(
+                    layer,
+                    clone_function=clone_function,
+                    call_function=call_function,
+                    cache=cache,
+                )
+                cache[id(layer)] = clone
+                return clone
+        clone = clone_function(layer)
+        cache[id(layer)] = clone
+        return clone
+
+    return wrapped_clone_function
+
+
+def _clone_sequential_model(model, clone_function, input_tensors=None):
     """Clone a `Sequential` model instance.
 
     Model cloning is similar to calling a model on new inputs,
     except that it creates new layers (and thus new weights) instead
     of sharing the weights of the existing layers.
 
     Args:
@@ -140,20 +268,14 @@
             By default, it clones the layer (without copying the weights).
 
     Returns:
         An instance of `Sequential` reproducing the behavior
         of the original model, on top of new inputs tensors,
         using newly instantiated weights.
     """
-    if clone_function is None:
-
-        def _clone_layer(layer):
-            return layer.__class__.from_config(layer.get_config())
-
-        clone_function = _clone_layer
 
     if not isinstance(model, Sequential):
         raise ValueError(
             "Expected `model` argument "
             "to be a `Sequential` model instance. "
             f"Received: model={model}"
         )
@@ -198,15 +320,17 @@
                 dtype=input_dtype,
                 name=input_name,
             )
             new_layers = [inputs] + new_layers
     return Sequential(new_layers, name=model.name, trainable=model.trainable)
 
 
-def _clone_functional_model(model, input_tensors=None, clone_function=None):
+def _clone_functional_model(
+    model, clone_function, input_tensors=None, call_function=None
+):
     """Clone a `Functional` model instance.
 
     Model cloning is similar to calling a model on new inputs,
     except that it creates new layers (and thus new weights) instead
     of sharing the weights of the existing layers.
 
     Input layers are always cloned.
@@ -220,25 +344,14 @@
             By default, it clones the layer (without copying the weights).
 
     Returns:
         An instance of `Functional` reproducing the behavior
         of the original model, on top of new inputs tensors,
         using newly instantiated weights.
     """
-    if clone_function is None:
-        seen = {}
-
-        def _clone_layer(layer):
-            if layer in seen:
-                return seen[layer]
-            new_layer = layer.__class__.from_config(layer.get_config())
-            seen[layer] = new_layer
-            return new_layer
-
-        clone_function = _clone_layer
 
     if not callable(clone_function):
         raise ValueError(
             "Expected `clone_function` argument to be a callable. "
             f"Received: clone_function={clone_function}"
         )
 
@@ -272,15 +385,17 @@
         )
 
     def operation_fn(layer):
         new_layer = clone_function(layer)
         return new_layer
 
     output_tensors = model._run_through_graph(
-        input_tensors, operation_fn=operation_fn
+        input_tensors,
+        operation_fn=operation_fn,
+        call_fn=call_function,
     )
 
     if functional_like_constructor(model.__class__):
         new_model = model.__class__(
             input_tensors, output_tensors, name=model.name
         )
     else:
```

### Comparing `keras-3.3.2/keras/src/models/functional.py` & `keras-3.3.3/keras/src/models/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,17 @@
 
     def _lock_state(self):
         # Unlike other layers, we allow Functional state to be mutable after
         # build. E.g. to attach a layer to a model that is not part of the
         # functional DAG.
         pass
 
+    def _obj_type(self):
+        return "Functional"
+
     @property
     def layers(self):
         layers = []
         for operation in self._operations:
             if isinstance(operation, Layer):
                 layers.append(operation)
         return layers
```

### Comparing `keras-3.3.2/keras/src/models/model.py` & `keras-3.3.3/keras/src/models/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import inspect
-import io
 import json
 import typing
 import warnings
 
-import keras.src.saving.saving_lib as saving_lib
 from keras.src import backend
 from keras.src import utils
 from keras.src.api_export import keras_export
 from keras.src.layers.layer import Layer
-from keras.src.models.variable_mapping import map_trackable_variables
+from keras.src.models.variable_mapping import map_saveable_variables
 from keras.src.saving import saving_api
 from keras.src.trainers import trainer as base_trainer
 from keras.src.utils import summary_utils
 from keras.src.utils import traceback_utils
 
 if backend.backend() == "tensorflow":
     from keras.src.backend.tensorflow.trainer import (
@@ -346,38 +344,14 @@
                 there is a mismatch in the number of weights, or a mismatch in
                 the shape of the weights.
         """
         saving_api.load_weights(
             self, filepath, skip_mismatch=skip_mismatch, **kwargs
         )
 
-    # Note: renaming this function will cause old pickles to be broken.
-    # This is probably not a huge deal, as pickle should not be a recommended
-    # saving format -- it should only be supported for use with distributed
-    # computing frameworks.
-    @classmethod
-    def _unpickle_model(cls, bytesio):
-        # pickle is not safe regardless of what you do.
-        return saving_lib._load_model_from_fileobj(
-            bytesio, custom_objects=None, compile=True, safe_mode=False
-        )
-
-    def __reduce__(self):
-        """__reduce__ is used to customize the behavior of `pickle.pickle()`.
-
-        The method returns a tuple of two elements: a function, and a list of
-        arguments to pass to that function.  In this case we just leverage the
-        keras saving library."""
-        buf = io.BytesIO()
-        saving_lib._save_model_to_fileobj(self, buf, "h5")
-        return (
-            self._unpickle_model,
-            (buf,),
-        )
-
     def quantize(self, mode):
         """Quantize the weights of the model.
 
         Note that the model must be built first before calling this method.
         `quantize` will recursively call `quantize(mode)` in all layers and
         will be skipped if the layer doesn't implement the function.
 
@@ -566,15 +540,15 @@
                 f"instance of {cls.__name__} from its config.\n\n"
                 f"Received config={config}\n\n"
                 f"Error encountered during deserialization: {e}"
             )
 
     def _get_variable_map(self):
         store = {}
-        map_trackable_variables(self, store=store, visited_trackables=set())
+        map_saveable_variables(self, store=store, visited_saveables=set())
         return store
 
 
 @keras_export("keras.models.model_from_json")
 def model_from_json(json_string, custom_objects=None):
     """Parses a JSON model configuration string and returns a model instance.
```

### Comparing `keras-3.3.2/keras/src/models/sequential.py` & `keras-3.3.3/keras/src/models/sequential.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,17 @@
             input_shape = self._layers[0].batch_shape
             self.build(input_shape)
 
     def _lock_state(self):
         # Unlike other layers, Sequential is mutable after build.
         pass
 
+    def _obj_type(self):
+        return "Sequential"
+
     def build(self, input_shape=None):
         if not isinstance(input_shape, (tuple, list)):
             # Do not attempt to build if the model does not have a single
             # input tensor.
             return
         if input_shape and not (
             isinstance(input_shape[0], int) or input_shape[0] is None
```

### Comparing `keras-3.3.2/keras/src/models/variable_mapping.py` & `keras-3.3.3/keras/src/models/variable_mapping.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 from keras.src.layers.layer import Layer
 from keras.src.metrics.metric import Metric
 from keras.src.optimizers.optimizer import Optimizer
 from keras.src.saving import saving_lib
+from keras.src.saving.keras_saveable import KerasSaveable
 
 
-def map_trackable_variables(trackable, store, visited_trackables):
-    # If the trackable has already been saved, skip it.
-    if id(trackable) in visited_trackables:
+def map_saveable_variables(saveable, store, visited_saveables):
+    # If the saveable has already been seen, skip it.
+    if id(saveable) in visited_saveables:
         return
 
-    visited_trackables.add(id(trackable))
+    visited_saveables.add(id(saveable))
 
     variables = []
-    if isinstance(trackable, Layer):
+    if isinstance(saveable, Layer):
         variables = (
-            trackable._trainable_variables + trackable._non_trainable_variables
+            saveable._trainable_variables + saveable._non_trainable_variables
         )
-    elif isinstance(trackable, Optimizer):
-        variables = trackable._variables
-    elif isinstance(trackable, Metric):
-        variables = trackable._variables
+    elif isinstance(saveable, Optimizer):
+        variables = saveable._variables
+    elif isinstance(saveable, Metric):
+        variables = saveable._variables
     for v in variables:
         if v.path in store:
             raise ValueError(
                 "The model contains two variables with a duplicate path: "
                 f"path='{v.path}' appears at least twice. "
                 f"This path is used for {v} and for {store[v.path]}. "
                 "In order to get a variable map, make sure to use "
                 "unique paths/names for each variable."
             )
         store[v.path] = v
 
-    # Recursively save state of children trackables (layers, optimizers, etc.)
-    for child_attr, child_obj in saving_lib._walk_trackable(trackable):
-        if saving_lib._is_keras_trackable(child_obj):
-            map_trackable_variables(
+    # Recursively save state of children saveables (layers, optimizers, etc.)
+    for child_attr, child_obj in saving_lib._walk_saveable(saveable):
+        if isinstance(child_obj, KerasSaveable):
+            map_saveable_variables(
                 child_obj,
                 store,
-                visited_trackables=visited_trackables,
+                visited_saveables=visited_saveables,
             )
         elif isinstance(child_obj, (list, dict, tuple, set)):
             map_container_variables(
                 child_obj,
                 store,
-                visited_trackables=visited_trackables,
+                visited_saveables=visited_saveables,
             )
 
 
-def map_container_variables(container, store, visited_trackables):
+def map_container_variables(container, store, visited_saveables):
     if isinstance(container, dict):
         container = list(container.values())
 
-    for trackable in container:
-        if saving_lib._is_keras_trackable(trackable):
-            map_trackable_variables(
-                trackable,
+    for saveable in container:
+        if isinstance(saveable, KerasSaveable):
+            map_saveable_variables(
+                saveable,
                 store,
-                visited_trackables=visited_trackables,
+                visited_saveables=visited_saveables,
             )
```

### Comparing `keras-3.3.2/keras/src/ops/__init__.py` & `keras-3.3.3/keras/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/ops/core.py` & `keras-3.3.3/keras/src/ops/core.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/ops/function.py` & `keras-3.3.3/keras/src/ops/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         )
 
     def call(self, inputs):
         """Computes output tensors for new inputs."""
         self._assert_input_compatibility(inputs)
         return self._run_through_graph(inputs, operation_fn=lambda op: op)
 
-    def _run_through_graph(self, inputs, operation_fn):
+    def _run_through_graph(self, inputs, operation_fn, call_fn=None):
         """Execute the graph.
 
         At each node we compute outputs via
         `operation_fn(node.operation)(*args, **kwargs)`.
         """
         inputs = tree.flatten(inputs)
 
@@ -144,15 +144,19 @@
                 if not node.operation or node.is_input:
                     continue  # Input tensors already exist.
 
                 if any(id(x) not in tensor_dict for x in node.input_tensors):
                     continue  # Node is not computable, try skipping.
 
                 args, kwargs = node.arguments.fill_in(tensor_dict)
-                outputs = operation_fn(node.operation)(*args, **kwargs)
+                op = operation_fn(node.operation)
+                if call_fn is not None:
+                    outputs = call_fn(op, *args, **kwargs)
+                else:
+                    outputs = op(*args, **kwargs)
 
                 # Update tensor_dict.
                 for x, y in zip(node.outputs, tree.flatten(outputs)):
                     tensor_dict[id(x)] = y
 
         output_tensors = []
         for x in self.outputs:
```

### Comparing `keras-3.3.2/keras/src/ops/image.py` & `keras-3.3.3/keras/src/ops/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,15 +544,15 @@
     if data_format == "channels_last":
         channels_in = image.shape[-1]
     elif data_format == "channels_first":
         channels_in = image.shape[-3]
     if not strides:
         strides = size
     out_dim = patch_h * patch_w * channels_in
-    kernel = backend.numpy.eye(out_dim)
+    kernel = backend.numpy.eye(out_dim, dtype=image.dtype)
     kernel = backend.numpy.reshape(
         kernel, (patch_h, patch_w, channels_in, out_dim)
     )
     _unbatched = False
     if len(image.shape) == 3:
         _unbatched = True
         image = backend.numpy.expand_dims(image, axis=0)
```

### Comparing `keras-3.3.2/keras/src/ops/math.py` & `keras-3.3.3/keras/src/ops/math.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/ops/nn.py` & `keras-3.3.3/keras/src/ops/nn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1806,16 +1806,16 @@
         )
 
     return backend.nn.batch_normalization(
         x, mean, variance, axis, offset, scale, epsilon
     )
 
 
-class CtcLoss(Operation):
-    def __init__(self, mask_index):
+class CTCLoss(Operation):
+    def __init__(self, mask_index=0):
         super().__init__()
         self.mask_index = mask_index
 
     def call(self, target, output, target_length, output_length):
         return backend.nn.ctc_loss(
             target, output, target_length, output_length, self.mask_index
         )
@@ -1834,16 +1834,16 @@
         )
         self._check_shape_first_dim(
             "target_length", target_length.shape, "target", target.shape
         )
         self._check_shape_first_dim(
             "output_length", output_length.shape, "output", output.shape
         )
-
-        return KerasTensor((target.shape[0],), dtype=target.dtype)
+        dtype = backend.result_type(output.dtype, "float32")
+        return KerasTensor((target.shape[0],), dtype=dtype)
 
 
 @keras_export(
     [
         "keras.ops.ctc_loss",
         "keras.ops.nn.ctc_loss",
     ]
@@ -1861,42 +1861,85 @@
         output_length: A tensor of shape `(batch_size,)` containing the
             output lengths.
         mask_index: The index of the mask character in the vocabulary.
             Defaults to `0`.
     """
 
     if any_symbolic_tensors((target, output, target_length, output_length)):
-        return CtcLoss(mask_index).symbolic_call(
+        return CTCLoss(mask_index).symbolic_call(
             target, output, target_length, output_length
         )
     return backend.nn.ctc_loss(
         target, output, target_length, output_length, mask_index
     )
 
 
+class CTCDecode(Operation):
+    def __init__(
+        self,
+        strategy="greedy",
+        beam_width=100,
+        top_paths=1,
+        merge_repeated=True,
+        mask_index=None,
+    ):
+        super().__init__()
+        self.strategy = strategy
+        self.beam_width = beam_width
+        self.top_paths = top_paths
+        self.merge_repeated = merge_repeated
+        self.mask_index = mask_index
+
+    def call(self, inputs, sequence_lengths):
+        return backend.nn.ctc_decode(
+            inputs,
+            sequence_lengths,
+            strategy=self.strategy,
+            beam_width=self.beam_width,
+            top_paths=self.top_paths,
+            merge_repeated=self.merge_repeated,
+            mask_index=self.mask_index,
+        )
+
+    def compute_output_spec(self, inputs, sequence_lengths):
+        inputs_shape = inputs.shape
+        if self.strategy == "greedy":
+            top_paths = 1
+        else:
+            top_paths = self.top_paths
+        dtype = backend.result_type(inputs.dtype, "float32")
+        return (
+            KerasTensor(
+                (top_paths, inputs_shape[0], inputs_shape[1]), dtype="int32"
+            ),
+            KerasTensor((inputs_shape[0], top_paths), dtype=dtype),
+        )
+
+
 @keras_export(
     [
         "keras.ops.ctc_decode",
         "keras.ops.nn.ctc_decode",
     ]
 )
 def ctc_decode(
     inputs,
     sequence_lengths,
-    strategy,
+    strategy="greedy",
     beam_width=100,
     top_paths=1,
     merge_repeated=True,
     mask_index=None,
 ):
     """Decodes the output of a CTC model.
 
     Args:
         inputs: A tensor of shape `(batch_size, max_length, num_classes)`
-            containing the logits (output of the model).
+            containing the logits (the output of the model).
+            They should *not* be normalized via softmax.
         sequence_lengths: A tensor of shape `(batch_size,)` containing the
             sequence lengths for the batch.
         strategy: A string for the decoding strategy. Supported values are
             `"greedy"` and `"beam_search"`.
         beam_width: An integer scalar beam width used in beam search.
             Defaults to 100.
         top_paths: An integer scalar, the number of top paths to return.
@@ -1904,28 +1947,34 @@
         merge_repeated: A boolean scalar, whether to merge repeated
             labels in the output. Defaults to `True`.
         mask_index: An integer scalar, the index of the mask character in
             the vocabulary. Defaults to `None`.
 
     Returns:
         A tuple containing:
-
-        - A list of decoded sequences.
-        - A list of the negative of the sum of the probability logits
-        (if strategy is `"greedy"`) or the log probability (if strategy is
-        `"beam_search"`) for each sequence.
+        - The tensor representing the list of decoded sequences. If
+            `strategy="greedy"`, the shape is `(1, batch_size, max_length)`. If
+            `strategy="beam_seatch"`, the shape is
+            `(top_paths, batch_size, max_length)`. Note that: `-1` indicates the
+            blank label.
+        - If `strategy="greedy"`, a tensor of shape `(batch_size, 1)`
+            representing the negative of the sum of the probability logits for
+            each sequence. If `strategy="beam_seatch"`, a tensor of shape
+            `(batch_size, top_paths)` representing the log probability for each
+            sequence.
     """
 
     if any_symbolic_tensors((inputs, sequence_lengths)):
-        raise NotImplementedError(
-            "CTC decoding is not supported with KerasTensors. Use it "
-            "inside the call() method of a Layer or the predict_step "
-            "method of a model."
-        )
-
+        return CTCDecode(
+            strategy=strategy,
+            beam_width=beam_width,
+            top_paths=top_paths,
+            merge_repeated=merge_repeated,
+            mask_index=mask_index,
+        ).symbolic_call(inputs, sequence_lengths)
     return backend.nn.ctc_decode(
         inputs=inputs,
         sequence_length=sequence_lengths,
         strategy=strategy,
         beam_width=beam_width,
         top_paths=top_paths,
         merge_repeated=merge_repeated,
@@ -1989,7 +2038,80 @@
     x = backend.convert_to_tensor(x)
     if len(x.shape) == 0:
         x = backend.numpy.expand_dims(x, axis=0)
     epsilon = backend.epsilon()
     norm = backend.linalg.norm(x, ord=order, axis=axis, keepdims=True)
     denom = backend.numpy.maximum(norm, epsilon)
     return backend.numpy.divide(x, denom)
+
+
+class PSNR(Operation):
+    def __init__(
+        self,
+        max_val,
+    ):
+        super().__init__()
+        self.max_val = max_val
+
+    def call(self, x1, x2):
+        return backend.nn.psnr(
+            x1=x1,
+            x2=x2,
+            max_val=self.max_val,
+        )
+
+    def compute_output_spec(self, x1, x2):
+        if len(x1.shape) != len(x2.shape):
+            raise ValueError("Inputs must have the same rank")
+
+        return KerasTensor(shape=())
+
+
+@keras_export(
+    [
+        "keras.ops.psnr",
+        "keras.ops.nn.psnr",
+    ]
+)
+def psnr(
+    x1,
+    x2,
+    max_val,
+):
+    """Peak Signal-to-Noise Ratio (PSNR) function.
+
+    This function computes the Peak Signal-to-Noise Ratio between two signals,
+    `x1` and `x2`. PSNR is a measure of the quality of a reconstructed signal.
+    The higher the PSNR, the closer the reconstructed signal is to the original
+    signal. Note that it can become negative when the signal power is
+    smaller that the noise power.
+
+    Args:
+        x1: The first input signal.
+        x2: The second input signal. Must have the same shape as `x1`.
+        max_val: The maximum possible value in the signals.
+
+    Returns:
+        float: The PSNR value between `x1` and `x2`.
+
+    Examples:
+
+    >>> x1 = keras.random.normal((2, 4, 4, 3))
+    >>> x2 = keras.random.normal((2, 4, 4, 3))
+    >>> max_val = 1.0
+    >>> keras.ops.nn.psnr(x1, x2, max_val)
+    -3.1697404
+    """
+    if any_symbolic_tensors(
+        (
+            x1,
+            x2,
+        )
+    ):
+        return PSNR(
+            max_val,
+        ).symbolic_call(x1, x2)
+    return backend.nn.psnr(
+        x1,
+        x2,
+        max_val,
+    )
```

### Comparing `keras-3.3.2/keras/src/ops/node.py` & `keras-3.3.3/keras/src/ops/node.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/ops/numpy.py` & `keras-3.3.3/keras/src/ops/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,151 +1,7 @@
-"""
-MANIFEST:
-
-abs
-absolute
-add
-all
-amax
-amin
-append
-arange
-arccos
-arccosh
-arcsin
-arcsinh
-arctan
-arctan2
-arctanh
-argmax
-argmin
-argsort
-array
-average
-bincount
-broadcast_to
-ceil
-clip
-concatenate
-conj
-conjugate
-copy
-correlate
-cos
-cosh
-count_nonzero
-cross
-cumprod
-cumsum
-diag
-diagonal
-diff
-digitize
-divide
-dot
-dtype
-einsum
-empty
-equal
-exp
-expand_dims
-expm1
-eye
-flip
-floor
-full
-full_like
-greater
-greater_equal
-hstack
-identity
-imag
-interp
-isclose
-isfinite
-isinf
-isnan
-less
-less_equal
-linspace
-log
-log10
-log1p
-log2
-logaddexp
-logical_and
-logical_not
-logical_or
-logspace
-matmul
-max
-maximum
-mean
-median
-meshgrid
-mgrid
-min
-minimum
-mod
-moveaxis
-multiply
-nan_to_num
-ndim
-nonzero
-not_equal
-ones
-ones_like
-outer
-pad
-percentile
-power
-prod
-quantile
-ravel
-real
-reciprocal
-repeat
-reshape
-roll
-round
-sign
-sin
-sinh
-size
-sort
-split
-sqrt
-square
-squeeze
-stack
-std
-subtract
-sum
-swapaxes
-take
-take_along_axis
-tan
-tanh
-tensordot
-tile
-trace
-transpose
-tri
-tril
-triu
-true_divide
-vdot
-vstack
-where
-zeros
-zeros_like
-
-
-"""
-
 import builtins
 import re
 
 import numpy as np
 
 from keras.src import backend
 from keras.src.api_export import keras_export
@@ -6243,15 +6099,15 @@
 
 
 class Select(Operation):
     def __init__(self):
         super().__init__()
 
     def call(self, condlist, choicelist, default=0):
-        return backend.numpy.correlate(condlist, choicelist, default)
+        return backend.numpy.select(condlist, choicelist, default)
 
     def compute_output_spec(self, condlist, choicelist, default=0):
         first_element = choicelist[0]
         return KerasTensor(first_element.shape, dtype=first_element.dtype)
 
 
 @keras_export(["keras.ops.select", "keras.ops.numpy.select"])
@@ -6299,7 +6155,39 @@
             "condlist and choicelist must not be empty. Received: "
             f"condlist = {condlist}, "
             f"choicelist = {choicelist}"
         )
     if any_symbolic_tensors(condlist + choicelist + [default]):
         return Select().symbolic_call(condlist, choicelist, default)
     return backend.numpy.select(condlist, choicelist, default)
+
+
+class Slogdet(Operation):
+    def __init__(self):
+        super().__init__()
+
+    def call(self, x):
+        return backend.numpy.slogdet(x)
+
+    def compute_output_spec(self, x):
+        sign = KerasTensor((), dtype=x.dtype)
+        logabsdet = KerasTensor((), dtype=x.dtype)
+        return (sign, logabsdet)
+
+
+@keras_export(["keras.ops.slogdet", "keras.ops.numpy.slogdet"])
+def slogdet(x):
+    """Compute the sign and natural logarithm of the determinant of a matrix.
+
+    Args:
+        x: Input matrix. It must 2D and square.
+
+    Returns:
+        A tuple `(sign, logabsdet)`. `sign` is a number representing
+        the sign of the determinant. For a real matrix, this is 1, 0, or -1.
+        For a complex matrix, this is a complex number with absolute value 1
+        (i.e., it is on the unit circle), or else 0.
+        `logabsdet` is the natural log of the absolute value of the determinant.
+    """
+    if any_symbolic_tensors((x,)):
+        return Slogdet().symbolic_call(x)
+    return backend.numpy.slogdet(x)
```

### Comparing `keras-3.3.2/keras/src/ops/operation.py` & `keras-3.3.3/keras/src/ops/operation.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/ops/operation_utils.py` & `keras-3.3.3/keras/src/ops/operation_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/ops/symbolic_arguments.py` & `keras-3.3.3/keras/src/ops/symbolic_arguments.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/optimizers/__init__.py` & `keras-3.3.3/keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/optimizers/adadelta.py` & `keras-3.3.3/keras/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/optimizers/adafactor.py` & `keras-3.3.3/keras/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/optimizers/adagrad.py` & `keras-3.3.3/keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/optimizers/adam.py` & `keras-3.3.3/keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/optimizers/adamax.py` & `keras-3.3.3/keras/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/optimizers/adamw.py` & `keras-3.3.3/keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/optimizers/base_optimizer.py` & `keras-3.3.3/keras/src/optimizers/base_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import warnings
 
 from keras.src import backend
 from keras.src import initializers
 from keras.src import ops
 from keras.src.optimizers.schedules import learning_rate_schedule
 from keras.src.saving import serialization_lib
+from keras.src.saving.keras_saveable import KerasSaveable
 from keras.src.utils import tracking
 from keras.src.utils.naming import auto_name
 
 
-class BaseOptimizer:
+class BaseOptimizer(KerasSaveable):
     def __init__(
         self,
         learning_rate,
         weight_decay=None,
         clipnorm=None,
         clipvalue=None,
         global_clipnorm=None,
@@ -810,14 +811,17 @@
         """
         if self.use_ema:
             # If the optimizer uses EMA, then when finalizing, we replace the
             # model variable value with its moving average stored inside
             # optimizer.
             self._overwrite_model_variables_with_average_value(var_list)
 
+    def _obj_type(self):
+        return "Optimizer"
+
     def get_config(self):
         """Returns the config of the optimizer.
 
         An optimizer config is a Python dictionary (serializable)
         containing the configuration of an optimizer.
         The same optimizer can be reinstantiated later
         (without any saved state) from this configuration.
```

### Comparing `keras-3.3.2/keras/src/optimizers/ftrl.py` & `keras-3.3.3/keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/optimizers/lion.py` & `keras-3.3.3/keras/src/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/optimizers/loss_scale_optimizer.py` & `keras-3.3.3/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/optimizers/nadam.py` & `keras-3.3.3/keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/optimizers/optimizer.py` & `keras-3.3.3/keras/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/optimizers/rmsprop.py` & `keras-3.3.3/keras/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/optimizers/schedules/__init__.py` & `keras-3.3.3/keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras-3.3.3/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/optimizers/sgd.py` & `keras-3.3.3/keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/quantizers/__init__.py` & `keras-3.3.3/keras/src/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/quantizers/quantizers.py` & `keras-3.3.3/keras/src/quantizers/quantizers.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/random/random.py` & `keras-3.3.3/keras/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/random/seed_generator.py` & `keras-3.3.3/keras/src/random/seed_generator.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/regularizers/__init__.py` & `keras-3.3.3/keras/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/regularizers/regularizers.py` & `keras-3.3.3/keras/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/saving/__init__.py` & `keras-3.3.3/keras/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/saving/object_registration.py` & `keras-3.3.3/keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/saving/saving_api.py` & `keras-3.3.3/keras/src/saving/saving_api.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/saving/saving_lib.py` & `keras-3.3.3/keras/src/saving/saving_lib.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,24 +37,24 @@
 
 def save_model(model, filepath, weights_format="h5"):
     """Save a zip-archive representing a Keras model to the given file or path.
 
     The zip-based archive contains the following structure:
 
     - JSON-based configuration file (config.json): Records of model, layer, and
-        other trackables' configuration.
-    - H5-based trackable state files, found in respective directories, such as
+        other saveables' configuration.
+    - H5-based saveable state files, found in respective directories, such as
         model/states.npz, model/dense_layer/states.npz, etc.
     - Metadata file.
 
-    The states of Keras trackables (layers, optimizers, loss, and metrics) are
+    The states of Keras saveables (layers, optimizers, loss, and metrics) are
     automatically saved as long as they can be discovered through the attributes
     returned by `dir(Model)`. Typically, the state includes the variables
-    associated with the trackable, but some specially purposed layers may
-    contain more such as the vocabularies stored in the hashmaps. The trackables
+    associated with the saveable, but some specially purposed layers may
+    contain more such as the vocabularies stored in the hashmaps. The saveables
     define how their states are saved by exposing `save_state()` and
     `load_state()` APIs.
 
     For the case of layer states, the variables will be visited as long as
     they are either 1) referenced via layer attributes, or 2) referenced via a
     container (list, tuple, or dict), and the container is referenced via a
     layer attribute.
@@ -125,15 +125,15 @@
         asset_store = DiskIOStore(_ASSETS_DIRNAME, archive=zf, mode="w")
 
         _save_state(
             model,
             weights_store=weights_store,
             assets_store=asset_store,
             inner_path="",
-            visited_trackables=set(),
+            visited_saveables=set(),
         )
         weights_store.close()
         asset_store.close()
 
 
 def load_model(filepath, custom_objects=None, compile=True, safe_mode=True):
     """Load a zip archive representing a Keras model."""
@@ -184,30 +184,30 @@
             )
 
         if len(all_filenames) > 3:
             asset_store = DiskIOStore(_ASSETS_DIRNAME, archive=zf, mode="r")
         else:
             asset_store = None
 
-        failed_trackables = set()
+        failed_saveables = set()
         error_msgs = {}
         _load_state(
             model,
             weights_store=weights_store,
             assets_store=asset_store,
             inner_path="",
-            visited_trackables=set(),
-            failed_trackables=failed_trackables,
+            visited_saveables=set(),
+            failed_saveables=failed_saveables,
             error_msgs=error_msgs,
         )
         weights_store.close()
         if asset_store:
             asset_store.close()
 
-        if failed_trackables:
+        if failed_saveables:
             _raise_loading_failure(error_msgs)
     return model
 
 
 def save_weights_only(model, filepath, objects_to_skip=None):
     """Save only the weights of a model to a target filepath (.weights.h5).
 
@@ -219,23 +219,23 @@
     if not filepath.endswith(".weights.h5"):
         raise ValueError(
             "Invalid `filepath` argument: expected a `.weights.h5` extension. "
             f"Received: filepath={filepath}"
         )
     weights_store = H5IOStore(filepath, mode="w")
     if objects_to_skip is not None:
-        visited_trackables = set(id(o) for o in objects_to_skip)
+        visited_saveables = set(id(o) for o in objects_to_skip)
     else:
-        visited_trackables = set()
+        visited_saveables = set()
     _save_state(
         model,
         weights_store=weights_store,
         assets_store=None,
         inner_path="",
-        visited_trackables=visited_trackables,
+        visited_saveables=visited_saveables,
     )
     weights_store.close()
 
 
 def load_weights_only(
     model, filepath, skip_mismatch=False, objects_to_skip=None
 ):
@@ -250,45 +250,45 @@
         weights_store = H5IOStore(filepath, mode="r")
     elif filepath.endswith(".keras"):
         archive = zipfile.ZipFile(filepath, "r")
         weights_store = H5IOStore(
             _VARS_FNAME + ".h5", archive=archive, mode="r"
         )
 
-    failed_trackables = set()
+    failed_saveables = set()
     if objects_to_skip is not None:
-        visited_trackables = set(id(o) for o in objects_to_skip)
+        visited_saveables = set(id(o) for o in objects_to_skip)
     else:
-        visited_trackables = set()
+        visited_saveables = set()
     error_msgs = {}
     _load_state(
         model,
         weights_store=weights_store,
         assets_store=None,
         inner_path="",
         skip_mismatch=skip_mismatch,
-        visited_trackables=visited_trackables,
-        failed_trackables=failed_trackables,
+        visited_saveables=visited_saveables,
+        failed_saveables=failed_saveables,
         error_msgs=error_msgs,
     )
     weights_store.close()
     if archive:
         archive.close()
 
-    if failed_trackables:
+    if failed_saveables:
         _raise_loading_failure(error_msgs, warn_only=skip_mismatch)
 
 
 def _raise_loading_failure(error_msgs, warn_only=False):
     first_key = list(error_msgs.keys())[0]
-    ex_trackable, ex_error = error_msgs[first_key]
+    ex_saveable, ex_error = error_msgs[first_key]
     msg = (
         f"A total of {len(error_msgs)} objects could not "
         "be loaded. Example error message for "
-        f"object {ex_trackable}:\n\n"
+        f"object {ex_saveable}:\n\n"
         f"{ex_error}\n\n"
         "List of objects that could not be loaded:\n"
         f"{[x[0] for x in error_msgs.values()]}"
     )
     if warn_only:
         warnings.warn(msg)
     else:
@@ -314,234 +314,235 @@
 def _name_key(name):
     """Make sure that private attributes are visited last."""
     if name.startswith("_"):
         return "~" + name
     return name
 
 
-def _walk_trackable(trackable):
-    from keras.src.models import Functional
-    from keras.src.models import Sequential
-
-    if isinstance(trackable, Sequential):
-        obj_type = "Sequential"
-    elif isinstance(trackable, Functional):
-        obj_type = "Functional"
-    elif isinstance(trackable, Layer):
-        obj_type = "Layer"
-    elif isinstance(trackable, Optimizer):
-        obj_type = "Optimizer"
-    elif isinstance(trackable, Metric):
-        obj_type = "Metric"
-    elif isinstance(trackable, Loss):
-        obj_type = "Loss"
-    else:
-        raise ValueError(f"Invalid obj_type: {obj_type}")
+def _walk_saveable(saveable):
+    from keras.src.saving.keras_saveable import KerasSaveable
+
+    if not isinstance(saveable, KerasSaveable):
+        raise ValueError(
+            "Expected object to be an "
+            "instance of `KerasSaveable`, but "
+            f"got {saveable} of type {type(saveable)}"
+        )
+
+    obj_type = saveable._obj_type()
     attr_skiplist = get_attr_skiplist(obj_type)
 
     # Save all layers directly tracked by Sequential and Functional first.
     # This helps avoid ordering concerns for subclassed Sequential or Functional
     # models with extra attributes--the internal Keras state take precedence.
     if obj_type in ("Sequential", "Functional"):
-        yield "layers", trackable.layers
+        yield "layers", saveable.layers
 
-    for child_attr in sorted(dir(trackable), key=lambda x: _name_key(x)):
+    for child_attr in sorted(dir(saveable), key=lambda x: _name_key(x)):
         if child_attr.startswith("__") or child_attr in attr_skiplist:
             continue
         try:
-            child_obj = getattr(trackable, child_attr)
+            child_obj = getattr(saveable, child_attr)
         except Exception:
             # Avoid raising the exception when visiting the attributes.
             continue
         yield child_attr, child_obj
 
 
 def _save_state(
-    trackable,
+    saveable,
     weights_store,
     assets_store,
     inner_path,
-    visited_trackables,
+    visited_saveables,
 ):
-    # If the trackable has already been saved, skip it.
-    if id(trackable) in visited_trackables:
+    from keras.src.saving.keras_saveable import KerasSaveable
+
+    # If the saveable has already been saved, skip it.
+    if id(saveable) in visited_saveables:
         return
 
-    if hasattr(trackable, "save_own_variables") and weights_store:
-        trackable.save_own_variables(weights_store.make(inner_path))
-    if hasattr(trackable, "save_assets") and assets_store:
-        trackable.save_assets(assets_store.make(inner_path))
-
-    visited_trackables.add(id(trackable))
-
-    # Recursively save state of children trackables (layers, optimizers, etc.)
-    for child_attr, child_obj in _walk_trackable(trackable):
-        if _is_keras_trackable(child_obj):
+    if hasattr(saveable, "save_own_variables") and weights_store:
+        saveable.save_own_variables(weights_store.make(inner_path))
+    if hasattr(saveable, "save_assets") and assets_store:
+        saveable.save_assets(assets_store.make(inner_path))
+
+    visited_saveables.add(id(saveable))
+
+    # Recursively save state of children saveables (layers, optimizers, etc.)
+    for child_attr, child_obj in _walk_saveable(saveable):
+        if isinstance(child_obj, KerasSaveable):
             _save_state(
                 child_obj,
                 weights_store,
                 assets_store,
                 inner_path=file_utils.join(inner_path, child_attr).replace(
                     "\\", "/"
                 ),
-                visited_trackables=visited_trackables,
+                visited_saveables=visited_saveables,
             )
         elif isinstance(child_obj, (list, dict, tuple, set)):
             _save_container_state(
                 child_obj,
                 weights_store,
                 assets_store,
                 inner_path=file_utils.join(inner_path, child_attr).replace(
                     "\\", "/"
                 ),
-                visited_trackables=visited_trackables,
+                visited_saveables=visited_saveables,
             )
 
 
 def _load_state(
-    trackable,
+    saveable,
     weights_store,
     assets_store,
     inner_path,
     skip_mismatch=False,
-    visited_trackables=None,
-    failed_trackables=None,
+    visited_saveables=None,
+    failed_saveables=None,
     error_msgs=None,
 ):
-    if visited_trackables and id(trackable) in visited_trackables:
+    from keras.src.saving.keras_saveable import KerasSaveable
+
+    if visited_saveables and id(saveable) in visited_saveables:
         return
 
     failure = False
 
-    if hasattr(trackable, "load_own_variables") and weights_store:
-        if skip_mismatch or failed_trackables is not None:
+    if hasattr(saveable, "load_own_variables") and weights_store:
+        if skip_mismatch or failed_saveables is not None:
             try:
-                trackable.load_own_variables(weights_store.get(inner_path))
+                saveable.load_own_variables(weights_store.get(inner_path))
             except Exception as e:
-                failed_trackables.add(id(trackable))
-                error_msgs[id(trackable)] = trackable, e
+                failed_saveables.add(id(saveable))
+                error_msgs[id(saveable)] = saveable, e
                 failure = True
         else:
-            trackable.load_own_variables(weights_store.get(inner_path))
+            saveable.load_own_variables(weights_store.get(inner_path))
 
-    if hasattr(trackable, "load_assets") and assets_store:
-        if skip_mismatch or failed_trackables is not None:
+    if hasattr(saveable, "load_assets") and assets_store:
+        if skip_mismatch or failed_saveables is not None:
             try:
-                trackable.load_assets(assets_store.get(inner_path))
+                saveable.load_assets(assets_store.get(inner_path))
             except Exception as e:
-                failed_trackables.add(id(trackable))
-                error_msgs[id(trackable)] = trackable, e
+                failed_saveables.add(id(saveable))
+                error_msgs[id(saveable)] = saveable, e
                 failure = True
         else:
-            trackable.load_assets(assets_store.get(inner_path))
+            saveable.load_assets(assets_store.get(inner_path))
 
-    if failed_trackables is not None:
-        currently_failed = len(failed_trackables)
+    if failed_saveables is not None:
+        currently_failed = len(failed_saveables)
     else:
         currently_failed = 0
 
-    # Recursively load states for Keras trackables such as layers/optimizers.
-    for child_attr, child_obj in _walk_trackable(trackable):
-        if _is_keras_trackable(child_obj):
+    # Recursively load states for Keras saveables such as layers/optimizers.
+    for child_attr, child_obj in _walk_saveable(saveable):
+        if isinstance(child_obj, KerasSaveable):
             _load_state(
                 child_obj,
                 weights_store,
                 assets_store,
                 inner_path=file_utils.join(inner_path, child_attr).replace(
                     "\\", "/"
                 ),
                 skip_mismatch=skip_mismatch,
-                visited_trackables=visited_trackables,
-                failed_trackables=failed_trackables,
+                visited_saveables=visited_saveables,
+                failed_saveables=failed_saveables,
                 error_msgs=error_msgs,
             )
         elif isinstance(child_obj, (list, dict, tuple, set)):
             _load_container_state(
                 child_obj,
                 weights_store,
                 assets_store,
                 inner_path=file_utils.join(inner_path, child_attr).replace(
                     "\\", "/"
                 ),
                 skip_mismatch=skip_mismatch,
-                visited_trackables=visited_trackables,
-                failed_trackables=failed_trackables,
+                visited_saveables=visited_saveables,
+                failed_saveables=failed_saveables,
                 error_msgs=error_msgs,
             )
 
-    if failed_trackables is not None:
-        newly_failed = len(failed_trackables) - currently_failed
+    if failed_saveables is not None:
+        newly_failed = len(failed_saveables) - currently_failed
     else:
         newly_failed = 0
 
     if not failure:
-        if visited_trackables is not None and newly_failed <= 0:
-            visited_trackables.add(id(trackable))
-        if id(trackable) in failed_trackables:
-            failed_trackables.remove(id(trackable))
-            error_msgs.pop(id(trackable))
+        if visited_saveables is not None and newly_failed <= 0:
+            visited_saveables.add(id(saveable))
+        if id(saveable) in failed_saveables:
+            failed_saveables.remove(id(saveable))
+            error_msgs.pop(id(saveable))
 
 
 def _save_container_state(
-    container, weights_store, assets_store, inner_path, visited_trackables
+    container, weights_store, assets_store, inner_path, visited_saveables
 ):
+    from keras.src.saving.keras_saveable import KerasSaveable
+
     used_names = {}
     if isinstance(container, dict):
         container = list(container.values())
 
-    for trackable in container:
-        if _is_keras_trackable(trackable):
-            # Do NOT address the trackable via `trackable.name`, since
+    for saveable in container:
+        if isinstance(saveable, KerasSaveable):
+            # Do NOT address the saveable via `saveable.name`, since
             # names are usually autogenerated and thus not reproducible
             # (i.e. they may vary across two instances of the same model).
-            name = naming.to_snake_case(trackable.__class__.__name__)
+            name = naming.to_snake_case(saveable.__class__.__name__)
             if name in used_names:
                 used_names[name] += 1
                 name = f"{name}_{used_names[name]}"
             else:
                 used_names[name] = 0
             _save_state(
-                trackable,
+                saveable,
                 weights_store,
                 assets_store,
                 inner_path=file_utils.join(inner_path, name).replace("\\", "/"),
-                visited_trackables=visited_trackables,
+                visited_saveables=visited_saveables,
             )
 
 
 def _load_container_state(
     container,
     weights_store,
     assets_store,
     inner_path,
     skip_mismatch,
-    visited_trackables,
-    failed_trackables,
+    visited_saveables,
+    failed_saveables,
     error_msgs,
 ):
+    from keras.src.saving.keras_saveable import KerasSaveable
+
     used_names = {}
     if isinstance(container, dict):
         container = list(container.values())
 
-    for trackable in container:
-        if _is_keras_trackable(trackable):
-            name = naming.to_snake_case(trackable.__class__.__name__)
+    for saveable in container:
+        if isinstance(saveable, KerasSaveable):
+            name = naming.to_snake_case(saveable.__class__.__name__)
             if name in used_names:
                 used_names[name] += 1
                 name = f"{name}_{used_names[name]}"
             else:
                 used_names[name] = 0
             _load_state(
-                trackable,
+                saveable,
                 weights_store,
                 assets_store,
                 inner_path=file_utils.join(inner_path, name).replace("\\", "/"),
                 skip_mismatch=skip_mismatch,
-                visited_trackables=visited_trackables,
-                failed_trackables=failed_trackables,
+                visited_saveables=visited_saveables,
+                failed_saveables=failed_saveables,
                 error_msgs=error_msgs,
             )
 
 
 class DiskIOStore:
     """Asset store backed by disk storage.
 
@@ -789,24 +790,18 @@
         ref_obj = Optimizer(1.0)
         skiplist += dir(ref_obj)
         skiplist.remove("variables")
     elif obj_type == "Loss":
         ref_obj = Loss()
         skiplist += dir(ref_obj)
     else:
-        raise ValueError(f"Invalid obj_type: {obj_type}")
+        raise ValueError(
+            f"get_attr_skiplist got invalid {obj_type=}. "
+            "Accepted values for `obj_type` are "
+            "['Layer', 'Functional', 'Sequential', 'Metric', "
+            "'Optimizer', 'Loss']"
+        )
+
     global_state.set_global_attribute(
         f"saving_attr_skiplist_{obj_type}", skiplist
     )
     return skiplist
-
-
-def _is_keras_trackable(obj):
-    return isinstance(
-        obj,
-        (
-            Layer,
-            Optimizer,
-            Metric,
-            Loss,
-        ),
-    )
```

### Comparing `keras-3.3.2/keras/src/saving/serialization_lib.py` & `keras-3.3.3/keras/src/saving/serialization_lib.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/testing/test_case.py` & `keras-3.3.3/keras/src/testing/test_case.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/testing/test_utils.py` & `keras-3.3.3/keras/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/trainers/compile_utils.py` & `keras-3.3.3/keras/src/trainers/compile_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     @property
     def variables(self):
         # Avoiding relying on implicit tracking since
         # CompileMetrics may be instantiated or built in a no tracking scope.
         if not self.built:
             return []
         vars = []
-        for m in self._flat_metrics + self._flat_weighted_metrics:
+        for m in self.metrics:
             if m is not None:
                 vars.extend(m.variables)
         return vars
 
     def build(self, y_true, y_pred):
         if self.output_names:
             output_names = self.output_names
```

### Comparing `keras-3.3.2/keras/src/trainers/data_adapters/__init__.py` & `keras-3.3.3/keras/src/trainers/data_adapters/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,14 +67,21 @@
         if y is not None:
             raise_unsupported_arg("y", "the targets", "PyDataset")
         if sample_weight is not None:
             raise_unsupported_arg(
                 "sample_weights", "the sample weights", "PyDataset"
             )
         return PyDatasetAdapter(x, class_weight=class_weight, shuffle=shuffle)
+        # TODO: should we warn or not?
+        # if x.num_batches is None and shuffle:
+        #     warnings.warn(
+        #         "`shuffle=True` was passed, but will be ignored since the "
+        #         "data `x` was provided as a infinite PyDataset. The "
+        #         "PyDataset is expected to already be shuffled."
+        # )
     elif is_torch_dataloader(x):
         if y is not None:
             raise_unsupported_arg("y", "the targets", "torch DataLoader")
         if sample_weight is not None:
             raise_unsupported_arg(
                 "sample_weights", "the sample weights", "torch DataLoader"
             )
```

### Comparing `keras-3.3.2/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras-3.3.3/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/trainers/data_adapters/array_slicing.py` & `keras-3.3.3/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/trainers/data_adapters/data_adapter.py` & `keras-3.3.3/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras-3.3.3/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras-3.3.3/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras-3.3.3/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import itertools
 import multiprocessing.dummy
 import queue
 import random
 import threading
 import time
 import warnings
 import weakref
@@ -149,31 +150,34 @@
             index: position of the batch in the PyDataset.
 
         Returns:
             A batch
         """
         raise NotImplementedError
 
-    def __len__(self):
-        """Number of batch in the PyDataset.
+    @property
+    def num_batches(self):
+        """Number of batches in the PyDataset.
 
         Returns:
-            The number of batches in the PyDataset.
+            The number of batches in the PyDataset or `None` to indicate that
+            the dataset is infinite.
         """
-        raise NotImplementedError
+        # For backwards compatibility, support `__len__`.
+        if hasattr(self, "__len__"):
+            return len(self)
+        raise NotImplementedError(
+            "You need to implement the `num_batches` property:\n\n"
+            "@property\ndef num_batches(self):\n  return ..."
+        )
 
     def on_epoch_end(self):
         """Method called at the end of every epoch."""
         pass
 
-    def __iter__(self):
-        """Create a generator that iterate over the PyDataset."""
-        for i in range(len(self)):
-            yield self[i]
-
 
 class PyDatasetAdapter(DataAdapter):
     """Adapter for `keras.utils.PyDataset` instances."""
 
     def __init__(
         self,
         x,
@@ -230,73 +234,83 @@
                     max_queue_size=self.py_dataset.max_queue_size,
                 )
                 return self.enqueuer.get()
 
         else:
 
             def generator_fn():
-                order = range(len(self.py_dataset))
-                if self.shuffle:
+                num_batches = self.py_dataset.num_batches
+                indices = (
+                    range(num_batches)
+                    if num_batches is not None
+                    else itertools.count()
+                )
+                if self.shuffle and num_batches is not None:
                     # Match the shuffle convention in OrderedEnqueuer.
-                    order = list(order)
-                    random.shuffle(order)
+                    indices = list(indices)
+                    random.shuffle(indices)
 
-                for i in order:
+                for i in indices:
                     yield self.py_dataset[i]
 
         return generator_fn
 
     def _get_iterator(self):
+        num_batches = self.py_dataset.num_batches
         gen_fn = self._make_multiprocessed_generator_fn()
         for i, batch in enumerate(gen_fn()):
             batch = self._standardize_batch(batch)
             yield batch
-            if i >= len(self.py_dataset) - 1 and self.enqueuer:
+            if (
+                self.enqueuer
+                and num_batches is not None
+                and i >= num_batches - 1
+            ):
                 self.enqueuer.stop()
 
     def get_numpy_iterator(self):
         return data_adapter_utils.get_numpy_iterator(self._get_iterator())
 
     def get_jax_iterator(self):
         return data_adapter_utils.get_jax_iterator(self._get_iterator())
 
     def get_tf_dataset(self):
         from keras.src.utils.module_utils import tensorflow as tf
 
+        num_batches = self.py_dataset.num_batches
         if self._output_signature is None:
-            num_samples = min(
-                data_adapter_utils.NUM_BATCHES_FOR_TENSOR_SPEC,
-                len(self.py_dataset),
-            )
+            num_samples = data_adapter_utils.NUM_BATCHES_FOR_TENSOR_SPEC
+            if num_batches is not None:
+                num_samples = min(num_samples, num_batches)
             batches = [
                 self._standardize_batch(self.py_dataset[i])
                 for i in range(num_samples)
             ]
             self._output_signature = data_adapter_utils.get_tensor_spec(batches)
 
         ds = tf.data.Dataset.from_generator(
             self._get_iterator,
             output_signature=self._output_signature,
         )
-        if self.shuffle:
+        if self.shuffle and num_batches is not None:
             ds = ds.shuffle(8)
         ds = ds.prefetch(tf.data.AUTOTUNE)
         return ds
 
     def get_torch_dataloader(self):
         return data_adapter_utils.get_torch_dataloader(self._get_iterator())
 
     def on_epoch_end(self):
         if self.enqueuer:
             self.enqueuer.stop()
         self.py_dataset.on_epoch_end()
 
     @property
     def num_batches(self):
-        return len(self.py_dataset)
+        return self.py_dataset.num_batches
 
     @property
     def batch_size(self):
         return None
 
 
 # Global variables to be shared across processes
@@ -516,53 +530,65 @@
         while True:
             time.sleep(0.1)
             if self.queue.unfinished_tasks == 0 or self.stop_signal.is_set():
                 return
 
     def _run(self):
         """Submits request to the executor and queue the `Future` objects."""
-        indices = list(range(len(self.py_dataset)))
-        if self.shuffle:
-            random.shuffle(indices)
-        self._send_py_dataset()  # Share the initial py_dataset
-        while True:
-            with closing(self.executor_fn(_SHARED_SEQUENCES)) as executor:
-                for i in indices:
+        try:
+            num_batches = self.py_dataset.num_batches
+            indices = (
+                range(num_batches)
+                if num_batches is not None
+                else itertools.count()
+            )
+            if self.shuffle and num_batches is not None:
+                indices = list(indices)
+                random.shuffle(indices)
+            self._send_py_dataset()  # Share the initial py_dataset
+            while True:
+                with closing(self.executor_fn(_SHARED_SEQUENCES)) as executor:
+                    for i in indices:
+                        if self.stop_signal.is_set():
+                            return
+
+                        self.queue.put(
+                            executor.apply_async(get_index, (self.uid, i)),
+                            block=True,
+                        )
+
+                    # Done with the current epoch, waiting for the final batches
+                    self._wait_queue()
+
                     if self.stop_signal.is_set():
+                        # We're done
                         return
 
-                    self.queue.put(
-                        executor.apply_async(get_index, (self.uid, i)),
-                        block=True,
-                    )
-
-                # Done with the current epoch, waiting for the final batches
-                self._wait_queue()
-
-                if self.stop_signal.is_set():
-                    # We're done
-                    return
-
-            # Call the internal on epoch end.
-            self.py_dataset.on_epoch_end()
-            self._send_py_dataset()  # Update the pool
+                # Call the internal on epoch end.
+                self.py_dataset.on_epoch_end()
+                self._send_py_dataset()  # Update the pool
+        except Exception as e:
+            self.queue.put(e)  # Report exception
 
     def get(self):
         """Creates a generator to extract data from the queue.
 
         Skip the data if it is `None`.
 
         Yields:
             The next element in the queue, i.e. a tuple
             `(inputs, targets)` or
             `(inputs, targets, sample_weights)`.
         """
         while self.is_running():
             try:
-                inputs = self.queue.get(block=True, timeout=5).get()
+                value = self.queue.get(block=True, timeout=5)
+                if isinstance(value, Exception):
+                    raise value  # Propagate exception from other thread
+                inputs = value.get()
                 if self.is_running():
                     self.queue.task_done()
                 if inputs is not None:
                     yield inputs
             except queue.Empty:
                 pass
             except Exception as e:
```

### Comparing `keras-3.3.2/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras-3.3.3/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras-3.3.3/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/trainers/epoch_iterator.py` & `keras-3.3.3/keras/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/trainers/trainer.py` & `keras-3.3.3/keras/src/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/tree/__init__.py` & `keras-3.3.3/keras/src/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/tree/dmtree_impl.py` & `keras-3.3.3/keras/src/tree/dmtree_impl.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/tree/optree_impl.py` & `keras-3.3.3/keras/src/tree/optree_impl.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/tree/tree_api.py` & `keras-3.3.3/keras/src/tree/tree_api.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/__init__.py` & `keras-3.3.3/keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/argument_validation.py` & `keras-3.3.3/keras/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/audio_dataset_utils.py` & `keras-3.3.3/keras/src/utils/audio_dataset_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,31 +405,48 @@
     ragged,
     shuffle=False,
     shuffle_buffer_size=None,
     seed=None,
 ):
     """Constructs a fixed-size dataset of audio and labels."""
     path_ds = tf.data.Dataset.from_tensor_slices(file_paths)
-    if shuffle:
-        path_ds = path_ds.shuffle(
-            buffer_size=shuffle_buffer_size or 1024, seed=seed
+    if label_mode:
+        label_ds = dataset_utils.labels_to_dataset(
+            labels, label_mode, num_classes
         )
+        ds = tf.data.Dataset.zip((path_ds, label_ds))
+    else:
+        ds = path_ds
 
-    audio_ds = path_ds.map(
-        lambda x: read_and_decode_audio(
-            x, sampling_rate, output_sequence_length
-        ),
-        num_parallel_calls=tf.data.AUTOTUNE,
-    )
-
-    if ragged:
-        audio_ds = audio_ds.map(
-            lambda x: tf.RaggedTensor.from_tensor(x),
+    if shuffle:
+        ds = ds.shuffle(buffer_size=shuffle_buffer_size or 1024, seed=seed)
+
+    if label_mode:
+        ds = ds.map(
+            lambda x, y: (
+                read_and_decode_audio(x, sampling_rate, output_sequence_length),
+                y,
+            ),
             num_parallel_calls=tf.data.AUTOTUNE,
         )
 
-    if label_mode:
-        label_ds = dataset_utils.labels_to_dataset(
-            labels, label_mode, num_classes
+        if ragged:
+            ds = ds.map(
+                lambda x, y: (tf.RaggedTensor.from_tensor(x), y),
+                num_parallel_calls=tf.data.AUTOTUNE,
+            )
+
+    else:
+        ds = ds.map(
+            lambda x: read_and_decode_audio(
+                x, sampling_rate, output_sequence_length
+            ),
+            num_parallel_calls=tf.data.AUTOTUNE,
         )
-        audio_ds = tf.data.Dataset.zip((audio_ds, label_ds))
-    return audio_ds
+
+        if ragged:
+            ds = ds.map(
+                lambda x: tf.RaggedTensor.from_tensor(x),
+                num_parallel_calls=tf.data.AUTOTUNE,
+            )
+
+    return ds
```

### Comparing `keras-3.3.2/keras/src/utils/backend_utils.py` & `keras-3.3.3/keras/src/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/code_stats.py` & `keras-3.3.3/keras/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/dataset_utils.py` & `keras-3.3.3/keras/src/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/dtype_utils.py` & `keras-3.3.3/keras/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/file_utils.py` & `keras-3.3.3/keras/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/image_dataset_utils.py` & `keras-3.3.3/keras/src/utils/image_dataset_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,38 +363,44 @@
     crop_to_aspect_ratio=False,
     pad_to_aspect_ratio=False,
     shuffle=False,
     shuffle_buffer_size=None,
     seed=None,
 ):
     """Constructs a dataset of images and labels."""
-    # TODO(fchollet): consider making num_parallel_calls settable
     path_ds = tf.data.Dataset.from_tensor_slices(image_paths)
-    if shuffle:
-        path_ds = path_ds.shuffle(
-            buffer_size=shuffle_buffer_size or 1024, seed=seed
+    if label_mode:
+        label_ds = dataset_utils.labels_to_dataset(
+            labels, label_mode, num_classes
         )
+        ds = tf.data.Dataset.zip((path_ds, label_ds))
+    else:
+        ds = path_ds
+
+    if shuffle:
+        ds = ds.shuffle(buffer_size=shuffle_buffer_size or 1024, seed=seed)
 
     args = (
         image_size,
         num_channels,
         interpolation,
         data_format,
         crop_to_aspect_ratio,
         pad_to_aspect_ratio,
     )
-    img_ds = path_ds.map(
-        lambda x: load_image(x, *args), num_parallel_calls=tf.data.AUTOTUNE
-    )
     if label_mode:
-        label_ds = dataset_utils.labels_to_dataset(
-            labels, label_mode, num_classes
+        ds = ds.map(
+            lambda x, y: (load_image(x, *args), y),
+            num_parallel_calls=tf.data.AUTOTUNE,
+        )
+    else:
+        ds = ds.map(
+            lambda x: load_image(x, *args), num_parallel_calls=tf.data.AUTOTUNE
         )
-        img_ds = tf.data.Dataset.zip((img_ds, label_ds))
-    return img_ds
+    return ds
 
 
 def load_image(
     path,
     image_size,
     num_channels,
     interpolation,
```

### Comparing `keras-3.3.2/keras/src/utils/image_utils.py` & `keras-3.3.3/keras/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/io_utils.py` & `keras-3.3.3/keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/jax_layer.py` & `keras-3.3.3/keras/src/utils/jax_layer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/model_visualization.py` & `keras-3.3.3/keras/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/module_utils.py` & `keras-3.3.3/keras/src/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/naming.py` & `keras-3.3.3/keras/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/numerical_utils.py` & `keras-3.3.3/keras/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/progbar.py` & `keras-3.3.3/keras/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/python_utils.py` & `keras-3.3.3/keras/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/rng_utils.py` & `keras-3.3.3/keras/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/sequence_utils.py` & `keras-3.3.3/keras/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/summary_utils.py` & `keras-3.3.3/keras/src/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/text_dataset_utils.py` & `keras-3.3.3/keras/src/utils/text_dataset_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,29 +254,36 @@
     max_length,
     shuffle=False,
     shuffle_buffer_size=None,
     seed=None,
 ):
     """Constructs a dataset of text strings and labels."""
     path_ds = tf.data.Dataset.from_tensor_slices(file_paths)
-    if shuffle:
-        path_ds = path_ds.shuffle(
-            buffer_size=shuffle_buffer_size or 1024, seed=seed
-        )
-
-    string_ds = path_ds.map(
-        lambda x: path_to_string_content(x, max_length),
-        num_parallel_calls=tf.data.AUTOTUNE,
-    )
     if label_mode:
         label_ds = dataset_utils.labels_to_dataset(
             labels, label_mode, num_classes
         )
-        string_ds = tf.data.Dataset.zip((string_ds, label_ds))
-    return string_ds
+        ds = tf.data.Dataset.zip((path_ds, label_ds))
+    else:
+        ds = path_ds
+
+    if shuffle:
+        ds = ds.shuffle(buffer_size=shuffle_buffer_size or 1024, seed=seed)
+
+    if label_mode:
+        ds = ds.map(
+            lambda x, y: (path_to_string_content(x, max_length), y),
+            num_parallel_calls=tf.data.AUTOTUNE,
+        )
+    else:
+        ds = ds.map(
+            lambda x: path_to_string_content(x, max_length),
+            num_parallel_calls=tf.data.AUTOTUNE,
+        )
+    return ds
 
 
 def path_to_string_content(path, max_length):
     txt = tf.io.read_file(path)
     if max_length is not None:
         txt = tf.strings.substr(txt, 0, max_length)
     return txt
```

### Comparing `keras-3.3.2/keras/src/utils/tf_utils.py` & `keras-3.3.3/keras/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/timeseries_dataset_utils.py` & `keras-3.3.3/keras/src/utils/timeseries_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/torch_utils.py` & `keras-3.3.3/keras/src/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/traceback_utils.py` & `keras-3.3.3/keras/src/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras/src/utils/tracking.py` & `keras-3.3.3/keras/src/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.2/keras.egg-info/PKG-INFO` & `keras-3.3.3/keras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras
-Version: 3.3.2
+Version: 3.3.3
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-3.3.2/keras.egg-info/SOURCES.txt` & `keras-3.3.3/keras.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -461,14 +461,15 @@
 keras/src/quantizers/quantizers.py
 keras/src/random/__init__.py
 keras/src/random/random.py
 keras/src/random/seed_generator.py
 keras/src/regularizers/__init__.py
 keras/src/regularizers/regularizers.py
 keras/src/saving/__init__.py
+keras/src/saving/keras_saveable.py
 keras/src/saving/object_registration.py
 keras/src/saving/saving_api.py
 keras/src/saving/saving_lib.py
 keras/src/saving/serialization_lib.py
 keras/src/testing/__init__.py
 keras/src/testing/test_case.py
 keras/src/testing/test_utils.py
```

### Comparing `keras-3.3.2/setup.py` & `keras-3.3.3/setup.py`

 * *Files identical despite different names*

