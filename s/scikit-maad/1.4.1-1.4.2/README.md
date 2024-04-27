# Comparing `tmp/scikit_maad-1.4.1.tar.gz` & `tmp/scikit_maad-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit_maad-1.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "scikit_maad-1.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `scikit_maad-1.4.1.tar` & `scikit_maad-1.4.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1258 2023-02-28 00:54:05.676869 scikit_maad-1.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      609 2023-02-28 00:54:05.676938 scikit_maad-1.4.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1462 2023-05-19 17:46:43.301771 scikit_maad-1.4.1/.github/workflows/ci-cd.yml
--rw-r--r--   0        0        0     1494 2023-02-28 00:54:05.677061 scikit_maad-1.4.1/.github/workflows/python-compatibility.yml
--rw-r--r--   0        0        0     1734 2023-06-15 19:25:27.299155 scikit_maad-1.4.1/.gitignore
--rw-r--r--   0        0        0      591 2023-02-28 00:54:05.677263 scikit_maad-1.4.1/CITATION.bib
--rw-r--r--   0        0        0     5223 2023-02-28 00:54:05.677375 scikit_maad-1.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3674 2023-03-10 21:26:34.971788 scikit_maad-1.4.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1505 2023-02-28 00:54:05.677527 scikit_maad-1.4.1/LICENSE
--rw-r--r--   0        0        0     7090 2024-03-02 07:21:53.026412 scikit_maad-1.4.1/README.md
--rw-r--r--   0        0        0     1177 2023-03-10 21:26:34.972381 scikit_maad-1.4.1/maad/__init__.py
--rw-r--r--   0        0        0     5782 2023-11-29 17:34:08.591828 scikit_maad-1.4.1/maad/features/__init__.py
--rw-r--r--   0        0        0   129783 2024-03-02 07:21:53.027629 scikit_maad-1.4.1/maad/features/alpha_indices.py
--rw-r--r--   0        0        0     8737 2024-03-02 07:21:53.028531 scikit_maad-1.4.1/maad/features/composite_soundscape_descriptors.py
--rw-r--r--   0        0        0    41647 2023-06-15 19:25:27.305113 scikit_maad-1.4.1/maad/features/shape.py
--rwxr-xr-x   0        0        0    13949 2023-06-16 02:36:27.999414 scikit_maad-1.4.1/maad/features/spectral.py
--rw-r--r--   0        0        0    13703 2023-06-16 02:39:32.947287 scikit_maad-1.4.1/maad/features/temporal.py
--rw-r--r--   0        0        0     1024 2023-11-21 01:32:55.303856 scikit_maad-1.4.1/maad/rois/__init__.py
--rw-r--r--   0        0        0     8114 2023-06-15 19:25:27.306255 scikit_maad-1.4.1/maad/rois/rois_1d.py
--rw-r--r--   0        0        0    33504 2023-11-21 01:38:07.669166 scikit_maad-1.4.1/maad/rois/rois_2d.py
--rw-r--r--   0        0        0     6379 2023-11-29 19:22:44.446889 scikit_maad-1.4.1/maad/rois/template_matching_func.py
--rw-r--r--   0        0        0     2946 2023-02-28 00:54:06.300338 scikit_maad-1.4.1/maad/sound/__init__.py
--rw-r--r--   0        0        0    16791 2023-06-15 19:25:27.307341 scikit_maad-1.4.1/maad/sound/filter.py
--rw-r--r--   0        0        0    18024 2023-06-15 19:25:27.307882 scikit_maad-1.4.1/maad/sound/input_output.py
--rw-r--r--   0        0        0     6185 2023-02-28 00:54:06.300692 scikit_maad-1.4.1/maad/sound/metrics.py
--rw-r--r--   0        0        0    39987 2023-05-19 17:46:43.305247 scikit_maad-1.4.1/maad/sound/spectral_subtraction.py
--rw-r--r--   0        0        0    18299 2023-02-28 00:54:06.300960 scikit_maad-1.4.1/maad/sound/spectro_func.py
--rw-r--r--   0        0        0    18910 2023-05-19 17:46:43.307126 scikit_maad-1.4.1/maad/sound/transform.py
--rw-r--r--   0        0        0     2665 2023-02-28 00:54:06.301271 scikit_maad-1.4.1/maad/sound/trim_func.py
--rw-r--r--   0        0        0     1857 2023-03-10 21:26:34.972832 scikit_maad-1.4.1/maad/spl/__init__.py
--rw-r--r--   0        0        0    33132 2023-02-28 00:54:06.301494 scikit_maad-1.4.1/maad/spl/active_space.py
--rw-r--r--   0        0        0    23435 2024-03-27 01:54:24.024902 scikit_maad-1.4.1/maad/spl/conversion_SPL.py
--rw-r--r--   0        0        0     5596 2023-02-28 00:54:06.301720 scikit_maad-1.4.1/maad/util/__init__.py
--rw-r--r--   0        0        0    11066 2024-03-02 07:21:53.029097 scikit_maad-1.4.1/maad/util/audio_metadata_utilities.py
--rw-r--r--   0        0        0    14953 2023-05-19 17:46:43.307469 scikit_maad-1.4.1/maad/util/math_func.py
--rw-r--r--   0        0        0    36215 2023-11-19 21:29:33.608560 scikit_maad-1.4.1/maad/util/miscellaneous.py
--rw-r--r--   0        0        0    15678 2023-11-22 17:21:31.825891 scikit_maad-1.4.1/maad/util/parser.py
--rw-r--r--   0        0        0    68303 2023-10-07 20:04:46.355685 scikit_maad-1.4.1/maad/util/visualization.py
--rw-r--r--   0        0        0    24595 2023-06-07 19:28:05.157520 scikit_maad-1.4.1/maad/util/xeno_canto.py
--rw-r--r--   0        0        0       88 2024-03-27 15:01:52.205549 scikit_maad-1.4.1/maad/version.py
--rw-r--r--   0        0        0     1726 2023-03-10 21:26:34.973235 scikit_maad-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     8720 1970-01-01 00:00:00.000000 scikit_maad-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1258 2023-02-28 00:54:05.676869 scikit_maad-1.4.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      609 2023-02-28 00:54:05.676938 scikit_maad-1.4.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1458 2024-04-27 17:22:25.511470 scikit_maad-1.4.2/.github/workflows/ci-cd.yml
+-rw-r--r--   0        0        0     1494 2023-02-28 00:54:05.677061 scikit_maad-1.4.2/.github/workflows/python-compatibility.yml
+-rw-r--r--   0        0        0     1734 2023-06-15 19:25:27.299155 scikit_maad-1.4.2/.gitignore
+-rw-r--r--   0        0        0      591 2023-02-28 00:54:05.677263 scikit_maad-1.4.2/CITATION.bib
+-rw-r--r--   0        0        0     5223 2023-02-28 00:54:05.677375 scikit_maad-1.4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3674 2023-03-10 21:26:34.971788 scikit_maad-1.4.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1505 2023-02-28 00:54:05.677527 scikit_maad-1.4.2/LICENSE
+-rw-r--r--   0        0        0     7090 2024-03-02 07:21:53.026412 scikit_maad-1.4.2/README.md
+-rw-r--r--   0        0        0     1239 2024-04-18 13:34:34.349239 scikit_maad-1.4.2/maad/__init__.py
+-rw-r--r--   0        0        0     5782 2023-11-29 17:34:08.591828 scikit_maad-1.4.2/maad/features/__init__.py
+-rw-r--r--   0        0        0   129783 2024-03-02 07:21:53.027629 scikit_maad-1.4.2/maad/features/alpha_indices.py
+-rw-r--r--   0        0        0     8692 2024-04-19 02:26:23.528114 scikit_maad-1.4.2/maad/features/composite_soundscape_descriptors.py
+-rw-r--r--   0        0        0    41647 2023-06-15 19:25:27.305113 scikit_maad-1.4.2/maad/features/shape.py
+-rwxr-xr-x   0        0        0    13949 2023-06-16 02:36:27.999414 scikit_maad-1.4.2/maad/features/spectral.py
+-rw-r--r--   0        0        0    13703 2023-06-16 02:39:32.947287 scikit_maad-1.4.2/maad/features/temporal.py
+-rw-r--r--   0        0        0     1024 2023-11-21 01:32:55.303856 scikit_maad-1.4.2/maad/rois/__init__.py
+-rw-r--r--   0        0        0     8114 2023-06-15 19:25:27.306255 scikit_maad-1.4.2/maad/rois/rois_1d.py
+-rw-r--r--   0        0        0    33504 2023-11-21 01:38:07.669166 scikit_maad-1.4.2/maad/rois/rois_2d.py
+-rw-r--r--   0        0        0     6379 2023-11-29 19:22:44.446889 scikit_maad-1.4.2/maad/rois/template_matching_func.py
+-rw-r--r--   0        0        0     2946 2023-02-28 00:54:06.300338 scikit_maad-1.4.2/maad/sound/__init__.py
+-rw-r--r--   0        0        0    16791 2023-06-15 19:25:27.307341 scikit_maad-1.4.2/maad/sound/filter.py
+-rw-r--r--   0        0        0    18024 2023-06-15 19:25:27.307882 scikit_maad-1.4.2/maad/sound/input_output.py
+-rw-r--r--   0        0        0     6185 2023-02-28 00:54:06.300692 scikit_maad-1.4.2/maad/sound/metrics.py
+-rw-r--r--   0        0        0    39987 2023-05-19 17:46:43.305247 scikit_maad-1.4.2/maad/sound/spectral_subtraction.py
+-rw-r--r--   0        0        0    18299 2023-02-28 00:54:06.300960 scikit_maad-1.4.2/maad/sound/spectro_func.py
+-rw-r--r--   0        0        0    18910 2023-05-19 17:46:43.307126 scikit_maad-1.4.2/maad/sound/transform.py
+-rw-r--r--   0        0        0     2665 2023-02-28 00:54:06.301271 scikit_maad-1.4.2/maad/sound/trim_func.py
+-rw-r--r--   0        0        0     1857 2023-03-10 21:26:34.972832 scikit_maad-1.4.2/maad/spl/__init__.py
+-rw-r--r--   0        0        0    33132 2023-02-28 00:54:06.301494 scikit_maad-1.4.2/maad/spl/active_space.py
+-rw-r--r--   0        0        0    23435 2024-03-27 01:54:24.024902 scikit_maad-1.4.2/maad/spl/conversion_SPL.py
+-rw-r--r--   0        0        0     5821 2024-04-18 13:34:34.349442 scikit_maad-1.4.2/maad/util/__init__.py
+-rw-r--r--   0        0        0    11066 2024-03-02 07:21:53.029097 scikit_maad-1.4.2/maad/util/audio_metadata_utilities.py
+-rw-r--r--   0        0        0    14953 2023-05-19 17:46:43.307469 scikit_maad-1.4.2/maad/util/math_func.py
+-rw-r--r--   0        0        0    36215 2023-11-19 21:29:33.608560 scikit_maad-1.4.2/maad/util/miscellaneous.py
+-rw-r--r--   0        0        0    19706 2024-04-23 16:33:59.740666 scikit_maad-1.4.2/maad/util/parser.py
+-rw-r--r--   0        0        0    88246 2024-04-23 16:33:59.741313 scikit_maad-1.4.2/maad/util/visualization.py
+-rw-r--r--   0        0        0    24620 2024-04-18 13:34:34.351668 scikit_maad-1.4.2/maad/util/xeno_canto.py
+-rw-r--r--   0        0        0       88 2024-04-27 19:40:45.962630 scikit_maad-1.4.2/maad/version.py
+-rw-r--r--   0        0        0     1726 2023-03-10 21:26:34.973235 scikit_maad-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     8720 1970-01-01 00:00:00.000000 scikit_maad-1.4.2/PKG-INFO
```

### Comparing `scikit_maad-1.4.1/.github/ISSUE_TEMPLATE/bug_report.md` & `scikit_maad-1.4.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/.github/ISSUE_TEMPLATE/feature_request.md` & `scikit_maad-1.4.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/.github/workflows/ci-cd.yml` & `scikit_maad-1.4.2/.github/workflows/ci-cd.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        os: [ubuntu-latest, windows-latest, macos-latest]
+        os: [ubuntu-latest, windows-latest, macos-13]
         python-version: ["3.8", "3.9", "3.10"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       id: cp310
```

### Comparing `scikit_maad-1.4.1/.github/workflows/python-compatibility.yml` & `scikit_maad-1.4.2/.github/workflows/python-compatibility.yml`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/.gitignore` & `scikit_maad-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/CITATION.bib` & `scikit_maad-1.4.2/CITATION.bib`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/CODE_OF_CONDUCT.md` & `scikit_maad-1.4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/CONTRIBUTING.md` & `scikit_maad-1.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/LICENSE` & `scikit_maad-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/README.md` & `scikit_maad-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/__init__.py` & `scikit_maad-1.4.2/maad/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,17 @@
     Compute descriptors to characterize sounds - :ref:`maad.features`
 
 rois
     Find regions of interest in 1D and 2D signals - :ref:`maad.rois`
 
 sound
     Load, preprocess and transform (e.g. stft) audio signals - :ref:`maad.sound`
+
+spl
+    Compute Sound Pressure Level (SPL) - :ref:`maad.spl`
     
 util
     Miscelaneous and useful set of tools used in the audio analysis framework - :ref:`maad.util`    
 """
 from .version import __version__
 
 # from . import spl
```

### Comparing `scikit_maad-1.4.1/maad/features/__init__.py` & `scikit_maad-1.4.2/maad/features/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/features/alpha_indices.py` & `scikit_maad-1.4.2/maad/features/alpha_indices.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/features/composite_soundscape_descriptors.py` & `scikit_maad-1.4.2/maad/features/composite_soundscape_descriptors.py`

 * *Files 3% similar despite different names*

```diff
@@ -207,18 +207,17 @@
     -------
     ax
         Axes of the figure
     """
     if ax == None:
         fig, ax = plt.subplots()
 
-    ax.imshow(graph.values.T, aspect='auto', origin='lower')
+    ax.imshow(graph.values.T, aspect='auto', origin='lower', 
+              extent=[int(graph.index[0]), int(graph.index[-1]), 
+                      graph.columns[0], graph.columns[-1]])
     ax.set_xlabel('Time (h)')
     ax.set_ylabel('Frequency (Hz)')
-    ytick_idx = np.arange(0, graph.shape[1], 20).astype(int)
-    ax.set_yticks(ytick_idx)
-    ax.set_yticklabels(graph.columns[ytick_idx].astype(float).astype(int).values)
 
     if savefig:
         plt.savefig(fname, bbox_inches='tight')
     
     return ax
```

### Comparing `scikit_maad-1.4.1/maad/features/shape.py` & `scikit_maad-1.4.2/maad/features/shape.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/features/spectral.py` & `scikit_maad-1.4.2/maad/features/spectral.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/features/temporal.py` & `scikit_maad-1.4.2/maad/features/temporal.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/rois/__init__.py` & `scikit_maad-1.4.2/maad/rois/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/rois/rois_1d.py` & `scikit_maad-1.4.2/maad/rois/rois_1d.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/rois/rois_2d.py` & `scikit_maad-1.4.2/maad/rois/rois_2d.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/rois/template_matching_func.py` & `scikit_maad-1.4.2/maad/rois/template_matching_func.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/sound/__init__.py` & `scikit_maad-1.4.2/maad/sound/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/sound/filter.py` & `scikit_maad-1.4.2/maad/sound/filter.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/sound/input_output.py` & `scikit_maad-1.4.2/maad/sound/input_output.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/sound/metrics.py` & `scikit_maad-1.4.2/maad/sound/metrics.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/sound/spectral_subtraction.py` & `scikit_maad-1.4.2/maad/sound/spectral_subtraction.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/sound/spectro_func.py` & `scikit_maad-1.4.2/maad/sound/spectro_func.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/sound/transform.py` & `scikit_maad-1.4.2/maad/sound/transform.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/sound/trim_func.py` & `scikit_maad-1.4.2/maad/sound/trim_func.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/spl/__init__.py` & `scikit_maad-1.4.2/maad/spl/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/spl/active_space.py` & `scikit_maad-1.4.2/maad/spl/active_space.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/spl/conversion_SPL.py` & `scikit_maad-1.4.2/maad/spl/conversion_SPL.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/util/__init__.py` & `scikit_maad-1.4.2/maad/util/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     plot_spectrum
     plot2d
     plot_spectrogram
     overlay_rois
     overlay_centroid
     plot_features_map
     plot_features
+    heatmap_by_date_and_time
     plot_correlation_map
     plot_shape
     false_Color_Spectro
 
 Mathematical
 ------------
 .. autosummary::
@@ -91,130 +92,138 @@
     audio_header
     filename_info
     get_metadata_file
     get_metadata_dir
 
 """
 
-from .miscellaneous import (index_bw,
-                           into_bins,
-                           shift_bit_length,
-                           rle,
-                           linear_scale,
-                           amplitude2dB,
-                           power2dB,
-                           dB2amplitude,
-                           dB2power,
-                           mean_dB,
-                           add_dB,
-                           nearest_idx,
-                           get_df_single_row,
-                           format_features,
-                           crossfade,
-                           crossfade_list)
-
-from .visualization import (rand_cmap,
-                           crop_image,
-                           save_figlist,
-                           plot1d,
-                           plot_wave,
-                           plot_spectrum,
-                           plot2d,
-                           plot_spectrogram,
-                           overlay_rois,
-                           overlay_centroid,
-                           plot_features_map,
-                           plot_features,
-                           plot_correlation_map,
-                           plot_shape,
-                           false_Color_Spectro)
-
-from .math_func import (running_mean,
-                         get_unimode,
-                         entropy,
-                         rms,
-                         kurtosis,
-                         skewness,
-                         moments)                     
-
-from .parser import (read_audacity_annot,
-                     write_audacity_annot,
-                     read_raven_annot,
-                     write_raven_annot,
-                     date_parser)
-
-from .xeno_canto import (xc_query,
-                         xc_multi_query,
-                         xc_selection,
-                         xc_download,
-                         # xc_save_csv,
-                         # xc_read_csv
-                         )
-
-from .audio_metadata_utilities import (check_file_format,
-                                       audio_header,
-                                       filename_info,
-                                       get_metadata_file,
-                                       get_metadata_dir)
+from .miscellaneous import (
+                        index_bw,
+                        into_bins,
+                        shift_bit_length,
+                        rle,
+                        linear_scale,
+                        amplitude2dB,
+                        power2dB,
+                        dB2amplitude,
+                        dB2power,
+                        mean_dB,
+                        add_dB,
+                        nearest_idx,
+                        get_df_single_row,
+                        format_features,
+                        crossfade,
+                        crossfade_list)
+
+from .visualization import (
+                        rand_cmap,
+                        crop_image,
+                        save_figlist,
+                        plot1d,
+                        plot_wave,
+                        plot_spectrum,
+                        plot2d,
+                        plot_spectrogram,
+                        overlay_rois,
+                        overlay_centroid,
+                        plot_features_map,
+                        heatmap_by_date_and_time,
+                        plot_features,
+                        plot_correlation_map,
+                        plot_shape,
+                        false_Color_Spectro)
+
+from .math_func import (
+                        running_mean,
+                        get_unimode,
+                        entropy,
+                        rms,
+                        kurtosis,
+                        skewness,
+                        moments)                     
+
+from .parser import (
+                    read_audacity_annot,
+                    write_audacity_annot,
+                    read_raven_annot,
+                    write_raven_annot,
+                    date_parser)
+
+from .xeno_canto import (
+                        xc_query,
+                        xc_multi_query,
+                        xc_selection,
+                        xc_download,
+                        # xc_save_csv,
+                        # xc_read_csv
+                        )
+
+from .audio_metadata_utilities import (
+                                    check_file_format,
+                                    audio_header,
+                                    filename_info,
+                                    get_metadata_file,
+                                    get_metadata_dir)
 
 __all__ = [
-           # miscellaneous 
-           'index_bw',
-           'into_bins',
-           'shift_bit_length',
-           'rle',
-           'linear_scale',
-           'amplitude2dB',
-           'power2dB',
-           'dB2amplitude',
-           'dB2power',
-           'mean_dB',
-           'add_dB',
-           'nearest_idx',
-           'get_df_single_row',
-           'format_features',
-           'crossfade',
-           'crossfade_list',
-           #  visualization      
-           'rand_cmap',
-           'crop_image',
-           'save_figlist',
-           'plot1d',
-           'plot_wave',
-           'plot_spectrum',
-           'plot2d',
-           'plot_spectrogram',
-           'overlay_rois',
-           'overlay_centroid',
-           'plot_features_map',
-           'plot_features',
-           'plot_correlation_map',
-           'plot_shape',
-           'false_Color_Spectro',
-           # math_func       
-           'running_mean',
-           'get_unimode',
-           'entropy',
-           'rms',
-           'kurtosis',
-           'skewness',
-           'moments',
-           # parser
-           'read_audacity_annot',
-           'write_audacity_annot',
-           'read_raven_annot',
-           'write_raven_annot',
-           'date_parser',
-           # xeno_canto
-           'xc_query',
-           'xc_multi_query',
-           'xc_selection',
-           'xc_download',
-           # 'xc_save_csv',
-           # 'xc_read_csv',
+            # miscellaneous 
+            'index_bw',
+            'into_bins',
+            'shift_bit_length',
+            'rle',
+            'linear_scale',
+            'amplitude2dB',
+            'power2dB',
+            'dB2amplitude',
+            'dB2power',
+            'mean_dB',
+            'add_dB',
+            'nearest_idx',
+            'get_df_single_row',
+            'format_features',
+            'crossfade',
+            'crossfade_list',
+            #  visualization      
+            'rand_cmap',
+            'crop_image',
+            'save_figlist',
+            'plot1d',
+            'plot_wave',
+            'plot_spectrum',
+            'plot2d',
+            'plot_spectrogram',
+            'overlay_rois',
+            'overlay_centroid',
+            'plot_features_map',
+            'plot_features',
+            'heatmap_by_date_and_time',
+            'plot_correlation_map',
+            'plot_shape',
+            'false_Color_Spectro',
+            # math_func       
+            'running_mean',
+            'get_unimode',
+            'entropy',
+            'rms',
+            'kurtosis',
+            'skewness',
+            'moments',
+            # parser
+            'read_audacity_annot',
+            'write_audacity_annot',
+            'read_raven_annot',
+            'write_raven_annot',
+            'date_parser',
+            # xeno_canto
+            'xc_query',
+            'xc_multi_query',
+            'xc_selection',
+            'xc_download',
+            # 'xc_save_csv',
+            # 'xc_read_csv',
             # audio_metadata_utilities
             'check_file_format',
             'audio_header',
             'filename_info',
             'get_metadata_file',
             'get_metadata_dir'
             ]
```

### Comparing `scikit_maad-1.4.1/maad/util/audio_metadata_utilities.py` & `scikit_maad-1.4.2/maad/util/audio_metadata_utilities.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/util/math_func.py` & `scikit_maad-1.4.2/maad/util/math_func.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/util/miscellaneous.py` & `scikit_maad-1.4.2/maad/util/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/maad/util/parser.py` & `scikit_maad-1.4.2/maad/util/parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 #%%
 # =============================================================================
 # Load the modules
 # =============================================================================
 # Import external modules
 import numpy as np 
 import pandas as pd
+import re
 import os
+import glob
 from datetime import datetime
 from pathlib import Path # in order to be Windows/linux/MacOS compatible
 
 
 #%%
 # =============================================================================
 # Private functions
@@ -122,40 +124,42 @@
         # the column contains a character
         tab_in[0] = tab_in[0].astype('str')
         if (tab_in[0].str.contains(r"\\", na = False).sum() > 0) :
 
             # arrange data
             t_info = tab_in.loc[np.arange(0, len(tab_in), 2), :]
             t_info = t_info.rename(index=str, columns={
-                                   0: 'min_t', 1: 'max_t', 2: 'label'})
+                                0: 'min_t', 1: 'max_t', 2: 'label'})
             t_info = t_info.reset_index(drop=True)
     
             f_info = tab_in.loc[np.arange(1, len(tab_in)+1, 2), :]
             f_info = f_info.rename(index=str, columns={
-                                   0: 'slash', 1: 'min_f', 2: 'max_f'})
+                                0: 'slash', 1: 'min_f', 2: 'max_f'})
             f_info = f_info.reset_index(drop=True)
     
             # return dataframe
-            tab_out = pd.concat([t_info['label'].astype('str'),
-                                 t_info['min_t'].astype('float32'),
-                                 f_info['min_f'].astype('float32'),
-                                 t_info['max_t'].astype('float32'),
-                                 f_info['max_f'].astype('float32')],  axis=1)
+            tab_out = pd.concat(
+                                [t_info['label'].astype('str'),
+                                t_info['min_t'].astype('float32'),
+                                f_info['min_f'].astype('float32'),
+                                t_info['max_t'].astype('float32'),
+                                f_info['max_f'].astype('float32')],  axis=1)
         else :
             tab_in = tab_in.rename(index=str, columns={
-                                   0: 'min_t', 1: 'max_t', 2: 'label'})
+                                0: 'min_t', 1: 'max_t', 2: 'label'})
             tab_in['min_f'] = np.nan
             tab_in['max_f'] = np.nan
             
             # return dataframe
-            tab_out = pd.concat([tab_in['label'].astype('str'),
-                                 tab_in['min_t'].astype('float32'),
-                                 tab_in['min_f'].astype('float32'),
-                                 tab_in['max_t'].astype('float32'),
-                                 tab_in['max_f'].astype('float32')],  axis=1)
+            tab_out = pd.concat([
+                                tab_in['label'].astype('str'),
+                                tab_in['min_t'].astype('float32'),
+                                tab_in['min_f'].astype('float32'),
+                                tab_in['max_t'].astype('float32'),
+                                tab_in['max_f'].astype('float32')],  axis=1)
     except :
         tab_out = pd.DataFrame()
 
     return tab_out
 
 #%%
 def write_audacity_annot(fname, df_rois, save_file=True):
@@ -173,15 +177,17 @@
         filename to save the segmentation
     df_rois: pandas dataframe
         Dataframe containing the coordinates corresponding to sound signatures
         In case of only temporal annotations : df_rois must contain at least
         the columns 'mint_t', 'max_t' 
         In case of bounding box (temporal eand frequency limits) :: df_rois 
         must contain at least the columns 'min_t', 'max_t', 'min_f', 'max_f'
-            
+    save_file: bool, optional, default=True
+        If True, the file is saved. If False, the file is not saved.
+
     Returns
     -------
     df_to_save
         Dataframe that has been saved
     
     Examples
     --------
@@ -211,25 +217,25 @@
         # if there is no label, create a vector with incremental values
         if 'label' not in df_rois:
             df_rois['label'] = np.arange(0,len(df_rois))
         
         # if no frequency coordinates, only temporal annotations
         if ('min_f' not in df_rois) or ('max_f' not in df_rois):
             df_to_save = pd.DataFrame({'min_t':df_rois.min_t, 
-                                       'max_t':df_rois.max_t, 
-                                       'label':df_rois.label})
+                                    'max_t':df_rois.max_t, 
+                                    'label':df_rois.label})
         else:
             df_to_save_odd = pd.DataFrame({'index': np.arange(0,len(df_rois)*2,2),
                                         'min_t':df_rois.min_t, 
                                         'max_t':df_rois.max_t, 
                                         'label':df_rois.label})
             df_to_save_even = pd.DataFrame({'index': np.arange(1,len(df_rois)*2,2),
-                                         'min_t':'\\', 
-                                         'max_t':df_rois.min_f, 
-                                         'label':df_rois.max_f})
+                                        'min_t':'\\', 
+                                        'max_t':df_rois.min_f, 
+                                        'label':df_rois.max_f})
             df_to_save = pd.concat([df_to_save_odd,df_to_save_even])
             df_to_save = df_to_save.set_index('index')
             df_to_save = df_to_save.sort_index()
             
     if save_file:
         df_to_save.to_csv(fname, index=False, header=False, sep='\t') 
     else:
@@ -311,97 +317,196 @@
         if not('View' in df_out.columns):
             df_out['View'] = 'Spectrogram 1'
         
         if not('Channel' in df_out.columns):
             df_out['Channel'] = 1
         
         # change column names
-        df_out.rename(columns={'min_t': 'Begin Time (s)', 
-                           'max_t': 'End Time (s)',
-                           'min_f': 'Low Freq (Hz)',
-                           'max_f': 'High Freq (Hz)'}, inplace=True)
+        df_out.rename(columns={
+                        'min_t': 'Begin Time (s)', 
+                        'max_t': 'End Time (s)',
+                        'min_f': 'Low Freq (Hz)',
+                        'max_f': 'High Freq (Hz)'}, inplace=True)
         
         # reorder column names
         colname_raven = ['Selection', 'View', 'Channel', 'Begin Time (s)',
-                         'End Time (s)', 'Low Freq (Hz)', 'High Freq (Hz)']
+                        'End Time (s)', 'Low Freq (Hz)', 'High Freq (Hz)']
         colname_order = colname_raven + df_out.columns[~df_out.columns.isin(colname_raven)].tolist()
         df_out = df_out.reindex(columns=colname_order)
         
         if save_file:
             df_out.to_csv(fname, sep='\t', index=False)
         else:
             pass
     
     return df_out
 
-
 #%%
-def date_parser (datadir, dateformat ="SM4", extension ='.wav', verbose=False):
+def date_parser(datadir, dateformat='%Y%m%d_%H%M%S', extension='.wav', prefix = '', verbose=False):
     """
-    Parse all filenames contained in a directory and its subdirectories.
-    
-    Keeps only filenames corresponding to extension.
-    Filenames must follow :
-        
-    - SM4 format (XXXX_yyyymmdd_hhmmss.wav) 
-    - or POSIX format (for audiomoth)  
-    
-    The result is a panda dataframe with 'Date' as index and 'File' (with full path as column) 
-    
+    Extracts dates from filenames in a given folder and subfolders.
+
     Parameters
     ----------
-    filename : string
-        filename must follow 
-        - SM4 format : XXXX_yyyymmdd_hhmmss.wav, ex: S4A03895_20190522_191500.wav
-        - Audiomoth format : 8 Hexa, ex: 5EE84AC8.wav
-            
+    datadir : str
+        Path to the folder to search for files.
+    dateformat : str, optional
+        Format string specifying the datetime pattern to extract.
+        The default is'%Y%m%d_%H%M%S'
+        For more information about the format codes, refer to the
+        `strftime format documentation <https://strftime.org/>`_.
+    extension : str, optional, 
+        File extension to filter files by (e.g., '.wav', '.mp3').
+        The default is '.wav'.
+    prefix : str, optional, 
+        Prefix of the filenames to match.
+        The default is ''.
+    verbose : bool, optional
+        If True, print the filenames as they are processed.
+        The default is False.
+
     Returns
     -------
-    df : Pandas dataframe
-        This dataframe has one column
-        - 'file' => full path + filename
-        and a index 'Date' with the type Datetime
-    
+    pandas.DataFrame
+        DataFrame containing the extracted dates as the index 'Date',
+        and the full file paths in a 'file' column.
+
+    Raises
+    ------
+    ValueError
+        If the datetime_format is invalid or does not match the filenames.
+
+    Notes
+    -----
+    This function searches for files in the specified folder and its subfolders
+    that have the given extension and match the specified prefix. It extracts
+    the dates from the filenames using the provided datetime_format.
+
+    The extracted dates are set as the index of the resulting DataFrame. The
+    'file' column contains the full file paths.
+
     Examples
     --------
-    >>> df = maad.util.date_parser("../data/indices/", dateformat='SM4', verbose=True)
+    >>> folder_path = '../../data/indices/'
+    >>> ext = '.wav'
+    >>> datetime_format = '%Y%m%d_%H%M%S'
+    >>> df = maad.util.date_parser(datadir=folder_path, dateformat=datetime_format, extension=ext)
+    >>> df
+                                                                    file
+    Date	
+    2019-05-22 00:00:00	../../data/indices/S4A03895_20190522_000000.wav
+    2019-05-22 00:15:00	../../data/indices/S4A03895_20190522_001500.wav
+    2019-05-22 00:30:00	../../data/indices/S4A03895_20190522_003000.wav
+    2019-05-22 00:45:00	../../data/indices/S4A03895_20190522_004500.wav
+    2019-05-22 01:00:00	../../data/indices/S4A03895_20190522_010000.wav
+                    ...	                                            ...
+    2019-05-22 22:45:00	../../data/indices/S4A03895_20190522_224500.wav
+    2019-05-22 23:00:00	../../data/indices/S4A03895_20190522_230000.wav
+    2019-05-22 23:15:00	../../data/indices/S4A03895_20190522_231500.wav
+    2019-05-22 23:30:00	../../data/indices/S4A03895_20190522_233000.wav
+    2019-05-22 23:45:00	../../data/indices/S4A03895_20190522_234500.wav
+
+
+    >>> df = maad.util.date_parser("../../data/indices/", dateformat='SM4', verbose=False)
     >>> list(df)
     >>> df
-                                                                 file
-    Date                                                             
-    2019-05-22 00:00:00  ../data/indices/S4A03895_20190522_000000.wav
-    2019-05-22 00:15:00  ../data/indices/S4A03895_20190522_001500.wav
-    2019-05-22 00:30:00  ../data/indices/S4A03895_20190522_003000.wav
-    2019-05-22 00:45:00  ../data/indices/S4A03895_20190522_004500.wav
-    2019-05-22 01:00:00  ../data/indices/S4A03895_20190522_010000.wav
-    2019-05-22 01:15:00  ../data/indices/S4A03895_20190522_011500.wav
-    2019-05-22 01:30:00  ../data/indices/S4A03895_20190522_013000.wav
-    2019-05-22 01:45:00  ../data/indices/S4A03895_20190522_014500.wav
-    2019-05-22 02:00:00  ../data/indices/S4A03895_20190522_020000.wav
-    ...
-    """
-    
-    c_file = []
-    c_date = []
-    # find a file in subdirectories
-    for root, subFolders, files in os.walk(datadir):
-        for count, file in enumerate(files):
-            if verbose: print(file)
-            if extension.upper() in file or extension.lower() in file :
-                filename = os.path.join(root, file)
-                file_stem = Path(filename).stem
-                c_file.append(filename) 
-                if dateformat == "SM4":
-                    c_date.append(_date_from_filename(file_stem))      
-                elif dateformat == "POSIX" :
-                    posix_time = int(file_stem, 16)
-                    dd = datetime.utcfromtimestamp(posix_time).strftime('%Y-%m-%d %H:%M:%S')
-                    c_date.append(dd)                          
-                
-    ####### SORTED BY DATE
-    # create a Pandas dataframe with date as index
-    df = pd.DataFrame({'file':c_file, 'Date':c_date})
-    # define Date as index
-    df.set_index('Date', inplace=True)
-    # sort dataframe by date
-    df = df.sort_index(axis=0)
+                                                                    file
+    Date	
+    2019-05-22 00:00:00	../../data/indices/S4A03895_20190522_000000.wav
+    2019-05-22 00:15:00	../../data/indices/S4A03895_20190522_001500.wav
+    2019-05-22 00:30:00	../../data/indices/S4A03895_20190522_003000.wav
+    2019-05-22 00:45:00	../../data/indices/S4A03895_20190522_004500.wav
+    2019-05-22 01:00:00	../../data/indices/S4A03895_20190522_010000.wav
+                    ...	                                            ...
+    2019-05-22 22:45:00	../../data/indices/S4A03895_20190522_224500.wav
+    2019-05-22 23:00:00	../../data/indices/S4A03895_20190522_230000.wav
+    2019-05-22 23:15:00	../../data/indices/S4A03895_20190522_231500.wav
+    2019-05-22 23:30:00	../../data/indices/S4A03895_20190522_233000.wav
+    2019-05-22 23:45:00	../../data/indices/S4A03895_20190522_234500.wav
+
+
+    """    
+
+    file_pattern = os.path.join(datadir, f'**/{prefix}*{extension}')
+    file_list = glob.glob(file_pattern, recursive=True)
+    data = []
+
+    for file_path in file_list:
+
+        # Extract the filename from the full path
+        filename = os.path.basename(file_path)
+
+        if dateformat == 'SM4':
+            date =_date_from_filename(filename)
+            data.append({'Date': date, 'file': file_path})
+        
+        elif dateformat == 'POSIX':
+            posix_time = int(Path(filename).stem, 16)
+            date = datetime.utcfromtimestamp(posix_time).strftime('%Y-%m-%d %H:%M:%S')
+            data.append({'Date': date, 'file': file_path})
+
+        else: 
+            # Construct a regex pattern to extract the date from the filename
+            pattern = _construct_pattern(dateformat)
+            # Search for the date in the filename
+            match = pattern.search(filename)
+            # If a match is found, extract the date
+            if match:
+                if verbose:
+                    print(f'File: {filename}')
+                # Extract the date from the filename
+                date_str = match.group()
+                # Parse the date string
+                try:
+                    date = datetime.strptime(date_str, dateformat)
+                    data.append({'Date': date, 'file': file_path})
+                except ValueError:
+                    print(f"Error parsing date: {date_str} in file: {filename}. The default date and time 1900-01-01 00:00:00 will be used.")
+                    # date by default
+                    data.append({'Date': "1900-01-01 00:00:01", 'file': file_path})
+            else:
+                print(f"No date found in file: {file_path}. The default date and time 1900-01-01 00:00:00 will be used.")
+                # date by default 1900-01-01 00:00:00
+                data.append({'Date': "1900-01-01 00:00:01", 'file': file_path})
+    if len(data) > 0:
+        df = pd.DataFrame(data)
+        df.set_index('Date', inplace=True)
+        # convert index to datetime 
+        df.index = pd.DatetimeIndex(df.index)
+        # sort dataframe by date
+        df = df.sort_index(axis=0)
+    else:
+        df = pd.DataFrame()
+
     return df
+
+def _construct_pattern(datetime_format):
+    format_dict = {
+        '%Y': r'(\d{4})',
+        '%y': r'(\d{2})',
+        '%m': r'(0[1-9]|1[0-2])',
+        '%d': r'(0[1-9]|1\d|2[0-9]|3[01])',
+        '%H': r'([01]\d|2[0-3])',
+        '%I': r'(0[1-9]|1[0-2])',
+        '%p': r'(AM|PM)',
+        '%M': r'([0-5]\d)',
+        '%S': r'([0-5]\d)',
+        '%f': r'(\d{6})',
+        '%j': r'(\d{3})',
+        '%U': r'(\d{2})',
+        '%W': r'(\d{2})',
+        '%w': r'(\d)',
+        '%A': r'(\w+)',
+        '%a': r'(\w+)',
+        '%B': r'(\w+)',
+        '%b': r'(\w+)',
+        '%c': r'(.+)',
+        '%x': r'(.+)',
+        '%X': r'(.+)',
+        '%%': r'%',
+    }
+    pattern = datetime_format
+    for code, regex in format_dict.items():
+        pattern = pattern.replace(code, regex)
+    pattern = re.compile(pattern)
+
+    return pattern
```

### Comparing `scikit_maad-1.4.1/maad/util/visualization.py` & `scikit_maad-1.4.2/maad/util/visualization.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from matplotlib.colors import LinearSegmentedColormap
 import matplotlib.patches as mpatches
 from matplotlib.axes import Axes
 import pandas as pd
 from skimage.io import imsave
 import colorsys
 from ast import literal_eval
+from datetime import datetime
 
 # min value
 import sys
 
 _MIN_ = sys.float_info.min
 
 # Importation from internal modules
@@ -34,47 +35,192 @@
             "`axes` must be an instance of matplotlib.axes.Axes. "
             "Found type(axes)={}".format(type(axes))
         )
     return axes
 
 
 #%%
