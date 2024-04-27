# Comparing `tmp/nendo_plugin_loopify-0.1.6.tar.gz` & `tmp/nendo_plugin_loopify-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nendo_plugin_loopify-0.1.6.tar", max compression
+gzip compressed data, was "nendo_plugin_loopify-0.1.7.tar", max compression
```

## Comparing `nendo_plugin_loopify-0.1.6.tar` & `nendo_plugin_loopify-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-12-29 19:31:35.314045 nendo_plugin_loopify-0.1.6/LICENSE
--rw-r--r--   0        0        0     2227 2024-01-28 19:49:00.951699 nendo_plugin_loopify-0.1.6/README.md
--rw-r--r--   0        0        0     3518 2024-02-21 09:13:35.785849 nendo_plugin_loopify-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      146 2024-02-21 09:13:39.122849 nendo_plugin_loopify-0.1.6/src/nendo_plugin_loopify/__init__.py
--rw-r--r--   0        0        0     7065 2023-12-29 19:31:35.319045 nendo_plugin_loopify-0.1.6/src/nendo_plugin_loopify/beatnet.py
--rw-r--r--   0        0        0  1612179 2023-12-29 19:31:35.356045 nendo_plugin_loopify-0.1.6/src/nendo_plugin_loopify/models/model.pt
--rw-r--r--   0        0        0     4060 2023-12-29 19:31:35.357045 nendo_plugin_loopify-0.1.6/src/nendo_plugin_loopify/plugin.py
--rw-r--r--   0        0        0     4147 2024-01-31 20:16:29.404526 nendo_plugin_loopify-0.1.6/src/nendo_plugin_loopify/utils.py
--rw-r--r--   0        0        0     3306 1970-01-01 00:00:00.000000 nendo_plugin_loopify-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-12-29 19:31:35.314045 nendo_plugin_loopify-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2227 2024-01-28 19:49:00.951699 nendo_plugin_loopify-0.1.7/README.md
+-rw-r--r--   0        0        0     3518 2024-04-27 12:31:08.498785 nendo_plugin_loopify-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      146 2024-04-27 12:31:09.404785 nendo_plugin_loopify-0.1.7/src/nendo_plugin_loopify/__init__.py
+-rw-r--r--   0        0        0     7065 2023-12-29 19:31:35.319045 nendo_plugin_loopify-0.1.7/src/nendo_plugin_loopify/beatnet.py
+-rw-r--r--   0        0        0  1612179 2023-12-29 19:31:35.356045 nendo_plugin_loopify-0.1.7/src/nendo_plugin_loopify/models/model.pt
+-rw-r--r--   0        0        0     4355 2024-04-27 12:30:08.641789 nendo_plugin_loopify-0.1.7/src/nendo_plugin_loopify/plugin.py
+-rw-r--r--   0        0        0     6916 2024-04-27 12:21:46.098824 nendo_plugin_loopify-0.1.7/src/nendo_plugin_loopify/utils.py
+-rw-r--r--   0        0        0     3306 1970-01-01 00:00:00.000000 nendo_plugin_loopify-0.1.7/PKG-INFO
```

### Comparing `nendo_plugin_loopify-0.1.6/LICENSE` & `nendo_plugin_loopify-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nendo_plugin_loopify-0.1.6/README.md` & `nendo_plugin_loopify-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nendo_plugin_loopify-0.1.6/pyproject.toml` & `nendo_plugin_loopify-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nendo-plugin-loopify"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
     "Aaron Abebe <aaron@okio.ai>"
 ]
 description = "Nendo plugin for automatic audio loop extraction."
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/okio-ai/nendo_plugin_loopify"
```

### Comparing `nendo_plugin_loopify-0.1.6/src/nendo_plugin_loopify/beatnet.py` & `nendo_plugin_loopify-0.1.7/src/nendo_plugin_loopify/beatnet.py`

 * *Files identical despite different names*

### Comparing `nendo_plugin_loopify-0.1.6/src/nendo_plugin_loopify/models/model.pt` & `nendo_plugin_loopify-0.1.7/src/nendo_plugin_loopify/models/model.pt`

 * *Files identical despite different names*

### Comparing `nendo_plugin_loopify-0.1.6/src/nendo_plugin_loopify/plugin.py` & `nendo_plugin_loopify-0.1.7/src/nendo_plugin_loopify/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Nendo,
     NendoConfig,
     NendoGeneratePlugin,
     NendoTrack,
 )
 
 from .beatnet import NendoBeatNet
-from .utils import choose_final_loops, get_loop_candidates
+from .utils import choose_final_loops, get_loop_candidates, QualityScore
 
 
 class Loopifier(NendoGeneratePlugin):
     """A plugin for Nendo that provides music loop generation capabilities.
 
     Attributes:
         nendo_instance (Nendo): The instance of Nendo using this plugin.
@@ -50,21 +50,25 @@
 
     @NendoGeneratePlugin.run_track
     def loopify_track(
         self,
         track: NendoTrack,
         n_loops: Optional[int] = 4,
         beats_per_loop: Optional[int] = 8,
+        loop_score: QualityScore = QualityScore.SPECTRAL_DISTANCE,
     ) -> List[NendoTrack]:
         """Run the BeatNet loopifier on the given track.
 
         Args:
             track (NendoTrack): The track to loopify.
             n_loops (int, optional): The number of loops to generate.
             beats_per_loop (int, optional): The number of beats per loop.
+            loop_score (QualityScore): The quality score used when selecting the loops.
+                Defaults to the combination of normalized spectral similarity
+                and distance score.
 
         Returns:
             List[NendoTrack]: The generated loops.
         """
         loops: List[NendoTrack] = []
 
         y, sr = track.signal, track.sr
@@ -88,15 +92,15 @@
         if len(loop_candidates) == 0:
             self.logger.warning(
                 "No loops found in track. Try to reduce the number of beats per loop."
             )
 
         self.logger.debug(f"Found {len(loop_candidates)} loop candidates.")
 
-        final_loops = choose_final_loops(loop_candidates, n_loops)
+        final_loops = choose_final_loops(loop_candidates, n_loops, loop_score)
         self.logger.debug(f"Found final loops:\n{final_loops}")
 
         for i, loop in enumerate(final_loops):
             loop_buffer = (
                 y[:, loop.start_sample : loop.end_sample]
                 if len(y.shape) > 1
                 else y[loop.start_sample : loop.end_sample]
```

### Comparing `nendo_plugin_loopify-0.1.6/PKG-INFO` & `nendo_plugin_loopify-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nendo-plugin-loopify
-Version: 0.1.6
+Version: 0.1.7
 Summary: Nendo plugin for automatic audio loop extraction.
 Home-page: https://okio.ai
 License: MIT
 Keywords: Nendo,Plugin,Loopification,Music loop generation,AI,Machine Learning,Audio,Generative,Music,Audio Production,Audio Generation,Audio Analysis
 Author: Aaron Abebe
 Author-email: aaron@okio.ai
 Requires-Python: >=3.8,<3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nendo-plugin-loopify Version: 0.1.6 Summary: Nendo
+Metadata-Version: 2.1 Name: nendo-plugin-loopify Version: 0.1.7 Summary: Nendo
 plugin for automatic audio loop extraction. Home-page: https://okio.ai License:
 MIT Keywords: Nendo,Plugin,Loopification,Music loop generation,AI,Machine
 Learning,Audio,Generative,Music,Audio Production,Audio Generation,Audio
 Analysis Author: Aaron Abebe Author-email: aaron@okio.ai Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
```

