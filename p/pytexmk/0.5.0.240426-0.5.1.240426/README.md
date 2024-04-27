# Comparing `tmp/pytexmk-0.5.0.240426.tar.gz` & `tmp/pytexmk-0.5.1.240426.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytexmk-0.5.0.240426.tar", last modified: Fri Apr 26 14:49:18 2024, max compression
+gzip compressed data, was "pytexmk-0.5.1.240426.tar", last modified: Fri Apr 26 15:20:15 2024, max compression
```

## Comparing `pytexmk-0.5.0.240426.tar` & `pytexmk-0.5.1.240426.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 14:49:18.821466 pytexmk-0.5.0.240426/
--rw-rw-r--   0 yanming   (1000) yanming   (1000)    35149 2024-02-28 15:10:35.000000 pytexmk-0.5.0.240426/LICENSE
--rw-rw-r--   0 yanming   (1000) yanming   (1000)       30 2024-03-06 03:27:48.000000 pytexmk-0.5.0.240426/MANIFEST.in
--rw-rw-r--   0 yanming   (1000) yanming   (1000)      466 2024-03-06 03:27:48.000000 pytexmk-0.5.0.240426/Makefile
--rw-r--r--   0 yanming   (1000) yanming   (1000)     9034 2024-04-26 14:49:18.821466 pytexmk-0.5.0.240426/PKG-INFO
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     7988 2024-04-26 14:37:00.000000 pytexmk-0.5.0.240426/README.md
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     1195 2024-03-21 15:51:11.000000 pytexmk-0.5.0.240426/pyproject.toml
--rw-rw-r--   0 yanming   (1000) yanming   (1000)       38 2024-04-26 14:49:18.821466 pytexmk-0.5.0.240426/setup.cfg
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 14:49:18.817467 pytexmk-0.5.0.240426/src/
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 14:49:18.821466 pytexmk-0.5.0.240426/src/pytexmk/
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     1940 2024-02-29 11:40:30.000000 pytexmk-0.5.0.240426/src/pytexmk/__init__.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)    11483 2024-04-26 14:44:17.000000 pytexmk-0.5.0.240426/src/pytexmk/__main__.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)    10195 2024-04-26 14:32:56.000000 pytexmk-0.5.0.240426/src/pytexmk/additional_operation.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     9922 2024-03-22 06:51:11.000000 pytexmk-0.5.0.240426/src/pytexmk/compile_model.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     5896 2024-03-22 06:50:52.000000 pytexmk-0.5.0.240426/src/pytexmk/info_print.py
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     1922 2024-04-26 14:37:34.000000 pytexmk-0.5.0.240426/src/pytexmk/version.py
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 14:49:18.821466 pytexmk-0.5.0.240426/src/pytexmk.egg-info/
--rw-r--r--   0 yanming   (1000) yanming   (1000)     9034 2024-04-26 14:49:18.000000 pytexmk-0.5.0.240426/src/pytexmk.egg-info/PKG-INFO
--rw-rw-r--   0 yanming   (1000) yanming   (1000)      441 2024-04-26 14:49:18.000000 pytexmk-0.5.0.240426/src/pytexmk.egg-info/SOURCES.txt
--rw-rw-r--   0 yanming   (1000) yanming   (1000)        1 2024-04-26 14:49:18.000000 pytexmk-0.5.0.240426/src/pytexmk.egg-info/dependency_links.txt
--rw-rw-r--   0 yanming   (1000) yanming   (1000)       41 2024-04-26 14:49:18.000000 pytexmk-0.5.0.240426/src/pytexmk.egg-info/entry_points.txt
--rw-rw-r--   0 yanming   (1000) yanming   (1000)       13 2024-04-26 14:49:18.000000 pytexmk-0.5.0.240426/src/pytexmk.egg-info/requires.txt
--rw-rw-r--   0 yanming   (1000) yanming   (1000)        8 2024-04-26 14:49:18.000000 pytexmk-0.5.0.240426/src/pytexmk.egg-info/top_level.txt
-drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 14:49:18.821466 pytexmk-0.5.0.240426/tests/
--rw-rw-r--   0 yanming   (1000) yanming   (1000)     9643 2024-03-22 06:30:29.000000 pytexmk-0.5.0.240426/tests/test.py
+drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 15:20:15.165012 pytexmk-0.5.1.240426/
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)    35149 2024-02-28 15:10:35.000000 pytexmk-0.5.1.240426/LICENSE
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)       30 2024-03-06 03:27:48.000000 pytexmk-0.5.1.240426/MANIFEST.in
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)      466 2024-03-06 03:27:48.000000 pytexmk-0.5.1.240426/Makefile
+-rw-r--r--   0 yanming   (1000) yanming   (1000)     9034 2024-04-26 15:20:15.165012 pytexmk-0.5.1.240426/PKG-INFO
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     7988 2024-04-26 14:37:00.000000 pytexmk-0.5.1.240426/README.md
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     1195 2024-03-21 15:51:11.000000 pytexmk-0.5.1.240426/pyproject.toml
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)       38 2024-04-26 15:20:15.165012 pytexmk-0.5.1.240426/setup.cfg
+drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 15:20:15.161012 pytexmk-0.5.1.240426/src/
+drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 15:20:15.161012 pytexmk-0.5.1.240426/src/pytexmk/
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     1940 2024-02-29 11:40:30.000000 pytexmk-0.5.1.240426/src/pytexmk/__init__.py
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)    11497 2024-04-26 15:19:03.000000 pytexmk-0.5.1.240426/src/pytexmk/__main__.py
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)    10250 2024-04-26 15:10:42.000000 pytexmk-0.5.1.240426/src/pytexmk/additional_operation.py
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     9922 2024-03-22 06:51:11.000000 pytexmk-0.5.1.240426/src/pytexmk/compile_model.py
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     5896 2024-03-22 06:50:52.000000 pytexmk-0.5.1.240426/src/pytexmk/info_print.py
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     1922 2024-04-26 15:19:26.000000 pytexmk-0.5.1.240426/src/pytexmk/version.py
+drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 15:20:15.165012 pytexmk-0.5.1.240426/src/pytexmk.egg-info/
+-rw-r--r--   0 yanming   (1000) yanming   (1000)     9034 2024-04-26 15:20:15.000000 pytexmk-0.5.1.240426/src/pytexmk.egg-info/PKG-INFO
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)      441 2024-04-26 15:20:15.000000 pytexmk-0.5.1.240426/src/pytexmk.egg-info/SOURCES.txt
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)        1 2024-04-26 15:20:15.000000 pytexmk-0.5.1.240426/src/pytexmk.egg-info/dependency_links.txt
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)       41 2024-04-26 15:20:15.000000 pytexmk-0.5.1.240426/src/pytexmk.egg-info/entry_points.txt
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)       13 2024-04-26 15:20:15.000000 pytexmk-0.5.1.240426/src/pytexmk.egg-info/requires.txt
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)        8 2024-04-26 15:20:15.000000 pytexmk-0.5.1.240426/src/pytexmk.egg-info/top_level.txt
+drwxrwxr-x   0 yanming   (1000) yanming   (1000)        0 2024-04-26 15:20:15.165012 pytexmk-0.5.1.240426/tests/
+-rw-rw-r--   0 yanming   (1000) yanming   (1000)     9643 2024-03-22 06:30:29.000000 pytexmk-0.5.1.240426/tests/test.py
```

### Comparing `pytexmk-0.5.0.240426/LICENSE` & `pytexmk-0.5.1.240426/LICENSE`

 * *Files identical despite different names*

### Comparing `pytexmk-0.5.0.240426/PKG-INFO` & `pytexmk-0.5.1.240426/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytexmk
-Version: 0.5.0.240426
+Version: 0.5.1.240426
 Summary: LaTeX 辅助编译命令行工具 LaTeX Auxiliary Compilation Command Line Tool
 Author-email: 焱铭 <lxb-yanming@foxmail.com>
 Project-URL: Homepage, https://github.com/YanMing-lxb/PyTeXMK
 Project-URL: Bug Tracker, https://github.com/YanMing-lxb/PyTeXMK/issues
 Keywords: LaTeX,build,latexmk
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `pytexmk-0.5.0.240426/README.md` & `pytexmk-0.5.1.240426/README.md`

 * *Files identical despite different names*

