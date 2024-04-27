# Comparing `tmp/travdata-0.3.2.tar.gz` & `tmp/travdata-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "travdata-0.3.2.tar", max compression
+gzip compressed data, was "travdata-0.4.0.tar", max compression
```

## Comparing `travdata-0.3.2.tar` & `travdata-0.4.0.tar`

### file list

```diff
@@ -1,44 +1,52 @@
--rw-r--r--   0        0        0     1095 2024-04-02 19:56:56.951187 travdata-0.3.2/LICENSE
--rw-r--r--   0        0        0     6682 2024-04-02 19:56:56.951187 travdata-0.3.2/README.rst
--rw-r--r--   0        0        0     1342 2024-04-02 19:56:56.959186 travdata-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      129 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/cli/__init__.py
--rwxr-xr-x   0        0        0     1277 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/cli/cli.py
--rw-r--r--   0        0        0        0 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/cli/cmds/__init__.py
--rw-r--r--   0        0        0     1937 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/cli/cmds/csvtoyaml.py
--rw-r--r--   0        0        0     4207 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/cli/cmds/extractcsvtables.py
--rw-r--r--   0        0        0     2617 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/cli/cmds/licenses.py
--rw-r--r--   0        0        0      646 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/cli/cmds/listbooks.py
--rw-r--r--   0        0        0    22253 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/cli/cmds/tradetable.py
--rw-r--r--   0        0        0      521 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/commontext.py
--rw-r--r--   0        0        0    12409 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/config.py
--rw-r--r--   0        0        0      616 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/csvutil.py
--rw-r--r--   0        0        0     1046 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/dataclassutil.py
--rw-r--r--   0        0        0        0 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/datatypes/__init__.py
--rw-r--r--   0        0        0     3914 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/datatypes/basic.py
--rw-r--r--   0        0        0        0 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/datatypes/core/__init__.py
--rw-r--r--   0        0        0      685 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/datatypes/core/trade.py
--rw-r--r--   0        0        0     3156 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/datatypes/core/worldcreation.py
--rw-r--r--   0        0        0      483 2024-04-02 19:56:56.959186 travdata-0.3.2/src/travdata/datatypes/yamlcodec.py
--rw-r--r--   0        0        0        0 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/extraction/__init__.py
--rw-r--r--   0        0        0     2357 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/extraction/parseutil.py
--rw-r--r--   0        0        0     8517 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/extraction/pdfextract.py
--rw-r--r--   0        0        0     4006 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/extraction/tabulautil.py
--rw-r--r--   0        0        0        0 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/gui/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/gui/extraction/__init__.py
--rw-r--r--   0        0        0    12253 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/gui/extraction/cfgwin.py
--rw-r--r--   0        0        0     4804 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/gui/extraction/runnerwin.py
--rw-r--r--   0        0        0      862 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/gui/gui.py
--rw-r--r--   0        0        0      766 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/gui/qtutil.py
--rw-r--r--   0        0        0        0 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/py.typed
--rw-r--r--   0        0        0        0 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/tableconverters/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/tableconverters/core/__init__.py
--rw-r--r--   0        0        0      550 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/tableconverters/core/registry.py
--rw-r--r--   0        0        0     2079 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/tableconverters/core/trade.py
--rw-r--r--   0        0        0     3802 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/tableconverters/core/worldcreation.py
--rw-r--r--   0        0        0     1093 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/tableconverters/registry.py
--rw-r--r--   0        0        0        0 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/travellermap/__init__.py
--rw-r--r--   0        0        0     3686 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/travellermap/apiurls.py
--rw-r--r--   0        0        0     2397 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/travellermap/sectorparse.py
--rw-r--r--   0        0        0     4879 2024-04-02 19:56:56.963186 travdata-0.3.2/src/travdata/travellermap/world.py
--rw-r--r--   0        0        0     7647 1970-01-01 00:00:00.000000 travdata-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-04-27 06:59:32.835359 travdata-0.4.0/LICENSE
+-rw-r--r--   0        0        0     6682 2024-04-27 06:59:32.835359 travdata-0.4.0/README.rst
+-rw-r--r--   0        0        0     1501 2024-04-27 06:59:32.847360 travdata-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       85 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/cli/__init__.py
+-rwxr-xr-x   0        0        0     1762 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/cli/cli.py
+-rw-r--r--   0        0        0      247 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/cli/cliutil.py
+-rw-r--r--   0        0        0        0 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/cli/cmds/__init__.py
+-rw-r--r--   0        0        0     1995 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/cli/cmds/csvtoyaml.py
+-rw-r--r--   0        0        0     6304 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/cli/cmds/extractcsvtables.py
+-rw-r--r--   0        0        0     2617 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/cli/cmds/licenses.py
+-rw-r--r--   0        0        0      693 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/cli/cmds/listbooks.py
+-rw-r--r--   0        0        0    22253 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/cli/cmds/tradetable.py
+-rw-r--r--   0        0        0      521 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/commontext.py
+-rw-r--r--   0        0        0    11835 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/config/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/config/cfgerror.py
+-rw-r--r--   0        0        0     4223 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/config/cfgextract.py
+-rw-r--r--   0        0        0      224 2024-04-27 06:59:32.847360 travdata-0.4.0/src/travdata/config/yamlreg.py
+-rw-r--r--   0        0        0     1495 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/csvutil.py
+-rw-r--r--   0        0        0     1046 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/dataclassutil.py
+-rw-r--r--   0        0        0        0 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/datatypes/__init__.py
+-rw-r--r--   0        0        0     3914 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/datatypes/basic.py
+-rw-r--r--   0        0        0        0 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/datatypes/core/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/datatypes/core/trade.py
+-rw-r--r--   0        0        0     3156 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/datatypes/core/worldcreation.py
+-rw-r--r--   0        0        0      483 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/datatypes/yamlcodec.py
+-rw-r--r--   0        0        0        0 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/extraction/__init__.py
+-rw-r--r--   0        0        0     5188 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/extraction/bookextract.py
+-rw-r--r--   0        0        0     2357 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/extraction/parseutil.py
+-rw-r--r--   0        0        0     8545 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/extraction/tableextract.py
+-rw-r--r--   0        0        0     4691 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/extraction/tabulautil.py
+-rw-r--r--   0        0        0    11853 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/filesio.py
+-rw-r--r--   0        0        0        0 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/gui/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/gui/extraction/__init__.py
+-rw-r--r--   0        0        0    19093 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/gui/extraction/cfgwin.py
+-rw-r--r--   0        0        0     4948 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/gui/extraction/runnerwin.py
+-rw-r--r--   0        0        0      872 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/gui/gui.py
+-rw-r--r--   0        0        0     1829 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/gui/qtutil.py
+-rw-r--r--   0        0        0        0 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/py.typed
+-rw-r--r--   0        0        0        0 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/tableconverters/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/tableconverters/core/__init__.py
+-rw-r--r--   0        0        0      550 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/tableconverters/core/registry.py
+-rw-r--r--   0        0        0     2079 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/tableconverters/core/trade.py
+-rw-r--r--   0        0        0     3802 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/tableconverters/core/worldcreation.py
+-rw-r--r--   0        0        0     1093 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/tableconverters/registry.py
+-rw-r--r--   0        0        0      171 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/travdatarelease.py
+-rw-r--r--   0        0        0        0 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/travellermap/__init__.py
+-rw-r--r--   0        0        0     3686 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/travellermap/apiurls.py
+-rw-r--r--   0        0        0     2397 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/travellermap/sectorparse.py
+-rw-r--r--   0        0        0     4879 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/travellermap/world.py
+-rw-r--r--   0        0        0     6679 2024-04-27 06:59:32.851359 travdata-0.4.0/src/travdata/yamlutil.py
+-rw-r--r--   0        0        0     7647 1970-01-01 00:00:00.000000 travdata-0.4.0/PKG-INFO
```

### Comparing `travdata-0.3.2/LICENSE` & `travdata-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `travdata-0.3.2/README.rst` & `travdata-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `travdata-0.3.2/pyproject.toml` & `travdata-0.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "travdata"
-version = "0.3.2"
+version = "0.4.0"
 description = "Data utility code for Mongoose Traveller TTRPG."
 authors = ["John Beisley <johnbeisleyuk@gmail.com>"]
 keywords = ["traveller", "ttrpg"]
 license = "MIT"
 readme = "README.rst"  # rebuilt from README.adoc
 repository = "https://github.com/huin/travdata"
 packages = [
@@ -50,7 +50,14 @@
 [tool.mypy]
 exclude = '''(?x)(
     travdata/gui/.*  # QtCore.pyi syntax error.
 )'''
 
 [tool.pylint.main]
 ignore-paths = ["oneoff"]
+
+[tool.pylint."messages control"]
+disable = [
+    "too-few-public-methods",
+    # mypy expects the ellipsis in Protocol methods.
+    "unnecessary-ellipsis",
+]
```

### Comparing `travdata-0.3.2/src/travdata/cli/cmds/csvtoyaml.py` & `travdata-0.4.0/src/travdata/cli/cmds/csvtoyaml.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 YAML files.
 """
 
 import argparse
 import csv
 import pathlib
 
-from travdata import csvutil
+from travdata import csvutil, filesio
 from travdata.datatypes import yamlcodec
 from travdata.tableconverters.core import registry
 
 
 def add_subparser(subparsers) -> None:
     """Adds a subcommand parser to ``subparsers``."""
     argparser: argparse.ArgumentParser = subparsers.add_parser(
@@ -37,29 +37,29 @@
     )
 
 
 def run(args: argparse.Namespace) -> None:
     """CLI entry point."""
     registry.load_all_converters()
 
-    created_directories: set[pathlib.Path] = set()
-    for conv_key, conv_fn in registry.CONVERTERS.converters.items():
-        in_group_dir = args.input_dir / conv_key.group_name
-        out_group_dir = args.output_dir / conv_key.group_name
-        if out_group_dir not in created_directories:
-            out_group_dir.mkdir(parents=True, exist_ok=True)
-        with (
-            csvutil.open_read(
-                in_group_dir / f"{conv_key.table_name}.csv",
-            ) as csv_file_in,
-            open(
-                out_group_dir / f"{conv_key.table_name}.yaml",
-                "wt",
-                encoding="utf-8",
-            ) as yaml_file_out,
-        ):
-            r = csv.DictReader(csv_file_in)
-            data = conv_fn(iter(r))
-            yamlcodec.DATATYPES_YAML.dump(
-                data=list(data),
-                stream=yaml_file_out,
-            )
+    with (
+        filesio.DirReader.open(args.input_dir) as csv_reader,
+        filesio.DirWriter.create(args.output_dir) as yaml_writer,
+    ):
+        for conv_key, conv_fn in registry.CONVERTERS.converters.items():
+            in_group_dir = pathlib.PurePath(conv_key.group_name)
+            out_group_dir = pathlib.PurePath(conv_key.group_name)
+            with (
+                csvutil.open_by_reader(
+                    csv_reader,
+                    in_group_dir / f"{conv_key.table_name}.csv",
+                ) as csv_file_in,
+                yaml_writer.open_write(
+                    out_group_dir / f"{conv_key.table_name}.yaml",
+                ) as yaml_file_out,
+            ):
+                r = csv.DictReader(csv_file_in)
+                data = conv_fn(iter(r))
+                yamlcodec.DATATYPES_YAML.dump(
+                    data=list(data),
+                    stream=yaml_file_out,
+                )
```

### Comparing `travdata-0.3.2/src/travdata/cli/cmds/licenses.py` & `travdata-0.4.0/src/travdata/cli/cmds/licenses.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.2/src/travdata/cli/cmds/listbooks.py` & `travdata-0.4.0/src/travdata/cli/cmds/listbooks.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,10 +18,11 @@
     config.add_config_flag(argparser)
     argparser.set_defaults(run=run)
 
 
 def run(args: argparse.Namespace) -> None:
     """CLI entry point."""
 
-    cfg = config.load_config_from_flag(args, [])
+    with config.config_reader(args) as cfg_reader:
+        cfg = config.load_config(cfg_reader)
     for name in sorted(cfg.books):
         print(name)
```

### Comparing `travdata-0.3.2/src/travdata/cli/cmds/tradetable.py` & `travdata-0.4.0/src/travdata/cli/cmds/tradetable.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.2/src/travdata/commontext.py` & `travdata-0.4.0/src/travdata/commontext.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.2/src/travdata/config.py` & `travdata-0.4.0/src/travdata/config/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,156 +7,62 @@
 * ``book.yaml`` relating to a single input PDF.
 
 See development.adoc for more information in how this is used.
 """
 
 from __future__ import annotations
 
-import abc
 import argparse
+import contextlib
 import dataclasses
 import pathlib
 import sys
 import textwrap
-from typing import Any, ClassVar, Iterator, Optional, cast, TYPE_CHECKING
+from typing import Any, ClassVar, Iterator, Optional, Self
 
-from ruamel import yaml
-from travdata import dataclassutil
+from travdata import filesio, travdatarelease, yamlutil
+from travdata.config import yamlreg
+from travdata.config import cfgextract
 
-if TYPE_CHECKING:
-    from _typeshed import DataclassInstance
 
-_YAML = yaml.YAML(typ="safe")
-# Retain the original ordering in mappings.
-_YAML.representer.sort_base_mapping_type_on_output = False
-
-__executable_environment__ = "development"
-
-
-_SET_METADATA = {"to_yaml": sorted, "from_yaml": set}
-
-
-class UserError(Exception):
-    """Exception raised for user errors."""
-
-
-class YamlDataclassMixin:
-    """Mixin for dataclasses created by YAML parsing.
-
-    It is necessary to implement __setstate__ in any dataclass instances that
-    have been parsed from YAML, because the YAML parser bypasses __init__. This
-    is needed because:
-
-    * Fields with defaults need to be set if not specified.
-    * Errors need to be raised for any fields missing a value that have no
-      default.
-    """
-
-    yaml_tag: ClassVar
-
-    def __setstate__(self, state):
-        try:
-            self.__init__(**state)
-        except Exception as e:
-            e.add_note(f"processing {self.yaml_tag} with {state=}")
-            raise
-
-    @classmethod
-    def to_yaml(cls, representer, node):
-        """Implements serialising the node as basic YAML types."""
-        mapping = {}
-        for field in dataclasses.fields(cast(type["DataclassInstance"], cls)):
-            value = getattr(node, field.name)
-            if not value and dataclassutil.has_default(field):
-                continue
-            if fn := field.metadata.get("to_yaml"):
-                value = fn(value)
-            mapping[field.name] = value
-        return representer.represent_mapping(cls.yaml_tag, mapping)
-
-    @classmethod
-    def from_yaml(cls, constructor, node):
-        """Implements deserialising the node from basic YAML types."""
-        data = constructor.construct_mapping(node)
-        if not isinstance(data, dict):
-            raise TypeError(data)
-        kwargs = {}
-        for field in dataclasses.fields(cast(type["DataclassInstance"], cls)):
-            try:
-                value = data.pop(field.name)
-            except KeyError:
-                if dataclassutil.has_default(field):
-                    continue
-                raise
-            if fn := field.metadata.get("from_yaml"):
-                value = fn(value)
-            kwargs[field.name] = value
-        if data:
-            names = ", ".join(sorted(data))
-            raise TypeError(f"unexpected fields {names} in {cls.yaml_tag}")
-        return cls(**kwargs)
-
-
-class RowFolder(abc.ABC):
-    """Abstract base marker for configuring row grouping."""
-
-
-@dataclasses.dataclass
-@_YAML.register_class
-class StaticRowCounts(RowFolder, YamlDataclassMixin):
-    """Specifies explicit input row counts for output grouped rows."""
-
-    yaml_tag: ClassVar = "!StaticRowCounts"
-    row_counts: list[int]
-
-
-@dataclasses.dataclass
-@_YAML.register_class
-class EmptyColumn(RowFolder, YamlDataclassMixin):
-    """Specifies to group rows by when a given column is empty."""
-
-    yaml_tag: ClassVar = "!EmptyColumn"
-    column_index: int
-
-
-@dataclasses.dataclass
-@_YAML.register_class
-class TableExtraction(YamlDataclassMixin):
-    """Configures the specifics of extracting the CSV from the PDF."""
-
-    yaml_tag: ClassVar = "!TableExtraction"
-    add_header_row: Optional[list[str]] = None
-    row_folding: list[RowFolder] = dataclasses.field(default_factory=list)
+TABULA_TEMPLATE_SUFFIX = ".tabula-template.json"
+_VERSION_FILE = pathlib.PurePath("version.txt")
 
 
 @dataclasses.dataclass
 class Table:
     """Defines metadata and extraction configuration relating to a single table.
 
     The "path" of group names and the table name form the path for both the
     ``.tabula-template.json`` file within the configuration directory and the
     output ``.csv`` file in the output directory.
     """
 
-    file_stem: pathlib.Path
-    type: str
+    file_stem: pathlib.PurePath
     tags: set[str] = dataclasses.field(default_factory=set)
-    extraction: Optional[TableExtraction] = dataclasses.field(default_factory=TableExtraction)
+    extraction: Optional[cfgextract.TableExtraction] = dataclasses.field(
+        default_factory=cfgextract.TableExtraction
+    )
+
+    @property
+    def tabula_template_path(self) -> pathlib.PurePath:
+        """Path to the Tabula template, assuming that it exists."""
+        return self.file_stem.with_suffix(TABULA_TEMPLATE_SUFFIX)
 
 
 @dataclasses.dataclass
 class Group:
     """Group of items to extract from the PDF.
 
     A top-level group within a book is often aligned with a book chapter.
 
     The table items have Tabula templates in ``.directory``.
     """
 
-    directory: pathlib.Path
+    rel_dir: pathlib.PurePath
     tags: set[str] = dataclasses.field(default_factory=set)
     tables: dict[str, Table] = dataclasses.field(default_factory=dict)
     groups: dict[str, "Group"] = dataclasses.field(default_factory=dict)
 
     def all_tables(self) -> Iterator[Table]:
         """Iterates over all tables in this group and its child groups.
 
@@ -164,220 +70,312 @@
         """
         yield from self.tables.values()
         for group in self.groups.values():
             yield from group.all_tables()
 
 
 @dataclasses.dataclass
-class Book(YamlDataclassMixin):
+class Book:
     """Top level information about a book."""
 
     id_: str
     name: str
     default_filename: str
     tags: set[str] = dataclasses.field(default_factory=set)
-    group: Optional[Group] = None
+    _group: Optional[Group] = None
+
+    def load_group(self, cfg_reader: filesio.Reader) -> Group:
+        """Loads and returns the top-level group in the `Book`."""
+        if self._group is None:
+            self._group = load_book(cfg_reader, self.id_, self.tags)
+        return self._group
 
 
 @dataclasses.dataclass
 class Config:
     """Top-level configuration."""
 
-    directory: pathlib.Path
     books: dict[str, Book] = dataclasses.field(default_factory=dict)
 
 
 @dataclasses.dataclass
-@_YAML.register_class
-class _YamlTable(YamlDataclassMixin):
+@yamlreg.YAML.register_class
+class _YamlTable(yamlutil.YamlMappingMixin):
     yaml_tag: ClassVar = "!Table"
-    type: Optional[str] = None
-    tags: set[str] = dataclasses.field(default_factory=set, metadata=_SET_METADATA)
-    extraction: Optional[TableExtraction] = None
+    tags: set[str] = dataclasses.field(default_factory=set, metadata=yamlutil.SET_METADATA)
+    extraction: Optional[cfgextract.TableExtraction] = None
 
-    def prepare(self, name: str, directory: pathlib.Path) -> Table:
+    def prepare(
+        self,
+        name: str,
+        rel_group_dir: pathlib.PurePath,
+        parent_tags: set[str],
+    ) -> Table:
         """Creates a ``Table`` from self.
 
         :param name: Name of the table within its ``Group.groups``.
-        :param directory: Path to the directory of the parent ``Group``,
-        relative to the top-level config directory.
+        :param rel_group_dir: Path to the directory of the table's parent
+        group's directory, relative to the top-level config directory.
+        :param parent_tags: Tags to inherit from parent ``Group``.
         :return: Prepared ``Table``.
         """
-        kw = dataclassutil.shallow_asdict(self)
-        return Table(file_stem=directory / name, **kw)
+        tags = self.tags | parent_tags
+        return Table(
+            file_stem=rel_group_dir / name,
+            tags=tags,
+            extraction=self.extraction,
+        )
 
 
 @dataclasses.dataclass
-@_YAML.register_class
-class _YamlGroup(YamlDataclassMixin):
+@yamlreg.YAML.register_class
+class _YamlGroup(yamlutil.YamlMappingMixin):
     yaml_tag: ClassVar = "!Group"
-    tags: set[str] = dataclasses.field(default_factory=set, metadata=_SET_METADATA)
+    tags: set[str] = dataclasses.field(default_factory=set, metadata=yamlutil.SET_METADATA)
+    templates: Optional[list[cfgextract.TableExtraction]] = None
     groups: dict[str, "_YamlGroup"] = dataclasses.field(default_factory=dict)
     tables: dict[str, _YamlTable] = dataclasses.field(default_factory=dict)
-    extraction_templates: Optional[list[TableExtraction]] = None
 
-    def prepare(self, rel_group_dir: pathlib.Path) -> Group:
+    def prepare(
+        self,
+        rel_group_dir: pathlib.PurePath,
+        parent_tags: set[str],
+    ) -> Group:
         """Creates a ``Group`` from self.
 
         :param rel_group_dir: Path to the directory of this group's directory,
         relative to the top-level config directory.
+        :param parent_tags: Tags to inherit from parent ``Group``.
         :return: Prepared ``Group``.
         """
+        tags = self.tags | parent_tags
         return Group(
-            directory=rel_group_dir,
-            tags=self.tags,
+            rel_dir=rel_group_dir,
+            tags=tags,
             tables={
-                name: table.prepare(name, rel_group_dir) for name, table in self.tables.items()
+                name: table.prepare(name, rel_group_dir, parent_tags=tags)
+                for name, table in self.tables.items()
             },
             groups={
-                name: group.prepare(rel_group_dir / name) for name, group in self.groups.items()
+                name: group.prepare(rel_group_dir / name, parent_tags=tags)
+                for name, group in self.groups.items()
             },
-            # extraction_templates not included, as it is only for use in
-            # anchoring and aliasing by the YAML file author at the time of YAML
-            # parsing.
+            # templates not included, as it is only for use in anchoring and
+            # aliasing by the cfgyaml.YAML.file author at the time of YAML parsing.
         )
 
 
 @dataclasses.dataclass
-@_YAML.register_class
-class _YamlBook(YamlDataclassMixin):
+@yamlreg.YAML.register_class
+class _YamlBook(yamlutil.YamlMappingMixin):
     yaml_tag: ClassVar = "!Book"
     name: str
     default_filename: str
-    tags: set[str] = dataclasses.field(default_factory=set, metadata=_SET_METADATA)
+    tags: set[str] = dataclasses.field(default_factory=set, metadata=yamlutil.SET_METADATA)
+
+    @classmethod
+    def yaml_create_empty(cls) -> Self:
+        return cls(name="", default_filename="")
 
     def prepare(
         self,
-        cfg_dir: pathlib.Path,
         book_id: str,
-        limit_books: list[str],
     ) -> Book:
         """Creates a ``Book`` from self.
 
-        :param cfg_dir: Path to the directory of the ``Config``.
+        :param cfg_reader: Reader for the configuration files.
         :param book_id: ID of the book within the parent _YamlConfig.
-        :param limit_books: Allowlist of book names to load configuration for.
         :return: Prepared ``Book``.
         """
-        book = Book(
+        tags = self.tags | {f"book/{self.name}"}
+        return Book(
             id_=book_id,
             name=self.name,
             default_filename=self.default_filename,
-            tags=self.tags,
+            tags=tags,
         )
-        if book_id in limit_books:
-            rel_book_dir = pathlib.Path(book_id)
-            cfg = _YAML.load(cfg_dir / rel_book_dir / "book.yaml")
-            book.group = _prepare_group(cfg, rel_book_dir)
-        return book
 
 
 @dataclasses.dataclass
-@_YAML.register_class
-class _YamlConfig(YamlDataclassMixin):
+@yamlreg.YAML.register_class
+class _YamlConfig(yamlutil.YamlMappingMixin):
     yaml_tag: ClassVar = "!Config"
     books: dict[str, _YamlBook]
 
-    def prepare(self, cfg_dir: pathlib.Path, limit_books: list[str]) -> Config:
+    @classmethod
+    def yaml_create_empty(cls) -> Self:
+        return cls(books={})
+
+    def prepare(self) -> Config:
         """Creates a ``Group`` from self.
 
-        :param cfg_dir: Path to the directory of the ``Config``.
-        :param limit_books: Allowlist of book names to load configuration for.
+        :param cfg_dir: Path to the directory of the top-level ``Config``.
         :return: Prepared ``Config``.
         """
         books: dict[str, Book] = {}
         for book_id, yaml_book in self.books.items():
-            books[book_id] = yaml_book.prepare(
-                cfg_dir=cfg_dir,
-                book_id=book_id,
-                limit_books=limit_books,
-            )
-        return Config(
-            directory=cfg_dir,
-            books=books,
-        )
+            books[book_id] = yaml_book.prepare(book_id=book_id)
+        return Config(books=books)
 
 
-def _prepare_group(cfg: Any, rel_book_dir: pathlib.Path) -> Group:
-    if not isinstance(cfg, _YamlGroup):
-        raise TypeError(cfg)
-    return cfg.prepare(rel_book_dir)
+def _prepare_group(
+    yaml_group: Any | _YamlGroup,
+    rel_book_dir: pathlib.PurePath,
+    parent_tags: set[str],
+) -> Group:
+    if not isinstance(yaml_group, _YamlGroup):
+        raise TypeError(yaml_group)
+    return yaml_group.prepare(
+        rel_group_dir=rel_book_dir,
+        parent_tags=parent_tags,
+    )
 
 
-def load_group_from_str(yaml_str: str) -> Group:
-    """Loads the configuration from the given string containing YAML."""
-    cfg = _YAML.load(yaml_str)
-    return _prepare_group(cfg, pathlib.Path("."))
+def load_book(
+    cfg_reader: filesio.Reader,
+    book_id: str,
+    parent_tags: set[str],
+) -> Group:
+    """Loads the book configuration from the given reader."""
+    rel_book_dir = pathlib.PurePath(book_id)
+    config_path = rel_book_dir / "book.yaml"
+    with cfg_reader.open_read(config_path) as f:
+        cfg = yamlreg.YAML.load(f)
+    return _prepare_group(
+        yaml_group=cfg,
+        rel_book_dir=rel_book_dir,
+        parent_tags=parent_tags,
+    )
+
 
+def parse_yaml_for_testing(yaml_str: str) -> Any:
+    """Parses the given cfgyaml.YAML. without preparing it.
 
-def _prepare_config(cfg: Any, cfg_dir: pathlib.Path, limit_books: list[str]) -> Config:
+    This is only exposed for testing purposes.
+
+    :param yaml_str: cfgyaml.YAML.to parse.
+    :return: Parsed objects.
+    """
+    return yamlreg.YAML.load(yaml_str)
+
+
+def _prepare_config(cfg: Any | _YamlConfig) -> Config:
     if not isinstance(cfg, _YamlConfig):
         raise TypeError(cfg)
-    return cfg.prepare(cfg_dir, limit_books)
+    return cfg.prepare()
+
+
+def load_config_version(cfg_reader: filesio.Reader) -> Optional[str]:
+    """Loads the configuration version from the ``cfg_reader``."""
+    try:
+        with cfg_reader.open_read(_VERSION_FILE) as f:
+            return f.read().rstrip()
+    except filesio.NotFoundError:
+        return None
+
 
+def save_config_version(cfg_writer: filesio.Writer, version: str) -> None:
+    """Writes the configuration version to the ``cfg_writer``."""
+    with cfg_writer.open_write(_VERSION_FILE) as f:
+        f.write(version)
 
-def load_config(cfg_dir: pathlib.Path, limit_books: list[str]) -> Config:
-    """Loads the configuration from the directory."""
-    cfg = _YAML.load(cfg_dir / "config.yaml")
-    return _prepare_config(cfg=cfg, cfg_dir=cfg_dir, limit_books=limit_books)
+
+def load_config(cfg_reader: filesio.Reader) -> Config:
+    """Loads the configuration from the ``cfg_reader``."""
+    with cfg_reader.open_read(pathlib.PurePath("config.yaml")) as f:
+        cfg = yamlreg.YAML.load(f)
+    return _prepare_config(cfg=cfg)
 
 
 def add_config_flag(argparser: argparse.ArgumentParser) -> None:
     """Adds the flag required to call ``load_config_from_flag`` on the parsed args."""
 
     default_config_dir = get_default_config_path()
 
     argparser.add_argument(
-        "--config-dir",
+        "--config",
         "-c",
         help=textwrap.dedent(
             """
-            Path to the configuration directory. This must contain a config.yaml
-            file, and its required Tabula templates. Some configurations for
-            this should be included with this program's distribution.
+            Path to the configuration. This must be either a directory or ZIP
+            file, directly containing a config.yaml file, book.yaml files in
+            directories, and its required Tabula templates. Some configurations
+            for this should be included with this program's distribution.
             """
         ),
         type=pathlib.Path,
-        metavar="CONFIG_DIR",
+        metavar="CONFIG_PATH",
         required=default_config_dir is None,
         default=default_config_dir,
     )
 
 
 def get_default_config_path() -> Optional[pathlib.Path]:
     """Returns the default path to the config directory.
 
     :raises RuntimeError: If the environment is not recognised.
-    :return: Default path to the config directory, if known.
+    :return: Default path to the config, if known.
     """
-    match __executable_environment__:
+    match travdatarelease.EXECUTABLE_ENVIRONMENT:
         case "development":
             install_dir = _data_dir_for_development()
         case "pyinstaller":
             install_dir = _data_dir_for_pyinstaller()
         case unknown_env:
             raise RuntimeError(f"unknown executable environment {unknown_env!r}")
 
+    config_zip = install_dir / "config.zip"
+    if config_zip.is_file():
+        return config_zip
+
     config_dir = install_dir / "config"
-    config_file = config_dir / "config.yaml"
-    if not config_file.is_file():
-        return None
-    return config_dir
+    if config_dir.is_dir():
+        return config_dir
+
+    return None
 
 
 def _data_dir_for_development() -> pathlib.Path:
     return pathlib.Path.cwd()
 
 
 def _data_dir_for_pyinstaller() -> pathlib.Path:
     return pathlib.Path(getattr(sys, "_MEIPASS"))
 
 
-def load_config_from_flag(args: argparse.Namespace, limit_books: list[str]) -> Config:
-    """Returns a ``Config`` specified by the parsed arguments.
+def config_reader(
+    args: argparse.Namespace,
+) -> contextlib.AbstractContextManager[filesio.Reader]:
+    """Returns a Reader for the configuration.
 
     :param args: Parsed arguments. This must have been generated from a parser
     that included the argument added by ``add_config_flag``.
-    :param limit_books: Name identifiers for the books to load configuration for.
-    :return: Loaded configuration.
+    :return: Context manager for a configuration reader.
+    """
+    path: pathlib.Path = args.config
+    output_type = filesio.IOType.AUTO.resolve_auto(path)
+    return output_type.open(path)
+
+
+def create_config_zip(
+    version: str,
+    config_dir: pathlib.Path,
+    config_zip: pathlib.Path,
+) -> None:
+    """Generates a config ZIP file.
+
+    :param version: Version to write into the configuration.
+    :param config_dir: Config directory to copy from.
+    :param config_zip: Config ZIP file to create.
     """
-    return load_config(args.config_dir, limit_books)
+    with (
+        filesio.DirReader.open(config_dir) as cfg_reader,
+        filesio.ZipWriter.create(config_zip) as cfg_writer,
+    ):
+        save_config_version(cfg_writer, version)
+
+        for path in sorted(cfg_reader.iter_files()):
+            with (
+                cfg_reader.open_read(path) as fr,
+                cfg_writer.open_write(path) as fw,
+            ):
+                fw.write(fr.read())
```

### Comparing `travdata-0.3.2/src/travdata/dataclassutil.py` & `travdata-0.4.0/src/travdata/dataclassutil.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.2/src/travdata/datatypes/basic.py` & `travdata-0.4.0/src/travdata/datatypes/basic.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.2/src/travdata/datatypes/core/trade.py` & `travdata-0.4.0/src/travdata/datatypes/core/trade.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.2/src/travdata/datatypes/core/worldcreation.py` & `travdata-0.4.0/src/travdata/datatypes/core/worldcreation.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.2/src/travdata/extraction/parseutil.py` & `travdata-0.4.0/src/travdata/extraction/parseutil.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.2/src/travdata/extraction/pdfextract.py` & `travdata-0.4.0/src/travdata/extraction/tableextract.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,160 +1,231 @@
 # -*- coding: utf-8 -*-
-"""Extracts tables from a PDF."""
+"""Extracts a single table from a PDF."""
 
-import csv
-import dataclasses
+import functools
 import itertools
 import pathlib
-from typing import Callable, Iterable, Iterator, Protocol, TypeAlias, cast
+import re
+from typing import IO, Iterable, Iterator, Protocol, TypeAlias
 
-from travdata import config, csvutil
+from travdata import config, filesio
+from travdata.config import cfgextract
 from travdata.extraction import parseutil, tabulautil
 
 
+_RX_ANYTHING = re.compile(".*")
+
+
 class TableReader(Protocol):
     """Required interface to extract a table from a PDF file.
 
     :param Protocol: _description_
     """
 
     def read_pdf_with_template(
         self,
         *,
         pdf_path: pathlib.Path,
-        template_path: pathlib.Path,
+        template_file: IO[str],
     ) -> list[tabulautil.TabulaTable]:
         """Reads tables from a PDF file, using the named template file.
 
         :param pdf_path: Path to the PDF file.
-        :param template_path: Path to the tabula-template.json file.
+        :param template_file: File-like reader for the Tabula template JSON
+        file.
         :return: List of extracted tables.
         """
         raise NotImplementedError
 
 
 class ConfigurationError(Exception):
     """Exception indication error in the given configuration."""
 
 
 def extract_table(
-    config_dir: pathlib.Path,
+    cfg_reader: filesio.Reader,
+    table: config.Table,
     pdf_path: pathlib.Path,
-    extraction: config.TableExtraction,
-    file_stem: pathlib.Path,
     table_reader: TableReader,
 ) -> Iterator[list[str]]:
     """Extracts a table from the PDF.
 
-    :param config_dir: Config directory containing the config.yaml file.
+    :cfg_reader: Configuration file reader.
+    :param table: Configuration of the table to extract. ``table.extraction``
+    must not be None.
     :param pdf_path: Path to the PDF to extract from.
-    :param file_stem: Path of the Tabula table template configuration.
-    :param extraction: Table configuration configuration.
-    :param tabula_cfg: Configuration for Tabula extractor.
+    :param tabula_reader: Used to read the table from the PDF.
     :returns: Iterator over rows from the table.
+    :raises ValueError: ``table.extraction`` is None.
     """
-    tabula_rows: Iterator[tabulautil.TabulaRow] = tabulautil.table_rows_concat(
-        table_reader.read_pdf_with_template(
-            pdf_path=pdf_path,
-            template_path=config_dir / file_stem.with_suffix(".tabula-template.json"),
+    if table.extraction is None:
+        raise ValueError(
+            f"extract_table called with table with `None` extraction: {table=}",
         )
-    )
-    text_rows = tabulautil.table_rows_text(tabula_rows)
 
-    if extraction.row_folding:
-        text_rows = _fold_rows(
-            lines=text_rows,
-            grouper=_MultiGrouper(
-                [_make_line_grouper(folder) for folder in extraction.row_folding]
-            ),
+    with cfg_reader.open_read(table.tabula_template_path) as tmpl_file:
+        tabula_rows: Iterator[tabulautil.TabulaRow] = tabulautil.table_rows_concat(
+            table_reader.read_pdf_with_template(
+                pdf_path=pdf_path,
+                template_file=tmpl_file,
+            )
         )
+        rows = tabulautil.table_rows_text(tabula_rows)
 
-    text_rows = _clean_rows(text_rows)
+        for transform_cfg in table.extraction.transforms:
+            rows = _transform(transform_cfg, rows)
 
-    if extraction.add_header_row is not None:
-        text_rows = itertools.chain([extraction.add_header_row], text_rows)
+        return _clean_rows(rows)
 
-    return text_rows
 
-
-_Line: TypeAlias = list[str]
-_LineGroup: TypeAlias = list[_Line]
 _Row: TypeAlias = list[str]
+_RowGroup: TypeAlias = list[_Row]
+
+
+def _transform(cfg: cfgextract.TableTransform, rows: Iterable[_Row]) -> Iterator[_Row]:
+    match cfg:
+        case cfgextract.ExpandColumnOnRegex():
+            return _expand_column_on_regex(cfg, rows)
+        case cfgextract.JoinColumns():
+            return _join_columns(cfg, rows)
+        case cfgextract.PrependRow():
+            return _prepend_row(cfg, rows)
+        case cfgextract.FoldRows():
+            return _fold_rows(cfg, rows)
+        case cfgextract.Transpose():
+            return _transpose(rows)
+        case cfgextract.WrapRowEveryN():
+            return _wrap_row_every_n(cfg, rows)
+        case _:
+            raise ConfigurationError(
+                f"{type(cfg).__name__} is an unknown type of TableTransform",
+            )
+
+
+def _expand_column_on_regex(
+    cfg: cfgextract.ExpandColumnOnRegex,
+    rows: Iterable[_Row],
+) -> Iterator[_Row]:
+    rx = re.compile(cfg.pattern)
+    for row in rows:
+        try:
+            prior, to_match, following = row[: cfg.column], row[cfg.column], row[cfg.column + 1 :]
+        except IndexError:
+            # Specified column not present. Pass-through as-is.
+            yield row
+            continue
+
+        new_row = prior
+
+        if rx_match := rx.fullmatch(to_match):
+            for cell_tmpl in cfg.on_match:
+                new_row.append(rx_match.expand(cell_tmpl))
+        elif rx_match := _RX_ANYTHING.fullmatch(to_match):
+            for cell_tmpl in cfg.default:
+                new_row.append(rx_match.expand(cell_tmpl))
+        else:
+            # Should never happen.
+            raise RuntimeError(f"{_RX_ANYTHING} failed to match {to_match!r}")
+
+        new_row.extend(following)
+        yield new_row
+
+
+def _join_columns(
+    cfg: cfgextract.JoinColumns,
+    rows: Iterable[_Row],
+) -> Iterator[_Row]:
+    delim = cfg.delim
+    from_, to = cfg.from_, cfg.to
+    for row in rows:
+        out_row = []
+
+        if from_ is not None:
+            out_row.extend(row[:from_])
+
+        if to_join := row[from_:to]:
+            out_row.append(delim.join(to_join))
+
+        if to is not None:
+            out_row.extend(row[to:])
+
+        yield out_row
+
+
+def _prepend_row(cfg: cfgextract.PrependRow, rows: Iterable[_Row]) -> Iterator[_Row]:
+    """Implements the config.PrependRow transformation."""
+    return itertools.chain([cfg.row], rows)
 
 
 class _LineGrouper(Protocol):
 
-    def group_lines(self, lines: Iterable[_Line]) -> Iterator[_LineGroup]:
+    def __call__(self, lines: Iterable[_Row]) -> Iterator[_RowGroup]:
         """Group input rows into groups, according to the implementation.
 
         :param lines: Input rows.
         :yield: Row groups.
         """
         raise NotImplementedError
 
 
-class _StaticRowLengths(_LineGrouper):
-    _line_counts: list[int]
-
-    def __init__(self, cfg: config.StaticRowCounts) -> None:
-        self._line_counts = list(cfg.row_counts)
+def _all_rows(lines: Iterable[_Row]) -> Iterator[_RowGroup]:
+    yield list(lines)
 
-    def group_lines(self, lines: Iterable[_Line]) -> Iterator[_LineGroup]:
-        for num_lines in self._line_counts:
-            yield list(itertools.islice(lines, num_lines))
 
+def _static_row_lengths(
+    cfg: cfgextract.StaticRowCounts, lines: Iterable[_Row]
+) -> Iterator[_RowGroup]:
+    for num_lines in cfg.row_counts:
+        yield list(itertools.islice(lines, num_lines))
+
+
+def _empty_column(cfg: cfgextract.EmptyColumn, lines: Iterable[_Row]) -> Iterator[_RowGroup]:
+    group: _RowGroup = []
+    for line in lines:
+        if line[cfg.column_index] == "":
+            group.append(line)
+        else:
+            if group:
+                yield group
+            group = [line]
+    if group:
+        yield group
 
-class _EmptyColumn(_LineGrouper):
-    _column_index: int
 
-    def __init__(self, cfg: config.EmptyColumn) -> None:
-        self._column_index = cfg.column_index
-
-    def group_lines(self, lines: Iterable[_Line]) -> Iterator[_LineGroup]:
-        group: _LineGroup = []
-        for line in lines:
-            if line[self._column_index] == "":
-                group.append(line)
-            else:
-                if group:
-                    yield group
-                group = [line]
-        if group:
-            yield group
-
-
-def _make_line_grouper(cfg: config.RowFolder) -> _LineGrouper:
+def _make_line_grouper(cfg: cfgextract.RowGrouper) -> _LineGrouper:
     match cfg:
-        case config.StaticRowCounts():
-            return _StaticRowLengths(cfg)
-        case config.EmptyColumn():
-            return _EmptyColumn(cfg)
+        case cfgextract.AllRows():
+            return _all_rows
+        case cfgextract.StaticRowCounts():
+            return functools.partial(_static_row_lengths, cfg)
+        case cfgextract.EmptyColumn():
+            return functools.partial(_empty_column, cfg)
         case _:
-            raise ConfigurationError(f"{type(cfg).__name__} is an unknown type of row folder")
-
-
-class _MultiGrouper(_LineGrouper):
-    _groupers: list[_LineGrouper]
+            raise ConfigurationError(
+                f"{type(cfg).__name__} is an unknown type of row folder",
+            )
 
-    def __init__(self, groupers: list[_LineGrouper]) -> None:
-        self._groupers = groupers
 
-    def group_lines(self, lines: Iterable[_Line]) -> Iterator[_LineGroup]:
-        for grouper in self._groupers:
-            yield from grouper.group_lines(lines)
-        # Everything remaining is in individual groups.
-        for line in lines:
-            yield [line]
+def _multi_grouper(groupers: list[_LineGrouper], lines: Iterable[_Row]) -> Iterator[_RowGroup]:
+    for grouper in groupers:
+        yield from grouper(lines)
+    # Everything remaining is in individual groups.
+    for line in lines:
+        yield [line]
 
 
 def _fold_rows(
-    lines: Iterable[_Line],
-    grouper: _LineGrouper,
+    cfg: cfgextract.FoldRows,
+    rows: Iterable[_Row],
 ) -> Iterator[_Row]:
-    for line_group in grouper.group_lines(lines):
+    """Implements the config.FoldRows transformation."""
+
+    grouper = _multi_grouper([_make_line_grouper(folder) for folder in cfg.group_by], rows)
+
+    for line_group in grouper:
         # List of cell texts, each of which contain the sequence of strings that
         # make up the resulting row's cells. The following is essentially a
         # transpose operation.
         row_accum: list[list[str]] = []
         for line in line_group:
             missing_count = len(line) - len(row_accum)
             if missing_count > 0:
@@ -164,112 +235,52 @@
                 if text:
                     acc.append(text)
 
         row: _Row = [" ".join(cell) for cell in row_accum]
         yield row
 
 
-def _clean_rows(rows: Iterable[list[str]]) -> Iterator[list[str]]:
-    for row in rows:
-        yield [parseutil.clean_text(text) for text in row]
-
-
-@dataclasses.dataclass
-class Progress:
-    """Progress report from ``extract_book``."""
-
-    completed: int
-    total: int
-
-
-@dataclasses.dataclass
-class ExtractionConfig:
-    """Extraction configuration.
-
-    :field config_dir: Path to top level directory of configuration.
-    :field output_dir: Path to top level directory for output.
-    :field input_pdf: Path to PDF file to extract from.
-    :field book_cfg: Configuration for book to extract tables from.
-    :field overwrite_existing: If true, overwrite existing CSV files.
-    """
-
-    config_dir: pathlib.Path
-    output_dir: pathlib.Path
-    input_pdf: pathlib.Path
-    book_cfg: config.Book
-    overwrite_existing: bool
-
-
-@dataclasses.dataclass
-class ExtractEvents:
-    """Extraction event callbacks.
-
-    :field on_progress: Called at the start and after each extraction attempt.
-    :field on_error: Called on any errors.
-    :field do_continue: Called at intervals. If it returns False, then no
-    further processing is attempted.
-    """
-
-    on_progress: Callable[[Progress], None]
-    on_error: Callable[[str], None]
-    do_continue: Callable[[], bool]
-
-
-def extract_book(
-    *,
-    table_reader: TableReader,
-    cfg: ExtractionConfig,
-    events: ExtractEvents,
-) -> None:
-    """Extracts an entire book to CSV.
-
-    :param table_reader: Extractor for individual tables from a PDF.
-    :param cfg: Configuration for extraction.
-    :param events: Event hooks to feed back progress, etc.
-    :raises RuntimeError: If ``cfg.book_cfg.group`` was not set.
-    """
-
-    if cfg.book_cfg.group is None:
-        raise RuntimeError("Book.group was not set")
-
-    output_tables: list[tuple[pathlib.Path, config.Table]] = []
-    for table in cfg.book_cfg.group.all_tables():
-        if table.extraction is None:
-            continue
-        out_filepath = cfg.output_dir / table.file_stem.with_suffix(".csv")
-
-        if cfg.overwrite_existing or not out_filepath.exists():
-            output_tables.append((out_filepath, table))
-
-    events.on_progress(Progress(0, len(output_tables)))
-
-    created_directories: set[pathlib.Path] = set()
-    for i, (out_filepath, table) in enumerate(output_tables, start=1):
-        if not events.do_continue():
-            return
+def _transpose(
+    rows: Iterable[_Row],
+) -> Iterator[_Row]:
+    orig_rows = list(rows)
+    orig_num_cols = max(len(row) for row in orig_rows)
+    orig_num_rows = len(orig_rows)
+
+    for i in range(orig_num_cols):
+        row: _Row = []
+        for j in range(orig_num_rows):
+            try:
+                cell = orig_rows[j][i]
+            except IndexError:
+                cell = ""
+            row.append(cell)
+        yield row
 
-        if table.extraction is None:
-            continue
-        extraction = table.extraction
 
-        out_filepath = cast(pathlib.Path, out_filepath)
-        table = cast(config.Table, table)
+def _wrap_row_every_n(
+    cfg: cfgextract.WrapRowEveryN,
+    rows: Iterable[_Row],
+) -> Iterator[_Row]:
+    if cfg.columns < 1:
+        raise ConfigurationError(f"{cfg.yaml_tag}.columns must be at least 1, but is {cfg.columns}")
+    accum: _Row = []
+    for row in rows:
+        for cell in row:
+            accum.append(cell)
+            l = len(accum)
+            if l == cfg.columns:
+                yield accum
+                accum = []
+            elif l < cfg.columns:
+                continue
+            else:
+                raise RuntimeError(
+                    f"too many items {l} in accumulated row versus maximum" f" of {cfg.columns}"
+                )
+    if accum:
+        yield accum
 
-        group_dir = out_filepath.parent
-        if group_dir not in created_directories:
-            group_dir.mkdir(parents=True, exist_ok=True)
-            created_directories.add(group_dir)
 
-        try:
-            rows = extract_table(
-                config_dir=cfg.config_dir,
-                pdf_path=cfg.input_pdf,
-                file_stem=table.file_stem,
-                extraction=extraction,
-                table_reader=table_reader,
-            )
-            with csvutil.open_write(out_filepath) as f:
-                csv.writer(f).writerows(rows)
-        except ConfigurationError as exc:
-            events.on_error(f"Configuration error while processing table {table.file_stem}: {exc}")
-        finally:
-            events.on_progress(Progress(i, len(output_tables)))
+def _clean_rows(rows: Iterable[list[str]]) -> Iterator[list[str]]:
+    for row in rows:
+        yield [parseutil.clean_text(text) for text in row]
```

### Comparing `travdata-0.3.2/src/travdata/extraction/tabulautil.py` & `travdata-0.4.0/src/travdata/extraction/tabulautil.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 """Utility wrapper for tabular-py."""
 
 import json
 import pathlib
-from typing import Iterable, Iterator, TypeAlias, TypedDict, cast
+import tempfile
+from typing import IO, Iterable, Iterator, TypeAlias, TypedDict, cast
 
 import jpype  # type: ignore[import-untyped]
 import tabula
 
 
 class TabulaCell(TypedDict):
     """Type of table cells emitted by tabula-py."""
@@ -56,14 +57,25 @@
         :param force_subprocess: Should Tabula be run as a child process, versus
         using the faster jpype.
         """
         self._force_subprocess = force_subprocess
         self._needs_shutdown = False
 
     def __enter__(self) -> "TabulaClient":
+        # Hack to get tabula initialised from the main thread, otherwise the
+        # application may not quit when multi-threaded (such as in a GUI).
+        with tempfile.NamedTemporaryFile() as tmpfile:
+            tmpfile.write(b"dummy data")
+            tmpfile.flush()
+            try:
+                _ = self._read_pdf(input_path=tmpfile.name, pages=[1])
+            except Exception:  # pylint: disable=broad-exception-caught
+                # Expected failure due to dummy file not being a real PDF.
+                pass
+
         return self
 
     def __exit__(self, *args) -> None:
         del args  # unused
         self.shutdown()
 
     def shutdown(self) -> None:
@@ -76,50 +88,56 @@
             jpype.shutdownJVM()
             self._needs_shutdown = False
 
     def read_pdf_with_template(
         self,
         *,
         pdf_path: pathlib.Path,
-        template_path: pathlib.Path,
+        template_file: IO[str],
     ) -> list[TabulaTable]:
         """Reads table(s) from a PDF, based on the Tabula template.
 
         :param pdf_path: Path to PDF to read from.
-        :param template_path: Path to the Tabula template JSON file.
+        :param template_file: File-like reader for the Tabula template JSON
+        file.
         :return: Tables read from the PDF.
         """
         self._needs_shutdown = not self._force_subprocess
 
         result: list[TabulaTable] = []
-        with template_path.open() as tf:
-            template = cast(list[_TemplateEntry], json.load(tf))
+        template = cast(list[_TemplateEntry], json.load(template_file))
 
         for entry in template:
             method = entry["extraction_method"]
             result.extend(
                 cast(
                     list[TabulaTable],
-                    tabula.read_pdf(  # pyright: ignore[reportPrivateImportUsage]
-                        pdf_path,
+                    self._read_pdf(
+                        input_path=pdf_path,
                         pages=[entry["page"]],
-                        java_options=["-Djava.awt.headless=true"],
                         multiple_tables=True,
-                        output_format="json",
                         area=[entry["y1"], entry["x1"], entry["y2"], entry["x2"]],
                         force_subprocess=self._force_subprocess,
                         stream=method == "stream",
                         guess=method == "guess",
                         lattice=method == "lattice",
                     ),
                 )
             )
 
         return result
 
+    def _read_pdf(self, **kwargs) -> list[TabulaTable]:
+        return cast(
+            list[TabulaTable],
+            tabula.read_pdf(  # pyright: ignore[reportPrivateImportUsage]
+                java_options=["-Djava.awt.headless=true"], output_format="json", **kwargs
+            ),
+        )
+
 
 def table_rows_concat(tables: Iterable[TabulaTable]) -> Iterator[TabulaRow]:
     """Concatenates rows from multiple Tabula tables into a single row iterator.
 
     :param tables: Tables to concatenate rows from.
     :yield: Rows from the tables.
     """
```

### Comparing `travdata-0.3.2/src/travdata/gui/extraction/runnerwin.py` & `travdata-0.4.0/src/travdata/gui/extraction/runnerwin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,81 @@
 # -*- coding: utf-8 -*-
 """Defines a window that monitors and manages extraction from a PDF."""
 
 # Pylint doesn't like QT much.
 # pylint: disable=I1101
 
+import pathlib
+import traceback
 from typing import Optional
 
 from PySide6 import QtCore, QtWidgets
 
-from travdata import config
-from travdata.extraction import pdfextract
+from travdata.extraction import bookextract, tableextract
 from travdata.gui import qtutil
 
 
 class _WorkerSignals(QtCore.QObject):
-    progress = QtCore.Signal(pdfextract.Progress)
+    progress = QtCore.Signal(bookextract.Progress)
+    output = QtCore.Signal(pathlib.PurePath)
     error = QtCore.Signal(str)
     stopped = QtCore.Signal()
     finished = QtCore.Signal()
 
 
 class _Worker(QtCore.QRunnable):
 
     def __init__(
         self,
-        cfg: pdfextract.ExtractionConfig,
-        table_reader: pdfextract.TableReader,
+        ext_cfg: bookextract.ExtractionConfig,
+        table_reader: tableextract.TableReader,
     ) -> None:
         super().__init__()
         self.signals = _WorkerSignals()
-        self._cfg = cfg
+        self._ext_cfg = ext_cfg
         self._table_reader = table_reader
         self._continue = True
 
     def stop(self) -> None:
         """Stops extraction as soon as possible."""
         self._continue = False
 
     @QtCore.Slot()
     def run(self) -> None:
         """Runs the extraction."""
         try:
-            if self._cfg.book_cfg.group is None:
-                cfg = config.load_config(self._cfg.config_dir, [self._cfg.book_cfg.id_])
-                self._cfg.book_cfg = cfg.books[self._cfg.book_cfg.id_]
-
-            pdfextract.extract_book(
+            bookextract.extract_book(
                 table_reader=self._table_reader,
-                cfg=self._cfg,
-                events=pdfextract.ExtractEvents(
+                ext_cfg=self._ext_cfg,
+                events=bookextract.ExtractEvents(
                     on_error=self.signals.error.emit,
+                    on_output=self.signals.output.emit,
                     on_progress=self.signals.progress.emit,
                     do_continue=lambda: self._continue,
                 ),
             )
-        except Exception as exc:  # pylint: disable=broad-exception-caught
-            self.signals.error.emit(str(exc))
+        except Exception:  # pylint: disable=broad-exception-caught
+            self.signals.error.emit(traceback.format_exc())
             self.signals.stopped.emit()
         else:
             self.signals.finished.emit()
 
 
 class ExtractionRunnerWindow(QtWidgets.QWidget):
     """Window to manage extraction from PDF."""
 
     closing = QtCore.Signal()
 
     _worker: Optional[_Worker]
 
     def __init__(
         self,
-        cfg: pdfextract.ExtractionConfig,
+        cfg: bookextract.ExtractionConfig,
         thread_pool: QtCore.QThreadPool,
-        table_reader: pdfextract.TableReader,
+        table_reader: tableextract.TableReader,
         *args,
         **kwargs,
     ) -> None:
         super().__init__(*args, **kwargs)
         self.setWindowTitle("Travdata Extraction")
 
         self._worker = None
@@ -105,14 +104,15 @@
         layout.addWidget(contents)
         self.setLayout(layout)
 
     def start_extraction(self) -> None:
         """Starts the extraction."""
         self._worker = _Worker(self._cfg, self._table_reader)
         self._worker.signals.progress.connect(self._progress)
+        self._worker.signals.output.connect(self._on_output)
         self._worker.signals.error.connect(self._error)
         self._worker.signals.finished.connect(self._finished)
         self._worker.signals.stopped.connect(self._stopped)
         self._thread_pool.start(self._worker)
 
     def stop_extraction(self) -> None:
         """Stops the extraction as soon as possible."""
@@ -130,22 +130,26 @@
 
     @QtCore.Slot()
     def _cancel(self) -> None:
         self._output_text_area.appendPlainText("Cancelling...")
         self.stop_extraction()
 
     @QtCore.Slot()
-    def _progress(self, progress: pdfextract.Progress) -> None:
+    def _progress(self, progress: bookextract.Progress) -> None:
         if progress.total != self._progress_bar.maximum():
             self._progress_bar.setMaximum(progress.total)
         self._progress_bar.setValue(progress.completed)
 
     @QtCore.Slot()
+    def _on_output(self, path: pathlib.PurePath) -> None:
+        self._output_text_area.appendPlainText(f"Output {path}")
+
+    @QtCore.Slot()
     def _error(self, error: str) -> None:
-        self._output_text_area.appendPlainText(error + "\n")
+        self._output_text_area.appendPlainText(error)
 
     @QtCore.Slot()
     def _finished(self) -> None:
         self._output_text_area.appendPlainText("Complete.")
         self._cancel_button.setEnabled(False)
 
     @QtCore.Slot()
```

### Comparing `travdata-0.3.2/src/travdata/gui/gui.py` & `travdata-0.4.0/src/travdata/gui/gui.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 
     with tabulautil.TabulaClient(
         force_subprocess=False,
     ) as tabula_client:
         window = cfgwin.ExtractionConfigWindow(
             thread_pool=QtCore.QThreadPool(),
             table_reader=tabula_client,
-            config_dir=config.get_default_config_path(),
+            default_config_path=config.get_default_config_path(),
         )
+
         window.show()
         sys.exit(app.exec())
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `travdata-0.3.2/src/travdata/tableconverters/core/registry.py` & `travdata-0.4.0/src/travdata/tableconverters/core/registry.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.2/src/travdata/tableconverters/core/trade.py` & `travdata-0.4.0/src/travdata/tableconverters/core/trade.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.2/src/travdata/tableconverters/core/worldcreation.py` & `travdata-0.4.0/src/travdata/tableconverters/core/worldcreation.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.2/src/travdata/tableconverters/registry.py` & `travdata-0.4.0/src/travdata/tableconverters/registry.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.2/src/travdata/travellermap/apiurls.py` & `travdata-0.4.0/src/travdata/travellermap/apiurls.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.2/src/travdata/travellermap/sectorparse.py` & `travdata-0.4.0/src/travdata/travellermap/sectorparse.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.2/src/travdata/travellermap/world.py` & `travdata-0.4.0/src/travdata/travellermap/world.py`

 * *Files identical despite different names*

### Comparing `travdata-0.3.2/PKG-INFO` & `travdata-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: travdata
-Version: 0.3.2
+Version: 0.4.0
 Summary: Data utility code for Mongoose Traveller TTRPG.
 Home-page: https://github.com/huin/travdata
 License: MIT
 Keywords: traveller,ttrpg
 Author: John Beisley
 Author-email: johnbeisleyuk@gmail.com
 Requires-Python: >=3.11,<4.0
```

