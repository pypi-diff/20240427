# Comparing `tmp/mssql-django-1.4.2.tar.gz` & `tmp/mssql_django-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mssql-django-1.4.2.tar", last modified: Thu Mar 14 23:36:19 2024, max compression
+gzip compressed data, was "mssql_django-1.5.tar", last modified: Fri Apr 26 22:39:30 2024, max compression
```

## Comparing `mssql-django-1.4.2.tar` & `mssql_django-1.5.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-03-14 23:36:19.585832 mssql-django-1.4.2/
--rw-rw-r--   0 root         (0) root         (0)     1673 2024-03-14 23:36:08.000000 mssql-django-1.4.2/LICENSE.txt
--rw-rw-r--   0 root         (0) root         (0)      114 2024-03-14 23:36:08.000000 mssql-django-1.4.2/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)     1791 2024-03-14 23:36:08.000000 mssql-django-1.4.2/NOTICE.md
--rw-r--r--   0 root         (0) root         (0)    11839 2024-03-14 23:36:19.585832 mssql-django-1.4.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    10625 2024-03-14 23:36:08.000000 mssql-django-1.4.2/README.md
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-03-14 23:36:19.577832 mssql-django-1.4.2/mssql/
--rw-rw-r--   0 root         (0) root         (0)      105 2024-03-14 23:36:08.000000 mssql-django-1.4.2/mssql/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    27845 2024-03-14 23:36:08.000000 mssql-django-1.4.2/mssql/base.py
--rw-rw-r--   0 root         (0) root         (0)     1926 2024-03-14 23:36:08.000000 mssql-django-1.4.2/mssql/client.py
--rw-rw-r--   0 root         (0) root         (0)    30002 2024-03-14 23:36:08.000000 mssql-django-1.4.2/mssql/compiler.py
--rw-rw-r--   0 root         (0) root         (0)     4554 2024-03-14 23:36:08.000000 mssql-django-1.4.2/mssql/creation.py
--rw-rw-r--   0 root         (0) root         (0)     3043 2024-03-14 23:36:08.000000 mssql-django-1.4.2/mssql/features.py
--rw-rw-r--   0 root         (0) root         (0)    20657 2024-03-14 23:36:08.000000 mssql-django-1.4.2/mssql/functions.py
--rw-rw-r--   0 root         (0) root         (0)    19922 2024-03-14 23:36:08.000000 mssql-django-1.4.2/mssql/introspection.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-03-14 23:36:19.577832 mssql-django-1.4.2/mssql/management/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-14 23:36:08.000000 mssql-django-1.4.2/mssql/management/__init__.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-03-14 23:36:19.577832 mssql-django-1.4.2/mssql/management/commands/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-14 23:36:08.000000 mssql-django-1.4.2/mssql/management/commands/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      656 2024-03-14 23:36:08.000000 mssql-django-1.4.2/mssql/management/commands/inspectdb.py
--rw-rw-r--   0 root         (0) root         (0)      850 2024-03-14 23:36:08.000000 mssql-django-1.4.2/mssql/management/commands/install_regex_clr.py
--rw-rw-r--   0 root         (0) root         (0)    28419 2024-03-14 23:36:08.000000 mssql-django-1.4.2/mssql/operations.py
--rw-rw-r--   0 root         (0) root         (0)     4608 2022-03-02 21:19:22.000000 mssql-django-1.4.2/mssql/regex_clr.dll
--rw-rw-r--   0 root         (0) root         (0)    76809 2024-03-14 23:36:08.000000 mssql-django-1.4.2/mssql/schema.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-03-14 23:36:19.585832 mssql-django-1.4.2/mssql_django.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11839 2024-03-14 23:36:19.000000 mssql-django-1.4.2/mssql_django.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2429 2024-03-14 23:36:19.000000 mssql-django-1.4.2/mssql_django.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2024-03-14 23:36:19.000000 mssql-django-1.4.2/mssql_django.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       34 2024-03-14 23:36:19.000000 mssql-django-1.4.2/mssql_django.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       14 2024-03-14 23:36:19.000000 mssql-django-1.4.2/mssql_django.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      122 2024-03-14 23:36:19.589832 mssql-django-1.4.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1631 2024-03-14 23:36:08.000000 mssql-django-1.4.2/setup.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-03-14 23:36:19.581832 mssql-django-1.4.2/testapp/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/__init__.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-03-14 23:36:19.585832 mssql-django-1.4.2/testapp/migrations/
--rw-rw-r--   0 root         (0) root         (0)     2392 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0001_initial.py
--rw-rw-r--   0 root         (0) root         (0)      772 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0002_test_unique_nullable_part1.py
--rw-rw-r--   0 root         (0) root         (0)      810 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0003_test_unique_nullable_part2.py
--rw-rw-r--   0 root         (0) root         (0)     1023 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0004_test_unique_type_change_part1.py
--rw-rw-r--   0 root         (0) root         (0)     1407 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0005_test_unique_type_change_part2.py
--rw-rw-r--   0 root         (0) root         (0)      743 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0006_test_remove_onetoone_field_part1.py
--rw-rw-r--   0 root         (0) root         (0)      376 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0007_test_remove_onetoone_field_part2.py
--rw-rw-r--   0 root         (0) root         (0)      584 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0008_test_drop_table_with_foreign_key_reference_part1.py
--rw-rw-r--   0 root         (0) root         (0)      477 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0009_test_drop_table_with_foreign_key_reference_part2.py
--rw-rw-r--   0 root         (0) root         (0)      761 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0010_pizza_topping.py
--rw-rw-r--   0 root         (0) root         (0)     2380 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0011_test_unique_constraints.py
--rw-rw-r--   0 root         (0) root         (0)      678 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0012_test_indexes_retained_part1.py
--rw-rw-r--   0 root         (0) root         (0)      797 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0013_test_indexes_retained_part2.py
--rw-rw-r--   0 root         (0) root         (0)      887 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0014_test_rename_m2mfield_part1.py
--rw-rw-r--   0 root         (0) root         (0)      597 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0015_test_rename_m2mfield_part2.py
--rw-rw-r--   0 root         (0) root         (0)      774 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0016_jsonmodel.py
--rw-rw-r--   0 root         (0) root         (0)     1335 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0017_binarydata_testcheckconstraintwithunicode_and_more.py
--rw-rw-r--   0 root         (0) root         (0)     1252 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0018_choice_question.py
--rw-rw-r--   0 root         (0) root         (0)     1161 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0019_customer_name_customer_address.py
--rw-rw-r--   0 root         (0) root         (0)      418 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0020_autofield_to_bigautofield.py
--rw-rw-r--   0 root         (0) root         (0)      790 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0021_multiple_autofield_to_bigauto.py
--rw-rw-r--   0 root         (0) root         (0)      579 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0022_timezone.py
--rw-rw-r--   0 root         (0) root         (0)      703 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0023_number.py
--rw-rw-r--   0 root         (0) root         (0)     1744 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0024_publisher_book.py
--rw-rw-r--   0 root         (0) root         (0)      676 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/0025_modelwithnullablefieldsofdifferenttypes.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/migrations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8359 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/models.py
--rw-rw-r--   0 root         (0) root         (0)     1390 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/runners.py
--rw-rw-r--   0 root         (0) root         (0)    16981 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/settings.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-03-14 23:36:19.585832 mssql-django-1.4.2/testapp/tests/
--rw-rw-r--   0 root         (0) root         (0)      461 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      868 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/tests/test_bitshift.py
--rw-rw-r--   0 root         (0) root         (0)    11269 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/tests/test_constraints.py
--rw-rw-r--   0 root         (0) root         (0)     5820 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/tests/test_expressions.py
--rw-rw-r--   0 root         (0) root         (0)     1324 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/tests/test_fields.py
--rw-rw-r--   0 root         (0) root         (0)     1739 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/tests/test_getorcreate.py
--rw-rw-r--   0 root         (0) root         (0)     9762 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/tests/test_indexes.py
--rw-rw-r--   0 root         (0) root         (0)     2008 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/tests/test_jsonfield.py
--rw-rw-r--   0 root         (0) root         (0)      484 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/tests/test_lookups.py
--rw-rw-r--   0 root         (0) root         (0)     3679 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/tests/test_multiple_databases.py
--rw-rw-r--   0 root         (0) root         (0)     1299 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/tests/test_queries.py
--rw-rw-r--   0 root         (0) root         (0)     4172 2024-03-14 23:36:08.000000 mssql-django-1.4.2/testapp/tests/test_timezones.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-04-26 22:39:30.350628 mssql_django-1.5/
+-rw-rw-r--   0 root         (0) root         (0)     1673 2024-04-26 22:39:14.000000 mssql_django-1.5/LICENSE.txt
+-rw-rw-r--   0 root         (0) root         (0)      114 2024-04-26 22:39:14.000000 mssql_django-1.5/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)     1791 2024-04-26 22:39:14.000000 mssql_django-1.5/NOTICE.md
+-rw-r--r--   0 root         (0) root         (0)    11837 2024-04-26 22:39:30.350628 mssql_django-1.5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    10625 2024-04-26 22:39:14.000000 mssql_django-1.5/README.md
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-04-26 22:39:30.338628 mssql_django-1.5/mssql/
+-rw-rw-r--   0 root         (0) root         (0)      105 2024-04-26 22:39:14.000000 mssql_django-1.5/mssql/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    27936 2024-04-26 22:39:14.000000 mssql_django-1.5/mssql/base.py
+-rw-rw-r--   0 root         (0) root         (0)     1926 2024-04-26 22:39:14.000000 mssql_django-1.5/mssql/client.py
+-rw-rw-r--   0 root         (0) root         (0)    30002 2024-04-26 22:39:14.000000 mssql_django-1.5/mssql/compiler.py
+-rw-rw-r--   0 root         (0) root         (0)     4554 2024-04-26 22:39:14.000000 mssql_django-1.5/mssql/creation.py
+-rw-rw-r--   0 root         (0) root         (0)     3043 2024-04-26 22:39:14.000000 mssql_django-1.5/mssql/features.py
+-rw-rw-r--   0 root         (0) root         (0)    20657 2024-04-26 22:39:14.000000 mssql_django-1.5/mssql/functions.py
+-rw-rw-r--   0 root         (0) root         (0)    20322 2024-04-26 22:39:14.000000 mssql_django-1.5/mssql/introspection.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-04-26 22:39:30.338628 mssql_django-1.5/mssql/management/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-26 22:39:14.000000 mssql_django-1.5/mssql/management/__init__.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-04-26 22:39:30.342628 mssql_django-1.5/mssql/management/commands/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-26 22:39:14.000000 mssql_django-1.5/mssql/management/commands/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      656 2024-04-26 22:39:14.000000 mssql_django-1.5/mssql/management/commands/inspectdb.py
+-rw-rw-r--   0 root         (0) root         (0)      850 2024-04-26 22:39:14.000000 mssql_django-1.5/mssql/management/commands/install_regex_clr.py
+-rw-rw-r--   0 root         (0) root         (0)    28419 2024-04-26 22:39:14.000000 mssql_django-1.5/mssql/operations.py
+-rw-rw-r--   0 root         (0) root         (0)     4608 2022-03-02 21:19:22.000000 mssql_django-1.5/mssql/regex_clr.dll
+-rw-rw-r--   0 root         (0) root         (0)    77032 2024-04-26 22:39:14.000000 mssql_django-1.5/mssql/schema.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-04-26 22:39:30.350628 mssql_django-1.5/mssql_django.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11837 2024-04-26 22:39:30.000000 mssql_django-1.5/mssql_django.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2429 2024-04-26 22:39:30.000000 mssql_django-1.5/mssql_django.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-04-26 22:39:30.000000 mssql_django-1.5/mssql_django.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       34 2024-04-26 22:39:30.000000 mssql_django-1.5/mssql_django.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       14 2024-04-26 22:39:30.000000 mssql_django-1.5/mssql_django.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      122 2024-04-26 22:39:30.350628 mssql_django-1.5/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1629 2024-04-26 22:39:14.000000 mssql_django-1.5/setup.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-04-26 22:39:30.342628 mssql_django-1.5/testapp/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/__init__.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-04-26 22:39:30.346628 mssql_django-1.5/testapp/migrations/
+-rw-rw-r--   0 root         (0) root         (0)     2392 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0001_initial.py
+-rw-rw-r--   0 root         (0) root         (0)      772 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0002_test_unique_nullable_part1.py
+-rw-rw-r--   0 root         (0) root         (0)      810 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0003_test_unique_nullable_part2.py
+-rw-rw-r--   0 root         (0) root         (0)     1023 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0004_test_unique_type_change_part1.py
+-rw-rw-r--   0 root         (0) root         (0)     1407 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0005_test_unique_type_change_part2.py
+-rw-rw-r--   0 root         (0) root         (0)      743 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0006_test_remove_onetoone_field_part1.py
+-rw-rw-r--   0 root         (0) root         (0)      376 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0007_test_remove_onetoone_field_part2.py
+-rw-rw-r--   0 root         (0) root         (0)      584 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0008_test_drop_table_with_foreign_key_reference_part1.py
+-rw-rw-r--   0 root         (0) root         (0)      477 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0009_test_drop_table_with_foreign_key_reference_part2.py
+-rw-rw-r--   0 root         (0) root         (0)      761 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0010_pizza_topping.py
+-rw-rw-r--   0 root         (0) root         (0)     2380 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0011_test_unique_constraints.py
+-rw-rw-r--   0 root         (0) root         (0)      678 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0012_test_indexes_retained_part1.py
+-rw-rw-r--   0 root         (0) root         (0)      797 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0013_test_indexes_retained_part2.py
+-rw-rw-r--   0 root         (0) root         (0)      887 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0014_test_rename_m2mfield_part1.py
+-rw-rw-r--   0 root         (0) root         (0)      597 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0015_test_rename_m2mfield_part2.py
+-rw-rw-r--   0 root         (0) root         (0)      774 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0016_jsonmodel.py
+-rw-rw-r--   0 root         (0) root         (0)     1335 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0017_binarydata_testcheckconstraintwithunicode_and_more.py
+-rw-rw-r--   0 root         (0) root         (0)     1252 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0018_choice_question.py
+-rw-rw-r--   0 root         (0) root         (0)     1161 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0019_customer_name_customer_address.py
+-rw-rw-r--   0 root         (0) root         (0)      418 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0020_autofield_to_bigautofield.py
+-rw-rw-r--   0 root         (0) root         (0)      790 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0021_multiple_autofield_to_bigauto.py
+-rw-rw-r--   0 root         (0) root         (0)      579 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0022_timezone.py
+-rw-rw-r--   0 root         (0) root         (0)      703 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0023_number.py
+-rw-rw-r--   0 root         (0) root         (0)     1744 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0024_publisher_book.py
+-rw-rw-r--   0 root         (0) root         (0)      676 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/0025_modelwithnullablefieldsofdifferenttypes.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/migrations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8359 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/models.py
+-rw-rw-r--   0 root         (0) root         (0)     1390 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/runners.py
+-rw-rw-r--   0 root         (0) root         (0)    16929 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/settings.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-04-26 22:39:30.350628 mssql_django-1.5/testapp/tests/
+-rw-rw-r--   0 root         (0) root         (0)      461 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      868 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/tests/test_bitshift.py
+-rw-rw-r--   0 root         (0) root         (0)    11269 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/tests/test_constraints.py
+-rw-rw-r--   0 root         (0) root         (0)     5820 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/tests/test_expressions.py
+-rw-rw-r--   0 root         (0) root         (0)     1324 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/tests/test_fields.py
+-rw-rw-r--   0 root         (0) root         (0)     1739 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/tests/test_getorcreate.py
+-rw-rw-r--   0 root         (0) root         (0)     9762 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/tests/test_indexes.py
+-rw-rw-r--   0 root         (0) root         (0)     2008 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/tests/test_jsonfield.py
+-rw-rw-r--   0 root         (0) root         (0)      484 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/tests/test_lookups.py
+-rw-rw-r--   0 root         (0) root         (0)     3679 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/tests/test_multiple_databases.py
+-rw-rw-r--   0 root         (0) root         (0)     1299 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/tests/test_queries.py
+-rw-rw-r--   0 root         (0) root         (0)     4172 2024-04-26 22:39:14.000000 mssql_django-1.5/testapp/tests/test_timezones.py
```

### Comparing `mssql-django-1.4.2/LICENSE.txt` & `mssql_django-1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/NOTICE.md` & `mssql_django-1.5/NOTICE.md`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/PKG-INFO` & `mssql_django-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mssql-django
-Version: 1.4.2
+Version: 1.5
 Summary: Django backend for Microsoft SQL Server
 Home-page: https://github.com/microsoft/mssql-django
 Author: Microsoft
 Author-email: opencode@microsoft.com
 License: BSD
 Project-URL: Release Notes, https://github.com/microsoft/mssql-django/releases
 Keywords: django
```

