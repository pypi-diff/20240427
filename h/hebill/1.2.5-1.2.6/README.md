# Comparing `tmp/hebill-1.2.5.tar.gz` & `tmp/hebill-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hebill-1.2.5.tar", last modified: Wed Apr 24 07:30:47 2024, max compression
+gzip compressed data, was "hebill-1.2.6.tar", last modified: Sat Apr 27 00:56:59 2024, max compression
```

## Comparing `hebill-1.2.5.tar` & `hebill-1.2.6.tar`

### file list

```diff
@@ -1,301 +1,306 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.877421 hebill-1.2.5/
--rw-rw-rw-   0        0        0       21 2024-02-17 00:02:01.000000 hebill-1.2.5/LICENSE.rst
--rw-rw-rw-   0        0        0      951 2024-04-24 07:30:47.876411 hebill-1.2.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.670162 hebill-1.2.5/hebill/
--rw-rw-rw-   0        0        0      533 2024-04-22 02:37:16.000000 hebill-1.2.5/hebill/README.MD
--rw-rw-rw-   0        0        0      341 2024-04-24 03:12:13.000000 hebill-1.2.5/hebill/__init__.py
--rw-rw-rw-   0        0        0      267 2024-04-24 07:29:27.000000 hebill-1.2.5/hebill/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.682173 hebill-1.2.5/hebill/dimensions/
--rw-rw-rw-   0        0        0      804 2024-04-22 02:09:35.000000 hebill-1.2.5/hebill/dimensions/README.MD
--rw-rw-rw-   0        0        0       30 2024-04-12 00:54:52.000000 hebill-1.2.5/hebill/dimensions/__init__.py
--rw-rw-rw-   0        0        0     1707 2024-04-12 04:30:14.000000 hebill-1.2.5/hebill/dimensions/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.684695 hebill-1.2.5/hebill/dir/
--rw-rw-rw-   0        0        0       23 2024-04-08 01:00:04.000000 hebill-1.2.5/hebill/dir/__init__.py
--rw-rw-rw-   0        0        0     2224 2024-04-09 00:29:06.000000 hebill-1.2.5/hebill/dir/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.686705 hebill-1.2.5/hebill/excel/
--rw-rw-rw-   0        0        0       25 2024-04-12 01:05:37.000000 hebill-1.2.5/hebill/excel/__init__.py
--rw-rw-rw-   0        0        0      511 2024-04-12 00:54:52.000000 hebill-1.2.5/hebill/excel/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.689704 hebill-1.2.5/hebill/file/
--rw-rw-rw-   0        0        0       24 2024-04-05 01:59:44.000000 hebill-1.2.5/hebill/file/__init__.py
--rw-rw-rw-   0        0        0     1958 2024-04-08 01:57:47.000000 hebill-1.2.5/hebill/file/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.691705 hebill-1.2.5/hebill/html/
--rw-rw-rw-   0        0        0       95 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.693722 hebill-1.2.5/hebill/html/components/
--rw-rw-rw-   0        0        0       60 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/components/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.695211 hebill-1.2.5/hebill/html/components/html/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:11:20.000000 hebill-1.2.5/hebill/html/components/html/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.697220 hebill-1.2.5/hebill/html/components/html/body/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:07.000000 hebill-1.2.5/hebill/html/components/html/body/__init__.py
--rw-rw-rw-   0        0        0      100 2024-04-05 08:05:17.000000 hebill-1.2.5/hebill/html/components/html/body/core.py
--rw-rw-rw-   0        0        0      424 2024-04-05 08:03:11.000000 hebill-1.2.5/hebill/html/components/html/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.698220 hebill-1.2.5/hebill/html/components/html/head/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:02.000000 hebill-1.2.5/hebill/html/components/html/head/__init__.py
--rw-rw-rw-   0        0        0      551 2024-04-05 08:05:17.000000 hebill-1.2.5/hebill/html/components/html/head/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.700618 hebill-1.2.5/hebill/html/components/html/head/title/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.5/hebill/html/components/html/head/title/__init__.py
--rw-rw-rw-   0        0        0      106 2024-04-05 08:05:17.000000 hebill-1.2.5/hebill/html/components/html/head/title/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.701616 hebill-1.2.5/hebill/html/components/html/libraries/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:36.000000 hebill-1.2.5/hebill/html/components/html/libraries/__init__.py
--rw-rw-rw-   0        0        0      367 2024-04-05 08:05:17.000000 hebill-1.2.5/hebill/html/components/html/libraries/libraries.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.703619 hebill-1.2.5/hebill/html/components/table/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:11:14.000000 hebill-1.2.5/hebill/html/components/table/__init__.py
--rw-rw-rw-   0        0        0      673 2024-04-05 08:08:29.000000 hebill-1.2.5/hebill/html/components/table/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.705679 hebill-1.2.5/hebill/html/components/table/tbody/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:13:04.000000 hebill-1.2.5/hebill/html/components/table/tbody/__init__.py
--rw-rw-rw-   0        0        0      565 2024-04-05 08:15:50.000000 hebill-1.2.5/hebill/html/components/table/tbody/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.707290 hebill-1.2.5/hebill/html/components/table/tbody/tr/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.5/hebill/html/components/table/tbody/tr/__init__.py
--rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.2.5/hebill/html/components/table/tbody/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.708902 hebill-1.2.5/hebill/html/components/table/tbody/tr/td/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.5/hebill/html/components/table/tbody/tr/td/__init__.py
--rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.2.5/hebill/html/components/table/tbody/tr/td/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.711097 hebill-1.2.5/hebill/html/components/table/thead/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:57.000000 hebill-1.2.5/hebill/html/components/table/thead/__init__.py
--rw-rw-rw-   0        0        0      565 2024-04-05 08:11:22.000000 hebill-1.2.5/hebill/html/components/table/thead/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.712742 hebill-1.2.5/hebill/html/components/table/thead/tr/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.5/hebill/html/components/table/thead/tr/__init__.py
--rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.2.5/hebill/html/components/table/thead/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.714395 hebill-1.2.5/hebill/html/components/table/thead/tr/th/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.5/hebill/html/components/table/thead/tr/th/__init__.py
--rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.2.5/hebill/html/components/table/thead/tr/th/core.py
--rw-rw-rw-   0        0        0      966 2024-04-05 07:58:22.000000 hebill-1.2.5/hebill/html/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.715989 hebill-1.2.5/hebill/html/nodes/
--rw-rw-rw-   0        0        0      186 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.717904 hebill-1.2.5/hebill/html/nodes/code/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:22.000000 hebill-1.2.5/hebill/html/nodes/code/__init__.py
--rw-rw-rw-   0        0        0      271 2024-04-05 08:03:49.000000 hebill-1.2.5/hebill/html/nodes/code/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.719489 hebill-1.2.5/hebill/html/nodes/comment/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:28.000000 hebill-1.2.5/hebill/html/nodes/comment/__init__.py
--rw-rw-rw-   0        0        0      512 2024-04-05 08:05:37.000000 hebill-1.2.5/hebill/html/nodes/comment/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.721084 hebill-1.2.5/hebill/html/nodes/content/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:33.000000 hebill-1.2.5/hebill/html/nodes/content/__init__.py
--rw-rw-rw-   0        0        0      357 2024-04-05 08:07:50.000000 hebill-1.2.5/hebill/html/nodes/content/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.723216 hebill-1.2.5/hebill/html/nodes/group/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:49.000000 hebill-1.2.5/hebill/html/nodes/group/__init__.py
--rw-rw-rw-   0        0        0      738 2024-04-05 08:07:50.000000 hebill-1.2.5/hebill/html/nodes/group/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.724818 hebill-1.2.5/hebill/html/nodes/group/create/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.5/hebill/html/nodes/group/create/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.726939 hebill-1.2.5/hebill/html/nodes/group/create/components/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:50:31.000000 hebill-1.2.5/hebill/html/nodes/group/create/components/__init__.py
--rw-rw-rw-   0        0        0      178 2024-04-05 07:56:53.000000 hebill-1.2.5/hebill/html/nodes/group/create/components/core.py
--rw-rw-rw-   0        0        0      752 2024-04-05 07:56:53.000000 hebill-1.2.5/hebill/html/nodes/group/create/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.728544 hebill-1.2.5/hebill/html/nodes/group/create/nodes/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:50:37.000000 hebill-1.2.5/hebill/html/nodes/group/create/nodes/__init__.py
--rw-rw-rw-   0        0        0      648 2024-04-05 07:56:53.000000 hebill-1.2.5/hebill/html/nodes/group/create/nodes/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.730688 hebill-1.2.5/hebill/html/nodes/group/create/tags/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:51:13.000000 hebill-1.2.5/hebill/html/nodes/group/create/tags/__init__.py
--rw-rw-rw-   0        0        0     2518 2024-04-05 07:56:53.000000 hebill-1.2.5/hebill/html/nodes/group/create/tags/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.732324 hebill-1.2.5/hebill/html/nodes/node/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:54.000000 hebill-1.2.5/hebill/html/nodes/node/__init__.py
--rw-rw-rw-   0        0        0     1104 2024-04-05 08:07:50.000000 hebill-1.2.5/hebill/html/nodes/node/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.733929 hebill-1.2.5/hebill/html/nodes/tag/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:58.000000 hebill-1.2.5/hebill/html/nodes/tag/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.735541 hebill-1.2.5/hebill/html/nodes/tag/attributes/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:09:38.000000 hebill-1.2.5/hebill/html/nodes/tag/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.737129 hebill-1.2.5/hebill/html/nodes/tag/attributes/classes/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:09:52.000000 hebill-1.2.5/hebill/html/nodes/tag/attributes/classes/__init__.py
--rw-rw-rw-   0        0        0      707 2024-03-09 00:40:03.000000 hebill-1.2.5/hebill/html/nodes/tag/attributes/classes/core.py
--rw-rw-rw-   0        0        0     1524 2024-04-05 08:11:22.000000 hebill-1.2.5/hebill/html/nodes/tag/attributes/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.738716 hebill-1.2.5/hebill/html/nodes/tag/attributes/styles/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:10:01.000000 hebill-1.2.5/hebill/html/nodes/tag/attributes/styles/__init__.py
--rw-rw-rw-   0        0        0      992 2024-03-09 00:40:03.000000 hebill-1.2.5/hebill/html/nodes/tag/attributes/styles/core.py
--rw-rw-rw-   0        0        0     1130 2024-04-05 08:11:22.000000 hebill-1.2.5/hebill/html/nodes/tag/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.739783 hebill-1.2.5/hebill/html/tags/
--rw-rw-rw-   0        0        0      617 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.741377 hebill-1.2.5/hebill/html/tags/a/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:21.000000 hebill-1.2.5/hebill/html/tags/a/__init__.py
--rw-rw-rw-   0        0        0      370 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/a/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.742434 hebill-1.2.5/hebill/html/tags/body/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:29.000000 hebill-1.2.5/hebill/html/tags/body/__init__.py
--rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/body/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.744029 hebill-1.2.5/hebill/html/tags/div/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:35.000000 hebill-1.2.5/hebill/html/tags/div/__init__.py
--rw-rw-rw-   0        0        0      213 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/div/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.745622 hebill-1.2.5/hebill/html/tags/h1/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.5/hebill/html/tags/h1/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/h1/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.746690 hebill-1.2.5/hebill/html/tags/h2/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.5/hebill/html/tags/h2/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/h2/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.747835 hebill-1.2.5/hebill/html/tags/h3/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.5/hebill/html/tags/h3/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/h3/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.749801 hebill-1.2.5/hebill/html/tags/h4/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.5/hebill/html/tags/h4/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/h4/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.751400 hebill-1.2.5/hebill/html/tags/h5/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.5/hebill/html/tags/h5/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/h5/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.753008 hebill-1.2.5/hebill/html/tags/h6/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.5/hebill/html/tags/h6/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/h6/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.754603 hebill-1.2.5/hebill/html/tags/head/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:23.000000 hebill-1.2.5/hebill/html/tags/head/__init__.py
--rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/head/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.756200 hebill-1.2.5/hebill/html/tags/html/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:34.000000 hebill-1.2.5/hebill/html/tags/html/__init__.py
--rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/html/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.758308 hebill-1.2.5/hebill/html/tags/input_text/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:58.000000 hebill-1.2.5/hebill/html/tags/input_text/__init__.py
--rw-rw-rw-   0        0        0      487 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/input_text/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.759891 hebill-1.2.5/hebill/html/tags/link/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:05.000000 hebill-1.2.5/hebill/html/tags/link/__init__.py
--rw-rw-rw-   0        0        0      212 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/link/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.761481 hebill-1.2.5/hebill/html/tags/script/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:27.000000 hebill-1.2.5/hebill/html/tags/script/__init__.py
--rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/script/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.763088 hebill-1.2.5/hebill/html/tags/span/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:32.000000 hebill-1.2.5/hebill/html/tags/span/__init__.py
--rw-rw-rw-   0        0        0      256 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/span/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.764683 hebill-1.2.5/hebill/html/tags/table/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:37.000000 hebill-1.2.5/hebill/html/tags/table/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/table/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.765739 hebill-1.2.5/hebill/html/tags/tbody/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:49.000000 hebill-1.2.5/hebill/html/tags/tbody/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/tbody/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.767847 hebill-1.2.5/hebill/html/tags/td/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:59.000000 hebill-1.2.5/hebill/html/tags/td/__init__.py
--rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/td/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.769431 hebill-1.2.5/hebill/html/tags/th/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:04.000000 hebill-1.2.5/hebill/html/tags/th/__init__.py
--rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/th/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.770923 hebill-1.2.5/hebill/html/tags/thead/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:10.000000 hebill-1.2.5/hebill/html/tags/thead/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/thead/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.772412 hebill-1.2.5/hebill/html/tags/title/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:16.000000 hebill-1.2.5/hebill/html/tags/title/__init__.py
--rw-rw-rw-   0        0        0      376 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/title/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.774933 hebill-1.2.5/hebill/html/tags/tr/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:21.000000 hebill-1.2.5/hebill/html/tags/tr/__init__.py
--rw-rw-rw-   0        0        0      127 2024-04-05 03:31:08.000000 hebill-1.2.5/hebill/html/tags/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.775932 hebill-1.2.5/hebill/image/
--rw-rw-rw-   0        0        0      653 2024-04-09 01:17:04.000000 hebill-1.2.5/hebill/image/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.779077 hebill-1.2.5/hebill/image/png/
--rw-rw-rw-   0        0        0        0 2024-04-05 04:11:13.000000 hebill-1.2.5/hebill/image/png/__init__.py
--rw-rw-rw-   0        0        0    60832 2024-04-12 00:49:55.000000 hebill-1.2.5/hebill/image/png/constants.py
--rw-rw-rw-   0        0        0     5804 2024-04-06 01:07:24.000000 hebill-1.2.5/hebill/image/png/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.781451 hebill-1.2.5/hebill/math/
--rw-rw-rw-   0        0        0       52 2024-04-16 07:28:38.000000 hebill-1.2.5/hebill/math/__init__.py
--rw-rw-rw-   0        0        0      440 2024-04-18 07:17:06.000000 hebill-1.2.5/hebill/math/ring_volume_weight.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.784482 hebill-1.2.5/hebill/mysql/
--rw-rw-rw-   0        0        0       76 2024-04-19 11:39:48.000000 hebill-1.2.5/hebill/mysql/__init__.py
--rw-rw-rw-   0        0        0       79 2024-03-22 03:00:14.000000 hebill-1.2.5/hebill/mysql/constants.py
--rw-rw-rw-   0        0        0     3772 2024-04-05 02:36:51.000000 hebill-1.2.5/hebill/mysql/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.788514 hebill-1.2.5/hebill/mysql/features/
--rw-rw-rw-   0        0        0      146 2024-04-05 03:00:49.000000 hebill-1.2.5/hebill/mysql/features/__init__.py
--rw-rw-rw-   0        0        0      847 2024-04-05 03:00:49.000000 hebill-1.2.5/hebill/mysql/features/table_describe_data.py
--rw-rw-rw-   0        0        0     1028 2024-04-05 03:00:49.000000 hebill-1.2.5/hebill/mysql/features/table_index_data.py
--rw-rw-rw-   0        0        0     1423 2024-04-05 03:00:49.000000 hebill-1.2.5/hebill/mysql/features/table_status_data.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.792526 hebill-1.2.5/hebill/mysql/plugins/
--rw-rw-rw-   0        0        0      134 2024-04-05 03:00:49.000000 hebill-1.2.5/hebill/mysql/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.795199 hebill-1.2.5/hebill/mysql/plugins/columns/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:49:25.000000 hebill-1.2.5/hebill/mysql/plugins/columns/__init__.py
--rw-rw-rw-   0        0        0      583 2024-03-22 12:26:14.000000 hebill-1.2.5/hebill/mysql/plugins/columns/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.796199 hebill-1.2.5/hebill/mysql/plugins/limits/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:49:33.000000 hebill-1.2.5/hebill/mysql/plugins/limits/__init__.py
--rw-rw-rw-   0        0        0      615 2024-03-22 12:26:14.000000 hebill-1.2.5/hebill/mysql/plugins/limits/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.798544 hebill-1.2.5/hebill/mysql/plugins/orders/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:49:41.000000 hebill-1.2.5/hebill/mysql/plugins/orders/__init__.py
--rw-rw-rw-   0        0        0      638 2024-03-22 12:26:14.000000 hebill-1.2.5/hebill/mysql/plugins/orders/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.802001 hebill-1.2.5/hebill/mysql/plugins/wheres/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:35:12.000000 hebill-1.2.5/hebill/mysql/plugins/wheres/__init__.py
--rw-rw-rw-   0        0        0     3174 2024-04-05 02:36:51.000000 hebill-1.2.5/hebill/mysql/plugins/wheres/condition.py
--rw-rw-rw-   0        0        0     2635 2024-03-22 15:25:59.000000 hebill-1.2.5/hebill/mysql/plugins/wheres/conditions.py
--rw-rw-rw-   0        0        0      206 2024-04-05 02:36:51.000000 hebill-1.2.5/hebill/mysql/plugins/wheres/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.803509 hebill-1.2.5/hebill/mysql/table/
--rw-rw-rw-   0        0        0       25 2024-04-05 03:00:49.000000 hebill-1.2.5/hebill/mysql/table/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.804520 hebill-1.2.5/hebill/mysql/table/column/
--rw-rw-rw-   0        0        0        0 2024-03-22 00:18:02.000000 hebill-1.2.5/hebill/mysql/table/column/__init__.py
--rw-rw-rw-   0        0        0       65 2024-04-05 03:00:49.000000 hebill-1.2.5/hebill/mysql/table/column/core.py
--rw-rw-rw-   0        0        0     7332 2024-04-05 03:00:49.000000 hebill-1.2.5/hebill/mysql/table/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.809206 hebill-1.2.5/hebill/mysql/table/data/
--rw-rw-rw-   0        0        0        0 2024-03-22 00:21:17.000000 hebill-1.2.5/hebill/mysql/table/data/__init__.py
--rw-rw-rw-   0        0        0      568 2024-03-22 03:43:57.000000 hebill-1.2.5/hebill/mysql/table/data/core.py
--rw-rw-rw-   0        0        0     1710 2024-03-22 11:35:59.000000 hebill-1.2.5/hebill/mysql/table/data/drop.py
--rw-rw-rw-   0        0        0     1564 2024-02-27 01:58:04.000000 hebill-1.2.5/hebill/mysql/table/data/insert.py
--rw-rw-rw-   0        0        0     2041 2024-03-22 11:35:59.000000 hebill-1.2.5/hebill/mysql/table/data/search.py
--rw-rw-rw-   0        0        0      722 2024-04-05 03:00:49.000000 hebill-1.2.5/hebill/mysql/table/data/update.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.812218 hebill-1.2.5/hebill/numeric/
--rw-rw-rw-   0        0        0       27 2024-04-09 02:38:00.000000 hebill-1.2.5/hebill/numeric/__init__.py
--rw-rw-rw-   0        0        0     1127 2024-04-10 07:14:07.000000 hebill-1.2.5/hebill/numeric/constants.py
--rw-rw-rw-   0        0        0    14209 2024-04-11 00:11:08.000000 hebill-1.2.5/hebill/numeric/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.814216 hebill-1.2.5/hebill/pdf/
--rw-rw-rw-   0        0        0      465 2024-04-19 11:23:54.000000 hebill-1.2.5/hebill/pdf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.815216 hebill-1.2.5/hebill/pdf/component/
--rw-rw-rw-   0        0        0        0 2024-03-19 08:57:35.000000 hebill-1.2.5/hebill/pdf/component/__init__.py
--rw-rw-rw-   0        0        0     2485 2024-04-09 02:04:40.000000 hebill-1.2.5/hebill/pdf/component/core.py
--rw-rw-rw-   0        0        0     1121 2024-03-20 08:39:59.000000 hebill-1.2.5/hebill/pdf/constants.py
--rw-rw-rw-   0        0        0     8799 2024-04-19 11:39:48.000000 hebill-1.2.5/hebill/pdf/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.819725 hebill-1.2.5/hebill/pdf/features/
--rw-rw-rw-   0        0        0        0 2024-04-09 01:59:41.000000 hebill-1.2.5/hebill/pdf/features/__init__.py
--rw-rw-rw-   0        0        0      441 2024-04-09 02:04:40.000000 hebill-1.2.5/hebill/pdf/features/configs.py
--rw-rw-rw-   0        0        0     1419 2024-04-09 02:04:40.000000 hebill-1.2.5/hebill/pdf/features/document_configs.py
--rw-rw-rw-   0        0        0     1382 2024-04-09 02:04:40.000000 hebill-1.2.5/hebill/pdf/features/page_configs.py
--rw-rw-rw-   0        0        0     4891 2024-04-09 02:04:40.000000 hebill-1.2.5/hebill/pdf/features/styles.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.821873 hebill-1.2.5/hebill/pdf/library/
--rw-rw-rw-   0        0        0        0 2024-03-19 01:10:28.000000 hebill-1.2.5/hebill/pdf/library/__init__.py
--rw-rw-rw-   0        0        0     8548 2024-03-19 00:59:10.000000 hebill-1.2.5/hebill/pdf/library/configs_selector_color.py
--rw-rw-rw-   0        0        0      826 2024-03-19 16:42:53.000000 hebill-1.2.5/hebill/pdf/library/configs_selector_font.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.843924 hebill-1.2.5/hebill/pdf/page/
--rw-rw-rw-   0        0        0        0 2024-03-19 01:10:08.000000 hebill-1.2.5/hebill/pdf/page/__init__.py
--rw-rw-rw-   0        0        0      886 2024-04-09 02:04:40.000000 hebill-1.2.5/hebill/pdf/page/_draw_.py
--rw-rw-rw-   0        0        0      382 2024-03-20 07:59:42.000000 hebill-1.2.5/hebill/pdf/page/_draw_line.py
--rw-rw-rw-   0        0        0      462 2024-03-20 07:59:42.000000 hebill-1.2.5/hebill/pdf/page/_draw_shape.py
--rw-rw-rw-   0        0        0      447 2024-03-20 07:59:42.000000 hebill-1.2.5/hebill/pdf/page/_draw_text.py
--rw-rw-rw-   0        0        0     3004 2024-04-09 02:04:40.000000 hebill-1.2.5/hebill/pdf/page/core.py
--rw-rw-rw-   0        0        0      413 2024-03-20 00:39:33.000000 hebill-1.2.5/hebill/pdf/page/draw_circle.py
--rw-rw-rw-   0        0        0      465 2024-03-20 00:39:33.000000 hebill-1.2.5/hebill/pdf/page/draw_ellipse.py
--rw-rw-rw-   0        0        0     1047 2024-03-20 08:33:48.000000 hebill-1.2.5/hebill/pdf/page/draw_grids.py
--rw-rw-rw-   0        0        0      457 2024-03-20 00:39:33.000000 hebill-1.2.5/hebill/pdf/page/draw_line.py
--rw-rw-rw-   0        0        0     1528 2024-03-20 07:59:42.000000 hebill-1.2.5/hebill/pdf/page/draw_path.py
--rw-rw-rw-   0        0        0      726 2024-03-20 04:01:39.000000 hebill-1.2.5/hebill/pdf/page/draw_rect.py
--rw-rw-rw-   0        0        0      668 2024-03-21 15:41:19.000000 hebill-1.2.5/hebill/pdf/page/draw_string.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.846923 hebill-1.2.5/hebill/pypi/
--rw-rw-rw-   0        0        0      526 2024-04-24 07:29:27.000000 hebill-1.2.5/hebill/pypi/README.MD
--rw-rw-rw-   0        0        0       24 2024-04-05 13:22:37.000000 hebill-1.2.5/hebill/pypi/__init__.py
--rw-rw-rw-   0        0        0     9086 2024-04-24 07:30:45.000000 hebill-1.2.5/hebill/pypi/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.848923 hebill-1.2.5/hebill/string/
--rw-rw-rw-   0        0        0       26 2024-04-10 02:30:43.000000 hebill-1.2.5/hebill/string/__init__.py
--rw-rw-rw-   0        0        0     1571 2024-04-19 11:39:48.000000 hebill-1.2.5/hebill/string/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.851431 hebill-1.2.5/hebill/sys/
--rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.2.5/hebill/sys/__init__.py
--rw-rw-rw-   0        0        0      626 2024-04-19 14:39:39.000000 hebill-1.2.5/hebill/sys/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.854445 hebill-1.2.5/hebill/url/
--rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.2.5/hebill/url/__init__.py
--rw-rw-rw-   0        0        0      317 2024-04-05 01:34:58.000000 hebill-1.2.5/hebill/url/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.857975 hebill-1.2.5/hebill/webserver/
--rw-rw-rw-   0        0        0      186 2024-04-22 02:16:02.000000 hebill-1.2.5/hebill/webserver/README.MD
--rw-rw-rw-   0        0        0       57 2024-04-19 11:39:48.000000 hebill-1.2.5/hebill/webserver/__init__.py
--rw-rw-rw-   0        0        0     1508 2024-04-19 11:41:02.000000 hebill-1.2.5/hebill/webserver/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.859976 hebill-1.2.5/hebill/webserver/features/
--rw-rw-rw-   0        0        0        0 2024-04-03 02:05:18.000000 hebill-1.2.5/hebill/webserver/features/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.860976 hebill-1.2.5/hebill/webserver/features/client/
--rw-rw-rw-   0        0        0        0 2024-04-03 02:05:55.000000 hebill-1.2.5/hebill/webserver/features/client/__init__.py
--rw-rw-rw-   0        0        0      143 2024-04-03 02:21:39.000000 hebill-1.2.5/hebill/webserver/features/client/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.862975 hebill-1.2.5/hebill/webserver/features/request/
--rw-rw-rw-   0        0        0        0 2024-04-03 02:09:21.000000 hebill-1.2.5/hebill/webserver/features/request/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.863974 hebill-1.2.5/hebill/webserver/features/request/cookie/
--rw-rw-rw-   0        0        0        0 2024-04-03 02:27:33.000000 hebill-1.2.5/hebill/webserver/features/request/cookie/__init__.py
--rw-rw-rw-   0        0        0      205 2024-04-03 03:01:28.000000 hebill-1.2.5/hebill/webserver/features/request/cookie/core.py
--rw-rw-rw-   0        0        0      587 2024-04-03 07:11:58.000000 hebill-1.2.5/hebill/webserver/features/request/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.865976 hebill-1.2.5/hebill/webserver/features/request/get/
--rw-rw-rw-   0        0        0        0 2024-04-03 02:09:55.000000 hebill-1.2.5/hebill/webserver/features/request/get/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-03 08:50:01.000000 hebill-1.2.5/hebill/webserver/features/request/get/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.868976 hebill-1.2.5/hebill/webserver/features/request/headers/
--rw-rw-rw-   0        0        0        0 2024-04-03 07:07:38.000000 hebill-1.2.5/hebill/webserver/features/request/headers/__init__.py
--rw-rw-rw-   0        0        0      219 2024-04-03 08:50:01.000000 hebill-1.2.5/hebill/webserver/features/request/headers/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.870705 hebill-1.2.5/hebill/webserver/features/request/post/
--rw-rw-rw-   0        0        0        0 2024-04-03 02:09:59.000000 hebill-1.2.5/hebill/webserver/features/request/post/__init__.py
--rw-rw-rw-   0        0        0      152 2024-04-03 02:21:39.000000 hebill-1.2.5/hebill/webserver/features/request/post/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.874241 hebill-1.2.5/hebill/webserver/features/website/
--rw-rw-rw-   0        0        0        0 2024-04-03 02:05:11.000000 hebill-1.2.5/hebill/webserver/features/website/__init__.py
--rw-rw-rw-   0        0        0      479 2024-04-03 03:01:28.000000 hebill-1.2.5/hebill/webserver/features/website/core.py
--rw-rw-rw-   0        0        0     2503 2024-04-19 11:39:48.000000 hebill-1.2.5/hebill/webserver/handle.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:30:47.875241 hebill-1.2.5/hebill.egg-info/
--rw-rw-rw-   0        0        0      951 2024-04-24 07:30:47.000000 hebill-1.2.5/hebill.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7186 2024-04-24 07:30:47.000000 hebill-1.2.5/hebill.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 07:30:47.000000 hebill-1.2.5/hebill.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2024-04-24 07:30:47.000000 hebill-1.2.5/hebill.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-24 07:30:47.000000 hebill-1.2.5/hebill.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      654 2024-04-24 07:30:46.000000 hebill-1.2.5/pack_upload_setup.py
--rw-rw-rw-   0        0        0       42 2024-04-24 07:30:47.877421 hebill-1.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.785862 hebill-1.2.6/
+-rw-rw-rw-   0        0        0       21 2024-02-17 00:02:01.000000 hebill-1.2.6/LICENSE.rst
+-rw-rw-rw-   0        0        0      951 2024-04-27 00:56:59.783861 hebill-1.2.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.424413 hebill-1.2.6/hebill/
+-rw-rw-rw-   0        0        0      533 2024-04-22 02:37:16.000000 hebill-1.2.6/hebill/README.MD
+-rw-rw-rw-   0        0        0      341 2024-04-24 03:12:13.000000 hebill-1.2.6/hebill/__init__.py
+-rw-rw-rw-   0        0        0      267 2024-04-27 00:56:57.000000 hebill-1.2.6/hebill/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.433933 hebill-1.2.6/hebill/dimensions/
+-rw-rw-rw-   0        0        0      804 2024-04-22 02:09:35.000000 hebill-1.2.6/hebill/dimensions/README.MD
+-rw-rw-rw-   0        0        0       30 2024-04-12 00:54:52.000000 hebill-1.2.6/hebill/dimensions/__init__.py
+-rw-rw-rw-   0        0        0     1707 2024-04-12 04:30:14.000000 hebill-1.2.6/hebill/dimensions/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.436538 hebill-1.2.6/hebill/dir/
+-rw-rw-rw-   0        0        0       23 2024-04-08 01:00:04.000000 hebill-1.2.6/hebill/dir/__init__.py
+-rw-rw-rw-   0        0        0     2224 2024-04-09 00:29:06.000000 hebill-1.2.6/hebill/dir/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.439540 hebill-1.2.6/hebill/excel/
+-rw-rw-rw-   0        0        0       25 2024-04-12 01:05:37.000000 hebill-1.2.6/hebill/excel/__init__.py
+-rw-rw-rw-   0        0        0      511 2024-04-12 00:54:52.000000 hebill-1.2.6/hebill/excel/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.441538 hebill-1.2.6/hebill/file/
+-rw-rw-rw-   0        0        0       24 2024-04-05 01:59:44.000000 hebill-1.2.6/hebill/file/__init__.py
+-rw-rw-rw-   0        0        0     1958 2024-04-08 01:57:47.000000 hebill-1.2.6/hebill/file/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.444047 hebill-1.2.6/hebill/html/
+-rw-rw-rw-   0        0        0       95 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.446054 hebill-1.2.6/hebill/html/components/
+-rw-rw-rw-   0        0        0       60 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/components/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.456290 hebill-1.2.6/hebill/html/components/html/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:11:20.000000 hebill-1.2.6/hebill/html/components/html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.460240 hebill-1.2.6/hebill/html/components/html/body/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:07.000000 hebill-1.2.6/hebill/html/components/html/body/__init__.py
+-rw-rw-rw-   0        0        0      100 2024-04-05 08:05:17.000000 hebill-1.2.6/hebill/html/components/html/body/core.py
+-rw-rw-rw-   0        0        0      424 2024-04-05 08:03:11.000000 hebill-1.2.6/hebill/html/components/html/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.462683 hebill-1.2.6/hebill/html/components/html/head/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:02.000000 hebill-1.2.6/hebill/html/components/html/head/__init__.py
+-rw-rw-rw-   0        0        0      551 2024-04-05 08:05:17.000000 hebill-1.2.6/hebill/html/components/html/head/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.465818 hebill-1.2.6/hebill/html/components/html/head/title/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.6/hebill/html/components/html/head/title/__init__.py
+-rw-rw-rw-   0        0        0      106 2024-04-05 08:05:17.000000 hebill-1.2.6/hebill/html/components/html/head/title/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.468069 hebill-1.2.6/hebill/html/components/html/libraries/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:36.000000 hebill-1.2.6/hebill/html/components/html/libraries/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-04-05 08:05:17.000000 hebill-1.2.6/hebill/html/components/html/libraries/libraries.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.470060 hebill-1.2.6/hebill/html/components/table/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:11:14.000000 hebill-1.2.6/hebill/html/components/table/__init__.py
+-rw-rw-rw-   0        0        0      673 2024-04-05 08:08:29.000000 hebill-1.2.6/hebill/html/components/table/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.472378 hebill-1.2.6/hebill/html/components/table/tbody/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:13:04.000000 hebill-1.2.6/hebill/html/components/table/tbody/__init__.py
+-rw-rw-rw-   0        0        0      565 2024-04-05 08:15:50.000000 hebill-1.2.6/hebill/html/components/table/tbody/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.475390 hebill-1.2.6/hebill/html/components/table/tbody/tr/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.6/hebill/html/components/table/tbody/tr/__init__.py
+-rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.2.6/hebill/html/components/table/tbody/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.477830 hebill-1.2.6/hebill/html/components/table/tbody/tr/td/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.6/hebill/html/components/table/tbody/tr/td/__init__.py
+-rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.2.6/hebill/html/components/table/tbody/tr/td/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.479869 hebill-1.2.6/hebill/html/components/table/thead/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:57.000000 hebill-1.2.6/hebill/html/components/table/thead/__init__.py
+-rw-rw-rw-   0        0        0      565 2024-04-05 08:11:22.000000 hebill-1.2.6/hebill/html/components/table/thead/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.482186 hebill-1.2.6/hebill/html/components/table/thead/tr/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.6/hebill/html/components/table/thead/tr/__init__.py
+-rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.2.6/hebill/html/components/table/thead/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.484995 hebill-1.2.6/hebill/html/components/table/thead/tr/th/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.6/hebill/html/components/table/thead/tr/th/__init__.py
+-rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.2.6/hebill/html/components/table/thead/tr/th/core.py
+-rw-rw-rw-   0        0        0      966 2024-04-05 07:58:22.000000 hebill-1.2.6/hebill/html/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.486511 hebill-1.2.6/hebill/html/nodes/
+-rw-rw-rw-   0        0        0      186 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.488511 hebill-1.2.6/hebill/html/nodes/code/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:22.000000 hebill-1.2.6/hebill/html/nodes/code/__init__.py
+-rw-rw-rw-   0        0        0      271 2024-04-05 08:03:49.000000 hebill-1.2.6/hebill/html/nodes/code/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.491021 hebill-1.2.6/hebill/html/nodes/comment/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:28.000000 hebill-1.2.6/hebill/html/nodes/comment/__init__.py
+-rw-rw-rw-   0        0        0      512 2024-04-05 08:05:37.000000 hebill-1.2.6/hebill/html/nodes/comment/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.494035 hebill-1.2.6/hebill/html/nodes/content/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:33.000000 hebill-1.2.6/hebill/html/nodes/content/__init__.py
+-rw-rw-rw-   0        0        0      357 2024-04-05 08:07:50.000000 hebill-1.2.6/hebill/html/nodes/content/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.497968 hebill-1.2.6/hebill/html/nodes/group/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:49.000000 hebill-1.2.6/hebill/html/nodes/group/__init__.py
+-rw-rw-rw-   0        0        0      738 2024-04-05 08:07:50.000000 hebill-1.2.6/hebill/html/nodes/group/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.500481 hebill-1.2.6/hebill/html/nodes/group/create/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.6/hebill/html/nodes/group/create/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.505026 hebill-1.2.6/hebill/html/nodes/group/create/components/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:50:31.000000 hebill-1.2.6/hebill/html/nodes/group/create/components/__init__.py
+-rw-rw-rw-   0        0        0      178 2024-04-05 07:56:53.000000 hebill-1.2.6/hebill/html/nodes/group/create/components/core.py
+-rw-rw-rw-   0        0        0      752 2024-04-05 07:56:53.000000 hebill-1.2.6/hebill/html/nodes/group/create/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.508524 hebill-1.2.6/hebill/html/nodes/group/create/nodes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:50:37.000000 hebill-1.2.6/hebill/html/nodes/group/create/nodes/__init__.py
+-rw-rw-rw-   0        0        0      648 2024-04-05 07:56:53.000000 hebill-1.2.6/hebill/html/nodes/group/create/nodes/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.510844 hebill-1.2.6/hebill/html/nodes/group/create/tags/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:51:13.000000 hebill-1.2.6/hebill/html/nodes/group/create/tags/__init__.py
+-rw-rw-rw-   0        0        0     2518 2024-04-05 07:56:53.000000 hebill-1.2.6/hebill/html/nodes/group/create/tags/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.513379 hebill-1.2.6/hebill/html/nodes/node/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:54.000000 hebill-1.2.6/hebill/html/nodes/node/__init__.py
+-rw-rw-rw-   0        0        0     1104 2024-04-05 08:07:50.000000 hebill-1.2.6/hebill/html/nodes/node/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.516757 hebill-1.2.6/hebill/html/nodes/tag/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:58.000000 hebill-1.2.6/hebill/html/nodes/tag/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.519647 hebill-1.2.6/hebill/html/nodes/tag/attributes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:09:38.000000 hebill-1.2.6/hebill/html/nodes/tag/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.522668 hebill-1.2.6/hebill/html/nodes/tag/attributes/classes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:09:52.000000 hebill-1.2.6/hebill/html/nodes/tag/attributes/classes/__init__.py
+-rw-rw-rw-   0        0        0      707 2024-03-09 00:40:03.000000 hebill-1.2.6/hebill/html/nodes/tag/attributes/classes/core.py
+-rw-rw-rw-   0        0        0     1524 2024-04-05 08:11:22.000000 hebill-1.2.6/hebill/html/nodes/tag/attributes/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.525678 hebill-1.2.6/hebill/html/nodes/tag/attributes/styles/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:10:01.000000 hebill-1.2.6/hebill/html/nodes/tag/attributes/styles/__init__.py
+-rw-rw-rw-   0        0        0      992 2024-03-09 00:40:03.000000 hebill-1.2.6/hebill/html/nodes/tag/attributes/styles/core.py
+-rw-rw-rw-   0        0        0     1130 2024-04-05 08:11:22.000000 hebill-1.2.6/hebill/html/nodes/tag/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.527717 hebill-1.2.6/hebill/html/tags/
+-rw-rw-rw-   0        0        0      617 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.530367 hebill-1.2.6/hebill/html/tags/a/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:21.000000 hebill-1.2.6/hebill/html/tags/a/__init__.py
+-rw-rw-rw-   0        0        0      370 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/a/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.532396 hebill-1.2.6/hebill/html/tags/body/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:29.000000 hebill-1.2.6/hebill/html/tags/body/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/body/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.534396 hebill-1.2.6/hebill/html/tags/div/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:35.000000 hebill-1.2.6/hebill/html/tags/div/__init__.py
+-rw-rw-rw-   0        0        0      213 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/div/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.537216 hebill-1.2.6/hebill/html/tags/h1/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.6/hebill/html/tags/h1/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/h1/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.539270 hebill-1.2.6/hebill/html/tags/h2/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.6/hebill/html/tags/h2/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/h2/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.541266 hebill-1.2.6/hebill/html/tags/h3/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.6/hebill/html/tags/h3/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/h3/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.543265 hebill-1.2.6/hebill/html/tags/h4/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.6/hebill/html/tags/h4/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/h4/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.545269 hebill-1.2.6/hebill/html/tags/h5/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.6/hebill/html/tags/h5/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/h5/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.547269 hebill-1.2.6/hebill/html/tags/h6/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.6/hebill/html/tags/h6/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/h6/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.549764 hebill-1.2.6/hebill/html/tags/head/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:23.000000 hebill-1.2.6/hebill/html/tags/head/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/head/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.552015 hebill-1.2.6/hebill/html/tags/html/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:34.000000 hebill-1.2.6/hebill/html/tags/html/__init__.py
+-rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/html/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.554170 hebill-1.2.6/hebill/html/tags/input_text/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:58.000000 hebill-1.2.6/hebill/html/tags/input_text/__init__.py
+-rw-rw-rw-   0        0        0      487 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/input_text/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.555219 hebill-1.2.6/hebill/html/tags/link/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:05.000000 hebill-1.2.6/hebill/html/tags/link/__init__.py
+-rw-rw-rw-   0        0        0      212 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/link/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.557232 hebill-1.2.6/hebill/html/tags/script/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:27.000000 hebill-1.2.6/hebill/html/tags/script/__init__.py
+-rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/script/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.562280 hebill-1.2.6/hebill/html/tags/span/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:32.000000 hebill-1.2.6/hebill/html/tags/span/__init__.py
+-rw-rw-rw-   0        0        0      256 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/span/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.566632 hebill-1.2.6/hebill/html/tags/table/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:37.000000 hebill-1.2.6/hebill/html/tags/table/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/table/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.572646 hebill-1.2.6/hebill/html/tags/tbody/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:49.000000 hebill-1.2.6/hebill/html/tags/tbody/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/tbody/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.579640 hebill-1.2.6/hebill/html/tags/td/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:59.000000 hebill-1.2.6/hebill/html/tags/td/__init__.py
+-rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/td/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.583156 hebill-1.2.6/hebill/html/tags/th/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:04.000000 hebill-1.2.6/hebill/html/tags/th/__init__.py
+-rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/th/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.593778 hebill-1.2.6/hebill/html/tags/thead/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:10.000000 hebill-1.2.6/hebill/html/tags/thead/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/thead/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.599588 hebill-1.2.6/hebill/html/tags/title/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:16.000000 hebill-1.2.6/hebill/html/tags/title/__init__.py
+-rw-rw-rw-   0        0        0      376 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/title/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.601636 hebill-1.2.6/hebill/html/tags/tr/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:21.000000 hebill-1.2.6/hebill/html/tags/tr/__init__.py
+-rw-rw-rw-   0        0        0      127 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.603099 hebill-1.2.6/hebill/image/
+-rw-rw-rw-   0        0        0      653 2024-04-09 01:17:04.000000 hebill-1.2.6/hebill/image/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.608112 hebill-1.2.6/hebill/image/png/
+-rw-rw-rw-   0        0        0        0 2024-04-05 04:11:13.000000 hebill-1.2.6/hebill/image/png/__init__.py
+-rw-rw-rw-   0        0        0    60832 2024-04-12 00:49:55.000000 hebill-1.2.6/hebill/image/png/constants.py
+-rw-rw-rw-   0        0        0     5804 2024-04-06 01:07:24.000000 hebill-1.2.6/hebill/image/png/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.611576 hebill-1.2.6/hebill/math/
+-rw-rw-rw-   0        0        0       52 2024-04-16 07:28:38.000000 hebill-1.2.6/hebill/math/__init__.py
+-rw-rw-rw-   0        0        0      440 2024-04-18 07:17:06.000000 hebill-1.2.6/hebill/math/ring_volume_weight.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.619979 hebill-1.2.6/hebill/mysql/
+-rw-rw-rw-   0        0        0       76 2024-04-19 11:39:48.000000 hebill-1.2.6/hebill/mysql/__init__.py
+-rw-rw-rw-   0        0        0       79 2024-03-22 03:00:14.000000 hebill-1.2.6/hebill/mysql/constants.py
+-rw-rw-rw-   0        0        0     3772 2024-04-05 02:36:51.000000 hebill-1.2.6/hebill/mysql/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.627977 hebill-1.2.6/hebill/mysql/features/
+-rw-rw-rw-   0        0        0      146 2024-04-05 03:00:49.000000 hebill-1.2.6/hebill/mysql/features/__init__.py
+-rw-rw-rw-   0        0        0      847 2024-04-05 03:00:49.000000 hebill-1.2.6/hebill/mysql/features/table_describe_data.py
+-rw-rw-rw-   0        0        0     1028 2024-04-05 03:00:49.000000 hebill-1.2.6/hebill/mysql/features/table_index_data.py
+-rw-rw-rw-   0        0        0     1423 2024-04-05 03:00:49.000000 hebill-1.2.6/hebill/mysql/features/table_status_data.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.628976 hebill-1.2.6/hebill/mysql/plugins/
+-rw-rw-rw-   0        0        0      134 2024-04-05 03:00:49.000000 hebill-1.2.6/hebill/mysql/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.644510 hebill-1.2.6/hebill/mysql/plugins/columns/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:25.000000 hebill-1.2.6/hebill/mysql/plugins/columns/__init__.py
+-rw-rw-rw-   0        0        0      583 2024-03-22 12:26:14.000000 hebill-1.2.6/hebill/mysql/plugins/columns/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.647013 hebill-1.2.6/hebill/mysql/plugins/limits/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:33.000000 hebill-1.2.6/hebill/mysql/plugins/limits/__init__.py
+-rw-rw-rw-   0        0        0      615 2024-03-22 12:26:14.000000 hebill-1.2.6/hebill/mysql/plugins/limits/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.650532 hebill-1.2.6/hebill/mysql/plugins/orders/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:41.000000 hebill-1.2.6/hebill/mysql/plugins/orders/__init__.py
+-rw-rw-rw-   0        0        0      638 2024-03-22 12:26:14.000000 hebill-1.2.6/hebill/mysql/plugins/orders/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.655540 hebill-1.2.6/hebill/mysql/plugins/wheres/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:35:12.000000 hebill-1.2.6/hebill/mysql/plugins/wheres/__init__.py
+-rw-rw-rw-   0        0        0     3174 2024-04-05 02:36:51.000000 hebill-1.2.6/hebill/mysql/plugins/wheres/condition.py
+-rw-rw-rw-   0        0        0     2635 2024-03-22 15:25:59.000000 hebill-1.2.6/hebill/mysql/plugins/wheres/conditions.py
+-rw-rw-rw-   0        0        0      206 2024-04-05 02:36:51.000000 hebill-1.2.6/hebill/mysql/plugins/wheres/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.658046 hebill-1.2.6/hebill/mysql/table/
+-rw-rw-rw-   0        0        0       25 2024-04-05 03:00:49.000000 hebill-1.2.6/hebill/mysql/table/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.661053 hebill-1.2.6/hebill/mysql/table/column/
+-rw-rw-rw-   0        0        0        0 2024-03-22 00:18:02.000000 hebill-1.2.6/hebill/mysql/table/column/__init__.py
+-rw-rw-rw-   0        0        0       65 2024-04-05 03:00:49.000000 hebill-1.2.6/hebill/mysql/table/column/core.py
+-rw-rw-rw-   0        0        0     7332 2024-04-05 03:00:49.000000 hebill-1.2.6/hebill/mysql/table/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.670854 hebill-1.2.6/hebill/mysql/table/data/
+-rw-rw-rw-   0        0        0        0 2024-03-22 00:21:17.000000 hebill-1.2.6/hebill/mysql/table/data/__init__.py
+-rw-rw-rw-   0        0        0      568 2024-03-22 03:43:57.000000 hebill-1.2.6/hebill/mysql/table/data/core.py
+-rw-rw-rw-   0        0        0     1710 2024-03-22 11:35:59.000000 hebill-1.2.6/hebill/mysql/table/data/drop.py
+-rw-rw-rw-   0        0        0     1564 2024-02-27 01:58:04.000000 hebill-1.2.6/hebill/mysql/table/data/insert.py
+-rw-rw-rw-   0        0        0     2041 2024-03-22 11:35:59.000000 hebill-1.2.6/hebill/mysql/table/data/search.py
+-rw-rw-rw-   0        0        0      722 2024-04-05 03:00:49.000000 hebill-1.2.6/hebill/mysql/table/data/update.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.676207 hebill-1.2.6/hebill/numeric/
+-rw-rw-rw-   0        0        0       27 2024-04-09 02:38:00.000000 hebill-1.2.6/hebill/numeric/__init__.py
+-rw-rw-rw-   0        0        0     1127 2024-04-10 07:14:07.000000 hebill-1.2.6/hebill/numeric/constants.py
+-rw-rw-rw-   0        0        0    14209 2024-04-11 00:11:08.000000 hebill-1.2.6/hebill/numeric/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.682868 hebill-1.2.6/hebill/pdf/
+-rw-rw-rw-   0        0        0      465 2024-04-19 11:23:54.000000 hebill-1.2.6/hebill/pdf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.685375 hebill-1.2.6/hebill/pdf/component/
+-rw-rw-rw-   0        0        0        0 2024-03-19 08:57:35.000000 hebill-1.2.6/hebill/pdf/component/__init__.py
+-rw-rw-rw-   0        0        0     2485 2024-04-09 02:04:40.000000 hebill-1.2.6/hebill/pdf/component/core.py
+-rw-rw-rw-   0        0        0     1121 2024-03-20 08:39:59.000000 hebill-1.2.6/hebill/pdf/constants.py
+-rw-rw-rw-   0        0        0     8799 2024-04-19 11:39:48.000000 hebill-1.2.6/hebill/pdf/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.693393 hebill-1.2.6/hebill/pdf/features/
+-rw-rw-rw-   0        0        0        0 2024-04-09 01:59:41.000000 hebill-1.2.6/hebill/pdf/features/__init__.py
+-rw-rw-rw-   0        0        0      441 2024-04-09 02:04:40.000000 hebill-1.2.6/hebill/pdf/features/configs.py
+-rw-rw-rw-   0        0        0     1419 2024-04-09 02:04:40.000000 hebill-1.2.6/hebill/pdf/features/document_configs.py
+-rw-rw-rw-   0        0        0     1382 2024-04-09 02:04:40.000000 hebill-1.2.6/hebill/pdf/features/page_configs.py
+-rw-rw-rw-   0        0        0     4891 2024-04-09 02:04:40.000000 hebill-1.2.6/hebill/pdf/features/styles.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.699392 hebill-1.2.6/hebill/pdf/library/
+-rw-rw-rw-   0        0        0        0 2024-03-19 01:10:28.000000 hebill-1.2.6/hebill/pdf/library/__init__.py
+-rw-rw-rw-   0        0        0     8548 2024-03-19 00:59:10.000000 hebill-1.2.6/hebill/pdf/library/configs_selector_color.py
+-rw-rw-rw-   0        0        0      826 2024-03-19 16:42:53.000000 hebill-1.2.6/hebill/pdf/library/configs_selector_font.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.723961 hebill-1.2.6/hebill/pdf/page/
+-rw-rw-rw-   0        0        0        0 2024-03-19 01:10:08.000000 hebill-1.2.6/hebill/pdf/page/__init__.py
+-rw-rw-rw-   0        0        0      886 2024-04-09 02:04:40.000000 hebill-1.2.6/hebill/pdf/page/_draw_.py
+-rw-rw-rw-   0        0        0      382 2024-03-20 07:59:42.000000 hebill-1.2.6/hebill/pdf/page/_draw_line.py
+-rw-rw-rw-   0        0        0      462 2024-03-20 07:59:42.000000 hebill-1.2.6/hebill/pdf/page/_draw_shape.py
+-rw-rw-rw-   0        0        0      447 2024-03-20 07:59:42.000000 hebill-1.2.6/hebill/pdf/page/_draw_text.py
+-rw-rw-rw-   0        0        0     3004 2024-04-09 02:04:40.000000 hebill-1.2.6/hebill/pdf/page/core.py
+-rw-rw-rw-   0        0        0      413 2024-03-20 00:39:33.000000 hebill-1.2.6/hebill/pdf/page/draw_circle.py
+-rw-rw-rw-   0        0        0      465 2024-03-20 00:39:33.000000 hebill-1.2.6/hebill/pdf/page/draw_ellipse.py
+-rw-rw-rw-   0        0        0     1047 2024-03-20 08:33:48.000000 hebill-1.2.6/hebill/pdf/page/draw_grids.py
+-rw-rw-rw-   0        0        0      457 2024-03-20 00:39:33.000000 hebill-1.2.6/hebill/pdf/page/draw_line.py
+-rw-rw-rw-   0        0        0     1528 2024-03-20 07:59:42.000000 hebill-1.2.6/hebill/pdf/page/draw_path.py
+-rw-rw-rw-   0        0        0      726 2024-03-20 04:01:39.000000 hebill-1.2.6/hebill/pdf/page/draw_rect.py
+-rw-rw-rw-   0        0        0      668 2024-03-21 15:41:19.000000 hebill-1.2.6/hebill/pdf/page/draw_string.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.729960 hebill-1.2.6/hebill/pypi/
+-rw-rw-rw-   0        0        0      526 2024-04-24 07:29:27.000000 hebill-1.2.6/hebill/pypi/README.MD
+-rw-rw-rw-   0        0        0       24 2024-04-05 13:22:37.000000 hebill-1.2.6/hebill/pypi/__init__.py
+-rw-rw-rw-   0        0        0     9132 2024-04-24 07:33:05.000000 hebill-1.2.6/hebill/pypi/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.734953 hebill-1.2.6/hebill/string/
+-rw-rw-rw-   0        0        0       26 2024-04-10 02:30:43.000000 hebill-1.2.6/hebill/string/__init__.py
+-rw-rw-rw-   0        0        0     1571 2024-04-19 11:39:48.000000 hebill-1.2.6/hebill/string/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.743822 hebill-1.2.6/hebill/sys/
+-rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.2.6/hebill/sys/__init__.py
+-rw-rw-rw-   0        0        0      626 2024-04-19 14:39:39.000000 hebill-1.2.6/hebill/sys/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.747283 hebill-1.2.6/hebill/url/
+-rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.2.6/hebill/url/__init__.py
+-rw-rw-rw-   0        0        0      317 2024-04-05 01:34:58.000000 hebill-1.2.6/hebill/url/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.755296 hebill-1.2.6/hebill/webserver/
+-rw-rw-rw-   0        0        0     1130 2024-04-27 00:45:17.000000 hebill-1.2.6/hebill/webserver/README.MD
+-rw-rw-rw-   0        0        0       94 2024-04-26 07:47:39.000000 hebill-1.2.6/hebill/webserver/__init__.py
+-rw-rw-rw-   0        0        0     1583 2024-04-26 08:04:39.000000 hebill-1.2.6/hebill/webserver/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.757155 hebill-1.2.6/hebill/webserver/features/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:05:18.000000 hebill-1.2.6/hebill/webserver/features/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.759213 hebill-1.2.6/hebill/webserver/features/client/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:05:55.000000 hebill-1.2.6/hebill/webserver/features/client/__init__.py
+-rw-rw-rw-   0        0        0      149 2024-04-26 01:22:46.000000 hebill-1.2.6/hebill/webserver/features/client/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.761534 hebill-1.2.6/hebill/webserver/features/request/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:09:21.000000 hebill-1.2.6/hebill/webserver/features/request/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.764532 hebill-1.2.6/hebill/webserver/features/request/cookies/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:27:33.000000 hebill-1.2.6/hebill/webserver/features/request/cookies/__init__.py
+-rw-rw-rw-   0        0        0      208 2024-04-26 01:22:46.000000 hebill-1.2.6/hebill/webserver/features/request/cookies/core.py
+-rw-rw-rw-   0        0        0      732 2024-04-26 01:22:46.000000 hebill-1.2.6/hebill/webserver/features/request/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.766771 hebill-1.2.6/hebill/webserver/features/request/gets/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:09:55.000000 hebill-1.2.6/hebill/webserver/features/request/gets/__init__.py
+-rw-rw-rw-   0        0        0      152 2024-04-26 01:22:46.000000 hebill-1.2.6/hebill/webserver/features/request/gets/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.774862 hebill-1.2.6/hebill/webserver/features/request/headers/
+-rw-rw-rw-   0        0        0        0 2024-04-03 07:07:38.000000 hebill-1.2.6/hebill/webserver/features/request/headers/__init__.py
+-rw-rw-rw-   0        0        0      219 2024-04-03 08:50:01.000000 hebill-1.2.6/hebill/webserver/features/request/headers/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.777861 hebill-1.2.6/hebill/webserver/features/request/posts/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:09:59.000000 hebill-1.2.6/hebill/webserver/features/request/posts/__init__.py
+-rw-rw-rw-   0        0        0      153 2024-04-26 01:22:46.000000 hebill-1.2.6/hebill/webserver/features/request/posts/core.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.779862 hebill-1.2.6/hebill/webserver/features/website/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:05:11.000000 hebill-1.2.6/hebill/webserver/features/website/__init__.py
+-rw-rw-rw-   0        0        0      479 2024-04-03 03:01:28.000000 hebill-1.2.6/hebill/webserver/features/website/core.py
+-rw-rw-rw-   0        0        0     2448 2024-04-26 08:48:38.000000 hebill-1.2.6/hebill/webserver/handle.py
+-rw-rw-rw-   0        0        0      709 2024-04-27 00:39:52.000000 hebill-1.2.6/hebill/webserver/handle_info.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.782859 hebill-1.2.6/hebill.egg-info/
+-rw-rw-rw-   0        0        0      951 2024-04-27 00:56:59.000000 hebill-1.2.6/hebill.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7270 2024-04-27 00:56:59.000000 hebill-1.2.6/hebill.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 00:56:59.000000 hebill-1.2.6/hebill.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2024-04-27 00:56:59.000000 hebill-1.2.6/hebill.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-27 00:56:59.000000 hebill-1.2.6/hebill.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      654 2024-04-27 00:56:58.000000 hebill-1.2.6/pack_upload_setup.py
+-rw-rw-rw-   0        0        0       42 2024-04-27 00:56:59.785862 hebill-1.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.780859 hebill-1.2.6/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-26 01:33:24.000000 hebill-1.2.6/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.781860 hebill-1.2.6/tests/webserver/
+-rw-rw-rw-   0        0        0        0 2024-04-26 01:33:30.000000 hebill-1.2.6/tests/webserver/__init__.py
```

### Comparing `hebill-1.2.5/PKG-INFO` & `hebill-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hebill
-Version: 1.2.5
+Version: 1.2.6
 Summary: Python Hebill
 Requires-Python: >=3.12
 Description-Content-Type: text/plain
 License-File: LICENSE.rst
 Requires-Dist: psutil==5.9.8
 Requires-Dist: pillow==10.3.0
 Requires-Dist: requests==2.31.0
