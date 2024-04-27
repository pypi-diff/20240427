# Comparing `tmp/arraylake-0.9.5.tar.gz` & `tmp/arraylake-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraylake-0.9.5.tar", max compression
+gzip compressed data, was "arraylake-0.9.6.tar", max compression
```

## Comparing `arraylake-0.9.5.tar` & `arraylake-0.9.6.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0      658 2024-03-26 02:58:48.915402 arraylake-0.9.5/README.md
--rw-r--r--   0        0        0      336 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/__init__.py
--rw-r--r--   0        0        0       63 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/__main__.py
--rw-r--r--   0        0        0    22003 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/api_utils.py
--rw-r--r--   0        0        0     9770 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/asyn.py
--rw-r--r--   0        0        0     3806 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/chunkstore/__init__.py
--rw-r--r--   0        0        0     4056 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/chunkstore/abc.py
--rw-r--r--   0        0        0     9759 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/chunkstore/base_chunkstore.py
--rw-r--r--   0        0        0     6664 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/chunkstore/fsspec_chunkstore.py
--rw-r--r--   0        0        0     1862 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/chunkstore/fsspec_compat.py
--rw-r--r--   0        0        0    10863 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/chunkstore/s3chunkstore.py
--rw-r--r--   0        0        0        0 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/cli/__init__.py
--rw-r--r--   0        0        0     4915 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/cli/auth.py
--rw-r--r--   0        0        0     4741 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/cli/config.py
--rw-r--r--   0        0        0     1615 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/cli/main.py
--rw-r--r--   0        0        0     3943 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/cli/repo.py
--rw-r--r--   0        0        0     4860 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/cli/utils.py
--rw-r--r--   0        0        0    10735 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/client.py
--rw-r--r--   0        0        0     7850 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/commits.py
--rw-r--r--   0        0        0     2976 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/config.py
--rw-r--r--   0        0        0      176 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/config.yaml
--rw-r--r--   0        0        0     5221 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/diagnostics.py
--rw-r--r--   0        0        0      297 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/exceptions.py
--rw-r--r--   0        0        0      194 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/experimental.py
--rw-r--r--   0        0        0     1082 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/log_util.py
--rw-r--r--   0        0        0      261 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/metastore/__init__.py
--rw-r--r--   0        0        0    15277 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/metastore/abc.py
--rw-r--r--   0        0        0    19638 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/metastore/http_metastore.py
--rw-r--r--   0        0        0        0 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/py.typed
--rw-r--r--   0        0        0    89456 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/repo.py
--rw-r--r--   0        0        0     7180 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/retrier.py
--rw-r--r--   0        0        0     4776 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/token.py
--rw-r--r--   0        0        0    21747 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/types.py
--rw-r--r--   0        0        0    17216 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/virtual.py
--rw-r--r--   0        0        0      851 2024-03-26 02:58:48.915402 arraylake-0.9.5/arraylake/zarr_util.py
--rw-r--r--   0        0        0     4890 2024-03-26 02:59:09.363358 arraylake-0.9.5/pyproject.toml
--rw-r--r--   0        0        0     2569 1970-01-01 00:00:00.000000 arraylake-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0      653 2024-04-27 00:28:22.714914 arraylake-0.9.6/README.md
+-rw-r--r--   0        0        0      416 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/__init__.py
+-rw-r--r--   0        0        0       63 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/__main__.py
+-rw-r--r--   0        0        0    22304 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/api_utils.py
+-rw-r--r--   0        0        0     9770 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/asyn.py
+-rw-r--r--   0        0        0     4001 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/chunkstore/__init__.py
+-rw-r--r--   0        0        0     4056 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/chunkstore/abc.py
+-rw-r--r--   0        0        0     9973 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/chunkstore/base_chunkstore.py
+-rw-r--r--   0        0        0     6664 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/chunkstore/fsspec_chunkstore.py
+-rw-r--r--   0        0        0     1862 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/chunkstore/fsspec_compat.py
+-rw-r--r--   0        0        0    10893 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/chunkstore/s3chunkstore.py
+-rw-r--r--   0        0        0        0 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/cli/__init__.py
+-rw-r--r--   0        0        0     4915 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/cli/auth.py
+-rw-r--r--   0        0        0     4741 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/cli/config.py
+-rw-r--r--   0        0        0     1615 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/cli/main.py
+-rw-r--r--   0        0        0     5630 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/cli/repo.py
+-rw-r--r--   0        0        0     4860 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/cli/utils.py
+-rw-r--r--   0        0        0    21046 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/client.py
+-rw-r--r--   0        0        0     8181 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/commits.py
+-rw-r--r--   0        0        0     2976 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/config.py
+-rw-r--r--   0        0        0      176 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/config.yaml
+-rw-r--r--   0        0        0     5221 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/diagnostics.py
+-rw-r--r--   0        0        0      345 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/exceptions.py
+-rw-r--r--   0        0        0      194 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/experimental.py
+-rw-r--r--   0        0        0     1082 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/log_util.py
+-rw-r--r--   0        0        0      261 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/metastore/__init__.py
+-rw-r--r--   0        0        0    15638 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/metastore/abc.py
+-rw-r--r--   0        0        0    23366 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/metastore/http_metastore.py
+-rw-r--r--   0        0        0        0 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/py.typed
+-rw-r--r--   0        0        0    92130 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/repo.py
+-rw-r--r--   0        0        0     7180 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/retrier.py
+-rw-r--r--   0        0        0     1526 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/strategies.py
+-rw-r--r--   0        0        0     4776 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/token.py
+-rw-r--r--   0        0        0    27584 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/types.py
+-rw-r--r--   0        0        0    17216 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/virtual.py
+-rw-r--r--   0        0        0      851 2024-04-27 00:28:22.714914 arraylake-0.9.6/arraylake/zarr_util.py
+-rw-r--r--   0        0        0     5405 2024-04-27 00:28:43.102988 arraylake-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 arraylake-0.9.6/PKG-INFO
```

### Comparing `arraylake-0.9.5/README.md` & `arraylake-0.9.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,12 +11,12 @@
 
 Check out the [documentation](https://docs.earthmover.io) to get started.
 
 ## Install
 
 ```
 # using pip
-pip install "arraylake[cli]"
+pip install "arraylake"
 
 # using conda
 conda install arraylake
 ```
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
                                   [Arraylake]
                          _e_a_r_t_h_m_o_v_e_r_._i_o - _d_o_c_u_m_e_n_t_a_t_i_o_n
 Arraylake is a cloud-based platform that understands a wide array of
 multidimensional scientific data. Organize, analyze, build, and
 collaborateâeffortlessly. Check out the [documentation](https://
 docs.earthmover.io) to get started. ## Install ``` # using pip pip install
-"arraylake[cli]" # using conda conda install arraylake ```
+"arraylake" # using conda conda install arraylake ```
```

### Comparing `arraylake-0.9.5/arraylake/api_utils.py` & `arraylake-0.9.6/arraylake/api_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,15 @@
             # technically we don't enforce this, for now it's for debugging purposes
             "client-name": "arraylake-python-client",
             "client-version": arraylake.__version__,
             # TODO: Remove this once managed sessions are mandatory for all users.
             "arraylake-feature-managed-sessions": str(self.managed_sessions),
         }
 
+        self._async_lock = asyncio.Lock()
         self._client = None
 
     def __getstate__(self):
         return (
             self.api_url,
             self.hint,
             self.token,
@@ -237,31 +238,34 @@
             self.hint,
             self.token,
             self.timeout,
             self.max_keepalive_connections,
             self.keepalive_expiry,
             self._default_headers,
         ) = state
+        self._async_lock = asyncio.Lock()
         self._client = None
 
     @retry_on_exception((httpx.TransportError), int(config.get("http.retries", 5)))
     async def _request(self, method: str, path: str, **kwargs) -> httpx.Response:
         """Convenience method to make a standard request with retry on RemoteProtocolError"""
         if self._client is None:
