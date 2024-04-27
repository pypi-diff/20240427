# Comparing `tmp/nestipy_peewee-0.1.0.tar.gz` & `tmp/nestipy_peewee-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy_peewee-0.1.0.tar", max compression
+gzip compressed data, was "nestipy_peewee-0.1.1.tar", max compression
```

## Comparing `nestipy_peewee-0.1.0.tar` & `nestipy_peewee-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-27 06:25:16.659735 nestipy_peewee-0.1.0/README.md
--rw-r--r--   0        0        0      464 2024-04-27 06:37:05.039788 nestipy_peewee-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      185 2024-04-27 07:50:37.316624 nestipy_peewee-0.1.0/src/nestipy_peewee/__init__.py
--rw-r--r--   0        0        0      500 2024-04-27 07:10:46.368156 nestipy_peewee-0.1.0/src/nestipy_peewee/peewee_builder.py
--rw-r--r--   0        0        0      402 2024-04-27 07:49:49.760614 nestipy_peewee-0.1.0/src/nestipy_peewee/peewee_decorator.py
--rw-r--r--   0        0        0       58 2024-04-27 06:47:04.319886 nestipy_peewee-0.1.0/src/nestipy_peewee/peewee_meta.py
--rw-r--r--   0        0        0     2327 2024-04-27 07:50:28.188622 nestipy_peewee-0.1.0/src/nestipy_peewee/peewee_module.py
--rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 nestipy_peewee-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy_peewee-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy_peewee-0.1.1/README.md
+-rw-r--r--   0        0        0      464 2024-04-27 15:34:53.188705 nestipy_peewee-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      185 2024-04-27 07:50:37.316624 nestipy_peewee-0.1.1/src/nestipy_peewee/__init__.py
+-rw-r--r--   0        0        0      500 2024-04-27 07:10:46.368156 nestipy_peewee-0.1.1/src/nestipy_peewee/peewee_builder.py
+-rw-r--r--   0        0        0      402 2024-04-27 07:49:49.760614 nestipy_peewee-0.1.1/src/nestipy_peewee/peewee_decorator.py
+-rw-r--r--   0        0        0       58 2024-04-27 06:47:04.319886 nestipy_peewee-0.1.1/src/nestipy_peewee/peewee_meta.py
+-rw-r--r--   0        0        0     2327 2024-04-27 07:50:28.188622 nestipy_peewee-0.1.1/src/nestipy_peewee/peewee_module.py
+-rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 nestipy_peewee-0.1.1/PKG-INFO
```

### Comparing `nestipy_peewee-0.1.0/src/nestipy_peewee/peewee_module.py` & `nestipy_peewee-0.1.1/src/nestipy_peewee/peewee_module.py`

 * *Files identical despite different names*

