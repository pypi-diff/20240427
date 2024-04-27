# Comparing `tmp/google-api-support-0.1.4.tar.gz` & `tmp/google_api_support-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-api-support-0.1.4.tar", last modified: Fri Sep  1 20:01:41 2023, max compression
+gzip compressed data, was "google_api_support-0.1.7.tar", last modified: Sat Apr 27 08:03:25 2024, max compression
```

## Comparing `google-api-support-0.1.4.tar` & `google_api_support-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 20:01:41.246527 google-api-support-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 20:01:41.242527 google-api-support-0.1.4/GoogleApiSupport/
--rw-r--r--   0 runner    (1001) docker     (999)       27 2023-09-01 20:01:29.000000 google-api-support-0.1.4/GoogleApiSupport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      808 2023-09-01 20:01:29.000000 google-api-support-0.1.4/GoogleApiSupport/apis.py
--rw-r--r--   0 runner    (1001) docker     (999)     8116 2023-09-01 20:01:29.000000 google-api-support-0.1.4/GoogleApiSupport/auth.py
--rw-r--r--   0 runner    (1001) docker     (999)    11863 2023-09-01 20:01:29.000000 google-api-support-0.1.4/GoogleApiSupport/drive.py
--rw-r--r--   0 runner    (1001) docker     (999)     8581 2023-09-01 20:01:29.000000 google-api-support-0.1.4/GoogleApiSupport/sheets.py
--rw-r--r--   0 runner    (1001) docker     (999)    12262 2023-09-01 20:01:29.000000 google-api-support-0.1.4/GoogleApiSupport/slides.py
--rw-r--r--   0 runner    (1001) docker     (999)    10203 2023-09-01 20:01:29.000000 google-api-support-0.1.4/GoogleApiSupport/spreadsheets.py
--rw-r--r--   0 runner    (1001) docker     (999)     1007 2023-09-01 20:01:29.000000 google-api-support-0.1.4/GoogleApiSupport/storage.py
--rw-r--r--   0 runner    (1001) docker     (999)     1210 2023-09-01 20:01:29.000000 google-api-support-0.1.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (999)     3737 2023-09-01 20:01:41.242527 google-api-support-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     3236 2023-09-01 20:01:29.000000 google-api-support-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 20:01:41.242527 google-api-support-0.1.4/google_api_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     3737 2023-09-01 20:01:41.000000 google-api-support-0.1.4/google_api_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      501 2023-09-01 20:01:41.000000 google-api-support-0.1.4/google_api_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-01 20:01:41.000000 google-api-support-0.1.4/google_api_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)      108 2023-09-01 20:01:41.000000 google-api-support-0.1.4/google_api_support.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       22 2023-09-01 20:01:41.000000 google-api-support-0.1.4/google_api_support.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-01 20:01:41.246527 google-api-support-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)      928 2023-09-01 20:01:29.000000 google-api-support-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 20:01:41.242527 google-api-support-0.1.4/test/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-01 20:01:29.000000 google-api-support-0.1.4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1969 2023-09-01 20:01:29.000000 google-api-support-0.1.4/test/test_spreadsheets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:03:25.780400 google_api_support-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:03:25.776400 google_api_support-0.1.7/GoogleApiSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-27 08:03:21.000000 google_api_support-0.1.7/GoogleApiSupport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-27 08:03:21.000000 google_api_support-0.1.7/GoogleApiSupport/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-04-27 08:03:21.000000 google_api_support-0.1.7/GoogleApiSupport/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-04-27 08:03:21.000000 google_api_support-0.1.7/GoogleApiSupport/drive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-04-27 08:03:21.000000 google_api_support-0.1.7/GoogleApiSupport/sheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12479 2024-04-27 08:03:21.000000 google_api_support-0.1.7/GoogleApiSupport/slides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-27 08:03:21.000000 google_api_support-0.1.7/GoogleApiSupport/spreadsheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-27 08:03:21.000000 google_api_support-0.1.7/GoogleApiSupport/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-27 08:03:21.000000 google_api_support-0.1.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-27 08:03:25.780400 google_api_support-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-27 08:03:21.000000 google_api_support-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:03:25.776400 google_api_support-0.1.7/google_api_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-27 08:03:25.000000 google_api_support-0.1.7/google_api_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-27 08:03:25.000000 google_api_support-0.1.7/google_api_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 08:03:25.000000 google_api_support-0.1.7/google_api_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-27 08:03:25.000000 google_api_support-0.1.7/google_api_support.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 08:03:25.000000 google_api_support-0.1.7/google_api_support.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 08:03:25.780400 google_api_support-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-27 08:03:21.000000 google_api_support-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:03:25.776400 google_api_support-0.1.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 08:03:21.000000 google_api_support-0.1.7/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-27 08:03:21.000000 google_api_support-0.1.7/test/test_spreadsheets.py
```

### Comparing `google-api-support-0.1.4/GoogleApiSupport/apis.py` & `google_api_support-0.1.7/GoogleApiSupport/apis.py`

 * *Files identical despite different names*

### Comparing `google-api-support-0.1.4/GoogleApiSupport/auth.py` & `google_api_support-0.1.7/GoogleApiSupport/auth.py`

 * *Files identical despite different names*

### Comparing `google-api-support-0.1.4/GoogleApiSupport/drive.py` & `google_api_support-0.1.7/GoogleApiSupport/drive.py`

 * *Files identical despite different names*

### Comparing `google-api-support-0.1.4/GoogleApiSupport/sheets.py` & `google_api_support-0.1.7/GoogleApiSupport/sheets.py`

 * *Files identical despite different names*

### Comparing `google-api-support-0.1.4/GoogleApiSupport/slides.py` & `google_api_support-0.1.7/GoogleApiSupport/slides.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,22 @@
                     if 'textRun' in line:
                         output += [line['textRun']['content']]
         return ''.join(output)
     except Exception as e:
         return '# Error in slide' + str(e)
 
 
+def get_presentation_notes(presentation_id):
+    notes = {}
+    slides = get_presentation_slides(presentation_id)
+    for slide in slides:
+        notes[slide['objectId']] = get_slide_notes(slide)
+    return notes
+
+
 def execute_batch_update(requests, presentation_id, additional_apis=[]):
     body = {
         'requests': requests
     }
     
     service = auth.get_service("slides", additional_apis=additional_apis)
     
@@ -373,16 +381,16 @@
         for page_element in slide['pageElements']:
             if page_element['objectId'] == element_id:
                 return page_element
             
 def get_page(presentation_id, page_id):
     presentation = get_presentation_info(presentation_id)
     for slide in presentation['slides']:
