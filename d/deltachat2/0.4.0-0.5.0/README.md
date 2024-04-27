# Comparing `tmp/deltachat2-0.4.0.tar.gz` & `tmp/deltachat2-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltachat2-0.4.0.tar", last modified: Sat Apr  6 20:45:30 2024, max compression
+gzip compressed data, was "deltachat2-0.5.0.tar", last modified: Sat Apr 27 17:50:25 2024, max compression
```

## Comparing `deltachat2-0.4.0.tar` & `deltachat2-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:45:30.865841 deltachat2-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:45:30.861841 deltachat2-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:45:30.861841 deltachat2-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-06 20:45:19.000000 deltachat2-0.4.0/.github/workflows/python-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-06 20:45:19.000000 deltachat2-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-06 20:45:19.000000 deltachat2-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-06 20:45:30.865841 deltachat2-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-06 20:45:19.000000 deltachat2-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:45:30.865841 deltachat2-0.4.0/deltachat2/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-06 20:45:19.000000 deltachat2-0.4.0/deltachat2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-06 20:45:19.000000 deltachat2-0.4.0/deltachat2/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-06 20:45:19.000000 deltachat2-0.4.0/deltachat2/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-06 20:45:19.000000 deltachat2-0.4.0/deltachat2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-06 20:45:19.000000 deltachat2-0.4.0/deltachat2/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-06 20:45:19.000000 deltachat2-0.4.0/deltachat2/rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-06 20:45:19.000000 deltachat2-0.4.0/deltachat2/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-06 20:45:19.000000 deltachat2-0.4.0/deltachat2/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-06 20:45:19.000000 deltachat2-0.4.0/deltachat2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:45:30.865841 deltachat2-0.4.0/deltachat2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-06 20:45:30.000000 deltachat2-0.4.0/deltachat2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-06 20:45:30.000000 deltachat2-0.4.0/deltachat2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 20:45:30.000000 deltachat2-0.4.0/deltachat2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-06 20:45:30.000000 deltachat2-0.4.0/deltachat2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-06 20:45:30.000000 deltachat2-0.4.0/deltachat2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:45:30.865841 deltachat2-0.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-06 20:45:19.000000 deltachat2-0.4.0/examples/client.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1256 2024-04-06 20:45:19.000000 deltachat2-0.4.0/examples/echobot.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-06 20:45:19.000000 deltachat2-0.4.0/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-06 20:45:19.000000 deltachat2-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 20:45:30.865841 deltachat2-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:25.544716 deltachat2-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:25.536716 deltachat2-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:25.540716 deltachat2-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-27 17:50:13.000000 deltachat2-0.5.0/.github/workflows/python-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-27 17:50:13.000000 deltachat2-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-27 17:50:13.000000 deltachat2-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-27 17:50:25.544716 deltachat2-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-27 17:50:13.000000 deltachat2-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:25.540716 deltachat2-0.5.0/deltachat2/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-27 17:50:13.000000 deltachat2-0.5.0/deltachat2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-27 17:50:13.000000 deltachat2-0.5.0/deltachat2/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-27 17:50:13.000000 deltachat2-0.5.0/deltachat2/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-27 17:50:13.000000 deltachat2-0.5.0/deltachat2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-04-27 17:50:13.000000 deltachat2-0.5.0/deltachat2/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-27 17:50:13.000000 deltachat2-0.5.0/deltachat2/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-27 17:50:13.000000 deltachat2-0.5.0/deltachat2/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-27 17:50:13.000000 deltachat2-0.5.0/deltachat2/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-27 17:50:13.000000 deltachat2-0.5.0/deltachat2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:25.540716 deltachat2-0.5.0/deltachat2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-27 17:50:25.000000 deltachat2-0.5.0/deltachat2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-27 17:50:25.000000 deltachat2-0.5.0/deltachat2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:50:25.000000 deltachat2-0.5.0/deltachat2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-27 17:50:25.000000 deltachat2-0.5.0/deltachat2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 17:50:25.000000 deltachat2-0.5.0/deltachat2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:50:25.540716 deltachat2-0.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-27 17:50:13.000000 deltachat2-0.5.0/examples/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1256 2024-04-27 17:50:13.000000 deltachat2-0.5.0/examples/echobot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-27 17:50:13.000000 deltachat2-0.5.0/examples/echobot_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-27 17:50:13.000000 deltachat2-0.5.0/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-27 17:50:13.000000 deltachat2-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 17:50:25.544716 deltachat2-0.5.0/setup.cfg
```

### Comparing `deltachat2-0.4.0/.github/workflows/python-ci.yml` & `deltachat2-0.5.0/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `deltachat2-0.4.0/LICENSE` & `deltachat2-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deltachat2-0.4.0/PKG-INFO` & `deltachat2-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat2
-Version: 0.4.0
+Version: 0.5.0
 Summary: Client library for Delta Chat core JSON-RPC interface
 Author-email: adbenitez <adb@merlinux.eu>
 Keywords: deltachat
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `deltachat2-0.4.0/README.md` & `deltachat2-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `deltachat2-0.4.0/deltachat2/_utils.py` & `deltachat2-0.5.0/deltachat2/_utils.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.4.0/deltachat2/bot.py` & `deltachat2-0.5.0/deltachat2/bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def __init__(
         self,
         rpc: Rpc,
         hooks: Optional[Iterable[Tuple[HookCallback, Union[type, EventFilter]]]] = None,
         logger: Optional[logging.Logger] = None,
         command_prefix: str = "/",
     ) -> None:
-        """The keyword arguments will be passed to Client superclass constructor."""
+        """If hooks is an instance of HookCollection, also its post-hooks will be registered."""
         self.command_prefix = command_prefix
         logger = logger or logging.getLogger("deltachat2.Bot")
         super().__init__(rpc, hooks, logger)
 
     def configure(self, account_id: int, email: str, password: str, **kwargs) -> None:
         """Configure the account with the given account ID."""
         kwargs.setdefault("bot", "1")
```

