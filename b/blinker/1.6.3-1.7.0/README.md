# Comparing `tmp/blinker-1.6.3.tar.gz` & `tmp/blinker-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blinker-1.6.3.tar", last modified: Sat Oct  7 14:11:34 2023, max compression
+gzip compressed data, was "blinker-1.7.0.tar", last modified: Wed Nov  1 22:00:54 2023, max compression
```

## Comparing `blinker-1.6.3.tar` & `blinker-1.7.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     3166 2023-10-07 14:11:34.000000 blinker-1.6.3/CHANGES.rst
--rw-r--r--   0        0        0     1054 2023-10-07 14:11:34.000000 blinker-1.6.3/LICENSE.rst
--rw-r--r--   0        0        0      990 2023-10-07 14:11:34.000000 blinker-1.6.3/README.rst
--rw-r--r--   0        0        0      634 2023-10-07 14:11:34.000000 blinker-1.6.3/docs/Makefile
--rw-r--r--   0        0        0     3627 2023-10-07 14:11:34.000000 blinker-1.6.3/docs/_static/blinker-named.png
--rw-r--r--   0        0        0     1195 2023-10-07 14:11:34.000000 blinker-1.6.3/docs/conf.py
--rw-r--r--   0        0        0     9761 2023-10-07 14:11:34.000000 blinker-1.6.3/docs/index.rst
--rw-r--r--   0        0        0      765 2023-10-07 14:11:34.000000 blinker-1.6.3/docs/make.bat
--rw-r--r--   0        0        0     1806 2023-10-07 14:11:34.000000 blinker-1.6.3/pyproject.toml
--rw-r--r--   0        0        0       33 2023-10-07 14:11:34.000000 blinker-1.6.3/requirements/dev.in
--rw-r--r--   0        0        0     1242 2023-10-07 14:11:34.000000 blinker-1.6.3/requirements/dev.txt
--rw-r--r--   0        0        0       43 2023-10-07 14:11:34.000000 blinker-1.6.3/requirements/docs.in
--rw-r--r--   0        0        0     1142 2023-10-07 14:11:34.000000 blinker-1.6.3/requirements/docs.txt
--rw-r--r--   0        0        0       22 2023-10-07 14:11:34.000000 blinker-1.6.3/requirements/tests.in
--rw-r--r--   0        0        0      381 2023-10-07 14:11:34.000000 blinker-1.6.3/requirements/tests.txt
--rw-r--r--   0        0        0        5 2023-10-07 14:11:34.000000 blinker-1.6.3/requirements/typing.in
--rw-r--r--   0        0        0      271 2023-10-07 14:11:34.000000 blinker-1.6.3/requirements/typing.txt
--rw-r--r--   0        0        0      408 2023-10-07 14:11:34.000000 blinker-1.6.3/src/blinker/__init__.py
--rw-r--r--   0        0        0     9096 2023-10-07 14:11:34.000000 blinker-1.6.3/src/blinker/_saferef.py
--rw-r--r--   0        0        0     4110 2023-10-07 14:11:34.000000 blinker-1.6.3/src/blinker/_utilities.py
--rw-r--r--   0        0        0    20293 2023-10-07 14:11:34.000000 blinker-1.6.3/src/blinker/base.py
--rw-r--r--   0        0        0        0 2023-10-07 14:11:34.000000 blinker-1.6.3/src/blinker/py.typed
--rw-r--r--   0        0        0     1135 2023-10-07 14:11:34.000000 blinker-1.6.3/tests/test_context.py
--rw-r--r--   0        0        0     3746 2023-10-07 14:11:34.000000 blinker-1.6.3/tests/test_saferef.py
--rw-r--r--   0        0        0    12962 2023-10-07 14:11:34.000000 blinker-1.6.3/tests/test_signals.py
--rw-r--r--   0        0        0      451 2023-10-07 14:11:34.000000 blinker-1.6.3/tests/test_utilities.py
--rw-r--r--   0        0        0      559 2023-10-07 14:11:34.000000 blinker-1.6.3/tox.ini
--rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 blinker-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0     3538 2023-11-01 22:00:54.000000 blinker-1.7.0/CHANGES.rst
+-rw-r--r--   0        0        0     1054 2023-11-01 22:00:54.000000 blinker-1.7.0/LICENSE.rst
+-rw-r--r--   0        0        0      990 2023-11-01 22:00:54.000000 blinker-1.7.0/README.rst
+-rw-r--r--   0        0        0      634 2023-11-01 22:00:54.000000 blinker-1.7.0/docs/Makefile
+-rw-r--r--   0        0        0     3627 2023-11-01 22:00:54.000000 blinker-1.7.0/docs/_static/blinker-named.png
+-rw-r--r--   0        0        0     1195 2023-11-01 22:00:54.000000 blinker-1.7.0/docs/conf.py
+-rw-r--r--   0        0        0    10257 2023-11-01 22:00:54.000000 blinker-1.7.0/docs/index.rst
+-rw-r--r--   0        0        0      765 2023-11-01 22:00:54.000000 blinker-1.7.0/docs/make.bat
+-rw-r--r--   0        0        0     1806 2023-11-01 22:00:54.000000 blinker-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-11-01 22:00:54.000000 blinker-1.7.0/requirements/dev.in
+-rw-r--r--   0        0        0     1244 2023-11-01 22:00:54.000000 blinker-1.7.0/requirements/dev.txt
+-rw-r--r--   0        0        0       43 2023-11-01 22:00:54.000000 blinker-1.7.0/requirements/docs.in
+-rw-r--r--   0        0        0     1432 2023-11-01 22:00:54.000000 blinker-1.7.0/requirements/docs.txt
+-rw-r--r--   0        0        0       22 2023-11-01 22:00:54.000000 blinker-1.7.0/requirements/tests.in
+-rw-r--r--   0        0        0      381 2023-11-01 22:00:54.000000 blinker-1.7.0/requirements/tests.txt
+-rw-r--r--   0        0        0        5 2023-11-01 22:00:54.000000 blinker-1.7.0/requirements/typing.in
+-rw-r--r--   0        0        0      271 2023-11-01 22:00:54.000000 blinker-1.7.0/requirements/typing.txt
+-rw-r--r--   0        0        0      408 2023-11-01 22:00:54.000000 blinker-1.7.0/src/blinker/__init__.py
+-rw-r--r--   0        0        0     9096 2023-11-01 22:00:54.000000 blinker-1.7.0/src/blinker/_saferef.py
+-rw-r--r--   0        0        0     2856 2023-11-01 22:00:54.000000 blinker-1.7.0/src/blinker/_utilities.py
+-rw-r--r--   0        0        0    20544 2023-11-01 22:00:54.000000 blinker-1.7.0/src/blinker/base.py
+-rw-r--r--   0        0        0        0 2023-11-01 22:00:54.000000 blinker-1.7.0/src/blinker/py.typed
+-rw-r--r--   0        0        0     1149 2023-11-01 22:00:54.000000 blinker-1.7.0/tests/test_context.py
+-rw-r--r--   0        0        0     3746 2023-11-01 22:00:54.000000 blinker-1.7.0/tests/test_saferef.py
+-rw-r--r--   0        0        0    12962 2023-11-01 22:00:54.000000 blinker-1.7.0/tests/test_signals.py
+-rw-r--r--   0        0        0      451 2023-11-01 22:00:54.000000 blinker-1.7.0/tests/test_utilities.py
+-rw-r--r--   0        0        0      557 2023-11-01 22:00:54.000000 blinker-1.7.0/tox.ini
+-rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 blinker-1.7.0/PKG-INFO
```

### Comparing `blinker-1.6.3/CHANGES.rst` & `blinker-1.7.0/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Version 1.7.0
+-------------
+
+Released 2023-11-01
+
+-   Fixed messages printed to standard error about unraisable exceptions during
+    signal cleanup, typically during interpreter shutdown. :pr:`123`
+-   Allow the Signal set_class to be customised, to allow calling of receivers
+    in registration order. :pr:`116`.
+-   Drop Python 3.7 and support Python 3.12. :pr:`126`
+
 Version 1.6.3
 -------------
 
 Released 2023-09-23
 
 -   Fix `SyncWrapperType` and `AsyncWrapperType` :pr:`108`
 -   Fixed issue where ``signal.connected_to`` would not disconnect the
