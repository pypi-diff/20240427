# Comparing `tmp/timeframe_event-1.1.7.tar.gz` & `tmp/timeframe_event-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeframe_event-1.1.7.tar", max compression
+gzip compressed data, was "timeframe_event-1.1.8.tar", max compression
```

## Comparing `timeframe_event-1.1.7.tar` & `timeframe_event-1.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35823 2024-02-12 13:05:15.147757 timeframe_event-1.1.7/LICENSE
--rw-r--r--   0        0        0     1396 2024-04-23 17:30:20.550686 timeframe_event-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     5473 2024-02-20 17:52:52.885986 timeframe_event-1.1.7/README.md
--rw-r--r--   0        0        0      321 2024-02-19 17:04:05.858099 timeframe_event-1.1.7/timeframe/__init__.py
--rw-r--r--   0        0        0    18002 2024-04-23 17:29:15.758818 timeframe_event-1.1.7/timeframe/timeframe.py
--rw-r--r--   0        0        0     6320 1970-01-01 00:00:00.000000 timeframe_event-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35823 2024-02-12 13:05:15.147757 timeframe_event-1.1.8/LICENSE
+-rw-r--r--   0        0        0     1396 2024-04-27 18:34:13.231842 timeframe_event-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0     5473 2024-02-20 17:52:52.885986 timeframe_event-1.1.8/README.md
+-rw-r--r--   0        0        0      321 2024-02-19 17:04:05.858099 timeframe_event-1.1.8/timeframe/__init__.py
+-rw-r--r--   0        0        0    18951 2024-04-23 17:31:52.286673 timeframe_event-1.1.8/timeframe/timeframe.py
+-rw-r--r--   0        0        0     6320 1970-01-01 00:00:00.000000 timeframe_event-1.1.8/PKG-INFO
```

### Comparing `timeframe_event-1.1.7/LICENSE` & `timeframe_event-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `timeframe_event-1.1.7/pyproject.toml` & `timeframe_event-1.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build]
 package_dir = {""= "timeframe"}
 
 [project]
 description = "Python timeframe tool for time monitoring for each event, error handling, traceback recording..."
 name = "timeframe-event"
-version = "1.1.7"
+version = "1.1.8"
 authors = [
     {"name"="i-am-unknown", "email"="iamaunknownpeople@protonmail.com"}
 ]
 readme = 'README.md'
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -23,15 +23,15 @@
 [project.urls]
 Homepage = "https://github.com/i-am-unknown-81514525/timeframe/tree/main"
 Issues = "https://github.com/i-am-unknown-81514525/timeframe/issues"
 
 [tool.poetry]
 description = "Python timeframe tool for time monitoring for each event, error handling, traceback recording..."
 name = "timeframe-event"
-version = "1.1.7"
+version = "1.1.8"
 authors = ["i-am-unknown <iamaunknownpeople@protonmail.com>"]
 readme = 'README.md'
 repository = "https://github.com/i-am-unknown-81514525/timeframe/tree/main"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent"
```

### Comparing `timeframe_event-1.1.7/README.md` & `timeframe_event-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `timeframe_event-1.1.7/timeframe/timeframe.py` & `timeframe_event-1.1.8/timeframe/timeframe.py`

 * *Files 8% similar despite different names*

```diff
@@ -227,15 +227,15 @@
         except:
             result = False
         await self._main._trigger_async(info=InfoPack(frame=self, parent=self._parent, tb=(exc_type, exc_val, exc_tb)))
         return result
 
 
 class Action(BaseFrame):
-    def __init__(self, main: TimeFrame[A, K], parent: Event, name: Optional[str] = None, retry_limit: int = 3,
+    def __init__(self, main: TimeFrame[A, K], parent: Union[Event, TimeFrame], name: Optional[str] = None, retry_limit: int = 3,
                  ignore_retries: Optional[Sequence[Type[BaseException]]] = None, check_exc_subclass: bool = False):
         real_ignore_retries: Sequence[Type[BaseException]] = ignore_retries or ()
         self._ignore_retries = real_ignore_retries
         if len(self._ignore_retries) == 0 and check_exc_subclass:
             msg = f'''
 You cannot set `check_exc_subclass` as True when no Exception type is provided in parameter `ignore_retries`
 Parameter Conflict:
@@ -342,15 +342,15 @@
     if index == 3:
         return '> - '
     return ''
 
 
 class TimeFrame(BaseFrame, Generic[A, K]):
     def __init__(self, *args: A, name: Optional[str] = None, rt: Union[Callable[..., Any], None] = None, **kwargs: K):
-        self._frames: MutableSequence[Event] = []
+        self._frames: MutableSequence[Union[Event, Action]] = []
         self._tb: list[str] = []
         self._rt: tuple[Optional[Callable[..., Any]], tuple[A, ...], dict[str, K]] = (rt, args, kwargs)
         self._re: Any = None
         super().__init__(name=name)
 
     @property
     def _init_content(self) -> list[str]:
@@ -359,14 +359,28 @@
         return content
 
     def create(self, name: Optional[str] = None) -> Event:
         group = Event(main=self, parent=self, name=name)
         self._frames.append(group)
         return group
 
+    def create_action(self, name: Optional[str] = None, retry_limit: int = 0,
+               ignore_retries: Optional[Sequence[Type[BaseException]]] = None,
+               check_exc_subclass: bool = False, *, retries: int = 3) -> Action:
+        if retries and not retry_limit:
+            warn('Usage of `retries` argument should be change to `retry_limit`', DeprecationWarning)
+        if retries and retry_limit and retries != retry_limit:
+            raise ValueError(
+                f'You should not supply both `retry_limit` and `retries` arguments and give them different value (retry_limit={retry_limit}, retries={retries})')
+        event = Action(main=self, parent=self, name=name, retry_limit=retry_limit or retries,
+                       ignore_retries=ignore_retries,
+                       check_exc_subclass=check_exc_subclass)
+        self._frames.append(event)
+        return event
+
     def _check_recur(self, source: TimeFrame[A, K] | Event | Action | Attempt) -> TypeGuard[
         Union[TimeFrame[A, K] | Event | Action]]:
         """Return a boolean value on whether it should continue recurring or stop"""
         if isinstance(source, Attempt):
             return False
         if isinstance(source, Action) and len(source._frames) == 1 and source._frames[0].state == State.SUCCESS:
             return False
```

### Comparing `timeframe_event-1.1.7/PKG-INFO` & `timeframe_event-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeframe-event
-Version: 1.1.7
+Version: 1.1.8
 Summary: Python timeframe tool for time monitoring for each event, error handling, traceback recording...
 Home-page: https://github.com/i-am-unknown-81514525/timeframe/tree/main
 Author: i-am-unknown
 Author-email: iamaunknownpeople@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