-            loop = asyncio.get_running_loop()
-            self._client = await get_client(
-                loop,
-                self.api_url,
-                self.token,
-                self.hint,
-                self._default_headers,
-                self.timeout,
-                self.max_keepalive_connections,
-                self.keepalive_expiry,
-            )
+            async with self._async_lock:
+                if self._client is None:  # double check the client wasn't just created
+                    loop = asyncio.get_running_loop()
+                    self._client = await get_client(
+                        loop,
+                        self.api_url,
+                        self.token,
+                        self.hint,
+                        self._default_headers,
+                        self.timeout,
+                        self.max_keepalive_connections,
+                        self.keepalive_expiry,
+                    )
         return await self._client.request(method, path, **kwargs)
 
     async def get_user(self) -> Union[ApiTokenInfo, UserInfo]:
         """Make an API request to the /user route to get the current authenticated user
 
         This is used in various places through the Arraylake client. For example, we use this method to:
         - determine the committer/author when creating a repo instance
```

### Comparing `arraylake-0.9.5/arraylake/asyn.py` & `arraylake-0.9.6/arraylake/asyn.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.5/arraylake/chunkstore/__init__.py` & `arraylake-0.9.6/arraylake/chunkstore/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 OS = TypeVar("OS", bound=ObjectStore)
 
 from typing import cast
 
 # TODO: fix Any typing here
 DEFAULT_STORES: Mapping[Platform, Any] = {
     "s3": S3ObjectStore,
+    "s3-compatible": S3ObjectStore,
     "minio": S3ObjectStore,
     "gs": GCSFSObjectStore,
 }
 
 
 def get_object_store_type(platform: Platform, object_store: type[OS] | None) -> type[OS]:
     object_store_type = DEFAULT_STORES[platform] if object_store is None else object_store
@@ -67,18 +68,23 @@
         object_store=object_store_type(bucket_name=bucket_name, kwargs=kwargs),
         prefix=prefix,
         schema_version=ChunkstoreSchemaVersion.V0,
         inline_threshold_bytes=inline_threshold_bytes,
     )
 
 
+def bucket_prefix(bucket: Bucket, repo_id: DBID) -> str:
+    id = repo_id.hex()
+    return f"{bucket.prefix}/{id}" if bucket.prefix else id
+
+
 # TODO: Consider making this a class method on Chunkstore
 def mk_chunkstore_from_bucket_config(bucket: Bucket, repo_id: DBID, inline_threshold_bytes: int = 0, **kwargs) -> BaseChunkstore:
     bucket_name = bucket.name
-    prefix = repo_id.hex()
+    prefix = bucket_prefix(bucket, repo_id)
     bucket_config = dict(bucket.extra_config)
     object_store_type: type[ObjectStore] = get_object_store_type(bucket.platform, object_store=None)
 
     # We make bucket config take precedence over kwargs
     # The main conflict we care about is endpoint_url
     # The previous version was equivalent to ChainMap(kwargs, bucket_config)
     # where kwargs took precedence over bucket_config.
```

### Comparing `arraylake-0.9.5/arraylake/chunkstore/abc.py` & `arraylake-0.9.6/arraylake/chunkstore/abc.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.5/arraylake/chunkstore/base_chunkstore.py` & `arraylake-0.9.6/arraylake/chunkstore/base_chunkstore.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,15 +234,19 @@
             data = await self.object_store.pull_data(
                 start_byte=chunk_ref.offset, length=chunk_ref.length, key=key, bucket=bucket_name or self.bucket_name
             )
 
         if validate:
             # TODO should this fail for virtual chunks? We never set the hash
             if chunk_ref.hash is None:
-                raise ValueError("chunk hash not set, cannot validate")
+                if chunk_ref.is_virtual():
+                    logger.warning("Cannot validate: chunk hash not set, this must be a virtual chunk")
+                    return data
+                else:
+                    raise HashValidationError("Cannot validate: chunk hash not set")
             hasher = get_hasher(chunk_ref.hash["method"])
             h = tokenize(data, hasher=hasher)
             if h != chunk_ref.hash["token"]:
                 raise HashValidationError(f"hashes did not match for key: {key}")
 
         return data
```

### Comparing `arraylake-0.9.5/arraylake/chunkstore/fsspec_chunkstore.py` & `arraylake-0.9.6/arraylake/chunkstore/fsspec_chunkstore.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.5/arraylake/chunkstore/fsspec_compat.py` & `arraylake-0.9.6/arraylake/chunkstore/fsspec_compat.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.5/arraylake/chunkstore/s3chunkstore.py` & `arraylake-0.9.6/arraylake/chunkstore/s3chunkstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 # https://github.com/fsspec/s3fs/blob/34a32198188164fd48d4d1abcb267f033d1d1ce1/s3fs/core.py#L63
 S3_RETRYABLE_ERRORS = (
     socket.timeout,
     botocore.exceptions.HTTPClientError,
     urllib3.exceptions.IncompleteRead,
     botocore.parsers.ResponseParserError,
     aiohttp.ClientPayloadError,
+    botocore.exceptions.ClientError,
 )
 
 
 # Below we set up a global cache for aiobotocore clients
 # There should be one per each event loop and set of configuration parameters
 # dicts aren't hashable, so we sort the keywords into key / value pairs
 @dataclass(eq=True, frozen=True)
@@ -207,15 +208,15 @@
         # Mypy cannot tell that self._session_cleint is not None (set it self._open())
         # Note: this can likely be removed once we drop support for Python 3.8
         if self._session_client is None:
             raise ValueError("session client not set")
         # TODO: Should raise an exception if the bucket does not exist
         await self._session_client.head_bucket(Bucket=self.bucket_name)
 
-    @retry_on_exception(S3_RETRYABLE_ERRORS, n=5)
+    @retry_on_exception(S3_RETRYABLE_ERRORS, n=20)
     async def put_data(self, *, data: bytes, key: str) -> None:
         await self._open()
         # Mypy cannot tell that self._session_client is not None (set it self._open())
         # Note: this can likely be removed once we drop support for Python 3.8
         if self._session_client is None:
             raise ValueError("session client not set")
         resp = await self._session_client.put_object(Bucket=self.bucket_name, Key=key, Body=data)
@@ -235,22 +236,22 @@
         response = await self._session_client.get_object(Bucket=bucket, Key=key, Range=byte_range)
         await logger.adebug("pull_data received response: %s", response)
         async with response["Body"] as stream:
             data = await stream.read()
         return data
 
     @property
-    async def is_anonymous_session(self):
+    async def is_anonymous_session(self) -> bool:
         await self._open()
         # Mypy cannot tell that self._session_client is not None (set it self._open())
         # Note: this can likely be removed once we drop support for Python 3.8
         if self._session_client is None:
             raise ValueError("session client not set")
         # TODO: Does _client_config always exist
-        return self._session_client._client_config.signature_version == botocore.UNSIGNED  # type: ignore
+        return self._session_client._client_config.signature_version == botocore.UNSIGNED
 
     def __repr__(self):
         status = self.status
         disp = f"{type(self).__name__}, bucket: {self.bucket_name}, status: {status}"
         if status == "OPEN":
             assert self._session_client is not None
             if hasattr(self._session_client, "_endpoint"):
```

### Comparing `arraylake-0.9.5/arraylake/cli/auth.py` & `arraylake-0.9.6/arraylake/cli/auth.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.5/arraylake/cli/config.py` & `arraylake-0.9.6/arraylake/cli/config.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.5/arraylake/cli/main.py` & `arraylake-0.9.6/arraylake/cli/main.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.5/arraylake/cli/repo.py` & `arraylake-0.9.6/arraylake/cli/repo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,40 @@
+import warnings
 from enum import Enum
 from typing import Optional
 
 import typer
 from rich import print_json
 from rich.table import Table
 
 from arraylake import AsyncClient
 from arraylake.cli.utils import coro, rich_console, simple_progress
 from arraylake.log_util import get_logger
+from arraylake.types import RepoOperationMode
 
-app = typer.Typer(help="Manage Arraylake repositories")
+app = typer.Typer(help="Manage Arraylake repositories", no_args_is_help=True)
 logger = get_logger(__name__)
 
 
 class ListOutputType(str, Enum):
     rich = "rich"
     json = "json"
 
 
 def _repos_table(repos, org):
     table = Table(title=f"Arraylake Repositories for [bold]{org}[/bold]", min_width=80)
     table.add_column("Name", justify="left", style="cyan", no_wrap=True, min_width=45)
     table.add_column("Created", justify="right", style="green", min_width=25)
     table.add_column("Updated", justify="right", style="green", min_width=25)
+    table.add_column("Status", justify="right", style="green", min_width=25)
+
+    mode_colors = {"online": "green", "maintenance": "yellow", "offline": "red"}
 
     for repo in repos:
-        table.add_row(repo.name, repo.created.isoformat(), repo.updated.isoformat())
+        table.add_row(repo.name, repo.created.isoformat(), repo.updated.isoformat(), repo.status.mode, style=mode_colors[repo.status.mode])
 
     return table
 
 
 @app.command(name="list")
 @coro  # type: ignore
 async def list_repos(
@@ -57,28 +62,32 @@
         rich_console.print("\nNo results")
 
 
 @app.command()
 @coro  # type: ignore
 async def create(
     repo_name: str = typer.Argument(..., help="Name of repository {ORG}/{REPO_NAME}"),
-    bucket_nickname: Optional[str] = typer.Option(None, help="Chunkstore bucket nickname"),
+    bucket_config_nickname: Optional[str] = typer.Option(None, help="Chunkstore bucket config nickname"),
+    bucket_nickname: Optional[str] = typer.Option(None, help="Chunkstore bucket config nickname (DEPRECATED)"),
 ):
     """**Create** a new repository
 
     **Examples**
 
     - Create new repository
 
         ```
-        $ arraylake repo create my-org/example-repo --bucket-nickname arraylake-bucket
+        $ arraylake repo create my-org/example-repo --bucket-config-nickname arraylake-bucket
         ```
     """
+    if bucket_nickname:
+        bucket_config_nickname = bucket_nickname
+        warnings.warn("bucket-nickname has been renamed to bucket-config-nickname and will be removed in Arraylake 0.10", FutureWarning)
     with simple_progress(f"Creating repo [bold]{repo_name}[/bold]..."):
-        await AsyncClient().create_repo(repo_name, bucket_nickname=bucket_nickname)
+        await AsyncClient().create_repo(repo_name, bucket_config_nickname=bucket_config_nickname)
 
 
 @app.command()
 @coro  # type: ignore
 async def delete(
     repo_name: str = typer.Argument(..., help="Name of repository {ORG}/{REPO_NAME}"),
     confirm: bool = typer.Option(False, help="confirm deletion without prompting"),
@@ -124,7 +133,37 @@
     await repo.checkout()
     _tree = await repo.tree(prefix=prefix, depth=depth)
 
     if output == "json":
         print_json(_tree.model_dump_json())
     else:
         rich_console.print(_tree._as_rich_tree(name=repo_name))
+
+
+@app.command()
+@coro  # type: ignore
+async def get_status(
+    repo_name: str = typer.Argument(..., help="Name of repository {ORG}/{REPO_NAME}"),
+    output: ListOutputType = typer.Option("rich", help="Output formatting"),
+):
+    repo = await AsyncClient().get_repo_object(repo_name)
+    if output == "json":
+        print_json(data=repo.status.model_dump())
+    else:
+        print(repo.status.mode.value)
+
+
+@app.command()
+@coro  # type: ignore
+async def set_status(
+    repo_name: str = typer.Argument(..., help="Name of repository {ORG}/{REPO_NAME}"),
+    mode: RepoOperationMode = typer.Argument(..., help="An option"),
+    message: str = typer.Option(None, help="Optional message to bind to state"),
+    output: ListOutputType = typer.Option("rich", help="Output formatting"),
+):
+    c = AsyncClient()
+    await c.set_repo_status(repo_name, mode, message)
+    repo = await c.get_repo_object(repo_name)
+    if output == "json":
+        print_json(data=repo.status.model_dump())
+    else:
+        print(repo.status.mode.value)
```

### Comparing `arraylake-0.9.5/arraylake/cli/utils.py` & `arraylake-0.9.6/arraylake/cli/utils.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.5/arraylake/commits.py` & `arraylake-0.9.6/arraylake/commits.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
-from collections.abc import Iterable, Iterator, Mapping
+from collections import defaultdict
+from collections.abc import Iterable, Iterator, Mapping, MutableMapping
 from dataclasses import dataclass
 from html import escape
 from typing import Callable, TypeVar
 
 from arraylake.exceptions import CommitNotFoundException
 from arraylake.types import (
     Branch,
@@ -14,57 +15,58 @@
     CommitID,
     DBIDBytes,
     Tag,
     TagName,
 )
 
 Node = TypeVar("Node")
+K = TypeVar("K")
+V = TypeVar("V")
 
 
 def get_ref(
     ref: CommitID | str,
     commits: Mapping[CommitID, Commit] | None = None,
     branches: Mapping[BranchName, CommitID] | None = None,
     tags: Mapping[TagName, CommitID] | None = None,
 ) -> tuple[CommitID | None, BranchName | None]:
-    if isinstance(ref, str):
-        try:
-            ref = CommitID.fromhex(ref)
-        except ValueError:
-            # Not a commit we will try branches and tags
-            pass
-
-    if isinstance(ref, DBIDBytes):
-        assert commits is not None
-        if ref in commits:
-            return (ref, None)
-        else:
-            raise ValueError(f"Commit {ref!r} was not found in commit history.")
-
     if branches is not None:
-        as_branch_name = BranchName(ref)
+        as_branch_name = BranchName(str(ref))
         maybe_branch_commit = branches.get(as_branch_name)
         if maybe_branch_commit:
             return (maybe_branch_commit, as_branch_name)
 
     if ref == "main":
         # We want the main branch to magically "exist" without users creating it
         # Other branches should fail to checkout if they have not been created by the user.
         # This enables the following use cases:
         #   - A user does `repo.checkout()` on a new repo
         #   - A user creates a repo, makes commits to branch "foo",
         #     and then tries to checkout main, which doesn't exist yet
         return (None, BranchName("main"))
 
-    # TODO: check that a "main" tag is not allowed?
     if tags is not None:
-        commit: CommitID | None = tags.get(TagName(ref))
+        commit: CommitID | None = tags.get(TagName(str(ref)))
         if commit is not None:
             return (commit, None)
 
+    if commits is not None:
+        if isinstance(ref, str):
+            try:
+                ref = CommitID.fromhex(ref)
+            except ValueError:
+                # Not a commit we will try branches and tags
+                pass
+
+        if isinstance(ref, DBIDBytes):
+            if ref in commits:
+                return (ref, None)
+            else:
+                raise ValueError(f"Commit {ref!r} was not found in commit history.")
+
     # no commits or tags were found for `ref`,
     # and we weren't asked for 'main' branch of an empty repo
     raise ValueError(f"Ref {ref!r} was not found in branches, tags, or commits.")
 
 
 def walk_commits(start_id: CommitID, get_node: Callable[[CommitID], Node], get_parent: Callable[[Node], CommitID | None]) -> Iterator[Node]:
     """Traverses a tree-like commit data structure, starting in the provided commit.
