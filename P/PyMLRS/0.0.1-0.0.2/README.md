# Comparing `tmp/PyMLRS-0.0.1.tar.gz` & `tmp/pymlrs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMLRS-0.0.1.tar", last modified: Wed Apr 10 13:02:49 2024, max compression
+gzip compressed data, was "pymlrs-0.0.2.tar", last modified: Sat Apr 27 05:36:09 2024, max compression
```

## Comparing `PyMLRS-0.0.1.tar` & `pymlrs-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 13:02:49.054963 PyMLRS-0.0.1/
--rw-rw-rw-   0        0        0     1094 2024-04-09 08:47:53.000000 PyMLRS-0.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0    10704 2024-04-10 13:02:49.049975 PyMLRS-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     9421 2024-04-10 12:59:28.000000 PyMLRS-0.0.1/README.md
--rw-rw-rw-   0        0        0      115 2024-04-10 09:37:56.000000 PyMLRS-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      674 2024-04-10 13:02:49.058950 PyMLRS-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1376 2024-04-10 13:01:38.000000 PyMLRS-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 13:02:48.945864 PyMLRS-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-10 13:02:48.973359 PyMLRS-0.0.1/src/PyMLRS/
--rw-rw-rw-   0        0        0    24915 2024-04-10 08:04:25.000000 PyMLRS-0.0.1/src/PyMLRS/Mep_panel.py
--rw-rw-rw-   0        0        0    11738 2024-04-09 07:05:50.000000 PyMLRS-0.0.1/src/PyMLRS/Rextractor.py
--rw-rw-rw-   0        0        0     9269 2024-03-23 09:04:34.000000 PyMLRS-0.0.1/src/PyMLRS/Threshold.xlsx
--rw-rw-rw-   0        0        0        0 2024-04-09 09:36:13.000000 PyMLRS-0.0.1/src/PyMLRS/__init__.py
--rw-rw-rw-   0        0        0  2964460 2024-03-27 08:50:12.000000 PyMLRS-0.0.1/src/PyMLRS/model.pkl
-drwxrwxrwx   0        0        0        0 2024-04-10 13:02:49.047979 PyMLRS-0.0.1/src/PyMLRS.egg-info/
--rw-rw-rw-   0        0        0    10704 2024-04-10 13:02:48.000000 PyMLRS-0.0.1/src/PyMLRS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2024-04-10 13:02:48.000000 PyMLRS-0.0.1/src/PyMLRS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 13:02:48.000000 PyMLRS-0.0.1/src/PyMLRS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      143 2024-04-10 13:02:48.000000 PyMLRS-0.0.1/src/PyMLRS.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-10 13:02:48.000000 PyMLRS-0.0.1/src/PyMLRS.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 05:36:09.310251 pymlrs-0.0.2/
+-rw-rw-rw-   0        0        0     1094 2024-04-09 08:47:53.000000 pymlrs-0.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0    10803 2024-04-27 05:36:09.308247 pymlrs-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9521 2024-04-27 05:28:23.000000 pymlrs-0.0.2/README.md
+-rw-rw-rw-   0        0        0      115 2024-04-10 09:37:56.000000 pymlrs-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      675 2024-04-27 05:36:09.326245 pymlrs-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2024-04-27 05:35:25.000000 pymlrs-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 05:36:08.943238 pymlrs-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-27 05:36:09.023766 pymlrs-0.0.2/src/PyMLRS/
+-rw-rw-rw-   0        0        0    24915 2024-04-10 08:04:25.000000 pymlrs-0.0.2/src/PyMLRS/Mep_panel.py
+-rw-rw-rw-   0        0        0    11738 2024-04-09 07:05:50.000000 pymlrs-0.0.2/src/PyMLRS/Rextractor.py
+-rw-rw-rw-   0        0        0     9269 2024-03-23 09:04:34.000000 pymlrs-0.0.2/src/PyMLRS/Threshold.xlsx
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:36:13.000000 pymlrs-0.0.2/src/PyMLRS/__init__.py
+-rw-rw-rw-   0        0        0  2964460 2024-03-27 08:50:12.000000 pymlrs-0.0.2/src/PyMLRS/model.pkl
+drwxrwxrwx   0        0        0        0 2024-04-27 05:36:09.243247 pymlrs-0.0.2/src/PyMLRS.egg-info/
+-rw-rw-rw-   0        0        0    10803 2024-04-27 05:36:08.000000 pymlrs-0.0.2/src/PyMLRS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2024-04-27 05:36:08.000000 pymlrs-0.0.2/src/PyMLRS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 05:36:08.000000 pymlrs-0.0.2/src/PyMLRS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      143 2024-04-27 05:36:08.000000 pymlrs-0.0.2/src/PyMLRS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-27 05:36:08.000000 pymlrs-0.0.2/src/PyMLRS.egg-info/top_level.txt
```

### Comparing `PyMLRS-0.0.1/LICENCE.txt` & `pymlrs-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `PyMLRS-0.0.1/PKG-INFO` & `pymlrs-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: PyMLRS
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for processing and interpreting DNA high-resolution melt and amplification curves for the meningoencephalitis panel.
-Home-page: https://github.com/PyPCR/PyPCR
+Home-page: https://github.com/PyPCR/PyMLRS
 Author: Chandru, Vikram
 Author-email: mlrs.project2024@gmail.com
 License: MIT
 Keywords: High Resolution Melt,Amplification Curve,Cycle threshold,PCR,rt-PCR,Meningoencephalitis,MEP,Pathogens,Bharathiar University
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,16 @@
 Requires-Dist: pandas==1.5.3
 Requires-Dist: Pillow==9.4.0
 Requires-Dist: plotly==5.13.1
 Requires-Dist: scikit_learn==1.4.1.post1
 Requires-Dist: scipy==1.13.0
 Requires-Dist: openpyxl==3.1.2
 
+![vikramAsset 2@4x](https://github.com/Vikram2305/gitcheck/assets/124907782/43ad9d19-dca3-4505-9c59-4a2dfa6cb08a)
+
 <div align="center">
     <br>
         <a href="" width="250px" height="250px" alt="pyHRM"></a>
       <br>
     <h1>PyMLRS</h1>
     <h2><b>A Python library for processing and interpreting DNA High-Resolution Melt and Amplification Curves for the Meningoencephalitis Panel</b></h2>
         <h4>
@@ -290,19 +292,17 @@
 ```
 from PyMLRS.Rextractor import rex_reader
 from PyMLRS.Mep_panel import Mep_diagnoser
 
 # File extraction from the rex file
 patient_id,hrm,ct = rex_reader("Your .rex file path")
 