```

### Comparing `blinker-1.6.3/LICENSE.rst` & `blinker-1.7.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `blinker-1.6.3/README.rst` & `blinker-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `blinker-1.6.3/docs/Makefile` & `blinker-1.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `blinker-1.6.3/docs/_static/blinker-named.png` & `blinker-1.7.0/docs/_static/blinker-named.png`

 * *Files identical despite different names*

### Comparing `blinker-1.6.3/docs/conf.py` & `blinker-1.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blinker-1.6.3/docs/index.rst` & `blinker-1.7.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  - permanently or temporarily connected receivers
  - automatically disconnected receivers via weak referencing
  - sending arbitrary data payloads
  - collecting return values from signal receivers
  - thread safety
 
 Blinker was written by Jason Kirtand and is provided under the MIT
-License. The library supports Python 3.7 or later; or PyPy3.9 or later.
+License. The library supports Python 3.8 or later; or PyPy3.9 or later.
 
 
 Decoupling With Named Signals
 -----------------------------
 
 Named signals are created with :func:`signal`:
 
@@ -331,14 +331,32 @@
            asyncio.run(func(*args, **kwargs))
 
        return inner
 
    await sig.send(_async_wrapper=wrapper)
 
 
+Call receivers in order of registration
+---------------------------------------
+
+It can be advantageous to call a signal's receivers in the order they
+were registered. To achieve this the storage class for receivers should
+be changed from an (unordered) set to an ordered set,
+
+.. code-block:: python
+
+    from blinker import Signal
+    from ordered_set import OrderedSet
+
+    Signal.set_class = OrderedSet
+
+Please note that ``ordered_set`` is a PyPI package and is not
+installed with blinker.
+
+
 API Documentation
 -----------------
 
 All public API members can (and should) be imported from ``blinker``::
 
   from blinker import ANY, signal
