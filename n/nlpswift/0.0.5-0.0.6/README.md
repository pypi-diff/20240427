# Comparing `tmp/nlpswift-0.0.5.tar.gz` & `tmp/nlpswift-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpswift-0.0.5.tar", last modified: Sat Apr 27 12:31:33 2024, max compression
+gzip compressed data, was "nlpswift-0.0.6.tar", last modified: Sat Apr 27 12:55:38 2024, max compression
```

## Comparing `nlpswift-0.0.5.tar` & `nlpswift-0.0.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-27 12:31:33.890172 nlpswift-0.0.5/
--rw-r--r--   0 zhpmatrix   (501) staff       (20)     1211 2024-04-24 11:30:31.000000 nlpswift-0.0.5/LICENSE
--rw-r--r--   0 zhpmatrix   (501) staff       (20)     1266 2024-04-27 12:31:33.889943 nlpswift-0.0.5/PKG-INFO
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      663 2024-04-24 11:30:31.000000 nlpswift-0.0.5/README.md
-drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-27 12:31:33.885976 nlpswift-0.0.5/nlpknife/
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      320 2024-04-27 11:47:53.000000 nlpswift-0.0.5/nlpknife/__init__.py
-drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-27 12:31:33.887054 nlpswift-0.0.5/nlpknife/db/
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      157 2024-04-24 11:30:31.000000 nlpswift-0.0.5/nlpknife/db/__init__.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)        0 2024-04-24 11:30:31.000000 nlpswift-0.0.5/nlpknife/db/es_helper.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)        0 2024-04-24 11:30:31.000000 nlpswift-0.0.5/nlpknife/db/minio_helper.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)     1362 2024-04-24 11:30:31.000000 nlpswift-0.0.5/nlpknife/db/mysql_helper.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      560 2024-04-24 11:30:31.000000 nlpswift-0.0.5/nlpknife/db/neo4j_helper.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      647 2024-04-24 14:16:10.000000 nlpswift-0.0.5/nlpknife/db/redis_helper.py
-drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-27 12:31:33.887837 nlpswift-0.0.5/nlpknife/evaluation/
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      204 2024-04-27 11:37:03.000000 nlpswift-0.0.5/nlpknife/evaluation/__init__.py
-drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-27 12:31:33.888144 nlpswift-0.0.5/nlpknife/evaluation/ner_eval_core/
--rw-r--r--   0 zhpmatrix   (501) staff       (20)        0 2024-04-24 11:30:31.000000 nlpswift-0.0.5/nlpknife/evaluation/ner_eval_core/__init__.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)    23342 2024-04-24 11:30:31.000000 nlpswift-0.0.5/nlpknife/evaluation/ner_eval_core/ner_eval.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)     5005 2024-04-24 11:30:31.000000 nlpswift-0.0.5/nlpknife/evaluation/ner_evaluation.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)     3733 2024-04-27 11:05:26.000000 nlpswift-0.0.5/nlpknife/evaluation/rag_evaluation.py
-drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-27 12:31:33.888625 nlpswift-0.0.5/nlpknife/extractor/
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      155 2024-04-24 11:30:31.000000 nlpswift-0.0.5/nlpknife/extractor/__init__.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)     1014 2024-04-24 14:16:49.000000 nlpswift-0.0.5/nlpknife/extractor/json_helper.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)     2014 2024-04-27 11:40:30.000000 nlpswift-0.0.5/nlpknife/logger.py
-drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-27 12:31:33.888857 nlpswift-0.0.5/nlpknife/message/
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      269 2024-04-24 11:30:31.000000 nlpswift-0.0.5/nlpknife/message/__init__.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)     1750 2024-04-24 11:30:31.000000 nlpswift-0.0.5/nlpknife/search.py
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      449 2024-04-24 11:30:31.000000 nlpswift-0.0.5/nlpknife/timer.py
-drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-27 12:31:33.889689 nlpswift-0.0.5/nlpswift.egg-info/
--rw-r--r--   0 zhpmatrix   (501) staff       (20)     1266 2024-04-27 12:31:33.000000 nlpswift-0.0.5/nlpswift.egg-info/PKG-INFO
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      717 2024-04-27 12:31:33.000000 nlpswift-0.0.5/nlpswift.egg-info/SOURCES.txt
--rw-r--r--   0 zhpmatrix   (501) staff       (20)        1 2024-04-27 12:31:33.000000 nlpswift-0.0.5/nlpswift.egg-info/dependency_links.txt
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      125 2024-04-27 12:31:33.000000 nlpswift-0.0.5/nlpswift.egg-info/requires.txt
--rw-r--r--   0 zhpmatrix   (501) staff       (20)        9 2024-04-27 12:31:33.000000 nlpswift-0.0.5/nlpswift.egg-info/top_level.txt
--rw-r--r--   0 zhpmatrix   (501) staff       (20)       38 2024-04-27 12:31:33.890214 nlpswift-0.0.5/setup.cfg
--rw-r--r--   0 zhpmatrix   (501) staff       (20)      965 2024-04-27 12:31:28.000000 nlpswift-0.0.5/setup.py
+drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-27 12:55:38.046357 nlpswift-0.0.6/
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)     1211 2024-04-27 12:43:14.000000 nlpswift-0.0.6/LICENSE
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)     1215 2024-04-27 12:55:38.046130 nlpswift-0.0.6/PKG-INFO
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      664 2024-04-27 12:43:14.000000 nlpswift-0.0.6/README.md
+drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-27 12:55:38.042721 nlpswift-0.0.6/nlpswift/
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      320 2024-04-27 12:55:27.000000 nlpswift-0.0.6/nlpswift/__init__.py
+drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-27 12:55:38.044236 nlpswift-0.0.6/nlpswift/db/
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      157 2024-04-27 12:43:14.000000 nlpswift-0.0.6/nlpswift/db/__init__.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)        0 2024-04-27 12:43:14.000000 nlpswift-0.0.6/nlpswift/db/es_helper.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)        0 2024-04-27 12:43:14.000000 nlpswift-0.0.6/nlpswift/db/minio_helper.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)     1362 2024-04-27 12:43:14.000000 nlpswift-0.0.6/nlpswift/db/mysql_helper.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      560 2024-04-27 12:43:14.000000 nlpswift-0.0.6/nlpswift/db/neo4j_helper.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      647 2024-04-27 12:43:14.000000 nlpswift-0.0.6/nlpswift/db/redis_helper.py
+drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-27 12:55:38.044906 nlpswift-0.0.6/nlpswift/evaluation/
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      204 2024-04-27 12:43:14.000000 nlpswift-0.0.6/nlpswift/evaluation/__init__.py
+drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-27 12:55:38.045129 nlpswift-0.0.6/nlpswift/evaluation/ner_eval_core/
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)        0 2024-04-27 12:43:14.000000 nlpswift-0.0.6/nlpswift/evaluation/ner_eval_core/__init__.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)    23342 2024-04-27 12:43:14.000000 nlpswift-0.0.6/nlpswift/evaluation/ner_eval_core/ner_eval.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)     5005 2024-04-27 12:50:09.000000 nlpswift-0.0.6/nlpswift/evaluation/ner_evaluation.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)     3733 2024-04-27 12:43:14.000000 nlpswift-0.0.6/nlpswift/evaluation/rag_evaluation.py
+drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-27 12:55:38.045490 nlpswift-0.0.6/nlpswift/extractor/
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      155 2024-04-27 12:43:14.000000 nlpswift-0.0.6/nlpswift/extractor/__init__.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)     1014 2024-04-27 12:43:14.000000 nlpswift-0.0.6/nlpswift/extractor/json_helper.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)     2014 2024-04-27 12:43:14.000000 nlpswift-0.0.6/nlpswift/logger.py
+drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-27 12:55:38.045655 nlpswift-0.0.6/nlpswift/message/
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      269 2024-04-27 12:43:14.000000 nlpswift-0.0.6/nlpswift/message/__init__.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)     1750 2024-04-27 12:43:14.000000 nlpswift-0.0.6/nlpswift/search.py
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      449 2024-04-27 12:43:14.000000 nlpswift-0.0.6/nlpswift/timer.py
+drwxr-xr-x   0 zhpmatrix   (501) staff       (20)        0 2024-04-27 12:55:38.045868 nlpswift-0.0.6/nlpswift.egg-info/
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)     1215 2024-04-27 12:55:38.000000 nlpswift-0.0.6/nlpswift.egg-info/PKG-INFO
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      717 2024-04-27 12:55:38.000000 nlpswift-0.0.6/nlpswift.egg-info/SOURCES.txt
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)        1 2024-04-27 12:55:38.000000 nlpswift-0.0.6/nlpswift.egg-info/dependency_links.txt
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      104 2024-04-27 12:55:38.000000 nlpswift-0.0.6/nlpswift.egg-info/requires.txt
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)        9 2024-04-27 12:55:38.000000 nlpswift-0.0.6/nlpswift.egg-info/top_level.txt
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)       38 2024-04-27 12:55:38.046400 nlpswift-0.0.6/setup.cfg
+-rw-r--r--   0 zhpmatrix   (501) staff       (20)      965 2024-04-27 12:55:04.000000 nlpswift-0.0.6/setup.py
```

### Comparing `nlpswift-0.0.5/LICENSE` & `nlpswift-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nlpswift-0.0.5/PKG-INFO` & `nlpswift-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpswift
-Version: 0.0.5
+Version: 0.0.6
 Summary: my nlpswift
 Home-page: https://github.com/zhpmatrix/nlpknife
 Download-URL: https://pypi.tuna.tsinghua.edu.cn/simple
 Author: zhp.matrix
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,16 +15,14 @@
 Requires-Dist: redis
 Requires-Dist: baidusearch
 Requires-Dist: gunicorn
 Requires-Dist: gevent
 Requires-Dist: flask
 Requires-Dist: ragas
 Requires-Dist: langchain
