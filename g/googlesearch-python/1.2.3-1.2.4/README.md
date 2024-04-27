# Comparing `tmp/googlesearch-python-1.2.3.tar.gz` & `tmp/googlesearch_python-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googlesearch-python-1.2.3.tar", last modified: Tue Apr  4 16:57:27 2023, max compression
+gzip compressed data, was "googlesearch_python-1.2.4.tar", last modified: Sat Apr 27 05:37:33 2024, max compression
```

## Comparing `googlesearch-python-1.2.3.tar` & `googlesearch_python-1.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-04 16:57:27.691681 googlesearch-python-1.2.3/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2023-04-04 04:00:46.000000 googlesearch-python-1.2.3/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2023-04-04 04:12:13.000000 googlesearch-python-1.2.3/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1980 2023-04-04 16:57:27.691681 googlesearch-python-1.2.3/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1503 2023-04-04 04:00:46.000000 googlesearch-python-1.2.3/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-04 16:57:27.687681 googlesearch-python-1.2.3/googlesearch/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2259 2023-04-04 16:56:47.000000 googlesearch-python-1.2.3/googlesearch/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      885 2023-04-04 16:56:58.000000 googlesearch-python-1.2.3/googlesearch/user_agents.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-04 16:57:27.691681 googlesearch-python-1.2.3/googlesearch_python.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1980 2023-04-04 16:57:27.000000 googlesearch-python-1.2.3/googlesearch_python.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      332 2023-04-04 16:57:27.000000 googlesearch-python-1.2.3/googlesearch_python.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-04 16:57:27.000000 googlesearch-python-1.2.3/googlesearch_python.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       35 2023-04-04 16:57:27.000000 googlesearch-python-1.2.3/googlesearch_python.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-04-04 16:57:27.000000 googlesearch-python-1.2.3/googlesearch_python.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       35 2023-04-04 04:00:46.000000 googlesearch-python-1.2.3/requirements.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      103 2023-04-04 16:57:27.691681 googlesearch-python-1.2.3/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      870 2023-04-04 16:57:15.000000 googlesearch-python-1.2.3/setup.py
+drwxr-xr-x   0 nv         (501) staff       (20)        0 2024-04-27 05:37:33.352836 googlesearch_python-1.2.4/
+-rw-r--r--   0 nv         (501) staff       (20)     1060 2024-04-27 05:21:17.000000 googlesearch_python-1.2.4/LICENSE
+-rw-r--r--   0 nv         (501) staff       (20)       25 2024-04-27 05:21:17.000000 googlesearch_python-1.2.4/MANIFEST.in
+-rw-r--r--   0 nv         (501) staff       (20)     2601 2024-04-27 05:37:33.352763 googlesearch_python-1.2.4/PKG-INFO
+-rw-r--r--   0 nv         (501) staff       (20)     2060 2024-04-27 05:34:18.000000 googlesearch_python-1.2.4/README.md
+drwxr-xr-x   0 nv         (501) staff       (20)        0 2024-04-27 05:37:33.351620 googlesearch_python-1.2.4/googlesearch/
+-rw-r--r--   0 nv         (501) staff       (20)     2538 2024-04-27 05:34:19.000000 googlesearch_python-1.2.4/googlesearch/__init__.py
+-rw-r--r--   0 nv         (501) staff       (20)      885 2024-04-27 05:21:17.000000 googlesearch_python-1.2.4/googlesearch/user_agents.py
+drwxr-xr-x   0 nv         (501) staff       (20)        0 2024-04-27 05:37:33.352563 googlesearch_python-1.2.4/googlesearch_python.egg-info/
+-rw-r--r--   0 nv         (501) staff       (20)     2601 2024-04-27 05:37:33.000000 googlesearch_python-1.2.4/googlesearch_python.egg-info/PKG-INFO
+-rw-r--r--   0 nv         (501) staff       (20)      332 2024-04-27 05:37:33.000000 googlesearch_python-1.2.4/googlesearch_python.egg-info/SOURCES.txt
+-rw-r--r--   0 nv         (501) staff       (20)        1 2024-04-27 05:37:33.000000 googlesearch_python-1.2.4/googlesearch_python.egg-info/dependency_links.txt
+-rw-r--r--   0 nv         (501) staff       (20)       35 2024-04-27 05:37:33.000000 googlesearch_python-1.2.4/googlesearch_python.egg-info/requires.txt
+-rw-r--r--   0 nv         (501) staff       (20)       13 2024-04-27 05:37:33.000000 googlesearch_python-1.2.4/googlesearch_python.egg-info/top_level.txt
+-rw-r--r--   0 nv         (501) staff       (20)       35 2024-04-27 05:21:17.000000 googlesearch_python-1.2.4/requirements.txt
+-rw-r--r--   0 nv         (501) staff       (20)      103 2024-04-27 05:37:33.353054 googlesearch_python-1.2.4/setup.cfg
+-rw-r--r--   0 nv         (501) staff       (20)      870 2024-04-27 05:36:01.000000 googlesearch_python-1.2.4/setup.py
```

### Comparing `googlesearch-python-1.2.3/LICENSE` & `googlesearch_python-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `googlesearch-python-1.2.3/PKG-INFO` & `googlesearch_python-1.2.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: googlesearch-python
-Version: 1.2.3
+Version: 1.2.4
 Summary: A Python library for scraping the Google search engine.
 Home-page: https://github.com/Nv7-GitHub/googlesearch
 Author: Nishant Vikramaditya
 Author-email: junk4Nv7@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: beautifulsoup4>=4.9
+Requires-Dist: requests>=2.20
 
 # googlesearch
 googlesearch is a Python library for searching Google, easily. googlesearch uses requests and BeautifulSoup4 to scrape Google. 
 
 ## Installation
 To install, run the following command:
 ```bash
