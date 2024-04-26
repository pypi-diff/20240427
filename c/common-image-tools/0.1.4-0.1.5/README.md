# Comparing `tmp/common_image_tools-0.1.4.tar.gz` & `tmp/common_image_tools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common_image_tools-0.1.4.tar", max compression
+gzip compressed data, was "common_image_tools-0.1.5.tar", max compression
```

## Comparing `common_image_tools-0.1.4.tar` & `common_image_tools-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-05-06 18:16:59.565000 common_image_tools-0.1.4/common_image_tools/__init__.py
--rw-r--r--   0        0        0     1730 2024-03-14 17:59:43.827812 common_image_tools-0.1.4/common_image_tools/conversion.py
--rw-r--r--   0        0        0     2125 2024-03-22 20:01:36.418214 common_image_tools-0.1.4/common_image_tools/operation.py
--rw-r--r--   0        0        0     5383 2024-03-22 20:03:18.254145 common_image_tools-0.1.4/common_image_tools/tool.py
--rw-r--r--   0        0        0      415 2024-03-15 00:42:27.227417 common_image_tools-0.1.4/common_image_tools/verification.py
--rw-r--r--   0        0        0      252 2024-03-15 00:41:36.599604 common_image_tools-0.1.4/common_image_tools/visualization.py
--rw-r--r--   0        0        0      530 2024-03-22 20:02:39.725904 common_image_tools-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      834 2023-07-13 16:44:25.164546 common_image_tools-0.1.4/README.md
--rw-r--r--   0        0        0     1508 1970-01-01 00:00:00.000000 common_image_tools-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 18:16:59.565000 common_image_tools-0.1.5/common_image_tools/__init__.py
+-rw-r--r--   0        0        0     2768 2024-04-26 23:47:44.007193 common_image_tools-0.1.5/common_image_tools/conversion.py
+-rw-r--r--   0        0        0     2180 2024-04-26 23:47:44.020791 common_image_tools-0.1.5/common_image_tools/operation.py
+-rw-r--r--   0        0        0     5816 2024-04-26 23:47:44.043038 common_image_tools-0.1.5/common_image_tools/tool.py
+-rw-r--r--   0        0        0     1359 2024-04-26 23:47:44.057023 common_image_tools-0.1.5/common_image_tools/verification.py
+-rw-r--r--   0        0        0      266 2024-04-26 23:47:44.073210 common_image_tools-0.1.5/common_image_tools/visualization.py
+-rw-r--r--   0        0        0      607 2024-04-26 23:47:44.088914 common_image_tools-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      832 2024-04-26 23:47:44.005195 common_image_tools-0.1.5/README.md
+-rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 common_image_tools-0.1.5/PKG-INFO
```

### Comparing `common_image_tools-0.1.4/common_image_tools/operation.py` & `common_image_tools-0.1.5/common_image_tools/operation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,15 @@
+# -*- coding: utf-8 -*-
+from math import ceil
+
 import cv2
 import numpy as np
-from math import ceil
 
 
 def resize_image_with_aspect_ratio(image: np.ndarray, size: tuple[int, int]) -> np.ndarray:
-    """
-    Resize an image while maintaining its aspect ratio using OpenCV.
-
-    """
     height, width = size
 
     # Calculate the aspect ratio
     aspect_ratio = width / float(height)
 
     # Calculate new dimensions while preserving the aspect ratio
     if image.shape[1] / image.shape[0] > aspect_ratio:
@@ -46,27 +44,30 @@
     # signed distance between the point and the nearest contour edge.
     result = cv2.pointPolygonTest(ctn, point, measureDist=False)
 
     return result >= 0
 
 
 def scale_bboxes(bboxes: list[tuple], scale_factor: float) -> list[tuple]:
-    """Ridimensiona i rettangoli per il fattore passato come parametro
-
-    :param bboxes: Lista di rettangoli da ridimensionare
-    :param scale_factor: Valore moltiplicativo
-    :return: Lista di rettangoli ridimensionati
-    """
     f_bboxes = []
     for box in bboxes:
         x, y, w, h = box
         f_bboxes.append(
             (ceil(x * scale_factor), ceil(y * scale_factor), ceil(w * scale_factor), ceil(h * scale_factor)))
 
     return f_bboxes
 
 
-def bbox_centroid(bbox):
+def bbox_centroid(bbox: tuple[int, int, int, int]) -> tuple[int, int]:
+    """
+    Calculate the centroid coordinates of a bounding box.
+
+    Parameters:
+        bbox (tuple): A tuple representing the bounding box in the format (x, y, width, height).
+
+    Returns:
+        tuple: A tuple containing the coordinates of the centroid as integers (center_x, center_y).
+    """
     x, y, w, h = bbox
     center_x = x + (w / 2)
     center_y = y + (h / 2)
     return int(center_x), int(center_y)
