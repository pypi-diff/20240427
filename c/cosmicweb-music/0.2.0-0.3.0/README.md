# Comparing `tmp/cosmicweb_music-0.2.0.tar.gz` & `tmp/cosmicweb_music-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmicweb_music-0.2.0.tar", max compression
+gzip compressed data, was "cosmicweb_music-0.3.0.tar", max compression
```

## Comparing `cosmicweb_music-0.2.0.tar` & `cosmicweb_music-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1075 2024-04-22 15:37:18.832803 cosmicweb_music-0.2.0/LICENSE
--rw-r--r--   0        0        0     1151 2024-04-22 15:37:18.832803 cosmicweb_music-0.2.0/README.md
--rw-r--r--   0        0        0       22 2024-04-22 15:37:18.832803 cosmicweb_music-0.2.0/cosmicweb_music/__init__.py
--rwxr-xr-x   0        0        0    13499 2024-04-22 15:37:18.832803 cosmicweb_music-0.2.0/cosmicweb_music/cosmICweb.py
--rw-r--r--   0        0        0     1034 2024-04-22 15:37:18.832803 cosmicweb_music-0.2.0/cosmicweb_music/data_types.py
--rw-r--r--   0        0        0     1942 2024-04-22 15:37:18.832803 cosmicweb_music-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 cosmicweb_music-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-04-27 17:16:45.536466 cosmicweb_music-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1288 2024-04-27 17:16:45.536466 cosmicweb_music-0.3.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-27 17:16:45.536466 cosmicweb_music-0.3.0/cosmicweb_music/__init__.py
+-rwxr-xr-x   0        0        0    15496 2024-04-27 17:16:45.536466 cosmicweb_music-0.3.0/cosmicweb_music/cosmICweb.py
+-rw-r--r--   0        0        0     1053 2024-04-27 17:16:45.536466 cosmicweb_music-0.3.0/cosmicweb_music/data_types.py
+-rw-r--r--   0        0        0     1942 2024-04-27 17:16:45.536466 cosmicweb_music-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2390 1970-01-01 00:00:00.000000 cosmicweb_music-0.3.0/PKG-INFO
```

### Comparing `cosmicweb_music-0.2.0/LICENSE` & `cosmicweb_music-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmicweb_music-0.2.0/README.md` & `cosmicweb_music-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,21 @@
   --common-directory      store all config files in the same directory instead
                           of individual directories for each halo
   --attempts INTEGER      number of attempts to download ellipsoids
   --verbose
   --help                  Show this message and exit.
 
 Commands:
+  collection   Download shared ICs using the collection UUID
   get          Download ICs using a target UUID generated on cosmICweb
   publication  Download published ICs using the publication name
 ```
 ### Examples
 ```bash
 cosmicweb-music publication agora-halos
 ```
 ```bash
 cosmicweb-music get f5399734-ad67-432b-ba4d-61bc2088136a
 ```
+```bash
+cosmicweb-music collection c30de0f3-ab4d-48ad-aa26-f20bb4b70bbd
+```
```

### Comparing `cosmicweb_music-0.2.0/cosmicweb_music/cosmICweb.py` & `cosmicweb_music-0.3.0/cosmicweb_music/cosmICweb.py`

 * *Files 11% similar despite different names*

