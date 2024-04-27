# Comparing `tmp/receipt_enhancer-0.1.4.tar.gz` & `tmp/receipt_enhancer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "receipt_enhancer-0.1.4.tar", max compression
+gzip compressed data, was "receipt_enhancer-0.1.5.tar", max compression
```

## Comparing `receipt_enhancer-0.1.4.tar` & `receipt_enhancer-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2024-03-06 17:46:27.092848 receipt_enhancer-0.1.4/LICENSE
--rw-r--r--   0        0        0     2381 2024-03-06 18:00:03.264872 receipt_enhancer-0.1.4/README.md
--rw-r--r--   0        0        0      500 2024-04-24 04:37:03.946422 receipt_enhancer-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       93 2024-03-06 17:48:19.540852 receipt_enhancer-0.1.4/receipt_enhancer/__init__.py
--rw-r--r--   0        0        0    15106 2024-04-24 04:30:27.650411 receipt_enhancer-0.1.4/receipt_enhancer/receipt_enhancer.py
--rw-r--r--   0        0        0     3188 1970-01-01 00:00:00.000000 receipt_enhancer-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-26 23:46:02.339918 receipt_enhancer-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2381 2024-04-26 23:46:02.339918 receipt_enhancer-0.1.5/README.md
+-rw-r--r--   0        0        0      500 2024-04-26 23:55:19.491916 receipt_enhancer-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       93 2024-04-26 23:46:02.339918 receipt_enhancer-0.1.5/receipt_enhancer/__init__.py
+-rw-r--r--   0        0        0    15114 2024-04-26 23:53:11.519916 receipt_enhancer-0.1.5/receipt_enhancer/receipt_enhancer.py
+-rw-r--r--   0        0        0     3188 1970-01-01 00:00:00.000000 receipt_enhancer-0.1.5/PKG-INFO
```

### Comparing `receipt_enhancer-0.1.4/LICENSE` & `receipt_enhancer-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `receipt_enhancer-0.1.4/README.md` & `receipt_enhancer-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `receipt_enhancer-0.1.4/receipt_enhancer/receipt_enhancer.py` & `receipt_enhancer-0.1.5/receipt_enhancer/receipt_enhancer.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
 
         return max(0, min(5, best_clip_limit))
 
     def __reduce_noise_and_texture(self, block):
 
         f_transform = np.fft.fft2(block)
         f_transform_shifted = np.fft.fftshift(f_transform)
-        magnitude_spectrum = 20 * np.log(np.abs(f_transform_shifted))
+        magnitude_spectrum = 20 * np.log(np.abs(f_transform_shifted) + 1e-10)
         _, thresholded_spectrum = cv2.threshold(magnitude_spectrum, np.mean(magnitude_spectrum), 255, cv2.THRESH_BINARY)
 
         high_frequency_mask = np.fft.ifftshift(thresholded_spectrum)
         high_frequency_mask = np.fft.ifft2(high_frequency_mask)
         high_frequency_mask = np.abs(high_frequency_mask)
 
         high_frequency_mask = cv2.normalize(high_frequency_mask, None, alpha=0, beta=1, norm_type=cv2.NORM_MINMAX)
```

### Comparing `receipt_enhancer-0.1.4/PKG-INFO` & `receipt_enhancer-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: receipt-enhancer
-Version: 0.1.4
+Version: 0.1.5
 Summary: This module is essential for preprocessing receipt images to improve visual quality and facilitate automatic analysis.
 License: MIT
 Keywords: document,nfe,invoice,receipt
 Author: Ricardo Castro
 Author-email: srrenks@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

