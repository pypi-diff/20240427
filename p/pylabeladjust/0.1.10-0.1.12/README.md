# Comparing `tmp/pylabeladjust-0.1.10.tar.gz` & `tmp/pylabeladjust-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylabeladjust-0.1.10.tar", max compression
+gzip compressed data, was "pylabeladjust-0.1.12.tar", max compression
```

## Comparing `pylabeladjust-0.1.10.tar` & `pylabeladjust-0.1.12.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2024-04-12 15:51:27.765165 pylabeladjust-0.1.10/LICENSE
--rw-r--r--   0        0        0     6924 2024-04-16 09:25:22.824669 pylabeladjust-0.1.10/README.md
--rw-r--r--   0        0        0       61 2024-04-15 12:28:42.751523 pylabeladjust-0.1.10/pylabeladjust/__init__.py
--rw-r--r--   0        0        0    11855 2024-04-13 01:41:05.089290 pylabeladjust-0.1.10/pylabeladjust/core.py
--rw-r--r--   0        0        0      514 2024-04-16 09:51:14.195613 pylabeladjust-0.1.10/pyproject.toml
--rw-r--r--   0        0        0     7706 1970-01-01 00:00:00.000000 pylabeladjust-0.1.10/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-12 15:51:27.765165 pylabeladjust-0.1.12/LICENSE
+-rw-r--r--   0        0        0     7414 2024-04-19 19:41:47.947641 pylabeladjust-0.1.12/README.md
+-rw-r--r--   0        0        0       61 2024-04-15 12:28:42.751523 pylabeladjust-0.1.12/pylabeladjust/__init__.py
+-rw-r--r--   0        0        0    12952 2024-04-26 16:16:40.390097 pylabeladjust-0.1.12/pylabeladjust/core.py
+-rw-r--r--   0        0        0      574 2024-04-26 16:46:46.790861 pylabeladjust-0.1.12/pyproject.toml
+-rw-r--r--   0        0        0     8196 1970-01-01 00:00:00.000000 pylabeladjust-0.1.12/PKG-INFO
```

### Comparing `pylabeladjust-0.1.10/LICENSE` & `pylabeladjust-0.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `pylabeladjust-0.1.10/README.md` & `pylabeladjust-0.1.12/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -47,18 +47,19 @@
 
 * `texts` (List[matplotlib.text.Text]): A list of text objects to be adjusted.
 * `speed` (float, optional): The speed of the adjustment process (movement, measured on the scale of the data). If left blank, speed is set to halve the size of the mean text-width. If your labels end up all over the place, you might want to decrease this value. If it looks like the adjustment didn't change much, although the algorithm spent dozens of seconds optimizing, the value might need to be increased.
 * `adjust_by_size` (bool, optional): Whether to adjust the texts based on their sizes. Defaults to True. This makes the positions of large text-blocks more robust, and shuffles smaller ones around more, which can result in a structurally more convincing layout, and speeds up the algorithms. You should check that small stuff didn't get shuffled away *too* far though. 
 * `radius_scale` (float, optional): The scale factor for the radius used in the adjustment process. Defaults to 1.1.
 * `max_iterations` (int, optional): The maximum number of iterations for the adjustment process. Defaults to 200. Increase if your layout still has overlaps after running the adjustment. This can usually be increased liberally because once there is little overlap anymore, the remaining iterations are very fast.
 * `plot_progress` (bool, optional): Whether to print out plots of the progress of the adjustment process. Defaults to False, and is mostly useful for debugging.
-* `margin_percentage` (int, optional): The percentage of margin to be added around the adjusted texts. Calculated from the width of rectangles. Defaults to 10.
+* `margin` (int, optional): The the size of the margin to add around the rectangles. Either a percentage, or an absolute value. Defaults to 0. 
+* `margin_type` (str, optional): How to add margins. Options are 'percentage' and 'absolute'. 'percentage' sets the margin as a percentage (given in `margin`) of the rectangles size. 'absolute`sets all margins to the same absolute value.
 * `return_optimization_process` (bool, optional): Whether to return the optimization process, a list of dataframes of all the positions the texts went through in the optimization process. Defaults to False.
 
