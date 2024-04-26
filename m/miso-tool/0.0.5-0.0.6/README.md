# Comparing `tmp/miso_tool-0.0.5.tar.gz` & `tmp/miso_tool-0.0.6.tar.gz`

## Comparing `miso_tool-0.0.5.tar` & `miso_tool-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 miso_tool-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 miso_tool-0.0.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 miso_tool-0.0.5/.github/workflows/pypi_deploy.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miso_tool-0.0.5/src/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 miso_tool-0.0.5/src/miso_tool/__about__.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 miso_tool-0.0.5/src/miso_tool/__init__.py
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 miso_tool-0.0.5/src/miso_tool/cleaning.py
--rw-r--r--   0        0        0     5466 2020-02-02 00:00:00.000000 miso_tool-0.0.5/src/miso_tool/cli.py
--rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 miso_tool-0.0.5/src/miso_tool/illumina.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 miso_tool-0.0.5/src/miso_tool/io.py
--rw-r--r--   0        0        0    10202 2020-02-02 00:00:00.000000 miso_tool-0.0.5/src/miso_tool/main.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 miso_tool-0.0.5/src/miso_tool/nanopore.py
--rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 miso_tool-0.0.5/src/miso_tool/samples.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 miso_tool-0.0.5/src/miso_tool/seqruns.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 miso_tool-0.0.5/src/miso_tool/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miso_tool-0.0.5/src/miso_tool/barcodes/__init__.py
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 miso_tool-0.0.5/src/miso_tool/barcodes/nanopore.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miso_tool-0.0.5/src/miso_tool/const/__init__.py
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 miso_tool-0.0.5/src/miso_tool/const/nanopore.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miso_tool-0.0.5/src/miso_tool/const/organisms.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 miso_tool-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 miso_tool-0.0.5/tests/test_cleaning.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 miso_tool-0.0.5/.gitignore
--rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 miso_tool-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0    10365 2020-02-02 00:00:00.000000 miso_tool-0.0.5/README.md
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 miso_tool-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 miso_tool-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 miso_tool-0.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 miso_tool-0.0.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 miso_tool-0.0.6/.github/workflows/pypi_deploy.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miso_tool-0.0.6/src/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 miso_tool-0.0.6/src/miso_tool/__about__.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 miso_tool-0.0.6/src/miso_tool/__init__.py
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 miso_tool-0.0.6/src/miso_tool/cleaning.py
+-rw-r--r--   0        0        0     5466 2020-02-02 00:00:00.000000 miso_tool-0.0.6/src/miso_tool/cli.py
+-rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 miso_tool-0.0.6/src/miso_tool/illumina.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 miso_tool-0.0.6/src/miso_tool/io.py
+-rw-r--r--   0        0        0    10202 2020-02-02 00:00:00.000000 miso_tool-0.0.6/src/miso_tool/main.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 miso_tool-0.0.6/src/miso_tool/nanopore.py
+-rw-r--r--   0        0        0     8060 2020-02-02 00:00:00.000000 miso_tool-0.0.6/src/miso_tool/samples.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 miso_tool-0.0.6/src/miso_tool/seqruns.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 miso_tool-0.0.6/src/miso_tool/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miso_tool-0.0.6/src/miso_tool/barcodes/__init__.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 miso_tool-0.0.6/src/miso_tool/barcodes/nanopore.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miso_tool-0.0.6/src/miso_tool/const/__init__.py
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 miso_tool-0.0.6/src/miso_tool/const/nanopore.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miso_tool-0.0.6/src/miso_tool/const/organisms.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 miso_tool-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 miso_tool-0.0.6/tests/test_cleaning.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 miso_tool-0.0.6/.gitignore
+-rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 miso_tool-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0    10365 2020-02-02 00:00:00.000000 miso_tool-0.0.6/README.md
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 miso_tool-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 miso_tool-0.0.6/PKG-INFO
```

### Comparing `miso_tool-0.0.5/CHANGELOG.md` & `miso_tool-0.0.6/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # miso-tool changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.0.6](https://github.com/CFIA-NCFAD/miso-tool/releases/tag/0.0.6) - 2024-04-26
+
+Add support for Nanopore native barcoding kit SQK-NBD114-96.
+
 ## [0.0.5](https://github.com/CFIA-NCFAD/miso-tool/releases/tag/0.0.5) - 2023-12-
 
 Illumina MiSeq with MiSeq Control Software v4.0.0 outputs FASTQ files to a different destination. This version of miso-tool adds support for this new destination.
 
 ## [0.0.4](https://github.com/CFIA-NCFAD/miso-tool/releases/tag/0.0.4) - 2023-12-18
 
 Added support for SQK-RBK114-96, which has the same barcode sequences as SQK-RBK110-96.