+def _is_single_value(value):
+    """
+    Check if a value is a single numeric value or a single character.
+
+    Parameters:
+    -----------
+        value (int, float, str): The value to be checked.
+
+    Returns:
+    --------
+        bool: True if the value is a single numeric value or a single character, False otherwise.
+    """
+    if isinstance(value, (int, float, str)):
+        if isinstance(value, (int, float)):
+            return True  # It's a numeric value
+        elif isinstance(value, str):
+            # Check if it's a single numeric character (0-9)
+            if len(value) == 1 and value.isdigit():
+                return True  # It's a single numeric character
+            else:
+                return False  # It's a string, but not a single character
+    return False  # It's not a single value
+
+#%%
+MIN_V = 1 # min week number possible
+MIN_m = 1 # min month number possible
+MIN_d = 1 # min day number possible
+MIN_H = 0 # min hour number possible
+MIN_M = 0 # min minute number possible
+
+MAX_V = 53 # max week number possible
+MAX_m = 12 # max month number possible
+MAX_d = 31 # max day number possible
+MAX_H = 23 # max hour number possible
+MAX_M = 59 # max minute number possible
+
+def _filter_dataframe_by_datetime(df, date_format, date_range):
+    """
+    Filter a DataFrame based on a specified date format and date range.
+
+    Parameters:
+    -----------
+        df : pandas.DataFrame
+            The DataFrame to be filtered.
+        date_format :str
+            The format of the date to be extracted from the DataFrame's index.
+        date_range : int, str, list
+            The range of dates to filter the DataFrame by.
+
+    Returns:
+    --------
+        pandas.DataFrame: The filtered DataFrame.
+
+    Raises:
+    -------
+        ValueError: If the date_format is not allowed or if the date_range is not a single value or a list.
+
+    Note:
+    -----
+        The date_format parameter can be one of the following:
+        - "%V": Week number
+        - "%Y": Year
+        - "%m-%d": Month and day
+        - "%a": Weekday
+        - "%m": Month
+        - "%d": Day
+        - "%y-%m-%d": Year, Month, and Day
+        - "%H:%M": Hour and minute (e.g., "13:42")
+
+        The date_range parameter can be one of the following:
+        - A single value (int or str) representing a specific date or time.
+        - A list of values (int or str) representing a range of dates or times.
+        For example, ["01-01", "01-31"] represents a range of dates from January 1st to January 31st.
+
+    """
+    # Extract the date portion from the DatetimeIndex based on the specified date format
+    try:
+        df['date_type'] = df.index.strftime(date_format)
+    except :
+        raise ValueError('Error in the date_format. Check the date_format parameter')
+
+    if _is_single_value(date_range) == True :
+        if (date_format == "%V") or (date_format == "%Y") or (date_format == "%m") or (date_format == "%d"):
+            # Filter by week number or by year or by month
+            df_filtered = df[df['date_type'].astype(int) == date_range]
+        elif (date_format == "%m-%d") or (date_format == "%H:%M") or (date_format == "%a") or (date_format == "%y-%m-%d"):
+            # Filter by time (hour:minutes)
+            # Filter by weekday (e.g., "Mon" for Monday)
+            # Filter by year-month-day (e.g., "23-01-01" for January 1, 2023)
+            # Filter by month and day (e.g., "01-01" for January 1)
+            df_filtered = df[df['date_type'] == date_range]
+        else :
+            print("Filtering was no possible. date_format {} is not allowed".format(date_format))
+            df_filtered = df
+
+    elif (len(date_range)==1) or(len(date_range)>2):
+        if (date_format == "%V") or (date_format == "%Y") or (date_format == "%m") or (date_format == "%d"):
+            # Filter by week number or by year or by month
+            df_filtered = df[df['date_type'].astype(int).isin(date_range)]
+        elif (date_format == "%m-%d") or (date_format == "%H:%M") or (date_format == "%a") or (date_format == "%y-%m-%d"):
+            # Filter by time (hour:minutes)
+            # Filter by weekday (e.g., "Mon" for Monday)
+            # Filter by year-month-day (e.g., "23-01-01" for January 1, 2023)
+            # Filter by month and day (e.g., "01-01" for January 1)
+            df_filtered = df[df['date_type'].isin(date_range)]
+        else :
+            print("Filtering was no possible. date_format {} is not allowed".format(date_format))
+            df_filtered = df
+    else:
+        if isinstance(date_range, list) : 
+            if (date_format == "%V") or (date_format == "%Y") or (date_format == "%m") or (date_format == "%d"):
+                # Filter by week number or by year or by month
+                df_filtered = df[df['date_type'].astype(int).between(date_range[0], date_range[1])]
+            elif (date_format == "%m-%d") or (date_format == "%H:%M") or (date_format == "%a") or (date_format == "%y-%m-%d"):
+                # Filter by time (hour:minutes)
+                # Filter by weekday (e.g., "Mon" for Monday)
+                # Filter by year-month-day (e.g., "23-01-01" for January 1, 2023)
+                # Filter by month and day (e.g., "01-01" for January 1)
+                if date_range[0] <= date_range[1] :
+                    df_filtered = df[df['date_type'].between(str(date_range[0]), str(date_range[1]))]
+                else :
+                    if date_format == "%H:%M" : 
+                        MAX = f'{MAX_H:02}:{MAX_M:02}'
+                        df_filtered_part1 = df[df['date_type'].between(str(date_range[0]), MAX)] 
+                        MIN = f'{MIN_H:02}:{MIN_M:02}'
+                        df_filtered_part2 = df[df['date_type'].between(MIN, str(date_range[1]))]  
+                        df_filtered = pd.concat([df_filtered_part1, df_filtered_part2], axis = 0)
+                    else :
+                        print("Filtering was no possible. The range must increase")
+                        df_filtered = df
+            else :
+                print("Filtering was no possible. date_format {} is not allowed".format(date_format))
+                df_filtered = df
+        else :
+            print("Filtering was no possible. date_range must be a single value or a list")
+            df_filtered = df
+
+    # Check if 'data_type' is in the DataFrame's columns
+    if 'date_type' in df_filtered.columns:
+        # If it exists, drop the column
+        df_filtered = df_filtered.drop('date_type', axis=1)
+
+    return df_filtered
+
+#%%
 def plot_shape(shape, params, row=0, ax=None, display_values=False):
     """ 
     Plot shape features in a bidimensional plot.
-     
+    
     Parameters 
     ---------- 
     shape: 1D array, pd.Series or pd.DataFrame 
         Shape features computed with shape_features function. 
-     
+    
     params: pd.DataFrame 
         Pandas dataframe returned by maad.features_rois.shape_features 
-     
+    
     row: int 
         Observation to be visualized 
-     
+    
     display_values: bool 
         Set to True to display the coefficient values. Default is False. 
-     
+    
     Returns 
     ------- 
     ax: matplotlib.axes 
         Axes of the figure 
-         
+    
     Examples 
     -------- 
     >>> from maad.sound import load, spectrogram 
     >>> from maad.features import shape_features, plot_shape 
     >>> import numpy as np 
     >>> s, fs = load('../data/spinetail.wav') 
     >>> Sxx, ts, f, ext = spectrogram(s, fs) 
     >>> shape, params = shape_features(np.log10(Sxx), resolution='high') 
     >>> plot_shape(shape, params) 
- 
+
     """
 
     # compute shape of matrix
     dirs_size = params.theta.unique().shape[0]
     scale_size = np.unique(params.freq).size * np.unique(params.pyr_level).size
     # reshape feature vector
     idx = params.sort_values(["theta", "pyr_level", "scale"]).index