-Requires-Dist: seqeval
-Requires-Dist: scikit-learn
 
 <!--
  * @Description: aka.zhp
  * @Version: 0.0.1
  * @Author: aka.zhp
  * @Date: 2024-01-04 23:38:05
  * @LastEditTime: 2024-04-23 10:43:14
@@ -44,15 +42,15 @@
 - [x] 数据库Helper
 - [x] 算法服务模版
 
 ## 安装与部署
 ### 在线安装
 
 ```shell
-pip install nlpknife
+pip install nlpswift
 ```
 ### 源码安装
 
 ```shell
 python setup.py install
 ```
```

### Comparing `nlpswift-0.0.5/README.md` & `nlpswift-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 - [x] 数据库Helper
 - [x] 算法服务模版
 
 ## 安装与部署
 ### 在线安装
 
 ```shell
-pip install nlpknife
+pip install nlpswift
 ```
 ### 源码安装
 
 ```shell
 python setup.py install
 ```
 
@@ -38,8 +38,8 @@
 ## FAQ
 
 **Q:**  ModuleNotFoundError: No module named 'zope.event'
 
 **A:**
 ```
 pip3 install --force-reinstall zope.event
-```
+```
```

### Comparing `nlpswift-0.0.5/nlpknife/db/mysql_helper.py` & `nlpswift-0.0.6/nlpswift/db/mysql_helper.py`

 * *Files identical despite different names*

