# Comparing `tmp/Paste-3.8.0.tar.gz` & `tmp/Paste-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Paste-3.8.0.tar", last modified: Sat Mar 16 14:50:51 2024, max compression
+gzip compressed data, was "Paste-3.9.0.tar", last modified: Fri Apr  5 17:23:20 2024, max compression
```

## Comparing `Paste-3.8.0.tar` & `Paste-3.9.0.tar`

### file list

```diff
@@ -1,273 +1,273 @@
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.022458 Paste-3.8.0/
--rw-r--r--   0 cdent      (503) staff       (20)      323 2020-01-26 15:30:37.000000 Paste-3.8.0/MANIFEST.in
--rw-r--r--   0 cdent      (503) staff       (20)     4908 2024-03-16 14:50:51.022296 Paste-3.8.0/PKG-INFO
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.021642 Paste-3.8.0/Paste.egg-info/
--rw-r--r--   0 cdent      (503) staff       (20)     4908 2024-03-16 14:50:50.000000 Paste-3.8.0/Paste.egg-info/PKG-INFO
--rw-r--r--   0 cdent      (503) staff       (20)     6420 2024-03-16 14:50:50.000000 Paste-3.8.0/Paste.egg-info/SOURCES.txt
--rw-r--r--   0 cdent      (503) staff       (20)        1 2024-03-16 14:50:50.000000 Paste-3.8.0/Paste.egg-info/dependency_links.txt
--rw-r--r--   0 cdent      (503) staff       (20)     1900 2024-03-16 14:50:50.000000 Paste-3.8.0/Paste.egg-info/entry_points.txt
--rw-r--r--   0 cdent      (503) staff       (20)        6 2024-03-16 14:50:50.000000 Paste-3.8.0/Paste.egg-info/namespace_packages.txt
--rw-r--r--   0 cdent      (503) staff       (20)        1 2024-03-16 14:50:50.000000 Paste-3.8.0/Paste.egg-info/not-zip-safe
--rw-r--r--   0 cdent      (503) staff       (20)       93 2024-03-16 14:50:50.000000 Paste-3.8.0/Paste.egg-info/requires.txt
--rw-r--r--   0 cdent      (503) staff       (20)        6 2024-03-16 14:50:50.000000 Paste-3.8.0/Paste.egg-info/top_level.txt
--rw-r--r--   0 cdent      (503) staff       (20)     3446 2024-03-16 14:39:27.000000 Paste-3.8.0/README.rst
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.939221 Paste-3.8.0/docs/
--rw-r--r--   0 cdent      (503) staff       (20)     4608 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/DeveloperGuidelines.txt
--rw-r--r--   0 cdent      (503) staff       (20)     3170 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/StyleGuide.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.939777 Paste-3.8.0/docs/_static/
--rw-r--r--   0 cdent      (503) staff       (20)     5988 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/_static/default.css
--rw-r--r--   0 cdent      (503) staff       (20)      194 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/_static/paste.css
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.940601 Paste-3.8.0/docs/community/
--rw-r--r--   0 cdent      (503) staff       (20)      571 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/community/index.txt
--rw-r--r--   0 cdent      (503) staff       (20)      759 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/community/mailing-list.txt
--rw-r--r--   0 cdent      (503) staff       (20)      141 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/community/repository.txt
--rw-r--r--   0 cdent      (503) staff       (20)     3886 2024-03-16 14:46:49.000000 Paste-3.8.0/docs/conf.py
--rw-r--r--   0 cdent      (503) staff       (20)     4500 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/developer-features.txt
--rw-r--r--   0 cdent      (503) staff       (20)    19254 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/do-it-yourself-framework.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.940863 Paste-3.8.0/docs/download/
--rw-r--r--   0 cdent      (503) staff       (20)     1383 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/download/index.txt
--rw-r--r--   0 cdent      (503) staff       (20)     3184 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/future.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.941431 Paste-3.8.0/docs/include/
--rw-r--r--   0 cdent      (503) staff       (20)      338 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/include/contact.txt
--rw-r--r--   0 cdent      (503) staff       (20)       66 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/include/reference_header.txt
--rw-r--r--   0 cdent      (503) staff       (20)     1985 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/index.txt
--rw-r--r--   0 cdent      (503) staff       (20)     1077 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/license.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.961550 Paste-3.8.0/docs/modules/
--rw-r--r--   0 cdent      (503) staff       (20)      312 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/auth.auth_tkt.txt
--rw-r--r--   0 cdent      (503) staff       (20)      273 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/auth.basic.txt
--rw-r--r--   0 cdent      (503) staff       (20)      186 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/auth.cas.txt
--rw-r--r--   0 cdent      (503) staff       (20)      314 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/auth.cookie.txt
--rw-r--r--   0 cdent      (503) staff       (20)      297 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/auth.digest.txt
--rw-r--r--   0 cdent      (503) staff       (20)      242 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/auth.form.txt
--rw-r--r--   0 cdent      (503) staff       (20)      272 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/auth.grantip.txt
--rw-r--r--   0 cdent      (503) staff       (20)      238 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/auth.multi.txt
--rw-r--r--   0 cdent      (503) staff       (20)      273 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/cascade.txt
--rw-r--r--   0 cdent      (503) staff       (20)      281 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/cgiapp.txt
--rw-r--r--   0 cdent      (503) staff       (20)      260 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/cgitb_catcher.txt
--rw-r--r--   0 cdent      (503) staff       (20)      280 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/debug.debugapp.txt
--rw-r--r--   0 cdent      (503) staff       (20)      354 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/debug.fsdiff.txt
--rw-r--r--   0 cdent      (503) staff       (20)      207 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/debug.prints.txt
--rw-r--r--   0 cdent      (503) staff       (20)      312 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/debug.profile.txt
--rw-r--r--   0 cdent      (503) staff       (20)      325 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/debug.watchthreads.txt
--rw-r--r--   0 cdent      (503) staff       (20)      243 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/debug.wdg_validate.txt
--rw-r--r--   0 cdent      (503) staff       (20)      288 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/errordocument.txt
--rw-r--r--   0 cdent      (503) staff       (20)      226 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/evalexception.txt
--rw-r--r--   0 cdent      (503) staff       (20)     1259 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/exceptions.txt
--rw-r--r--   0 cdent      (503) staff       (20)      248 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/fileapp.txt
--rw-r--r--   0 cdent      (503) staff       (20)      633 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/fixture.txt
--rw-r--r--   0 cdent      (503) staff       (20)      226 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/gzipper.txt
--rw-r--r--   0 cdent      (503) staff       (20)     1604 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/httpexceptions.txt
--rw-r--r--   0 cdent      (503) staff       (20)      216 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/httpheaders.txt
--rw-r--r--   0 cdent      (503) staff       (20)      202 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/httpserver.txt
--rw-r--r--   0 cdent      (503) staff       (20)      272 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/lint.txt
--rw-r--r--   0 cdent      (503) staff       (20)      232 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/pony.txt
--rw-r--r--   0 cdent      (503) staff       (20)      246 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/progress.txt
--rw-r--r--   0 cdent      (503) staff       (20)      306 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/proxy.txt
--rw-r--r--   0 cdent      (503) staff       (20)      232 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/recursive.txt
--rw-r--r--   0 cdent      (503) staff       (20)      372 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/registry.txt
--rw-r--r--   0 cdent      (503) staff       (20)      293 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/reloader.txt
--rw-r--r--   0 cdent      (503) staff       (20)      501 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/request.txt
--rw-r--r--   0 cdent      (503) staff       (20)      353 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/response.txt
--rw-r--r--   0 cdent      (503) staff       (20)      243 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/session.txt
--rw-r--r--   0 cdent      (503) staff       (20)      284 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/transaction.txt
--rw-r--r--   0 cdent      (503) staff       (20)      208 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/translogger.txt
--rw-r--r--   0 cdent      (503) staff       (20)      185 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/url.txt
--rw-r--r--   0 cdent      (503) staff       (20)      224 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/urlmap.txt
--rw-r--r--   0 cdent      (503) staff       (20)      392 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/urlparser.txt
--rw-r--r--   0 cdent      (503) staff       (20)      332 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/util.import_string.txt
--rw-r--r--   0 cdent      (503) staff       (20)      260 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/util.multidict.txt
--rw-r--r--   0 cdent      (503) staff       (20)      520 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/wsgilib.txt
--rw-r--r--   0 cdent      (503) staff       (20)      279 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/wsgiwrappers.txt
--rw-r--r--   0 cdent      (503) staff       (20)    41287 2024-03-16 14:42:52.000000 Paste-3.8.0/docs/news.txt
--rw-r--r--   0 cdent      (503) staff       (20)     6405 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/paste-httpserver-threadpool.txt
--rw-r--r--   0 cdent      (503) staff       (20)      933 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/test_server.ini
--rw-r--r--   0 cdent      (503) staff       (20)     5073 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/testing-applications.txt
--rw-r--r--   0 cdent      (503) staff       (20)    12875 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/url-parsing-with-wsgi.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.962515 Paste-3.8.0/docs/web/
--rw-r--r--   0 cdent      (503) staff       (20)     5756 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/web/default-site.css
--rw-r--r--   0 cdent      (503) staff       (20)     1653 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/web/site.js
--rw-r--r--   0 cdent      (503) staff       (20)     1241 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/web/style.css
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.972219 Paste-3.8.0/paste/
--rw-r--r--   0 cdent      (503) staff       (20)      551 2023-10-15 13:05:17.000000 Paste-3.8.0/paste/__init__.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.975432 Paste-3.8.0/paste/auth/
--rw-r--r--   0 cdent      (503) staff       (20)      444 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/auth/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)    16187 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/auth/auth_tkt.py
--rw-r--r--   0 cdent      (503) staff       (20)     4213 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/auth/basic.py
--rw-r--r--   0 cdent      (503) staff       (20)     3996 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/auth/cas.py
--rw-r--r--   0 cdent      (503) staff       (20)    16273 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/auth/cookie.py
--rw-r--r--   0 cdent      (503) staff       (20)     9272 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/auth/digest.py
--rw-r--r--   0 cdent      (503) staff       (20)     5444 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/auth/form.py
--rw-r--r--   0 cdent      (503) staff       (20)     3989 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/auth/grantip.py
--rw-r--r--   0 cdent      (503) staff       (20)     3042 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/auth/multi.py
--rw-r--r--   0 cdent      (503) staff       (20)    16244 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/auth/open_id.py
--rw-r--r--   0 cdent      (503) staff       (20)     4474 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/cascade.py
--rw-r--r--   0 cdent      (503) staff       (20)     9688 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/cgiapp.py
--rw-r--r--   0 cdent      (503) staff       (20)     3803 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/cgitb_catcher.py
--rw-r--r--   0 cdent      (503) staff       (20)     4312 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/config.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.977026 Paste-3.8.0/paste/cowbell/
--rw-r--r--   0 cdent      (503) staff       (20)     3727 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/cowbell/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)   132993 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/cowbell/bell-ascending.png
--rw-r--r--   0 cdent      (503) staff       (20)   124917 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/cowbell/bell-descending.png
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.979998 Paste-3.8.0/paste/debug/
--rw-r--r--   0 cdent      (503) staff       (20)      221 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/debug/__init__.py
--rwxr-xr-x   0 cdent      (503) staff       (20)     2855 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/debug/debugapp.py
--rwxr-xr-x   0 cdent      (503) staff       (20)    14916 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/debug/doctest_webapp.py
--rw-r--r--   0 cdent      (503) staff       (20)    12902 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/debug/fsdiff.py
--rw-r--r--   0 cdent      (503) staff       (20)     5444 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/debug/prints.py
--rw-r--r--   0 cdent      (503) staff       (20)     7553 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/debug/profile.py
--rwxr-xr-x   0 cdent      (503) staff       (20)     3395 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/debug/testserver.py
--rw-r--r--   0 cdent      (503) staff       (20)    10832 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/debug/watchthreads.py
--rw-r--r--   0 cdent      (503) staff       (20)     4261 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/debug/wdg_validate.py
--rw-r--r--   0 cdent      (503) staff       (20)    13855 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/errordocument.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.980806 Paste-3.8.0/paste/evalexception/
--rw-r--r--   0 cdent      (503) staff       (20)      282 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/evalexception/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)     2111 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/evalexception/evalcontext.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.982667 Paste-3.8.0/paste/evalexception/media/
--rw-r--r--   0 cdent      (503) staff       (20)   202262 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/evalexception/media/MochiKit.packed.js
--rw-r--r--   0 cdent      (503) staff       (20)     4257 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/evalexception/media/debug.js
--rw-r--r--   0 cdent      (503) staff       (20)      359 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/evalexception/media/minus.jpg
--rw-r--r--   0 cdent      (503) staff       (20)      361 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/evalexception/media/plus.jpg
--rw-r--r--   0 cdent      (503) staff       (20)    22142 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/evalexception/middleware.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.984450 Paste-3.8.0/paste/exceptions/
--rw-r--r--   0 cdent      (503) staff       (20)      252 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/exceptions/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)    19661 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/exceptions/collector.py
--rw-r--r--   0 cdent      (503) staff       (20)    16954 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/exceptions/errormiddleware.py
--rw-r--r--   0 cdent      (503) staff       (20)    19464 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/exceptions/formatter.py
--rw-r--r--   0 cdent      (503) staff       (20)     4565 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/exceptions/reporter.py
--rw-r--r--   0 cdent      (503) staff       (20)     4069 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/exceptions/serial_number_generator.py
--rw-r--r--   0 cdent      (503) staff       (20)    13698 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/fileapp.py
--rw-r--r--   0 cdent      (503) staff       (20)    59245 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/fixture.py
--rw-r--r--   0 cdent      (503) staff       (20)     3923 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/flup_session.py
--rw-r--r--   0 cdent      (503) staff       (20)     3818 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/gzipper.py
--rw-r--r--   0 cdent      (503) staff       (20)    24244 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/httpexceptions.py
--rw-r--r--   0 cdent      (503) staff       (20)    43120 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/httpheaders.py
--rwxr-xr-x   0 cdent      (503) staff       (20)    57052 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/httpserver.py
--rw-r--r--   0 cdent      (503) staff       (20)    14920 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/lint.py
--rw-r--r--   0 cdent      (503) staff       (20)     7783 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/modpython.py
--rw-r--r--   0 cdent      (503) staff       (20)     2279 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/pony.py
--rwxr-xr-x   0 cdent      (503) staff       (20)     8162 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/progress.py
--rw-r--r--   0 cdent      (503) staff       (20)     9200 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/proxy.py
--rw-r--r--   0 cdent      (503) staff       (20)    14605 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/recursive.py
--rw-r--r--   0 cdent      (503) staff       (20)    22250 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/registry.py
--rw-r--r--   0 cdent      (503) staff       (20)     6000 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/reloader.py
--rw-r--r--   0 cdent      (503) staff       (20)    13883 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/request.py
--rw-r--r--   0 cdent      (503) staff       (20)     7659 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/response.py
--rw-r--r--   0 cdent      (503) staff       (20)    11396 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/session.py
--rw-r--r--   0 cdent      (503) staff       (20)     4363 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/transaction.py
--rw-r--r--   0 cdent      (503) staff       (20)     5159 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/translogger.py
--rw-r--r--   0 cdent      (503) staff       (20)    14440 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/url.py
--rw-r--r--   0 cdent      (503) staff       (20)     9248 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/urlmap.py
--rw-r--r--   0 cdent      (503) staff       (20)    26451 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/urlparser.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.991961 Paste-3.8.0/paste/util/
--rw-r--r--   0 cdent      (503) staff       (20)    83603 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/PySourceColor.py
--rw-r--r--   0 cdent      (503) staff       (20)       86 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)     1849 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/classinit.py
--rw-r--r--   0 cdent      (503) staff       (20)     1361 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/classinstance.py
--rw-r--r--   0 cdent      (503) staff       (20)      861 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/converters.py
--rw-r--r--   0 cdent      (503) staff       (20)     2412 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/dateinterval.py
--rw-r--r--   0 cdent      (503) staff       (20)    10796 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/datetimeutil.py
--rw-r--r--   0 cdent      (503) staff       (20)     1427 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/filemixin.py
--rw-r--r--   0 cdent      (503) staff       (20)     3808 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/finddata.py
--rw-r--r--   0 cdent      (503) staff       (20)      782 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/findpackage.py
--rw-r--r--   0 cdent      (503) staff       (20)     3114 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/import_string.py
--rw-r--r--   0 cdent      (503) staff       (20)    19071 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/intset.py
--rw-r--r--   0 cdent      (503) staff       (20)     9267 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/ip4.py
--rw-r--r--   0 cdent      (503) staff       (20)     1197 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/killthread.py
--rw-r--r--   0 cdent      (503) staff       (20)     3988 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/looper.py
--rw-r--r--   0 cdent      (503) staff       (20)     6604 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/mimeparse.py
--rw-r--r--   0 cdent      (503) staff       (20)    12405 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/multidict.py
--rw-r--r--   0 cdent      (503) staff       (20)     2011 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/quoting.py
--rw-r--r--   0 cdent      (503) staff       (20)     5565 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/scgiserver.py
--rw-r--r--   0 cdent      (503) staff       (20)    23670 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/template.py
--rw-r--r--   0 cdent      (503) staff       (20)     8175 2022-06-22 10:14:29.000000 Paste-3.8.0/paste/util/threadedprint.py
--rw-r--r--   0 cdent      (503) staff       (20)     1484 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/threadinglocal.py
--rw-r--r--   0 cdent      (503) staff       (20)    20260 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/wsgilib.py
--rw-r--r--   0 cdent      (503) staff       (20)    22173 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/wsgiwrappers.py
--rwxr-xr-x   0 cdent      (503) staff       (20)      234 2020-01-26 15:30:37.000000 Paste-3.8.0/regen-docs
--rw-r--r--   0 cdent      (503) staff       (20)      162 2024-03-16 14:50:51.022824 Paste-3.8.0/setup.cfg
--rw-r--r--   0 cdent      (503) staff       (20)     4612 2024-03-16 14:43:51.000000 Paste-3.8.0/setup.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.001687 Paste-3.8.0/tests/
--rw-r--r--   0 cdent      (503) staff       (20)      138 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/__init__.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.002833 Paste-3.8.0/tests/cgiapp_data/
--rwxr-xr-x   0 cdent      (503) staff       (20)       41 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/cgiapp_data/error.cgi
--rwxr-xr-x   0 cdent      (503) staff       (20)     2000 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/cgiapp_data/form.cgi
--rwxr-xr-x   0 cdent      (503) staff       (20)      132 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/cgiapp_data/ok.cgi
--rwxr-xr-x   0 cdent      (503) staff       (20)      185 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/cgiapp_data/stderr.cgi
--rw-r--r--   0 cdent      (503) staff       (20)     4132 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/template.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.004180 Paste-3.8.0/tests/test_auth/
--rw-r--r--   0 cdent      (503) staff       (20)        0 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_auth/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)     1465 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_auth/test_auth_cookie.py
--rw-r--r--   0 cdent      (503) staff       (20)     3026 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_auth/test_auth_digest.py
--rw-r--r--   0 cdent      (503) staff       (20)     3598 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_auth/test_auth_tkt.py
--rw-r--r--   0 cdent      (503) staff       (20)     2053 2020-10-12 12:27:11.000000 Paste-3.8.0/tests/test_cgiapp.py
--rw-r--r--   0 cdent      (503) staff       (20)     2157 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_cgitb_catcher.py
--rw-r--r--   0 cdent      (503) staff       (20)     2846 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_config.py
--rw-r--r--   0 cdent      (503) staff       (20)     1506 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_doctests.py
--rw-r--r--   0 cdent      (503) staff       (20)     3461 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_errordocument.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.005552 Paste-3.8.0/tests/test_exceptions/
--rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_exceptions/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)     3286 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_exceptions/test_error_middleware.py
--rw-r--r--   0 cdent      (503) staff       (20)     4985 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_exceptions/test_formatter.py
--rw-r--r--   0 cdent      (503) staff       (20)     4263 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_exceptions/test_httpexceptions.py
--rw-r--r--   0 cdent      (503) staff       (20)     1280 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_exceptions/test_reporter.py
--rw-r--r--   0 cdent      (503) staff       (20)     9589 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_fileapp.py
--rw-r--r--   0 cdent      (503) staff       (20)     2489 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_fixture.py
--rw-r--r--   0 cdent      (503) staff       (20)     1240 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_grantip.py
--rw-r--r--   0 cdent      (503) staff       (20)      886 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_gzipper.py
--rw-r--r--   0 cdent      (503) staff       (20)     6843 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_httpheaders.py
--rw-r--r--   0 cdent      (503) staff       (20)     3229 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_httpserver.py
--rw-r--r--   0 cdent      (503) staff       (20)      477 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_import_string.py
--rw-r--r--   0 cdent      (503) staff       (20)     5116 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_multidict.py
--rw-r--r--   0 cdent      (503) staff       (20)      721 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_profilemiddleware.py
--rw-r--r--   0 cdent      (503) staff       (20)      624 2023-04-30 11:31:00.000000 Paste-3.8.0/tests/test_proxy.py
--rw-r--r--   0 cdent      (503) staff       (20)     4178 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_recursive.py
--rw-r--r--   0 cdent      (503) staff       (20)    11013 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_registry.py
--rw-r--r--   0 cdent      (503) staff       (20)     2323 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_request.py
--rw-r--r--   0 cdent      (503) staff       (20)     1463 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_request_form.py
--rw-r--r--   0 cdent      (503) staff       (20)      369 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_response.py
--rw-r--r--   0 cdent      (503) staff       (20)     1548 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_session.py
--rw-r--r--   0 cdent      (503) staff       (20)     1786 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_urlmap.py
--rw-r--r--   0 cdent      (503) staff       (20)     6944 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_urlparser.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.006936 Paste-3.8.0/tests/test_util/
--rw-r--r--   0 cdent      (503) staff       (20)        0 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_util/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)     6109 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_util/test_datetimeutil.py
--rw-r--r--   0 cdent      (503) staff       (20)    11873 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_util/test_mimeparse.py
--rw-r--r--   0 cdent      (503) staff       (20)      997 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_util/test_quoting.py
--rw-r--r--   0 cdent      (503) staff       (20)      842 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_wsgilib.py
--rw-r--r--   0 cdent      (503) staff       (20)     6380 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_wsgiwrappers.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.007724 Paste-3.8.0/tests/urlparser_data/
--rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/__init__.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.008021 Paste-3.8.0/tests/urlparser_data/deep/
--rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/deep/index.html
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.008348 Paste-3.8.0/tests/urlparser_data/deep/sub/
--rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/deep/sub/Main.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.009469 Paste-3.8.0/tests/urlparser_data/find_file/
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.009896 Paste-3.8.0/tests/urlparser_data/find_file/dir with spaces/
--rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/find_file/dir with spaces/test 4.html
--rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/find_file/index.txt
--rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/find_file/test 3.html
--rw-r--r--   0 cdent      (503) staff       (20)        6 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/find_file/test2.html
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.011002 Paste-3.8.0/tests/urlparser_data/hook/
--rw-r--r--   0 cdent      (503) staff       (20)      289 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/hook/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)      200 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/urlparser_data/hook/app.py
--rw-r--r--   0 cdent      (503) staff       (20)      201 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/urlparser_data/hook/index.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.011263 Paste-3.8.0/tests/urlparser_data/not_found/
--rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/not_found/__init__.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.017973 Paste-3.8.0/tests/urlparser_data/not_found/recur/
--rw-r--r--   0 cdent      (503) staff       (20)      374 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/not_found/recur/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)        9 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/not_found/recur/isfound.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.018946 Paste-3.8.0/tests/urlparser_data/not_found/simple/
--rw-r--r--   0 cdent      (503) staff       (20)      134 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/not_found/simple/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)        9 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/not_found/simple/found.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.019567 Paste-3.8.0/tests/urlparser_data/not_found/user/
--rw-r--r--   0 cdent      (503) staff       (20)      411 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/not_found/user/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)      204 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/urlparser_data/not_found/user/list.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.020483 Paste-3.8.0/tests/urlparser_data/python/
--rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/python/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)      183 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/python/simpleapp.py
--rw-r--r--   0 cdent      (503) staff       (20)      208 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/python/stream.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.021177 Paste-3.8.0/tests/urlparser_data/python/sub/
--rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/python/sub/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)      186 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/python/sub/simpleapp.py
--rw-r--r--   0 cdent      (503) staff       (20)        8 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/secured.txt
--rw-r--r--   0 cdent      (503) staff       (20)      365 2023-10-19 10:24:33.000000 Paste-3.8.0/tox.ini
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.322429 Paste-3.9.0/
+-rw-r--r--   0 cdent      (503) staff       (20)      323 2020-01-26 15:30:37.000000 Paste-3.9.0/MANIFEST.in
+-rw-r--r--   0 cdent      (503) staff       (20)     4882 2024-04-05 17:23:20.322298 Paste-3.9.0/PKG-INFO
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.321807 Paste-3.9.0/Paste.egg-info/
+-rw-r--r--   0 cdent      (503) staff       (20)     4882 2024-04-05 17:23:20.000000 Paste-3.9.0/Paste.egg-info/PKG-INFO
+-rw-r--r--   0 cdent      (503) staff       (20)     6420 2024-04-05 17:23:20.000000 Paste-3.9.0/Paste.egg-info/SOURCES.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        1 2024-04-05 17:23:20.000000 Paste-3.9.0/Paste.egg-info/dependency_links.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     1900 2024-04-05 17:23:20.000000 Paste-3.9.0/Paste.egg-info/entry_points.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        6 2024-04-05 17:23:20.000000 Paste-3.9.0/Paste.egg-info/namespace_packages.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        1 2024-04-05 17:23:20.000000 Paste-3.9.0/Paste.egg-info/not-zip-safe
+-rw-r--r--   0 cdent      (503) staff       (20)       82 2024-04-05 17:23:20.000000 Paste-3.9.0/Paste.egg-info/requires.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        6 2024-04-05 17:23:20.000000 Paste-3.9.0/Paste.egg-info/top_level.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     3446 2024-03-16 14:39:27.000000 Paste-3.9.0/README.rst
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.256258 Paste-3.9.0/docs/
+-rw-r--r--   0 cdent      (503) staff       (20)     4608 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/DeveloperGuidelines.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     3170 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/StyleGuide.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.256777 Paste-3.9.0/docs/_static/
+-rw-r--r--   0 cdent      (503) staff       (20)     5988 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/_static/default.css
+-rw-r--r--   0 cdent      (503) staff       (20)      194 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/_static/paste.css
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.257640 Paste-3.9.0/docs/community/
+-rw-r--r--   0 cdent      (503) staff       (20)      571 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/community/index.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      759 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/community/mailing-list.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      141 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/community/repository.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     3887 2024-03-31 18:16:14.000000 Paste-3.9.0/docs/conf.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4500 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/developer-features.txt
+-rw-r--r--   0 cdent      (503) staff       (20)    19254 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/do-it-yourself-framework.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.257917 Paste-3.9.0/docs/download/
+-rw-r--r--   0 cdent      (503) staff       (20)     1383 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/download/index.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     3184 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/future.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.258435 Paste-3.9.0/docs/include/
+-rw-r--r--   0 cdent      (503) staff       (20)      338 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/include/contact.txt
+-rw-r--r--   0 cdent      (503) staff       (20)       66 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/include/reference_header.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     1985 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/index.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     1077 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/license.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.277081 Paste-3.9.0/docs/modules/
+-rw-r--r--   0 cdent      (503) staff       (20)      312 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/auth.auth_tkt.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      273 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/auth.basic.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      186 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/auth.cas.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      314 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/auth.cookie.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      297 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/auth.digest.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      242 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/auth.form.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      272 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/auth.grantip.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      238 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/auth.multi.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      273 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/cascade.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      281 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/cgiapp.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      260 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/cgitb_catcher.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      280 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/debug.debugapp.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      354 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/debug.fsdiff.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      207 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/debug.prints.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      312 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/debug.profile.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      325 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/debug.watchthreads.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      243 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/debug.wdg_validate.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      288 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/errordocument.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      226 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/evalexception.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     1259 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/exceptions.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      248 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/fileapp.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      633 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/fixture.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      226 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/gzipper.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     1604 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/httpexceptions.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      216 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/httpheaders.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      202 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/httpserver.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      272 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/lint.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      232 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/pony.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      246 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/progress.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      306 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/proxy.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      232 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/recursive.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      372 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/registry.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      293 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/reloader.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      501 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/request.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      353 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/response.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      243 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/session.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      284 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/transaction.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      208 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/translogger.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      185 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/url.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      224 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/urlmap.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      392 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/urlparser.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      332 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/util.import_string.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      260 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/util.multidict.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      520 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/wsgilib.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      279 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/modules/wsgiwrappers.txt
+-rw-r--r--   0 cdent      (503) staff       (20)    41358 2024-04-05 17:19:39.000000 Paste-3.9.0/docs/news.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     6405 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/paste-httpserver-threadpool.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      933 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/test_server.ini
+-rw-r--r--   0 cdent      (503) staff       (20)     5073 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/testing-applications.txt
+-rw-r--r--   0 cdent      (503) staff       (20)    12875 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/url-parsing-with-wsgi.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.277989 Paste-3.9.0/docs/web/
+-rw-r--r--   0 cdent      (503) staff       (20)     5756 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/web/default-site.css
+-rw-r--r--   0 cdent      (503) staff       (20)     1653 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/web/site.js
+-rw-r--r--   0 cdent      (503) staff       (20)     1241 2020-01-26 15:30:37.000000 Paste-3.9.0/docs/web/style.css
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.286982 Paste-3.9.0/paste/
+-rw-r--r--   0 cdent      (503) staff       (20)      551 2023-10-15 13:05:17.000000 Paste-3.9.0/paste/__init__.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.289862 Paste-3.9.0/paste/auth/
+-rw-r--r--   0 cdent      (503) staff       (20)      444 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/auth/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)    16208 2024-03-31 18:16:14.000000 Paste-3.9.0/paste/auth/auth_tkt.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4197 2024-03-31 18:16:14.000000 Paste-3.9.0/paste/auth/basic.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4050 2024-03-31 18:16:14.000000 Paste-3.9.0/paste/auth/cas.py
+-rw-r--r--   0 cdent      (503) staff       (20)    16287 2024-03-31 18:16:14.000000 Paste-3.9.0/paste/auth/cookie.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9272 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/auth/digest.py
+-rw-r--r--   0 cdent      (503) staff       (20)     5444 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/auth/form.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3989 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/auth/grantip.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3042 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/auth/multi.py
+-rw-r--r--   0 cdent      (503) staff       (20)    16244 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/auth/open_id.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4474 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/cascade.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9818 2024-03-31 18:16:14.000000 Paste-3.9.0/paste/cgiapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3803 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/cgitb_catcher.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4312 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/config.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.291231 Paste-3.9.0/paste/cowbell/
+-rw-r--r--   0 cdent      (503) staff       (20)     3727 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/cowbell/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)   132993 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/cowbell/bell-ascending.png
+-rw-r--r--   0 cdent      (503) staff       (20)   124917 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/cowbell/bell-descending.png
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.294039 Paste-3.9.0/paste/debug/
+-rw-r--r--   0 cdent      (503) staff       (20)      221 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/debug/__init__.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)     2855 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/debug/debugapp.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)    14916 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/debug/doctest_webapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)    12902 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/debug/fsdiff.py
+-rw-r--r--   0 cdent      (503) staff       (20)     5444 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/debug/prints.py
+-rw-r--r--   0 cdent      (503) staff       (20)     7553 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/debug/profile.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)     3395 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/debug/testserver.py
+-rw-r--r--   0 cdent      (503) staff       (20)    10027 2024-04-05 17:18:46.000000 Paste-3.9.0/paste/debug/watchthreads.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4261 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/debug/wdg_validate.py
+-rw-r--r--   0 cdent      (503) staff       (20)    13855 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/errordocument.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.294881 Paste-3.9.0/paste/evalexception/
+-rw-r--r--   0 cdent      (503) staff       (20)      282 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/evalexception/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2111 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/evalexception/evalcontext.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.296537 Paste-3.9.0/paste/evalexception/media/
+-rw-r--r--   0 cdent      (503) staff       (20)   202262 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/evalexception/media/MochiKit.packed.js
+-rw-r--r--   0 cdent      (503) staff       (20)     4257 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/evalexception/media/debug.js
+-rw-r--r--   0 cdent      (503) staff       (20)      359 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/evalexception/media/minus.jpg
+-rw-r--r--   0 cdent      (503) staff       (20)      361 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/evalexception/media/plus.jpg
+-rw-r--r--   0 cdent      (503) staff       (20)    22187 2024-03-31 18:16:14.000000 Paste-3.9.0/paste/evalexception/middleware.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.298053 Paste-3.9.0/paste/exceptions/
+-rw-r--r--   0 cdent      (503) staff       (20)      252 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/exceptions/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)    19657 2024-03-31 18:16:14.000000 Paste-3.9.0/paste/exceptions/collector.py
+-rw-r--r--   0 cdent      (503) staff       (20)    16954 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/exceptions/errormiddleware.py
+-rw-r--r--   0 cdent      (503) staff       (20)    19464 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/exceptions/formatter.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4565 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/exceptions/reporter.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4104 2024-03-31 18:16:14.000000 Paste-3.9.0/paste/exceptions/serial_number_generator.py
+-rw-r--r--   0 cdent      (503) staff       (20)    14070 2024-03-31 18:16:14.000000 Paste-3.9.0/paste/fileapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)    59463 2024-03-31 18:16:14.000000 Paste-3.9.0/paste/fixture.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3923 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/flup_session.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3818 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/gzipper.py
+-rw-r--r--   0 cdent      (503) staff       (20)    24244 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/httpexceptions.py
+-rw-r--r--   0 cdent      (503) staff       (20)    43120 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/httpheaders.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)    56999 2024-03-31 18:16:14.000000 Paste-3.9.0/paste/httpserver.py
+-rw-r--r--   0 cdent      (503) staff       (20)    14920 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/lint.py
+-rw-r--r--   0 cdent      (503) staff       (20)     7783 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/modpython.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2279 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/pony.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)     8162 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/progress.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9185 2024-03-31 18:16:14.000000 Paste-3.9.0/paste/proxy.py
+-rw-r--r--   0 cdent      (503) staff       (20)    14605 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/recursive.py
+-rw-r--r--   0 cdent      (503) staff       (20)    22250 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/registry.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6000 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/reloader.py
+-rw-r--r--   0 cdent      (503) staff       (20)    13883 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/request.py
+-rw-r--r--   0 cdent      (503) staff       (20)     7659 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/response.py
+-rw-r--r--   0 cdent      (503) staff       (20)    11396 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/session.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4363 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/transaction.py
+-rw-r--r--   0 cdent      (503) staff       (20)     5149 2024-03-31 18:16:14.000000 Paste-3.9.0/paste/translogger.py
+-rw-r--r--   0 cdent      (503) staff       (20)    14440 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/url.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9248 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/urlmap.py
+-rw-r--r--   0 cdent      (503) staff       (20)    26451 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/urlparser.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.303933 Paste-3.9.0/paste/util/
+-rw-r--r--   0 cdent      (503) staff       (20)    83603 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/util/PySourceColor.py
+-rw-r--r--   0 cdent      (503) staff       (20)       86 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/util/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1849 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/util/classinit.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1361 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/util/classinstance.py
+-rw-r--r--   0 cdent      (503) staff       (20)      861 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/util/converters.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2412 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/util/dateinterval.py
+-rw-r--r--   0 cdent      (503) staff       (20)    10796 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/util/datetimeutil.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1427 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/util/filemixin.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3808 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/util/finddata.py
+-rw-r--r--   0 cdent      (503) staff       (20)      782 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/util/findpackage.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3114 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/util/import_string.py
+-rw-r--r--   0 cdent      (503) staff       (20)    19071 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/util/intset.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9267 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/util/ip4.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1197 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/util/killthread.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3988 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/util/looper.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6604 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/util/mimeparse.py
+-rw-r--r--   0 cdent      (503) staff       (20)    12405 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/util/multidict.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1976 2024-03-31 18:16:14.000000 Paste-3.9.0/paste/util/quoting.py
+-rw-r--r--   0 cdent      (503) staff       (20)     5565 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/util/scgiserver.py
+-rw-r--r--   0 cdent      (503) staff       (20)    23898 2024-03-31 18:16:14.000000 Paste-3.9.0/paste/util/template.py
+-rw-r--r--   0 cdent      (503) staff       (20)     8174 2024-03-31 18:16:14.000000 Paste-3.9.0/paste/util/threadedprint.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1484 2020-01-26 15:30:37.000000 Paste-3.9.0/paste/util/threadinglocal.py
+-rw-r--r--   0 cdent      (503) staff       (20)    20260 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/wsgilib.py
+-rw-r--r--   0 cdent      (503) staff       (20)    22173 2024-03-16 14:39:27.000000 Paste-3.9.0/paste/wsgiwrappers.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)      234 2020-01-26 15:30:37.000000 Paste-3.9.0/regen-docs
+-rw-r--r--   0 cdent      (503) staff       (20)      162 2024-04-05 17:23:20.322731 Paste-3.9.0/setup.cfg
+-rw-r--r--   0 cdent      (503) staff       (20)     4590 2024-04-05 17:19:08.000000 Paste-3.9.0/setup.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.310568 Paste-3.9.0/tests/
+-rw-r--r--   0 cdent      (503) staff       (20)      138 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/__init__.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.311726 Paste-3.9.0/tests/cgiapp_data/
+-rwxr-xr-x   0 cdent      (503) staff       (20)       41 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/cgiapp_data/error.cgi
+-rwxr-xr-x   0 cdent      (503) staff       (20)     2000 2024-03-16 14:39:27.000000 Paste-3.9.0/tests/cgiapp_data/form.cgi
+-rwxr-xr-x   0 cdent      (503) staff       (20)      132 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/cgiapp_data/ok.cgi
+-rwxr-xr-x   0 cdent      (503) staff       (20)      185 2024-03-16 14:39:27.000000 Paste-3.9.0/tests/cgiapp_data/stderr.cgi
+-rw-r--r--   0 cdent      (503) staff       (20)     4132 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/template.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.312866 Paste-3.9.0/tests/test_auth/
+-rw-r--r--   0 cdent      (503) staff       (20)        0 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/test_auth/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1430 2024-03-31 18:16:14.000000 Paste-3.9.0/tests/test_auth/test_auth_cookie.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3078 2024-03-31 18:16:14.000000 Paste-3.9.0/tests/test_auth/test_auth_digest.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3598 2024-03-16 14:39:27.000000 Paste-3.9.0/tests/test_auth/test_auth_tkt.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2059 2024-03-31 18:16:14.000000 Paste-3.9.0/tests/test_cgiapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2163 2024-03-31 18:16:14.000000 Paste-3.9.0/tests/test_cgitb_catcher.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2846 2024-03-16 14:39:27.000000 Paste-3.9.0/tests/test_config.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1506 2024-03-16 14:39:27.000000 Paste-3.9.0/tests/test_doctests.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3467 2024-03-31 18:16:14.000000 Paste-3.9.0/tests/test_errordocument.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.314291 Paste-3.9.0/tests/test_exceptions/
+-rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/test_exceptions/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3292 2024-03-31 18:16:14.000000 Paste-3.9.0/tests/test_exceptions/test_error_middleware.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4985 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/test_exceptions/test_formatter.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4263 2024-03-16 14:39:27.000000 Paste-3.9.0/tests/test_exceptions/test_httpexceptions.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1290 2024-03-31 18:16:14.000000 Paste-3.9.0/tests/test_exceptions/test_reporter.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9601 2024-03-31 18:16:14.000000 Paste-3.9.0/tests/test_fileapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2477 2024-03-31 18:16:14.000000 Paste-3.9.0/tests/test_fixture.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1246 2024-03-31 18:16:14.000000 Paste-3.9.0/tests/test_grantip.py
+-rw-r--r--   0 cdent      (503) staff       (20)      886 2024-03-16 14:39:27.000000 Paste-3.9.0/tests/test_gzipper.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6843 2024-03-16 14:39:27.000000 Paste-3.9.0/tests/test_httpheaders.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3229 2024-03-16 14:39:27.000000 Paste-3.9.0/tests/test_httpserver.py
+-rw-r--r--   0 cdent      (503) staff       (20)      502 2024-03-31 18:16:14.000000 Paste-3.9.0/tests/test_import_string.py
+-rw-r--r--   0 cdent      (503) staff       (20)     5116 2024-03-16 14:39:27.000000 Paste-3.9.0/tests/test_multidict.py
+-rw-r--r--   0 cdent      (503) staff       (20)      762 2024-03-31 18:16:14.000000 Paste-3.9.0/tests/test_profilemiddleware.py
+-rw-r--r--   0 cdent      (503) staff       (20)      624 2023-04-30 11:31:00.000000 Paste-3.9.0/tests/test_proxy.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4184 2024-03-31 18:16:14.000000 Paste-3.9.0/tests/test_recursive.py
+-rw-r--r--   0 cdent      (503) staff       (20)    11058 2024-03-31 18:16:14.000000 Paste-3.9.0/tests/test_registry.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2343 2024-03-31 18:16:14.000000 Paste-3.9.0/tests/test_request.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1495 2024-03-31 18:16:14.000000 Paste-3.9.0/tests/test_request_form.py
+-rw-r--r--   0 cdent      (503) staff       (20)      382 2024-03-31 18:16:14.000000 Paste-3.9.0/tests/test_response.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1548 2024-03-16 14:39:27.000000 Paste-3.9.0/tests/test_session.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1786 2024-03-16 14:39:27.000000 Paste-3.9.0/tests/test_urlmap.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6996 2024-03-31 18:16:14.000000 Paste-3.9.0/tests/test_urlparser.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.315416 Paste-3.9.0/tests/test_util/
+-rw-r--r--   0 cdent      (503) staff       (20)        0 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/test_util/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6109 2024-03-16 14:39:27.000000 Paste-3.9.0/tests/test_util/test_datetimeutil.py
+-rw-r--r--   0 cdent      (503) staff       (20)    12021 2024-03-31 18:16:14.000000 Paste-3.9.0/tests/test_util/test_mimeparse.py
+-rw-r--r--   0 cdent      (503) staff       (20)      997 2024-03-16 14:39:27.000000 Paste-3.9.0/tests/test_util/test_quoting.py
+-rw-r--r--   0 cdent      (503) staff       (20)      842 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/test_wsgilib.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6380 2024-03-16 14:39:27.000000 Paste-3.9.0/tests/test_wsgiwrappers.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.316083 Paste-3.9.0/tests/urlparser_data/
+-rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/__init__.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.316354 Paste-3.9.0/tests/urlparser_data/deep/
+-rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/deep/index.html
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.316631 Paste-3.9.0/tests/urlparser_data/deep/sub/
+-rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/deep/sub/Main.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.317445 Paste-3.9.0/tests/urlparser_data/find_file/
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.317715 Paste-3.9.0/tests/urlparser_data/find_file/dir with spaces/
+-rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/find_file/dir with spaces/test 4.html
+-rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/find_file/index.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/find_file/test 3.html
+-rw-r--r--   0 cdent      (503) staff       (20)        6 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/find_file/test2.html
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.318503 Paste-3.9.0/tests/urlparser_data/hook/
+-rw-r--r--   0 cdent      (503) staff       (20)      289 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/hook/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)      200 2024-03-16 14:39:27.000000 Paste-3.9.0/tests/urlparser_data/hook/app.py
+-rw-r--r--   0 cdent      (503) staff       (20)      201 2024-03-16 14:39:27.000000 Paste-3.9.0/tests/urlparser_data/hook/index.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.318771 Paste-3.9.0/tests/urlparser_data/not_found/
+-rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/not_found/__init__.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.319328 Paste-3.9.0/tests/urlparser_data/not_found/recur/
+-rw-r--r--   0 cdent      (503) staff       (20)      374 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/not_found/recur/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)        9 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/not_found/recur/isfound.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.319850 Paste-3.9.0/tests/urlparser_data/not_found/simple/
+-rw-r--r--   0 cdent      (503) staff       (20)      134 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/not_found/simple/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)        9 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/not_found/simple/found.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.320309 Paste-3.9.0/tests/urlparser_data/not_found/user/
+-rw-r--r--   0 cdent      (503) staff       (20)      411 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/not_found/user/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)      204 2024-03-16 14:39:27.000000 Paste-3.9.0/tests/urlparser_data/not_found/user/list.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.321049 Paste-3.9.0/tests/urlparser_data/python/
+-rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/python/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)      183 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/python/simpleapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)      208 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/python/stream.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-05 17:23:20.321508 Paste-3.9.0/tests/urlparser_data/python/sub/
+-rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/python/sub/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)      186 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/python/sub/simpleapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)        8 2020-01-26 15:30:37.000000 Paste-3.9.0/tests/urlparser_data/secured.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      365 2023-10-19 10:24:33.000000 Paste-3.9.0/tox.ini
```

### Comparing `Paste-3.8.0/PKG-INFO` & `Paste-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Paste
-Version: 3.8.0
+Version: 3.9.0
 Summary: Tools for using a Web Server Gateway Interface stack
 Home-page: https://pythonpaste.readthedocs.io/
 Author: Chris Dent
 Author-email: chris.dent@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/cdent/paste
 Project-URL: Bug Tracker, https://github.com/cdent/paste/issues
