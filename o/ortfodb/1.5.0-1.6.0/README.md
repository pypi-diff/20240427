# Comparing `tmp/ortfodb-1.5.0.tar.gz` & `tmp/ortfodb-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ortfodb-1.5.0.tar", max compression
+gzip compressed data, was "ortfodb-1.6.0.tar", max compression
```

## Comparing `ortfodb-1.5.0.tar` & `ortfodb-1.6.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      209 2024-04-12 21:43:37.285597 ortfodb-1.5.0/README.md
--rw-r--r--   0        0        0      917 2024-04-18 20:03:07.941753 ortfodb-1.5.0/ortfodb/__init__.py
--rw-r--r--   0        0        0     9744 2024-04-20 11:25:50.063488 ortfodb-1.5.0/ortfodb/configuration.py
--rw-r--r--   0        0        0    15626 2024-04-20 11:25:50.943522 ortfodb-1.5.0/ortfodb/database.py
--rw-r--r--   0        0        0     5285 2024-04-20 11:25:51.776888 ortfodb-1.5.0/ortfodb/exporter.py
--rw-r--r--   0        0        0     4485 2024-04-20 11:25:52.596919 ortfodb-1.5.0/ortfodb/tags.py
--rw-r--r--   0        0        0     4389 2024-04-20 11:25:53.416951 ortfodb-1.5.0/ortfodb/technologies.py
--rw-r--r--   0        0        0      301 2024-04-20 11:25:55.053680 ortfodb-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 ortfodb-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      209 2024-04-12 21:43:37.285597 ortfodb-1.6.0/README.md
+-rw-r--r--   0        0        0      917 2024-04-18 20:03:07.941753 ortfodb-1.6.0/ortfodb/__init__.py
+-rw-r--r--   0        0        0     9344 2024-04-27 00:52:31.041863 ortfodb-1.6.0/ortfodb/configuration.py
+-rw-r--r--   0        0        0    16283 2024-04-27 00:52:31.898561 ortfodb-1.6.0/ortfodb/database.py
+-rw-r--r--   0        0        0     5285 2024-04-27 00:52:32.698591 ortfodb-1.6.0/ortfodb/exporter.py
+-rw-r--r--   0        0        0     4485 2024-04-27 00:52:33.515287 ortfodb-1.6.0/ortfodb/tags.py
+-rw-r--r--   0        0        0     4389 2024-04-27 00:52:34.315317 ortfodb-1.6.0/ortfodb/technologies.py
+-rw-r--r--   0        0        0      301 2024-04-27 00:52:36.012046 ortfodb-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 ortfodb-1.6.0/PKG-INFO
```

### Comparing `ortfodb-1.5.0/ortfodb/__init__.py` & `ortfodb-1.6.0/ortfodb/__init__.py`

 * *Files identical despite different names*

### Comparing `ortfodb-1.5.0/ortfodb/configuration.py` & `ortfodb-1.6.0/ortfodb/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Any, Optional, Dict, TypeVar, Callable, Type, cast
+from typing import List, Any, Dict, Optional, TypeVar, Callable, Type, cast
 
 
 T = TypeVar("T")
 
 
 def from_list(f: Callable[[Any], T], x: Any) -> List[T]:
     assert isinstance(x, list)
@@ -20,33 +20,33 @@
 
 
 def from_int(x: Any) -> int:
     assert isinstance(x, int) and not isinstance(x, bool)
     return x
 
 
+def from_dict(f: Callable[[Any], T], x: Any) -> Dict[str, T]:
+    assert isinstance(x, dict)
+    return { k: f(v) for (k, v) in x.items() }
+
+
 def from_none(x: Any) -> Any:
     assert x is None
     return x
 
 
 def from_union(fs, x):
     for f in fs:
         try:
             return f(x)
         except:
             pass
     assert False
 
 
-def from_dict(f: Callable[[Any], T], x: Any) -> Dict[str, T]:
-    assert isinstance(x, dict)
-    return { k: f(v) for (k, v) in x.items() }
-
-
 def to_class(c: Type[T], x: Any) -> dict:
     assert isinstance(x, c)
     return cast(Any, x).to_dict()
 
 
 class ExtractColorsConfiguration:
     default_files: List[str]
