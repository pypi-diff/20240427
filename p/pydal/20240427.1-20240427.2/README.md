# Comparing `tmp/pydal-20240427.1.tar.gz` & `tmp/pydal-20240427.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydal-20240427.1.tar", last modified: Sat Apr 27 07:06:54 2024, max compression
+gzip compressed data, was "pydal-20240427.2.tar", last modified: Sat Apr 27 07:19:15 2024, max compression
```

## Comparing `pydal-20240427.1.tar` & `pydal-20240427.2.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:06:54.095218 pydal-20240427.1/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      344 2022-10-17 00:44:46.000000 pydal-20240427.1/AUTHORS
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6546 2022-10-17 00:44:46.000000 pydal-20240427.1/CHANGES
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1555 2022-10-17 00:44:46.000000 pydal-20240427.1/LICENSE.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      170 2022-11-11 06:37:56.000000 pydal-20240427.1/MANIFEST.in
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2903 2024-04-27 07:06:54.095218 pydal-20240427.1/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2034 2022-10-17 00:44:46.000000 pydal-20240427.1/README.md
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:06:54.061884 pydal-20240427.1/docs/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6758 2022-10-17 00:44:46.000000 pydal-20240427.1/docs/Makefile
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8083 2023-05-07 23:00:04.000000 pydal-20240427.1/docs/conf.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      833 2022-10-17 00:44:46.000000 pydal-20240427.1/docs/index.rst
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2834 2022-10-17 00:44:46.000000 pydal-20240427.1/docs/pydal.adapters.rst
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      664 2022-10-17 00:44:46.000000 pydal-20240427.1/docs/pydal.helpers.rst
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       29 2022-10-17 00:44:46.000000 pydal-20240427.1/docs/requirements.txt
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:06:54.065217 pydal-20240427.1/pydal/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      179 2024-04-27 07:02:56.000000 pydal-20240427.1/pydal/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5440 2023-11-15 07:07:33.000000 pydal-20240427.1/pydal/_compat.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      466 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/_gae.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      208 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/_globals.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      396 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/_load.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:06:54.071884 pydal-20240427.1/pydal/adapters/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2372 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/adapters/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    38911 2023-11-15 07:07:34.000000 pydal-20240427.1/pydal/adapters/base.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5691 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/adapters/couchdb.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2000 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/adapters/db2.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3145 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/adapters/firebird.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18365 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/adapters/google.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2076 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/adapters/informix.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1882 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/adapters/ingres.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    37772 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/adapters/mongo.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6161 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/adapters/mssql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3412 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/adapters/mysql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9172 2023-11-12 03:29:21.000000 pydal-20240427.1/pydal/adapters/oracle.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9327 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/adapters/postgres.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1460 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/adapters/sap.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4894 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/adapters/snowflake.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4392 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/adapters/sqlite.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      799 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/adapters/teradata.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    38529 2023-12-28 08:14:12.000000 pydal-20240427.1/pydal/base.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6427 2023-05-07 22:57:59.000000 pydal-20240427.1/pydal/connection.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:06:54.071884 pydal-20240427.1/pydal/contrib/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/contrib/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    44546 2023-11-15 07:07:34.000000 pydal-20240427.1/pydal/contrib/imap_adapter.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    79360 2023-11-15 07:07:34.000000 pydal-20240427.1/pydal/contrib/ipaddress.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    10686 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/contrib/mockimaplib.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4071 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/contrib/ordereddict.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5584 2023-05-07 22:58:06.000000 pydal-20240427.1/pydal/contrib/portalocker.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    33372 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/contrib/reserved_sql_keywords.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3532 2023-05-07 22:58:07.000000 pydal-20240427.1/pydal/default_validators.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:06:54.075218 pydal-20240427.1/pydal/dialects/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3803 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/dialects/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    23464 2023-05-07 22:58:13.000000 pydal-20240427.1/pydal/dialects/base.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1390 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/dialects/couchdb.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3374 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/dialects/db2.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4307 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/dialects/firebird.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5953 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/dialects/google.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3275 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/dialects/informix.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3929 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/dialects/ingres.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    22110 2023-05-07 22:58:11.000000 pydal-20240427.1/pydal/dialects/mongo.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    15763 2023-11-15 07:07:34.000000 pydal-20240427.1/pydal/dialects/mssql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3413 2023-05-07 22:51:50.000000 pydal-20240427.1/pydal/dialects/mysql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8928 2023-05-07 22:58:13.000000 pydal-20240427.1/pydal/dialects/oracle.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    14406 2023-11-12 03:31:51.000000 pydal-20240427.1/pydal/dialects/postgre.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3001 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/dialects/sap.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    12077 2023-05-07 22:58:18.000000 pydal-20240427.1/pydal/dialects/snowflake.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4295 2023-05-07 22:52:12.000000 pydal-20240427.1/pydal/dialects/sqlite.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3400 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/dialects/teradata.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3180 2023-11-15 07:07:34.000000 pydal-20240427.1/pydal/drivers.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      347 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/exceptions.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:06:54.078551 pydal-20240427.1/pydal/helpers/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/helpers/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      652 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/helpers/_internals.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    16544 2023-11-15 07:07:34.000000 pydal-20240427.1/pydal/helpers/classes.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      971 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/helpers/gae.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    14816 2023-11-15 07:07:34.000000 pydal-20240427.1/pydal/helpers/methods.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1144 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/helpers/regex.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    16447 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/helpers/rest.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1839 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/helpers/serializers.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    27287 2023-05-07 22:58:25.000000 pydal-20240427.1/pydal/migrator.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   128654 2024-04-27 07:02:34.000000 pydal-20240427.1/pydal/objects.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:06:54.081884 pydal-20240427.1/pydal/parsers/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3394 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/parsers/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4718 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/parsers/base.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      360 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/parsers/google.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1605 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/parsers/mongo.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1654 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/parsers/oracle.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      815 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/parsers/postgre.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1043 2023-11-15 07:07:34.000000 pydal-20240427.1/pydal/parsers/sqlite.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:06:54.081884 pydal-20240427.1/pydal/representers/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8806 2023-11-15 07:07:35.000000 pydal-20240427.1/pydal/representers/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8793 2023-11-15 07:07:35.000000 pydal-20240427.1/pydal/representers/base.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1210 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/representers/couchdb.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      680 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/representers/db2.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1446 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/representers/google.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      884 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/representers/informix.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1757 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/representers/mongo.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      948 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/representers/mssql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      214 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/representers/mysql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1286 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/representers/oracle.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1643 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/representers/postgre.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      752 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/representers/sqlite.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    22855 2023-11-15 07:07:35.000000 pydal-20240427.1/pydal/restapi.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:06:54.085218 pydal-20240427.1/pydal/tools/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/tools/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2120 2023-11-15 06:54:34.000000 pydal-20240427.1/pydal/tools/tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1904 2022-10-17 00:44:46.000000 pydal-20240427.1/pydal/utils.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   158790 2023-11-19 17:50:44.000000 pydal-20240427.1/pydal/validators.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:06:54.065217 pydal-20240427.1/pydal.egg-info/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2903 2024-04-27 07:06:53.000000 pydal-20240427.1/pydal.egg-info/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3314 2024-04-27 07:06:54.000000 pydal-20240427.1/pydal.egg-info/SOURCES.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-04-27 07:06:53.000000 pydal-20240427.1/pydal.egg-info/dependency_links.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        6 2024-04-27 07:06:53.000000 pydal-20240427.1/pydal.egg-info/top_level.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      905 2024-04-27 07:02:34.000000 pydal-20240427.1/pyproject.toml
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       99 2024-04-27 07:06:54.095218 pydal-20240427.1/setup.cfg
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:06:54.088551 pydal-20240427.1/tests/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      355 2023-05-07 23:00:04.000000 pydal-20240427.1/tests/__init__.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:06:54.091884 pydal-20240427.1/tests/__pycache__/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      625 2024-04-27 07:03:00.000000 pydal-20240427.1/tests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1648 2023-12-28 08:14:31.000000 pydal-20240427.1/tests/__pycache__/_adapt.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      299 2023-12-28 08:14:32.000000 pydal-20240427.1/tests/__pycache__/_compat.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1997 2023-12-28 08:14:32.000000 pydal-20240427.1/tests/__pycache__/_helpers.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    17046 2023-12-28 08:14:32.000000 pydal-20240427.1/tests/__pycache__/base.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6517 2023-12-28 08:14:32.000000 pydal-20240427.1/tests/__pycache__/caching.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    12212 2023-12-28 08:14:32.000000 pydal-20240427.1/tests/__pycache__/contribs.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5665 2023-12-28 08:14:32.000000 pydal-20240427.1/tests/__pycache__/indexes.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    38716 2023-12-28 08:14:32.000000 pydal-20240427.1/tests/__pycache__/is_url_validators.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    10845 2023-12-28 08:14:32.000000 pydal-20240427.1/tests/__pycache__/restapi.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7654 2023-12-28 08:14:32.000000 pydal-20240427.1/tests/__pycache__/smart_query.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   283900 2023-12-28 08:14:31.000000 pydal-20240427.1/tests/__pycache__/sql.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2554 2023-12-28 08:14:32.000000 pydal-20240427.1/tests/__pycache__/tags.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6751 2023-12-28 08:14:32.000000 pydal-20240427.1/tests/__pycache__/validation.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   100862 2023-12-28 08:14:32.000000 pydal-20240427.1/tests/__pycache__/validators.cpython-311.pyc
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      954 2022-10-17 00:44:46.000000 pydal-20240427.1/tests/_adapt.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       95 2022-10-17 00:44:46.000000 pydal-20240427.1/tests/_compat.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      765 2023-05-07 23:00:04.000000 pydal-20240427.1/tests/_helpers.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8103 2023-11-15 07:07:11.000000 pydal-20240427.1/tests/base.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2554 2023-05-07 23:00:03.000000 pydal-20240427.1/tests/caching.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4954 2023-11-15 07:07:11.000000 pydal-20240427.1/tests/contribs.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2279 2023-05-07 23:00:03.000000 pydal-20240427.1/tests/indexes.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    29359 2023-11-15 07:07:11.000000 pydal-20240427.1/tests/is_url_validators.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    99826 2023-11-15 07:07:14.000000 pydal-20240427.1/tests/nosql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    14072 2023-11-15 07:07:11.000000 pydal-20240427.1/tests/restapi.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    12552 2023-05-07 23:00:04.000000 pydal-20240427.1/tests/smart_query.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   137750 2023-11-15 07:07:15.000000 pydal-20240427.1/tests/sql.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      990 2023-05-07 23:00:04.000000 pydal-20240427.1/tests/tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3604 2023-11-15 06:55:22.000000 pydal-20240427.1/tests/validation.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    66909 2023-11-15 07:07:13.000000 pydal-20240427.1/tests/validators.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.949208 pydal-20240427.2/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      344 2022-10-17 00:44:46.000000 pydal-20240427.2/AUTHORS
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6546 2022-10-17 00:44:46.000000 pydal-20240427.2/CHANGES
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1555 2022-10-17 00:44:46.000000 pydal-20240427.2/LICENSE.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      170 2022-11-11 06:37:56.000000 pydal-20240427.2/MANIFEST.in
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2903 2024-04-27 07:19:15.949208 pydal-20240427.2/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2034 2022-10-17 00:44:46.000000 pydal-20240427.2/README.md
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.915874 pydal-20240427.2/docs/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6758 2022-10-17 00:44:46.000000 pydal-20240427.2/docs/Makefile
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8083 2023-05-07 23:00:04.000000 pydal-20240427.2/docs/conf.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      833 2022-10-17 00:44:46.000000 pydal-20240427.2/docs/index.rst
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2834 2022-10-17 00:44:46.000000 pydal-20240427.2/docs/pydal.adapters.rst
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      664 2022-10-17 00:44:46.000000 pydal-20240427.2/docs/pydal.helpers.rst
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       29 2022-10-17 00:44:46.000000 pydal-20240427.2/docs/requirements.txt
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.922541 pydal-20240427.2/pydal/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      179 2024-04-27 07:19:02.000000 pydal-20240427.2/pydal/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5440 2023-11-15 07:07:33.000000 pydal-20240427.2/pydal/_compat.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      466 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/_gae.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      208 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/_globals.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      396 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/_load.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.925874 pydal-20240427.2/pydal/adapters/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2372 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    38911 2023-11-15 07:07:34.000000 pydal-20240427.2/pydal/adapters/base.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5691 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/couchdb.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2000 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/db2.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3145 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/firebird.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18365 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2076 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/informix.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1882 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/ingres.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    37772 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/mongo.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6161 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/mssql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3412 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/mysql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9172 2023-11-12 03:29:21.000000 pydal-20240427.2/pydal/adapters/oracle.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9327 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/postgres.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1460 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/sap.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4894 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/snowflake.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4392 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/sqlite.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      799 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/adapters/teradata.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    38529 2023-12-28 08:14:12.000000 pydal-20240427.2/pydal/base.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6427 2023-05-07 22:57:59.000000 pydal-20240427.2/pydal/connection.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.929208 pydal-20240427.2/pydal/contrib/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/contrib/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    44546 2023-11-15 07:07:34.000000 pydal-20240427.2/pydal/contrib/imap_adapter.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    79360 2023-11-15 07:07:34.000000 pydal-20240427.2/pydal/contrib/ipaddress.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    10686 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/contrib/mockimaplib.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4071 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/contrib/ordereddict.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5584 2023-05-07 22:58:06.000000 pydal-20240427.2/pydal/contrib/portalocker.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    33372 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/contrib/reserved_sql_keywords.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3532 2023-05-07 22:58:07.000000 pydal-20240427.2/pydal/default_validators.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.932541 pydal-20240427.2/pydal/dialects/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3803 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/dialects/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    23464 2023-05-07 22:58:13.000000 pydal-20240427.2/pydal/dialects/base.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1390 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/dialects/couchdb.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3374 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/dialects/db2.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4307 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/dialects/firebird.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5953 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/dialects/google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3275 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/dialects/informix.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3929 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/dialects/ingres.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    22110 2023-05-07 22:58:11.000000 pydal-20240427.2/pydal/dialects/mongo.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    15763 2023-11-15 07:07:34.000000 pydal-20240427.2/pydal/dialects/mssql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3413 2023-05-07 22:51:50.000000 pydal-20240427.2/pydal/dialects/mysql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8928 2023-05-07 22:58:13.000000 pydal-20240427.2/pydal/dialects/oracle.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    14406 2023-11-12 03:31:51.000000 pydal-20240427.2/pydal/dialects/postgre.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3001 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/dialects/sap.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    12077 2023-05-07 22:58:18.000000 pydal-20240427.2/pydal/dialects/snowflake.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4295 2023-05-07 22:52:12.000000 pydal-20240427.2/pydal/dialects/sqlite.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3400 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/dialects/teradata.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3180 2023-11-15 07:07:34.000000 pydal-20240427.2/pydal/drivers.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      347 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/exceptions.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.935875 pydal-20240427.2/pydal/helpers/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/helpers/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      652 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/helpers/_internals.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    16544 2023-11-15 07:07:34.000000 pydal-20240427.2/pydal/helpers/classes.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      971 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/helpers/gae.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    14816 2023-11-15 07:07:34.000000 pydal-20240427.2/pydal/helpers/methods.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1144 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/helpers/regex.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    16447 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/helpers/rest.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1839 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/helpers/serializers.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    27287 2023-05-07 22:58:25.000000 pydal-20240427.2/pydal/migrator.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   128832 2024-04-27 07:18:46.000000 pydal-20240427.2/pydal/objects.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.935875 pydal-20240427.2/pydal/parsers/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3394 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/parsers/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4718 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/parsers/base.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      360 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/parsers/google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1605 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/parsers/mongo.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1654 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/parsers/oracle.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      815 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/parsers/postgre.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1043 2023-11-15 07:07:34.000000 pydal-20240427.2/pydal/parsers/sqlite.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.939208 pydal-20240427.2/pydal/representers/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8806 2023-11-15 07:07:35.000000 pydal-20240427.2/pydal/representers/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8793 2023-11-15 07:07:35.000000 pydal-20240427.2/pydal/representers/base.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1210 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/couchdb.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      680 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/db2.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1446 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      884 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/informix.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1757 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/mongo.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      948 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/mssql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      214 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/mysql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1286 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/oracle.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1643 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/postgre.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      752 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/representers/sqlite.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    22855 2023-11-15 07:07:35.000000 pydal-20240427.2/pydal/restapi.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.939208 pydal-20240427.2/pydal/tools/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/tools/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2120 2023-11-15 06:54:34.000000 pydal-20240427.2/pydal/tools/tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1904 2022-10-17 00:44:46.000000 pydal-20240427.2/pydal/utils.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   158790 2023-11-19 17:50:44.000000 pydal-20240427.2/pydal/validators.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.922541 pydal-20240427.2/pydal.egg-info/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2903 2024-04-27 07:19:15.000000 pydal-20240427.2/pydal.egg-info/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3314 2024-04-27 07:19:15.000000 pydal-20240427.2/pydal.egg-info/SOURCES.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-04-27 07:19:15.000000 pydal-20240427.2/pydal.egg-info/dependency_links.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        6 2024-04-27 07:19:15.000000 pydal-20240427.2/pydal.egg-info/top_level.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      905 2024-04-27 07:19:10.000000 pydal-20240427.2/pyproject.toml
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       99 2024-04-27 07:19:15.949208 pydal-20240427.2/setup.cfg
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.942541 pydal-20240427.2/tests/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      355 2023-05-07 23:00:04.000000 pydal-20240427.2/tests/__init__.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-27 07:19:15.949208 pydal-20240427.2/tests/__pycache__/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      625 2024-04-27 07:03:00.000000 pydal-20240427.2/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1648 2023-12-28 08:14:31.000000 pydal-20240427.2/tests/__pycache__/_adapt.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      299 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/_compat.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1997 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/_helpers.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    17046 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6517 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/caching.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    12212 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/contribs.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5665 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/indexes.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    38716 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/is_url_validators.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    10845 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/restapi.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7654 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/smart_query.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   283900 2023-12-28 08:14:31.000000 pydal-20240427.2/tests/__pycache__/sql.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2554 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/tags.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6751 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/validation.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   100862 2023-12-28 08:14:32.000000 pydal-20240427.2/tests/__pycache__/validators.cpython-311.pyc
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      954 2022-10-17 00:44:46.000000 pydal-20240427.2/tests/_adapt.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       95 2022-10-17 00:44:46.000000 pydal-20240427.2/tests/_compat.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      765 2023-05-07 23:00:04.000000 pydal-20240427.2/tests/_helpers.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8103 2023-11-15 07:07:11.000000 pydal-20240427.2/tests/base.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2554 2023-05-07 23:00:03.000000 pydal-20240427.2/tests/caching.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     4954 2023-11-15 07:07:11.000000 pydal-20240427.2/tests/contribs.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2279 2023-05-07 23:00:03.000000 pydal-20240427.2/tests/indexes.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    29359 2023-11-15 07:07:11.000000 pydal-20240427.2/tests/is_url_validators.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    99826 2023-11-15 07:07:14.000000 pydal-20240427.2/tests/nosql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    14072 2023-11-15 07:07:11.000000 pydal-20240427.2/tests/restapi.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    12552 2023-05-07 23:00:04.000000 pydal-20240427.2/tests/smart_query.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   137750 2023-11-15 07:07:15.000000 pydal-20240427.2/tests/sql.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      990 2023-05-07 23:00:04.000000 pydal-20240427.2/tests/tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3604 2023-11-15 06:55:22.000000 pydal-20240427.2/tests/validation.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    66909 2023-11-15 07:07:13.000000 pydal-20240427.2/tests/validators.py
```

### Comparing `pydal-20240427.1/CHANGES` & `pydal-20240427.2/CHANGES`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/LICENSE.txt` & `pydal-20240427.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/PKG-INFO` & `pydal-20240427.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydal
-Version: 20240427.1
+Version: 20240427.2
 Summary: pyDAL is a Database Abstraction Layer. It generates queries for SQlite, PotsgreSQL, MySQL, and other backends. It was originally part of the web2py frameworks but it is now an independent project. Example: db.define_table("thing",Field("name")) and db.thing.insert(name="Pizza")
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/pydal
 Project-URL: Bug Tracker, https://github.com/web2py/pydal/issues
 Project-URL: Documentation, https://py4web.com/_documentation/static/en/chapter-07.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pydal-20240427.1/README.md` & `pydal-20240427.2/README.md`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/docs/Makefile` & `pydal-20240427.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/docs/conf.py` & `pydal-20240427.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/docs/index.rst` & `pydal-20240427.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/docs/pydal.adapters.rst` & `pydal-20240427.2/docs/pydal.adapters.rst`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/docs/pydal.helpers.rst` & `pydal-20240427.2/docs/pydal.helpers.rst`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/_compat.py` & `pydal-20240427.2/pydal/_compat.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/adapters/__init__.py` & `pydal-20240427.2/pydal/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/adapters/base.py` & `pydal-20240427.2/pydal/adapters/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/adapters/couchdb.py` & `pydal-20240427.2/pydal/adapters/couchdb.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/adapters/db2.py` & `pydal-20240427.2/pydal/adapters/db2.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/adapters/firebird.py` & `pydal-20240427.2/pydal/adapters/firebird.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/adapters/google.py` & `pydal-20240427.2/pydal/adapters/google.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/adapters/informix.py` & `pydal-20240427.2/pydal/adapters/informix.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/adapters/ingres.py` & `pydal-20240427.2/pydal/adapters/ingres.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/adapters/mongo.py` & `pydal-20240427.2/pydal/adapters/mongo.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/adapters/mssql.py` & `pydal-20240427.2/pydal/adapters/mssql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/adapters/mysql.py` & `pydal-20240427.2/pydal/adapters/mysql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/adapters/oracle.py` & `pydal-20240427.2/pydal/adapters/oracle.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/adapters/postgres.py` & `pydal-20240427.2/pydal/adapters/postgres.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/adapters/sap.py` & `pydal-20240427.2/pydal/adapters/sap.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/adapters/snowflake.py` & `pydal-20240427.2/pydal/adapters/snowflake.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/adapters/sqlite.py` & `pydal-20240427.2/pydal/adapters/sqlite.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/adapters/teradata.py` & `pydal-20240427.2/pydal/adapters/teradata.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/base.py` & `pydal-20240427.2/pydal/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/connection.py` & `pydal-20240427.2/pydal/connection.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/contrib/imap_adapter.py` & `pydal-20240427.2/pydal/contrib/imap_adapter.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/contrib/ipaddress.py` & `pydal-20240427.2/pydal/contrib/ipaddress.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/contrib/mockimaplib.py` & `pydal-20240427.2/pydal/contrib/mockimaplib.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/contrib/ordereddict.py` & `pydal-20240427.2/pydal/contrib/ordereddict.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/contrib/portalocker.py` & `pydal-20240427.2/pydal/contrib/portalocker.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/contrib/reserved_sql_keywords.py` & `pydal-20240427.2/pydal/contrib/reserved_sql_keywords.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/default_validators.py` & `pydal-20240427.2/pydal/default_validators.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/dialects/__init__.py` & `pydal-20240427.2/pydal/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/dialects/base.py` & `pydal-20240427.2/pydal/dialects/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/dialects/couchdb.py` & `pydal-20240427.2/pydal/dialects/couchdb.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/dialects/db2.py` & `pydal-20240427.2/pydal/dialects/db2.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/dialects/firebird.py` & `pydal-20240427.2/pydal/dialects/firebird.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/dialects/google.py` & `pydal-20240427.2/pydal/dialects/google.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/dialects/informix.py` & `pydal-20240427.2/pydal/dialects/informix.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/dialects/ingres.py` & `pydal-20240427.2/pydal/dialects/ingres.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/dialects/mongo.py` & `pydal-20240427.2/pydal/dialects/mongo.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/dialects/mssql.py` & `pydal-20240427.2/pydal/dialects/mssql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/dialects/mysql.py` & `pydal-20240427.2/pydal/dialects/mysql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/dialects/oracle.py` & `pydal-20240427.2/pydal/dialects/oracle.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/dialects/postgre.py` & `pydal-20240427.2/pydal/dialects/postgre.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/dialects/sap.py` & `pydal-20240427.2/pydal/dialects/sap.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/dialects/snowflake.py` & `pydal-20240427.2/pydal/dialects/snowflake.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/dialects/sqlite.py` & `pydal-20240427.2/pydal/dialects/sqlite.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/dialects/teradata.py` & `pydal-20240427.2/pydal/dialects/teradata.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/drivers.py` & `pydal-20240427.2/pydal/drivers.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/helpers/_internals.py` & `pydal-20240427.2/pydal/helpers/_internals.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/helpers/classes.py` & `pydal-20240427.2/pydal/helpers/classes.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/helpers/gae.py` & `pydal-20240427.2/pydal/helpers/gae.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/helpers/methods.py` & `pydal-20240427.2/pydal/helpers/methods.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/helpers/regex.py` & `pydal-20240427.2/pydal/helpers/regex.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/helpers/rest.py` & `pydal-20240427.2/pydal/helpers/rest.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/helpers/serializers.py` & `pydal-20240427.2/pydal/helpers/serializers.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/migrator.py` & `pydal-20240427.2/pydal/migrator.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/objects.py` & `pydal-20240427.2/pydal/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -623,20 +623,25 @@
             referees = pr.pop(self._tablename)
             for referee in referees:
                 if referee.type.startswith("list:reference "):
                     self._referenced_by_list.append(referee)
                 else:
                     self._referenced_by.append(referee)
 
