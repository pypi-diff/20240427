# Comparing `tmp/labelme_toolkit-1.1.0.tar.gz` & `tmp/labelme_toolkit-1.1.1.tar.gz`

## Comparing `labelme_toolkit-1.1.0.tar` & `labelme_toolkit-1.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/Makefile
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/README.md
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/__init__.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/__main__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_formats.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_json.py
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_labelme.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_migrations.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_paths.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_testing.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_browsers/__init__.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_browsers/_images.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_browsers/css/modern-normalize.min.css
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_cli/__init__.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_cli/_extract_image.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_cli/_extract_image_test.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_cli/_install_toolkit_pro.py
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_cli/_json_to_mask.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_cli/_json_to_mask_test.py
--rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_cli/_json_to_visualization.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_cli/_json_to_visualization_test.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_cli/_list_labels.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_cli/_list_labels_test.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_data/.gitignore
--rw-r--r--   0        0        0   891941 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_data/dogs.json
--rw-r--r--   0        0        0   396616 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_data/small_dataset.zip
--rwxr-xr-x   0        0        0   147408 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_data/small_dataset/2011_000003.jpg
--rw-r--r--   0        0        0     9345 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_data/small_dataset/2011_000003.json
--rwxr-xr-x   0        0        0   108615 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_data/small_dataset/2011_000006.jpg
--rw-r--r--   0        0        0    10129 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_data/small_dataset/2011_000006.json
--rwxr-xr-x   0        0        0   136977 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_data/small_dataset/2011_000025.jpg
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/labelme_toolkit/_data/small_dataset/2011_000025.json
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/Makefile
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/README.md
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/__main__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_formats.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_json.py
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_labelme.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_migrations.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_paths.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_testing.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_browsers/__init__.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_browsers/_images.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_browsers/css/modern-normalize.min.css
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_cli/__init__.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_cli/_extract_image.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_cli/_extract_image_test.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_cli/_install_toolkit_pro.py
+-rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_cli/_json_to_mask.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_cli/_json_to_mask_test.py
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_cli/_json_to_visualization.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_cli/_json_to_visualization_test.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_cli/_list_labels.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_cli/_list_labels_test.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_data/.gitignore
+-rw-r--r--   0        0        0   891941 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_data/dogs.json
+-rw-r--r--   0        0        0   396616 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_data/small_dataset.zip
+-rwxr-xr-x   0        0        0   147408 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_data/small_dataset/2011_000003.jpg
+-rw-r--r--   0        0        0     9345 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_data/small_dataset/2011_000003.json
+-rwxr-xr-x   0        0        0   108615 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_data/small_dataset/2011_000006.jpg
+-rw-r--r--   0        0        0    10129 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_data/small_dataset/2011_000006.json
+-rwxr-xr-x   0        0        0   136977 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_data/small_dataset/2011_000025.jpg
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/labelme_toolkit/_data/small_dataset/2011_000025.json
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 labelme_toolkit-1.1.1/PKG-INFO
```

### Comparing `labelme_toolkit-1.1.0/Makefile` & `labelme_toolkit-1.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.0/.github/workflows/ci.yml` & `labelme_toolkit-1.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.0/labelme_toolkit/_labelme.py` & `labelme_toolkit-1.1.1/labelme_toolkit/_labelme.py`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.0/labelme_toolkit/_paths.py` & `labelme_toolkit-1.1.1/labelme_toolkit/_paths.py`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.0/labelme_toolkit/_browsers/_images.py` & `labelme_toolkit-1.1.1/labelme_toolkit/_browsers/_images.py`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.0/labelme_toolkit/_browsers/css/modern-normalize.min.css` & `labelme_toolkit-1.1.1/labelme_toolkit/_browsers/css/modern-normalize.min.css`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.0/labelme_toolkit/_cli/_extract_image.py` & `labelme_toolkit-1.1.1/labelme_toolkit/_cli/_extract_image.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 from typing import Dict
 from typing import List
 
 import click
 import PIL.Image
 from loguru import logger
 
-from labelme_toolkit import _json
-from labelme_toolkit import _migrations
-from labelme_toolkit import _paths
-from labelme_toolkit._cli import cli
+from .. import _json
+from .. import _migrations
+from .. import _paths
 
 
 def _extract_image(json_file: str, output_dir: str) -> None:
     with open(json_file) as f:
         json_data: Dict = json.load(f)
     _migrations.migrate_json_data(json_data=json_data)
 
@@ -39,15 +38,15 @@
     json_data["imageData"] = None
     json_data["imagePath"] = os.path.relpath(output_image_file, output_dir)
     with open(output_json_file, "w") as f:
         json.dump(json_data, f, indent=2)
     logger.info(f"Saved to: {output_json_file!r}")
 
 