@@ -22,15 +22,14 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
 Classifier: Framework :: Paste
 Requires-Python: >=3
 Requires-Dist: setuptools
-Requires-Dist: six>=1.4.0
 Provides-Extra: subprocess
 Provides-Extra: hotshot
 Provides-Extra: flup
 Requires-Dist: flup; extra == "flup"
 Provides-Extra: paste
 Provides-Extra: openid
 Requires-Dist: python-openid; extra == "openid"
```

### Comparing `Paste-3.8.0/Paste.egg-info/PKG-INFO` & `Paste-3.9.0/Paste.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Paste
-Version: 3.8.0
+Version: 3.9.0
 Summary: Tools for using a Web Server Gateway Interface stack
 Home-page: https://pythonpaste.readthedocs.io/
 Author: Chris Dent
 Author-email: chris.dent@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/cdent/paste
 Project-URL: Bug Tracker, https://github.com/cdent/paste/issues
@@ -22,15 +22,14 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
 Classifier: Framework :: Paste
 Requires-Python: >=3
 Requires-Dist: setuptools
-Requires-Dist: six>=1.4.0
 Provides-Extra: subprocess
 Provides-Extra: hotshot
 Provides-Extra: flup
 Requires-Dist: flup; extra == "flup"
 Provides-Extra: paste
 Provides-Extra: openid
 Requires-Dist: python-openid; extra == "openid"