@@ -132,15 +134,15 @@
     tags: Mapping[TagName, CommitID]
     """Mapping of tag name to Commit ID"""
     branches: Mapping[BranchName, CommitID]
     """Mapping of branch name to Commit ID"""
 
     def __init__(self, commit_list: Iterable[Commit], tag_list: Iterable[Tag], branch_list=Iterable[Branch]):
         self.commits = {commit.id: commit for commit in commit_list}
-        self.tags = {tag.id: tag.commit_id for tag in tag_list}
+        self.tags = {tag.label: tag.commit.id for tag in tag_list}
         self.branches = {branch.id: branch.commit_id for branch in branch_list}
 
     def get_commit_tree(self, commit_id: CommitID) -> CommitTree:
         """Get the commit tree for a given commit ID.
 
         Args:
             commit_id: the commit ID to start from
@@ -158,14 +160,21 @@
 
         Returns:
             CommitID, BranchName
         """
         return get_ref(ref, self.commits, self.branches, self.tags)
 
 
+def invert_mapping(mapping: Mapping[K, V]):
+    merged: MutableMapping[V, list[K]] = defaultdict(list)
+    for k, v in mapping.items():
+        merged[v].append(k)
+    return merged
+
+
 @dataclass(frozen=True)
 class CommitLog:
     """Used to display commit history to the user."""
 
     repo_name: str
     """Name of the repo"""
     commit_id: CommitID | None
@@ -201,19 +210,27 @@
             console.print(f"Author: {commit.author_entry()}")
             console.print(f"Date:   {commit.commit_time}")
             console.print(Padding(commit.message, (1, 4)))
 
     def _repr_html_(self):
         html = """<ul style="list-style-type: none; margin: 0; padding: 0;">\n"""
 
+        def row(col1: str, col2: str) -> str:
+            return f"   <tr><td style='text-align:right'>{col1}</td><td style='text-align:left'>{col2}</td></tr>"
+
+        commit_tags = invert_mapping(self.commit_data.tags)
         for commit in self:
             html += """ <li>\n  <table style="border: 1px dashed grey">\n"""
-            html += f"""   <tr><td style="text-align:right">Commit ID</td><td style="text-align:left"><b>{escape(str(commit.id))}</b></td></tr>\n"""  # noqa: E501
-            html += f"""   <tr><td style="text-align:right">Author</td><td style="text-align:left">{escape(commit.author_entry())}</td></tr>\n"""  # noqa: E501
-            html += f"""   <tr><td style="text-align:right">Date</td><td style="text-align:left">{escape(commit.commit_time.isoformat())}</td></tr>\n"""  # noqa: E501
+            html += row("Commit ID", "<b>" + escape(str(commit.id)) + "</b>")
+            html += row("Author", escape(commit.author_entry()))
+            html += row("Date", escape(commit.commit_time.isoformat()))
+
+            tags = commit_tags[commit.id]
+            if tags:
+                html += row("Tags", ", ".join(tags))
             html += "  </table>\n"
             message = escape(commit.message).replace("\n", "<br />")
-            html += f"""  <p style="padding: 1em 3em;">{message}</p>\n"""
+            html += f"""  <p style="padding: 1em 2em;">{message}</p>\n"""
             html += " </li>\n"
         html += "</ul>\n"
 
         return html
```

### Comparing `arraylake-0.9.5/arraylake/config.py` & `arraylake-0.9.6/arraylake/config.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.5/arraylake/diagnostics.py` & `arraylake-0.9.6/arraylake/diagnostics.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.5/arraylake/log_util.py` & `arraylake-0.9.6/arraylake/log_util.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.5/arraylake/metastore/abc.py` & `arraylake-0.9.6/arraylake/metastore/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,24 @@
     BranchName,
     CollectionName,
     Commit,
     CommitID,
     DocResponse,
     NewCommit,
     NewSession,
+    NewTag,
     Path,
     PathSizeResponse,
     Repo,
     SessionExpirationUpdate,
     SessionID,
     SessionInfo,
     SessionPathsResponse,
     Tag,
+    TagName,
     Tree,
 )
 
 
 class InvalidRequest(Exception):
     pass
 
@@ -138,26 +140,26 @@
         -------
         Commit
             Commit object
         """
         ...
 
     @abstractmethod
-    async def get_tags(self) -> tuple[Tag, ...]:
+    async def get_tags(self, names: Sequence[TagName] | None = None) -> tuple[Tag, ...]:
         """Get all the tags for the repo.
 
         Returns
         -------
         tuple
          Tuple of Tag objects
         """
         ...
 
     @abstractmethod
-    async def get_branches(self, names: Sequence[BranchName] = []) -> tuple[Branch, ...]:
+    async def get_branches(self, names: Sequence[BranchName] = ()) -> tuple[Branch, ...]:
         """Get all the branches for the repo.
 
         Parameters
         ----------
         names : Sequence[BranchName]
             Only return information for these branches
 
