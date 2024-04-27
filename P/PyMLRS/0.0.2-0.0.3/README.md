# Comparing `tmp/pymlrs-0.0.2.tar.gz` & `tmp/pymlrs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymlrs-0.0.2.tar", last modified: Sat Apr 27 05:36:09 2024, max compression
+gzip compressed data, was "pymlrs-0.0.3.tar", last modified: Sat Apr 27 06:15:34 2024, max compression
```

## Comparing `pymlrs-0.0.2.tar` & `pymlrs-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 05:36:09.310251 pymlrs-0.0.2/
--rw-rw-rw-   0        0        0     1094 2024-04-09 08:47:53.000000 pymlrs-0.0.2/LICENCE.txt
--rw-rw-rw-   0        0        0    10803 2024-04-27 05:36:09.308247 pymlrs-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     9521 2024-04-27 05:28:23.000000 pymlrs-0.0.2/README.md
--rw-rw-rw-   0        0        0      115 2024-04-10 09:37:56.000000 pymlrs-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      675 2024-04-27 05:36:09.326245 pymlrs-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1377 2024-04-27 05:35:25.000000 pymlrs-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 05:36:08.943238 pymlrs-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-27 05:36:09.023766 pymlrs-0.0.2/src/PyMLRS/
--rw-rw-rw-   0        0        0    24915 2024-04-10 08:04:25.000000 pymlrs-0.0.2/src/PyMLRS/Mep_panel.py
--rw-rw-rw-   0        0        0    11738 2024-04-09 07:05:50.000000 pymlrs-0.0.2/src/PyMLRS/Rextractor.py
--rw-rw-rw-   0        0        0     9269 2024-03-23 09:04:34.000000 pymlrs-0.0.2/src/PyMLRS/Threshold.xlsx
--rw-rw-rw-   0        0        0        0 2024-04-09 09:36:13.000000 pymlrs-0.0.2/src/PyMLRS/__init__.py
--rw-rw-rw-   0        0        0  2964460 2024-03-27 08:50:12.000000 pymlrs-0.0.2/src/PyMLRS/model.pkl
-drwxrwxrwx   0        0        0        0 2024-04-27 05:36:09.243247 pymlrs-0.0.2/src/PyMLRS.egg-info/
--rw-rw-rw-   0        0        0    10803 2024-04-27 05:36:08.000000 pymlrs-0.0.2/src/PyMLRS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2024-04-27 05:36:08.000000 pymlrs-0.0.2/src/PyMLRS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 05:36:08.000000 pymlrs-0.0.2/src/PyMLRS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      143 2024-04-27 05:36:08.000000 pymlrs-0.0.2/src/PyMLRS.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-27 05:36:08.000000 pymlrs-0.0.2/src/PyMLRS.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 06:15:34.650114 pymlrs-0.0.3/
+-rw-rw-rw-   0        0        0     1094 2024-04-09 08:47:53.000000 pymlrs-0.0.3/LICENCE.txt
+-rw-rw-rw-   0        0        0    10786 2024-04-27 06:15:34.649116 pymlrs-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9504 2024-04-27 06:13:46.000000 pymlrs-0.0.3/README.md
+-rw-rw-rw-   0        0        0      115 2024-04-10 09:37:56.000000 pymlrs-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      675 2024-04-27 06:15:34.667144 pymlrs-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2024-04-27 05:41:02.000000 pymlrs-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 06:15:34.268089 pymlrs-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-27 06:15:34.468916 pymlrs-0.0.3/src/PyMLRS/
+-rw-rw-rw-   0        0        0    24916 2024-04-27 05:40:29.000000 pymlrs-0.0.3/src/PyMLRS/Mep_panel.py
+-rw-rw-rw-   0        0        0    11738 2024-04-09 07:05:50.000000 pymlrs-0.0.3/src/PyMLRS/Rextractor.py
+-rw-rw-rw-   0        0        0     9269 2024-03-23 09:04:34.000000 pymlrs-0.0.3/src/PyMLRS/Threshold.xlsx
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:36:13.000000 pymlrs-0.0.3/src/PyMLRS/__init__.py
+-rw-rw-rw-   0        0        0  2964460 2024-03-27 08:50:12.000000 pymlrs-0.0.3/src/PyMLRS/model.pkl
+drwxrwxrwx   0        0        0        0 2024-04-27 06:15:34.636793 pymlrs-0.0.3/src/PyMLRS.egg-info/
+-rw-rw-rw-   0        0        0    10786 2024-04-27 06:15:34.000000 pymlrs-0.0.3/src/PyMLRS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2024-04-27 06:15:34.000000 pymlrs-0.0.3/src/PyMLRS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 06:15:34.000000 pymlrs-0.0.3/src/PyMLRS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      143 2024-04-27 06:15:34.000000 pymlrs-0.0.3/src/PyMLRS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-27 06:15:34.000000 pymlrs-0.0.3/src/PyMLRS.egg-info/top_level.txt
```

### Comparing `pymlrs-0.0.2/LICENCE.txt` & `pymlrs-0.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pymlrs-0.0.2/PKG-INFO` & `pymlrs-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMLRS
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for processing and interpreting DNA high-resolution melt and amplification curves for the meningoencephalitis panel.
 Home-page: https://github.com/PyPCR/PyMLRS
 Author: Chandru, Vikram
 Author-email: mlrs.project2024@gmail.com
 License: MIT
 Keywords: High Resolution Melt,Amplification Curve,Cycle threshold,PCR,rt-PCR,Meningoencephalitis,MEP,Pathogens,Bharathiar University
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 Requires-Dist: pandas==1.5.3
 Requires-Dist: Pillow==9.4.0
 Requires-Dist: plotly==5.13.1
 Requires-Dist: scikit_learn==1.4.1.post1
 Requires-Dist: scipy==1.13.0
 Requires-Dist: openpyxl==3.1.2
 