### Comparing `mssql-django-1.4.2/README.md` & `mssql_django-1.5/README.md`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/mssql/base.py` & `mssql_django-1.5/mssql/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -614,32 +614,34 @@
         # pyodbc uses '?' instead of '%s' as parameter placeholder.
         if params is not None and params != []:
             sql = sql % tuple('?' * len(params))
 
         return sql
 
     def format_group_by_params(self, query, params):
+        # Prepare query for string formatting
+        query = re.sub(r'%\w+', '{}', query)
+
         if params:
             # Insert None params directly into the query
             if None in params:
-                null_params = ['NULL' if param is None else '%s' for param in params]
-                query = query % tuple(null_params)
+                null_params = ['NULL' if param is None else '{}' for param in params]
+                query = query.format(*null_params)
                 params = tuple(p for p in params if p is not None)
             params = [(param, type(param)) for param in params]
             params_dict = {param: '@var%d' % i for i, param in enumerate(set(params))}
             args = [params_dict[param] for param in params]
 
             variables = []
             params = []
             for key, value in params_dict.items():
                 datatype = self._as_sql_type(key[1], key[0])
                 variables.append("%s %s = %%s " % (value, datatype))
                 params.append(key[0])
-            query = ('DECLARE %s \n' % ','.join(variables)) + (query % tuple(args))
-
+            query = ('DECLARE %s \n' % ','.join(variables)) + (query.format(*args))
         return query, params
 
     def format_params(self, params):
         fp = []
         if params is not None:
             for p in params:
                 if isinstance(p, str):
