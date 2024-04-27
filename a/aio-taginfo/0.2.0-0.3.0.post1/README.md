# Comparing `tmp/aio_taginfo-0.2.0.tar.gz` & `tmp/aio_taginfo-0.3.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_taginfo-0.2.0.tar", max compression
+gzip compressed data, was "aio_taginfo-0.3.0.post1.tar", max compression
```

## Comparing `aio_taginfo-0.2.0.tar` & `aio_taginfo-0.3.0.post1.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0      767 2023-10-20 02:14:59.272492 aio_taginfo-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2023-10-20 02:14:59.272492 aio_taginfo-0.2.0/LICENSE
--rw-r--r--   0        0        0     7328 2023-10-20 02:14:59.272492 aio_taginfo-0.2.0/README.md
--rw-r--r--   0        0        0     1178 2023-10-20 02:14:59.272492 aio_taginfo-0.2.0/aio_taginfo/__init__.py
--rw-r--r--   0        0        0       21 2023-10-20 02:14:59.272492 aio_taginfo-0.2.0/aio_taginfo/api/__init__.py
--rw-r--r--   0        0        0     2093 2023-10-20 02:14:59.272492 aio_taginfo-0.2.0/aio_taginfo/api/v4/__init__.py
--rw-r--r--   0        0        0     4312 2023-10-20 02:14:59.272492 aio_taginfo-0.2.0/aio_taginfo/api/v4/_internal.py
--rw-r--r--   0        0        0      718 2023-10-20 02:14:59.276492 aio_taginfo-0.2.0/aio_taginfo/api/v4/key/__init__.py
--rw-r--r--   0        0        0       45 2023-10-20 02:14:59.276492 aio_taginfo-0.2.0/aio_taginfo/api/v4/key/distribution/__init__.py
--rw-r--r--   0        0        0     1035 2023-10-20 02:14:59.276492 aio_taginfo-0.2.0/aio_taginfo/api/v4/key/distribution/nodes.py
--rw-r--r--   0        0        0     3796 2023-10-20 02:14:59.276492 aio_taginfo-0.2.0/aio_taginfo/api/v4/key/overview.py
--rw-r--r--   0        0        0     1627 2023-10-20 02:14:59.276492 aio_taginfo-0.2.0/aio_taginfo/api/v4/key/prevalent_values.py
--rw-r--r--   0        0        0     2643 2023-10-20 02:14:59.276492 aio_taginfo-0.2.0/aio_taginfo/api/v4/key/similar.py
--rw-r--r--   0        0        0       33 2023-10-20 02:14:59.276492 aio_taginfo-0.2.0/aio_taginfo/api/v4/site/__init__.py
--rw-r--r--   0        0        0       40 2023-10-20 02:14:59.276492 aio_taginfo-0.2.0/aio_taginfo/api/v4/site/config/__init__.py
--rw-r--r--   0        0        0     1590 2023-10-20 02:14:59.276492 aio_taginfo-0.2.0/aio_taginfo/api/v4/site/config/geodistribution.py
--rw-r--r--   0        0        0      701 2023-10-20 02:14:59.276492 aio_taginfo-0.2.0/aio_taginfo/error.py
--rw-r--r--   0        0        0     2885 2023-10-20 02:14:59.276492 aio_taginfo-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     8866 1970-01-01 00:00:00.000000 aio_taginfo-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-27 04:57:44.153163 aio_taginfo-0.3.0.post1/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2024-04-27 04:57:44.153163 aio_taginfo-0.3.0.post1/LICENSE
+-rw-r--r--   0        0        0     9128 2024-04-27 04:57:44.153163 aio_taginfo-0.3.0.post1/README.md
+-rw-r--r--   0        0        0     1547 2024-04-27 04:57:44.157163 aio_taginfo-0.3.0.post1/aio_taginfo/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-27 04:57:44.157163 aio_taginfo-0.3.0.post1/aio_taginfo/api/__init__.py
+-rw-r--r--   0        0        0     2254 2024-04-27 04:57:44.157163 aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/__init__.py
+-rw-r--r--   0        0        0     4312 2024-04-27 04:57:44.157163 aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/_internal.py
+-rw-r--r--   0        0        0      732 2024-04-27 04:57:44.157163 aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/key/__init__.py
+-rw-r--r--   0        0        0       45 2024-04-27 04:57:44.157163 aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/key/distribution/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-27 04:57:44.157163 aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/key/distribution/nodes.py
+-rw-r--r--   0        0        0     3867 2024-04-27 04:57:44.157163 aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/key/overview.py
+-rw-r--r--   0        0        0     1642 2024-04-27 04:57:44.157163 aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/key/prevalent_values.py
+-rw-r--r--   0        0        0     2652 2024-04-27 04:57:44.157163 aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/key/similar.py
+-rw-r--r--   0        0        0       33 2024-04-27 04:57:44.157163 aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/site/__init__.py
+-rw-r--r--   0        0        0       40 2024-04-27 04:57:44.157163 aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/site/config/__init__.py
+-rw-r--r--   0        0        0     1604 2024-04-27 04:57:44.157163 aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/site/config/geodistribution.py
+-rw-r--r--   0        0        0       33 2024-04-27 04:57:44.157163 aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/tags/__init__.py
+-rw-r--r--   0        0        0     4378 2024-04-27 04:57:44.157163 aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/tags/popular.py
+-rw-r--r--   0        0        0      743 2024-04-27 04:57:44.157163 aio_taginfo-0.3.0.post1/aio_taginfo/error.py
+-rw-r--r--   0        0        0        0 2024-04-27 04:57:44.157163 aio_taginfo-0.3.0.post1/aio_taginfo/py.typed
+-rw-r--r--   0        0        0     2900 2024-04-27 04:57:44.157163 aio_taginfo-0.3.0.post1/pyproject.toml
+-rw-r--r--   0        0        0    10609 1970-01-01 00:00:00.000000 aio_taginfo-0.3.0.post1/PKG-INFO
```

### Comparing `aio_taginfo-0.2.0/CHANGELOG.md` & `aio_taginfo-0.3.0.post1/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 This project adheres to [Semantic Versioning](http://semver.org/).
 
 <br>
 
+## [0.3.0] – 2024-04-27
+* Implement `/api/4/tags/popular` endpoint
+* Relax `aiohttp` requirement to `^3.9` (from `~3.9.0b0`)
+* Relax `pydantic` requirement to `^2.4` (from `~2.4`)
+* Add `py.typed` to make the package PEP 561 compatible
+
+<br>
+
 ## [0.2.0] – 2023-10-20
 * Add Python 3.12 support
 * Drop Python 3.9 support
 * Increased `aiohttp` requirement to `~3.9.0b0`
 * Enable `speedups` extra of `aiohttp`
 
 <br>
@@ -18,8 +26,9 @@
   * `/api/4/key/distribution/nodes`
   * `/api/4/key/overview`
   * `/api/4/key/prevalent_values`
   * `/api/4/key/similar`
   * `/api/4/site/config/geodistribution`
 
 [0.1.0]: https://github.com/timwie/aio-taginfo/releases/tag/v0.1.0
-[0.1.0]: https://github.com/timwie/aio-taginfo/releases/tag/v0.2.0
+[0.2.0]: https://github.com/timwie/aio-taginfo/releases/tag/v0.2.0
+[0.3.0]: https://github.com/timwie/aio-taginfo/releases/tag/v0.3.0
```

### Comparing `aio_taginfo-0.2.0/LICENSE` & `aio_taginfo-0.3.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_taginfo-0.2.0/aio_taginfo/api/v4/__init__.py` & `aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 from typing import Generic, TypeVar
 
 from pydantic import Field, HttpUrl, model_validator
 from pydantic.dataclasses import dataclass
 
 
 __all__ = (
-    "key",
-    "site",
+    "key",  # pyright: ignore[reportUnsupportedDunderAll]
+    "site",  # pyright: ignore[reportUnsupportedDunderAll]
     "Response",
     "PngResponse",
     "SortOrder",
     "ObjectType",
     "PrintingDirection",
 )
 
 
 T = TypeVar("T")
 
 
-@dataclass
+@dataclass(kw_only=True)
 class Response(Generic[T]):
     """
     JSON data response.
 
     Attributes:
         data: Payload specific to the called endpoint
         data_until: All changes in the source until this date are reflected in this taginfo result
@@ -40,26 +40,26 @@
     data_until: datetime = Field(repr=False, frozen=True)
     url: HttpUrl = Field(repr=False, frozen=True)
     total: int = Field(ge=0, repr=True, frozen=True)
     page: int | None = Field(default=None, gt=0, repr=True, frozen=True)
     rp: int | None = Field(default=None, gt=0, repr=True, frozen=True)
 
 
-@dataclass
+@dataclass(kw_only=True)
 class PngResponse:
     """
     PNG image response.
 
     Attributes:
         data: PNG data
     """
 
     data: bytes = Field(repr=False, frozen=True)
 
-    @model_validator(mode="after")
+    @model_validator(mode="after")  # pyright: ignore[reportArgumentType]
     def post_root(self) -> "PngResponse":
         """Basic PNG validation by checking for magic bytes."""
         if not self.data.startswith(_PNG_MAGIC):
             msg = "did not find PNG magic bytes"
             raise AssertionError(msg)
         return self
```

### Comparing `aio_taginfo-0.2.0/aio_taginfo/api/v4/_internal.py` & `aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/_internal.py`

 * *Files identical despite different names*

### Comparing `aio_taginfo-0.2.0/aio_taginfo/api/v4/key/__init__.py` & `aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/key/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """`/api/v4/key/` endpoints."""
 
 from pydantic import Field
 from pydantic.dataclasses import dataclass
 
 
-@dataclass
+@dataclass(kw_only=True)
 class PrevalentValue:
     """
     One value of a given tag and the number of times it was used.
 
     Attributes:
         value: The tag value or ``None`` to count the sum of the counts for all values not listed
         count: Number of objects with this tag value
```

### Comparing `aio_taginfo-0.2.0/aio_taginfo/api/v4/key/distribution/nodes.py` & `aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/key/distribution/nodes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """`/api/v4/key/distribution/nodes` endpoint."""
+
 from typing import Annotated
 
 from aio_taginfo.api.v4 import PngResponse
 from aio_taginfo.api.v4._internal import api_get_png, api_params
 
 from aiohttp import ClientSession
 from pydantic import Field, StringConstraints
 from pydantic.dataclasses import dataclass
 
 
-@dataclass
+@dataclass(kw_only=True)
 class _Params:
-    key: Annotated[
-        str, StringConstraints(min_length=1, strip_whitespace=True, strict=True)
-    ] = Field(repr=True, frozen=True)
+    key: Annotated[str, StringConstraints(min_length=1, strip_whitespace=True, strict=True)] = (
+        Field(repr=True, frozen=True)
+    )
 
 
 async def call(key: str, session: ClientSession | None = None) -> PngResponse:
     """
     Get map with distribution of this key in the database (nodes only).
 
     https://taginfo.openstreetmap.org/taginfo/apidoc#api_4_key_distribution_nodes
```

### Comparing `aio_taginfo-0.2.0/aio_taginfo/api/v4/key/overview.py` & `aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/key/overview.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """`/api/v4/key/overview` endpoint."""
+
 from typing import Annotated
 
 from aio_taginfo.api.v4 import ObjectType, PrintingDirection, Response
 from aio_taginfo.api.v4._internal import api_get_json, api_params
 from aio_taginfo.api.v4.key import PrevalentValue
 
 from aiohttp import ClientSession
@@ -15,15 +16,15 @@
     "KeyOverview",
     "KeyDescription",
     "KeyObjectCount",
     "KeyWikiPage",
 )
 
 
-@dataclass
+@dataclass(kw_only=True)
 class _Params:
     key: Annotated[str, StringConstraints(min_length=1, strip_whitespace=True)] = Field(
         repr=True, frozen=True
     )
 
 
 async def call(
@@ -46,15 +47,15 @@
         path="key/overview",
         cls=Response[KeyOverview],
         session=session,
         params=api_params(_Params, key=key),
     )
 
 
-@dataclass
+@dataclass(kw_only=True)
 class KeyObjectCount:
     """
     Usage statistic of a given key for a given type of object.
 
     Attributes:
         type: Object type
         count: Number of objects with this type and key
@@ -64,29 +65,29 @@
 
     type: ObjectType = Field(repr=True, frozen=True)
     count: int = Field(ge=0, repr=True, frozen=True)
     count_fraction: float = Field(ge=0.0, le=1.0, allow_inf_nan=False, repr=True, frozen=True)
     values: int = Field(ge=0, repr=True, frozen=True)
 
 
-@dataclass
+@dataclass(kw_only=True)
 class KeyDescription:
     """
     Description of a given key in some language.
 
     Attributes:
         text: Description text
         dir: Printing direction for this language
     """
 
     text: str = Field(min_length=1, repr=True, frozen=True)
     dir: PrintingDirection = Field(repr=False, frozen=True)
 
 
-@dataclass
+@dataclass(kw_only=True)
 class KeyWikiPage:
     """
     Language code for which a wiki page about a given key are available.
 
     Attributes:
         lang: Language code
         english: English name of this language
@@ -96,15 +97,15 @@
 
     lang: str = Field(min_length=2, repr=True, frozen=True)
     english: str = Field(min_length=1, repr=True, frozen=True)
     native: str = Field(min_length=1, repr=True, frozen=True)
     dir: PrintingDirection = Field(repr=False, frozen=True)
 
 
-@dataclass
+@dataclass(kw_only=True)
 class KeyOverview:
     """
     Various data for a given key.
 
     Attributes:
         key: The tag key that was requested
         users: Number of users last editing objects with this key
```

### Comparing `aio_taginfo-0.2.0/aio_taginfo/api/v4/key/prevalent_values.py` & `aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/key/prevalent_values.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """`/api/v4/key/prevalent_values` endpoint."""
+
 from typing import Annotated
 
 from aio_taginfo.api.v4 import ObjectType, Response
 from aio_taginfo.api.v4._internal import api_get_json, api_params
 from aio_taginfo.api.v4.key import PrevalentValue
 
 from aiohttp import ClientSession
 from pydantic import Field, StringConstraints
 from pydantic.dataclasses import dataclass
 
 
-@dataclass
+@dataclass(kw_only=True)
 class _Params:
     key: Annotated[str, StringConstraints(min_length=1, strip_whitespace=True)] = Field(
         repr=True, frozen=True
     )
     min_fraction: float = Field(ge=0.01, le=1.0, allow_inf_nan=False, repr=True, frozen=True)
     filter: ObjectType = Field(repr=True, frozen=True)
```

### Comparing `aio_taginfo-0.2.0/aio_taginfo/api/v4/key/similar.py` & `aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/key/similar.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 __all__ = (
     "call",
     "SimilarKey",
     "SimilarKeySorting",
 )
 
 
-@dataclass
+@dataclass(kw_only=True)
 class SimilarKey:
     """
     Result of a key that is similar to a given key.
 
     Attributes:
         other_key: other key
         count_all: number of objects that have the other key
@@ -38,37 +38,37 @@
     """Sort options for similar keys."""
 
     OTHER_KEY = "other_key"
     COUNT_ALL = "count_all"
     SIMILARITY = "similarity"
 
 
-@dataclass
+@dataclass(kw_only=True)
 class _Params:
     key: Annotated[str, StringConstraints(min_length=1, strip_whitespace=True)] = Field(
         repr=True, frozen=True
     )
     query: Annotated[str, StringConstraints(min_length=1, strip_whitespace=True)] | None = Field(
         repr=True, frozen=True
     )
     sortname: SimilarKeySorting = Field(repr=True, frozen=True)
     sortorder: SortOrder = Field(repr=True, frozen=True)
     page: int = Field(gt=0, repr=True, frozen=True)
     rp: int = Field(ge=0, repr=True, frozen=True)
 
 
-async def call(  # noqa: PLR0913
+async def call(
     key: str,
     query: str | None = None,
     sortname: SimilarKeySorting = SimilarKeySorting.OTHER_KEY,
     sortorder: SortOrder = SortOrder.ASC,
     page: int = 1,
     rp: int = 0,
     session: ClientSession | None = None,
-) -> Response[list["SimilarKey"]]:
+) -> Response[list[SimilarKey]]:
     """
     Find keys that are similar to a given key.
 
     https://taginfo.openstreetmap.org/taginfo/apidoc#api_4_key_similar
 
     Args:
         key: tag key
```

### Comparing `aio_taginfo-0.2.0/aio_taginfo/api/v4/site/config/geodistribution.py` & `aio_taginfo-0.3.0.post1/aio_taginfo/api/v4/site/config/geodistribution.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     return await api_get_json(
         path="/api/4/site/config/geodistribution",
         cls=SiteConfigGeodistribution,
         session=session,
     )
 
 
-@dataclass
+@dataclass(kw_only=True)
 class SiteConfigGeodistribution:
     """
     Information about the background map for distribution charts.
 
     Attributes:
         width: width of background image
         height: height of background image
```

### Comparing `aio_taginfo-0.2.0/aio_taginfo/error.py` & `aio_taginfo-0.3.0.post1/aio_taginfo/error.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 import pydantic
 
 
 class TagInfoError(Exception):
     """Base class for taginfo API errors."""
 
 
-@dataclass
+@dataclass(kw_only=True)
 class TagInfoValueError(Exception):
     """Failed to validate given parameters; did not call the taginfo API."""
 
     cause: pydantic.ValidationError
 
 
-@dataclass
+@dataclass(kw_only=True)
 class TagInfoCallError(Exception):
     """Failed HTTP call to the taginfo API."""
 
     cause: aiohttp.ClientError
 
 
-@dataclass
+@dataclass(kw_only=True)
 class TagInfoValidationError(Exception):
     """
     Failed to validate the response of the taginfo API.
 
     This should usually indicate a bug in this library.
     """
```

### Comparing `aio_taginfo-0.2.0/pyproject.toml` & `aio_taginfo-0.3.0.post1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-taginfo"
-version = "0.2.0"
+version = "0.3.0.post1"
 description = "Async client for the OpenStreetMap taginfo API"
 authors = ["Tim Wiechers <mail@timwie.dev>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/timwie/aio-taginfo"
 documentation = "https://www.timwie.dev/aio-taginfo/"
 packages = [{ include = "aio_taginfo" }]
@@ -27,65 +27,82 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Topic :: Scientific/Engineering :: GIS",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Internet :: WWW/HTTP",
     "Typing :: Typed",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
-    "Programming Language :: Python :: 3 :: Only",
 ]
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/timwie/aio-taginfo/blob/main/CHANGELOG.md"
 "Coverage" = "https://codecov.io/gh/timwie/aio-taginfo"
 
 [tool.poetry.dependencies]
-aiohttp = { version = "~3.9.0b0", extras = ["speedups"] }
-pydantic = "~2.4"
+aiohttp = { version = "^3.9", extras = ["speedups"] }
+pydantic = "^2.4"
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
-aioresponses = "^0.7.4"
-black = "^23.10.0"
+aioresponses = "^0.7.6"
 codecov = "^2.1.13"
 invoke = "^2.2.0"
-isort = "^5.12.0"
-mypy = "^1.6.1"
-pdoc = "^14.1.0"
-pytest = "^7.4.2"
-pytest-asyncio = "^0.21.1"
-pytest-cov = "^4.1.0"
+isort = "^5.13.2"
+mypy = "^1.10.0"
+pdoc = "^14.4.0"
+pytest = "^8.1.2"
+pytest-asyncio = "^0.23.5"
+pytest-cov = "^5.0.0"
 pytest-randomly = "^3.15.0"
-ruff = "^0.1.1"
-pyright = "^1.1.332"
+ruff = "^0.4.1"
+pyright = "^1.1.360"
 
 [tool.ruff]
-# https://github.com/charliermarsh/ruff#configuration
-# https://beta.ruff.rs/docs/rules/
+# https://docs.astral.sh/ruff/settings/
+# https://docs.astral.sh/ruff/rules/
 line-length = 100
 target-version = "py310"
+
+[tool.ruff.lint]
 select = [
-    "F", "E", "W", "N", "D", "UP",
-    "ANN", "S", "B", "C4", "EM", "SIM", "ARG",
-    "PL", "TRY", "PERF", "RUF"
+    "ANN",
+    "ARG",
+    "B",
+    "C4",
+    "D",
+    "DTZ",
+    "E",
+    "EM",
+    "F",
+    "FBT",
+    "N",
+    "PERF",
+    "PL",
+    "PTH",
+    "RUF",
+    "S",
+    "SIM",
+    "TRY",
+    "UP",
+    "W",
 ]
 ignore = [
-    "D105", "D107", "D203", "D212",
     "ANN003", "ANN101", "ANN102", "ANN401",
     "C408",
-    "PLR2004", "PLW2901",
-    "TRY003",
+    "D105", "D107", "D203", "D212",
+    "PLR0913", "PLR2004", "PLW2901",
     "S101",
+    "TRY003",
+    "UP015",
 ]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.black]
 # https://github.com/psf/black#configuration
 line-length = 100
 
 [tool.isort]
```