```

### Comparing `hebill-1.2.5/hebill/README.MD` & `hebill-1.2.6/hebill/README.MD`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/dimensions/README.MD` & `hebill-1.2.6/hebill/dimensions/README.MD`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/dimensions/core.py` & `hebill-1.2.6/hebill/dimensions/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/dir/core.py` & `hebill-1.2.6/hebill/dir/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/file/core.py` & `hebill-1.2.6/hebill/file/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/html/components/html/head/core.py` & `hebill-1.2.6/hebill/html/components/html/head/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/html/components/table/core.py` & `hebill-1.2.6/hebill/html/components/table/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/html/components/table/tbody/core.py` & `hebill-1.2.6/hebill/html/components/table/tbody/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/html/components/table/tbody/tr/core.py` & `hebill-1.2.6/hebill/html/components/table/tbody/tr/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/html/components/table/thead/core.py` & `hebill-1.2.6/hebill/html/components/table/thead/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/html/components/table/thead/tr/core.py` & `hebill-1.2.6/hebill/html/components/table/thead/tr/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/html/core.py` & `hebill-1.2.6/hebill/html/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/html/nodes/comment/core.py` & `hebill-1.2.6/hebill/html/nodes/comment/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/html/nodes/group/core.py` & `hebill-1.2.6/hebill/html/nodes/group/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/html/nodes/group/create/core.py` & `hebill-1.2.6/hebill/html/nodes/group/create/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/html/nodes/group/create/nodes/core.py` & `hebill-1.2.6/hebill/html/nodes/group/create/nodes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/html/nodes/group/create/tags/core.py` & `hebill-1.2.6/hebill/html/nodes/group/create/tags/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/html/nodes/node/core.py` & `hebill-1.2.6/hebill/html/nodes/node/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/html/nodes/tag/attributes/classes/core.py` & `hebill-1.2.6/hebill/html/nodes/tag/attributes/classes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/html/nodes/tag/attributes/core.py` & `hebill-1.2.6/hebill/html/nodes/tag/attributes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/html/nodes/tag/attributes/styles/core.py` & `hebill-1.2.6/hebill/html/nodes/tag/attributes/styles/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/html/nodes/tag/core.py` & `hebill-1.2.6/hebill/html/nodes/tag/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/html/tags/__init__.py` & `hebill-1.2.6/hebill/html/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/image/__init__.py` & `hebill-1.2.6/hebill/image/__init__.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/image/png/constants.py` & `hebill-1.2.6/hebill/image/png/constants.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/image/png/core.py` & `hebill-1.2.6/hebill/image/png/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/mysql/core.py` & `hebill-1.2.6/hebill/mysql/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/mysql/features/table_describe_data.py` & `hebill-1.2.6/hebill/mysql/features/table_describe_data.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/mysql/features/table_index_data.py` & `hebill-1.2.6/hebill/mysql/features/table_index_data.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/mysql/features/table_status_data.py` & `hebill-1.2.6/hebill/mysql/features/table_status_data.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/mysql/plugins/columns/core.py` & `hebill-1.2.6/hebill/mysql/plugins/columns/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/mysql/plugins/limits/core.py` & `hebill-1.2.6/hebill/mysql/plugins/limits/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/mysql/plugins/orders/core.py` & `hebill-1.2.6/hebill/mysql/plugins/orders/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/mysql/plugins/wheres/condition.py` & `hebill-1.2.6/hebill/mysql/plugins/wheres/condition.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/mysql/plugins/wheres/conditions.py` & `hebill-1.2.6/hebill/mysql/plugins/wheres/conditions.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/mysql/table/core.py` & `hebill-1.2.6/hebill/mysql/table/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/mysql/table/data/core.py` & `hebill-1.2.6/hebill/mysql/table/data/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/mysql/table/data/drop.py` & `hebill-1.2.6/hebill/mysql/table/data/drop.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/mysql/table/data/insert.py` & `hebill-1.2.6/hebill/mysql/table/data/insert.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/mysql/table/data/search.py` & `hebill-1.2.6/hebill/mysql/table/data/search.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/mysql/table/data/update.py` & `hebill-1.2.6/hebill/mysql/table/data/update.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/numeric/constants.py` & `hebill-1.2.6/hebill/numeric/constants.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/numeric/core.py` & `hebill-1.2.6/hebill/numeric/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/pdf/component/core.py` & `hebill-1.2.6/hebill/pdf/component/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/pdf/constants.py` & `hebill-1.2.6/hebill/pdf/constants.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/pdf/core.py` & `hebill-1.2.6/hebill/pdf/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/pdf/features/document_configs.py` & `hebill-1.2.6/hebill/pdf/features/document_configs.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/pdf/features/page_configs.py` & `hebill-1.2.6/hebill/pdf/features/page_configs.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/pdf/features/styles.py` & `hebill-1.2.6/hebill/pdf/features/styles.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/pdf/library/configs_selector_color.py` & `hebill-1.2.6/hebill/pdf/library/configs_selector_color.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/pdf/library/configs_selector_font.py` & `hebill-1.2.6/hebill/pdf/library/configs_selector_font.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/pdf/page/_draw_.py` & `hebill-1.2.6/hebill/pdf/page/_draw_.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/pdf/page/core.py` & `hebill-1.2.6/hebill/pdf/page/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/pdf/page/draw_grids.py` & `hebill-1.2.6/hebill/pdf/page/draw_grids.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/pdf/page/draw_path.py` & `hebill-1.2.6/hebill/pdf/page/draw_path.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/pdf/page/draw_rect.py` & `hebill-1.2.6/hebill/pdf/page/draw_rect.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/pdf/page/draw_string.py` & `hebill-1.2.6/hebill/pdf/page/draw_string.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/pypi/README.MD` & `hebill-1.2.6/hebill/pypi/README.MD`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/pypi/core.py` & `hebill-1.2.6/hebill/pypi/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,16 @@
             lines.append(f'{' ' * 4}packages=[')
             for n in self.packages:
                 lines.append(f'{' ' * 8}\'{n}\',')
             lines.append(f'{' ' * 4}],')
         else:  # find_packages
             lines.append(f'{' ' * 4}packages=find_packages(),')
             # lines.append(f'{' ' * 8}\'{self.module.__name__}\',')
+
+        # 打包所有内部markdown文件
         lines.append(f'{' ' * 4}package_data={{')
         lines.append(f'{' ' * 8}\'\': [\'*.md\', \'*.MD\'],')
         lines.append(f'{' ' * 4}}},')
 
         lines.append(f'{' ' * 4}install_requires=[')
         if len(self.install_requires) > 0:
             for n, v in self.install_requires.items():
```