### Comparing `nlpswift-0.0.5/nlpknife/db/neo4j_helper.py` & `nlpswift-0.0.6/nlpswift/db/neo4j_helper.py`

 * *Files identical despite different names*

### Comparing `nlpswift-0.0.5/nlpknife/db/redis_helper.py` & `nlpswift-0.0.6/nlpswift/db/redis_helper.py`

 * *Files identical despite different names*

### Comparing `nlpswift-0.0.5/nlpknife/evaluation/ner_eval_core/ner_eval.py` & `nlpswift-0.0.6/nlpswift/evaluation/ner_eval_core/ner_eval.py`

 * *Files identical despite different names*

### Comparing `nlpswift-0.0.5/nlpknife/evaluation/ner_evaluation.py` & `nlpswift-0.0.6/nlpswift/evaluation/ner_evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 from pprint import pprint
 
 from sklearn.metrics import classification_report as token_report
 from seqeval.metrics import classification_report as entity_report
-from nlpknife.evaluation.ner_eval_core.ner_eval import collect_named_entities
-from nlpknife.evaluation.ner_eval_core.ner_eval import Evaluator
-from nlpknife.evaluation.ner_eval_core.ner_eval import compute_metrics, collect_named_entities
+from nlpswift.evaluation.ner_eval_core.ner_eval import collect_named_entities
+from nlpswift.evaluation.ner_eval_core.ner_eval import Evaluator
+from nlpswift.evaluation.ner_eval_core.ner_eval import compute_metrics, collect_named_entities
 
 
 """
     scikit-learn=0.21.3测试通过
     REF:
         http://www.davidsbatista.net/blog/2018/05/09/Named_Entity_Evaluation/
 """