```

### Comparing `blinker-1.6.3/docs/make.bat` & `blinker-1.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `blinker-1.6.3/pyproject.toml` & `blinker-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Software Development :: Libraries",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://blinker.readthedocs.io"
 Documentation = "https://blinker.readthedocs.io"
 "Source Code" = "https://github.com/pallets-eco/blinker/"
 "Issue Tracker" = "https://github.com/pallets-eco/blinker/issues/"
@@ -47,15 +47,15 @@
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 testpaths = ["tests"]
 filterwarnings = ["error"]
 
 [tool.mypy]
-python_version = "3.7"
+python_version = "3.8"
 files = ["src/blinker"]
 show_error_codes = true
 pretty = true
 #strict = true
 allow_redefinition = true
 disallow_subclassing_any = true
 #disallow_untyped_calls = true
```

### Comparing `blinker-1.6.3/requirements/dev.txt` & `blinker-1.7.0/requirements/dev.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 # SHA1:39179f2c476f94362aa0705be059a488d7e38b6d
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-build==0.10.0
+build==1.0.3
     # via pip-tools
-cachetools==5.3.1
+cachetools==5.3.2
     # via tox
-cfgv==3.3.1
+cfgv==3.4.0
     # via pre-commit
-chardet==5.1.0
+chardet==5.2.0
     # via tox
-click==8.1.3
+click==8.1.7
     # via
     #   pip-compile-multi
     #   pip-tools
 colorama==0.4.6
     # via tox
-distlib==0.3.6
+distlib==0.3.7
     # via virtualenv
-filelock==3.12.2
+filelock==3.13.1
     # via
     #   tox
     #   virtualenv
-identify==2.5.24
+identify==2.5.31
     # via pre-commit
 nodeenv==1.8.0
     # via pre-commit
-packaging==23.1
+packaging==23.2
     # via
     #   build
     #   pyproject-api
     #   tox
 pip-compile-multi==2.6.3
     # via -r requirements/dev.in
-pip-tools==6.13.0
+pip-tools==7.3.0
     # via pip-compile-multi
-platformdirs==3.8.0
+platformdirs==3.11.0
     # via
     #   tox
     #   virtualenv
-pluggy==1.2.0
+pluggy==1.3.0
     # via tox
-pre-commit==3.3.3
+pre-commit==3.5.0
     # via -r requirements/dev.in
-pyproject-api==1.5.2
+pyproject-api==1.6.1
     # via tox
 pyproject-hooks==1.0.0
     # via build
-pyyaml==6.0
+pyyaml==6.0.1
     # via pre-commit
 toposort==1.10
     # via pip-compile-multi
-tox==4.6.3
+tox==4.11.3
     # via -r requirements/dev.in
-virtualenv==20.23.1
+virtualenv==20.24.6
     # via
     #   pre-commit
     #   tox
