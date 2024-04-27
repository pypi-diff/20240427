# Comparing `tmp/brave_search-0.1.8.tar.gz` & `tmp/brave_search-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brave_search-0.1.8.tar", max compression
+gzip compressed data, was "brave_search-0.2.0.tar", max compression
```

## Comparing `brave_search-0.1.8.tar` & `brave_search-0.2.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    10420 2024-03-09 12:31:59.811484 brave_search-0.1.8/LICENSE.MD
--rw-r--r--   0        0        0     4926 2024-03-11 21:58:27.124332 brave_search-0.1.8/README.md
--rw-r--r--   0        0        0     4583 2024-03-11 21:58:51.083585 brave_search-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       78 2023-12-01 12:01:03.058624 brave_search-0.1.8/src/brave/__init__.py
--rw-r--r--   0        0        0     4442 2023-12-03 18:38:37.425306 brave_search-0.1.8/src/brave/async_brave.py
--rw-r--r--   0        0        0     6320 2024-03-11 21:58:27.126491 brave_search-0.1.8/src/brave/client.py
--rw-r--r--   0        0        0      140 2023-12-19 12:18:55.721219 brave_search-0.1.8/src/brave/exceptions.py
--rw-r--r--   0        0        0     1336 2023-12-19 12:18:55.722403 brave_search-0.1.8/src/brave/goggles/README.md
--rw-r--r--   0        0        0       25 2023-12-04 15:45:58.439411 brave_search-0.1.8/src/brave/goggles/__init__.py
--rw-r--r--   0        0        0      169 2023-12-04 15:45:58.442242 brave_search-0.1.8/src/brave/goggles/directory.py
--rw-r--r--   0        0        0     6614 2023-12-04 15:45:58.448415 brave_search-0.1.8/src/brave/goggles/sample_goggle.goggle
--rw-r--r--   0        0        0     1115 2023-12-04 17:02:16.473377 brave_search-0.1.8/src/brave/goggles/thought_leadership.goggle
--rw-r--r--   0        0        0     1335 2023-12-19 12:18:55.723020 brave_search-0.1.8/src/brave/sync.py
--rw-r--r--   0        0        0      122 2023-12-03 18:38:37.429228 brave_search-0.1.8/src/brave/types/__init__.py
--rw-r--r--   0        0        0        0 2023-12-03 18:38:37.429267 brave_search-0.1.8/src/brave/types/image/__init__.py
--rw-r--r--   0        0        0      718 2023-12-03 18:38:37.440675 brave_search-0.1.8/src/brave/types/image/image_query.py
--rw-r--r--   0        0        0     1100 2023-12-03 18:38:37.443820 brave_search-0.1.8/src/brave/types/image/image_result.py
--rw-r--r--   0        0        0      556 2023-12-03 18:38:37.447770 brave_search-0.1.8/src/brave/types/image/image_search_response.py
--rw-r--r--   0        0        0      298 2023-12-03 18:38:37.448297 brave_search-0.1.8/src/brave/types/image/properties.py
--rw-r--r--   0        0        0     1085 2024-03-11 21:58:27.126882 brave_search-0.1.8/src/brave/types/not_implemented.py
--rw-r--r--   0        0        0        0 2023-12-03 18:38:37.450446 brave_search-0.1.8/src/brave/types/shared/__init__.py
--rw-r--r--   0        0        0      694 2023-12-03 18:38:37.454543 brave_search-0.1.8/src/brave/types/shared/meta_url.py
--rw-r--r--   0        0        0      936 2024-03-11 21:58:27.127329 brave_search-0.1.8/src/brave/types/shared/thumbnail.py
--rw-r--r--   0        0        0      570 2024-02-21 19:14:28.309913 brave_search-0.1.8/src/brave/types/web/answer.py
--rw-r--r--   0        0        0     1079 2023-12-03 18:38:37.464257 brave_search-0.1.8/src/brave/types/web/article.py
--rw-r--r--   0        0        0      987 2024-03-11 21:58:27.127622 brave_search-0.1.8/src/brave/types/web/book.py
--rw-r--r--   0        0        0      450 2023-12-04 11:59:41.814921 brave_search-0.1.8/src/brave/types/web/button_result.py
--rw-r--r--   0        0        0      274 2023-12-03 18:38:37.469030 brave_search-0.1.8/src/brave/types/web/contact.py
--rw-r--r--   0        0        0      628 2023-12-03 18:38:37.470776 brave_search-0.1.8/src/brave/types/web/data_provider.py
--rw-r--r--   0        0        0      850 2023-12-04 11:59:41.817670 brave_search-0.1.8/src/brave/types/web/deep_result.py
--rw-r--r--   0        0        0     1553 2023-12-04 11:59:41.820137 brave_search-0.1.8/src/brave/types/web/discussions.py
--rw-r--r--   0        0        0     1192 2024-02-21 19:14:28.310974 brave_search-0.1.8/src/brave/types/web/faq.py
--rw-r--r--   0        0        0      840 2023-12-04 11:59:41.823941 brave_search-0.1.8/src/brave/types/web/image.py
--rw-r--r--   0        0        0     3088 2023-12-04 11:59:41.825156 brave_search-0.1.8/src/brave/types/web/info_box.py
--rw-r--r--   0        0        0      729 2023-12-04 11:59:41.826179 brave_search-0.1.8/src/brave/types/web/knowledge_graph.py
--rw-r--r--   0        0        0      356 2023-12-03 18:38:37.481081 brave_search-0.1.8/src/brave/types/web/language.py
--rw-r--r--   0        0        0     2287 2023-12-03 18:38:37.488353 brave_search-0.1.8/src/brave/types/web/location_result.py
--rw-r--r--   0        0        0     1184 2023-12-04 11:59:41.827406 brave_search-0.1.8/src/brave/types/web/mixed_response.py
--rw-r--r--   0        0        0     1164 2023-12-03 18:38:37.489835 brave_search-0.1.8/src/brave/types/web/movie_data.py
--rw-r--r--   0        0        0     1476 2024-03-11 21:58:27.127859 brave_search-0.1.8/src/brave/types/web/news.py
--rw-r--r--   0        0        0      408 2023-12-03 18:38:37.493572 brave_search-0.1.8/src/brave/types/web/offer.py
--rw-r--r--   0        0        0     1009 2023-12-03 18:38:37.495526 brave_search-0.1.8/src/brave/types/web/opening_hours.py
--rw-r--r--   0        0        0      625 2023-12-03 18:38:37.498228 brave_search-0.1.8/src/brave/types/web/person.py
--rw-r--r--   0        0        0      366 2023-12-03 18:38:37.501471 brave_search-0.1.8/src/brave/types/web/picture_results.py
--rw-r--r--   0        0        0      871 2023-12-03 18:38:37.503660 brave_search-0.1.8/src/brave/types/web/postal_address.py
--rw-r--r--   0        0        0      292 2023-12-03 18:38:37.507344 brave_search-0.1.8/src/brave/types/web/price.py
--rw-r--r--   0        0        0      994 2023-12-03 18:38:37.509226 brave_search-0.1.8/src/brave/types/web/product.py
--rw-r--r--   0        0        0      554 2023-12-03 18:38:37.511207 brave_search-0.1.8/src/brave/types/web/profile.py
--rw-r--r--   0        0        0     3043 2023-12-03 18:38:37.517647 brave_search-0.1.8/src/brave/types/web/query.py
--rw-r--r--   0        0        0      713 2023-12-03 18:38:37.521619 brave_search-0.1.8/src/brave/types/web/rating.py
--rw-r--r--   0        0        0     1404 2023-12-04 11:59:41.831251 brave_search-0.1.8/src/brave/types/web/result.py
--rw-r--r--   0        0        0     1719 2023-12-03 18:38:37.526914 brave_search-0.1.8/src/brave/types/web/reviews.py
--rw-r--r--   0        0        0      632 2023-12-03 18:38:37.530555 brave_search-0.1.8/src/brave/types/web/search.py
--rw-r--r--   0        0        0     5648 2024-03-11 21:57:20.959135 brave_search-0.1.8/src/brave/types/web/search_result.py
--rw-r--r--   0        0        0      293 2023-12-03 18:38:37.538160 brave_search-0.1.8/src/brave/types/web/unit.py
--rw-r--r--   0        0        0      929 2023-12-04 11:59:41.833097 brave_search-0.1.8/src/brave/types/web/url.py
--rw-r--r--   0        0        0     1796 2023-12-05 10:37:17.257811 brave_search-0.1.8/src/brave/types/web/videos.py
--rw-r--r--   0        0        0     5458 2024-03-11 21:58:27.128277 brave_search-0.1.8/src/brave/types/web/web_search_response.py
--rw-r--r--   0        0        0     5754 1970-01-01 00:00:00.000000 brave_search-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    10420 2024-03-09 12:31:59.811484 brave_search-0.2.0/LICENSE.MD
+-rw-r--r--   0        0        0     4928 2024-04-27 15:34:11.238498 brave_search-0.2.0/README.md
+-rw-r--r--   0        0        0     4592 2024-04-27 15:36:49.827632 brave_search-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-12-01 12:01:03.058624 brave_search-0.2.0/src/brave/__init__.py
+-rw-r--r--   0        0        0     4442 2023-12-03 18:38:37.425306 brave_search-0.2.0/src/brave/async_brave.py
+-rw-r--r--   0        0        0     6320 2024-03-11 21:58:27.126491 brave_search-0.2.0/src/brave/client.py
+-rw-r--r--   0        0        0      140 2023-12-19 12:18:55.721219 brave_search-0.2.0/src/brave/exceptions.py
+-rw-r--r--   0        0        0     1336 2023-12-19 12:18:55.722403 brave_search-0.2.0/src/brave/goggles/README.md
+-rw-r--r--   0        0        0       25 2023-12-04 15:45:58.439411 brave_search-0.2.0/src/brave/goggles/__init__.py
+-rw-r--r--   0        0        0      169 2023-12-04 15:45:58.442242 brave_search-0.2.0/src/brave/goggles/directory.py
+-rw-r--r--   0        0        0     6614 2023-12-04 15:45:58.448415 brave_search-0.2.0/src/brave/goggles/sample_goggle.goggle
+-rw-r--r--   0        0        0     1115 2023-12-04 17:02:16.473377 brave_search-0.2.0/src/brave/goggles/thought_leadership.goggle
+-rw-r--r--   0        0        0     1375 2024-04-27 15:34:11.259776 brave_search-0.2.0/src/brave/sync.py
+-rw-r--r--   0        0        0      122 2023-12-03 18:38:37.429228 brave_search-0.2.0/src/brave/types/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-03 18:38:37.429267 brave_search-0.2.0/src/brave/types/image/__init__.py
+-rw-r--r--   0        0        0      718 2023-12-03 18:38:37.440675 brave_search-0.2.0/src/brave/types/image/image_query.py
+-rw-r--r--   0        0        0     1100 2023-12-03 18:38:37.443820 brave_search-0.2.0/src/brave/types/image/image_result.py
+-rw-r--r--   0        0        0      556 2023-12-03 18:38:37.447770 brave_search-0.2.0/src/brave/types/image/image_search_response.py
+-rw-r--r--   0        0        0      298 2023-12-03 18:38:37.448297 brave_search-0.2.0/src/brave/types/image/properties.py
+-rw-r--r--   0        0        0     1085 2024-03-11 21:58:27.126882 brave_search-0.2.0/src/brave/types/not_implemented.py
+-rw-r--r--   0        0        0        0 2023-12-03 18:38:37.450446 brave_search-0.2.0/src/brave/types/shared/__init__.py
+-rw-r--r--   0        0        0      694 2023-12-03 18:38:37.454543 brave_search-0.2.0/src/brave/types/shared/meta_url.py
+-rw-r--r--   0        0        0      936 2024-03-11 21:58:27.127329 brave_search-0.2.0/src/brave/types/shared/thumbnail.py
+-rw-r--r--   0        0        0      570 2024-02-21 19:14:28.309913 brave_search-0.2.0/src/brave/types/web/answer.py
+-rw-r--r--   0        0        0     1079 2023-12-03 18:38:37.464257 brave_search-0.2.0/src/brave/types/web/article.py
+-rw-r--r--   0        0        0      987 2024-03-11 21:58:27.127622 brave_search-0.2.0/src/brave/types/web/book.py
+-rw-r--r--   0        0        0      450 2023-12-04 11:59:41.814921 brave_search-0.2.0/src/brave/types/web/button_result.py
+-rw-r--r--   0        0        0      274 2023-12-03 18:38:37.469030 brave_search-0.2.0/src/brave/types/web/contact.py
+-rw-r--r--   0        0        0      628 2023-12-03 18:38:37.470776 brave_search-0.2.0/src/brave/types/web/data_provider.py
+-rw-r--r--   0        0        0      850 2023-12-04 11:59:41.817670 brave_search-0.2.0/src/brave/types/web/deep_result.py
+-rw-r--r--   0        0        0     1553 2023-12-04 11:59:41.820137 brave_search-0.2.0/src/brave/types/web/discussions.py
+-rw-r--r--   0        0        0     1192 2024-02-21 19:14:28.310974 brave_search-0.2.0/src/brave/types/web/faq.py
+-rw-r--r--   0        0        0      840 2023-12-04 11:59:41.823941 brave_search-0.2.0/src/brave/types/web/image.py
+-rw-r--r--   0        0        0     3088 2023-12-04 11:59:41.825156 brave_search-0.2.0/src/brave/types/web/info_box.py
+-rw-r--r--   0        0        0      729 2023-12-04 11:59:41.826179 brave_search-0.2.0/src/brave/types/web/knowledge_graph.py
+-rw-r--r--   0        0        0      356 2023-12-03 18:38:37.481081 brave_search-0.2.0/src/brave/types/web/language.py
+-rw-r--r--   0        0        0     2287 2023-12-03 18:38:37.488353 brave_search-0.2.0/src/brave/types/web/location_result.py
+-rw-r--r--   0        0        0     1184 2023-12-04 11:59:41.827406 brave_search-0.2.0/src/brave/types/web/mixed_response.py
+-rw-r--r--   0        0        0     1164 2023-12-03 18:38:37.489835 brave_search-0.2.0/src/brave/types/web/movie_data.py
+-rw-r--r--   0        0        0     1476 2024-03-11 21:58:27.127859 brave_search-0.2.0/src/brave/types/web/news.py
+-rw-r--r--   0        0        0      408 2023-12-03 18:38:37.493572 brave_search-0.2.0/src/brave/types/web/offer.py
+-rw-r--r--   0        0        0     1009 2023-12-03 18:38:37.495526 brave_search-0.2.0/src/brave/types/web/opening_hours.py
+-rw-r--r--   0        0        0      625 2023-12-03 18:38:37.498228 brave_search-0.2.0/src/brave/types/web/person.py
+-rw-r--r--   0        0        0      366 2023-12-03 18:38:37.501471 brave_search-0.2.0/src/brave/types/web/picture_results.py
+-rw-r--r--   0        0        0      871 2023-12-03 18:38:37.503660 brave_search-0.2.0/src/brave/types/web/postal_address.py
+-rw-r--r--   0        0        0      292 2023-12-03 18:38:37.507344 brave_search-0.2.0/src/brave/types/web/price.py
+-rw-r--r--   0        0        0      994 2023-12-03 18:38:37.509226 brave_search-0.2.0/src/brave/types/web/product.py
+-rw-r--r--   0        0        0      554 2023-12-03 18:38:37.511207 brave_search-0.2.0/src/brave/types/web/profile.py
+-rw-r--r--   0        0        0     3043 2023-12-03 18:38:37.517647 brave_search-0.2.0/src/brave/types/web/query.py
+-rw-r--r--   0        0        0      713 2023-12-03 18:38:37.521619 brave_search-0.2.0/src/brave/types/web/rating.py
+-rw-r--r--   0        0        0     1404 2023-12-04 11:59:41.831251 brave_search-0.2.0/src/brave/types/web/result.py
+-rw-r--r--   0        0        0     1719 2023-12-03 18:38:37.526914 brave_search-0.2.0/src/brave/types/web/reviews.py
+-rw-r--r--   0        0        0      632 2023-12-03 18:38:37.530555 brave_search-0.2.0/src/brave/types/web/search.py
+-rw-r--r--   0        0        0     5648 2024-03-11 21:57:20.959135 brave_search-0.2.0/src/brave/types/web/search_result.py
+-rw-r--r--   0        0        0      293 2023-12-03 18:38:37.538160 brave_search-0.2.0/src/brave/types/web/unit.py
+-rw-r--r--   0        0        0      929 2023-12-04 11:59:41.833097 brave_search-0.2.0/src/brave/types/web/url.py
+-rw-r--r--   0        0        0     1796 2023-12-05 10:37:17.257811 brave_search-0.2.0/src/brave/types/web/videos.py
+-rw-r--r--   0        0        0     5458 2024-03-11 21:58:27.128277 brave_search-0.2.0/src/brave/types/web/web_search_response.py
+-rw-r--r--   0        0        0     5776 1970-01-01 00:00:00.000000 brave_search-0.2.0/PKG-INFO
```

### Comparing `brave_search-0.1.8/LICENSE.MD` & `brave_search-0.2.0/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/README.md` & `brave_search-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Brave Search API
 
 ## Overview
