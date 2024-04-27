# Comparing `tmp/spectrum_io-0.4.2.tar.gz` & `tmp/spectrum_io-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_io-0.4.2.tar", max compression
+gzip compressed data, was "spectrum_io-0.4.3.tar", max compression
```

## Comparing `spectrum_io-0.4.2.tar` & `spectrum_io-0.4.3.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1102 2024-01-29 13:45:39.847184 spectrum_io-0.4.2/LICENSE
--rw-r--r--   0        0        0     2409 2024-01-29 13:45:39.847184 spectrum_io-0.4.2/README.rst
--rw-r--r--   0        0        0     2388 2024-01-29 13:45:39.847184 spectrum_io-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1051 2024-01-29 13:45:39.847184 spectrum_io-0.4.2/spectrum_io/__init__.py
--rw-r--r--   0        0        0      351 2024-01-29 13:45:39.847184 spectrum_io-0.4.2/spectrum_io/__main__.py
--rw-r--r--   0        0        0      133 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/d/__init__.py
--rw-r--r--   0        0        0     6759 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/d/bruker.py
--rw-r--r--   0        0        0     5690 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/d/masterPeak.py
--rw-r--r--   0        0        0    13238 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/d/masterSpectrum.py
--rw-r--r--   0        0        0     1919 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/d/peak.py
--rw-r--r--   0        0        0      104 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/file/__init__.py
--rw-r--r--   0        0        0      556 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/file/csv.py
--rw-r--r--   0        0        0     5912 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/file/hdf5.py
--rw-r--r--   0        0        0        0 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/py.typed
--rw-r--r--   0        0        0      105 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/raw/__init__.py
--rw-r--r--   0        0        0    13364 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/raw/msraw.py
--rw-r--r--   0        0        0     3897 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/raw/thermo_raw.py
--rw-r--r--   0        0        0      146 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/search_result/__init__.py
--rw-r--r--   0        0        0     4333 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/search_result/mascot.py
--rw-r--r--   0        0        0     6178 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/search_result/maxquant.py
--rw-r--r--   0        0        0     4143 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/search_result/msamanda.py
--rw-r--r--   0        0        0     2937 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/search_result/msfragger.py
--rw-r--r--   0        0        0     2626 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/search_result/sage.py
--rw-r--r--   0        0        0     2735 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/search_result/search_results.py
--rw-r--r--   0        0        0      238 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/spectral_library/__init__.py
--rw-r--r--   0        0        0    21794 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/spectral_library/digest.py
--rw-r--r--   0        0        0    45056 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/spectral_library/dlib/myPrositLib.dlib
--rw-r--r--   0        0        0     7590 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/spectral_library/dlib.py
--rw-r--r--   0        0        0    98385 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/spectral_library/msp/myPrositLib.msp
--rw-r--r--   0        0        0     2112 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/spectral_library/msp.py
--rw-r--r--   0        0        0     3784 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/spectral_library/spectral_library.py
--rw-r--r--   0        0        0   565091 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/spectral_library/spectronaut/myPrositLib.csv
--rw-r--r--   0        0        0     2493 2024-01-29 13:45:39.851184 spectrum_io-0.4.2/spectrum_io/spectral_library/spectronaut.py
--rw-r--r--   0        0        0     3601 1970-01-01 00:00:00.000000 spectrum_io-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-27 15:10:51.928840 spectrum_io-0.4.3/LICENSE
+-rw-r--r--   0        0        0     2409 2024-04-27 15:10:51.928840 spectrum_io-0.4.3/README.rst
+-rw-r--r--   0        0        0     2370 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1051 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/__init__.py
+-rw-r--r--   0        0        0      351 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/__main__.py
+-rw-r--r--   0        0        0      133 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/d/__init__.py
+-rw-r--r--   0        0        0     6872 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/d/bruker.py
+-rw-r--r--   0        0        0     5690 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/d/masterPeak.py
+-rw-r--r--   0        0        0    13238 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/d/masterSpectrum.py
+-rw-r--r--   0        0        0     1919 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/d/peak.py
+-rw-r--r--   0        0        0      104 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/file/__init__.py
+-rw-r--r--   0        0        0      556 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/file/csv.py
+-rw-r--r--   0        0        0     5912 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/file/hdf5.py
+-rw-r--r--   0        0        0        0 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/py.typed
+-rw-r--r--   0        0        0      105 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/raw/__init__.py
+-rw-r--r--   0        0        0    13364 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/raw/msraw.py
+-rw-r--r--   0        0        0     3897 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/raw/thermo_raw.py
+-rw-r--r--   0        0        0      177 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/search_result/__init__.py
+-rw-r--r--   0        0        0     4333 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/search_result/mascot.py
+-rw-r--r--   0        0        0     6178 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/search_result/maxquant.py
+-rw-r--r--   0        0        0     4143 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/search_result/msamanda.py
+-rw-r--r--   0        0        0     2937 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/search_result/msfragger.py
+-rw-r--r--   0        0        0     2542 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/search_result/sage.py
+-rw-r--r--   0        0        0     2791 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/search_result/search_results.py
+-rw-r--r--   0        0        0     5547 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/search_result/xisearch.py
+-rw-r--r--   0        0        0      238 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/spectral_library/__init__.py
+-rw-r--r--   0        0        0    21794 2024-04-27 15:10:51.936841 spectrum_io-0.4.3/spectrum_io/spectral_library/digest.py
+-rw-r--r--   0        0        0    45056 2024-04-27 15:10:51.936841 spectrum_io-0.4.3/spectrum_io/spectral_library/dlib/myPrositLib.dlib
+-rw-r--r--   0        0        0     8539 2024-04-27 15:10:51.936841 spectrum_io-0.4.3/spectrum_io/spectral_library/dlib.py
+-rw-r--r--   0        0        0    98385 2024-04-27 15:10:51.936841 spectrum_io-0.4.3/spectrum_io/spectral_library/msp/myPrositLib.msp
+-rw-r--r--   0        0        0     2319 2024-04-27 15:10:51.936841 spectrum_io-0.4.3/spectrum_io/spectral_library/msp.py
+-rw-r--r--   0        0        0     3799 2024-04-27 15:10:51.936841 spectrum_io-0.4.3/spectrum_io/spectral_library/spectral_library.py
+-rw-r--r--   0        0        0   565091 2024-04-27 15:10:51.936841 spectrum_io-0.4.3/spectrum_io/spectral_library/spectronaut/myPrositLib.csv
+-rw-r--r--   0        0        0     2833 2024-04-27 15:10:51.936841 spectrum_io-0.4.3/spectrum_io/spectral_library/spectronaut.py
+-rw-r--r--   0        0        0     3562 1970-01-01 00:00:00.000000 spectrum_io-0.4.3/PKG-INFO
```

### Comparing `spectrum_io-0.4.2/LICENSE` & `spectrum_io-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.2/README.rst` & `spectrum_io-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.2/pyproject.toml` & `spectrum_io-0.4.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectrum_io"
-version = "0.4.2"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.4.3"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "IO related functionalities for oktoberfest."
 authors = ["Wilhelmlab at Technical University of Munich"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/wilhelm-lab/spectrum_io"
 repository = "https://github.com/wilhelm-lab/spectrum_io"
 documentation = "https://spectrum_io.readthedocs.io"
@@ -25,16 +25,15 @@
 PyYAML = ">=5.4.1"
 numpy = "^1.18.1"
 pandas = "^1.3.0"
 h5py = "^3.1.0"
 pymzml = "^2.5.0"
 pyteomics = "^4.3.3"
 lxml= '^4.5.2'
-tables = "^3.6.1"
-spectrum-fundamentals = ">=0.5.0,<0.6.0"
+spectrum-fundamentals = ">=0.5.2,<0.6.0"
 alphatims = "^1.0.8"
 sortedcontainers = "^2.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.2.3"
 coverage = {extras = ["toml"], version = ">=5.3"}
 safety = ">=1.9.0"
```

### Comparing `spectrum_io-0.4.2/spectrum_io/__init__.py` & `spectrum_io-0.4.3/spectrum_io/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for spectrum_io."""
 
 __author__ = "Mario Picciani"
 __email__ = "mario.picciani@tum.de"
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 
 import logging
 import logging.handlers
 import sys
 import time
 
 from . import d, file, raw
```

### Comparing `spectrum_io-0.4.2/spectrum_io/d/bruker.py` & `spectrum_io-0.4.3/spectrum_io/d/bruker.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,17 @@
         mz_values=True,
         intensity_values=True,
         corrected_intensity_values=False,
         raw_indices_sorted=False,
     )
     df.columns = ["FRAME", "SCAN", "PRECURSOR", "RETENTION_TIME", "INV_ION_MOBILITY", "MZ", "INTENSITIES"]
 
+    # converting RETENTION TIME from seconds to minutes
+    df["RETENTION_TIME"] = df["RETENTION_TIME"].div(60)
+
     # aggregation
     df_combined_grouped = (
         df.merge(
             scan_to_precursor_map[
                 ["SCAN_NUM_BEGIN", "SCAN_NUM_END", "PRECURSOR", "FRAME", "COLLISION_ENERGY"]
             ].drop_duplicates()
         )
```

### Comparing `spectrum_io-0.4.2/spectrum_io/d/masterPeak.py` & `spectrum_io-0.4.3/spectrum_io/d/masterPeak.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.2/spectrum_io/d/masterSpectrum.py` & `spectrum_io-0.4.3/spectrum_io/d/masterSpectrum.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.2/spectrum_io/d/peak.py` & `spectrum_io-0.4.3/spectrum_io/d/peak.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.2/spectrum_io/file/csv.py` & `spectrum_io-0.4.3/spectrum_io/file/csv.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.2/spectrum_io/file/hdf5.py` & `spectrum_io-0.4.3/spectrum_io/file/hdf5.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.2/spectrum_io/raw/msraw.py` & `spectrum_io-0.4.3/spectrum_io/raw/msraw.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.2/spectrum_io/raw/thermo_raw.py` & `spectrum_io-0.4.3/spectrum_io/raw/thermo_raw.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.2/spectrum_io/search_result/mascot.py` & `spectrum_io-0.4.3/spectrum_io/search_result/mascot.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.2/spectrum_io/search_result/maxquant.py` & `spectrum_io-0.4.3/spectrum_io/search_result/maxquant.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.2/spectrum_io/search_result/msamanda.py` & `spectrum_io-0.4.3/spectrum_io/search_result/msamanda.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.2/spectrum_io/search_result/msfragger.py` & `spectrum_io-0.4.3/spectrum_io/search_result/msfragger.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.2/spectrum_io/search_result/sage.py` & `spectrum_io-0.4.3/spectrum_io/search_result/sage.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,21 +17,21 @@
     def read_result(self, tmt_labeled: str = "") -> pd.DataFrame:
         """
         Function to read a msms tsv and perform some basic formatting.
 
         :param tmt_labeled: tmt label as str
         :return: pd.DataFrame with the formatted data
         """
-        logger.info("Reading msms.tsv file")
+        logger.info(f"Reading {self.path}")
         df = pd.read_csv(
             self.path,
-            usecols=["filename", "scannr", "peptide", "charge", "hyperscore", "calcmass", "proteins"],
+            usecols=["filename", "scannr", "peptide", "charge", "hyperscore", "calcmass", "label", "proteins"],
             sep="\t",
         )
-        logger.info("Finished reading msms.tsv file")
+        logger.info(f"Finished reading {self.path}")
 
         # Standardize column names
         df.columns = df.columns.str.upper()
         df.columns = df.columns.str.replace(" ", "_")
 
         df = Sage.update_columns_for_prosit(df, tmt_labeled)
         return filter_valid_prosit_sequences(df)
@@ -47,30 +47,27 @@
         """
         df = df.rename(
             columns={
                 "FILENAME": "RAW_FILE",
                 "SCANNR": "SCAN_NUMBER",
                 "PEPTIDE": "MODIFIED_SEQUENCE",
                 "CHARGE": "PRECURSOR_CHARGE",
+                "CALCMASS": "MASS",
+                "HYPERSCORE": "SCORE",
+                "LABEL": "REVERSE",
             }
         )
 
         # removing .mzML
         df["RAW_FILE"] = df["RAW_FILE"].str.replace(".mzML", "", regex=True)
         # extracting only the scan number
         df["SCAN_NUMBER"] = [int(x.rsplit("=", 1)[-1]) for x in df["SCAN_NUMBER"]]
         # creating a column of decoys and targets
-        df["REVERSE"] = df["PROTEINS"].str.startswith("rev_")
+        df["REVERSE"] = df["REVERSE"] < 0
         # removing modification to create the unmodified sequences
-        df["SEQUENCE"] = df["MODIFIED_SEQUENCE"].str.replace(r"\[.*?\]", "", regex=True)
+        df["SEQUENCE"] = df["MODIFIED_SEQUENCE"].str.replace(r"\-|\[.*?\]", "", regex=True)
         # length of the peptide
         df["PEPTIDE_LENGTH"] = df["SEQUENCE"].str.len()
-        # mass of the peptide
-        df["MASS"] = df["CALCMASS"]
-        # score of the peptide
-        df["SCORE"] = df["HYPERSCORE"]
-        # converting proforma to unimode
-        print(df)
+        # converting sage to unimod
         df["MODIFIED_SEQUENCE"] = sage_to_internal(df["MODIFIED_SEQUENCE"])
 
-        print(df.columns)
         return df
```

### Comparing `spectrum_io-0.4.2/spectrum_io/search_result/search_results.py` & `spectrum_io-0.4.3/spectrum_io/search_result/search_results.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,19 @@
         """
         if isinstance(path, str):
             path = Path(path)
         self.path = path
 
     @abstractmethod
     def read_result(self, tmt_labeled: str):
-        """Read result."""
+        """Read result.
+
+        :param tmt_labeled: tmt label as str
+
+        """
         raise NotImplementedError
 
     def generate_internal(self, tmt_labeled: str, out_path: Optional[Union[str, Path]] = None) -> pd.DataFrame:
         """
         Generate df and save to out_path if provided.
 
         :param out_path: path to output
```

### Comparing `spectrum_io-0.4.2/spectrum_io/spectral_library/digest.py` & `spectrum_io-0.4.3/spectrum_io/spectral_library/digest.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.2/spectrum_io/spectral_library/dlib/myPrositLib.dlib` & `spectrum_io-0.4.3/spectrum_io/spectral_library/dlib/myPrositLib.dlib`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.2/spectrum_io/spectral_library/dlib.py` & `spectrum_io-0.4.3/spectrum_io/spectral_library/dlib.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sqlite3
 import zlib
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import IO, Dict, Union
 
 import numpy as np
 import pandas as pd
 from spectrum_fundamentals.constants import PARTICLE_MASSES
 from spectrum_fundamentals.mod_string import internal_to_mod_mass, internal_without_mods
 
 from .spectral_library import SpectralLibrary
@@ -22,15 +22,24 @@
     "PrecursorMz",
 ]
 
 
 class DLib(SpectralLibrary):
     """Main to init a DLib obj."""
 
-    def _calculate_masked_values(self, fragmentmz: List[np.ndarray], intensities: List[np.ndarray]):
+    def _initialize(self, out: Union[IO, sqlite3.Connection]):
+        if isinstance(out, IO):
+            raise TypeError("Not supported. Use msp/spectronaut if you want to write a text file.")
+        if self.mode == "w":
+            DLib._create_database(out)
+
+    def _get_handle(self):
+        return sqlite3.connect(self.out_path)
+
+    def _calculate_masked_values(self, fragmentmz: np.ndarray, intensities: np.ndarray):
         """
         Internal function that masks, filters, byte encodes, swaps and compresses fragmentmz \
         and intensities.
 
         This will produce the data for the following columns in this order:
             - 'MassArray'
             - 'IntensityArray',
@@ -40,144 +49,153 @@
         :param intensities: intensities provided in __init__
         :return: 4 lists as described above
         """
         mz_bytes_list = []
         i_bytes_list = []
         mz_lengths = []
         i_lengths = []
-        for mz, i in zip(fragmentmz, intensities):
+
+        full_mask = self._fragment_filter_passed(fragmentmz, intensities)
+        for mz, i, mask in zip(fragmentmz, intensities, np.array(full_mask)):
             # mask to only existing peaks
-            mask = i >= self.min_intensity_threshold
             sort_index = np.argsort(mz[mask])
             masked_mz_ordered = mz[mask][sort_index]
             masked_i_ordered = i[mask][sort_index]
 
             # convert arrays to big-endian byte blops
             masked_mz_ordered = np.array(masked_mz_ordered, dtype=np.double)
             masked_i_ordered = np.array(masked_i_ordered * 100, dtype=np.float32)
             masked_mz_ordered.byteswap(inplace=True)
             masked_i_ordered.byteswap(inplace=True)
             bytes_mz = bytes(masked_mz_ordered)
             bytes_i = bytes(masked_i_ordered)
             mz_bytes_list.append(zlib.compress(bytes_mz))
-            i_bytes_list.append(zlib.compress(bytes(bytes_i)))
+            i_bytes_list.append(zlib.compress(bytes_i))
             mz_lengths.append(len(bytes_mz))
             i_lengths.append(len(bytes_i))
         return mz_bytes_list, i_bytes_list, mz_lengths, i_lengths
 
     @staticmethod
-    def create_database(path: Union[str, Path]):
+    def _create_database(conn: sqlite3.Connection):
         """
         Creates the database file with prefab tables entries, peptidetoprotein (p2p) and metadata, according to the \
         dlib specification.
 
-        :param path: specifies the path of the created database file
+        :param conn: specifies the path of the created database file
         """
         sql_create_entries = """
-            CREATE TABLE entries
-            (   PrecursorMz double not null,
-                PrecursorCharge int not null,
-                PeptideModSeq string not null,
-                PeptideSeq string not null,
-                Copies int not null,
-                RTInSeconds double not null,
-                Score double not null,
-                MassEncodedLength int not null,
-                MassArray blob not null,
-                IntensityEncodedLength int not null,
-                IntensityArray blob not null,
-                CorrelationEncodedLength int,
-                CorrelationArray blob,
-                RTInSecondsStart double,
-                RTInSecondsStop double,
-                MedianChromatogramEncodedLength int,
-                MedianChromatogramArray blob,
-                SourceFile string not null
+            CREATE TABLE IF NOT EXISTS entries
+            (
+                PrecursorMz REAL NOT NULL,
+                PrecursorCharge INTEGER NOT NULL,
+                PeptideModSeq TEXT NOT NULL,
+                PeptideSeq TEXT NOT NULL,
+                Copies INTEGER NOT NULL DEFAULT 1,
+                RTInSeconds REAL NUT NULL,
+                Score REAL NOT NULL DEFAULT 0,
+                MassEncodedLength INTEGER NOT NULL,
+                MassArray BLOB NOT NULL,
+                IntensityEncodedLength INTEGER NOT NULL,
+                IntensityArray BLOB NOT NULL,
+                CorrelationEncodedLength INTEGER,
+                CorrelationArray BLOB,
+                RTInSecondsStart REAL,
+                RTInSecondsStop REAL,
+                MedianChromatogramEncodedLength INTEGER,
+                MedianChromatogramArray BLOB,
+                SourceFile TEXT NOT NULL DEFAULT 'Oktoberfest'
             )
         """
         sql_create_p2p = """
-            CREATE TABLE peptidetoprotein
-            (PeptideSeq string not null, isDecoy boolean, ProteinAccession string not null)
+            CREATE TABLE IF NOT EXISTS peptidetoprotein
+            (
+                PeptideSeq TEXT NOT NULL,
+                isDecoy BOOL DEFAULT FALSE,
+                ProteinAccession TEXT NOT NULL DEFAULT 'UNKNOWN'
+            )
         """
         sql_create_meta = """
-            CREATE TABLE metadata (Key string not null, Value string not null)
+            CREATE TABLE IF NOT EXISTS metadata (Key string not null, Value string not null)
         """
         sql_insert_meta = "INSERT INTO metadata VALUES (?,?)"
-        conn = sqlite3.connect(path)
         c = conn.cursor()
         c.execute(sql_create_entries)
         c.execute(sql_create_p2p)
         c.execute(sql_create_meta)
         c.execute(sql_insert_meta, ["version", "0.1.14"])
         c.execute(sql_insert_meta, ["staleProteinMapping", "true"])
         conn.commit()
 
-    def write(self):
-        """Writes the entries ad p2p table to file."""
-        self._write_entries(index=False, if_exists="append", method="multi", chunksize=self.chunksize)
-        self._write_p2p(index=False, if_exists="append", method="multi", chunksize=self.chunksize)
-
-    def _write_entries(self, *args, **kwargs):
-        """
-        Internal function to write the entries table.
-
-        :param args: forwarded to pandas.to_sql
-        :param kwargs: forwarded to pandas.to_sql
-        """
-        conn = sqlite3.connect(self.out_path)
-        self.entries.to_sql(name="entries", con=conn, *args, **kwargs)
-        conn.commit()
+    def _write(self, out: Union[IO, sqlite3.Connection], data: Dict[str, np.ndarray], metadata: pd.DataFrame):
+        if isinstance(out, IO):
+            raise TypeError("Not supported. Use msp/spectronaut if you want to write a text file.")
+        seqs = metadata["SEQUENCE"]
+        modseqs = metadata["MODIFIED_SEQUENCE"]
+        mass_mod_sequences = internal_to_mod_mass(modseqs)
+
+        p_charges = metadata["PRECURSOR_CHARGE"]
+        p_mzs = (metadata["MASS"] + (p_charges * PARTICLE_MASSES["PROTON"])) / p_charges
+        # ces = metadata["COLLISION_ENERGY"]
+
+        # prepare spectra
+        irts = data["irt"][:, 0]  # should create a 1D view of the (n_peptides, 1) shaped array
+        f_mzss = data["mz"]
+        f_intss = data["intensities"]
+        # f_annotss = data["annotation"].astype("S", copy=False)
+
+        masked_values = self._calculate_masked_values(f_mzss, f_intss)
+
+        data_list = [*masked_values, p_charges, mass_mod_sequences, seqs, irts, p_mzs]
+        entries = pd.DataFrame(dict(zip(DLIB_COL_NAMES, data_list)))
+        p2p = pd.DataFrame({"PeptideSeq": seqs})
+
+        out.execute("BEGIN")
 
-    def _write_p2p(self, *args, **kwargs):
-        """
-        Internal function to write the p2p table.
+        entries.to_sql(index=False, name="entries", con=out, if_exists="append", method="multi")
+        p2p.to_sql(index=False, name="peptidetoprotein", con=out, if_exists="append", method="multi")
 
-        :param args: forwarded to pandas.to_sql
-        :param kwargs: forwarded to pandas.to_sql
-        """
-        conn = sqlite3.connect(self.out_path)
-        self.p2p.to_sql(name="peptidetoprotein", con=conn, *args, **kwargs)
-        conn.commit()
+        out.commit()
+        # conn.close()
 
-    def prepare_spectrum(self):
+        # def prepare_spectrum(self):
         """Converts grpc output and metadata dataframe into dlib format."""
         # precursor_mz: Union[List[float], np.ndarray],
         # precursor_charges: Union[List[int], np.ndarray],
         # modified_sequences: List[str],
         # retention_times: Union[List[float], np.ndarray],
         # fragmentmz: List[np.ndarray],
         # intensities: List[np.ndarray],
 
-        intensities = self.grpc_output[list(self.grpc_output)[0]]["intensity"]
-        fragment_mz = self.grpc_output[list(self.grpc_output)[0]]["fragmentmz"]
+        # intensities = self.grpc_output[list(self.grpc_output)[0]]["intensity"]
+        # fragment_mz = self.grpc_output[list(self.grpc_output)[0]]["fragmentmz"]
         # annotation = self.grpc_output[list(self.grpc_output)[0]]["annotation"]
-        irt = self.grpc_output[list(self.grpc_output)[1]]
-        retention_times = irt.flatten()
-        modified_sequences = self.spectra_input["MODIFIED_SEQUENCE"]
-
-        precursor_charges = self.spectra_input["PRECURSOR_CHARGE"]
-        precursor_masses = self.spectra_input["MASS"]
-        precursor_mz = (precursor_masses + (precursor_charges * PARTICLE_MASSES["PROTON"])) / precursor_charges
+        # irt = self.grpc_output[list(self.grpc_output)[1]]
+        # retention_times = irt.flatten()
+        # modified_sequences = self.spectra_input["MODIFIED_SEQUENCE"]
+
+        # precursor_charges = self.spectra_input["PRECURSOR_CHARGE"]
+        # precursor_masses = self.spectra_input["MASS"]
+        # precursor_mz = (precursor_masses + (precursor_charges * PARTICLE_MASSES["PROTON"])) / precursor_charges
 
-        self.create_database(self.out_path)
+        # self.create_database(self.out_path)
 
         # gather all values for the entries table and create pandas DataFrame
-        masked_values = self._calculate_masked_values(fragment_mz, intensities)
-        mass_mod_sequences = internal_to_mod_mass(modified_sequences)
-        sequences = internal_without_mods(modified_sequences)
-        data_list = [*masked_values, precursor_charges, mass_mod_sequences, sequences, retention_times, precursor_mz]
-        self.entries = pd.DataFrame(dict(zip(DLIB_COL_NAMES, data_list)))
+        # masked_values = self._calculate_masked_values(fragment_mz, intensities)
+        # mass_mod_sequences = internal_to_mod_mass(modified_sequences)
+        # sequences = internal_without_mods(modified_sequences)
+        # data_list = [*masked_values, precursor_charges, mass_mod_sequences, sequences, retention_times, precursor_mz]
+        # self.entries = pd.DataFrame(dict(zip(DLIB_COL_NAMES, data_list)))
 
         # hardcoded entries that we currently not use.
         # Visit https://bitbucket.org/searleb/encyclopedia/wiki/EncyclopeDIA%20File%20Formats for dlib specs
-        self.entries["Copies"] = 1  # this is hardcorded for now and unused
-        self.entries["Score"] = 0
-        self.entries["CorrelationEncodedLength"] = None
-        self.entries["CorrelationArray"] = None
-        self.entries["RTInSecondsStart"] = None
-        self.entries["RTInSecondsStop"] = None
-        self.entries["MedianChromatogramEncodedLength"] = None
-        self.entries["MedianChromatogramArray"] = None
-        self.entries["SourceFile"] = "Prosit"
+        # self.entries["Copies"] = 1  # this is hardcorded for now and unused
+        # self.entries["Score"] = 0
+        # self.entries["CorrelationEncodedLength"] = None
+        # self.entries["CorrelationArray"] = None
+        # self.entries["RTInSecondsStart"] = None
+        # self.entries["RTInSecondsStop"] = None
+        # self.entries["MedianChromatogramEncodedLength"] = None
+        # self.entries["MedianChromatogramArray"] = None
+        # self.entries["SourceFile"] = "Prosit"
 
         # gather all values for the p2p table and create pandas DataFrame
-        self.p2p = pd.DataFrame({"PeptideSeq": sequences, "isDecoy": False, "ProteinAccession": "unknown"})
+        # self.p2p = pd.DataFrame({"PeptideSeq": sequences, "isDecoy": False, "ProteinAccession": "unknown"})
```

### Comparing `spectrum_io-0.4.2/spectrum_io/spectral_library/msp/myPrositLib.msp` & `spectrum_io-0.4.3/spectrum_io/spectral_library/msp/myPrositLib.msp`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.2/spectrum_io/spectral_library/spectral_library.py` & `spectrum_io-0.4.3/spectrum_io/spectral_library/spectral_library.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import abstractmethod
 from multiprocessing import Queue
 from multiprocessing.managers import ValueProxy
 from pathlib import Path
+from sqlite3 import Connection
 from typing import IO, Dict, Optional, Union
 
 import numpy as np
 import pandas as pd
 
 
 class SpectralLibrary:
@@ -40,27 +41,30 @@
     def write(self, *args, **kwargs):
         """
         Write content to the output file.
 
         :param args: Positional arguments to be passed to the internal _write method.
         :param kwargs: Keyword arguments to be passed to the internal _write method.
         """
-        with open(self.out_path, self.mode) as out:
-            self._write_header(out)
+        with self._get_handle() as out:
+            self._initialize(out)
             self._write(out, *args, **kwargs)
 
+    def _get_handle(self):
+        return open(self.out_path, self.mode)
+
     def async_write(self, queue: Queue, progress: ValueProxy):
         """
         Asynchronously write content to the output file from a queue.
 
         :param queue: A queue from which content will be retrieved for writing.
         :param progress: An integer value representing the progress of the writing process.
         """
-        with open(self.out_path, self.mode) as out:
-            self._write_header(out)
+        with self._get_handle() as out:
+            self._initialize(out)
             while True:
                 content = queue.get()
                 if content is None:
                     break
                 self._write(out, *content)
                 progress.value += 1
 
@@ -78,29 +82,24 @@
         :param f_int: The fragment's (predicted) intensity
 
         :return: boolean (array) that determines if the fragment passes the filter
         """
         return (f_mz != -1) & (f_int >= self.min_intensity_threshold)
 
     @abstractmethod
-    def _write(self, out: IO, data: Dict[str, np.ndarray], metadata: pd.DataFrame):
+    def _write(self, out: Union[IO, Connection], data: Dict[str, np.ndarray], metadata: pd.DataFrame):
         """
         Internal writer function.
 
         This function takes a batch of data and corresponding metadata and writes it to the provided
         output file handle. The file handle logic is provided using the public write or async_write
         functions.
 
         :param out: file handle accepting the data to be written to disk
         :param data: Dictionary containing TODO keys and corresponding values as numpy array
         :param metadata: a dataframe that contains the columns TODO
         """
         pass
 
     @abstractmethod
-    def _write_header(self, out: IO):
-        pass
-
-    @abstractmethod
-    def prepare_spectrum(self):
-        """Prepare spectrum."""
+    def _initialize(self, out: Union[IO, Connection]):
         pass
```

### Comparing `spectrum_io-0.4.2/spectrum_io/spectral_library/spectronaut/myPrositLib.csv` & `spectrum_io-0.4.3/spectrum_io/spectral_library/spectronaut/myPrositLib.csv`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.2/spectrum_io/spectral_library/spectronaut.py` & `spectrum_io-0.4.3/spectrum_io/spectral_library/spectronaut.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import re
 from itertools import chain, cycle
-from typing import IO, Dict, Tuple
+from sqlite3 import Connection
+from typing import IO, Dict, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from spectrum_fundamentals.constants import PARTICLE_MASSES
 from spectrum_fundamentals.mod_string import internal_to_spectronaut, internal_without_mods
 
 from .spectral_library import SpectralLibrary
@@ -21,16 +22,18 @@
         m = re.match(r"([by])(\d+)\+(\d)(?:-(\w+))?", f_annot.decode())
         if m is None:
             raise ValueError(f"Malformed annotation string encountered: {f_annot.decode()}")
         return (
             f"{f_int:.4f},{f_mz:.8f},{m.group(2)},{m.group(1)},{m.group(3)},{m.group(4) if m.group(4) else 'noloss'}\n"
         )
 
-    def _write(self, out: IO, data: Dict[str, np.ndarray], metadata: pd.DataFrame):
+    def _write(self, out: Union[IO, Connection], data: Dict[str, np.ndarray], metadata: pd.DataFrame):
         # prepare metadata
+        if isinstance(out, Connection):
+            raise TypeError("Not supported. Use DLib if you want to write a database file.")
         seqs = metadata["SEQUENCE"]
         modseqs = internal_to_spectronaut(metadata["MODIFIED_SEQUENCE"].apply(lambda x: "_" + x + "_"))
         p_charges = metadata["PRECURSOR_CHARGE"]
         p_mzs = (metadata["MASS"] + (p_charges * PARTICLE_MASSES["PROTON"])) / p_charges
         ces = metadata["COLLISION_ENERGY"]
 
         # prepare spectra
@@ -45,13 +48,15 @@
             f_intss, f_mzss, modseqs, seqs, p_charges, p_mzs, irts, ces, f_annotss
         ):
             cond = self._fragment_filter_passed(f_mzs, f_ints)
             line_start = [f"{modseq},{seq},{seq},{p_charge},{p_mz:.8f},{irt:.2f},{ce},"]
             fragment_list = vec_assemble(f_ints[cond], f_mzs[cond], f_annots[cond])
             out.writelines(chain.from_iterable(zip(cycle(line_start), fragment_list)))
 
-    def _write_header(self, out: IO):
+    def _initialize(self, out: Union[IO, Connection]):
+        if isinstance(out, Connection):
+            raise TypeError("Not supported. Use DLib if you want to write a database file.")
         if self.mode == "w":
             out.write(
                 "ModifiedPeptide,LabeledPeptide,StrippedPeptide,PrecursorCharge,PrecursorMz,iRT,CollisionEnergy,"
                 "RelativeFragmentIntensity,FragmentMz,FragmentNumber,FragmentType,FragmentCharge,FragmentLossType\n"
             )
```

### Comparing `spectrum_io-0.4.2/PKG-INFO` & `spectrum_io-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum_io
-Version: 0.4.2
+Version: 0.4.3
 Summary: IO related functionalities for oktoberfest.
 Home-page: https://github.com/wilhelm-lab/spectrum_io
 License: MIT
 Author: Wilhelmlab at Technical University of Munich
 Requires-Python: >=3.8.0,<3.11.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,16 +18,15 @@
 Requires-Dist: lxml (>=4.5.2,<5.0.0)
 Requires-Dist: numpy (>=1.18.1,<2.0.0)
 Requires-Dist: pandas (>=1.3.0,<2.0.0)
 Requires-Dist: pymzml (>=2.5.0,<3.0.0)
 Requires-Dist: pyteomics (>=4.3.3,<5.0.0)
 Requires-Dist: rich (>=10.3.0)
 Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0)
-Requires-Dist: spectrum-fundamentals (>=0.5.0,<0.6.0)
-Requires-Dist: tables (>=3.6.1,<4.0.0)
+Requires-Dist: spectrum-fundamentals (>=0.5.2,<0.6.0)
 Project-URL: Documentation, https://spectrum_io.readthedocs.io
 Project-URL: Repository, https://github.com/wilhelm-lab/spectrum_io
 Description-Content-Type: text/x-rst
 
 spectrum_io
 ===========================
```