@@ -35,14 +37,19 @@
 search("Google", num_results=100)
 ```
 In addition, you can change the language google searches in. For example, to get results in French run the following program:
 ```python
 from googlesearch import search
 search("Google", lang="fr")
 ```
+If you want to turn off the safe search function (this function is on by default), you can do this:
+```python
+from googlesearch import search
+search("Google", safe=None)
+```
 To extract more information, such as the description or the result URL, use an advanced search:
 ```python
 from googlesearch import search
 search("Google", advanced=True)
 # Returns a list of SearchResult
 # Properties:
 # - title
@@ -50,7 +57,18 @@
 # - description
 ```
 If requesting more than 100 results, googlesearch will send multiple requests to go through the pages. To increase the time between these requests, use `sleep_interval`:
 ```python
 from googlesearch import search
 search("Google", sleep_interval=5, num_results=200)
 ```
+
+If you are using a HTTP Rotating Proxy which requires you to install their CA Certificate, you can simply add `ssl_verify=False` in the `search()` method to avoid SSL Verification.
+```python
+from googlesearch import search
+
+proxy = 'http://API:@proxy.host.com:8080/'
+
+j = search("proxy test", num_results=100, lang="en", proxy=proxy, ssl_verify=False)
+for i in j:
+    print(i)
+```
```

### Comparing `googlesearch-python-1.2.3/README.md` & `googlesearch_python-1.2.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -21,22 +21,38 @@
 search("Google", num_results=100)
 ```
 In addition, you can change the language google searches in. For example, to get results in French run the following program:
 ```python
 from googlesearch import search
 search("Google", lang="fr")
 ```
+If you want to turn off the safe search function (this function is on by default), you can do this:
+```python
+from googlesearch import search
+search("Google", safe=None)
+```
 To extract more information, such as the description or the result URL, use an advanced search:
 ```python
 from googlesearch import search
 search("Google", advanced=True)
 # Returns a list of SearchResult
 # Properties:
 # - title
 # - url
 # - description
 ```
 If requesting more than 100 results, googlesearch will send multiple requests to go through the pages. To increase the time between these requests, use `sleep_interval`:
 ```python
 from googlesearch import search
 search("Google", sleep_interval=5, num_results=200)
-```
+```
+
+If you are using a HTTP Rotating Proxy which requires you to install their CA Certificate, you can simply add `ssl_verify=False` in the `search()` method to avoid SSL Verification.
+```python
+from googlesearch import search
+
+proxy = 'http://API:@proxy.host.com:8080/'
+
+j = search("proxy test", num_results=100, lang="en", proxy=proxy, ssl_verify=False)
+for i in j:
+    print(i)
+```
```

### Comparing `googlesearch-python-1.2.3/googlesearch/__init__.py` & `googlesearch_python-1.2.4/googlesearch/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """googlesearch is a Python library for searching Google, easily."""
 from time import sleep
 from bs4 import BeautifulSoup
 from requests import get
 from .user_agents import get_useragent
+import urllib
 
 
-def _req(term, results, lang, start, proxies, timeout):
+def _req(term, results, lang, start, proxies, timeout, safe, ssl_verify):
     resp = get(
         url="https://www.google.com/search",
         headers={
             "User-Agent": get_useragent()
         },
         params={
             "q": term,
             "num": results + 2,  # Prevents multiple requests
             "hl": lang,
             "start": start,
+            "safe": safe,
         },
         proxies=proxies,
         timeout=timeout,
+        verify=ssl_verify,
     )
     resp.raise_for_status()
     return resp
 
 
 class SearchResult:
     def __init__(self, url, title, description):