### Comparing `deltachat2-0.4.0/deltachat2/client.py` & `deltachat2-0.5.0/deltachat2/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,69 @@
 """Event loop implementations offering high level event handling/hooking."""
 
 import logging
 from typing import Callable, Dict, Iterable, Optional, Set, Tuple, Type, Union
 
-from .events import EventFilter, HookCallback, RawEvent
+from .events import EventFilter, HookCallback, HookCollection, RawEvent
 from .rpc import Rpc
 from .types import CoreEvent, Event
 
+_HooksIndex = Dict[type, Set[Tuple[HookCallback, EventFilter]]]
+
 
 class Client:
     """Delta Chat client that listen to raw core events for multiple account."""
 
     def __init__(
         self,
         rpc: Rpc,
         hooks: Optional[Iterable[Tuple[HookCallback, Union[type, EventFilter]]]] = None,
         logger: Optional[logging.Logger] = None,
     ) -> None:
+        """If hooks is an instance of HookCollection, also its post-hooks will be registered."""
         self.rpc = rpc
         self.logger = logger or logging.getLogger("deltachat2.Client")
-        self._hooks: Dict[type, Set[Tuple[HookCallback, EventFilter]]] = {}
+        self._hooks: _HooksIndex = {}
+        self._post_hooks: _HooksIndex = {}
         self.add_hooks(hooks or [])
+        if isinstance(hooks, HookCollection):
+            self.add_post_hooks(hooks.post_hooks_iter())
 
     def add_hooks(self, hooks: Iterable[Tuple[HookCallback, Union[type, EventFilter]]]) -> None:
         """Register event hooks callbacks."""
         for hook, event in hooks:
             self.add_hook(hook, event)
 
+    def add_post_hooks(
+        self, hooks: Iterable[Tuple[HookCallback, Union[type, EventFilter]]]
+    ) -> None:
+        """Register event post-hooks callbacks."""
+        for hook, event in hooks:
+            self.add_post_hook(hook, event)
+
     def add_hook(self, hook: HookCallback, event: Union[type, EventFilter] = RawEvent) -> None:
-        """Register hook for the given event filter."""
+        """Register hook to be called when an event that matches the given filter is received."""
         event2 = event() if isinstance(event, type) else event
         self._hooks.setdefault(type(event2), set()).add((hook, event2))
 
     def remove_hook(self, hook: HookCallback, event: Union[type, EventFilter]) -> None:
         """Unregister hook from the given event filter."""
         event2 = event() if isinstance(event, type) else event
         self._hooks.get(type(event2), set()).remove((hook, event2))
 
+    def add_post_hook(self, hook: HookCallback, event: Union[type, EventFilter] = RawEvent) -> None:
+        """Register hook to be called after an event that matches the given filter is processed."""
+        event2 = event() if isinstance(event, type) else event
+        self._post_hooks.setdefault(type(event2), set()).add((hook, event2))
+
+    def remove_post_hook(self, hook: HookCallback, event: Union[type, EventFilter]) -> None:
+        """Unregister post-hook from the given event filter."""
+        event2 = event() if isinstance(event, type) else event
+        self._post_hooks.get(type(event2), set()).remove((hook, event2))
+
     def configure(self, account_id: int, email: str, password: str, **kwargs) -> None:
         """Configure the account with the given account ID."""
         self.rpc.set_config(account_id, "addr", email)
         self.rpc.set_config(account_id, "mail_pw", password)
         if kwargs:
             self.rpc.batch_set_config(account_id, kwargs)
         self.rpc.configure(account_id)