```

### Comparing `Paste-3.8.0/Paste.egg-info/SOURCES.txt` & `Paste-3.9.0/Paste.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/Paste.egg-info/entry_points.txt` & `Paste-3.9.0/Paste.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/README.rst` & `Paste-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/DeveloperGuidelines.txt` & `Paste-3.9.0/docs/DeveloperGuidelines.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/StyleGuide.txt` & `Paste-3.9.0/docs/StyleGuide.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/_static/default.css` & `Paste-3.9.0/docs/_static/default.css`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/community/index.txt` & `Paste-3.9.0/docs/community/index.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/community/mailing-list.txt` & `Paste-3.9.0/docs/community/mailing-list.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/conf.py` & `Paste-3.9.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 #
 # The contents of this file are pickled, so don't put values in the namespace
 # that aren't pickleable (module imports are okay, they're removed automatically).
 #
 # All configuration values have a default value; values that are commented out
 # serve to show the default value.
 
-import sys
 
 # If your extensions are in another directory, add it here.
+#import sys
 #sys.path.append('some/directory')
 
 # General configuration
 # ---------------------
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
```

### Comparing `Paste-3.8.0/docs/developer-features.txt` & `Paste-3.9.0/docs/developer-features.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/do-it-yourself-framework.txt` & `Paste-3.9.0/docs/do-it-yourself-framework.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/download/index.txt` & `Paste-3.9.0/docs/download/index.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/future.txt` & `Paste-3.9.0/docs/future.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/index.txt` & `Paste-3.9.0/docs/index.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/license.txt` & `Paste-3.9.0/docs/license.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/modules/exceptions.txt` & `Paste-3.9.0/docs/modules/exceptions.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/modules/fixture.txt` & `Paste-3.9.0/docs/modules/fixture.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/modules/httpexceptions.txt` & `Paste-3.9.0/docs/modules/httpexceptions.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/modules/wsgilib.txt` & `Paste-3.9.0/docs/modules/wsgilib.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/news.txt` & `Paste-3.9.0/docs/news.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 News
 ====
 
 .. contents::
 