```

### Comparing `miso_tool-0.0.5/.github/workflows/ci.yml` & `miso_tool-0.0.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `miso_tool-0.0.5/.github/workflows/pypi_deploy.yml` & `miso_tool-0.0.6/.github/workflows/pypi_deploy.yml`

 * *Files identical despite different names*

### Comparing `miso_tool-0.0.5/src/miso_tool/cleaning.py` & `miso_tool-0.0.6/src/miso_tool/cleaning.py`

 * *Files identical despite different names*

### Comparing `miso_tool-0.0.5/src/miso_tool/cli.py` & `miso_tool-0.0.6/src/miso_tool/cli.py`

 * *Files identical despite different names*

### Comparing `miso_tool-0.0.5/src/miso_tool/illumina.py` & `miso_tool-0.0.6/src/miso_tool/illumina.py`

 * *Files identical despite different names*

### Comparing `miso_tool-0.0.5/src/miso_tool/io.py` & `miso_tool-0.0.6/src/miso_tool/io.py`

 * *Files identical despite different names*

### Comparing `miso_tool-0.0.5/src/miso_tool/main.py` & `miso_tool-0.0.6/src/miso_tool/main.py`

 * *Files identical despite different names*

### Comparing `miso_tool-0.0.5/src/miso_tool/samples.py` & `miso_tool-0.0.6/src/miso_tool/samples.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional, Tuple
 
-from miso_tool.nanopore import get_rbk11096_barcode
+from miso_tool.nanopore import get_nbd11496_barcode, get_rbk11096_barcode
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class SamplesRunsInfo:
     id_to_sample: dict[str, dict]
@@ -207,11 +207,17 @@
                 seqkit = run.get("sequencingKit", None)
                 if seqkit is not None and seqkit in ("SQK-RBK110-96", "SQK-RBK114-96"):
                     barcode = get_rbk11096_barcode(barcode)
                     if barcode is None:
                         error_msg = f"Could not find RBK110-96/RBK114-96 barcode for {sampleid} in run {run['name']}"
                         raise ValueError(error_msg)
                     return barcode, None
+                elif seqkit is not None and seqkit in ("SQK-NBD114-96",):
+                    barcode = get_nbd11496_barcode(barcode)
+                    if barcode is None:
+                        error_msg = f"Could not find NBD114-96 barcode for {sampleid} in run {run['name']}"
+                        raise ValueError(error_msg)
+                    return barcode, None
                 else:
                     return barcode, barcode_two
     error_msg = f"Could not find sample {sampleid} in run {run['name']}"
     raise ValueError(error_msg)
```

### Comparing `miso_tool-0.0.5/src/miso_tool/seqruns.py` & `miso_tool-0.0.6/src/miso_tool/seqruns.py`

 * *Files identical despite different names*

### Comparing `miso_tool-0.0.5/src/miso_tool/barcodes/nanopore.py` & `miso_tool-0.0.6/src/miso_tool/const/nanopore.py`

 * *Files identical despite different names*

### Comparing `miso_tool-0.0.5/src/miso_tool/const/nanopore.py` & `miso_tool-0.0.6/src/miso_tool/barcodes/nanopore.py`

 * *Files 22% similar despite different names*

```diff
@@ -92,7 +92,106 @@
     "GGCTCCATAGGAACTCACGCTACT": "barcode91",
     "TTGTGAGTGGAAAGATACAGGACC": "barcode92",
     "AGTTTCCATCACTTCAGACTTGGG": "barcode93",
     "GATTGTCCTCAAACTGCCACCTAC": "barcode94",
     "CCTGTCTGGAAGAAGAATGGACTT": "barcode95",
     "CTGAACGGTCATAGAGTCCACCAT": "barcode96",
 }
