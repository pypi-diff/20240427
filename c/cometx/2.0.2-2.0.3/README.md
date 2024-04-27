# Comparing `tmp/cometx-2.0.2-py3-none-any.whl.zip` & `tmp/cometx-2.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,30 +1,31 @@
-Zip file size: 62349 bytes, number of entries: 28
+Zip file size: 63468 bytes, number of entries: 29
 -rw-rw-r--  2.0 unx      546 b- defN 24-Jan-08 19:44 cometx/__init__.py
 -rw-rw-r--  2.0 unx     1227 b- defN 23-Nov-10 01:51 cometx/_typing.py
--rw-rw-r--  2.0 unx      642 b- defN 24-Apr-22 13:43 cometx/_version.py
+-rw-rw-r--  2.0 unx      642 b- defN 24-Apr-26 14:16 cometx/_version.py
 -rw-rw-r--  2.0 unx     5468 b- defN 24-Mar-01 14:40 cometx/api.py
 -rw-rw-r--  2.0 unx    32107 b- defN 23-Nov-28 14:15 cometx/generate_utils.py
 -rw-rw-r--  2.0 unx     5065 b- defN 24-Jan-30 12:08 cometx/utils.py
 -rw-rw-r--  2.0 unx     3068 b- defN 24-Mar-13 13:53 cometx/cli/__init__.py
 -rw-rw-r--  2.0 unx     4908 b- defN 24-Mar-13 13:53 cometx/cli/config.py
--rw-rw-r--  2.0 unx    25569 b- defN 24-Apr-22 13:34 cometx/cli/copy.py
+-rw-rw-r--  2.0 unx    25931 b- defN 24-Apr-22 20:23 cometx/cli/copy.py
+-rw-rw-r--  2.0 unx     2408 b- defN 24-Apr-22 20:22 cometx/cli/copy_utils.py
 -rw-rw-r--  2.0 unx     3891 b- defN 23-Nov-29 19:06 cometx/cli/delete_assets.py
 -rw-rw-r--  2.0 unx     8496 b- defN 24-Apr-19 12:01 cometx/cli/download.py
 -rw-rw-r--  2.0 unx     2255 b- defN 24-Feb-19 13:03 cometx/cli/list_command.py
 -rw-rw-r--  2.0 unx     9772 b- defN 24-Jan-30 19:31 cometx/cli/log.py
 -rw-rw-r--  2.0 unx     4423 b- defN 24-Apr-18 14:07 cometx/cli/reproduce.py
 -rw-rw-r--  2.0 unx     6777 b- defN 24-Feb-08 14:09 cometx/cli/utils.py
 -rw-rw-r--  2.0 unx      388 b- defN 24-Jan-08 19:43 cometx/framework/__init__.py
--rw-rw-r--  2.0 unx    25497 b- defN 24-Apr-22 13:34 cometx/framework/wandb.py
+-rw-rw-r--  2.0 unx    25567 b- defN 24-Apr-26 14:14 cometx/framework/wandb.py
 -rw-rw-r--  2.0 unx      443 b- defN 24-Jan-08 19:45 cometx/framework/comet/__init__.py
 -rw-rw-r--  2.0 unx    46062 b- defN 24-Apr-21 11:45 cometx/framework/comet/download_manager.py
 -rw-rw-r--  2.0 unx      379 b- defN 23-Nov-28 14:15 cometx/tools/__init__.py
 -rw-rw-r--  2.0 unx     2473 b- defN 23-Nov-28 14:15 cometx/tools/dataset.py
 -rw-rw-r--  2.0 unx    10560 b- defN 23-Nov-28 14:15 cometx/tools/pointcloud.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Apr-22 13:44 cometx-2.0.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx    11385 b- defN 24-Apr-22 13:44 cometx-2.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-22 13:44 cometx-2.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       43 b- defN 24-Apr-22 13:44 cometx-2.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-22 13:44 cometx-2.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2231 b- defN 24-Apr-22 13:44 cometx-2.0.2.dist-info/RECORD
-28 files, 225131 bytes uncompressed, 58811 bytes compressed:  73.9%
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-26 14:17 cometx-2.0.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    11385 b- defN 24-Apr-26 14:17 cometx-2.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-26 14:17 cometx-2.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 24-Apr-26 14:17 cometx-2.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-26 14:17 cometx-2.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2312 b- defN 24-Apr-26 14:17 cometx-2.0.3.dist-info/RECORD
+29 files, 228052 bytes uncompressed, 59806 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -21,14 +21,17 @@
 
 Filename: cometx/cli/config.py
 Comment: 
 
 Filename: cometx/cli/copy.py
 Comment: 
 
