# Comparing `tmp/easypaddleocr-0.1.3.tar.gz` & `tmp/easypaddleocr-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easypaddleocr-0.1.3.tar", last modified: Fri Jan  5 06:23:54 2024, max compression
+gzip compressed data, was "easypaddleocr-0.1.4.tar", last modified: Sat Apr 27 14:40:03 2024, max compression
```

## Comparing `easypaddleocr-0.1.3.tar` & `easypaddleocr-0.1.4.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:54.792123 easypaddleocr-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    34519 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-01-05 06:23:54.792123 easypaddleocr-0.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:54.776122 easypaddleocr-0.1.3/easypaddleocr/
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/infer_cls_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/infer_det_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/infer_rec_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/infer_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/tools_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:54.776122 easypaddleocr-0.1.3/easypaddleocr/torchocr/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:54.776122 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/collate_fn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:54.780122 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/ColorJitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15584 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/abinet_aug.py
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/copy_paste.py
--rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/ct_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    28635 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/drrg_targets.py
--rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/east_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    20193 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/fce_aug.py
--rw-r--r--   0 runner    (1001) docker     (127)    25842 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/fce_targets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/iaa_augment.py
--rw-r--r--   0 runner    (1001) docker     (127)    44263 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/label_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/make_border_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/make_pse_gt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/make_shrink_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    40691 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/pg_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/randaugment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/random_crop_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    26725 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/rec_img_aug.py
--rw-r--r--   0 runner    (1001) docker     (127)    28698 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/sast_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/ssl_img_aug.py
--rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/table_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:54.780122 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/text_image_aug/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/text_image_aug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/text_image_aug/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/text_image_aug/warp_mls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/multi_scale_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/pgnet_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/pubtab_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/data/simple_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:54.780122 easypaddleocr-0.1.3/easypaddleocr/torchocr/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/engine/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:54.784122 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:54.784122 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/architectures/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/architectures/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/architectures/distillation_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:54.784122 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/det_mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/det_resnet_vd.py
--rw-r--r--   0 runner    (1001) docker     (127)    10073 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/rec_hgnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14753 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/rec_lcnetv3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/rec_mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/rec_mv1_enhance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/rec_nrtr_mtb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/rec_resnet_31.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/rec_resnet_vd.py
--rw-r--r--   0 runner    (1001) docker     (127)    19956 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/rec_svtrnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:54.788123 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/heads/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/heads/cls_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/heads/det_db_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/heads/multiheadAttention.py
--rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/heads/rec_att_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/heads/rec_ctc_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/heads/rec_multi_head.py
--rw-r--r--   0 runner    (1001) docker     (127)    25935 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/heads/rec_nrtr_head.py
--rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/heads/rec_sar_head.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:54.788123 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/necks/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/necks/db_fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/necks/intracl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/necks/rnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:54.788123 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9151 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/transforms/tps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:54.788123 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/cls_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/ct_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/db_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    10821 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/drrg_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/east_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/fce_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/locality_aware_nms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/pg_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/picodet_postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:54.788123 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/pse_postprocess/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/pse_postprocess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:54.788123 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/pse_postprocess/pse/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/pse_postprocess/pse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/pse_postprocess/pse/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/pse_postprocess/pse_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    37952 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/rec_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    13048 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/sast_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/table_postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:54.792123 easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/ckpt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:54.792123 easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/e2e_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/e2e_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/e2e_utils/extract_batchsize.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/e2e_utils/extract_textpoint_fast.py
--rw-r--r--   0 runner    (1001) docker     (127)    21466 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/e2e_utils/extract_textpoint_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/e2e_utils/pgnet_pp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/e2e_utils/visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/gen_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/poly_nms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/easypaddleocr/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 06:23:54.792123 easypaddleocr-0.1.3/easypaddleocr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-01-05 06:23:54.000000 easypaddleocr-0.1.3/easypaddleocr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-01-05 06:23:54.000000 easypaddleocr-0.1.3/easypaddleocr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 06:23:54.000000 easypaddleocr-0.1.3/easypaddleocr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-01-05 06:23:54.000000 easypaddleocr-0.1.3/easypaddleocr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-05 06:23:54.000000 easypaddleocr-0.1.3/easypaddleocr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-01-05 06:23:41.000000 easypaddleocr-0.1.3/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-05 06:23:54.792123 easypaddleocr-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:40:03.777261 easypaddleocr-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    34519 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-27 14:40:03.777261 easypaddleocr-0.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:40:03.757261 easypaddleocr-0.1.4/easypaddleocr/
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/infer_cls_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/infer_det_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/infer_rec_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/infer_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/tools_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:40:03.761261 easypaddleocr-0.1.4/easypaddleocr/torchocr/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:40:03.761261 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/collate_fn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:40:03.765261 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/ColorJitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15584 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/abinet_aug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/copy_paste.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/ct_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28635 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/drrg_targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/east_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20193 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/fce_aug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25842 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/fce_targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/iaa_augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44263 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/label_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/make_border_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/make_pse_gt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/make_shrink_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40691 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/pg_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/randaugment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/random_crop_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26725 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/rec_img_aug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28698 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/sast_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/ssl_img_aug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/table_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:40:03.765261 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/text_image_aug/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/text_image_aug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/text_image_aug/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/text_image_aug/warp_mls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/multi_scale_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/pgnet_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/pubtab_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/data/simple_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:40:03.765261 easypaddleocr-0.1.4/easypaddleocr/torchocr/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/engine/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:40:03.765261 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:40:03.765261 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/architectures/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/architectures/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/architectures/distillation_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:40:03.769261 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/det_mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/det_resnet_vd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10073 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/rec_hgnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14753 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/rec_lcnetv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/rec_mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/rec_mv1_enhance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/rec_nrtr_mtb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/rec_resnet_31.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/rec_resnet_vd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19956 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/rec_svtrnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:40:03.769261 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/heads/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/heads/cls_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/heads/det_db_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/heads/multiheadAttention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/heads/rec_att_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/heads/rec_ctc_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/heads/rec_multi_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25935 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/heads/rec_nrtr_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/heads/rec_sar_head.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:40:03.769261 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/necks/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/necks/db_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/necks/intracl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/necks/rnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:40:03.769261 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9151 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/transforms/tps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:40:03.773261 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/cls_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/ct_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/db_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10821 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/drrg_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/east_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/fce_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/locality_aware_nms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/pg_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/picodet_postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:40:03.773261 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/pse_postprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/pse_postprocess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:40:03.773261 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/pse_postprocess/pse/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/pse_postprocess/pse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/pse_postprocess/pse/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/pse_postprocess/pse_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37952 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/rec_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13048 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/sast_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/table_postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:40:03.773261 easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/ckpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:40:03.777261 easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/e2e_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/e2e_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/e2e_utils/extract_batchsize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/e2e_utils/extract_textpoint_fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21466 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/e2e_utils/extract_textpoint_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/e2e_utils/pgnet_pp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/e2e_utils/visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/gen_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/poly_nms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/easypaddleocr/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:40:03.777261 easypaddleocr-0.1.4/easypaddleocr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-27 14:40:03.000000 easypaddleocr-0.1.4/easypaddleocr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-27 14:40:03.000000 easypaddleocr-0.1.4/easypaddleocr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 14:40:03.000000 easypaddleocr-0.1.4/easypaddleocr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-27 14:40:03.000000 easypaddleocr-0.1.4/easypaddleocr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-27 14:40:03.000000 easypaddleocr-0.1.4/easypaddleocr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-27 14:39:59.000000 easypaddleocr-0.1.4/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 14:40:03.777261 easypaddleocr-0.1.4/setup.cfg
```

### Comparing `easypaddleocr-0.1.3/LICENCE` & `easypaddleocr-0.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/PKG-INFO` & `easypaddleocr-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easypaddleocr
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple, optional tool for PaddleOCR Detection, direction classification and recognition on CPU and GPU using torch.
 Author: pk5ls20, hv0905
 Project-URL: Code, https://github.com/pk5ls20/EasyPaddleOCR
 Project-URL: Documentation, https://github.com/pk5ls20/EasyPaddleOCR
 Project-URL: Download, https://pypi.org/project/easypaddleocr
 Project-URL: Homepage, https://github.com/pk5ls20/EasyPaddleOCR
 Project-URL: Issues, https://github.com/pk5ls20/EasyPaddleOCR/issues
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: shapely
 Requires-Dist: scikit-image
 Requires-Dist: imgaug
 Requires-Dist: pyclipper
 Requires-Dist: numpy
