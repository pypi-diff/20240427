# Comparing `tmp/django_querysets_single_query_fetch-0.0.5.tar.gz` & `tmp/django_querysets_single_query_fetch-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_querysets_single_query_fetch-0.0.5.tar", last modified: Tue Mar 26 13:10:05 2024, max compression
+gzip compressed data, was "django_querysets_single_query_fetch-0.0.6.tar", last modified: Fri Apr 26 16:58:49 2024, max compression
```

## Comparing `django_querysets_single_query_fetch-0.0.5.tar` & `django_querysets_single_query_fetch-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 nishantsingh   (501) staff       (20)        0 2024-03-26 13:10:05.574560 django_querysets_single_query_fetch-0.0.5/
--rw-r--r--   0 nishantsingh   (501) staff       (20)      286 2024-03-26 13:10:05.574236 django_querysets_single_query_fetch-0.0.5/PKG-INFO
--rw-r--r--   0 nishantsingh   (501) staff       (20)     3037 2024-03-11 09:28:08.000000 django_querysets_single_query_fetch-0.0.5/README.md
-drwxr-xr-x   0 nishantsingh   (501) staff       (20)        0 2024-03-26 13:10:05.572145 django_querysets_single_query_fetch-0.0.5/django_querysets_single_query_fetch/
--rw-rw-r--   0 nishantsingh   (501) staff       (20)        0 2024-02-21 16:23:03.000000 django_querysets_single_query_fetch-0.0.5/django_querysets_single_query_fetch/__init__.py
--rw-rw-r--   0 nishantsingh   (501) staff       (20)      198 2024-02-21 17:09:35.000000 django_querysets_single_query_fetch-0.0.5/django_querysets_single_query_fetch/apps.py
--rw-r--r--   0 nishantsingh   (501) staff       (20)    16463 2024-03-26 13:09:40.000000 django_querysets_single_query_fetch-0.0.5/django_querysets_single_query_fetch/service.py
-drwxr-xr-x   0 nishantsingh   (501) staff       (20)        0 2024-03-26 13:10:05.573902 django_querysets_single_query_fetch-0.0.5/django_querysets_single_query_fetch.egg-info/
--rw-r--r--   0 nishantsingh   (501) staff       (20)      286 2024-03-26 13:10:05.000000 django_querysets_single_query_fetch-0.0.5/django_querysets_single_query_fetch.egg-info/PKG-INFO
--rw-r--r--   0 nishantsingh   (501) staff       (20)      509 2024-03-26 13:10:05.000000 django_querysets_single_query_fetch-0.0.5/django_querysets_single_query_fetch.egg-info/SOURCES.txt
--rw-r--r--   0 nishantsingh   (501) staff       (20)        1 2024-03-26 13:10:05.000000 django_querysets_single_query_fetch-0.0.5/django_querysets_single_query_fetch.egg-info/dependency_links.txt
--rw-r--r--   0 nishantsingh   (501) staff       (20)        1 2024-02-21 16:46:05.000000 django_querysets_single_query_fetch-0.0.5/django_querysets_single_query_fetch.egg-info/not-zip-safe
--rw-r--r--   0 nishantsingh   (501) staff       (20)        9 2024-03-26 13:10:05.000000 django_querysets_single_query_fetch-0.0.5/django_querysets_single_query_fetch.egg-info/requires.txt
--rw-r--r--   0 nishantsingh   (501) staff       (20)       36 2024-03-26 13:10:05.000000 django_querysets_single_query_fetch-0.0.5/django_querysets_single_query_fetch.egg-info/top_level.txt
--rw-r--r--   0 nishantsingh   (501) staff       (20)       38 2024-03-26 13:10:05.574620 django_querysets_single_query_fetch-0.0.5/setup.cfg
--rw-r--r--   0 nishantsingh   (501) staff       (20)      511 2024-03-26 13:09:40.000000 django_querysets_single_query_fetch-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:58:49.184812 django_querysets_single_query_fetch-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-26 16:58:49.184812 django_querysets_single_query_fetch-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-26 16:58:32.000000 django_querysets_single_query_fetch-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:58:49.180812 django_querysets_single_query_fetch-0.0.6/django_querysets_single_query_fetch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:58:32.000000 django_querysets_single_query_fetch-0.0.6/django_querysets_single_query_fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-26 16:58:32.000000 django_querysets_single_query_fetch-0.0.6/django_querysets_single_query_fetch/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16589 2024-04-26 16:58:32.000000 django_querysets_single_query_fetch-0.0.6/django_querysets_single_query_fetch/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:58:49.180812 django_querysets_single_query_fetch-0.0.6/django_querysets_single_query_fetch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-26 16:58:49.000000 django_querysets_single_query_fetch-0.0.6/django_querysets_single_query_fetch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-26 16:58:49.000000 django_querysets_single_query_fetch-0.0.6/django_querysets_single_query_fetch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:58:49.000000 django_querysets_single_query_fetch-0.0.6/django_querysets_single_query_fetch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:58:49.000000 django_querysets_single_query_fetch-0.0.6/django_querysets_single_query_fetch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 16:58:49.000000 django_querysets_single_query_fetch-0.0.6/django_querysets_single_query_fetch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-26 16:58:49.000000 django_querysets_single_query_fetch-0.0.6/django_querysets_single_query_fetch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:58:49.184812 django_querysets_single_query_fetch-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-26 16:58:32.000000 django_querysets_single_query_fetch-0.0.6/setup.py
```

### Comparing `django_querysets_single_query_fetch-0.0.5/README.md` & `django_querysets_single_query_fetch-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `django_querysets_single_query_fetch-0.0.5/django_querysets_single_query_fetch/service.py` & `django_querysets_single_query_fetch-0.0.6/django_querysets_single_query_fetch/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     FlatValuesListIterable,
     ModelIterable,
     ValuesIterable,
     ValuesListIterable,
     get_related_populators,
 )
 from django.utils.dateparse import parse_datetime
+from psycopg2.extensions import QuotedString
 
 logger = logging.getLogger(__name__)
 
 
 class QuerysetCountWrapper:
     """
     Wrapper around queryset to indicate that we want to fetch count of the queryset
@@ -185,19 +186,18 @@
             )  # add col aliases other wise json
             # build object cant handle same column name from two tables => two duplicate keys in dict
             # (one primary, one joined for example)
         except EmptyResultSet:
             return ""
 
         for param in params:
-            if (
-                isinstance(param, str)
-                or isinstance(param, UUID)
-                or isinstance(param, datetime.datetime)
-            ):
+            if isinstance(param, str):
+                # this is to handle special char handling
+                param = QuotedString(param).getquoted().decode("utf-8")
+            elif isinstance(param, UUID) or isinstance(param, datetime.datetime):
                 param = f"'{param}'"
             elif isinstance(param, int) or isinstance(param, float):
                 # type which can be passed as is
                 pass
             else:
                 # keep strict
                 raise ValueError(f"Unsupported param type: {type(param)}")
@@ -313,17 +313,17 @@
                     pass  # May happen in qs1 | qs2 scenarios.
                 else:
                     setattr(obj, field.name, rel_obj)
 
             obj_fields_cache = {}
             # because of json_agg some field level parsing/handling broke, patch it for prefetched objects
             for prefetched_obj_name, prefetched_obj in obj._state.fields_cache.items():
-                obj_fields_cache[
-                    prefetched_obj_name
-                ] = self._transform_object_to_handle_json_agg(obj=prefetched_obj)
+                obj_fields_cache[prefetched_obj_name] = (
+                    self._transform_object_to_handle_json_agg(obj=prefetched_obj)
+                )
             obj._state.fields_cache = obj_fields_cache
             instances.append(obj)
         return instances
 
     def _convert_raw_results_to_final_queryset_results(
         self, queryset: QuerySet, queryset_raw_results: list
     ):
@@ -364,23 +364,21 @@
                 final_result_list.append(
                     None
                 )  # will be replaced by actual result below
 
         non_empty_django_sqls_for_querysets = [
             sql for sql in django_sqls_for_querysets if sql
         ]
-
         if non_empty_django_sqls_for_querysets:
             raw_sql = f"""
                 SELECT
                     json_build_object(
                         {', '.join([f"'{i}', {sql}" for i, sql in enumerate(non_empty_django_sqls_for_querysets)])}
                 )
             """
-
             with connections["default"].cursor() as cursor:
                 cursor.execute(raw_sql, params={})
                 raw_sql_result_dict: dict = cursor.fetchone()[0]
         else:
             # all querysets are always empty (EmptyResultSet)
             raw_sql_result_dict = {}
```