@@ -114,108 +260,107 @@
     ax.set_yticklabels(yticklab)
     ax.set_xlabel("Scale")
     ax.set_ylabel("Theta")
     plt.show()
 
     return ax
 
-
 #%%
 def overlay_centroid(im_ref, centroid, savefig=None, **kwargs):
     """ 
     Overlay centroids on the original spectrogram 
-     
+    
     Parameters 
     ---------- 
     Sxx :  2D array 
         Spectrogram 
-               
+        
     centroid: pandas DataFrame 
         DataFrame with centroid descriptors (centroid_f, centroid_t) 
         Do format_features(rois,tn,fn) before using overlay_centroid to be sure that 
         the format of the DataFrame is correct 
-             
+            
     savefig : string, optional, default is None 
         Root filename (with full path) is required to save the figures. Postfix 
         is added to the root filename. 
-         
+        
     kwargs, optional. This parameter is used by plt.plot and savefig functions 
             
         - savefilename : str, optional, default :'_spectro_overlaycentroid.png' 
             Postfix of the figure filename 
-         
+        
         - extent : list of scalars [left, right, bottom, top], optional, default: None
             The location, in data-coordinates, of the lower-left and
             upper-right corners. If `None`, the image is positioned such that
             the pixel centers fall on zero-based (row, column) indices.
-         
+        
         - title : string, optional, default : 'Spectrogram' 
             title of the figure 
-         
+        
         - xlabel : string, optional, default : 'Time [s]' 
             label of the horizontal axis 
-         
+        
         - ylabel : string, optional, default : 'Amplitude [AU]' 
             label of the vertical axis 
-         
+        
         - cmap : string or Colormap object, optional, default is 'gray' 
             See https://matplotlib.org/examples/color/colormaps_reference.html 
             in order to get all the  existing colormaps 
             examples: 'hsv', 'hot', 'bone', 'tab20c', 'jet', 'seismic',  
             'viridis'... 
-         
+        
         - vmin, vmax : scalar, optional, default: None 
             `vmin` and `vmax` are used in conjunction with norm to normalize 
             luminance data.  Note if you pass a `norm` instance, your 
             settings for `vmin` and `vmax` will be ignored. 
-                 
+        
         - dpi : integer, optional, default is 96 
             Dot per inch.  
             For printed version, choose high dpi (i.e. dpi=300) => slow 
             For screen version, choose low dpi (i.e. dpi=96) => fast 
-         
+        
         - format : string, optional, default is 'png' 
             Format to save the figure  
-         
+        
         ... and more, see matplotlib  
- 
+
     Returns 
     ------- 
     ax  
         axis object (see matplotlib) 
     fig  
         figure object (see matplotlib) 
- 
+
     Examples
     --------
- 
+
     Get centroid from the whole power spectrogram 
- 
+
     >>> from maad.sound import load, spectrogram
     >>> from maad.features import centroid_features
     >>> from maad.util import (power2dB, format_features, overlay_rois, plot2d,
-                               overlay_centroid)
-     
+                            overlay_centroid)
+    
     Load audio and compute spectrogram 
-     
+    
     >>> s, fs = load('../data/spinetail.wav') 
     >>> Sxx,tn,fn,ext = spectrogram(s, fs, db_range=80) 
     >>> Sxx = power2dB(Sxx, db_range=80)
-     
+    
     Load annotations and plot
     
     >>> from maad.util import read_audacity_annot
     >>> rois = read_audacity_annot('../data/spinetail.txt') 
     >>> rois = format_features(rois, tn, fn) 
     >>> ax, fig = plot2d (Sxx, extent=ext)
     >>> ax, fig = overlay_rois(Sxx,rois, extent=ext, ax=ax, fig=fig)
     
     Compute the centroid of each rois, format to get results in the 
     temporal and spectral domain and overlay the centroids.
-     
+    
     >>> centroid = centroid_features(Sxx, rois) 
     >>> centroid = format_features(centroid, tn, fn)
     >>> ax, fig = overlay_centroid(Sxx,centroid, extent=ext, ax=ax, fig=fig)
     
     """
     
     # Check format of the input data