-Requires-Dist: opencv-python
+Requires-Dist: opencv-python-headless
 Requires-Dist: Pillow
 Requires-Dist: pyyaml
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: loguru
 Requires-Dist: huggingface_hub
 
@@ -35,12 +35,14 @@
 
 easyPaddleOCR = EasyPaddleOCR(use_angle_cls=True, needWarmUp=True)
 image_path = 'your-picture-filepath'
 image_ndarray = np.array(cv2.imread(image_path))
 result = easyPaddleOCR.ocr(image_ndarray)
 print(result)
 ```
-
 ## Reference
 - https://github.com/WenmuZhou/PytorchOCR
 - https://github.com/PaddlePaddle/PaddleOCR
 - https://github.com/frotms/PaddleOCR2Pytorch
+
+## Additional Notes:
+**This repository was originally the Fork of https://github.com/WenmuZhou/PytorchOCR**
```

### Comparing `easypaddleocr-0.1.3/easypaddleocr/__init__.py` & `easypaddleocr-0.1.4/easypaddleocr/__init__.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/infer_cls_class.py` & `easypaddleocr-0.1.4/easypaddleocr/infer_cls_class.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/infer_det_class.py` & `easypaddleocr-0.1.4/easypaddleocr/infer_det_class.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/infer_rec_class.py` & `easypaddleocr-0.1.4/easypaddleocr/infer_rec_class.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/infer_system.py` & `easypaddleocr-0.1.4/easypaddleocr/infer_system.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/tools_utility.py` & `easypaddleocr-0.1.4/easypaddleocr/tools_utility.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/__init__.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/collate_fn.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/collate_fn.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/__init__.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/__init__.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/abinet_aug.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/abinet_aug.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/copy_paste.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/copy_paste.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/ct_process.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/ct_process.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/drrg_targets.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/drrg_targets.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/east_process.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/east_process.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/fce_aug.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/fce_aug.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/fce_targets.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/fce_targets.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/iaa_augment.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/iaa_augment.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/label_ops.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/label_ops.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/make_border_map.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/make_border_map.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/make_pse_gt.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/make_pse_gt.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/make_shrink_map.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/make_shrink_map.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/operators.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/operators.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/pg_process.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/pg_process.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/randaugment.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/randaugment.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/random_crop_data.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/random_crop_data.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/rec_img_aug.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/rec_img_aug.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/sast_process.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/sast_process.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/ssl_img_aug.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/ssl_img_aug.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/table_ops.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/table_ops.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/text_image_aug/augment.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/text_image_aug/augment.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/imaug/text_image_aug/warp_mls.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/imaug/text_image_aug/warp_mls.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/multi_scale_sampler.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/multi_scale_sampler.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/pgnet_dataset.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/pgnet_dataset.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/pubtab_dataset.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/pubtab_dataset.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/data/simple_dataset.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/data/simple_dataset.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/engine/config.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/engine/config.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/architectures/base_model.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/architectures/base_model.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/architectures/distillation_model.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/architectures/distillation_model.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/__init__.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/det_mobilenet_v3.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/det_mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/det_resnet_vd.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/det_resnet_vd.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/rec_hgnet.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/rec_hgnet.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/rec_lcnetv3.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/rec_lcnetv3.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/rec_mobilenet_v3.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/rec_mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/rec_mv1_enhance.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/rec_mv1_enhance.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/rec_nrtr_mtb.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/rec_nrtr_mtb.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/rec_resnet_31.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/rec_resnet_31.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/rec_resnet_vd.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/rec_resnet_vd.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/backbones/rec_svtrnet.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/backbones/rec_svtrnet.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/common.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/common.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/heads/__init__.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/heads/__init__.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/heads/cls_head.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/heads/cls_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/heads/det_db_head.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/heads/det_db_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/heads/multiheadAttention.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/heads/multiheadAttention.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/heads/rec_att_head.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/heads/rec_att_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/heads/rec_ctc_head.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/heads/rec_ctc_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/heads/rec_multi_head.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/heads/rec_multi_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/heads/rec_nrtr_head.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/heads/rec_nrtr_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/heads/rec_sar_head.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/heads/rec_sar_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/necks/db_fpn.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/necks/db_fpn.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/necks/intracl.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/necks/intracl.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/necks/rnn.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/necks/rnn.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/modeling/transforms/tps.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/modeling/transforms/tps.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/__init__.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/cls_postprocess.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/cls_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/ct_postprocess.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/ct_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/db_postprocess.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/db_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/drrg_postprocess.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/drrg_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/east_postprocess.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/east_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/fce_postprocess.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/fce_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/locality_aware_nms.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/locality_aware_nms.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/pg_postprocess.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/pg_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/picodet_postprocess.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/picodet_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/pse_postprocess/pse/__init__.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/pse_postprocess/pse/__init__.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/pse_postprocess/pse_postprocess.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/pse_postprocess/pse_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/rec_postprocess.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/rec_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/sast_postprocess.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/sast_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/postprocess/table_postprocess.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/postprocess/table_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/ckpt.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/ckpt.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/e2e_utils/extract_batchsize.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/e2e_utils/extract_batchsize.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/e2e_utils/extract_textpoint_fast.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/e2e_utils/extract_textpoint_fast.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/e2e_utils/extract_textpoint_slow.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/e2e_utils/extract_textpoint_slow.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/e2e_utils/pgnet_pp_utils.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/e2e_utils/pgnet_pp_utils.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/e2e_utils/visual.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/e2e_utils/visual.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/gen_label.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/gen_label.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/logging.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/logging.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/poly_nms.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/poly_nms.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/stats.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/stats.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/utility.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/utility.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/torchocr/utils/visual.py` & `easypaddleocr-0.1.4/easypaddleocr/torchocr/utils/visual.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr/utility.py` & `easypaddleocr-0.1.4/easypaddleocr/utility.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/easypaddleocr.egg-info/PKG-INFO` & `easypaddleocr-0.1.4/easypaddleocr.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easypaddleocr
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple, optional tool for PaddleOCR Detection, direction classification and recognition on CPU and GPU using torch.
 Author: pk5ls20, hv0905
 Project-URL: Code, https://github.com/pk5ls20/EasyPaddleOCR
 Project-URL: Documentation, https://github.com/pk5ls20/EasyPaddleOCR
 Project-URL: Download, https://pypi.org/project/easypaddleocr
 Project-URL: Homepage, https://github.com/pk5ls20/EasyPaddleOCR
 Project-URL: Issues, https://github.com/pk5ls20/EasyPaddleOCR/issues
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: shapely
 Requires-Dist: scikit-image
 Requires-Dist: imgaug
 Requires-Dist: pyclipper
 Requires-Dist: numpy
