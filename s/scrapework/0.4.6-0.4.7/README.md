# Comparing `tmp/scrapework-0.4.6.tar.gz` & `tmp/scrapework-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapework-0.4.6.tar", max compression
+gzip compressed data, was "scrapework-0.4.7.tar", max compression
```

## Comparing `scrapework-0.4.6.tar` & `scrapework-0.4.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4032 2024-04-17 02:34:41.441785 scrapework-0.4.6/README.md
--rw-r--r--   0        0        0      866 2024-04-17 02:34:53.361707 scrapework-0.4.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/__init__.py
--rw-r--r--   0        0        0     2265 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/cache.py
--rw-r--r--   0        0        0        0 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/core/__init__.py
--rw-r--r--   0        0        0      506 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/core/collector.py
--rw-r--r--   0        0        0      567 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/core/context.py
--rw-r--r--   0        0        0      424 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/core/http_client.py
--rw-r--r--   0        0        0      873 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/core/logger.py
--rw-r--r--   0        0        0     2435 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/handlers.py
--rw-r--r--   0        0        0     3729 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/items.py
--rw-r--r--   0        0        0     2810 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/middleware.py
--rw-r--r--   0        0        0      221 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/module.py
--rw-r--r--   0        0        0      194 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/monitors.py
--rw-r--r--   0        0        0      862 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/observer.py
--rw-r--r--   0        0        0      979 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/parsers.py
--rw-r--r--   0        0        0      546 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/processors.py
--rw-r--r--   0        0        0     3258 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/reporter.py
--rw-r--r--   0        0        0     2854 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/request.py
--rw-r--r--   0        0        0     5730 2024-04-17 02:34:41.441785 scrapework-0.4.6/scrapework/scraper.py
--rw-r--r--   0        0        0     5038 1970-01-01 00:00:00.000000 scrapework-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     4155 2024-04-26 11:37:42.858691 scrapework-0.4.7/README.md
+-rw-r--r--   0        0        0      874 2024-04-26 11:37:52.778712 scrapework-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/__init__.py
+-rw-r--r--   0        0        0     2265 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/cache.py
+-rw-r--r--   0        0        0        0 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/core/__init__.py
+-rw-r--r--   0        0        0      506 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/core/collector.py
+-rw-r--r--   0        0        0      567 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/core/context.py
+-rw-r--r--   0        0        0      424 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/core/http_client.py
+-rw-r--r--   0        0        0      873 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/core/logger.py
+-rw-r--r--   0        0        0     2435 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/handlers.py
+-rw-r--r--   0        0        0     3729 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/items.py
+-rw-r--r--   0        0        0     2810 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/middleware.py
+-rw-r--r--   0        0        0      221 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/module.py
+-rw-r--r--   0        0        0      194 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/monitors.py
+-rw-r--r--   0        0        0      862 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/observer.py
+-rw-r--r--   0        0        0      979 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/parsers.py
+-rw-r--r--   0        0        0      546 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/processors.py
+-rw-r--r--   0        0        0     3258 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/reporter.py
+-rw-r--r--   0        0        0     2854 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/request.py
+-rw-r--r--   0        0        0     5730 2024-04-26 11:37:42.858691 scrapework-0.4.7/scrapework/scraper.py
+-rw-r--r--   0        0        0     5161 1970-01-01 00:00:00.000000 scrapework-0.4.7/PKG-INFO
```

### Comparing `scrapework-0.4.6/README.md` & `scrapework-0.4.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -40,33 +40,36 @@
                 'text': quote.css('span.text::text').get(),
                 'author': quote.css('span small::text').get(),
             }
 
     def process(self, items, config):
         for item in items:
             print(f"Quote: {item['text']}, Author: {item['author']}")
-```
 
-Similar to Scrapy `parse`, the `extract` method is an expected and this is where you define your scraping logic. It's called with the HTTP response of the initial URL.
 
-### Run the Scraper
+scraper = SimpleScraper()
+scraper.run(['http://quotes.toscrape.com'])
+
+```
+
+Similar to Scrapy `parse`, the `extract` method is an expected and this is where you define your scraping logic. It's called with the HTTP response of the initial URL. You can use the `parsel.Selector` object to extract data from the HTML using `css` or `xpath`.
 
 To run the Scraper, you need to create an instance and call the `run` method passing the URLs to scrape:
 
 ```python
 scraper = SimpleScraper()
 scraper.run(['http://quotes.toscrape.com'])
 ```
 
 ### Modules Configuration
 
