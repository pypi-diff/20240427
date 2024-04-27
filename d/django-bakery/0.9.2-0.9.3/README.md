# Comparing `tmp/django-bakery-0.9.2.tar.gz` & `tmp/django-bakery-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-bakery-0.9.2.tar", last modified: Sun Apr  2 22:00:22 2017, max compression
+gzip compressed data, was "dist/django-bakery-0.9.3.tar", last modified: Wed Apr 12 19:18:15 2017, max compression
```

## Comparing `django-bakery-0.9.2.tar` & `django-bakery-0.9.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 palewire  (1001) palewire  (1001)        0 2017-04-02 22:00:22.000000 django-bakery-0.9.2/
-drwxrwxr-x   0 palewire  (1001) palewire  (1001)        0 2017-04-02 22:00:22.000000 django-bakery-0.9.2/bakery/
--rw-rw-r--   0 palewire  (1001) palewire  (1001)      271 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/static_urls.py
--rw-rw-r--   0 palewire  (1001) palewire  (1001)      855 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/__init__.py
-drwxrwxr-x   0 palewire  (1001) palewire  (1001)        0 2017-04-02 22:00:22.000000 django-bakery-0.9.2/bakery/views/
--rw-rw-r--   0 palewire  (1001) palewire  (1001)    10680 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/views/dates.py
--rw-rw-r--   0 palewire  (1001) palewire  (1001)      635 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/views/__init__.py
--rw-rw-r--   0 palewire  (1001) palewire  (1001)     2752 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/views/detail.py
--rw-rw-r--   0 palewire  (1001) palewire  (1001)     1447 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/views/list.py
--rw-rw-r--   0 palewire  (1001) palewire  (1001)     6076 2017-04-02 21:52:18.000000 django-bakery-0.9.2/bakery/views/base.py
--rw-rw-r--   0 palewire  (1001) palewire  (1001)     6820 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/models.py
-drwxrwxr-x   0 palewire  (1001) palewire  (1001)        0 2017-04-02 22:00:22.000000 django-bakery-0.9.2/bakery/tests/
--rw-rw-r--   0 palewire  (1001) palewire  (1001)    17634 2017-04-02 21:40:55.000000 django-bakery-0.9.2/bakery/tests/__init__.py
-drwxrwxr-x   0 palewire  (1001) palewire  (1001)        0 2017-04-02 22:00:22.000000 django-bakery-0.9.2/bakery/tests/media/
--rw-rw-r--   0 palewire  (1001) palewire  (1001)       17 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/tests/media/bar.js
-drwxrwxr-x   0 palewire  (1001) palewire  (1001)        0 2017-04-02 22:00:22.000000 django-bakery-0.9.2/bakery/tests/templates/
--rw-rw-r--   0 palewire  (1001) palewire  (1001)       16 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/tests/templates/404.html
--rw-rw-r--   0 palewire  (1001) palewire  (1001)       13 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/tests/templates/indexview.html
--rw-rw-r--   0 palewire  (1001) palewire  (1001)       13 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/tests/templates/monthview.html
--rw-rw-r--   0 palewire  (1001) palewire  (1001)       13 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/tests/templates/yearview.html
--rw-rw-r--   0 palewire  (1001) palewire  (1001)       22 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/tests/templates/jsonview.json
--rw-rw-r--   0 palewire  (1001) palewire  (1001)       13 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/tests/templates/listview.html
--rw-rw-r--   0 palewire  (1001) palewire  (1001)       13 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/tests/templates/dayview.html
--rw-rw-r--   0 palewire  (1001) palewire  (1001)       14 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/tests/templates/templateview.html
--rw-rw-r--   0 palewire  (1001) palewire  (1001)       13 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/tests/templates/detailview.html
-drwxrwxr-x   0 palewire  (1001) palewire  (1001)        0 2017-04-02 22:00:22.000000 django-bakery-0.9.2/bakery/tests/static/
--rw-rw-r--   0 palewire  (1001) palewire  (1001)       14 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/tests/static/robots.txt
--rw-rw-r--   0 palewire  (1001) palewire  (1001)       12 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/tests/static/foo.bar
-drwxrwxr-x   0 palewire  (1001) palewire  (1001)        0 2017-04-02 22:00:22.000000 django-bakery-0.9.2/bakery/tests/static/djcelery/
--rw-rw-r--   0 palewire  (1001) palewire  (1001)       82 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/tests/static/djcelery/style.css
--rw-rw-r--   0 palewire  (1001) palewire  (1001)    15086 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/tests/static/favicon.ico
--rw-rw-r--   0 palewire  (1001) palewire  (1001)       24 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/tests/static/test.css
--rw-rw-r--   0 palewire  (1001) palewire  (1001)     2264 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/tasks.py
--rw-rw-r--   0 palewire  (1001) palewire  (1001)      783 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/feeds.py
--rw-rw-r--   0 palewire  (1001) palewire  (1001)     5652 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/static_views.py
-drwxrwxr-x   0 palewire  (1001) palewire  (1001)        0 2017-04-02 22:00:22.000000 django-bakery-0.9.2/bakery/management/
--rw-rw-r--   0 palewire  (1001) palewire  (1001)        0 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/management/__init__.py
-drwxrwxr-x   0 palewire  (1001) palewire  (1001)        0 2017-04-02 22:00:22.000000 django-bakery-0.9.2/bakery/management/commands/
--rw-rw-r--   0 palewire  (1001) palewire  (1001)      375 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/management/commands/unbuild.py
--rw-rw-r--   0 palewire  (1001) palewire  (1001)      393 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/management/commands/buildserver.py
--rw-rw-r--   0 palewire  (1001) palewire  (1001)     3228 2017-04-02 21:40:55.000000 django-bakery-0.9.2/bakery/management/commands/__init__.py
--rw-rw-r--   0 palewire  (1001) palewire  (1001)    11519 2017-04-02 21:40:55.000000 django-bakery-0.9.2/bakery/management/commands/publish.py
--rw-rw-r--   0 palewire  (1001) palewire  (1001)     8429 2017-04-02 21:40:55.000000 django-bakery-0.9.2/bakery/management/commands/build.py
--rw-rw-r--   0 palewire  (1001) palewire  (1001)     1413 2017-04-02 18:03:07.000000 django-bakery-0.9.2/bakery/management/commands/unpublish.py
--rw-rw-r--   0 palewire  (1001) palewire  (1001)      134 2017-04-02 22:00:22.000000 django-bakery-0.9.2/setup.cfg
--rw-rw-r--   0 palewire  (1001) palewire  (1001)     4155 2017-04-02 21:56:32.000000 django-bakery-0.9.2/setup.py
--rw-rw-r--   0 palewire  (1001) palewire  (1001)      859 2017-04-02 22:00:22.000000 django-bakery-0.9.2/PKG-INFO
--rw-rw-r--   0 palewire  (1001) palewire  (1001)      139 2017-04-02 18:03:07.000000 django-bakery-0.9.2/MANIFEST.in
--rw-rw-r--   0 palewire  (1001) palewire  (1001)     1741 2017-04-02 18:03:07.000000 django-bakery-0.9.2/README.md
-drwxrwxr-x   0 palewire  (1001) palewire  (1001)        0 2017-04-02 22:00:22.000000 django-bakery-0.9.2/django_bakery.egg-info/
--rw-rw-r--   0 palewire  (1001) palewire  (1001)        7 2017-04-02 22:00:22.000000 django-bakery-0.9.2/django_bakery.egg-info/top_level.txt
--rw-rw-r--   0 palewire  (1001) palewire  (1001)      859 2017-04-02 22:00:22.000000 django-bakery-0.9.2/django_bakery.egg-info/PKG-INFO
--rw-rw-r--   0 palewire  (1001) palewire  (1001)       23 2017-04-02 22:00:22.000000 django-bakery-0.9.2/django_bakery.egg-info/requires.txt
--rw-rw-r--   0 palewire  (1001) palewire  (1001)     1257 2017-04-02 22:00:22.000000 django-bakery-0.9.2/django_bakery.egg-info/SOURCES.txt
--rw-rw-r--   0 palewire  (1001) palewire  (1001)        1 2017-04-02 22:00:22.000000 django-bakery-0.9.2/django_bakery.egg-info/dependency_links.txt
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2017-04-12 19:18:15.000000 django-bakery-0.9.3/
+-rw-r--r--   0 ben       (1000) ben       (1000)      859 2017-04-12 19:18:15.000000 django-bakery-0.9.3/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)      155 2017-04-12 19:18:15.000000 django-bakery-0.9.3/setup.cfg
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1741 2015-08-14 20:50:41.000000 django-bakery-0.9.3/README.md
+-rw-r--r--   0 ben       (1000) ben       (1000)     4155 2017-04-12 19:17:20.000000 django-bakery-0.9.3/setup.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)      139 2015-08-14 20:50:41.000000 django-bakery-0.9.3/MANIFEST.in
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2017-04-12 19:18:15.000000 django-bakery-0.9.3/django_bakery.egg-info/
+-rw-rw-r--   0 ben       (1000) ben       (1000)      859 2017-04-12 19:18:15.000000 django-bakery-0.9.3/django_bakery.egg-info/PKG-INFO
+-rw-rw-r--   0 ben       (1000) ben       (1000)        7 2017-04-12 19:18:15.000000 django-bakery-0.9.3/django_bakery.egg-info/top_level.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)        1 2017-04-12 19:18:15.000000 django-bakery-0.9.3/django_bakery.egg-info/dependency_links.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)       23 2017-04-12 19:18:15.000000 django-bakery-0.9.3/django_bakery.egg-info/requires.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1257 2017-04-12 19:18:15.000000 django-bakery-0.9.3/django_bakery.egg-info/SOURCES.txt
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2017-04-12 19:18:15.000000 django-bakery-0.9.3/bakery/
+-rw-rw-r--   0 ben       (1000) ben       (1000)      271 2016-08-04 22:36:33.000000 django-bakery-0.9.3/bakery/static_urls.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     2264 2015-08-14 20:50:41.000000 django-bakery-0.9.3/bakery/tasks.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)      855 2016-09-01 01:27:28.000000 django-bakery-0.9.3/bakery/__init__.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2017-04-12 19:18:15.000000 django-bakery-0.9.3/bakery/tests/
+-rw-r--r--   0 ben       (1000) ben       (1000)    17741 2017-04-12 17:28:52.000000 django-bakery-0.9.3/bakery/tests/__init__.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2017-04-12 19:18:15.000000 django-bakery-0.9.3/bakery/tests/templates/
+-rw-rw-r--   0 ben       (1000) ben       (1000)       22 2015-08-14 20:50:41.000000 django-bakery-0.9.3/bakery/tests/templates/jsonview.json
+-rw-rw-r--   0 ben       (1000) ben       (1000)       13 2016-03-27 05:31:36.000000 django-bakery-0.9.3/bakery/tests/templates/dayview.html
+-rw-rw-r--   0 ben       (1000) ben       (1000)       13 2015-08-14 20:50:41.000000 django-bakery-0.9.3/bakery/tests/templates/detailview.html
+-rw-rw-r--   0 ben       (1000) ben       (1000)       13 2016-03-27 05:31:36.000000 django-bakery-0.9.3/bakery/tests/templates/yearview.html
+-rw-rw-r--   0 ben       (1000) ben       (1000)       16 2015-08-14 20:50:41.000000 django-bakery-0.9.3/bakery/tests/templates/404.html
+-rw-rw-r--   0 ben       (1000) ben       (1000)       13 2015-08-14 20:50:41.000000 django-bakery-0.9.3/bakery/tests/templates/listview.html
+-rw-rw-r--   0 ben       (1000) ben       (1000)       13 2016-03-27 05:31:36.000000 django-bakery-0.9.3/bakery/tests/templates/monthview.html
+-rw-rw-r--   0 ben       (1000) ben       (1000)       14 2015-08-14 20:50:41.000000 django-bakery-0.9.3/bakery/tests/templates/templateview.html
+-rw-rw-r--   0 ben       (1000) ben       (1000)       13 2016-03-27 05:31:36.000000 django-bakery-0.9.3/bakery/tests/templates/indexview.html
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2017-04-12 19:18:15.000000 django-bakery-0.9.3/bakery/tests/static/
+-rw-rw-r--   0 ben       (1000) ben       (1000)       12 2015-08-14 20:50:41.000000 django-bakery-0.9.3/bakery/tests/static/foo.bar
+-rw-rw-r--   0 ben       (1000) ben       (1000)       14 2015-08-14 20:50:41.000000 django-bakery-0.9.3/bakery/tests/static/robots.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)    15086 2015-08-14 20:50:41.000000 django-bakery-0.9.3/bakery/tests/static/favicon.ico
+-rw-rw-r--   0 ben       (1000) ben       (1000)       24 2015-08-14 20:50:41.000000 django-bakery-0.9.3/bakery/tests/static/test.css
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2017-04-12 19:18:15.000000 django-bakery-0.9.3/bakery/tests/static/djcelery/
+-rw-rw-r--   0 ben       (1000) ben       (1000)       82 2015-08-14 20:50:41.000000 django-bakery-0.9.3/bakery/tests/static/djcelery/style.css
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2017-04-12 19:18:15.000000 django-bakery-0.9.3/bakery/tests/media/
+-rw-rw-r--   0 ben       (1000) ben       (1000)       17 2015-08-14 20:50:41.000000 django-bakery-0.9.3/bakery/tests/media/bar.js
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2017-04-12 19:18:15.000000 django-bakery-0.9.3/bakery/management/
+-rw-rw-r--   0 ben       (1000) ben       (1000)        0 2015-08-14 20:50:41.000000 django-bakery-0.9.3/bakery/management/__init__.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2017-04-12 19:18:15.000000 django-bakery-0.9.3/bakery/management/commands/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1413 2017-03-24 18:16:22.000000 django-bakery-0.9.3/bakery/management/commands/unpublish.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     8429 2017-03-30 16:53:57.000000 django-bakery-0.9.3/bakery/management/commands/build.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     3228 2017-03-31 20:09:50.000000 django-bakery-0.9.3/bakery/management/commands/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    11519 2017-03-31 17:45:58.000000 django-bakery-0.9.3/bakery/management/commands/publish.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)      375 2015-08-14 20:50:41.000000 django-bakery-0.9.3/bakery/management/commands/unbuild.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)      393 2015-08-14 20:50:41.000000 django-bakery-0.9.3/bakery/management/commands/buildserver.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      783 2017-02-20 20:31:24.000000 django-bakery-0.9.3/bakery/feeds.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     6820 2016-03-27 05:31:36.000000 django-bakery-0.9.3/bakery/models.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2017-04-12 19:18:15.000000 django-bakery-0.9.3/bakery/views/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1447 2017-02-20 20:31:24.000000 django-bakery-0.9.3/bakery/views/list.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)      635 2016-03-27 05:31:36.000000 django-bakery-0.9.3/bakery/views/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     2752 2017-03-24 00:03:52.000000 django-bakery-0.9.3/bakery/views/detail.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     6713 2017-04-12 18:55:10.000000 django-bakery-0.9.3/bakery/views/base.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    10680 2017-03-24 00:03:52.000000 django-bakery-0.9.3/bakery/views/dates.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     5652 2017-02-20 20:31:24.000000 django-bakery-0.9.3/bakery/static_views.py
```

### Comparing `django-bakery-0.9.2/bakery/__init__.py` & `django-bakery-0.9.3/bakery/__init__.py`

 * *Files identical despite different names*

### Comparing `django-bakery-0.9.2/bakery/views/dates.py` & `django-bakery-0.9.3/bakery/views/dates.py`

 * *Files identical despite different names*

### Comparing `django-bakery-0.9.2/bakery/views/__init__.py` & `django-bakery-0.9.3/bakery/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-bakery-0.9.2/bakery/views/detail.py` & `django-bakery-0.9.3/bakery/views/detail.py`

 * *Files identical despite different names*

### Comparing `django-bakery-0.9.2/bakery/views/list.py` & `django-bakery-0.9.3/bakery/views/list.py`

 * *Files identical despite different names*

### Comparing `django-bakery-0.9.2/bakery/views/base.py` & `django-bakery-0.9.3/bakery/views/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import sys
 import gzip
 import logging
 import mimetypes
 from django.conf import settings
 from bakery import DEFAULT_GZIP_CONTENT_TYPES
 from django.test.client import RequestFactory
