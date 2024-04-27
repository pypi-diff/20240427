# Comparing `tmp/python_alist-0.0.9.8.1.tar.gz` & `tmp/python_alist-0.0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_alist-0.0.9.8.1.tar", max compression
+gzip compressed data, was "python_alist-0.0.9.9.tar", max compression
```

## Comparing `python_alist-0.0.9.8.1.tar` & `python_alist-0.0.9.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_alist-0.0.9.8.1/LICENSE
--rw-r--r--   0        0        0   121010 2023-12-29 07:39:14.838684 python_alist-0.0.9.8.1/alist/__init__.py
--rw-r--r--   0        0        0       87 2023-12-19 14:24:48.850918 python_alist-0.0.9.8.1/alist/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_alist-0.0.9.8.1/alist/util/_init_mimetypes.py
--rw-r--r--   0        0        0    13056 2023-12-14 09:14:41.064229 python_alist-0.0.9.8.1/alist/util/download.py
--rw-r--r--   0        0        0    12845 2023-12-29 08:16:16.677384 python_alist-0.0.9.8.1/alist/util/file.py
--rw-r--r--   0        0        0     7277 2023-12-30 05:04:08.462757 python_alist-0.0.9.8.1/alist/util/ignore.py
--rw-r--r--   0        0        0      678 2023-12-19 11:57:30.557217 python_alist-0.0.9.8.1/alist/util/iter.py
--rw-r--r--   0        0        0     1795 2023-12-14 11:01:07.350145 python_alist-0.0.9.8.1/alist/util/property.py
--rw-r--r--   0        0        0     2751 2023-12-29 05:26:01.836028 python_alist-0.0.9.8.1/alist/util/response.py
--rw-r--r--   0        0        0     5230 2023-12-19 14:03:21.120801 python_alist-0.0.9.8.1/alist/util/text.py
--rw-r--r--   0        0        0     2114 2023-12-10 10:45:36.285664 python_alist-0.0.9.8.1/alist/util/urlopen.py
--rw-r--r--   0        0        0     1208 2023-12-30 05:07:09.763398 python_alist-0.0.9.8.1/pyproject.toml
--rw-r--r--   0        0        0    23318 2023-12-29 08:04:11.889075 python_alist-0.0.9.8.1/readme.md
--rw-r--r--   0        0        0    24505 1970-01-01 00:00:00.000000 python_alist-0.0.9.8.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_alist-0.0.9.9/LICENSE
+-rw-r--r--   0        0        0   136178 2024-01-12 04:00:08.605975 python_alist-0.0.9.9/alist/__init__.py
+-rw-r--r--   0        0        0       87 2023-12-19 14:24:48.850918 python_alist-0.0.9.9/alist/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_alist-0.0.9.9/alist/util/_init_mimetypes.py
+-rw-r--r--   0        0        0    13056 2023-12-14 09:14:41.064229 python_alist-0.0.9.9/alist/util/download.py
+-rw-r--r--   0        0        0    12845 2023-12-29 08:16:16.677384 python_alist-0.0.9.9/alist/util/file.py
+-rw-r--r--   0        0        0     7277 2023-12-30 05:04:08.462757 python_alist-0.0.9.9/alist/util/ignore.py
+-rw-r--r--   0        0        0      678 2023-12-19 11:57:30.557217 python_alist-0.0.9.9/alist/util/iter.py
+-rw-r--r--   0        0        0     1795 2023-12-14 11:01:07.350145 python_alist-0.0.9.9/alist/util/property.py
+-rw-r--r--   0        0        0     2751 2023-12-29 05:26:01.836028 python_alist-0.0.9.9/alist/util/response.py
+-rw-r--r--   0        0        0     5230 2023-12-19 14:03:21.120801 python_alist-0.0.9.9/alist/util/text.py
+-rw-r--r--   0        0        0     2114 2023-12-10 10:45:36.285664 python_alist-0.0.9.9/alist/util/urlopen.py
+-rw-r--r--   0        0        0     1206 2024-01-12 04:04:30.702528 python_alist-0.0.9.9/pyproject.toml
+-rw-r--r--   0        0        0    23318 2023-12-29 08:04:11.889075 python_alist-0.0.9.9/readme.md
+-rw-r--r--   0        0        0    24503 1970-01-01 00:00:00.000000 python_alist-0.0.9.9/PKG-INFO
```

### Comparing `python_alist-0.0.9.8.1/LICENSE` & `python_alist-0.0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python_alist-0.0.9.8.1/alist/__init__.py` & `python_alist-0.0.9.9/alist/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -246,14 +246,95 @@
             if not 200 <= resp["code"] < 300:
                 raise PermissionError(errno.EACCES, resp)
             self.async_session.headers["Authorization"] = self.session.headers["Authorization"] = resp["data"]["token"]
         else:
             self.session.headers.pop("Authorization", None)
             self.async_session.headers.pop("Authorization", None)
 