@@ -182,60 +182,55 @@
         result["repository"] = from_str(self.repository)
         return result
 
 
 class Configuration:
     """Configuration represents what the ortfodb.yaml configuration file describes."""
 
-    build_metadata_file: Optional[str]
     exporters: Optional[Dict[str, Dict[str, Any]]]
     """Exporter-specific configuration. Maps exporter names to their configuration."""
 
     extract_colors: Optional[ExtractColorsConfiguration]
     make_gifs: Optional[MakeGIFSConfiguration]
     make_thumbnails: Optional[MakeThumbnailsConfiguration]
     media: Optional[MediaConfiguration]
     projects_at: str
     """Path to the directory containing all projects. Must be absolute."""
 
     scattered_mode_folder: str
     tags: Optional[TagsConfiguration]
     technologies: Optional[TechnologiesConfiguration]
 
-    def __init__(self, build_metadata_file: Optional[str], exporters: Optional[Dict[str, Dict[str, Any]]], extract_colors: Optional[ExtractColorsConfiguration], make_gifs: Optional[MakeGIFSConfiguration], make_thumbnails: Optional[MakeThumbnailsConfiguration], media: Optional[MediaConfiguration], projects_at: str, scattered_mode_folder: str, tags: Optional[TagsConfiguration], technologies: Optional[TechnologiesConfiguration]) -> None:
-        self.build_metadata_file = build_metadata_file
+    def __init__(self, exporters: Optional[Dict[str, Dict[str, Any]]], extract_colors: Optional[ExtractColorsConfiguration], make_gifs: Optional[MakeGIFSConfiguration], make_thumbnails: Optional[MakeThumbnailsConfiguration], media: Optional[MediaConfiguration], projects_at: str, scattered_mode_folder: str, tags: Optional[TagsConfiguration], technologies: Optional[TechnologiesConfiguration]) -> None:
         self.exporters = exporters
         self.extract_colors = extract_colors
         self.make_gifs = make_gifs
         self.make_thumbnails = make_thumbnails
         self.media = media
         self.projects_at = projects_at
         self.scattered_mode_folder = scattered_mode_folder
         self.tags = tags
         self.technologies = technologies
 
     @staticmethod
     def from_dict(obj: Any) -> 'Configuration':
         assert isinstance(obj, dict)
-        build_metadata_file = from_union([from_str, from_none], obj.get("build metadata file"))
         exporters = from_union([lambda x: from_dict(lambda x: from_dict(lambda x: x, x), x), from_none], obj.get("exporters"))
         extract_colors = from_union([ExtractColorsConfiguration.from_dict, from_none], obj.get("extract colors"))
         make_gifs = from_union([MakeGIFSConfiguration.from_dict, from_none], obj.get("make gifs"))
         make_thumbnails = from_union([MakeThumbnailsConfiguration.from_dict, from_none], obj.get("make thumbnails"))
         media = from_union([MediaConfiguration.from_dict, from_none], obj.get("media"))
         projects_at = from_str(obj.get("projects at"))
         scattered_mode_folder = from_str(obj.get("scattered mode folder"))
         tags = from_union([TagsConfiguration.from_dict, from_none], obj.get("tags"))
         technologies = from_union([TechnologiesConfiguration.from_dict, from_none], obj.get("technologies"))
-        return Configuration(build_metadata_file, exporters, extract_colors, make_gifs, make_thumbnails, media, projects_at, scattered_mode_folder, tags, technologies)
+        return Configuration(exporters, extract_colors, make_gifs, make_thumbnails, media, projects_at, scattered_mode_folder, tags, technologies)
 
     def to_dict(self) -> dict:
         result: dict = {}
-        if self.build_metadata_file is not None:
-            result["build metadata file"] = from_union([from_str, from_none], self.build_metadata_file)
         if self.exporters is not None:
             result["exporters"] = from_union([lambda x: from_dict(lambda x: from_dict(lambda x: x, x), x), from_none], self.exporters)
         if self.extract_colors is not None:
             result["extract colors"] = from_union([lambda x: to_class(ExtractColorsConfiguration, x), from_none], self.extract_colors)
         if self.make_gifs is not None:
             result["make gifs"] = from_union([lambda x: to_class(MakeGIFSConfiguration, x), from_none], self.make_gifs)
         if self.make_thumbnails is not None:
```

### Comparing `ortfodb-1.5.0/ortfodb/database.py` & `ortfodb-1.6.0/ortfodb/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Any, List, Dict, TypeVar, Type, cast, Callable
+from typing import Any, Dict, List, TypeVar, Type, cast, Callable
+from datetime import datetime
+import dateutil.parser
 
 
 T = TypeVar("T")
 
 
 def from_bool(x: Any) -> bool:
     assert isinstance(x, bool)
@@ -25,29 +27,33 @@
 
 
 def to_float(x: Any) -> float:
     assert isinstance(x, (int, float))
     return x
 
 
+def from_datetime(x: Any) -> datetime:
+    return dateutil.parser.parse(x)
+
+
 def to_class(c: Type[T], x: Any) -> dict:
     assert isinstance(x, c)
     return cast(Any, x).to_dict()
 
 
-def from_list(f: Callable[[Any], T], x: Any) -> List[T]:
-    assert isinstance(x, list)
-    return [f(y) for y in x]
-
-
 def from_dict(f: Callable[[Any], T], x: Any) -> Dict[str, T]:
     assert isinstance(x, dict)
     return { k: f(v) for (k, v) in x.items() }
 
 
+def from_list(f: Callable[[Any], T], x: Any) -> List[T]:
+    assert isinstance(x, list)
+    return [f(y) for y in x]
+
+
 class MediaAttributes:
     """MediaAttributes stores which HTML attributes should be added to the media."""
 
     autoplay: bool
     """Controlled with attribute character > (adds)"""
 
     controls: bool
@@ -180,41 +186,47 @@
 
     content_type: str
     dimensions: ImageDimensions
     dist_source: str
     duration: float
     """in seconds"""
 
+    hash: str
+    """Hash of the media file, used for caching purposes. Could also serve as an integrity
+    check.
+    The value is the MD5 hash, base64-encoded.
+    """
     has_sound: bool
     id: str
     index: int
     online: bool
     relative_source: str
     size: int
     """in bytes"""
 
     text: str
     thumbnails: ThumbnailsMap
-    thumbnails_built_at: str
+    thumbnails_built_at: datetime
     title: str
     type: str
     url: str
 
-    def __init__(self, alt: str, analyzed: bool, anchor: str, attributes: MediaAttributes, caption: str, colors: ColorPalette, content: str, content_type: str, dimensions: ImageDimensions, dist_source: str, duration: float, has_sound: bool, id: str, index: int, online: bool, relative_source: str, size: int, text: str, thumbnails: ThumbnailsMap, thumbnails_built_at: str, title: str, type: str, url: str) -> None:
+    def __init__(self, alt: str, analyzed: bool, anchor: str, attributes: MediaAttributes, caption: str, colors: ColorPalette, content: str, content_type: str, dimensions: ImageDimensions, dist_source: str, duration: float, hash: str, has_sound: bool, id: str, index: int, online: bool, relative_source: str, size: int, text: str, thumbnails: ThumbnailsMap, thumbnails_built_at: datetime, title: str, type: str, url: str) -> None:
         self.alt = alt
         self.analyzed = analyzed
         self.anchor = anchor
         self.attributes = attributes
         self.caption = caption
         self.colors = colors
         self.content = content
         self.content_type = content_type
         self.dimensions = dimensions
         self.dist_source = dist_source
         self.duration = duration
+        self.hash = hash
         self.has_sound = has_sound
         self.id = id
         self.index = index
         self.online = online
         self.relative_source = relative_source
         self.size = size
         self.text = text
@@ -234,79 +246,85 @@
         caption = from_str(obj.get("caption"))
         colors = ColorPalette.from_dict(obj.get("colors"))
         content = from_str(obj.get("content"))
         content_type = from_str(obj.get("contentType"))
         dimensions = ImageDimensions.from_dict(obj.get("dimensions"))
         dist_source = from_str(obj.get("distSource"))
         duration = from_float(obj.get("duration"))
