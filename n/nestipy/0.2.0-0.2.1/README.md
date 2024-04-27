# Comparing `tmp/nestipy-0.2.0.tar.gz` & `tmp/nestipy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy-0.2.0.tar", max compression
+gzip compressed data, was "nestipy-0.2.1.tar", max compression
```

## Comparing `nestipy-0.2.0.tar` & `nestipy-0.2.1.tar`

### file list

```diff
@@ -1,116 +1,118 @@
--rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy-0.2.0/LICENSE
--rw-r--r--   0        0        0     1913 2024-04-26 12:17:55.140372 nestipy-0.2.0/README.md
--rw-r--r--   0        0        0     1046 2024-04-26 12:17:55.152372 nestipy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-29 12:35:05.153461 nestipy-0.2.0/src/nestipy/__init__.py
--rw-r--r--   0        0        0     1151 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/__init__.py
--rw-r--r--   0        0        0     1489 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      652 2024-03-29 11:21:44.572810 nestipy-0.2.0/src/nestipy/common/__pycache__/http_method.cpython-311.pyc
--rw-r--r--   0        0        0      978 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/config/__init__.py
--rw-r--r--   0        0        0      246 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/decorator/__init__.py
--rw-r--r--   0        0        0     2957 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/decorator/class_.py
--rw-r--r--   0        0        0     1204 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/decorator/method.py
--rw-r--r--   0        0        0      367 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/exception/__init__.py
--rw-r--r--   0        0        0      732 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/exception/decorator.py
--rw-r--r--   0        0        0      433 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/exception/http.py
--rw-r--r--   0        0        0      364 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/exception/interface.py
--rw-r--r--   0        0        0     2531 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/exception/message.py
--rw-r--r--   0        0        0      113 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/exception/meta.py
--rw-r--r--   0        0        0     1686 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/exception/status.py
--rw-r--r--   0        0        0      164 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/guards/__init__.py
--rw-r--r--   0        0        0      326 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/guards/can_activate.py
--rw-r--r--   0        0        0      332 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/guards/decorator.py
--rw-r--r--   0        0        0       45 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/guards/meta.py
--rw-r--r--   0        0        0      719 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/helpers/__init__.py
--rw-r--r--   0        0        0      208 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/http_/__init__.py
--rw-r--r--   0        0        0     4503 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/http_/multipart.py
--rw-r--r--   0        0        0     4231 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/http_/request.py
--rw-r--r--   0        0        0     4989 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/http_/response.py
--rw-r--r--   0        0        0      478 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/http_/test.py
--rw-r--r--   0        0        0     1403 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/http_/upload_file.py
--rw-r--r--   0        0        0      303 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/http_/websocket.py
--rw-r--r--   0        0        0      199 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/interceptor/__init__.py
--rw-r--r--   0        0        0      489 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/interceptor/decorator.py
--rw-r--r--   0        0        0      352 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/interceptor/interface.py
--rw-r--r--   0        0        0       52 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/interceptor/meta.py
--rw-r--r--   0        0        0      168 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/middleware/__init__.py
--rw-r--r--   0        0        0      695 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/middleware/cors.py
--rw-r--r--   0        0        0      323 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/middleware/interface.py
--rw-r--r--   0        0        0      100 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/middleware/meta.py
--rw-r--r--   0        0        0      167 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/template/__init__.py
--rw-r--r--   0        0        0      274 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/template/decorator.py
--rw-r--r--   0        0        0      627 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/template/interface.py
--rw-r--r--   0        0        0      109 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/template/meta.py
--rw-r--r--   0        0        0     1590 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/common/utils.py
--rw-r--r--   0        0        0      779 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/__init__.py
--rw-r--r--   0        0        0      986 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    16492 2024-03-29 11:21:44.576810 nestipy-0.2.0/src/nestipy/core/__pycache__/app_context.cpython-311.pyc
--rw-r--r--   0        0        0     1929 2024-03-29 11:21:44.576810 nestipy-0.2.0/src/nestipy/core/__pycache__/factory.cpython-311.pyc
--rw-r--r--   0        0        0     1567 2024-03-29 11:21:44.576810 nestipy-0.2.0/src/nestipy/core/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0      212 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/adapter/__init__.py
--rw-r--r--   0        0        0     4224 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/adapter/blacksheep_adapter.py
--rw-r--r--   0        0        0     3803 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/adapter/fastapi_adapter.py
--rw-r--r--   0        0        0     5666 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/adapter/http_adapter.py
--rw-r--r--   0        0        0      418 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/constant.py
--rw-r--r--   0        0        0        0 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/context/__init__.py
--rw-r--r--   0        0        0     1250 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/context/argument_host.py
--rw-r--r--   0        0        0      802 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/context/execution_context.py
--rw-r--r--   0        0        0      369 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/context/http_argument_host.py
--rw-r--r--   0        0        0       90 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/exception/__init__.py
--rw-r--r--   0        0        0     4040 2024-04-26 12:17:55.156372 nestipy-0.2.0/src/nestipy/core/exception/processor.py
--rw-r--r--   0        0        0       75 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/guards/__init__.py
--rw-r--r--   0        0        0     2164 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/guards/processor.py
--rw-r--r--   0        0        0     2758 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/instance_loader.py
--rw-r--r--   0        0        0       82 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/interceptor/__init__.py
--rw-r--r--   0        0        0     2569 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/interceptor/processor.py
--rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/meta/__init__.py
--rw-r--r--   0        0        0      380 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/meta/controller_metadata_creator.py
--rw-r--r--   0        0        0     4040 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/meta/metadata_creator.py
--rw-r--r--   0        0        0      771 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/meta/module_metadata_creator.py
--rw-r--r--   0        0        0      374 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/meta/provider_metadata_creator.py
--rw-r--r--   0        0        0      162 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/middleware/__init__.py
--rw-r--r--   0        0        0     3949 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/middleware/executor.py
--rw-r--r--   0        0        0     8673 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/nestipy_application.py
--rw-r--r--   0        0        0      913 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/nestipy_factory.py
--rw-r--r--   0        0        0       89 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/platform/__init__.py
--rw-r--r--   0        0        0      608 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3199 2024-03-29 11:21:44.576810 nestipy-0.2.0/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc
--rw-r--r--   0        0        0     7185 2024-03-29 11:21:44.576810 nestipy-0.2.0/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc
--rw-r--r--   0        0        0     7397 2024-03-29 11:21:44.576810 nestipy-0.2.0/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/router/__init__.py
--rw-r--r--   0        0        0     2879 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/router/route_explorer.py
--rw-r--r--   0        0        0      510 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/router/route_extractor.py
--rw-r--r--   0        0        0     7859 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/router/router_proxy.py
--rw-r--r--   0        0        0      184 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/template/__init__.py
--rw-r--r--   0        0        0     1004 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/template/minimal_jinja.py
--rw-r--r--   0        0        0     1457 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/core/template/processor.py
--rw-r--r--   0        0        0      282 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/__init__.py
--rw-r--r--   0        0        0     1533 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/decorator.py
--rw-r--r--   0        0        0     2244 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/graphql_adapter.py
--rw-r--r--   0        0        0     1111 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/graphql_asgi.py
--rw-r--r--   0        0        0     1871 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/graphql_explorer.py
--rw-r--r--   0        0        0      547 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/graphql_module.py
--rw-r--r--   0        0        0     4326 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/graphql_proxy.py
--rw-r--r--   0        0        0      289 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/meta.py
--rw-r--r--   0        0        0     1531 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/playground/graphql-playground-default.html
--rw-r--r--   0        0        0     3486 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/playground/graphql-playground-graphiql.html
--rw-r--r--   0        0        0      704 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/pubsub.py
--rw-r--r--   0        0        0      648 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/strawberry/__init__.py
--rw-r--r--   0        0        0     2103 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/strawberry/strawberry_adapter.py
--rw-r--r--   0        0        0     1588 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/strawberry/strawberry_asgi.py
--rw-r--r--   0        0        0      110 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/graphql/test.py
--rw-r--r--   0        0        0     1105 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/openapi/__init__.py
--rw-r--r--   0        0        0       49 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/openapi/constant.py
--rw-r--r--   0        0        0     3139 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/openapi/decorator.py
--rw-r--r--   0        0        0     1500 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/openapi/document_builder.py
--rw-r--r--   0        0        0      423 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/openapi/explorer.py
--rw-r--r--   0        0        0     1323 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/openapi/swagger.html
--rw-r--r--   0        0        0     2195 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/openapi/swagger_module.py
--rw-r--r--   0        0        0     2728 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/openapi/test.py
--rw-r--r--   0        0        0      220 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/types_/__init__.py
--rw-r--r--   0        0        0      393 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/types_/handler.py
--rw-r--r--   0        0        0      123 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/types_/http.py
--rw-r--r--   0        0        0      254 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/websocket/__init__.py
--rw-r--r--   0        0        0     2988 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/websocket/adapter.py
--rw-r--r--   0        0        0      716 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/websocket/decorator.py
--rw-r--r--   0        0        0     4517 2024-04-26 12:17:55.160372 nestipy-0.2.0/src/nestipy/websocket/proxy.py
--rw-r--r--   0        0        0     3554 1970-01-01 00:00:00.000000 nestipy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy-0.2.1/README.md
+-rw-r--r--   0        0        0     1046 2024-04-27 15:31:08.560661 nestipy-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-29 12:35:05.153461 nestipy-0.2.1/src/nestipy/__init__.py
+-rw-r--r--   0        0        0     1151 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/__init__.py
+-rw-r--r--   0        0        0     1489 2024-04-27 15:03:54.888341 nestipy-0.2.1/src/nestipy/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      652 2024-03-29 11:21:44.572810 nestipy-0.2.1/src/nestipy/common/__pycache__/http_method.cpython-311.pyc
+-rw-r--r--   0        0        0      978 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/config/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/decorator/__init__.py
+-rw-r--r--   0        0        0     2957 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/decorator/class_.py
+-rw-r--r--   0        0        0     1204 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/decorator/method.py
+-rw-r--r--   0        0        0      367 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/exception/__init__.py
+-rw-r--r--   0        0        0      732 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/exception/decorator.py
+-rw-r--r--   0        0        0      433 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/exception/http.py
+-rw-r--r--   0        0        0      364 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/exception/interface.py
+-rw-r--r--   0        0        0     2531 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/exception/message.py
+-rw-r--r--   0        0        0      113 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/exception/meta.py
+-rw-r--r--   0        0        0     1686 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/exception/status.py
+-rw-r--r--   0        0        0      164 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/guards/__init__.py
+-rw-r--r--   0        0        0      326 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/guards/can_activate.py
+-rw-r--r--   0        0        0      332 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/guards/decorator.py
+-rw-r--r--   0        0        0       45 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/guards/meta.py
+-rw-r--r--   0        0        0      719 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/helpers/__init__.py
+-rw-r--r--   0        0        0      208 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/http_/__init__.py
+-rw-r--r--   0        0        0     4503 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/http_/multipart.py
+-rw-r--r--   0        0        0     4231 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/http_/request.py
+-rw-r--r--   0        0        0     4989 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/http_/response.py
+-rw-r--r--   0        0        0      478 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/http_/test.py
+-rw-r--r--   0        0        0     1403 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/http_/upload_file.py
+-rw-r--r--   0        0        0      303 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/http_/websocket.py
+-rw-r--r--   0        0        0      199 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/interceptor/__init__.py
+-rw-r--r--   0        0        0      489 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/interceptor/decorator.py
+-rw-r--r--   0        0        0      352 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/interceptor/interface.py
+-rw-r--r--   0        0        0       52 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/interceptor/meta.py
+-rw-r--r--   0        0        0      168 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/middleware/__init__.py
+-rw-r--r--   0        0        0      695 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/middleware/cors.py
+-rw-r--r--   0        0        0      323 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/middleware/interface.py
+-rw-r--r--   0        0        0      100 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/middleware/meta.py
+-rw-r--r--   0        0        0      167 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/template/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/template/decorator.py
+-rw-r--r--   0        0        0      627 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/template/interface.py
+-rw-r--r--   0        0        0      109 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/template/meta.py
+-rw-r--r--   0        0        0     1590 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/common/utils.py
+-rw-r--r--   0        0        0      882 2024-04-27 15:16:06.308484 nestipy-0.2.1/src/nestipy/core/__init__.py
+-rw-r--r--   0        0        0     1114 2024-04-27 15:17:40.212502 nestipy-0.2.1/src/nestipy/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    16492 2024-03-29 11:21:44.576810 nestipy-0.2.1/src/nestipy/core/__pycache__/app_context.cpython-311.pyc
+-rw-r--r--   0        0        0     1929 2024-03-29 11:21:44.576810 nestipy-0.2.1/src/nestipy/core/__pycache__/factory.cpython-311.pyc
+-rw-r--r--   0        0        0     1567 2024-03-29 11:21:44.576810 nestipy-0.2.1/src/nestipy/core/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0      212 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/core/adapter/__init__.py
+-rw-r--r--   0        0        0     4224 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/core/adapter/blacksheep_adapter.py
+-rw-r--r--   0        0        0     3803 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/core/adapter/fastapi_adapter.py
+-rw-r--r--   0        0        0     5666 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/core/adapter/http_adapter.py
+-rw-r--r--   0        0        0      418 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/core/constant.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/core/context/__init__.py
+-rw-r--r--   0        0        0     1250 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/core/context/argument_host.py
+-rw-r--r--   0        0        0      802 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/core/context/execution_context.py
+-rw-r--r--   0        0        0      369 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/core/context/http_argument_host.py
+-rw-r--r--   0        0        0      730 2024-04-27 15:14:06.840460 nestipy-0.2.1/src/nestipy/core/discover.py
+-rw-r--r--   0        0        0       90 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/core/exception/__init__.py
+-rw-r--r--   0        0        0     4040 2024-04-26 12:17:55.156372 nestipy-0.2.1/src/nestipy/core/exception/processor.py
+-rw-r--r--   0        0        0       75 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/core/guards/__init__.py
+-rw-r--r--   0        0        0     2164 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/core/guards/processor.py
+-rw-r--r--   0        0        0     3739 2024-04-27 15:28:39.940632 nestipy-0.2.1/src/nestipy/core/instance_loader.py
+-rw-r--r--   0        0        0       82 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/core/interceptor/__init__.py
+-rw-r--r--   0        0        0     2569 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/core/interceptor/processor.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/core/meta/__init__.py
+-rw-r--r--   0        0        0      380 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/core/meta/controller_metadata_creator.py
+-rw-r--r--   0        0        0     4040 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/core/meta/metadata_creator.py
+-rw-r--r--   0        0        0      771 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/core/meta/module_metadata_creator.py
+-rw-r--r--   0        0        0      374 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/core/meta/provider_metadata_creator.py
+-rw-r--r--   0        0        0      162 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/core/middleware/__init__.py
+-rw-r--r--   0        0        0     3949 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/core/middleware/executor.py
+-rw-r--r--   0        0        0     8889 2024-04-27 15:24:30.668583 nestipy-0.2.1/src/nestipy/core/nestipy_application.py
+-rw-r--r--   0        0        0      913 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/core/nestipy_factory.py
+-rw-r--r--   0        0        0      107 2024-04-27 15:17:12.268497 nestipy-0.2.1/src/nestipy/core/on_init.py
+-rw-r--r--   0        0        0       89 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/core/platform/__init__.py
+-rw-r--r--   0        0        0      608 2024-04-27 15:03:56.320341 nestipy-0.2.1/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3199 2024-03-29 11:21:44.576810 nestipy-0.2.1/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc
+-rw-r--r--   0        0        0     7185 2024-03-29 11:21:44.576810 nestipy-0.2.1/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc
+-rw-r--r--   0        0        0     7397 2024-03-29 11:21:44.576810 nestipy-0.2.1/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/core/router/__init__.py
+-rw-r--r--   0        0        0     2879 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/core/router/route_explorer.py
+-rw-r--r--   0        0        0      510 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/core/router/route_extractor.py
+-rw-r--r--   0        0        0     7920 2024-04-27 06:23:56.643738 nestipy-0.2.1/src/nestipy/core/router/router_proxy.py
+-rw-r--r--   0        0        0      184 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/core/template/__init__.py
+-rw-r--r--   0        0        0     1004 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/core/template/minimal_jinja.py
+-rw-r--r--   0        0        0     1457 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/core/template/processor.py
+-rw-r--r--   0        0        0      282 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/graphql/__init__.py
+-rw-r--r--   0        0        0     1533 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/graphql/decorator.py
+-rw-r--r--   0        0        0     2244 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/graphql/graphql_adapter.py
+-rw-r--r--   0        0        0     1111 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/graphql/graphql_asgi.py
+-rw-r--r--   0        0        0     1871 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/graphql/graphql_explorer.py
+-rw-r--r--   0        0        0      547 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/graphql/graphql_module.py
+-rw-r--r--   0        0        0     4326 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/graphql/graphql_proxy.py
+-rw-r--r--   0        0        0      289 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/graphql/meta.py
+-rw-r--r--   0        0        0     1531 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/graphql/playground/graphql-playground-default.html
+-rw-r--r--   0        0        0     3486 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/graphql/playground/graphql-playground-graphiql.html
+-rw-r--r--   0        0        0      704 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/graphql/pubsub.py
+-rw-r--r--   0        0        0      648 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/graphql/strawberry/__init__.py
+-rw-r--r--   0        0        0     2103 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/graphql/strawberry/strawberry_adapter.py
+-rw-r--r--   0        0        0     1588 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/graphql/strawberry/strawberry_asgi.py
+-rw-r--r--   0        0        0      110 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/graphql/test.py
+-rw-r--r--   0        0        0     1105 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/openapi/__init__.py
+-rw-r--r--   0        0        0       49 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/openapi/constant.py
+-rw-r--r--   0        0        0     3139 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/openapi/decorator.py
+-rw-r--r--   0        0        0     1500 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/openapi/document_builder.py
+-rw-r--r--   0        0        0      423 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/openapi/explorer.py
+-rw-r--r--   0        0        0     1323 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/openapi/swagger.html
+-rw-r--r--   0        0        0     2195 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/openapi/swagger_module.py
+-rw-r--r--   0        0        0     2728 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/openapi/test.py
+-rw-r--r--   0        0        0      220 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/types_/__init__.py
+-rw-r--r--   0        0        0      393 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/types_/handler.py
+-rw-r--r--   0        0        0      123 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/types_/http.py
+-rw-r--r--   0        0        0      254 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/websocket/__init__.py
+-rw-r--r--   0        0        0     2988 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/websocket/adapter.py
+-rw-r--r--   0        0        0      716 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/websocket/decorator.py
+-rw-r--r--   0        0        0     4517 2024-04-26 12:17:55.160372 nestipy-0.2.1/src/nestipy/websocket/proxy.py
+-rw-r--r--   0        0        0     3547 1970-01-01 00:00:00.000000 nestipy-0.2.1/PKG-INFO
```

### Comparing `nestipy-0.2.0/LICENSE` & `nestipy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/README.md` & `nestipy-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     ├── README.md
     
        
 ```
 
 ## Documentation
 
-View full documentation from [here](https://nestipy.github.io/nestipy).
+View full documentation from [here](https://nestipy.vercel.app).
 
 ## Support
 
 Nestipy is an MIT-licensed open source project. It can grow thanks to the sponsors and support from the amazing backers.
 If you'd like to join them, please [read more here].
 
 ## Stay in touch
```

