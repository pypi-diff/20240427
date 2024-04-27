# Comparing `tmp/django-torque-0.5.7.tar.gz` & `tmp/django_torque-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-torque-0.5.7.tar", last modified: Fri Jan 26 22:59:56 2024, max compression
+gzip compressed data, was "django_torque-0.6.0.tar", last modified: Sat Apr 27 17:49:01 2024, max compression
```

## Comparing `django-torque-0.5.7.tar` & `django_torque-0.6.0.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-01-26 22:59:56.094587 django-torque-0.5.7/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2237 2024-01-26 22:59:56.094587 django-torque-0.5.7/PKG-INFO
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1624 2023-02-19 01:57:21.000000 django-torque-0.5.7/README.md
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-01-26 22:59:56.094587 django-torque-0.5.7/django_torque.egg-info/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2237 2024-01-26 22:59:56.000000 django-torque-0.5.7/django_torque.egg-info/PKG-INFO
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3068 2024-01-26 22:59:56.000000 django-torque-0.5.7/django_torque.egg-info/SOURCES.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        1 2024-01-26 22:59:56.000000 django-torque-0.5.7/django_torque.egg-info/dependency_links.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       68 2024-01-26 22:59:56.000000 django-torque-0.5.7/django_torque.egg-info/requires.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        7 2024-01-26 22:59:56.000000 django-torque-0.5.7/django_torque.egg-info/top_level.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       38 2024-01-26 22:59:56.094587 django-torque-0.5.7/setup.cfg
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1186 2023-08-28 15:18:57.000000 django-torque-0.5.7/setup.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-01-26 22:59:56.078587 django-torque-0.5.7/torque/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.5.7/torque/__init__.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       87 2023-02-19 01:57:21.000000 django-torque-0.5.7/torque/apps.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-01-26 22:59:56.078587 django-torque-0.5.7/torque/cache_rebuilder/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       72 2023-02-19 01:57:21.000000 django-torque-0.5.7/torque/cache_rebuilder/__init__.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      568 2023-10-30 13:59:37.000000 django-torque-0.5.7/torque/cache_rebuilder/apps.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     6729 2023-10-30 13:58:29.000000 django-torque-0.5.7/torque/cache_rebuilder/background.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-01-26 22:59:56.074587 django-torque-0.5.7/torque/management/
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-01-26 22:59:56.078587 django-torque-0.5.7/torque/management/commands/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.5.7/torque/management/commands/__init__.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1116 2023-02-19 01:57:21.000000 django-torque-0.5.7/torque/management/commands/remove_unattached.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      292 2023-10-30 14:00:33.000000 django-torque-0.5.7/torque/management/commands/run_cache_rebuilder.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-01-26 22:59:56.094587 django-torque-0.5.7/torque/migrations/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    12575 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0001_initial.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      436 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0002_auto_20210321_1604.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      450 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0003_auto_20210321_1725.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      728 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0005_auto_20210323_1303.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      572 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0006_auto_20210323_1623.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      838 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0007_auto_20210406_1738.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      372 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0008_auto_20210406_1909.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      402 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0009_sheetconfig_search_cache_dirty.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1359 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0010_tableofcontentscache.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      460 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0011_auto_20210416_1739.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      392 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0012_searchcacherow_dirty.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      397 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0013_spreadsheet_last_updated.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      403 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0014_tableofcontentscache_rendered_html.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      363 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0015_remove_tableofcontentscache_rendered_data.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2471 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0016_auto_20210721_1444.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      660 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0017_auto_20210721_1621.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      302 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0018_delete_permissiongroup.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      824 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0019_auto_20210721_1720.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      391 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0020_tableofcontents_raw.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      325 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0021_remove_column_type.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      635 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0022_auto_20210905_1430.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      836 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0023_auto_20210905_1454.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      766 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0024_auto_20210905_1535.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      790 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0025_auto_20210905_1624.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      892 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0026_auto_20210905_1638.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1332 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0027_auto_20210905_1642.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1327 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0028_auto_20210905_1659.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2537 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0029_auto_20210905_1716.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      579 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0030_auto_20210927_1304.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      706 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0031_auto_20210930_1328.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      398 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0032_searchcachedocument_filtered_data.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      876 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0033_csvspecification.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1642 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0034_auto_20220209_1209.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      390 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0035_template_in_config.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      802 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0036_remove_searchcachedocument_torque_search_data_ve_0ad953_gin_and_more.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      471 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0037_template_dirty.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      520 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0038_wiki_linked_wiki_keys.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      391 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0039_document_attached.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      455 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0040_value_unique_value_for_field_document.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      416 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0041_searchcachedocument_explore_rank.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1244 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0042_documentdictcache.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      460 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0043_documentdictcache_unique_document_dict.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      413 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0044_documentdictcache_dirty.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      668 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0045_templatecachedocument_dirty_and_more.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      324 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0046_delete_templatecachedocument.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1584 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0047_templatecachedocument_and_more.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      392 2023-09-02 17:46:03.000000 django-torque-0.5.7/torque/migrations/0048_rename_search_cache_dirty_wikiconfig_cache_dirty.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.5.7/torque/migrations/__init__.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    27643 2024-01-26 22:57:36.000000 django-torque-0.5.7/torque/models.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     5182 2024-01-26 22:57:36.000000 django-torque-0.5.7/torque/urls.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3145 2023-10-27 01:58:43.000000 django-torque-0.5.7/torque/utils.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       22 2024-01-26 22:04:49.000000 django-torque-0.5.7/torque/version.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    37505 2024-01-26 22:57:36.000000 django-torque-0.5.7/torque/views.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-04-27 17:49:01.082759 django_torque-0.6.0/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    34523 2024-04-27 17:48:43.000000 django_torque-0.6.0/LICENSE
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2825 2024-04-27 17:49:01.082759 django_torque-0.6.0/PKG-INFO
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2190 2024-04-26 20:01:53.000000 django_torque-0.6.0/README.md
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-04-27 17:49:01.082759 django_torque-0.6.0/django_torque.egg-info/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2825 2024-04-27 17:49:01.000000 django_torque-0.6.0/django_torque.egg-info/PKG-INFO
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3076 2024-04-27 17:49:01.000000 django_torque-0.6.0/django_torque.egg-info/SOURCES.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        1 2024-04-27 17:49:01.000000 django_torque-0.6.0/django_torque.egg-info/dependency_links.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       68 2024-04-27 17:49:01.000000 django_torque-0.6.0/django_torque.egg-info/requires.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        7 2024-04-27 17:49:01.000000 django_torque-0.6.0/django_torque.egg-info/top_level.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       38 2024-04-27 17:49:01.082759 django_torque-0.6.0/setup.cfg
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1186 2023-08-28 15:18:57.000000 django_torque-0.6.0/setup.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-04-27 17:49:01.066759 django_torque-0.6.0/torque/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django_torque-0.6.0/torque/__init__.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       87 2023-02-19 01:57:21.000000 django_torque-0.6.0/torque/apps.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-04-27 17:49:01.066759 django_torque-0.6.0/torque/cache_rebuilder/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       72 2023-02-19 01:57:21.000000 django_torque-0.6.0/torque/cache_rebuilder/__init__.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      594 2024-04-27 17:39:34.000000 django_torque-0.6.0/torque/cache_rebuilder/apps.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     6735 2024-02-16 00:56:38.000000 django_torque-0.6.0/torque/cache_rebuilder/background.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-04-27 17:49:01.062759 django_torque-0.6.0/torque/management/
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-04-27 17:49:01.066759 django_torque-0.6.0/torque/management/commands/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django_torque-0.6.0/torque/management/commands/__init__.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1116 2023-02-19 01:57:21.000000 django_torque-0.6.0/torque/management/commands/remove_unattached.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      293 2024-04-27 17:39:34.000000 django_torque-0.6.0/torque/management/commands/run_cache_rebuilder.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-04-27 17:49:01.078759 django_torque-0.6.0/torque/migrations/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    12575 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0001_initial.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      436 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0002_auto_20210321_1604.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      450 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0003_auto_20210321_1725.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      728 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0005_auto_20210323_1303.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      572 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0006_auto_20210323_1623.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      838 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0007_auto_20210406_1738.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      372 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0008_auto_20210406_1909.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      402 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0009_sheetconfig_search_cache_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1359 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0010_tableofcontentscache.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      460 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0011_auto_20210416_1739.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      392 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0012_searchcacherow_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      397 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0013_spreadsheet_last_updated.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      403 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0014_tableofcontentscache_rendered_html.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      363 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0015_remove_tableofcontentscache_rendered_data.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2471 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0016_auto_20210721_1444.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      660 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0017_auto_20210721_1621.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      302 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0018_delete_permissiongroup.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      824 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0019_auto_20210721_1720.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      391 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0020_tableofcontents_raw.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      325 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0021_remove_column_type.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      635 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0022_auto_20210905_1430.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      836 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0023_auto_20210905_1454.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      766 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0024_auto_20210905_1535.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      790 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0025_auto_20210905_1624.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      892 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0026_auto_20210905_1638.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1332 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0027_auto_20210905_1642.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1327 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0028_auto_20210905_1659.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2537 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0029_auto_20210905_1716.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      579 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0030_auto_20210927_1304.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      706 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0031_auto_20210930_1328.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      398 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0032_searchcachedocument_filtered_data.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      876 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0033_csvspecification.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1642 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0034_auto_20220209_1209.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      390 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0035_template_in_config.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      802 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0036_remove_searchcachedocument_torque_search_data_ve_0ad953_gin_and_more.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      471 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0037_template_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      520 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0038_wiki_linked_wiki_keys.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      391 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0039_document_attached.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      455 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0040_value_unique_value_for_field_document.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      416 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0041_searchcachedocument_explore_rank.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1244 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0042_documentdictcache.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      460 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0043_documentdictcache_unique_document_dict.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      413 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0044_documentdictcache_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      668 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0045_templatecachedocument_dirty_and_more.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      324 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0046_delete_templatecachedocument.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1584 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0047_templatecachedocument_and_more.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      392 2023-09-02 17:46:03.000000 django_torque-0.6.0/torque/migrations/0048_rename_search_cache_dirty_wikiconfig_cache_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django_torque-0.6.0/torque/migrations/__init__.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    27760 2024-04-27 17:39:35.000000 django_torque-0.6.0/torque/models.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     5539 2024-04-26 20:01:53.000000 django_torque-0.6.0/torque/urls.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3145 2023-10-27 01:58:43.000000 django_torque-0.6.0/torque/utils.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       22 2024-04-27 17:44:16.000000 django_torque-0.6.0/torque/version.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    40612 2024-04-27 17:39:35.000000 django_torque-0.6.0/torque/views.py
```

### Comparing `django-torque-0.5.7/PKG-INFO` & `django_torque-0.6.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: django-torque
-Version: 0.5.7
+Version: 0.6.0
 Summary: django app for torque
 Home-page: https://code.librehq.com/ots/mediawiki/torque
 Author: Open Tech Strategies, LLC
 Author-email: frankduncan@opentechstrategies.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: mwclient
 Requires-Dist: python-magic
 Requires-Dist: jinja2
 Requires-Dist: werkzeug
 Requires-Dist: django
 Requires-Dist: psycopg2-binary
 Requires-Dist: orjson
