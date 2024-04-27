# Comparing `tmp/DocumentAI_std-0.2.5.dev1.tar.gz` & `tmp/DocumentAI_std-0.2.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DocumentAI_std-0.2.5.dev1.tar", last modified: Mon Apr  8 16:32:57 2024, max compression
+gzip compressed data, was "DocumentAI_std-0.2.6.dev1.tar", last modified: Fri Apr 26 17:23:04 2024, max compression
```

## Comparing `DocumentAI_std-0.2.5.dev1.tar` & `DocumentAI_std-0.2.6.dev1.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-04-08 16:32:57.365007 DocumentAI_std-0.2.5.dev1/
-drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-04-08 16:32:57.361675 DocumentAI_std-0.2.5.dev1/DocumentAI_std/
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        0 2024-02-13 09:46:28.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std/__init__.py
-drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-04-08 16:32:57.365007 DocumentAI_std-0.2.5.dev1/DocumentAI_std/base/
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        0 2024-02-13 09:46:28.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std/base/__init__.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     4851 2024-03-12 10:10:29.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std/base/doc_element.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     3296 2024-03-12 09:46:38.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std/base/doc_element_classification.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     3723 2024-03-05 18:02:12.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std/base/doc_enum.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     5867 2024-03-12 09:44:24.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std/base/document.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     2694 2024-03-12 10:36:03.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std/base/document_entity_classification.py
-drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-04-08 16:32:57.365007 DocumentAI_std-0.2.5.dev1/DocumentAI_std/datasets/
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        0 2024-02-13 09:46:28.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std/datasets/__init__.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     2822 2024-02-21 12:00:42.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std/datasets/wildreceipt.py
-drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-04-08 16:32:57.365007 DocumentAI_std-0.2.5.dev1/DocumentAI_std/utils/
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     7727 2024-04-08 12:26:36.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std/utils/OCR_adapter.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        0 2024-02-13 10:23:11.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std/utils/__init__.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      708 2024-02-21 11:59:46.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std/utils/base_utils.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     4855 2024-03-26 08:47:18.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std/utils/image_utils.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     6919 2024-03-09 14:06:30.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std/utils/layout_utils.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     7406 2024-03-05 17:11:24.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std/utils/text_utils.py
-drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-04-08 16:32:57.361675 DocumentAI_std-0.2.5.dev1/DocumentAI_std.egg-info/
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      190 2024-04-08 16:32:57.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std.egg-info/PKG-INFO
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      793 2024-04-08 16:32:57.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std.egg-info/SOURCES.txt
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        1 2024-04-08 16:32:57.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std.egg-info/dependency_links.txt
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      143 2024-04-08 16:32:57.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std.egg-info/requires.txt
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)       15 2024-04-08 16:32:57.000000 DocumentAI_std-0.2.5.dev1/DocumentAI_std.egg-info/top_level.txt
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        0 2024-01-24 16:32:43.000000 DocumentAI_std-0.2.5.dev1/LICENSE
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)       24 2024-04-07 11:51:59.000000 DocumentAI_std-0.2.5.dev1/MANIFEST.in
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      190 2024-04-08 16:32:57.365007 DocumentAI_std-0.2.5.dev1/PKG-INFO
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     1571 2024-02-21 12:09:25.000000 DocumentAI_std-0.2.5.dev1/README.md
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      143 2024-04-08 16:31:54.000000 DocumentAI_std-0.2.5.dev1/requirements.txt
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)       38 2024-04-08 16:32:57.365007 DocumentAI_std-0.2.5.dev1/setup.cfg
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      720 2024-04-08 16:32:16.000000 DocumentAI_std-0.2.5.dev1/setup.py
+drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-04-26 17:23:04.541039 DocumentAI_std-0.2.6.dev1/
+drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-04-26 17:23:04.541039 DocumentAI_std-0.2.6.dev1/DocumentAI_std/
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        0 2024-02-13 09:46:28.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std/__init__.py
+drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-04-26 17:23:04.541039 DocumentAI_std-0.2.6.dev1/DocumentAI_std/base/
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        0 2024-02-13 09:46:28.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std/base/__init__.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     4851 2024-03-12 10:10:29.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std/base/doc_element.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     3296 2024-03-12 09:46:38.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std/base/doc_element_classification.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     3723 2024-03-05 18:02:12.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std/base/doc_enum.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     5867 2024-03-12 09:44:24.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std/base/document.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     2694 2024-03-12 10:36:03.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std/base/document_entity_classification.py
+drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-04-26 17:23:04.541039 DocumentAI_std-0.2.6.dev1/DocumentAI_std/datasets/
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        0 2024-02-13 09:46:28.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std/datasets/__init__.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     4242 2024-04-26 14:57:10.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std/datasets/cord.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     2622 2024-04-26 14:58:56.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std/datasets/funsd.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     2814 2024-04-26 11:41:52.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std/datasets/wildreceipt.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     2678 2024-04-26 16:29:42.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std/datasets/xfund.py
+drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-04-26 17:23:04.541039 DocumentAI_std-0.2.6.dev1/DocumentAI_std/utils/
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     7774 2024-04-26 10:47:09.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std/utils/OCR_adapter.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        0 2024-02-13 10:23:11.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std/utils/__init__.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     4515 2024-04-26 14:57:10.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std/utils/base_utils.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     4855 2024-03-26 08:47:18.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std/utils/image_utils.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     6919 2024-03-09 14:06:30.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std/utils/layout_utils.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     7406 2024-03-05 17:11:24.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std/utils/text_utils.py
+drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-04-26 17:23:04.541039 DocumentAI_std-0.2.6.dev1/DocumentAI_std.egg-info/
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      190 2024-04-26 17:23:04.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std.egg-info/PKG-INFO
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      891 2024-04-26 17:23:04.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std.egg-info/SOURCES.txt
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        1 2024-04-26 17:23:04.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std.egg-info/dependency_links.txt
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      143 2024-04-26 17:23:04.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std.egg-info/requires.txt
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)       15 2024-04-26 17:23:04.000000 DocumentAI_std-0.2.6.dev1/DocumentAI_std.egg-info/top_level.txt
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        0 2024-01-24 16:32:43.000000 DocumentAI_std-0.2.6.dev1/LICENSE
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)       24 2024-04-07 11:51:59.000000 DocumentAI_std-0.2.6.dev1/MANIFEST.in
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      190 2024-04-26 17:23:04.541039 DocumentAI_std-0.2.6.dev1/PKG-INFO
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     1571 2024-02-21 12:09:25.000000 DocumentAI_std-0.2.6.dev1/README.md
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      143 2024-04-08 16:31:54.000000 DocumentAI_std-0.2.6.dev1/requirements.txt
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)       38 2024-04-26 17:23:04.541039 DocumentAI_std-0.2.6.dev1/setup.cfg
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      589 2024-04-26 17:22:58.000000 DocumentAI_std-0.2.6.dev1/setup.py
```

### Comparing `DocumentAI_std-0.2.5.dev1/DocumentAI_std/base/doc_element.py` & `DocumentAI_std-0.2.6.dev1/DocumentAI_std/base/doc_element.py`

 * *Files identical despite different names*

### Comparing `DocumentAI_std-0.2.5.dev1/DocumentAI_std/base/doc_element_classification.py` & `DocumentAI_std-0.2.6.dev1/DocumentAI_std/base/doc_element_classification.py`

 * *Files identical despite different names*

### Comparing `DocumentAI_std-0.2.5.dev1/DocumentAI_std/base/doc_enum.py` & `DocumentAI_std-0.2.6.dev1/DocumentAI_std/base/doc_enum.py`

 * *Files identical despite different names*

### Comparing `DocumentAI_std-0.2.5.dev1/DocumentAI_std/base/document.py` & `DocumentAI_std-0.2.6.dev1/DocumentAI_std/base/document.py`

 * *Files identical despite different names*

### Comparing `DocumentAI_std-0.2.5.dev1/DocumentAI_std/base/document_entity_classification.py` & `DocumentAI_std-0.2.6.dev1/DocumentAI_std/base/document_entity_classification.py`

 * *Files identical despite different names*

### Comparing `DocumentAI_std-0.2.5.dev1/DocumentAI_std/datasets/wildreceipt.py` & `DocumentAI_std-0.2.6.dev1/DocumentAI_std/datasets/wildreceipt.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             img_path = json_data["file_name"]
             annotations = json_data["annotations"]
 
             box_targets, text_targets, label_targets = zip(
                 *[
                     (
                         BaseUtils.X1X2X3X4_to_xywh(annotation["box"]),
-                        annotation["text"].lower(),
+                        annotation["text"],
                         annotation["label"],
                     )
                     for annotation in annotations
                 ]
             )
 
             ocr_output = {
```

### Comparing `DocumentAI_std-0.2.5.dev1/DocumentAI_std/utils/OCR_adapter.py` & `DocumentAI_std-0.2.6.dev1/DocumentAI_std/utils/OCR_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,18 @@
         Args:
             easy_ocr_output (list): List containing OCR output from EasyOCR engine.
 
         Returns:
             dict: Dictionary containing standardized OCR output with 'bbox' and 'content' keys.
         """
         bbox_content_pairs = [
-            (list(map(int, BaseUtils.X1X2X3X4_to_xywh(sum(text_box[0], [])))), text_box[1])
+            (
+                list(map(int, BaseUtils.X1X2X3X4_to_xywh(sum(text_box[0], [])))),
+                text_box[1],
+            )
             for text_box in easy_ocr_output
         ]
 
         bbox, content = zip(*bbox_content_pairs)
 
         return {"bbox": list(bbox), "content": list(content)}
```

### Comparing `DocumentAI_std-0.2.5.dev1/DocumentAI_std/utils/image_utils.py` & `DocumentAI_std-0.2.6.dev1/DocumentAI_std/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `DocumentAI_std-0.2.5.dev1/DocumentAI_std/utils/layout_utils.py` & `DocumentAI_std-0.2.6.dev1/DocumentAI_std/utils/layout_utils.py`

 * *Files identical despite different names*

### Comparing `DocumentAI_std-0.2.5.dev1/DocumentAI_std/utils/text_utils.py` & `DocumentAI_std-0.2.6.dev1/DocumentAI_std/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `DocumentAI_std-0.2.5.dev1/DocumentAI_std.egg-info/SOURCES.txt` & `DocumentAI_std-0.2.6.dev1/DocumentAI_std.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 DocumentAI_std/base/__init__.py
 DocumentAI_std/base/doc_element.py
 DocumentAI_std/base/doc_element_classification.py
 DocumentAI_std/base/doc_enum.py
 DocumentAI_std/base/document.py
 DocumentAI_std/base/document_entity_classification.py
 DocumentAI_std/datasets/__init__.py
+DocumentAI_std/datasets/cord.py
+DocumentAI_std/datasets/funsd.py
 DocumentAI_std/datasets/wildreceipt.py
+DocumentAI_std/datasets/xfund.py
 DocumentAI_std/utils/OCR_adapter.py
 DocumentAI_std/utils/__init__.py
 DocumentAI_std/utils/base_utils.py
 DocumentAI_std/utils/image_utils.py
 DocumentAI_std/utils/layout_utils.py
 DocumentAI_std/utils/text_utils.py
```

### Comparing `DocumentAI_std-0.2.5.dev1/README.md` & `DocumentAI_std-0.2.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `DocumentAI_std-0.2.5.dev1/setup.py` & `DocumentAI_std-0.2.6.dev1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="DocumentAI_std",
-    version="0.2.5.dev1",
+    version="0.2.6.dev1",
     # packages=find_packages(where='DocumentAI_std'),  # Include all packages within this directory
     packages=find_packages(exclude=["DocumentAI_std.tests"]),
     # package_dir={'': 'DocumentAI_std'},  # Set root package directory
     install_requires=required,
     url="",
     license="",
     author="Hamza Gbada",
     author_email="",
     description="The main standards for Latis Document AI project",
 )
-# TODO: about tesseract: https://stackoverflow.com/questions/63048908/how-do-i-install-a-new-language-pack-for-tesseract-on-windows
```