#### html2text {}

```diff
@@ -6,12 +6,12 @@
 Under the hood, Nestipy makes use of _F_a_s_t_A_P_I, but also provides compatibility
 with a wide range of other libraries, like _B_l_a_c_k_s_h_e_e_p, allowing for easy use of
 the myriad of third-party plugins which are available.
 ## Getting started ```cmd pip install nestipy-cli nestipy new my_app cd my_app
 python main.py ``` ``` âââ src â âââ __init__.py âââ
 app_module.py âââ app_controller.py âââ app_service.py âââ
 main.py âââ requirements.txt âââ README.md ``` ## Documentation
-View full documentation from [here](https://nestipy.github.io/nestipy). ##
-Support Nestipy is an MIT-licensed open source project. It can grow thanks to
-the sponsors and support from the amazing backers. If you'd like to join them,
+View full documentation from [here](https://nestipy.vercel.app). ## Support
+Nestipy is an MIT-licensed open source project. It can grow thanks to the
+sponsors and support from the amazing backers. If you'd like to join them,
 please [read more here]. ## Stay in touch - Author - [Tsiresy Mila](https://
 tsiresymila.vercel.app) ## License Nestipy is [MIT licensed](LICENSE).
```

### Comparing `nestipy-0.2.0/pyproject.toml` & `nestipy-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nestipy"
-version = "0.2.0"
+version = "0.2.1"
 description = "Nestipy is a Python framework built on top of BlackSheep that follows the modular architecture of NestJS"
 authors = ["tsiresymila <tsiresymila@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "nestipy", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `nestipy-0.2.0/src/nestipy/common/__init__.py` & `nestipy-0.2.1/src/nestipy/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/common/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.2.1/src/nestipy/common/__pycache__/__init__.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x27142a66 (Thu Apr 25 08:28:23 2024 UTC)
+moddate:  0x739b2b66 (Fri Apr 26 12:17:55 2024 UTC)
 files sz: 1151
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `nestipy-0.2.0/src/nestipy/common/__pycache__/http_method.cpython-311.pyc` & `nestipy-0.2.1/src/nestipy/common/__pycache__/http_method.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/common/config/__init__.py` & `nestipy-0.2.1/src/nestipy/common/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/common/decorator/class_.py` & `nestipy-0.2.1/src/nestipy/common/decorator/class_.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/common/decorator/method.py` & `nestipy-0.2.1/src/nestipy/common/decorator/method.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/common/exception/decorator.py` & `nestipy-0.2.1/src/nestipy/common/exception/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/common/exception/message.py` & `nestipy-0.2.1/src/nestipy/common/exception/message.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/common/exception/status.py` & `nestipy-0.2.1/src/nestipy/common/exception/status.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/common/helpers/__init__.py` & `nestipy-0.2.1/src/nestipy/common/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/common/http_/multipart.py` & `nestipy-0.2.1/src/nestipy/common/http_/multipart.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/common/http_/request.py` & `nestipy-0.2.1/src/nestipy/common/http_/request.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/common/http_/response.py` & `nestipy-0.2.1/src/nestipy/common/http_/response.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/common/http_/upload_file.py` & `nestipy-0.2.1/src/nestipy/common/http_/upload_file.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/common/middleware/cors.py` & `nestipy-0.2.1/src/nestipy/common/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/common/template/interface.py` & `nestipy-0.2.1/src/nestipy/common/template/interface.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/common/utils.py` & `nestipy-0.2.1/src/nestipy/common/utils.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/__init__.py` & `nestipy-0.2.1/src/nestipy/core/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from .adapter.http_adapter import HttpAdapter
 from .constant import AppKey
 from .context.execution_context import ExecutionContext, ArgumentHost, HttpArgumentHost
+from .discover import DiscoverService
 from .middleware import MiddlewareConsumer
 from .nestipy_application import NestipyApplication, NestipyApplicationConfig
 from .nestipy_factory import NestipyFactory
+from .on_init import OnInit
 from .platform import NestipyFastApiApplication, NestipyBlackSheepApplication
 from .template import MinimalJinjaTemplateEngine
 
 __all__ = [
     "NestipyFactory",
     "NestipyApplication",
     "NestipyApplicationConfig",
@@ -15,9 +17,11 @@
     "ExecutionContext",
     "ArgumentHost",
     "HttpArgumentHost",
     "NestipyFastApiApplication",
     "NestipyBlackSheepApplication",
     "MinimalJinjaTemplateEngine",
     "AppKey",
-    "MiddlewareConsumer"
+    "MiddlewareConsumer",
+    "DiscoverService",
+    "OnInit"
 ]
```

### Comparing `nestipy-0.2.0/src/nestipy/core/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.2.1/src/nestipy/core/__pycache__/__init__.cpython-311.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,21 +1,22 @@
 magic:    0xa70d0d0a
-moddate:  0xf0d52866 (Wed Apr 24 09:50:40 2024 UTC)
-files sz: 779
+moddate:  0xb6162d66 (Sat Apr 27 15:16:06 2024 UTC)
+files sz: 882
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c046d055a056d065a066d075a070100640064046c086d095a09010064
-      0064056c0a6d0b5a0b6d0c5a0c0100640064066c0d6d0e5a0e0100640064
-      076c0f6d105a106d115a110100640064086c126d135a13010067006409a2
-      015a14640a5300
+      0064056c0a6d0b5a0b0100640064066c0c6d0d5a0d6d0e5a0e0100640064
+      076c0f6d105a100100640064086c116d125a120100640064096c136d145a
+      146d155a1501006400640a6c166d175a1701006700640ba2015a18640c53
+      00
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (1)
                  4 LOAD_CONST               1 (('HttpAdapter',))
                  6 IMPORT_NAME              0 (adapter.http_adapter)
                  8 IMPORT_FROM              1 (HttpAdapter)
                 10 STORE_NAME               1 (HttpAdapter)
@@ -36,71 +37,87 @@
                 36 IMPORT_FROM              6 (ArgumentHost)
                 38 STORE_NAME               6 (ArgumentHost)
                 40 IMPORT_FROM              7 (HttpArgumentHost)
                 42 STORE_NAME               7 (HttpArgumentHost)
                 44 POP_TOP
    
      4          46 LOAD_CONST               0 (1)
-                48 LOAD_CONST               4 (('MiddlewareConsumer',))
-                50 IMPORT_NAME              8 (middleware)
-                52 IMPORT_FROM              9 (MiddlewareConsumer)
-                54 STORE_NAME               9 (MiddlewareConsumer)
+                48 LOAD_CONST               4 (('DiscoverService',))
+                50 IMPORT_NAME              8 (discover)
+                52 IMPORT_FROM              9 (DiscoverService)
+                54 STORE_NAME               9 (DiscoverService)
                 56 POP_TOP
    
      5          58 LOAD_CONST               0 (1)
-                60 LOAD_CONST               5 (('NestipyApplication', 'NestipyApplicationConfig'))
-                62 IMPORT_NAME             10 (nestipy_application)
-                64 IMPORT_FROM             11 (NestipyApplication)
-                66 STORE_NAME              11 (NestipyApplication)
-                68 IMPORT_FROM             12 (NestipyApplicationConfig)
-                70 STORE_NAME              12 (NestipyApplicationConfig)
-                72 POP_TOP
-   
-     6          74 LOAD_CONST               0 (1)
-                76 LOAD_CONST               6 (('NestipyFactory',))
-                78 IMPORT_NAME             13 (nestipy_factory)
-                80 IMPORT_FROM             14 (NestipyFactory)
-                82 STORE_NAME              14 (NestipyFactory)
+                60 LOAD_CONST               5 (('MiddlewareConsumer',))
+                62 IMPORT_NAME             10 (middleware)
+                64 IMPORT_FROM             11 (MiddlewareConsumer)
+                66 STORE_NAME              11 (MiddlewareConsumer)
+                68 POP_TOP
+   
+     6          70 LOAD_CONST               0 (1)
+                72 LOAD_CONST               6 (('NestipyApplication', 'NestipyApplicationConfig'))
+                74 IMPORT_NAME             12 (nestipy_application)
+                76 IMPORT_FROM             13 (NestipyApplication)
+                78 STORE_NAME              13 (NestipyApplication)
+                80 IMPORT_FROM             14 (NestipyApplicationConfig)
+                82 STORE_NAME              14 (NestipyApplicationConfig)
                 84 POP_TOP
    
      7          86 LOAD_CONST               0 (1)
-                88 LOAD_CONST               7 (('NestipyFastApiApplication', 'NestipyBlackSheepApplication'))
-                90 IMPORT_NAME             15 (platform)
-                92 IMPORT_FROM             16 (NestipyFastApiApplication)
-                94 STORE_NAME              16 (NestipyFastApiApplication)
-                96 IMPORT_FROM             17 (NestipyBlackSheepApplication)
-                98 STORE_NAME              17 (NestipyBlackSheepApplication)
-               100 POP_TOP
-   
-     8         102 LOAD_CONST               0 (1)
-               104 LOAD_CONST               8 (('MinimalJinjaTemplateEngine',))
-               106 IMPORT_NAME             18 (template)
-               108 IMPORT_FROM             19 (MinimalJinjaTemplateEngine)
-               110 STORE_NAME              19 (MinimalJinjaTemplateEngine)
-               112 POP_TOP
-   
-    10         114 BUILD_LIST               0
-               116 LOAD_CONST               9 (('NestipyFactory', 'NestipyApplication', 'NestipyApplicationConfig', 'HttpAdapter', 'ExecutionContext', 'ArgumentHost', 'HttpArgumentHost', 'NestipyFastApiApplication', 'NestipyBlackSheepApplication', 'MinimalJinjaTemplateEngine', 'AppKey', 'MiddlewareConsumer'))
-               118 LIST_EXTEND              1
-               120 STORE_NAME              20 (__all__)
-               122 LOAD_CONST              10 (None)
-               124 RETURN_VALUE
+                88 LOAD_CONST               7 (('NestipyFactory',))
+                90 IMPORT_NAME             15 (nestipy_factory)
+                92 IMPORT_FROM             16 (NestipyFactory)
+                94 STORE_NAME              16 (NestipyFactory)
+                96 POP_TOP
+   
+     8          98 LOAD_CONST               0 (1)
+               100 LOAD_CONST               8 (('OnInit',))
+               102 IMPORT_NAME             17 (on_init)
+               104 IMPORT_FROM             18 (OnInit)
+               106 STORE_NAME              18 (OnInit)
+               108 POP_TOP
+   
+     9         110 LOAD_CONST               0 (1)
+               112 LOAD_CONST               9 (('NestipyFastApiApplication', 'NestipyBlackSheepApplication'))
+               114 IMPORT_NAME             19 (platform)
+               116 IMPORT_FROM             20 (NestipyFastApiApplication)
+               118 STORE_NAME              20 (NestipyFastApiApplication)
+               120 IMPORT_FROM             21 (NestipyBlackSheepApplication)
+               122 STORE_NAME              21 (NestipyBlackSheepApplication)
+               124 POP_TOP
+   
+    10         126 LOAD_CONST               0 (1)
+               128 LOAD_CONST              10 (('MinimalJinjaTemplateEngine',))
+               130 IMPORT_NAME             22 (template)
+               132 IMPORT_FROM             23 (MinimalJinjaTemplateEngine)
+               134 STORE_NAME              23 (MinimalJinjaTemplateEngine)
+               136 POP_TOP
+   
+    12         138 BUILD_LIST               0
+               140 LOAD_CONST              11 (('NestipyFactory', 'NestipyApplication', 'NestipyApplicationConfig', 'HttpAdapter', 'ExecutionContext', 'ArgumentHost', 'HttpArgumentHost', 'NestipyFastApiApplication', 'NestipyBlackSheepApplication', 'MinimalJinjaTemplateEngine', 'AppKey', 'MiddlewareConsumer', 'DiscoverService', 'OnInit'))
+               142 LIST_EXTEND              1
+               144 STORE_NAME              24 (__all__)
+               146 LOAD_CONST              12 (None)
+               148 RETURN_VALUE
    consts
       1
       ('HttpAdapter',)
       ('AppKey',)
       ('ExecutionContext', 'ArgumentHost', 'HttpArgumentHost')
+      ('DiscoverService',)
       ('MiddlewareConsumer',)
       ('NestipyApplication', 'NestipyApplicationConfig')
       ('NestipyFactory',)
+      ('OnInit',)
       ('NestipyFastApiApplication', 'NestipyBlackSheepApplication')
       ('MinimalJinjaTemplateEngine',)
-      ('NestipyFactory', 'NestipyApplication', 'NestipyApplicationConfig', 'HttpAdapter', 'ExecutionContext', 'ArgumentHost', 'HttpArgumentHost', 'NestipyFastApiApplication', 'NestipyBlackSheepApplication', 'MinimalJinjaTemplateEngine', 'AppKey', 'MiddlewareConsumer')
+      ('NestipyFactory', 'NestipyApplication', 'NestipyApplicationConfig', 'HttpAdapter', 'ExecutionContext', 'ArgumentHost', 'HttpArgumentHost', 'NestipyFastApiApplication', 'NestipyBlackSheepApplication', 'MinimalJinjaTemplateEngine', 'AppKey', 'MiddlewareConsumer', 'DiscoverService', 'OnInit')
       None
-   names      ('adapter.http_adapter', 'HttpAdapter', 'constant', 'AppKey', 'context.execution_context', 'ExecutionContext', 'ArgumentHost', 'HttpArgumentHost', 'middleware', 'MiddlewareConsumer', 'nestipy_application', 'NestipyApplication', 'NestipyApplicationConfig', 'nestipy_factory', 'NestipyFactory', 'platform', 'NestipyFastApiApplication', 'NestipyBlackSheepApplication', 'template', 'MinimalJinjaTemplateEngine', '__all__')
+   names      ('adapter.http_adapter', 'HttpAdapter', 'constant', 'AppKey', 'context.execution_context', 'ExecutionContext', 'ArgumentHost', 'HttpArgumentHost', 'discover', 'DiscoverService', 'middleware', 'MiddlewareConsumer', 'nestipy_application', 'NestipyApplication', 'NestipyApplicationConfig', 'nestipy_factory', 'NestipyFactory', 'on_init', 'OnInit', 'platform', 'NestipyFastApiApplication', 'NestipyBlackSheepApplication', 'template', 'MinimalJinjaTemplateEngine', '__all__')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/tsiresy/work/python/nestipy/src/nestipy/core/__init__.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c0114010c0110010c0110010c02
+   lnotab 0x00ff02010c010c0114010c010c0110010c010c0110010c02
```

### Comparing `nestipy-0.2.0/src/nestipy/core/__pycache__/app_context.cpython-311.pyc` & `nestipy-0.2.1/src/nestipy/core/__pycache__/app_context.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/__pycache__/factory.cpython-311.pyc` & `nestipy-0.2.1/src/nestipy/core/__pycache__/factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/__pycache__/utils.cpython-311.pyc` & `nestipy-0.2.1/src/nestipy/core/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/adapter/blacksheep_adapter.py` & `nestipy-0.2.1/src/nestipy/core/adapter/blacksheep_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/adapter/fastapi_adapter.py` & `nestipy-0.2.1/src/nestipy/core/adapter/fastapi_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/adapter/http_adapter.py` & `nestipy-0.2.1/src/nestipy/core/adapter/http_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/context/argument_host.py` & `nestipy-0.2.1/src/nestipy/core/context/argument_host.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/context/execution_context.py` & `nestipy-0.2.1/src/nestipy/core/context/execution_context.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/exception/processor.py` & `nestipy-0.2.1/src/nestipy/core/exception/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/guards/processor.py` & `nestipy-0.2.1/src/nestipy/core/guards/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/instance_loader.py` & `nestipy-0.2.1/src/nestipy/core/instance_loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import typing
 from typing import Type, Any
 
 from nestipy_dynamic_module import DynamicModule, MiddlewareConsumer, NestipyModule
 from nestipy_ioc import NestipyContainer, ModuleProviderDict
 from nestipy_metadata import ModuleMetadata, Reflect
 
+from .discover import DiscoverService
+from .on_init import OnInit
 from ..graphql.graphql_module import GraphqlModule
 
 
 class InstanceType(enum.Enum):
     providers: str = 'Provider'
     controller: str = 'Controller',
     module: str = 'Module'
@@ -19,54 +21,75 @@
     """
     Create all instance of controller and providers, resolvers, middleware
     use before route mapper
     """
     _is_controller: bool = False
     _module_instances: list = []
     graphql_instance: GraphqlModule = None
+    discover: DiscoverService
 
     async def create_instances(self, modules: list[Type]) -> GraphqlModule:
+        self.discover = await NestipyContainer.get_instance().get(DiscoverService)
         for module in modules:
             if isinstance(module, DynamicModule):
                 module = module.module
             if module in self._module_instances:
                 continue
-            await self._create_providers(module)
+            providers = await self._create_providers(module)
+            self.discover.add_provider(*providers)
             self._is_controller = True
-            await self._create_controllers(module)
+            controllers = await self._create_controllers(module)
+            self.discover.add_controller(*controllers)
             self._is_controller = False
             instance = await self.create_instance(module)
-            self._module_instances.append(module)
+            self.discover.add_module(instance)
             if isinstance(instance, GraphqlModule):
                 self.graphql_instance = instance
             imports = Reflect.get_metadata(module, ModuleMetadata.Imports, [])
             await self.create_instances(imports)
         return self.graphql_instance
 
-    async def _create_providers(self, module: Type) -> None:
+    async def _create_providers(self, module: Type) -> list:
+        provider_instance = []
         for provider in Reflect.get_metadata(module, ModuleMetadata.Providers, []):
             if isinstance(provider, ModuleProviderDict):
                 continue
-            await self.create_instance(provider)
+            ins = await self.create_instance(provider)
+            provider_instance.append(ins)
+        return provider_instance
 
-    async def _create_controllers(self, module: Type) -> None:
+    async def _create_controllers(self, module: Type) -> list:
+        controller_instance = []
         for controller in Reflect.get_metadata(module, ModuleMetadata.Controllers, []):
-            await self.create_instance(controller)
+            ins = await self.create_instance(controller)
+            controller_instance.append(ins)
+        return controller_instance
 
     async def create_instance(self, class_ref: Type) -> object:
         instance = await NestipyContainer.get_instance().get(class_ref)
         await self.initialize_instance(class_ref, instance)
         return instance
 
     @classmethod
     async def initialize_instance(cls, class_ref: Type, instance: Any) -> None:
         # call configure for module
         if issubclass(class_ref, NestipyModule):
             consumer = MiddlewareConsumer(module=class_ref)
             module = typing.cast(NestipyModule, instance)
             module.configure(consumer)
-            await module.on_startup()
+            # await module.on_startup()
+        elif issubclass(class_ref, OnInit):
+            ins = typing.cast(OnInit, instance)
+            await ins.on_startup()
 
     async def destroy(self):
-        for module in self._module_instances:
+        for module in self.discover.get_all_module():
             if isinstance(module, NestipyModule):
                 await module.on_shutdown()
+
+        for provider in self.discover.get_all_provider():
+            if isinstance(provider, OnInit):
+                await provider.on_shutdown()
+
+        for controller in self.discover.get_all_controller():
+            if isinstance(controller, OnInit):
+                await controller.on_shutdown()
```

### Comparing `nestipy-0.2.0/src/nestipy/core/interceptor/processor.py` & `nestipy-0.2.1/src/nestipy/core/interceptor/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/meta/metadata_creator.py` & `nestipy-0.2.1/src/nestipy/core/meta/metadata_creator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/meta/module_metadata_creator.py` & `nestipy-0.2.1/src/nestipy/core/meta/module_metadata_creator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/middleware/executor.py` & `nestipy-0.2.1/src/nestipy/core/middleware/executor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/nestipy_application.py` & `nestipy-0.2.1/src/nestipy/core/nestipy_application.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import dataclasses
 import logging
 import os.path
 import traceback
 from typing import Type, Callable, Literal, Union, Any, TYPE_CHECKING
 
+from nestipy_dynamic_module import DynamicModule
+from nestipy_ioc import MiddlewareContainer, MiddlewareProxy, NestipyContainer, ModuleProviderDict
+from nestipy_metadata import ModuleMetadata, Reflect
+from openapidocs.v3 import PathItem
+
 from nestipy.common.http_ import Response, Request
 from nestipy.common.middleware import NestipyMiddleware
 from nestipy.common.template import TemplateEngine, TemplateKey
 from nestipy.common.utils import uniq_list
 from nestipy.core.template import MinimalJinjaTemplateEngine
 from nestipy.graphql.graphql_adapter import GraphqlAdapter
 from nestipy.graphql.strawberry.strawberry_adapter import StrawberryAdapter
-from nestipy_dynamic_module import DynamicModule
-from nestipy_ioc import MiddlewareContainer, MiddlewareProxy, NestipyContainer, ModuleProviderDict
-from nestipy_metadata import ModuleMetadata, Reflect
-from openapidocs.v3 import PathItem
-
 from .adapter.fastapi_adapter import FastApiAdapter
 from .adapter.http_adapter import HttpAdapter
+from .discover import DiscoverService
 from .instance_loader import InstanceLoader
 from .meta.controller_metadata_creator import ControllerMetadataCreator
 from .meta.module_metadata_creator import ModuleMetadataCreator
 from .meta.provider_metadata_creator import ProviderMetadataCreator
 from .router.router_proxy import RouterProxy
 from ..graphql.graphql_proxy import GraphqlProxy
 from ..types_ import NextFn
@@ -78,27 +79,29 @@
             if isinstance(m, DynamicModule):
                 modules.append(m.module)
             else:
                 modules.append(m)
         return uniq_list(modules)
 
     def init(self, root_module: Type):
+        self._root_module = root_module
+        self._add_root_module_provider(DiscoverService, _init=False)
+        self._set_metadata()
 
-        provider_metadata_maker = ProviderMetadataCreator(root_module, is_root=True)
+    def _set_metadata(self):
+        provider_metadata_maker = ProviderMetadataCreator(self._root_module, is_root=True)
         provider_metadata_maker.create()
 
-        controller_metadata_maker = ControllerMetadataCreator(root_module, is_root=True)
+        controller_metadata_maker = ControllerMetadataCreator(self._root_module, is_root=True)
         controller_metadata_maker.create()
 
         # optional
-        module_metadata_maker = ModuleMetadataCreator(root_module)
+        module_metadata_maker = ModuleMetadataCreator(self._root_module)
         module_metadata_maker.create()
 
-        self._root_module = root_module
-
     async def _setup(self):
         try:
             modules = self._get_modules(self._root_module)
             graphql_module_instance = await self.instance_loader.create_instances(modules)
             # create and register route to platform adapter
             self._openapi_paths = self._router_proxy.apply_routes(modules)
             # check if graphql is enabled
@@ -186,20 +189,21 @@
         self._http_adapter.add_global_filters(*filters)
         self._add_root_module_provider(*filters)
 
     def use_global_guards(self, *guards: Union[Type, "CanActivate"]):
         self._http_adapter.add_global_guards(*guards)
         # self._add_root_module_provider(*guards)
 
-    def _add_root_module_provider(self, *providers: Union[ModuleProviderDict, Type]):
+    def _add_root_module_provider(self, *providers: Union[ModuleProviderDict, Type], _init: bool = True):
         root_providers: list = Reflect.get_metadata(self._root_module, ModuleMetadata.Providers, [])
         root_providers = root_providers + list(providers)
         Reflect.set_metadata(self._root_module, ModuleMetadata.Providers, root_providers)
         #  re init setting metadata
-        self.init(self._root_module)
+        if _init:
+            self._set_metadata()
 
     def use_io_adapter(self, io_adapter: IoAdapter):
         # edit root module provider
         # TODO refactor
         NestipyContainer.get_instance().add_singleton_instance(IoAdapter, io_adapter)
         self._add_root_module_provider(ModuleProviderDict(token=IoAdapter, value=io_adapter))
         # setup io adapter to http_adapter
```

### Comparing `nestipy-0.2.0/src/nestipy/core/nestipy_factory.py` & `nestipy-0.2.1/src/nestipy/core/nestipy_factory.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.2.1/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8ea61f66 (Wed Apr 17 10:38:06 2024 UTC)
+moddate:  0x739b2b66 (Fri Apr 26 12:17:55 2024 UTC)
 files sz: 89
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `nestipy-0.2.0/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc` & `nestipy-0.2.1/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc` & `nestipy-0.2.1/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc` & `nestipy-0.2.1/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/router/route_explorer.py` & `nestipy-0.2.1/src/nestipy/core/router/route_explorer.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/router/router_proxy.py` & `nestipy-0.2.1/src/nestipy/core/router/router_proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,16 +83,22 @@
                 json_data = await req.json()
                 context_container.set_value(NestipyContextProperty.body, json_data)
 
             # TODO: req.files
 
             container = NestipyContainer.get_instance()
             controller_method_handler = getattr(controller, method_name)
-            execution_context = ExecutionContext(self.router, module_ref, controller, controller_method_handler, req,
-                                                 res)
+            execution_context = ExecutionContext(
+                self.router,
+                module_ref,
+                controller,
+                controller_method_handler,
+                req,
+                res
+            )
             context_container.set_value(NestipyContextProperty.execution_context, execution_context)
             handler_response: Response
             try:
                 # TODO : Refactor
                 guard_processor: GuardProcessor = await NestipyContainer.get_instance().get(GuardProcessor)
                 can_activate = await guard_processor.process(execution_context)
                 if not can_activate[0]:
```

### Comparing `nestipy-0.2.0/src/nestipy/core/template/minimal_jinja.py` & `nestipy-0.2.1/src/nestipy/core/template/minimal_jinja.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/core/template/processor.py` & `nestipy-0.2.1/src/nestipy/core/template/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/graphql/decorator.py` & `nestipy-0.2.1/src/nestipy/graphql/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/graphql/graphql_adapter.py` & `nestipy-0.2.1/src/nestipy/graphql/graphql_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/graphql/graphql_asgi.py` & `nestipy-0.2.1/src/nestipy/graphql/graphql_asgi.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/graphql/graphql_explorer.py` & `nestipy-0.2.1/src/nestipy/graphql/graphql_explorer.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/graphql/graphql_module.py` & `nestipy-0.2.1/src/nestipy/graphql/graphql_module.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/graphql/graphql_proxy.py` & `nestipy-0.2.1/src/nestipy/graphql/graphql_proxy.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/graphql/playground/graphql-playground-default.html` & `nestipy-0.2.1/src/nestipy/graphql/playground/graphql-playground-default.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/graphql/playground/graphql-playground-graphiql.html` & `nestipy-0.2.1/src/nestipy/graphql/playground/graphql-playground-graphiql.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/graphql/pubsub.py` & `nestipy-0.2.1/src/nestipy/graphql/pubsub.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/graphql/strawberry/__init__.py` & `nestipy-0.2.1/src/nestipy/graphql/strawberry/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/graphql/strawberry/strawberry_adapter.py` & `nestipy-0.2.1/src/nestipy/graphql/strawberry/strawberry_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/graphql/strawberry/strawberry_asgi.py` & `nestipy-0.2.1/src/nestipy/graphql/strawberry/strawberry_asgi.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/openapi/__init__.py` & `nestipy-0.2.1/src/nestipy/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/openapi/decorator.py` & `nestipy-0.2.1/src/nestipy/openapi/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/openapi/document_builder.py` & `nestipy-0.2.1/src/nestipy/openapi/document_builder.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/openapi/swagger.html` & `nestipy-0.2.1/src/nestipy/openapi/swagger.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/openapi/swagger_module.py` & `nestipy-0.2.1/src/nestipy/openapi/swagger_module.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/openapi/test.py` & `nestipy-0.2.1/src/nestipy/openapi/test.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/websocket/adapter.py` & `nestipy-0.2.1/src/nestipy/websocket/adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/websocket/decorator.py` & `nestipy-0.2.1/src/nestipy/websocket/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/src/nestipy/websocket/proxy.py` & `nestipy-0.2.1/src/nestipy/websocket/proxy.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.0/PKG-INFO` & `nestipy-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestipy
-Version: 0.2.0
+Version: 0.2.1
 Summary: Nestipy is a Python framework built on top of BlackSheep that follows the modular architecture of NestJS
 Author: tsiresymila
 Author-email: tsiresymila@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -76,15 +76,15 @@
     ├── README.md
     
        
 ```
 
 ## Documentation
 
-View full documentation from [here](https://nestipy.github.io/nestipy).
+View full documentation from [here](https://nestipy.vercel.app).
 
 ## Support
 
 Nestipy is an MIT-licensed open source project. It can grow thanks to the sponsors and support from the amazing backers.
 If you'd like to join them, please [read more here].
 
 ## Stay in touch
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nestipy Version: 0.2.0 Summary: Nestipy is a Python
+Metadata-Version: 2.1 Name: nestipy Version: 0.2.1 Summary: Nestipy is a Python
 framework built on top of BlackSheep that follows the modular architecture of
 NestJS Author: tsiresymila Author-email: tsiresymila@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Dist: aiofile (>=3.8.8,<4.0.0) Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: autoflake (>=2.3.0,<3.0.0) Requires-Dist: autopep8
@@ -28,12 +28,12 @@
 Under the hood, Nestipy makes use of _F_a_s_t_A_P_I, but also provides compatibility
 with a wide range of other libraries, like _B_l_a_c_k_s_h_e_e_p, allowing for easy use of
 the myriad of third-party plugins which are available.
 ## Getting started ```cmd pip install nestipy-cli nestipy new my_app cd my_app
 python main.py ``` ``` âââ src â âââ __init__.py âââ
 app_module.py âââ app_controller.py âââ app_service.py âââ
 main.py âââ requirements.txt âââ README.md ``` ## Documentation
-View full documentation from [here](https://nestipy.github.io/nestipy). ##
-Support Nestipy is an MIT-licensed open source project. It can grow thanks to
-the sponsors and support from the amazing backers. If you'd like to join them,
+View full documentation from [here](https://nestipy.vercel.app). ## Support
+Nestipy is an MIT-licensed open source project. It can grow thanks to the
+sponsors and support from the amazing backers. If you'd like to join them,
 please [read more here]. ## Stay in touch - Author - [Tsiresy Mila](https://
 tsiresymila.vercel.app) ## License Nestipy is [MIT licensed](LICENSE).
```

