# Comparing `tmp/nichord-0.2.7.tar.gz` & `tmp/nichord-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nichord-0.2.7.tar", last modified: Tue Oct 17 11:56:32 2023, max compression
+gzip compressed data, was "nichord-0.3.0.tar", last modified: Sat Apr 27 11:08:13 2024, max compression
```

## Comparing `nichord-0.2.7.tar` & `nichord-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-10-17 11:56:32.201980 nichord-0.2.7/
--rw-rw-rw-   0        0        0     1089 2023-07-30 21:29:25.000000 nichord-0.2.7/LICENSE.txt
--rw-rw-rw-   0        0        0      877 2023-10-17 11:56:32.201980 nichord-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0    10118 2023-09-28 18:00:44.000000 nichord-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-10-17 11:56:32.197980 nichord-0.2.7/nichord/
--rw-rw-rw-   0        0        0      756 2022-11-12 03:49:12.000000 nichord-0.2.7/nichord/__init__.py
--rw-rw-rw-   0        0        0    35861 2023-10-17 11:55:30.000000 nichord-0.2.7/nichord/chord.py
--rw-rw-rw-   0        0        0     4893 2022-11-13 19:54:36.000000 nichord-0.2.7/nichord/combine.py
--rw-rw-rw-   0        0        0      615 2023-10-17 11:27:18.000000 nichord-0.2.7/nichord/convert.py
--rw-rw-rw-   0        0        0     5404 2023-08-03 16:00:59.000000 nichord-0.2.7/nichord/coord_labeler.py
--rw-rw-rw-   0        0        0     5505 2023-10-17 11:22:29.000000 nichord-0.2.7/nichord/glassbrain.py
--rw-rw-rw-   0        0        0     2156 2023-07-24 20:52:49.000000 nichord-0.2.7/nichord/patch_RendererAgg.py
--rw-rw-rw-   0        0        0     4394 2023-08-03 16:00:59.000000 nichord-0.2.7/nichord/peak.py
-drwxrwxrwx   0        0        0        0 2023-10-17 11:56:32.200980 nichord-0.2.7/nichord.egg-info/
--rw-rw-rw-   0        0        0      877 2023-10-17 11:56:32.000000 nichord-0.2.7/nichord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-10-17 11:56:32.000000 nichord-0.2.7/nichord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-17 11:56:32.000000 nichord-0.2.7/nichord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-10-17 11:56:32.000000 nichord-0.2.7/nichord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-10-17 11:56:32.000000 nichord-0.2.7/nichord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-17 11:56:32.201980 nichord-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1525 2023-10-17 11:55:43.000000 nichord-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:08:13.385664 nichord-0.3.0/
+-rw-rw-rw-   0        0        0     1089 2023-07-30 21:29:25.000000 nichord-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1104 2024-04-27 11:08:13.384667 nichord-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10452 2024-04-27 11:07:45.000000 nichord-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 11:08:13.369667 nichord-0.3.0/nichord/
+-rw-rw-rw-   0        0        0      774 2024-03-04 18:44:17.000000 nichord-0.3.0/nichord/__init__.py
+-rw-rw-rw-   0        0        0    37315 2024-04-27 10:59:21.000000 nichord-0.3.0/nichord/chord.py
+-rw-rw-rw-   0        0        0     4733 2024-04-27 11:03:36.000000 nichord-0.3.0/nichord/combine.py
+-rw-rw-rw-   0        0        0      615 2023-10-17 11:27:18.000000 nichord-0.3.0/nichord/convert.py
+-rw-rw-rw-   0        0        0     5404 2023-08-03 16:00:59.000000 nichord-0.3.0/nichord/coord_labeler.py
+-rw-rw-rw-   0        0        0     6103 2024-04-27 10:59:21.000000 nichord-0.3.0/nichord/glassbrain.py
+-rw-rw-rw-   0        0        0     2156 2023-07-24 20:52:49.000000 nichord-0.3.0/nichord/patch_RendererAgg.py
+-rw-rw-rw-   0        0        0     4394 2023-08-03 16:00:59.000000 nichord-0.3.0/nichord/peak.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:08:13.384667 nichord-0.3.0/nichord.egg-info/
+-rw-rw-rw-   0        0        0     1104 2024-04-27 11:08:13.000000 nichord-0.3.0/nichord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2024-04-27 11:08:13.000000 nichord-0.3.0/nichord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 11:08:13.000000 nichord-0.3.0/nichord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-27 11:08:13.000000 nichord-0.3.0/nichord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-27 11:08:13.000000 nichord-0.3.0/nichord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 11:08:13.385664 nichord-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1554 2024-04-27 11:07:45.000000 nichord-0.3.0/setup.py
```

### Comparing `nichord-0.2.7/LICENSE.txt` & `nichord-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nichord-0.2.7/README.md` & `nichord-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-![PyPI](https://img.shields.io/pypi/v/nichord) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nichord?link=https%3A%2F%2Fpypi.org%2Fproject%2Fnichord%2F)
-
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nichord?link=https%3A%2F%2Fpypi.org%2Fproject%2Fnichord%2F) ![PyPI](https://img.shields.io/pypi/v/nichord) [![Conda](https://anaconda.org/conda-forge/nichord/badges/version.svg)](https://anaconda.org/conda-forge/nichord)
 
 # NiChord
 
 `NiChord` is a Python package for visualizing functional connectivity data. This package was inspired by [NeuroMArVL](https://immersive.erc.monash.edu/neuromarvl/?example=40496078-effa-4ac3-9d3e-cb7f946e7dd1_137.147.133.145), an online visualization tool. Although the code was designed for neuroscience research, it can be used with any configuration of edge and label data.
 
 <p align="center">
   <img src="example\outside_chord_example.png"  width="600" />
@@ -105,27 +104,24 @@
 ```Python
 from nichord.combine import combine_imgs
 
 fp_combined = 'ex0_combined.png'
 combine_imgs(fp_glass, fp_chord, fp_combined)
 ```
 
-Notably, these functions have many other optional variables (e.g., passing specific colors for each network label using a dictionary). 
-
-<p align="center">
-  <img src="example\ex0.png" width="800"/>
-</p>
+Notably, these functions have many other optional variables. For example, `plot_chord`, `plot_glassbrain`, and `plot_and_combine` all take `edge_threshold` as an argument, which operates the same as in [nilearn](https://nilearn.github.io/dev/modules/generated/nilearn.plotting.plot_connectome.html). Also, you can pass specific colors for each network label using a dictionary.
 
 Further information on these optional variables can be seen by examining `example\example.py`, which contains code used to generate the two examples from the first section of this README. You can also learn about these by reading the hinting/documentation within each function.
 
 ### Plotting everything at once
 
 You can also use `combine.plot_and_combine` to do `plot_chord`, `plot_glassbrain`, and `combine_image` with a single function. `plot_and_combine` will create (if needed) and use directories `chord` and `glass` wherever you specify the combined image to be made with `dir_out`.
 
 ```Python
+from nichord.combine import plot_and_combine
 
 network_colors = {'Uncertain': 'black', 'Visual': 'purple',
                   'SM': 'darkturquoise', 'DAN': 'green', 'VAN': 'fuchsia',
                   'Limbic': 'burlywood', 'FPCN': 'orange', 'DMN': 'red'}
 
 network_order = ['FPCN', 'DMN', 'DAN', 'Visual', 'SM', 'Limbic', 
                  'Uncertain', 'VAN']
@@ -213,12 +209,12 @@
 malfunctioning code in `nichord.patch_RenderAgg.py`. The patch is automatically 
 applied when calling `chord.plot_chord_diagram(...)` with the default argument 
 `do_monkeypatch=True`. 
 
 The glass brain diagrams rely on the plotting tools from [`nilearn`](https://nilearn.github.io/modules/generated/nilearn.plotting.plot_connectome.html), whereas the chord diagrams is made from scratch by drawing shapes in [`matplotlib`](https://matplotlib.org/).
 
 ## Authors
-`NiChord` was created by Paul C. Bogdan with help from [Jonathan Shobrook](https://github.com/shobrook) as part of our research in the [Dolcos Lab](https://dolcoslab.beckman.illinois.edu/) at the Beckman Institute for Advanced Science and Technology and the University of Illinois at  Urbana-Champaign. 
+`NiChord` was created by Paul C. Bogdan with help from [Jonathan Shobrook](https://github.com/shobrook) as part of our research in the [Dolcos Lab](https://dolcoslab.beckman.illinois.edu/) at the Beckman Institute for Advanced Science and Technology and the University of Illinois at Urbana-Champaign. 
 
-If you are using `NiChord` in your work, we ask that you please cite the paper below or the present reporsitory:
+If you are using `NiChord` in your work, it would be nice if you please cite the paper below or the present reporsitory:
 
-Bogdan, P.C., Iordan, A. D., Shobrook, J., & Dolcos, F. (2023). ConnSearch: A Framework for Functional Connectivity Analysis Designed for Interpretability and Effectiveness at Limited Sample Sizes. *NeuroImage*, 120274.
+Bogdan, P.C., Iordan, A.D., Shobrook, J., & Dolcos, F. (2023). ConnSearch: A Framework for Functional Connectivity Analysis Designed for Interpretability and Effectiveness at Limited Sample Sizes. *NeuroImage*, 120274.
```

### Comparing `nichord-0.2.7/nichord/__init__.py` & `nichord-0.3.0/nichord/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 from .coord_labeler import (get_idx_to_label,
                             find_closest,
                             AttrDict,
                             get_yeo_atlas)
 from .glassbrain import plot_glassbrain
 from .patch_RendererAgg import (NeuoChordRenderAgg,
                                 do_monkey_patch)
-from .combine import combine_imgs
+from .combine import combine_imgs, plot_and_combine
```

### Comparing `nichord-0.2.7/nichord/chord.py` & `nichord-0.3.0/nichord/chord.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import math
 import warnings
 
 import matplotlib
 from matplotlib import patches
+from nilearn._utils.param_validation import check_threshold
 from scipy import interpolate
 
 from collections import defaultdict
 import matplotlib.pyplot as plt
 import numpy as np
 from math import radians
 from typing import Union, Tuple
 from collections import OrderedDict
 
+from scipy.stats import scoreatpercentile
+
+
 class ROI_to_degree:
     """
     Used to calculate an ROI's position within the rim/label.
     Within the rim/label, ROIs are positioned based on their y coordinate
         (i.e., how anterior/posterior it is). If no coordinate is provided,
         the ROIs are positioned randomly (see plot_chord_diagram(...)).
     """
@@ -87,14 +91,15 @@
                label_fontsize: int = 60,
                do_monkeypatch: bool = True,
                vmin: Union[None, int, float] = None,
                vmax: Union[None, int, float] = None,
                plot_count: bool = False,
                plot_abs_sum: bool = False,
                norm_thickness: bool = False,
+               edge_threshold: Union[float, int, str] = 0.,
                dpi: int = 400) -> None:
     """
     Plots the chord diagram and either saves a file if fp_chord is not None or
         opens it in a matplotlib window. For most of the arguments in these
         function, if None is passed, then a default setting is generated and
         used.
 
@@ -129,27 +134,41 @@
         be added for ROIs in edges used for arcs.
     :param ROI_circle_radius: The radius used for the ROI circles
     :param do_monkeypatch: There is seemingly a bug in matplotlib that prevents
         cleanly rotating characters. The matplotlib team has been notified about
         this, and a potential fix has been suggested. Until that is incorporated
         into matplotlib, the fix is being "monkeypatched". See
         chord.plot_rim_label(...) and patch_RenderAgg.py.
+    :param edge_threshold: This parameter acts the same as edge_threshold in
+        nilearn.plotting.plot_connectome. Edges whose abs(weight) is under
+        the threshold are omitted. edge_threshold can be a float or a string
+        representing a percentile (e.g., "25"). The latter causes edges below
+        the percentile to be omitted.
     """
 
     network_order, network_colors = \
         _network_order_colors_check(network_order, network_colors, idx_to_label)
 
     if edge_weights is None:
         edge_weights = [1] * len(edges)
+    else:
+        edge_weights, edges = _threshold_proc(edge_threshold, edge_weights,
+                                              edges)
+
 
     if vmin is None:
         vmin = min(edge_weights)
     if vmax is None:
         vmax = max(edge_weights)
 
+    if vmin == vmax:
+        raise ValueError(f'vmin and vmax cannot be equal. '
+                         f'Note: your inputs only provide {len(edges)} edges '
+                         f'after thresholding')
+
     if cmap is None:
         if abs(vmin - vmax) < 1e-6:
             cmap = plt.get_cmap('Greys')
         else:
             cmap = plt.get_cmap('turbo')
     elif isinstance(cmap, str):
         cmap = plt.get_cmap(cmap)
@@ -431,15 +450,15 @@
               seven_point_arc: bool = False,
               vmin: Union[float, int] = -1,
               vmax: Union[float, int] = 1,
               plot_count: bool = True,
               plot_abs_sum: bool = False,
               norm_thickness: bool = False,
               max_linewidth: Union[float, int] = 28,
-              sub_min_thickness: bool = False
+              sub_min_thickness: bool = False,
               ) -> (float, float):
     """
     Plots the arcs between each ROI. Within the rim/label, ROIs are positioned
         based on their y coordinate (i.e., how anterior/posterior it is). If
         no coordinate is provided, the ROIs are positioned randomly
         (see plot_chord_diagram(...)).
 
@@ -772,8 +791,25 @@
 def cart_to_polar(x: Union[float, int], y: Union[float, int]) -> Tuple[
     float, float]:
     """
     Converts cartesian points (x, y) to polar (r, theta)
     """
     z = x + y * 1j
     r, theta = np.abs(z), np.angle(z)
-    return r, theta
+    return r, theta
+
+
+def _threshold_proc(edge_threshold, edge_weights, edges):
+    if edge_threshold == 0: return edge_weights, edges
+    edge_threshold = check_threshold(
+        edge_threshold,
+        np.abs(edge_weights),
+        scoreatpercentile,
+        "edge_threshold",
+    )
+
+    if edge_threshold > 0:
+        edges = [edge for edge, weight in zip(edges, edge_weights)
+                 if abs(weight) > edge_threshold]
+        edge_weights = [weight for weight in edge_weights
+                        if abs(weight) > edge_threshold]
+    return edge_weights, edges
```

### Comparing `nichord-0.2.7/nichord/combine.py` & `nichord-0.3.0/nichord/combine.py`

 * *Files 13% similar despite different names*

```diff
@@ -73,15 +73,16 @@
                      cmap: Union[None, str, matplotlib.colors.Colormap] = None,
                      network_order: Union[list, None] = None,
                      network_colors: Union[dict, None] = None,
                      chord_kwargs: Union[None, dict] = None,
                      glass_kwargs: Union[None, dict] = None,
                      title: Union[None, str] = None,
                      only1glass: bool = False,
-                     fontsize: int = 82
+                     fontsize: int = 82,
+                     edge_threshold: Union[float, int, str] = 0.,
                      ) -> None:
     name, file_ext = os.path.splitext(fn)
     if file_ext == '':
         file_ext = '.png'
 
     dir_chord = os.path.join(dir_out, 'chord')
     if not os.path.isdir(dir_chord): os.mkdir(dir_chord)
@@ -89,31 +90,25 @@
     if not os.path.isdir(dir_glass): os.mkdir(dir_glass)
 
     fp_chord = os.path.join(dir_chord, f'{name}_chord{file_ext}')
     fp_glass = os.path.join(dir_glass, f'{name}_glass{file_ext}')
     fp_combined = os.path.join(dir_out, f'{name}{file_ext}')
 
     if chord_kwargs is None: chord_kwargs = {}
-    if 'network_order' not in chord_kwargs:
-        chord_kwargs['network_order'] = network_order
-    if 'network_colors' not in chord_kwargs:
-        chord_kwargs['network_colors'] = network_colors
-    if 'cmap' not in chord_kwargs:
-        chord_kwargs['cmap'] = cmap
+    if glass_kwargs is None: glass_kwargs = {}
+    keys = ['network_order', 'network_colors', 'cmap', 'edge_threshold']
+    vals = [network_order, network_colors, cmap, edge_threshold]
+    for key, val in zip(keys, vals):
+        if key not in chord_kwargs:
+            chord_kwargs[key] = val
+        if key not in glass_kwargs:
+            glass_kwargs[key] = val
 
     plot_chord(idx_to_label, edges, edge_weights=edge_weights,
                coords=coords, fp_chord=fp_chord,
                **chord_kwargs)
 
-    if glass_kwargs is None: glass_kwargs = {}
-    if 'network_order' not in glass_kwargs:
-        glass_kwargs['network_order'] = network_order
-    if 'network_colors' not in glass_kwargs:
-        glass_kwargs['network_colors'] = network_colors
-    if 'cmap' not in glass_kwargs:
-        glass_kwargs['cmap'] = cmap
-
     plot_glassbrain(idx_to_label, edges, edge_weights, fp_glass,
                     coords, **glass_kwargs)
 
     combine_imgs(fp_glass, fp_chord, fp_combined, title=title,
                  only1glass=only1glass, fontsize=fontsize)
```

### Comparing `nichord-0.2.7/nichord/convert.py` & `nichord-0.3.0/nichord/convert.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.7/nichord/coord_labeler.py` & `nichord-0.3.0/nichord/coord_labeler.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.7/nichord/glassbrain.py` & `nichord-0.3.0/nichord/glassbrain.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from nilearn import plotting
 import matplotlib
 from typing import Union
 
-from nichord.chord import _network_order_colors_check
+from nichord.chord import _network_order_colors_check, _threshold_proc
 
 
 def plot_glassbrain(idx_to_label: dict,
                     edges: Union[list, np.ndarray],
                     edge_weights: Union[None, list, np.ndarray],
                     fp_glass: Union[None, str],
                     coords: Union[list, np.ndarray] = None,
@@ -16,15 +16,17 @@
                     node_size: Union[None, float, int, list, np.ndarray] = 5,
                     linewidths: Union[None, float, int, list] = 6,
                     alphas: Union[None, float, int, list] = None,
                     network_order: Union[None, list] = None,
                     network_colors: Union[None, dict] = None,
                     dpi: int = 400,
                     vmin: Union[None, int, float] = None,
-                    vmax: Union[None, int, float] = None) -> None:
+                    vmax: Union[None, int, float] = None,
+                    edge_threshold: Union[float, int, str] = 0.,
+                    ) -> None:
     """
     Plots the connectome on a brain, where the node colors correspond to the
         ROI's label (specified by idx_to_label). Each edge's color correspond
         to the edge's weight or is set to gray if all weighst are equal to 1.
         Can either be used to save a file or open the connectome in your
         browser, depending on whether fp_out is None.
 
