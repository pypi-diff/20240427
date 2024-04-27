# Comparing `tmp/es_wait-0.3.3.tar.gz` & `tmp/es_wait-0.3.5.tar.gz`

## Comparing `es_wait-0.3.3.tar` & `es_wait-0.3.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 es_wait-0.3.3/pytest.ini
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 es_wait-0.3.3/src/es_wait/__init__.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 es_wait-0.3.3/src/es_wait/args.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 es_wait-0.3.3/src/es_wait/base.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 es_wait-0.3.3/src/es_wait/exists.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 es_wait-0.3.3/src/es_wait/health.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 es_wait-0.3.3/src/es_wait/relocate.py
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 es_wait-0.3.3/src/es_wait/restore.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 es_wait-0.3.3/src/es_wait/snapshot.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 es_wait-0.3.3/src/es_wait/task.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 es_wait-0.3.3/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.3.3/LICENSE
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.3.3/README.md
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 es_wait-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 es_wait-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 es_wait-0.3.5/pytest.ini
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 es_wait-0.3.5/src/es_wait/__init__.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 es_wait-0.3.5/src/es_wait/args.py
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 es_wait-0.3.5/src/es_wait/base.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 es_wait-0.3.5/src/es_wait/exists.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 es_wait-0.3.5/src/es_wait/health.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 es_wait-0.3.5/src/es_wait/relocate.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 es_wait-0.3.5/src/es_wait/restore.py
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 es_wait-0.3.5/src/es_wait/snapshot.py
+-rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 es_wait-0.3.5/src/es_wait/task.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 es_wait-0.3.5/.gitignore
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.3.5/LICENSE
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.3.5/README.md
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 es_wait-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 es_wait-0.3.5/PKG-INFO
```

### Comparing `es_wait-0.3.3/src/es_wait/args.py` & `es_wait-0.3.5/src/es_wait/args.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """Args Class"""
+
 import typing as t
 
+
 class Args(t.Dict):
     """
     Initialize with None values for all accepted settings
 
     Contains :py:meth:`update_settings` and :py:meth:`asdict` methods
     """
+
     def __init__(
-            self,
-            settings: t.Dict[str, t.Any] = None,
-            defaults: t.Dict[str, t.Any] = None,
-        ):
+        self,
+        settings: t.Dict[str, t.Any] = None,
+        defaults: t.Dict[str, t.Any] = None,
+    ):
         """Updatable object that turns dictionary keys into properties"""
         self.settings = settings
         if defaults is None:
             defaults = {}
         self.set_defaults(defaults)
         if settings is None:
             self.settings = defaults
@@ -41,21 +44,23 @@
         """Return as a dictionary"""
         retval = {}
         if isinstance(self.settings, dict):
             for setting in self.settings:
                 retval[setting] = getattr(self, setting, None)
         return retval
 
+
 class TaskArgs(Args):
     """Task-specific child class of Args"""
+
     def __init__(
-            self,
-            settings: t.Dict[str, t.Any] = None,
-            defaults: t.Dict[str, t.Any] = None,
-        ):
+        self,
+        settings: t.Dict[str, t.Any] = None,
+        defaults: t.Dict[str, t.Any] = None,
+    ):
         super().__init__(settings=settings, defaults=defaults)
         self.action = None
         self.completed = False
         self.description = None
         self.response = {}
         self.running_time_in_nanos = 0
         self.task = None
```

### Comparing `es_wait-0.3.3/src/es_wait/base.py` & `es_wait-0.3.5/src/es_wait/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """Base Waiter Class"""
+
 import typing as t
 import logging
 from time import sleep
 from datetime import datetime, timezone
 from elasticsearch8 import Elasticsearch
 
+
 class Waiter:
     """Class Definition"""
+
     ACTIONS = ['any', 'listed', 'actions']