-    def _filter_fields(self, record, id=False):
+    def _filter_fields(self, record, allow_id=False, writable_only=False):
         return dict(
             [
                 (k, v)
                 for (k, v) in iteritems(record)
-                if k in self.fields and (getattr(self, k).type != "id" or id)
+                # include fields if
+                if (
+                    k in self.fields
+                    and (allow_id or getattr(self, k).type != "id")  # are valid
+                    and (not writable_only or getattr(self, k).writable)  # are not ids
+                )  # are writable
             ]
         )
 
     def _build_query(self, key):
         """for keyed table only"""
         query = None
         for k, v in iteritems(key):
@@ -916,24 +921,22 @@
                 pass
             elif field.name in fields:
                 # only write if the field was passed and no error
                 new_fields[field.name] = value
         return response, new_fields
 
     def validate_and_insert(self, **fields):
-        if "id" in fields and "id" in self.fields and self.fields["id"].type == "id":
-            del fields["id"]
+        fields = self._filter_fields(fields, allow_id=False, writable_only=True)
         response, new_fields = self._validate_fields(fields, "default")
         if not response.get("errors"):
             response["id"] = self.insert(**new_fields)
         return response
 
     def validate_and_update(self, _key, **fields):
-        if "id" in fields and "id" in self.fields and self.fields["id"].type == "id":
-            del fields["id"]
+        fields = self._filter_fields(fields, allow_id=False, writable_only=True)
         record = self(**_key) if isinstance(_key, dict) else self(_key)
         response, new_fields = self._validate_fields(fields, "update", record.id)
         #: do the update
         if not response.get("errors") and record:
             if "_id" in self:
                 myset = self._db(self._id == record[self._id.name])
             else:
```

### Comparing `pydal-20240427.1/pydal/parsers/__init__.py` & `pydal-20240427.2/pydal/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/parsers/base.py` & `pydal-20240427.2/pydal/parsers/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/parsers/mongo.py` & `pydal-20240427.2/pydal/parsers/mongo.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/parsers/oracle.py` & `pydal-20240427.2/pydal/parsers/oracle.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/parsers/postgre.py` & `pydal-20240427.2/pydal/parsers/postgre.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/parsers/sqlite.py` & `pydal-20240427.2/pydal/parsers/sqlite.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/representers/__init__.py` & `pydal-20240427.2/pydal/representers/__init__.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/representers/base.py` & `pydal-20240427.2/pydal/representers/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/representers/couchdb.py` & `pydal-20240427.2/pydal/representers/couchdb.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/representers/db2.py` & `pydal-20240427.2/pydal/representers/db2.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/representers/google.py` & `pydal-20240427.2/pydal/representers/google.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/representers/informix.py` & `pydal-20240427.2/pydal/representers/informix.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/representers/mongo.py` & `pydal-20240427.2/pydal/representers/mongo.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/representers/mssql.py` & `pydal-20240427.2/pydal/representers/mssql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/representers/oracle.py` & `pydal-20240427.2/pydal/representers/oracle.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/representers/postgre.py` & `pydal-20240427.2/pydal/representers/postgre.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/representers/sqlite.py` & `pydal-20240427.2/pydal/representers/sqlite.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/restapi.py` & `pydal-20240427.2/pydal/restapi.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/tools/tags.py` & `pydal-20240427.2/pydal/tools/tags.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/utils.py` & `pydal-20240427.2/pydal/utils.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal/validators.py` & `pydal-20240427.2/pydal/validators.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pydal.egg-info/PKG-INFO` & `pydal-20240427.2/pydal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydal
-Version: 20240427.1
+Version: 20240427.2
 Summary: pyDAL is a Database Abstraction Layer. It generates queries for SQlite, PotsgreSQL, MySQL, and other backends. It was originally part of the web2py frameworks but it is now an independent project. Example: db.define_table("thing",Field("name")) and db.thing.insert(name="Pizza")
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/pydal
 Project-URL: Bug Tracker, https://github.com/web2py/pydal/issues
 Project-URL: Documentation, https://py4web.com/_documentation/static/en/chapter-07.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pydal-20240427.1/pydal.egg-info/SOURCES.txt` & `pydal-20240427.2/pydal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/pyproject.toml` & `pydal-20240427.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pydal"