-# Create Object
-md = Mep_diagnoser()
-
 # Interpreting the results
 for id in patient_id:
+    md = Mep_diagnoser()
     hrm_data = md.transform_hrm(hrm[id])
     ct_data = md.transform_ct(ct[id])
     melt = md.hrm_to_melt(figure = False)
     hrm_features = md.hrm_feature_extraction()
     ct_values = md.ct_value()
     result = md.predict_result()
     report = md.report( output_fie_path=f"{id}.pdf",patient_id=id)
@@ -321,9 +321,7 @@
     <tr>
       <td align='center' valign='top'><a href="https://github.com/chandru-g24"> <img src="https://avatars.githubusercontent.com/u/111188572?s=400&u=befb7d97d2b8419a715a22b09d92f825bdc33906&v=4" width = '60px;' alt='Chandru G'/> <br /> <sub><b><a href="https://www.linkedin.com/in/chandru-g24/"> Chandru Ganeshan</a></b></sub></a><br /></td>
       <td align='center' valign='top'><a href="https://github.com/Vikram2305"> <img src="https://avatars.githubusercontent.com/u/124907782?s=400&u=a5d9c4ca9f08e5bb5e88bc4d049d5e80703d1c89&v=4" width = '60px;' alt='Vikram S'/> <br /> <sub><b><a href="https://www.linkedin.com/in/vikram-sekar/"> Vikram Sekar</a></b></sub></a><br /></td>
     </tr>
   </tbody>
   
 </table>