@@ -269,28 +414,27 @@
         format = kwargs.pop("format", "png")
         filename = kwargs.pop("filename", "_spectro_overlaycentroid")
         filename = savefig + filename + "." + format
         fig.savefig(filename, bbox_inches="tight", dpi=dpi, format=format, **kwargs)
 
     return ax, fig
 
-
 #%%
 def overlay_rois(im_ref, rois, edge_color=None, unique_labels= None, 
                  textbox_label=False, savefig=None, **kwargs):
     """ 
     Display bounding boxes with time-frequency regions of interest over a spectrogram.
     
     Regions of interest (ROIs) must be provided. They can be loaded as manual annotations or computed using automated methods (see the example section).
-     
+    
     Parameters 
     ---------- 
     im_ref : 2d ndarray of scalars 
         Spectrogram (or image) 
- 
+
     rois_bbox : pandas.DataFrame
         Contains the bounding box of each ROI. The pandas.DataFrame must have columns
         ['min_x', 'max_x', 'min_y', 'max_y']. If your data is in the time-frequency
         format ['min_t', 'max_t', 'min_f', 'max_f'], use the function
         maad.util.format_features to get the cooresponding
         x, y coordinates.
         
@@ -312,63 +456,63 @@
         a list is given as argument, the number element in the list should 
         be the same as the number of edge_color
     
     textbox_label: bool
         Display a text box above the bounding box indicating the name of the label.
         The rois_bbox pandas.DataFrame must have a column called 'label' with names
         assigned to each ROI.
- 
+
     savefig : string, optional, default is None 
         Root filename (with full path) is required to save the figures. Postfix 
         is added to the root filename. 
-         
+        
     kwargs, optional. This parameter is used by plt.plot and savefig functions 
             
         - savefilename : str, optional, default :'_spectro_overlayrois.png' 
             Postfix of the figure filename 
             
         - extent : list of scalars [left, right, bottom, top], optional, default: None
             The location, in data-coordinates, of the lower-left and
             upper-right corners. If `None`, the image is positioned such that
             the pixel centers fall on zero-based (row, column) indices.  
-         
+        
         - title : string, optional, default : 'Spectrogram' 
             title of the figure 
-         
+        
         - xlabel : string, optional, default : 'Time [s]' 
             label of the horizontal axis 
-         
+        
         - ylabel : string, optional, default : 'Amplitude [AU]' 
             label of the vertical axis 
-         
+        
         - cmap : string or Colormap object, optional, default is 'gray' 
             See https://matplotlib.org/examples/color/colormaps_reference.html 
             in order to get all the  existing colormaps 
             examples: 'hsv', 'hot', 'bone', 'tab20c', 'jet', 'seismic',  
             'viridis'... 
-         
+        
         - vmin, vmax : scalar, optional, default: None 
             `vmin` and `vmax` are used in conjunction with norm to normalize 
             luminance data.  Note if you pass a `norm` instance, your 
             settings for `vmin` and `vmax` will be ignored. 
-         
+        
         - dpi : integer, optional, default is 96 
             Dot per inch.  
             For printed version, choose high dpi (i.e. dpi=300) => slow 
             For screen version, choose low dpi (i.e. dpi=96) => fast 
-         
+        
         - format : string, optional, default is 'png' 
             Format to save the figure  
-         
+        
         ... and more, see matplotlib  
- 
+
     Returns 
     ------- 
     ax : axis object (see matplotlib) 
-         
+        
     fig : figure object (see matplotlib) 
     
     Examples 
     -------- 
     
     Simple display of bounding boxes over the spectrogram.
     
@@ -516,15 +660,15 @@
             linewidth=1,
         )
         # draw the rectangle
         ax.add_patch(rect)
         
         if textbox_label:
             textbox = dict(boxstyle='square', fc=color[ii], 
-                           ec=color[ii], alpha=1, pad=0, linewidth=2)
+                        ec=color[ii], alpha=1, pad=0, linewidth=2)
             ax.text(x0*x_scaling + xmin, (y1+2)*y_scaling + ymin, 
                     str(row.label), 
                     color='white',
                     fontweight='semibold',
                     fontsize='small',
                     fontfamily='sans-serif',
                     fontvariant='small-caps',
@@ -540,25 +684,24 @@
         format = kwargs.pop("format", "png")
         filename = kwargs.pop("filename", "_spectro_overlayrois")
         filename = savefig + filename + "." + format
         fig.savefig(filename, bbox_inches="tight", dpi=dpi, format=format, **kwargs)
 
     return ax, fig
 
-
 #%%
 def plot1d(x, y, ax=None, **kwargs):
     """
     Plot the waveform or spectrum of an audio signal. 
     
     Parameters
     ----------
     x : 1d ndarray of integer
         Vector containing the abscissa values (horizontal axis)
