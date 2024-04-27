# Comparing `tmp/django_ninja_jwt-5.3.0.tar.gz` & `tmp/django_ninja_jwt-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ninja_jwt-5.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_ninja_jwt-5.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_ninja_jwt-5.3.0.tar` & `django_ninja_jwt-5.3.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     4962 2024-01-06 10:52:56.511298 django_ninja_jwt-5.3.0/README.md
--rw-r--r--   0        0        0       80 2024-01-06 10:52:56.515298 django_ninja_jwt-5.3.0/ninja_jwt/__init__.py
--rw-r--r--   0        0        0     5229 2024-01-06 10:52:56.515298 django_ninja_jwt-5.3.0/ninja_jwt/authentication.py
--rw-r--r--   0        0        0     4732 2024-01-06 10:52:56.515298 django_ninja_jwt-5.3.0/ninja_jwt/backends.py
--rw-r--r--   0        0        0     1384 2024-01-06 10:52:56.515298 django_ninja_jwt-5.3.0/ninja_jwt/compat.py
--rw-r--r--   0        0        0     6399 2024-01-06 10:52:56.515298 django_ninja_jwt-5.3.0/ninja_jwt/controller.py
--rw-r--r--   0        0        0     1229 2024-01-06 10:52:56.515298 django_ninja_jwt-5.3.0/ninja_jwt/exceptions.py
--rw-r--r--   0        0        0     2050 2024-01-06 10:52:56.515298 django_ninja_jwt-5.3.0/ninja_jwt/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2918 2024-01-06 10:52:56.515298 django_ninja_jwt-5.3.0/ninja_jwt/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2057 2024-01-06 10:52:56.515298 django_ninja_jwt-5.3.0/ninja_jwt/locale/de_CH/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2937 2024-01-06 10:52:56.515298 django_ninja_jwt-5.3.0/ninja_jwt/locale/de_CH/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2350 2024-01-06 10:52:56.515298 django_ninja_jwt-5.3.0/ninja_jwt/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3109 2024-01-06 10:52:56.515298 django_ninja_jwt-5.3.0/ninja_jwt/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2166 2024-01-06 10:52:56.515298 django_ninja_jwt-5.3.0/ninja_jwt/locale/es_AR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3152 2024-01-06 10:52:56.515298 django_ninja_jwt-5.3.0/ninja_jwt/locale/es_AR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2128 2024-01-06 10:52:56.515298 django_ninja_jwt-5.3.0/ninja_jwt/locale/es_CL/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3034 2024-01-06 10:52:56.515298 django_ninja_jwt-5.3.0/ninja_jwt/locale/es_CL/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2363 2024-01-06 10:52:56.515298 django_ninja_jwt-5.3.0/ninja_jwt/locale/fa_IR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3257 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/fa_IR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2352 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3116 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2333 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/id_ID/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3092 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/id_ID/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2433 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3203 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2720 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3410 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1989 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/nl_NL/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2888 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/nl_NL/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2106 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/pl_PL/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2997 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/pl_PL/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2324 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3081 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2548 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3257 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/ro/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2784 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/ru_RU/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3698 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/ru_RU/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2281 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3063 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/sv/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2326 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3079 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/tr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3039 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/uk_UA/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3940 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/uk_UA/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2162 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2939 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3257 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/models.py
--rw-r--r--   0        0        0        0 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/routers/__init__.py
--rw-r--r--   0        0        0      445 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/routers/blacklist.py
--rw-r--r--   0        0        0     1458 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/routers/obtain.py
--rw-r--r--   0        0        0      423 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/routers/verify.py
--rw-r--r--   0        0        0    11904 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/schema.py
--rw-r--r--   0        0        0     3007 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/schema_control.py
--rw-r--r--   0        0        0     3966 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/settings.py
--rw-r--r--   0        0        0      327 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/state.py
--rw-r--r--   0        0        0      128 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/__init__.py
--rw-r--r--   0        0        0     2341 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/admin.py
--rw-r--r--   0        0        0      266 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/apps.py
--rw-r--r--   0        0        0        0 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/management/__init__.py
--rw-r--r--   0        0        0        0 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/management/commands/__init__.py
--rw-r--r--   0        0        0      355 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/management/commands/flushexpiredtokens.py
--rw-r--r--   0        0        0     2003 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/migrations/0001_initial.py
--rw-r--r--   0        0        0      366 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/migrations/0002_outstandingtoken_jti_hex.py
--rw-r--r--   0        0        0      906 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/migrations/0003_auto_20171017_2007.py
--rw-r--r--   0        0        0      369 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/migrations/0004_auto_20171017_2013.py
--rw-r--r--   0        0        0      293 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/migrations/0005_remove_outstandingtoken_jti.py
--rw-r--r--   0        0        0      338 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/migrations/0006_auto_20171017_2113.py
--rw-r--r--   0        0        0      759 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/migrations/0007_auto_20171017_2214.py
--rw-r--r--   0        0        0      691 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/migrations/0008_migrate_to_bigautofield.py
--rw-r--r--   0        0        0      692 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py
--rw-r--r--   0        0        0      578 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/migrations/0011_linearizes_history.py
--rw-r--r--   0        0        0      698 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/migrations/0012_alter_outstandingtoken_user.py
--rw-r--r--   0        0        0        0 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/migrations/__init__.py
--rw-r--r--   0        0        0     1583 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/models.py
--rw-r--r--   0        0        0    11606 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/tokens.py
--rw-r--r--   0        0        0     1726 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/ninja_jwt/utils.py
--rw-r--r--   0        0        0     2804 2024-01-06 10:52:56.519298 django_ninja_jwt-5.3.0/pyproject.toml
--rw-r--r--   0        0        0     7790 1970-01-01 00:00:00.000000 django_ninja_jwt-5.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4962 2024-04-27 05:58:50.160813 django_ninja_jwt-5.3.1/README.md
+-rw-r--r--   0        0        0       80 2024-04-27 05:58:50.164813 django_ninja_jwt-5.3.1/ninja_jwt/__init__.py
+-rw-r--r--   0        0        0     5229 2024-04-27 05:58:50.164813 django_ninja_jwt-5.3.1/ninja_jwt/authentication.py
+-rw-r--r--   0        0        0     4732 2024-04-27 05:58:50.164813 django_ninja_jwt-5.3.1/ninja_jwt/backends.py
+-rw-r--r--   0        0        0     1384 2024-04-27 05:58:50.164813 django_ninja_jwt-5.3.1/ninja_jwt/compat.py
+-rw-r--r--   0        0        0     6544 2024-04-27 05:58:50.164813 django_ninja_jwt-5.3.1/ninja_jwt/controller.py
+-rw-r--r--   0        0        0     1229 2024-04-27 05:58:50.164813 django_ninja_jwt-5.3.1/ninja_jwt/exceptions.py
+-rw-r--r--   0        0        0     2050 2024-04-27 05:58:50.164813 django_ninja_jwt-5.3.1/ninja_jwt/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2918 2024-04-27 05:58:50.164813 django_ninja_jwt-5.3.1/ninja_jwt/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2057 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/de_CH/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2937 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/de_CH/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2350 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3109 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2166 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3152 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/es_AR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2128 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/es_CL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3034 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/es_CL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2363 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/fa_IR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3257 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/fa_IR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2352 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3116 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2333 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/id_ID/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3092 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/id_ID/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2433 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3203 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2720 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3410 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1989 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/nl_NL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2888 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/nl_NL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2106 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2997 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2324 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3081 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2548 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3257 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/ro/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2784 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/ru_RU/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3698 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/ru_RU/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2281 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3063 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/sv/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2326 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3079 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3039 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/uk_UA/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3940 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/uk_UA/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2162 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2939 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3257 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/models.py
+-rw-r--r--   0        0        0        0 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/routers/__init__.py
+-rw-r--r--   0        0        0      459 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/routers/blacklist.py
+-rw-r--r--   0        0        0     1458 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/routers/obtain.py
+-rw-r--r--   0        0        0      434 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/routers/verify.py
+-rw-r--r--   0        0        0    11904 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/schema.py
+-rw-r--r--   0        0        0     3007 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/schema_control.py
+-rw-r--r--   0        0        0     3966 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/settings.py
+-rw-r--r--   0        0        0      327 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/state.py
+-rw-r--r--   0        0        0      128 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/__init__.py
+-rw-r--r--   0        0        0     2341 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/admin.py
+-rw-r--r--   0        0        0      266 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/apps.py
+-rw-r--r--   0        0        0        0 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/management/commands/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/management/commands/flushexpiredtokens.py
+-rw-r--r--   0        0        0     2003 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/migrations/0001_initial.py
+-rw-r--r--   0        0        0      366 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/migrations/0002_outstandingtoken_jti_hex.py
+-rw-r--r--   0        0        0      906 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/migrations/0003_auto_20171017_2007.py
+-rw-r--r--   0        0        0      369 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/migrations/0004_auto_20171017_2013.py
+-rw-r--r--   0        0        0      293 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/migrations/0005_remove_outstandingtoken_jti.py
+-rw-r--r--   0        0        0      338 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/migrations/0006_auto_20171017_2113.py
+-rw-r--r--   0        0        0      759 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/migrations/0007_auto_20171017_2214.py
+-rw-r--r--   0        0        0      691 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/migrations/0008_migrate_to_bigautofield.py
+-rw-r--r--   0        0        0      692 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py
+-rw-r--r--   0        0        0      578 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/migrations/0011_linearizes_history.py
+-rw-r--r--   0        0        0      698 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/migrations/0012_alter_outstandingtoken_user.py
+-rw-r--r--   0        0        0        0 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/migrations/__init__.py
+-rw-r--r--   0        0        0     1583 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/models.py
+-rw-r--r--   0        0        0    11606 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/tokens.py
+-rw-r--r--   0        0        0     1726 2024-04-27 05:58:50.168813 django_ninja_jwt-5.3.1/ninja_jwt/utils.py
+-rw-r--r--   0        0        0     2804 2024-04-27 05:58:50.172813 django_ninja_jwt-5.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7790 1970-01-01 00:00:00.000000 django_ninja_jwt-5.3.1/PKG-INFO
```

### Comparing `django_ninja_jwt-5.3.0/README.md` & `django_ninja_jwt-5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/authentication.py` & `django_ninja_jwt-5.3.1/ninja_jwt/authentication.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/backends.py` & `django_ninja_jwt-5.3.1/ninja_jwt/backends.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/compat.py` & `django_ninja_jwt-5.3.1/ninja_jwt/compat.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/controller.py` & `django_ninja_jwt-5.3.1/ninja_jwt/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from asgiref.sync import sync_to_async
-from ninja import Schema
 from ninja_extra import ControllerBase, api_controller, http_post
 from ninja_extra.permissions import AllowAny
 
 from ninja_jwt.schema_control import SchemaControl
 from ninja_jwt.settings import api_settings
 
 __all__ = [
@@ -27,27 +26,28 @@
 
 
 class TokenVerificationController(ControllerBase):
     auto_import = False
 
     @http_post(
         "/verify",
-        response={200: Schema},
+        response={200: schema.verify_schema.get_response_schema()},
         url_name="token_verify",
     )
     def verify_token(self, token: schema.verify_schema):
-        return token.to_response_schema()
+        asas = token.to_response_schema()
+        return asas
 
 
 class TokenBlackListController(ControllerBase):
     auto_import = False
 
     @http_post(
         "/blacklist",
-        response={200: Schema},
+        response={200: schema.blacklist_schema.get_response_schema()},
         url_name="token_blacklist",
     )
     def blacklist_token(self, refresh: schema.blacklist_schema):
         return refresh.to_response_schema()
 
 
 class TokenObtainPairController(ControllerBase):
@@ -110,27 +110,27 @@
 
     auto_import = False
 
 
 class AsyncTokenVerificationController(TokenVerificationController):
     @http_post(
         "/verify",
-        response={200: Schema},
+        response={200: schema.verify_schema.get_response_schema()},
         url_name="token_verify",
     )
     async def verify_token(self, token: schema.verify_schema):
         return token.to_response_schema()
 
 
 class AsyncTokenBlackListController(TokenBlackListController):
     auto_import = False
 
     @http_post(
         "/blacklist",
-        response={200: Schema},
+        response={200: schema.blacklist_schema.get_response_schema()},
         url_name="token_blacklist",
     )
     async def blacklist_token(self, refresh: schema.blacklist_schema):
         return refresh.to_response_schema()
 
 
 class AsyncTokenObtainPairController(TokenObtainPairController):
```

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/exceptions.py` & `django_ninja_jwt-5.3.1/ninja_jwt/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/cs/LC_MESSAGES/django.mo` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/cs/LC_MESSAGES/django.po` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/de_CH/LC_MESSAGES/django.mo` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/de_CH/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/de_CH/LC_MESSAGES/django.po` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/de_CH/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/es/LC_MESSAGES/django.mo` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/es/LC_MESSAGES/django.po` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/es_AR/LC_MESSAGES/django.mo` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/es_AR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/es_AR/LC_MESSAGES/django.po` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/es_AR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/es_CL/LC_MESSAGES/django.mo` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/es_CL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/es_CL/LC_MESSAGES/django.po` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/es_CL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/fa_IR/LC_MESSAGES/django.mo` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/fa_IR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/fa_IR/LC_MESSAGES/django.po` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/fa_IR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/fr/LC_MESSAGES/django.mo` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/fr/LC_MESSAGES/django.po` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/id_ID/LC_MESSAGES/django.mo` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/id_ID/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/id_ID/LC_MESSAGES/django.po` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/id_ID/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/it_IT/LC_MESSAGES/django.mo` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/it_IT/LC_MESSAGES/django.po` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/ko_KR/LC_MESSAGES/django.mo` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/ko_KR/LC_MESSAGES/django.po` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/nl_NL/LC_MESSAGES/django.mo` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/nl_NL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/nl_NL/LC_MESSAGES/django.po` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/nl_NL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/pl_PL/LC_MESSAGES/django.mo` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/pl_PL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/pl_PL/LC_MESSAGES/django.po` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/pt_BR/LC_MESSAGES/django.mo` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/pt_BR/LC_MESSAGES/django.po` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/ro/LC_MESSAGES/django.mo` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/ro/LC_MESSAGES/django.po` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/ru_RU/LC_MESSAGES/django.mo` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/ru_RU/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/ru_RU/LC_MESSAGES/django.po` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/ru_RU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/sv/LC_MESSAGES/django.mo` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/sv/LC_MESSAGES/django.po` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/tr/LC_MESSAGES/django.mo` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/tr/LC_MESSAGES/django.po` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/uk_UA/LC_MESSAGES/django.mo` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/uk_UA/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/uk_UA/LC_MESSAGES/django.po` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/uk_UA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/zh_Hans/LC_MESSAGES/django.mo` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/locale/zh_Hans/LC_MESSAGES/django.po` & `django_ninja_jwt-5.3.1/ninja_jwt/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/models.py` & `django_ninja_jwt-5.3.1/ninja_jwt/models.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/routers/obtain.py` & `django_ninja_jwt-5.3.1/ninja_jwt/routers/obtain.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/schema.py` & `django_ninja_jwt-5.3.1/ninja_jwt/schema.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/schema_control.py` & `django_ninja_jwt-5.3.1/ninja_jwt/schema_control.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/settings.py` & `django_ninja_jwt-5.3.1/ninja_jwt/settings.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/admin.py` & `django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/admin.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/migrations/0001_initial.py` & `django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/migrations/0003_auto_20171017_2007.py` & `django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/migrations/0003_auto_20171017_2007.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/migrations/0007_auto_20171017_2214.py` & `django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/migrations/0007_auto_20171017_2214.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/migrations/0008_migrate_to_bigautofield.py` & `django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/migrations/0008_migrate_to_bigautofield.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py` & `django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/migrations/0010_fix_migrate_to_bigautofield.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/migrations/0011_linearizes_history.py` & `django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/migrations/0011_linearizes_history.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/migrations/0012_alter_outstandingtoken_user.py` & `django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/migrations/0012_alter_outstandingtoken_user.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/token_blacklist/models.py` & `django_ninja_jwt-5.3.1/ninja_jwt/token_blacklist/models.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/tokens.py` & `django_ninja_jwt-5.3.1/ninja_jwt/tokens.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/ninja_jwt/utils.py` & `django_ninja_jwt-5.3.1/ninja_jwt/utils.py`

 * *Files identical despite different names*

### Comparing `django_ninja_jwt-5.3.0/pyproject.toml` & `django_ninja_jwt-5.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 [project.optional-dependencies]
 test = [
     "cryptography",
     "pytest",
     "pytest-cov",
     "pytest-django",
     "pytest-asyncio",
-    "ruff ==0.1.9",
+    "ruff ==0.3.4",
     "django-stubs",
     "python-jose==3.3.0",
     "click==8.1.7",
     "freezegun"
 ]
 
 crypto = [
```

### Comparing `django_ninja_jwt-5.3.0/PKG-INFO` & `django_ninja_jwt-5.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ninja-jwt
-Version: 5.3.0
+Version: 5.3.1
 Summary: Django Ninja JWT - JSON Web Token for Django-Ninja
 Author-email: Ezeudoh Tochukwu <tochukwu.ezeudoh@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -46,15 +46,15 @@
 Requires-Dist: mkdocs-markdownextradata-plugin >=0.1.7,<0.3.0 ; extra == "doc"
 Requires-Dist: mkdocstrings ; extra == "doc"
 Requires-Dist: cryptography ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-django ; extra == "test"
 Requires-Dist: pytest-asyncio ; extra == "test"
-Requires-Dist: ruff ==0.1.9 ; extra == "test"
+Requires-Dist: ruff ==0.3.4 ; extra == "test"
 Requires-Dist: django-stubs ; extra == "test"
 Requires-Dist: python-jose==3.3.0 ; extra == "test"
 Requires-Dist: click==8.1.7 ; extra == "test"
 Requires-Dist: freezegun ; extra == "test"
 Project-URL: Documentation, https://github.com/eadwinCode/django-ninja-jwt
 Project-URL: Source, https://github.com/eadwinCode/django-ninja-jwt
 Provides-Extra: crypto
```