-
-
```

#### html2text {}

```diff
@@ -1,20 +1,22 @@
-Metadata-Version: 2.1 Name: PyMLRS Version: 0.0.1 Summary: A library for
+Metadata-Version: 2.1 Name: PyMLRS Version: 0.0.2 Summary: A library for
 processing and interpreting DNA high-resolution melt and amplification curves
-for the meningoencephalitis panel. Home-page: https://github.com/PyPCR/PyPCR
+for the meningoencephalitis panel. Home-page: https://github.com/PyPCR/PyMLRS
 Author: Chandru, Vikram Author-email: mlrs.project2024@gmail.com License: MIT
 Keywords: High Resolution Melt,Amplification Curve,Cycle threshold,PCR,rt-
 PCR,Meningoencephalitis,MEP,Pathogens,Bharathiar University Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENCE.txt Requires-
 Dist: fpdf==1.7.2 Requires-Dist: matplotlib==3.6.3 Requires-Dist: numpy==1.23.5
 Requires-Dist: pandas==1.5.3 Requires-Dist: Pillow==9.4.0 Requires-Dist:
 plotly==5.13.1 Requires-Dist: scikit_learn==1.4.1.post1 Requires-Dist:
-scipy==1.13.0 Requires-Dist: openpyxl==3.1.2
+scipy==1.13.0 Requires-Dist: openpyxl==3.1.2 ![vikramAsset 2@4x](https://
+github.com/Vikram2305/gitcheck/assets/124907782/43ad9d19-dca3-4505-9c59-
+4a2dfa6cb08a)
 
 
                              ************ PPyyMMLLRRSS ************
 ********** AA PPyytthhoonn lliibbrraarryy ffoorr pprroocceessssiinngg aanndd iinntteerrpprreettiinngg DDNNAA HHiigghh--RReessoolluuttiioonn MMeelltt
        aanndd AAmmpplliiffiiccaattiioonn CCuurrvveess ffoorr tthhee MMeenniinnggooeenncceepphhaalliittiiss PPaanneell **********
          ****** _II_nn_ss_tt_aa_ll_ll_aa_tt_ii_oo_nn ?â??¢ _FF_ee_aa_tt_uu_rr_ee_ss ?â??¢ _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ?â??¢ _HH_ee_ll_pp ******
 # PyMLRS
@@ -134,21 +136,21 @@
 Interpreting the results by providing patient ID manually hrm_data =
 md.transform_hrm(hrm[id]) ct_data = md.transform_ct(ct[id]) melt =
 md.hrm_to_melt(figure = False) hrm_features = md.hrm_feature_extraction()
 ct_values = md.ct_value() result = md.predict_result() report = md.report
 ( output_fie_path=f"{id}.pdf",patient_id=id) ``` ### Sample code Snippet for
 interpreting all individual result ``` from PyMLRS.Rextractor import rex_reader
 from PyMLRS.Mep_panel import Mep_diagnoser # File extraction from the rex file
-patient_id,hrm,ct = rex_reader("Your .rex file path") # Create Object md =
-Mep_diagnoser() # Interpreting the results for id in patient_id: hrm_data =
-md.transform_hrm(hrm[id]) ct_data = md.transform_ct(ct[id]) melt =
-md.hrm_to_melt(figure = False) hrm_features = md.hrm_feature_extraction()
-ct_values = md.ct_value() result = md.predict_result() report = md.report
-( output_fie_path=f"{id}.pdf",patient_id=id) ``` # Getting Help If you need to
-get in touch with the team, please contact through email address:
+patient_id,hrm,ct = rex_reader("Your .rex file path") # Interpreting the
+results for id in patient_id: md = Mep_diagnoser() hrm_data = md.transform_hrm
+(hrm[id]) ct_data = md.transform_ct(ct[id]) melt = md.hrm_to_melt(figure =
+False) hrm_features = md.hrm_feature_extraction() ct_values = md.ct_value()
+result = md.predict_result() report = md.report( output_fie_path=f"
+{id}.pdf",patient_id=id) ``` # Getting Help If you need to get in touch with
+the team, please contact through email address:
 [chandruganeshan24@gmail.com](mailto:chandruganeshan24@gmail.com)
 [vikramsekar2305@gmail.com](mailto:vikramsekar2305@gmail.com) # Developers The
 developer of this Software are M.Sc Data Analytics Students in Department of
 Computer Application at [Bharathiar University](https://b-u.ac.in/23/
 department-computer-applications)
   _[_C_h_a_n_d_r_u_ _G_]     _[_V_i_k_r_a_m_ _S_]
 _CC_hh_aa_nn_dd_rr_uu_ _GG_aa_nn_ee_ss_hh_aa_nn _VV_ii_kk_rr_aa_mm_ _SS_ee_kk_aa_rr