-             
+        
     y : 1d ndarray of scalar
         Vector containing the ordinate values (vertical axis)  
     
     ax : axis, optional, default is None
         Draw the signal on this specific axis. Allow multiple plots on the same
         axis.
             
@@ -621,23 +764,23 @@
     >>> fig, ax = maad.util.plot1d(tn,s)
     
     >>> Sxx_power,tn,fn,_ = maad.sound.spectrogram(s,fs)
     
     Convert spectrogram into dB SPL
     
     >>> Lxx = maad.spl.power2dBSPL(Sxx_power, gain=42) 
-       
+    
     Plot the spectrum at t = 7s
     
     >>> index = maad.util.nearest_idx(tn,7)
     >>> fig_kwargs = {'figtitle':'Spectrum (PSD)',
-                      'xlabel':'Frequency [Hz]',
-                      'ylabel':'Power [dB]',
-                      'linewidth': 0.5
-                      }
+                    'xlabel':'Frequency [Hz]',
+                    'ylabel':'Power [dB]',
+                    'linewidth': 0.5
+                    }
     
     >>> fig, ax = maad.util.plot1d(fn, Lxx[:,index], **fig_kwargs)
     """
 
     figsize = kwargs.pop("figsize", (4, 10))
     facecolor = kwargs.pop("facecolor", "w")
     edgecolor = kwargs.pop("edgecolor", "k")
@@ -680,15 +823,14 @@
 
     # Display the figure now
     if now:
         plt.show()
 
     return ax, fig
 
-
 #%%
 def plot_wave(s, fs, tlims=None, ax=None, **kwargs):
     """
     Plot audio waveform.
     
     Parameters
     ----------