+
     def __init__(
-            self,
-            client: Elasticsearch,
-            action: t.Union[str, t.Sequence[str]] = None,
-            pause: float = 9,    # The delay between checks
-            timeout: float = -1, # How long is too long
-        ) -> None:
+        self,
+        client: Elasticsearch,
+        action: str = '',
+        pause: float = 9,  # The delay between checks
+        timeout: float = -1,  # How long is too long
+    ) -> None:
         self.logger = logging.getLogger('es_wait.Base')
         self.client = client
         self.action = action
         self.pause = pause
         self.timeout = timeout
         self.checkid = 'check for Waiter class'
 
@@ -54,37 +58,40 @@
         success = False
         self.logger.debug('Only logging every %s seconds', frequency)
         while True:
             elapsed = int((self.now - start_time).total_seconds())
             if elapsed == 0:
                 loggit = False
             else:
-                loggit = elapsed % frequency == 0 # Only log every frequency seconds
+                loggit = elapsed % frequency == 0  # Only frequency seconds
             response = self.check
             # Successfully completed task.
             if response:
                 self.logger.debug('%s finished executing', self.checkid)
                 total = f'{(self.now - start_time).total_seconds():.2f}'
                 self.logger.debug('Elapsed time: %s seconds', total)
                 success = True
                 break
             # Not success, and reached timeout (if defined)
             if (self.timeout != -1) and (elapsed >= self.timeout):
-                msg = f'The {self.checkid} did not complete within {self.timeout} seconds.'
+                msg = (
+                    f'The {self.checkid} did not complete within {self.timeout} '
+                    f'seconds.'
+                )
                 self.logger.error(msg)
                 break
             # Not timed out and not yet success, so we wait.
             if loggit:
                 msg = (
-                    f'The {self.checkid} is not yet complete. {elapsed} total seconds have '
-                    f'elapsed. Pausing {self.pause} seconds between checks.'
+                    f'The {self.checkid} is not yet complete. {elapsed} total seconds '
+                    f'have elapsed. Pausing {self.pause} seconds between checks.'
                 )
                 self.logger.debug(msg)
-            sleep(self.pause) # Actual wait here
+            sleep(self.pause)  # Actual wait here
 
         if not success:
             msg = (
-                f'The {self.checkid} failed to complete in the '
-                f'timeout period of {self.timeout} seconds'
+                f'The {self.checkid} failed to complete in the timeout period of '
+                f'{self.timeout} seconds'
             )
             self.logger.error(msg)
             raise TimeoutError(msg)
```

### Comparing `es_wait-0.3.3/src/es_wait/exists.py` & `es_wait-0.3.5/src/es_wait/exists.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,71 @@
 """Entity Exists"""
+
 import typing as t
 import logging
 from elasticsearch8 import Elasticsearch
 from .base import Waiter
 
 # pylint: disable=missing-docstring,too-many-arguments
 
+
 class Exists(Waiter):
     """Class Definition"""
-    ACTIONS: t.Optional[str] = None
+
     IDX_OR_DS = ['index', 'datastream', 'idx', 'ds']
     TEMPLATE = ['index_template', 'template', 'tmpl']
     COMPONENT = ['component_template', 'component', 'comp']
+
     def __init__(
-            self,
-            client: Elasticsearch,
-            action: t.Optional[str] = None,
-            pause: float = 1.5,
-            timeout: float = 15,
-            name: str = None,
-            kind: str = None
-        ) -> None:
+        self,
+        client: Elasticsearch,
+        action: str = '',
+        pause: float = 1.5,
+        timeout: float = 15,
+        name: str = '',
+        kind: str = '',
+    ) -> None:
         super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Exists')
         self.name = name
         self.kind = kind
         self.empty_check('name')
         self.empty_check('kind')
         self.checkid = f'check for {self.kindmap} {name} to exist'
 
     @property
     def check(self) -> bool:
         """
         Check if the named entity exists, based on kind
         """
         doit = {
-            'index or datastream': self.client.indices.exists(index=self.name),
-            'index template': self.client.indices.exists_index_template(name=self.name),
-            'component template': self.client.cluster.exists_component_template(name=self.name),
-            'FAIL': False
+            'index or datastream': {
+                'func': self.client.indices.exists,
+                'kwargs': {'index': self.name},
+            },
+            'index template': {
+                'func': self.client.indices.exists_index_template,
+                'kwargs': {'name': self.name},
+            },
+            'component template': {
+                'func': self.client.cluster.exists_component_template,
+                'kwargs': {'name': self.name},
+            },
+            'FAIL': {'func': False, 'kwargs': {}},
         }
