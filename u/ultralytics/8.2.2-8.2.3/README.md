# Comparing `tmp/ultralytics-8.2.2.tar.gz` & `tmp/ultralytics-8.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics-8.2.2.tar", last modified: Fri Apr 19 03:48:43 2024, max compression
+gzip compressed data, was "ultralytics-8.2.3.tar", last modified: Fri Apr 26 15:55:32 2024, max compression
```

## Comparing `ultralytics-8.2.2.tar` & `ultralytics-8.2.3.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.182316 ultralytics-8.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-19 03:47:33.000000 ultralytics-8.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    40385 2024-04-19 03:48:43.182316 ultralytics-8.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    36682 2024-04-19 03:47:33.000000 ultralytics-8.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-04-19 03:47:33.000000 ultralytics-8.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 03:48:43.182316 ultralytics-8.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.146317 ultralytics-8.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-19 03:47:33.000000 ultralytics-8.2.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-19 03:47:33.000000 ultralytics-8.2.2/tests/test_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-19 03:47:33.000000 ultralytics-8.2.2/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-19 03:47:33.000000 ultralytics-8.2.2/tests/test_explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-04-19 03:47:33.000000 ultralytics-8.2.2/tests/test_integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)    22927 2024-04-19 03:47:33.000000 ultralytics-8.2.2/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.146317 ultralytics-8.2.2/ultralytics/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.146317 ultralytics-8.2.2/ultralytics/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/assets/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.146317 ultralytics-8.2.2/ultralytics/cfg/
--rw-r--r--   0 runner    (1001) docker     (127)    21312 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.150317 ultralytics-8.2.2/ultralytics/cfg/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/DOTAv1.5.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/DOTAv1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/african-wildlife.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/brain-tumor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/carparts-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/coco-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/coco128.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/coco8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/coco8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/coco8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/crack-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/dota8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    29705 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/lvis.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/open-images-v7.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/package-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/tiger-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/xView.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.138317 ultralytics-8.2.2/ultralytics/cfg/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.150317 ultralytics-8.2.2/ultralytics/cfg/models/rt-detr/
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.150317 ultralytics-8.2.2/ultralytics/cfg/models/v3/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v3/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v3/yolov3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.150317 ultralytics-8.2.2/ultralytics/cfg/models/v5/
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v5/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v5/yolov5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.150317 ultralytics-8.2.2/ultralytics/cfg/models/v6/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v6/yolov6.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.154317 ultralytics-8.2.2/ultralytics/cfg/models/v8/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-cls.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-ghost.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-obb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-world.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-worldv2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.154317 ultralytics-8.2.2/ultralytics/cfg/models/v9/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v9/yolov9c-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v9/yolov9c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v9/yolov9e-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v9/yolov9e.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.154317 ultralytics-8.2.2/ultralytics/cfg/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/trackers/botsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/trackers/bytetrack.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.158317 ultralytics-8.2.2/ultralytics/data/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)    57741 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.158317 ultralytics-8.2.2/ultralytics/data/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/explorer/explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.158317 ultralytics-8.2.2/ultralytics/data/explorer/gui/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/explorer/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/explorer/gui/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/explorer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23142 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/split_dota.py
--rw-r--r--   0 runner    (1001) docker     (127)    30869 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.162317 ultralytics-8.2.2/ultralytics/engine/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54507 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/engine/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    40019 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/engine/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/engine/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)    30667 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/engine/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    34987 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/engine/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/engine/tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/engine/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.162317 ultralytics-8.2.2/ultralytics/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/hub/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.162317 ultralytics-8.2.2/ultralytics/models/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.162317 ultralytics-8.2.2/ultralytics/models/fastsam/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/fastsam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/fastsam/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/fastsam/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/fastsam/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/fastsam/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/fastsam/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.162317 ultralytics-8.2.2/ultralytics/models/nas/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/nas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/nas/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/nas/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/nas/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.162317 ultralytics-8.2.2/ultralytics/models/rtdetr/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/rtdetr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/rtdetr/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/rtdetr/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/rtdetr/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/rtdetr/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.166317 ultralytics-8.2.2/ultralytics/models/sam/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/amg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.166317 ultralytics-8.2.2/ultralytics/models/sam/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/modules/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/modules/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    29125 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/modules/tiny_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23614 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.166317 ultralytics-8.2.2/ultralytics/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/utils/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.166317 ultralytics-8.2.2/ultralytics/models/yolo/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.166317 ultralytics-8.2.2/ultralytics/models/yolo/classify/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.166317 ultralytics-8.2.2/ultralytics/models/yolo/detect/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/detect/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/detect/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/detect/val.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.170317 ultralytics-8.2.2/ultralytics/models/yolo/obb/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/obb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/obb/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/obb/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/obb/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.170317 ultralytics-8.2.2/ultralytics/models/yolo/pose/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/pose/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/pose/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/pose/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.170317 ultralytics-8.2.2/ultralytics/models/yolo/segment/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/segment/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.170317 ultralytics-8.2.2/ultralytics/models/yolo/world/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/world/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/world/train_world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.170317 ultralytics-8.2.2/ultralytics/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30864 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/nn/autobackend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.174317 ultralytics-8.2.2/ultralytics/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/nn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/nn/modules/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    22338 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/nn/modules/head.py
--rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/nn/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/nn/modules/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    43623 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/nn/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.174317 ultralytics-8.2.2/ultralytics/solutions/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/solutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/solutions/ai_gym.py
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/solutions/distance_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12276 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/solutions/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/solutions/object_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/solutions/queue_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/solutions/speed_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.174317 ultralytics-8.2.2/ultralytics/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/trackers/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/trackers/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    18871 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/trackers/byte_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/trackers/track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.174317 ultralytics-8.2.2/ultralytics/trackers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/trackers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/trackers/utils/gmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/trackers/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/trackers/utils/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.178316 ultralytics-8.2.2/ultralytics/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    39286 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    18539 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.178316 ultralytics-8.2.2/ultralytics/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/clearml.py
--rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/comet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/dvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/neptune.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/raytune.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/wb.py
--rw-r--r--   0 runner    (1001) docker     (127)    27971 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    32717 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    53518 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    33309 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    47332 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/tal.py
--rw-r--r--   0 runner    (1001) docker     (127)    25916 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/triton.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.178316 ultralytics-8.2.2/ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40385 2024-04-19 03:48:43.000000 ultralytics-8.2.2/ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-04-19 03:48:43.000000 ultralytics-8.2.2/ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 03:48:43.000000 ultralytics-8.2.2/ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-19 03:48:43.000000 ultralytics-8.2.2/ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-19 03:48:43.000000 ultralytics-8.2.2/ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 03:48:43.000000 ultralytics-8.2.2/ultralytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.159191 ultralytics-8.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-26 15:54:14.000000 ultralytics-8.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    40385 2024-04-26 15:55:32.155191 ultralytics-8.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    36682 2024-04-26 15:54:14.000000 ultralytics-8.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-04-26 15:54:14.000000 ultralytics-8.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:55:32.159191 ultralytics-8.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.119191 ultralytics-8.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-26 15:54:14.000000 ultralytics-8.2.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-26 15:54:14.000000 ultralytics-8.2.3/tests/test_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-26 15:54:14.000000 ultralytics-8.2.3/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-26 15:54:14.000000 ultralytics-8.2.3/tests/test_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-04-26 15:54:14.000000 ultralytics-8.2.3/tests/test_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23016 2024-04-26 15:54:14.000000 ultralytics-8.2.3/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.119191 ultralytics-8.2.3/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.119191 ultralytics-8.2.3/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.119191 ultralytics-8.2.3/ultralytics/cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)    21312 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.127191 ultralytics-8.2.3/ultralytics/cfg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/DOTAv1.5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/DOTAv1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/african-wildlife.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/brain-tumor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/carparts-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/crack-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/dota8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    29705 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/lvis.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/open-images-v7.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/package-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/tiger-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/datasets/xView.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.115191 ultralytics-8.2.3/ultralytics/cfg/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.127191 ultralytics-8.2.3/ultralytics/cfg/models/rt-detr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.127191 ultralytics-8.2.3/ultralytics/cfg/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.127191 ultralytics-8.2.3/ultralytics/cfg/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.127191 ultralytics-8.2.3/ultralytics/cfg/models/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v6/yolov6.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.131191 ultralytics-8.2.3/ultralytics/cfg/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-ghost.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-obb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-world.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-worldv2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.131191 ultralytics-8.2.3/ultralytics/cfg/models/v9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v9/yolov9c-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v9/yolov9c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v9/yolov9e-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/models/v9/yolov9e.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.131191 ultralytics-8.2.3/ultralytics/cfg/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/trackers/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/cfg/trackers/bytetrack.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.131191 ultralytics-8.2.3/ultralytics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57741 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/data/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.131191 ultralytics-8.2.3/ultralytics/data/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/data/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/data/explorer/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.135191 ultralytics-8.2.3/ultralytics/data/explorer/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/data/explorer/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/data/explorer/gui/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/data/explorer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23142 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/data/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/data/split_dota.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30869 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.135191 ultralytics-8.2.3/ultralytics/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54507 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40019 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30667 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34987 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/engine/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.135191 ultralytics-8.2.3/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.135191 ultralytics-8.2.3/ultralytics/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.135191 ultralytics-8.2.3/ultralytics/models/fastsam/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/fastsam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/fastsam/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/fastsam/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/fastsam/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/fastsam/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/fastsam/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.139191 ultralytics-8.2.3/ultralytics/models/nas/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/nas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/nas/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/nas/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/nas/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.139191 ultralytics-8.2.3/ultralytics/models/rtdetr/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/rtdetr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/rtdetr/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/rtdetr/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/rtdetr/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/rtdetr/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.139191 ultralytics-8.2.3/ultralytics/models/sam/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.139191 ultralytics-8.2.3/ultralytics/models/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29125 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/sam/modules/tiny_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23614 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.139191 ultralytics-8.2.3/ultralytics/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/utils/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.139191 ultralytics-8.2.3/ultralytics/models/yolo/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.143191 ultralytics-8.2.3/ultralytics/models/yolo/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.143191 ultralytics-8.2.3/ultralytics/models/yolo/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/detect/val.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.143191 ultralytics-8.2.3/ultralytics/models/yolo/obb/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/obb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/obb/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/obb/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/obb/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.143191 ultralytics-8.2.3/ultralytics/models/yolo/pose/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.143191 ultralytics-8.2.3/ultralytics/models/yolo/segment/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.143191 ultralytics-8.2.3/ultralytics/models/yolo/world/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/world/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/models/yolo/world/train_world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.143191 ultralytics-8.2.3/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30864 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/nn/autobackend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.147191 ultralytics-8.2.3/ultralytics/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/nn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/nn/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22338 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/nn/modules/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/nn/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/nn/modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43623 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.147191 ultralytics-8.2.3/ultralytics/solutions/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/solutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/solutions/ai_gym.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/solutions/distance_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12276 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/solutions/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/solutions/object_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/solutions/queue_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/solutions/speed_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.147191 ultralytics-8.2.3/ultralytics/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18871 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/trackers/byte_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/trackers/track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.147191 ultralytics-8.2.3/ultralytics/trackers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/trackers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/trackers/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/trackers/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/trackers/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.151191 ultralytics-8.2.3/ultralytics/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    39286 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23470 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.155191 ultralytics-8.2.3/ultralytics/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/callbacks/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27971 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32717 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53518 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33309 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47332 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25916 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/triton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-26 15:54:14.000000 ultralytics-8.2.3/ultralytics/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:55:32.155191 ultralytics-8.2.3/ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40385 2024-04-26 15:55:32.000000 ultralytics-8.2.3/ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-04-26 15:55:32.000000 ultralytics-8.2.3/ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:55:32.000000 ultralytics-8.2.3/ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-26 15:55:32.000000 ultralytics-8.2.3/ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-26 15:55:32.000000 ultralytics-8.2.3/ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 15:55:32.000000 ultralytics-8.2.3/ultralytics.egg-info/top_level.txt
```

### Comparing `ultralytics-8.2.2/LICENSE` & `ultralytics-8.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/PKG-INFO` & `ultralytics-8.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.2.2
+Version: 8.2.3
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Author: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/ultralytics/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.2.2 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.2.3 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Author: Glenn Jocher, Ayush
 Chaurasia, Jing Qiu Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics/ Keywords: machine-
 learning,deep-learning,computer-