+        hash = from_str(obj.get("hash"))
         has_sound = from_bool(obj.get("hasSound"))
         id = from_str(obj.get("id"))
         index = from_int(obj.get("index"))
         online = from_bool(obj.get("online"))
         relative_source = from_str(obj.get("relativeSource"))
         size = from_int(obj.get("size"))
         text = from_str(obj.get("text"))
         thumbnails = ThumbnailsMap.from_dict(obj.get("thumbnails"))
-        thumbnails_built_at = from_str(obj.get("thumbnailsBuiltAt"))
+        thumbnails_built_at = from_datetime(obj.get("thumbnailsBuiltAt"))
         title = from_str(obj.get("title"))
         type = from_str(obj.get("type"))
         url = from_str(obj.get("url"))
-        return ContentBlock(alt, analyzed, anchor, attributes, caption, colors, content, content_type, dimensions, dist_source, duration, has_sound, id, index, online, relative_source, size, text, thumbnails, thumbnails_built_at, title, type, url)
+        return ContentBlock(alt, analyzed, anchor, attributes, caption, colors, content, content_type, dimensions, dist_source, duration, hash, has_sound, id, index, online, relative_source, size, text, thumbnails, thumbnails_built_at, title, type, url)
 
     def to_dict(self) -> dict:
         result: dict = {}
         result["alt"] = from_str(self.alt)
         result["analyzed"] = from_bool(self.analyzed)
         result["anchor"] = from_str(self.anchor)
         result["attributes"] = to_class(MediaAttributes, self.attributes)
         result["caption"] = from_str(self.caption)
         result["colors"] = to_class(ColorPalette, self.colors)
         result["content"] = from_str(self.content)
         result["contentType"] = from_str(self.content_type)
         result["dimensions"] = to_class(ImageDimensions, self.dimensions)
         result["distSource"] = from_str(self.dist_source)
         result["duration"] = to_float(self.duration)
+        result["hash"] = from_str(self.hash)
         result["hasSound"] = from_bool(self.has_sound)
         result["id"] = from_str(self.id)
         result["index"] = from_int(self.index)
         result["online"] = from_bool(self.online)
         result["relativeSource"] = from_str(self.relative_source)
         result["size"] = from_int(self.size)
         result["text"] = from_str(self.text)
         result["thumbnails"] = to_class(ThumbnailsMap, self.thumbnails)
-        result["thumbnailsBuiltAt"] = from_str(self.thumbnails_built_at)
+        result["thumbnailsBuiltAt"] = self.thumbnails_built_at.isoformat()
         result["title"] = from_str(self.title)
         result["type"] = from_str(self.type)
         result["url"] = from_str(self.url)
         return result
 
 
 class LocalizedContent:
+    abbreviations: Dict[str, str]
     blocks: List[ContentBlock]
     footnotes: Dict[str, str]
     layout: List[List[str]]
     title: str
 
-    def __init__(self, blocks: List[ContentBlock], footnotes: Dict[str, str], layout: List[List[str]], title: str) -> None:
+    def __init__(self, abbreviations: Dict[str, str], blocks: List[ContentBlock], footnotes: Dict[str, str], layout: List[List[str]], title: str) -> None:
+        self.abbreviations = abbreviations
         self.blocks = blocks
         self.footnotes = footnotes
         self.layout = layout
         self.title = title
 
     @staticmethod
     def from_dict(obj: Any) -> 'LocalizedContent':
         assert isinstance(obj, dict)
+        abbreviations = from_dict(from_str, obj.get("abbreviations"))
         blocks = from_list(ContentBlock.from_dict, obj.get("blocks"))
         footnotes = from_dict(from_str, obj.get("footnotes"))
         layout = from_list(lambda x: from_list(from_str, x), obj.get("layout"))
         title = from_str(obj.get("title"))
-        return LocalizedContent(blocks, footnotes, layout, title)
+        return LocalizedContent(abbreviations, blocks, footnotes, layout, title)
 
     def to_dict(self) -> dict:
         result: dict = {}