```diff
@@ -122,28 +122,42 @@
         api_token=sim["api_token"],
         MUSIC=sim["ics"],
         settings=content["configuration"],
         accessed_at=datetime.now(),
     )
 
 
-def fetch_publication(
-    cosmicweb_url: str, publication_name: str, traceback_radius
+def fetch_multiple(
+    cosmicweb_url: str,
+    traceback_radius,
+    publication_name: str = None,
+    collection_uuid: str = None,
 ) -> DownloadConfig:
+    if publication_name:
+        url = f"{cosmicweb_url}/api/publications/{publication_name}"
+    elif collection_uuid:
+        url = f"{cosmicweb_url}/api/collections/{collection_uuid}"
+    else:
+        raise ValueError("must provide either publication_name or collection_uuid")
     try:
-        r = requests.get(cosmicweb_url + "/api/publications/" + publication_name)
+        r = requests.get(url)
         # This will raise an error if not successful
         r.raise_for_status()
     except requests.exceptions.HTTPError as e:
         logging.critical("Failed downloading from cosmICweb.")
         logging.critical(e)
         sys.exit(1)
     content = r.json()
     sim = content["simulation"]
-    halo_names = [h["name"] for h in content["halos"]]
+    halo_names = []
+    for h in content["halos"]:
+        name = h["name"]
+        if name is None:
+            name = str(h["id"])
+        halo_names.append(name)
     halo_ids = [h["id"] for h in content["halos"]]
     halo_urls = [
         "{url}/simulation/{sid}/halo/{hid}".format(
             url=sim["api_url"], sid=sim["api_id"], hid=h["id"]
         )
         for h in content["halos"]
     ]
@@ -181,34 +195,52 @@
         param = line.split("=")[0].strip()
         if param in parameters:
             line = line.split("=")[0] + f"= {parameters[param]}"
         new_lines.append(line)
     return "\n".join(new_lines)
 
 
+def normalize_lineendings(text: str) -> str:
+    return text.replace("\r\n", "\n")
+
+
 def music_config_to_template(config: DownloadConfig) -> str:
     music_config = config.MUSIC
+    music_config = {k: normalize_lineendings(v) for k, v in music_config.items()}
+
     settings = config.settings
     # TODO: apply output configuration
     config = (
         "[setup]\n" + music_config["setup"] + "\n\n<ELLIPSOID_TEMPLATE>\n\n"
         "[cosmology]\n" + music_config["cosmology"] + "\n\n"
         "[random]\n" + music_config["random"] + "\n\n"
-        "[poisson]\n" + music_config["poisson"]
+        "[poisson]\n" + music_config["poisson"] + "\n\n"
     )
     if settings:
         config = apply_config_parameter(
             config,
             {
                 "levelmin": settings["resolution"]["low"],
                 "levelmin_TF": settings["resolution"]["low"],
                 "levelmax": settings["resolution"]["high"],
                 "zstart": settings["startRedshift"],
             },
         )
+        if settings["outputType"]:
+            config += f"""
+[output]
+format = {settings["outputType"]}
+filename = {settings["outputFilename"]}
+            """.strip()
+            config += "\n"
+            for k, v in settings["outputOptions"]:
+                config += f"{k} = {v}\n"
+    if not settings or not settings["outputType"]:
+        # TODO: allow specifying output format via cli argument
+        config += "[output]\n# TODO: add output options"
     return config
 
 
 def compose_template(
     template: str,
     ellipsoid: Ellipsoid,
     config: DownloadConfig,
@@ -320,24 +352,38 @@
     logging.info("Download configuration successfully fetched")
     return process_config(config, args, store)
 
 
 def publication_mode(
     args: Args, publication_name: str, traceback_radius, store=True
 ) -> None | str:
-    logging.info(
-        "Fetching publication " + publication_name + " from the cosmICweb server"
+    logging.info(f"Fetching publication {publication_name} from the cosmICweb server")
+    config = fetch_multiple(
+        args.url, traceback_radius, publication_name=publication_name
     )
-    config = fetch_publication(args.url, publication_name, traceback_radius)
     args = args._replace(output_path=os.path.join(args.output_path, publication_name))
     logging.debug("Output directory set to " + args.output_path)
     logging.info("Publication successfully fetched")
     return process_config(config, args, store)
 
 
+def collection_mode(
+    args: Args, collection_uuid: str, traceback_radius, store=True
+) -> None | str:
+    logging.info(f"Fetching collection {collection_uuid} from the cosmICweb server")
+    config = fetch_multiple(args.url, traceback_radius, collection_uuid=collection_uuid)
+    args = args._replace(
+        output_path=os.path.join(args.output_path, config.simulation_name)
+    )
+    logging.debug("Output directory set to " + args.output_path)
+    logging.info("Publication successfully fetched")
+    print(config)
+    return process_config(config, args, store)
+
+
 def dir_path(p: str) -> str:
     if os.path.isdir(p):
         return p
     else:
         raise NotADirectoryError(p)
 
 
@@ -388,9 +434,21 @@
 @click.pass_context
 def publication(ctx, publication_name, traceback_radius):
     traceback_radius = float(traceback_radius)
     args: Args = ctx.obj
     publication_mode(args, publication_name, traceback_radius)
 
 
+@cli.command(help="Download shared ICs using the collection UUID")
+@click.argument("collection")
+@click.option(
+    "--traceback_radius", type=click.Choice(["1", "2", "4", "10"]), default="2"
+)
+@click.pass_context
+def collection(ctx, collection, traceback_radius):
+    traceback_radius = float(traceback_radius)
+    args: Args = ctx.obj
+    collection_mode(args, collection, traceback_radius)
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `cosmicweb_music-0.2.0/cosmicweb_music/data_types.py` & `cosmicweb_music-0.3.0/cosmicweb_music/data_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from datetime import datetime
-from typing import NamedTuple, Any, List, Dict, TypedDict
+from typing import NamedTuple, Any, List, Dict, TypedDict, Tuple
 
 
 class Ellipsoid(NamedTuple):
     center: List[float]
     shape: List[List[float]]
     traceback_radius: float
     radius_definition: str
