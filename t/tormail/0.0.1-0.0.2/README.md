# Comparing `tmp/tormail-0.0.1.tar.gz` & `tmp/tormail-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tormail-0.0.1.tar", last modified: Sat Apr 27 13:48:39 2024, max compression
+gzip compressed data, was "tormail-0.0.2.tar", last modified: Sat Apr 27 15:50:20 2024, max compression
```

## Comparing `tormail-0.0.1.tar` & `tormail-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 13:48:39.037876 tormail-0.0.1/
--rw-rw-rw-   0        0        0       54 2024-04-27 13:48:39.035875 tormail-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-27 13:44:27.000000 tormail-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 13:48:39.037876 tormail-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      224 2024-04-27 13:47:45.000000 tormail-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 13:48:39.012875 tormail-0.0.1/tormail/
--rw-rw-rw-   0        0        0       23 2024-04-27 13:45:42.000000 tormail-0.0.1/tormail/__init__.py
--rw-rw-rw-   0        0        0       50 2024-04-27 13:45:19.000000 tormail-0.0.1/tormail/main.py
-drwxrwxrwx   0        0        0        0 2024-04-27 13:48:39.033875 tormail-0.0.1/tormail.egg-info/
--rw-rw-rw-   0        0        0       54 2024-04-27 13:48:38.000000 tormail-0.0.1/tormail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2024-04-27 13:48:38.000000 tormail-0.0.1/tormail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 13:48:38.000000 tormail-0.0.1/tormail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-27 13:48:38.000000 tormail-0.0.1/tormail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 15:50:20.557896 tormail-0.0.2/
+-rw-rw-rw-   0        0        0       86 2024-04-27 15:50:20.555896 tormail-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-27 13:44:27.000000 tormail-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 15:50:20.557896 tormail-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      190 2024-04-27 15:49:16.000000 tormail-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 15:50:20.541896 tormail-0.0.2/tormail/
+-rw-rw-rw-   0        0        0       58 2024-04-27 15:46:08.000000 tormail-0.0.2/tormail/__init__.py
+-rw-rw-rw-   0        0        0     1727 2024-04-27 15:35:57.000000 tormail-0.0.2/tormail/listen.py
+-rw-rw-rw-   0        0        0     3373 2024-04-27 15:45:49.000000 tormail-0.0.2/tormail/mail.py
+drwxrwxrwx   0        0        0        0 2024-04-27 15:50:20.553897 tormail-0.0.2/tormail.egg-info/
+-rw-rw-rw-   0        0        0       86 2024-04-27 15:50:20.000000 tormail-0.0.2/tormail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2024-04-27 15:50:20.000000 tormail-0.0.2/tormail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 15:50:20.000000 tormail-0.0.2/tormail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-27 15:50:20.000000 tormail-0.0.2/tormail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-27 15:50:20.000000 tormail-0.0.2/tormail.egg-info/top_level.txt
```