-        return doit[self.kindmap]
+        return bool(doit[self.kindmap]['func'](**doit[self.kindmap]['kwargs']))
 
     @property
-    def kindmap(self) -> t.Literal[
-            'index or datastream', 'index template', 'component template', 'FAIL']:
+    def kindmap(
+        self,
+    ) -> t.Literal[
+        'index or datastream', 'index template', 'component template', 'FAIL'
+    ]:
         """This is a little way to ensure many possibilities come down to one"""
         if self.kind in self.IDX_OR_DS:
             return 'index or datastream'
         if self.kind in self.TEMPLATE:
             return 'index template'
         if self.kind in self.COMPONENT:
             return 'component template'
         self.logger.error('%s is not an acceptable value for kind', self.kind)
-        return 'FAIL' # We should not see this, like, ever
+        return 'FAIL'  # We should not see this, like, ever
```

### Comparing `es_wait-0.3.3/src/es_wait/health.py` & `es_wait-0.3.5/src/es_wait/health.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """Health Check"""
+
 import typing as t
 import logging
 from elasticsearch8 import Elasticsearch
 from .base import Waiter
 
 # pylint: disable=missing-docstring,too-many-arguments
 
+
 class Health(Waiter):
     ACTIONS = ['allocation', 'cluster_routing', 'mount', 'replicas', 'shrink']
     RELO_ACTIONS = ['allocation', 'cluster_routing']
     STATUS_ACTIONS = ['mount', 'replicas', 'shrink']
     RELO_ARGS = {'relocating_shards': 0}
     STATUS_ARGS = {'status': 'green'}
+
     def __init__(
-            self,
-            client: Elasticsearch,
-            action: t.Literal[
-                'allocation', 'cluster_routing', 'mount', 'replicas', 'shrink'] = None,
-            pause: float = 1.5,
-            timeout: float = 15,
-            ) -> None:
+        self,
+        client: Elasticsearch,
+        action: t.Literal[
+            'allocation', 'cluster_routing', 'mount', 'replicas', 'shrink'
+        ] = None,
+        pause: float = 1.5,
+        timeout: float = 15,
+    ) -> None:
         super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Health')
         self.empty_check('action')
         self.checkid = self.getcheckid
 
     @property
     def argmap(self) -> t.Union[t.Dict[str, int], t.Dict[str, str]]:
@@ -35,34 +39,41 @@
         msg = f'{self.action} is not an acceptable value for action'
         self.logger.error(msg)
         raise ValueError(msg)
 
     @property
     def check(self) -> bool:
         """
-        This function calls `client.cluster.` :py:meth:`~.elasticsearch.client.ClusterClient.health`
-        and, based on the contents of self.argmap, will return ``True`` or ``False`` depending on
-        whether that particular keyword appears in the output, and has the expected value.
+        This function calls `client.cluster.`
+        :py:meth:`~.elasticsearch.client.ClusterClient.health` and, based on the
+        contents of self.argmap, will return ``True`` or ``False`` depending on whether
+        that particular keyword appears in the output, and has the expected value.
 
         If multiple keys are provided, all must match for a ``True`` response.
         """
         output = self.client.cluster.health()
         check = True
         args = self.argmap
         for key, value in args.items():
             # First, verify that the key is in output
-            if not key in output:
+            if key not in output:
                 raise KeyError(f'Key "{key}" not in cluster health output')
-            # Verify that the output matches the expected value 
-            if not output[key] == value:
-                msg = f'NO MATCH: Value for key "{value}", health check output: {output[key]}'
+            # Verify that the output matches the expected value
+            if output[key] != value:
+                msg = (
+                    f'NO MATCH: Value for key "{value}", health check output: '
+                    f'{output[key]}'
+                )
                 self.logger.debug(msg)