### Comparing `hebill-1.2.5/hebill/string/core.py` & `hebill-1.2.6/hebill/string/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/sys/core.py` & `hebill-1.2.6/hebill/sys/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.5/hebill/webserver/core.py` & `hebill-1.2.6/hebill/webserver/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 import os
 from .handle import Handle
+from .handle_info import HandleInfo
 from http.server import HTTPServer
+from ..sys import Sys
 
 
 class WebServer:
-    def __init__(self, host: str = '', port: int = 8000, root: str = None, handle=None):
-        self._handle = handle if handle is not None else Handle
+    def __init__(self,  host: str = '', port: int = 8000, root: str = None, handle: Handle = None):
         self._host = host
         self._port = port
         self._server = None
+        self._handle = handle if handle is not None else HandleInfo
         self._root = root if root else os.getcwd()
 
     @property
-    def handle(self): return self._handle
-
-    @property
     def host(self) -> str: return self._host
 
     @property
     def port(self) -> int: return self._port
 
     @property
+    def handle(self) -> Handle: return self._handle
+
+    @property
     def server(self) -> HTTPServer:
         if self._server is None:
             self._server = HTTPServer((self.host, self.port), self.handle)
         return self._server
 
     def start(self):
-        print(f'服务器开始运行')
+        print(f'Hebill: Server started and listing on:')
         if self.host:
             print(f'- http://{self.host}:{self.port}')
         else:
             print(f'- http://127.0.0.1:{self.port}')
             print(f'- http://localhost:{self.port}')