+Filename: cometx/cli/copy_utils.py
+Comment: 
+
 Filename: cometx/cli/delete_assets.py
 Comment: 
 
 Filename: cometx/cli/download.py
 Comment: 
 
 Filename: cometx/cli/list_command.py
@@ -60,26 +63,26 @@
 
 Filename: cometx/tools/dataset.py
 Comment: 
 
 Filename: cometx/tools/pointcloud.py
 Comment: 
 
-Filename: cometx-2.0.2.dist-info/LICENSE
+Filename: cometx-2.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: cometx-2.0.2.dist-info/METADATA
+Filename: cometx-2.0.3.dist-info/METADATA
 Comment: 
 
-Filename: cometx-2.0.2.dist-info/WHEEL
+Filename: cometx-2.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: cometx-2.0.2.dist-info/entry_points.txt
+Filename: cometx-2.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: cometx-2.0.2.dist-info/top_level.txt
+Filename: cometx-2.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: cometx-2.0.2.dist-info/RECORD
+Filename: cometx-2.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cometx/_version.py

```diff
@@ -8,9 +8,9 @@
 #
 #  Sign up for free at http://www.comet-ml.com
 #  Copyright (C) 2015-2022 Comet ML INC
 #  This file can not be copied and/or distributed without
 #  the express permission of Comet ML Inc.
 # *******************************************************
 
-version_info = (2, 0, 2)
+version_info = (2, 0, 3)
 __version__ = ".".join(map(str, version_info))
```

## cometx/cli/copy.py

```diff
@@ -53,14 +53,15 @@
     InstalledPackagesMessage,
     MetricMessage,
     StandardOutputMessage,
     SystemDetailsMessage,
 )
 
 from ..utils import remove_extra_slashes
+from .copy_utils import upload_single_offline_experiment
 
 ADDITIONAL_ARGS = False
 
 
 def get_parser_arguments(parser):
     parser.add_argument(
         "COMET_SOURCE",
@@ -311,20 +312,30 @@
             self.copied_reports = True
 
         experiment = self.create_experiment(workspace_dst, project_dst)
         # copy experiment_folder stuff to experiment
         # copy all resources to existing or new experiment
         self.log_all(experiment, experiment_folder)
         experiment.end()
+
         print(
             f"Uploading {experiment.offline_directory}/{experiment._get_offline_archive_file_name()}"
         )
-        os.system(
-            f"comet upload {experiment.offline_directory}/{experiment._get_offline_archive_file_name()}"
+        url = upload_single_offline_experiment(
+            offline_archive_path=os.path.join(
+                experiment.offline_directory,
+                experiment._get_offline_archive_file_name(),
+            ),
+            settings=self.api.config,
+            force_upload=False,
         )
+        if url:
+            print("Experiment copied to: %s" % url)
+        else:
+            print("ERROR: this experiment failed to copy")
 
     def log_metadata(self, experiment, filename):
         if self.debug:
             with experiment.context_manager("ignore"):
                 print("log_metadata...")
         if os.path.exists(filename):
             metadata = json.load(open(filename))
```

## cometx/framework/wandb.py

```diff
@@ -638,15 +638,19 @@
             task()
         else:
             # add to queue
             self.queue.submit(task)
 
     def download_metrics(self, run):
         print("    downloading metrics...")
-        samples = run.history(pandas=False, samples=1)[0]
+        history = run.history(pandas=False, samples=1)
+        if not history:
+            return
+
+        samples = history[0]
         metrics = list(samples.keys())
         metrics_summary_path = self.get_path(run, filename="metrics_summary.jsonl")
         with open(metrics_summary_path, "w") as fp:
             for count, metric in enumerate(metrics):
                 if self.ignore_metric_name(metric):
                     continue
                 # Is it a metric?
```

## Comparing `cometx-2.0.2.dist-info/LICENSE` & `cometx-2.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cometx-2.0.2.dist-info/METADATA` & `cometx-2.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cometx
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python tools for Comet
 Home-page: https://github.com/comet-ml/comet-sdk-extensions/
 Author: cometx development team
 License: MIT License
 Keywords: ai,artificial intelligence,python,machine learning
 Platform: Linux
 Platform: Mac OS X
```

## Comparing `cometx-2.0.2.dist-info/RECORD` & `cometx-2.0.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 cometx/__init__.py,sha256=BrAXZ_G0gGubKyJ1bC41s1Bs9zKGIbsCtGFNXwosiO0,546
 cometx/_typing.py,sha256=I0YU2x7xLMclwkoobUbJHe6k2XuIufQUzawnv-GsEDo,1227