-                check = False # We do not match
+                check = False  # We do not match
             else:
-                msg = f'MATCH: Value for key "{value}", health check output: {output[key]}'
+                msg = (
+                    f'MATCH: Value for key "{value}", health check output: '
+                    f'{output[key]}'
+                )
                 self.logger.debug(msg)
         if check:
             self.logger.debug('Health check for action %s passed.', self.action)
         return check
 
     @property
     def getcheckid(self) -> t.AnyStr:
```

### Comparing `es_wait-0.3.3/src/es_wait/relocate.py` & `es_wait-0.3.5/src/es_wait/relocate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 """Relocate Check"""
+
 import typing as t
 import logging
 from elasticsearch8 import Elasticsearch
 from .base import Waiter
 
 # pylint: disable=missing-docstring,too-many-arguments
 
+
 class Relocate(Waiter):
     ACTIONS: t.Optional[str] = None
+
     def __init__(
-            self,
-            client: Elasticsearch,
-            action: t.Optional[str] = None,
-            pause: float = 9,
-            timeout: float = -1,
-            name: str = None,
-        ) -> None:
+        self,
+        client: Elasticsearch,
+        action: t.Optional[str] = None,
+        pause: float = 9,
+        timeout: float = -1,
+        name: str = None,
+    ) -> None:
         super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Health')
         self.name = name
         self.empty_check('name')
         self.checkid = f'check for the {self.name} index relocation process to complete'
 
     @property
     def check(self) -> bool:
         """
-        This function calls `client.cluster.` :py:meth:`~.elasticsearch.client.ClusterClient.state`
-        with a given index to check if all of the shards for that index are in the ``STARTED``
-        state. It will return ``True`` if all primary and replica shards are in the ``STARTED``
-        state, and it will return ``False`` if any shard is in a different state.
+        This function calls `client.cluster.`
+        :py:meth:`~.elasticsearch.client.ClusterClient.state` with a given index to
+        check if all of the shards for that index are in the ``STARTED`` state. It will
+        return ``True`` if all primary and replica shards are in the ``STARTED`` state,
+        and it will return ``False`` if any shard is in a different state.
         """
         finished = self.finished_state
         if finished:
             self.logger.debug('Relocate Check for index: "%s" has passed.', self.name)
         return finished
 
     @property
     def finished_state(self) -> bool:
-        return (
-            all(
-                all(shard['state'] == "STARTED" for shard in shards)
-                for shards in self.routing_table.values()
-            )
+        return all(
+            all(shard['state'] == "STARTED" for shard in shards)
+            for shards in self.routing_table.values()
         )
 
     @property
     def routing_table(self) -> t.Dict:
         msg = f'Unable to get routing table data from cluster state for {self.name}'
         try:
             result = self.client.cluster.state(index=self.name)
```

### Comparing `es_wait-0.3.3/src/es_wait/restore.py` & `es_wait-0.3.5/src/es_wait/restore.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,71 @@
 """Snapshot Restore Check"""
+
 import typing as t
 import logging
 from elasticsearch8 import Elasticsearch
 from .base import Waiter
 
 # pylint: disable=missing-docstring,too-many-arguments
 
+
 class Restore(Waiter):
     ACTIONS: t.Optional[str] = None
+
     def __init__(
-            self,
-            client: Elasticsearch,
-            action: t.Optional[str] = None,
-            pause: float = 9,
-            timeout: float = -1,
-            index_list: t.Sequence[str] = None,
-        ) -> None:
+        self,
+        client: Elasticsearch,
+        action: t.Optional[str] = None,
+        pause: float = 9,
+        timeout: float = -1,
+        index_list: t.Sequence[str] = None,
+    ) -> None:
         super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Snapshot')
         self.index_list = index_list
         self.empty_check('index_list')
         self.checkid = 'check for completion of index_list restoration from snapshot'
 
     @property
     def check(self) -> bool:
         """
-        Calls `client.indices.` :py:meth:`~.elasticsearch.client.IndicesClient.recovery`
-        with a list of indices to check for complete recovery.  It will return ``True`` if recovery
-        of those indices is complete, and ``False`` otherwise.  It is designed to fail fast: if a
-        single shard is encountered that is still recovering (not in ``DONE`` stage), it will
-        immediately return ``False``, rather than complete iterating over the rest of the response.
+        Calls `client.indices.`
+        :py:meth:`~.elasticsearch.client.IndicesClient.recovery` with a list of indices
+        to check for complete recovery.  It will return ``True`` if recovery of those
+        indices is complete, and ``False`` otherwise.  It is designed to fail fast: if
+        a single shard is encountered that is still recovering (not in ``DONE`` stage),
+        it will immediately return ``False``, rather than complete iterating over the
+        rest of the response.
         """
         response = {}
         for chunk in self.index_list_chunks:
             chunk_response = self.get_recovery(chunk)
             if chunk_response == {}:
-                self.logger.debug('_recovery API returned an empty response. Trying again.')
+                self.logger.debug(
+                    '_recovery API returned an empty response. Trying again.'
+                )
                 return False
             response.update(chunk_response)
         self.logger.debug('Provided indices: %s', self.index_list)
         self.logger.debug('Found indices: %s', list(response.keys()))
-        for index,data in response.items():
+        for index, data in response.items():
             for shard in data['shards']:
                 stage = shard['stage']
                 if stage != 'DONE':
                     print(f'Index {index} is still in stage {stage}')
 
         # If we've gotten here, all of the indices have recovered
         return True
 
     @property
     def index_list_chunks(self) -> t.Sequence[t.Sequence[t.AnyStr]]:
         """
         This utility chunks very large index lists into 3KB chunks.
-        It measures the size as a csv string, then converts back into a list for the return value.
+        It measures the size as a csv string, then converts back into a list for the
+        return value.
         """
         chunks = []
         chunk = ""
         for index in self.index_list:
             if len(chunk) < 3072:
                 if not chunk:
                     chunk = index
@@ -69,10 +77,13 @@
         chunks.append(chunk.split(','))
         return chunks
 
     def get_recovery(self, chunk: t.Sequence[str]) -> t.Dict:
         try:
             chunk_response = self.client.indices.recovery(index=chunk, human=True)
         except Exception as err:
-            msg = f'Unable to obtain recovery information for specified indices. Error: {err}'
+            msg = (
+                f'Unable to obtain recovery information for specified indices. Error: '
+                f'{err}'
+            )
             raise ValueError(msg) from err
         return chunk_response
```

### Comparing `es_wait-0.3.3/src/es_wait/snapshot.py` & `es_wait-0.3.5/src/es_wait/snapshot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,76 @@
 """Snapshot Check"""
+
 import typing as t
 import logging
 from elasticsearch8 import Elasticsearch
 from .base import Waiter
 
 # pylint: disable=missing-docstring,too-many-arguments
 
+
 class Snapshot(Waiter):
     ACTIONS: t.Optional[str] = None
+
     def __init__(
-            self,
-            client: Elasticsearch,
-            action: t.Optional[str] = None,
-            pause: float = 9,
-            timeout: float = -1,
-            snapshot: str = None,
-            repository: str = None,
-        ) -> None:
+        self,
+        client: Elasticsearch,
+        action: t.Optional[str] = None,
+        pause: float = 9,
+        timeout: float = -1,
+        snapshot: str = None,
+        repository: str = None,
+    ) -> None:
         super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Snapshot')
         self.snapshot = snapshot
         self.repository = repository
         self.empty_check('snapshot')
         self.empty_check('repository')
         self.checkid = f'check for snapshot {self.snapshot} completion'
 
     @property
     def check(self) -> bool:
         """
-        This function calls `client.snapshot.` :py:meth:`~.elasticsearch.client.SnapshotClient.get`
-        and tests to see whether the snapshot is complete, and if so, with what status.  It will log
-        errors according to the result. If the snapshot is still ``IN_PROGRESS``, it will return
-        ``False``. ``SUCCESS`` will be an ``INFO`` level message, ``PARTIAL`` nets a ``WARNING``
-        message, ``FAILED`` is an ``ERROR``, message, and all others will be a ``WARNING`` level
-        message.
+        This function calls `client.snapshot.`
+        :py:meth:`~.elasticsearch.client.SnapshotClient.get` and tests to see whether
+        the snapshot is complete, and if so, with what status. It will log errors
+        according to the result. If the snapshot is still ``IN_PROGRESS``, it will
+        return ``False``. ``SUCCESS`` will be an ``INFO`` level message, ``PARTIAL``
+        nets a ``WARNING`` message, ``FAILED`` is an ``ERROR``, message, and all others
+        will be a ``WARNING`` level message.
         """
         state = self.snapstate['snapshots'][0]['state']
         retval = True
         if state == 'IN_PROGRESS':
             retval = False
         if retval:
             self.log_completion(state)
         return retval
 
     @property
     def snapstate(self) -> t.Dict:
         result = {}
         try:
-            result = self.client.snapshot.get(repository=self.repository, snapshot=self.snapshot)
+            result = self.client.snapshot.get(
+                repository=self.repository, snapshot=self.snapshot
+            )
         except Exception as err:
             raise ValueError(
-                f'Unable to obtain information for snapshot "{self.snapshot}" in repository '
-                f'"{self.repository}". Error: {err}'
+                f'Unable to obtain information for snapshot "{self.snapshot}" in '
+                f'repository "{self.repository}". Error: {err}'
             ) from err
         return result
 
     def log_completion(self, state: str) -> None:
         if state == 'SUCCESS':
             self.logger.info('Snapshot %s successfully completed.', self.snapshot)
         elif state == 'PARTIAL':
-            self.logger.warning('Snapshot %s completed with state PARTIAL.', self.snapshot)
+            self.logger.warning(
+                'Snapshot %s completed with state PARTIAL.', self.snapshot
+            )
         elif state == 'FAILED':
             self.logger.error('Snapshot %s completed with state FAILED.', self.snapshot)
         else:
-            self.logger.warning('Snapshot %s completed with state: %s', self.snapshot, state)
+            self.logger.warning(
+                'Snapshot %s completed with state: %s', self.snapshot, state
+            )
```

### Comparing `es_wait-0.3.3/src/es_wait/task.py` & `es_wait-0.3.5/src/es_wait/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,90 @@
 """Task Check"""
+
 import typing as t
 import logging
 from time import localtime, strftime
 from elasticsearch8 import Elasticsearch
 from .base import Waiter
 from .args import TaskArgs
 
 # pylint: disable=missing-docstring,too-many-arguments
 
+
 class Task(Waiter):
     ACTIONS = ['forcemerge', 'reindex', 'update_by_query']
+
     def __init__(
-            self,
-            client: Elasticsearch,
-            action: t.Literal['forcemerge', 'reindex', 'update_by_query'] = None,
-            pause: float = 9,
-            timeout: float = -1,
-            task_id: str = None,
-        ) -> None:
+        self,
+        client: Elasticsearch,
+        action: t.Literal['forcemerge', 'reindex', 'update_by_query'] = None,
+        pause: float = 9,
+        timeout: float = -1,
+        task_id: str = None,
+    ) -> None:
         super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Health')
         self.task_id = task_id
         self.empty_check(task_id)
         self.task_data = None
         self.task = None
         self.checkid = f'check for the {self.action} task to complete'
 
     @property
     def check(self) -> bool:
         """
-        This function calls `client.tasks.` :py:meth:`~.elasticsearch.client.TasksClient.get` with
-        the provided ``task_id``.  If the task data contains ``'completed': True``, then it will
-        return ``True``. If the task is not completed, it will log some information about the task
-        and return ``False``
+        This function calls `client.tasks.`
+        :py:meth:`~.elasticsearch.client.TasksClient.get` with the provided
+        ``task_id``.  If the task data contains ``'completed': True``, then it will
+        return ``True``. If the task is not completed, it will log some information
+        about the task and return ``False``
         """
         try:
-            self.task_data = TaskArgs(settings=self.client.tasks.get(task_id=self.task_id))
+            self.task_data = TaskArgs(
+                settings=self.client.tasks.get(task_id=self.task_id)
+            )
         except Exception as err:
-            msg = f'Unable to obtain task information for task_id "{self.task_id}". Exception {err}'
+            msg = (
+                f'Unable to obtain task information for task_id "{self.task_id}". '
+                f'Exception {err}'
+            )
             raise ValueError(msg) from err
         self.task = TaskArgs(settings=self.task_data.task)
         self.reindex_check()
         return self.task_complete
 
     def reindex_check(self) -> None:
         if self.task.action == 'indices:data/write/reindex':
             self.logger.debug("It's a REINDEX task")
             self.logger.debug('TASK_DATA: %s', self.task_data.asdict)
             self.logger.debug('TASK_DATA keys: %s', list(self.task_data.asdict.keys()))
             if self.task_data.response:
                 if 'failures' in self.task_data.response:
                     msg = (
-                        f'Failures found in reindex response: {self.task_data.response["failures"]}'
+                        f'Failures found in reindex response: '
+                        f'{self.task_data.response["failures"]}'
                     )
                     raise ValueError(msg)
 
     @property
     def task_complete(self) -> bool:
         running_time = 0.000000001 * self.task.running_time_in_nanos
         self.logger.debug('Running time: %s seconds', running_time)
         if self.task_data.completed:
             completion_time = (running_time * 1000) + self.task['start_time_in_millis']
-            time_string = strftime('%Y-%m-%dT%H:%M:%S', localtime(completion_time/1000))
-            self.logger.debug('Task "%s" completed at %s.', self.task.description, time_string)
+            time_string = strftime(
+                '%Y-%m-%dT%H:%M:%S', localtime(completion_time / 1000)
+            )
+            self.logger.debug(
+                'Task "%s" completed at %s.', self.task.description, time_string
+            )
             retval = True
         else:
             # Log the task status here.
             self.logger.debug('Full Task Data: %s', self.task_data.asdict)
             msg = (
-                f'Task "{self.task.description}" with task_id "{self.task_id}" has been running '
-                f'for {running_time} seconds'
+                f'Task "{self.task.description}" with task_id "{self.task_id}" has '
+                f'been running for {running_time} seconds'
             )
             self.logger.debug(msg)
             retval = False
         return retval
```

### Comparing `es_wait-0.3.3/.gitignore` & `es_wait-0.3.5/.gitignore`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
 
+.flake8
+.black
+pylintrc
+pylintrc.toml
+
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
@@ -136,14 +141,15 @@
 .ropeproject
 
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
+mypy.ini
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
 # pytype static type analyzer
@@ -154,7 +160,9 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+.vscode
```

### Comparing `es_wait-0.3.3/LICENSE` & `es_wait-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `es_wait-0.3.3/pyproject.toml` & `es_wait-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -97,17 +97,18 @@
 ]
 all = [
   "style",
   "typing",
 ]
 
 [tool.black]
-target-version = ["py38"]
-line-length = 120
+target-version = ['py38']
+line-length = 88
 skip-string-normalization = true
+include = '\.pyi?$'
 
 [tool.ruff]
 target-version = "py38"
 line-length = 120
 select = [
   "A",
   "ARG",
@@ -194,8 +195,8 @@
     "requests",
     "pytest >=7.2.1",
     "pytest-cov",
 ]
 
 [publish.index.repos.main]
 url = "https://upload.pypi.org/legacy/"
-username = "__token__"
+username = "__token__"
```

### Comparing `es_wait-0.3.3/PKG-INFO` & `es_wait-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: es-wait
-Version: 0.3.3
+Version: 0.3.5
 Summary: Helping you wait for certain Elasticsearch tasks and API calls to finish
 Project-URL: Documentation, https://github.com/untergeek/es-wait#readme
 Project-URL: Issues, https://github.com/untergeek/es-wait/issues
 Project-URL: Source, https://github.com/untergeek/es-wait
 Author-email: Aaron Mildenstein <untergeek@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
```