-@cli.command()
+@click.command()
 @click.argument("file_or_dir", type=click.Path(exists=True), required=True)
 def extract_image(file_or_dir) -> None:
     """Extract image from a JSON file.
 
     Pass a JSON file or directory to extract from.
 
     Examples:
```

### Comparing `labelme_toolkit-1.1.0/labelme_toolkit/_cli/_extract_image_test.py` & `labelme_toolkit-1.1.1/labelme_toolkit/_cli/_extract_image_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import os.path as osp
 import subprocess
 
 import numpy as np
 import PIL.Image
 
-from labelme_toolkit._testing import small_dataset  # noqa
+from .._testing import small_dataset  # noqa
 
 
 def test_extract_image(small_dataset):  # noqa
     subprocess.check_call(["labelmetk", "extract-image", small_dataset])
 
     assert osp.isdir(osp.join(small_dataset + ".export"))
     json_files = glob.glob(osp.join(small_dataset + ".export", "*.json"))
```

### Comparing `labelme_toolkit-1.1.0/labelme_toolkit/_cli/_install_toolkit_pro.py` & `labelme_toolkit-1.1.1/labelme_toolkit/_cli/_install_toolkit_pro.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 import os.path as osp
 import subprocess
 import urllib.request
 
 import click
 from loguru import logger
 
-from labelme_toolkit._cli import cli
 
-
-@cli.command()
+@click.command()
 @click.option(
     "--access-key",
     prompt=True,
     help="access key to install",
 )
 @click.option(
     "--version",
     default="latest",
     help="version to install",
 )
-def install_toolkit_pro(access_key: str, version: str):
+@click.option(
+    "--yes",
+    is_flag=True,
+    help="install without confirmation",
+)
+@click.option(
+    "--list-versions",
+    is_flag=True,
+    help="list available versions",
+)
+def install_toolkit_pro(access_key: str, version: str, yes: bool, list_versions: bool):
     """Install Toolkit Pro.
 
     Examples:
 
      \b
      $ labelmetk install-toolkit-pro  # install latest
      $ labelmetk install-toolkit-pro --version 1.0.0
@@ -35,24 +43,32 @@
 
     url_path = f"https://labelmeai.github.io/toolkit-pro/{access_key}"
 
     with urllib.request.urlopen(osp.join(url_path, "versions")) as response:
         data = response.read()
         versions = [version.strip() for version in data.decode("utf-8").splitlines()]
 
-    logger.info(f"Available versions: {versions}")
+    if list_versions:
+        for version in versions:
+            click.echo(version)
+        return
 
     if version == "latest":
         version = versions[-1]
-        logger.info(f"Version: {version} (latest)")
+        logger.info(f"Installing version: {version} (latest)")
     elif version not in versions:
         logger.error(f"Version {version} is not available")
         return
     else:
-        logger.info(f"Version: {version}")
+        logger.info(f"Installing version: {version}")
+
+    if not yes:
+        if not click.confirm("Do you want to install?"):
+            click.echo("Installation is canceled.")
+            return
 
     cmd = [
         "pip",
         "install",
         "-I",
         osp.join(url_path, f"labelme_toolkit_pro-{version}-py3-none-any.whl"),
     ]
```

### Comparing `labelme_toolkit-1.1.0/labelme_toolkit/_cli/_json_to_mask.py` & `labelme_toolkit-1.1.1/labelme_toolkit/_cli/_json_to_mask.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 from typing import Optional
 
 import click
 import numpy as np
 import PIL.Image
 from loguru import logger
 