@@ -187,14 +189,19 @@
         Returns
         -------
         CommitID
         """
         ...
 
     @abstractmethod
+    async def new_tag(self, tag: NewTag) -> Tag:
+        """Create a new tag."""
+        ...
+
+    @abstractmethod
     async def old_style_rebase(self, commit_id: CommitID, upstream_branch: BranchName) -> CommitID:
         """Old signature for rebase method, needed for tests and compatibility with clients <= 0.7.6
 
         Delete this method once arraylake 0.7.6 is no longer supported
         """
         ...
 
@@ -242,14 +249,22 @@
     async def delete_branch(self, branch: BranchName) -> bool:
         """Delete the named branch.
 
         Returns: True if the branch was deleted.
         """
         ...
 
+    @abstractmethod
+    async def delete_tag(self, branch: TagName) -> bool:
+        """Delete the named tag.
+
+        Returns: True if the tag was deleted.
+        """
+        ...
+
     # Confusingly, these generator methods cannot be declared async for typing to work properly
     # https://stackoverflow.com/a/56947440
     # https://github.com/python/mypy/issues/5385#issuecomment-407281656
 
     @abstractmethod
     def get_all_paths_for_session(
         self, session_id: SessionID, base_commit: CommitID | None, *, collection: CollectionName, limit: int = 0
```

### Comparing `arraylake-0.9.5/arraylake/metastore/http_metastore.py` & `arraylake-0.9.6/arraylake/metastore/http_metastore.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,65 @@
 from __future__ import annotations
 
 from collections.abc import AsyncGenerator, Generator, Mapping, Sequence
 from dataclasses import dataclass, field
 from typing import Any, TypeVar
+from uuid import UUID
 
 from pydantic import TypeAdapter
 
 from arraylake.api_utils import ArraylakeHttpClient, handle_response
 from arraylake.asyn import async_gather
 from arraylake.config import config
 from arraylake.metastore.abc import Metastore, MetastoreDatabase
 from arraylake.types import (
     Branch,
     BranchName,
+    BucketModifyRequest,
+    BucketResponse,
     BulkCreateDocBody,
     CollectionName,
     Commit,
     CommitID,
     DocResponse,
     DocSessionsResponse,
+    NewBucket,
     NewCommit,
+    NewRepoOperationStatus,
     NewSession,
+    NewTag,
     Path,
     PathSizeResponse,
     Repo,
     RepoCreateBody,
+    RepoOperationMode,
+    RepoOperationStatusResponse,
     SessionExpirationUpdate,
     SessionID,
     SessionInfo,
     SessionPathsResponse,
     Tag,
+    TagName,
     Tree,
     UpdateBranchBody,
 )
 
 # type adapters
 LIST_DATABASES_ADAPTER = TypeAdapter(list[Repo])
 GET_COMMITS_ADAPTER = TypeAdapter(list[Commit])
 GET_TAGS_ADAPTER = TypeAdapter(list[Tag])
 GET_BRANCHES_ADAPTER = TypeAdapter(list[Branch])
 GET_ALL_SESSIONS_FOR_PATH_ADAPTER = TypeAdapter(list[DocSessionsResponse])
 GET_ALL_PATHS_FOR_SESSION_ADAPTER = TypeAdapter(list[SessionPathsResponse])
 GET_DOCS_ADAPTER = TypeAdapter(list[DocResponse])
-LIST_OF_PATHS_ADAPTER = TypeAdapter(list[Path])
+LIST_PATHS_ADAPTER = TypeAdapter(list[Path])
 ADD_DOCS_ADAPTER = TypeAdapter(list[BulkCreateDocBody])
-LIST_OF_SESSIONS_ADAPTER = TypeAdapter(list[SessionInfo])
+LIST_SESSIONS_ADAPTER = TypeAdapter(list[SessionInfo])
+LIST_BUCKETS_ADAPTER = TypeAdapter(list[BucketResponse])
+LIST_REPOS_FOR_BUCKET_ADAPTER = TypeAdapter(list[Repo])
 
 T = TypeVar("T")
 
 
 def chunks(seq: Sequence[T], size: int) -> Generator[Sequence[T], None, None]:
     return (seq[pos : (pos + size)] for pos in range(0, len(seq), size))  # noqa: E203
 
@@ -116,21 +127,61 @@
         handle_response(response)  # raise error on 404
         db_config = HttpMetastoreDatabaseConfig(
             http_metastore_config=self._config,
             repo=name,
         )
         return HttpMetastoreDatabase(db_config)
 
+    async def set_repo_status(self, name: str, mode: RepoOperationMode, message: str | None = None) -> RepoOperationStatusResponse:
+        """Set repo status"""
+        new_status = NewRepoOperationStatus(mode=mode, message=message)
+        response = await self._request("PUT", f"/orgs/{self._config.org}/{name}/status", content=new_status.model_dump_json())
+        handle_response(response)
+        return RepoOperationStatusResponse.model_validate_json(response.content)
+
     async def delete_database(self, name: str, *, imsure: bool = False, imreallysure: bool = False) -> None:
         if not (imsure and imreallysure):
             raise ValueError("Don't do this unless you're really sure. Once the database has been deleted, it's gone forever.")
 
         response = await self._request("DELETE", f"/orgs/{self._config.org}/{name}")
         handle_response(response)
 
+    async def create_bucket_config(self, bucket_config: NewBucket) -> BucketResponse:
+        response = await self._request("POST", f"/orgs/{self._config.org}/buckets", content=bucket_config.model_dump_json())
+        handle_response(response)
+        return BucketResponse.model_validate_json(response.content)
+
+    async def get_bucket_config(self, bucket_id: UUID) -> BucketResponse:
+        response = await self._request("GET", f"/orgs/{self._config.org}/buckets/{bucket_id}")
+        handle_response(response)
+        return BucketResponse.model_validate_json(response.content)
+
+    async def modify_bucket_config(self, bucket_id: UUID, bucket_config: BucketModifyRequest) -> BucketResponse:
+        response = await self._request("PATCH", f"/orgs/{self._config.org}/buckets/{bucket_id}", content=bucket_config.model_dump_json())
+        handle_response(response)
+        return BucketResponse.model_validate_json(response.content)
+
+    async def delete_bucket_config(self, bucket_id: UUID) -> None:
+        response = await self._request("DELETE", f"/orgs/{self._config.org}/buckets/{bucket_id}")
+        handle_response(response)
+
+    async def list_bucket_configs(self) -> list[BucketResponse]:
+        response = await self._request("GET", f"/orgs/{self._config.org}/buckets")
+        handle_response(response)
+        return LIST_BUCKETS_ADAPTER.validate_json(response.content)
+
+    async def list_repos_for_bucket_config(self, bucket_id: UUID) -> list[Repo]:
+        response = await self._request("GET", f"/orgs/{self._config.org}/buckets/{bucket_id}/repos")
+        handle_response(response)
+        return LIST_REPOS_FOR_BUCKET_ADAPTER.validate_json(response.content)
+
+    async def set_default_bucket_config(self, bucket_id: UUID) -> None:
+        response = await self._request("POST", f"/orgs/{self._config.org}/buckets/{bucket_id}/default")
+        handle_response(response)
+
 
 @dataclass
 class HttpMetastoreDatabaseConfig:
     """Encapsulates the configuration for an HttpMetastoreDatabase"""
 
     http_metastore_config: HttpMetastoreConfig
     repo: str
@@ -190,28 +241,42 @@
             yield commit
 
     async def get_commit_by_id(self, commit_id: CommitID) -> Commit:
         response = await self._request("GET", f"{self._repo_path}/commits/{commit_id}")
         handle_response(response)
         return Commit.model_validate_json(response.content)
 
-    async def get_tags(self) -> tuple[Tag, ...]:
-        response = await self._request("GET", f"{self._repo_path}/tags")
+    async def get_tags(self, names: Sequence[TagName] | None = None) -> tuple[Tag, ...]:
+        params = {"names": names} if names else {}
+        response = await self._request("GET", f"{self._repo_path}/tags", params=params)
         handle_response(response)
         return tuple(GET_TAGS_ADAPTER.validate_json(response.content))
 
     async def get_branches(self, names: Sequence[BranchName] = []) -> tuple[Branch, ...]:
         params = {"names": names} if names else {}
         response = await self._request("GET", f"{self._repo_path}/branches", params=params)
         handle_response(response)
         return tuple(GET_BRANCHES_ADAPTER.validate_json(response.content))
 
     async def get_refs(self) -> tuple[tuple[Tag, ...], tuple[Branch, ...]]:
         return tuple(await async_gather(self.get_tags(), self.get_branches()))
 
+    async def new_tag(self, tag: NewTag) -> Tag:
+        response = await self._request("PUT", f"{self._repo_path}/tags", content=tag.model_dump_json())
+        handle_response(response)
+        return Tag.model_validate(response.json())
+
+    async def delete_tag(self, tag_name: TagName) -> bool:
+        response = await self._request("DELETE", f"{self._repo_path}/tags", params={"name": tag_name})
+        handle_response(response)
+        # Note: any possible errors are re-raised from handle_response,
+        # so if we get here, we have succeeded adding a tag.
+        # and "acknowledged" is always True
+        return response.json()["acknowledged"]
+
     async def new_commit(self, commit_info: NewCommit) -> CommitID:
         response = await self._request("PUT", f"{self._repo_path}/commits", content=commit_info.model_dump_json())
         handle_response(response)
         return CommitID.fromhex(response.json()["_id"])
 
     async def old_style_rebase(self, commit_id: CommitID, upstream_branch: BranchName) -> CommitID:
         """Old method, needed for tests and compatibility with clients <= 0.7.6
@@ -244,14 +309,22 @@
         new_commit: CommitID,
         new_branch: bool = False,
     ) -> None:
         body = UpdateBranchBody(branch=branch, session_id=session_id, new_commit=new_commit, base_commit=base_commit, new_branch=new_branch)
         response = await self._request("PUT", f"{self._repo_path}/branches", content=body.model_dump_json())
         handle_response(response)
 
+    async def delete_branch(self, branch_name: BranchName) -> bool:
+        response = await self._request("DELETE", f"{self._repo_path}/branches", params={"name": branch_name})
+        handle_response(response)
+        # Note: any possible errors are re-raised from handle_response,
+        # so if we get here, we have succeeded adding a tag.
+        # and "acknowledged" is always True
+        return response.json()["acknowledged"]
+
     # FIXME: Do we need to re-home this, since it collides with the /sessions
     # path prefix?
     async def get_all_sessions_for_path(self, path: Path, *, collection: CollectionName) -> AsyncGenerator[DocSessionsResponse, None]:
         # keys are sids, values are deleted or not
         response = await self._request("GET", f"{self._repo_path}/sessions/{collection}/{path}")
         handle_response(response)
 
@@ -296,15 +369,15 @@
         for doc in docs:
             yield doc
 
     async def list_active_sessions(self) -> Sequence[SessionInfo]:
         response = await self._request("GET", f"{self._repo_path}/sessions")
         handle_response(response)
 
-        return LIST_OF_SESSIONS_ADAPTER.validate_json(response.content)
+        return LIST_SESSIONS_ADAPTER.validate_json(response.content)
 
     async def create_session(self, session_request: NewSession) -> SessionInfo:
         response = await self._request("POST", f"{self._repo_path}/sessions", content=session_request.model_dump_json())
         handle_response(response)
 
         return SessionInfo.model_validate_json(response.content)
 
@@ -348,24 +421,24 @@
             ]
         )
 
     async def del_docs(
         self, paths: Sequence[Path], *, collection: CollectionName, session_id: SessionID, base_commit: CommitID | None
     ) -> None:
         params = {"session_id": session_id, "base_commit": base_commit}