@@ -30,37 +33,39 @@
         self.title = title
         self.description = description
 
     def __repr__(self):
         return f"SearchResult(url={self.url}, title={self.title}, description={self.description})"
 
 
-def search(term, num_results=10, lang="en", proxy=None, advanced=False, sleep_interval=0, timeout=5):
+def search(term, num_results=10, lang="en", proxy=None, advanced=False, sleep_interval=0, timeout=5, safe="active", ssl_verify=None):
     """Search the Google search engine"""
 
-    escaped_term = term.replace(" ", "+")
+    escaped_term = urllib.parse.quote_plus(term) # make 'site:xxx.xxx.xxx ' works.
 
     # Proxy
     proxies = None
     if proxy:
         if proxy.startswith("https"):
             proxies = {"https": proxy}
         else:
             proxies = {"http": proxy}
 
     # Fetch
     start = 0
     while start < num_results:
         # Send request
         resp = _req(escaped_term, num_results - start,
-                    lang, start, proxies, timeout)
+                    lang, start, proxies, timeout, safe, ssl_verify)
 
         # Parse
         soup = BeautifulSoup(resp.text, "html.parser")
         result_block = soup.find_all("div", attrs={"class": "g"})
+        if len(result_block) ==0:
+            start += 1
         for result in result_block:
             # Find link, title, description
             link = result.find("a", href=True)
             title = result.find("h3")
             description_box = result.find(
                 "div", {"style": "-webkit-line-clamp:2"})
             if description_box:
@@ -68,7 +73,10 @@
                 if link and title and description:
                     start += 1
                     if advanced:
                         yield SearchResult(link["href"], title.text, description)
                     else:
                         yield link["href"]
         sleep(sleep_interval)
+
+        if start == 0:
+            return []
```

### Comparing `googlesearch-python-1.2.3/googlesearch/user_agents.py` & `googlesearch_python-1.2.4/googlesearch/user_agents.py`

 * *Files identical despite different names*

### Comparing `googlesearch-python-1.2.3/googlesearch_python.egg-info/PKG-INFO` & `googlesearch_python-1.2.4/googlesearch_python.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: googlesearch-python
-Version: 1.2.3
+Version: 1.2.4
 Summary: A Python library for scraping the Google search engine.
 Home-page: https://github.com/Nv7-GitHub/googlesearch
 Author: Nishant Vikramaditya
 Author-email: junk4Nv7@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: beautifulsoup4>=4.9
+Requires-Dist: requests>=2.20
 
 # googlesearch
 googlesearch is a Python library for searching Google, easily. googlesearch uses requests and BeautifulSoup4 to scrape Google. 
 
 ## Installation
 To install, run the following command:
 ```bash
@@ -35,14 +37,19 @@
 search("Google", num_results=100)
 ```
 In addition, you can change the language google searches in. For example, to get results in French run the following program:
 ```python
 from googlesearch import search
 search("Google", lang="fr")
 ```
+If you want to turn off the safe search function (this function is on by default), you can do this:
+```python
+from googlesearch import search
+search("Google", safe=None)
+```
 To extract more information, such as the description or the result URL, use an advanced search:
 ```python
 from googlesearch import search
 search("Google", advanced=True)
 # Returns a list of SearchResult
 # Properties:
 # - title
@@ -50,7 +57,18 @@
 # - description
 ```
 If requesting more than 100 results, googlesearch will send multiple requests to go through the pages. To increase the time between these requests, use `sleep_interval`:
 ```python
 from googlesearch import search
 search("Google", sleep_interval=5, num_results=200)
 ```
+
+If you are using a HTTP Rotating Proxy which requires you to install their CA Certificate, you can simply add `ssl_verify=False` in the `search()` method to avoid SSL Verification.
+```python
+from googlesearch import search
+
+proxy = 'http://API:@proxy.host.com:8080/'
+
+j = search("proxy test", num_results=100, lang="en", proxy=proxy, ssl_verify=False)
+for i in j:
+    print(i)
+```
```

### Comparing `googlesearch-python-1.2.3/setup.py` & `googlesearch_python-1.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r", encoding='UTF-8') as fh:
     requirements = fh.read().split("\n")
 
 setup(
     name="googlesearch-python",
-    version="1.2.3",
+    version="1.2.4",
     author="Nishant Vikramaditya",
     author_email="junk4Nv7@gmail.com",
     description="A Python library for scraping the Google search engine.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nv7-GitHub/googlesearch",
     packages=["googlesearch"],
```