-The function edits your `texts` object in place, so you can just resume plotting. It also will return a dataframe of the new positions, and if `return_optimization_process` is set to true, a list of dataframes of the intermediate steps.
+The function edits your `texts` object in place, so you can just resume plotting. Note that it will set your alignment (ha, va) It also will return a dataframe of the new positions, and if `return_optimization_process` is set to true, a list of dataframes of the intermediate steps.
 
 
 
 We can also adjust rectangles which are not labels directly. In that case, the function expects a `pandas`-dataframe, with the columns `x`,`y`,`height`,`width`.
 The syntax will look very similar to above:
 
 ```
@@ -69,16 +70,16 @@
 
 * `rectangle_data` (DataFrame): A `pandas`-dataframe, with the columns `x`,`y`,`height`,`width`.
 * `speed` (float, optional): The speed of the adjustment process (movement, measured on the scale of the data). If left blank, speed is set to halve the size of the mean text-width. If your labels end up all over the place, you might want to decrease this value. If it looks like the adjustment didn't change much, although the algorithm spent dozens of seconds optimizing, the value might need to be increased.
 * `adjust_by_size` (bool, optional): Whether to adjust the texts based on their sizes. Defaults to True. This makes the positions of large text-blocks more robust, and shuffles smaller ones around more, which can result in a structurally more convincing layout, and speeds up the algorithms. You should check that small stuff didn't get shuffled away *too* far though. 
 * `radius_scale` (float, optional): The scale factor for the radius used in the adjustment process. Defaults to 1.1.
 * `max_iterations` (int, optional): The maximum number of iterations for the adjustment process. Defaults to 200. Increase if your layout still has overlaps after running the adjustment. This can usually be increased liberally because once there is little overlap anymore, the remaining iterations are very fast.
 * `plot_progress` (bool, optional): Whether to print out plots of the progress of the adjustment process. Defaults to False, and is mostly useful for debugging.
-* `margin_percentage` (int, optional): The percentage of margin to be added around the adjusted texts. Calculated from the width of rectangles. Defaults to 10.
-* `return_optimization_process` (bool, optional): Whether to return the optimization process, a list of dataframes of all the positions the texts went through in the optimization process. Defaults to False.
+* `margin` (int, optional): The the size of the margin to add around the rectangles. Either a percentage, or an absolute value. Defaults to 10. 
+* `margin_type` (str, optional): How to add margins. Options are 'percentage' and 'absolute'. 'percentage' sets the margin as a percentage (given in `margin`) of the rectangles size. 'absolute`sets all margins to the same absolute value.* `return_optimization_process` (bool, optional): Whether to return the optimization process, a list of dataframes of all the positions the texts went through in the optimization process. Defaults to False.
 
 
 <img src="https://raw.githubusercontent.com/MNoichl/pylabeladjust/main/images/layout_process_rectangles.gif" width="672" />
 
 
 
 # To-Do
```

### Comparing `pylabeladjust-0.1.10/pylabeladjust/core.py` & `pylabeladjust-0.1.12/pylabeladjust/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,39 +5,45 @@
 import random
 import pandas as pd
 import matplotlib.pyplot as plt
 import matplotlib.patches as patches
 
 
 def adjust_labels(rectangle_data, speed=None, adjust_by_size=True, radius_scale=1.1, 
-                  max_iterations=100, plot_progress=False, margin_percentage=0, return_optimization_process=False):
+                  max_iterations=100, plot_progress=False, margin=0, margin_type='percentage', return_optimization_process=False):
     """
     Adjusts the labels of rectangles in the given rectangle_data DataFrame to avoid overlapping.
 
     Args:
         rectangle_data (DataFrame): A DataFrame containing the rectangle data.
         speed (float, optional): The speed at which the labels are adjusted. Defaults to None, then it uses 1/2th of the width of the mean rectangle.
         adjust_by_size (bool, optional): Whether to adjust the labels based on the size of the rectangles. Defaults to True.
             radius_scale (float, optional): The scale factor for the repulsion radius. Defaults to 1.1.
         max_iterations (int, optional): The maximum number of iterations to perform. Defaults to 100.
         plot_progress (bool, optional): Whether to plot the progress of label adjustment. Defaults to False.
-        margin_percentage (int, optional): The percentage of margin to add around the rectangles. Defaults to 0. 
+        margin (int, optional): The the size of the margin to add around the rectangles. Either a percentage, or an absolute value. Defaults to 0. 
+        margin_type (str, optional): How to add margins. Options are 'percentage' and 'absolute'. 
 
     Returns:
         DataFrame: The adjusted rectangle_data DataFrame.
     """
     # Make a copy to avoid modifying the original DataFrame outside this function
     rectangle_data = rectangle_data.copy()
 
     # Calculate speed if not provided
     if speed is None:
         speed = 0.5 * (rectangle_data['width'].mean() )
         
     # Calculate and apply margin
-    margin_width = rectangle_data['width'] * margin_percentage / 100
+    if margin_type == 'percentage':
+        margin_width = rectangle_data['width'] * margin / 100
+    elif margin_type == 'absolute':
+        margin_width = margin
+        
+        
     rectangle_data['x'] -= margin_width
     rectangle_data['y'] -= margin_width
     rectangle_data['width'] += 2 * margin_width
     rectangle_data['height'] += 2 * margin_width
     
     if return_optimization_process:
         optimization_process = []
