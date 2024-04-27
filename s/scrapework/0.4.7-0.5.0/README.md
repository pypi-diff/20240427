# Comparing `tmp/scrapework-0.4.7.tar.gz` & `tmp/scrapework-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapework-0.4.7.tar", max compression
+gzip compressed data, was "scrapework-0.5.0.tar", max compression
```

## Comparing `scrapework-0.4.7.tar` & `scrapework-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4155 2024-04-26 11:37:42.858691 scrapework-0.4.7/README.md
--rw-r--r--   0        0        0      874 2024-04-26 11:37:52.778712 scrapework-0.4.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/__init__.py
--rw-r--r--   0        0        0     2265 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/cache.py
--rw-r--r--   0        0        0        0 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/core/__init__.py
--rw-r--r--   0        0        0      506 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/core/collector.py
--rw-r--r--   0        0        0      567 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/core/context.py
--rw-r--r--   0        0        0      424 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/core/http_client.py
--rw-r--r--   0        0        0      873 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/core/logger.py
--rw-r--r--   0        0        0     2435 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/handlers.py
--rw-r--r--   0        0        0     3729 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/items.py
--rw-r--r--   0        0        0     2810 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/middleware.py
--rw-r--r--   0        0        0      221 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/module.py
--rw-r--r--   0        0        0      194 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/monitors.py
--rw-r--r--   0        0        0      862 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/observer.py
--rw-r--r--   0        0        0      979 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/parsers.py
--rw-r--r--   0        0        0      546 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/processors.py
--rw-r--r--   0        0        0     3258 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/reporter.py
--rw-r--r--   0        0        0     2854 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/request.py
--rw-r--r--   0        0        0     5730 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/scraper.py
--rw-r--r--   0        0        0     5161 1970-01-01 00:00:00.000000 scrapework-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     4204 2024-04-27 04:36:13.284043 scrapework-0.5.0/README.md
+-rw-r--r--   0        0        0      897 2024-04-27 04:36:23.592099 scrapework-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-27 04:36:13.284043 scrapework-0.5.0/scrapework/__init__.py
+-rw-r--r--   0        0        0     2265 2024-04-27 04:36:13.284043 scrapework-0.5.0/scrapework/cache.py
+-rw-r--r--   0        0        0        0 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/core/__init__.py
+-rw-r--r--   0        0        0      506 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/core/collector.py
+-rw-r--r--   0        0        0      567 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/core/context.py
+-rw-r--r--   0        0        0      424 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/core/http_client.py
+-rw-r--r--   0        0        0      873 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/core/logger.py
+-rw-r--r--   0        0        0     2435 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/handlers.py
+-rw-r--r--   0        0        0     3729 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/items.py
+-rw-r--r--   0        0        0     2979 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/middleware.py
+-rw-r--r--   0        0        0      221 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/module.py
+-rw-r--r--   0        0        0      194 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/monitors.py
+-rw-r--r--   0        0        0      862 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/observer.py
+-rw-r--r--   0        0        0      979 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/parsers.py
+-rw-r--r--   0        0        0      546 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/processors.py
+-rw-r--r--   0        0        0     3258 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/reporter.py
+-rw-r--r--   0        0        0     4638 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/request.py
+-rw-r--r--   0        0        0     5901 2024-04-27 04:36:13.288043 scrapework-0.5.0/scrapework/scraper.py
+-rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 scrapework-0.5.0/PKG-INFO
```

### Comparing `scrapework-0.4.7/README.md` & `scrapework-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,20 @@
 
 To run the tests, use the following command:
 
 ```sh
 pytest tests/
 ```
 
+using playwright:
+
+```sh
+playwright install
+```
+
 ## Contributing
 
 Contributions are welcome! Please read the contributing guidelines first.
 
 ## License
 
 Scrapework is licensed under the MIT License.