### Comparing `pytexmk-0.5.0.240426/pyproject.toml` & `pytexmk-0.5.1.240426/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytexmk-0.5.0.240426/src/pytexmk/__init__.py` & `pytexmk-0.5.1.240426/src/pytexmk/__init__.py`

 * *Files identical despite different names*

### Comparing `pytexmk-0.5.0.240426/src/pytexmk/__main__.py` & `pytexmk-0.5.1.240426/src/pytexmk/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  ··························································Y8b·d88P·····
  ···························································"Y88P"······
  =======================================================================
 
  -----------------------------------------------------------------------
 Author       : 焱铭
 Date         : 2024-02-28 23:11:52 +0800
-LastEditTime : 2024-04-26 22:43:47 +0800
+LastEditTime : 2024-04-26 23:19:03 +0800
 Github       : https://github.com/YanMing-lxb/
 FilePath     : /PyTeXMK/src/pytexmk/__main__.py
 Description  : 
  -----------------------------------------------------------------------
 '''
 # -*- coding: utf-8 -*-
 import argparse
@@ -123,45 +123,45 @@
     parser.add_argument('-C', '--Clean', action='store_true', help="清除所有辅助文件和 pdf 文件")
     parser.add_argument('-nq', '--no-quiet', action='store_true', help="非安静模式运行，此模式下显示编译过程")
     parser.add_argument('-cp', '--clean-pdf', action='store_true', help="清理 pdf 文件，当 LaTeX 编译过程中警告 invalid X X R object 时，可使用此参数清理所有 pdf 文件")
     
     parser.add_argument('document', nargs='?', help="要被编译的文件名")
     args = parser.parse_args()
 
-    tex_files = search_tex_file # 运行 search_tex_file 函数搜索当前目录下所有 tex 文件
+    tex_files = search_tex_file() # 运行 search_tex_file 函数搜索当前目录下所有 tex 文件
     magic_comments = search_magic_comments(tex_files, magic_comments_keys) # 运行 search_magic_comments 函数搜索 tex_files 列表中是否存在 magic comments
 
     # --------------------------------------------------------------------------------
     # 输出文件路径判断
     # --------------------------------------------------------------------------------
-    if magic_comments['outdir']: # 如果存在 magic comments 且 outdir 存在
+    if magic_comments.get('outdir'): # 如果存在 magic comments 且 outdir 存在
         outdir = magic_comments['outdir'] # 使用 magic comments 中的 outdir 作为输出目录
         print(f"通过魔法注释找到输出目录为 {outdir}！")
 
     # --------------------------------------------------------------------------------
     # 主文件逻辑判断
     # --------------------------------------------------------------------------------
     if args.document: # pytexmk 指定 latex 文件
         file_name = check_file_name(args.document) # check_file_name 函数检查 args.document 参数输入的文件名是否正确
     else: # pytexmk 未指定 latex 文件
-        if magic_comments['root']: # 如果存在 magic comments 且 root 存在
+        if magic_comments.get('root'): # 如果存在 magic comments 且 root 存在
             file_name = check_file_name(magic_comments['root']) # 使用 magic comments 中的 root 作为文件名
             print(f"通过魔法注释找到 {file_name}.tex 文件！")
         else: # pytexmk 和魔法注释都不存在，使用search_main_file方法搜索主文件
             file_name = search_main_file(tex_files)
     # --------------------------------------------------------------------------------
     # 编译类型判断
     # --------------------------------------------------------------------------------
     if args.xelatex:
         tex_name = "xelatex"
     elif args.pdflatex:
         tex_name = "pdflatex"
     elif args.lualatex:
         tex_name = "lualatex"
-    elif magic_comments['program']: # 如果存在 magic comments 且 program 存在
+    elif magic_comments.get('program'): # 如果存在 magic comments 且 program 存在
         tex_name = magic_comments['program'] # 使用 magic comments 中的 program 作为编译器
         print(f"通过魔法注释设置编译器为 {tex_name}！")
 
     # --------------------------------------------------------------------------------
     # 编译程序运行
     # --------------------------------------------------------------------------------
```

### Comparing `pytexmk-0.5.0.240426/src/pytexmk/additional_operation.py` & `pytexmk-0.5.1.240426/src/pytexmk/additional_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  ··························································Y8b·d88P·····
  ···························································"Y88P"······
  =======================================================================
 
  -----------------------------------------------------------------------
 Author       : 焱铭
 Date         : 2024-02-29 16:02:37 +0800
-LastEditTime : 2024-04-26 22:32:56 +0800
+LastEditTime : 2024-04-26 23:10:42 +0800
 Github       : https://github.com/YanMing-lxb/
 FilePath     : /PyTeXMK/src/pytexmk/additional_operation.py
 Description  : 
  -----------------------------------------------------------------------
 '''
 # -*- coding: utf-8 -*-
 import os