@@ -90,15 +96,15 @@
                     
 
     # Revert margin expansion
     rectangle_data['x'] += margin_width
     rectangle_data['y'] += margin_width
     rectangle_data['width'] -= 2 * margin_width
     rectangle_data['height'] -= 2 * margin_width
-
+    rectangle_data = rectangle_data[['x', 'y', 'width', 'height']]
     if return_optimization_process:
         return rectangle_data, optimization_process 
     else:
         return rectangle_data
 
 def repulse(rect1_idx, rect2_idx, rectangle_data, speed, adjust_by_size, radius_scale):
     """
@@ -163,15 +169,15 @@
 
 
 
                   
                   
 
 def adjust_texts(texts, speed=None, adjust_by_size=True, radius_scale=1.1, 
-                  max_iterations=200, plot_progress=True, margin_percentage=10, return_optimization_process=False):
+                  max_iterations=200, plot_progress=True, margin=0, margin_type='percentage', return_optimization_process=False):
     """
     Adjusts the positions of texts on a plot to avoid overlapping.
 
     Args:
         texts (List[matplotlib.text.Text]): A list of text objects to be adjusted.
         speed (float, optional): The speed of the adjustment process. Defaults to None, in which case it uses 1/2th of the width of the mean text.
         adjust_by_size (bool, optional): Whether to adjust the texts based on their sizes. Defaults to True.
