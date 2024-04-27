# Comparing `tmp/pdf2dcm-0.4.1.tar.gz` & `tmp/pdf2dcm-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf2dcm-0.4.1.tar", max compression
+gzip compressed data, was "pdf2dcm-0.5.0.tar", max compression
```

## Comparing `pdf2dcm-0.4.1.tar` & `pdf2dcm-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2023-03-16 04:09:48.115398 pdf2dcm-0.4.1/LICENSE
--rw-r--r--   0        0        0     4133 2023-03-16 04:09:48.115398 pdf2dcm-0.4.1/README.md
--rw-r--r--   0        0        0      107 2023-03-16 04:09:49.003465 pdf2dcm-0.4.1/pdf2dcm/__init__.py
--rw-r--r--   0        0        0     3815 2023-03-16 04:09:48.115398 pdf2dcm-0.4.1/pdf2dcm/base.py
--rw-r--r--   0        0        0     3227 2023-03-16 04:09:48.115398 pdf2dcm-0.4.1/pdf2dcm/pdf2encaps.py
--rw-r--r--   0        0        0     4865 2023-03-16 04:09:48.115398 pdf2dcm-0.4.1/pdf2dcm/pdf2rgb.py
--rw-r--r--   0        0        0      449 2023-03-16 04:09:48.115398 pdf2dcm-0.4.1/pdf2dcm/utils/uid.py
--rw-r--r--   0        0        0      913 2023-03-16 04:09:49.003465 pdf2dcm-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4957 1970-01-01 00:00:00.000000 pdf2dcm-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-16 06:29:56.426812 pdf2dcm-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4501 2024-04-16 06:29:56.426812 pdf2dcm-0.5.0/README.md
+-rw-r--r--   0        0        0      107 2024-04-16 06:29:56.426812 pdf2dcm-0.5.0/pdf2dcm/__init__.py
+-rw-r--r--   0        0        0     3993 2024-04-16 06:29:56.426812 pdf2dcm-0.5.0/pdf2dcm/base.py
+-rw-r--r--   0        0        0     3437 2024-04-16 06:29:56.426812 pdf2dcm-0.5.0/pdf2dcm/pdf2encaps.py
+-rw-r--r--   0        0        0     5044 2024-04-16 06:29:56.426812 pdf2dcm-0.5.0/pdf2dcm/pdf2rgb.py
+-rw-r--r--   0        0        0      449 2024-04-16 06:29:56.426812 pdf2dcm-0.5.0/pdf2dcm/utils/uid.py
+-rw-r--r--   0        0        0      984 2024-04-27 18:30:37.180546 pdf2dcm-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5380 1970-01-01 00:00:00.000000 pdf2dcm-0.5.0/PKG-INFO
```

### Comparing `pdf2dcm-0.4.1/LICENSE` & `pdf2dcm-0.5.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Abhijeet Parida
+Copyright (c) 2023-2024 Abhijeet Parida
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pdf2dcm-0.4.1/README.md` & `pdf2dcm-0.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -89,17 +89,34 @@
 
 - The name of the output dicom is same as the name of the input pdf
 - If no template is provided no repersonalisation takes place
 - It is possible to produce dicoms without a suffix by simply passing `suffix=""` to the `converter.run()`
 
 ## Repersonalisation
 
-It is the process of copying over data regarding the identity of the encapsualted pdf from a template dicom. Currently, the fileds that are repersonalised are-
+It is the process of copying over data regarding the identity of the encapsualted pdf from a template dicom. Currently, the fields that are repersonalised by default are-
 
 - PatientName
 - PatientID
 - PatientSex
 - StudyInstanceUID
 - ~~SeriesInstanceUID~~
 - ~~SOPInstanceUID~~
 
 The fields `SeriesInstanceUID` and `SOPInstanceUID` have been removed from the repersonalization by copying as it violates the DICOM standards.
+
+You can set the fields to repersonalize by passing repersonalisation_fields into `Pdf2EncapsDCM()`, or `Pdf2RgbSC()`
+
+Example:
+
+```python
+fields = [
+    "PatientName",
+    "PatientID",
+    "PatientSex",
+    "StudyInstanceUID",
+    "AccessionNumber"
+]
+converter = Pdf2RgbSC(repersonalisation_fields=fields)
+```
+
+note: this will overwrite the default fields.
```

### Comparing `pdf2dcm-0.4.1/pdf2dcm/base.py` & `pdf2dcm-0.5.0/pdf2dcm/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,21 +10,24 @@
 from typing import List
 import datetime
 
 import warnings
 
 
 class BaseConverter(ABC):
-    def __init__(self):
-        self.repersonalisation_fields = [
-            "PatientName",
-            "PatientID",
-            "PatientSex",
-            "StudyInstanceUID",
-        ]
+    def __init__(self, repersonalisation_fields=[]):
+        if len(repersonalisation_fields):
+            self.repersonalisation_fields = repersonalisation_fields
+        else:
+            self.repersonalisation_fields = [
+                "PatientName",
+                "PatientID",
+                "PatientSex",
+                "StudyInstanceUID",
+            ]
 
     def personalize_dcm(
         self, template_dcm_path: Path, pdf_dcm: FileDataset
     ) -> FileDataset:
         template_dcm = pydicom.dcmread(template_dcm_path)
 
         for field in self.repersonalisation_fields:
```

### Comparing `pdf2dcm-0.4.1/pdf2dcm/pdf2encaps.py` & `pdf2dcm-0.5.0/pdf2dcm/pdf2encaps.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,21 @@
 from pathlib import Path
 from typing import List
 import os
 from pydicom.dataset import FileMetaDataset, FileDataset
 
 
 class Pdf2EncapsDCM(BaseConverter):
