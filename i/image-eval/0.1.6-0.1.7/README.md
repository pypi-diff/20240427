# Comparing `tmp/image_eval-0.1.6-py3-none-any.whl.zip` & `tmp/image_eval-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 22740 bytes, number of entries: 14
+Zip file size: 22743 bytes, number of entries: 14
 -rw-rw-r--  2.0 unx    14031 b- defN 24-Apr-27 00:35 eval.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-22 19:40 image_eval/__init__.py
 -rw-rw-r--  2.0 unx     5590 b- defN 24-Apr-27 04:24 image_eval/encoders.py
 -rw-rw-r--  2.0 unx    12627 b- defN 24-Apr-27 04:40 image_eval/evaluators.py
 -rw-rw-r--  2.0 unx     2758 b- defN 24-Apr-27 04:24 image_eval/improved_aesthetic_predictor.py
 -rw-rw-r--  2.0 unx     5152 b- defN 24-Apr-22 19:40 image_eval/local_ab_test.py
 -rw-rw-r--  2.0 unx     1176 b- defN 24-Apr-26 23:36 image_eval/model_utils.py
 -rw-rw-r--  2.0 unx     5096 b- defN 24-Apr-26 00:16 image_eval/pairwise_evaluators.py
--rw-rw-r--  2.0 unx     1066 b- defN 24-Apr-27 04:41 image_eval-0.1.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx    11870 b- defN 24-Apr-27 04:41 image_eval-0.1.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-27 04:41 image_eval-0.1.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       41 b- defN 24-Apr-27 04:41 image_eval-0.1.6.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       16 b- defN 24-Apr-27 04:41 image_eval-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1157 b- defN 24-Apr-27 04:41 image_eval-0.1.6.dist-info/RECORD
-14 files, 60672 bytes uncompressed, 20816 bytes compressed:  65.7%
+-rw-rw-r--  2.0 unx     1066 b- defN 24-Apr-27 04:42 image_eval-0.1.7.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    11870 b- defN 24-Apr-27 04:42 image_eval-0.1.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-27 04:42 image_eval-0.1.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       41 b- defN 24-Apr-27 04:42 image_eval-0.1.7.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       16 b- defN 24-Apr-27 04:42 image_eval-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1157 b- defN 24-Apr-27 04:42 image_eval-0.1.7.dist-info/RECORD
+14 files, 60672 bytes uncompressed, 20819 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: image_eval/model_utils.py
 Comment: 
 
 Filename: image_eval/pairwise_evaluators.py
 Comment: 
 
-Filename: image_eval-0.1.6.dist-info/LICENSE
+Filename: image_eval-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: image_eval-0.1.6.dist-info/METADATA
+Filename: image_eval-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: image_eval-0.1.6.dist-info/WHEEL
+Filename: image_eval-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: image_eval-0.1.6.dist-info/entry_points.txt
+Filename: image_eval-0.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: image_eval-0.1.6.dist-info/top_level.txt
+Filename: image_eval-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: image_eval-0.1.6.dist-info/RECORD
+Filename: image_eval-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `image_eval-0.1.6.dist-info/LICENSE` & `image_eval-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `image_eval-0.1.6.dist-info/METADATA` & `image_eval-0.1.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-eval
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library for evaluating image generation models
 Author: Storia AI
 Author-email: founders@storia.ai
 License: MIT License
         
         Copyright (c) 2023 Storia AI
```

## Comparing `image_eval-0.1.6.dist-info/RECORD` & `image_eval-0.1.7.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 image_eval/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 image_eval/encoders.py,sha256=8-7O1jZIBmrtee7V29ehxIURloZZQBYeRqaR_y9CxxI,5590
 image_eval/evaluators.py,sha256=YgCI3jZRc8O_dZ0509nSu6GJU5e57Vr718PzBNO-8BQ,12627
 image_eval/improved_aesthetic_predictor.py,sha256=kJFNkfxzpLR2EpDjCetLQcTlSBbYIz4nNwKJ10ZF9W4,2758
 image_eval/local_ab_test.py,sha256=oxHmPDzNQxHj7pDuB3NUEn5Hz0JTH6FeNHLFwsR-3Bg,5152
 image_eval/model_utils.py,sha256=dJEb4ogk0G6CS3wWS8lyzCtDH4f3Ke77IoEACQpK3SI,1176
 image_eval/pairwise_evaluators.py,sha256=sBWwsDD_lbW3gOTSzCz8HazvsQSyEXEUBnDDBBheY9M,5096
-image_eval-0.1.6.dist-info/LICENSE,sha256=yhXCoLY4h2EitiVksxCHxXzjkE1Nthg9GBhSAveEt2o,1066
-image_eval-0.1.6.dist-info/METADATA,sha256=J3_EChoKUC5Uax0FeLsiY6Dwl4y4-CcN1jgKb8Ms1Jg,11870
-image_eval-0.1.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-image_eval-0.1.6.dist-info/entry_points.txt,sha256=QoNCapAPdB35dsvN0O044nZnyI8sPhNa-jYRsZkE4Cw,41
-image_eval-0.1.6.dist-info/top_level.txt,sha256=zCqjk6bURpU8wHHpTmdj8CaZ9mPaIkNuUZrtal-CmEw,16
-image_eval-0.1.6.dist-info/RECORD,,
+image_eval-0.1.7.dist-info/LICENSE,sha256=yhXCoLY4h2EitiVksxCHxXzjkE1Nthg9GBhSAveEt2o,1066
+image_eval-0.1.7.dist-info/METADATA,sha256=YundBmiaVktUzKuK34BGoXV1MzQBxRNMtVPxEex6woY,11870
+image_eval-0.1.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+image_eval-0.1.7.dist-info/entry_points.txt,sha256=QoNCapAPdB35dsvN0O044nZnyI8sPhNa-jYRsZkE4Cw,41
+image_eval-0.1.7.dist-info/top_level.txt,sha256=zCqjk6bURpU8wHHpTmdj8CaZ9mPaIkNuUZrtal-CmEw,16
+image_eval-0.1.7.dist-info/RECORD,,
```

