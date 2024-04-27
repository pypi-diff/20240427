# Comparing `tmp/MODApy-0.8.0.tar.gz` & `tmp/MODApy-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MODApy-0.8.0.tar", last modified: Sun Apr 14 11:20:20 2024, max compression
+gzip compressed data, was "MODApy-0.8.1.tar", last modified: Sat Apr 27 19:14:35 2024, max compression
```

## Comparing `MODApy-0.8.0.tar` & `MODApy-0.8.1.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-14 11:20:20.060520 MODApy-0.8.0/
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    35147 2023-03-11 19:24:07.000000 MODApy-0.8.0/LICENSE
-drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-14 11:20:20.056244 MODApy-0.8.0/MODApy/
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)      297 2024-04-07 18:02:09.000000 MODApy-0.8.0/MODApy/__init__.py
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     6593 2024-04-07 18:02:09.000000 MODApy-0.8.0/MODApy/cfg.py
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    30224 2024-04-14 11:10:14.000000 MODApy-0.8.0/MODApy/cmd_line.py
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     3656 2024-04-07 18:02:09.000000 MODApy-0.8.0/MODApy/coverage.py
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     8208 2024-04-07 18:02:09.000000 MODApy-0.8.0/MODApy/downloader.py
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     7416 2024-04-07 18:02:09.000000 MODApy-0.8.0/MODApy/modaapi.py
--rw-r--r--   0 juan.vazquez   (502) staff       (20)     6342 2024-04-07 18:02:09.000000 MODApy-0.8.0/MODApy/parquetvardb.py
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    19642 2024-04-07 18:02:09.000000 MODApy-0.8.0/MODApy/pipeline.py
--rw-r--r--   0 juan.vazquez   (502) staff       (20)     1300 2024-04-03 22:26:23.000000 MODApy-0.8.0/MODApy/utils.py
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    21570 2024-04-14 11:10:14.000000 MODApy-0.8.0/MODApy/variantsdb.py
--rw-r--r--   0 juan.vazquez   (502) staff       (20)     5418 2024-04-07 18:02:09.000000 MODApy-0.8.0/MODApy/vcfanalysis.py
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    47643 2024-04-14 11:10:14.000000 MODApy-0.8.0/MODApy/vcfmgr.py
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)       22 2024-04-07 18:02:09.000000 MODApy-0.8.0/MODApy/version.py
-drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-14 11:20:20.059934 MODApy-0.8.0/MODApy/www/
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    52660 2023-03-11 19:24:07.000000 MODApy-0.8.0/MODApy/www/wespipelinebam.png
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)   113893 2023-03-11 19:24:07.000000 MODApy-0.8.0/MODApy/www/wespipelinefull.png
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    52084 2023-03-11 19:24:07.000000 MODApy-0.8.0/MODApy/www/wespipelinevcf.png
-drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-14 11:20:20.058640 MODApy-0.8.0/MODApy.egg-info/
--rw-r--r--   0 juan.vazquez   (502) staff       (20)     3354 2024-04-14 11:20:20.000000 MODApy-0.8.0/MODApy.egg-info/PKG-INFO
--rw-r--r--   0 juan.vazquez   (502) staff       (20)      560 2024-04-14 11:20:20.000000 MODApy-0.8.0/MODApy.egg-info/SOURCES.txt
--rw-r--r--   0 juan.vazquez   (502) staff       (20)        1 2024-04-14 11:20:20.000000 MODApy-0.8.0/MODApy.egg-info/dependency_links.txt
--rw-r--r--   0 juan.vazquez   (502) staff       (20)       48 2024-04-14 11:20:20.000000 MODApy-0.8.0/MODApy.egg-info/entry_points.txt
--rw-r--r--   0 juan.vazquez   (502) staff       (20)      172 2024-04-14 11:20:20.000000 MODApy-0.8.0/MODApy.egg-info/requires.txt
--rw-r--r--   0 juan.vazquez   (502) staff       (20)        7 2024-04-14 11:20:20.000000 MODApy-0.8.0/MODApy.egg-info/top_level.txt
--rw-r--r--   0 juan.vazquez   (502) staff       (20)     3354 2024-04-14 11:20:20.060330 MODApy-0.8.0/PKG-INFO
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     2640 2023-03-11 19:24:07.000000 MODApy-0.8.0/README.md
--rw-r--r--   0 juan.vazquez   (502) staff       (20)       84 2023-05-21 18:43:17.000000 MODApy-0.8.0/pyproject.toml
--rw-r--r--   0 juan.vazquez   (502) staff       (20)       38 2024-04-14 11:20:20.060577 MODApy-0.8.0/setup.cfg
--rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     2112 2023-05-14 18:54:50.000000 MODApy-0.8.0/setup.py
+drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-27 19:14:35.072023 MODApy-0.8.1/
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    35147 2023-03-11 19:24:07.000000 MODApy-0.8.1/LICENSE
+drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-27 19:14:35.060063 MODApy-0.8.1/MODApy/
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)      297 2024-04-07 18:02:09.000000 MODApy-0.8.1/MODApy/__init__.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     6593 2024-04-07 18:02:09.000000 MODApy-0.8.1/MODApy/cfg.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    30629 2024-04-27 19:13:22.000000 MODApy-0.8.1/MODApy/cmd_line.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     3656 2024-04-07 18:02:09.000000 MODApy-0.8.1/MODApy/coverage.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     8208 2024-04-07 18:02:09.000000 MODApy-0.8.1/MODApy/downloader.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     7416 2024-04-07 18:02:09.000000 MODApy-0.8.1/MODApy/modaapi.py
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)     6342 2024-04-07 18:02:09.000000 MODApy-0.8.1/MODApy/parquetvardb.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    19642 2024-04-07 18:02:09.000000 MODApy-0.8.1/MODApy/pipeline.py
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)     1300 2024-04-03 22:26:23.000000 MODApy-0.8.1/MODApy/utils.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    21570 2024-04-14 11:10:14.000000 MODApy-0.8.1/MODApy/variantsdb.py
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)     5418 2024-04-07 18:02:09.000000 MODApy-0.8.1/MODApy/vcfanalysis.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    47643 2024-04-14 11:10:14.000000 MODApy-0.8.1/MODApy/vcfmgr.py
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)       22 2024-04-27 19:13:22.000000 MODApy-0.8.1/MODApy/version.py
+drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-27 19:14:35.066869 MODApy-0.8.1/MODApy/www/
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    52660 2023-03-11 19:24:07.000000 MODApy-0.8.1/MODApy/www/wespipelinebam.png
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)   113893 2023-03-11 19:24:07.000000 MODApy-0.8.1/MODApy/www/wespipelinefull.png
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)    52084 2023-03-11 19:24:07.000000 MODApy-0.8.1/MODApy/www/wespipelinevcf.png
+drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-27 19:14:35.064370 MODApy-0.8.1/MODApy.egg-info/
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)     3354 2024-04-27 19:14:34.000000 MODApy-0.8.1/MODApy.egg-info/PKG-INFO
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)      645 2024-04-27 19:14:35.000000 MODApy-0.8.1/MODApy.egg-info/SOURCES.txt
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)        1 2024-04-27 19:14:34.000000 MODApy-0.8.1/MODApy.egg-info/dependency_links.txt
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)       48 2024-04-27 19:14:34.000000 MODApy-0.8.1/MODApy.egg-info/entry_points.txt
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)      172 2024-04-27 19:14:34.000000 MODApy-0.8.1/MODApy.egg-info/requires.txt
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)        7 2024-04-27 19:14:34.000000 MODApy-0.8.1/MODApy.egg-info/top_level.txt
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)     3354 2024-04-27 19:14:35.071750 MODApy-0.8.1/PKG-INFO
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     2640 2023-03-11 19:24:07.000000 MODApy-0.8.1/README.md
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)       84 2023-05-21 18:43:17.000000 MODApy-0.8.1/pyproject.toml
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)       38 2024-04-27 19:14:35.072119 MODApy-0.8.1/setup.cfg
+-rwxr-xr-x   0 juan.vazquez   (502) staff       (20)     2112 2023-05-14 18:54:50.000000 MODApy-0.8.1/setup.py
+drwxr-xr-x   0 juan.vazquez   (502) staff       (20)        0 2024-04-27 19:14:35.070133 MODApy-0.8.1/tests/
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)     1321 2024-04-07 18:02:09.000000 MODApy-0.8.1/tests/test_cfg.py
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)     1275 2023-05-21 18:43:17.000000 MODApy-0.8.1/tests/test_utils.py
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)     1214 2024-04-07 18:02:09.000000 MODApy-0.8.1/tests/test_vcfanalysis.py
+-rw-r--r--   0 juan.vazquez   (502) staff       (20)      479 2024-04-07 20:02:44.000000 MODApy-0.8.1/tests/test_vcfmgr.py
```

### Comparing `MODApy-0.8.0/LICENSE` & `MODApy-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.0/MODApy/cfg.py` & `MODApy-0.8.1/MODApy/cfg.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.0/MODApy/cmd_line.py` & `MODApy-0.8.1/MODApy/cmd_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -513,19 +513,26 @@
         )
         parser.add_argument(
             "-Patient",
             required=True,
             help="Patient File Path - It needs to match exactly to the one found \
               inside Patients folder",
         )