@@ -15,18 +15,18 @@
     low: int
     high: int
 
 
 class Configuration(TypedDict):
     outputType: str
     resolution: Resolution
-    outputOptions: List[Any]
+    outputOptions: List[Tuple[str, str]]
     startRedshift: int
     outputFilename: str
-    separateFolders: bool
+    seperateFolders: bool
     tracebackRadius: int | float | str
 
 
 class ICSections(TypedDict):
     setup: str
     random: str
     cosmology: str
```

### Comparing `cosmicweb_music-0.2.0/pyproject.toml` & `cosmicweb_music-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.poetry]
-version = "0.2.0"
+version = "0.3.0"
 name = "cosmicweb-music"
 description = "Script to download initial conditions for zoom-in cosmological simulations from the cosmICweb service."
 authors = [
     "Michael Buehlmann <buehlmann.michi@gmail.com>",
     "Lukas Winkler <python@lw1.at>",
 ]
 license = "MIT"
@@ -16,15 +16,15 @@
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering",
     "Intended Audience :: Science/Research",
 ]
 
 [tool.bumpversion]
-current_version = "0.2.0"
+current_version = "0.3.0"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 tag = true
 sign_tags = false
 tag_name = "v{new_version}"
```

### Comparing `cosmicweb_music-0.2.0/PKG-INFO` & `cosmicweb_music-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmicweb-music
-Version: 0.2.0
+Version: 0.3.0
 Summary: Script to download initial conditions for zoom-in cosmological simulations from the cosmICweb service.
 Home-page: https://github.com/cosmo-sims/cosmicweb-music
 License: MIT
 Keywords: scientific computing
 Author: Michael Buehlmann
 Author-email: buehlmann.michi@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -45,18 +45,22 @@
   --common-directory      store all config files in the same directory instead
                           of individual directories for each halo
   --attempts INTEGER      number of attempts to download ellipsoids
   --verbose
   --help                  Show this message and exit.
 
 Commands:
+  collection   Download shared ICs using the collection UUID
   get          Download ICs using a target UUID generated on cosmICweb
   publication  Download published ICs using the publication name
 ```
 ### Examples
 ```bash
 cosmicweb-music publication agora-halos
 ```
 ```bash
 cosmicweb-music get f5399734-ad67-432b-ba4d-61bc2088136a
 ```
+```bash
+cosmicweb-music collection c30de0f3-ab4d-48ad-aa26-f20bb4b70bbd
+```
```