@@ -184,16 +184,17 @@
     return file_name
 
 # --------------------------------------------------------------------------------
 # 定义魔法注释检索函数
 # --------------------------------------------------------------------------------
 def search_magic_comments(tex_files, magic_comments_keys):
     magic_comments = {}  # 创建空字典用于存储结果
-    for file_path in tex_files:  # 遍历tex文件列表
-        with open(file_path, 'r') as file:  # 打开文件
-            for _ in range(50):  # 遍历文件的前50行
-                line = file.readline()  # 读取一行内容
-                for magic_comments_key in magic_comments_keys:  # 遍历关键字列表
-                    if f"% !TEX {magic_comments_key} =" in line:  # 如果关键字出现在这一行
-                        magic_comment = line.split(f"% !TEX {magic_comments_key} = ")[1].strip()  # 提取对应的值
-                        magic_comments[magic_comments_key] = magic_comment  # 将键值对存入字典
+    if len(tex_files):
+        for file_path in tex_files:  # 遍历tex文件列表
+            with open(file_path, 'r') as file:  # 打开文件
+                for _ in range(50):  # 遍历文件的前50行
+                    line = file.readline()  # 读取一行内容
+                    for magic_comments_key in magic_comments_keys:  # 遍历关键字列表
+                        if f"% !TEX {magic_comments_key} =" in line:  # 如果关键字出现在这一行
+                            magic_comment = line.split(f"% !TEX {magic_comments_key} = ")[1].strip()  # 提取对应的值
+                            magic_comments[magic_comments_key] = magic_comment  # 将键值对存入字典
     return magic_comments  # 返回提取的键值对字典