```

### Comparing `ultralytics-8.2.2/README.md` & `ultralytics-8.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/pyproject.toml` & `ultralytics-8.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/tests/test_cli.py` & `ultralytics-8.2.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/tests/test_cuda.py` & `ultralytics-8.2.3/tests/test_cuda.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/tests/test_engine.py` & `ultralytics-8.2.3/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/tests/test_explorer.py` & `ultralytics-8.2.3/tests/test_explorer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/tests/test_integrations.py` & `ultralytics-8.2.3/tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/tests/test_python.py` & `ultralytics-8.2.3/tests/test_python.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,15 @@
 @pytest.mark.skipif(not TORCH_1_13, reason="OpenVINO requires torch>=1.13")
 def test_export_openvino():
     """Test exporting the YOLO model to OpenVINO format."""
     f = YOLO(MODEL).export(format="openvino")
     YOLO(f)(SOURCE)  # exported model inference
 
 
+@pytest.mark.skipif(not TORCH_1_9, reason="CoreML>=7.2 not supported with PyTorch<=1.8")
 @pytest.mark.skipif(WINDOWS, reason="CoreML not supported on Windows")  # RuntimeError: BlobWriter not loaded
 @pytest.mark.skipif(IS_RASPBERRYPI, reason="CoreML not supported on Raspberry Pi")
 @pytest.mark.skipif(checks.IS_PYTHON_3_12, reason="CoreML not supported in Python 3.12")
 def test_export_coreml():
     """Test exporting the YOLO model to CoreML format."""
     if MACOS:
         f = YOLO(MODEL).export(format="coreml")