-cometx/_version.py,sha256=2VCMrUAi2IS9Neq6C5_Mm9RyMuYdiLO5yLk-NLEIxFM,642
+cometx/_version.py,sha256=mW5LuHXuCGdoImgK8mu_JNaG-OLgYEdchd7Lveat05g,642
 cometx/api.py,sha256=mjW5l-lh2gF68uM--oI6xHYXLxiOmFqgRz0nRnSiEM8,5468
 cometx/generate_utils.py,sha256=kv2SE0YZWOr3l85DJyQOmQh_YprZ_2jDBRDYPb6gLIQ,32107
 cometx/utils.py,sha256=lt9iuHu0oGr6F6_nm4351dxUMxLqpjgJIgz75Z-xQ5Y,5065
 cometx/cli/__init__.py,sha256=voafk9dNZOp6aR4P8rQubaS_pWtvJePWg_gAyO-ayuk,3068
 cometx/cli/config.py,sha256=9XDHgDr2Dz3p54rlHN6cPiPF6vOhaJJzSkDLBEMC7M4,4908
-cometx/cli/copy.py,sha256=G2fFxFjhMKlLzlfLZ9AwfAoitwFklR_GreC5YLcXwLE,25569
+cometx/cli/copy.py,sha256=PO9Vti_5jTyHVR6Utc21cPSHu5Cfb8tw4ZpTR1NNS00,25931
+cometx/cli/copy_utils.py,sha256=CJzm9MrkXtGhTxsbpbQHIeDM-K44Vgsm64XpmuNv_mE,2408
 cometx/cli/delete_assets.py,sha256=0Yn5GZYRhwAxKPVatUyzg7B5RgQRiQwi5GUn0R6lFRE,3891
 cometx/cli/download.py,sha256=1C_pR7y7ydUhi8cfbqYwXp-E13ThWfLibdDXLV_WCdM,8496
 cometx/cli/list_command.py,sha256=gstyM4nJ8LJWOdLnm_O6jK7Jctj5w3QUs0pGZVI5DU4,2255
 cometx/cli/log.py,sha256=Q8K6FFSf57zzxdpbh4GUswFkgloj9DU6NCZijgtk-0Y,9772
 cometx/cli/reproduce.py,sha256=P0D73cKi-BNB7nGFnjgDpseN2UVOqikOLB3uxqH77WI,4423
 cometx/cli/utils.py,sha256=-Cqf4yqQJ72dEATiXdq37URm_aePn-oNwrJvW_AFIgg,6777
 cometx/framework/__init__.py,sha256=EObGelztamarpe5VUuroE-z3ARPNQEeCV1GYo4KiTZg,388
-cometx/framework/wandb.py,sha256=L7CvNiDouDws1xe40-GJESSbWtqYRvjzgYT_QKveqKQ,25497
+cometx/framework/wandb.py,sha256=dhnYfVYNVkALaABSq2SEs1Dy1AlHzdhB5UvLOGW9tJY,25567
 cometx/framework/comet/__init__.py,sha256=hgl6TWV2cmvaDkfb_jZKnegOso--TCqpPRYriWahfbE,443
 cometx/framework/comet/download_manager.py,sha256=qD5Obv4cqcUzSOl0o1JpZuK2un0uJNTu-SBJYgLDfAM,46062
 cometx/tools/__init__.py,sha256=FRj-VhQ5qGHPIwMY9dZZTcBu0HiwsfdvODeZ87Vyio4,379
 cometx/tools/dataset.py,sha256=J_QS0EhDx9Q6wE39Wus4I-pXzwtHDyPbpCJAGms9nCo,2473
 cometx/tools/pointcloud.py,sha256=aO8tqmnAcdzCzFbJ8Lse6wigwAoT_dowMyzLuHGJVqk,10560
-cometx-2.0.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-cometx-2.0.2.dist-info/METADATA,sha256=kX7WswpwIBybYGa7QbVEJ7-CozDpsyf8lgi27F35SU4,11385
-cometx-2.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-cometx-2.0.2.dist-info/entry_points.txt,sha256=uC7qLDZi6lmkkyl6TNRhcL5O28A_B4aklYU-LgPUPYc,43
-cometx-2.0.2.dist-info/top_level.txt,sha256=zLvh8_4zj6N060ZSiJEPtCZhFamoROgHV8BHmg0QFqA,7
-cometx-2.0.2.dist-info/RECORD,,
+cometx-2.0.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+cometx-2.0.3.dist-info/METADATA,sha256=SZHvhse4E2XBLwSjzVTUAtsyZxnfZRAx5cQkW_vGh5I,11385
+cometx-2.0.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+cometx-2.0.3.dist-info/entry_points.txt,sha256=uC7qLDZi6lmkkyl6TNRhcL5O28A_B4aklYU-LgPUPYc,43
+cometx-2.0.3.dist-info/top_level.txt,sha256=zLvh8_4zj6N060ZSiJEPtCZhFamoROgHV8BHmg0QFqA,7
+cometx-2.0.3.dist-info/RECORD,,
```

