# Comparing `tmp/xtn-tools-pro-1.0.0.0.2.tar.gz` & `tmp/xtn-tools-pro-1.0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xtn-tools-pro-1.0.0.0.2.tar", last modified: Fri Apr 19 10:22:11 2024, max compression
+gzip compressed data, was "dist\xtn-tools-pro-1.0.0.0.3.tar", last modified: Sat Apr 27 07:51:03 2024, max compression
```

## Comparing `xtn-tools-pro-1.0.0.0.2.tar` & `xtn-tools-pro-1.0.0.0.3.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 10:22:11.000000 xtn-tools-pro-1.0.0.0.2/
--rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtn-tools-pro-1.0.0.0.2/LICENSE
--rw-rw-rw-   0        0        0      287 2024-04-19 10:22:11.000000 xtn-tools-pro-1.0.0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtn-tools-pro-1.0.0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-19 10:22:11.000000 xtn-tools-pro-1.0.0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1189 2024-04-19 10:21:56.000000 xtn-tools-pro-1.0.0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 10:22:11.000000 xtn-tools-pro-1.0.0.0.2/xtn_tools_pro/
--rw-rw-rw-   0        0        0      395 2024-04-18 05:24:09.000000 xtn-tools-pro-1.0.0.0.2/xtn_tools_pro/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 10:22:11.000000 xtn-tools-pro-1.0.0.0.2/xtn_tools_pro/db/
--rw-rw-rw-   0        0        0     5567 2024-04-19 08:42:19.000000 xtn-tools-pro-1.0.0.0.2/xtn_tools_pro/db/MongoDB.py
--rw-rw-rw-   0        0        0     4003 2024-04-18 07:53:11.000000 xtn-tools-pro-1.0.0.0.2/xtn_tools_pro/db/RedisDB.py
--rw-rw-rw-   0        0        0      416 2024-04-18 05:40:27.000000 xtn-tools-pro-1.0.0.0.2/xtn_tools_pro/db/__init__.py
--rw-rw-rw-   0        0        0     2630 2024-04-19 10:12:45.000000 xtn-tools-pro-1.0.0.0.2/xtn_tools_pro/tools.py
--rw-rw-rw-   0        0        0     1512 2024-04-19 10:21:05.000000 xtn-tools-pro-1.0.0.0.2/xtn_tools_pro/tools_flie.py
--rw-rw-rw-   0        0        0     4867 2024-04-19 10:12:45.000000 xtn-tools-pro-1.0.0.0.2/xtn_tools_pro/tools_time.py
-drwxrwxrwx   0        0        0        0 2024-04-19 10:22:11.000000 xtn-tools-pro-1.0.0.0.2/xtn_tools_pro.egg-info/
--rw-rw-rw-   0        0        0      287 2024-04-19 10:22:11.000000 xtn-tools-pro-1.0.0.0.2/xtn_tools_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2024-04-19 10:22:11.000000 xtn-tools-pro-1.0.0.0.2/xtn_tools_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 10:22:11.000000 xtn-tools-pro-1.0.0.0.2/xtn_tools_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-19 10:22:11.000000 xtn-tools-pro-1.0.0.0.2/xtn_tools_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-19 10:22:11.000000 xtn-tools-pro-1.0.0.0.2/xtn_tools_pro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/
+-rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtn-tools-pro-1.0.0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      287 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtn-tools-pro-1.0.0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2024-04-27 06:01:26.000000 xtn-tools-pro-1.0.0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/
+-rw-rw-rw-   0        0        0      395 2024-04-18 05:24:09.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/db/
+-rw-rw-rw-   0        0        0     5567 2024-04-19 08:42:19.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/db/MongoDB.py
+-rw-rw-rw-   0        0        0     6053 2024-04-27 07:30:36.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/db/RedisDB.py
+-rw-rw-rw-   0        0        0      416 2024-04-18 05:40:27.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/proxy/
+-rw-rw-rw-   0        0        0     9842 2024-04-27 07:38:44.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/proxy/XiaoXiangProxy.py
+-rw-rw-rw-   0        0        0      418 2024-04-27 04:18:50.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/proxy/__init__.py
+-rw-rw-rw-   0        0        0     2630 2024-04-19 10:12:45.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/tools.py
+-rw-rw-rw-   0        0        0     1512 2024-04-19 10:21:05.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/tools_flie.py
+-rw-rw-rw-   0        0        0     4867 2024-04-19 10:12:45.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/tools_time.py
+drwxrwxrwx   0        0        0        0 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro.egg-info/
+-rw-rw-rw-   0        0        0      287 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-27 07:51:03.000000 xtn-tools-pro-1.0.0.0.3/xtn_tools_pro.egg-info/top_level.txt
```

### Comparing `xtn-tools-pro-1.0.0.0.2/setup.py` & `xtn-tools-pro-1.0.0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,25 +11,26 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="xtn-tools-pro",  # 模块名称
-    version="1.0.0.0.2",  # 版本
+    version="1.0.0.0.3",  # 版本
     author="xtn",  # 作者
     author_email="czw011122@163.com",  # 作者邮箱
     description="xtn 开发工具",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据(更多描述信息)
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
     # 依赖模块
     install_requires=[
         "pymongo",
-        "redis"
+        "redis",
+        "requests"
     ],
     python_requires='>=3',
 )
```

### Comparing `xtn-tools-pro-1.0.0.0.2/xtn_tools_pro/db/MongoDB.py` & `xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/db/MongoDB.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.0.2/xtn_tools_pro/tools.py` & `xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/tools.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.0.2/xtn_tools_pro/tools_flie.py` & `xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/tools_flie.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.0.2/xtn_tools_pro/tools_time.py` & `xtn-tools-pro-1.0.0.0.3/xtn_tools_pro/tools_time.py`

 * *Files identical despite different names*