+3.9.0
+-----
+
+* Remove dead format_environ code in watchthread.py app.
+
 3.8.0
 -----
 
 * Remove remainder of Python 2 code. Thanks a-detiste.
 
 3.7.0
 -----
```

### Comparing `Paste-3.8.0/docs/paste-httpserver-threadpool.txt` & `Paste-3.9.0/docs/paste-httpserver-threadpool.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/test_server.ini` & `Paste-3.9.0/docs/test_server.ini`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/testing-applications.txt` & `Paste-3.9.0/docs/testing-applications.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/url-parsing-with-wsgi.txt` & `Paste-3.9.0/docs/url-parsing-with-wsgi.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/web/default-site.css` & `Paste-3.9.0/docs/web/default-site.css`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/web/site.js` & `Paste-3.9.0/docs/web/site.js`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/docs/web/style.css` & `Paste-3.9.0/docs/web/style.css`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/__init__.py` & `Paste-3.9.0/paste/__init__.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/auth/auth_tkt.py` & `Paste-3.9.0/paste/auth/auth_tkt.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 list of groups) and ``REMOTE_USER_DATA`` (arbitrary string data).
 
 This module is an alternative to the ``paste.auth.cookie`` module;
 it's primary benefit is compatibility with mod_auth_tkt, which in turn
 makes it possible to use the same authentication process with
 non-Python code run under Apache.
 """
-import six
 import time as time_mod
 try:
     import hashlib
 except ImportError:
     # mimic hashlib (will work for md5, fail for secure hashes)
     import md5 as hashlib
 from http.cookies import SimpleCookie
@@ -198,23 +197,25 @@
     user_data = maybe_encode(user_data)
     digest0 = maybe_encode(digest_algo(
         encode_ip_timestamp(ip, timestamp) + secret + userid + b'\0'
         + tokens + b'\0' + user_data).hexdigest())
     digest = digest_algo(digest0 + secret).hexdigest()
     return maybe_encode(digest)
 
+def int2byte(i):
+    return bytes((i,))
 
 def encode_ip_timestamp(ip, timestamp):
-    ip_chars = b''.join(map(six.int2byte, map(int, ip.split('.'))))
+    ip_chars = b''.join(map(int2byte, map(int, ip.split('.'))))
     t = int(timestamp)
     ts = ((t & 0xff000000) >> 24,
           (t & 0xff0000) >> 16,
           (t & 0xff00) >> 8,
           t & 0xff)
-    ts_chars = b''.join(map(six.int2byte, ts))
+    ts_chars = b''.join(map(int2byte, ts))
     return (ip_chars + ts_chars)
 
 
 def maybe_encode(s, encoding='utf8'):
     if isinstance(s, str):
         s = s.encode(encoding)
     return s
```

### Comparing `Paste-3.8.0/paste/auth/basic.py` & `Paste-3.9.0/paste/auth/basic.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 >>> serve(AuthBasicHandler(dump_environ, realm, authfunc))
 serving on...
 
 .. [1] http://www.w3.org/Protocols/HTTP/1.0/draft-ietf-http-spec.html#BasicAA
 """
 from base64 import b64decode
 