+        result["abbreviations"] = from_dict(from_str, self.abbreviations)
         result["blocks"] = from_list(lambda x: to_class(ContentBlock, x), self.blocks)
         result["footnotes"] = from_dict(from_str, self.footnotes)
         result["layout"] = from_list(lambda x: from_list(from_str, x), self.layout)
         result["title"] = from_str(self.title)
         return result
 
 
@@ -391,53 +409,53 @@
         result["tags"] = from_list(from_str, self.tags)
         result["thumbnail"] = from_str(self.thumbnail)
         result["titleStyle"] = from_str(self.title_style)
         result["wip"] = from_bool(self.wip)
         return result
 
 
-class AnalyzedWork:
-    """AnalyzedWork represents a complete work, with analyzed mediae."""
+class Work:
+    """Work represents a given work in the database."""
 
-    built_at: str
+    built_at: datetime
     content: Dict[str, LocalizedContent]
     description_hash: str
     id: str
     metadata: WorkMetadata
     partial: bool
 
-    def __init__(self, built_at: str, content: Dict[str, LocalizedContent], description_hash: str, id: str, metadata: WorkMetadata, partial: bool) -> None:
+    def __init__(self, built_at: datetime, content: Dict[str, LocalizedContent], description_hash: str, id: str, metadata: WorkMetadata, partial: bool) -> None:
         self.built_at = built_at
         self.content = content
         self.description_hash = description_hash
         self.id = id
         self.metadata = metadata
         self.partial = partial
 
     @staticmethod
-    def from_dict(obj: Any) -> 'AnalyzedWork':
+    def from_dict(obj: Any) -> 'Work':
         assert isinstance(obj, dict)
-        built_at = from_str(obj.get("builtAt"))
+        built_at = from_datetime(obj.get("builtAt"))
         content = from_dict(LocalizedContent.from_dict, obj.get("content"))
         description_hash = from_str(obj.get("descriptionHash"))
         id = from_str(obj.get("id"))
         metadata = WorkMetadata.from_dict(obj.get("metadata"))
         partial = from_bool(obj.get("Partial"))
-        return AnalyzedWork(built_at, content, description_hash, id, metadata, partial)
+        return Work(built_at, content, description_hash, id, metadata, partial)
 
     def to_dict(self) -> dict:
         result: dict = {}
-        result["builtAt"] = from_str(self.built_at)
+        result["builtAt"] = self.built_at.isoformat()
         result["content"] = from_dict(lambda x: to_class(LocalizedContent, x), self.content)
         result["descriptionHash"] = from_str(self.description_hash)
         result["id"] = from_str(self.id)
         result["metadata"] = to_class(WorkMetadata, self.metadata)
         result["Partial"] = from_bool(self.partial)
         return result
 
 
-def database_from_dict(s: Any) -> Dict[str, AnalyzedWork]:
-    return from_dict(AnalyzedWork.from_dict, s)
+def database_from_dict(s: Any) -> Dict[str, Work]:
+    return from_dict(Work.from_dict, s)
 
 
-def database_to_dict(x: Dict[str, AnalyzedWork]) -> Any:
-    return from_dict(lambda x: to_class(AnalyzedWork, x), x)
+def database_to_dict(x: Dict[str, Work]) -> Any:
+    return from_dict(lambda x: to_class(Work, x), x)
```

### Comparing `ortfodb-1.5.0/ortfodb/exporter.py` & `ortfodb-1.6.0/ortfodb/exporter.py`

 * *Files identical despite different names*

### Comparing `ortfodb-1.5.0/ortfodb/tags.py` & `ortfodb-1.6.0/ortfodb/tags.py`

 * *Files identical despite different names*

### Comparing `ortfodb-1.5.0/ortfodb/technologies.py` & `ortfodb-1.6.0/ortfodb/technologies.py`

 * *Files identical despite different names*

### Comparing `ortfodb-1.5.0/PKG-INFO` & `ortfodb-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortfodb
-Version: 1.5.0
+Version: 1.6.0
 Summary: ortfodb client library
 License: MIT
 Author: Ewen Le Bihan
 Author-email: hey@ewen.works
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

