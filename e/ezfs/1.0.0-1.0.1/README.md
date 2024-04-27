# Comparing `tmp/ezfs-1.0.0.tar.gz` & `tmp/ezfs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezfs-1.0.0.tar", last modified: Sun Apr 21 21:44:33 2024, max compression
+gzip compressed data, was "ezfs-1.0.1.tar", last modified: Sat Apr 27 18:12:15 2024, max compression
```

## Comparing `ezfs-1.0.0.tar` & `ezfs-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2024-04-21 21:44:33.052657 ezfs-1.0.0/
--rw-r--r--   0 dfritz     (502) staff       (20)     1068 2024-04-15 03:05:45.000000 ezfs-1.0.0/LICENSE
--rw-r--r--   0 dfritz     (502) staff       (20)       34 2024-04-19 22:50:42.000000 ezfs-1.0.0/MANIFEST.in
--rw-r--r--   0 dfritz     (502) staff       (20)    10391 2024-04-21 21:44:33.052294 ezfs-1.0.0/PKG-INFO
--rw-r--r--   0 dfritz     (502) staff       (20)     9010 2024-04-21 20:53:46.000000 ezfs-1.0.0/README.md
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2024-04-21 21:44:33.051767 ezfs-1.0.0/ezfs.egg-info/
--rw-r--r--   0 dfritz     (502) staff       (20)    10391 2024-04-21 21:44:33.000000 ezfs-1.0.0/ezfs.egg-info/PKG-INFO
--rw-r--r--   0 dfritz     (502) staff       (20)      191 2024-04-21 21:44:33.000000 ezfs-1.0.0/ezfs.egg-info/SOURCES.txt
--rw-r--r--   0 dfritz     (502) staff       (20)        1 2024-04-21 21:44:33.000000 ezfs-1.0.0/ezfs.egg-info/dependency_links.txt
--rw-r--r--   0 dfritz     (502) staff       (20)       41 2024-04-21 21:44:33.000000 ezfs-1.0.0/ezfs.egg-info/requires.txt
--rw-r--r--   0 dfritz     (502) staff       (20)        5 2024-04-21 21:44:33.000000 ezfs-1.0.0/ezfs.egg-info/top_level.txt
--rw-r--r--   0 dfritz     (502) staff       (20)    21453 2024-04-21 21:41:43.000000 ezfs-1.0.0/ezfs.py
--rw-r--r--   0 dfritz     (502) staff       (20)     5278 2024-04-21 21:22:33.000000 ezfs-1.0.0/pyproject.toml
--rw-r--r--   0 dfritz     (502) staff       (20)       38 2024-04-21 21:44:33.052703 ezfs-1.0.0/setup.cfg
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2024-04-27 18:12:15.193072 ezfs-1.0.1/
+-rw-r--r--   0 dfritz     (502) staff       (20)     1068 2024-04-27 18:07:45.000000 ezfs-1.0.1/LICENSE
+-rw-r--r--   0 dfritz     (502) staff       (20)       34 2024-04-19 22:50:42.000000 ezfs-1.0.1/MANIFEST.in
+-rw-r--r--   0 dfritz     (502) staff       (20)    10730 2024-04-27 18:12:15.192464 ezfs-1.0.1/PKG-INFO
+-rw-r--r--   0 dfritz     (502) staff       (20)     9153 2024-04-27 18:07:45.000000 ezfs-1.0.1/README.md
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2024-04-27 18:12:15.191271 ezfs-1.0.1/ezfs.egg-info/
+-rw-r--r--   0 dfritz     (502) staff       (20)    10730 2024-04-27 18:12:15.000000 ezfs-1.0.1/ezfs.egg-info/PKG-INFO
+-rw-r--r--   0 dfritz     (502) staff       (20)      191 2024-04-27 18:12:15.000000 ezfs-1.0.1/ezfs.egg-info/SOURCES.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)        1 2024-04-27 18:12:15.000000 ezfs-1.0.1/ezfs.egg-info/dependency_links.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)       97 2024-04-27 18:12:15.000000 ezfs-1.0.1/ezfs.egg-info/requires.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)        5 2024-04-27 18:12:15.000000 ezfs-1.0.1/ezfs.egg-info/top_level.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)    27624 2024-04-27 18:07:45.000000 ezfs-1.0.1/ezfs.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     5343 2024-04-27 18:07:45.000000 ezfs-1.0.1/pyproject.toml
+-rw-r--r--   0 dfritz     (502) staff       (20)       38 2024-04-27 18:12:15.193142 ezfs-1.0.1/setup.cfg
```

### Comparing `ezfs-1.0.0/LICENSE` & `ezfs-1.0.1/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 David Fritz
+Copyright (c) 2024 David Fritz
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ezfs-1.0.0/PKG-INFO` & `ezfs-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezfs
-Version: 1.0.0
+Version: 1.0.1
 Summary: Minimalistic virtual filesystem adapters for Python
 Author: David Fritz
 License: MIT
 Project-URL: Home, https://github.com/pyranha-labs/ezfs
 Project-URL: Changelog, https://github.com/pyranha-labs/ezfs/releases
 Project-URL: Issues, https://github.com/pyranha-labs/ezfs/issues
 Keywords: filesystem,s3,compression