-Scrapework can be extended using various modules:
+Scrapework can be extended using modules:
 
 - `middleware` to configure the request handling (chache, proxy, ...).
-- `handlers`: comes with various handlers (log, save to file, save to database.)
+- `handlers`: to export the data, save them to file or database.
 - `reporters`: to export and log the scraping events and metadata.
 
 ## Flow
 
 The scraping flow consists of the following steps:
 
 1. **Webpage downloading**: Fetch the webpages using `httpx`. Optionally, use `middleware` to handle requests.
```

### Comparing `scrapework-0.4.6/pyproject.toml` & `scrapework-0.4.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapework"
-version = "v0.4.6"
+version = "v0.4.7"
 description = "simple scraping framework"
 authors = ["Stéphane Busso <stephane.busso@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sbusso/scrapework"
 homepage = "https://github.com/sbusso/scrapework"
 
@@ -21,15 +21,15 @@
 hishel = ">=0.0.24,<0.0.27"
 rich = "^13.7.1"
 fake-useragent = "^1.5.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 pytest = "^8.1.1"
-ruff = "^0.3.4"
+ruff = ">=0.3.4,<0.5.0"
 
 
 [tool.poetry-dynamic-versioning]
 enable = true
 vcs = "git"
 
 [build-system]
```

### Comparing `scrapework-0.4.6/scrapework/cache.py` & `scrapework-0.4.7/scrapework/cache.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.6/scrapework/core/context.py` & `scrapework-0.4.7/scrapework/core/context.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.6/scrapework/core/logger.py` & `scrapework-0.4.7/scrapework/core/logger.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.6/scrapework/handlers.py` & `scrapework-0.4.7/scrapework/handlers.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.6/scrapework/items.py` & `scrapework-0.4.7/scrapework/items.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.6/scrapework/middleware.py` & `scrapework-0.4.7/scrapework/middleware.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.6/scrapework/observer.py` & `scrapework-0.4.7/scrapework/observer.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.6/scrapework/parsers.py` & `scrapework-0.4.7/scrapework/parsers.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.6/scrapework/processors.py` & `scrapework-0.4.7/scrapework/processors.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.6/scrapework/reporter.py` & `scrapework-0.4.7/scrapework/reporter.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.6/scrapework/request.py` & `scrapework-0.4.7/scrapework/request.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.6/scrapework/scraper.py` & `scrapework-0.4.7/scrapework/scraper.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.4.6/PKG-INFO` & `scrapework-0.4.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapework
-Version: 0.4.6
+Version: 0.4.7
 Summary: simple scraping framework
 Home-page: https://github.com/sbusso/scrapework
 License: MIT
 Author: Stéphane Busso
 Author-email: stephane.busso@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -67,33 +67,36 @@
                 'text': quote.css('span.text::text').get(),
                 'author': quote.css('span small::text').get(),
             }
 
     def process(self, items, config):
         for item in items:
             print(f"Quote: {item['text']}, Author: {item['author']}")
-```
 
-Similar to Scrapy `parse`, the `extract` method is an expected and this is where you define your scraping logic. It's called with the HTTP response of the initial URL.
 
-### Run the Scraper
+scraper = SimpleScraper()
+scraper.run(['http://quotes.toscrape.com'])
+
+```
+
+Similar to Scrapy `parse`, the `extract` method is an expected and this is where you define your scraping logic. It's called with the HTTP response of the initial URL. You can use the `parsel.Selector` object to extract data from the HTML using `css` or `xpath`.
 
 To run the Scraper, you need to create an instance and call the `run` method passing the URLs to scrape:
 
 ```python
 scraper = SimpleScraper()
 scraper.run(['http://quotes.toscrape.com'])
 ```
 
 ### Modules Configuration
 
-Scrapework can be extended using various modules:
+Scrapework can be extended using modules:
 
 - `middleware` to configure the request handling (chache, proxy, ...).
-- `handlers`: comes with various handlers (log, save to file, save to database.)
+- `handlers`: to export the data, save them to file or database.
 - `reporters`: to export and log the scraping events and metadata.
 
 ## Flow
 
 The scraping flow consists of the following steps:
 
 1. **Webpage downloading**: Fetch the webpages using `httpx`. Optionally, use `middleware` to handle requests.
```