```

### Comparing `mssql-django-1.4.2/mssql/client.py` & `mssql_django-1.5/mssql/client.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/mssql/compiler.py` & `mssql_django-1.5/mssql/compiler.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/mssql/creation.py` & `mssql_django-1.5/mssql/creation.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/mssql/features.py` & `mssql_django-1.5/mssql/features.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/mssql/functions.py` & `mssql_django-1.5/mssql/functions.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/mssql/introspection.py` & `mssql_django-1.5/mssql/introspection.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,27 +73,30 @@
                 field_type = 'CharField'
         return field_type
 
     def get_table_list(self, cursor):
         """
         Returns a list of table and view names in the current database.
         """
-        sql = """SELECT
-                    TABLE_NAME,
-                    TABLE_TYPE,
-                    CAST(ep.value AS VARCHAR) AS COMMENT
-                FROM INFORMATION_SCHEMA.TABLES i
-                LEFT JOIN sys.tables t ON t.name = i.TABLE_NAME
-                LEFT JOIN sys.extended_properties ep ON t.object_id = ep.major_id
-                AND ((ep.name = 'MS_DESCRIPTION' AND ep.minor_id = 0) OR ep.value IS NULL)
-                AND i.TABLE_SCHEMA = %s""" % (
-            get_schema_name())
+        if VERSION >= (4, 2) and self.connection.features.supports_comments:
+            sql = """SELECT
+                        TABLE_NAME,
+                        TABLE_TYPE,
+                        CAST(ep.value AS VARCHAR) AS COMMENT
+                    FROM INFORMATION_SCHEMA.TABLES i
+                    LEFT JOIN sys.tables t ON t.name = i.TABLE_NAME
+                    LEFT JOIN sys.extended_properties ep ON t.object_id = ep.major_id
+                    AND ((ep.name = 'MS_DESCRIPTION' AND ep.minor_id = 0) OR ep.value IS NULL)
+                    WHERE i.TABLE_SCHEMA = %s""" % (
+                get_schema_name())
+        else:
+            sql = 'SELECT TABLE_NAME, TABLE_TYPE FROM INFORMATION_SCHEMA.TABLES WHERE TABLE_SCHEMA = %s' % (get_schema_name())
         cursor.execute(sql)
         types = {'BASE TABLE': 't', 'VIEW': 'v'}