-import six
-
 from paste.httpexceptions import HTTPUnauthorized
 from paste.httpheaders import (
     AUTHORIZATION,
     AUTH_TYPE,
     REMOTE_USER,
     WWW_AUTHENTICATE,
 )
@@ -49,15 +47,15 @@
     def authenticate(self, environ):
         authorization = AUTHORIZATION(environ)
         if not authorization:
             return self.build_authentication()
         (authmeth, auth) = authorization.split(' ', 1)
         if 'basic' != authmeth.lower():
             return self.build_authentication()
-        auth = six.ensure_text(b64decode(six.ensure_binary(auth.strip())))
+        auth = b64decode(auth.strip().encode('ascii')).decode('ascii')
         username, password = auth.split(':', 1)
         if self.authfunc(environ, username, password):
             return username
         return self.build_authentication()
 
     __call__ = authenticate
```

### Comparing `Paste-3.8.0/paste/auth/cas.py` & `Paste-3.9.0/paste/auth/cas.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 This implementation has the goal of maintaining current path arguments
 passed to the system so that it can be used as middleware at any stage
 of processing.  It has the secondary goal of allowing for other
 authentication methods to be used concurrently.
 """
 from urllib.parse import urlencode
+from urllib.request import urlopen
 from paste.request import construct_url
 from paste.httpexceptions import HTTPSeeOther, HTTPForbidden
 
 class CASLoginFailure(HTTPForbidden):
     """ The exception raised if the authority returns 'no' """
 
 class CASAuthenticate(HTTPSeeOther):
@@ -90,10 +91,10 @@
 
 __all__ = ['CASLoginFailure', 'CASAuthenticate', 'AuthCASHandler' ]
 
 if '__main__' == __name__:
     authority = "https://secure.its.yale.edu/cas/servlet/"
     from paste.wsgilib import dump_environ
     from paste.httpserver import serve
-    from paste.httpexceptions import *
+    from paste.httpexceptions import HTTPExceptionHandler
     serve(HTTPExceptionHandler(
              AuthCASHandler(dump_environ, authority)))
```

### Comparing `Paste-3.8.0/paste/auth/cookie.py` & `Paste-3.9.0/paste/auth/cookie.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,16 @@
   ...     return DataApp(page, content_type="text/html")(
   ...                    environ, start_response)
   >>> serve(AuthCookieHandler(testapp))
   serving on...
 
 """
 
-import hmac, base64, random, six, time, warnings
+import hmac, base64, random, time, warnings
+from functools import reduce
 try:
     from hashlib import sha1
 except ImportError:
     # NOTE: We have to use the callable with hashlib (hashlib.sha1),
     # otherwise hmac only accepts the sha module object itself
     import sha as sha1
 from paste.request import get_cookies
@@ -58,15 +59,15 @@
 # @@: Should this be using urllib.quote?
 # build encode/decode functions to safely pack away values
 _encode = [('\\', '\\x5c'), ('"', '\\x22'),
            ('=', '\\x3d'), (';', '\\x3b')]
 _decode = [(v, k) for (k, v) in _encode]
 _decode.reverse()
 def encode(s, sublist = _encode):