-Python wrapper for the [Brave Search API](https://search.brave.com/api).
+Python wrapper for the [Brave Search API](https://brave.com/search/api/).
 
 Brave Search doesn’t track you or your queries, it's a privacy-preserving alternative to Google Search. It offers many endpoints for developers to build on top of. This module is a wrapper for the Brave Search API.
 
 This repo is under active development, functionality may change.
 If you have any suggestions or requests, please open an issue.
 
 ## Installation
@@ -50,14 +50,27 @@
 brave = AsyncBrave()
 
 query = "cobalt mining"
 num_results = 10
 
 search_results = await brave.search(q=query, count=num_results)
 ```
+
+To return the raw JSON response that has not been validated through the pydantic model use the `raw` flag:
+
+```python
+
+from brave import Brave
+
+query = "George Orwell, 1984"
+num_results = 10
+
+search_results = brave.search(q=query, raw=True)
+```
+
 ## Features
 
 ### Download PDFs:
 
 Use the `download_pdfs` method to download all PDFs found in the search results. This method returns a list of file paths to the downloaded PDFs. You can use Goggles to boost PDFs in your search results.
 
 ```python
@@ -139,26 +152,14 @@
 
 query = "cobalt mining"
 num_results = 10
 
 search_results = brave.search(q=query, goggles_id=thought_leadership, count=num_results)
 ```
 
-To return the raw JSON response that has not been validated through the pydantic model use the `raw` flag:
-
-```python
-
-from brave import Brave
-
-query = "George Orwell, 1984"
-num_results = 10
-
-search_results = brave.search(q=query, raw=True)
-```
-
 ## Local Installation
 
 This package uses Poetry for dependency management. To start developing here, you need to install Poetry
 
 * Follow the instructions on the [official docs](https://python-poetry.org/docs/master/#installing-with-the-official-installer)
 
 Once you have Poetry installed on your system simply run:
```

### Comparing `brave_search-0.1.8/pyproject.toml` & `brave_search-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brave-search"
-version = "0.1.8"
+version = "0.2.0"
 description = "Brave Search API wrapper"
 authors = ["Kayvane Shakerifar"]
 readme = "README.md"
 homepage = "https://github.com/kayvane1/brave-api"
 repository = "https://github.com/kayvane1/brave-api"
 keywords = ['search', 'brave', 'api']  # noqa
 packages = [
@@ -14,15 +14,15 @@
 [tool.poetry.build]
 generate-setup-file = false
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.26.0"
-httpx = "^0.25.2"
+httpx = "^0.24.0||^0.25.2"
 tenacity = "^8.2.3"
 pydantic = "^2.5.2"
 pytest-asyncio = "^0.23.2"
 numpy = "^1.24.4"
 
 [tool.poetry.group.test]
 optional = true
```

### Comparing `brave_search-0.1.8/src/brave/async_brave.py` & `brave_search-0.2.0/src/brave/async_brave.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/client.py` & `brave_search-0.2.0/src/brave/client.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/goggles/README.md` & `brave_search-0.2.0/src/brave/goggles/README.md`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/goggles/sample_goggle.goggle` & `brave_search-0.2.0/src/brave/goggles/sample_goggle.goggle`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/goggles/thought_leadership.goggle` & `brave_search-0.2.0/src/brave/goggles/thought_leadership.goggle`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/sync.py` & `brave_search-0.2.0/src/brave/sync.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,9 +32,11 @@
         headers = self._prepare_headers()
         try:
             response = requests.get(url, headers=headers, params=params)
             response.raise_for_status()  # Raises HTTPError for bad requests
             return response
         except requests.exceptions.HTTPError as e:
             logger.warning(f"HTTP error occurred: {e}")
+            raise e
         except requests.exceptions.RequestException as e:
             logger.warning(f"Request error occurred: {e}")
+            raise e
```

### Comparing `brave_search-0.1.8/src/brave/types/image/image_query.py` & `brave_search-0.2.0/src/brave/types/image/image_query.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/image/image_result.py` & `brave_search-0.2.0/src/brave/types/image/image_result.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/image/image_search_response.py` & `brave_search-0.2.0/src/brave/types/image/image_search_response.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/not_implemented.py` & `brave_search-0.2.0/src/brave/types/not_implemented.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/shared/meta_url.py` & `brave_search-0.2.0/src/brave/types/shared/meta_url.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/shared/thumbnail.py` & `brave_search-0.2.0/src/brave/types/shared/thumbnail.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/answer.py` & `brave_search-0.2.0/src/brave/types/web/answer.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/article.py` & `brave_search-0.2.0/src/brave/types/web/article.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/book.py` & `brave_search-0.2.0/src/brave/types/web/book.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/data_provider.py` & `brave_search-0.2.0/src/brave/types/web/data_provider.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/deep_result.py` & `brave_search-0.2.0/src/brave/types/web/deep_result.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/discussions.py` & `brave_search-0.2.0/src/brave/types/web/discussions.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/faq.py` & `brave_search-0.2.0/src/brave/types/web/faq.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/image.py` & `brave_search-0.2.0/src/brave/types/web/image.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/info_box.py` & `brave_search-0.2.0/src/brave/types/web/info_box.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/knowledge_graph.py` & `brave_search-0.2.0/src/brave/types/web/knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/location_result.py` & `brave_search-0.2.0/src/brave/types/web/location_result.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/mixed_response.py` & `brave_search-0.2.0/src/brave/types/web/mixed_response.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/movie_data.py` & `brave_search-0.2.0/src/brave/types/web/movie_data.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/news.py` & `brave_search-0.2.0/src/brave/types/web/news.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/opening_hours.py` & `brave_search-0.2.0/src/brave/types/web/opening_hours.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/person.py` & `brave_search-0.2.0/src/brave/types/web/person.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/postal_address.py` & `brave_search-0.2.0/src/brave/types/web/postal_address.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/product.py` & `brave_search-0.2.0/src/brave/types/web/product.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/profile.py` & `brave_search-0.2.0/src/brave/types/web/profile.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/query.py` & `brave_search-0.2.0/src/brave/types/web/query.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/rating.py` & `brave_search-0.2.0/src/brave/types/web/rating.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/result.py` & `brave_search-0.2.0/src/brave/types/web/result.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/reviews.py` & `brave_search-0.2.0/src/brave/types/web/reviews.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/search.py` & `brave_search-0.2.0/src/brave/types/web/search.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/search_result.py` & `brave_search-0.2.0/src/brave/types/web/search_result.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/url.py` & `brave_search-0.2.0/src/brave/types/web/url.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/videos.py` & `brave_search-0.2.0/src/brave/types/web/videos.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/src/brave/types/web/web_search_response.py` & `brave_search-0.2.0/src/brave/types/web/web_search_response.py`

 * *Files identical despite different names*

### Comparing `brave_search-0.1.8/PKG-INFO` & `brave_search-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: brave-search
-Version: 0.1.8
+Version: 0.2.0
 Summary: Brave Search API wrapper
 Home-page: https://github.com/kayvane1/brave-api
 Keywords: search,brave,api
 Author: Kayvane Shakerifar
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: httpx (>=0.25.2,<0.26.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0 || >=0.25.2,<0.26.0)
 Requires-Dist: numpy (>=1.24.4,<2.0.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Requires-Dist: pytest-asyncio (>=0.23.2,<0.24.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Project-URL: Repository, https://github.com/kayvane1/brave-api
 Description-Content-Type: text/markdown
 
 # Brave Search API
 
 ## Overview
-Python wrapper for the [Brave Search API](https://search.brave.com/api).
+Python wrapper for the [Brave Search API](https://brave.com/search/api/).
 
 Brave Search doesn’t track you or your queries, it's a privacy-preserving alternative to Google Search. It offers many endpoints for developers to build on top of. This module is a wrapper for the Brave Search API.
 
 This repo is under active development, functionality may change.
 If you have any suggestions or requests, please open an issue.
 
 ## Installation
@@ -72,14 +72,27 @@
 brave = AsyncBrave()
 
 query = "cobalt mining"
 num_results = 10
 
 search_results = await brave.search(q=query, count=num_results)
 ```
+
+To return the raw JSON response that has not been validated through the pydantic model use the `raw` flag:
+
+```python
+
+from brave import Brave
+
+query = "George Orwell, 1984"
+num_results = 10
+
+search_results = brave.search(q=query, raw=True)
+```
+
 ## Features
 
 ### Download PDFs:
 
 Use the `download_pdfs` method to download all PDFs found in the search results. This method returns a list of file paths to the downloaded PDFs. You can use Goggles to boost PDFs in your search results.
 
 ```python
@@ -161,26 +174,14 @@
 
 query = "cobalt mining"
 num_results = 10
 
 search_results = brave.search(q=query, goggles_id=thought_leadership, count=num_results)
 ```
 
-To return the raw JSON response that has not been validated through the pydantic model use the `raw` flag:
-
-```python
-
-from brave import Brave
-
-query = "George Orwell, 1984"
-num_results = 10
-
-search_results = brave.search(q=query, raw=True)
-```
-
 ## Local Installation
 
 This package uses Poetry for dependency management. To start developing here, you need to install Poetry
 
 * Follow the instructions on the [official docs](https://python-poetry.org/docs/master/#installing-with-the-official-installer)
 
 Once you have Poetry installed on your system simply run:
```