-        if VERSION >= (4, 2):
+        if VERSION >= (4, 2) and self.connection.features.supports_comments:
             return [TableInfo(row[0], types.get(row[1]), row[2])
                     for row in cursor.fetchall()
                     if row[0] not in self.ignored_tables]
         else:
             return [BaseTableInfo(row[0], types.get(row[1]))
                     for row in cursor.fetchall()
                     if row[0] not in self.ignored_tables]
@@ -141,15 +144,15 @@
                             WHERE t.name = '%s' and c.name = '%s'
                             """ % (table_name, column[0])
                     cursor.execute(sql)
                     collation_name = cursor.fetchone()
                     column.append(collation_name[0] if collation_name else '')
                 else:
                     column.append('')
-            if VERSION >= (4, 2):
+            if VERSION >= (4, 2) and self.connection.features.supports_comments:
                 sql = """select CAST(ep.value AS VARCHAR) AS COMMENT
                         FROM sys.columns c
                         INNER JOIN sys.tables t ON c.object_id = t.object_id
                         INNER JOIN sys.extended_properties ep ON c.object_id=ep.major_id AND ep.minor_id = c.column_id
                         WHERE t.name = '%s' AND c.name = '%s' AND ep.name = 'MS_Description'
                         """ % (table_name, column[0])
                 cursor.execute(sql)
@@ -170,16 +173,15 @@
                 start = 0
                 end = -1
                 for _ in range(2):
                     if default_value[start] == '(' and default_value[end] == ')':
                         start += 1
                         end -= 1
                 column[7] = default_value[start:end + 1]
-
-            if VERSION >= (4, 2):
+            if VERSION >= (4, 2) and self.connection.features.supports_comments:
                 items.append(FieldInfo(*column))
             else:
                 items.append(BaseFieldInfo(*column))
         return items
 
     def get_sequences(self, cursor, table_name, table_fields=()):
         cursor.execute(f"""