-    def __init__(self):
-        """Class for Encapsulated PDF generation"""
-        super().__init__()
+    def __init__(self, repersonalisation_fields=[]):
+        """Class for Encapsulated PDF generation
+        
+        Args:
+            repersonalisation_fields (List<String>, optional): fields to be copied to the new image
+        """
+        super().__init__(repersonalisation_fields=repersonalisation_fields)
 
     def _get_encapspdf_meta(self) -> FileMetaDataset:
         """Get and set the file meta information for the pdf encaps dicom
 
         Returns:
             FileMetaDataset: header meta info of he dicom
         """
```

### Comparing `pdf2dcm-0.4.1/pdf2dcm/pdf2rgb.py` & `pdf2dcm-0.5.0/pdf2dcm/pdf2rgb.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,24 +7,26 @@
 from pydicom.uid import generate_uid
 from pdf2image import convert_from_path
 from copy import deepcopy
 from PIL import Image
 
 
 class Pdf2RgbSC(BaseConverter):
-    def __init__(self, dpi=144, merge_pages=False):
+    def __init__(self, dpi=144, merge_pages=False, repersonalisation_fields=[]):
         """Class for the generation RGB Secondary capture
 
         Args:
             dpi (int, optional): dots per inch, set resolution of the image. Defaults to 144.
             merge_pages (bool, optional): multiple pgs must be put into 1 dicom. Defaults to False.
+            repersonalisation_fields (List<String>, optional): fields to be copied to the new image
+
         """
         self.merge_pages_flag = merge_pages
         self.dpi = dpi
-        super().__init__()
+        super().__init__(repersonalisation_fields=repersonalisation_fields)
 
     def _get_rgbsc_meta(self) -> FileMetaDataset:
         """Get and set the file meta information for the rgb secondary capture dicom
 
         Returns:
             FileMetaDataset: header meta info of the dicom
         """
```

### Comparing `pdf2dcm-0.4.1/PKG-INFO` & `pdf2dcm-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: pdf2dcm
-Version: 0.4.1
+Version: 0.5.0
 Summary: A PDF to Dicom Converter
-Home-page: https://github.com/a-parida12/pdf2dcm
+Home-page: https://a-parida12.github.io/pdf2dcm/pdf2dcm/
 License: MIT
 Keywords: dicom,pdf,pdf2dcm,pdf2dicom,pydicom,pdf2dicomRGB
 Author: Abhijeet Parida
 Author-email: abhijeet.parida@tum.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pdf2image (>=1.16.0,<2.0.0)
-Requires-Dist: pillow (>=9.2.0,<10.0.0)
-Requires-Dist: pydicom (>=2.2.2,<3.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pdf2image (>=1.16.3,<2.0.0)
+Requires-Dist: pillow (>=9.5,<11.0)
+Requires-Dist: pydicom (>=2.3.0,<3.0.0)
 Project-URL: Repository, https://github.com/a-parida12/pdf2dcm
 Description-Content-Type: text/markdown
 
 # pdf2dcm
 [![PyPI version](https://img.shields.io/pypi/v/pdf2dcm.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/pdf2dcm/) [![Supported Python versions](https://img.shields.io/pypi/pyversions/pdf2dcm.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/pdf2dcm)[![Downloads](https://static.pepy.tech/personalized-badge/pdf2dcm?period=month&units=abbreviation&left_color=brightgreen&right_color=blue&left_text=PyPi%20Velocity)](https://pepy.tech/project/pdf2dcm) [![Downloads](https://static.pepy.tech/personalized-badge/pdf2dcm?period=total&units=abbreviation&left_color=brightgreen&right_color=blue&left_text=PyPi%20Downloads)](https://pepy.tech/project/pdf2dcm)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)[![codecov](https://codecov.io/gh/a-parida12/pdf2dcm/branch/main/graph/badge.svg?token=MGY9MHRP46)](https://codecov.io/gh/a-parida12/pdf2dcm)[![Test Pipeline](https://github.com/a-parida12/pdf2dcm/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/a-parida12/pdf2dcm/actions/workflows/test.yml)[![Release Pipeline](https://github.com/a-parida12/pdf2dcm/actions/workflows/release.yml/badge.svg?branch=main)](https://github.com/a-parida12/pdf2dcm/actions/workflows/release.yml)
 
@@ -111,18 +112,34 @@
 
 - The name of the output dicom is same as the name of the input pdf
 - If no template is provided no repersonalisation takes place
 - It is possible to produce dicoms without a suffix by simply passing `suffix=""` to the `converter.run()`
 
 ## Repersonalisation
 
-It is the process of copying over data regarding the identity of the encapsualted pdf from a template dicom. Currently, the fileds that are repersonalised are-
+It is the process of copying over data regarding the identity of the encapsualted pdf from a template dicom. Currently, the fields that are repersonalised by default are-
 
 - PatientName
 - PatientID
 - PatientSex
 - StudyInstanceUID
 - ~~SeriesInstanceUID~~
 - ~~SOPInstanceUID~~
 
 The fields `SeriesInstanceUID` and `SOPInstanceUID` have been removed from the repersonalization by copying as it violates the DICOM standards.
 
+You can set the fields to repersonalize by passing repersonalisation_fields into `Pdf2EncapsDCM()`, or `Pdf2RgbSC()`
+
+Example:
+
+```python
+fields = [
+    "PatientName",
+    "PatientID",
+    "PatientSex",
+    "StudyInstanceUID",
+    "AccessionNumber"
+]
+converter = Pdf2RgbSC(repersonalisation_fields=fields)
+```
+
+note: this will overwrite the default fields.
```