+    # Undocumented
+
+    def me_update(
+        self, 
+        /, 
+        payload: dict, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        return self.request(
+            "/api/me/update", 
+            json=payload, 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_index_progress(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        return self.request(
+            "/api/admin/index/progress", 
+            "GET", 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_index_build(
+        self, 
+        /, 
+        payload: dict, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        return self.request(
+            "/api/admin/index/build", 
+            json=payload, 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_index_clear(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        return self.request(
+            "/api/admin/index/clear", 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_index_stop(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        return self.request(
+            "/api/admin/index/stop", 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_index_update(
+        self, 
+        /, 
+        payload: dict, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        return self.request(
+            "/api/admin/index/update", 
+            json=payload, 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
     # [auth](https://alist.nn.ci/guide/api/auth.html)
 
     def auth_login(
         self, 
         /, 
         payload: dict, 
         async_: bool = False, 
@@ -399,26 +480,28 @@
         return self.request(
             "/api/fs/mkdir", 
             json=payload, 
             async_=async_, 
             **request_kwargs, 
         )
 
-    # NOTE: AList 改名的限制：
-    #   1. 受到网盘的改名限制，例如如果挂载的是 115，就不能包含特殊符号 " < > ，也不能改扩展名，各个网盘限制不同
-    #   2. 可以包含斜杠  \，但是改名后，这个文件不能被删改了，因为只能被罗列，但不能单独找到
-    #   3. 名字里（basename）中包含 /，会被替换为 |
     def fs_rename(
         self, 
         /, 
         payload: dict, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
-        "https://alist.nn.ci/guide/api/fs.html#post-重命名文件"
+        """https://alist.nn.ci/guide/api/fs.html#post-重命名文件
+
+        NOTE: AList 改名的限制：
+        1. 受到网盘的改名限制，例如如果挂载的是 115，就不能包含特殊符号 " < > ，也不能改扩展名，各个网盘限制不同
+        2. 可以包含斜杠  \，但是改名后，这个文件不能被删改了，因为只能被罗列，但不能单独找到
+        3. 名字里（basename）中包含 /，会被替换为 |
+        """
         return self.request(
             "/api/fs/rename", 
             json=payload, 
             async_=async_, 
             **request_kwargs, 
         )
 
@@ -551,28 +634,30 @@
         return self.request(
             "/api/fs/recursive_move", 
             json=payload, 
             async_=async_, 
             **request_kwargs, 
         )
 
-    # NOTE: AList 上传时的问题：
-    #   1. 上传文件成功不会更新缓存，但新增文件夹会更新缓存
-    #   2. 上传时路径中包含斜杠 \，视为路径分隔符 /
-    #   3. put 接口是流式上传，但是不支持 chunked，目前用 requests 上传空文件为处理为 chunked，会报错，这是 requests 的问题
     def fs_put(
         self, 
         /, 
         local_path_or_file: bytes | str | PathLike | SupportsRead[bytes] | TextIOWrapper, 
         remote_path: str, 
         as_task: bool = False, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
-        "https://alist.nn.ci/guide/api/fs.html#put-流式上传文件"
+        """https://alist.nn.ci/guide/api/fs.html#put-流式上传文件
+
+        NOTE: AList 上传的限制：
+        1. 上传文件成功不会更新缓存，但新增文件夹会更新缓存
+        2. 上传时路径中包含斜杠 \，视为路径分隔符 /
+        3. put 接口是流式上传，但是不支持 chunked，目前用 requests 上传空文件为处理为 chunked，会报错，这是 requests 的问题
+        """
         headers = request_kwargs.setdefault("headers", {})
         headers["File-Path"] = quote(remote_path)
         if as_task:
             headers["As-Task"] = "true"
         if hasattr(local_path_or_file, "read"):
             file = local_path_or_file
             if isinstance(file, TextIOWrapper):
@@ -1209,14 +1294,27 @@
         return self.request(
             "/api/admin/task/upload/retry", 
             params=payload, 
             async_=async_, 
             **request_kwargs, 
         )
 
+    def admin_task_upload_retry_failed(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "Undocumented"
+        return self.request(
+            "/api/admin/task/upload/retry_failed", 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
     def admin_task_upload_clear_done(
         self, 
         /, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
         "https://alist.nn.ci/guide/api/admin/task.html#post-清除已完成任务"
@@ -1235,14 +1333,369 @@
         "https://alist.nn.ci/guide/api/admin/task.html#post-清除已成功任务"
         return self.request(
             "/api/admin/task/upload/clear_succeeded", 
             async_=async_, 
             **request_kwargs, 
         )
 
+    def admin_task_copy_done(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#get-获取已完成任务"
+        return self.request(
+            "/api/admin/task/copy/done", 
+            "GET", 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_copy_undone(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#get-获取未完成任务"
+        return self.request(
+            "/api/admin/task/copy/undone", 
+            "GET", 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_copy_delete(
+        self, 
+        /, 
+        payload: int | str | dict, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#post-删除任务"
+        if isinstance(payload, (int, str)):
+            payload = {"tid": payload}
+        return self.request(
+            "/api/admin/task/copy/delete", 
+            params=payload, 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_copy_cancel(
+        self, 
+        /, 
+        payload: int | str | dict, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#post-取消任务"
+        if isinstance(payload, (int, str)):
+            payload = {"tid": payload}
+        return self.request(
+            "/api/admin/task/copy/cancel", 
+            params=payload, 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_copy_retry(
+        self, 
+        /, 
+        payload: int | str | dict, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#post-重试任务"
+        if isinstance(payload, (int, str)):
+            payload = {"tid": payload}
+        return self.request(
+            "/api/admin/task/copy/retry", 
+            params=payload, 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_copy_retry_failed(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "Undocumented"
+        return self.request(
+            "/api/admin/task/copy/retry_failed", 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_copy_clear_done(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#post-清除已完成任务"
+        return self.request(
+            "/api/admin/task/copy/clear_done", 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_copy_clear_succeeded(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#post-清除已成功任务"
+        return self.request(
+            "/api/admin/task/copy/clear_succeeded", 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_offline_download_done(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#get-获取已完成任务"
+        return self.request(
+            "/api/admin/task/offline_download/done", 
+            "GET", 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_offline_download_undone(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#get-获取未完成任务"
+        return self.request(
+            "/api/admin/task/offline_download/undone", 
+            "GET", 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_offline_download_delete(
+        self, 
+        /, 
+        payload: int | str | dict, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#post-删除任务"
+        if isinstance(payload, (int, str)):
+            payload = {"tid": payload}
+        return self.request(
+            "/api/admin/task/offline_download/delete", 
+            params=payload, 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_offline_download_cancel(
+        self, 
+        /, 
+        payload: int | str | dict, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#post-取消任务"
+        if isinstance(payload, (int, str)):
+            payload = {"tid": payload}
+        return self.request(
+            "/api/admin/task/offline_download/cancel", 
+            params=payload, 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_offline_download_retry(
+        self, 
+        /, 
+        payload: int | str | dict, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#post-重试任务"
+        if isinstance(payload, (int, str)):
+            payload = {"tid": payload}
+        return self.request(
+            "/api/admin/task/offline_download/retry", 
+            params=payload, 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_offline_download_retry_failed(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "Undocumented"
+        return self.request(
+            "/api/admin/task/offline_download/retry_failed", 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_offline_download_clear_done(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#post-清除已完成任务"
+        return self.request(
+            "/api/admin/task/offline_download/clear_done", 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_offline_download_clear_succeeded(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#post-清除已成功任务"
+        return self.request(
+            "/api/admin/task/offline_download/clear_succeeded", 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+
+    def admin_task_offline_download_transfer_done(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#get-获取已完成任务"
+        return self.request(
+            "/api/admin/task/offline_download_transfer/done", 
+            "GET", 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_offline_download_transfer_undone(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#get-获取未完成任务"
+        return self.request(
+            "/api/admin/task/offline_download_transfer/undone", 
+            "GET", 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_offline_download_transfer_delete(
+        self, 
+        /, 
+        payload: int | str | dict, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#post-删除任务"
+        if isinstance(payload, (int, str)):
+            payload = {"tid": payload}
+        return self.request(
+            "/api/admin/task/offline_download_transfer/delete", 
+            params=payload, 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_offline_download_transfer_cancel(
+        self, 
+        /, 
+        payload: int | str | dict, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#post-取消任务"
+        if isinstance(payload, (int, str)):
+            payload = {"tid": payload}
+        return self.request(
+            "/api/admin/task/offline_download_transfer/cancel", 
+            params=payload, 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_offline_download_transfer_retry(
+        self, 
+        /, 
+        payload: int | str | dict, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#post-重试任务"
+        if isinstance(payload, (int, str)):
+            payload = {"tid": payload}
+        return self.request(
+            "/api/admin/task/offline_download_transfer/retry", 
+            params=payload, 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_offline_download_transfer_retry_failed(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "Undocumented"
+        return self.request(
+            "/api/admin/task/offline_download_transfer/retry_failed", 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_offline_download_transfer_clear_done(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#post-清除已完成任务"
+        return self.request(
+            "/api/admin/task/offline_download_transfer/clear_done", 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
+    def admin_task_offline_download_transfer_clear_succeeded(
+        self, 
+        /, 
+        async_: bool = False, 
+        **request_kwargs, 
+    ) -> dict:
+        "https://alist.nn.ci/guide/api/admin/task.html#post-清除已成功任务"
+        return self.request(
+            "/api/admin/task/offline_download_transfer/clear_succeeded", 
+            async_=async_, 
+            **request_kwargs, 
+        )
+
     ########## Other Encapsulations ##########
 
     @cached_property
     def fs(self, /) -> AlistFileSystem:
         return AlistFileSystem(self)
 
     def get_url(self, /, path: str) -> str:
@@ -1457,34 +1910,20 @@
         if dst_password is None:
             dst_password = self.password
         dst = self.fs.copy(
             self, 
             dst_path, 
             dst_password=dst_password, 
             overwrite_or_ignore=overwrite_or_ignore, 
+            recursive=True, 
         )
         if not dst:
             return None
         return type(self)(self.fs, dst, dst_password)
 
-    def copytree(
-        self, 
-        /, 
-        dst_dir: str | PathLike[str], 
-        dst_password: Optional[str] = None, 
-    ) -> AlistPath:
-        if dst_password is None:
-            dst_password = self.password
-        dst = self.fs.copytree(
-            self, 
-            dst_dir, 
-            dst_password=dst_password, 
-        )
-        return type(self)(self.fs, dst, dst_password)
-
     def download(
         self, 
         /, 
         local_dir: bytes | str | PathLike = "", 
         no_root: bool = False, 
         write_mode: Literal["", "x", "w", "a"] = "w", 
         download: Optional[Callable[[str, SupportsWrite[bytes]], Any]] = None, 
@@ -2222,16 +2661,16 @@
         }
         return self.client.fs_regex_rename(payload, **self.request_kwargs)
 
     @check_response
     def fs_remove(
         self, 
         /, 
+        src_dir: str | PathLike[str], 
         names: list[str], 
-        src_dir: str | PathLike[str] = "", 
         _check: bool = True, 
     ) -> dict:
         if not names:
             return {"code": 200}
         if isinstance(src_dir, AlistPath):
             src_dir = src_dir.path
         elif _check:
@@ -2380,14 +2819,15 @@
         self, 
         /, 
         src_path: str | PathLike[str], 
         dst_path: str | PathLike[str], 
         src_password: str = "", 
         dst_password: str = "", 
         overwrite_or_ignore: Optional[bool] = None, 
+        recursive: bool = False, 
         _check: bool = True, 
     ) -> Optional[str]:
         if isinstance(src_path, AlistPath):
             if not src_password:
                 src_password = src_path.password
             src_path = src_path.path
         elif _check:
@@ -2396,85 +2836,169 @@
             if not dst_password:
                 dst_password = dst_path.password
             dst_path = dst_path.path
         elif _check:
             dst_path = self.abspath(dst_path)
         src_path = cast(str, src_path)
         dst_path = cast(str, dst_path)
+        if _check:
+            src_attr = self.attr(src_path, src_password, _check=False)
+            if src_attr["is_dir"]:
+                if recursive:
+                    return self.copytree(
+                        src_path, 
+                        dst_path, 
+                        src_password, 
+                        dst_password, 
+                        overwrite_or_ignore=overwrite_or_ignore, 
+                        _check=False, 
+                    )
+                if overwrite_or_ignore == False:
+                    return None
+                raise IsADirectoryError(
+                    errno.EISDIR, f"source path {src_path!r} is a directory: {src_path!r} -> {dst_path!r}")
         if src_path == dst_path:
             if overwrite_or_ignore is None:
                 raise SameFileError(src_path)
             return None
-        if commonpath((src_path, dst_path)) == dst_path:
-            raise PermissionError(errno.EPERM, f"copy a file to its subordinate path is not allowed: {src_path!r} -> {dst_path!r}")
-        src_attr = self.attr(src_path, src_password, _check=False)
-        if src_attr["is_dir"]:
-            raise IsADirectoryError(errno.EISDIR, f"source path {src_path!r} is a directory: {src_path!r} -> {dst_path!r}")
+        elif commonpath((src_path, dst_path)) == dst_path:
+            if overwrite_or_ignore == False:
+                return None
+            raise PermissionError(
+                errno.EPERM, 
+                f"copy a file as its ancestor is not allowed: {src_path!r} -> {dst_path!r}", 
+            )
+        elif commonpath((src_path, dst_path)) == src_path:
+            if overwrite_or_ignore == False:
+                return None
+            raise PermissionError(
+                errno.EPERM, 
+                f"copy a file as its descendant is not allowed: {src_path!r} -> {dst_path!r}", 
+            )
+        src_dir, src_name = split(src_path)
+        dst_dir, dst_name = split(dst_path)
         try:
             dst_attr = self.attr(dst_path, dst_password, _check=False)
         except FileNotFoundError:
             pass
         else:
             if dst_attr["is_dir"]:
+                if overwrite_or_ignore == False:
+                    return None
                 raise IsADirectoryError(errno.EISDIR, f"destination path {src_path!r} is a directory: {src_path!r} -> {dst_path!r}")
             elif overwrite_or_ignore is None:
                 raise FileExistsError(errno.EEXIST, f"destination path {dst_path!r} already exists: {src_path!r} -> {dst_path!r}")
             elif not overwrite_or_ignore:
                 return None
-            self.fs_remove([basename(dst_path)], dirname(dst_path), _check=False)
-        src_dir, src_name = split(src_path)
-        dst_dir, dst_name = split(dst_path)
+            self.fs_remove(dst_dir, [dst_name], _check=False)
         if src_name == dst_name:
             self.fs_copy(src_dir, dst_dir, [src_name], _check=False)
         else:
             src_storage = self.storage_of(src_dir, src_password, _check=False)
             dst_storage = self.storage_of(dst_dir, dst_password, _check=False)
             if src_storage != dst_storage:
+                if overwrite_or_ignore == False:
+                    return None
                 raise PermissionError(errno.EPERM, f"cross storages replication does not allow renaming: [{src_storage!r}]{src_path!r} -> [{dst_storage!r}]{dst_path!r}")
             tempdirname = str(uuid4())
             tempdir = joinpath(dst_dir, tempdirname)
             self.fs_mkdir(tempdir, _check=False)
             try:
                 self.fs_copy(src_dir, tempdir, [src_name], _check=False)
                 self.fs_rename(joinpath(tempdir, src_name), dst_name, _check=False)
                 self.fs_move(tempdir, dst_dir, [dst_name], _check=False)
             finally:
-                self.fs_remove([tempdirname], dst_dir, _check=False)
+                self.fs_remove(dst_dir, [tempdirname], _check=False)
         return dst_path
 
     def copytree(
         self, 
         /, 
         src_path: str | PathLike[str], 
-        dst_dir: str | PathLike[str], 
+        dst_path: str | PathLike[str], 
+        src_password: str = "", 
         dst_password: str = "", 
+        overwrite_or_ignore: Optional[bool] = None, 
         _check: bool = True, 
-    ) -> str:
+    ) -> Optional[str]:
         if isinstance(src_path, AlistPath):
+            if not src_password:
+                src_password = src_path.password
             src_path = src_path.path
         elif _check:
             src_path = self.abspath(src_path)
-        if isinstance(dst_dir, AlistPath):
+        if isinstance(dst_path, AlistPath):
             if not dst_password:
-                dst_password = dst_dir.password
-            dst_dir = dst_dir.path
+                dst_password = dst_path.password
+            dst_path = dst_path.path
         elif _check:
-            dst_dir = self.abspath(dst_dir)
+            dst_path = self.abspath(dst_path)
         src_path = cast(str, src_path)
-        dst_dir = cast(str, dst_dir)
-        if dirname(src_path) == dst_dir:
-            raise SameFileError(src_path)
-        elif src_path == dst_dir or commonpath((src_path, dst_dir)) == dst_dir:
-            raise PermissionError(errno.EPERM, f"copy a directory to its subordinate path is not allowed: {src_path!r} ->> {dst_dir!r}")
-        elif not self.attr(dst_dir, dst_password, _check=False)["is_dir"]:
-            raise NotADirectoryError(errno.ENOTDIR, f"destination is not directory: {src_path!r} ->> {dst_dir!r}")
-        elif self.exists(joinpath(dst_dir, basename(src_path))):
-            raise FileExistsError(errno.EEXIST, f"destination already exists: {src_path!r} ->> {dst_dir!r}")
-        self.fs_copy(dirname(src_path), dst_dir, [basename(src_path)], _check=False)
-        return dst_dir
+        dst_path = cast(str, dst_path)
+        if _check:
+            src_attr = self.attr(src_path, src_password, _check=False)
+            if not src_attr["is_dir"]:
+                return self.copy(
+                    src_path, 
+                    dst_path, 
+                    src_password, 
+                    dst_password, 
+                    overwrite_or_ignore=overwrite_or_ignore, 
+                    _check=False, 
+                )
+        if src_path == dst_path:
+            if overwrite_or_ignore is None:
+                raise SameFileError(src_path)
+            return None
+        elif commonpath((src_path, dst_path)) == dst_path:
+            if overwrite_or_ignore == False:
+                return None
+            raise PermissionError(errno.EPERM, f"copy a directory to its subordinate path is not allowed: {src_path!r} ->> {dst_path!r}")
+        src_dir, src_name = split(src_path)
+        dst_dir, dst_name = split(dst_path)
+        try:
+            dst_attr = self.attr(dst_path, dst_password, _check=False)
+        except FileNotFoundError:
+            if src_name == dst_name:
+                self.fs_copy(src_dir, dst_dir, [src_name], _check=False)
+                return dst_path
+            self.makedirs(dst_path, dst_password, exist_ok=True, _check=False)
+        else:
+            if not dst_attr["is_dir"]:
+                if overwrite_or_ignore == False:
+                    return None
+                raise NotADirectoryError(
+                    errno.ENOTDIR, 
+                    f"destination is not directory: {src_path!r} ->> {dst_path!r}", 
+                )
+            elif overwrite_or_ignore is None:
+                raise FileExistsError(
+                    errno.EEXIST, 
+                    f"destination already exists: {src_path!r} ->> {dst_path!r}", 
+                )
+        for attr in self.listdir_attr(src_path):
+            if attr["is_dir"]:
+                self.copytree(
+                    joinpath(src_path, attr["name"]), 
+                    joinpath(dst_path, attr["name"]), 
+                    src_password=src_password, 
+                    dst_password=dst_password, 
+                    overwrite_or_ignore=overwrite_or_ignore, 
+                    _check=False, 
+                )
+            else:
+                self.copy(
+                    joinpath(src_path, attr["name"]), 
+                    joinpath(dst_path, attr["name"]), 
+                    src_password=src_password, 
+                    dst_password=dst_password, 
+                    overwrite_or_ignore=overwrite_or_ignore, 
+                    _check=False, 
+                )
+        return dst_path
 
     def download(
         self, 
         /, 
         path: str | PathLike[str], 
         local_path_or_file: bytes | str | PathLike | SupportsWrite[bytes] | TextIOWrapper = "", 
         write_mode: Literal["", "x", "w", "a"] = "w", 
@@ -3165,15 +3689,15 @@
             path = self.abspath(path)
         path = cast(str, path)
         if path == "/":
             if recursive:
                 try:
                     storages = self.list_storage()
                 except PermissionError:
-                    self.fs_remove(self.listdir("/", password, refresh=True), "/", _check=False)
+                    self.fs_remove("/", self.listdir("/", password, refresh=True), _check=False)
                 else:
                     for storage in storages:
                         self.fs_remove_storage(storage["id"])
                 return
             else:
                 raise PermissionError(errno.EPERM, "remove the root directory is not allowed")
         attr = self.attr(path, password, _check=False)
@@ -3188,15 +3712,15 @@
                 if attr.get("hash_info") is None:
                     raise
             else:
                 for storage in storages:
                     if commonpath((storage["mount_path"], path)) == path:
                         self.fs_remove_storage(storage["id"])
                         return
-        self.fs_remove([basename(path)], dirname(path), _check=False)
+        self.fs_remove(dirname(path), [basename(path)], _check=False)
 
     def removedirs(
         self, 
         /, 
         path: str | PathLike[str], 
         password: str = "", 
         _check: bool = True, 
@@ -3232,15 +3756,15 @@
                         remove_storage(storage["id"])
                         del_dir = ""
                         break
                 else:
                     del_dir = parent_dir
                 parent_dir = dirname(parent_dir)
             if del_dir:
-                self.fs_remove([basename(del_dir)], parent_dir, _check=False)
+                self.fs_remove(parent_dir, [basename(del_dir)], _check=False)
         except OSError as e:
             pass
 
     def rename(
         self, 
         /, 
         src_path: str | PathLike[str], 
@@ -3296,15 +3820,15 @@
                     if dst_attr["is_dir"]:
                         if self.get_directory_capacity(dst_path, dst_password, _check=False):
                             raise OSError(errno.ENOTEMPTY, f"directory {dst_path!r} is not empty: {src_path!r} -> {dst_path!r}")
                     else:
                         raise NotADirectoryError(errno.ENOTDIR, f"{dst_path!r} is not a directory: {src_path!r} -> {dst_path!r}")
                 elif dst_attr["is_dir"]:
                     raise IsADirectoryError(errno.EISDIR, f"{dst_path!r} is a directory: {src_path!r} -> {dst_path!r}")
-                self.fs_remove([dst_name], dst_dir, _check=False)
+                self.fs_remove(dst_dir, [dst_name], _check=False)
             else:
                 raise FileExistsError(errno.EEXIST, f"{dst_path!r} already exists: {src_path!r} -> {dst_path!r}")
         src_storage = self.storage_of(src_dir, src_password, _check=False)
         dst_storage = self.storage_of(dst_dir, dst_password, _check=False)
         if src_name == dst_name:
             if src_storage != dst_storage:
                 warn("cross storages movement will retain the original file: {src_path!r} |-> {dst_path!r}")
@@ -3405,15 +3929,15 @@
             raise PermissionError(errno.EPERM, "remove the root directory is not allowed")
         elif self.is_storage(path, password, _check=False):
             raise PermissionError(errno.EPERM, f"remove a storage by `rmdir` is not allowed: {path!r}")
         elif not self.attr(path, password, _check=False)["is_dir"]:
             raise NotADirectoryError(errno.ENOTDIR, path)
         elif not self.is_empty(path, password, _check=False):
             raise OSError(errno.ENOTEMPTY, f"directory not empty: {path!r}")
-        self.fs_remove([basename(path)], dirname(path), _check=False)
+        self.fs_remove(dirname(path), [basename(path)], _check=False)
 
     def rmtree(
         self, 
         /, 
         path: str | PathLike[str], 
         password: str = "", 
         _check: bool = True, 
@@ -3426,36 +3950,35 @@
         path: str | PathLike[str] = "", 
         password: str = "", 
         refresh: Optional[bool] = None, 
         _check: bool = True, 
     ) -> Iterator[AlistPath]:
         return iter(self.listdir_path(path, password, refresh=refresh, _check=_check))
 
-    # TODO: 需要进一步实现，更准确的 st_mode
     def stat(
         self, 
         /, 
         path: str | PathLike[str] = "", 
         password: str = "", 
         _check: bool = True, 
     ) -> stat_result:
         attr = self.attr(path, password, _check=_check)
         is_dir = attr.get("is_dir", False)
         lastest_update = attr["lastest_update"]
         return stat_result((
-            (S_IFDIR if is_dir else S_IFREG) | 0o777, 
-            0, 
-            0, 
-            1, 
-            0, 
-            0, 
-            0 if is_dir else attr["size"], 
-            lastest_update.timestamp(), 
-            parse_datetime(attr["modified"]).timestamp(), 
-            parse_datetime(attr["created"]).timestamp(), 
+            (S_IFDIR if is_dir else S_IFREG) | 0o777, # mode
+            0, # ino
+            0, # dev
+            1, # nlink
+            0, # uid
+            0, # gid
+            attr.get("size", 0), # size
+            lastest_update.timestamp(), # atime
+            parse_datetime(attr["modified"]).timestamp(), # mtime
+            parse_datetime(attr["created"]).timestamp(), # ctime
         ))
 
     def storage_of(
         self, 
         /, 
         path: str | PathLike[str] = "", 
         password: str = "", 
@@ -3557,15 +4080,15 @@
         else:
             if overwrite_or_ignore is None:
                 raise FileExistsError(errno.EEXIST, path)
             elif attr["is_dir"]:
                 raise IsADirectoryError(errno.EISDIR, path)
             elif not overwrite_or_ignore:
                 return path
-            self.fs_remove([basename(path)], dirname(path), _check=False)
+            self.fs_remove(dirname(path), [basename(path)], _check=False)
         size: int
         if hasattr(file, "getbuffer"):
             size = len(file.getbuffer()) # type: ignore
         else:
             try:
                 fd = file.fileno() # type: ignore
             except (UnsupportedOperation, AttributeError):
@@ -3798,17 +4321,18 @@
             tio = TextIOWrapper(bio, encoding=encoding, errors=errors, newline=newline)
             tio.write(text)
             tio.flush()
             bio.seek(0)
         return self.write_bytes(path, bio, password=password, as_task=as_task, _check=_check)
 
     cd  = chdir
+    cp  = copy
     pwd = getcwd
     ls  = listdir
     ll  = listdir_path
+    mv  = move
     rm  = remove
 
-# TODO: 自动根据文档 https://alist.nn.ci/guide/api 生成 AlistClient 类
+
 # TODO: 所有类和函数都要有文档
 # TODO: 所有类和函数都要有单元测试
-# TODO: 支持异步IO
 # TODO: 上传下载都支持进度条，下载支持多线程（返回 Future）
```

### Comparing `python_alist-0.0.9.8.1/alist/util/_init_mimetypes.py` & `python_alist-0.0.9.9/alist/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_alist-0.0.9.8.1/alist/util/download.py` & `python_alist-0.0.9.9/alist/util/download.py`

 * *Files identical despite different names*

### Comparing `python_alist-0.0.9.8.1/alist/util/file.py` & `python_alist-0.0.9.9/alist/util/file.py`

 * *Files identical despite different names*

### Comparing `python_alist-0.0.9.8.1/alist/util/ignore.py` & `python_alist-0.0.9.9/alist/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_alist-0.0.9.8.1/alist/util/iter.py` & `python_alist-0.0.9.9/alist/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_alist-0.0.9.8.1/alist/util/property.py` & `python_alist-0.0.9.9/alist/util/property.py`

 * *Files identical despite different names*

### Comparing `python_alist-0.0.9.8.1/alist/util/response.py` & `python_alist-0.0.9.9/alist/util/response.py`

 * *Files identical despite different names*

### Comparing `python_alist-0.0.9.8.1/alist/util/text.py` & `python_alist-0.0.9.9/alist/util/text.py`

 * *Files identical despite different names*

### Comparing `python_alist-0.0.9.8.1/alist/util/urlopen.py` & `python_alist-0.0.9.9/alist/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_alist-0.0.9.8.1/pyproject.toml` & `python_alist-0.0.9.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-alist"
-version = "0.0.9.8.1"
+version = "0.0.9.9"
 description = "Python wrapper for alist."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-wrap-alist-web-api"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-wrap-alist-web-api"
 keywords = ["nas", "alist"]
```

### Comparing `python_alist-0.0.9.8.1/readme.md` & `python_alist-0.0.9.9/readme.md`

 * *Files identical despite different names*

### Comparing `python_alist-0.0.9.8.1/PKG-INFO` & `python_alist-0.0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-alist
-Version: 0.0.9.8.1
+Version: 0.0.9.9
 Summary: Python wrapper for alist.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-wrap-alist-web-api
 License: MIT
 Keywords: nas,alist
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