-        if slide['objectID'] == page_id:
-            return page
+        if slide['objectId'] == page_id:
+            return slide
 
 
 def replace_shape_with_chart(presentation_id: str, placeholder_text, spreadsheet_id, chart_id, linking_mode='NOT_LINKED_IMAGE', target_id_pages=[]):
     requests = []
       
     requests.append(
         {
```

### Comparing `google-api-support-0.1.4/GoogleApiSupport/spreadsheets.py` & `google_api_support-0.1.7/GoogleApiSupport/spreadsheets.py`

 * *Files identical despite different names*

### Comparing `google-api-support-0.1.4/GoogleApiSupport/storage.py` & `google_api_support-0.1.7/GoogleApiSupport/storage.py`

 * *Files identical despite different names*

### Comparing `google-api-support-0.1.4/LICENSE.md` & `google_api_support-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `google-api-support-0.1.4/PKG-INFO` & `google_api_support-0.1.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,234 +1,206 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 676f 6f67  : 2.1.Name: goog
-00000020: 6c65 2d61 7069 2d73 7570 706f 7274 0a56  le-api-support.V
-00000030: 6572 7369 6f6e 3a20 302e 312e 340a 5375  ersion: 0.1.4.Su
-00000040: 6d6d 6172 793a 2049 6e20 7468 6973 2070  mmary: In this p
-00000050: 6163 6b61 6765 2079 6f75 2077 696c 6c20  ackage you will 
-00000060: 6669 6e64 2066 756e 6374 696f 6e73 2074  find functions t
-00000070: 6f20 6465 616c 2077 6974 6820 676f 6f67  o deal with goog
-00000080: 6c65 2061 7069 732e 2053 6865 6574 732c  le apis. Sheets,
-00000090: 2044 7269 7665 2c20 5374 6f72 6167 6520   Drive, Storage 
-000000a0: 616e 6420 536c 6964 6573 0a48 6f6d 652d  and Slides.Home-
-000000b0: 7061 6765 3a20 6874 7470 733a 2f2f 6769  page: https://gi
-000000c0: 7468 7562 2e63 6f6d 2f76 7065 7265 7a62  thub.com/vperezb
-000000d0: 2f67 6f6f 676c 652d 6170 692d 7375 7070  /google-api-supp
-000000e0: 6f72 740a 4175 7468 6f72 3a20 56c3 ad63  ort.Author: V..c
-000000f0: 746f 7220 50c3 a972 657a 2042 6572 7275  tor P..rez Berru
-00000100: 657a 6f0a 4175 7468 6f72 2d65 6d61 696c  ezo.Author-email
-00000110: 3a20 7669 6374 6f72 2e70 6572 657a 2e62  : victor.perez.b
-00000120: 6572 7275 657a 6f40 676d 6169 6c2e 636f  erruezo@gmail.co
-00000130: 6d0a 436c 6173 7369 6669 6572 3a20 5072  m.Classifier: Pr
-00000140: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000150: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000160: 330a 436c 6173 7369 6669 6572 3a20 4c69  3.Classifier: Li
-00000170: 6365 6e73 6520 3a3a 2050 7562 6c69 6320  cense :: Public 
-00000180: 446f 6d61 696e 0a43 6c61 7373 6966 6965  Domain.Classifie
-00000190: 723a 2044 6576 656c 6f70 6d65 6e74 2053  r: Development S
-000001a0: 7461 7475 7320 3a3a 2033 202d 2041 6c70  tatus :: 3 - Alp
-000001b0: 6861 0a44 6573 6372 6970 7469 6f6e 2d43  ha.Description-C
-000001c0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-000001d0: 742f 6d61 726b 646f 776e 0a4c 6963 656e  t/markdown.Licen
-000001e0: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-000001f0: 2e6d 640a 0a23 2067 6f6f 676c 652d 6170  .md..# google-ap
-00000200: 692d 7375 7070 6f72 740a 0a53 6f6d 6520  i-support..Some 
-00000210: 6675 6e63 7469 6f6e 7320 746f 206d 616b  functions to mak
-00000220: 6520 476f 6f67 6c65 2041 5049 7320 6d6f  e Google APIs mo
-00000230: 7265 2075 7361 626c 652e 0a0a 2323 2049  re usable...## I
-00000240: 6e73 7461 6c6c 0a0a 6070 6970 2069 6e73  nstall..`pip ins
-00000250: 7461 6c6c 2067 6f6f 676c 652d 6170 692d  tall google-api-
-00000260: 7375 7070 6f72 7460 0a0a 2323 2043 6f6e  support`..## Con
-00000270: 7472 6962 7574 650a 0a54 6865 2063 6f6e  tribute..The con
-00000280: 7472 6962 7574 696f 6e73 2061 7265 2065  tributions are e
-00000290: 6e63 6f75 7261 6765 6420 736f 2074 6865  ncouraged so the
-000002a0: 206c 6962 7261 7279 2063 616e 206b 6565   library can kee
-000002b0: 7020 6772 6f77 696e 6720 616e 6420 6865  p growing and he
-000002c0: 6c70 206d 6f72 6520 7065 6f70 6c65 2e0a  lp more people..
-000002d0: 0a59 6f75 2063 616e 2061 6c73 6f20 6372  .You can also cr
-000002e0: 6561 7465 2061 6e20 6973 7375 6520 696e  eate an issue in
-000002f0: 206f 7264 6572 2074 6f20 706f 696e 7420   order to point 
-00000300: 6f74 6865 7220 636f 6e74 7269 6275 746f  other contributo
-00000310: 7273 2074 6f20 6465 7369 7265 6420 6675  rs to desired fu
-00000320: 6e63 7469 6f6e 616c 6974 6965 732e 0a0a  nctionalities...
-00000330: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000340: 3a2f 2f64 6973 636f 7264 2e67 672f 5a42  ://discord.gg/ZB
-00000350: 7951 736d 7852 2220 7461 7267 6574 3d22  yQsmxR" target="
-00000360: 5f62 6c61 6e6b 223e 0a20 2020 203c 696d  _blank">.    <im
-00000370: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
-00000380: 6d67 2e73 6869 656c 6473 2e69 6f2f 6469  mg.shields.io/di
-00000390: 7363 6f72 642f 3330 3833 3233 3035 3635  scord/3083230565
-000003a0: 3932 3438 3634 3230 3f6c 6f67 6f3d 6469  92486420?logo=di
-000003b0: 7363 6f72 6422 2061 6c74 3d22 4469 7363  scord" alt="Disc
-000003c0: 6f72 6420 4368 6174 2220 2f3e 0a20 203c  ord Chat" />.  <
-000003d0: 2f61 3e0a 0a23 2320 4675 6e63 7469 6f6e  /a>..## Function
-000003e0: 7320 6176 616c 6961 626c 650a 0a2a 2053  s avaliable..* S
-000003f0: 6865 6574 730a 2020 2a20 4765 7420 7061  heets.  * Get pa
-00000400: 6e64 6173 2e64 6174 6166 7261 6d65 2066  ndas.dataframe f
-00000410: 726f 6d20 5368 6565 7473 0a20 202a 2055  rom Sheets.  * U
-00000420: 706c 6f61 6420 7061 6e64 6173 2e64 6174  pload pandas.dat
-00000430: 6166 7261 6d65 2074 6f20 5368 6565 7473  aframe to Sheets
-00000440: 0a20 202a 2052 6574 7269 6576 6520 7368  .  * Retrieve sh
-00000450: 6565 7420 6e61 6d65 730a 2020 2a20 4164  eet names.  * Ad
-00000460: 6420 7368 6565 7473 2074 6f20 6120 7370  d sheets to a sp
-00000470: 7265 6164 7368 6565 740a 2020 2a20 4372  readsheet.  * Cr
-00000480: 6561 7465 206e 6577 2073 7072 6561 6473  eate new spreads
-00000490: 6865 6574 0a2a 2053 6c69 6465 730a 2020  heet.* Slides.  
-000004a0: 2a20 4372 6561 7465 2070 7265 7365 6e74  * Create present
-000004b0: 6174 696f 6e0a 2020 2a20 4765 7420 7072  ation.  * Get pr
-000004c0: 6573 656e 7461 7469 6f6e 2069 6e66 6f0a  esentation info.
-000004d0: 2020 2a20 4765 7420 7072 6573 656e 7461    * Get presenta
-000004e0: 7469 6f6e 2073 6c69 6465 730a 2020 2a20  tion slides.  * 
-000004f0: 4765 7420 736c 6964 6520 6e6f 7465 730a  Get slide notes.
-00000500: 2020 2a20 5265 706c 6163 6520 7465 7874    * Replace text
-00000510: 0a20 202a 2052 6570 6c61 6365 2073 6861  .  * Replace sha
-00000520: 7065 2077 6974 6820 696d 6167 650a 2020  pe with image.  
-00000530: 2a20 5265 706c 6163 6520 696d 6167 650a  * Replace image.
-00000540: 2020 2a20 4765 7420 736c 6964 6520 6e6f    * Get slide no
-00000550: 7465 730a 2020 2a20 4261 7463 6820 7265  tes.  * Batch re
-00000560: 706c 6163 6520 7465 7874 0a20 202a 2042  place text.  * B
-00000570: 6174 6368 2072 6570 6c61 6365 2073 6861  atch replace sha
-00000580: 7065 7320 7769 7468 2069 6d61 6765 730a  pes with images.
-00000590: 2020 2a20 496e 7365 7274 2069 6d61 6765    * Insert image
-000005a0: 0a20 202a 2044 7570 6c69 6361 7465 206f  .  * Duplicate o
-000005b0: 626a 6563 740a 2020 2a20 4465 6c65 7465  bject.  * Delete
-000005c0: 206f 626a 6563 740a 2020 2a20 4261 7463   object.  * Batc
-000005d0: 6820 6465 6c65 7465 206f 626a 6563 740a  h delete object.
-000005e0: 2020 2a20 4465 6c65 7465 2074 6578 740a    * Delete text.
-000005f0: 2020 2a20 4261 7463 6820 6465 6c65 7465    * Batch delete
-00000600: 2074 6578 740a 2020 2a20 4465 6c65 7465   text.  * Delete
-00000610: 2070 7265 7365 6e74 6174 696f 6e20 6e6f   presentation no
-00000620: 7465 730a 2020 2a20 5472 616e 7366 6f72  tes.  * Transfor
-00000630: 6d20 6f62 6a65 6374 0a2a 2044 7269 7665  m object.* Drive
-00000640: 0a20 202a 2047 6574 2066 696c 6520 6e61  .  * Get file na
-00000650: 6d65 0a20 202a 204d 6f76 6520 6669 6c65  me.  * Move file
-00000660: 0a20 202a 2044 656c 6574 6520 6669 6c65  .  * Delete file
-00000670: 0a20 202a 2043 6f70 7920 6669 6c65 0a20  .  * Copy file. 
-00000680: 202a 2055 706c 6f61 6420 696d 6167 650a   * Upload image.
-00000690: 2020 2a20 4372 6561 7465 2066 6f6c 6465    * Create folde
-000006a0: 720a 2020 2a20 4c69 7374 2066 6f6c 6465  r.  * List folde
-000006b0: 7273 2069 6e20 666f 6c64 6572 0a20 202a  rs in folder.  *
-000006c0: 2047 6574 2066 6f6c 6465 7220 6964 2062   Get folder id b
-000006d0: 7920 6e61 6d65 0a20 202a 2047 6574 2066  y name.  * Get f
-000006e0: 6f6c 6465 7220 6964 2062 7920 7061 7468  older id by path
-000006f0: 0a20 202a 2044 6f77 6e6c 6f61 6420 6669  .  * Download fi
-00000700: 6c65 0a0a 2a20 5374 6f72 6167 650a 2020  le..* Storage.  
-00000710: 2a20 5570 6c6f 6164 2061 2066 696c 6520  * Upload a file 
-00000720: 746f 2067 6f6f 676c 6520 7374 6f72 6167  to google storag
-00000730: 6520 616e 6420 6765 7420 6974 7320 5552  e and get its UR
-00000740: 4c0a 0a23 2320 5374 6570 7320 746f 2075  L..## Steps to u
-00000750: 7365 2067 6f6f 676c 6520 5368 6565 7473  se google Sheets
-00000760: 2041 5049 0a0a 496e 206f 7264 6572 2074   API..In order t
-00000770: 6f20 7573 6520 476f 6f67 6c65 2041 5049  o use Google API
-00000780: 7320 796f 7520 7769 6c6c 206e 6565 6420  s you will need 
-00000790: 746f 2061 7574 6865 6e74 6963 6174 652c  to authenticate,
-000007a0: 2074 6869 7320 7374 6570 7320 6775 6964   this steps guid
-000007b0: 6520 796f 7520 7468 726f 7567 6820 7468  e you through th
-000007c0: 6520 7072 6f63 6573 733a 0a0a 302e 2043  e process:..0. C
-000007d0: 7265 6174 6520 6120 7072 6f6a 6563 7420  reate a project 
-000007e0: 696e 2063 6f6e 736f 6c65 2e64 6576 656c  in console.devel
-000007f0: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
-00000800: 0a0a 3c68 7474 7073 3a2f 2f63 6f6e 736f  ..<https://conso
-00000810: 6c65 2e64 6576 656c 6f70 6572 732e 676f  le.developers.go
-00000820: 6f67 6c65 2e63 6f6d 3e0a 0a30 2e20 4372  ogle.com>..0. Cr
-00000830: 6561 7465 2067 6f6f 676c 6520 7365 7276  eate google serv
-00000840: 6963 6520 6163 636f 756e 742e 0a20 2020  ice account..   
-00000850: 2030 2e20 476f 2074 6f20 3c68 7474 7073   0. Go to <https
-00000860: 3a2f 2f63 6f6e 736f 6c65 2e64 6576 656c  ://console.devel
-00000870: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
-00000880: 2f70 726f 6a65 6374 7365 6c65 6374 6f72  /projectselector
-00000890: 2f61 7069 732f 6372 6564 656e 7469 616c  /apis/credential
-000008a0: 733e 2061 6e64 2063 7265 6174 6520 6120  s> and create a 
-000008b0: 6e65 7720 7072 6f6a 6563 742e 0a20 2020  new project..   
-000008c0: 2021 5b43 7265 6174 6520 6120 6465 7665   ![Create a deve
-000008d0: 6c6f 7065 7273 2070 726f 6a65 6374 5d28  lopers project](
-000008e0: 646f 6373 2f69 6d67 2f63 7265 6174 655f  docs/img/create_
-000008f0: 7072 6f6a 6563 742e 504e 4729 0a0a 2020  project.PNG)..  
-00000900: 2020 302e 2043 7265 6174 6520 6372 6564    0. Create cred
-00000910: 656e 7469 616c 732e 0a20 2020 2021 5b5d  entials..    ![]
-00000920: 2864 6f63 732f 696d 672f 6368 6f6f 7365  (docs/img/choose
-00000930: 5f63 7265 6465 6e74 6961 6c73 2e50 4e47  _credentials.PNG
-00000940: 290a 2020 2020 2020 2020 2a20 496e 2074  ).        * In t
-00000950: 6869 7320 6669 7273 7420 7665 7273 696f  his first versio
-00000960: 6e2c 2069 2077 696c 6c20 6578 706c 6169  n, i will explai
-00000970: 6e20 686f 7720 746f 2064 6561 6c20 7769  n how to deal wi
-00000980: 7468 2053 6572 7669 6365 7320 6163 636f  th Services acco
-00000990: 756e 7473 2c20 736f 2073 656c 6563 7420  unts, so select 
-000009a0: 2253 6572 7669 6365 2061 6363 6f75 6e74  "Service account
-000009b0: 206b 6579 222e 0a0a 2020 2020 302e 2043   key"...    0. C
-000009c0: 7265 6174 6520 6120 7365 7276 6963 6520  reate a service 
-000009d0: 6163 636f 756e 742e 0a20 2020 2021 5b5d  account..    ![]
-000009e0: 2864 6f63 732f 696d 672f 6372 6561 7465  (docs/img/create
-000009f0: 5f73 6572 7669 6365 5f61 6363 6f75 6e74  _service_account
-00000a00: 2e50 4e47 290a 2020 2020 2020 2020 2a20  .PNG).        * 
-00000a10: 446f 776e 6c6f 6164 2074 6865 202e 6a73  Download the .js
-00000a20: 6f6e 2066 696c 6520 616e 6420 4b45 4550  on file and KEEP
-00000a30: 2049 5420 5341 4645 2e0a 0a20 2020 2030   IT SAFE...    0
-00000a40: 2e20 4e6f 7720 796f 7520 6861 7665 2079  . Now you have y
-00000a50: 6f75 7220 7365 7276 6963 6520 6163 636f  our service acco
-00000a60: 756e 7420 6372 6561 7465 6420 696e 7369  unt created insi
-00000a70: 6465 2079 6f75 7220 6e65 7720 7072 6f6a  de your new proj
-00000a80: 6563 742e 0a20 2020 2021 5b5d 2864 6f63  ect..    ![](doc
-00000a90: 732f 696d 672f 6372 6561 7465 5f73 6572  s/img/create_ser
-00000aa0: 7669 6365 5f61 6363 6f75 6e74 2e50 4e47  vice_account.PNG
-00000ab0: 290a 0a20 2020 2030 2e20 436f 7079 2079  )..    0. Copy y
-00000ac0: 6f75 7220 2275 7365 7220 6964 2220 696e  our "user id" in
-00000ad0: 2022 4d61 6e61 6765 2073 6572 7669 6365   "Manage service
-00000ae0: 2061 6363 6f75 6e74 7322 2074 6f20 7573   accounts" to us
-00000af0: 6520 6974 206c 6174 6572 2e0a 2020 2020  e it later..    
-00000b00: 2020 2020 2a20 4974 206c 6f6f 6b73 206c      * It looks l
-00000b10: 696b 6520 7468 6973 206f 6e65 3a20 6066  ike this one: `f
-00000b20: 6972 7374 2d73 6572 7669 6365 2d61 6363  irst-service-acc
-00000b30: 6f75 6e74 4065 7861 6d70 6c65 2d69 642d  ount@example-id-
-00000b40: 3137 3538 3230 2e69 616d 2e67 7365 7276  175820.iam.gserv
-00000b50: 6963 6561 6363 6f75 6e74 2e63 6f6d 600a  iceaccount.com`.
-00000b60: 0a20 2020 2030 2e20 476f 2074 6f20 796f  .    0. Go to yo
-00000b70: 7572 2064 6173 6862 6f61 7264 2073 6372  ur dashboard scr
-00000b80: 6565 6e20 616e 6420 676f 2074 6f20 2245  een and go to "E
-00000b90: 4e41 424c 4520 4150 4953 2041 4e44 2053  NABLE APIS AND S
-00000ba0: 4552 5649 4345 5322 2074 6f20 2275 6e6c  ERVICES" to "unl
-00000bb0: 6f63 6b22 2074 6865 2064 6573 6972 6564  ock" the desired
-00000bc0: 2041 5049 2063 616c 6c73 2e0a 2020 2020   API calls..    
-00000bd0: 496e 206f 7572 2065 7861 6d70 6c65 2c20  In our example, 
-00000be0: 7765 2077 696c 6c20 6a75 7374 2065 6e61  we will just ena
-00000bf0: 626c 6520 2247 6f6f 676c 6520 7368 6565  ble "Google shee
-00000c00: 7473 2041 5049 222e 0a20 2020 2021 5b5d  ts API"..    ![]
-00000c10: 2864 6f63 732f 696d 672f 656e 6162 6c65  (docs/img/enable
-00000c20: 5f61 7069 732e 504e 4729 0a20 2020 2021  _apis.PNG).    !
-00000c30: 5b5d 2864 6f63 732f 696d 672f 6163 7469  [](docs/img/acti
-00000c40: 7661 7465 5f73 6865 6574 732e 504e 4729  vate_sheets.PNG)
-00000c50: 0a0a 2323 2043 6865 636b 2074 6865 2073  ..## Check the s
-00000c60: 7065 6369 6669 6320 6372 6564 656e 7469  pecific credenti
-00000c70: 616c 7320 646f 6375 6d65 6e74 6174 696f  als documentatio
-00000c80: 6e20 6669 6c65 0a0a 5b43 7265 6465 6e74  n file..[Credent
-00000c90: 6961 6c73 2064 6f63 756d 656e 7461 7469  ials documentati
-00000ca0: 6f6e 5d28 2f64 6f63 732f 7365 7475 705f  on](/docs/setup_
-00000cb0: 6372 6564 656e 7469 616c 732e 6d64 290a  credentials.md).
-00000cc0: 0a23 2320 4d61 6e75 616c 6c79 2069 6e73  .## Manually ins
-00000cd0: 7461 6c6c 2064 6570 656e 6465 6e63 6965  tall dependencie
-00000ce0: 730a 0a60 7069 7020 696e 7374 616c 6c20  s..`pip install 
-00000cf0: 6874 7470 6c69 6232 206f 6175 7468 3263  httplib2 oauth2c
-00000d00: 6c69 656e 7420 7061 6e64 6173 2067 6f6f  lient pandas goo
-00000d10: 676c 652d 6170 692d 7079 7468 6f6e 2d63  gle-api-python-c
-00000d20: 6c69 656e 7420 676f 6f67 6c65 2e61 7574  lient google.aut
-00000d30: 682e 7472 616e 7370 6f72 742e 7265 7175  h.transport.requ
-00000d40: 6573 7473 2067 6f6f 676c 652e 6f61 7574  ests google.oaut
-00000d50: 6832 2e63 7265 6465 6e74 6961 6c73 2067  h2.credentials g
-00000d60: 6f6f 676c 655f 6175 7468 5f6f 6175 7468  oogle_auth_oauth
-00000d70: 6c69 622e 666c 6f77 600a 0a23 2320 436f  lib.flow`..## Co
-00000d80: 6d70 6c65 7465 2066 6972 7374 2075 7365  mplete first use
-00000d90: 2065 7861 6d70 6c65 0a0a 2323 2320 4578   example..### Ex
-00000da0: 616d 706c 6520 7573 696e 6720 7669 7274  ample using virt
-00000db0: 7561 6c65 6e76 2069 6e20 6261 7368 2074  ualenv in bash t
-00000dc0: 6572 6d69 6e61 6c0a 0a60 7669 7274 7561  erminal..`virtua
-00000dd0: 6c65 6e76 2076 656e 7660 0a60 7069 7020  lenv venv`.`pip 
-00000de0: 696e 7374 616c 6c20 676f 6f67 6c65 2d61  install google-a
-00000df0: 7069 2d73 7570 706f 7274 600a 6070 6970  pi-support`.`pip
-00000e00: 2069 6e73 7461 6c6c 206a 7570 7974 6572   install jupyter
-00000e10: 6c61 6260 0a60 736f 7572 6365 2076 656e  lab`.`source ven
-00000e20: 762f 5363 7269 7074 732f 6163 7469 7661  v/Scripts/activa
-00000e30: 7465 600a 6065 7870 6f72 7420 474f 4f47  te`.`export GOOG
-00000e40: 4c45 5f41 5050 4c49 4341 5449 4f4e 5f43  LE_APPLICATION_C
-00000e50: 5245 4445 4e54 4941 4c53 3d43 3a2f 7061  REDENTIALS=C:/pa
-00000e60: 7468 2f74 6f2f 6d79 2f73 6572 7669 6365  th/to/my/service
-00000e70: 5f61 6363 6f75 6e74 5f63 7265 6465 6e74  _account_credent
-00000e80: 6961 6c73 2e6a 736f 6e60 0a60 6a75 7079  ials.json`.`jupy
-00000e90: 7465 7220 6c61 6260 0a                   ter lab`.
+00000000: 2320 676f 6f67 6c65 2d61 7069 2d73 7570  # google-api-sup
+00000010: 706f 7274 0a0a 536f 6d65 2066 756e 6374  port..Some funct
+00000020: 696f 6e73 2074 6f20 6d61 6b65 2047 6f6f  ions to make Goo
+00000030: 676c 6520 4150 4973 206d 6f72 6520 7573  gle APIs more us
+00000040: 6162 6c65 2e0a 0a23 2320 496e 7374 616c  able...## Instal
+00000050: 6c0a 0a60 7069 7020 696e 7374 616c 6c20  l..`pip install 
+00000060: 676f 6f67 6c65 2d61 7069 2d73 7570 706f  google-api-suppo
+00000070: 7274 600a 0a23 2320 436f 6e74 7269 6275  rt`..## Contribu
+00000080: 7465 0a0a 5468 6520 636f 6e74 7269 6275  te..The contribu
+00000090: 7469 6f6e 7320 6172 6520 656e 636f 7572  tions are encour
+000000a0: 6167 6564 2073 6f20 7468 6520 6c69 6272  aged so the libr
+000000b0: 6172 7920 6361 6e20 6b65 6570 2067 726f  ary can keep gro
+000000c0: 7769 6e67 2061 6e64 2068 656c 7020 6d6f  wing and help mo
+000000d0: 7265 2070 656f 706c 652e 0a0a 596f 7520  re people...You 
+000000e0: 6361 6e20 616c 736f 2063 7265 6174 6520  can also create 
+000000f0: 616e 2069 7373 7565 2069 6e20 6f72 6465  an issue in orde
+00000100: 7220 746f 2070 6f69 6e74 206f 7468 6572  r to point other
+00000110: 2063 6f6e 7472 6962 7574 6f72 7320 746f   contributors to
+00000120: 2064 6573 6972 6564 2066 756e 6374 696f   desired functio
+00000130: 6e61 6c69 7469 6573 2e0a 0a23 2320 4675  nalities...## Fu
+00000140: 6e63 7469 6f6e 7320 6176 616c 6961 626c  nctions avaliabl
+00000150: 650a 0a2a 2053 6865 6574 730a 2020 2a20  e..* Sheets.  * 
+00000160: 4765 7420 7061 6e64 6173 2e64 6174 6166  Get pandas.dataf
+00000170: 7261 6d65 2066 726f 6d20 5368 6565 7473  rame from Sheets
+00000180: 0a20 202a 2055 706c 6f61 6420 7061 6e64  .  * Upload pand
+00000190: 6173 2e64 6174 6166 7261 6d65 2074 6f20  as.dataframe to 
+000001a0: 5368 6565 7473 0a20 202a 2052 6574 7269  Sheets.  * Retri
+000001b0: 6576 6520 7368 6565 7420 6e61 6d65 730a  eve sheet names.
+000001c0: 2020 2a20 4164 6420 7368 6565 7473 2074    * Add sheets t
+000001d0: 6f20 6120 7370 7265 6164 7368 6565 740a  o a spreadsheet.
+000001e0: 2020 2a20 4372 6561 7465 206e 6577 2073    * Create new s
+000001f0: 7072 6561 6473 6865 6574 0a2a 2053 6c69  preadsheet.* Sli
+00000200: 6465 730a 2020 2a20 4372 6561 7465 2070  des.  * Create p
+00000210: 7265 7365 6e74 6174 696f 6e0a 2020 2a20  resentation.  * 
+00000220: 4765 7420 7072 6573 656e 7461 7469 6f6e  Get presentation
+00000230: 2069 6e66 6f0a 2020 2a20 4765 7420 7072   info.  * Get pr
+00000240: 6573 656e 7461 7469 6f6e 2073 6c69 6465  esentation slide
+00000250: 730a 2020 2a20 4765 7420 736c 6964 6520  s.  * Get slide 
+00000260: 6e6f 7465 730a 2020 2a20 5265 706c 6163  notes.  * Replac
+00000270: 6520 7465 7874 0a20 202a 2052 6570 6c61  e text.  * Repla
+00000280: 6365 2073 6861 7065 2077 6974 6820 696d  ce shape with im
+00000290: 6167 650a 2020 2a20 5265 706c 6163 6520  age.  * Replace 
+000002a0: 696d 6167 650a 2020 2a20 4765 7420 736c  image.  * Get sl
+000002b0: 6964 6520 6e6f 7465 730a 2020 2a20 4261  ide notes.  * Ba
+000002c0: 7463 6820 7265 706c 6163 6520 7465 7874  tch replace text
+000002d0: 0a20 202a 2042 6174 6368 2072 6570 6c61  .  * Batch repla
+000002e0: 6365 2073 6861 7065 7320 7769 7468 2069  ce shapes with i
+000002f0: 6d61 6765 730a 2020 2a20 496e 7365 7274  mages.  * Insert
+00000300: 2069 6d61 6765 0a20 202a 2044 7570 6c69   image.  * Dupli
+00000310: 6361 7465 206f 626a 6563 740a 2020 2a20  cate object.  * 
+00000320: 4465 6c65 7465 206f 626a 6563 740a 2020  Delete object.  
+00000330: 2a20 4261 7463 6820 6465 6c65 7465 206f  * Batch delete o
+00000340: 626a 6563 740a 2020 2a20 4465 6c65 7465  bject.  * Delete
+00000350: 2074 6578 740a 2020 2a20 4261 7463 6820   text.  * Batch 
+00000360: 6465 6c65 7465 2074 6578 740a 2020 2a20  delete text.  * 
+00000370: 4465 6c65 7465 2070 7265 7365 6e74 6174  Delete presentat
+00000380: 696f 6e20 6e6f 7465 730a 2020 2a20 5472  ion notes.  * Tr
+00000390: 616e 7366 6f72 6d20 6f62 6a65 6374 0a2a  ansform object.*
+000003a0: 2044 7269 7665 0a20 202a 2047 6574 2066   Drive.  * Get f
+000003b0: 696c 6520 6e61 6d65 0a20 202a 204d 6f76  ile name.  * Mov
+000003c0: 6520 6669 6c65 0a20 202a 2044 656c 6574  e file.  * Delet
+000003d0: 6520 6669 6c65 0a20 202a 2043 6f70 7920  e file.  * Copy 
+000003e0: 6669 6c65 0a20 202a 2055 706c 6f61 6420  file.  * Upload 
+000003f0: 696d 6167 650a 2020 2a20 4372 6561 7465  image.  * Create
+00000400: 2066 6f6c 6465 720a 2020 2a20 4c69 7374   folder.  * List
+00000410: 2066 6f6c 6465 7273 2069 6e20 666f 6c64   folders in fold
+00000420: 6572 0a20 202a 2047 6574 2066 6f6c 6465  er.  * Get folde
+00000430: 7220 6964 2062 7920 6e61 6d65 0a20 202a  r id by name.  *
+00000440: 2047 6574 2066 6f6c 6465 7220 6964 2062   Get folder id b
+00000450: 7920 7061 7468 0a20 202a 2044 6f77 6e6c  y path.  * Downl
+00000460: 6f61 6420 6669 6c65 0a0a 2a20 5374 6f72  oad file..* Stor
+00000470: 6167 650a 2020 2a20 5570 6c6f 6164 2061  age.  * Upload a
+00000480: 2066 696c 6520 746f 2067 6f6f 676c 6520   file to google 
+00000490: 7374 6f72 6167 6520 616e 6420 6765 7420  storage and get 
+000004a0: 6974 7320 5552 4c0a 0a23 2320 5374 6570  its URL..## Step
+000004b0: 7320 746f 2075 7365 2067 6f6f 676c 6520  s to use google 
+000004c0: 5368 6565 7473 2041 5049 0a0a 496e 206f  Sheets API..In o
+000004d0: 7264 6572 2074 6f20 7573 6520 476f 6f67  rder to use Goog
+000004e0: 6c65 2041 5049 7320 796f 7520 7769 6c6c  le APIs you will
+000004f0: 206e 6565 6420 746f 2061 7574 6865 6e74   need to authent
+00000500: 6963 6174 652c 2074 6869 7320 7374 6570  icate, this step
+00000510: 7320 6775 6964 6520 796f 7520 7468 726f  s guide you thro
+00000520: 7567 6820 7468 6520 7072 6f63 6573 733a  ugh the process:
+00000530: 0a0a 302e 2043 7265 6174 6520 6120 7072  ..0. Create a pr
+00000540: 6f6a 6563 7420 696e 2063 6f6e 736f 6c65  oject in console
+00000550: 2e64 6576 656c 6f70 6572 732e 676f 6f67  .developers.goog
+00000560: 6c65 2e63 6f6d 0a0a 3c68 7474 7073 3a2f  le.com..<https:/
+00000570: 2f63 6f6e 736f 6c65 2e64 6576 656c 6f70  /console.develop
+00000580: 6572 732e 676f 6f67 6c65 2e63 6f6d 3e0a  ers.google.com>.
+00000590: 0a30 2e20 4372 6561 7465 2067 6f6f 676c  .0. Create googl
+000005a0: 6520 7365 7276 6963 6520 6163 636f 756e  e service accoun
+000005b0: 742e 0a20 2020 2030 2e20 476f 2074 6f20  t..    0. Go to 
+000005c0: 3c68 7474 7073 3a2f 2f63 6f6e 736f 6c65  <https://console
+000005d0: 2e64 6576 656c 6f70 6572 732e 676f 6f67  .developers.goog
+000005e0: 6c65 2e63 6f6d 2f70 726f 6a65 6374 7365  le.com/projectse
+000005f0: 6c65 6374 6f72 2f61 7069 732f 6372 6564  lector/apis/cred
+00000600: 656e 7469 616c 733e 2061 6e64 2063 7265  entials> and cre
+00000610: 6174 6520 6120 6e65 7720 7072 6f6a 6563  ate a new projec
+00000620: 742e 0a20 2020 2021 5b43 7265 6174 6520  t..    ![Create 
+00000630: 6120 6465 7665 6c6f 7065 7273 2070 726f  a developers pro
+00000640: 6a65 6374 5d28 646f 6373 2f69 6d67 2f63  ject](docs/img/c
+00000650: 7265 6174 655f 7072 6f6a 6563 742e 504e  reate_project.PN
+00000660: 4729 0a0a 2020 2020 302e 2043 7265 6174  G)..    0. Creat
+00000670: 6520 6372 6564 656e 7469 616c 732e 0a20  e credentials.. 
+00000680: 2020 2021 5b5d 2864 6f63 732f 696d 672f     ![](docs/img/
+00000690: 6368 6f6f 7365 5f63 7265 6465 6e74 6961  choose_credentia
+000006a0: 6c73 2e50 4e47 290a 2020 2020 2020 2020  ls.PNG).        
+000006b0: 2a20 496e 2074 6869 7320 6669 7273 7420  * In this first 
+000006c0: 7665 7273 696f 6e2c 2069 2077 696c 6c20  version, i will 
+000006d0: 6578 706c 6169 6e20 686f 7720 746f 2064  explain how to d
+000006e0: 6561 6c20 7769 7468 2053 6572 7669 6365  eal with Service
+000006f0: 7320 6163 636f 756e 7473 2c20 736f 2073  s accounts, so s
+00000700: 656c 6563 7420 2253 6572 7669 6365 2061  elect "Service a
+00000710: 6363 6f75 6e74 206b 6579 222e 0a0a 2020  ccount key"...  
+00000720: 2020 302e 2043 7265 6174 6520 6120 7365    0. Create a se
+00000730: 7276 6963 6520 6163 636f 756e 742e 0a20  rvice account.. 
+00000740: 2020 2021 5b5d 2864 6f63 732f 696d 672f     ![](docs/img/
+00000750: 6372 6561 7465 5f73 6572 7669 6365 5f61  create_service_a
+00000760: 6363 6f75 6e74 2e50 4e47 290a 2020 2020  ccount.PNG).    
+00000770: 2020 2020 2a20 446f 776e 6c6f 6164 2074      * Download t
+00000780: 6865 202e 6a73 6f6e 2066 696c 6520 616e  he .json file an
+00000790: 6420 4b45 4550 2049 5420 5341 4645 2e0a  d KEEP IT SAFE..
+000007a0: 0a20 2020 2030 2e20 4e6f 7720 796f 7520  .    0. Now you 
+000007b0: 6861 7665 2079 6f75 7220 7365 7276 6963  have your servic
+000007c0: 6520 6163 636f 756e 7420 6372 6561 7465  e account create
+000007d0: 6420 696e 7369 6465 2079 6f75 7220 6e65  d inside your ne
+000007e0: 7720 7072 6f6a 6563 742e 0a20 2020 2021  w project..    !
+000007f0: 5b5d 2864 6f63 732f 696d 672f 6372 6561  [](docs/img/crea
+00000800: 7465 5f73 6572 7669 6365 5f61 6363 6f75  te_service_accou
+00000810: 6e74 2e50 4e47 290a 0a20 2020 2030 2e20  nt.PNG)..    0. 
+00000820: 436f 7079 2079 6f75 7220 2275 7365 7220  Copy your "user 
+00000830: 6964 2220 696e 2022 4d61 6e61 6765 2073  id" in "Manage s
+00000840: 6572 7669 6365 2061 6363 6f75 6e74 7322  ervice accounts"
+00000850: 2074 6f20 7573 6520 6974 206c 6174 6572   to use it later
+00000860: 2e0a 2020 2020 2020 2020 2a20 4974 206c  ..        * It l
+00000870: 6f6f 6b73 206c 696b 6520 7468 6973 206f  ooks like this o
+00000880: 6e65 3a20 6066 6972 7374 2d73 6572 7669  ne: `first-servi
+00000890: 6365 2d61 6363 6f75 6e74 4065 7861 6d70  ce-account@examp
+000008a0: 6c65 2d69 642d 3137 3538 3230 2e69 616d  le-id-175820.iam
+000008b0: 2e67 7365 7276 6963 6561 6363 6f75 6e74  .gserviceaccount
+000008c0: 2e63 6f6d 600a 0a20 2020 2030 2e20 476f  .com`..    0. Go
+000008d0: 2074 6f20 796f 7572 2064 6173 6862 6f61   to your dashboa
+000008e0: 7264 2073 6372 6565 6e20 616e 6420 676f  rd screen and go
+000008f0: 2074 6f20 2245 4e41 424c 4520 4150 4953   to "ENABLE APIS
+00000900: 2041 4e44 2053 4552 5649 4345 5322 2074   AND SERVICES" t
+00000910: 6f20 2275 6e6c 6f63 6b22 2074 6865 2064  o "unlock" the d
+00000920: 6573 6972 6564 2041 5049 2063 616c 6c73  esired API calls
+00000930: 2e0a 2020 2020 496e 206f 7572 2065 7861  ..    In our exa
+00000940: 6d70 6c65 2c20 7765 2077 696c 6c20 6a75  mple, we will ju
+00000950: 7374 2065 6e61 626c 6520 2247 6f6f 676c  st enable "Googl
+00000960: 6520 7368 6565 7473 2041 5049 222e 0a20  e sheets API".. 
+00000970: 2020 2021 5b5d 2864 6f63 732f 696d 672f     ![](docs/img/
+00000980: 656e 6162 6c65 5f61 7069 732e 504e 4729  enable_apis.PNG)
+00000990: 0a20 2020 2021 5b5d 2864 6f63 732f 696d  .    ![](docs/im
+000009a0: 672f 6163 7469 7661 7465 5f73 6865 6574  g/activate_sheet
+000009b0: 732e 504e 4729 0a0a 2323 2043 6865 636b  s.PNG)..## Check
+000009c0: 2074 6865 2073 7065 6369 6669 6320 6372   the specific cr
+000009d0: 6564 656e 7469 616c 7320 646f 6375 6d65  edentials docume
+000009e0: 6e74 6174 696f 6e20 6669 6c65 0a0a 5b43  ntation file..[C
+000009f0: 7265 6465 6e74 6961 6c73 2064 6f63 756d  redentials docum
+00000a00: 656e 7461 7469 6f6e 5d28 2f64 6f63 732f  entation](/docs/
+00000a10: 7365 7475 705f 6372 6564 656e 7469 616c  setup_credential
+00000a20: 732e 6d64 290a 0a23 2320 4d61 6e75 616c  s.md)..## Manual
+00000a30: 6c79 2069 6e73 7461 6c6c 2064 6570 656e  ly install depen
+00000a40: 6465 6e63 6965 730a 0a60 7069 7020 696e  dencies..`pip in
+00000a50: 7374 616c 6c20 6874 7470 6c69 6232 206f  stall httplib2 o
+00000a60: 6175 7468 3263 6c69 656e 7420 7061 6e64  auth2client pand
+00000a70: 6173 2067 6f6f 676c 652d 6170 692d 7079  as google-api-py
+00000a80: 7468 6f6e 2d63 6c69 656e 7420 676f 6f67  thon-client goog
+00000a90: 6c65 2e61 7574 682e 7472 616e 7370 6f72  le.auth.transpor
+00000aa0: 742e 7265 7175 6573 7473 2067 6f6f 676c  t.requests googl
+00000ab0: 652e 6f61 7574 6832 2e63 7265 6465 6e74  e.oauth2.credent
+00000ac0: 6961 6c73 2067 6f6f 676c 655f 6175 7468  ials google_auth
+00000ad0: 5f6f 6175 7468 6c69 622e 666c 6f77 600a  _oauthlib.flow`.
+00000ae0: 0a23 2320 436f 6d70 6c65 7465 2066 6972  .## Complete fir
+00000af0: 7374 2075 7365 2065 7861 6d70 6c65 0a0a  st use example..
+00000b00: 2323 2320 4578 616d 706c 6520 7573 696e  ### Example usin
+00000b10: 6720 7669 7274 7561 6c65 6e76 2069 6e20  g virtualenv in 
+00000b20: 6261 7368 2074 6572 6d69 6e61 6c0a 0a60  bash terminal..`
+00000b30: 7669 7274 7561 6c65 6e76 2076 656e 7660  virtualenv venv`
+00000b40: 0a60 7069 7020 696e 7374 616c 6c20 676f  .`pip install go
+00000b50: 6f67 6c65 2d61 7069 2d73 7570 706f 7274  ogle-api-support
+00000b60: 600a 6070 6970 2069 6e73 7461 6c6c 206a  `.`pip install j
+00000b70: 7570 7974 6572 6c61 6260 0a60 736f 7572  upyterlab`.`sour
+00000b80: 6365 2076 656e 762f 5363 7269 7074 732f  ce venv/Scripts/
+00000b90: 6163 7469 7661 7465 600a 6065 7870 6f72  activate`.`expor
+00000ba0: 7420 474f 4f47 4c45 5f41 5050 4c49 4341  t GOOGLE_APPLICA
+00000bb0: 5449 4f4e 5f43 5245 4445 4e54 4941 4c53  TION_CREDENTIALS
+00000bc0: 3d43 3a2f 7061 7468 2f74 6f2f 6d79 2f73  =C:/path/to/my/s
+00000bd0: 6572 7669 6365 5f61 6363 6f75 6e74 5f63  ervice_account_c
+00000be0: 7265 6465 6e74 6961 6c73 2e6a 736f 6e60  redentials.json`
+00000bf0: 0a60 6a75 7079 7465 7220 6c61 6260 0a0a  .`jupyter lab`..
+00000c00: 2323 2053 6574 7570 2074 6f20 6465 7665  ## Setup to deve
+00000c10: 6c6f 7065 6d65 6e74 0a0a 6076 6972 7475  lopement..`virtu
+00000c20: 616c 656e 7620 7665 6e76 600a 6070 6970  alenv venv`.`pip
+00000c30: 2069 6e73 7461 6c6c 202e 600a 6070 6970   install .`.`pip
+00000c40: 2069 6e73 7461 6c6c 206a 7570 7974 6572   install jupyter
+00000c50: 6c61 6260 0a60 736f 7572 6365 2076 656e  lab`.`source ven
+00000c60: 762f 5363 7269 7074 732f 6163 7469 7661  v/Scripts/activa
+00000c70: 7465 600a 6065 7870 6f72 7420 474f 4f47  te`.`export GOOG
+00000c80: 4c45 5f41 5050 4c49 4341 5449 4f4e 5f43  LE_APPLICATION_C
+00000c90: 5245 4445 4e54 4941 4c53 3d43 3a2f 7061  REDENTIALS=C:/pa
+00000ca0: 7468 2f74 6f2f 6d79 2f73 6572 7669 6365  th/to/my/service
+00000cb0: 5f61 6363 6f75 6e74 5f63 7265 6465 6e74  _account_credent
+00000cc0: 6961 6c73 2e6a 736f 6e60 0a60 6a75 7079  ials.json`.`jupy
+00000cd0: 7465 7220 6c61 6260                      ter lab`
```

### Comparing `google-api-support-0.1.4/README.md` & `google_api_support-0.1.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,203 +1,250 @@
-00000000: 2320 676f 6f67 6c65 2d61 7069 2d73 7570  # google-api-sup
-00000010: 706f 7274 0a0a 536f 6d65 2066 756e 6374  port..Some funct
-00000020: 696f 6e73 2074 6f20 6d61 6b65 2047 6f6f  ions to make Goo
-00000030: 676c 6520 4150 4973 206d 6f72 6520 7573  gle APIs more us
-00000040: 6162 6c65 2e0a 0a23 2320 496e 7374 616c  able...## Instal
-00000050: 6c0a 0a60 7069 7020 696e 7374 616c 6c20  l..`pip install 
-00000060: 676f 6f67 6c65 2d61 7069 2d73 7570 706f  google-api-suppo
-00000070: 7274 600a 0a23 2320 436f 6e74 7269 6275  rt`..## Contribu
-00000080: 7465 0a0a 5468 6520 636f 6e74 7269 6275  te..The contribu
-00000090: 7469 6f6e 7320 6172 6520 656e 636f 7572  tions are encour
-000000a0: 6167 6564 2073 6f20 7468 6520 6c69 6272  aged so the libr
-000000b0: 6172 7920 6361 6e20 6b65 6570 2067 726f  ary can keep gro
-000000c0: 7769 6e67 2061 6e64 2068 656c 7020 6d6f  wing and help mo
-000000d0: 7265 2070 656f 706c 652e 0a0a 596f 7520  re people...You 
-000000e0: 6361 6e20 616c 736f 2063 7265 6174 6520  can also create 
-000000f0: 616e 2069 7373 7565 2069 6e20 6f72 6465  an issue in orde
-00000100: 7220 746f 2070 6f69 6e74 206f 7468 6572  r to point other
-00000110: 2063 6f6e 7472 6962 7574 6f72 7320 746f   contributors to
-00000120: 2064 6573 6972 6564 2066 756e 6374 696f   desired functio
-00000130: 6e61 6c69 7469 6573 2e0a 0a20 203c 6120  nalities...  <a 
-00000140: 6872 6566 3d22 6874 7470 733a 2f2f 6469  href="https://di
-00000150: 7363 6f72 642e 6767 2f5a 4279 5173 6d78  scord.gg/ZByQsmx
-00000160: 5222 2074 6172 6765 743d 225f 626c 616e  R" target="_blan
-00000170: 6b22 3e0a 2020 2020 3c69 6d67 2073 7263  k">.    <img src
-00000180: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00000190: 6965 6c64 732e 696f 2f64 6973 636f 7264  ields.io/discord
-000001a0: 2f33 3038 3332 3330 3536 3539 3234 3836  /308323056592486
-000001b0: 3432 303f 6c6f 676f 3d64 6973 636f 7264  420?logo=discord
-000001c0: 2220 616c 743d 2244 6973 636f 7264 2043  " alt="Discord C
-000001d0: 6861 7422 202f 3e0a 2020 3c2f 613e 0a0a  hat" />.  </a>..
-000001e0: 2323 2046 756e 6374 696f 6e73 2061 7661  ## Functions ava
-000001f0: 6c69 6162 6c65 0a0a 2a20 5368 6565 7473  liable..* Sheets
-00000200: 0a20 202a 2047 6574 2070 616e 6461 732e  .  * Get pandas.
-00000210: 6461 7461 6672 616d 6520 6672 6f6d 2053  dataframe from S
-00000220: 6865 6574 730a 2020 2a20 5570 6c6f 6164  heets.  * Upload
-00000230: 2070 616e 6461 732e 6461 7461 6672 616d   pandas.datafram
-00000240: 6520 746f 2053 6865 6574 730a 2020 2a20  e to Sheets.  * 
-00000250: 5265 7472 6965 7665 2073 6865 6574 206e  Retrieve sheet n
-00000260: 616d 6573 0a20 202a 2041 6464 2073 6865  ames.  * Add she
-00000270: 6574 7320 746f 2061 2073 7072 6561 6473  ets to a spreads
-00000280: 6865 6574 0a20 202a 2043 7265 6174 6520  heet.  * Create 
-00000290: 6e65 7720 7370 7265 6164 7368 6565 740a  new spreadsheet.
-000002a0: 2a20 536c 6964 6573 0a20 202a 2043 7265  * Slides.  * Cre
-000002b0: 6174 6520 7072 6573 656e 7461 7469 6f6e  ate presentation
-000002c0: 0a20 202a 2047 6574 2070 7265 7365 6e74  .  * Get present
-000002d0: 6174 696f 6e20 696e 666f 0a20 202a 2047  ation info.  * G
-000002e0: 6574 2070 7265 7365 6e74 6174 696f 6e20  et presentation 
-000002f0: 736c 6964 6573 0a20 202a 2047 6574 2073  slides.  * Get s
-00000300: 6c69 6465 206e 6f74 6573 0a20 202a 2052  lide notes.  * R
-00000310: 6570 6c61 6365 2074 6578 740a 2020 2a20  eplace text.  * 
-00000320: 5265 706c 6163 6520 7368 6170 6520 7769  Replace shape wi
-00000330: 7468 2069 6d61 6765 0a20 202a 2052 6570  th image.  * Rep
-00000340: 6c61 6365 2069 6d61 6765 0a20 202a 2047  lace image.  * G
-00000350: 6574 2073 6c69 6465 206e 6f74 6573 0a20  et slide notes. 
-00000360: 202a 2042 6174 6368 2072 6570 6c61 6365   * Batch replace
-00000370: 2074 6578 740a 2020 2a20 4261 7463 6820   text.  * Batch 
-00000380: 7265 706c 6163 6520 7368 6170 6573 2077  replace shapes w
-00000390: 6974 6820 696d 6167 6573 0a20 202a 2049  ith images.  * I
-000003a0: 6e73 6572 7420 696d 6167 650a 2020 2a20  nsert image.  * 
-000003b0: 4475 706c 6963 6174 6520 6f62 6a65 6374  Duplicate object
-000003c0: 0a20 202a 2044 656c 6574 6520 6f62 6a65  .  * Delete obje
-000003d0: 6374 0a20 202a 2042 6174 6368 2064 656c  ct.  * Batch del
-000003e0: 6574 6520 6f62 6a65 6374 0a20 202a 2044  ete object.  * D
-000003f0: 656c 6574 6520 7465 7874 0a20 202a 2042  elete text.  * B
-00000400: 6174 6368 2064 656c 6574 6520 7465 7874  atch delete text
-00000410: 0a20 202a 2044 656c 6574 6520 7072 6573  .  * Delete pres
-00000420: 656e 7461 7469 6f6e 206e 6f74 6573 0a20  entation notes. 
-00000430: 202a 2054 7261 6e73 666f 726d 206f 626a   * Transform obj
-00000440: 6563 740a 2a20 4472 6976 650a 2020 2a20  ect.* Drive.  * 
-00000450: 4765 7420 6669 6c65 206e 616d 650a 2020  Get file name.  
-00000460: 2a20 4d6f 7665 2066 696c 650a 2020 2a20  * Move file.  * 
-00000470: 4465 6c65 7465 2066 696c 650a 2020 2a20  Delete file.  * 
-00000480: 436f 7079 2066 696c 650a 2020 2a20 5570  Copy file.  * Up
-00000490: 6c6f 6164 2069 6d61 6765 0a20 202a 2043  load image.  * C
-000004a0: 7265 6174 6520 666f 6c64 6572 0a20 202a  reate folder.  *
-000004b0: 204c 6973 7420 666f 6c64 6572 7320 696e   List folders in
-000004c0: 2066 6f6c 6465 720a 2020 2a20 4765 7420   folder.  * Get 
-000004d0: 666f 6c64 6572 2069 6420 6279 206e 616d  folder id by nam
-000004e0: 650a 2020 2a20 4765 7420 666f 6c64 6572  e.  * Get folder
-000004f0: 2069 6420 6279 2070 6174 680a 2020 2a20   id by path.  * 
-00000500: 446f 776e 6c6f 6164 2066 696c 650a 0a2a  Download file..*
-00000510: 2053 746f 7261 6765 0a20 202a 2055 706c   Storage.  * Upl
-00000520: 6f61 6420 6120 6669 6c65 2074 6f20 676f  oad a file to go
-00000530: 6f67 6c65 2073 746f 7261 6765 2061 6e64  ogle storage and
-00000540: 2067 6574 2069 7473 2055 524c 0a0a 2323   get its URL..##
-00000550: 2053 7465 7073 2074 6f20 7573 6520 676f   Steps to use go
-00000560: 6f67 6c65 2053 6865 6574 7320 4150 490a  ogle Sheets API.
-00000570: 0a49 6e20 6f72 6465 7220 746f 2075 7365  .In order to use
-00000580: 2047 6f6f 676c 6520 4150 4973 2079 6f75   Google APIs you
-00000590: 2077 696c 6c20 6e65 6564 2074 6f20 6175   will need to au
-000005a0: 7468 656e 7469 6361 7465 2c20 7468 6973  thenticate, this
-000005b0: 2073 7465 7073 2067 7569 6465 2079 6f75   steps guide you
-000005c0: 2074 6872 6f75 6768 2074 6865 2070 726f   through the pro
-000005d0: 6365 7373 3a0a 0a30 2e20 4372 6561 7465  cess:..0. Create
-000005e0: 2061 2070 726f 6a65 6374 2069 6e20 636f   a project in co
-000005f0: 6e73 6f6c 652e 6465 7665 6c6f 7065 7273  nsole.developers
-00000600: 2e67 6f6f 676c 652e 636f 6d0a 0a3c 6874  .google.com..<ht
-00000610: 7470 733a 2f2f 636f 6e73 6f6c 652e 6465  tps://console.de
-00000620: 7665 6c6f 7065 7273 2e67 6f6f 676c 652e  velopers.google.
-00000630: 636f 6d3e 0a0a 302e 2043 7265 6174 6520  com>..0. Create 
-00000640: 676f 6f67 6c65 2073 6572 7669 6365 2061  google service a
-00000650: 6363 6f75 6e74 2e0a 2020 2020 302e 2047  ccount..    0. G
-00000660: 6f20 746f 203c 6874 7470 733a 2f2f 636f  o to <https://co
-00000670: 6e73 6f6c 652e 6465 7665 6c6f 7065 7273  nsole.developers
-00000680: 2e67 6f6f 676c 652e 636f 6d2f 7072 6f6a  .google.com/proj
-00000690: 6563 7473 656c 6563 746f 722f 6170 6973  ectselector/apis
-000006a0: 2f63 7265 6465 6e74 6961 6c73 3e20 616e  /credentials> an
-000006b0: 6420 6372 6561 7465 2061 206e 6577 2070  d create a new p
-000006c0: 726f 6a65 6374 2e0a 2020 2020 215b 4372  roject..    ![Cr
-000006d0: 6561 7465 2061 2064 6576 656c 6f70 6572  eate a developer
-000006e0: 7320 7072 6f6a 6563 745d 2864 6f63 732f  s project](docs/
-000006f0: 696d 672f 6372 6561 7465 5f70 726f 6a65  img/create_proje
-00000700: 6374 2e50 4e47 290a 0a20 2020 2030 2e20  ct.PNG)..    0. 
-00000710: 4372 6561 7465 2063 7265 6465 6e74 6961  Create credentia
-00000720: 6c73 2e0a 2020 2020 215b 5d28 646f 6373  ls..    ![](docs
-00000730: 2f69 6d67 2f63 686f 6f73 655f 6372 6564  /img/choose_cred
-00000740: 656e 7469 616c 732e 504e 4729 0a20 2020  entials.PNG).   
-00000750: 2020 2020 202a 2049 6e20 7468 6973 2066       * In this f
-00000760: 6972 7374 2076 6572 7369 6f6e 2c20 6920  irst version, i 
-00000770: 7769 6c6c 2065 7870 6c61 696e 2068 6f77  will explain how
-00000780: 2074 6f20 6465 616c 2077 6974 6820 5365   to deal with Se
-00000790: 7276 6963 6573 2061 6363 6f75 6e74 732c  rvices accounts,
-000007a0: 2073 6f20 7365 6c65 6374 2022 5365 7276   so select "Serv
-000007b0: 6963 6520 6163 636f 756e 7420 6b65 7922  ice account key"
-000007c0: 2e0a 0a20 2020 2030 2e20 4372 6561 7465  ...    0. Create
-000007d0: 2061 2073 6572 7669 6365 2061 6363 6f75   a service accou
-000007e0: 6e74 2e0a 2020 2020 215b 5d28 646f 6373  nt..    ![](docs
-000007f0: 2f69 6d67 2f63 7265 6174 655f 7365 7276  /img/create_serv
-00000800: 6963 655f 6163 636f 756e 742e 504e 4729  ice_account.PNG)
-00000810: 0a20 2020 2020 2020 202a 2044 6f77 6e6c  .        * Downl
-00000820: 6f61 6420 7468 6520 2e6a 736f 6e20 6669  oad the .json fi
-00000830: 6c65 2061 6e64 204b 4545 5020 4954 2053  le and KEEP IT S
-00000840: 4146 452e 0a0a 2020 2020 302e 204e 6f77  AFE...    0. Now
-00000850: 2079 6f75 2068 6176 6520 796f 7572 2073   you have your s
-00000860: 6572 7669 6365 2061 6363 6f75 6e74 2063  ervice account c
-00000870: 7265 6174 6564 2069 6e73 6964 6520 796f  reated inside yo
-00000880: 7572 206e 6577 2070 726f 6a65 6374 2e0a  ur new project..
-00000890: 2020 2020 215b 5d28 646f 6373 2f69 6d67      ![](docs/img
-000008a0: 2f63 7265 6174 655f 7365 7276 6963 655f  /create_service_
-000008b0: 6163 636f 756e 742e 504e 4729 0a0a 2020  account.PNG)..  
-000008c0: 2020 302e 2043 6f70 7920 796f 7572 2022    0. Copy your "
-000008d0: 7573 6572 2069 6422 2069 6e20 224d 616e  user id" in "Man
-000008e0: 6167 6520 7365 7276 6963 6520 6163 636f  age service acco
-000008f0: 756e 7473 2220 746f 2075 7365 2069 7420  unts" to use it 
-00000900: 6c61 7465 722e 0a20 2020 2020 2020 202a  later..        *
-00000910: 2049 7420 6c6f 6f6b 7320 6c69 6b65 2074   It looks like t
-00000920: 6869 7320 6f6e 653a 2060 6669 7273 742d  his one: `first-
-00000930: 7365 7276 6963 652d 6163 636f 756e 7440  service-account@
-00000940: 6578 616d 706c 652d 6964 2d31 3735 3832  example-id-17582
-00000950: 302e 6961 6d2e 6773 6572 7669 6365 6163  0.iam.gserviceac
-00000960: 636f 756e 742e 636f 6d60 0a0a 2020 2020  count.com`..    
-00000970: 302e 2047 6f20 746f 2079 6f75 7220 6461  0. Go to your da
-00000980: 7368 626f 6172 6420 7363 7265 656e 2061  shboard screen a
-00000990: 6e64 2067 6f20 746f 2022 454e 4142 4c45  nd go to "ENABLE
-000009a0: 2041 5049 5320 414e 4420 5345 5256 4943   APIS AND SERVIC
-000009b0: 4553 2220 746f 2022 756e 6c6f 636b 2220  ES" to "unlock" 
-000009c0: 7468 6520 6465 7369 7265 6420 4150 4920  the desired API 
-000009d0: 6361 6c6c 732e 0a20 2020 2049 6e20 6f75  calls..    In ou
-000009e0: 7220 6578 616d 706c 652c 2077 6520 7769  r example, we wi
-000009f0: 6c6c 206a 7573 7420 656e 6162 6c65 2022  ll just enable "
-00000a00: 476f 6f67 6c65 2073 6865 6574 7320 4150  Google sheets AP
-00000a10: 4922 2e0a 2020 2020 215b 5d28 646f 6373  I"..    ![](docs
-00000a20: 2f69 6d67 2f65 6e61 626c 655f 6170 6973  /img/enable_apis
-00000a30: 2e50 4e47 290a 2020 2020 215b 5d28 646f  .PNG).    ![](do
-00000a40: 6373 2f69 6d67 2f61 6374 6976 6174 655f  cs/img/activate_
-00000a50: 7368 6565 7473 2e50 4e47 290a 0a23 2320  sheets.PNG)..## 
-00000a60: 4368 6563 6b20 7468 6520 7370 6563 6966  Check the specif
-00000a70: 6963 2063 7265 6465 6e74 6961 6c73 2064  ic credentials d
-00000a80: 6f63 756d 656e 7461 7469 6f6e 2066 696c  ocumentation fil
-00000a90: 650a 0a5b 4372 6564 656e 7469 616c 7320  e..[Credentials 
-00000aa0: 646f 6375 6d65 6e74 6174 696f 6e5d 282f  documentation](/
-00000ab0: 646f 6373 2f73 6574 7570 5f63 7265 6465  docs/setup_crede
-00000ac0: 6e74 6961 6c73 2e6d 6429 0a0a 2323 204d  ntials.md)..## M
-00000ad0: 616e 7561 6c6c 7920 696e 7374 616c 6c20  anually install 
-00000ae0: 6465 7065 6e64 656e 6369 6573 0a0a 6070  dependencies..`p
-00000af0: 6970 2069 6e73 7461 6c6c 2068 7474 706c  ip install httpl
-00000b00: 6962 3220 6f61 7574 6832 636c 6965 6e74  ib2 oauth2client
-00000b10: 2070 616e 6461 7320 676f 6f67 6c65 2d61   pandas google-a
-00000b20: 7069 2d70 7974 686f 6e2d 636c 6965 6e74  pi-python-client
-00000b30: 2067 6f6f 676c 652e 6175 7468 2e74 7261   google.auth.tra
-00000b40: 6e73 706f 7274 2e72 6571 7565 7374 7320  nsport.requests 
-00000b50: 676f 6f67 6c65 2e6f 6175 7468 322e 6372  google.oauth2.cr
-00000b60: 6564 656e 7469 616c 7320 676f 6f67 6c65  edentials google
-00000b70: 5f61 7574 685f 6f61 7574 686c 6962 2e66  _auth_oauthlib.f
-00000b80: 6c6f 7760 0a0a 2323 2043 6f6d 706c 6574  low`..## Complet
-00000b90: 6520 6669 7273 7420 7573 6520 6578 616d  e first use exam
-00000ba0: 706c 650a 0a23 2323 2045 7861 6d70 6c65  ple..### Example
-00000bb0: 2075 7369 6e67 2076 6972 7475 616c 656e   using virtualen
-00000bc0: 7620 696e 2062 6173 6820 7465 726d 696e  v in bash termin
-00000bd0: 616c 0a0a 6076 6972 7475 616c 656e 7620  al..`virtualenv 
-00000be0: 7665 6e76 600a 6070 6970 2069 6e73 7461  venv`.`pip insta
-00000bf0: 6c6c 2067 6f6f 676c 652d 6170 692d 7375  ll google-api-su
-00000c00: 7070 6f72 7460 0a60 7069 7020 696e 7374  pport`.`pip inst
-00000c10: 616c 6c20 6a75 7079 7465 726c 6162 600a  all jupyterlab`.
-00000c20: 6073 6f75 7263 6520 7665 6e76 2f53 6372  `source venv/Scr
-00000c30: 6970 7473 2f61 6374 6976 6174 6560 0a60  ipts/activate`.`
-00000c40: 6578 706f 7274 2047 4f4f 474c 455f 4150  export GOOGLE_AP
-00000c50: 504c 4943 4154 494f 4e5f 4352 4544 454e  PLICATION_CREDEN
-00000c60: 5449 414c 533d 433a 2f70 6174 682f 746f  TIALS=C:/path/to
-00000c70: 2f6d 792f 7365 7276 6963 655f 6163 636f  /my/service_acco
-00000c80: 756e 745f 6372 6564 656e 7469 616c 732e  unt_credentials.
-00000c90: 6a73 6f6e 600a 606a 7570 7974 6572 206c  json`.`jupyter l
-00000ca0: 6162 600a                                ab`.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 676f 6f67  : 2.1.Name: goog
+00000020: 6c65 2d61 7069 2d73 7570 706f 7274 0a56  le-api-support.V
+00000030: 6572 7369 6f6e 3a20 302e 312e 370a 5375  ersion: 0.1.7.Su
+00000040: 6d6d 6172 793a 2049 6e20 7468 6973 2070  mmary: In this p
+00000050: 6163 6b61 6765 2079 6f75 2077 696c 6c20  ackage you will 
+00000060: 6669 6e64 2066 756e 6374 696f 6e73 2074  find functions t
+00000070: 6f20 6465 616c 2077 6974 6820 676f 6f67  o deal with goog
+00000080: 6c65 2061 7069 732e 2053 6865 6574 732c  le apis. Sheets,
+00000090: 2044 7269 7665 2c20 5374 6f72 6167 6520   Drive, Storage 
+000000a0: 616e 6420 536c 6964 6573 0a48 6f6d 652d  and Slides.Home-
+000000b0: 7061 6765 3a20 6874 7470 733a 2f2f 6769  page: https://gi
+000000c0: 7468 7562 2e63 6f6d 2f76 7065 7265 7a62  thub.com/vperezb
+000000d0: 2f67 6f6f 676c 652d 6170 692d 7375 7070  /google-api-supp
+000000e0: 6f72 740a 4175 7468 6f72 3a20 56c3 ad63  ort.Author: V..c
+000000f0: 746f 7220 50c3 a972 657a 2042 6572 7275  tor P..rez Berru
+00000100: 657a 6f0a 4175 7468 6f72 2d65 6d61 696c  ezo.Author-email
+00000110: 3a20 7670 6572 657a 6240 7072 6f74 6f6e  : vperezb@proton
+00000120: 2e6d 650a 436c 6173 7369 6669 6572 3a20  .me.Classifier: 
+00000130: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000140: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000150: 3a20 330a 436c 6173 7369 6669 6572 3a20  : 3.Classifier: 
+00000160: 4c69 6365 6e73 6520 3a3a 2050 7562 6c69  License :: Publi
+00000170: 6320 446f 6d61 696e 0a43 6c61 7373 6966  c Domain.Classif
+00000180: 6965 723a 2044 6576 656c 6f70 6d65 6e74  ier: Development
+00000190: 2053 7461 7475 7320 3a3a 2033 202d 2041   Status :: 3 - A
+000001a0: 6c70 6861 0a44 6573 6372 6970 7469 6f6e  lpha.Description
+000001b0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+000001c0: 6578 742f 6d61 726b 646f 776e 0a4c 6963  ext/markdown.Lic
+000001d0: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
+000001e0: 5345 2e6d 640a 5265 7175 6972 6573 2d44  SE.md.Requires-D
+000001f0: 6973 743a 2067 6f6f 676c 652d 6170 692d  ist: google-api-
+00000200: 7079 7468 6f6e 2d63 6c69 656e 740a 5265  python-client.Re
+00000210: 7175 6972 6573 2d44 6973 743a 2068 7474  quires-Dist: htt
+00000220: 706c 6962 320a 5265 7175 6972 6573 2d44  plib2.Requires-D
+00000230: 6973 743a 206f 6175 7468 3263 6c69 656e  ist: oauth2clien
+00000240: 740a 5265 7175 6972 6573 2d44 6973 743a  t.Requires-Dist:
+00000250: 2070 616e 6461 730a 5265 7175 6972 6573   pandas.Requires
+00000260: 2d44 6973 743a 2067 6f6f 676c 652d 636c  -Dist: google-cl
+00000270: 6f75 642d 7374 6f72 6167 650a 5265 7175  oud-storage.Requ
+00000280: 6972 6573 2d44 6973 743a 2067 6f6f 676c  ires-Dist: googl
+00000290: 652d 6175 7468 0a52 6571 7569 7265 732d  e-auth.Requires-
+000002a0: 4469 7374 3a20 676f 6f67 6c65 5f61 7574  Dist: google_aut
+000002b0: 685f 6f61 7574 686c 6962 0a0a 2320 676f  h_oauthlib..# go
+000002c0: 6f67 6c65 2d61 7069 2d73 7570 706f 7274  ogle-api-support
+000002d0: 0a0a 536f 6d65 2066 756e 6374 696f 6e73  ..Some functions
+000002e0: 2074 6f20 6d61 6b65 2047 6f6f 676c 6520   to make Google 
+000002f0: 4150 4973 206d 6f72 6520 7573 6162 6c65  APIs more usable
+00000300: 2e0a 0a23 2320 496e 7374 616c 6c0a 0a60  ...## Install..`
+00000310: 7069 7020 696e 7374 616c 6c20 676f 6f67  pip install goog
+00000320: 6c65 2d61 7069 2d73 7570 706f 7274 600a  le-api-support`.
+00000330: 0a23 2320 436f 6e74 7269 6275 7465 0a0a  .## Contribute..
+00000340: 5468 6520 636f 6e74 7269 6275 7469 6f6e  The contribution
+00000350: 7320 6172 6520 656e 636f 7572 6167 6564  s are encouraged
+00000360: 2073 6f20 7468 6520 6c69 6272 6172 7920   so the library 
+00000370: 6361 6e20 6b65 6570 2067 726f 7769 6e67  can keep growing
+00000380: 2061 6e64 2068 656c 7020 6d6f 7265 2070   and help more p
+00000390: 656f 706c 652e 0a0a 596f 7520 6361 6e20  eople...You can 
+000003a0: 616c 736f 2063 7265 6174 6520 616e 2069  also create an i
+000003b0: 7373 7565 2069 6e20 6f72 6465 7220 746f  ssue in order to
+000003c0: 2070 6f69 6e74 206f 7468 6572 2063 6f6e   point other con
+000003d0: 7472 6962 7574 6f72 7320 746f 2064 6573  tributors to des
+000003e0: 6972 6564 2066 756e 6374 696f 6e61 6c69  ired functionali
+000003f0: 7469 6573 2e0a 0a23 2320 4675 6e63 7469  ties...## Functi
+00000400: 6f6e 7320 6176 616c 6961 626c 650a 0a2a  ons avaliable..*
+00000410: 2053 6865 6574 730a 2020 2a20 4765 7420   Sheets.  * Get 
+00000420: 7061 6e64 6173 2e64 6174 6166 7261 6d65  pandas.dataframe
+00000430: 2066 726f 6d20 5368 6565 7473 0a20 202a   from Sheets.  *
+00000440: 2055 706c 6f61 6420 7061 6e64 6173 2e64   Upload pandas.d
+00000450: 6174 6166 7261 6d65 2074 6f20 5368 6565  ataframe to Shee
+00000460: 7473 0a20 202a 2052 6574 7269 6576 6520  ts.  * Retrieve 
+00000470: 7368 6565 7420 6e61 6d65 730a 2020 2a20  sheet names.  * 
+00000480: 4164 6420 7368 6565 7473 2074 6f20 6120  Add sheets to a 
+00000490: 7370 7265 6164 7368 6565 740a 2020 2a20  spreadsheet.  * 
+000004a0: 4372 6561 7465 206e 6577 2073 7072 6561  Create new sprea
+000004b0: 6473 6865 6574 0a2a 2053 6c69 6465 730a  dsheet.* Slides.
+000004c0: 2020 2a20 4372 6561 7465 2070 7265 7365    * Create prese
+000004d0: 6e74 6174 696f 6e0a 2020 2a20 4765 7420  ntation.  * Get 
+000004e0: 7072 6573 656e 7461 7469 6f6e 2069 6e66  presentation inf
+000004f0: 6f0a 2020 2a20 4765 7420 7072 6573 656e  o.  * Get presen
+00000500: 7461 7469 6f6e 2073 6c69 6465 730a 2020  tation slides.  
+00000510: 2a20 4765 7420 736c 6964 6520 6e6f 7465  * Get slide note
+00000520: 730a 2020 2a20 5265 706c 6163 6520 7465  s.  * Replace te
+00000530: 7874 0a20 202a 2052 6570 6c61 6365 2073  xt.  * Replace s
+00000540: 6861 7065 2077 6974 6820 696d 6167 650a  hape with image.
+00000550: 2020 2a20 5265 706c 6163 6520 696d 6167    * Replace imag
+00000560: 650a 2020 2a20 4765 7420 736c 6964 6520  e.  * Get slide 
+00000570: 6e6f 7465 730a 2020 2a20 4261 7463 6820  notes.  * Batch 
+00000580: 7265 706c 6163 6520 7465 7874 0a20 202a  replace text.  *
+00000590: 2042 6174 6368 2072 6570 6c61 6365 2073   Batch replace s
+000005a0: 6861 7065 7320 7769 7468 2069 6d61 6765  hapes with image
+000005b0: 730a 2020 2a20 496e 7365 7274 2069 6d61  s.  * Insert ima
+000005c0: 6765 0a20 202a 2044 7570 6c69 6361 7465  ge.  * Duplicate
+000005d0: 206f 626a 6563 740a 2020 2a20 4465 6c65   object.  * Dele
+000005e0: 7465 206f 626a 6563 740a 2020 2a20 4261  te object.  * Ba
+000005f0: 7463 6820 6465 6c65 7465 206f 626a 6563  tch delete objec
+00000600: 740a 2020 2a20 4465 6c65 7465 2074 6578  t.  * Delete tex
+00000610: 740a 2020 2a20 4261 7463 6820 6465 6c65  t.  * Batch dele
+00000620: 7465 2074 6578 740a 2020 2a20 4465 6c65  te text.  * Dele
+00000630: 7465 2070 7265 7365 6e74 6174 696f 6e20  te presentation 
+00000640: 6e6f 7465 730a 2020 2a20 5472 616e 7366  notes.  * Transf
+00000650: 6f72 6d20 6f62 6a65 6374 0a2a 2044 7269  orm object.* Dri
+00000660: 7665 0a20 202a 2047 6574 2066 696c 6520  ve.  * Get file 
+00000670: 6e61 6d65 0a20 202a 204d 6f76 6520 6669  name.  * Move fi
+00000680: 6c65 0a20 202a 2044 656c 6574 6520 6669  le.  * Delete fi
+00000690: 6c65 0a20 202a 2043 6f70 7920 6669 6c65  le.  * Copy file
+000006a0: 0a20 202a 2055 706c 6f61 6420 696d 6167  .  * Upload imag
+000006b0: 650a 2020 2a20 4372 6561 7465 2066 6f6c  e.  * Create fol
+000006c0: 6465 720a 2020 2a20 4c69 7374 2066 6f6c  der.  * List fol
+000006d0: 6465 7273 2069 6e20 666f 6c64 6572 0a20  ders in folder. 
+000006e0: 202a 2047 6574 2066 6f6c 6465 7220 6964   * Get folder id
+000006f0: 2062 7920 6e61 6d65 0a20 202a 2047 6574   by name.  * Get
+00000700: 2066 6f6c 6465 7220 6964 2062 7920 7061   folder id by pa
+00000710: 7468 0a20 202a 2044 6f77 6e6c 6f61 6420  th.  * Download 
+00000720: 6669 6c65 0a0a 2a20 5374 6f72 6167 650a  file..* Storage.
+00000730: 2020 2a20 5570 6c6f 6164 2061 2066 696c    * Upload a fil
+00000740: 6520 746f 2067 6f6f 676c 6520 7374 6f72  e to google stor
+00000750: 6167 6520 616e 6420 6765 7420 6974 7320  age and get its 
+00000760: 5552 4c0a 0a23 2320 5374 6570 7320 746f  URL..## Steps to
+00000770: 2075 7365 2067 6f6f 676c 6520 5368 6565   use google Shee
+00000780: 7473 2041 5049 0a0a 496e 206f 7264 6572  ts API..In order
+00000790: 2074 6f20 7573 6520 476f 6f67 6c65 2041   to use Google A
+000007a0: 5049 7320 796f 7520 7769 6c6c 206e 6565  PIs you will nee
+000007b0: 6420 746f 2061 7574 6865 6e74 6963 6174  d to authenticat
+000007c0: 652c 2074 6869 7320 7374 6570 7320 6775  e, this steps gu
+000007d0: 6964 6520 796f 7520 7468 726f 7567 6820  ide you through 
+000007e0: 7468 6520 7072 6f63 6573 733a 0a0a 302e  the process:..0.
+000007f0: 2043 7265 6174 6520 6120 7072 6f6a 6563   Create a projec
+00000800: 7420 696e 2063 6f6e 736f 6c65 2e64 6576  t in console.dev
+00000810: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
+00000820: 6f6d 0a0a 3c68 7474 7073 3a2f 2f63 6f6e  om..<https://con
+00000830: 736f 6c65 2e64 6576 656c 6f70 6572 732e  sole.developers.
+00000840: 676f 6f67 6c65 2e63 6f6d 3e0a 0a30 2e20  google.com>..0. 
+00000850: 4372 6561 7465 2067 6f6f 676c 6520 7365  Create google se
+00000860: 7276 6963 6520 6163 636f 756e 742e 0a20  rvice account.. 
+00000870: 2020 2030 2e20 476f 2074 6f20 3c68 7474     0. Go to <htt
+00000880: 7073 3a2f 2f63 6f6e 736f 6c65 2e64 6576  ps://console.dev
+00000890: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
+000008a0: 6f6d 2f70 726f 6a65 6374 7365 6c65 6374  om/projectselect
+000008b0: 6f72 2f61 7069 732f 6372 6564 656e 7469  or/apis/credenti
+000008c0: 616c 733e 2061 6e64 2063 7265 6174 6520  als> and create 
+000008d0: 6120 6e65 7720 7072 6f6a 6563 742e 0a20  a new project.. 
+000008e0: 2020 2021 5b43 7265 6174 6520 6120 6465     ![Create a de
+000008f0: 7665 6c6f 7065 7273 2070 726f 6a65 6374  velopers project
+00000900: 5d28 646f 6373 2f69 6d67 2f63 7265 6174  ](docs/img/creat
+00000910: 655f 7072 6f6a 6563 742e 504e 4729 0a0a  e_project.PNG)..
+00000920: 2020 2020 302e 2043 7265 6174 6520 6372      0. Create cr
+00000930: 6564 656e 7469 616c 732e 0a20 2020 2021  edentials..    !
+00000940: 5b5d 2864 6f63 732f 696d 672f 6368 6f6f  [](docs/img/choo
+00000950: 7365 5f63 7265 6465 6e74 6961 6c73 2e50  se_credentials.P
+00000960: 4e47 290a 2020 2020 2020 2020 2a20 496e  NG).        * In
+00000970: 2074 6869 7320 6669 7273 7420 7665 7273   this first vers
+00000980: 696f 6e2c 2069 2077 696c 6c20 6578 706c  ion, i will expl
+00000990: 6169 6e20 686f 7720 746f 2064 6561 6c20  ain how to deal 
+000009a0: 7769 7468 2053 6572 7669 6365 7320 6163  with Services ac
+000009b0: 636f 756e 7473 2c20 736f 2073 656c 6563  counts, so selec
+000009c0: 7420 2253 6572 7669 6365 2061 6363 6f75  t "Service accou
+000009d0: 6e74 206b 6579 222e 0a0a 2020 2020 302e  nt key"...    0.
+000009e0: 2043 7265 6174 6520 6120 7365 7276 6963   Create a servic
+000009f0: 6520 6163 636f 756e 742e 0a20 2020 2021  e account..    !
+00000a00: 5b5d 2864 6f63 732f 696d 672f 6372 6561  [](docs/img/crea
+00000a10: 7465 5f73 6572 7669 6365 5f61 6363 6f75  te_service_accou
+00000a20: 6e74 2e50 4e47 290a 2020 2020 2020 2020  nt.PNG).        
+00000a30: 2a20 446f 776e 6c6f 6164 2074 6865 202e  * Download the .
+00000a40: 6a73 6f6e 2066 696c 6520 616e 6420 4b45  json file and KE
+00000a50: 4550 2049 5420 5341 4645 2e0a 0a20 2020  EP IT SAFE...   
+00000a60: 2030 2e20 4e6f 7720 796f 7520 6861 7665   0. Now you have
+00000a70: 2079 6f75 7220 7365 7276 6963 6520 6163   your service ac
+00000a80: 636f 756e 7420 6372 6561 7465 6420 696e  count created in
+00000a90: 7369 6465 2079 6f75 7220 6e65 7720 7072  side your new pr
+00000aa0: 6f6a 6563 742e 0a20 2020 2021 5b5d 2864  oject..    ![](d
+00000ab0: 6f63 732f 696d 672f 6372 6561 7465 5f73  ocs/img/create_s
+00000ac0: 6572 7669 6365 5f61 6363 6f75 6e74 2e50  ervice_account.P
+00000ad0: 4e47 290a 0a20 2020 2030 2e20 436f 7079  NG)..    0. Copy
+00000ae0: 2079 6f75 7220 2275 7365 7220 6964 2220   your "user id" 
+00000af0: 696e 2022 4d61 6e61 6765 2073 6572 7669  in "Manage servi
+00000b00: 6365 2061 6363 6f75 6e74 7322 2074 6f20  ce accounts" to 
+00000b10: 7573 6520 6974 206c 6174 6572 2e0a 2020  use it later..  
+00000b20: 2020 2020 2020 2a20 4974 206c 6f6f 6b73        * It looks
+00000b30: 206c 696b 6520 7468 6973 206f 6e65 3a20   like this one: 
+00000b40: 6066 6972 7374 2d73 6572 7669 6365 2d61  `first-service-a
+00000b50: 6363 6f75 6e74 4065 7861 6d70 6c65 2d69  ccount@example-i
+00000b60: 642d 3137 3538 3230 2e69 616d 2e67 7365  d-175820.iam.gse
+00000b70: 7276 6963 6561 6363 6f75 6e74 2e63 6f6d  rviceaccount.com
+00000b80: 600a 0a20 2020 2030 2e20 476f 2074 6f20  `..    0. Go to 
+00000b90: 796f 7572 2064 6173 6862 6f61 7264 2073  your dashboard s
+00000ba0: 6372 6565 6e20 616e 6420 676f 2074 6f20  creen and go to 
+00000bb0: 2245 4e41 424c 4520 4150 4953 2041 4e44  "ENABLE APIS AND
+00000bc0: 2053 4552 5649 4345 5322 2074 6f20 2275   SERVICES" to "u
+00000bd0: 6e6c 6f63 6b22 2074 6865 2064 6573 6972  nlock" the desir
+00000be0: 6564 2041 5049 2063 616c 6c73 2e0a 2020  ed API calls..  
+00000bf0: 2020 496e 206f 7572 2065 7861 6d70 6c65    In our example
+00000c00: 2c20 7765 2077 696c 6c20 6a75 7374 2065  , we will just e
+00000c10: 6e61 626c 6520 2247 6f6f 676c 6520 7368  nable "Google sh
+00000c20: 6565 7473 2041 5049 222e 0a20 2020 2021  eets API"..    !
+00000c30: 5b5d 2864 6f63 732f 696d 672f 656e 6162  [](docs/img/enab
+00000c40: 6c65 5f61 7069 732e 504e 4729 0a20 2020  le_apis.PNG).   
+00000c50: 2021 5b5d 2864 6f63 732f 696d 672f 6163   ![](docs/img/ac
+00000c60: 7469 7661 7465 5f73 6865 6574 732e 504e  tivate_sheets.PN
+00000c70: 4729 0a0a 2323 2043 6865 636b 2074 6865  G)..## Check the
+00000c80: 2073 7065 6369 6669 6320 6372 6564 656e   specific creden
+00000c90: 7469 616c 7320 646f 6375 6d65 6e74 6174  tials documentat
+00000ca0: 696f 6e20 6669 6c65 0a0a 5b43 7265 6465  ion file..[Crede
+00000cb0: 6e74 6961 6c73 2064 6f63 756d 656e 7461  ntials documenta
+00000cc0: 7469 6f6e 5d28 2f64 6f63 732f 7365 7475  tion](/docs/setu
+00000cd0: 705f 6372 6564 656e 7469 616c 732e 6d64  p_credentials.md
+00000ce0: 290a 0a23 2320 4d61 6e75 616c 6c79 2069  )..## Manually i
+00000cf0: 6e73 7461 6c6c 2064 6570 656e 6465 6e63  nstall dependenc
+00000d00: 6965 730a 0a60 7069 7020 696e 7374 616c  ies..`pip instal
+00000d10: 6c20 6874 7470 6c69 6232 206f 6175 7468  l httplib2 oauth
+00000d20: 3263 6c69 656e 7420 7061 6e64 6173 2067  2client pandas g
+00000d30: 6f6f 676c 652d 6170 692d 7079 7468 6f6e  oogle-api-python
+00000d40: 2d63 6c69 656e 7420 676f 6f67 6c65 2e61  -client google.a
+00000d50: 7574 682e 7472 616e 7370 6f72 742e 7265  uth.transport.re
+00000d60: 7175 6573 7473 2067 6f6f 676c 652e 6f61  quests google.oa
+00000d70: 7574 6832 2e63 7265 6465 6e74 6961 6c73  uth2.credentials
+00000d80: 2067 6f6f 676c 655f 6175 7468 5f6f 6175   google_auth_oau
+00000d90: 7468 6c69 622e 666c 6f77 600a 0a23 2320  thlib.flow`..## 
+00000da0: 436f 6d70 6c65 7465 2066 6972 7374 2075  Complete first u
+00000db0: 7365 2065 7861 6d70 6c65 0a0a 2323 2320  se example..### 
+00000dc0: 4578 616d 706c 6520 7573 696e 6720 7669  Example using vi
+00000dd0: 7274 7561 6c65 6e76 2069 6e20 6261 7368  rtualenv in bash
+00000de0: 2074 6572 6d69 6e61 6c0a 0a60 7669 7274   terminal..`virt
+00000df0: 7561 6c65 6e76 2076 656e 7660 0a60 7069  ualenv venv`.`pi
+00000e00: 7020 696e 7374 616c 6c20 676f 6f67 6c65  p install google
+00000e10: 2d61 7069 2d73 7570 706f 7274 600a 6070  -api-support`.`p
+00000e20: 6970 2069 6e73 7461 6c6c 206a 7570 7974  ip install jupyt
+00000e30: 6572 6c61 6260 0a60 736f 7572 6365 2076  erlab`.`source v
+00000e40: 656e 762f 5363 7269 7074 732f 6163 7469  env/Scripts/acti
+00000e50: 7661 7465 600a 6065 7870 6f72 7420 474f  vate`.`export GO
+00000e60: 4f47 4c45 5f41 5050 4c49 4341 5449 4f4e  OGLE_APPLICATION
+00000e70: 5f43 5245 4445 4e54 4941 4c53 3d43 3a2f  _CREDENTIALS=C:/
+00000e80: 7061 7468 2f74 6f2f 6d79 2f73 6572 7669  path/to/my/servi
+00000e90: 6365 5f61 6363 6f75 6e74 5f63 7265 6465  ce_account_crede
+00000ea0: 6e74 6961 6c73 2e6a 736f 6e60 0a60 6a75  ntials.json`.`ju
+00000eb0: 7079 7465 7220 6c61 6260 0a0a 2323 2053  pyter lab`..## S
+00000ec0: 6574 7570 2074 6f20 6465 7665 6c6f 7065  etup to develope
+00000ed0: 6d65 6e74 0a0a 6076 6972 7475 616c 656e  ment..`virtualen
+00000ee0: 7620 7665 6e76 600a 6070 6970 2069 6e73  v venv`.`pip ins
+00000ef0: 7461 6c6c 202e 600a 6070 6970 2069 6e73  tall .`.`pip ins
+00000f00: 7461 6c6c 206a 7570 7974 6572 6c61 6260  tall jupyterlab`
+00000f10: 0a60 736f 7572 6365 2076 656e 762f 5363  .`source venv/Sc
+00000f20: 7269 7074 732f 6163 7469 7661 7465 600a  ripts/activate`.
+00000f30: 6065 7870 6f72 7420 474f 4f47 4c45 5f41  `export GOOGLE_A
+00000f40: 5050 4c49 4341 5449 4f4e 5f43 5245 4445  PPLICATION_CREDE
+00000f50: 4e54 4941 4c53 3d43 3a2f 7061 7468 2f74  NTIALS=C:/path/t
+00000f60: 6f2f 6d79 2f73 6572 7669 6365 5f61 6363  o/my/service_acc
+00000f70: 6f75 6e74 5f63 7265 6465 6e74 6961 6c73  ount_credentials
+00000f80: 2e6a 736f 6e60 0a60 6a75 7079 7465 7220  .json`.`jupyter 
+00000f90: 6c61 6260 0a                             lab`.
```

### Comparing `google-api-support-0.1.4/google_api_support.egg-info/PKG-INFO` & `google_api_support-0.1.7/google_api_support.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,234 +1,250 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 676f 6f67  : 2.1.Name: goog
 00000020: 6c65 2d61 7069 2d73 7570 706f 7274 0a56  le-api-support.V
-00000030: 6572 7369 6f6e 3a20 302e 312e 340a 5375  ersion: 0.1.4.Su
+00000030: 6572 7369 6f6e 3a20 302e 312e 370a 5375  ersion: 0.1.7.Su
 00000040: 6d6d 6172 793a 2049 6e20 7468 6973 2070  mmary: In this p
 00000050: 6163 6b61 6765 2079 6f75 2077 696c 6c20  ackage you will 
 00000060: 6669 6e64 2066 756e 6374 696f 6e73 2074  find functions t
 00000070: 6f20 6465 616c 2077 6974 6820 676f 6f67  o deal with goog
 00000080: 6c65 2061 7069 732e 2053 6865 6574 732c  le apis. Sheets,
 00000090: 2044 7269 7665 2c20 5374 6f72 6167 6520   Drive, Storage 
 000000a0: 616e 6420 536c 6964 6573 0a48 6f6d 652d  and Slides.Home-
 000000b0: 7061 6765 3a20 6874 7470 733a 2f2f 6769  page: https://gi
 000000c0: 7468 7562 2e63 6f6d 2f76 7065 7265 7a62  thub.com/vperezb
 000000d0: 2f67 6f6f 676c 652d 6170 692d 7375 7070  /google-api-supp
 000000e0: 6f72 740a 4175 7468 6f72 3a20 56c3 ad63  ort.Author: V..c
 000000f0: 746f 7220 50c3 a972 657a 2042 6572 7275  tor P..rez Berru
 00000100: 657a 6f0a 4175 7468 6f72 2d65 6d61 696c  ezo.Author-email
-00000110: 3a20 7669 6374 6f72 2e70 6572 657a 2e62  : victor.perez.b
-00000120: 6572 7275 657a 6f40 676d 6169 6c2e 636f  erruezo@gmail.co
-00000130: 6d0a 436c 6173 7369 6669 6572 3a20 5072  m.Classifier: Pr
-00000140: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000150: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000160: 330a 436c 6173 7369 6669 6572 3a20 4c69  3.Classifier: Li
-00000170: 6365 6e73 6520 3a3a 2050 7562 6c69 6320  cense :: Public 
-00000180: 446f 6d61 696e 0a43 6c61 7373 6966 6965  Domain.Classifie
-00000190: 723a 2044 6576 656c 6f70 6d65 6e74 2053  r: Development S
-000001a0: 7461 7475 7320 3a3a 2033 202d 2041 6c70  tatus :: 3 - Alp
-000001b0: 6861 0a44 6573 6372 6970 7469 6f6e 2d43  ha.Description-C
-000001c0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-000001d0: 742f 6d61 726b 646f 776e 0a4c 6963 656e  t/markdown.Licen
-000001e0: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-000001f0: 2e6d 640a 0a23 2067 6f6f 676c 652d 6170  .md..# google-ap
-00000200: 692d 7375 7070 6f72 740a 0a53 6f6d 6520  i-support..Some 
-00000210: 6675 6e63 7469 6f6e 7320 746f 206d 616b  functions to mak
-00000220: 6520 476f 6f67 6c65 2041 5049 7320 6d6f  e Google APIs mo
-00000230: 7265 2075 7361 626c 652e 0a0a 2323 2049  re usable...## I
-00000240: 6e73 7461 6c6c 0a0a 6070 6970 2069 6e73  nstall..`pip ins
-00000250: 7461 6c6c 2067 6f6f 676c 652d 6170 692d  tall google-api-
-00000260: 7375 7070 6f72 7460 0a0a 2323 2043 6f6e  support`..## Con
-00000270: 7472 6962 7574 650a 0a54 6865 2063 6f6e  tribute..The con
-00000280: 7472 6962 7574 696f 6e73 2061 7265 2065  tributions are e
-00000290: 6e63 6f75 7261 6765 6420 736f 2074 6865  ncouraged so the
-000002a0: 206c 6962 7261 7279 2063 616e 206b 6565   library can kee
-000002b0: 7020 6772 6f77 696e 6720 616e 6420 6865  p growing and he
-000002c0: 6c70 206d 6f72 6520 7065 6f70 6c65 2e0a  lp more people..
-000002d0: 0a59 6f75 2063 616e 2061 6c73 6f20 6372  .You can also cr
-000002e0: 6561 7465 2061 6e20 6973 7375 6520 696e  eate an issue in
-000002f0: 206f 7264 6572 2074 6f20 706f 696e 7420   order to point 
-00000300: 6f74 6865 7220 636f 6e74 7269 6275 746f  other contributo
-00000310: 7273 2074 6f20 6465 7369 7265 6420 6675  rs to desired fu
-00000320: 6e63 7469 6f6e 616c 6974 6965 732e 0a0a  nctionalities...
-00000330: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000340: 3a2f 2f64 6973 636f 7264 2e67 672f 5a42  ://discord.gg/ZB
-00000350: 7951 736d 7852 2220 7461 7267 6574 3d22  yQsmxR" target="
-00000360: 5f62 6c61 6e6b 223e 0a20 2020 203c 696d  _blank">.    <im
-00000370: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
-00000380: 6d67 2e73 6869 656c 6473 2e69 6f2f 6469  mg.shields.io/di
-00000390: 7363 6f72 642f 3330 3833 3233 3035 3635  scord/3083230565
-000003a0: 3932 3438 3634 3230 3f6c 6f67 6f3d 6469  92486420?logo=di
-000003b0: 7363 6f72 6422 2061 6c74 3d22 4469 7363  scord" alt="Disc
-000003c0: 6f72 6420 4368 6174 2220 2f3e 0a20 203c  ord Chat" />.  <
-000003d0: 2f61 3e0a 0a23 2320 4675 6e63 7469 6f6e  /a>..## Function
-000003e0: 7320 6176 616c 6961 626c 650a 0a2a 2053  s avaliable..* S
-000003f0: 6865 6574 730a 2020 2a20 4765 7420 7061  heets.  * Get pa
-00000400: 6e64 6173 2e64 6174 6166 7261 6d65 2066  ndas.dataframe f
-00000410: 726f 6d20 5368 6565 7473 0a20 202a 2055  rom Sheets.  * U
-00000420: 706c 6f61 6420 7061 6e64 6173 2e64 6174  pload pandas.dat
-00000430: 6166 7261 6d65 2074 6f20 5368 6565 7473  aframe to Sheets
-00000440: 0a20 202a 2052 6574 7269 6576 6520 7368  .  * Retrieve sh
-00000450: 6565 7420 6e61 6d65 730a 2020 2a20 4164  eet names.  * Ad
-00000460: 6420 7368 6565 7473 2074 6f20 6120 7370  d sheets to a sp
-00000470: 7265 6164 7368 6565 740a 2020 2a20 4372  readsheet.  * Cr
-00000480: 6561 7465 206e 6577 2073 7072 6561 6473  eate new spreads
-00000490: 6865 6574 0a2a 2053 6c69 6465 730a 2020  heet.* Slides.  
-000004a0: 2a20 4372 6561 7465 2070 7265 7365 6e74  * Create present
-000004b0: 6174 696f 6e0a 2020 2a20 4765 7420 7072  ation.  * Get pr
-000004c0: 6573 656e 7461 7469 6f6e 2069 6e66 6f0a  esentation info.
-000004d0: 2020 2a20 4765 7420 7072 6573 656e 7461    * Get presenta
-000004e0: 7469 6f6e 2073 6c69 6465 730a 2020 2a20  tion slides.  * 
-000004f0: 4765 7420 736c 6964 6520 6e6f 7465 730a  Get slide notes.
-00000500: 2020 2a20 5265 706c 6163 6520 7465 7874    * Replace text
-00000510: 0a20 202a 2052 6570 6c61 6365 2073 6861  .  * Replace sha
-00000520: 7065 2077 6974 6820 696d 6167 650a 2020  pe with image.  
-00000530: 2a20 5265 706c 6163 6520 696d 6167 650a  * Replace image.
-00000540: 2020 2a20 4765 7420 736c 6964 6520 6e6f    * Get slide no
-00000550: 7465 730a 2020 2a20 4261 7463 6820 7265  tes.  * Batch re
-00000560: 706c 6163 6520 7465 7874 0a20 202a 2042  place text.  * B
-00000570: 6174 6368 2072 6570 6c61 6365 2073 6861  atch replace sha
-00000580: 7065 7320 7769 7468 2069 6d61 6765 730a  pes with images.
-00000590: 2020 2a20 496e 7365 7274 2069 6d61 6765    * Insert image
-000005a0: 0a20 202a 2044 7570 6c69 6361 7465 206f  .  * Duplicate o
-000005b0: 626a 6563 740a 2020 2a20 4465 6c65 7465  bject.  * Delete
-000005c0: 206f 626a 6563 740a 2020 2a20 4261 7463   object.  * Batc
-000005d0: 6820 6465 6c65 7465 206f 626a 6563 740a  h delete object.
-000005e0: 2020 2a20 4465 6c65 7465 2074 6578 740a    * Delete text.
-000005f0: 2020 2a20 4261 7463 6820 6465 6c65 7465    * Batch delete
-00000600: 2074 6578 740a 2020 2a20 4465 6c65 7465   text.  * Delete
-00000610: 2070 7265 7365 6e74 6174 696f 6e20 6e6f   presentation no
-00000620: 7465 730a 2020 2a20 5472 616e 7366 6f72  tes.  * Transfor
-00000630: 6d20 6f62 6a65 6374 0a2a 2044 7269 7665  m object.* Drive
-00000640: 0a20 202a 2047 6574 2066 696c 6520 6e61  .  * Get file na
-00000650: 6d65 0a20 202a 204d 6f76 6520 6669 6c65  me.  * Move file
-00000660: 0a20 202a 2044 656c 6574 6520 6669 6c65  .  * Delete file
-00000670: 0a20 202a 2043 6f70 7920 6669 6c65 0a20  .  * Copy file. 
-00000680: 202a 2055 706c 6f61 6420 696d 6167 650a   * Upload image.
-00000690: 2020 2a20 4372 6561 7465 2066 6f6c 6465    * Create folde
-000006a0: 720a 2020 2a20 4c69 7374 2066 6f6c 6465  r.  * List folde
-000006b0: 7273 2069 6e20 666f 6c64 6572 0a20 202a  rs in folder.  *
-000006c0: 2047 6574 2066 6f6c 6465 7220 6964 2062   Get folder id b
-000006d0: 7920 6e61 6d65 0a20 202a 2047 6574 2066  y name.  * Get f
-000006e0: 6f6c 6465 7220 6964 2062 7920 7061 7468  older id by path
-000006f0: 0a20 202a 2044 6f77 6e6c 6f61 6420 6669  .  * Download fi
-00000700: 6c65 0a0a 2a20 5374 6f72 6167 650a 2020  le..* Storage.  
-00000710: 2a20 5570 6c6f 6164 2061 2066 696c 6520  * Upload a file 
-00000720: 746f 2067 6f6f 676c 6520 7374 6f72 6167  to google storag
-00000730: 6520 616e 6420 6765 7420 6974 7320 5552  e and get its UR
-00000740: 4c0a 0a23 2320 5374 6570 7320 746f 2075  L..## Steps to u
-00000750: 7365 2067 6f6f 676c 6520 5368 6565 7473  se google Sheets
-00000760: 2041 5049 0a0a 496e 206f 7264 6572 2074   API..In order t
-00000770: 6f20 7573 6520 476f 6f67 6c65 2041 5049  o use Google API
-00000780: 7320 796f 7520 7769 6c6c 206e 6565 6420  s you will need 
-00000790: 746f 2061 7574 6865 6e74 6963 6174 652c  to authenticate,
-000007a0: 2074 6869 7320 7374 6570 7320 6775 6964   this steps guid
-000007b0: 6520 796f 7520 7468 726f 7567 6820 7468  e you through th
-000007c0: 6520 7072 6f63 6573 733a 0a0a 302e 2043  e process:..0. C
-000007d0: 7265 6174 6520 6120 7072 6f6a 6563 7420  reate a project 
-000007e0: 696e 2063 6f6e 736f 6c65 2e64 6576 656c  in console.devel
-000007f0: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
-00000800: 0a0a 3c68 7474 7073 3a2f 2f63 6f6e 736f  ..<https://conso
-00000810: 6c65 2e64 6576 656c 6f70 6572 732e 676f  le.developers.go
-00000820: 6f67 6c65 2e63 6f6d 3e0a 0a30 2e20 4372  ogle.com>..0. Cr
-00000830: 6561 7465 2067 6f6f 676c 6520 7365 7276  eate google serv
-00000840: 6963 6520 6163 636f 756e 742e 0a20 2020  ice account..   
-00000850: 2030 2e20 476f 2074 6f20 3c68 7474 7073   0. Go to <https
-00000860: 3a2f 2f63 6f6e 736f 6c65 2e64 6576 656c  ://console.devel
-00000870: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
-00000880: 2f70 726f 6a65 6374 7365 6c65 6374 6f72  /projectselector
-00000890: 2f61 7069 732f 6372 6564 656e 7469 616c  /apis/credential
-000008a0: 733e 2061 6e64 2063 7265 6174 6520 6120  s> and create a 
-000008b0: 6e65 7720 7072 6f6a 6563 742e 0a20 2020  new project..   
-000008c0: 2021 5b43 7265 6174 6520 6120 6465 7665   ![Create a deve
-000008d0: 6c6f 7065 7273 2070 726f 6a65 6374 5d28  lopers project](
-000008e0: 646f 6373 2f69 6d67 2f63 7265 6174 655f  docs/img/create_
-000008f0: 7072 6f6a 6563 742e 504e 4729 0a0a 2020  project.PNG)..  
-00000900: 2020 302e 2043 7265 6174 6520 6372 6564    0. Create cred
-00000910: 656e 7469 616c 732e 0a20 2020 2021 5b5d  entials..    ![]
-00000920: 2864 6f63 732f 696d 672f 6368 6f6f 7365  (docs/img/choose
-00000930: 5f63 7265 6465 6e74 6961 6c73 2e50 4e47  _credentials.PNG
-00000940: 290a 2020 2020 2020 2020 2a20 496e 2074  ).        * In t
-00000950: 6869 7320 6669 7273 7420 7665 7273 696f  his first versio
-00000960: 6e2c 2069 2077 696c 6c20 6578 706c 6169  n, i will explai
-00000970: 6e20 686f 7720 746f 2064 6561 6c20 7769  n how to deal wi
-00000980: 7468 2053 6572 7669 6365 7320 6163 636f  th Services acco
-00000990: 756e 7473 2c20 736f 2073 656c 6563 7420  unts, so select 
-000009a0: 2253 6572 7669 6365 2061 6363 6f75 6e74  "Service account
-000009b0: 206b 6579 222e 0a0a 2020 2020 302e 2043   key"...    0. C
-000009c0: 7265 6174 6520 6120 7365 7276 6963 6520  reate a service 
-000009d0: 6163 636f 756e 742e 0a20 2020 2021 5b5d  account..    ![]
-000009e0: 2864 6f63 732f 696d 672f 6372 6561 7465  (docs/img/create
-000009f0: 5f73 6572 7669 6365 5f61 6363 6f75 6e74  _service_account
-00000a00: 2e50 4e47 290a 2020 2020 2020 2020 2a20  .PNG).        * 
-00000a10: 446f 776e 6c6f 6164 2074 6865 202e 6a73  Download the .js
-00000a20: 6f6e 2066 696c 6520 616e 6420 4b45 4550  on file and KEEP
-00000a30: 2049 5420 5341 4645 2e0a 0a20 2020 2030   IT SAFE...    0
-00000a40: 2e20 4e6f 7720 796f 7520 6861 7665 2079  . Now you have y
-00000a50: 6f75 7220 7365 7276 6963 6520 6163 636f  our service acco
-00000a60: 756e 7420 6372 6561 7465 6420 696e 7369  unt created insi
-00000a70: 6465 2079 6f75 7220 6e65 7720 7072 6f6a  de your new proj
-00000a80: 6563 742e 0a20 2020 2021 5b5d 2864 6f63  ect..    ![](doc
-00000a90: 732f 696d 672f 6372 6561 7465 5f73 6572  s/img/create_ser
-00000aa0: 7669 6365 5f61 6363 6f75 6e74 2e50 4e47  vice_account.PNG
-00000ab0: 290a 0a20 2020 2030 2e20 436f 7079 2079  )..    0. Copy y
-00000ac0: 6f75 7220 2275 7365 7220 6964 2220 696e  our "user id" in
-00000ad0: 2022 4d61 6e61 6765 2073 6572 7669 6365   "Manage service
-00000ae0: 2061 6363 6f75 6e74 7322 2074 6f20 7573   accounts" to us
-00000af0: 6520 6974 206c 6174 6572 2e0a 2020 2020  e it later..    
-00000b00: 2020 2020 2a20 4974 206c 6f6f 6b73 206c      * It looks l
-00000b10: 696b 6520 7468 6973 206f 6e65 3a20 6066  ike this one: `f
-00000b20: 6972 7374 2d73 6572 7669 6365 2d61 6363  irst-service-acc
-00000b30: 6f75 6e74 4065 7861 6d70 6c65 2d69 642d  ount@example-id-
-00000b40: 3137 3538 3230 2e69 616d 2e67 7365 7276  175820.iam.gserv
-00000b50: 6963 6561 6363 6f75 6e74 2e63 6f6d 600a  iceaccount.com`.
-00000b60: 0a20 2020 2030 2e20 476f 2074 6f20 796f  .    0. Go to yo
-00000b70: 7572 2064 6173 6862 6f61 7264 2073 6372  ur dashboard scr
-00000b80: 6565 6e20 616e 6420 676f 2074 6f20 2245  een and go to "E
-00000b90: 4e41 424c 4520 4150 4953 2041 4e44 2053  NABLE APIS AND S
-00000ba0: 4552 5649 4345 5322 2074 6f20 2275 6e6c  ERVICES" to "unl
-00000bb0: 6f63 6b22 2074 6865 2064 6573 6972 6564  ock" the desired
-00000bc0: 2041 5049 2063 616c 6c73 2e0a 2020 2020   API calls..    
-00000bd0: 496e 206f 7572 2065 7861 6d70 6c65 2c20  In our example, 
-00000be0: 7765 2077 696c 6c20 6a75 7374 2065 6e61  we will just ena
-00000bf0: 626c 6520 2247 6f6f 676c 6520 7368 6565  ble "Google shee
-00000c00: 7473 2041 5049 222e 0a20 2020 2021 5b5d  ts API"..    ![]
-00000c10: 2864 6f63 732f 696d 672f 656e 6162 6c65  (docs/img/enable
-00000c20: 5f61 7069 732e 504e 4729 0a20 2020 2021  _apis.PNG).    !
-00000c30: 5b5d 2864 6f63 732f 696d 672f 6163 7469  [](docs/img/acti
-00000c40: 7661 7465 5f73 6865 6574 732e 504e 4729  vate_sheets.PNG)
-00000c50: 0a0a 2323 2043 6865 636b 2074 6865 2073  ..## Check the s
-00000c60: 7065 6369 6669 6320 6372 6564 656e 7469  pecific credenti
-00000c70: 616c 7320 646f 6375 6d65 6e74 6174 696f  als documentatio
-00000c80: 6e20 6669 6c65 0a0a 5b43 7265 6465 6e74  n file..[Credent
-00000c90: 6961 6c73 2064 6f63 756d 656e 7461 7469  ials documentati
-00000ca0: 6f6e 5d28 2f64 6f63 732f 7365 7475 705f  on](/docs/setup_
-00000cb0: 6372 6564 656e 7469 616c 732e 6d64 290a  credentials.md).
-00000cc0: 0a23 2320 4d61 6e75 616c 6c79 2069 6e73  .## Manually ins
-00000cd0: 7461 6c6c 2064 6570 656e 6465 6e63 6965  tall dependencie
-00000ce0: 730a 0a60 7069 7020 696e 7374 616c 6c20  s..`pip install 
-00000cf0: 6874 7470 6c69 6232 206f 6175 7468 3263  httplib2 oauth2c
-00000d00: 6c69 656e 7420 7061 6e64 6173 2067 6f6f  lient pandas goo
-00000d10: 676c 652d 6170 692d 7079 7468 6f6e 2d63  gle-api-python-c
-00000d20: 6c69 656e 7420 676f 6f67 6c65 2e61 7574  lient google.aut
-00000d30: 682e 7472 616e 7370 6f72 742e 7265 7175  h.transport.requ
-00000d40: 6573 7473 2067 6f6f 676c 652e 6f61 7574  ests google.oaut
-00000d50: 6832 2e63 7265 6465 6e74 6961 6c73 2067  h2.credentials g
-00000d60: 6f6f 676c 655f 6175 7468 5f6f 6175 7468  oogle_auth_oauth
-00000d70: 6c69 622e 666c 6f77 600a 0a23 2320 436f  lib.flow`..## Co
-00000d80: 6d70 6c65 7465 2066 6972 7374 2075 7365  mplete first use
-00000d90: 2065 7861 6d70 6c65 0a0a 2323 2320 4578   example..### Ex
-00000da0: 616d 706c 6520 7573 696e 6720 7669 7274  ample using virt
-00000db0: 7561 6c65 6e76 2069 6e20 6261 7368 2074  ualenv in bash t
-00000dc0: 6572 6d69 6e61 6c0a 0a60 7669 7274 7561  erminal..`virtua
-00000dd0: 6c65 6e76 2076 656e 7660 0a60 7069 7020  lenv venv`.`pip 
-00000de0: 696e 7374 616c 6c20 676f 6f67 6c65 2d61  install google-a
-00000df0: 7069 2d73 7570 706f 7274 600a 6070 6970  pi-support`.`pip
-00000e00: 2069 6e73 7461 6c6c 206a 7570 7974 6572   install jupyter
-00000e10: 6c61 6260 0a60 736f 7572 6365 2076 656e  lab`.`source ven
-00000e20: 762f 5363 7269 7074 732f 6163 7469 7661  v/Scripts/activa
-00000e30: 7465 600a 6065 7870 6f72 7420 474f 4f47  te`.`export GOOG
-00000e40: 4c45 5f41 5050 4c49 4341 5449 4f4e 5f43  LE_APPLICATION_C
-00000e50: 5245 4445 4e54 4941 4c53 3d43 3a2f 7061  REDENTIALS=C:/pa
-00000e60: 7468 2f74 6f2f 6d79 2f73 6572 7669 6365  th/to/my/service
-00000e70: 5f61 6363 6f75 6e74 5f63 7265 6465 6e74  _account_credent
-00000e80: 6961 6c73 2e6a 736f 6e60 0a60 6a75 7079  ials.json`.`jupy
-00000e90: 7465 7220 6c61 6260 0a                   ter lab`.
+00000110: 3a20 7670 6572 657a 6240 7072 6f74 6f6e  : vperezb@proton
+00000120: 2e6d 650a 436c 6173 7369 6669 6572 3a20  .me.Classifier: 
+00000130: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000140: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000150: 3a20 330a 436c 6173 7369 6669 6572 3a20  : 3.Classifier: 
+00000160: 4c69 6365 6e73 6520 3a3a 2050 7562 6c69  License :: Publi
+00000170: 6320 446f 6d61 696e 0a43 6c61 7373 6966  c Domain.Classif
+00000180: 6965 723a 2044 6576 656c 6f70 6d65 6e74  ier: Development
+00000190: 2053 7461 7475 7320 3a3a 2033 202d 2041   Status :: 3 - A
+000001a0: 6c70 6861 0a44 6573 6372 6970 7469 6f6e  lpha.Description
+000001b0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+000001c0: 6578 742f 6d61 726b 646f 776e 0a4c 6963  ext/markdown.Lic
+000001d0: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
+000001e0: 5345 2e6d 640a 5265 7175 6972 6573 2d44  SE.md.Requires-D
+000001f0: 6973 743a 2067 6f6f 676c 652d 6170 692d  ist: google-api-
+00000200: 7079 7468 6f6e 2d63 6c69 656e 740a 5265  python-client.Re
+00000210: 7175 6972 6573 2d44 6973 743a 2068 7474  quires-Dist: htt
+00000220: 706c 6962 320a 5265 7175 6972 6573 2d44  plib2.Requires-D
+00000230: 6973 743a 206f 6175 7468 3263 6c69 656e  ist: oauth2clien
+00000240: 740a 5265 7175 6972 6573 2d44 6973 743a  t.Requires-Dist:
+00000250: 2070 616e 6461 730a 5265 7175 6972 6573   pandas.Requires
+00000260: 2d44 6973 743a 2067 6f6f 676c 652d 636c  -Dist: google-cl
+00000270: 6f75 642d 7374 6f72 6167 650a 5265 7175  oud-storage.Requ
+00000280: 6972 6573 2d44 6973 743a 2067 6f6f 676c  ires-Dist: googl
+00000290: 652d 6175 7468 0a52 6571 7569 7265 732d  e-auth.Requires-
+000002a0: 4469 7374 3a20 676f 6f67 6c65 5f61 7574  Dist: google_aut
+000002b0: 685f 6f61 7574 686c 6962 0a0a 2320 676f  h_oauthlib..# go
+000002c0: 6f67 6c65 2d61 7069 2d73 7570 706f 7274  ogle-api-support
+000002d0: 0a0a 536f 6d65 2066 756e 6374 696f 6e73  ..Some functions
+000002e0: 2074 6f20 6d61 6b65 2047 6f6f 676c 6520   to make Google 
+000002f0: 4150 4973 206d 6f72 6520 7573 6162 6c65  APIs more usable
+00000300: 2e0a 0a23 2320 496e 7374 616c 6c0a 0a60  ...## Install..`
+00000310: 7069 7020 696e 7374 616c 6c20 676f 6f67  pip install goog
+00000320: 6c65 2d61 7069 2d73 7570 706f 7274 600a  le-api-support`.
+00000330: 0a23 2320 436f 6e74 7269 6275 7465 0a0a  .## Contribute..
+00000340: 5468 6520 636f 6e74 7269 6275 7469 6f6e  The contribution
+00000350: 7320 6172 6520 656e 636f 7572 6167 6564  s are encouraged
+00000360: 2073 6f20 7468 6520 6c69 6272 6172 7920   so the library 
+00000370: 6361 6e20 6b65 6570 2067 726f 7769 6e67  can keep growing
+00000380: 2061 6e64 2068 656c 7020 6d6f 7265 2070   and help more p
+00000390: 656f 706c 652e 0a0a 596f 7520 6361 6e20  eople...You can 
+000003a0: 616c 736f 2063 7265 6174 6520 616e 2069  also create an i
+000003b0: 7373 7565 2069 6e20 6f72 6465 7220 746f  ssue in order to
+000003c0: 2070 6f69 6e74 206f 7468 6572 2063 6f6e   point other con
+000003d0: 7472 6962 7574 6f72 7320 746f 2064 6573  tributors to des
+000003e0: 6972 6564 2066 756e 6374 696f 6e61 6c69  ired functionali
+000003f0: 7469 6573 2e0a 0a23 2320 4675 6e63 7469  ties...## Functi
+00000400: 6f6e 7320 6176 616c 6961 626c 650a 0a2a  ons avaliable..*
+00000410: 2053 6865 6574 730a 2020 2a20 4765 7420   Sheets.  * Get 
+00000420: 7061 6e64 6173 2e64 6174 6166 7261 6d65  pandas.dataframe
+00000430: 2066 726f 6d20 5368 6565 7473 0a20 202a   from Sheets.  *
+00000440: 2055 706c 6f61 6420 7061 6e64 6173 2e64   Upload pandas.d
+00000450: 6174 6166 7261 6d65 2074 6f20 5368 6565  ataframe to Shee
+00000460: 7473 0a20 202a 2052 6574 7269 6576 6520  ts.  * Retrieve 
+00000470: 7368 6565 7420 6e61 6d65 730a 2020 2a20  sheet names.  * 
+00000480: 4164 6420 7368 6565 7473 2074 6f20 6120  Add sheets to a 
+00000490: 7370 7265 6164 7368 6565 740a 2020 2a20  spreadsheet.  * 
+000004a0: 4372 6561 7465 206e 6577 2073 7072 6561  Create new sprea
+000004b0: 6473 6865 6574 0a2a 2053 6c69 6465 730a  dsheet.* Slides.
+000004c0: 2020 2a20 4372 6561 7465 2070 7265 7365    * Create prese
+000004d0: 6e74 6174 696f 6e0a 2020 2a20 4765 7420  ntation.  * Get 
+000004e0: 7072 6573 656e 7461 7469 6f6e 2069 6e66  presentation inf
+000004f0: 6f0a 2020 2a20 4765 7420 7072 6573 656e  o.  * Get presen
+00000500: 7461 7469 6f6e 2073 6c69 6465 730a 2020  tation slides.  
+00000510: 2a20 4765 7420 736c 6964 6520 6e6f 7465  * Get slide note
+00000520: 730a 2020 2a20 5265 706c 6163 6520 7465  s.  * Replace te
+00000530: 7874 0a20 202a 2052 6570 6c61 6365 2073  xt.  * Replace s
+00000540: 6861 7065 2077 6974 6820 696d 6167 650a  hape with image.
+00000550: 2020 2a20 5265 706c 6163 6520 696d 6167    * Replace imag
+00000560: 650a 2020 2a20 4765 7420 736c 6964 6520  e.  * Get slide 
+00000570: 6e6f 7465 730a 2020 2a20 4261 7463 6820  notes.  * Batch 
+00000580: 7265 706c 6163 6520 7465 7874 0a20 202a  replace text.  *
+00000590: 2042 6174 6368 2072 6570 6c61 6365 2073   Batch replace s
+000005a0: 6861 7065 7320 7769 7468 2069 6d61 6765  hapes with image
+000005b0: 730a 2020 2a20 496e 7365 7274 2069 6d61  s.  * Insert ima
+000005c0: 6765 0a20 202a 2044 7570 6c69 6361 7465  ge.  * Duplicate
+000005d0: 206f 626a 6563 740a 2020 2a20 4465 6c65   object.  * Dele
+000005e0: 7465 206f 626a 6563 740a 2020 2a20 4261  te object.  * Ba
+000005f0: 7463 6820 6465 6c65 7465 206f 626a 6563  tch delete objec
+00000600: 740a 2020 2a20 4465 6c65 7465 2074 6578  t.  * Delete tex
+00000610: 740a 2020 2a20 4261 7463 6820 6465 6c65  t.  * Batch dele
+00000620: 7465 2074 6578 740a 2020 2a20 4465 6c65  te text.  * Dele
+00000630: 7465 2070 7265 7365 6e74 6174 696f 6e20  te presentation 
+00000640: 6e6f 7465 730a 2020 2a20 5472 616e 7366  notes.  * Transf
+00000650: 6f72 6d20 6f62 6a65 6374 0a2a 2044 7269  orm object.* Dri
+00000660: 7665 0a20 202a 2047 6574 2066 696c 6520  ve.  * Get file 
+00000670: 6e61 6d65 0a20 202a 204d 6f76 6520 6669  name.  * Move fi
+00000680: 6c65 0a20 202a 2044 656c 6574 6520 6669  le.  * Delete fi
+00000690: 6c65 0a20 202a 2043 6f70 7920 6669 6c65  le.  * Copy file
+000006a0: 0a20 202a 2055 706c 6f61 6420 696d 6167  .  * Upload imag
+000006b0: 650a 2020 2a20 4372 6561 7465 2066 6f6c  e.  * Create fol
+000006c0: 6465 720a 2020 2a20 4c69 7374 2066 6f6c  der.  * List fol
+000006d0: 6465 7273 2069 6e20 666f 6c64 6572 0a20  ders in folder. 
+000006e0: 202a 2047 6574 2066 6f6c 6465 7220 6964   * Get folder id
+000006f0: 2062 7920 6e61 6d65 0a20 202a 2047 6574   by name.  * Get
+00000700: 2066 6f6c 6465 7220 6964 2062 7920 7061   folder id by pa
+00000710: 7468 0a20 202a 2044 6f77 6e6c 6f61 6420  th.  * Download 
+00000720: 6669 6c65 0a0a 2a20 5374 6f72 6167 650a  file..* Storage.
+00000730: 2020 2a20 5570 6c6f 6164 2061 2066 696c    * Upload a fil
+00000740: 6520 746f 2067 6f6f 676c 6520 7374 6f72  e to google stor
+00000750: 6167 6520 616e 6420 6765 7420 6974 7320  age and get its 
+00000760: 5552 4c0a 0a23 2320 5374 6570 7320 746f  URL..## Steps to
+00000770: 2075 7365 2067 6f6f 676c 6520 5368 6565   use google Shee
+00000780: 7473 2041 5049 0a0a 496e 206f 7264 6572  ts API..In order
+00000790: 2074 6f20 7573 6520 476f 6f67 6c65 2041   to use Google A
+000007a0: 5049 7320 796f 7520 7769 6c6c 206e 6565  PIs you will nee
+000007b0: 6420 746f 2061 7574 6865 6e74 6963 6174  d to authenticat
+000007c0: 652c 2074 6869 7320 7374 6570 7320 6775  e, this steps gu
+000007d0: 6964 6520 796f 7520 7468 726f 7567 6820  ide you through 
+000007e0: 7468 6520 7072 6f63 6573 733a 0a0a 302e  the process:..0.
+000007f0: 2043 7265 6174 6520 6120 7072 6f6a 6563   Create a projec
+00000800: 7420 696e 2063 6f6e 736f 6c65 2e64 6576  t in console.dev
+00000810: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
+00000820: 6f6d 0a0a 3c68 7474 7073 3a2f 2f63 6f6e  om..<https://con
+00000830: 736f 6c65 2e64 6576 656c 6f70 6572 732e  sole.developers.
+00000840: 676f 6f67 6c65 2e63 6f6d 3e0a 0a30 2e20  google.com>..0. 
+00000850: 4372 6561 7465 2067 6f6f 676c 6520 7365  Create google se
+00000860: 7276 6963 6520 6163 636f 756e 742e 0a20  rvice account.. 
+00000870: 2020 2030 2e20 476f 2074 6f20 3c68 7474     0. Go to <htt
+00000880: 7073 3a2f 2f63 6f6e 736f 6c65 2e64 6576  ps://console.dev
+00000890: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
+000008a0: 6f6d 2f70 726f 6a65 6374 7365 6c65 6374  om/projectselect
+000008b0: 6f72 2f61 7069 732f 6372 6564 656e 7469  or/apis/credenti
+000008c0: 616c 733e 2061 6e64 2063 7265 6174 6520  als> and create 
+000008d0: 6120 6e65 7720 7072 6f6a 6563 742e 0a20  a new project.. 
+000008e0: 2020 2021 5b43 7265 6174 6520 6120 6465     ![Create a de
+000008f0: 7665 6c6f 7065 7273 2070 726f 6a65 6374  velopers project
+00000900: 5d28 646f 6373 2f69 6d67 2f63 7265 6174  ](docs/img/creat
+00000910: 655f 7072 6f6a 6563 742e 504e 4729 0a0a  e_project.PNG)..
+00000920: 2020 2020 302e 2043 7265 6174 6520 6372      0. Create cr
+00000930: 6564 656e 7469 616c 732e 0a20 2020 2021  edentials..    !
+00000940: 5b5d 2864 6f63 732f 696d 672f 6368 6f6f  [](docs/img/choo
+00000950: 7365 5f63 7265 6465 6e74 6961 6c73 2e50  se_credentials.P
+00000960: 4e47 290a 2020 2020 2020 2020 2a20 496e  NG).        * In
+00000970: 2074 6869 7320 6669 7273 7420 7665 7273   this first vers
+00000980: 696f 6e2c 2069 2077 696c 6c20 6578 706c  ion, i will expl
+00000990: 6169 6e20 686f 7720 746f 2064 6561 6c20  ain how to deal 
+000009a0: 7769 7468 2053 6572 7669 6365 7320 6163  with Services ac
+000009b0: 636f 756e 7473 2c20 736f 2073 656c 6563  counts, so selec
+000009c0: 7420 2253 6572 7669 6365 2061 6363 6f75  t "Service accou
+000009d0: 6e74 206b 6579 222e 0a0a 2020 2020 302e  nt key"...    0.
+000009e0: 2043 7265 6174 6520 6120 7365 7276 6963   Create a servic
+000009f0: 6520 6163 636f 756e 742e 0a20 2020 2021  e account..    !
+00000a00: 5b5d 2864 6f63 732f 696d 672f 6372 6561  [](docs/img/crea
+00000a10: 7465 5f73 6572 7669 6365 5f61 6363 6f75  te_service_accou
+00000a20: 6e74 2e50 4e47 290a 2020 2020 2020 2020  nt.PNG).        
+00000a30: 2a20 446f 776e 6c6f 6164 2074 6865 202e  * Download the .
+00000a40: 6a73 6f6e 2066 696c 6520 616e 6420 4b45  json file and KE
+00000a50: 4550 2049 5420 5341 4645 2e0a 0a20 2020  EP IT SAFE...   
+00000a60: 2030 2e20 4e6f 7720 796f 7520 6861 7665   0. Now you have
+00000a70: 2079 6f75 7220 7365 7276 6963 6520 6163   your service ac
+00000a80: 636f 756e 7420 6372 6561 7465 6420 696e  count created in
+00000a90: 7369 6465 2079 6f75 7220 6e65 7720 7072  side your new pr
+00000aa0: 6f6a 6563 742e 0a20 2020 2021 5b5d 2864  oject..    ![](d
+00000ab0: 6f63 732f 696d 672f 6372 6561 7465 5f73  ocs/img/create_s
+00000ac0: 6572 7669 6365 5f61 6363 6f75 6e74 2e50  ervice_account.P
+00000ad0: 4e47 290a 0a20 2020 2030 2e20 436f 7079  NG)..    0. Copy
+00000ae0: 2079 6f75 7220 2275 7365 7220 6964 2220   your "user id" 
+00000af0: 696e 2022 4d61 6e61 6765 2073 6572 7669  in "Manage servi
+00000b00: 6365 2061 6363 6f75 6e74 7322 2074 6f20  ce accounts" to 
+00000b10: 7573 6520 6974 206c 6174 6572 2e0a 2020  use it later..  
+00000b20: 2020 2020 2020 2a20 4974 206c 6f6f 6b73        * It looks
+00000b30: 206c 696b 6520 7468 6973 206f 6e65 3a20   like this one: 
+00000b40: 6066 6972 7374 2d73 6572 7669 6365 2d61  `first-service-a
+00000b50: 6363 6f75 6e74 4065 7861 6d70 6c65 2d69  ccount@example-i
+00000b60: 642d 3137 3538 3230 2e69 616d 2e67 7365  d-175820.iam.gse
+00000b70: 7276 6963 6561 6363 6f75 6e74 2e63 6f6d  rviceaccount.com
+00000b80: 600a 0a20 2020 2030 2e20 476f 2074 6f20  `..    0. Go to 
+00000b90: 796f 7572 2064 6173 6862 6f61 7264 2073  your dashboard s
+00000ba0: 6372 6565 6e20 616e 6420 676f 2074 6f20  creen and go to 
+00000bb0: 2245 4e41 424c 4520 4150 4953 2041 4e44  "ENABLE APIS AND
+00000bc0: 2053 4552 5649 4345 5322 2074 6f20 2275   SERVICES" to "u
+00000bd0: 6e6c 6f63 6b22 2074 6865 2064 6573 6972  nlock" the desir
+00000be0: 6564 2041 5049 2063 616c 6c73 2e0a 2020  ed API calls..  
+00000bf0: 2020 496e 206f 7572 2065 7861 6d70 6c65    In our example
+00000c00: 2c20 7765 2077 696c 6c20 6a75 7374 2065  , we will just e
+00000c10: 6e61 626c 6520 2247 6f6f 676c 6520 7368  nable "Google sh
+00000c20: 6565 7473 2041 5049 222e 0a20 2020 2021  eets API"..    !
+00000c30: 5b5d 2864 6f63 732f 696d 672f 656e 6162  [](docs/img/enab
+00000c40: 6c65 5f61 7069 732e 504e 4729 0a20 2020  le_apis.PNG).   
+00000c50: 2021 5b5d 2864 6f63 732f 696d 672f 6163   ![](docs/img/ac
+00000c60: 7469 7661 7465 5f73 6865 6574 732e 504e  tivate_sheets.PN
+00000c70: 4729 0a0a 2323 2043 6865 636b 2074 6865  G)..## Check the
+00000c80: 2073 7065 6369 6669 6320 6372 6564 656e   specific creden
+00000c90: 7469 616c 7320 646f 6375 6d65 6e74 6174  tials documentat
+00000ca0: 696f 6e20 6669 6c65 0a0a 5b43 7265 6465  ion file..[Crede
+00000cb0: 6e74 6961 6c73 2064 6f63 756d 656e 7461  ntials documenta
+00000cc0: 7469 6f6e 5d28 2f64 6f63 732f 7365 7475  tion](/docs/setu
+00000cd0: 705f 6372 6564 656e 7469 616c 732e 6d64  p_credentials.md
+00000ce0: 290a 0a23 2320 4d61 6e75 616c 6c79 2069  )..## Manually i
+00000cf0: 6e73 7461 6c6c 2064 6570 656e 6465 6e63  nstall dependenc
+00000d00: 6965 730a 0a60 7069 7020 696e 7374 616c  ies..`pip instal
+00000d10: 6c20 6874 7470 6c69 6232 206f 6175 7468  l httplib2 oauth
+00000d20: 3263 6c69 656e 7420 7061 6e64 6173 2067  2client pandas g
+00000d30: 6f6f 676c 652d 6170 692d 7079 7468 6f6e  oogle-api-python
+00000d40: 2d63 6c69 656e 7420 676f 6f67 6c65 2e61  -client google.a
+00000d50: 7574 682e 7472 616e 7370 6f72 742e 7265  uth.transport.re
+00000d60: 7175 6573 7473 2067 6f6f 676c 652e 6f61  quests google.oa
+00000d70: 7574 6832 2e63 7265 6465 6e74 6961 6c73  uth2.credentials
+00000d80: 2067 6f6f 676c 655f 6175 7468 5f6f 6175   google_auth_oau
+00000d90: 7468 6c69 622e 666c 6f77 600a 0a23 2320  thlib.flow`..## 
+00000da0: 436f 6d70 6c65 7465 2066 6972 7374 2075  Complete first u
+00000db0: 7365 2065 7861 6d70 6c65 0a0a 2323 2320  se example..### 
+00000dc0: 4578 616d 706c 6520 7573 696e 6720 7669  Example using vi
+00000dd0: 7274 7561 6c65 6e76 2069 6e20 6261 7368  rtualenv in bash
+00000de0: 2074 6572 6d69 6e61 6c0a 0a60 7669 7274   terminal..`virt
+00000df0: 7561 6c65 6e76 2076 656e 7660 0a60 7069  ualenv venv`.`pi
+00000e00: 7020 696e 7374 616c 6c20 676f 6f67 6c65  p install google
+00000e10: 2d61 7069 2d73 7570 706f 7274 600a 6070  -api-support`.`p
+00000e20: 6970 2069 6e73 7461 6c6c 206a 7570 7974  ip install jupyt
+00000e30: 6572 6c61 6260 0a60 736f 7572 6365 2076  erlab`.`source v
+00000e40: 656e 762f 5363 7269 7074 732f 6163 7469  env/Scripts/acti
+00000e50: 7661 7465 600a 6065 7870 6f72 7420 474f  vate`.`export GO
+00000e60: 4f47 4c45 5f41 5050 4c49 4341 5449 4f4e  OGLE_APPLICATION
+00000e70: 5f43 5245 4445 4e54 4941 4c53 3d43 3a2f  _CREDENTIALS=C:/
+00000e80: 7061 7468 2f74 6f2f 6d79 2f73 6572 7669  path/to/my/servi
+00000e90: 6365 5f61 6363 6f75 6e74 5f63 7265 6465  ce_account_crede
+00000ea0: 6e74 6961 6c73 2e6a 736f 6e60 0a60 6a75  ntials.json`.`ju
+00000eb0: 7079 7465 7220 6c61 6260 0a0a 2323 2053  pyter lab`..## S
+00000ec0: 6574 7570 2074 6f20 6465 7665 6c6f 7065  etup to develope
+00000ed0: 6d65 6e74 0a0a 6076 6972 7475 616c 656e  ment..`virtualen
+00000ee0: 7620 7665 6e76 600a 6070 6970 2069 6e73  v venv`.`pip ins
+00000ef0: 7461 6c6c 202e 600a 6070 6970 2069 6e73  tall .`.`pip ins
+00000f00: 7461 6c6c 206a 7570 7974 6572 6c61 6260  tall jupyterlab`
+00000f10: 0a60 736f 7572 6365 2076 656e 762f 5363  .`source venv/Sc
+00000f20: 7269 7074 732f 6163 7469 7661 7465 600a  ripts/activate`.
+00000f30: 6065 7870 6f72 7420 474f 4f47 4c45 5f41  `export GOOGLE_A
+00000f40: 5050 4c49 4341 5449 4f4e 5f43 5245 4445  PPLICATION_CREDE
+00000f50: 4e54 4941 4c53 3d43 3a2f 7061 7468 2f74  NTIALS=C:/path/t
+00000f60: 6f2f 6d79 2f73 6572 7669 6365 5f61 6363  o/my/service_acc
+00000f70: 6f75 6e74 5f63 7265 6465 6e74 6961 6c73  ount_credentials
+00000f80: 2e6a 736f 6e60 0a60 6a75 7079 7465 7220  .json`.`jupyter 
+00000f90: 6c61 6260 0a                             lab`.
```

### Comparing `google-api-support-0.1.4/setup.py` & `google_api_support-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="google-api-support",
-    version="0.1.4",
+    version="0.1.7",
     author="Víctor Pérez Berruezo",
-    author_email="victor.perez.berruezo@gmail.com",
+    author_email="vperezb@proton.me",
     description="In this package you will find functions to deal with google apis. Sheets, Drive, Storage and Slides",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vperezb/google-api-support",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `google-api-support-0.1.4/test/test_spreadsheets.py` & `google_api_support-0.1.7/test/test_spreadsheets.py`

 * *Files identical despite different names*

