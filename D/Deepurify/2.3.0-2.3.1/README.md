# Comparing `tmp/Deepurify-2.3.0.tar.gz` & `tmp/Deepurify-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Deepurify-2.3.0.tar", last modified: Sat Apr 27 07:16:15 2024, max compression
+gzip compressed data, was "Deepurify-2.3.1.tar", last modified: Sat Apr 27 07:58:49 2024, max compression
```

## Comparing `Deepurify-2.3.0.tar` & `Deepurify-2.3.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 07:16:15.666612 Deepurify-2.3.0/
-drwxrwxrwx   0        0        0        0 2024-04-27 07:16:15.632703 Deepurify-2.3.0/Deepurify/
-drwxrwxrwx   0        0        0        0 2024-04-27 07:16:15.640681 Deepurify-2.3.0/Deepurify/Dataset/
--rw-rw-rw-   0        0        0    12493 2024-04-27 00:53:37.000000 Deepurify-2.3.0/Deepurify/Dataset/SequenceDataset.py
--rw-rw-rw-   0        0        0        0 2024-04-27 00:53:37.000000 Deepurify-2.3.0/Deepurify/Dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 07:16:15.649658 Deepurify-2.3.0/Deepurify/Model/
--rw-rw-rw-   0        0        0     5187 2024-04-27 00:53:37.000000 Deepurify-2.3.0/Deepurify/Model/Convolutions.py
--rw-rw-rw-   0        0        0      385 2024-04-27 00:53:37.000000 Deepurify-2.3.0/Deepurify/Model/Embedding.py
--rw-rw-rw-   0        0        0    12525 2024-04-27 00:53:37.000000 Deepurify-2.3.0/Deepurify/Model/EncoderModels.py
--rw-rw-rw-   0        0        0    10509 2024-04-27 00:53:37.000000 Deepurify-2.3.0/Deepurify/Model/FormerLayers.py
--rw-rw-rw-   0        0        0     4528 2024-04-27 00:53:37.000000 Deepurify-2.3.0/Deepurify/Model/Loss.py
--rw-rw-rw-   0        0        0        0 2024-04-27 00:53:37.000000 Deepurify-2.3.0/Deepurify/Model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 07:16:15.652649 Deepurify-2.3.0/Deepurify/Train/
--rw-rw-rw-   0        0        0     1427 2024-04-27 00:53:38.000000 Deepurify-2.3.0/Deepurify/Train/Scheduler.py
--rw-rw-rw-   0        0        0    12332 2024-04-27 00:53:38.000000 Deepurify-2.3.0/Deepurify/Train/TrainUtils.py
--rw-rw-rw-   0        0        0        0 2024-04-27 00:53:38.000000 Deepurify-2.3.0/Deepurify/Train/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 07:16:15.664618 Deepurify-2.3.0/Deepurify/Utils/
--rw-rw-rw-   0        0        0     8885 2024-04-27 00:53:38.000000 Deepurify-2.3.0/Deepurify/Utils/BuildFilesUtils.py
--rw-rw-rw-   0        0        0     3839 2024-04-27 00:53:38.000000 Deepurify-2.3.0/Deepurify/Utils/CallGenesUtils.py
--rw-rw-rw-   0        0        0    12866 2024-04-27 00:53:38.000000 Deepurify-2.3.0/Deepurify/Utils/DataUtils.py
--rw-rw-rw-   0        0        0    18246 2024-04-27 00:53:38.000000 Deepurify-2.3.0/Deepurify/Utils/FilterContamUtils.py
--rw-rw-rw-   0        0        0    11288 2024-04-27 00:53:38.000000 Deepurify-2.3.0/Deepurify/Utils/HmmUtils.py
--rw-rw-rw-   0        0        0    11900 2024-04-27 00:53:38.000000 Deepurify-2.3.0/Deepurify/Utils/IOUtils.py
--rw-rw-rw-   0        0        0     5864 2024-04-27 00:53:38.000000 Deepurify-2.3.0/Deepurify/Utils/KMeans.py
--rw-rw-rw-   0        0        0    42061 2024-04-27 00:53:38.000000 Deepurify-2.3.0/Deepurify/Utils/LabelBinsUtils.py
--rw-rw-rw-   0        0        0     7975 2024-04-27 00:53:38.000000 Deepurify-2.3.0/Deepurify/Utils/ProdigalUtils.py
--rw-rw-rw-   0        0        0    14921 2024-04-27 00:53:38.000000 Deepurify-2.3.0/Deepurify/Utils/RunCMDUtils.py
--rw-rw-rw-   0        0        0    12053 2024-04-27 00:53:38.000000 Deepurify-2.3.0/Deepurify/Utils/SelectBinsUitls.py
--rw-rw-rw-   0        0        0    18772 2024-04-27 00:53:38.000000 Deepurify-2.3.0/Deepurify/Utils/SequenceUtils.py
--rw-rw-rw-   0        0        0        0 2024-04-27 00:53:38.000000 Deepurify-2.3.0/Deepurify/Utils/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-27 00:53:39.000000 Deepurify-2.3.0/Deepurify/__init__.py
--rw-rw-rw-   0        0        0    11010 2024-04-27 00:53:37.000000 Deepurify-2.3.0/Deepurify/clean_func.py
--rw-rw-rw-   0        0        0    17501 2024-04-27 00:53:37.000000 Deepurify-2.3.0/Deepurify/cli.py
--rw-rw-rw-   0        0        0    26901 2024-04-27 00:53:37.000000 Deepurify-2.3.0/Deepurify/decontamination.py
--rw-rw-rw-   0        0        0     3221 2024-04-27 00:53:37.000000 Deepurify-2.3.0/Deepurify/integration.py
-drwxrwxrwx   0        0        0        0 2024-04-27 07:16:15.638686 Deepurify-2.3.0/Deepurify.egg-info/
--rw-rw-rw-   0        0        0      299 2024-04-27 07:16:15.000000 Deepurify-2.3.0/Deepurify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1117 2024-04-27 07:16:15.000000 Deepurify-2.3.0/Deepurify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 07:16:15.000000 Deepurify-2.3.0/Deepurify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-27 07:16:15.000000 Deepurify-2.3.0/Deepurify.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-27 07:16:15.000000 Deepurify-2.3.0/Deepurify.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2024-04-27 07:16:15.000000 Deepurify-2.3.0/Deepurify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-27 07:16:15.000000 Deepurify-2.3.0/Deepurify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2024-04-27 00:54:01.000000 Deepurify-2.3.0/LICENSE
--rw-rw-rw-   0        0        0      299 2024-04-27 07:16:15.665615 Deepurify-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     5693 2024-04-27 06:18:23.000000 Deepurify-2.3.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 07:16:15.666612 Deepurify-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0      650 2024-04-27 02:49:59.000000 Deepurify-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 07:58:49.450846 Deepurify-2.3.1/
+drwxrwxrwx   0        0        0        0 2024-04-27 07:58:49.420926 Deepurify-2.3.1/Deepurify/
+drwxrwxrwx   0        0        0        0 2024-04-27 07:58:49.428905 Deepurify-2.3.1/Deepurify/Dataset/
+-rw-rw-rw-   0        0        0    12493 2024-04-27 00:53:37.000000 Deepurify-2.3.1/Deepurify/Dataset/SequenceDataset.py
+-rw-rw-rw-   0        0        0        0 2024-04-27 00:53:37.000000 Deepurify-2.3.1/Deepurify/Dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 07:58:49.434888 Deepurify-2.3.1/Deepurify/Model/
+-rw-rw-rw-   0        0        0     5187 2024-04-27 00:53:37.000000 Deepurify-2.3.1/Deepurify/Model/Convolutions.py
+-rw-rw-rw-   0        0        0      385 2024-04-27 00:53:37.000000 Deepurify-2.3.1/Deepurify/Model/Embedding.py
+-rw-rw-rw-   0        0        0    12525 2024-04-27 00:53:37.000000 Deepurify-2.3.1/Deepurify/Model/EncoderModels.py
+-rw-rw-rw-   0        0        0    10509 2024-04-27 00:53:37.000000 Deepurify-2.3.1/Deepurify/Model/FormerLayers.py
+-rw-rw-rw-   0        0        0     4528 2024-04-27 00:53:37.000000 Deepurify-2.3.1/Deepurify/Model/Loss.py
+-rw-rw-rw-   0        0        0        0 2024-04-27 00:53:37.000000 Deepurify-2.3.1/Deepurify/Model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 07:58:49.436883 Deepurify-2.3.1/Deepurify/Train/
+-rw-rw-rw-   0        0        0     1427 2024-04-27 00:53:38.000000 Deepurify-2.3.1/Deepurify/Train/Scheduler.py
+-rw-rw-rw-   0        0        0    12332 2024-04-27 00:53:38.000000 Deepurify-2.3.1/Deepurify/Train/TrainUtils.py
+-rw-rw-rw-   0        0        0        0 2024-04-27 00:53:38.000000 Deepurify-2.3.1/Deepurify/Train/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 07:58:49.448851 Deepurify-2.3.1/Deepurify/Utils/
+-rw-rw-rw-   0        0        0     8885 2024-04-27 00:53:38.000000 Deepurify-2.3.1/Deepurify/Utils/BuildFilesUtils.py
+-rw-rw-rw-   0        0        0     3839 2024-04-27 00:53:38.000000 Deepurify-2.3.1/Deepurify/Utils/CallGenesUtils.py
+-rw-rw-rw-   0        0        0    12866 2024-04-27 00:53:38.000000 Deepurify-2.3.1/Deepurify/Utils/DataUtils.py
+-rw-rw-rw-   0        0        0    18246 2024-04-27 00:53:38.000000 Deepurify-2.3.1/Deepurify/Utils/FilterContamUtils.py
+-rw-rw-rw-   0        0        0    11288 2024-04-27 00:53:38.000000 Deepurify-2.3.1/Deepurify/Utils/HmmUtils.py
+-rw-rw-rw-   0        0        0    11900 2024-04-27 00:53:38.000000 Deepurify-2.3.1/Deepurify/Utils/IOUtils.py
+-rw-rw-rw-   0        0        0     5864 2024-04-27 00:53:38.000000 Deepurify-2.3.1/Deepurify/Utils/KMeans.py
+-rw-rw-rw-   0        0        0    42061 2024-04-27 00:53:38.000000 Deepurify-2.3.1/Deepurify/Utils/LabelBinsUtils.py
+-rw-rw-rw-   0        0        0     7975 2024-04-27 00:53:38.000000 Deepurify-2.3.1/Deepurify/Utils/ProdigalUtils.py
+-rw-rw-rw-   0        0        0    14921 2024-04-27 00:53:38.000000 Deepurify-2.3.1/Deepurify/Utils/RunCMDUtils.py
+-rw-rw-rw-   0        0        0    12053 2024-04-27 00:53:38.000000 Deepurify-2.3.1/Deepurify/Utils/SelectBinsUitls.py
+-rw-rw-rw-   0        0        0    18772 2024-04-27 00:53:38.000000 Deepurify-2.3.1/Deepurify/Utils/SequenceUtils.py
+-rw-rw-rw-   0        0        0        0 2024-04-27 00:53:38.000000 Deepurify-2.3.1/Deepurify/Utils/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-27 00:53:39.000000 Deepurify-2.3.1/Deepurify/__init__.py
+-rw-rw-rw-   0        0        0    11010 2024-04-27 00:53:37.000000 Deepurify-2.3.1/Deepurify/clean_func.py
+-rw-rw-rw-   0        0        0    17666 2024-04-27 07:54:26.000000 Deepurify-2.3.1/Deepurify/cli.py
+-rw-rw-rw-   0        0        0    26901 2024-04-27 00:53:37.000000 Deepurify-2.3.1/Deepurify/decontamination.py
+-rw-rw-rw-   0        0        0     3221 2024-04-27 00:53:37.000000 Deepurify-2.3.1/Deepurify/integration.py
+drwxrwxrwx   0        0        0        0 2024-04-27 07:58:49.427907 Deepurify-2.3.1/Deepurify.egg-info/
+-rw-rw-rw-   0        0        0      299 2024-04-27 07:58:49.000000 Deepurify-2.3.1/Deepurify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1117 2024-04-27 07:58:49.000000 Deepurify-2.3.1/Deepurify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 07:58:49.000000 Deepurify-2.3.1/Deepurify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-27 07:58:49.000000 Deepurify-2.3.1/Deepurify.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-27 07:58:49.000000 Deepurify-2.3.1/Deepurify.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2024-04-27 07:58:49.000000 Deepurify-2.3.1/Deepurify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-27 07:58:49.000000 Deepurify-2.3.1/Deepurify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2024-04-27 00:54:01.000000 Deepurify-2.3.1/LICENSE
+-rw-rw-rw-   0        0        0      299 2024-04-27 07:58:49.449849 Deepurify-2.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5725 2024-04-27 07:23:11.000000 Deepurify-2.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 07:58:49.450846 Deepurify-2.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      650 2024-04-27 07:58:34.000000 Deepurify-2.3.1/setup.py
```

### Comparing `Deepurify-2.3.0/Deepurify/Dataset/SequenceDataset.py` & `Deepurify-2.3.1/Deepurify/Dataset/SequenceDataset.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/Model/Convolutions.py` & `Deepurify-2.3.1/Deepurify/Model/Convolutions.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/Model/EncoderModels.py` & `Deepurify-2.3.1/Deepurify/Model/EncoderModels.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/Model/FormerLayers.py` & `Deepurify-2.3.1/Deepurify/Model/FormerLayers.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/Model/Loss.py` & `Deepurify-2.3.1/Deepurify/Model/Loss.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/Train/Scheduler.py` & `Deepurify-2.3.1/Deepurify/Train/Scheduler.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/Train/TrainUtils.py` & `Deepurify-2.3.1/Deepurify/Train/TrainUtils.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/Utils/BuildFilesUtils.py` & `Deepurify-2.3.1/Deepurify/Utils/BuildFilesUtils.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/Utils/CallGenesUtils.py` & `Deepurify-2.3.1/Deepurify/Utils/CallGenesUtils.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/Utils/DataUtils.py` & `Deepurify-2.3.1/Deepurify/Utils/DataUtils.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/Utils/FilterContamUtils.py` & `Deepurify-2.3.1/Deepurify/Utils/FilterContamUtils.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/Utils/HmmUtils.py` & `Deepurify-2.3.1/Deepurify/Utils/HmmUtils.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/Utils/IOUtils.py` & `Deepurify-2.3.1/Deepurify/Utils/IOUtils.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/Utils/KMeans.py` & `Deepurify-2.3.1/Deepurify/Utils/KMeans.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/Utils/LabelBinsUtils.py` & `Deepurify-2.3.1/Deepurify/Utils/LabelBinsUtils.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/Utils/ProdigalUtils.py` & `Deepurify-2.3.1/Deepurify/Utils/ProdigalUtils.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/Utils/RunCMDUtils.py` & `Deepurify-2.3.1/Deepurify/Utils/RunCMDUtils.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/Utils/SelectBinsUitls.py` & `Deepurify-2.3.1/Deepurify/Utils/SelectBinsUitls.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/Utils/SequenceUtils.py` & `Deepurify-2.3.1/Deepurify/Utils/SequenceUtils.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/clean_func.py` & `Deepurify-2.3.1/Deepurify/clean_func.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/cli.py` & `Deepurify-2.3.1/Deepurify/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,38 +177,43 @@
     )
     clean_parser.add_argument(
         "--taxo_tree_path",
         default=None,
         type=str,
         help="The path of taxonomic tree. (In database folder) Defaults to None.",
     )