-Requires-Dist: opencv-python
+Requires-Dist: opencv-python-headless
 Requires-Dist: Pillow
 Requires-Dist: pyyaml
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: loguru
 Requires-Dist: huggingface_hub
 
@@ -35,12 +35,14 @@
 
 easyPaddleOCR = EasyPaddleOCR(use_angle_cls=True, needWarmUp=True)
 image_path = 'your-picture-filepath'
 image_ndarray = np.array(cv2.imread(image_path))
 result = easyPaddleOCR.ocr(image_ndarray)
 print(result)
 ```
-
 ## Reference
 - https://github.com/WenmuZhou/PytorchOCR
 - https://github.com/PaddlePaddle/PaddleOCR
 - https://github.com/frotms/PaddleOCR2Pytorch
+
+## Additional Notes:
+**This repository was originally the Fork of https://github.com/WenmuZhou/PytorchOCR**
```

### Comparing `easypaddleocr-0.1.3/easypaddleocr.egg-info/SOURCES.txt` & `easypaddleocr-0.1.4/easypaddleocr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.1.3/pyproject.toml` & `easypaddleocr-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "easypaddleocr"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     { name = "pk5ls20" },
     { name = "hv0905" }
 ]
 description = "A simple, optional tool for PaddleOCR Detection, direction classification and recognition on CPU and GPU using torch."
 readme = "readme.md"
 license = { file="LICENSE" }
@@ -16,18 +16,18 @@
 urls = {Code = "https://github.com/pk5ls20/EasyPaddleOCR", Documentation = "https://github.com/pk5ls20/EasyPaddleOCR", Download = "https://pypi.org/project/easypaddleocr", Homepage = "https://github.com/pk5ls20/EasyPaddleOCR", Issues = "https://github.com/pk5ls20/EasyPaddleOCR/issues"}
 dependencies = [
     "shapely",
     "scikit-image",
     "imgaug",
     "pyclipper",
     "numpy",
-    "opencv-python",
+    "opencv-python-headless",
     "Pillow",
     "pyyaml",
     "torch",
     "torchvision",
     "loguru",
     "huggingface_hub"
 ]
 
 [tool.setuptools.packages.find]
-exclude = ["test_images"]
+exclude = ["test"]
```