-![vikramAsset 2@4x](https://github.com/Vikram2305/gitcheck/assets/124907782/43ad9d19-dca3-4505-9c59-4a2dfa6cb08a)
+<img src= "https://github.com/PyPCR/PyMLRS/blob/main/PyMLRS.png?raw=true" alt = "PyMLRS Logo">
 
 <div align="center">
     <br>
         <a href="" width="250px" height="250px" alt="pyHRM"></a>
       <br>
     <h1>PyMLRS</h1>
     <h2><b>A Python library for processing and interpreting DNA High-Resolution Melt and Amplification Curves for the Meningoencephalitis Panel</b></h2>
```

#### html2text {}

```diff
@@ -1,22 +1,20 @@
-Metadata-Version: 2.1 Name: PyMLRS Version: 0.0.2 Summary: A library for
+Metadata-Version: 2.1 Name: PyMLRS Version: 0.0.3 Summary: A library for
 processing and interpreting DNA high-resolution melt and amplification curves
 for the meningoencephalitis panel. Home-page: https://github.com/PyPCR/PyMLRS
 Author: Chandru, Vikram Author-email: mlrs.project2024@gmail.com License: MIT
 Keywords: High Resolution Melt,Amplification Curve,Cycle threshold,PCR,rt-
 PCR,Meningoencephalitis,MEP,Pathogens,Bharathiar University Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENCE.txt Requires-
 Dist: fpdf==1.7.2 Requires-Dist: matplotlib==3.6.3 Requires-Dist: numpy==1.23.5
 Requires-Dist: pandas==1.5.3 Requires-Dist: Pillow==9.4.0 Requires-Dist:
 plotly==5.13.1 Requires-Dist: scikit_learn==1.4.1.post1 Requires-Dist:
-scipy==1.13.0 Requires-Dist: openpyxl==3.1.2 ![vikramAsset 2@4x](https://
-github.com/Vikram2305/gitcheck/assets/124907782/43ad9d19-dca3-4505-9c59-
-4a2dfa6cb08a)
+scipy==1.13.0 Requires-Dist: openpyxl==3.1.2[Â "PyMLRSÂ Logo"]
 
 
                              ************ PPyyMMLLRRSS ************
 ********** AA PPyytthhoonn lliibbrraarryy ffoorr pprroocceessssiinngg aanndd iinntteerrpprreettiinngg DDNNAA HHiigghh--RReessoolluuttiioonn MMeelltt
        aanndd AAmmpplliiffiiccaattiioonn CCuurrvveess ffoorr tthhee MMeenniinnggooeenncceepphhaalliittiiss PPaanneell **********
          ****** _II_nn_ss_tt_aa_ll_ll_aa_tt_ii_oo_nn ?â??¢ _FF_ee_aa_tt_uu_rr_ee_ss ?â??¢ _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ?â??¢ _HH_ee_ll_pp ******
 # PyMLRS
```

### Comparing `pymlrs-0.0.2/README.md` & `pymlrs-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![vikramAsset 2@4x](https://github.com/Vikram2305/gitcheck/assets/124907782/43ad9d19-dca3-4505-9c59-4a2dfa6cb08a)
+<img src= "https://github.com/PyPCR/PyMLRS/blob/main/PyMLRS.png?raw=true" alt = "PyMLRS Logo">
 
 <div align="center">
     <br>
         <a href="" width="250px" height="250px" alt="pyHRM"></a>
       <br>
     <h1>PyMLRS</h1>
     <h2><b>A Python library for processing and interpreting DNA High-Resolution Melt and Amplification Curves for the Meningoencephalitis Panel</b></h2>
```

#### html2text {}

```diff
@@ -1,9 +1,8 @@
-![vikramAsset 2@4x](https://github.com/Vikram2305/gitcheck/assets/124907782/
-43ad9d19-dca3-4505-9c59-4a2dfa6cb08a)
+[Â "PyMLRSÂ Logo"]
 
 
                              ************ PPyyMMLLRRSS ************
 ********** AA PPyytthhoonn lliibbrraarryy ffoorr pprroocceessssiinngg aanndd iinntteerrpprreettiinngg DDNNAA HHiigghh--RReessoolluuttiioonn MMeelltt
        aanndd AAmmpplliiffiiccaattiioonn CCuurrvveess ffoorr tthhee MMeenniinnggooeenncceepphhaalliittiiss PPaanneell **********
          ****** _II_nn_ss_tt_aa_ll_ll_aa_tt_ii_oo_nn ?â??¢ _FF_ee_aa_tt_uu_rr_ee_ss ?â??¢ _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ?â??¢ _HH_ee_ll_pp ******
 # PyMLRS
```

### Comparing `pymlrs-0.0.2/setup.cfg` & `pymlrs-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2050 794d 4c52 530d 0a76 6572 7369   = PyMLRS..versi
-00000020: 6f6e 203d 2030 2e30 2e32 0d0a 6175 7468  on = 0.0.2..auth
+00000020: 6f6e 203d 2030 2e30 2e33 0d0a 6175 7468  on = 0.0.3..auth
 00000030: 6f72 203d 2043 6861 6e64 7275 2c20 5669  or = Chandru, Vi
 00000040: 6b72 616d 0d0a 6175 7468 6f72 5f65 6d61  kram..author_ema
 00000050: 696c 203d 206d 6c72 732e 7072 6f6a 6563  il = mlrs.projec
 00000060: 7432 3032 3440 676d 6169 6c2e 636f 6d0d  t2024@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000080: 204c 6962 7261 7279 2066 6f72 2070 726f   Library for pro
 00000090: 6365 7373 696e 6720 616e 6420 696e 7465  cessing and inte
```

### Comparing `pymlrs-0.0.2/setup.py` & `pymlrs-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 rd_file = os.path.join(dir_path, 'README.md')
 
 with io.open(rd_file, encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='PyMLRS',
-    version='0.0.2',
+    version='0.0.3',
     description='A library for processing and interpreting DNA high-resolution melt and amplification curves for the meningoencephalitis panel.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/PyPCR/PyMLRS',
     authors=["ChandruGaneshan", "VikramSekar"],
     authors_email=['chandruganeshan24@gmail.com', 'vikramsekar2305@gmail.com'],
     license='MIT',
```

### Comparing `pymlrs-0.0.2/src/PyMLRS/Mep_panel.py` & `pymlrs-0.0.3/src/PyMLRS/Mep_panel.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,15 +434,15 @@
         plt.close()
         plt.clf()
 
         # Create a PDF object
         pdf = FPDF(format="A4")
         pdf.add_page()
         pdf.set_font("Arial", "B", 16)
-        pdf.cell(0, 10, "PyPCR Report", ln=True)
+        pdf.cell(0, 10, "PyMLRS Report", ln=True)
         pdf.set_font("Arial", "", 10)
         pdf.cell(
             0, 7, f"Patient ID: {patient_id}", ln=True)
         pdf.cell(0, 7, f"Date: {datetime.now().date()}", ln=True)
         pdf.cell(
             0, 7, f"Time: {datetime.now().strftime('%I:%M:%S %p')}", ln=True)
         pdf.set_font("Arial", "", 12)
```

### Comparing `pymlrs-0.0.2/src/PyMLRS/Rextractor.py` & `pymlrs-0.0.3/src/PyMLRS/Rextractor.py`

 * *Files identical despite different names*

### Comparing `pymlrs-0.0.2/src/PyMLRS/Threshold.xlsx` & `pymlrs-0.0.3/src/PyMLRS/Threshold.xlsx`

 * *Files identical despite different names*

### Comparing `pymlrs-0.0.2/src/PyMLRS/model.pkl` & `pymlrs-0.0.3/src/PyMLRS/model.pkl`

 * *Files identical despite different names*

### Comparing `pymlrs-0.0.2/src/PyMLRS.egg-info/PKG-INFO` & `pymlrs-0.0.3/src/PyMLRS.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMLRS
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for processing and interpreting DNA high-resolution melt and amplification curves for the meningoencephalitis panel.
 Home-page: https://github.com/PyPCR/PyMLRS
 Author: Chandru, Vikram
 Author-email: mlrs.project2024@gmail.com
 License: MIT
 Keywords: High Resolution Melt,Amplification Curve,Cycle threshold,PCR,rt-PCR,Meningoencephalitis,MEP,Pathogens,Bharathiar University
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 Requires-Dist: pandas==1.5.3
 Requires-Dist: Pillow==9.4.0
 Requires-Dist: plotly==5.13.1
 Requires-Dist: scikit_learn==1.4.1.post1
 Requires-Dist: scipy==1.13.0
 Requires-Dist: openpyxl==3.1.2
 
-![vikramAsset 2@4x](https://github.com/Vikram2305/gitcheck/assets/124907782/43ad9d19-dca3-4505-9c59-4a2dfa6cb08a)
+<img src= "https://github.com/PyPCR/PyMLRS/blob/main/PyMLRS.png?raw=true" alt = "PyMLRS Logo">
 
 <div align="center">
     <br>
         <a href="" width="250px" height="250px" alt="pyHRM"></a>
       <br>
     <h1>PyMLRS</h1>
     <h2><b>A Python library for processing and interpreting DNA High-Resolution Melt and Amplification Curves for the Meningoencephalitis Panel</b></h2>
```

#### html2text {}

```diff
@@ -1,22 +1,20 @@
-Metadata-Version: 2.1 Name: PyMLRS Version: 0.0.2 Summary: A library for
+Metadata-Version: 2.1 Name: PyMLRS Version: 0.0.3 Summary: A library for
 processing and interpreting DNA high-resolution melt and amplification curves
 for the meningoencephalitis panel. Home-page: https://github.com/PyPCR/PyMLRS
 Author: Chandru, Vikram Author-email: mlrs.project2024@gmail.com License: MIT
 Keywords: High Resolution Melt,Amplification Curve,Cycle threshold,PCR,rt-
 PCR,Meningoencephalitis,MEP,Pathogens,Bharathiar University Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENCE.txt Requires-
 Dist: fpdf==1.7.2 Requires-Dist: matplotlib==3.6.3 Requires-Dist: numpy==1.23.5
 Requires-Dist: pandas==1.5.3 Requires-Dist: Pillow==9.4.0 Requires-Dist:
 plotly==5.13.1 Requires-Dist: scikit_learn==1.4.1.post1 Requires-Dist:
-scipy==1.13.0 Requires-Dist: openpyxl==3.1.2 ![vikramAsset 2@4x](https://
-github.com/Vikram2305/gitcheck/assets/124907782/43ad9d19-dca3-4505-9c59-
-4a2dfa6cb08a)
+scipy==1.13.0 Requires-Dist: openpyxl==3.1.2[Â "PyMLRSÂ Logo"]
 
 
                              ************ PPyyMMLLRRSS ************
 ********** AA PPyytthhoonn lliibbrraarryy ffoorr pprroocceessssiinngg aanndd iinntteerrpprreettiinngg DDNNAA HHiigghh--RReessoolluuttiioonn MMeelltt
        aanndd AAmmpplliiffiiccaattiioonn CCuurrvveess ffoorr tthhee MMeenniinnggooeenncceepphhaalliittiiss PPaanneell **********
          ****** _II_nn_ss_tt_aa_ll_ll_aa_tt_ii_oo_nn ?â??¢ _FF_ee_aa_tt_uu_rr_ee_ss ?â??¢ _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ?â??¢ _HH_ee_ll_pp ******
 # PyMLRS
```