-            from ..sys import Sys
-            ips = Sys.local_ips()
-            for ip in ips:
-                print(f'- http://{ip}:{self.port}')
-            print(f'- http://{self.host}:{self.port}')
+            for ip in Sys.local_ips():
+                if ip != '' and ip is not None and '::' not in ip:
+                    print(f'- http://{ip}:{self.port}')
 
         try:
             self.server.serve_forever()
+
         except KeyboardInterrupt:
-            print(f'服务器已经停止工作')
+            print(f'Hebill: Server stopped by keyboard interrupt.')
             pass
 
-    def close(self):
+    def stop(self):
         self.server.server_close()
-        print(f'服务器已经停止工作')
+        print(f'Hebill: Server stopped.')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hebill-1.2.5/hebill/webserver/handle.py` & `hebill-1.2.6/hebill/webserver/handle.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,62 @@
 from http.cookies import SimpleCookie
 from http.server import BaseHTTPRequestHandler
 from urllib.parse import parse_qs, urlparse
+from .features.request.core import Request
 
 
 class Handle(BaseHTTPRequestHandler):
     def __init__(self, client_address, request, server):
+        self._requests = Request()
         super().__init__(client_address, request, server)
-        self._get: dict = {}
-        self._post: dict = {}
-        self._cookie: dict = {}
+
+    @property
+    def requests(self) -> Request:
+        return self._requests
+
+    def response(self) -> str:
+        return f'Hello World.'
 
     def do_GET(self):
         # 由于每次连接都会有GET favicon.ico，避免多余的GET处理
         if self.path == '/favicon.ico':
             from ..image import PNGIconHebill
             icon = PNGIconHebill()
             self.send_response(200)
             self.send_header('Content-type', 'image/x-icon')
             self.end_headers()
             self.wfile.write(icon.bites)
         else:
             # Refer to the reference.txt