```

### Comparing `pytexmk-0.5.0.240426/src/pytexmk/compile_model.py` & `pytexmk-0.5.1.240426/src/pytexmk/compile_model.py`

 * *Files identical despite different names*

### Comparing `pytexmk-0.5.0.240426/src/pytexmk/info_print.py` & `pytexmk-0.5.1.240426/src/pytexmk/info_print.py`

 * *Files identical despite different names*

### Comparing `pytexmk-0.5.0.240426/src/pytexmk/version.py` & `pytexmk-0.5.1.240426/src/pytexmk/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,18 @@
  ··························································Y8b·d88P·····
  ···························································"Y88P"······
  =======================================================================
 
  -----------------------------------------------------------------------
 Author       : 焱铭
 Date         : 2024-03-01 15:52:28 +0800
-LastEditTime : 2024-04-26 22:37:34 +0800
+LastEditTime : 2024-04-26 23:19:26 +0800
 Github       : https://github.com/YanMing-lxb/
 FilePath     : /PyTeXMK/src/pytexmk/version.py
 Description  : 
  -----------------------------------------------------------------------
 '''
 # -*- coding: utf-8 -*-
 #!/usr/bin/env python
 
 script_name = 'PyTeXMK'
-__version__ = '0.5.0.240426'
+__version__ = '0.5.1.240426'
```

### Comparing `pytexmk-0.5.0.240426/src/pytexmk.egg-info/PKG-INFO` & `pytexmk-0.5.1.240426/src/pytexmk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytexmk
-Version: 0.5.0.240426
+Version: 0.5.1.240426
 Summary: LaTeX 辅助编译命令行工具 LaTeX Auxiliary Compilation Command Line Tool
 Author-email: 焱铭 <lxb-yanming@foxmail.com>
 Project-URL: Homepage, https://github.com/YanMing-lxb/PyTeXMK
 Project-URL: Bug Tracker, https://github.com/YanMing-lxb/PyTeXMK/issues
 Keywords: LaTeX,build,latexmk
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `pytexmk-0.5.0.240426/tests/test.py` & `pytexmk-0.5.1.240426/tests/test.py`

 * *Files identical despite different names*