@@ -41,14 +42,25 @@
 from the database to ensure that no unintentional data loss occurs.  However, admins
 may want to remove that data to reflect the upgrades in the data.
 
 `remove_unattached` removes those items.  Each field/document that gets uploaded will
 be marked as `attached`.  If there are edits associated with a field or document, then
 the `--forced` argument is required.
 
+## run_cache_rebuilder
+
+`run_cache_rebuilder` starts up the cache rebuilder.  This is responsible for all
+the cache regeneration, and split off to a separate application in order to ensure
+that it doesn't affect the main process.  It IS required to run, though, as it
+does important database upkeep items as part of it's workflow.
+
+If you want to run it as part of the application instead of separately, add
+`"torque.cache_rebuilder",` as an `INSTALLED_APP` in your settings file, as
+is exampled in [test_settings.py](test_settings.py) and [INSTALL.md](INSTALL.md)
+
 ## Removing attachment files
 
 As a system runs, old FileField files can hang around on the hard drive.  Those
 are usually uploaded attachments and templates.  This can start to take up
 too much space.  To remove, one was is to use
 [https://github.com/akolpakov/django-unused-media](django-unused-media):
```

### Comparing `django-torque-0.5.7/django_torque.egg-info/PKG-INFO` & `django_torque-0.6.0/django_torque.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: django-torque
-Version: 0.5.7
+Version: 0.6.0
 Summary: django app for torque
 Home-page: https://code.librehq.com/ots/mediawiki/torque
 Author: Open Tech Strategies, LLC
 Author-email: frankduncan@opentechstrategies.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: mwclient
 Requires-Dist: python-magic
 Requires-Dist: jinja2
 Requires-Dist: werkzeug
 Requires-Dist: django
 Requires-Dist: psycopg2-binary
 Requires-Dist: orjson
@@ -41,14 +42,25 @@
 from the database to ensure that no unintentional data loss occurs.  However, admins
 may want to remove that data to reflect the upgrades in the data.
 
 `remove_unattached` removes those items.  Each field/document that gets uploaded will
 be marked as `attached`.  If there are edits associated with a field or document, then
 the `--forced` argument is required.
 
+## run_cache_rebuilder
+
+`run_cache_rebuilder` starts up the cache rebuilder.  This is responsible for all
+the cache regeneration, and split off to a separate application in order to ensure
+that it doesn't affect the main process.  It IS required to run, though, as it
+does important database upkeep items as part of it's workflow.
+
+If you want to run it as part of the application instead of separately, add
+`"torque.cache_rebuilder",` as an `INSTALLED_APP` in your settings file, as
+is exampled in [test_settings.py](test_settings.py) and [INSTALL.md](INSTALL.md)
+
 ## Removing attachment files
 
 As a system runs, old FileField files can hang around on the hard drive.  Those
 are usually uploaded attachments and templates.  This can start to take up
 too much space.  To remove, one was is to use
 [https://github.com/akolpakov/django-unused-media](django-unused-media):
```

### Comparing `django-torque-0.5.7/django_torque.egg-info/SOURCES.txt` & `django_torque-0.6.0/django_torque.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 ./torque/__init__.py
 ./torque/apps.py
 ./torque/models.py
 ./torque/urls.py
 ./torque/utils.py
```

### Comparing `django-torque-0.5.7/setup.py` & `django_torque-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/cache_rebuilder/apps.py` & `django_torque-0.6.0/torque/cache_rebuilder/apps.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,12 +5,14 @@
 
 
 class CacheRebuilderConfig(AppConfig):
     name = "torque.cache_rebuilder"
 
     def ready(self):
         # This check makes sure that this only boots once
-        if os.environ.get("RUN_MAIN", None) != "true" and not os.environ.get(
-            "DISABLE_CACHE_REBUILDER", False
-        ) and not getattr(settings, "DISABLE_CACHE_REBUILDER", False):
+        if (
+            os.environ.get("RUN_MAIN", None) != "true"
+            and not os.environ.get("DISABLE_CACHE_REBUILDER", False)
+            and not getattr(settings, "DISABLE_CACHE_REBUILDER", False)
+        ):
             cache_rebuilder = background.CacheRebuilder()
             cache_rebuilder.start()
```

### Comparing `django-torque-0.5.7/torque/cache_rebuilder/background.py` & `django_torque-0.6.0/torque/cache_rebuilder/background.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         num = models.SearchCacheDocument.objects.filter(dirty=True).count()
         if num > 0:
             print("Rebuilding %s search cache documents" % num)
 
         for cache_document in models.SearchCacheDocument.objects.filter(dirty=True):
             collection = cache_document.document.collection
             for config in collection.configs.all():
-                document_dict = cache_document.document.to_dict(config)
+                document_dict = cache_document.document.to_dict(config, None)
                 cache_document.data = " ".join(list(map(str, document_dict.values())))
                 cache_document.dirty = False
                 cache_document.save()
                 models.SearchCacheDocument.objects.filter(id=cache_document.id).update(
                     data_vector=SearchVector("data")
                 )
```

### Comparing `django-torque-0.5.7/torque/management/commands/remove_unattached.py` & `django_torque-0.6.0/torque/management/commands/remove_unattached.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0001_initial.py` & `django_torque-0.6.0/torque/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0005_auto_20210323_1303.py` & `django_torque-0.6.0/torque/migrations/0005_auto_20210323_1303.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0006_auto_20210323_1623.py` & `django_torque-0.6.0/torque/migrations/0006_auto_20210323_1623.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0007_auto_20210406_1738.py` & `django_torque-0.6.0/torque/migrations/0007_auto_20210406_1738.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0010_tableofcontentscache.py` & `django_torque-0.6.0/torque/migrations/0010_tableofcontentscache.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0016_auto_20210721_1444.py` & `django_torque-0.6.0/torque/migrations/0016_auto_20210721_1444.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0017_auto_20210721_1621.py` & `django_torque-0.6.0/torque/migrations/0017_auto_20210721_1621.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0019_auto_20210721_1720.py` & `django_torque-0.6.0/torque/migrations/0019_auto_20210721_1720.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0022_auto_20210905_1430.py` & `django_torque-0.6.0/torque/migrations/0022_auto_20210905_1430.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0023_auto_20210905_1454.py` & `django_torque-0.6.0/torque/migrations/0023_auto_20210905_1454.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0024_auto_20210905_1535.py` & `django_torque-0.6.0/torque/migrations/0024_auto_20210905_1535.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0025_auto_20210905_1624.py` & `django_torque-0.6.0/torque/migrations/0025_auto_20210905_1624.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0026_auto_20210905_1638.py` & `django_torque-0.6.0/torque/migrations/0026_auto_20210905_1638.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0027_auto_20210905_1642.py` & `django_torque-0.6.0/torque/migrations/0027_auto_20210905_1642.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0028_auto_20210905_1659.py` & `django_torque-0.6.0/torque/migrations/0028_auto_20210905_1659.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0029_auto_20210905_1716.py` & `django_torque-0.6.0/torque/migrations/0029_auto_20210905_1716.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0030_auto_20210927_1304.py` & `django_torque-0.6.0/torque/migrations/0030_auto_20210927_1304.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0031_auto_20210930_1328.py` & `django_torque-0.6.0/torque/migrations/0031_auto_20210930_1328.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0033_csvspecification.py` & `django_torque-0.6.0/torque/migrations/0033_csvspecification.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0034_auto_20220209_1209.py` & `django_torque-0.6.0/torque/migrations/0034_auto_20220209_1209.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0036_remove_searchcachedocument_torque_search_data_ve_0ad953_gin_and_more.py` & `django_torque-0.6.0/torque/migrations/0036_remove_searchcachedocument_torque_search_data_ve_0ad953_gin_and_more.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0038_wiki_linked_wiki_keys.py` & `django_torque-0.6.0/torque/migrations/0038_wiki_linked_wiki_keys.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0042_documentdictcache.py` & `django_torque-0.6.0/torque/migrations/0042_documentdictcache.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0045_templatecachedocument_dirty_and_more.py` & `django_torque-0.6.0/torque/migrations/0045_templatecachedocument_dirty_and_more.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/migrations/0047_templatecachedocument_and_more.py` & `django_torque-0.6.0/torque/migrations/0047_templatecachedocument_and_more.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/models.py` & `django_torque-0.6.0/torque/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,17 +187,17 @@
             .prefetch_related("field")
             .prefetch_related("document")
             .values("document_id", "document__key", "field__name", "latest")
         )
         new_documents = {}
         for value in values:
             try:
-                new_documents[value["document_id"]]["fields"][
-                    value["field__name"]
-                ] = orjson.loads(value["latest"])
+                new_documents[value["document_id"]]["fields"][value["field__name"]] = (
+                    orjson.loads(value["latest"])
+                )
             except KeyError:
                 new_documents[value["document_id"]] = {
                     "key": value["document__key"],
                     "fields": {value["field__name"]: orjson.loads(value["latest"])},
                 }
 
         document_dicts = []
@@ -295,34 +295,40 @@
     # When uploading a collection, if documents have been dropped off, then they are
     # no longer actively attached.  Instead of just removing them right away, and
     # losing any Value or ValueEdits associated, we just mark them as unattached,
     # and then we can later clean them up if we want.
     attached = models.BooleanField(default=True)
 
     def to_dict(self, config, version):
+        fields = None
+        if config:
+            fields = config.valid_fields.all()
+        else:
+            fields = self.collection.fields.all()
+
         if not version or version == "latest":
             try:
                 return orjson.loads(
                     DocumentDictCache.objects.get(
                         document=self, wiki_config=config
                     ).dictionary
                 )
             except DocumentDictCache.DoesNotExist:
                 new_document = {"key": self.key, "fields": {}}
-                for value in self.values.filter(field__in=config.valid_fields.all()).values(
+                for value in self.values.filter(field__in=fields).values(
                     "field__name", "latest"
                 ):
                     new_document["fields"][value["field__name"]] = orjson.loads(
                         value["latest"]
                     )
 
                 return new_document
         elif version == "original":
             new_document = {"key": self.key, "fields": {}}
-            for value in self.values.filter(field__in=config.valid_fields.all()).values(
+            for value in self.values.filter(field__in=fields).values(
                 "field__name", "original"
             ):
                 new_document["fields"][value["field__name"]] = orjson.loads(
                     value["original"]
                 )
 
             return new_document
```

### Comparing `django-torque-0.5.7/torque/urls.py` & `django_torque-0.6.0/torque/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,18 @@
         views.get_document_view,
     ),
     path(
         "api/collections/<collection_name>/documents/<key>/version/<version>.<fmt>",
         views.get_document_view,
     ),
     path(
+        "api/collections/<collection_name>/documents/<key>/attachments.<fmt>",
+        views.get_attachments,
+    ),
+    path(
         "api/collections/<collection_name>/documents/<key>/attachments/<attachment>",
         views.get_attachment,
     ),
     path(
         "api/collections/<collection_name>/documents/<key>/fields/<field>.<fmt>",
         views.field,
     ),
@@ -78,14 +82,19 @@
             ),
             path(
                 "api/%s/<collection_name>/%s/<key>/version/<version>.<fmt>"
                 % (settings.TORQUE_COLLECTIONS_ALIAS, settings.TORQUE_DOCUMENTS_ALIAS),
                 views.get_document_view,
             ),
             path(
+                "api/%s/<collection_name>/%s/<key>/attachments.<fmt>"
+                % (settings.TORQUE_COLLECTIONS_ALIAS, settings.TORQUE_DOCUMENTS_ALIAS),
+                views.get_attachments,
+            ),
+            path(
                 "api/%s/<collection_name>/%s/<key>/attachments/<attachment>"
                 % (settings.TORQUE_COLLECTIONS_ALIAS, settings.TORQUE_DOCUMENTS_ALIAS),
                 views.get_attachment,
             ),
             path(
                 "api/%s/<collection_name>/%s/<key>/fields/<field>.<fmt>"
                 % (settings.TORQUE_COLLECTIONS_ALIAS, settings.TORQUE_DOCUMENTS_ALIAS),
```

### Comparing `django-torque-0.5.7/torque/utils.py` & `django_torque-0.6.0/torque/utils.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.7/torque/views.py` & `django_torque-0.6.0/torque/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -135,14 +135,18 @@
                     value = selected_object[filter.name()]
                     if value not in filter.ignored_values():
                         if value not in counts:
                             counts[value] = {"name": value, "total": 0}
 
                         counts[value]["total"] += 1
 
+        for value in filters.get(filter.name(), []):
+            if value not in counts:
+                counts[value] = {"name": value, "total": 0}
+
         filter_result = {
             "name": filter.name(),
             "display": filter.display_name(),
             "counts": {name: counts[name] for name in filter.sort(list(counts.keys()))},
         }
 
         filter_results.append(filter_result)
@@ -188,15 +192,17 @@
     # But, if we decide we need results to go to another renderer, it may
     # be worth being more clear about what we're doing here via the interface.
     #
     # This has gotten weird because the results are actually html from cached
     # results
     if fmt == "mwiki":
         template = models.Template.objects.get(
-            type="Search", collection=template_config.collection, wiki=template_config.wiki,
+            type="Search",
+            collection=template_config.collection,
+            wiki=template_config.wiki,
         )
 
         cache_or = Q()
         for r in returned_results[offset : (offset + 20)]:
             cache_or |= Q(
                 document_dict__wiki_config=r.wiki_config,
                 document_dict__document=r.document,
@@ -302,19 +308,23 @@
         "filter_results": filter_results,
     }
 
     if not filters_only:
         mwiki_text = ""
 
         result_set = [
-            orjson.loads(
-                models.DocumentDictCache.objects.get(
-                    document=r.document, wiki_config__group=r.group
-                ).dictionary
-            )["fields"]
+            {
+                "collection_name": r.collection.name,
+                "document_key": r.document.key,
+                "fields": orjson.loads(
+                    models.DocumentDictCache.objects.get(
+                        document=r.document, wiki_config__group=r.group
+                    ).dictionary
+                )["fields"],
+            }
             for r in returned_results[offset : (offset + 100)]
         ]
         explore_templates = models.Template.objects.filter(
             type="Explore",
             collection=template_config.collection,
         )
         if explore_templates:
@@ -323,26 +333,38 @@
                     explore_templates.get(name=template_name).get_file_contents()
                 )
             else:
                 template = jinja_env.from_string(
                     explore_templates.get(is_default=True).get_file_contents()
                 )
             mwiki_text += template.render(
-                {template_config.collection.object_data_name(): result_set}
+                {
+                    template_config.collection.object_data_name(): [
+                        r["fields"] for r in result_set
+                    ]
+                }
             )
         else:
             for result in result_set:
                 template = jinja_env.from_string(
                     models.Template.objects.get(
                         name="Search", collection=template_config.collection
                     ).get_file_contents()
                 )
+                mwiki_text += (
+                    "<div class='result'><div class='result--actions'><div class='result--select--holder' data-collection='%s' data-document='%s'></div></div>"
+                    % (
+                        result["collection_name"],
+                        result["document_key"],
+                    )
+                )
                 mwiki_text += template.render(
-                    {template_config.collection.object_name: result}
+                    {template_config.collection.object_name: result["fields"]}
                 )
+                mwiki_text += "</div>"
                 mwiki_text += "\n\n"
 
         response["results"] = [
             (r["collection__name"], r["document__key"])
             for r in returned_results.values("collection__name", "document__key")
         ]
         response["mwiki_text"] = mwiki_text
@@ -507,15 +529,15 @@
                 wiki=wiki,
                 group=group,
             )
 
             response["fields"] = [
                 field.name for field in wiki_config.valid_fields.all()
             ]