@@ -186,26 +192,58 @@
     """
     ax = plt.gca()
     bbox_list = []
     renderer = ax.figure.canvas.get_renderer()
 
     for text in texts:
         bbox = text.get_window_extent(renderer).transformed(ax.transData.inverted())
-        bbox_list.append([bbox.x0, bbox.y0, bbox.x1-bbox.x0, bbox.y1-bbox.y0 ])
+        bbox_list.append([bbox.x0, bbox.y0, bbox.width, bbox.height])
+        
     rectangle_df = pd.DataFrame(bbox_list, columns=['x', 'y', 'width', 'height'])
     
+    
     if return_optimization_process:
         rectangles_adjusted, optimization_process = adjust_labels(rectangle_df, speed=speed, adjust_by_size=adjust_by_size, radius_scale=radius_scale, max_iterations=max_iterations,
-                                        margin_percentage=margin_percentage,return_optimization_process=True)
+                                        margin=margin, margin_type=margin_type,return_optimization_process=True)
     else:
         rectangles_adjusted = adjust_labels(rectangle_df, speed=speed, adjust_by_size=adjust_by_size, radius_scale=radius_scale, max_iterations=max_iterations,
-                                        margin_percentage=margin_percentage,return_optimization_process=False)
-        
+                                        margin=margin, margin_type=margin_type,return_optimization_process=False)
+
+    new_xs, new_ys = [], []
+    print('Resetting positions to accord with alignment')
     for ix, row in rectangles_adjusted.iterrows():
-        texts[ix].set_position((row['x'], row['y']))
+        text = texts[ix]
+        ha = text.get_ha()
+        va = text.get_va()
+        print(ha, va)
+        # Reset positions based on ha and va
+        if ha == 'center':
+            new_x = row['x'] + row['width'] / 2
+        elif ha == 'right':
+            new_x = row['x'] + row['width']
+        else:
+            new_x = row['x']
+
+        if va == 'center':
+            new_y = row['y'] + row['height'] / 2
+        elif va == 'top':
+            new_y = row['y'] + row['height']
+        else:
+            new_y = row['y']
+
+        text.set_position((new_x, new_y))
+
+        new_xs.append(new_x)
+        new_ys.append(new_y)
+        
+    rectangles_adjusted['x'] = new_xs
+    rectangles_adjusted['y'] = new_ys
+
+    
+
     if return_optimization_process:
         return rectangles_adjusted, optimization_process
     else:
         return rectangles_adjusted
 
 
 def plot_rectangles(ax, rectangles_dataframe, color='red', set_limits=True, facecolor='none', alpha=1.):
```

### Comparing `pylabeladjust-0.1.10/PKG-INFO` & `pylabeladjust-0.1.12/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylabeladjust
-Version: 0.1.10
+Version: 0.1.12
 Summary: `pylabeladjust` is a port of Gephi's Label-Adjust algorithm to python.
 License: GPL-3.0
 Author: MNoichl
 Author-email: noichlmax@hotmail.co.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -67,18 +67,19 @@
 
 * `texts` (List[matplotlib.text.Text]): A list of text objects to be adjusted.
 * `speed` (float, optional): The speed of the adjustment process (movement, measured on the scale of the data). If left blank, speed is set to halve the size of the mean text-width. If your labels end up all over the place, you might want to decrease this value. If it looks like the adjustment didn't change much, although the algorithm spent dozens of seconds optimizing, the value might need to be increased.
 * `adjust_by_size` (bool, optional): Whether to adjust the texts based on their sizes. Defaults to True. This makes the positions of large text-blocks more robust, and shuffles smaller ones around more, which can result in a structurally more convincing layout, and speeds up the algorithms. You should check that small stuff didn't get shuffled away *too* far though. 
 * `radius_scale` (float, optional): The scale factor for the radius used in the adjustment process. Defaults to 1.1.
 * `max_iterations` (int, optional): The maximum number of iterations for the adjustment process. Defaults to 200. Increase if your layout still has overlaps after running the adjustment. This can usually be increased liberally because once there is little overlap anymore, the remaining iterations are very fast.
 * `plot_progress` (bool, optional): Whether to print out plots of the progress of the adjustment process. Defaults to False, and is mostly useful for debugging.
-* `margin_percentage` (int, optional): The percentage of margin to be added around the adjusted texts. Calculated from the width of rectangles. Defaults to 10.
+* `margin` (int, optional): The the size of the margin to add around the rectangles. Either a percentage, or an absolute value. Defaults to 0. 
+* `margin_type` (str, optional): How to add margins. Options are 'percentage' and 'absolute'. 'percentage' sets the margin as a percentage (given in `margin`) of the rectangles size. 'absolute`sets all margins to the same absolute value.
 * `return_optimization_process` (bool, optional): Whether to return the optimization process, a list of dataframes of all the positions the texts went through in the optimization process. Defaults to False.
 
-The function edits your `texts` object in place, so you can just resume plotting. It also will return a dataframe of the new positions, and if `return_optimization_process` is set to true, a list of dataframes of the intermediate steps.
+The function edits your `texts` object in place, so you can just resume plotting. Note that it will set your alignment (ha, va) It also will return a dataframe of the new positions, and if `return_optimization_process` is set to true, a list of dataframes of the intermediate steps.
 
 
 
 We can also adjust rectangles which are not labels directly. In that case, the function expects a `pandas`-dataframe, with the columns `x`,`y`,`height`,`width`.
 The syntax will look very similar to above:
 
 ```
@@ -89,16 +90,16 @@
 
 * `rectangle_data` (DataFrame): A `pandas`-dataframe, with the columns `x`,`y`,`height`,`width`.
 * `speed` (float, optional): The speed of the adjustment process (movement, measured on the scale of the data). If left blank, speed is set to halve the size of the mean text-width. If your labels end up all over the place, you might want to decrease this value. If it looks like the adjustment didn't change much, although the algorithm spent dozens of seconds optimizing, the value might need to be increased.
 * `adjust_by_size` (bool, optional): Whether to adjust the texts based on their sizes. Defaults to True. This makes the positions of large text-blocks more robust, and shuffles smaller ones around more, which can result in a structurally more convincing layout, and speeds up the algorithms. You should check that small stuff didn't get shuffled away *too* far though. 
 * `radius_scale` (float, optional): The scale factor for the radius used in the adjustment process. Defaults to 1.1.
 * `max_iterations` (int, optional): The maximum number of iterations for the adjustment process. Defaults to 200. Increase if your layout still has overlaps after running the adjustment. This can usually be increased liberally because once there is little overlap anymore, the remaining iterations are very fast.
 * `plot_progress` (bool, optional): Whether to print out plots of the progress of the adjustment process. Defaults to False, and is mostly useful for debugging.
-* `margin_percentage` (int, optional): The percentage of margin to be added around the adjusted texts. Calculated from the width of rectangles. Defaults to 10.
-* `return_optimization_process` (bool, optional): Whether to return the optimization process, a list of dataframes of all the positions the texts went through in the optimization process. Defaults to False.
+* `margin` (int, optional): The the size of the margin to add around the rectangles. Either a percentage, or an absolute value. Defaults to 10. 
+* `margin_type` (str, optional): How to add margins. Options are 'percentage' and 'absolute'. 'percentage' sets the margin as a percentage (given in `margin`) of the rectangles size. 'absolute`sets all margins to the same absolute value.* `return_optimization_process` (bool, optional): Whether to return the optimization process, a list of dataframes of all the positions the texts went through in the optimization process. Defaults to False.
 
 
 <img src="https://raw.githubusercontent.com/MNoichl/pylabeladjust/main/images/layout_process_rectangles.gif" width="672" />
 
 
 
 # To-Do
```