-version = "20240427.1"
+version = "20240427.2"
 authors = [{ name="Massimo Di Pierro", email="massimo.dipierro@gmail.com" },]
 description = 'pyDAL is a Database Abstraction Layer. It generates queries for SQlite, PotsgreSQL, MySQL, and other backends. It was originally part of the web2py frameworks but it is now an independent project. Example: db.define_table("thing",Field("name")) and db.thing.insert(name="Pizza")'
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: BSD License",
```

### Comparing `pydal-20240427.1/tests/__pycache__/__init__.cpython-311.pyc` & `pydal-20240427.2/tests/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/__pycache__/_adapt.cpython-311.pyc` & `pydal-20240427.2/tests/__pycache__/_adapt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/__pycache__/_helpers.cpython-311.pyc` & `pydal-20240427.2/tests/__pycache__/_helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/__pycache__/base.cpython-311.pyc` & `pydal-20240427.2/tests/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/__pycache__/caching.cpython-311.pyc` & `pydal-20240427.2/tests/__pycache__/caching.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/__pycache__/contribs.cpython-311.pyc` & `pydal-20240427.2/tests/__pycache__/contribs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/__pycache__/indexes.cpython-311.pyc` & `pydal-20240427.2/tests/__pycache__/indexes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/__pycache__/is_url_validators.cpython-311.pyc` & `pydal-20240427.2/tests/__pycache__/is_url_validators.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/__pycache__/restapi.cpython-311.pyc` & `pydal-20240427.2/tests/__pycache__/restapi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/__pycache__/smart_query.cpython-311.pyc` & `pydal-20240427.2/tests/__pycache__/smart_query.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/__pycache__/sql.cpython-311.pyc` & `pydal-20240427.2/tests/__pycache__/sql.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/__pycache__/tags.cpython-311.pyc` & `pydal-20240427.2/tests/__pycache__/tags.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/__pycache__/validation.cpython-311.pyc` & `pydal-20240427.2/tests/__pycache__/validation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/__pycache__/validators.cpython-311.pyc` & `pydal-20240427.2/tests/__pycache__/validators.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/_adapt.py` & `pydal-20240427.2/tests/_adapt.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/_helpers.py` & `pydal-20240427.2/tests/_helpers.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/base.py` & `pydal-20240427.2/tests/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/caching.py` & `pydal-20240427.2/tests/caching.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/contribs.py` & `pydal-20240427.2/tests/contribs.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/indexes.py` & `pydal-20240427.2/tests/indexes.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/is_url_validators.py` & `pydal-20240427.2/tests/is_url_validators.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/nosql.py` & `pydal-20240427.2/tests/nosql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/restapi.py` & `pydal-20240427.2/tests/restapi.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/smart_query.py` & `pydal-20240427.2/tests/smart_query.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/sql.py` & `pydal-20240427.2/tests/sql.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/tags.py` & `pydal-20240427.2/tests/tags.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/validation.py` & `pydal-20240427.2/tests/validation.py`

 * *Files identical despite different names*

### Comparing `pydal-20240427.1/tests/validators.py` & `pydal-20240427.2/tests/validators.py`

 * *Files identical despite different names*

