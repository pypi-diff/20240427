# Comparing `tmp/flowdata-0.1.3.tar.gz` & `tmp/flowdata-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flowdata-0.1.3.tar", last modified: Mon Apr 22 01:52:54 2024, max compression
+gzip compressed data, was "dist/flowdata-0.1.4.tar", last modified: Sat Apr 27 01:42:23 2024, max compression
```

## Comparing `flowdata-0.1.3.tar` & `flowdata-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 01:52:54.000000 flowdata-0.1.3/
--rw-r--r--   0 root         (0) root         (0)     2477 2024-04-22 01:52:54.000000 flowdata-0.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1592 2024-04-22 01:51:41.000000 flowdata-0.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 01:52:54.000000 flowdata-0.1.3/flowdata/
--rw-r--r--   0 root         (0) root         (0)      107 2024-04-20 13:02:13.000000 flowdata-0.1.3/flowdata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4201 2024-04-22 01:39:39.000000 flowdata-0.1.3/flowdata/_io.py
--rw-r--r--   0 root         (0) root         (0)     1128 2024-04-19 12:06:46.000000 flowdata-0.1.3/flowdata/_logger.py
--rw-r--r--   0 root         (0) root         (0)     3501 2024-04-21 03:41:45.000000 flowdata-0.1.3/flowdata/data_flow.py
--rw-r--r--   0 root         (0) root         (0)     2931 2024-04-21 03:02:04.000000 flowdata-0.1.3/flowdata/data_parallel.py
--rw-r--r--   0 root         (0) root         (0)     6187 2024-04-20 12:40:02.000000 flowdata-0.1.3/flowdata/decorator.py
--rw-r--r--   0 root         (0) root         (0)      809 2024-04-21 03:33:07.000000 flowdata-0.1.3/flowdata/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 01:52:54.000000 flowdata-0.1.3/flowdata.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2477 2024-04-22 01:52:53.000000 flowdata-0.1.3/flowdata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      379 2024-04-22 01:52:53.000000 flowdata-0.1.3/flowdata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 01:52:53.000000 flowdata-0.1.3/flowdata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-22 01:52:53.000000 flowdata-0.1.3/flowdata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-22 01:52:53.000000 flowdata-0.1.3/flowdata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 01:52:54.000000 flowdata-0.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      710 2024-04-22 01:52:41.000000 flowdata-0.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 01:52:54.000000 flowdata-0.1.3/test/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 03:35:00.000000 flowdata-0.1.3/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      709 2024-04-21 03:41:25.000000 flowdata-0.1.3/test/test_flow.py
--rw-r--r--   0 root         (0) root         (0)      884 2024-04-21 02:48:07.000000 flowdata-0.1.3/test/test_multitask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 01:42:23.000000 flowdata-0.1.4/
+-rw-r--r--   0 root         (0) root         (0)     2477 2024-04-27 01:42:23.000000 flowdata-0.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1592 2024-04-22 01:51:41.000000 flowdata-0.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 01:42:23.000000 flowdata-0.1.4/flowdata/
+-rw-r--r--   0 root         (0) root         (0)      160 2024-04-26 08:43:39.000000 flowdata-0.1.4/flowdata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4201 2024-04-22 01:39:39.000000 flowdata-0.1.4/flowdata/_io.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-19 12:06:46.000000 flowdata-0.1.4/flowdata/_logger.py
+-rw-r--r--   0 root         (0) root         (0)     3515 2024-04-26 08:30:15.000000 flowdata-0.1.4/flowdata/data_flow.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2024-04-24 01:48:18.000000 flowdata-0.1.4/flowdata/data_parallel.py
+-rw-r--r--   0 root         (0) root         (0)     6737 2024-04-22 12:36:13.000000 flowdata-0.1.4/flowdata/decorator.py
+-rw-r--r--   0 root         (0) root         (0)      874 2024-04-26 08:43:27.000000 flowdata-0.1.4/flowdata/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 01:42:23.000000 flowdata-0.1.4/flowdata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2477 2024-04-27 01:42:23.000000 flowdata-0.1.4/flowdata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-27 01:42:23.000000 flowdata-0.1.4/flowdata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 01:42:23.000000 flowdata-0.1.4/flowdata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-27 01:42:23.000000 flowdata-0.1.4/flowdata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-27 01:42:23.000000 flowdata-0.1.4/flowdata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 01:42:23.000000 flowdata-0.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      710 2024-04-22 12:22:04.000000 flowdata-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 01:42:23.000000 flowdata-0.1.4/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 03:35:00.000000 flowdata-0.1.4/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      580 2024-04-22 12:43:00.000000 flowdata-0.1.4/test/test_dataParallel.py
+-rw-r--r--   0 root         (0) root         (0)      709 2024-04-21 03:41:25.000000 flowdata-0.1.4/test/test_flow.py
+-rw-r--r--   0 root         (0) root         (0)      884 2024-04-21 02:48:07.000000 flowdata-0.1.4/test/test_multitask.py
```

### Comparing `flowdata-0.1.3/PKG-INFO` & `flowdata-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowdata
-Version: 0.1.3
+Version: 0.1.4
 Summary: 流式数据简易处理包
 Home-page: https://github.com/zouweidong91/flowdata
 Author: zouweidong
 Author-email: zouweidong72@gmail.com
 License: UNKNOWN
 Description: # flowdata
         流式数据简易处理工具