```

### Comparing `mssql-django-1.4.2/mssql/management/commands/inspectdb.py` & `mssql_django-1.5/mssql/management/commands/inspectdb.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/mssql/management/commands/install_regex_clr.py` & `mssql_django-1.5/mssql/management/commands/install_regex_clr.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/mssql/operations.py` & `mssql_django-1.5/mssql/operations.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/mssql/regex_clr.dll` & `mssql_django-1.5/mssql/regex_clr.dll`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/mssql/schema.py` & `mssql_django-1.5/mssql/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,17 +384,18 @@
     def _add_deferred_unique_index_for_field(self, field, statement):
         self._deferred_unique_indexes[str(field)].append(statement)
 
     def _column_generated_sql(self, field):
         """Return the SQL to use in a GENERATED ALWAYS clause."""
         expression_sql, params = field.generated_sql(self.connection)
         persistency_sql = "PERSISTED" if field.db_persist else ""
-        if params:
+        if self.connection.features.requires_literal_defaults:
             expression_sql = expression_sql % tuple(self.quote_value(p) for p in params)
-        return f"AS {expression_sql} {persistency_sql}"
+            params = ()
+        return f"GENERATED ALWAYS AS ({expression_sql}) {persistency_sql}", params
 
     def _alter_field(self, model, old_field, new_field, old_type, new_type,
                      old_db_params, new_db_params, strict=False):
         """Actually perform a "physical" (non-ManyToMany) field update."""
 
         # the backend doesn't support altering a column to/from AutoField as
         # SQL Server cannot alter columns to add and remove IDENTITY properties
@@ -1020,14 +1021,16 @@
         if field.many_to_many and field.remote_field.through._meta.auto_created:
             return self.create_model(field.remote_field.through)
         # Get the column's definition
         definition, params = self.column_sql(model, field, include_default=True)
         # It might not actually have a column behind it
         if definition is None:
             return
+        if col_type_suffix := field.db_type_suffix(connection=self.connection):
+            definition += f" {col_type_suffix}"
         # Remove column type from definition if field is generated
         if (django_version >= (5,0) and field.generated):
             definition = definition[definition.find('AS'):]
         # Nullable columns with default values require 'WITH VALUES' to set existing rows
         if 'DEFAULT' in definition and field.null:
             definition = definition.replace('NULL', 'WITH VALUES')
```

