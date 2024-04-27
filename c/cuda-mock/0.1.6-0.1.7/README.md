# Comparing `tmp/cuda-mock-0.1.6.tar.gz` & `tmp/cuda-mock-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuda-mock-0.1.6.tar", last modified: Sun Apr 14 13:47:52 2024, max compression
+gzip compressed data, was "dist/cuda-mock-0.1.7.tar", last modified: Sat Apr 27 10:19:23 2024, max compression
```

## Comparing `cuda-mock-0.1.6.tar` & `cuda-mock-0.1.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 13:47:52.925115 cuda-mock-0.1.6/
--rw-r--r--   0 root         (0) root         (0)     1495 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3472 2024-04-14 13:47:52.925115 cuda-mock-0.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3164 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 13:47:52.917116 cuda-mock-0.1.6/include/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/GlobalVarMgr.h
--rw-r--r--   0 root         (0) root         (0)     3118 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/backtrace.h
--rw-r--r--   0 root         (0) root         (0)     1505 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/cuda_mock.h
--rw-r--r--   0 root         (0) root         (0)     3205 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/env_util.h
--rw-r--r--   0 root         (0) root         (0)    13039 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/hook.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 13:47:52.917116 cuda-mock-0.1.6/include/logger/
--rw-r--r--   0 root         (0) root         (0)     1899 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/logger/StringRef.h
--rw-r--r--   0 root         (0) root         (0)    16271 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/logger/logger.h
--rw-r--r--   0 root         (0) root         (0)      658 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/logger/logger_stl.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 13:47:52.921115 cuda-mock-0.1.6/include/profile/
--rw-r--r--   0 root         (0) root         (0)     1603 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/profile/Timer.h
--rw-r--r--   0 root         (0) root         (0)    24151 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/support.h
--rw-r--r--   0 root         (0) root         (0)      340 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/include/xpu_mock.h
--rw-r--r--   0 root         (0) root         (0)      350 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-14 13:47:52.925115 cuda-mock-0.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2516 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 13:47:52.913116 cuda-mock-0.1.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 13:47:52.921115 cuda-mock-0.1.6/src/cuda_mock/
--rw-r--r--   0 root         (0) root         (0)      147 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/src/cuda_mock/__init__.py
--rw-r--r--   0 root         (0) root         (0)      216 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/src/cuda_mock/ctypes_helper.py
--rw-r--r--   0 root         (0) root         (0)     8620 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/src/cuda_mock/cuda_mock_impl.py
--rw-r--r--   0 root         (0) root         (0)     2701 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/src/cuda_mock/dynamic_obj.py
--rw-r--r--   0 root         (0) root         (0)    16779 2024-04-14 13:37:13.000000 cuda-mock-0.1.6/src/cuda_mock/gpu_validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 13:47:52.925115 cuda-mock-0.1.6/src/cuda_mock.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3472 2024-04-14 13:47:52.000000 cuda-mock-0.1.6/src/cuda_mock.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      624 2024-04-14 13:47:52.000000 cuda-mock-0.1.6/src/cuda_mock.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 13:47:52.000000 cuda-mock-0.1.6/src/cuda_mock.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 13:37:51.000000 cuda-mock-0.1.6/src/cuda_mock.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-14 13:47:52.000000 cuda-mock-0.1.6/src/cuda_mock.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/
+-rw-r--r--   0 root         (0) root         (0)     1495 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4227 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3919 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/include/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/GlobalVarMgr.h
+-rw-r--r--   0 root         (0) root         (0)     3118 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/backtrace.h
+-rw-r--r--   0 root         (0) root         (0)     1505 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/cuda_mock.h
+-rw-r--r--   0 root         (0) root         (0)     3205 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/env_util.h
+-rw-r--r--   0 root         (0) root         (0)    13039 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/hook.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/include/logger/
+-rw-r--r--   0 root         (0) root         (0)     1899 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/logger/StringRef.h
+-rw-r--r--   0 root         (0) root         (0)    16271 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/logger/logger.h
+-rw-r--r--   0 root         (0) root         (0)      658 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/logger/logger_stl.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/include/profile/
+-rw-r--r--   0 root         (0) root         (0)     1603 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/profile/Timer.h
+-rw-r--r--   0 root         (0) root         (0)    24151 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/support.h
+-rw-r--r--   0 root         (0) root         (0)      340 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/include/xpu_mock.h
+-rw-r--r--   0 root         (0) root         (0)      350 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2516 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/src/cuda_mock/
+-rw-r--r--   0 root         (0) root         (0)      254 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/src/cuda_mock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      216 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/src/cuda_mock/ctypes_helper.py
+-rw-r--r--   0 root         (0) root         (0)     8620 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/src/cuda_mock/cuda_mock_impl.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/src/cuda_mock/dynamic_obj.py
+-rw-r--r--   0 root         (0) root         (0)    19425 2024-04-27 10:10:54.000000 cuda-mock-0.1.7/src/cuda_mock/gpu_validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/src/cuda_mock.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4227 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/src/cuda_mock.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      624 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/src/cuda_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/src/cuda_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 10:11:30.000000 cuda-mock-0.1.7/src/cuda_mock.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-27 10:19:23.000000 cuda-mock-0.1.7/src/cuda_mock.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `cuda-mock-0.1.6/LICENSE` & `cuda-mock-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.6/include/GlobalVarMgr.h` & `cuda-mock-0.1.7/include/GlobalVarMgr.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.6/include/backtrace.h` & `cuda-mock-0.1.7/include/backtrace.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.6/include/cuda_mock.h` & `cuda-mock-0.1.7/include/cuda_mock.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.6/include/env_util.h` & `cuda-mock-0.1.7/include/env_util.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.6/include/hook.h` & `cuda-mock-0.1.7/include/hook.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.6/include/logger/StringRef.h` & `cuda-mock-0.1.7/include/logger/StringRef.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.6/include/logger/logger.h` & `cuda-mock-0.1.7/include/logger/logger.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.6/include/logger/logger_stl.h` & `cuda-mock-0.1.7/include/logger/logger_stl.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.6/include/profile/Timer.h` & `cuda-mock-0.1.7/include/profile/Timer.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.6/include/support.h` & `cuda-mock-0.1.7/include/support.h`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.6/setup.py` & `cuda-mock-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
         subprocess.check_call(['cmake', f'{script_dir}'] + cmake_args + ninja_args, cwd=build_dir)
         subprocess.check_call(['cmake', '--build', '.'], cwd=build_dir)
         subprocess.check_call([f'{install_cmd}', 'install'], cwd=build_dir)
 
 setup(
     name="cuda-mock",
-    version="0.1.6",
+    version="0.1.7",
     author="lipracer",
     author_email="lipracer@gmail.com",
     description="a tools hook some api call at runtime",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
 
     url="https://github.com/lipracer/torch-cuda-mock",
```

### Comparing `cuda-mock-0.1.6/src/cuda_mock/cuda_mock_impl.py` & `cuda-mock-0.1.7/src/cuda_mock/cuda_mock_impl.py`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.6/src/cuda_mock/dynamic_obj.py` & `cuda-mock-0.1.7/src/cuda_mock/dynamic_obj.py`

 * *Files identical despite different names*

### Comparing `cuda-mock-0.1.6/src/cuda_mock/gpu_validation.py` & `cuda-mock-0.1.7/src/cuda_mock/gpu_validation.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 
 def validation_log_debug(*args):
     log(*args, 0)
 
 def validation_log_warn(*args):
     log(*args, 1)
 
+def subprocess_log(*args):
+    msg = ''
+    for arg in args:
+        msg += str(arg)
+    print(f"[{os.getpid()}]{msg}")
+
 class gpu_validation:
     global_op_index = 0
 
     def __init__(self, model_key, atol, rtol, address, port, cache_dir='/tmp', fallback=False):
         self.model_key = model_key
         self.atol = atol
         self.rtol = rtol
@@ -223,20 +229,20 @@
     def __del__(self):
         if hasattr(self, "connection"):
             self.connection.close()
         else:
             validation_log_info("has not connect")
 
 def exec_shell(command):
-    validation_log_debug(f"exec command:{command}")
+    subprocess_log(f"exec command:{command}")
     try:
         result = subprocess.run(command, shell=True, check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         return result.returncode
     except subprocess.CalledProcessError as e:
-        validation_log_warn("Error:", e)
+        subprocess_log("Error:", e)
         return -1
     return -1
 
 def sync_pull_file(address, name, cache_dir, fuzzy_matching=False):
     new_file_name = ''
     def find_file():
         nonlocal new_file_name
@@ -253,70 +259,151 @@
     while True: 
         file_list = os.popen(f"bcecmd bos ls -a {address}").read().strip()
         file_list = file_list.split('\n')
         if find_file():
             break
         time.sleep(0.5)
     bos_file_path = os.path.join(address, new_file_name)
-    exec_shell(f"bcecmd bos cp {bos_file_path} {cache_dir}/ -y")
-    validation_log_debug(f"pull file:{os.path.join(cache_dir, name)}")
+
+    try_count = 3
+    while try_count > 0:
+        if exec_shell(f"bcecmd bos cp {bos_file_path} {cache_dir}/ -y") == 0:
+            break
+        try_count -= 1
+    assert try_count >= 0, "bos_send_file send {file} fail!"
+
+    
+    validation_log_debug(f"pull file:{os.path.join(cache_dir, new_file_name)}")
 
     return os.path.join(cache_dir, new_file_name)
 
 global_bos_msg_index = 0
 
 def encode_path_msg(name, msg):
     global global_bos_msg_index
     result = f"{name}_{global_bos_msg_index}_msg_{msg}"
     global_bos_msg_index += 1
     return result
 
-def bos_send_file(obj, file):
+import multiprocessing
+from multiprocessing import Queue
+import time
+from datetime import datetime
+import shutil
+from functools import partial
+
+class TaskContext:
+    def __init__(self):
+        self.queue = Queue()
+        self.p = multiprocessing.Process(
+            target=self.task_consumer,
+            args=(),
+            kwargs={},
+        )
+        self.p.start()
+    
+    def task_consumer(self):
+        subprocess_log(f"start background process task count:{self.queue.qsize()}")
+        while True:
+            if self.queue.empty():
+                time.sleep(0.01)
+                continue
+            subprocess_log(f"remain task count:{self.queue.qsize()}")
+            task = self.queue.get()
+            if isinstance(task, TerminateTask):
+                break
+            task()
+
+    def put_task(self, task):
+        self.queue.put(task)
+    
+    def task_over(self):
+        validation_log_info("task over wait sync file!")
+        self.queue.put(TerminateTask())
+        self.p.join()
+
+def uninitialize():
+    gTaskContext.task_over()
+
+import atexit
+atexit.register(uninitialize)
+
+class SimpleTask:
+    def __init__(self, file, dst_path):
+        self.file = file
+        self.dst_path = dst_path
+
+    def __call__(self):
+        try_count = 3
+        while try_count > 0:
+            if exec_shell(f"bcecmd bos cp {self.file} {self.dst_path} -y") == 0:
+                exec_shell(f"rm -f {self.file}")
+                break
+            try_count -= 1
+        assert try_count >= 0, "bos_send_file send {file} fail!"
+
+class TerminateTask:
+    pass
+
+
+gTaskContext = TaskContext()
+
+def bos_send_file_impl(obj, file):
     try_count = 3
     while try_count > 0:
         if exec_shell(f"bcecmd bos cp {file} {obj.address} -y") == 0:
             break
         try_count -= 1
     assert try_count >= 0, "bos_send_file send {file} fail!"
+        
+
+def bos_send_file(obj, file, sync=True):
+    if sync:
+        bos_send_file_impl(obj, file)
+    else:
+        gTaskContext.put_task(SimpleTask(file, obj.address))
 
-def bos_send_msg(obj, msg):
+
+def bos_send_msg(obj, msg, sync=True):
     msg_path = encode_path_msg(obj.get_tensor_file_path(), msg)
     with open(msg_path, "wt+") as f:
         f.write(msg)
-    bos_send_file(obj, msg_path)
+    bos_send_file(obj, msg_path, sync)
 
 def bos_recv_msg(obj):
     global global_bos_msg_index
     op_name_path = sync_pull_file(obj.address, f"{obj.get_tensor_file_name()}_{global_bos_msg_index}_msg_", obj.cache_dir, True)
     global_bos_msg_index += 1
     op_name = ''
     with open(op_name_path, "rt+") as f:
         op_name = f.read().strip()
     bos_name = op_name_path.split('/')[-1]
-    assert exec_shell(f"bcecmd bos rm {os.path.join(obj.address, bos_name)} -y")==0, "clear msg fail!"
+    # assert exec_shell(f"bcecmd bos rm {os.path.join(obj.address, bos_name)} -y")==0, "clear msg fail!"
     return op_name
 
 
 class bos_gpu_validation_master(gpu_validation_master):
     def __init__(self, model_key, atol, rtol, address, port, cache_dir='/tmp', fallback=False, offline=False):
         super().__init__(model_key, atol, rtol, address, port, cache_dir, fallback)
         if not self.address.endswith('/'):
             self.address += '/'
         self.offline = offline
 
     def recv_msg_impl(self):
         return bos_recv_msg(self)
 
     def send_msg_impl(self, msg):
-        bos_send_msg(self, msg)
+        sync = False if self.offline else True
+        bos_send_msg(self, msg, sync)
 
     def send_tensor_impl(self, tensor):
         validation_log_info(self.get_tensor_file_path())
         torch.save(tensor, self.get_tensor_file_path())
-        bos_send_file(self, self.get_tensor_file_path())
+        sync = False if self.offline else True
+        bos_send_file(self, self.get_tensor_file_path(), sync)
 
     def recv_tensor_impl(self):
         tensor_path = sync_pull_file(self.address, self.get_tensor_file_name(), self.cache_dir)
         return torch.load(tensor_path)
 
     def recv_result_impl(self):
         if self.offline:
@@ -328,27 +415,32 @@
     def __init__(self, model_key, atol, rtol, address, port, cache_dir='/tmp', fallback=False, offline=False):
         super().__init__(model_key, atol, rtol, address, port, cache_dir, fallback)
         if not self.address.endswith('/'):
             self.address += '/'
         self.offline = offline
 
     def send_msg_impl(self, msg):
-        bos_send_msg(self, msg)
+        sync = False if self.offline else True
+        bos_send_msg(self, msg, sync)
 
     def recv_msg_impl(self):
         return bos_recv_msg(self)
 
     def send_tensor_impl(self, tensor):
         validation_log_info(self.get_tensor_file_path())
         torch.save(tensor, self.get_tensor_file_path())
-        bos_send_file(self, self.get_tensor_file_path())
+        sync = False if self.offline else True
+        bos_send_file(self, self.get_tensor_file_path(), sync)
 
     def recv_tensor_impl(self):
         tensor_path = sync_pull_file(self.address, self.get_tensor_file_name(), self.cache_dir)
-        return torch.load(tensor_path)
+        tensor = torch.load(tensor_path)
+        exec_shell(f"rm -f {tensor_path}")
+        return tensor
+
 
     def send_result_impl(self, result):
         if self.offline:
             return
         return self.send_msg_impl(result)
 
 token = "test6"
@@ -402,55 +494,61 @@
     validation.increase_index()
 
 import torch
 from torch.utils._pytree import tree_flatten, tree_map
 import functools
 from torch.utils._python_dispatch import TorchDispatchMode
 
+is_nvidia_gpu = os.environ.get('CUDA_VERSION', None) or os.environ.get('NVIDIA_VISIBLE_DEVICES', None)
+validation_filter_port = os.environ.get('VALIDATION_FILTER_PORT', None)
+
 class GpuValidation(TorchDispatchMode):
     '''
     master is the device will be validation
     client is golden device 
     '''
-    def __init__(self, is_gpu, model_key, atol, rtol, address, port=SOCKET_PORT, cache_dir='/tmp', use_bos=False, fallback=False, offline=False):
-        self.is_gpu = is_gpu
+    def __init__(self, model_key, atol, rtol, address, port=SOCKET_PORT, cache_dir='/tmp', use_bos=True, fallback=False, offline=True):
+        self.is_gpu = is_nvidia_gpu
         self.fallback = fallback
         self.offline = offline
         if not use_bos:
             master = socket_gpu_validation_master
             client = socket_gpu_validation_client
         else:
             master = bos_gpu_validation_master
             client = bos_gpu_validation_client
-        if is_gpu:
+        if self.is_gpu:
             self.validation = client(model_key, atol, rtol, address, port, cache_dir, fallback, offline=offline)
             validation_log_debug(f"initialize client validation completed!")
         else:
             self.validation = master(model_key, atol, rtol, address, port, cache_dir, fallback, offline=offline)
             validation_log_debug(f"initialize master validation completed!")
 
     def __torch_dispatch__(self, op, types, dev_args=(), dev_kwargs=None):
         validation_log_info(f"will call op:{op}")
 
         result = op(*dev_args, **dev_kwargs)
+
+        if validation_filter_port:
+            if self.validation.port != int(validation_filter_port):
+                return result
         
         if isinstance(result, torch.Tensor):
             self.validation.validate(result, f"{op}")
             if not self.offline or self.is_gpu:
                 validation_log_info(f"validate op:{op} dtype:{result.dtype} shape:{result.shape} result:{self.validation.result}")
             if self.fallback and not self.is_gpu:
                 self.validation.increase_index()
                 return self.validation.golden_result
             self.validation.increase_index()
         else:
             validation_log_info(f'skip not tensor result:{type(result)} op:{op}')
 
         return result
 
-
 import torch
 import torch.nn as nn
 
 class SimpleNN(nn.Module):
     def __init__(self, input_size, hidden_size, output_size):
         super(SimpleNN, self).__init__()
         self.fc1 = nn.Linear(input_size, hidden_size)  # 输入层到隐藏层的全连接层
@@ -460,15 +558,15 @@
     def forward(self, x):
         x = self.fc1(x)  # 输入层到隐藏层的线性变换
         x = self.relu(x)  # 非线性激活函数
         x = self.fc2(x)  # 隐藏层到输出层的线性变换
         return x
 
 def mytest_validation_master():
-    with GpuValidation(False, token, 1e-3, 1e-3, "127.0.0.1", SOCKET_PORT, './'):
+    with GpuValidation(token, 1e-3, 1e-3, "", SOCKET_PORT, './'):
         input_size = 5
         hidden_size = 10
         output_size = 2
         model = SimpleNN(input_size, hidden_size, output_size)
 
         # 准备输入数据
         input_data = torch.randn(3, input_size)  # 创建一个3x5的随机输入张量
@@ -476,15 +574,15 @@
         # 将输入数据传递给模型，获取模型的输出
         output = model(input_data)
 
         # 打印模型输出
         print("模型输出：", output)
 
 def mytest_validation_client():
-    with GpuValidation(True, token, 1e-3, 1e-3, "127.0.0.1", SOCKET_PORT):
+    with GpuValidation(token, 1e-3, 1e-3, "", SOCKET_PORT):
         input_size = 5
         hidden_size = 10
         output_size = 2
         model = SimpleNN(input_size, hidden_size, output_size)
 
         # 准备输入数据
         input_data = torch.randn(3, input_size)  # 创建一个3x5的随机输入张量
```

### Comparing `cuda-mock-0.1.6/src/cuda_mock.egg-info/SOURCES.txt` & `cuda-mock-0.1.7/src/cuda_mock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