```

### Comparing `scrapework-0.4.7/pyproject.toml` & `scrapework-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapework"
-version = "v0.4.7"
+version = "v0.5.0"
 description = "simple scraping framework"
 authors = ["Stéphane Busso <stephane.busso@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sbusso/scrapework"
 homepage = "https://github.com/sbusso/scrapework"
 
@@ -17,14 +17,15 @@
 parsel = "^1.9.0"
 courlan = "^1.0.0"
 trafilatura = "^1.8.0"
 httpx = "^0.27.0"
 hishel = ">=0.0.24,<0.0.27"
 rich = "^13.7.1"
 fake-useragent = "^1.5.1"
+playwright = "^1.43.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 pytest = "^8.1.1"
 ruff = ">=0.3.4,<0.5.0"
```

### Comparing `scrapework-0.4.7/scrapework/cache.py` & `scrapework-0.5.0/scrapework/cache.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.7/scrapework/core/context.py` & `scrapework-0.5.0/scrapework/core/context.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.7/scrapework/core/logger.py` & `scrapework-0.5.0/scrapework/core/logger.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.7/scrapework/handlers.py` & `scrapework-0.5.0/scrapework/handlers.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.7/scrapework/items.py` & `scrapework-0.5.0/scrapework/items.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.7/scrapework/middleware.py` & `scrapework-0.5.0/scrapework/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,7 +99,13 @@
         super().__init__()
         self.proxies = proxies
 
     def process_request(self, ctx: Context, request: Request):
         proxy = choice(self.proxies)
         request.proxy = proxy.url
         return request
+
+
+class PlaywrightMiddleware(RequestMiddleware):
+    def process_request(self, ctx: Context, request: Request):
+        request.playwright = True
+        return request
```

### Comparing `scrapework-0.4.7/scrapework/observer.py` & `scrapework-0.5.0/scrapework/observer.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.7/scrapework/parsers.py` & `scrapework-0.5.0/scrapework/parsers.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.7/scrapework/processors.py` & `scrapework-0.5.0/scrapework/processors.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.7/scrapework/reporter.py` & `scrapework-0.5.0/scrapework/reporter.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.7/scrapework/scraper.py` & `scrapework-0.5.0/scrapework/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,19 @@
 
             self.visited_urls.append(url_with_callback.url)
 
             new_items = url_with_callback.extract(ctx, Selector(response.text))
 
             # TODO: self.process(ctx, new_items)
 
-            items += list(new_items)
+            # append new_items to items, Items can be a list or a dict
+            if isinstance(new_items, dict):
+                items.append(new_items)
+            else:
+                items += new_items
 
             iter_end_time = datetime.datetime.now()
             items_count = len(items)
             ctx.collector.set("items_count", items_count)
             ctx.collector.jobs.append(
                 JobCollector(
                     url=url_with_callback.url,
```

### Comparing `scrapework-0.4.7/PKG-INFO` & `scrapework-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapework
-Version: 0.4.7
+Version: 0.5.0
 Summary: simple scraping framework
 Home-page: https://github.com/sbusso/scrapework
 License: MIT
 Author: Stéphane Busso
 Author-email: stephane.busso@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.68,<2.0.0)
 Requires-Dist: courlan (>=1.0.0,<2.0.0)
 Requires-Dist: fake-useragent (>=1.5.1,<2.0.0)
 Requires-Dist: hishel (>=0.0.24,<0.0.27)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: parsel (>=1.9.0,<2.0.0)
+Requires-Dist: playwright (>=1.43.0,<2.0.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: trafilatura (>=1.8.0,<2.0.0)
 Project-URL: Repository, https://github.com/sbusso/scrapework
 Description-Content-Type: text/markdown
@@ -156,14 +157,20 @@
 
 To run the tests, use the following command:
 
 ```sh
 pytest tests/
 ```
 
+using playwright:
+
+```sh
+playwright install
+```
+
 ## Contributing
 
 Contributions are welcome! Please read the contributing guidelines first.
 
 ## License
 
 Scrapework is licensed under the MIT License.
```