```

### Comparing `flowdata-0.1.3/README.md` & `flowdata-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `flowdata-0.1.3/flowdata/_io.py` & `flowdata-0.1.4/flowdata/_io.py`

 * *Files identical despite different names*

### Comparing `flowdata-0.1.3/flowdata/_logger.py` & `flowdata-0.1.4/flowdata/_logger.py`

 * *Files identical despite different names*

### Comparing `flowdata-0.1.3/flowdata/data_flow.py` & `flowdata-0.1.4/flowdata/data_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,17 +37,19 @@
         num = 0
         for i, item in enumerate(item_iter):
 
             if i < offset: continue
             num += 1
             if head_num and num > head_num: break
             
-            yield item
             if self.verbose:
                 logger.info("准备处理第%s条数据", i)
+            
+            yield item
+
         
 
     def count_data(self, item_iter):
         """任务执行统计
         """
         for item in item_iter:
             self.counter['total_num'] += 1
```

### Comparing `flowdata-0.1.3/flowdata/data_parallel.py` & `flowdata-0.1.4/flowdata/data_parallel.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,60 +26,60 @@
         """
         self.item_iter_fn = item_iter_fn
         self.work_num = work_num
         self.process_fn = process_fn
         self.args = args
         self.kwargs = kwargs
 
-        self.pip_in = mp.Queue(MAX_QUEUE_SIZE)  # 输入pip
-        self.pip_out = mp.Queue(MAX_QUEUE_SIZE)  # 数据处理后输出pip   
+        self.queue_in = mp.Queue(MAX_QUEUE_SIZE)  # 接收数据的queue
+        self.queue_out = mp.Queue(MAX_QUEUE_SIZE)  # 数据处理后输出queue  
         self.p_list: List[mp.Process] = []
         
 
     @interrupt_catch
     def recv_data(self):
         """数据放入队列
         """
         for item in self.item_iter_fn():
-            self.pip_in.put(item)
-        self.pip_in.put(FLAG.END)   # 队列放入终止标志
+            self.queue_in.put(item)
+        self.queue_in.put(FLAG.END)   # 队列放入终止标志
 
 
     def send_data(self):
         """数据从队列取出
         """
         while True:
-            data = self.pip_out.get(block=True, timeout=None)
+            data = self.queue_out.get(block=True, timeout=None)
             if data == FLAG.END:
                 break
             yield data
       
 
     @interrupt_catch
     def work(self, work_done_value, work_i:int):
         """[summary]
 
         Args:
             work_done_value ([type]): [跟踪子进程是否结束]
             work_i ([int]): [进程索引id，外部任务可能用到]
         """
         while True:
-            data = self.pip_in.get(block=True, timeout=None)
+            data = self.queue_in.get(block=True, timeout=None)
             if data == FLAG.END:
-                self.pip_in.put(FLAG.END)  # 解决多进程退出问题
+                self.queue_in.put(FLAG.END)  # 解决多进程退出问题
                 break
 
             data = self.process_fn(data, work_i=work_i, *self.args, **self.kwargs)
-            self.pip_out.put(data)
+            self.queue_out.put(data)
 
         with work_done_value.get_lock():
             work_done_value.value += 1
 
             if work_done_value.value >= self.work_num:
-                self.pip_out.put(FLAG.END)   # 队列放入终止标志
+                self.queue_out.put(FLAG.END)   # 队列放入终止标志
 
 
     def run(self):
         # 接收数据进程
         recv_p = mp.Process(target = self.recv_data)
         recv_p.start()
         self.p_list.append(recv_p)
```

### Comparing `flowdata-0.1.3/flowdata/decorator.py` & `flowdata-0.1.4/flowdata/decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 """
 常用装饰器
 """
-
 import functools
 import os
 import threading
 import time
 import traceback
+from concurrent import futures
 
 from ._logger import logger
 
 
 def timer(info="", threshold=0.5):
     """计时器
 