+from bakery.management.commands import get_s3_client
 from django.views.generic import RedirectView, TemplateView
 from django.core.urlresolvers import reverse, NoReverseMatch
 logger = logging.getLogger(__name__)
 
 
 class BuildableMixin(object):
     """
@@ -188,7 +189,25 @@
             try:
                 url = reverse(self.pattern_name, args=args, kwargs=kwargs)
             except NoReverseMatch:
                 return None
         else:
             return None
         return url
+
+    def post_publish(self, bucket):
+        logger.debug("Adding S3 redirect header from {} to in {} to {}".format(
+            self.build_path,
+            bucket.name,
+            self.get_redirect_url()
+        ))
+        s3_client, s3_resource = get_s3_client()
+        s3_client.copy_object(
+            ACL='public-read',
+            Bucket=bucket.name,
+            CopySource={
+                 'Bucket': bucket.name,
+                 'Key': self.build_path
+            },
+            Key=self.build_path,
+            WebsiteRedirectLocation=self.get_redirect_url()
+        )
```

### Comparing `django-bakery-0.9.2/bakery/models.py` & `django-bakery-0.9.3/bakery/models.py`

 * *Files identical despite different names*

### Comparing `django-bakery-0.9.2/bakery/tests/__init__.py` & `django-bakery-0.9.3/bakery/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,14 +264,16 @@
         v.build()
         MockRedirectView().build()
         build_path = os.path.join(
             settings.BUILD_DIR,
             "detail/badurl.html"
         )
         self.assertTrue(os.path.exists(build_path))
+        # with mock_s3():
+        #     MockRedirectView().post_publish(settings.AWS_BUCKET_NAME)
 
     def test_404_view(self):
         v = views.Buildable404View()
         v.build_method
         v.build()
         build_path = os.path.join(settings.BUILD_DIR, '404.html')
         self.assertTrue(os.path.exists(build_path))
@@ -345,15 +347,16 @@
     def _create_bucket(self):
         s3 = boto3.resource('s3')
         s3.Bucket(settings.AWS_BUCKET_NAME).create()
 
     def _get_bucket_objects(self):
         s3_client, s3_resource = get_s3_client()
         return s3_client.list_objects_v2(
-            Bucket=settings.AWS_BUCKET_NAME).get('Contents', [])
+            Bucket=settings.AWS_BUCKET_NAME
+        ).get('Contents', [])
 
     def test_publish_cmd(self):
         with mock_s3():
             self._create_bucket()
             call_command("build")
             call_command("publish", no_pooling=True, verbosity=3)
             local_file_list = []
```

### Comparing `django-bakery-0.9.2/bakery/tests/static/favicon.ico` & `django-bakery-0.9.3/bakery/tests/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-bakery-0.9.2/bakery/tasks.py` & `django-bakery-0.9.3/bakery/tasks.py`

 * *Files identical despite different names*

### Comparing `django-bakery-0.9.2/bakery/feeds.py` & `django-bakery-0.9.3/bakery/feeds.py`

 * *Files identical despite different names*

### Comparing `django-bakery-0.9.2/bakery/static_views.py` & `django-bakery-0.9.3/bakery/static_views.py`

 * *Files identical despite different names*

### Comparing `django-bakery-0.9.2/bakery/management/commands/__init__.py` & `django-bakery-0.9.3/bakery/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django-bakery-0.9.2/bakery/management/commands/publish.py` & `django-bakery-0.9.3/bakery/management/commands/publish.py`

 * *Files identical despite different names*

### Comparing `django-bakery-0.9.2/bakery/management/commands/build.py` & `django-bakery-0.9.3/bakery/management/commands/build.py`

 * *Files identical despite different names*

### Comparing `django-bakery-0.9.2/bakery/management/commands/unpublish.py` & `django-bakery-0.9.3/bakery/management/commands/unpublish.py`

 * *Files identical despite different names*

### Comparing `django-bakery-0.9.2/setup.py` & `django-bakery-0.9.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         # djcelery.setup_loader()
         from django.core.management import call_command
         call_command('test', 'bakery.tests', verbosity=3)
 
 
 setup(
     name='django-bakery',
-    version='0.9.2',
+    version='0.9.3',
     description='A set of helpers for baking your Django site out as flat files',
     author='The Los Angeles Times Data Desk',
     author_email='datadesk@latimes.com',
     url='http://www.github.com/datadesk/django-bakery/',
     license="MIT",
     packages=(
         'bakery',
```

### Comparing `django-bakery-0.9.2/PKG-INFO` & `django-bakery-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-bakery
-Version: 0.9.2
+Version: 0.9.3
 Summary: A set of helpers for baking your Django site out as flat files
 Home-page: http://www.github.com/datadesk/django-bakery/
 Author: The Los Angeles Times Data Desk
 Author-email: datadesk@latimes.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-bakery-0.9.2/README.md` & `django-bakery-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `django-bakery-0.9.2/django_bakery.egg-info/PKG-INFO` & `django-bakery-0.9.3/django_bakery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-bakery
-Version: 0.9.2
+Version: 0.9.3
 Summary: A set of helpers for baking your Django site out as flat files
 Home-page: http://www.github.com/datadesk/django-bakery/
 Author: The Los Angeles Times Data Desk
 Author-email: datadesk@latimes.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-bakery-0.9.2/django_bakery.egg-info/SOURCES.txt` & `django-bakery-0.9.3/django_bakery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