-    return six.moves.reduce((lambda a, b: a.replace(b[0], b[1])), sublist, str(s))
+    return reduce((lambda a, b: a.replace(b[0], b[1])), sublist, str(s))
 decode = lambda s: encode(s, _decode)
 
 class CookieTooLarge(RuntimeError):
     def __init__(self, content, cookie):
         RuntimeError.__init__("Signed cookie exceeds maximum size of 4096")
         self.content = content
         self.cookie = cookie
```

### Comparing `Paste-3.8.0/paste/auth/digest.py` & `Paste-3.9.0/paste/auth/digest.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/auth/form.py` & `Paste-3.9.0/paste/auth/form.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/auth/grantip.py` & `Paste-3.9.0/paste/auth/grantip.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/auth/multi.py` & `Paste-3.9.0/paste/auth/multi.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/auth/open_id.py` & `Paste-3.9.0/paste/auth/open_id.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/cascade.py` & `Paste-3.9.0/paste/cascade.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/cgiapp.py` & `Paste-3.9.0/paste/cgiapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,25 @@
 import sys
 import subprocess
 from urllib.parse import quote
 try:
     import select
 except ImportError:
     select = None
-import six
 
 from paste.util import converters
 
 __all__ = ['CGIError', 'CGIApplication']
 
+def ensure_text(s, encoding='utf-8', errors='strict'):
+    if type(s) is str:
+        return s
+    else:
+        return s.decode(encoding, errors)
+
 class CGIError(Exception):
     """
     Raised when the CGI script can't be found or doesn't
     act like a proper CGI script.
     """
 
 class CGIApplication:
@@ -36,15 +41,15 @@
     def __init__(self,
                  global_conf,
                  script,
                  path=None,
                  include_os_environ=True,
                  query_string=None):
         if global_conf:
-            raise NotImplemented(
+            raise NotImplementedError(
                 "global_conf is no longer supported for CGIApplication "
                 "(use make_cgi_application); please pass None instead")
         self.script_filename = script
         if path is None:
             path = os.environ.get('PATH', '').split(':')
         self.path = path
         if '?' in script:
@@ -154,15 +159,15 @@
                     if ' ' not in value:
                         # WSGI requires this space, sometimes CGI scripts don't set it:
                         value = '%s General' % value
                     self.status = value
                 else:
                     self.headers.append((name, value))
 
-class StdinReader(object):
+class StdinReader:
 
     def __init__(self, stdin, content_length):
         self.stdin = stdin
         self.content_length = content_length
 
     @classmethod
     def from_environ(cls, environ):
@@ -248,15 +253,15 @@
         if proc.stderr in rlist:
             data = os.read(proc.stderr.fileno(), 1024)
             if data == b"":
                 proc.stderr.close()
                 read_set.remove(proc.stderr)
             if trans_nl:
                 data = proc._translate_newlines(data)
-            stderr.write(six.ensure_text(data))
+            stderr.write(ensure_text(data))
 
     try:
         proc.wait()
     except OSError as e:
         if e.errno != 10:
             raise
```

### Comparing `Paste-3.8.0/paste/cgitb_catcher.py` & `Paste-3.9.0/paste/cgitb_catcher.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/config.py` & `Paste-3.9.0/paste/config.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/cowbell/__init__.py` & `Paste-3.9.0/paste/cowbell/__init__.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/cowbell/bell-ascending.png` & `Paste-3.9.0/paste/cowbell/bell-ascending.png`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/cowbell/bell-descending.png` & `Paste-3.9.0/paste/cowbell/bell-descending.png`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/debug/debugapp.py` & `Paste-3.9.0/paste/debug/debugapp.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/debug/doctest_webapp.py` & `Paste-3.9.0/paste/debug/doctest_webapp.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/debug/fsdiff.py` & `Paste-3.9.0/paste/debug/fsdiff.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/debug/prints.py` & `Paste-3.9.0/paste/debug/prints.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/debug/profile.py` & `Paste-3.9.0/paste/debug/profile.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/debug/testserver.py` & `Paste-3.9.0/paste/debug/testserver.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/debug/watchthreads.py` & `Paste-3.9.0/paste/debug/watchthreads.py`

 * *Files 4% similar despite different names*

```diff
@@ -270,37 +270,14 @@
     frame = frames[thread_id]
     out = StringIO()
     traceback.print_stack(frame, file=out)
     return out.getvalue()
 
 hide_keys = ['paste.httpserver.thread_pool']
 
-def format_environ(environ):
-    if environ is None:
-        return environ_template.substitute(
-            key='---',
-            value='No environment registered for this thread yet')
-    environ_rows = []
-    for key, value in sorted(environ.items()):
-        if key in hide_keys:
-            continue
-        try:
-            if key.upper() != key:
-                value = repr(value)
-            environ_rows.append(
-                environ_template.substitute(
-                key=cgi.escape(str(key)),
-                value=cgi.escape(str(value))))
-        except Exception as e:
-            environ_rows.append(
-                environ_template.substitute(
-                key=cgi.escape(str(key)),
-                value='Error in <code>repr()</code>: %s' % e))
-    return ''.join(environ_rows)
-
 def format_time(time_length):
     if time_length >= 60*60:
         # More than an hour
         time_string = '%i:%02i:%02i' % (int(time_length/60/60),
                                         int(time_length/60) % 60,
                                         time_length % 60)
     elif time_length >= 120:
```

### Comparing `Paste-3.8.0/paste/debug/wdg_validate.py` & `Paste-3.9.0/paste/debug/wdg_validate.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/errordocument.py` & `Paste-3.9.0/paste/errordocument.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/evalexception/evalcontext.py` & `Paste-3.9.0/paste/evalexception/evalcontext.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/evalexception/media/MochiKit.packed.js` & `Paste-3.9.0/paste/evalexception/media/MochiKit.packed.js`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/evalexception/media/debug.js` & `Paste-3.9.0/paste/evalexception/media/debug.js`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/evalexception/middleware.py` & `Paste-3.9.0/paste/evalexception/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 from paste import registry
 from paste import request
 from paste import response
 from paste.evalexception import evalcontext
 
 limit = 200
 
+def cmp(a, b):
+    return (a > b) - (a < b)
+
 def html_quote(v):
     """
     Escape HTML characters, plus translate None to ''
     """
     if v is None:
         return ''
     return html.escape(str(v), 1)
```

### Comparing `Paste-3.8.0/paste/exceptions/collector.py` & `Paste-3.9.0/paste/exceptions/collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,15 +378,15 @@
         return result
 
     def safeStr(self, obj):
         try:
             return str(obj)
         except UnicodeEncodeError:
             try:
-                return unicode(obj).encode(FALLBACK_ENCODING, 'replace')
+                return str(obj).encode(FALLBACK_ENCODING, 'replace')
             except UnicodeEncodeError:
                 # This is when something is really messed up, but this can
                 # happen when the __str__ of an object has to handle unicode
                 return repr(obj)
 
 limit = 200
```

### Comparing `Paste-3.8.0/paste/exceptions/errormiddleware.py` & `Paste-3.9.0/paste/exceptions/errormiddleware.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/exceptions/formatter.py` & `Paste-3.9.0/paste/exceptions/formatter.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/exceptions/reporter.py` & `Paste-3.9.0/paste/exceptions/reporter.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/exceptions/serial_number_generator.py` & `Paste-3.9.0/paste/exceptions/serial_number_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 """
 
 try:
     from hashlib import md5
 except ImportError:
     from md5 import md5
 
-import six
+import operator
+byte2int = operator.itemgetter(0)
 
 good_characters = "23456789abcdefghjkmnpqrtuvwxyz"
 
 base = len(good_characters)
 
 def make_identifier(number):
     """
@@ -67,15 +68,15 @@
         s = str(s)
         s = s.encode('utf-8')
     h = hasher(s)
     bin_hash = h.digest()
     modulo = base ** length
     number = 0
     for c in list(bin_hash):
-        number = (number * 256 + six.byte2int([c])) % modulo
+        number = (number * 256 + byte2int([c])) % modulo
     ident = make_identifier(number)
     if pad:
         ident = good_characters[0]*(length-len(ident)) + ident
     if group:
         parts = []
         while ident:
             parts.insert(0, ident[-group:])
```

### Comparing `Paste-3.8.0/paste/fileapp.py` & `Paste-3.9.0/paste/fileapp.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,37 @@
 """
 This module handles sending static content such as in-memory data or
 files.  At this time it has cache helpers and understands the
 if-modified-since request header.
 """
 
 import os, time, mimetypes, zipfile, tarfile
-from paste.httpexceptions import *
-from paste.httpheaders import *
+from paste.httpexceptions import (
+    HTTPBadRequest,
+    HTTPForbidden,
+    HTTPMethodNotAllowed,
+    HTTPNotFound,
+    HTTPRequestRangeNotSatisfiable,
+)
+from paste.httpheaders import (
+    get_header,
+    list_headers,
+    ACCEPT_RANGES,
+    CACHE_CONTROL,
+    CONTENT_DISPOSITION,
+    CONTENT_LENGTH,
+    CONTENT_RANGE,
+    CONTENT_TYPE,
+    ETAG,
+    EXPIRES,
+    IF_MODIFIED_SINCE,
+    IF_NONE_MATCH,
+    LAST_MODIFIED,
+    RANGE,
+)
 
 CACHE_SIZE = 4096
 BLOCK_SIZE = 4096 * 16
 
 __all__ = ['DataApp', 'FileApp', 'DirectoryApp', 'ArchiveStore']
 
 class DataApp(object):
```

### Comparing `Paste-3.8.0/paste/fixture.py` & `Paste-3.9.0/paste/fixture.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,32 @@
 import shutil
 import smtplib
 import shlex
 import re
 import subprocess
 from urllib.parse import urlencode
 from urllib import parse as urlparse
-from six.moves.http_cookies import BaseCookie
-import six
+from http.cookies import BaseCookie
 
 from paste import wsgilib
 from paste import lint
 from paste.response import HeaderDict
 
+def ensure_binary(s):
+    if isinstance(s, bytes):
+        return s
+    else:
+        return s.encode('utf-8')
+
+def ensure_str(s, encoding='utf-8', errors='strict'):
+    if type(s) is str:
+        return s
+    else:
+        return s.decode(encoding, errors)
+
 def tempnam_no_warning(*args):
     """
     An os.tempnam with the warning turned off, because sometimes
     you just need to use this and don't care about the stupid
     security warning.
     """
     return os.tempnam(*args)
@@ -329,26 +340,26 @@
         boundary = '----------a_BoUnDaRy%s$' % random.random()
         content_type = 'multipart/form-data; boundary=%s' % boundary
         boundary = boundary.encode('ascii')
 
         lines = []
         for key, value in params:
             lines.append(b'--'+boundary)
-            line = b'Content-Disposition: form-data; name="%s"' % six.ensure_binary(key)
+            line = b'Content-Disposition: form-data; name="%s"' % ensure_binary(key)
             lines.append(line)
             lines.append(b'')
-            line = six.ensure_binary(value)
+            line = ensure_binary(value)
             lines.append(line)
         for file_info in files:
             key, filename, value = self._get_file_info(file_info)
             lines.append(b'--'+boundary)
             line = (b'Content-Disposition: form-data; name="%s"; filename="%s"'
-                         % (six.ensure_binary(key), six.ensure_binary(filename)))
+                         % (ensure_binary(key), ensure_binary(filename)))
             lines.append(line)