@@ -34,14 +34,27 @@
                     logger.warning(f'执行函数[%s]%s，耗时 %f 秒 进程号 %s，线程号 %s', func.__name__, f"[info: {info}]" if info else "",
                                 time.time() - start, os.getpid(), threading.currentThread().ident)
             return res
         return wrapper
     return _timer
 
 
+# 超时判断 此种方式只是会跑出超时异常，但是func依然会继续执行，直到结束
+# task_fn加上此装饰器，解决torch与python多进程不兼容导致卡死 ？？
+def timeout(seconds=10000, works=2):
+    executor = futures.ThreadPoolExecutor(works)
+    def decorator(func):
+        @functools.wraps(func)
+        def wrapper(*args, **kw):
+            future = executor.submit(func, *args, **kw)
+            return future.result(timeout=seconds)
+        return wrapper
+    return decorator
+
+
 def err_catch(info="", level='error'):
     """异常捕获装饰器
 
     Args:
         info (str, optional): 辅助日志. Defaults to "".
         level (str, optional): 异常信息等级. Defaults to 'error'.
     """
```

### Comparing `flowdata-0.1.3/flowdata/task.py` & `flowdata-0.1.4/flowdata/task.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,7 +22,12 @@
         )
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
         return wrapper
     return _add_task
 
+
+
+def clear_task():
+    while TASK_LIST:
+        TASK_LIST.pop()
```

### Comparing `flowdata-0.1.3/flowdata.egg-info/PKG-INFO` & `flowdata-0.1.4/flowdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowdata
-Version: 0.1.3
+Version: 0.1.4
 Summary: 流式数据简易处理包
 Home-page: https://github.com/zouweidong91/flowdata
 Author: zouweidong
 Author-email: zouweidong72@gmail.com
 License: UNKNOWN
 Description: # flowdata
         流式数据简易处理工具
```

### Comparing `flowdata-0.1.3/setup.py` & `flowdata-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 NAME = 'flowdata'
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = '流式数据简易处理包'
 EMAIL = 'zouweidong72@gmail.com'
 AUTHOR = 'zouweidong'
 
 
 setup(
     name=NAME,
```

### Comparing `flowdata-0.1.3/test/test_flow.py` & `flowdata-0.1.4/test/test_flow.py`

 * *Files identical despite different names*

### Comparing `flowdata-0.1.3/test/test_multitask.py` & `flowdata-0.1.4/test/test_multitask.py`

 * *Files identical despite different names*