-            print(self.headers)
-            headers = dict(self.headers)
-            cookies = {}
-            if 'Cookie' in headers:
-                for key, morsel in SimpleCookie(headers['Cookie']).items():
-                    cookies[key] = morsel.value
-            q = urlparse(self.path).query
-            get = {}
-            if q:
-                for p in q.split('&'):
+            for key, value in dict(self.headers).items():
+                self.requests.headers[key] = value
+
+            if 'Cookie' in self.requests.headers:
+                for key, morsel in SimpleCookie(self.requests.headers['Cookie']).items():
+                    self.requests.cookies[key] = morsel.value
+            get_parameters = urlparse(self.path).query
+            if get_parameters:
+                for p in get_parameters.split('&'):
                     k, v = p.split('=')
-                    if get.get(k) is None:
-                        get[k] = []
-                    get[k].append(v)
-            from .features.request.core import Request
-            request = Request(
-                cookies,
-                get,
-                parse_qs(self.rfile.read(
-                    int(self.headers['Content-Length']) if 'Content-Length' in self.headers else 0).decode('utf-8')),
-                headers
-            )
-            print(request.cookie)
-            print(request.get)
-            print(request.post)
-            print(request.headers)
+                    self.requests.gets[k] = v
+            url = self.rfile.read(int(self.headers['Content-Length']) if 'Content-Length' in self.headers else 0)
+            post_parameters = parse_qs(url.decode('utf-8'))
+            for k, v in post_parameters.items():
+                self.requests.posts[k] = v
             # 继续相关操作
             try:
                 # 发送响应状态码
                 self.send_response(200)
                 # 设置响应头
                 self.send_header('Content-type', 'text/html')
                 self.end_headers()
                 # 响应内容