-            fcontent = mimetypes.guess_type(six.ensure_str(filename, 'ascii', 'ignore'))[0]
+            fcontent = mimetypes.guess_type(ensure_str(filename, 'ascii', 'ignore'))[0]
             line = (b'Content-Type: %s'
                     % (fcontent.encode('ascii') if fcontent else b'application/octet-stream'))
             lines.append(line)
             lines.append(b'')
             lines.append(value)
         lines.append(b'--' + boundary + b'--')
         lines.append(b'')
```

### Comparing `Paste-3.8.0/paste/flup_session.py` & `Paste-3.9.0/paste/flup_session.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/gzipper.py` & `Paste-3.9.0/paste/gzipper.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/httpexceptions.py` & `Paste-3.9.0/paste/httpexceptions.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/httpheaders.py` & `Paste-3.9.0/paste/httpheaders.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/httpserver.py` & `Paste-3.9.0/paste/httpserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 import traceback
 import io
 import socket, sys, threading
 import posixpath
 import time
 import os
 from itertools import count
-from six.moves import _thread
-from six.moves import queue
-from six.moves.BaseHTTPServer import BaseHTTPRequestHandler, HTTPServer
-from six.moves.socketserver import ThreadingMixIn
+import _thread
+import queue
+from http.server import BaseHTTPRequestHandler, HTTPServer
+from socketserver import ThreadingMixIn
 from urllib.parse import unquote, urlsplit
 from paste.util import converters
 import logging
 try:
     from paste.util import killthread
 except ImportError:
     # Not available, probably no ctypes
```

### Comparing `Paste-3.8.0/paste/lint.py` & `Paste-3.9.0/paste/lint.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/modpython.py` & `Paste-3.9.0/paste/modpython.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/pony.py` & `Paste-3.9.0/paste/pony.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/progress.py` & `Paste-3.9.0/paste/progress.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/proxy.py` & `Paste-3.9.0/paste/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     use = egg:Paste#proxy
     address = http://server3:8680/exist/rest/db/orgs/sch/config/
     allowed_request_methods = GET
 
 """
 
-from six.moves import http_client as httplib
+import http.client as httplib
 from urllib import parse as urlparse
 from urllib.parse import quote
 
 from paste import httpexceptions
 from paste.util.converters import aslist
 
 # Remove these headers from response (specify lower case header
```

### Comparing `Paste-3.8.0/paste/recursive.py` & `Paste-3.9.0/paste/recursive.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/registry.py` & `Paste-3.9.0/paste/registry.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/reloader.py` & `Paste-3.9.0/paste/reloader.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/request.py` & `Paste-3.9.0/paste/request.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/response.py` & `Paste-3.9.0/paste/response.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/session.py` & `Paste-3.9.0/paste/session.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/transaction.py` & `Paste-3.9.0/paste/transaction.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/translogger.py` & `Paste-3.9.0/paste/translogger.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 Middleware for logging requests, using Apache combined log format
 """
 
 import logging
 import time
-from six.moves.urllib.parse import quote
+from urllib.parse import quote
 
 class TransLogger:
     """
     This logging middleware will log all requests as they go through.
     They are, by default, sent to a logger named ``'wsgi'`` at the
     INFO level.
```

### Comparing `Paste-3.8.0/paste/url.py` & `Paste-3.9.0/paste/url.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/urlmap.py` & `Paste-3.9.0/paste/urlmap.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/urlparser.py` & `Paste-3.9.0/paste/urlparser.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/util/PySourceColor.py` & `Paste-3.9.0/paste/util/PySourceColor.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/util/classinit.py` & `Paste-3.9.0/paste/util/classinit.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/util/classinstance.py` & `Paste-3.9.0/paste/util/classinstance.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/util/converters.py` & `Paste-3.9.0/paste/util/converters.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/util/dateinterval.py` & `Paste-3.9.0/paste/util/dateinterval.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/util/datetimeutil.py` & `Paste-3.9.0/paste/util/datetimeutil.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/util/filemixin.py` & `Paste-3.9.0/paste/util/filemixin.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/util/finddata.py` & `Paste-3.9.0/paste/util/finddata.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/util/findpackage.py` & `Paste-3.9.0/paste/util/findpackage.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/util/import_string.py` & `Paste-3.9.0/paste/util/import_string.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/util/intset.py` & `Paste-3.9.0/paste/util/intset.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/util/ip4.py` & `Paste-3.9.0/paste/util/ip4.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/util/killthread.py` & `Paste-3.9.0/paste/util/killthread.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/util/looper.py` & `Paste-3.9.0/paste/util/looper.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/util/mimeparse.py` & `Paste-3.9.0/paste/util/mimeparse.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/util/multidict.py` & `Paste-3.9.0/paste/util/multidict.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/util/quoting.py` & `Paste-3.9.0/paste/util/quoting.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # (c) 2005 Ian Bicking and contributors; written for Paste (http://pythonpaste.org)
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 
+import html
+import html.entities
 import re
-from six.moves import html_entities
 from urllib.parse import quote, unquote
-import six
-
-import html
-
 
 __all__ = ['html_quote', 'html_unquote', 'url_quote', 'url_unquote',
            'strip_html']
 
 default_encoding = 'UTF-8'
 
 def html_quote(v, encoding=None):
@@ -26,18 +23,18 @@
         return html.escape(v.decode(encoding), 1).encode(encoding)
     elif isinstance(v, str):
         return html.escape(v, 1)
     else:
         return html.escape(str(v), 1)
 
 _unquote_re = re.compile(r'&([a-zA-Z]+);')
-def _entity_subber(match, name2c=html_entities.name2codepoint):
+def _entity_subber(match, name2c=html.entities.name2codepoint):
     code = name2c.get(match.group(1))
     if code:
-        return six.unichr(code)
+        return chr(code)
     else:
         return match.group(0)
 
 def html_unquote(s, encoding=None):
     r"""
     Decode the value.