-    
+
     ######################
     #### build parser ####
     ######################
-    
-    re_bin_parser = subparsers.add_parser("re-bin", help="The **Re-Bin** mode. Binning the contigs and cleaning the MAGs with applying the re-binning strategy." + \
-        " This mode can ensemble (or apply single binner) the binning results from different binners. Make sure there is no space in the contigs' names.")
+
+    re_bin_parser = subparsers.add_parser("re-bin", help="The **Re-Bin** mode. Binning the contigs and cleaning the MAGs with applying the re-binning strategy." +
+                                          " This mode can ensemble (or apply single binner) the binning results from different binners. Make sure there is no space in the contigs' names.")
     # Add parameter
     re_bin_parser.add_argument(
         "-c",
         "--contigs path",
         required=True,
         help="The contigs fasta path.")
     re_bin_parser.add_argument(
         "-s",
         "--sorted_bam_path",
         required=True,
         help="The sorted bam path.")
-    
+    re_bin_parser.add_argument(
+        "-o",
+        "--output_path",
+        required=True,
+        help="The folder used to output cleaned MAGs.")
+
     ### optional ###
     re_bin_parser.add_argument(
         "--binning_mode",
         default=None,
-        help="The semibin2, concoct, metabat2 will all be run if this parameter is None." + \
+        help="The semibin2, concoct, metabat2 will all be run if this parameter is None." +
         " The other modes are: 'semibin2', 'concoct', and 'metabat2'. Defaults to None.",
         type=str)
     re_bin_parser.add_argument(
         "--gpu_num",
         default=1,
         help="""The number of GPUs to be used can be specified. Defaults to 1.
         If you set it to 0, the code will utilize the CPU. 
@@ -321,16 +326,15 @@
     )
     re_bin_parser.add_argument(
         "--taxo_tree_path",
         default=None,
         type=str,
         help="The path of taxonomic tree. (In database folder) Defaults to None.",
     )
-    
-    
+
     ### main part ###
     args = myparser.parse_args()
     if args.command == "clean":
         s_ratio = 1. / float(args.gpu_num)
         gpu_work_ratio = [s_ratio for _ in range(int(args.gpu_num) - 1)]
         gpu_work_ratio.append(1. - sum(gpu_work_ratio))
         cleanMAGs(
@@ -385,8 +389,8 @@
         print("#################################")
         print("### RUN THE DEEPURIFY PROJECT ###")
         print("#################################")
         print()
         print("Please use 'deepurify -h' for helping.")
 
 # if __name__ == "__main__":
-#     main()
+#     main()
```

### Comparing `Deepurify-2.3.0/Deepurify/decontamination.py` & `Deepurify-2.3.1/Deepurify/decontamination.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify/integration.py` & `Deepurify-2.3.1/Deepurify/integration.py`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/Deepurify.egg-info/SOURCES.txt` & `Deepurify-2.3.1/Deepurify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/LICENSE` & `Deepurify-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Deepurify-2.3.0/README.md` & `Deepurify-2.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,21 +26,25 @@
 
 **Note**: Ensure that all the listed dependencies above are installed and functioning without any errors.
 
 
 ## Installation:
 **FIRST STEP**
 Create deepurify's conda environment by using this command:
+
 ```
 conda env create -n deepurify -f deepurify-conda-env.yml
 ```
 
 **SECOND STEP**
 Deepurify can be installed using pip. 
+
 ```
+conda activate deepurify
+
 pip install Deepurify==2.3.0
 ```
 
 
 ## Download Files and Set Environment Variable for Running
 - Download the database (required files) for running Deepurify from this **[LINK](https://drive.google.com/file/d/1FXpxoXFYHcX9QAFe7U6zfM8YjalxNLFk/view?usp=sharing)**.
```

### Comparing `Deepurify-2.3.0/setup.py` & `Deepurify-2.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 name = 'Deepurify'
 requires_list = open('./requirements.txt', 'r', encoding='utf8').readlines()
 requires_list = [i.strip() for i in requires_list]
 
 setup(
     name=name,
-    version='2.3.0',
+    version='2.3.1',
     author="Bohao Zou",
     author_email='csbhzou@comp.hkbu.edu.hk',
     description="The purification tool for improving the quality of MAGs.",
     python_requires=">=3.8",
     packages=find_packages(),
     package_data={"": ["*"]},
     include_package_data=True,
```