-wheel==0.40.0
+wheel==0.41.3
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `blinker-1.6.3/requirements/docs.txt` & `blinker-1.7.0/requirements/docs.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,56 +3,64 @@
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 alabaster==0.7.13
     # via sphinx
-babel==2.12.1
+babel==2.13.1
     # via sphinx
 certifi==2023.7.22
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.3.2
     # via requests
 docutils==0.20.1
     # via sphinx
 idna==3.4
     # via requests
 imagesize==1.4.1
     # via sphinx
 jinja2==3.1.2
     # via sphinx
 markupsafe==2.1.3
     # via jinja2
-packaging==23.1
+packaging==23.2
     # via
     #   pallets-sphinx-themes
     #   sphinx
 pallets-sphinx-themes==2.1.1
-    # via -r docs.in
-pygments==2.15.1
+    # via -r requirements/docs.in
+pygments==2.16.1
     # via sphinx
 requests==2.31.0
     # via sphinx
 snowballstemmer==2.2.0
     # via sphinx
-sphinx==7.0.1
+sphinx==7.2.6
     # via
-    #   -r docs.in
+    #   -r requirements/docs.in
     #   pallets-sphinx-themes
     #   sphinx-issues
+    #   sphinxcontrib-applehelp
+    #   sphinxcontrib-devhelp
+    #   sphinxcontrib-htmlhelp
+    #   sphinxcontrib-qthelp
+    #   sphinxcontrib-serializinghtml
 sphinx-issues==3.0.1
-    # via -r docs.in
-sphinxcontrib-applehelp==1.0.4
+    # via -r requirements/docs.in
+sphinxcontrib-applehelp==1.0.7
     # via sphinx
-sphinxcontrib-devhelp==1.0.2
+sphinxcontrib-devhelp==1.0.5
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.1
+sphinxcontrib-htmlhelp==2.0.4
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.3
+sphinxcontrib-qthelp==1.0.6
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.5
+sphinxcontrib-serializinghtml==1.1.9
     # via sphinx
-urllib3==2.0.3
+urllib3==2.0.7
     # via requests
+
+# The following packages are considered to be unsafe in a requirements file:
+# setuptools
```

### Comparing `blinker-1.6.3/src/blinker/_saferef.py` & `blinker-1.7.0/src/blinker/_saferef.py`

 * *Files identical despite different names*

### Comparing `blinker-1.6.3/src/blinker/base.py` & `blinker-1.7.0/src/blinker/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 """
 from __future__ import annotations
 
 import typing as t
 from collections import defaultdict
 from contextlib import contextmanager
+from inspect import iscoroutinefunction
 from warnings import warn
 from weakref import WeakValueDictionary
 
 from blinker._utilities import annotatable_weakref
 from blinker._utilities import hashable_identity
 from blinker._utilities import IdentityType
-from blinker._utilities import is_coroutine_function
 from blinker._utilities import lazy_property
 from blinker._utilities import reference
 from blinker._utilities import symbol
 from blinker._utilities import WeakTypes
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
@@ -35,22 +35,28 @@
     AsyncWrapperType = t.Callable[[t.Callable[P, t.Awaitable[T]]], t.Callable[P, T]]
     SyncWrapperType = t.Callable[[t.Callable[P, T]], t.Callable[P, t.Awaitable[T]]]
 
 ANY = symbol("ANY")
 ANY.__doc__ = 'Token for "any sender".'
 ANY_ID = 0
 
+# NOTE: We need a reference to cast for use in weakref callbacks otherwise
+#       t.cast may have already been set to None during finalization.
+cast = t.cast
+
 
 class Signal:
     """A notification emitter."""
 
     #: An :obj:`ANY` convenience synonym, allows ``Signal.ANY``
     #: without an additional import.
     ANY = ANY
 
+    set_class: type[set] = set
+
     @lazy_property
     def receiver_connected(self) -> Signal:
         """Emitted after each :meth:`connect`.
 
         The signal sender is the signal instance, and the :meth:`connect`
         arguments are passed through: *receiver*, *sender*, and *weak*.
 
@@ -95,16 +101,20 @@
         #:
         #: The values of this mapping are not meaningful outside of the
         #: internal :class:`Signal` implementation, however the boolean value
         #: of the mapping is useful as an extremely efficient check to see if
         #: any receivers are connected to the signal.
         self.receivers: dict[IdentityType, t.Callable | annotatable_weakref] = {}
         self.is_muted = False
-        self._by_receiver: dict[IdentityType, set[IdentityType]] = defaultdict(set)
-        self._by_sender: dict[IdentityType, set[IdentityType]] = defaultdict(set)
+        self._by_receiver: dict[IdentityType, set[IdentityType]] = defaultdict(
+            self.set_class
+        )
+        self._by_sender: dict[IdentityType, set[IdentityType]] = defaultdict(
+            self.set_class
+        )
         self._weak_senders: dict[IdentityType, annotatable_weakref] = {}
 
     def connect(
         self, receiver: T_callable, sender: t.Any = ANY, weak: bool = True
     ) -> T_callable:
         """Connect *receiver* to signal events sent by *sender*.
 
