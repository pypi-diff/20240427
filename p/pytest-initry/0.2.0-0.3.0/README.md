# Comparing `tmp/pytest_initry-0.2.0.tar.gz` & `tmp/pytest_initry-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_initry-0.2.0.tar", max compression
+gzip compressed data, was "pytest_initry-0.3.0.tar", max compression
```

## Comparing `pytest_initry-0.2.0.tar` & `pytest_initry-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1072 2024-04-09 17:28:57.000000 pytest_initry-0.2.0/LICENSE
--rw-r--r--   0        0        0      645 2024-04-09 17:28:34.000000 pytest_initry-0.2.0/README.md
--rw-r--r--   0        0        0      924 2024-04-14 12:17:05.000000 pytest_initry-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-08 19:27:30.000000 pytest_initry-0.2.0/pytest_initry/__init__.py
--rw-r--r--   0        0        0    11084 2024-04-14 15:05:50.000000 pytest_initry-0.2.0/pytest_initry/plugin.py
--rw-r--r--   0        0        0       85 2024-04-09 17:28:07.000000 pytest_initry-0.2.0/pytest_initry/protobufs/__init__.py
--rw-r--r--   0        0        0     1014 2024-04-14 14:30:38.374723 pytest_initry-0.2.0/pytest_initry/protobufs/responses_pb2.py
--rw-r--r--   0        0        0      391 2024-04-14 14:30:38.374723 pytest_initry-0.2.0/pytest_initry/protobufs/responses_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-14 14:30:38.374723 pytest_initry-0.2.0/pytest_initry/protobufs/responses_pb2_grpc.py
--rw-r--r--   0        0        0     2936 2024-04-14 14:30:38.454723 pytest_initry-0.2.0/pytest_initry/protobufs/test_pb2.py
--rw-r--r--   0        0        0     2858 2024-04-14 14:30:38.454723 pytest_initry-0.2.0/pytest_initry/protobufs/test_pb2.pyi
--rw-r--r--   0        0        0     6171 2024-04-14 14:30:38.454723 pytest_initry-0.2.0/pytest_initry/protobufs/test_pb2_grpc.py
--rw-r--r--   0        0        0     1885 2024-04-14 14:30:38.410723 pytest_initry-0.2.0/pytest_initry/protobufs/test_run_pb2.py
--rw-r--r--   0        0        0     1293 2024-04-14 14:30:38.410723 pytest_initry-0.2.0/pytest_initry/protobufs/test_run_pb2.pyi
--rw-r--r--   0        0        0     3998 2024-04-14 14:30:38.414723 pytest_initry-0.2.0/pytest_initry/protobufs/test_run_pb2_grpc.py
--rw-r--r--   0        0        0     1585 2024-04-14 14:30:38.490723 pytest_initry-0.2.0/pytest_initry/protobufs/tests_pb2.py
--rw-r--r--   0        0        0     1248 2024-04-14 14:30:38.490723 pytest_initry-0.2.0/pytest_initry/protobufs/tests_pb2.pyi
--rw-r--r--   0        0        0     2444 2024-04-14 14:30:38.490723 pytest_initry-0.2.0/pytest_initry/protobufs/tests_pb2_grpc.py
--rw-r--r--   0        0        0     1413 1970-01-01 00:00:00.000000 pytest_initry-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-15 05:59:57.071545 pytest_initry-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2536 2024-04-25 20:06:26.000000 pytest_initry-0.3.0/README.md
+-rw-r--r--   0        0        0      901 2024-04-25 13:05:19.000000 pytest_initry-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 05:59:57.071545 pytest_initry-0.3.0/pytest_initry/__init__.py
+-rw-r--r--   0        0        0    15176 2024-04-27 14:31:52.000000 pytest_initry-0.3.0/pytest_initry/plugin.py
+-rw-r--r--   0        0        0       85 2024-04-15 05:59:57.071545 pytest_initry-0.3.0/pytest_initry/protobufs/__init__.py
+-rw-r--r--   0        0        0     1014 2024-04-25 09:38:03.860906 pytest_initry-0.3.0/pytest_initry/protobufs/responses_pb2.py
+-rw-r--r--   0        0        0      391 2024-04-25 09:38:03.860906 pytest_initry-0.3.0/pytest_initry/protobufs/responses_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-25 09:38:03.860906 pytest_initry-0.3.0/pytest_initry/protobufs/responses_pb2_grpc.py
+-rw-r--r--   0        0        0     2936 2024-04-25 09:38:03.936906 pytest_initry-0.3.0/pytest_initry/protobufs/test_pb2.py
+-rw-r--r--   0        0        0     2858 2024-04-25 09:38:03.936906 pytest_initry-0.3.0/pytest_initry/protobufs/test_pb2.pyi
+-rw-r--r--   0        0        0     6171 2024-04-25 09:38:03.936906 pytest_initry-0.3.0/pytest_initry/protobufs/test_pb2_grpc.py
+-rw-r--r--   0        0        0     1885 2024-04-25 09:38:03.900906 pytest_initry-0.3.0/pytest_initry/protobufs/test_run_pb2.py
+-rw-r--r--   0        0        0     1293 2024-04-25 09:38:03.900906 pytest_initry-0.3.0/pytest_initry/protobufs/test_run_pb2.pyi
+-rw-r--r--   0        0        0     3998 2024-04-25 09:38:03.900906 pytest_initry-0.3.0/pytest_initry/protobufs/test_run_pb2_grpc.py
+-rw-r--r--   0        0        0     1635 2024-04-25 09:38:03.976906 pytest_initry-0.3.0/pytest_initry/protobufs/tests_pb2.py
+-rw-r--r--   0        0        0     1370 2024-04-25 09:38:03.976906 pytest_initry-0.3.0/pytest_initry/protobufs/tests_pb2.pyi
+-rw-r--r--   0        0        0     2444 2024-04-25 09:38:03.976906 pytest_initry-0.3.0/pytest_initry/protobufs/tests_pb2_grpc.py
+-rw-r--r--   0        0        0     3336 1970-01-01 00:00:00.000000 pytest_initry-0.3.0/PKG-INFO
```

### Comparing `pytest_initry-0.2.0/LICENSE` & `pytest_initry-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.2.0/pyproject.toml` & `pytest_initry-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-initry"
-version = "0.2.0"
+version = "0.3.0"
 description = "Plugin for sending automation test data from Pytest to the initry"
 authors = ["Andrejs Smirnovs <and.inbx@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Framework :: Pytest",
 ]