-        content = LIST_OF_PATHS_ADAPTER.dump_json(list(paths))
+        content = LIST_PATHS_ADAPTER.dump_json(list(paths))
         response = await self._request("PUT", f"{self._repo_path}/contents/{collection}/_bulk_delete", content=content, params=params)
         handle_response(response)
 
     async def _get_docs(
         self, paths: Sequence[Path], collection: CollectionName, session_id: SessionID, base_commit: CommitID | None
     ) -> list[DocResponse]:
         """Submits a list of paths to the server to be retrieved in bulk."""
         params = {"session_id": session_id, "base_commit": str(base_commit) if base_commit else None}
-        content = LIST_OF_PATHS_ADAPTER.dump_json(list(paths))
+        content = LIST_PATHS_ADAPTER.dump_json(list(paths))
         response = await self._request("POST", f"{self._repo_path}/contents/{collection}/_bulk_get", content=content, params=params)
         handle_response(response)
         return GET_DOCS_ADAPTER.validate_json(response.content)
 
     async def get_docs(
         self, paths: Sequence[Path], *, collection: CollectionName, session_id: SessionID, base_commit: CommitID | None
     ) -> AsyncGenerator[DocResponse, None]:
@@ -405,15 +478,15 @@
                 "all_subdirs": all_subdirs,
                 "filter": filter,
             },
         )
         handle_response(response)
 
         # TODO: stream or paginate this
-        paths = LIST_OF_PATHS_ADAPTER.validate_json(response.content)
+        paths = LIST_PATHS_ADAPTER.validate_json(response.content)
         for path in paths:
             yield path
 
     async def getsize(
         self,
         prefix: str,
         *,
@@ -475,10 +548,7 @@
         }
         response = await self._request(
             "PUT",
             f"{self._repo_path}/contents/nodes/rename",
             params=params,
         )
         handle_response(response)
