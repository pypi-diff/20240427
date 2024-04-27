# Comparing `tmp/rapidocr_pdf-0.0.8-py3-none-any.whl.zip` & `tmp/rapidocr_pdf-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 8761 bytes, number of entries: 8
--rw-r--r--  2.0 unx      124 b- defN 23-Dec-04 01:39 rapidocr_pdf/__init__.py
--rw-r--r--  2.0 unx     4631 b- defN 23-Dec-04 01:39 rapidocr_pdf/main.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Dec-04 01:40 rapidocr_pdf-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     3244 b- defN 23-Dec-04 01:40 rapidocr_pdf-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-04 01:40 rapidocr_pdf-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       57 b- defN 23-Dec-04 01:40 rapidocr_pdf-0.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Dec-04 01:40 rapidocr_pdf-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      669 b- defN 23-Dec-04 01:40 rapidocr_pdf-0.0.8.dist-info/RECORD
-8 files, 20187 bytes uncompressed, 7585 bytes compressed:  62.4%
+Zip file size: 9218 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      124 b- defN 24-Apr-27 12:47 rapidocr_pdf/__init__.py
+-rw-r--r--  2.0 unx     4976 b- defN 24-Apr-27 12:47 rapidocr_pdf/main.py
+-rw-r--r--  2.0 unx      280 b- defN 24-Apr-27 12:47 rapidocr_pdf/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-27 12:47 rapidocr_pdf-0.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3338 b- defN 24-Apr-27 12:47 rapidocr_pdf-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-27 12:47 rapidocr_pdf-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 24-Apr-27 12:47 rapidocr_pdf-0.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-27 12:47 rapidocr_pdf-0.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      746 b- defN 24-Apr-27 12:47 rapidocr_pdf-0.1.0.dist-info/RECORD
+9 files, 20982 bytes uncompressed, 7924 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
 Filename: rapidocr_pdf/__init__.py
 Comment: 
 
 Filename: rapidocr_pdf/main.py
 Comment: 
 
-Filename: rapidocr_pdf-0.0.8.dist-info/LICENSE
+Filename: rapidocr_pdf/utils.py
 Comment: 
 
-Filename: rapidocr_pdf-0.0.8.dist-info/METADATA
+Filename: rapidocr_pdf-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: rapidocr_pdf-0.0.8.dist-info/WHEEL
+Filename: rapidocr_pdf-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: rapidocr_pdf-0.0.8.dist-info/entry_points.txt
+Filename: rapidocr_pdf-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: rapidocr_pdf-0.0.8.dist-info/top_level.txt
+Filename: rapidocr_pdf-0.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapidocr_pdf-0.0.8.dist-info/RECORD
+Filename: rapidocr_pdf-0.1.0.dist-info/top_level.txt
+Comment: 
+
+Filename: rapidocr_pdf-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapidocr_pdf/main.py

```diff
@@ -7,28 +7,34 @@
 from typing import Dict, List, Tuple, Union
 
 import cv2
 import filetype
 import fitz
 import numpy as np
 
-try:
-    from rapidocr_onnxruntime import RapidOCR
-except:
-    warnings.warn(
-        "Can't find the rapidocr_onnxruntime module,"
-        "try to import the rapidocr_openvino"
-    )
-    from rapidocr_openvino import RapidOCR
+from .utils import import_package
 
 
 class PDFExtracter:
     def __init__(self, dpi=200, **ocr_kwargs):
         self.dpi = dpi
-        self.text_sys = RapidOCR(**ocr_kwargs)
+
+        ocr_engine = import_package("rapidocr_onnxruntime")
+        if ocr_engine is None:
+            ocr_engine = import_package("rapidocr_openvino")
+
+            if ocr_engine is None:
+                ocr_engine = import_package("rapidocr_paddle")
+
+            if ocr_engine is None:
+                raise ModuleNotFoundError(
+                    "Can't find the rapidocr_onnxruntime/rapidocr_openvino/rapidocr_paddle package.\n Please pip install rapidocr_onnxruntime to run the code."
+                )
+
+        self.text_sys = ocr_engine.RapidOCR(**ocr_kwargs)
         self.empyt_list = []
 
     def __call__(
         self,
         content: Union[str, Path, bytes],
         force_ocr: bool = False,
     ) -> List[List[Union[str, str, str]]]:
@@ -73,15 +79,15 @@
         texts, need_ocr_idxs = {}, []
         with fitz.open(stream=pdf_data) as doc:
             for i, page in enumerate(doc):
                 if force_ocr:
                     need_ocr_idxs.append(i)
                     continue
 
-                text = page.get_text()
+                text = page.get_text("text", sort=True)
                 if text:
                     texts[str(i)] = text
                 else:
                     need_ocr_idxs.append(i)
         return texts, need_ocr_idxs
 
     def read_pdf_with_image(self, pdf_data: bytes, need_ocr_idxs: List) -> Dict:
```