@@ -737,15 +879,14 @@
     else:
         t = np.linspace(0, s.shape[0] / fs, s.shape[0])
 
     ax, fig = plot1d(t, s, ax, **kwargs)
 
     return ax
 
-
 #%%
 def plot_spectrum(pxx, f_idx, ax=None, flims=None, log_scale=False, fill=True, **kwargs):
     """
     Plot power spectral density estimate (PSD).
     
     Parameters
     ----------
@@ -815,28 +956,27 @@
     amp_min = pxx.min()
     ax, fig = plot1d(f_idx, pxx, ax=ax, ylabel=ylabel, xlabel=xlabel, **kwargs)
     if fill:
         ax.fill_between(f_idx, amp_min, pxx, alpha=0.3, fc="grey")
 
     return ax
 
-
 #%%
 def plot2d(im, ax=None, colorbar=True, **kwargs):
     """
     Display the spectrogram of an audio signal. 
     
     The spectrogram should be previously computed using the function 
     ``maad.sound.spectrogram``.
     
     Parameters
     ----------
     im : 2D numpy array 
         Image or Spectrogram
-             
+        
     ax : axis, optional, default is None
         Draw the image on this specific axis. Allow multiple plots on the same
         figure.
             
     kwargs, optional
         - figsize : tuple of integers, optional, default: (4,13)
             width, height in inches.  
@@ -866,17 +1006,17 @@
             upper-right corners. If `None`, the image is positioned such that
             the pixel centers fall on zero-based (row, column) indices.
         - now : boolean, optional, default : True
             if True, display now. Cannot display multiple images. 
             To display mutliple images, set now=False until the last call for 
             the last image    
         - interpolation : list of string [None, 'none', 'nearest', 'bilinear', 
-           'bicubic', 'spline16','spline36', 'hanning', 'hamming', 'hermite', 
-           'kaiser', 'quadric','catrom', 'gaussian', 'bessel', 'mitchell', 
-           'sinc', 'lanczos'], optional, default : None
+            'bicubic', 'spline16','spline36', 'hanning', 'hamming', 'hermite', 
+            'kaiser', 'quadric','catrom', 'gaussian', 'bessel', 'mitchell', 
+            'sinc', 'lanczos'], optional, default : None
             
         ... and more, see matplotlib
         
     Returns
     -------
     fig : Figure
         The Figure instance 