+        parser.add_argument(
+            "-annotate_patients",
+            action="store_true",
+            default=False,
+            help="Keep Temp files, otherwise just creates annotated vcf file.",
+        )
         # ignore first argument
         try:
             args = parser.parse_args(argv[2:])
             panel = configuration.panelsPath + args.Panel + ".xlsx"
             patient = configuration.patientPath + args.Patient
+            annotate_patients = args.annotate_patients
             checkFile(patient, ".vcf")
             checkFile(panel, ".xlsx")
             logger.info(
                 "Running %s on patient %s" % (str(args.Panel), str(args.Patient))
             )
             result = vcfmgr.ParsedVCF.from_vcf(patient).panel(panel)
             outpath = (
@@ -538,30 +545,33 @@
                 + ".xlsx"
             )
             os.makedirs(os.path.dirname(outpath), exist_ok=True)
             result.vcf_to_excel(outpath)
             logger.info("Annotating VARDB Freq")
             fileName = outpath.rsplit("/", maxsplit=1)[1]
             patient = pd.read_excel(outpath)
-            # columns = [
-            #    "CHROM",
-            #    "POS",
-            #    "REF",
-            #    "ALT",
-            #    "GENE_NAME",
-            #    "HGVS.C",
-            #    "HGVS.P",
-            #    "FREQ",
-            #    "ALLELE_FREQ",
-            # ]
+            if annotate_patients is False:
+                columns = [
+                    "CHROM",
+                    "POS",
+                    "REF",
+                    "ALT",
+                    "GENE_NAME",
+                    "HGVS.C",
+                    "HGVS.P",
+                    "FREQ",
+                    "ALLELE_FREQ",
+                ]
+            else:
+                columns = None
             db = variantsdb.VariantsDB.from_csvdb(
                 configuration.variantsDBPath.rsplit("/", maxsplit=1)[0],
-                #    columns=columns,
+                columns=columns,
             )