## Comparing `rapidocr_pdf-0.0.8.dist-info/LICENSE` & `rapidocr_pdf-0.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rapidocr_pdf-0.0.8.dist-info/METADATA` & `rapidocr_pdf-0.1.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidocr-pdf
-Version: 0.0.8
+Version: 0.1.0
 Summary: Tools of extracting PDF content based on RapidOCR
 Home-page: https://github.com/RapidAI/RapidOCRPDF
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: rapidocr_pdf,rapidocr_onnxruntime,ocr,onnxruntime,openvino
 Platform: Any
@@ -12,21 +12,24 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6,<3.12
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: filetype >=1.2.0
 Requires-Dist: pymupdf
 Requires-Dist: rapidocr-onnxruntime
 Provides-Extra: onnxruntime
 Requires-Dist: rapidocr-onnxruntime ; extra == 'onnxruntime'
 Provides-Extra: openvino
 Requires-Dist: rapidocr-openvino ; extra == 'openvino'
+Provides-Extra: paddle
+Requires-Dist: rapidocr-paddle ; extra == 'paddle'
 
 ## RapidOCRPDF
 <p>
     <a href=""><img src="https://img.shields.io/badge/Python->=3.6,<3.12-aff.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg"></a>
     <a href="https://pypi.org/project/rapidocr-pdf/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rapidocr-pdf"></a>
     <a href="https://pepy.tech/project/rapidocr-pdf"><img src="https://static.pepy.tech/personalized-badge/rapidocr-pdf?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads"></a>
@@ -76,9 +79,7 @@
    - **Output**：`List` \[**Page num**, **Page content** + **score**\], ：
        ```python
        [
            ['0', '达大学拉斯维加斯分校）的一次中文评测中获得最', '0.8969868'],
            ['1', 'ABCNet: Real-time Scene Text Spotting with Adaptive Bezier-Curve Network∗\nYuliang Liu‡†', '0.8969868'],
        ]
        ```