```

### Comparing `nlpswift-0.0.5/nlpknife/evaluation/rag_evaluation.py` & `nlpswift-0.0.6/nlpswift/evaluation/rag_evaluation.py`

 * *Files identical despite different names*

### Comparing `nlpswift-0.0.5/nlpknife/extractor/json_helper.py` & `nlpswift-0.0.6/nlpswift/extractor/json_helper.py`

 * *Files identical despite different names*

### Comparing `nlpswift-0.0.5/nlpknife/logger.py` & `nlpswift-0.0.6/nlpswift/logger.py`

 * *Files identical despite different names*

### Comparing `nlpswift-0.0.5/nlpknife/search.py` & `nlpswift-0.0.6/nlpswift/search.py`

 * *Files identical despite different names*

### Comparing `nlpswift-0.0.5/nlpswift.egg-info/PKG-INFO` & `nlpswift-0.0.6/nlpswift.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpswift
-Version: 0.0.5
+Version: 0.0.6
 Summary: my nlpswift
 Home-page: https://github.com/zhpmatrix/nlpknife
 Download-URL: https://pypi.tuna.tsinghua.edu.cn/simple
 Author: zhp.matrix
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,16 +15,14 @@
 Requires-Dist: redis
 Requires-Dist: baidusearch
 Requires-Dist: gunicorn
 Requires-Dist: gevent
 Requires-Dist: flask
 Requires-Dist: ragas
 Requires-Dist: langchain
-Requires-Dist: seqeval
-Requires-Dist: scikit-learn
 
 <!--
  * @Description: aka.zhp
  * @Version: 0.0.1
  * @Author: aka.zhp
  * @Date: 2024-01-04 23:38:05
  * @LastEditTime: 2024-04-23 10:43:14
@@ -44,15 +42,15 @@
 - [x] 数据库Helper
 - [x] 算法服务模版
 
 ## 安装与部署
 ### 在线安装
 
 ```shell
-pip install nlpknife
+pip install nlpswift
 ```
 ### 源码安装
 
 ```shell
 python setup.py install
 ```
```

### Comparing `nlpswift-0.0.5/setup.py` & `nlpswift-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Author: aka.zhp
 Date: 2024-01-04 21:12:45
 LastEditTime: 2024-04-23 10:16:11
 '''
 import setuptools
 import os, shutil
 from distutils.core import setup
-from nlpknife import __version__ as version
+from nlpswift import __version__ as version
 
 with open("./requirements.txt", "r") as f:
     install_requires = f.read().splitlines()
 print(install_requires)
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
```