-            patient = db.annotate_excel(patient, fileName)
+            patient = db.annotate_excel(patient, fileName, annotate_patients)
             logger.info("Single Analisis Complete")
             logger.info("File available at:%s" % outpath)
         except Exception as err:
             logger.info("Single Analisis Failed")
             logger.debug(f"Error was: {err}", exc_info=True)
 
         return 0
```

### Comparing `MODApy-0.8.0/MODApy/coverage.py` & `MODApy-0.8.1/MODApy/coverage.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.0/MODApy/downloader.py` & `MODApy-0.8.1/MODApy/downloader.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.0/MODApy/modaapi.py` & `MODApy-0.8.1/MODApy/modaapi.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.0/MODApy/parquetvardb.py` & `MODApy-0.8.1/MODApy/parquetvardb.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.0/MODApy/pipeline.py` & `MODApy-0.8.1/MODApy/pipeline.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.0/MODApy/utils.py` & `MODApy-0.8.1/MODApy/utils.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.0/MODApy/variantsdb.py` & `MODApy-0.8.1/MODApy/variantsdb.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.0/MODApy/vcfanalysis.py` & `MODApy-0.8.1/MODApy/vcfanalysis.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.0/MODApy/vcfmgr.py` & `MODApy-0.8.1/MODApy/vcfmgr.py`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.0/MODApy/www/wespipelinebam.png` & `MODApy-0.8.1/MODApy/www/wespipelinebam.png`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.0/MODApy/www/wespipelinefull.png` & `MODApy-0.8.1/MODApy/www/wespipelinefull.png`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.0/MODApy/www/wespipelinevcf.png` & `MODApy-0.8.1/MODApy/www/wespipelinevcf.png`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.0/MODApy.egg-info/PKG-INFO` & `MODApy-0.8.1/MODApy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MODApy
-Version: 0.8.0
+Version: 0.8.1
 Summary: Package to perform several analysis on Multi-Omics Data
 Home-page: https://github.com/juancgvazquez/MODApy
 Author: Juan Carlos Vázquez, Elmer A. Fernández
 Author-email: juancgvazquez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `MODApy-0.8.0/MODApy.egg-info/SOURCES.txt` & `MODApy-0.8.1/MODApy.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -19,8 +19,12 @@
 MODApy.egg-info/SOURCES.txt
 MODApy.egg-info/dependency_links.txt
 MODApy.egg-info/entry_points.txt
 MODApy.egg-info/requires.txt
 MODApy.egg-info/top_level.txt
 MODApy/www/wespipelinebam.png
 MODApy/www/wespipelinefull.png
-MODApy/www/wespipelinevcf.png
+MODApy/www/wespipelinevcf.png
+tests/test_cfg.py
+tests/test_utils.py
+tests/test_vcfanalysis.py
+tests/test_vcfmgr.py
```

### Comparing `MODApy-0.8.0/PKG-INFO` & `MODApy-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MODApy
-Version: 0.8.0
+Version: 0.8.1
 Summary: Package to perform several analysis on Multi-Omics Data
 Home-page: https://github.com/juancgvazquez/MODApy
 Author: Juan Carlos Vázquez, Elmer A. Fernández
 Author-email: juancgvazquez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `MODApy-0.8.0/README.md` & `MODApy-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `MODApy-0.8.0/setup.py` & `MODApy-0.8.1/setup.py`

 * *Files identical despite different names*