-        else:
+        elif "admin" in request.GET:
             response["fields"] = [field.name for field in collection.fields.all()]
 
         response["last_updated"] = collection.last_updated.isoformat()
 
         return JsonResponse(response)
     else:
         raise Exception(f"Invalid format {fmt}")
@@ -556,42 +578,55 @@
             return HttpResponse()
     else:
         raise Exception(f"Invalid format {fmt}")
 
 
 def get_documents(request, collection_name, fmt):
     collection = models.Collection.objects.get(name=collection_name)
-    group = request.GET["group"]
+    group = request.GET.get("group")
+    admin = request.GET.get("admin")
     wiki = get_wiki_from_request(request, collection_name)
 
-    wiki_config = models.WikiConfig.objects.get(
-        collection=collection,
-        wiki=wiki,
-        group=group,
-    )
-
     if fmt == "json":
-        return JsonResponse(
-            [document.key for document in wiki_config.valid_ids.all()], safe=False
-        )
+        if group:
+            wiki_config = models.WikiConfig.objects.get(
+                collection=collection,
+                wiki=wiki,
+                group=group,
+            )
+            return JsonResponse(
+                [document.key for document in wiki_config.valid_ids.all()], safe=False
+            )
+        elif admin:
+            return JsonResponse(
+                [document.key for document in collection.documents.all()], safe=False
+            )
     else:
         raise Exception(f"Invalid format {fmt}")
 
 