-                self.wfile.write(b"Hello, world!")  # 将字符串转换为字节流并发送
+                self.wfile.write(self.response().encode('utf-8'))  # 将字符串转换为字节流并发送
             except ConnectionAbortedError as e:
-                print("用户已经中断连接或其他异常:", e)
+                print("Hebill: Connection interrupted by user.", e)
 
     def do_POST(self):
         pass
 
     def do_PUT(self):
         pass
```

### Comparing `hebill-1.2.5/hebill.egg-info/PKG-INFO` & `hebill-1.2.6/hebill.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hebill
-Version: 1.2.5
+Version: 1.2.6
 Summary: Python Hebill
 Requires-Python: >=3.12
 Description-Content-Type: text/plain
 License-File: LICENSE.rst
 Requires-Dist: psutil==5.9.8
 Requires-Dist: pillow==10.3.0
 Requires-Dist: requests==2.31.0
```

### Comparing `hebill-1.2.5/hebill.egg-info/SOURCES.txt` & `hebill-1.2.6/hebill.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -188,22 +188,25 @@
 hebill/sys/core.py
 hebill/url/__init__.py
 hebill/url/core.py
 hebill/webserver/README.MD
 hebill/webserver/__init__.py
 hebill/webserver/core.py
 hebill/webserver/handle.py