-
-
```

### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: rapidocr-pdf Version: 0.0.8 Summary: Tools of
+Metadata-Version: 2.1 Name: rapidocr-pdf Version: 0.1.0 Summary: Tools of
 extracting PDF content based on RapidOCR Home-page: https://github.com/RapidAI/
 RapidOCRPDF Author: SWHL Author-email: liekkaskono@163.com License: Apache-2.0
 Keywords: rapidocr_pdf,rapidocr_onnxruntime,ocr,onnxruntime,openvino Platform:
 Any Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6,<3.12 Description-Content-Type: text/markdown Requires-
-Dist: filetype >=1.2.0 Requires-Dist: pymupdf Requires-Dist: rapidocr-
-onnxruntime Provides-Extra: onnxruntime Requires-Dist: rapidocr-onnxruntime ;
-extra == 'onnxruntime' Provides-Extra: openvino Requires-Dist: rapidocr-
-openvino ; extra == 'openvino' ## RapidOCRPDF
+Requires-Python: >=3.6,<3.12 Description-Content-Type: text/markdown License-
+File: LICENSE Requires-Dist: filetype >=1.2.0 Requires-Dist: pymupdf Requires-
+Dist: rapidocr-onnxruntime Provides-Extra: onnxruntime Requires-Dist: rapidocr-
+onnxruntime ; extra == 'onnxruntime' Provides-Extra: openvino Requires-Dist:
+rapidocr-openvino ; extra == 'openvino' Provides-Extra: paddle Requires-Dist:
+rapidocr-paddle ; extra == 'paddle' ## RapidOCRPDF
 [https://img.shields.io/badge/Python->=3.6,<3.12-aff.svg][https://
 img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg]_[_P_y_P_I_]_[_h_t_t_p_s_:_/_/
 _s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_p_e_r_s_o_n_a_l_i_z_e_d_-_b_a_d_g_e_/_r_a_p_i_d_o_c_r_-
 _p_d_f_?_p_e_r_i_o_d_=_t_o_t_a_l_&_u_n_i_t_s_=_a_b_b_r_e_v_i_a_t_i_o_n_&_l_e_f_t___c_o_l_o_r_=_g_r_e_y_&_r_i_g_h_t___c_o_l_o_r_=_b_l_u_e_&_l_e_f_t___t_e_x_t_=_D_o_w_n_l_o_a_d_s_]
 _[_S_e_m_V_e_r_2_._0_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]_[_G_i_t_H_u_b_]
 - Relying on [RapidOCR](https://github.com/RapidAI/RapidOCR), quickly extract
 text from PDF, including scanned PDF and encrypted PDF. - Layout restore is not
```

## Comparing `rapidocr_pdf-0.0.8.dist-info/RECORD` & `rapidocr_pdf-0.1.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 rapidocr_pdf/__init__.py,sha256=ZKLhEqbDsbmmJqfqgtEtdmttuP1lAahqwH1Pc3nFMlI,124
-rapidocr_pdf/main.py,sha256=qorwoG_986oYhUoIk75t7FQ2Ck2Anw_xAwQr9GTl73c,4631
-rapidocr_pdf-0.0.8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-rapidocr_pdf-0.0.8.dist-info/METADATA,sha256=afmyDJLiWGmtfDvnSBP5Mvl-h7fDpHkpIgeo83iuhGE,3244
-rapidocr_pdf-0.0.8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-rapidocr_pdf-0.0.8.dist-info/entry_points.txt,sha256=dQ50ORbkK0BYQBJ1BNsgwNQ00KG7qr9gGTdhb_-m8A4,57
-rapidocr_pdf-0.0.8.dist-info/top_level.txt,sha256=cUWcSy5Kx0UwXhykCHUGic4Ldb3_z-frD6O7gKShomQ,13
-rapidocr_pdf-0.0.8.dist-info/RECORD,,
+rapidocr_pdf/main.py,sha256=660XLtjSI3nk9dHiAKL8eBpsC-vYvDfCovmy1FSlRDY,4976
+rapidocr_pdf/utils.py,sha256=jOP9CrPh1Cp-64KrcWWmOhvVmQMfciFHDH64uSolM4E,280
+rapidocr_pdf-0.1.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+rapidocr_pdf-0.1.0.dist-info/METADATA,sha256=o7cZZkJH3DWbfW2TPFFLR91dwmLsOEUJ3e1ncFQb4Qo,3338
+rapidocr_pdf-0.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+rapidocr_pdf-0.1.0.dist-info/entry_points.txt,sha256=Tn3_89lHUWrQ71NrFiy2l9wOZ2WKehwUiKjtZqHZVIE,56
+rapidocr_pdf-0.1.0.dist-info/top_level.txt,sha256=cUWcSy5Kx0UwXhykCHUGic4Ldb3_z-frD6O7gKShomQ,13
+rapidocr_pdf-0.1.0.dist-info/RECORD,,
```