-def get_document(group, wiki, key, version, fmt, collection_name, view=None):
+def get_document(group, admin, wiki, key, version, fmt, collection_name, view=None):
     collection = models.Collection.objects.get(name=collection_name)
-    wiki_config = models.WikiConfig.objects.get(
-        collection=collection,
-        wiki=wiki,
-        group=group,
-    )
 
-    document = wiki_config.valid_ids.get(key=key, collection=collection).to_dict(
-        wiki_config, version
-    )["fields"]
+    wiki_config = None
+    if group or not admin:
+        wiki_config = models.WikiConfig.objects.get(
+            collection=collection,
+            wiki=wiki,
+            group=group,
+        )
+
+        document = wiki_config.valid_ids.get(key=key, collection=collection).to_dict(
+            wiki_config, version
+        )["fields"]
+    # We only allow admin style access to documents when using them from a data/api
+    # point of view, just to be extra sure that normal wiki viewership remains group
+    # based from both a permissions point of view, but also from a cache one
+    elif admin and fmt in ["json", "dict"]:
+        document = collection.documents.get(key=key).to_dict(None, version)["fields"]
 
     if fmt == "json":
         return JsonResponse(document)
     elif fmt == "dict":
         return document
 
     templates = models.Template.objects.filter(
@@ -634,28 +669,39 @@
         except models.TemplateCacheDocument.DoesNotExist:
             return HttpResponse("")
     else:
         raise Exception(f"Invalid format {fmt}")
 
 
 def get_document_view(request, collection_name, key, fmt, version="latest"):
-    group = request.GET["group"]
+    group = request.GET.get("group")
+    admin = request.GET.get("admin")
     wiki = get_wiki_from_request(request, collection_name)
 
     return get_document(
-        group, wiki, key, version, fmt, collection_name, request.GET.get("view", None)
+        group,
+        admin,
+        wiki,
+        key,
+        version,
+        fmt,
+        collection_name,
+        request.GET.get("view", None),
     )
 
 
 def field(request, collection_name, key, field, fmt):
     field = urllib.parse.unquote_plus(field)
     if request.method == "GET":
-        group = request.GET["group"]
+        group = request.GET.get("group")
+        admin = request.GET.get("admin")
         wiki = get_wiki_from_request(request, collection_name)
-        document = get_document(group, wiki, key, None, "dict", collection_name, None)
+        document = get_document(
+            group, admin, wiki, key, None, "dict", collection_name, None
+        )
 
         value = document
         for level in field.split("||"):
             if isinstance(value, list):
                 level = int(level)
 
             value = value[level]
@@ -666,30 +712,74 @@
         group = post_fields["group"]
         wiki = get_wiki(post_fields, collection_name)
         new_value = post_fields["new_value"]
         edit_record(collection_name, key, group, wiki, field, new_value)
         return HttpResponse(201)
 
 
+def get_attachments(request, collection_name, key, fmt):
+    group = request.GET.get("group")
+    admin = request.GET.get("admin")
+    wiki = get_wiki_from_request(request, collection_name)
+
+    attachments = []
+    collection = models.Collection.objects.get(name=collection_name)
+    document = collection.documents.get(key=key)
+
+    if group:
+        wiki_config = models.WikiConfig.objects.get(
+            collection=collection,
+            wiki=wiki,
+            group=group,
+        )
+        attachments = []
+
+        for potential_attachment in models.Attachment.objects.filter(document=document):
+            if wiki_config.valid_fields.filter(
+                id=potential_attachment.permissions_field.id
+            ).exists():
+                attachments.append(potential_attachment)
+    elif admin:
+        attachments = models.Attachment.objects.filter(document=document)
+
+    if fmt == "json":
+        return JsonResponse(
+            [
+                {
+                    "name": a.name,
+                    "size": a.file.size,
+                }
+                for a in attachments
+            ],
+            safe=False,
+        )
+    else:
+        raise Exception(f"Invalid format {fmt}")
+
+
 def get_attachment(request, collection_name, key, attachment):
-    group = request.GET["group"]
+    group = request.GET.get("group")
+    admin = request.GET.get("admin")
     wiki = get_wiki_from_request(request, collection_name)
     attachment_name = secure_filename(urllib.parse.unquote_plus(attachment))
 
     collection = models.Collection.objects.get(name=collection_name)
-    wiki_config = models.WikiConfig.objects.get(
-        collection=collection,
-        wiki=wiki,
-        group=group,
-    )
     document = collection.documents.get(key=key)
     attachment = models.Attachment.objects.get(name=attachment_name, document=document)
 
-    if not wiki_config.valid_fields.filter(id=attachment.permissions_field.id).exists():
-        raise Exception("Not permitted to see this attachment.")
+    if group or not admin:
+        wiki_config = models.WikiConfig.objects.get(
+            collection=collection,
+            wiki=wiki,
+            group=group,
+        )
+        if not wiki_config.valid_fields.filter(
+            id=attachment.permissions_field.id
+        ).exists():
+            raise Exception("Not permitted to see this attachment.")
 
     content_type = magic.from_buffer(attachment.file.open("rb").read(1024), mime=True)
     return FileResponse(
         attachment.file.open("rb"), filename=attachment_name, content_type=content_type
     )
```