@@ -885,20 +1025,20 @@
         
     Examples
     --------
     >>> w, fs = maad.sound.load('../data/cold_forest_daylight.wav') 
     >>> Sxx_power,tn,fn,_ = maad.sound.spectrogram(w,fs)
     >>> Lxx = maad.spl.power2dBSPL(Sxx_power, gain=42) # convert into dB SPL
     >>> fig_kwargs = {'vmax': Lxx.max(),
-                      'vmin':0,
-                      'extent':(tn[0], tn[-1], fn[0], fn[-1]),
-                      'title':'Power spectrogram density (PSD) in dB SPL',
-                      'xlabel':'Time [s]',
-                      'ylabel':'Frequency [Hz]',
-                      }
+                    'vmin':0,
+                    'extent':(tn[0], tn[-1], fn[0], fn[-1]),
+                    'title':'Power spectrogram density (PSD) in dB SPL',
+                    'xlabel':'Time [s]',
+                    'ylabel':'Frequency [Hz]',
+                    }
     >>> fig, ax = maad.util.plot2d(Lxx,interpolation=None,**fig_kwargs)      
         
     """
 
     # matplotlib parameters
     title = kwargs.pop("title", "")
     ylabel = kwargs.pop("ylabel", "Frequency [Hz]")
@@ -1044,15 +1184,15 @@
     type : string
         'bright' for strong colors, 'soft' for pastel colors. Default is 'bright'
     first_color_black : bool, optional
         Option to use first color as black. Default is True  
     last_color_black : bool, optional   
         Option to use last color as black. Default is False
     seed : int, optional
-         Fix the seed of the random engine. Default is 321   
+        Fix the seed of the random engine. Default is 321   
     verbose  : bool, optional   
         Prints the number of labels and shows the colormap. Default is False
     
     Returns
     -------
     random_colormap : Colormap 
         Colormap type used by matplotlib
@@ -1162,29 +1302,29 @@
     
     Examples
     --------
     >>> w, fs = maad.sound.load('../data/cold_forest_daylight.wav') 
     >>> Sxx_power,tn,fn,_ = maad.sound.spectrogram(w,fs)
     >>> Lxx = maad.spl.power2dBSPL(Sxx_power, gain=42) # convert into dB SPL
     >>> fig_kwargs = {'vmax': Lxx.max(),
-                      'vmin':0,
-                      'extent':(tn[0], tn[-1], fn[0], fn[-1]),
-                      'title':'Power spectrogram density (PSD)',
-                      'xlabel':'Time [s]',
-                      'ylabel':'Frequency [Hz]',
-                      }
+                    'vmin':0,
+                    'extent':(tn[0], tn[-1], fn[0], fn[-1]),
+                    'title':'Power spectrogram density (PSD)',
+                    'xlabel':'Time [s]',
+                    'ylabel':'Frequency [Hz]',
+                    }
     >>> fig, ax = maad.util.plot2d(Lxx,**fig_kwargs)      
     >>> Lxx_crop, tn_crop, fn_crop = maad.util.crop_image(Lxx, tn, fn, fcrop=(2000,10000), tcrop=(0,30))
     >>> fig_kwargs = {'vmax': Lxx.max(),
-                      'vmin':0,
-                      'extent':(tn_crop[0], tn_crop[-1], fn_crop[0], fn_crop[-1]),
-                      'title':'Crop of the power spectrogram density (PSD)',
-                      'xlabel':'Time [s]',
-                      'ylabel':'Frequency [Hz]',
-                      }
+                    'vmin':0,
+                    'extent':(tn_crop[0], tn_crop[-1], fn_crop[0], fn_crop[-1]),
+                    'title':'Crop of the power spectrogram density (PSD)',
+                    'xlabel':'Time [s]',
+                    'ylabel':'Frequency [Hz]',
+                    }
     >>> fig, ax = maad.util.plot2d(Lxx_crop,**fig_kwargs)  
     """
 
     if tcrop is not None:
         indt = (tn >= tcrop[0]) * (tn <= tcrop[1])
         im = im[:, indt]
         # redefine tn
@@ -1196,15 +1336,15 @@
         ]
         # redefine fn
         fn = fn[np.where(indf > 0)]
 
     return im, tn, fn
 
 
-# =============================================================================
+#%%
 def save_figlist(fname, figlist):
     """
     Save a list of figures or spectrograms to disk.
     
     Parameters
     ----------
     fname: string
@@ -1216,16 +1356,15 @@
     This function does not return any variable.
         
     """
     for i, fig in enumerate(figlist):
         fname_save = "%d_%s" % (i, fname)
         imsave(fname_save, fig)
 
-
-# =============================================================================
+#%%
 def plot_features_map(df, norm=True, mode="24h", **kwargs):
     """
     Plot features values on a heatmap.
     
     The plot has the features the vertical axis and the time on the horizontal axis.
     
     Parameters
@@ -1290,15 +1429,15 @@
         
     Returns
     -------
     fig : Figure
         The Figure instance 
     ax : Axis
         The Axis instance   
-       
+    
     Examples
     --------
     see plot_extract_alpha_indices.py advanced example for a complete example
     
     >>> import numpy as np
     >>> import pandas as pd
     >>> np.random.seed(2021)
@@ -1354,17 +1493,319 @@
     plt.setp(ax.get_yticklabels(), rotation=0, ha="right", fontsize=10)
     plt.setp(ax.get_xticklabels(), rotation=90, ha="center", fontsize=10)
     fig.tight_layout()
     plt.show()
 
     return fig, ax
 
+#%%
+def heatmap_by_date_and_time (
+                    dataframe,
+                    disp_column,
+                    date_format = "%V", # see https://docs.python.org/3/library/datetime.html 
+                    date_range = [1,53],
+                    time_resolution = "30T",
+                    time_range = ["00:00", "23:59"],
+                    start_hour = "00:00",
+                    full_display = False,
+                    date_min_to_disp = 1,
+                    date_max_to_disp = 53,
+                    cb_legend = "",
+                    display = True,
+                    verbose = False,
+                    **kwargs,
+                    ) :
+    """
+    Plot a heatmap of a features by time (x-axis) and date (y-axis).
 