+hebill/webserver/handle_info.py
 hebill/webserver/features/__init__.py
 hebill/webserver/features/client/__init__.py
 hebill/webserver/features/client/core.py
 hebill/webserver/features/request/__init__.py
 hebill/webserver/features/request/core.py
-hebill/webserver/features/request/cookie/__init__.py
-hebill/webserver/features/request/cookie/core.py
-hebill/webserver/features/request/get/__init__.py
-hebill/webserver/features/request/get/core.py
+hebill/webserver/features/request/cookies/__init__.py
+hebill/webserver/features/request/cookies/core.py
+hebill/webserver/features/request/gets/__init__.py
+hebill/webserver/features/request/gets/core.py
 hebill/webserver/features/request/headers/__init__.py
 hebill/webserver/features/request/headers/core.py
-hebill/webserver/features/request/post/__init__.py
-hebill/webserver/features/request/post/core.py
+hebill/webserver/features/request/posts/__init__.py
+hebill/webserver/features/request/posts/core.py
 hebill/webserver/features/website/__init__.py
-hebill/webserver/features/website/core.py
+hebill/webserver/features/website/core.py
+tests/__init__.py
+tests/webserver/__init__.py
```

### Comparing `hebill-1.2.5/pack_upload_setup.py` & `hebill-1.2.6/pack_upload_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 setup(
     name='hebill',
-    version='1.2.5',
+    version='1.2.6',
     description='Python Hebill',
     long_description=open(r'D:\SDK\GitHub\python_hebill\hebill\README.MD', encoding='utf-8').read(),
     long_description_content_type='text/plain',
     packages=find_packages(),
     package_data={
         '': ['*.md', '*.MD'],
     },
```