@@ -286,15 +296,15 @@
         """
         if self.is_muted:
             return []
 
         sender = self._extract_sender(sender)
         results = []
         for receiver in self.receivers_for(sender):
-            if is_coroutine_function(receiver):
+            if iscoroutinefunction(receiver):
                 if _async_wrapper is None:
                     raise RuntimeError("Cannot send to a coroutine function")
                 receiver = _async_wrapper(receiver)
             result = receiver(sender, **kwargs)
             results.append((receiver, result))
         return results
 
@@ -318,15 +328,15 @@
         """
         if self.is_muted:
             return []
 
         sender = self._extract_sender(sender)
         results = []
         for receiver in self.receivers_for(sender):
-            if not is_coroutine_function(receiver):
+            if not iscoroutinefunction(receiver):
                 if _sync_wrapper is None:
                     raise RuntimeError("Cannot send to a non-coroutine function")
                 receiver = _sync_wrapper(receiver)
             result = await receiver(sender, **kwargs)
             results.append((receiver, result))
         return results
 
@@ -423,19 +433,19 @@
             self.receivers.pop(receiver_id, None)
         else:
             self._by_sender[sender_id].discard(receiver_id)
             self._by_receiver[receiver_id].discard(sender_id)
 
     def _cleanup_receiver(self, receiver_ref: annotatable_weakref) -> None:
         """Disconnect a receiver from all senders."""
-        self._disconnect(t.cast(IdentityType, receiver_ref.receiver_id), ANY_ID)
+        self._disconnect(cast(IdentityType, receiver_ref.receiver_id), ANY_ID)
 
     def _cleanup_sender(self, sender_ref: annotatable_weakref) -> None:
         """Disconnect all receivers from a sender."""
-        sender_id = t.cast(IdentityType, sender_ref.sender_id)
+        sender_id = cast(IdentityType, sender_ref.sender_id)
         assert sender_id != ANY_ID
         self._weak_senders.pop(sender_id, None)
         for receiver_id in self._by_sender.pop(sender_id, ()):
             self._by_receiver[receiver_id].discard(sender_id)
 
     def _cleanup_bookkeeping(self) -> None:
         """Prune unused sender/receiver bookkeeping. Not threadsafe.
@@ -498,15 +508,15 @@
         Signal.__init__(self, doc)
 
         #: The name of this signal.
         self.name = name
 
     def __repr__(self) -> str:
         base = Signal.__repr__(self)
-        return f"{base[:-1]}; {self.name!r}>"
+        return f"{base[:-1]}; {self.name!r}>"  # noqa: E702
 
 
 class Namespace(dict):
     """A mapping of signal names to signals."""
 
     def signal(self, name: str, doc: str | None = None) -> NamedSignal:
         """Return the :class:`NamedSignal` *name*, creating it if required.
```

### Comparing `blinker-1.6.3/tests/test_context.py` & `blinker-1.7.0/tests/test_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,27 +40,27 @@
     pass
 
 
 class BaseFailure(BaseException):
     pass
 
 
-@pytest.mark.parametrize('exc_type', [Failure, BaseFailure])
+@pytest.mark.parametrize("exc_type", [Failure, BaseFailure])
 def test_temp_connection_failure(exc_type):
     sig = Signal()
 
     canary = []
 
     def receiver(sender):
         canary.append(sender)
 
     class Failure(Exception):
         pass
 
-    with pytest.raises(exc_type):
+    with pytest.raises(exc_type):  # noqa: B908
         sig.send(1)
         with sig.connected_to(receiver):
             sig.send(2)
             raise exc_type
         sig.send(3)
 
     assert canary == [2]
```

### Comparing `blinker-1.6.3/tests/test_saferef.py` & `blinker-1.7.0/tests/test_saferef.py`

 * *Files identical despite different names*

### Comparing `blinker-1.6.3/tests/test_signals.py` & `blinker-1.7.0/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `blinker-1.6.3/tox.ini` & `blinker-1.7.0/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 envlist =
-    py3{12,11,10,9,8,7}
+    py3{12,11,10,9,8}
     pypy310
     docs
     style
     typing
 skip_missing_interpreters = true
 
 [testenv]
```

### Comparing `blinker-1.6.3/PKG-INFO` & `blinker-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: blinker
-Version: 1.6.3
+Version: 1.7.0
 Summary: Fast, simple object-to-object and broadcast signaling
 Keywords: signal,emit,events,broadcast
 Author-email: Jason Kirtland <jek@discorporate.us>
 Maintainer-email: Pallets Ecosystem <contact@palletsprojects.com>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries
```