```

### Comparing `Paste-3.8.0/paste/util/scgiserver.py` & `Paste-3.9.0/paste/util/scgiserver.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/util/template.py` & `Paste-3.9.0/paste/util/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,27 +27,37 @@
 ``sub(content, **kw)`` substitutes the template immediately.  You
 can use ``__name='tmpl.html'`` to set the name of the template.
 
 If there are syntax errors ``TemplateError`` will be raised.
 """
 
 import re
-import six
 import sys
 from html import escape
 from urllib.parse import quote
 from paste.util.looper import looper
 
 __all__ = ['TemplateError', 'Template', 'sub', 'HTMLTemplate',
            'sub_html', 'html', 'bunch']
 
 token_re = re.compile(r'\{\{|\}\}')
 in_re = re.compile(r'\s+in\s+')
 var_re = re.compile(r'^[a-z_][a-z0-9_]*$', re.I)
 
+def reraise(tp, value, tb=None):
+    try:
+        if value is None:
+            value = tp()
+        if value.__traceback__ is not tb:
+            raise value.with_traceback(tb)
+        raise value
+    finally:
+        value = None
+        tb = None
+
 class TemplateError(Exception):
     """Exception raised while parsing a template
     """
 
     def __init__(self, message, position, name=None):
         self.message = message
         self.position = position
@@ -204,37 +214,37 @@
             exc_info = sys.exc_info()
             e = exc_info[1]
             if getattr(e, 'args'):
                 arg0 = e.args[0]
             else:
                 arg0 = str(e)
             e.args = (self._add_line_info(arg0, pos),)
-            six.reraise(exc_info[0], e, exc_info[2])
+            reraise(exc_info[0], e, exc_info[2])
 
     def _exec(self, code, ns, pos):
         __traceback_hide__ = True
         try:
             exec(code, ns)
         except:
             exc_info = sys.exc_info()
             e = exc_info[1]
             e.args = (self._add_line_info(e.args[0], pos),)
-            six.reraise(exc_info[0], e, exc_info[2])
+            reraise(exc_info[0], e, exc_info[2])
 
     def _repr(self, value, pos):
         __traceback_hide__ = True
         try:
             if value is None:
                 return ''
             value = str(value)
         except:
             exc_info = sys.exc_info()
             e = exc_info[1]
             e.args = (self._add_line_info(e.args[0], pos),)
-            six.reraise(exc_info[0], e, exc_info[2])
+            reraise(exc_info[0], e, exc_info[2])
         else:
             if self._unicode and isinstance(value, bytes):
                 if not self.decode_encoding:
                     raise UnicodeDecodeError(
                         'Cannot decode str value %r into unicode '
                         '(no default_encoding provided)' % value)
                 value = value.decode(self.default_encoding)
```

### Comparing `Paste-3.8.0/paste/util/threadedprint.py` & `Paste-3.9.0/paste/util/threadedprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             self._defaultfunc = self._writeerror
         self._default = default
         self._factory = factory
         self._paramwriter = paramwriter
         self._catchers = {}
 
     def write(self, v, currentThread=threading.current_thread):
-        name = current_thread().name
+        name = currentThread().name
         catchers = self._catchers
         if not catchers.has_key(name):
             self._defaultfunc(name, v)
         else:
             catcher = catchers[name]
             catcher.write(v)
```

### Comparing `Paste-3.8.0/paste/util/threadinglocal.py` & `Paste-3.9.0/paste/util/threadinglocal.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/wsgilib.py` & `Paste-3.9.0/paste/wsgilib.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/paste/wsgiwrappers.py` & `Paste-3.9.0/paste/wsgiwrappers.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/setup.py` & `Paste-3.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # - update version in setup.py (__version__)
 # - update changelog: docs/news.txt
 # - commit and push to git
 # - make release
 #
 # The final step will release to pypi and to Github
 
-__version__ = '3.8.0'
+__version__ = '3.9.0'
 
 from setuptools import setup, find_packages
 import sys, os
 sys.path.append(os.path.join(os.path.dirname(__file__),
                                 'paste', 'util'))
 import finddata
 
@@ -52,15 +52,14 @@
       packages=find_packages(exclude=['ez_setup', 'examples', 'packages', 'tests*']),
       package_data=finddata.find_package_data(
           exclude_directories=finddata.standard_exclude_directories + ('tests',)),
       namespace_packages=['paste'],
       zip_safe=False,
       install_requires=[
         'setuptools',  # pkg_resources
-        'six>=1.4.0',
         ],
       extras_require={
         'subprocess': [],
         'hotshot': [],
         'Flup': ['flup'],
         'Paste': [],
         'openid': ['python-openid'],
```

### Comparing `Paste-3.8.0/tests/cgiapp_data/form.cgi` & `Paste-3.9.0/tests/cgiapp_data/form.cgi`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/tests/template.txt` & `Paste-3.9.0/tests/template.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/tests/test_auth/test_auth_cookie.py` & `Paste-3.9.0/tests/test_auth/test_auth_cookie.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # (c) 2005 Clark C. Evans
 # This module is part of the Python Paste Project and is released under
 # the MIT License: http://www.opensource.org/licenses/mit-license.php
 
 from paste.auth import cookie
 from paste.wsgilib import raw_interactive, dump_environ
 from paste.response import header_value
-from paste.httpexceptions import *
 
 def build(application,setenv, *args, **kwargs):
     def setter(environ, start_response):
         save = environ['paste.auth.cookie'].append
         for (k,v) in setenv.items():
             save(k)
             environ[k] = v
```

### Comparing `Paste-3.8.0/tests/test_auth/test_auth_digest.py` & `Paste-3.9.0/tests/test_auth/test_auth_digest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # (c) 2005 Clark C. Evans
 # This module is part of the Python Paste Project and is released under
 # the MIT License: http://www.opensource.org/licenses/mit-license.php
 
-from paste.auth.digest import *
+from paste.auth.digest import digest_password, AuthDigestHandler
 from paste.wsgilib import raw_interactive
-from paste.httpexceptions import *
+from paste.httpexceptions import HTTPExceptionHandler
 from paste.httpheaders import AUTHORIZATION, WWW_AUTHENTICATE, REMOTE_USER
 import os
 
 def application(environ, start_response):
     content = REMOTE_USER(environ)
     start_response("200 OK",(('Content-Type', 'text/plain'),
                              ('Content-Length', len(content))))
```

### Comparing `Paste-3.8.0/tests/test_auth/test_auth_tkt.py` & `Paste-3.9.0/tests/test_auth/test_auth_tkt.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/tests/test_cgiapp.py` & `Paste-3.9.0/tests/test_cgiapp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 
 import pytest
 
 from paste.cgiapp import CGIApplication, CGIError
-from paste.fixture import *
+from paste.fixture import TestApp
 
 data_dir = os.path.join(os.path.dirname(__file__), 'cgiapp_data')
 
 # these CGI scripts can't work on Windows or Jython
 if sys.platform != 'win32' and not sys.platform.startswith('java'):
 
     # Ensure the CGI scripts are called with the same python interpreter. Put a
```

### Comparing `Paste-3.8.0/tests/test_cgitb_catcher.py` & `Paste-3.9.0/tests/test_cgitb_catcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from paste.fixture import *
+from paste.fixture import TestApp
 from paste.cgitb_catcher import CgitbMiddleware
 from paste import lint
 from .test_exceptions.test_error_middleware import clear_middleware
 
 def do_request(app, expect_status=500):
     app = lint.middleware(app)
     app = CgitbMiddleware(app, {}, display=True)
```

### Comparing `Paste-3.8.0/tests/test_config.py` & `Paste-3.9.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/tests/test_doctests.py` & `Paste-3.9.0/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/tests/test_errordocument.py` & `Paste-3.9.0/tests/test_errordocument.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from paste.errordocument import forward
-from paste.fixture import *
+from paste.fixture import TestApp
 from paste.recursive import RecursiveMiddleware
 
 def simple_app(environ, start_response):
     start_response("200 OK", [('Content-type', 'text/plain')])
     return [b'requested page returned']
 
 def not_found_app(environ, start_response):
```

### Comparing `Paste-3.8.0/tests/test_exceptions/test_error_middleware.py` & `Paste-3.9.0/tests/test_exceptions/test_error_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from paste.fixture import *
+from paste.fixture import TestApp
 from paste.exceptions.errormiddleware import ErrorMiddleware
 from paste import lint
 from paste.util.quoting import strip_html
 #
 # For some strange reason, these 4 lines cannot be removed or the regression
 # test breaks; is it counting the number of lines in the file somehow?
 #
```

### Comparing `Paste-3.8.0/tests/test_exceptions/test_formatter.py` & `Paste-3.9.0/tests/test_exceptions/test_formatter.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/tests/test_exceptions/test_httpexceptions.py` & `Paste-3.9.0/tests/test_exceptions/test_httpexceptions.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/tests/test_exceptions/test_reporter.py` & `Paste-3.9.0/tests/test_exceptions/test_reporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 import os
-from paste.exceptions.reporter import *
+from paste.exceptions.reporter import LogReporter
 from paste.exceptions import collector
 
 def setup_file(fn, content=None):
     dir = os.path.join(os.path.dirname(__file__), 'reporter_output')
     fn = os.path.join(dir, fn)
     if os.path.exists(dir):
         if os.path.exists(fn):
```

### Comparing `Paste-3.8.0/tests/test_fileapp.py` & `Paste-3.9.0/tests/test_fileapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import time
 import random
 import os
 import tempfile
 from email.utils import parsedate_tz, mktime_tz
 
 from paste import fileapp
-from paste.fileapp import *
-from paste.fixture import *
+from paste.fileapp import DataApp
+from paste.fixture import TestApp
 
 # NOTE(haypo): don't use string.letters because the order of lower and upper
 # case letters changes when locale.setlocale() is called for the first time
 LETTERS = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ'
 
 def test_data():
     harness = TestApp(DataApp(b'mycontent'))
```

### Comparing `Paste-3.8.0/tests/test_fixture.py` & `Paste-3.9.0/tests/test_fixture.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import cgi
-
 from paste.debug.debugapp import SimpleApplication, SlowConsumer
 from paste.fixture import TestApp
 from paste.wsgiwrappers import WSGIRequest
 
 
 def test_fixture():
     app = TestApp(SimpleApplication())
```

### Comparing `Paste-3.8.0/tests/test_grantip.py` & `Paste-3.9.0/tests/test_grantip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from paste.auth import grantip
-from paste.fixture import *
+from paste.fixture import TestApp
 
 def _make_app():
     def application(environ, start_response):
         start_response('200 OK', [('content-type', 'text/plain')])
         lines = [
             str(environ.get('REMOTE_USER')),
             ':',
```

### Comparing `Paste-3.8.0/tests/test_gzipper.py` & `Paste-3.9.0/tests/test_gzipper.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/tests/test_httpheaders.py` & `Paste-3.9.0/tests/test_httpheaders.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/tests/test_httpserver.py` & `Paste-3.9.0/tests/test_httpserver.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/tests/test_multidict.py` & `Paste-3.9.0/tests/test_multidict.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/tests/test_profilemiddleware.py` & `Paste-3.9.0/tests/test_profilemiddleware.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from paste.fixture import *
+from paste.fixture import TestApp
 try:
-    from paste.debug.profile import *
+    from paste.debug.profile import ProfileMiddleware, profile_decorator
     disable = False
 except ImportError:
     disable = True
 
 if not disable:
     def simple_app(environ, start_response):
         start_response('200 OK', [('content-type', 'text/html')])
```

### Comparing `Paste-3.8.0/tests/test_proxy.py` & `Paste-3.9.0/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/tests/test_recursive.py` & `Paste-3.9.0/tests/test_recursive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .test_errordocument import simple_app
-from paste.fixture import *
+from paste.fixture import TestApp
 from paste.recursive import RecursiveMiddleware, ForwardRequestException
 
 def error_docs_app(environ, start_response):
     if environ['PATH_INFO'] == '/not_found':
         start_response("404 Not found", [('Content-type', 'text/plain')])
         return [b'Not found']
     elif environ['PATH_INFO'] == '/error':
```

### Comparing `Paste-3.8.0/tests/test_registry.py` & `Paste-3.9.0/tests/test_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # (c) 2005 Ben Bangert
 # This module is part of the Python Paste Project and is released under
 # the MIT License: http://www.opensource.org/licenses/mit-license.php
 
 import pytest
 
-from paste.fixture import *
-from paste.registry import *
-from paste.registry import Registry
+from paste.fixture import TestApp
+from paste.registry import (
+    Registry,
+    RegistryManager,
+    StackedObjectProxy,
+    restorer,
+)
 from paste.evalexception.middleware import EvalException
 
 regobj = StackedObjectProxy()
 secondobj = StackedObjectProxy(default=dict(hi='people'))
 
 def simpleapp(environ, start_response):
     status = '200 OK'
```

### Comparing `Paste-3.8.0/tests/test_request.py` & `Paste-3.9.0/tests/test_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # (c) 2005 Ben Bangert
 # This module is part of the Python Paste Project and is released under
 # the MIT License: http://www.opensource.org/licenses/mit-license.php
-from paste.fixture import *
-from paste.request import *
+from paste.fixture import TestApp
+from paste.request import get_cookie_dict
 from paste.wsgiwrappers import WSGIRequest
 
 def simpleapp(environ, start_response):
     status = '200 OK'
     response_headers = [('Content-type','text/plain')]
     start_response(status, response_headers)
     request = WSGIRequest(environ)
```

### Comparing `Paste-3.8.0/tests/test_request_form.py` & `Paste-3.9.0/tests/test_request_form.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import io
 
-from paste.request import *
+from paste.request import parse_formvars, parse_querystring
 from paste.util.multidict import MultiDict
 
 def test_parse_querystring():
     e = {'QUERY_STRING': 'a=1&b=2&c=3&b=4'}
     d = parse_querystring(e)
     assert d == [('a', '1'), ('b', '2'), ('c', '3'), ('b', '4')]
     assert e['paste.parsed_querystring'] == (
```

### Comparing `Paste-3.8.0/tests/test_session.py` & `Paste-3.9.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/tests/test_urlmap.py` & `Paste-3.9.0/tests/test_urlmap.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/tests/test_urlparser.py` & `Paste-3.9.0/tests/test_urlparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
-from paste.urlparser import *
-from paste.fixture import *
+
+from paste.urlparser import PkgResourcesParser, StaticURLParser, URLParser
+from paste.fixture import TestApp
 from pkg_resources import get_distribution
 
 def relative_path(name):
     here = os.path.join(os.path.dirname(os.path.abspath(__file__)),
                         'urlparser_data')
     f = os.path.join('urlparser_data', '..', 'urlparser_data', name)
     return os.path.join(here, f)
```

### Comparing `Paste-3.8.0/tests/test_util/test_datetimeutil.py` & `Paste-3.9.0/tests/test_util/test_datetimeutil.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/tests/test_util/test_mimeparse.py` & `Paste-3.9.0/tests/test_util/test_mimeparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # (c) 2010 Ch. Zwerschke and contributors
 # This module is part of the Python Paste Project and is released under
 # the MIT License: http://www.opensource.org/licenses/mit-license.php
 
-from paste.util.mimeparse import *
+from paste.util.mimeparse import (
+    best_match,
+    desired_matches,
+    fitness_and_quality_parsed,
+    parse_media_range,
+    parse_mime_type,
+    quality,
+    quality_parsed,
+)
 
 def test_parse_mime_type():
     parse = parse_mime_type
     assert parse('*/*') == ('*', '*', {})
     assert parse('text/html') == ('text', 'html', {})
     assert parse('audio/*; q=0.2') == ('audio', '*', {'q': '0.2'})
     assert parse('text/x-dvi;level=1') == ('text', 'x-dvi', {'level': '1'})
```

### Comparing `Paste-3.8.0/tests/test_util/test_quoting.py` & `Paste-3.9.0/tests/test_util/test_quoting.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/tests/test_wsgilib.py` & `Paste-3.9.0/tests/test_wsgilib.py`

 * *Files identical despite different names*

### Comparing `Paste-3.8.0/tests/test_wsgiwrappers.py` & `Paste-3.9.0/tests/test_wsgiwrappers.py`

 * *Files identical despite different names*