@@ -25,20 +25,26 @@
 Classifier: Typing :: Typed
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: blosc
+Requires-Dist: blosc; extra == "blosc"
+Provides-Extra: brotli
+Requires-Dist: brotli; extra == "brotli"
 Provides-Extra: s3
 Requires-Dist: boto3; extra == "s3"
-Provides-Extra: zstd
-Requires-Dist: zstandard; extra == "zstd"
 Provides-Extra: lz4
 Requires-Dist: lz4; extra == "lz4"
+Provides-Extra: snappy
+Requires-Dist: python-snappy; extra == "snappy"
+Provides-Extra: zstd
+Requires-Dist: zstandard; extra == "zstd"
 
 
 [![os: windows mac linux](https://img.shields.io/badge/os-linux_|_macos_|_windows-blue)](https://docs.python.org/3.10/)
 [![python: 3.10+](https://img.shields.io/badge/python-3.10_|_3.11_|_3.12-blue)](https://devguide.python.org/versions)
 [![python style: google](https://img.shields.io/badge/python%20style-google-blue)](https://google.github.io/styleguide/pyguide.html)
 [![imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://github.com/PyCQA/isort)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -76,17 +82,21 @@
     * [Optimized Remote Filesystem Example](#optimized-remote-filesystem-example)
   * [Contributing](#contributing)
 
 
 ## Compatibility
 
 - Supports Python 3.10+
-- Supports `gzip`, `zstd`, and `lz4` compression types (when installed separately)
-- Supports `S3` storage (when installed separately)
-- Theoretically any compression type, or backend storage type, by extending `File`, `Filesystem`, and `Compressor`
+- Supports multiple compression types
+  - `bz2`, `gzip`, `lzma` (when built into Python)
+  - `blosc`, `brotli`, `lz4`, `snappy`, and `zstd` (when installed separately)
+- Support multiple storage types
+  - `sqlite3` (when built into Python)
+  - `S3` (when installed separately)
+- Theoretically any compression type, or backend storage type, by extending `Compressor`, `File`, and `Filesystem` 
 
 
 ## Getting Started
 
 ### Installation
 
 Install EZFS via pip:
```

### Comparing `ezfs-1.0.0/README.md` & `ezfs-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -38,17 +38,21 @@
     * [Optimized Remote Filesystem Example](#optimized-remote-filesystem-example)
   * [Contributing](#contributing)
 
 
 ## Compatibility
 
 - Supports Python 3.10+
-- Supports `gzip`, `zstd`, and `lz4` compression types (when installed separately)
-- Supports `S3` storage (when installed separately)
-- Theoretically any compression type, or backend storage type, by extending `File`, `Filesystem`, and `Compressor`
+- Supports multiple compression types
+  - `bz2`, `gzip`, `lzma` (when built into Python)
+  - `blosc`, `brotli`, `lz4`, `snappy`, and `zstd` (when installed separately)
+- Support multiple storage types
+  - `sqlite3` (when built into Python)
+  - `S3` (when installed separately)
+- Theoretically any compression type, or backend storage type, by extending `Compressor`, `File`, and `Filesystem` 
 
 
 ## Getting Started
 
 ### Installation
 
 Install EZFS via pip:
```

### Comparing `ezfs-1.0.0/ezfs.egg-info/PKG-INFO` & `ezfs-1.0.1/ezfs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezfs
-Version: 1.0.0
+Version: 1.0.1
 Summary: Minimalistic virtual filesystem adapters for Python
 Author: David Fritz
 License: MIT
 Project-URL: Home, https://github.com/pyranha-labs/ezfs
 Project-URL: Changelog, https://github.com/pyranha-labs/ezfs/releases
 Project-URL: Issues, https://github.com/pyranha-labs/ezfs/issues
 Keywords: filesystem,s3,compression
@@ -25,20 +25,26 @@
 Classifier: Typing :: Typed
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: blosc
+Requires-Dist: blosc; extra == "blosc"
+Provides-Extra: brotli
+Requires-Dist: brotli; extra == "brotli"
 Provides-Extra: s3
 Requires-Dist: boto3; extra == "s3"
-Provides-Extra: zstd
-Requires-Dist: zstandard; extra == "zstd"
 Provides-Extra: lz4
 Requires-Dist: lz4; extra == "lz4"
+Provides-Extra: snappy
+Requires-Dist: python-snappy; extra == "snappy"
+Provides-Extra: zstd
+Requires-Dist: zstandard; extra == "zstd"
 
 
 [![os: windows mac linux](https://img.shields.io/badge/os-linux_|_macos_|_windows-blue)](https://docs.python.org/3.10/)
 [![python: 3.10+](https://img.shields.io/badge/python-3.10_|_3.11_|_3.12-blue)](https://devguide.python.org/versions)
 [![python style: google](https://img.shields.io/badge/python%20style-google-blue)](https://google.github.io/styleguide/pyguide.html)
 [![imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://github.com/PyCQA/isort)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -76,17 +82,21 @@
     * [Optimized Remote Filesystem Example](#optimized-remote-filesystem-example)
   * [Contributing](#contributing)
 
 
 ## Compatibility
 
 - Supports Python 3.10+
-- Supports `gzip`, `zstd`, and `lz4` compression types (when installed separately)
-- Supports `S3` storage (when installed separately)
-- Theoretically any compression type, or backend storage type, by extending `File`, `Filesystem`, and `Compressor`
+- Supports multiple compression types
+  - `bz2`, `gzip`, `lzma` (when built into Python)
+  - `blosc`, `brotli`, `lz4`, `snappy`, and `zstd` (when installed separately)
+- Support multiple storage types
+  - `sqlite3` (when built into Python)
+  - `S3` (when installed separately)
+- Theoretically any compression type, or backend storage type, by extending `Compressor`, `File`, and `Filesystem` 
 
 
 ## Getting Started
 
 ### Installation
 
 Install EZFS via pip:
```

### Comparing `ezfs-1.0.0/ezfs.py` & `ezfs-1.0.1/ezfs.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,38 +12,53 @@
 No additional functionality is guaranteed by File objects in order to maintain
 simplicity and consistency across all forms of storage.
 
 Includes the following basic adapters that can used directly, or as examples for more complex implementations:
 - Local storage
 - In-memory storage
 - Remote storage (S3)
+- Database storage (SQLite)
 """
 
 from __future__ import annotations
 
 import abc
 import os
+import re
+import typing
 from contextlib import contextmanager
 from io import UnsupportedOperation
 from types import ModuleType
 from typing import Callable
+from typing import Iterable
 
 try:
     from typing import override  # pylint: disable=ungrouped-imports
 except ImportError:
     try:
         from typing_extensions import override
     except ModuleNotFoundError:
 
         def override(func: Callable) -> Callable:
             """Passthrough decorator for environments where typing is not enabled."""
             return func
 
 
-__version__ = "1.0.0"
+if typing.TYPE_CHECKING:
+    try:
+        import sqlite3
+    except ModuleNotFoundError:
+
+        class sqlite3:  # pylint: disable=invalid-name
+            """Placeholder module for typing."""
+
+            Cursor = None
+
+
+__version__ = "1.0.1"
 # Compressors may either be a module, or subclass of Compressor,
 # with `compress()` and `decompress()` functions.
 __COMPRESSORS__: dict[str, Compressor | ModuleType | None] = {
     None: None,
     "none": None,
 }
 __COMPRESSOR_SETUP_COMPLETE__ = False
@@ -543,34 +558,194 @@
         self.client = self._session.client("s3")
 
     @override
     def _get_file(self, file: str, mode: str, encoding: str, compression: str) -> File:
         return S3BotoFile(self, file, mode=mode, encoding=encoding, compression=compression)
 
 
+class SQLiteFile(File):
+    """File-like object in a SQLite database."""
+
+    def __init__(
+        self,
+        filesystem: SQLiteFilesystem,
+        file: str,
+        mode: str = "rt",
+        encoding: str = "utf-8",
+        compression: str = NO_COMPRESSION,
+    ) -> None:
+        """Initialize the base attributes of the file-like database object for read and write operations.
+
+        Args:
+            filesystem: Original filesystem used to create the File.
+            file: Location of the object in the database table.
+            mode: Options used to open the file.
+            encoding: Name of the encoding used to decode or encode the file when in text mode.
+            compression: Type of compression used when reading or writing the file contents.
+        """
+        super().__init__(filesystem, file, mode=mode, encoding=encoding, compression=compression)
+        self.filesystem: SQLiteFilesystem = filesystem  # Set again with typehint to avoid lint warnings.
+
+    @override
+    def __repr__(self) -> str:
+        return f"sqlite3://{self.filesystem.database}?table_name={self.filesystem.table_name}&file={self.file}"
+
+    @override
+    def close(self) -> None:
+        # No action required for database files.
+        pass
+
+    @override
+    def _read(self) -> bytes | str:
+        res = self.filesystem.execute(self.filesystem.read_query, (self.file,)).fetchone()
+        if res is None:
+            raise FileNotFoundError(2, f"No such file: '{self.file}'")
+        content = res[0]
+        return content
+
+    @override
+    def _write(self, data: bytes | str) -> int:
+        self.filesystem.execute(self.filesystem.write_query, (self.file, data, data))
+        self.filesystem.commit()
+        return len(data)
+
+
+class SQLiteFilesystem(Filesystem):
+    """Collection of file-like objects available in a database using SQLite."""
+
+    def __init__(
+        self,
+        database: str,
+        table_name: str = "files",
+        file_col: str = "file",
+        content_col: str = "content",
+        compression: str = NO_COMPRESSION,
+    ) -> None:
+        """Initialize the base attributes of the database filesystem for read and write operations.
+
+        Args:
+            database: The path to the database file to be opened. e.g., "example.db", ":memory:", etc.
+            table_name: Name of the table with data available as files in the filesystem.
+            file_col: Name of the column in the table that contains the path to the files.
+            content_col: Name of the column in the table that contains the raw contents for the files.
+            compression: Default compression type to use when reading or writing file contents.
+                Use basic string name to load from default compressor cache.
+        """
+        for name, value in (
+            ("table_name", table_name),
+            ("file_col", file_col),
+            ("content_col", content_col),
+        ):
+            if not re.match(r"^[A-za-z0-9_]+$", value):
+                raise ValueError(f"{name} may only contain letters, numbers, and underscores.")
+        super().__init__(compression=compression)
+        try:
+            # pylint: disable=import-outside-toplevel,redefined-outer-name,reimported
+            import sqlite3
+
+        except ModuleNotFoundError as error:
+            raise ModuleNotFoundError(f"sqlite3 is required to use {self.__class__.__name__}") from error
+
+        # Save the database and table name to allow string representations in files,
+        # but cache the templates to prevent modifications from impacting later execution.
+        self.database = database
+        self.table_name = table_name  # Save the table name to allow
+        self._connection = sqlite3.connect(database)
+        self._cursor = self._connection.cursor()
+
+        # Cache the query strings to reduce overhead.
+        # "nosec" added due to validation before this point.
+        self._create_query = f"CREATE TABLE {table_name}({file_col} TEXT(255) PRIMARY KEY, {content_col} BLOB)"  # nosec
+        self.read_query = f"SELECT {content_col} FROM {table_name} WHERE {file_col} = (?) LIMIT 1"  # nosec
+        self.write_query = (
+            f"INSERT INTO {table_name}({file_col}, {content_col}) VALUES(?, ?) "  # nosec
+            f"ON CONFLICT({file_col}) DO UPDATE SET {content_col}=?;"
+        )
+
+    def commit(self) -> None:
+        """Commit any pending transactions to the database backend."""
+        self._connection.commit()
+
+    def create_table(self) -> None:
+        """Create a basic table to use for storage."""
+        self.execute(self._create_query)
+
+    def execute(self, sql: str, params: Iterable | dict = ()) -> sqlite3.Cursor:
+        """Execute a SQL statement against the backend storage table.
+
+        Args:
+            sql: A single SQL statement.
+            params: Iterable of values to bind to placeholders in sql, or dict if named placeholders are used.
+
+        Returns:
+            The cursor used to execute the statement, allowing caller to fetch results.
+        """
+        return self._cursor.execute(sql, params)
+
+    @override
+    def _get_file(self, file: str, mode: str, encoding: str, compression: str) -> SQLiteFile:
+        return SQLiteFile(self, file, mode=mode, encoding=encoding, compression=compression)
+
+
 def init_compressors() -> list[str]:
     """Search the system for available compression algorithms.
 
     Returns:
         List of the available compression types for reading and writing files.
     """
     global __COMPRESSOR_SETUP_COMPLETE__  # pylint: disable=global-statement
     __COMPRESSOR_SETUP_COMPLETE__ = True
+
+    # pylint: disable=import-outside-toplevel
+    # Builtin compression modules.
+    try:
+        import bz2
+
+        __COMPRESSORS__["bz2"] = bz2
+    except ModuleNotFoundError:
+        pass
     try:
-        import gzip  # pylint: disable=import-outside-toplevel
+        import gzip
 
         __COMPRESSORS__["gzip"] = gzip
     except ModuleNotFoundError:
         pass
     try:
-        import zstandard  # pylint: disable=import-outside-toplevel
+        import lzma
 
-        __COMPRESSORS__["zstd"] = zstandard
+        __COMPRESSORS__["lzma"] = lzma
+    except ModuleNotFoundError:
+        pass
+
+    # Third-party compression modules.
+    try:
+        import blosc
+
+        __COMPRESSORS__["blosc"] = blosc
     except ModuleNotFoundError:
         pass
     try:
-        import lz4.frame  # pylint: disable=import-outside-toplevel
+        import brotli
+
+        __COMPRESSORS__["brotli"] = brotli
+    except ModuleNotFoundError:
+        pass
+    try:
+        import lz4.frame
 
         __COMPRESSORS__["lz4"] = lz4.frame
     except ModuleNotFoundError:
         pass
-    return list(set(str(key).lower() for key in __COMPRESSORS__))
+    try:
+        import snappy
+
+        __COMPRESSORS__["snappy"] = snappy
+    except ModuleNotFoundError:
+        pass
+    try:
+        import zstandard
+
+        __COMPRESSORS__["zstd"] = zstandard
+    except ModuleNotFoundError:
+        pass
+
+    return sorted(set(str(key).lower() for key in __COMPRESSORS__))
```

### Comparing `ezfs-1.0.0/pyproject.toml` & `ezfs-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,20 @@
 
 [project.urls]
 Home = "https://github.com/pyranha-labs/ezfs"
 Changelog = "https://github.com/pyranha-labs/ezfs/releases"
 Issues = "https://github.com/pyranha-labs/ezfs/issues"
 
 [project.optional-dependencies]
+blosc = ["blosc"]
+brotli = ["brotli"]
 s3 = ["boto3"]
-zstd = ["zstandard"]
 lz4 = ["lz4"]
+snappy = ["python-snappy"]
+zstd = ["zstandard"]
 
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
```