```

### Comparing `ultralytics-8.2.2/ultralytics/__init__.py` & `ultralytics-8.2.3/ultralytics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
-__version__ = "8.2.2"
+__version__ = "8.2.3"
 
 from ultralytics.data.explorer.explorer import Explorer
 from ultralytics.models import RTDETR, SAM, YOLO, YOLOWorld
 from ultralytics.models.fastsam import FastSAM
 from ultralytics.models.nas import NAS
 from ultralytics.utils import ASSETS, SETTINGS
 from ultralytics.utils.checks import check_yolo as checks
```

### Comparing `ultralytics-8.2.2/ultralytics/assets/bus.jpg` & `ultralytics-8.2.3/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/assets/zidane.jpg` & `ultralytics-8.2.3/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/__init__.py` & `ultralytics-8.2.3/ultralytics/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/Argoverse.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/DOTAv1.5.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/DOTAv1.5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/DOTAv1.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/DOTAv1.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/GlobalWheat2020.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/ImageNet.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/Objects365.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/SKU-110K.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/VOC.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/VisDrone.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/african-wildlife.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/african-wildlife.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/brain-tumor.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/brain-tumor.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/carparts-seg.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/carparts-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/coco-pose.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/coco.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/coco128-seg.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/coco128.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/coco8-pose.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/coco8-seg.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/coco8.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/crack-seg.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/crack-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/dota8.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/dota8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/lvis.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/lvis.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/open-images-v7.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/open-images-v7.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/package-seg.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/package-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/tiger-pose.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/tiger-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/datasets/xView.yaml` & `ultralytics-8.2.3/ultralytics/cfg/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/default.yaml` & `ultralytics-8.2.3/ultralytics/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v3/yolov3-spp.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v3/yolov3-tiny.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v3/yolov3.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v5/yolov5-p6.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v5/yolov5.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v6/yolov6.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v6/yolov6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-cls.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-ghost.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-ghost.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-obb.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-obb.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-p2.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-p6.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-pose.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-seg.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-world.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-world.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-worldv2.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8-worldv2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v9/yolov9c-seg.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v9/yolov9c-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v9/yolov9c.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v9/yolov9c.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v9/yolov9e-seg.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v9/yolov9e-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/models/v9/yolov9e.yaml` & `ultralytics-8.2.3/ultralytics/cfg/models/v9/yolov9e.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/trackers/botsort.yaml` & `ultralytics-8.2.3/ultralytics/cfg/trackers/botsort.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/cfg/trackers/bytetrack.yaml` & `ultralytics-8.2.3/ultralytics/cfg/trackers/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/data/__init__.py` & `ultralytics-8.2.3/ultralytics/data/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/data/annotator.py` & `ultralytics-8.2.3/ultralytics/data/annotator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/data/augment.py` & `ultralytics-8.2.3/ultralytics/data/augment.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/data/base.py` & `ultralytics-8.2.3/ultralytics/data/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/data/build.py` & `ultralytics-8.2.3/ultralytics/data/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/data/converter.py` & `ultralytics-8.2.3/ultralytics/data/converter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/data/dataset.py` & `ultralytics-8.2.3/ultralytics/data/dataset.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/data/explorer/explorer.py` & `ultralytics-8.2.3/ultralytics/data/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/data/explorer/gui/dash.py` & `ultralytics-8.2.3/ultralytics/data/explorer/gui/dash.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/data/explorer/utils.py` & `ultralytics-8.2.3/ultralytics/data/explorer/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/data/loaders.py` & `ultralytics-8.2.3/ultralytics/data/loaders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/data/split_dota.py` & `ultralytics-8.2.3/ultralytics/data/split_dota.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/data/utils.py` & `ultralytics-8.2.3/ultralytics/data/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/engine/exporter.py` & `ultralytics-8.2.3/ultralytics/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/engine/model.py` & `ultralytics-8.2.3/ultralytics/engine/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/engine/predictor.py` & `ultralytics-8.2.3/ultralytics/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/engine/results.py` & `ultralytics-8.2.3/ultralytics/engine/results.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/engine/trainer.py` & `ultralytics-8.2.3/ultralytics/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/engine/tuner.py` & `ultralytics-8.2.3/ultralytics/engine/tuner.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/engine/validator.py` & `ultralytics-8.2.3/ultralytics/engine/validator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/hub/__init__.py` & `ultralytics-8.2.3/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/hub/auth.py` & `ultralytics-8.2.3/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/hub/session.py` & `ultralytics-8.2.3/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/hub/utils.py` & `ultralytics-8.2.3/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/fastsam/model.py` & `ultralytics-8.2.3/ultralytics/models/fastsam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/fastsam/predict.py` & `ultralytics-8.2.3/ultralytics/models/fastsam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/fastsam/prompt.py` & `ultralytics-8.2.3/ultralytics/models/fastsam/prompt.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/fastsam/utils.py` & `ultralytics-8.2.3/ultralytics/models/fastsam/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/fastsam/val.py` & `ultralytics-8.2.3/ultralytics/models/fastsam/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/nas/model.py` & `ultralytics-8.2.3/ultralytics/models/nas/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/nas/predict.py` & `ultralytics-8.2.3/ultralytics/models/nas/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/nas/val.py` & `ultralytics-8.2.3/ultralytics/models/nas/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/rtdetr/model.py` & `ultralytics-8.2.3/ultralytics/models/rtdetr/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/rtdetr/predict.py` & `ultralytics-8.2.3/ultralytics/models/rtdetr/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/rtdetr/train.py` & `ultralytics-8.2.3/ultralytics/models/rtdetr/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/rtdetr/val.py` & `ultralytics-8.2.3/ultralytics/models/rtdetr/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/sam/amg.py` & `ultralytics-8.2.3/ultralytics/models/sam/amg.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/sam/build.py` & `ultralytics-8.2.3/ultralytics/models/sam/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/sam/model.py` & `ultralytics-8.2.3/ultralytics/models/sam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/sam/modules/decoders.py` & `ultralytics-8.2.3/ultralytics/models/sam/modules/decoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/sam/modules/encoders.py` & `ultralytics-8.2.3/ultralytics/models/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/sam/modules/sam.py` & `ultralytics-8.2.3/ultralytics/models/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/sam/modules/tiny_encoder.py` & `ultralytics-8.2.3/ultralytics/models/sam/modules/tiny_encoder.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/sam/modules/transformer.py` & `ultralytics-8.2.3/ultralytics/models/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/sam/predict.py` & `ultralytics-8.2.3/ultralytics/models/sam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/utils/loss.py` & `ultralytics-8.2.3/ultralytics/models/utils/loss.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/utils/ops.py` & `ultralytics-8.2.3/ultralytics/models/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/yolo/classify/predict.py` & `ultralytics-8.2.3/ultralytics/models/yolo/classify/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/yolo/classify/train.py` & `ultralytics-8.2.3/ultralytics/models/yolo/classify/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/yolo/classify/val.py` & `ultralytics-8.2.3/ultralytics/models/yolo/classify/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/yolo/detect/predict.py` & `ultralytics-8.2.3/ultralytics/models/yolo/detect/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/yolo/detect/train.py` & `ultralytics-8.2.3/ultralytics/models/yolo/detect/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/yolo/detect/val.py` & `ultralytics-8.2.3/ultralytics/models/yolo/detect/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/yolo/model.py` & `ultralytics-8.2.3/ultralytics/models/yolo/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/yolo/obb/predict.py` & `ultralytics-8.2.3/ultralytics/models/yolo/obb/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/yolo/obb/train.py` & `ultralytics-8.2.3/ultralytics/models/yolo/obb/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/yolo/obb/val.py` & `ultralytics-8.2.3/ultralytics/models/yolo/obb/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/yolo/pose/predict.py` & `ultralytics-8.2.3/ultralytics/models/yolo/pose/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/yolo/pose/train.py` & `ultralytics-8.2.3/ultralytics/models/yolo/pose/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/yolo/pose/val.py` & `ultralytics-8.2.3/ultralytics/models/yolo/pose/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/yolo/segment/predict.py` & `ultralytics-8.2.3/ultralytics/models/yolo/segment/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/yolo/segment/train.py` & `ultralytics-8.2.3/ultralytics/models/yolo/segment/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/yolo/segment/val.py` & `ultralytics-8.2.3/ultralytics/models/yolo/segment/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/yolo/world/train.py` & `ultralytics-8.2.3/ultralytics/models/yolo/world/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/models/yolo/world/train_world.py` & `ultralytics-8.2.3/ultralytics/models/yolo/world/train_world.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/nn/__init__.py` & `ultralytics-8.2.3/ultralytics/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/nn/autobackend.py` & `ultralytics-8.2.3/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/nn/modules/__init__.py` & `ultralytics-8.2.3/ultralytics/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/nn/modules/block.py` & `ultralytics-8.2.3/ultralytics/nn/modules/block.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/nn/modules/conv.py` & `ultralytics-8.2.3/ultralytics/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/nn/modules/head.py` & `ultralytics-8.2.3/ultralytics/nn/modules/head.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/nn/modules/transformer.py` & `ultralytics-8.2.3/ultralytics/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/nn/modules/utils.py` & `ultralytics-8.2.3/ultralytics/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/nn/tasks.py` & `ultralytics-8.2.3/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/solutions/ai_gym.py` & `ultralytics-8.2.3/ultralytics/solutions/ai_gym.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/solutions/distance_calculation.py` & `ultralytics-8.2.3/ultralytics/solutions/distance_calculation.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/solutions/heatmap.py` & `ultralytics-8.2.3/ultralytics/solutions/heatmap.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/solutions/object_counter.py` & `ultralytics-8.2.3/ultralytics/solutions/object_counter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/solutions/queue_management.py` & `ultralytics-8.2.3/ultralytics/solutions/queue_management.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/solutions/speed_estimation.py` & `ultralytics-8.2.3/ultralytics/solutions/speed_estimation.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/trackers/basetrack.py` & `ultralytics-8.2.3/ultralytics/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/trackers/bot_sort.py` & `ultralytics-8.2.3/ultralytics/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/trackers/byte_tracker.py` & `ultralytics-8.2.3/ultralytics/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/trackers/track.py` & `ultralytics-8.2.3/ultralytics/trackers/track.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/trackers/utils/gmc.py` & `ultralytics-8.2.3/ultralytics/trackers/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/trackers/utils/kalman_filter.py` & `ultralytics-8.2.3/ultralytics/trackers/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/trackers/utils/matching.py` & `ultralytics-8.2.3/ultralytics/trackers/utils/matching.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/__init__.py` & `ultralytics-8.2.3/ultralytics/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/autobatch.py` & `ultralytics-8.2.3/ultralytics/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/benchmarks.py` & `ultralytics-8.2.3/ultralytics/utils/benchmarks.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,26 +21,31 @@
 TensorFlow Edge TPU     | `edgetpu`                 | yolov8n_edgetpu.tflite
 TensorFlow.js           | `tfjs`                    | yolov8n_web_model/
 PaddlePaddle            | `paddle`                  | yolov8n_paddle_model/
 NCNN                    | `ncnn`                    | yolov8n_ncnn_model/
 """
 
 import glob
+import os
 import platform
+import re
+import shutil
 import time
 from pathlib import Path
 
 import numpy as np
 import torch.cuda
+import yaml
 
 from ultralytics import YOLO, YOLOWorld
 from ultralytics.cfg import TASK2DATA, TASK2METRIC
 from ultralytics.engine.exporter import export_formats
 from ultralytics.utils import ARM64, ASSETS, IS_JETSON, IS_RASPBERRYPI, LINUX, LOGGER, MACOS, TQDM, WEIGHTS_DIR
 from ultralytics.utils.checks import IS_PYTHON_3_12, check_requirements, check_yolo
+from ultralytics.utils.downloads import safe_download
 from ultralytics.utils.files import file_size
 from ultralytics.utils.torch_utils import select_device
 
 
 def benchmark(
     model=WEIGHTS_DIR / "yolov8n.pt", data=None, imgsz=160, half=False, int8=False, device="cpu", verbose=False
 ):
@@ -148,14 +153,141 @@
         metrics = df[key].array  # values to compare to floor
         floor = verbose  # minimum metric floor to pass, i.e. = 0.29 mAP for YOLOv5n
         assert all(x > floor for x in metrics if pd.notna(x)), f"Benchmark failure: metric(s) < floor {floor}"
 
     return df
 
 
+class RF100Benchmark:
+    def __init__(self):
+        """Function for initialization of RF100Benchmark."""
+        self.ds_names = []
+        self.ds_cfg_list = []
+        self.rf = None
+        self.val_metrics = ["class", "images", "targets", "precision", "recall", "map50", "map95"]
+
+    def set_key(self, api_key):
+        """
+        Set Roboflow API key for processing.
+
+        Args:
+            api_key (str): The API key.
+        """
+
+        check_requirements("roboflow")
+        from roboflow import Roboflow
+
+        self.rf = Roboflow(api_key=api_key)
+
+    def parse_dataset(self, ds_link_txt="datasets_links.txt"):
+        """
+        Parse dataset links and downloads datasets.
+
+        Args:
+            ds_link_txt (str): Path to dataset_links file.
+        """
+
+        (shutil.rmtree("rf-100"), os.mkdir("rf-100")) if os.path.exists("rf-100") else os.mkdir("rf-100")
+        os.chdir("rf-100")
+        os.mkdir("ultralytics-benchmarks")
+        safe_download("https://ultralytics.com/assets/datasets_links.txt")
+
+        with open(ds_link_txt, "r") as file:
+            for line in file:
+                try:
+                    _, url, workspace, project, version = re.split("/+", line.strip())
+                    self.ds_names.append(project)
+                    proj_version = f"{project}-{version}"
+                    if not Path(proj_version).exists():
+                        self.rf.workspace(workspace).project(project).version(version).download("yolov8")
+                    else:
+                        print("Dataset already downloaded.")
+                    self.ds_cfg_list.append(Path.cwd() / proj_version / "data.yaml")
+                except Exception:
+                    continue
+
+        return self.ds_names, self.ds_cfg_list
+
+    def fix_yaml(self, path):
+        """
+        Function to fix yaml train and val path.
+
+        Args:
+            path (str): YAML file path.
+        """
+
+        with open(path, "r") as file:
+            yaml_data = yaml.safe_load(file)
+        yaml_data["train"] = "train/images"
+        yaml_data["val"] = "valid/images"
+        with open(path, "w") as file:
+            yaml.safe_dump(yaml_data, file)
+
+    def evaluate(self, yaml_path, val_log_file, eval_log_file, list_ind):
+        """
+        Model evaluation on validation results.
+
+        Args:
+            yaml_path (str): YAML file path.
+            val_log_file (str): val_log_file path.
+            eval_log_file (str): eval_log_file path.
+            list_ind (int): Index for current dataset.
+        """
+        skip_symbols = ["🚀", "⚠️", "💡", "❌"]
+        with open(yaml_path) as stream:
+            class_names = yaml.safe_load(stream)["names"]
+        with open(val_log_file, "r", encoding="utf-8") as f:
+            lines = f.readlines()
+            eval_lines = []
+            for line in lines:
+                if any(symbol in line for symbol in skip_symbols):
+                    continue
+                entries = line.split(" ")
+                entries = list(filter(lambda val: val != "", entries))
+                entries = [e.strip("\n") for e in entries]
+                start_class = False
+                for e in entries:
+                    if e == "all":
+                        if "(AP)" not in entries:
+                            if "(AR)" not in entries:
+                                # parse all
+                                eval = {}
+                                eval["class"] = entries[0]
+                                eval["images"] = entries[1]
+                                eval["targets"] = entries[2]
+                                eval["precision"] = entries[3]
+                                eval["recall"] = entries[4]
+                                eval["map50"] = entries[5]
+                                eval["map95"] = entries[6]
+                                eval_lines.append(eval)
+
+                    if e in class_names:
+                        eval = {}
+                        eval["class"] = entries[0]
+                        eval["images"] = entries[1]
+                        eval["targets"] = entries[2]
+                        eval["precision"] = entries[3]
+                        eval["recall"] = entries[4]
+                        eval["map50"] = entries[5]
+                        eval["map95"] = entries[6]
+                        eval_lines.append(eval)
+        map_val = 0.0
+        if len(eval_lines) > 1:
+            print("There's more dicts")
+            for lst in eval_lines:
+                if lst["class"] == "all":
+                    map_val = lst["map50"]
+        else:
+            print("There's only one dict res")
+            map_val = [res["map50"] for res in eval_lines][0]
+
+        with open(eval_log_file, "a") as f:
+            f.write(f"{self.ds_names[list_ind]}: {map_val}\n")
+
+
 class ProfileModels:
     """
     ProfileModels class for profiling different models on ONNX and TensorRT.
 
     This class profiles the performance of different models, returning results such as model speed and FLOPs.
 
     Attributes:
```

### Comparing `ultralytics-8.2.2/ultralytics/utils/callbacks/base.py` & `ultralytics-8.2.3/ultralytics/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/callbacks/clearml.py` & `ultralytics-8.2.3/ultralytics/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/callbacks/comet.py` & `ultralytics-8.2.3/ultralytics/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/callbacks/dvc.py` & `ultralytics-8.2.3/ultralytics/utils/callbacks/dvc.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/callbacks/hub.py` & `ultralytics-8.2.3/ultralytics/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/callbacks/mlflow.py` & `ultralytics-8.2.3/ultralytics/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/callbacks/neptune.py` & `ultralytics-8.2.3/ultralytics/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/callbacks/raytune.py` & `ultralytics-8.2.3/ultralytics/utils/callbacks/raytune.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/callbacks/tensorboard.py` & `ultralytics-8.2.3/ultralytics/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/callbacks/wb.py` & `ultralytics-8.2.3/ultralytics/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/checks.py` & `ultralytics-8.2.3/ultralytics/utils/checks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/dist.py` & `ultralytics-8.2.3/ultralytics/utils/dist.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/downloads.py` & `ultralytics-8.2.3/ultralytics/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/errors.py` & `ultralytics-8.2.3/ultralytics/utils/errors.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/files.py` & `ultralytics-8.2.3/ultralytics/utils/files.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/instance.py` & `ultralytics-8.2.3/ultralytics/utils/instance.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/loss.py` & `ultralytics-8.2.3/ultralytics/utils/loss.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/metrics.py` & `ultralytics-8.2.3/ultralytics/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/ops.py` & `ultralytics-8.2.3/ultralytics/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/patches.py` & `ultralytics-8.2.3/ultralytics/utils/patches.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/plotting.py` & `ultralytics-8.2.3/ultralytics/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/tal.py` & `ultralytics-8.2.3/ultralytics/utils/tal.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/torch_utils.py` & `ultralytics-8.2.3/ultralytics/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/triton.py` & `ultralytics-8.2.3/ultralytics/utils/triton.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics/utils/tuner.py` & `ultralytics-8.2.3/ultralytics/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics.egg-info/PKG-INFO` & `ultralytics-8.2.3/ultralytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.2.2
+Version: 8.2.3
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Author: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/ultralytics/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.2.2 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.2.3 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Author: Glenn Jocher, Ayush
 Chaurasia, Jing Qiu Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics/ Keywords: machine-
 learning,deep-learning,computer-
```

### Comparing `ultralytics-8.2.2/ultralytics.egg-info/SOURCES.txt` & `ultralytics-8.2.3/ultralytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.2/ultralytics.egg-info/requires.txt` & `ultralytics-8.2.3/ultralytics.egg-info/requires.txt`

 * *Files identical despite different names*