+
+nbd114_96 = {
+    "CACAAAGACACCGACAACTTTCTT": "barcode01",
+    "ACAGACGACTACAAACGGAATCGA": "barcode02",
+    "CCTGGTAACTGGGACACAAGACTC": "barcode03",
+    "TAGGGAAACACGATAGAATCCGAA": "barcode04",
+    "AAGGTTACACAAACCCTGGACAAG": "barcode05",
+    "GACTACTTTCTGCCTTTGCGAGAA": "barcode06",
+    "AAGGATTCATTCCCACGGTAACAC": "barcode07",
+    "ACGTAACTTGGTTTGTTCCCTGAA": "barcode08",
+    "AACCAAGACTCGCTGTGCCTAGTT": "barcode09",
+    "GAGAGGACAAAGGTTTCAACGCTT": "barcode10",
+    "TCCATTCCCTCCGATAGATGAAAC": "barcode11",
+    "TCCGATTCTGCTTCTTTCTACCTG": "barcode12",
+    "AGAACGACTTCCATACTCGTGTGA": "barcode13",
+    "AACGAGTCTCTTGGGACCCATAGA": "barcode14",
+    "AGGTCTACCTCGCTAACACCACTG": "barcode15",
+    "CGTCAACTGACAGTGGTTCGTACT": "barcode16",
+    "ACCCTCCAGGAAAGTACCTCTGAT": "barcode17",
+    "CCAAACCCAACAACCTAGATAGGC": "barcode18",
+    "GTTCCTCGTGCAGTGTCAAGAGAT": "barcode19",
+    "TTGCGTCCTGTTACGAGAACTCAT": "barcode20",
+    "GAGCCTCTCATTGTCCGTTCTCTA": "barcode21",
+    "ACCACTGCCATGTATCAAAGTACG": "barcode22",
+    "CTTACTACCCAGTGAACCTCCTCG": "barcode23",
+    "GCATAGTTCTGCATGATGGGTTAG": "barcode24",
+    "GTAAGTTGGGTATGCAACGCAATG": "barcode25",
+    "CATACAGCGACTACGCATTCTCAT": "barcode26",
+    "CGACGGTTAGATTCACCTCTTACA": "barcode27",
+    "TGAAACCTAAGAAGGCACCGTATC": "barcode28",
+    "CTAGACACCTTGGGTTGACAGACC": "barcode29",
+    "TCAGTGAGGATCTACTTCGACCCA": "barcode30",
+    "TGCGTACAGCAATCAGTTACATTG": "barcode31",
+    "CCAGTAGAAGTCCGACAACGTCAT": "barcode32",
+    "CAGACTTGGTACGGTTGGGTAACT": "barcode33",
+    "GGACGAAGAACTCAAGTCAAAGGC": "barcode34",
+    "CTACTTACGAAGCTGAGGGACTGC": "barcode35",
+    "ATGTCCCAGTTAGAGGAGGAAACA": "barcode36",
+    "GCTTGCGATTGATGCTTAGTATCA": "barcode37",
+    "ACCACAGGAGGACGATACAGAGAA": "barcode38",
+    "CCACAGTGTCAACTAGAGCCTCTC": "barcode39",
+    "TAGTTTGGATGACCAAGGATAGCC": "barcode40",
+    "GGAGTTCGTCCAGAGAAGTACACG": "barcode41",
+    "CTACGTGTAAGGCATACCTGCCAG": "barcode42",
+    "CTTTCGTTGTTGACTCGACGGTAG": "barcode43",
+    "AGTAGAAAGGGTTCCTTCCCACTC": "barcode44",
+    "GATCCAACAGAGATGCCTTCAGTG": "barcode45",
+    "GCTGTGTTCCACTTCATTCTCCTG": "barcode46",
+    "GTGCAACTTTCCCACAGGTAGTTC": "barcode47",
+    "CATCTGGAACGTGGTACACCTGTA": "barcode48",
+    "ACTGGTGCAGCTTTGAACATCTAG": "barcode49",
+    "ATGGACTTTGGTAACTTCCTGCGT": "barcode50",
+    "GTTGAATGAGCCTACTGGGTCCTC": "barcode51",
+    "TGAGAGACAAGATTGTTCGTGGAC": "barcode52",
+    "AGATTCAGACCGTCTCATGCAAAG": "barcode53",
+    "CAAGAGCTTTGACTAAGGAGCATG": "barcode54",
+    "TGGAAGATGAGACCCTGATCTACG": "barcode55",
+    "TCACTACTCAACAGGTGGCATGAA": "barcode56",
+    "GCTAGGTCAATCTCCTTCGGAAGT": "barcode57",
+    "CAGGTTACTCCTCCGTGAGTCTGA": "barcode58",
+    "TCAATCAAGAAGGGAAAGCAAGGT": "barcode59",
+    "CATGTTCAACCAAGGCTTCTATGG": "barcode60",
+    "AGAGGGTACTATGTGCCTCAGCAC": "barcode61",
+    "CACCCACACTTACTTCAGGACGTA": "barcode62",
+    "TTCTGAAGTTCCTGGGTCTTGAAC": "barcode63",
+    "GACAGACACCGTTCATCGACTTTC": "barcode64",
+    "TTCTCAGTCTTCCTCCAGACAAGG": "barcode65",
+    "CCGATCCTTGTGGCTTCTAACTTC": "barcode66",
+    "GTTTGTCATACTCGTGTGCTCACC": "barcode67",
+    "GAATCTAAGCAAACACGAAGGTGG": "barcode68",
+    "TACAGTCCGAGCCTCATGTGATCT": "barcode69",
+    "ACCGAGATCCTACGAATGGAGTGT": "barcode70",
+    "CCTGGGAGCATCAGGTAGTAACAG": "barcode71",
+    "TAGCTGACTGTCTTCCATACCGAC": "barcode72",
+    "AAGAAACAGGATGACAGAACCCTC": "barcode73",
+    "TACAAGCATCCCAACACTTCCACT": "barcode74",
+    "GACCATTGTGATGAACCCTGTTGT": "barcode75",
+    "ATGCTTGTTACATCAACCCTGGAC": "barcode76",
+    "CGACCTGTTTCTCAGGGATACAAC": "barcode77",
+    "AACAACCGAACCTTTGAATCAGAA": "barcode78",
+    "TCTCGGAGATAGTTCTCACTGCTG": "barcode79",
+    "CGGATGAACATAGGATAGCGATTC": "barcode80",
+    "CCTCATCTTGTGAAGTTGTTTCGG": "barcode81",
+    "ACGGTATGTCGAGTTCCAGGACTA": "barcode82",
+    "TGGCTTGATCTAGGTAAGGTCGAA": "barcode83",
+    "GTAGTGGACCTAGAACCTGTGCCA": "barcode84",
+    "AACGGAGGAGTTAGTTGGATGATC": "barcode85",
+    "AGGTGATCCCAACAAGCGTAAGTA": "barcode86",
+    "TACATGCTCCTGTTGTTAGGGAGG": "barcode87",
+    "TCTTCTACTACCGATCCGAAGCAG": "barcode88",
+    "ACAGCATCAATGTTTGGCTAGTTG": "barcode89",
+    "GATGTAGAGGGTACGGTTTGAGGC": "barcode90",
+    "GGCTCCATAGGAACTCACGCTACT": "barcode91",
+    "TTGTGAGTGGAAAGATACAGGACC": "barcode92",
+    "AGTTTCCATCACTTCAGACTTGGG": "barcode93",
+    "GATTGTCCTCAAACTGCCACCTAC": "barcode94",
+    "CCTGTCTGGAAGAAGAATGGACTT": "barcode95",
+    "CTGAACGGTCATAGAGTCCACCAT": "barcode96",
+}
```

### Comparing `miso_tool-0.0.5/tests/test_cleaning.py` & `miso_tool-0.0.6/tests/test_cleaning.py`

 * *Files identical despite different names*

### Comparing `miso_tool-0.0.5/.gitignore` & `miso_tool-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `miso_tool-0.0.5/LICENSE.txt` & `miso_tool-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miso_tool-0.0.5/README.md` & `miso_tool-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `miso_tool-0.0.5/pyproject.toml` & `miso_tool-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `miso_tool-0.0.5/PKG-INFO` & `miso_tool-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: miso-tool
-Version: 0.0.5
+Version: 0.0.6
 Summary: A tool to work with sequencing run and sample info from MISO LIMS Pinery JSON data
 Project-URL: Documentation, https://github.com/unknown/miso-tool#readme
 Project-URL: Issues, https://github.com/unknown/miso-tool/issues
 Project-URL: Source, https://github.com/unknown/miso-tool
 Author-email: Peter Kruczkiewicz <peter.kruczkiewicz@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