@@ -44,24 +46,32 @@
     :param linewidths: linewidths used for the edges
     :param alphas: alphas used for the edges
     :param network_colors: dict mapping each label to a matplotlib color. If
         None, then default colors will be set based on matplotlib.
     :param network_order: If network_colors is None, then this list
         will specify the order in which default matplotlib colors will be
         assigned to networks.
+    :param edge_threshold: This parameter acts the same as edge_threshold in
+        nilearn.plotting.plot_connectome. Edges whose abs(weight) is under
+        the threshold are omitted. edge_threshold can be a float or a string
+        representing a percentile (e.g., "25"). The latter causes edges below
+        the percentile to be omitted.
     """
 
     network_order, network_colors = \
         _network_order_colors_check(network_order, network_colors, idx_to_label)
 
     if isinstance(cmap, str):
         cmap = plt.get_cmap(cmap)
 
     if edge_weights is None:
         edge_weights = [1] * len(edges)
+    else:
+        edge_weights, edges = _threshold_proc(edge_threshold, edge_weights,
+                                              edges)
 
     nonzero_node_idxs = list(set(node_idx for tup in edges for node_idx in tup))
     n = len(nonzero_node_idxs)
     adj = np.zeros((n, n))
     if all(weight == 1 for weight in edge_weights):
         node_idx_to_i = dict(
             (node_idx, i) for i, node_idx in enumerate(nonzero_node_idxs))
```

### Comparing `nichord-0.2.7/nichord/patch_RendererAgg.py` & `nichord-0.3.0/nichord/patch_RendererAgg.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.7/nichord/peak.py` & `nichord-0.3.0/nichord/peak.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.7/setup.py` & `nichord-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,24 +5,23 @@
     from distutils.core import setup
 
 if sys.version_info[:3] < (3, 7, 0):
     print("Requires Python 3.7 to run.")
     sys.exit(1)
 
 desc = '`NiChord` is a Python package for visualizing functional connectivity data. To find out more about the ' \
-       'package and see a package, take a look at its [GitHub repo](https://github.com/paulcbogdan/NiChord)'
-
-'To find out more about the package and see an example, see its .'
+       'package and see a package, take a look at its [GitHub repo](https://github.com/paulcbogdan/NiChord). ' \
+       'The package is also available via [conda](https://anaconda.org/conda-forge/nichord).'
 
 setup(
     name="nichord",
     description="Creates chord diagrams for connectivity/graph data",
     long_description=desc,
     long_description_content_type="text/markdown",
-    version="v0.2.7",
+    version="v0.3.0",
     packages=["nichord"],
     python_requires=">=3.7",
     url="https://github.com/paulcbogdan/NiChord",
     author="paulcbogdan",
     author_email="paulcbogdan@gmail.com",
     install_requires=["nilearn",
                       "pandas",
```