```

### Comparing `PyMLRS-0.0.1/README.md` & `pymlrs-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+![vikramAsset 2@4x](https://github.com/Vikram2305/gitcheck/assets/124907782/43ad9d19-dca3-4505-9c59-4a2dfa6cb08a)
+
 <div align="center">
     <br>
         <a href="" width="250px" height="250px" alt="pyHRM"></a>
       <br>
     <h1>PyMLRS</h1>
     <h2><b>A Python library for processing and interpreting DNA High-Resolution Melt and Amplification Curves for the Meningoencephalitis Panel</b></h2>
         <h4>
@@ -265,19 +267,17 @@
 ```
 from PyMLRS.Rextractor import rex_reader
 from PyMLRS.Mep_panel import Mep_diagnoser
 
 # File extraction from the rex file
 patient_id,hrm,ct = rex_reader("Your .rex file path")
 
-# Create Object
-md = Mep_diagnoser()
-
 # Interpreting the results
 for id in patient_id:
+    md = Mep_diagnoser()
     hrm_data = md.transform_hrm(hrm[id])
     ct_data = md.transform_ct(ct[id])
     melt = md.hrm_to_melt(figure = False)
     hrm_features = md.hrm_feature_extraction()
     ct_values = md.ct_value()
     result = md.predict_result()
     report = md.report( output_fie_path=f"{id}.pdf",patient_id=id)
@@ -296,9 +296,7 @@
     <tr>
       <td align='center' valign='top'><a href="https://github.com/chandru-g24"> <img src="https://avatars.githubusercontent.com/u/111188572?s=400&u=befb7d97d2b8419a715a22b09d92f825bdc33906&v=4" width = '60px;' alt='Chandru G'/> <br /> <sub><b><a href="https://www.linkedin.com/in/chandru-g24/"> Chandru Ganeshan</a></b></sub></a><br /></td>
       <td align='center' valign='top'><a href="https://github.com/Vikram2305"> <img src="https://avatars.githubusercontent.com/u/124907782?s=400&u=a5d9c4ca9f08e5bb5e88bc4d049d5e80703d1c89&v=4" width = '60px;' alt='Vikram S'/> <br /> <sub><b><a href="https://www.linkedin.com/in/vikram-sekar/"> Vikram Sekar</a></b></sub></a><br /></td>
     </tr>
   </tbody>
   
 </table>
-
-
```

#### html2text {}

```diff
@@ -1,7 +1,9 @@
+![vikramAsset 2@4x](https://github.com/Vikram2305/gitcheck/assets/124907782/
+43ad9d19-dca3-4505-9c59-4a2dfa6cb08a)
 
 
                              ************ PPyyMMLLRRSS ************
 ********** AA PPyytthhoonn lliibbrraarryy ffoorr pprroocceessssiinngg aanndd iinntteerrpprreettiinngg DDNNAA HHiigghh--RReessoolluuttiioonn MMeelltt
        aanndd AAmmpplliiffiiccaattiioonn CCuurrvveess ffoorr tthhee MMeenniinnggooeenncceepphhaalliittiiss PPaanneell **********
          ****** _II_nn_ss_tt_aa_ll_ll_aa_tt_ii_oo_nn ?â??¢ _FF_ee_aa_tt_uu_rr_ee_ss ?â??¢ _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ?â??¢ _HH_ee_ll_pp ******
 # PyMLRS
@@ -121,21 +123,21 @@
 Interpreting the results by providing patient ID manually hrm_data =
 md.transform_hrm(hrm[id]) ct_data = md.transform_ct(ct[id]) melt =
 md.hrm_to_melt(figure = False) hrm_features = md.hrm_feature_extraction()
 ct_values = md.ct_value() result = md.predict_result() report = md.report
 ( output_fie_path=f"{id}.pdf",patient_id=id) ``` ### Sample code Snippet for
 interpreting all individual result ``` from PyMLRS.Rextractor import rex_reader
 from PyMLRS.Mep_panel import Mep_diagnoser # File extraction from the rex file
-patient_id,hrm,ct = rex_reader("Your .rex file path") # Create Object md =
-Mep_diagnoser() # Interpreting the results for id in patient_id: hrm_data =
-md.transform_hrm(hrm[id]) ct_data = md.transform_ct(ct[id]) melt =
-md.hrm_to_melt(figure = False) hrm_features = md.hrm_feature_extraction()
-ct_values = md.ct_value() result = md.predict_result() report = md.report
-( output_fie_path=f"{id}.pdf",patient_id=id) ``` # Getting Help If you need to
-get in touch with the team, please contact through email address:
+patient_id,hrm,ct = rex_reader("Your .rex file path") # Interpreting the
+results for id in patient_id: md = Mep_diagnoser() hrm_data = md.transform_hrm
+(hrm[id]) ct_data = md.transform_ct(ct[id]) melt = md.hrm_to_melt(figure =
+False) hrm_features = md.hrm_feature_extraction() ct_values = md.ct_value()
+result = md.predict_result() report = md.report( output_fie_path=f"
+{id}.pdf",patient_id=id) ``` # Getting Help If you need to get in touch with
+the team, please contact through email address:
 [chandruganeshan24@gmail.com](mailto:chandruganeshan24@gmail.com)
 [vikramsekar2305@gmail.com](mailto:vikramsekar2305@gmail.com) # Developers The
 developer of this Software are M.Sc Data Analytics Students in Department of
 Computer Application at [Bharathiar University](https://b-u.ac.in/23/
 department-computer-applications)
   _[_C_h_a_n_d_r_u_ _G_]     _[_V_i_k_r_a_m_ _S_]
 _CC_hh_aa_nn_dd_rr_uu_ _GG_aa_nn_ee_ss_hh_aa_nn _VV_ii_kk_rr_aa_mm_ _SS_ee_kk_aa_rr
```

### Comparing `PyMLRS-0.0.1/setup.cfg` & `pymlrs-0.0.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2050 794d 4c52 530d 0a76 6572 7369   = PyMLRS..versi
-00000020: 6f6e 203d 2030 2e30 2e31 0d0a 6175 7468  on = 0.0.1..auth
+00000020: 6f6e 203d 2030 2e30 2e32 0d0a 6175 7468  on = 0.0.2..auth
 00000030: 6f72 203d 2043 6861 6e64 7275 2c20 5669  or = Chandru, Vi
 00000040: 6b72 616d 0d0a 6175 7468 6f72 5f65 6d61  kram..author_ema
 00000050: 696c 203d 206d 6c72 732e 7072 6f6a 6563  il = mlrs.projec
 00000060: 7432 3032 3440 676d 6169 6c2e 636f 6d0d  t2024@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000080: 204c 6962 7261 7279 2066 6f72 2070 726f   Library for pro
 00000090: 6365 7373 696e 6720 616e 6420 696e 7465  cessing and inte
@@ -17,27 +17,27 @@
 00000100: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 00000110: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
 00000120: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
 00000130: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
 00000140: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
 00000150: 0d0a 7572 6c20 3d20 2768 7474 7073 3a2f  ..url = 'https:/
 00000160: 2f67 6974 6875 622e 636f 6d2f 5079 5043  /github.com/PyPC
-00000170: 522f 5079 5043 5227 0d0a 636c 6173 7369  R/PyPCR'..classi
-00000180: 6669 6572 7320 3d20 0d0a 0950 726f 6772  fiers = ...Progr
-00000190: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001a0: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
-000001b0: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
-000001c0: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
-000001d0: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
-000001e0: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
-000001f0: 2049 6e64 6570 656e 6465 6e74 0d0a 0d0a   Independent....
-00000200: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
-00000210: 6765 5f64 6972 203d 200d 0a09 3d20 7372  ge_dir = ...= sr
-00000220: 630d 0a70 6163 6b61 6765 7320 3d20 6669  c..packages = fi
-00000230: 6e64 3a0d 0a70 7974 686f 6e5f 7265 7175  nd:..python_requ
-00000240: 6972 6573 203d 203e 3d33 2e36 0d0a 0d0a  ires = >=3.6....
-00000250: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000260: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
-00000270: 2073 7263 0d0a 0d0a 5b65 6767 5f69 6e66   src....[egg_inf
-00000280: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000290: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-000002a0: 0d0a                                     ..
+00000170: 522f 5079 4d4c 5253 270d 0a63 6c61 7373  R/PyMLRS'..class
+00000180: 6966 6965 7273 203d 200d 0a09 5072 6f67  ifiers = ...Prog
+00000190: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000001a0: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
+000001b0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
+000001c0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
+000001d0: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
+000001e0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
+000001f0: 5320 496e 6465 7065 6e64 656e 740d 0a0d  S Independent...
+00000200: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
+00000210: 6167 655f 6469 7220 3d20 0d0a 093d 2073  age_dir = ...= s
+00000220: 7263 0d0a 7061 636b 6167 6573 203d 2066  rc..packages = f
+00000230: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
+00000240: 7569 7265 7320 3d20 3e3d 332e 360d 0a0d  uires = >=3.6...
+00000250: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+00000260: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
+00000270: 3d20 7372 630d 0a0d 0a5b 6567 675f 696e  = src....[egg_in
+00000280: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+00000290: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+000002a0: 0a0d 0a                                  ...
```

### Comparing `PyMLRS-0.0.1/setup.py` & `pymlrs-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 rd_file = os.path.join(dir_path, 'README.md')
 
 with io.open(rd_file, encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='PyMLRS',
-    version='0.0.1',
+    version='0.0.2',
     description='A library for processing and interpreting DNA high-resolution melt and amplification curves for the meningoencephalitis panel.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/PyPCR/PyPCR',
+    url='https://github.com/PyPCR/PyMLRS',
     authors=["ChandruGaneshan", "VikramSekar"],
     authors_email=['chandruganeshan24@gmail.com', 'vikramsekar2305@gmail.com'],
     license='MIT',
     keywords=['High Resolution Melt', 'Amplification Curve', "Cycle threshold",
               'PCR', 'rt-PCR', 'Meningoencephalitis', "MEP", 'Pathogens', "Bharathiar University"],
     packages=find_packages(where='src'),
     package_dir={"": "src"},
```

### Comparing `PyMLRS-0.0.1/src/PyMLRS/Mep_panel.py` & `pymlrs-0.0.2/src/PyMLRS/Mep_panel.py`

 * *Files identical despite different names*

### Comparing `PyMLRS-0.0.1/src/PyMLRS/Rextractor.py` & `pymlrs-0.0.2/src/PyMLRS/Rextractor.py`

 * *Files identical despite different names*

### Comparing `PyMLRS-0.0.1/src/PyMLRS/Threshold.xlsx` & `pymlrs-0.0.2/src/PyMLRS/Threshold.xlsx`

 * *Files identical despite different names*

### Comparing `PyMLRS-0.0.1/src/PyMLRS/model.pkl` & `pymlrs-0.0.2/src/PyMLRS/model.pkl`

 * *Files identical despite different names*

### Comparing `PyMLRS-0.0.1/src/PyMLRS.egg-info/PKG-INFO` & `pymlrs-0.0.2/src/PyMLRS.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: PyMLRS
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for processing and interpreting DNA high-resolution melt and amplification curves for the meningoencephalitis panel.
-Home-page: https://github.com/PyPCR/PyPCR
+Home-page: https://github.com/PyPCR/PyMLRS
 Author: Chandru, Vikram
 Author-email: mlrs.project2024@gmail.com
 License: MIT
 Keywords: High Resolution Melt,Amplification Curve,Cycle threshold,PCR,rt-PCR,Meningoencephalitis,MEP,Pathogens,Bharathiar University
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,16 @@
 Requires-Dist: pandas==1.5.3
 Requires-Dist: Pillow==9.4.0
 Requires-Dist: plotly==5.13.1
 Requires-Dist: scikit_learn==1.4.1.post1
 Requires-Dist: scipy==1.13.0
 Requires-Dist: openpyxl==3.1.2
 
+![vikramAsset 2@4x](https://github.com/Vikram2305/gitcheck/assets/124907782/43ad9d19-dca3-4505-9c59-4a2dfa6cb08a)
+
 <div align="center">
     <br>
         <a href="" width="250px" height="250px" alt="pyHRM"></a>
       <br>
     <h1>PyMLRS</h1>
     <h2><b>A Python library for processing and interpreting DNA High-Resolution Melt and Amplification Curves for the Meningoencephalitis Panel</b></h2>
         <h4>
@@ -290,19 +292,17 @@
 ```
 from PyMLRS.Rextractor import rex_reader
 from PyMLRS.Mep_panel import Mep_diagnoser
 
 # File extraction from the rex file
 patient_id,hrm,ct = rex_reader("Your .rex file path")
 
-# Create Object
-md = Mep_diagnoser()
-
 # Interpreting the results
 for id in patient_id:
+    md = Mep_diagnoser()
     hrm_data = md.transform_hrm(hrm[id])
     ct_data = md.transform_ct(ct[id])
     melt = md.hrm_to_melt(figure = False)
     hrm_features = md.hrm_feature_extraction()
     ct_values = md.ct_value()
     result = md.predict_result()
     report = md.report( output_fie_path=f"{id}.pdf",patient_id=id)
@@ -321,9 +321,7 @@
     <tr>
       <td align='center' valign='top'><a href="https://github.com/chandru-g24"> <img src="https://avatars.githubusercontent.com/u/111188572?s=400&u=befb7d97d2b8419a715a22b09d92f825bdc33906&v=4" width = '60px;' alt='Chandru G'/> <br /> <sub><b><a href="https://www.linkedin.com/in/chandru-g24/"> Chandru Ganeshan</a></b></sub></a><br /></td>
       <td align='center' valign='top'><a href="https://github.com/Vikram2305"> <img src="https://avatars.githubusercontent.com/u/124907782?s=400&u=a5d9c4ca9f08e5bb5e88bc4d049d5e80703d1c89&v=4" width = '60px;' alt='Vikram S'/> <br /> <sub><b><a href="https://www.linkedin.com/in/vikram-sekar/"> Vikram Sekar</a></b></sub></a><br /></td>
     </tr>
   </tbody>
   
 </table>
-
-
```

#### html2text {}

```diff
@@ -1,20 +1,22 @@
-Metadata-Version: 2.1 Name: PyMLRS Version: 0.0.1 Summary: A library for
+Metadata-Version: 2.1 Name: PyMLRS Version: 0.0.2 Summary: A library for
 processing and interpreting DNA high-resolution melt and amplification curves
-for the meningoencephalitis panel. Home-page: https://github.com/PyPCR/PyPCR
+for the meningoencephalitis panel. Home-page: https://github.com/PyPCR/PyMLRS
 Author: Chandru, Vikram Author-email: mlrs.project2024@gmail.com License: MIT
 Keywords: High Resolution Melt,Amplification Curve,Cycle threshold,PCR,rt-
 PCR,Meningoencephalitis,MEP,Pathogens,Bharathiar University Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENCE.txt Requires-
 Dist: fpdf==1.7.2 Requires-Dist: matplotlib==3.6.3 Requires-Dist: numpy==1.23.5
 Requires-Dist: pandas==1.5.3 Requires-Dist: Pillow==9.4.0 Requires-Dist:
 plotly==5.13.1 Requires-Dist: scikit_learn==1.4.1.post1 Requires-Dist:
-scipy==1.13.0 Requires-Dist: openpyxl==3.1.2
+scipy==1.13.0 Requires-Dist: openpyxl==3.1.2 ![vikramAsset 2@4x](https://
+github.com/Vikram2305/gitcheck/assets/124907782/43ad9d19-dca3-4505-9c59-
+4a2dfa6cb08a)
 
 
                              ************ PPyyMMLLRRSS ************
 ********** AA PPyytthhoonn lliibbrraarryy ffoorr pprroocceessssiinngg aanndd iinntteerrpprreettiinngg DDNNAA HHiigghh--RReessoolluuttiioonn MMeelltt
        aanndd AAmmpplliiffiiccaattiioonn CCuurrvveess ffoorr tthhee MMeenniinnggooeenncceepphhaalliittiiss PPaanneell **********
          ****** _II_nn_ss_tt_aa_ll_ll_aa_tt_ii_oo_nn ?â??¢ _FF_ee_aa_tt_uu_rr_ee_ss ?â??¢ _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ?â??¢ _HH_ee_ll_pp ******
 # PyMLRS
@@ -134,21 +136,21 @@
 Interpreting the results by providing patient ID manually hrm_data =
 md.transform_hrm(hrm[id]) ct_data = md.transform_ct(ct[id]) melt =
 md.hrm_to_melt(figure = False) hrm_features = md.hrm_feature_extraction()
 ct_values = md.ct_value() result = md.predict_result() report = md.report
 ( output_fie_path=f"{id}.pdf",patient_id=id) ``` ### Sample code Snippet for
 interpreting all individual result ``` from PyMLRS.Rextractor import rex_reader
 from PyMLRS.Mep_panel import Mep_diagnoser # File extraction from the rex file
-patient_id,hrm,ct = rex_reader("Your .rex file path") # Create Object md =
-Mep_diagnoser() # Interpreting the results for id in patient_id: hrm_data =
-md.transform_hrm(hrm[id]) ct_data = md.transform_ct(ct[id]) melt =
-md.hrm_to_melt(figure = False) hrm_features = md.hrm_feature_extraction()
-ct_values = md.ct_value() result = md.predict_result() report = md.report
-( output_fie_path=f"{id}.pdf",patient_id=id) ``` # Getting Help If you need to
-get in touch with the team, please contact through email address:
+patient_id,hrm,ct = rex_reader("Your .rex file path") # Interpreting the
+results for id in patient_id: md = Mep_diagnoser() hrm_data = md.transform_hrm
+(hrm[id]) ct_data = md.transform_ct(ct[id]) melt = md.hrm_to_melt(figure =
+False) hrm_features = md.hrm_feature_extraction() ct_values = md.ct_value()
+result = md.predict_result() report = md.report( output_fie_path=f"
+{id}.pdf",patient_id=id) ``` # Getting Help If you need to get in touch with
+the team, please contact through email address:
 [chandruganeshan24@gmail.com](mailto:chandruganeshan24@gmail.com)
 [vikramsekar2305@gmail.com](mailto:vikramsekar2305@gmail.com) # Developers The
 developer of this Software are M.Sc Data Analytics Students in Department of
 Computer Application at [Bharathiar University](https://b-u.ac.in/23/
 department-computer-applications)
   _[_C_h_a_n_d_r_u_ _G_]     _[_V_i_k_r_a_m_ _S_]
 _CC_hh_aa_nn_dd_rr_uu_ _GG_aa_nn_ee_ss_hh_aa_nn _VV_ii_kk_rr_aa_mm_ _SS_ee_kk_aa_rr
```