-from labelme_toolkit import _browsers
-from labelme_toolkit import _labelme
-from labelme_toolkit import _migrations
-from labelme_toolkit import _paths
-from labelme_toolkit._cli import cli
+from .. import _browsers
+from .. import _labelme
+from .. import _migrations
+from .. import _paths
 
 
 def _json_to_mask(
     json_file: str,
     output_dir: str,
     include_labels: Optional[List[str]] = None,
     exclude_labels: Optional[List[str]] = None,
@@ -65,15 +64,15 @@
     output_file = os.path.join(output_dir, "mask.png")
     PIL.Image.fromarray(mask.astype("uint8") * 255).save(output_file)
     logger.info(f"Saved to: {output_file!r}")
 
     return output_file
 
 
-@cli.command()
+@click.command()
 @click.argument("file_or_dir", type=click.Path(exists=True), required=True)
 @click.option(
     "--include-labels",
     type=str,
     multiple=True,
     help="labels to include (cannot be used with --exclude-labels)",
     default=None,
```

### Comparing `labelme_toolkit-1.1.0/labelme_toolkit/_cli/_json_to_visualization.py` & `labelme_toolkit-1.1.1/labelme_toolkit/_cli/_json_to_visualization.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 from typing import Optional
 
 import click
 import imgviz
 import PIL.Image
 from loguru import logger
 
-from labelme_toolkit import _browsers
-from labelme_toolkit import _json
-from labelme_toolkit import _labelme
-from labelme_toolkit import _migrations
-from labelme_toolkit import _paths
-from labelme_toolkit._cli import cli
+from .. import _browsers
+from .. import _json
+from .. import _labelme
+from .. import _migrations
+from .. import _paths
 
 
 def _json_to_visualization(
     json_file: str,
     output_dir: str,
     exclude_labels: Optional[List[str]] = None,
 ) -> str:
@@ -80,15 +79,15 @@
     output_file = os.path.join(output_dir, "visualization.png")
     image.save(output_file)
     logger.info(f"Saved to: {output_file!r}")
 
     return output_file
 
 
-@cli.command()
+@click.command()
 @click.argument("file_or_dir", type=click.Path(exists=True), required=True)
 @click.option(
     "--exclude-labels",
     type=str,
     multiple=True,
     help="labels to exclude",
     default=None,
```

### Comparing `labelme_toolkit-1.1.0/labelme_toolkit/_cli/_json_to_visualization_test.py` & `labelme_toolkit-1.1.1/labelme_toolkit/_cli/_json_to_visualization_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import glob
 import os.path as osp
 import subprocess
 
 import numpy as np
 import PIL.Image
 
-from labelme_toolkit._testing import small_dataset  # noqa
+from .._testing import small_dataset  # noqa
 
 
 def test_json_to_visualization(small_dataset):  # noqa
     subprocess.check_call(["labelmetk", "json-to-visualization", small_dataset])
 
     assert osp.isdir(osp.join(small_dataset + ".export"))
     visualization_files = glob.glob(
```

### Comparing `labelme_toolkit-1.1.0/labelme_toolkit/_cli/_list_labels.py` & `labelme_toolkit-1.1.1/labelme_toolkit/_cli/_list_labels.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import json
 from typing import List
 
 import click
 
-from labelme_toolkit import _paths
-from labelme_toolkit._cli import cli
+from .. import _paths
 
 
-@cli.command()
+@click.command()
 @click.argument("file_or_dir", type=click.Path(exists=True), required=True)
 def list_labels(file_or_dir: str):
     """List unique labels in the JSON files.
 
     Pass a JSON file or directory to list unique labels from.
 
     Example:
@@ -29,8 +28,8 @@
     for json_file in json_files:
         with open(json_file) as f:
             json_data = json.load(f)
 
         for json_shape in json_data["shapes"]:
             unique_labels.add(json_shape["label"])
 
-    print("\n".join(sorted(unique_labels)))
+    click.echo("\n".join(sorted(unique_labels)))
```

### Comparing `labelme_toolkit-1.1.0/labelme_toolkit/_data/dogs.json` & `labelme_toolkit-1.1.1/labelme_toolkit/_data/dogs.json`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.0/labelme_toolkit/_data/small_dataset.zip` & `labelme_toolkit-1.1.1/labelme_toolkit/_data/small_dataset.zip`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.0/labelme_toolkit/_data/small_dataset/2011_000003.jpg` & `labelme_toolkit-1.1.1/labelme_toolkit/_data/small_dataset/2011_000003.jpg`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.0/labelme_toolkit/_data/small_dataset/2011_000003.json` & `labelme_toolkit-1.1.1/labelme_toolkit/_data/small_dataset/2011_000003.json`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.0/labelme_toolkit/_data/small_dataset/2011_000006.jpg` & `labelme_toolkit-1.1.1/labelme_toolkit/_data/small_dataset/2011_000006.jpg`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.0/labelme_toolkit/_data/small_dataset/2011_000006.json` & `labelme_toolkit-1.1.1/labelme_toolkit/_data/small_dataset/2011_000006.json`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.0/labelme_toolkit/_data/small_dataset/2011_000025.jpg` & `labelme_toolkit-1.1.1/labelme_toolkit/_data/small_dataset/2011_000025.jpg`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.0/labelme_toolkit/_data/small_dataset/2011_000025.json` & `labelme_toolkit-1.1.1/labelme_toolkit/_data/small_dataset/2011_000025.json`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.0/pyproject.toml` & `labelme_toolkit-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `labelme_toolkit-1.1.0/PKG-INFO` & `labelme_toolkit-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: labelme-toolkit
-Version: 1.1.0
+Version: 1.1.1
 Summary: Labelme Toolkit
 Project-URL: Homepage, https://github.com/labelmeai/toolkit
 Author-email: Kentaro Wada <www.kentaro.wada@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