```

### Comparing `common_image_tools-0.1.4/common_image_tools/tool.py` & `common_image_tools-0.1.5/common_image_tools/tool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 import cv2
 import numpy as np
 from PIL import Image
 
 
 def opencv_built_with_gstreamer() -> bool:
     """Check if OpenCV has been built with GStreamer support.
@@ -142,20 +143,26 @@
         PIL.Image: Image in PIL format (RGB)
     """
     from PIL import Image
 
     return Image.new("RGB", size, color)
 
 
-def create_cv2_image(size: tuple, color: tuple) -> np.ndarray:
-    """Create a cv2 image with the specified color and size.
+def create_cv2_image(size: tuple[int, int], color: tuple[int, int, int]) -> np.ndarray:
+    """
+    Creates a NumPy array representing an image using OpenCV conventions.
 
-    Args:
-        size (tuple): Size of the image
-        color (tuple): Color of the image in BGR format
+    Parameters:
+        size (tuple[int, int]): A tuple specifying the dimensions of the image in the format (height, width).
+        color (tuple[int, int, int]): A tuple representing the color of the image in BGR (Blue, Green, Red) format.
 
     Returns:
-        np.ndarray: Image in opencv format (BGR)
+        np.ndarray: An image represented as a NumPy array with dimensions (height, width, 3).
+                    Each pixel in the image will have the specified color.
+
+    Example:
+        >>> create_cv2_image((100, 200), (0, 255, 0))
+        Returns a 100x200 green image.
     """
     img = np.zeros((size[0], size[1], 3), np.uint8)
     img[:] = color
     return img
```

### Comparing `common_image_tools-0.1.4/pyproject.toml` & `common_image_tools-0.1.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 [tool.poetry]
 name = "common-image-tools"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Federico Lanzani <federico@federicolanzani.com>"]
 readme = "README.md"
 packages = [{include = "common_image_tools"}]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 pillow = ">=9.5.0"
 opencv-python = "~4.8.0.76"
 color-transfer = "^0.1"
 scikit-image = "^0.21.0"
-dlib = "^19.24.2"
+dlib = "^19.20.0"
 
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 matplotlib = "^3.7.2"
+pre-commit = "^3.5.0"
+pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
+mypy = "^1.9.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-
```

### Comparing `common_image_tools-0.1.4/README.md` & `common_image_tools-0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Common Image Tools
 
 ## Description
-common_image_tools is a repository containing a curated collection of commonly used image manipulation functions for 
-computer vision projects. These tools provide a set of handy functions for performing various image processing tasks, 
+common_image_tools is a repository containing a curated collection of commonly used image manipulation functions for
+computer vision projects. These tools provide a set of handy functions for performing various image processing tasks,
 such as resizing, cropping, filtering, and more.
 
 ## Installation
 To install common_image_tools, simply run the following command:
 ```bash
 pip install common-image-tools
 ```
@@ -17,12 +17,12 @@
 
 ### Conversion
 
 ### Visualization
 
 
 ## Contributing
-Contributions are welcome! If you have any suggestions, improvements, or new features to add, please open an issue or 
+Contributions are welcome! If you have any suggestions, improvements, or new features to add, please open an issue or
 submit a pull request. Make sure to follow the existing coding style and include appropriate tests.
 
 ## License
-This project is licensed under the MIT License - see the LICENSE file for details.
+This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `common_image_tools-0.1.4/PKG-INFO` & `common_image_tools-0.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: common-image-tools
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Federico Lanzani
 Author-email: federico@federicolanzani.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: color-transfer (>=0.1,<0.2)
-Requires-Dist: dlib (>=19.24.2,<20.0.0)
+Requires-Dist: dlib (>=19.20.0,<20.0.0)
 Requires-Dist: opencv-python (>=4.8.0.76,<4.9.0.0)
 Requires-Dist: pillow (>=9.5.0)
 Requires-Dist: scikit-image (>=0.21.0,<0.22.0)
 Description-Content-Type: text/markdown
 
 # Common Image Tools
 
 ## Description
-common_image_tools is a repository containing a curated collection of commonly used image manipulation functions for 
-computer vision projects. These tools provide a set of handy functions for performing various image processing tasks, 
+common_image_tools is a repository containing a curated collection of commonly used image manipulation functions for
+computer vision projects. These tools provide a set of handy functions for performing various image processing tasks,
 such as resizing, cropping, filtering, and more.
 
 ## Installation
 To install common_image_tools, simply run the following command:
 ```bash
 pip install common-image-tools
 ```
@@ -36,12 +37,13 @@
 
 ### Conversion
 
 ### Visualization
 
 
 ## Contributing
-Contributions are welcome! If you have any suggestions, improvements, or new features to add, please open an issue or 
+Contributions are welcome! If you have any suggestions, improvements, or new features to add, please open an issue or
 submit a pull request. Make sure to follow the existing coding style and include appropriate tests.
 
 ## License
 This project is licensed under the MIT License - see the LICENSE file for details.
+
```