-
-    async def delete_branch(self, branch_name: BranchName) -> bool:
-        raise NotImplementedError("Branch delete not supported")
```

### Comparing `arraylake-0.9.5/arraylake/repo.py` & `arraylake-0.9.6/arraylake/repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,29 +67,33 @@
     DocumentNotFoundError,
     InvalidPrefixError,
 )
 from arraylake.log_util import get_logger
 from arraylake.metastore import MetastoreDatabase
 from arraylake.types import (
     Author,
+    Branch,
     BranchName,
     CollectionName,
     Commit,
     CommitID,
     CommitIDHex,
     DBIDBytes,
     NewCommit,
     NewSession,
+    NewTag,
     Path,
     ReferenceData,
     SessionExpirationUpdate,
     SessionID,
     SessionInfo,
     SessionPathsResponse,
     SessionType,
+    Tag,
+    TagName,
     Tree,
     to_dbid_bytes,
 )
 from arraylake.virtual import (
     VirtualLocation,
     reformat_kerchunk_refs,
     scan_grib2,
@@ -340,14 +344,20 @@
         return self._commit_data
 
     async def commit_log(self) -> CommitLog:
         """Returns the #CommitLog for the current session."""
 
         return CommitLog(self.repo_name, self.session.base_commit, await self.commit_data(True))
 
+    async def tags(self) -> Sequence[Tag]:
+        return await self.db.get_tags()
+
+    async def branches(self) -> Sequence[Branch]:
+        return await self.db.get_branches()
+
     async def status(self, limit: int = 1000) -> SessionStatus:
         """Returns the #SessionStatus for the current session.
 
         Args:
             limit (int): [Optional] The number of modified paths to return. Defaults to 1000, passing 0
             is equivalent to setting no limit.
         """
@@ -359,33 +369,33 @@
         return SessionStatus(repo_name=self.repo_name, session=self.session, modified_paths=list(modified_paths))
 
     async def ping(self) -> None:
         """Ping the metastore to confirm connection"""
         await self.db.ping()
         await self.chunkstore.ping()
 
-    async def _get_ref_for_checkout(self, ref: str | CommitID):
+    async def _get_ref_for_checkout(self, ref: str | CommitID | None) -> tuple[CommitID | None, BranchName | None]:
         from .commits import get_ref
 
+        if ref is None:
+            return (self.session.base_commit, self.session.branch)
+
         if isinstance(ref, str):
+            # This is a perf optimization to avoid downloading a large number of commits if we can.
+            branch_list, tag_list = await async_gather(self.db.get_branches(names=[BranchName(ref)]), self.db.get_tags([TagName(ref)]))
+            branches = {branch.id: branch.commit_id for branch in branch_list}
+            tags = {tag.label: tag.commit.id for tag in tag_list}
             try:
-                ref = CommitID.fromhex(ref)
+                return get_ref(ref, commits=None, branches=branches, tags=tags)
             except ValueError:
-                # Not a commit we will try branches and tags
+                # not a branch or a tag, try commits
                 pass
 
-        if isinstance(ref, DBIDBytes):
-            commit_data = await self.commit_data()
-            return get_ref(ref, commits=commit_data.commits, branches=commit_data.branches, tags=commit_data.tags)
-        else:
-            branches_list = await self.db.get_branches(names=[BranchName(ref)])
-            branches = {branch.id: branch.commit_id for branch in branches_list}
-            tag_list = await self.db.get_tags()
-            tags = {tag.id: tag.commit_id for tag in tag_list}
-            return get_ref(ref, branches=branches, tags=tags)
+        commit_data = await self.commit_data()
+        return get_ref(ref, commits=commit_data.commits, branches=commit_data.branches, tags=commit_data.tags)
 
     async def list_active_sessions(self) -> Sequence[SessionInfo]:
         """Obtain a time-ordered list of active sessions"""
         return await self.db.list_active_sessions()
 
     async def create_session(
         self,
@@ -399,17 +409,14 @@
         Args:
             ref: The branch or commit to start the session from.
             for_writing: Whether the session is for writing or reading. Defaults to True (for writing).
             expires_in: The duration the session should last. Defaults to 24 hours, maximum acceptable value is 7 days.
             message: A description or message annotating the session. Defaults to None."""
         session_start_time = datetime.datetime.utcnow()
 
-        # TODO: This is a temporary hack to allow our users to pass CommitIDs
-        # instead of strings. We need to change the type annotation to match
-        ref = str(ref) if isinstance(ref, DBIDBytes) else ref
         commit, branch = await self._get_ref_for_checkout(ref)
 
         session_type = SessionType.read_only
 
         if for_writing:
             session_type = SessionType.write
 
@@ -835,29 +842,61 @@
         return branch_latest_commit
 
     @_write_op
     async def _rename(self, src_path: Path, dst_path: Path) -> None:
         session = self.session
         await self.db.rename(src_path, dst_path, session_id=session.id, base_commit=session.base_commit)
 
+    async def tag(self, tag_name: str, commit_id: str | CommitID | None = None, *, message: str | None = None) -> Tag:
+        if tag_name == str(self.session.branch):
+            raise ValueError(f"Cannot create tag {tag_name!r} because a branch of the same name already exists.")
+        tag = TagName(tag_name)
+        # need to know latest commit to allow `repo.commit("foo").tag("zoo")`
+        await self.commit_data(refresh=True)
+        commit_id, _ = await self._get_ref_for_checkout(commit_id)
+        if commit_id is None:
+            raise ValueError("Can't create a tag without creating a commit first.")
+        return await self.db.new_tag(
+            NewTag(label=tag, commit_id=commit_id, message=message, author_name=self.author.name, author_email=self.author.email)
+        )
+
+    async def delete_tag(self, tag_name: str) -> None:
+        """Delete a tag.
+
+        Args:
+            tag_name: Name of tag to delete
+        """
+        await self.db.delete_tag(TagName(tag_name))
+
     async def new_branch(self, branch_name: str) -> None:
         """Create a new branch based on the current session reference
 
         Args:
             branch_name: New branch name
         """
 
         branch = BranchName(branch_name)
+        maybe_tag = TagName(branch_name)
         if self._session is None:
             # this was added to make mypy happy but is not covered by tests
             raise ValueError("There is no session active. You have to call checkout first.")
-        if branch == self.session.branch or (await self.db.get_branches([branch])):
-            raise ValueError(f"Branch {branch} already exists.")
+        # TODO: migrate to async_gather, or a new get_ref endpoint
+        has_ref = await self.db.get_branches([branch]) or await self.db.get_tags([TagName(maybe_tag)])
+        if branch == self.session.branch or has_ref:
+            raise ValueError(f"Branch {branch!r} already exists.")
         self._session.branch = branch
 
+    async def delete_branch(self, branch: str) -> None:
+        """Delete a branch.
+
+        Args:
+            branch: Name of branch to delete
+        """
+        await self.db.delete_branch(BranchName(branch))
+
     @_write_op
     async def _set_doc(self, path: Path, *, content: dict) -> None:
         """Write a single document to the metastore
 
         Parameters
         ----------
         path : str
@@ -1435,17 +1474,17 @@
             kwargs: Additional arguments to pass to the kerchunk
               [file format backend](https://fsspec.github.io/kerchunk/reference.html#file-format-backends).
               Do not pass `storage_options` or `inline_threshold`.
         """
         fs_config = self._validate_fs_config_for_uri(grib_uri)
         kerchunk_refs = scan_grib2(fs_config, grib_uri, **kwargs)
         meta_docs, chunk_locations, inlined_refs = reformat_kerchunk_refs(kerchunk_refs, path)
-        await self._set_docs(meta_docs)
-        await self._set_chunk_refs(self._chunk_locations_to_refs(chunk_locations))
-        await self._set_chunks(inlined_refs)
+        await async_gather(
+            self._set_docs(meta_docs), self._set_chunks(inlined_refs), self._set_chunk_refs(self._chunk_locations_to_refs(chunk_locations))
+        )
 
     @_write_op
     async def add_virtual_netcdf(self, netcdf_uri: str, path: Path, **kwargs) -> None:
         """Add a virtual Netcdf dataset to the repo.
 
         Args:
             netcdf_uri: The path to the netCDF file. Only `s3://` and `gs://` URIs are supported.
@@ -1456,16 +1495,15 @@
               Do not pass `storage_options` or `inline_threshold`.
         """
         fs_config = self._validate_fs_config_for_uri(netcdf_uri)
         kerchunk_refs = scan_netcdf(fs_config, netcdf_uri, **kwargs)
         meta_docs, chunk_locations, inlined_refs = reformat_kerchunk_refs(kerchunk_refs, path)
         if inlined_refs:
             raise ValueError("Inlined references are not supported by Arraylake.")
-        await self._set_docs(meta_docs)
-        await self._set_chunk_refs(self._chunk_locations_to_refs(chunk_locations))
+        await async_gather(self._set_docs(meta_docs), self._set_chunk_refs(self._chunk_locations_to_refs(chunk_locations)))
 
     @_write_op
     async def add_virtual_zarr(self, zarr_uri: str, path: Path) -> None:
         """Add a virtual Zarr dataset to the repo.
 
         Args:
             zarr_uri: The path to the Zarr store. Only Zarr V2 stores and `s3://` or `gs://` URIs are supported at the moment.
@@ -1496,16 +1534,15 @@
             per overview level named '0', '1', '2', etc.
         """
         fs_config = self._validate_fs_config_for_uri(tiff_uri)
         kerchunk_refs = scan_tiff(fs_config, tiff_uri, name, **kwargs)
         meta_docs, chunk_locations, inlined_refs = reformat_kerchunk_refs(kerchunk_refs, path)
         if inlined_refs:
             raise ValueError("Inlined references are not supported by Arraylake.")
-        await self._set_docs(meta_docs)
-        await self._set_chunk_refs(self._chunk_locations_to_refs(chunk_locations))
+        await async_gather(self._set_docs(meta_docs), self._set_chunk_refs(self._chunk_locations_to_refs(chunk_locations)))
 
     async def filter_metadata(self, filter: str) -> list[str]:
         """
         Filter repo metadata documents using a JMSE search string.
 
         https://jmespath.org/specification.html
         """
@@ -1647,23 +1684,47 @@
         """Fast-forward the session.
         Attempts to update the session base commit to the latest branch tip.
         Will fail if the same paths have been modified in the current session and on the branch.
         """
 
         return self._synchronize(self._arepo.fast_forward)
 
+    def tag(self, tag_name: str, commit_id: str | CommitID | None = None, *, message: str | None = None) -> Tag:
+        """Add a new tag.
+
+        Args:
+            tag_name: Tag name
+            commit_id: Commit to tag
+        """
+        return self._synchronize(self._arepo.tag, tag_name=tag_name, commit_id=commit_id, message=message)
+
+    def delete_tag(self, tag_name: str) -> None:
+        """Delete an existing tag.
+
+        Args:
+            tag_name: Tag name
+        """
+        self._synchronize(self._arepo.delete_tag, tag_name=tag_name)
+
     def new_branch(self, branch: str) -> None:
         """Create a new branch based on the current session reference
 
         Args:
             branch_name: New branch name
         """
-
         return self._synchronize(self._arepo.new_branch, branch)
 
+    def delete_branch(self, branch: str) -> None:
+        """Delete an existing branch.
+
+        Args:
+            branch: Branch name
+        """
+        self._synchronize(self._arepo.delete_branch, branch=branch)
+
     def list_active_sessions(self) -> Sequence[SessionInfo]:
         """List all active sessions."""
         return self._synchronize(self._arepo.list_active_sessions)
 
     def create_session(
         self,
         ref: str | CommitID = "main",
@@ -1779,16 +1840,27 @@
         Args:
            limit (int): [Optional] The number of modified paths to return. Defaults to 1000, passing 0
            is equivalent to setting no limit."""
         return self._synchronize(self._arepo.status, limit=limit)
 
     @property
     def commit_log(self):
+        """Returns a log of all commits on the current branch."""
         return self._synchronize(self._arepo.commit_log)
 
+    @property
+    def tags(self):
+        "Returns a list of tag names."
+        return self._synchronize(self._arepo.tags)
+
+    @property
+    def branches(self):
+        """Returns a list of branch names."""
+        return self._synchronize(self._arepo.branches)
+
     def add_virtual_grib(self, grib_uri: str, path: Path) -> None:
         """Add a virtual GRIB2 dataset to the repo.
 
         Args:
             path: The path within the repo where the virtual dataset should be created.
             grib_uri: The path to the GRIB2 file. Only `s3://` or `gs://` URIs are supported at the moment.
         """
```

### Comparing `arraylake-0.9.5/arraylake/retrier.py` & `arraylake-0.9.6/arraylake/retrier.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.5/arraylake/token.py` & `arraylake-0.9.6/arraylake/token.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.5/arraylake/types.py` & `arraylake-0.9.6/arraylake/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import sys
 from collections.abc import Iterator, Mapping
 from dataclasses import dataclass
 from datetime import datetime, timedelta, timezone
 from enum import Enum, IntEnum
 from typing import Annotated, Any, Literal, NewType, Optional, Union
 from uuid import UUID
@@ -12,14 +14,15 @@
     BaseModel,
     ConfigDict,
     EmailStr,
     EncodedBytes,
     EncoderProtocol,
     Field,
     SecretStr,
+    computed_field,
     field_serializer,
     field_validator,
     model_validator,
 )
 from typing_extensions import TypedDict
 
 if sys.version_info >= (3, 11):
@@ -197,44 +200,175 @@
     # AUTHENTICATED_PUBLIC: Visible to any authenticated user of Arraylake.
     AUTHENTICATED_PUBLIC = "AUTHENTICATED_PUBLIC"
 
     # PUBLIC: Visible to anybody on the public internet.
     # PUBLIC = "PUBLIC"
 
 
-Platform = Literal["s3", "minio", "gs"]
-AuthMethod = Literal["customer_managed_role", "bucket_policy", "hmac", "anonymous"]
+Platform = Literal["s3", "s3-compatible", "minio", "gs"]
+
+
+class CustomerManagedRoleAuth(BaseModel):
+    method: Literal["customer_managed_role"]
+    external_customer_id: str
+    external_role_name: str
+
+
+class BucketPolicyAuth(BaseModel):
+    method: Literal["bucket_policy"]
+
+
+class HmacAuth(BaseModel):
+    method: Literal["hmac"]
+    access_key_id: SecretStr
+    secret_access_key: SecretStr
+
+    @field_serializer("access_key_id", "secret_access_key", when_used="json")
+    def dump_secret(self, v):
+        return v.get_secret_value()
+
+
+class AnonymousAuth(BaseModel):
+    method: Literal["anonymous"]
+
+
+AuthConfig = Union[CustomerManagedRoleAuth, BucketPolicyAuth, HmacAuth, AnonymousAuth]
 
 
 class Bucket(BaseModel):
     id: UUID
     nickname: str
     platform: Platform
     name: str
+    created: datetime = Field(default_factory=utc_now)
+    updated: datetime
+    created_by: Optional[EmailStr] = None
+    prefix: str = ""
     extra_config: Mapping[str, Union[str, bool]]
 
+    # NOTE: To prevent credential leakage, we don't share the auth_config here.
+
+    @model_validator(mode="before")
+    @classmethod
+    def set_initial_updated(cls, data: Any) -> Any:
+        if isinstance(data, dict) and "updated" not in data:
+            data["updated"] = data.get("created", utc_now())
+        return data
+
+    @field_validator("created", "updated")
+    @classmethod
+    def timestamp_in_utc_tz(cls, v: datetime) -> datetime:
+        return v.replace(tzinfo=timezone.utc)
+
+    @field_serializer("created", "updated")
+    def serialize_datetime(self, dt: datetime) -> str:
+        return datetime_to_isoformat(dt)
+
+
+class NewBucket(BaseModel):
+    nickname: str
+    platform: Platform
+    name: str
+    prefix: str = ""  # default for compatibility with older data
+    extra_config: Mapping[str, Union[str, bool]]
+    auth_config: AuthConfig = Field(discriminator="method")
+
+    # NOTE: Validation on name is not necessary, as S3 has fairly strict naming
+    # rules. If name doesn't exactly match the S3 bucket name, then we have a
+    # bigger problem than simple naming rules.
+
+    @field_validator("prefix")
+    @classmethod
+    def validate_prefix(cls, prefix: str) -> str:
+        # Remove leading and trailing whitespace.
+        prefix = prefix.strip()
+        if len(prefix) > 900:  # S3 max key size minus some buffer for key
+            raise ValueError("Bucket prefix must be at most 900 characters long.")
+        if prefix.startswith("/") or prefix.endswith("/"):
+            raise ValueError("Bucket prefix must not start or end with a slash.")
+        return prefix
+
+    @field_validator("nickname")
+    @classmethod
+    def validate_nickname(cls, nickname: str) -> str:
+        # Remove leading and trailing whitespace.
+        nickname = nickname.strip()
+
+        # NOTE: We only impose a limit on string size. This is intended to be a
+        # human-friendly identifier, so we're looser than e.g. S3 regarding
+        # naming conventions and restrictions.
+        if len(nickname) < 3:
+            raise ValueError("Bucket nickname must be at least 3 characters long.")
+        if len(nickname) > 64:
+            raise ValueError("Bucket nickname must be at most 64 characters long.")
+        return nickname
+
+    def region_name(self) -> str | None:
+        region = self.extra_config.get("region_name")
+        return str(region) if region else None
+
+
+class BucketModifyRequest(BaseModel):
+    """A request with optional fields to modify a bucket's config on a per-field
+    basis."""
+
+    nickname: str | None = None
+    platform: Platform | None = None
+    name: str | None = None
+    prefix: str | None = None
+    extra_config: dict[str, Any] | None = None
+    auth_config: AuthConfig | None = None
+
+
+class BucketResponse(Bucket):
+    is_default: bool
+
+    # NOTE: Once written, credential secrets are not included in the response.
+    # However, for UX purposes, we return the *type* of auth method, so that
+    # values can be modified in the UI.
+    auth_method: str
+
+
+class RepoOperationMode(StrEnum):
+    ONLINE = "online"
+    MAINTENANCE = "maintenance"
+    OFFLINE = "offline"
+
+
+class NewRepoOperationStatus(BaseModel):
+    mode: RepoOperationMode
+    message: str | None = None
+
+
+class RepoOperationStatusResponse(NewRepoOperationStatus):
+    initiated_by: dict
+    estimated_end_time: datetime | None = None
+
 
 class Repo(ModelWithID):
     org: str
     name: str
     created: datetime = Field(default_factory=utc_now)
     updated: datetime
     description: Optional[str] = None
     created_by: Optional[UUID] = None
     visibility: RepoVisibility = RepoVisibility.PRIVATE
-    bucket: Optional[Bucket] = None
+    bucket: Optional[BucketResponse] = None
+    status: RepoOperationStatusResponse
 
     def _asdict(self):
         """custom dict method ready to be serialized as json"""
         d = self.model_dump()
         d["id"] = str(d["id"])
         if self.created_by is not None:
             d["created_by"] = str(d["created_by"])
         if d["bucket"]:
             d["bucket"]["id"] = str(d["bucket"]["id"])
+        if d["status"]["estimated_end_time"]:
+            d["status"]["estimated_end_time"] = datetime_to_isoformat(d["status"]["estimated_end_time"])
         return d
 
     def __repr__(self):
         return f"<Repo {self.org}/{self.name} created at {self.created} by {self.created_by}. Last updated at {self.updated}>"
 
     @model_validator(mode="before")
     @classmethod
@@ -264,17 +398,17 @@
         else:
             return f"<{self.email}>"
 
 
 class NewCommit(BaseModel):
     session_id: SessionID
     session_start_time: datetime
-    parent_commit: Optional[CommitID] = None
+    parent_commit: CommitID | None = None
     commit_time: datetime
-    author_name: Optional[str] = None
+    author_name: str | None = None
     author_email: EmailStr
     # TODO: add constraints once we drop python 3.8
     # https://github.com/pydantic/pydantic/issues/156
     message: str
 
     @field_serializer("parent_commit")
     def serialize_commit_id(self, parent_commit: Optional[CommitID]) -> Optional[CommitIDHex]:
@@ -339,36 +473,88 @@
         return to_dbid_bytes(id)
 
     @field_serializer("commit_id")
     def serialize_commit_id(self, commit_id: CommitID) -> CommitIDHex:
         return str(commit_id)
 
 
-class Tag(BaseModel):
-    id: TagName = Field(alias="_id")
+class NewTag(BaseModel):
+    label: TagName
     commit_id: CommitID
+    # TODO: add constraints once we drop python 3.8
+    # https://github.com/pydantic/pydantic/issues/156
+    message: str | None
+    author_name: Optional[str] = None
+    author_email: EmailStr
 
     model_config = ConfigDict(populate_by_name=True, arbitrary_types_allowed=True)
 
     @field_validator("commit_id", mode="before")
     @classmethod
     def validate_commit_id(cls, id: CommitID) -> DBIDBytes:
         return to_dbid_bytes(id)
 
     @field_serializer("commit_id")
     def serialize_commit_id(self, commit_id: CommitID) -> CommitIDHex:
         return str(commit_id)
 
 
+class Tag(BaseModel):
+    # ---
+    # This field exists for backcompat with arraylake<=0.9.5
+    # Delete when we don't support those versions
+    id: TagName = Field(alias="label")
+    # ---
+
+    label: TagName
+    created_at: datetime
+    commit: Commit
+    # TODO: add constraints once we drop python 3.8
+    # https://github.com/pydantic/pydantic/issues/156
+    message: str | None
+    author_name: Optional[str] = None
+    author_email: EmailStr
+
+    # ---
+    # These fields exist for backcompat with arraylake<=0.9.5
+    # Delete when we don't support those versions
+    @computed_field  # type: ignore[misc]
+    @property
+    def _id(self) -> TagName:
+        return self.label
+
+    @computed_field  # type: ignore[misc]
+    @property
+    def commit_id(self) -> CommitID:
+        return self.commit.id
+
+    @field_validator("commit_id", mode="before")
+    @classmethod
+    def validate_commit_id(cls, id: CommitID) -> DBIDBytes:
+        return to_dbid_bytes(id)
+
+    @field_serializer("commit_id")
+    def serialize_commit_id(self, commit_id: CommitID) -> CommitIDHex:
+        return str(commit_id)
+
+    # ---
+
+    @field_serializer("created_at")
+    def serialize_created_at_time(self, t: datetime) -> str:
+        return datetime_to_isoformat(t)
+
+    model_config = ConfigDict(populate_by_name=True, arbitrary_types_allowed=True)
+
+
 @dataclass
 class DocResponse:
     id: str  # not DBID
     session_id: SessionID
     path: Path
-    content: Optional[Mapping[str, Any]] = None
+    content: Mapping[str, Any] | None = None
     deleted: bool = False
 
     def __post_init__(self):
         checks = [
             isinstance(self.id, str),
             # session_id: Cannot use isinstance() with NewType, so we use str
             isinstance(self.session_id, str),
@@ -422,42 +608,42 @@
         # it has to be None
         if v == ChunkstoreSchemaVersion.V0:
             return None
         else:
             return v
 
     @classmethod
-    def new_virtual(cls, for_version: ChunkstoreSchemaVersion, uri: str, offset: int, length: int, sid: SessionID) -> "ReferenceData":
+    def new_virtual(cls, for_version: ChunkstoreSchemaVersion, uri: str, offset: int, length: int, sid: SessionID) -> ReferenceData:
         return cls(
             uri=uri,
             offset=offset,
             length=length,
             hash=None,
             v=for_version,
             sid=None if for_version == ChunkstoreSchemaVersion.V0 else sid,
         )
 
     @classmethod
-    def new_inline(cls, for_version: ChunkstoreSchemaVersion, data: str, length: int, hash: ChunkHash, sid: SessionID) -> "ReferenceData":
+    def new_inline(cls, for_version: ChunkstoreSchemaVersion, data: str, length: int, hash: ChunkHash, sid: SessionID) -> ReferenceData:
         assert data.startswith("inline://") or data.startswith("base64:"), "Invalid inline data format"
         return cls(
             uri=data,
             offset=0,
             length=length,
             hash=hash,
             v=for_version,
             sid=None if for_version == ChunkstoreSchemaVersion.V0 else sid,
         )
 
     @classmethod
-    def new_materialized_v0(cls, uri: str, length: int, hash: ChunkHash) -> "ReferenceData":
+    def new_materialized_v0(cls, uri: str, length: int, hash: ChunkHash) -> ReferenceData:
         return cls(uri=uri, offset=0, length=length, hash=hash, v=ChunkstoreSchemaVersion.V0, sid=None)
 
     @classmethod
-    def new_materialized_v1(cls, length: int, hash: ChunkHash, sid: SessionID) -> "ReferenceData":
+    def new_materialized_v1(cls, length: int, hash: ChunkHash, sid: SessionID) -> ReferenceData:
         return cls(
             uri=None,
             offset=0,
             length=length,
             hash=hash,
             v=ChunkstoreSchemaVersion.V1,
             sid=sid,
@@ -623,15 +809,15 @@
     elif isinstance(arr.data_type, dict):
         return str(arr.data_type["type"])
     else:
         raise ValueError(f"unexpected array type {type(arr.data_type)}")
 
 
 class Tree(BaseModel):
-    trees: dict[str, "Tree"] = {}
+    trees: dict[str, Tree] = {}
     arrays: dict[str, Array] = {}
     attributes: dict[str, Any] = {}
 
     def _as_rich_tree(self, name: str = "/"):
         from rich.jupyter import JupyterMixin
         from rich.tree import Tree as _RichTree
```

### Comparing `arraylake-0.9.5/arraylake/virtual.py` & `arraylake-0.9.6/arraylake/virtual.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.5/arraylake/zarr_util.py` & `arraylake-0.9.6/arraylake/zarr_util.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.5/pyproject.toml` & `arraylake-0.9.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "arraylake"
-version = "0.9.5"  # placeholder
+version = "0.9.6"  # placeholder
 description = "Python client for ArrayLake"
 authors = ["Joe Hamman <joe@earthmover.io>"]
 readme = "README.md"
 packages = [{include = "arraylake"}]
 
+[[tool.poetry.source]]
+name = "pytorch-cpu-src"
+url = "https://download.pytorch.org/whl/cpu"
+priority = "explicit"
+
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "pep440"
 strict = true
 
 
 # Poetry doesn't allows us to install min specified version, so we duplicate
 # from ci/client-install-min-deps.sh here
 # https://github.com/python-poetry/poetry/issues/3527#issuecomment-939549116
 [tool.poetry.dependencies]
-python = ">=3.9,<3.13"
+python = ">=3.10,<3.13"
 aiobotocore = { version = "^2.4.0", extras = ["boto3"]}
 boto3 = "^1.24"
 botocore = "^1.27"
 uvloop = { version = ">=0.17,<1.0", markers="os_name=='posix'", optional = true}
 zarr = ">=2.14,<=2.18"
 numcodecs = "!=0.12.0"
-numpy = "^1.20"
+numpy = "^1.23"
 donfig = ">=0.7,<1.0"
 pydantic = {extras = ["email"], version = "^2.3"}
 httpx = ">=0.23.0,<1.0"
 ruamel-yaml = { version = ">=0.17,<1.0" }
 typer = { version = ">=0.6.1,<1.0" }
 rich = { version = ">=12.6,<14.0" }
 cachetools = "^5.3.2"
-structlog = "^23.1.0"
+structlog = "^24.1.0"
 python-dateutil = "^2.8"
 click = { version = "^8.1" }
 aioitertools = "^0.11.0"
 fsspec = ">=2023.01.0"
 gcsfs = ">=2023.01"
 kerchunk = { version = ">=0.1,<1.0,!=0.2.1", optional = true }
 tifffile = { version = ">=2023.2.27", optional = true }
@@ -81,18 +86,18 @@
 [tool.poetry.group.maximal]
 # By default, dependencies across all non-optional groups will be installed when executing poetry install.
 optional = false
 [tool.poetry.group.maximal.dependencies]
 netCDF4 = "^1.6.1"
 xarray = ">=2022.12.0"
 rioxarray = "^0.15"
-pandas = ">=1.3"
+pandas = "^2"
 dask = ">=2022.10.2"
 distributed = ">=2022.10.2"
-scipy = "^1.10.1"
+scipy = "^1.10"
 
 [tool.poetry.group.grib]
 # By default, dependencies across all non-optional groups will be installed when executing poetry install.
 optional = true
 
 [tool.poetry.group.grib.dependencies]
 cfgrib = "^0.9"
@@ -101,19 +106,24 @@
 ipdb = "^0.13.13"
 
 [tool.poetry.group.performance]
 # By default, dependencies across all non-optional groups will be installed when executing poetry install.
 optional = true
 
 [tool.poetry.group.performance.dependencies]
-locust = "^2.16.1"
-xarray = ">=2022.12.0"
-pandas = "^1.3"
-dask = "^2022.10.2"
-distributed = "^2022.10.2"
+locust = ">=2.16"
+xarray = ">=2023.12"
+pandas = ">=1.3"
+dask = ">=2023.10"
+distributed = ">=2023.10"
+xbatcher = ">=0.3.0"
+ipython = ">=7"
+# Note: this does not work on macos
+# Using custom wheel makes locking quite slow. pip install pytorch in performance.Dockerfile instead
+# torch = {version = ">=2.2.1", source = "pytorch-cpu-src"}
 
 [tool.poetry.scripts]
 arraylake = 'arraylake.cli.main:app'
 al = 'arraylake.cli.main:app'
 
 [tool.poetry.extras]
 virtual = ["kerchunk", "h5py", "s3fs", "tifffile"]
@@ -133,14 +143,16 @@
 [tool.pytest.ini_options]
 markers = ["slow: mark test as slow", "add_object_store: add object store backend to test"]
 norecursedirs = ["tests/helpers"]
 filterwarnings = [
     'ignore:.*pkg_resources.*:DeprecationWarning',
     'ignore:.*make_current is deprecated; start the event loop first.*:DeprecationWarning',
     'ignore:.*no current event loop.*:DeprecationWarning',
+    'error:ZARR_V3_EXPERIMENTAL_API must be set before importing the arraylake client .*:UserWarning',
+    'ignore:The experimental Zarr V3 implementation .*:FutureWarning'
 ]
 asyncio_mode = "auto"
 
 
 [tool.mypy]
 warn_unused_configs = true
 warn_redundant_casts = true
```

### Comparing `arraylake-0.9.5/PKG-INFO` & `arraylake-0.9.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: arraylake
-Version: 0.9.5
+Version: 0.9.6
 Summary: Python client for ArrayLake
 Author: Joe Hamman
 Author-email: joe@earthmover.io
-Requires-Python: >=3.9,<3.13
+Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: grib
 Provides-Extra: virtual
 Provides-Extra: widgets
 Provides-Extra: xarray
@@ -27,21 +26,21 @@
 Requires-Dist: fsspec (>=2023.01.0)
 Requires-Dist: gcsfs (>=2023.01)
 Requires-Dist: h5py (>=3.7.0,<4.0.0) ; extra == "virtual"
 Requires-Dist: httpx (>=0.23.0,<1.0)
 Requires-Dist: ipytree (>=0.2.2,<1.0) ; extra == "widgets"
 Requires-Dist: kerchunk (>=0.1,<1.0,!=0.2.1) ; extra == "virtual" or extra == "grib"
 Requires-Dist: numcodecs (!=0.12.0)
-Requires-Dist: numpy (>=1.20,<2.0)
+Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: pydantic[email] (>=2.3,<3.0)
 Requires-Dist: python-dateutil (>=2.8,<3.0)
 Requires-Dist: rich (>=12.6,<14.0)
 Requires-Dist: ruamel-yaml (>=0.17,<1.0)
 Requires-Dist: s3fs (>=2023.01.0) ; extra == "virtual" or extra == "grib"
-Requires-Dist: structlog (>=23.1.0,<24.0.0)
+Requires-Dist: structlog (>=24.1.0,<25.0.0)
 Requires-Dist: tifffile (>=2023.2.27) ; extra == "virtual"
 Requires-Dist: typer (>=0.6.1,<1.0)
 Requires-Dist: uvloop (>=0.17,<1.0) ; os_name == "posix"
 Requires-Dist: xarray (>=v2022.12.0) ; extra == "xarray"
 Requires-Dist: zarr (>=2.14,<=2.18)
 Description-Content-Type: text/markdown
 
@@ -58,13 +57,13 @@
 
 Check out the [documentation](https://docs.earthmover.io) to get started.
 
 ## Install
 
 ```
 # using pip
-pip install "arraylake[cli]"
+pip install "arraylake"
 
 # using conda
 conda install arraylake
 ```
```

#### html2text {}

```diff
@@ -1,33 +1,32 @@
-Metadata-Version: 2.1 Name: arraylake Version: 0.9.5 Summary: Python client for
+Metadata-Version: 2.1 Name: arraylake Version: 0.9.6 Summary: Python client for
 ArrayLake Author: Joe Hamman Author-email: joe@earthmover.io Requires-Python:
->=3.9,<3.13 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Provides-Extra: grib Provides-Extra:
-virtual Provides-Extra: widgets Provides-Extra: xarray Requires-Dist:
-aiobotocore[boto3] (>=2.4.0,<3.0.0) Requires-Dist: aioitertools
-(>=0.11.0,<0.12.0) Requires-Dist: boto3 (>=1.24,<2.0) Requires-Dist: botocore
-(>=1.27,<2.0) Requires-Dist: cachetools (>=5.3.2,<6.0.0) Requires-Dist: cfgrib
-(>=0.9,<0.10) ; extra == "grib" Requires-Dist: click (>=8.1,<9.0) Requires-
-Dist: donfig (>=0.7,<1.0) Requires-Dist: eccodes (>=1.6,<2.0) ; extra == "grib"
-Requires-Dist: ecmwflibs (>=0.5,<=0.5.1) ; extra == "grib" Requires-Dist:
-fsspec (>=2023.01.0) Requires-Dist: gcsfs (>=2023.01) Requires-Dist: h5py
-(>=3.7.0,<4.0.0) ; extra == "virtual" Requires-Dist: httpx (>=0.23.0,<1.0)
-Requires-Dist: ipytree (>=0.2.2,<1.0) ; extra == "widgets" Requires-Dist:
-kerchunk (>=0.1,<1.0,!=0.2.1) ; extra == "virtual" or extra == "grib" Requires-
-Dist: numcodecs (!=0.12.0) Requires-Dist: numpy (>=1.20,<2.0) Requires-Dist:
-pydantic[email] (>=2.3,<3.0) Requires-Dist: python-dateutil (>=2.8,<3.0)
-Requires-Dist: rich (>=12.6,<14.0) Requires-Dist: ruamel-yaml (>=0.17,<1.0)
-Requires-Dist: s3fs (>=2023.01.0) ; extra == "virtual" or extra == "grib"
-Requires-Dist: structlog (>=23.1.0,<24.0.0) Requires-Dist: tifffile
+>=3.10,<3.13 Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Provides-
+Extra: grib Provides-Extra: virtual Provides-Extra: widgets Provides-Extra:
+xarray Requires-Dist: aiobotocore[boto3] (>=2.4.0,<3.0.0) Requires-Dist:
+aioitertools (>=0.11.0,<0.12.0) Requires-Dist: boto3 (>=1.24,<2.0) Requires-
+Dist: botocore (>=1.27,<2.0) Requires-Dist: cachetools (>=5.3.2,<6.0.0)
+Requires-Dist: cfgrib (>=0.9,<0.10) ; extra == "grib" Requires-Dist: click
+(>=8.1,<9.0) Requires-Dist: donfig (>=0.7,<1.0) Requires-Dist: eccodes
+(>=1.6,<2.0) ; extra == "grib" Requires-Dist: ecmwflibs (>=0.5,<=0.5.1) ; extra
+== "grib" Requires-Dist: fsspec (>=2023.01.0) Requires-Dist: gcsfs (>=2023.01)
+Requires-Dist: h5py (>=3.7.0,<4.0.0) ; extra == "virtual" Requires-Dist: httpx
+(>=0.23.0,<1.0) Requires-Dist: ipytree (>=0.2.2,<1.0) ; extra == "widgets"
+Requires-Dist: kerchunk (>=0.1,<1.0,!=0.2.1) ; extra == "virtual" or extra ==
+"grib" Requires-Dist: numcodecs (!=0.12.0) Requires-Dist: numpy (>=1.23,<2.0)
+Requires-Dist: pydantic[email] (>=2.3,<3.0) Requires-Dist: python-dateutil
+(>=2.8,<3.0) Requires-Dist: rich (>=12.6,<14.0) Requires-Dist: ruamel-yaml
+(>=0.17,<1.0) Requires-Dist: s3fs (>=2023.01.0) ; extra == "virtual" or extra
+== "grib" Requires-Dist: structlog (>=24.1.0,<25.0.0) Requires-Dist: tifffile
 (>=2023.2.27) ; extra == "virtual" Requires-Dist: typer (>=0.6.1,<1.0)
 Requires-Dist: uvloop (>=0.17,<1.0) ; os_name == "posix" Requires-Dist: xarray
 (>=v2022.12.0) ; extra == "xarray" Requires-Dist: zarr (>=2.14,<=2.18)
 Description-Content-Type: text/markdown
                                   [Arraylake]
                          _e_a_r_t_h_m_o_v_e_r_._i_o - _d_o_c_u_m_e_n_t_a_t_i_o_n
 Arraylake is a cloud-based platform that understands a wide array of
 multidimensional scientific data. Organize, analyze, build, and
 collaborateâeffortlessly. Check out the [documentation](https://
 docs.earthmover.io) to get started. ## Install ``` # using pip pip install
-"arraylake[cli]" # using conda conda install arraylake ```
+"arraylake" # using conda conda install arraylake ```
```