@@ -15,23 +15,22 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pytest = "^8.1.1"
 grpcio = "^1.62.1"
 protobuf = "^5.26.1"
+httpx = "0.27.0"
 
 
 [tool.poetry.plugins]
 pytest11 = { pytest-initry = "pytest_initry.plugin" }
 
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^8.1.1"
-pre-commit = "^3.7.0"
 ruff = "^0.3.5"
 
 
 [tool.ruff]
 target-version = "py311"
 line-length = 120
 exclude = [
```

### Comparing `pytest_initry-0.2.0/pytest_initry/protobufs/responses_pb2.py` & `pytest_initry-0.3.0/pytest_initry/protobufs/responses_pb2.py`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.2.0/pytest_initry/protobufs/test_pb2.py` & `pytest_initry-0.3.0/pytest_initry/protobufs/test_pb2.py`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.2.0/pytest_initry/protobufs/test_pb2.pyi` & `pytest_initry-0.3.0/pytest_initry/protobufs/test_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.2.0/pytest_initry/protobufs/test_pb2_grpc.py` & `pytest_initry-0.3.0/pytest_initry/protobufs/test_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.2.0/pytest_initry/protobufs/test_run_pb2.py` & `pytest_initry-0.3.0/pytest_initry/protobufs/test_run_pb2.py`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.2.0/pytest_initry/protobufs/test_run_pb2.pyi` & `pytest_initry-0.3.0/pytest_initry/protobufs/test_run_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.2.0/pytest_initry/protobufs/test_run_pb2_grpc.py` & `pytest_initry-0.3.0/pytest_initry/protobufs/test_run_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pytest_initry-0.2.0/pytest_initry/protobufs/tests_pb2.py` & `pytest_initry-0.3.0/pytest_initry/protobufs/tests_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 
 _sym_db = _symbol_database.Default()
 
 
 import responses_pb2 as responses__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0btests.proto\x1a\x0fresponses.proto\"b\n\x04Test\x12\x0e\n\x06nodeid\x18\x01 \x01(\t\x12\x10\n\x08location\x18\x02 \x01(\t\x12\x0c\n\x04uuid\x18\x03 \x01(\t\x12\x15\n\rtest_run_uuid\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\"*\n\x12\x43reateTestsRequest\x12\x14\n\x05tests\x18\x01 \x03(\x0b\x32\x05.Test2=\n\x0cTestsService\x12-\n\x0b\x43reateTests\x12\x13.CreateTestsRequest\x1a\t.StatusOkb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0btests.proto\x1a\x0fresponses.proto\"b\n\x04Test\x12\x0e\n\x06nodeid\x18\x01 \x01(\t\x12\x10\n\x08location\x18\x02 \x01(\t\x12\x0c\n\x04uuid\x18\x03 \x01(\t\x12\x15\n\rtest_run_uuid\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\"C\n\x12\x43reateTestsRequest\x12\x14\n\x05tests\x18\x01 \x03(\x0b\x32\x05.Test\x12\x17\n\x0fonly_tests_info\x18\x02 \x01(\x08\x32=\n\x0cTestsService\x12-\n\x0b\x43reateTests\x12\x13.CreateTestsRequest\x1a\t.StatusOkb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tests_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_TEST']._serialized_start=32
   _globals['_TEST']._serialized_end=130
   _globals['_CREATETESTSREQUEST']._serialized_start=132
-  _globals['_CREATETESTSREQUEST']._serialized_end=174
-  _globals['_TESTSSERVICE']._serialized_start=176
-  _globals['_TESTSSERVICE']._serialized_end=237
+  _globals['_CREATETESTSREQUEST']._serialized_end=199
+  _globals['_TESTSSERVICE']._serialized_start=201
+  _globals['_TESTSSERVICE']._serialized_end=262
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pytest_initry-0.2.0/pytest_initry/protobufs/tests_pb2.pyi` & `pytest_initry-0.3.0/pytest_initry/protobufs/tests_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -17,11 +17,13 @@
     location: str
     uuid: str
     test_run_uuid: str
     description: str
     def __init__(self, nodeid: _Optional[str] = ..., location: _Optional[str] = ..., uuid: _Optional[str] = ..., test_run_uuid: _Optional[str] = ..., description: _Optional[str] = ...) -> None: ...
 
 class CreateTestsRequest(_message.Message):
-    __slots__ = ("tests",)
+    __slots__ = ("tests", "only_tests_info")
     TESTS_FIELD_NUMBER: _ClassVar[int]
+    ONLY_TESTS_INFO_FIELD_NUMBER: _ClassVar[int]
     tests: _containers.RepeatedCompositeFieldContainer[Test]
-    def __init__(self, tests: _Optional[_Iterable[_Union[Test, _Mapping]]] = ...) -> None: ...
+    only_tests_info: bool
+    def __init__(self, tests: _Optional[_Iterable[_Union[Test, _Mapping]]] = ..., only_tests_info: bool = ...) -> None: ...
```

### Comparing `pytest_initry-0.2.0/pytest_initry/protobufs/tests_pb2_grpc.py` & `pytest_initry-0.3.0/pytest_initry/protobufs/tests_pb2_grpc.py`

 * *Files identical despite different names*