### Comparing `mssql-django-1.4.2/mssql_django.egg-info/PKG-INFO` & `mssql_django-1.5/mssql_django.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mssql-django
-Version: 1.4.2
+Version: 1.5
 Summary: Django backend for Microsoft SQL Server
 Home-page: https://github.com/microsoft/mssql-django
 Author: Microsoft
 Author-email: opencode@microsoft.com
 License: BSD
 Project-URL: Release Notes, https://github.com/microsoft/mssql-django/releases
 Keywords: django
```

### Comparing `mssql-django-1.4.2/mssql_django.egg-info/SOURCES.txt` & `mssql_django-1.5/mssql_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/setup.py` & `mssql_django-1.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='mssql-django',
-    version='1.4.2',
+    version='1.5',
     description='Django backend for Microsoft SQL Server',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Microsoft',
     author_email='opencode@microsoft.com',
     url='https://github.com/microsoft/mssql-django',
     project_urls={
```

### Comparing `mssql-django-1.4.2/testapp/migrations/0001_initial.py` & `mssql_django-1.5/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0002_test_unique_nullable_part1.py` & `mssql_django-1.5/testapp/migrations/0002_test_unique_nullable_part1.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0003_test_unique_nullable_part2.py` & `mssql_django-1.5/testapp/migrations/0003_test_unique_nullable_part2.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0004_test_unique_type_change_part1.py` & `mssql_django-1.5/testapp/migrations/0004_test_unique_type_change_part1.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0005_test_unique_type_change_part2.py` & `mssql_django-1.5/testapp/migrations/0005_test_unique_type_change_part2.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0006_test_remove_onetoone_field_part1.py` & `mssql_django-1.5/testapp/migrations/0006_test_remove_onetoone_field_part1.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0008_test_drop_table_with_foreign_key_reference_part1.py` & `mssql_django-1.5/testapp/migrations/0008_test_drop_table_with_foreign_key_reference_part1.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0010_pizza_topping.py` & `mssql_django-1.5/testapp/migrations/0010_pizza_topping.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0011_test_unique_constraints.py` & `mssql_django-1.5/testapp/migrations/0011_test_unique_constraints.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0012_test_indexes_retained_part1.py` & `mssql_django-1.5/testapp/migrations/0012_test_indexes_retained_part1.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0013_test_indexes_retained_part2.py` & `mssql_django-1.5/testapp/migrations/0013_test_indexes_retained_part2.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0014_test_rename_m2mfield_part1.py` & `mssql_django-1.5/testapp/migrations/0014_test_rename_m2mfield_part1.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0015_test_rename_m2mfield_part2.py` & `mssql_django-1.5/testapp/migrations/0015_test_rename_m2mfield_part2.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0016_jsonmodel.py` & `mssql_django-1.5/testapp/migrations/0016_jsonmodel.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0017_binarydata_testcheckconstraintwithunicode_and_more.py` & `mssql_django-1.5/testapp/migrations/0017_binarydata_testcheckconstraintwithunicode_and_more.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0018_choice_question.py` & `mssql_django-1.5/testapp/migrations/0018_choice_question.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0019_customer_name_customer_address.py` & `mssql_django-1.5/testapp/migrations/0019_customer_name_customer_address.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0021_multiple_autofield_to_bigauto.py` & `mssql_django-1.5/testapp/migrations/0021_multiple_autofield_to_bigauto.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0022_timezone.py` & `mssql_django-1.5/testapp/migrations/0022_timezone.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0023_number.py` & `mssql_django-1.5/testapp/migrations/0023_number.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0024_publisher_book.py` & `mssql_django-1.5/testapp/migrations/0024_publisher_book.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/migrations/0025_modelwithnullablefieldsofdifferenttypes.py` & `mssql_django-1.5/testapp/migrations/0025_modelwithnullablefieldsofdifferenttypes.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/models.py` & `mssql_django-1.5/testapp/models.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/runners.py` & `mssql_django-1.5/testapp/runners.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/settings.py` & `mssql_django-1.5/testapp/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,14 @@
     # Django 4.1
     'aggregation.test_filter_argument.FilteredAggregateTests.test_filtered_aggregate_on_exists',
     'aggregation.tests.AggregateTestCase.test_aggregation_exists_multivalued_outeref',
     'annotations.tests.NonAggregateAnnotationTestCase.test_full_expression_annotation_with_aggregation',
     'db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_extract_lookup_name_sql_injection',
     'db_functions.datetime.test_extract_trunc.DateFunctionTests.test_extract_lookup_name_sql_injection',
     'schema.tests.SchemaTests.test_autofield_to_o2o',
-    'schema.tests.SchemaTests.test_add_auto_field',
     'prefetch_related.tests.PrefetchRelatedTests.test_m2m_prefetching_iterator_with_chunks',
     'migrations.test_operations.OperationTests.test_create_model_with_boolean_expression_in_check_constraint',
     'queries.test_qs_combinators.QuerySetSetOperationTests.test_union_in_subquery_related_outerref',
     # These tests pass on SQL Server 2022 or newer
     'model_fields.test_jsonfield.TestQuerying.test_has_key_list',
     'model_fields.test_jsonfield.TestQuerying.test_has_key_null_value',
     'model_fields.test_jsonfield.TestQuerying.test_lookups_with_key_transform',
```

### Comparing `mssql-django-1.4.2/testapp/tests/test_bitshift.py` & `mssql_django-1.5/testapp/tests/test_bitshift.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/tests/test_constraints.py` & `mssql_django-1.5/testapp/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/tests/test_expressions.py` & `mssql_django-1.5/testapp/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/tests/test_fields.py` & `mssql_django-1.5/testapp/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/tests/test_getorcreate.py` & `mssql_django-1.5/testapp/tests/test_getorcreate.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/tests/test_indexes.py` & `mssql_django-1.5/testapp/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/tests/test_jsonfield.py` & `mssql_django-1.5/testapp/tests/test_jsonfield.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/tests/test_multiple_databases.py` & `mssql_django-1.5/testapp/tests/test_multiple_databases.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/tests/test_queries.py` & `mssql_django-1.5/testapp/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.4.2/testapp/tests/test_timezones.py` & `mssql_django-1.5/testapp/tests/test_timezones.py`

 * *Files identical despite different names*