@@ -69,13 +92,17 @@
             raw_event = self.rpc.get_next_event()
             event = Event(raw_event.context_id, CoreEvent(raw_event.event))
             self._on_event(event, RawEvent)
             if func(event):
                 return event
 
     def _on_event(self, event: Event, filter_type: Type[EventFilter]) -> None:
-        for hook, evfilter in self._hooks.get(filter_type, []):
+        self._notify(self._hooks, event, filter_type)
+        self._notify(self._post_hooks, event, filter_type)
+
+    def _notify(self, hooks: _HooksIndex, event: Event, filter_type: Type[EventFilter]) -> None:
+        for hook, evfilter in hooks.get(filter_type, []):
             if evfilter.filter(event.event):
                 try:
                     hook(self, event.account_id, event.event)
                 except Exception as ex:
                     self.logger.exception(ex)
```

### Comparing `deltachat2-0.4.0/deltachat2/events.py` & `deltachat2-0.5.0/deltachat2/events.py`

 * *Files 6% similar despite different names*

```diff
@@ -178,29 +178,47 @@
         if self.pattern:
             match = self.pattern(event.msg.text)
             if not match:
                 return False
         return super()._call_func(event)
 
 
+_HookSet = Set[Tuple[HookCallback, Union[type, EventFilter]]]
+
+
 class HookCollection:
     """
-    Helper class to collect event hooks that can later be added to a Delta Chat client.
+    Helper class to collect event hooks and post-hooks
+    that can be later added to a Delta Chat client.
     """
 
     def __init__(self) -> None:
-        self._hooks: Set[Tuple[HookCallback, Union[type, EventFilter]]] = set()
+        self._hooks: _HookSet = set()
+        self._post_hooks: _HookSet = set()
 
     def __iter__(self) -> Iterator[Tuple[HookCallback, Union[type, EventFilter]]]:
         return iter(self._hooks)
 
-    def on(self, event: Union[type, EventFilter]) -> HookDecorator:  # noqa
-        """Register decorated function as listener for the given event."""
+    def post_hooks_iter(self) -> Iterator[Tuple[HookCallback, Union[type, EventFilter]]]:
+        """Iterator over the registered post-hooks"""
+        return iter(self._post_hooks)
+
+    def on(self, event: Union[type, EventFilter]) -> HookDecorator:
+        """Register decorated function to be called for events that match the given filter."""
+        return self._on(self._hooks, event)
+
+    def after(self, event: Union[type, EventFilter]) -> HookDecorator:
+        """Register decorated function to be called after an event that matches
+        the given filter is processed.
+        """
+        return self._on(self._post_hooks, event)
+
+    def _on(self, hooks: _HookSet, event: Union[type, EventFilter]) -> HookDecorator:
         if isinstance(event, type):
             event = event()
         assert isinstance(event, EventFilter), "Invalid event filter"
 
         def _decorator(func: HookCallback) -> HookCallback:
-            self._hooks.add((func, event))
+            hooks.add((func, event))
             return func
 
         return _decorator
```

### Comparing `deltachat2-0.4.0/deltachat2/rpc.py` & `deltachat2-0.5.0/deltachat2/rpc.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.4.0/deltachat2/transport.py` & `deltachat2-0.5.0/deltachat2/transport.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.4.0/deltachat2/types.py` & `deltachat2-0.5.0/deltachat2/types.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.4.0/deltachat2/util.py` & `deltachat2-0.5.0/deltachat2/util.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.4.0/deltachat2.egg-info/PKG-INFO` & `deltachat2-0.5.0/deltachat2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat2
-Version: 0.4.0
+Version: 0.5.0
 Summary: Client library for Delta Chat core JSON-RPC interface
 Author-email: adbenitez <adb@merlinux.eu>
 Keywords: deltachat
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `deltachat2-0.4.0/examples/client.py` & `deltachat2-0.5.0/examples/client.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.4.0/examples/echobot.py` & `deltachat2-0.5.0/examples/echobot.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.4.0/pyproject.toml` & `deltachat2-0.5.0/pyproject.toml`

 * *Files identical despite different names*