-# =============================================================================
+    Parameters
+    ----------
+    dataframe : pandas.DataFrame
+        The input DataFrame containing the data.
+        Must contain a column (or index) date in the format %Y-%m-%d %H:%M%S
+    disp_column : str
+        The name of the column to be displayed.
+    date_format : str, optional
+        The format of the date. The default is "%V".
+        (See https://docs.python.org/3/library/datetime.html for format codes)
+        Possible format are :
+        - "%V" for week number (from 1 to 53)
+        - "%m" for Month (from 1 to 12)
+        - "%d" for Day (from 1 to 31 depending on the month)
+        - "%m-%d" for Date without year (from 01-01 to 12-31)
+        - "%y-%m-%d" for Date with year 
+    date_range : list of int, optional
+        The range of date types to include. The default is [1, 53].
+        The format of the range depends on date_format.
+        For instance, to get all the samples in the March, date_range would be 
+        [03-01, 03-31] and date_format would be "%m-%d"
+    time_resolution : str, optional
+        The time resolution. The default is "30T".
+        T is for minute. 30T means a time resolution of 30 min. 
+        Everything within this intervale is averaged
+        Other time formats are H for hour and D for day.
+    time_range : list of str, optional
+        The time range to consider. The default is ["00:00", "23:59"].
+    start_hour : str, optional
+        The start hour. The default is "12:00".
+    full_display : bool, optional
+        Whether to display the full date range. The default is False.
+    date_min_to_disp : int, optional
+        The minimum date on the y-axis. The default is 1.
+        The value depends on the date_format. 
+        See date_format to know the possible formats and the range of possible values
+    date_max_to_disp : int, optional
+        The maximum date on the y-axis. The default is 53.
+        The value depends on the date_format. 
+        See date_format to know the possible formats and the range of possible values
+    cb_legend : str, optional
+        The colorbar legend label. The default is "".
+    verbose : bool, optional
+        If True, display verbose information. The default is False.
+    **kwargs
+        Specific to this function:
+        
+        - ftime : Time format to display as x label by default '%Y-%m-%d'(see https://docs.python.org/fr/3.6/library/datetime.html?highlight=strftime#strftime-strptime-behavior)
+            
+        Specific to matplotlib:
+            
+        - figsize : tuple of integers, optional, default: (4,10) width, height in inches.  
+        
+        - title : string, optional, default : 'Spectrogram' title of the figure
+        
+        - xlabel : string, optional, default : 'Time [s]' label of the horizontal axis
+
+        - ylabel : string, optional, default : 'Amplitude [AU]' label of the vertical axis
+            
+        - xticks : tuple of ndarrays, optional, default : none
+            * ticks : array_like => A list of positions at which ticks should be placed. You can pass an empty list to disable yticks.
+            * labels : array_like, optional =>  A list of explicit labels to place at the given locs.
+            
+        - yticks : tuple of ndarrays, optional, default : none
+            * ticks : array_like => A list of positions at which ticks should be placed. You can pass an empty list to disable yticks.
+            * labels : array_like, optional =>  A list of explicit labels to place at the given locs.
+        
+        - cmap : string or Colormap object, optional, default is 'gray'
+            See https://matplotlib.org/examples/color/colormaps_reference.html
+            in order to get all the  existing colormaps
+            examples: 'hsv', 'hot', 'bone', 'tab20c', 'jet', 'seismic', 
+            'viridis'...
+        
+        - vmin, vmax : scalar, optional, default: None
+            `vmin` and `vmax` are used in conjunction with norm to normalize
+            luminance data.  Note if you pass a `norm` instance, your
+            settings for `vmin` and `vmax` will be ignored.
+        
+        - extent : list of scalars [left, right, bottom, top], optional, default: None
+            The location, in data-coordinates, of the lower-left and
+            upper-right corners. If `None`, the image is positioned such that
+            the pixel centers fall on zero-based (row, column) indices.
+        
+        - now : boolean, optional, default : True
+            if True, display now. Cannot display multiple images. 
+            To display mutliple images, set now=False until the last call for 
+            the last image      
+            
+        ... and more, see matplotlib
 
+    Returns
+    -------
+    df_mean : pd.DataFrame
+        The heatmap with mean values.
+    
+    df_std :pd.DataFrame
+        The heatmap with standard deviation values.
+
+    fig : matplotlib.figure.Figure
+        The generated matplotlib figure.
+
+    ax : matplotlib.axes.Axes
+        The generated matplotlib axis.
+    """
+
+    # test if dataframe is not a pd.DataFrame
+    if isinstance(dataframe, pd.DataFrame) == False:
+        if verbose :
+            print("***WARNING*** dataframe must be a valid pandas dataframe")
+        return
+    
+    # copy the dataframe
+    df = dataframe.copy()
+
+    # keep some columns
+    df = df.filter([disp_column,'date'])
+
+    try :
+        if not('date' in df)  :  
+            df = df.reset_index(['date'])
+        # convert date to datetime
+        df['date'] = pd.to_datetime(df['date'])
+        # set the index to date
+        df.set_index(['date'], inplace=True)
+        # convert index to datetime 
+        df.index = pd.DatetimeIndex(df.index)
+        # sort dataframe by date
+        df = df.sort_index(axis=0)
+    except :
+        raise Exception("***WARNING*** df must have a valid date index that could be converted in Datetime type")
+
+    # filter by time
+    df = _filter_dataframe_by_datetime(df, "%H:%M", time_range)
+    # filter by date_type
+    df = _filter_dataframe_by_datetime(df, date_format, date_range)
+
+    # # Extract hour and minute
+    df['time'] = df.index.strftime("%H:%M")
+
+    # # Extract week, year, weekday or date
+    df['date_type'] = df.index.strftime(date_format) 
+
+    # create a matrix with date_type (week, year, weekday, date) as columns and time (hour) as rows
+    df_mean = df.groupby(['time', 'date_type'])[disp_column].aggregate('mean').unstack()
+
+    # Resample the timeline. Need to reformat the time in datetime before resampling
+    df_mean = df_mean.reset_index()
+    df_mean.index = pd.to_datetime(df_mean['time'], format='%H:%M')
+    df_mean.drop(columns=['time'], inplace = True)
+    df_mean = df_mean.resample(time_resolution).mean()
+    df_std = df_mean.resample(time_resolution).std()
+    df_mean.index = df_mean.index.strftime("%H:%M")
+    df_std.index = df_std.index.strftime("%H:%M")
+
+    if display == True : 
+
+        # try to use seaborn if installed
+        try:
+            import seaborn as sns
+            sns.set_theme("paper")
+        except ImportError as e:
+            if verbose :
+                print("seaborn is not installed, use default settings")
+
+        if full_display == True :
+            # Create a list of unique index of type 'hour' for x axis
+            time_min = datetime.strptime("00:00", "%H:%M")
+            time_max = datetime.strptime("23:59", "%H:%M")
+            x_label = pd.date_range(time_min, time_max, freq=time_resolution).strftime("%H:%M")
+            x_label = x_label.values
+            # Create a vector for y axis depending on date_format
+            if date_format == "%V" :
+                y_label = [f'{x:02d}' for x in np.arange(date_min_to_disp,date_max_to_disp+1)]
+            elif date_format == "%m" :
+                y_label = [f'{x:02d}' for x in np.arange(date_min_to_disp,date_max_to_disp+1)]   
+            elif (date_format == "%y-%m-%d") or (date_format == "%m-%d") or (date_format == "%d"):
+                date_min_to_disp = datetime.strptime(str(date_min_to_disp), date_format)
+                date_max_to_disp = datetime.strptime(str(date_max_to_disp), date_format)
+                y_label = pd.date_range(date_min_to_disp, date_max_to_disp, freq='D').strftime(date_format)
+                y_label = y_label.values
+            else:
+                # by default per week
+                y_label = [f'{x:02d}' for x in np.arange(1,53)]
+            # create an prefilled dataframe with all weeks and time
+            df2 = pd.DataFrame(index=x_label, 
+                            columns=y_label,
+                            dtype = 'float')
+            df2.reset_index(inplace=True)
+            df2 = df2.rename(columns={"index":"time"})
+            df2.set_index("time", inplace=True)
+
+            for idx, row in df_mean.iterrows() :
+                df2.loc[idx] = row
+            
+            df_mean=df2
+        
+        # rename the unique column with the corresponding name
+        if date_format == "%V" : df_mean.columns.name='Week number'
+        if date_format == "%m" : df_mean.columns.name='Month'
+        if date_format == "%d" : df_mean.columns.name='Day'
+        if date_format == "%m-%d" : df_mean.columns.name='Date'
+        if date_format == "%y-%m-%d" : df_mean.columns.name='Date'
+
+        # shift the time to start at start_hour and finish at start_hour, in order to center
+        # the graph at start_hour + 12h
+        df_part1 = df_mean[df_mean.index >= start_hour]
+        df_part2 = df_mean[df_mean.index < start_hour]
+        df_part2.sort_index(inplace=True)
+        df = pd.concat([df_part1,df_part2])  
+        
+        # Get the list of unique index of type 'hour'
+        x_label = [i + j for i, j in zip(map(str, df.index.values), [" "] * len(df))]
+
+        # plot
+        # matplotlib parameters
+        fig = kwargs.pop("fig", None)
+        ax = kwargs.pop("ax", None) 
+        xlabel = kwargs.pop("xlabel", "Hours")
+        ylabel = kwargs.pop("ylabel", df_mean.columns.name)
+        now = kwargs.pop("now", True)
+        vmin = kwargs.pop("vmin", np.nanpercentile(df,1))
+        vmax = kwargs.pop("vmax", np.nanpercentile(df,99))
+        cmap = kwargs.pop("cmap", "RdPu")
+        title = kwargs.pop("title", None)
+        figsize = kwargs.pop("figsize", (len(df)*0.33*0.75, len(list(df))*0.26*0.75 +0.75))
+        
+        # Create a figure and a subplot associated
+        if (fig is None) or (ax is None) :
+            fig = plt.figure(figsize=figsize)
+            ax = fig.add_subplot(111)
+
+        # display image
+        caxes = ax.matshow(df.transpose(), 
+                        interpolation = "None",
+                        aspect="auto", 
+                        cmap = cmap,
+                        vmin = vmin,
+                        vmax = vmax,
+                        **kwargs
+                        )
+        if cb_legend =="" :
+            fig.colorbar(caxes, shrink=0.75, label=disp_column)
+        else:
+            fig.colorbar(caxes, shrink=0.75, label=cb_legend)
+        # Set ticks on both sides of axes on
+        ax.tick_params(which='major', axis="x", bottom=False, top=False, 
+                    labelbottom=True, labeltop=False)
+        ax.tick_params(which='minor', axis="x", length = 0)
+        # We want to show all ticks...
+        ax.set_yticks(np.arange(len(df.columns)))
+        ax.set_xticks(np.arange(len(x_label)))
+        # ... and label them with the respective list entries
+        ax.set_yticklabels(df.columns)
+        ax.set_xticklabels(x_label)
+        
+        # Minor ticks
+        ax.set_xticks(np.arange(-0.5, len(df.index), 1), minor=True)
+        ax.set_yticks(np.arange(-0.5, len(list(df)), 1), minor=True)
+
+        # Gridlines based on minor ticks
+        ax.grid(which='major', color='w', linestyle='-', linewidth=0)
+        ax.grid(which='minor', color='w', linestyle='-', linewidth=1)
+        
+        # add title to the axis
+        ax.set_xlabel(xlabel)
+        ax.set_ylabel(ylabel)
+                
+        # Rotate the tick labels and set their alignment.
+        plt.setp(ax.get_yticklabels(), rotation=0, ha="right", fontsize=10)
+        plt.setp(ax.get_xticklabels(), rotation=90, ha="center", fontsize=10)
+        plt.tight_layout()
+
+        # Adding a title to the figure
+        if title is not None:
+            fig.suptitle(title)
+
+        if now :
+            plt.show()
+    else :
+        fig = None
+        ax = None
+
+    return df_mean, df_std, fig, ax
+
+# =============================================================================
 
 def plot_features(df, ax=None, norm=True, mode="24h", **kwargs):
     """
     Plot the variation of features values (ie. indices) in the DataFrame obtained 
     with ``maad.features``.
             
     Parameters
@@ -1449,14 +1890,15 @@
     list_markers = tuple(list(Line2D.markers.keys())[0:-4])
     markers = itertools.cycle(list_markers)
     prop_cycle = plt.rcParams["axes.prop_cycle"]
     colors = itertools.cycle(prop_cycle.by_key()["color"])
 
     figsize = kwargs.pop("figsize", (5, 5))
     kwargs.pop("label", None)
+    now = kwargs.pop("now", True)
 
     # if no ax, create a figure and a subplot associated a figure otherwise
     # find the figure that belongs to ax
     if ax is None:
         fig, ax = plt.subplots(**kwargs)
         fig.set_size_inches(figsize)
     else:
@@ -1474,15 +1916,18 @@
         )
 
     if mode == "24h":
         ax.set_xlabel("Day time (Hour)")
     ax.grid()
     ax.legend()
     fig.tight_layout()
-    # plt.show()
+
+    # Display the figure now
+    if now:
+        plt.show()
 
     return fig, ax
 
 
 # =============================================================================
 def plot_correlation_map(df, R_threshold=0.75, method="spearman", **kwargs):
     """
```

### Comparing `scikit_maad-1.4.1/maad/util/xeno_canto.py` & `scikit_maad-1.4.2/maad/util/xeno_canto.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
             if verbose:
                 print("Keeped metadata for", len(df_dataset), "files after formating date")
         
         if (format_time == True) and (format_date == True) :         
             # add a column with the week number
             df_dataset['week'] = pd.to_datetime(df_dataset['date']).dt.isocalendar()['week'] # type: ignore
             # add a column with datetime in DateTime format
-            df_dataset['datetime'] =  pd.to_datetime(df_dataset['time']+' '+ df_dataset['date'])
+            df_dataset['datetime'] =  pd.to_datetime(df_dataset['time']+' '+ df_dataset['date'], format="%H:%M %Y-%m-%d")
 
     # if no limit in the number of files
     if max_nb_files is not None :
         # test if the number of files is greater than the maximum number of
         # resquested files
         if len(df_dataset) > max_nb_files : 
             df_dataset = df_dataset.sample(n = max_nb_files,
```

### Comparing `scikit_maad-1.4.1/pyproject.toml` & `scikit_maad-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_maad-1.4.1/PKG-INFO` & `scikit_maad-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-maad
-Version: 1.4.1
+Version: 1.4.2
 Summary: Open-source and modular toolbox for quantitative soundscape analysis in Python
 Keywords: ecoacoustics,bioacoustics,ecology,sound pressure level,signal processing
 Author-email: scikit-maad developers <scikit.maad@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

