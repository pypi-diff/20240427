# Comparing `tmp/bigxml-1.0.0.tar.gz` & `tmp/bigxml-1.0.1.tar.gz`

## Comparing `bigxml-1.0.0.tar` & `bigxml-1.0.1.tar`

### file list

```diff
@@ -1,71 +1,72 @@
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 bigxml-1.0.0/.prettierrc.yaml
--rw-r--r--   0        0        0     8321 2020-02-02 00:00:00.000000 bigxml-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 bigxml-1.0.0/dev-requirements.txt
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 bigxml-1.0.0/tox.ini
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 bigxml-1.0.0/.github/workflows/build.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 bigxml-1.0.0/.vscode/env
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 bigxml-1.0.0/.vscode/extensions.json
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 bigxml-1.0.0/.vscode/launch.json
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 bigxml-1.0.0/.vscode/settings.json
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 bigxml-1.0.0/docs/conftest.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 bigxml-1.0.0/docs/mkdocs.yml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bigxml-1.0.0/docs/src/CNAME
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 bigxml-1.0.0/docs/src/decorators.md
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 bigxml-1.0.0/docs/src/encodings.md
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 bigxml-1.0.0/docs/src/exceptions.md
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 bigxml-1.0.0/docs/src/faq.md
--rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 bigxml-1.0.0/docs/src/handlers.md
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 bigxml-1.0.0/docs/src/index.md
--rw-r--r--   0        0        0     5080 2020-02-02 00:00:00.000000 bigxml-1.0.0/docs/src/namespaces.md
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 bigxml-1.0.0/docs/src/nodes.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 bigxml-1.0.0/docs/src/parser.md
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 bigxml-1.0.0/docs/src/quickstart.md
--rw-r--r--   0        0        0     7773 2020-02-02 00:00:00.000000 bigxml-1.0.0/docs/src/recipes.md
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 bigxml-1.0.0/docs/src/streams.md
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 bigxml-1.0.0/docs/src/typing.md
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 bigxml-1.0.0/docs/src/css/extra.css
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 bigxml-1.0.0/src/bigxml/__init__.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 bigxml-1.0.0/src/bigxml/exceptions.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 bigxml-1.0.0/src/bigxml/handle_mgr.py
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 bigxml-1.0.0/src/bigxml/handler_creator.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 bigxml-1.0.0/src/bigxml/handler_marker.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 bigxml-1.0.0/src/bigxml/marks.py
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 bigxml-1.0.0/src/bigxml/nodes.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bigxml-1.0.0/src/bigxml/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigxml-1.0.0/src/bigxml/py.typed
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 bigxml-1.0.0/src/bigxml/stream.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 bigxml-1.0.0/src/bigxml/typing.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 bigxml-1.0.0/src/bigxml/utils.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 bigxml-1.0.0/stubs/defusedxml/ElementTree.pyi
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 bigxml-1.0.0/stubs/defusedxml/__init__.pyi
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/integration/README.md
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/integration/test_comments.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/integration/test_encodings.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/integration/test_invalid_xml.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/integration/test_maths.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/integration/test_namespaces.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/integration/test_ram_usage.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/integration/test_security.py
--rw-r--r--   0        0        0     9351 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/integration/test_typing.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/integration/test_wikipedia_export.py
--rw-r--r--   0        0        0   118848 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/integration/wikipedia_python_export.xml.xz
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/unit/test_exceptions.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/unit/test_handle_mgr.py
--rw-r--r--   0        0        0    26774 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/unit/test_handler_creator.py
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/unit/test_handler_marker.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/unit/test_marks.py
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/unit/test_nodes_element_attributes.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/unit/test_nodes_element_get_text.py
--rw-r--r--   0        0        0     6070 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/unit/test_parser.py
--rw-r--r--   0        0        0     5869 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/unit/test_stream.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/unit/test_utils_autostart_generator.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/unit/test_utils_extract_namespace_name.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/unit/test_utils_get_mandatory_params.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/unit/test_utils_iter_with_rollback.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 bigxml-1.0.0/tests/unit/test_utils_iterable.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 bigxml-1.0.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 bigxml-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 bigxml-1.0.0/README.md
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 bigxml-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 bigxml-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 bigxml-1.0.1/.prettierrc.yaml
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 bigxml-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 bigxml-1.0.1/dev-requirements.txt
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 bigxml-1.0.1/tox.ini
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 bigxml-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 bigxml-1.0.1/.vscode/env
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 bigxml-1.0.1/.vscode/extensions.json
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 bigxml-1.0.1/.vscode/launch.json
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 bigxml-1.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigxml-1.0.1/docs/__init__.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 bigxml-1.0.1/docs/conftest.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 bigxml-1.0.1/docs/mkdocs.yml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bigxml-1.0.1/docs/src/CNAME
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 bigxml-1.0.1/docs/src/decorators.md
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 bigxml-1.0.1/docs/src/encodings.md
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 bigxml-1.0.1/docs/src/exceptions.md
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 bigxml-1.0.1/docs/src/faq.md
+-rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 bigxml-1.0.1/docs/src/handlers.md
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 bigxml-1.0.1/docs/src/index.md
+-rw-r--r--   0        0        0     5080 2020-02-02 00:00:00.000000 bigxml-1.0.1/docs/src/namespaces.md
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 bigxml-1.0.1/docs/src/nodes.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 bigxml-1.0.1/docs/src/parser.md
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 bigxml-1.0.1/docs/src/quickstart.md
+-rw-r--r--   0        0        0     7773 2020-02-02 00:00:00.000000 bigxml-1.0.1/docs/src/recipes.md
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 bigxml-1.0.1/docs/src/streams.md
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 bigxml-1.0.1/docs/src/typing.md
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 bigxml-1.0.1/docs/src/css/extra.css
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 bigxml-1.0.1/src/bigxml/__init__.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 bigxml-1.0.1/src/bigxml/exceptions.py
+-rw-r--r--   0        0        0     5531 2020-02-02 00:00:00.000000 bigxml-1.0.1/src/bigxml/handle_mgr.py
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 bigxml-1.0.1/src/bigxml/handler_creator.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 bigxml-1.0.1/src/bigxml/handler_marker.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 bigxml-1.0.1/src/bigxml/marks.py
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 bigxml-1.0.1/src/bigxml/nodes.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 bigxml-1.0.1/src/bigxml/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigxml-1.0.1/src/bigxml/py.typed
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 bigxml-1.0.1/src/bigxml/stream.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 bigxml-1.0.1/src/bigxml/typing.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 bigxml-1.0.1/src/bigxml/utils.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 bigxml-1.0.1/stubs/defusedxml/ElementTree.pyi
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 bigxml-1.0.1/stubs/defusedxml/__init__.pyi
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/integration/README.md
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/integration/test_comments.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/integration/test_encodings.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/integration/test_invalid_xml.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/integration/test_maths.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/integration/test_namespaces.py
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/integration/test_ram_usage.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/integration/test_security.py
+-rw-r--r--   0        0        0     9351 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/integration/test_typing.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/integration/test_wikipedia_export.py
+-rw-r--r--   0        0        0   118848 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/integration/wikipedia_python_export.xml.xz
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/unit/test_exceptions.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/unit/test_handle_mgr.py
+-rw-r--r--   0        0        0    26158 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/unit/test_handler_creator.py
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/unit/test_handler_marker.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/unit/test_marks.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/unit/test_nodes_element_attributes.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/unit/test_nodes_element_get_text.py
+-rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/unit/test_parser.py
+-rw-r--r--   0        0        0     5869 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/unit/test_stream.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/unit/test_utils_autostart_generator.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/unit/test_utils_extract_namespace_name.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/unit/test_utils_get_mandatory_params.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/unit/test_utils_iter_with_rollback.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 bigxml-1.0.1/tests/unit/test_utils_iterable.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 bigxml-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 bigxml-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 bigxml-1.0.1/README.md
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bigxml-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 bigxml-1.0.1/PKG-INFO
```

### Comparing `bigxml-1.0.0/CHANGELOG.md` & `bigxml-1.0.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,30 @@
 - Only direct imports from top-level module `bigxml` are considered public API
 - A change that only impacts type hints validation is not considered a breaking change
 - Removing support for a version of Python that is not [officially
   supported][python-versions] anymore is not considered a breaking change
 
 [python-versions]: https://devguide.python.org/versions/#supported-versions
 
+## [1.0.1] - 2024-04-27
+
+[1.0.1]: https://github.com/rogdham/bigxml/compare/v1.0.0...v1.0.1
+
+This is a maintenance release. Internal tooling is being upgraded, featuring support for
+pytest version 8 and formatting of the codebase with ruff.
+
+### :house: Internal
+
+- Change code formatter from black to ruff
+- Fix doctests not being run with other tests
+- Fix coverage report under some versions of PyPy
+- Upgrade dev dependencies
+- Remove pylint, assuming its benefits are provided by the ruff+mypy combo
+- Use trusted publishing for PyPi releases
+
 ## [1.0.0] - 2023-10-21
 
 [1.0.0]: https://github.com/rogdham/bigxml/compare/v0.10.0...v1.0.0
 
 Let's celebrate version 1! :tada: We know that `bigxml` has already been used in
 production for years, but now it's official.
```

### Comparing `bigxml-1.0.0/.github/workflows/build.yml` & `bigxml-1.0.1/.github/workflows/build.yml`

 * *Files 8% similar despite different names*

```diff
@@ -18,78 +18,81 @@
           - "3.10"
           - "3.11"
           - "3.12"
           - "pypy-3.8"
           - "pypy-3.9"
           - "pypy-3.10"
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python ${{ matrix.python }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
       - name: Install dependencies
         run: pip install tox
       - name: Run tests
         run: tox run -e py
 
   tests-misc:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         env:
           - build
           - docs
-          - format
           - lint
           - type
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           # build env: fetch all commits for version computation
           fetch-depth: ${{ matrix.env == 'build' && '0' || '1' }}
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.12"
       - name: Install dependencies
         run: pip install tox
       - name: Run ${{ matrix.env }}
         run: tox run -e ${{ matrix.env }}
       - if: ${{ matrix.env == 'build' || matrix.env  == 'docs' }}
         name: Save ${{ matrix.env }} artifacts
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: ${{ matrix.env }}
           path: dist
 
   publish:
     if: startsWith(github.ref, 'refs/tags')
     needs:
       - tests-py
       - tests-misc
     runs-on: ubuntu-latest
+    environment: publish
+    permissions:
+      id-token: write # This permission is mandatory for trusted publishing
     steps:
       - name: Restore build artifacts
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: build
           path: dist
       - name: Publish to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          password: ${{ secrets.pypi_password }}
+          verbose: true
+          print-hash: true
 
   deploy-docs:
     needs: publish
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Restore build artifacts
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: docs
           path: dist
       - name: Deploy docs
         uses: JamesIves/github-pages-deploy-action@v4
         with:
           branch: gh-pages
```

### Comparing `bigxml-1.0.0/.vscode/settings.json` & `bigxml-1.0.1/.vscode/settings.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7633928571428571%*

 * *Differences: {"'[python]'": "{'editor.codeActionsOnSave': {'source.organizeImports': 'explicit'}, "*

 * *               "'editor.defaultFormatter': 'charliermarsh.ruff'}",*

 * * 'delete': "['python.formatting.provider', 'python.linting.mypyEnabled', "*

 * *           "'python.linting.pylintEnabled']"}*

```diff
@@ -5,16 +5,17 @@
             88
         ],
         "editor.wordWrap": "on",
         "editor.wordWrapColumn": 88
     },
     "[python]": {
         "editor.codeActionsOnSave": {
-            "source.organizeImports": true
-        }
+            "source.organizeImports": "explicit"
+        },
+        "editor.defaultFormatter": "charliermarsh.ruff"
     },
     "[yaml]": {
         "editor.defaultFormatter": "esbenp.prettier-vscode",
         "editor.tabSize": 2
     },
     "editor.detectIndentation": false,
     "editor.formatOnSave": true,
@@ -29,12 +30,9 @@
         ".pytest_cache": true,
         ".ruff_cache": true,
         ".tox": true,
         "env": true
     },
     "files.insertFinalNewline": true,
     "python.envFile": "${workspaceFolder}/.vscode/env",
-    "python.formatting.provider": "black",
-    "python.linting.mypyEnabled": true,
-    "python.linting.pylintEnabled": true,
     "python.testing.pytestEnabled": true
 }
```

### Comparing `bigxml-1.0.0/docs/conftest.py` & `bigxml-1.0.1/docs/conftest.py`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/docs/mkdocs.yml` & `bigxml-1.0.1/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/docs/src/decorators.md` & `bigxml-1.0.1/docs/src/decorators.md`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/docs/src/encodings.md` & `bigxml-1.0.1/docs/src/encodings.md`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/docs/src/exceptions.md` & `bigxml-1.0.1/docs/src/exceptions.md`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/docs/src/faq.md` & `bigxml-1.0.1/docs/src/faq.md`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/docs/src/handlers.md` & `bigxml-1.0.1/docs/src/handlers.md`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/docs/src/index.md` & `bigxml-1.0.1/docs/src/index.md`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/docs/src/namespaces.md` & `bigxml-1.0.1/docs/src/namespaces.md`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/docs/src/nodes.md` & `bigxml-1.0.1/docs/src/nodes.md`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/docs/src/parser.md` & `bigxml-1.0.1/docs/src/parser.md`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/docs/src/quickstart.md` & `bigxml-1.0.1/docs/src/quickstart.md`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/docs/src/recipes.md` & `bigxml-1.0.1/docs/src/recipes.md`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/docs/src/streams.md` & `bigxml-1.0.1/docs/src/streams.md`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/docs/src/typing.md` & `bigxml-1.0.1/docs/src/typing.md`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/docs/src/css/extra.css` & `bigxml-1.0.1/docs/src/css/extra.css`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/src/bigxml/exceptions.py` & `bigxml-1.0.1/src/bigxml/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,11 +20,10 @@
         yield from iterable
     except ParseError as ex:
         raise BigXmlError(str(ex), security=False) from ex
     except DefusedXmlException as ex:
         # defusedxml has usable wording in it's exception's doc
         # except for base DefusedXmlException
         msg = (ex.__doc__ or "").strip()
-        # pylint: disable-next=unidiomatic-typecheck
         if not msg or type(ex) is DefusedXmlException:
             msg = "Invalid XML"
         raise BigXmlError(msg, security=True) from ex
```

### Comparing `bigxml-1.0.0/src/bigxml/handle_mgr.py` & `bigxml-1.0.1/src/bigxml/handle_mgr.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,73 +40,65 @@
     ] = None
 
     # iter_from
 
     @overload
     def iter_from(
         self,
-    ) -> Iterator["Never"]:
-        # we don't have '...' as body in this overload as a workaround
-        # to prevent 'not-an-iterable' error in pylint
-        # see https://github.com/PyCQA/astroid/issues/1015
-        return iter(())
+    ) -> Iterator["Never"]: ...
 
     @overload
     def iter_from(
         self,
         *handlers: Union[
             str,
             List[str],
             Tuple[str, ...],
         ],
-    ) -> Iterator["XMLElement"]:
-        ...
+    ) -> Iterator["XMLElement"]: ...
 
     @overload
     def iter_from(
         self,
         *handlers: Union[
             Callable[[Union["XMLElement", "XMLText"]], Optional[Iterable[T]]],
             ClassHandlerWithCustomWrapper0[T],
             ClassHandlerWithCustomWrapper1[T],
             Type[ClassHandlerWithCustomWrapper0[T]],
             Type[ClassHandlerWithCustomWrapper1[T]],
         ],
-    ) -> Iterator[T]:
-        ...
+    ) -> Iterator[T]: ...
 
     @overload
     def iter_from(
         self,
         *handlers: Union[
             Callable[[Union["XMLElement", "XMLText"]], Optional[Iterable[T]]],
             ClassHandlerWithCustomWrapper0[T],
             ClassHandlerWithCustomWrapper1[T],
             Type[ClassHandlerWithCustomWrapper0[T]],
             Type[ClassHandlerWithCustomWrapper1[T]],
             Type[T],
         ],
-    ) -> Iterator[T]:
-        ...
+    ) -> Iterator[T]: ...
 
     @overload
     def iter_from(
         self,
         *handlers: Union[
             Callable[[Union["XMLElement", "XMLText"]], Optional[Iterable[T]]],
             ClassHandlerWithCustomWrapper0[T],
             ClassHandlerWithCustomWrapper1[T],
             Type[ClassHandlerWithCustomWrapper0[T]],
             Type[ClassHandlerWithCustomWrapper1[T]],
             str,
             List[str],
             Tuple[str, ...],
         ],
-    ) -> Iterator[Union["XMLElement", T]]:
-        ...
+    ) -> Iterator[Union["XMLElement", T]]: ...
 
     @overload
     def iter_from(
         self,
         *handlers: Union[
             Callable[[Union["XMLElement", "XMLText"]], Optional[Iterable[T]]],
             ClassHandlerWithCustomWrapper0[T],
@@ -114,91 +106,84 @@
             Type[ClassHandlerWithCustomWrapper0[T]],
             Type[ClassHandlerWithCustomWrapper1[T]],
             Type[T],
             str,
             List[str],
             Tuple[str, ...],
         ],
-    ) -> Iterator[Union["XMLElement", T]]:
-        ...
+    ) -> Iterator[Union["XMLElement", T]]: ...
 
     @overload  # type: ignore[misc]
     def iter_from(
         self,
         *handlers: Any,  # noqa: ANN401
-    ) -> Iterator[object]:
-        ...
+    ) -> Iterator[object]: ...
 
     def iter_from(self, *handlers: Any) -> Iterator[object]:
         if not self._handle:
             raise RuntimeError("No handle to use")
         handler = create_handler(*handlers)
-        return self._handle(handler)  # pylint: disable=not-callable
+        return self._handle(handler)
 
     # return_from
 
     @overload
     def return_from(
         self,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @overload
     def return_from(
         self,
         *handlers: Union[
             str,
             List[str],
             Tuple[str, ...],
         ],
-    ) -> Optional["XMLElement"]:
-        ...
+    ) -> Optional["XMLElement"]: ...
 
     @overload
     def return_from(
         self,
         *handlers: Union[
             Callable[[Union["XMLElement", "XMLText"]], Optional[Iterable[T]]],
             ClassHandlerWithCustomWrapper0[T],
             ClassHandlerWithCustomWrapper1[T],
             Type[ClassHandlerWithCustomWrapper0[T]],
             Type[ClassHandlerWithCustomWrapper1[T]],
         ],
-    ) -> Optional[T]:
-        ...
+    ) -> Optional[T]: ...
 
     @overload
     def return_from(
         self,
         *handlers: Union[
             Callable[[Union["XMLElement", "XMLText"]], Optional[Iterable[T]]],
             ClassHandlerWithCustomWrapper0[T],
             ClassHandlerWithCustomWrapper1[T],
             Type[ClassHandlerWithCustomWrapper0[T]],
             Type[ClassHandlerWithCustomWrapper1[T]],
             Type[T],
         ],
-    ) -> Optional[T]:
-        ...
+    ) -> Optional[T]: ...
 
     @overload
     def return_from(
         self,
         *handlers: Union[
             Callable[[Union["XMLElement", "XMLText"]], Optional[Iterable[T]]],
             ClassHandlerWithCustomWrapper0[T],
             ClassHandlerWithCustomWrapper1[T],
             Type[ClassHandlerWithCustomWrapper0[T]],
             Type[ClassHandlerWithCustomWrapper1[T]],
             str,
             List[str],
             Tuple[str, ...],
         ],
-    ) -> Optional[Union["XMLElement", T]]:
-        ...
+    ) -> Optional[Union["XMLElement", T]]: ...
 
     @overload
     def return_from(
         self,
         *handlers: Union[
             Callable[[Union["XMLElement", "XMLText"]], Optional[Iterable[T]]],
             ClassHandlerWithCustomWrapper0[T],
@@ -206,19 +191,17 @@
             Type[ClassHandlerWithCustomWrapper0[T]],
             Type[ClassHandlerWithCustomWrapper1[T]],
             str,
             List[str],
             Tuple[str, ...],
             Type[T],
         ],
-    ) -> Optional[Union["XMLElement", T]]:
-        ...
+    ) -> Optional[Union["XMLElement", T]]: ...
 
     @overload
     def return_from(
         self,
         *handlers: object,
-    ) -> Optional[object]:
-        ...
+    ) -> Optional[object]: ...
 
     def return_from(self, *handlers: Any) -> Optional[Any]:
         return last_item_or_none(self.iter_from(*handlers))
```

### Comparing `bigxml-1.0.0/src/bigxml/handler_creator.py` & `bigxml-1.0.1/src/bigxml/handler_creator.py`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/src/bigxml/handler_marker.py` & `bigxml-1.0.1/src/bigxml/handler_marker.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,39 +11,35 @@
 # iter_from and return_from.
 
 # Also, a lot of the typing complexity comes from the fact that
 # decorators can be applied on both functions, methods & staticmethods
 # plus xml_handle_text can be applied without parenthesis as well
 
 
-# pylint: disable-next=invalid-name
 class ___xml_handle_xxx_wrapped(Protocol[T_co]):  # noqa: N801
     # wrapper for classes
     @overload
     def __call__(  # type: ignore[misc]
         self,
         obj: K,
-    ) -> K:
-        ...
+    ) -> K: ...
 
     # wrapper for functions
     @overload
     def __call__(
         self,
         obj: Callable[[T_co], Optional[Iterable[T]]],
-    ) -> Callable[[Union[XMLElement, XMLText]], Optional[Iterable[T]]]:
-        ...
+    ) -> Callable[[Union[XMLElement, XMLText]], Optional[Iterable[T]]]: ...
 
     # wrapper for methods
     @overload
     def __call__(
         self,
         obj: Callable[[U, T_co], Optional[Iterable[T]]],
-    ) -> Callable[[U, Union[XMLElement, XMLText]], Optional[Iterable[T]]]:
-        ...
+    ) -> Callable[[U, Union[XMLElement, XMLText]], Optional[Iterable[T]]]: ...
 
 
 def xml_handle_element(*args: str) -> ___xml_handle_xxx_wrapped[XMLElement]:
     if not args:
         raise TypeError("Call to xml_handle_element without any args")
 
     def wrapper(obj: F) -> F:
@@ -70,30 +66,27 @@
     ...
 
 
 # @xml_handle_text (for functions)
 @overload
 def xml_handle_text(
     obj: Callable[[XMLText], Optional[Iterable[T]]], /
-) -> Callable[[Union[XMLElement, XMLText]], Optional[Iterable[T]]]:
-    ...
+) -> Callable[[Union[XMLElement, XMLText]], Optional[Iterable[T]]]: ...
 
 
 # @xml_handle_text (for methods)
 @overload
 def xml_handle_text(
     obj: Callable[[U, XMLText], Optional[Iterable[T]]], /
-) -> Callable[[U, Union[XMLElement, XMLText]], Optional[Iterable[T]]]:
-    ...
+) -> Callable[[U, Union[XMLElement, XMLText]], Optional[Iterable[T]]]: ...
 
 
 # @xml_handle_text(...) (for functions & methods)
 @overload
-def xml_handle_text(*args: str) -> ___xml_handle_xxx_wrapped[XMLText]:
-    ...
+def xml_handle_text(*args: str) -> ___xml_handle_xxx_wrapped[XMLText]: ...
 
 
 def xml_handle_text(*args: Any) -> Any:
     # @xml_handle_text
     if len(args) == 1 and callable(args[0]):  # https://stackoverflow.com/q/653368
         return xml_handle_element(XMLText.name)(args[0])
```

### Comparing `bigxml-1.0.0/src/bigxml/nodes.py` & `bigxml-1.0.1/src/bigxml/nodes.py`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/src/bigxml/parser.py` & `bigxml-1.0.1/src/bigxml/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,14 @@
             node = XMLText(text=text, parents=parents)
             yield from handler(node)
 
     def create_node(elem: "Element", iteration: int) -> Union[XMLElement, XMLText]:
         node = XMLElement(
             name=elem.tag, attributes=XMLElementAttributes(elem.attrib), parents=parents
         )
-        # pylint: disable=protected-access
         node._handle = lambda h: _parse(  # noqa: SLF001
             iterator, h, (*parents, node), elem, iteration
         )
         return node
 
     for action, elem in iterator:
         if action == "start":
```

### Comparing `bigxml-1.0.0/src/bigxml/stream.py` & `bigxml-1.0.1/src/bigxml/stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     for substream in substreams:
         yield from _flatten_stream(substream)
 
 
 @autostart_generator
 def _convert_to_read(
-    data_stream: Generator[Optional[memoryview], int, None]
+    data_stream: Generator[Optional[memoryview], int, None],
 ) -> Generator[bytes, int, None]:
     size = yield b""
     while True:
         try:
             buffer = data_stream.send(size)
         except StopIteration:
             break
```

### Comparing `bigxml-1.0.0/src/bigxml/typing.py` & `bigxml-1.0.1/src/bigxml/typing.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,35 +13,31 @@
 
 if sys.version_info < (3, 10):  # pragma: no cover
     from typing_extensions import ParamSpec
 else:  # pragma: no cover
     from typing import ParamSpec
 
 
-# pylint: disable=unused-argument
-
-
 P = ParamSpec("P")
 T = TypeVar("T")
 U = TypeVar("U")
 F = TypeVar("F", bound=Callable[..., Any])
 K = TypeVar("K", bound=Type[Any])
 
 T_co = TypeVar("T_co", covariant=True)
 
 
 class SupportsRead(Protocol[T_co]):
-    def read(self, size: Optional[int] = None) -> T_co:
-        ...  # pragma: no cover
+    def read(self, size: Optional[int] = None) -> T_co: ...  # pragma: no cover
 
 
 Streamable = Union[SupportsRead[bytes], bytes, Iterable["Streamable"]]
 
 
 class ClassHandlerWithCustomWrapper0(Protocol[T_co]):
-    def xml_handler(self) -> Optional[Iterable[T_co]]:
-        ...  # pragma: no cover
+    def xml_handler(self) -> Optional[Iterable[T_co]]: ...  # pragma: no cover
 
 
 class ClassHandlerWithCustomWrapper1(Protocol[T_co]):
-    def xml_handler(self, items: Iterator[Any]) -> Optional[Iterable[T_co]]:
-        ...  # pragma: no cover
+    def xml_handler(
+        self, items: Iterator[Any]
+    ) -> Optional[Iterable[T_co]]: ...  # pragma: no cover
```

### Comparing `bigxml-1.0.0/src/bigxml/utils.py` & `bigxml-1.0.1/src/bigxml/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,30 +57,30 @@
     except StopIteration:
         return False
     last_item_or_none(iterator)
     return True
 
 
 def transform_to_iterator(
-    fct: Callable[P, Optional[Iterable[T]]]
+    fct: Callable[P, Optional[Iterable[T]]],
 ) -> Callable[P, Iterator[T]]:
     @wraps(fct)
     def wrapped(*args: P.args, **kwargs: P.kwargs) -> Iterator[T]:
         return_value = fct(*args, **kwargs)
         if return_value is None:
             return iter(())  # empty iterator
         return iter(return_value)
 
     return wrapped
 
 
 def get_mandatory_params(fct: Callable[..., object]) -> Tuple[str, ...]:
     try:
         sig = signature(fct)
-    except (ValueError, TypeError):
+    except (ValueError, TypeError):  # pragma: no cover
         return ()  # e.g. for built-in
     return tuple(
         param.name
         for param in sig.parameters.values()
         if param.kind
         in (
             Parameter.POSITIONAL_ONLY,
@@ -88,15 +88,15 @@
             Parameter.KEYWORD_ONLY,
         )
         and param.default == sig.empty
     )
 
 
 def autostart_generator(
-    fct: Callable[P, Generator[T, U, None]]
+    fct: Callable[P, Generator[T, U, None]],
 ) -> Callable[P, Generator[T, U, None]]:
     @wraps(fct)
     def wrapped(*args: P.args, **kwargs: P.kwargs) -> Generator[T, U, None]:
         generator = fct(*args, **kwargs)
         next(generator)  # ignore first yielded value
         return generator
```

### Comparing `bigxml-1.0.0/stubs/defusedxml/ElementTree.pyi` & `bigxml-1.0.1/stubs/defusedxml/ElementTree.pyi`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/tests/conftest.py` & `bigxml-1.0.1/tests/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from pathlib import Path
 from typing import List
 
 import pytest
 
 
 def pytest_collection_modifyitems(
-    # pylint: disable=unused-argument
     config: pytest.Config,  # noqa: ARG001
     items: List[pytest.Item],
 ) -> None:
     root = Path(__file__).parent.parent
     for item in items:
         relative = Path(item.fspath).parent.relative_to(root)
         if relative.parent.name == "docs":
```

### Comparing `bigxml-1.0.0/tests/integration/test_comments.py` & `bigxml-1.0.1/tests/integration/test_comments.py`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/tests/integration/test_encodings.py` & `bigxml-1.0.1/tests/integration/test_encodings.py`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/tests/integration/test_invalid_xml.py` & `bigxml-1.0.1/tests/integration/test_invalid_xml.py`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/tests/integration/test_maths.py` & `bigxml-1.0.1/tests/integration/test_maths.py`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/tests/integration/test_namespaces.py` & `bigxml-1.0.1/tests/integration/test_namespaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             with pytest.warns(UserWarning):
                 # current implementation uses "first" attribute in that case
                 # but you should not rely on it and specify the namespace to use
                 yield ("bbb", "yyy default", node.attributes["yyy"])
 
         @staticmethod
         def xml_handler(
-            generator: Iterator[Tuple[str, str, str]]
+            generator: Iterator[Tuple[str, str, str]],
         ) -> Iterator[Tuple[str, str, str]]:
             yield from generator
 
     assert list(Parser(XML).iter_from(Handler)) == [
         ("aaa", "https://example.com/xml/", ""),
         ("aaa", "https://example.com/xml/aaa", ""),
         ("aaa_ex", "https://example.com/xml/ex", ""),
```

### Comparing `bigxml-1.0.0/tests/integration/test_ram_usage.py` & `bigxml-1.0.1/tests/integration/test_ram_usage.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from bigxml import Parser, XMLText, xml_handle_text
 
 
 @pytest.fixture
 def ram_usage() -> Iterator[Callable[[], float]]:
     try:
-        import tracemalloc  # pylint: disable=import-outside-toplevel
+        import tracemalloc
     except ImportError:  # e.g. PyPy
         pytest.skip("tracemalloc module not available")
 
     try:
         tracemalloc.start()
         yield lambda: tracemalloc.get_traced_memory()[1]
     finally:
@@ -44,26 +44,24 @@
         else:
             assert ram_used() < ram_limit, "Consumes too much RAM"
 
     yield b"</root>"
 
 
 def test_with_handler(
-    # pylint: disable=redefined-outer-name
     ram_usage: Callable[[], float],
 ) -> None:
     @xml_handle_text("root", "entry", "nb")
     def handler(node: XMLText) -> Iterator[int]:
         yield int(node.text)
 
     items = Parser(big_stream(ram_usage)).iter_from(handler)
 
     for exp, item in enumerate(items):
         assert item == exp
 
 
 def test_no_handler(
-    # pylint: disable=redefined-outer-name
     ram_usage: Callable[[], float],
 ) -> None:
     items: Iterator[object] = Parser(big_stream(ram_usage)).iter_from()
     assert not list(items)
```

### Comparing `bigxml-1.0.0/tests/integration/test_security.py` & `bigxml-1.0.1/tests/integration/test_security.py`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/tests/integration/test_typing.py` & `bigxml-1.0.1/tests/integration/test_typing.py`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/tests/integration/test_wikipedia_export.py` & `bigxml-1.0.1/tests/integration/test_wikipedia_export.py`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/tests/integration/wikipedia_python_export.xml.xz` & `bigxml-1.0.1/tests/integration/wikipedia_python_export.xml.xz`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/tests/unit/test_exceptions.py` & `bigxml-1.0.1/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/tests/unit/test_handle_mgr.py` & `bigxml-1.0.1/tests/unit/test_handle_mgr.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 def handler_c(_node: Union[XMLElement, XMLText]) -> Iterator[object]:
     yield from ()
 
 
 def handle(
-    handler: Callable[[Union[XMLElement, XMLText]], Iterator[int]]
+    handler: Callable[[Union[XMLElement, XMLText]], Iterator[int]],
 ) -> Iterator[int]:
     node = Mock()
     for item in handler(node):
         yield item * 1_000
 
 
 def test_iter_from_no_handle() -> None:
@@ -38,19 +38,19 @@
     hmgr = HandleMgr()
     with pytest.raises(RuntimeError):
         hmgr.return_from(handler_a)
 
 
 def test_iter_from_handle() -> None:
     hmgr = HandleMgr()
-    hmgr._handle = handle  # pylint: disable=protected-access
+    hmgr._handle = handle
     assert list(hmgr.iter_from(handler_a)) == [13_000, 37_000]
     assert list(hmgr.iter_from(handler_b)) == [42_000]
     assert not list(hmgr.iter_from(handler_c))
 
 
 def test_return_from_handle() -> None:
     hmgr = HandleMgr()
-    hmgr._handle = handle  # pylint: disable=protected-access
+    hmgr._handle = handle
     assert hmgr.return_from(handler_a) == 37_000
     assert hmgr.return_from(handler_b) == 42_000
     assert hmgr.return_from(handler_c) is None
```

### Comparing `bigxml-1.0.0/tests/unit/test_handler_creator.py` & `bigxml-1.0.1/tests/unit/test_handler_creator.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,22 +68,21 @@
         def handle(
             handler: Callable[[Union[XMLElement, XMLText]], Iterator[object]],
             children: List[Union[XMLElement, XMLText]],
         ) -> Iterable[object]:
             for child in children:
                 yield from handler(child)
 
-        # pylint: disable=protected-access
         node_parent._handle = partial(handle, children=children)  # type: ignore[assignment]
 
     return nodes
 
 
 def cases(
-    *args: Tuple[Tuple[str, ...], Optional[str], Optional[str]]
+    *args: Tuple[Tuple[str, ...], Optional[str], Optional[str]],
 ) -> pytest.MarkDecorator:
     tests: List["ParameterSet"] = []
     for node_path, expected_text, expected_node_name in args:
         nodes = create_nodes(*node_path)
         if expected_node_name is None:
             assert expected_text is None
             expected_node = None
@@ -111,15 +110,15 @@
                 id=">".join(node_path),
             )
         )
 
     return pytest.mark.parametrize("test_create_handler", tests)
 
 
-TEST_CREATE_HANDLER_TYPE = Callable[..., None]  # pylint: disable=invalid-name
+TEST_CREATE_HANDLER_TYPE = Callable[..., None]
 
 #
 # no handler
 #
 
 
 def test_no_handlers() -> None:
@@ -138,15 +137,15 @@
     (("{foo}a",), "catchall", "{foo}a"),
     (("d0", "d1"), "catchall", "d0"),
     (("d0", "d1", "d2"), "catchall", "d0"),
     ((":text:",), "catchall", ":text:"),
 )
 def test_one_catchall(test_create_handler: TEST_CREATE_HANDLER_TYPE) -> None:
     def catchall(
-        node: Union[XMLElement, XMLText]
+        node: Union[XMLElement, XMLText],
     ) -> Iterator[Tuple[str, Union[XMLElement, XMLText]]]:
         yield ("catchall", node)
 
     test_create_handler(catchall)
 
 
 @cases(
@@ -303,15 +302,15 @@
         @xml_handle_text("t0", "t1")
         @staticmethod
         def handle5(node: XMLText) -> Iterator[Tuple[str, XMLText]]:
             yield ("5", node)
 
         @staticmethod
         def xml_handler(
-            generator: Iterator[Tuple[str, Union[XMLElement, XMLText]]]
+            generator: Iterator[Tuple[str, Union[XMLElement, XMLText]]],
         ) -> Iterator[Tuple[str, Union[XMLElement, XMLText]]]:
             yield from generator
 
     handler = Handler() if instantiate_class else Handler
     test_create_handler(handler)
 
 
@@ -333,15 +332,15 @@
         @xml_handle_element("a")
         @staticmethod
         def handle0(node: XMLElement) -> Iterator[Tuple[str, XMLElement]]:
             yield ("0", node)
 
         @staticmethod
         def xml_handler(
-            generator: Iterator[Tuple[str, XMLElement]]
+            generator: Iterator[Tuple[str, XMLElement]],
         ) -> Iterator[Tuple[str, XMLElement]]:
             yield from generator
 
     handler = Handler() if instantiate_class else Handler
     test_create_handler(handler)
 
 
@@ -367,41 +366,41 @@
         @xml_handle_element("a")
         @staticmethod
         def handle0(node: XMLElement) -> Iterator[Tuple[str, XMLElement]]:
             yield ("0", node)
 
         @staticmethod
         def xml_handler(
-            generator: Iterator[Tuple[str, XMLElement]]
+            generator: Iterator[Tuple[str, XMLElement]],
         ) -> Iterator[Tuple[str, XMLElement]]:
             yield from generator
 
     @xml_handle_element("y1")
     class DeepHandler1:
         @xml_handle_element("a")
         @staticmethod
         def handle1(node: XMLElement) -> Iterator[Tuple[str, XMLElement]]:
             yield ("1", node)
 
         @staticmethod
         def xml_handler(
-            generator: Iterator[Tuple[str, XMLElement]]
+            generator: Iterator[Tuple[str, XMLElement]],
         ) -> Iterator[Tuple[str, XMLElement]]:
             yield from generator
 
     @xml_handle_element("x")
     class Handler:
         deep_handler0 = DeepHandler0()
 
         def __init__(self) -> None:
             self.deep_handler1 = DeepHandler1()
 
         @staticmethod
         def xml_handler(
-            generator: Iterator[Tuple[str, XMLElement]]
+            generator: Iterator[Tuple[str, XMLElement]],
         ) -> Iterator[Tuple[str, XMLElement]]:
             yield from generator
 
     handler = Handler() if instantiate_class else Handler
     test_create_handler(handler)
 
 
@@ -447,16 +446,14 @@
     assert len(items) == 1
     assert isinstance(items[0], Handler)
 
 
 @pytest.mark.parametrize("init_mandatory", [False, True])
 @pytest.mark.parametrize("init_optional", [False, True])
 def test_class_init(init_mandatory: bool, init_optional: bool) -> None:
-    # pylint: disable=too-many-locals
-
     @xml_handle_element("x", "y")
     class HandlerA:
         def __init__(self, node: XMLElement, answer: int = 42) -> None:
             self.seen: List[XMLElement] = []
             self.root = node
             self.answer = answer
 
@@ -489,36 +486,34 @@
         def __init__(self) -> None:
             self.seen: List[XMLElement] = []
 
         @xml_handle_element("a", "b")
         def handle0(self, node: XMLElement) -> None:
             self.seen.append(node)
 
-    Handler: Type[object]  # noqa: N806 # pylint: disable=invalid-name
+    Handler: Type[object]  # noqa: N806
     if init_mandatory:
         Handler = HandlerA if init_optional else HandlerB  # noqa: N806
     else:
         Handler = HandlerC if init_optional else HandlerD  # noqa: N806
 
     #   x -> y0 -> a0 -> b0
     #                 -> b1
     #           -> a1 -> b2
     #     -> y1 -> a2 -> b3
     #
     # Handler should be instantiated on y0 and y1
     #
     # the use of namespaces below is to avoid e.g. node_y0==node_y1
     #
-    # pylint: disable=unbalanced-tuple-unpacking
     node_x, node_y0 = create_nodes("x", "{y0}y")
     _, node_a0, node_b0 = create_nodes("{a0}a", "{b0}b", parent=node_y0)
     _, node_b1 = create_nodes("{b1}b", parent=node_a0)
     _, _, node_b2 = create_nodes("{a1}a", "{b2}b", parent=node_y0)
     _, node_y1, _, node_b3 = create_nodes("{y1}y", "{a2}a", "{b3}b", parent=node_x)
-    # pylint: enable=unbalanced-tuple-unpacking
 
     handler = create_handler(Handler)
     items: List[Any] = list(handler(node_x))
     assert all(isinstance(item, Handler) for item in items)
     assert len(items) == 2
     assert items[0].seen == [node_b0, node_b1, node_b2]
     assert items[1].seen == [node_b3]
@@ -540,18 +535,16 @@
 
         @xml_handle_text
         def handle0(self, node: XMLText) -> None:
             self.node = node
 
     #   x -> y0 -> :text:
     #     -> y1 -> z
-    # pylint: disable=unbalanced-tuple-unpacking
     node_x, _, node_txt0 = create_nodes("x", "y0", ":text:")
     _, node_y1, node_txt1 = create_nodes("y1", ":text:", parent=node_x)
-    # pylint: enable=unbalanced-tuple-unpacking
 
     handler = create_handler(Handler)
     items: List[Any] = list(handler(node_x))
     assert all(isinstance(item, Handler) for item in items)
     assert len(items) == 2
     assert items[0].root == node_txt0
     assert items[0].node is None
@@ -623,18 +616,16 @@
 
         def xml_handler(self) -> Iterator[Tuple[str, Optional[XMLElement]]]:
             yield ("start", None)
             for txt, node in self.nodes:
                 yield (f"_{txt}", node)
             yield ("end", None)
 
-    # pylint: disable=unbalanced-tuple-unpacking
     node_x, node_a = create_nodes("x", "a")
     _, node_b = create_nodes("b", parent=node_x)
-    # pylint: enable=unbalanced-tuple-unpacking
 
     handler = create_handler(Handler)
     assert list(handler(node_x)) == [
         ("start", None),
         ("_x", node_a),
         ("_y", node_b),
         ("end", None),
@@ -701,18 +692,16 @@
                 yield (f"oops{txt}", node)
             for txt, node in generator:
                 yield (f"h{txt}", node)
             for txt, node in self.nodes:
                 yield (f"_{txt}", node)
             yield ("end", None)
 
-    # pylint: disable=unbalanced-tuple-unpacking
     node_x, node_a = create_nodes("x", "a")
     _, node_b = create_nodes("b", parent=node_x)
-    # pylint: enable=unbalanced-tuple-unpacking
 
     handler = create_handler(Handler)
     assert list(handler(node_x)) == [
         ("start", None),
         ("h0", node_a),
         ("h1", node_b),
         ("_x", node_a),
@@ -732,25 +721,23 @@
         @xml_handle_element("b")
         @staticmethod
         def handle1(node: XMLElement) -> Iterable[Tuple[str, XMLElement]]:
             yield ("1", node)
 
         @staticmethod
         def xml_handler(
-            generator: Iterable[Tuple[str, XMLElement]]
+            generator: Iterable[Tuple[str, XMLElement]],
         ) -> Iterable[Tuple[str, Optional[XMLElement]]]:
             yield ("start", None)
             for txt, node in generator:
                 yield (f"h{txt}", node)
             yield ("end", None)
 
-    # pylint: disable=unbalanced-tuple-unpacking
     node_x, node_a = create_nodes("x", "a")
     _, node_b = create_nodes("b", parent=node_x)
-    # pylint: enable=unbalanced-tuple-unpacking
 
     handler = create_handler(Handler)
     assert list(handler(node_x)) == [
         ("start", None),
         ("h0", node_a),
         ("h1", node_b),
         ("end", None),
@@ -822,20 +809,20 @@
 # Invalid handler
 #
 
 
 def test_catchall_handler_not_alone() -> None:
     @xml_handle_element("a")
     def handle(
-        node: Union[XMLElement, XMLText]
+        node: Union[XMLElement, XMLText],
     ) -> Iterator[Tuple[str, Union[XMLElement, XMLText]]]:
         yield ("0", node)
 
     def catchall(
-        node: Union[XMLElement, XMLText]
+        node: Union[XMLElement, XMLText],
     ) -> Iterator[Tuple[str, Union[XMLElement, XMLText]]]:
         yield ("1", node)
 
     # ok alone
     create_handler(handle)
     create_handler(catchall)
 
@@ -846,38 +833,38 @@
     with pytest.raises(TypeError) as exc_info:
         create_handler(catchall, handle)
     assert str(exc_info.value).startswith("(): catchall handler exists: <function ")
 
 
 def test_several_catchall_handlers() -> None:
     def catchall0(
-        node: Union[XMLElement, XMLText]
+        node: Union[XMLElement, XMLText],
     ) -> Iterator[Tuple[str, Union[XMLElement, XMLText]]]:
         yield ("0", node)
 
     def catchall1(
-        node: Union[XMLElement, XMLText]
+        node: Union[XMLElement, XMLText],
     ) -> Iterator[Tuple[str, Union[XMLElement, XMLText]]]:
         yield ("1", node)
 
     with pytest.raises(TypeError) as exc_info:
         create_handler(catchall0, catchall1)
     assert str(exc_info.value).startswith("(): catchall handler exists: <function ")
 
 
 def test_concurrent_handlers() -> None:
     @xml_handle_element("a", "b", "c")
     def handle0(
-        node: Union[XMLElement, XMLText]
+        node: Union[XMLElement, XMLText],
     ) -> Iterator[Tuple[str, Union[XMLElement, XMLText]]]:
         yield ("0", node)
 
     @xml_handle_element("a", "b", "c")
     def handle1(
-        node: Union[XMLElement, XMLText]
+        node: Union[XMLElement, XMLText],
     ) -> Iterator[Tuple[str, Union[XMLElement, XMLText]]]:
         yield ("0", node)
 
     with pytest.raises(TypeError) as exc_info:
         create_handler(handle0, handle1)
     assert str(exc_info.value).startswith(
         "('a', 'b', 'c'): catchall handler exists: <function "
```

### Comparing `bigxml-1.0.0/tests/unit/test_handler_marker.py` & `bigxml-1.0.1/tests/unit/test_handler_marker.py`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/tests/unit/test_marks.py` & `bigxml-1.0.1/tests/unit/test_marks.py`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/tests/unit/test_nodes_element_attributes.py` & `bigxml-1.0.1/tests/unit/test_nodes_element_attributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,19 +70,19 @@
 
 def test_len() -> None:
     assert len(XML_ELEMENT_ATTRIBUTES) == 13
 
 
 def test_eq() -> None:
     i = XMLElementAttributes({"foo": "bar"})
-    assert i == i  # noqa: PLR0124 # pylint: disable=comparison-with-itself
+    assert i == i  # noqa: PLR0124
     assert i == XMLElementAttributes(i)
 
     j = XMLElementAttributes({"{}foo": "bar"})
-    assert j == j  # noqa: PLR0124 # pylint: disable=comparison-with-itself
+    assert j == j  # noqa: PLR0124
     assert j == XMLElementAttributes(j)
 
     assert i == j
     assert XMLElementAttributes(i) == j
     assert i == XMLElementAttributes(j)
     assert XMLElementAttributes(i) == XMLElementAttributes(j)
```

### Comparing `bigxml-1.0.0/tests/unit/test_nodes_element_get_text.py` & `bigxml-1.0.1/tests/unit/test_nodes_element_get_text.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 def create_element(*children: Union[XMLElement, XMLText]) -> XMLElement:
     node = XMLElement("foo", Mock(), ())  # don't care about parents
     handle = Mock()
 
     def side_effect(
         handler: Callable[
             [Union[XMLElement, XMLText]], Iterator[Union[XMLElement, XMLText]]
-        ]
+        ],
     ) -> Iterator[Union[XMLElement, XMLText]]:
         for child in children:
             yield from handler(child)
 
     handle.side_effect = side_effect
-    node._handle = handle  # pylint: disable=protected-access
+    node._handle = handle
     return node
 
 
 @pytest.mark.parametrize("text", ["abc", "  \n  abc \n  "])
 def test_element_get_text_direct(text: str) -> None:
     node = create_element(create_text(text))
     assert node.text == "abc"
```

### Comparing `bigxml-1.0.0/tests/unit/test_parser.py` & `bigxml-1.0.1/tests/unit/test_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 
 import pytest
 
 from bigxml.handler_marker import xml_handle_element
 from bigxml.nodes import XMLElement, XMLElementAttributes, XMLText
 from bigxml.parser import Parser
 
-HANDLER_TYPE = Callable[  # pylint: disable=invalid-name
+HANDLER_TYPE = Callable[
     [Union[XMLElement, XMLText]],
     Iterator[Tuple[str, Union[XMLElement, XMLText]]],
 ]
 
 
 @pytest.fixture
 def handler() -> HANDLER_TYPE:
     return_values = count()
 
     def handler_fct(
-        node: Union[XMLElement, XMLText]
+        node: Union[XMLElement, XMLText],
     ) -> Iterator[Tuple[str, Union[XMLElement, XMLText]]]:
         yield (f"handler-yield-{next(return_values)}", node)
 
     return handler_fct
 
 
 def elem(
@@ -60,15 +60,14 @@
         ),
     ],
     ids=["self-closing", "empty", "with text", "with children", "attributes", "xmlns"],
 )
 def test_root_level(
     xml: bytes,
     node: XMLElement,
-    # pylint: disable=redefined-outer-name
     handler: Callable[
         [Union[XMLElement, XMLText]],
         Iterator[Tuple[str, Union[XMLElement, XMLText]]],
     ],
 ) -> None:
     parser = Parser(xml)
     assert list(parser.iter_from(handler)) == [
@@ -130,15 +129,14 @@
         "depth",
         "big texts",
     ],
 )
 def test_content(
     xml_content: bytes,
     nodes: List[Union[XMLElement, XMLText]],
-    # pylint: disable=redefined-outer-name
     handler: HANDLER_TYPE,
 ) -> None:
     @xml_handle_element("root")
     def root_handler(
         node: XMLElement,
     ) -> Iterator[Tuple[str, Union[XMLElement, XMLText]]]:
         yield from node.iter_from(handler)
@@ -160,19 +158,18 @@
 
     parser = Parser(b"<root><foo>hello</foo><foo>world</foo><foo>!</foo></root>")
     nodes = parser.iter_from(root_handler)
     first_node = next(nodes)
     second_node = next(nodes)
     assert second_node.text == "world"
     with pytest.raises(RuntimeError):
-        first_node.text  # pylint: disable=pointless-statement  # noqa: B018
+        first_node.text  # noqa: B018
 
 
 def test_many_small_streams(
-    # pylint: disable=redefined-outer-name
     handler: HANDLER_TYPE,
 ) -> None:
     xml = b"<root>Hello<foo />World</root>"
     xml_parts = [bytes([v]) for v in xml]  # characters one by one
     assert len(xml_parts) == 30
 
     nodes = [text_h_node, elem_f_node, text_w_node]
@@ -186,15 +183,14 @@
     parser = Parser(*xml_parts)
     assert list(parser.iter_from(root_handler)) == [
         (f"handler-yield-{i}", node) for i, node in enumerate(nodes)
     ]
 
 
 def test_insecurely_allow_entities(
-    # pylint: disable=redefined-outer-name
     handler: HANDLER_TYPE,
 ) -> None:
     xml = b'<!DOCTYPE root [<!ENTITY pi "&#960;">]><root>&pi;</root>'
 
     @xml_handle_element("root")
     def root_handler(
         node: XMLElement,
```

### Comparing `bigxml-1.0.0/tests/unit/test_stream.py` & `bigxml-1.0.1/tests/unit/test_stream.py`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/tests/unit/test_utils_autostart_generator.py` & `bigxml-1.0.1/tests/unit/test_utils_autostart_generator.py`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/tests/unit/test_utils_get_mandatory_params.py` & `bigxml-1.0.1/tests/unit/test_utils_get_mandatory_params.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=unused-argument
 # ruff: noqa: ARG001
 
 from typing import Callable, List, Tuple
 
 import pytest
 
 from bigxml.utils import get_mandatory_params
@@ -24,15 +23,14 @@
     pass  # for tests
 
 
 def fct4(arg0, /, arg1, *, arg2, arg3=3):  # type: ignore[no-untyped-def] # noqa: ANN001,ANN201
     pass  # for tests
 
 
-# pylint: disable-next=line-too-long
 def fct5(arg0, /, arg1, *arg2, arg3, arg4=4, **arg5):  # type: ignore[no-untyped-def] # noqa: ANN001,ANN002,ANN003,ANN201
     pass  # for tests
 
 
 def fct6(
     arg0: int,
     /,
@@ -41,17 +39,14 @@
     arg3: int,
     arg4: int = 4,
     **arg5: List[int],
 ) -> None:
     pass  # for tests
 
 
-# pylint: enable=unused-argument
-
-
 @pytest.mark.parametrize(
     ["fct", "expected"],
     [
         (fct0, ()),
         (fct1, ("arg0",)),
         (fct2, ("arg0", "arg1", "arg2")),
         (fct3, ()),
```

### Comparing `bigxml-1.0.0/tests/unit/test_utils_iter_with_rollback.py` & `bigxml-1.0.1/tests/unit/test_utils_iter_with_rollback.py`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/tests/unit/test_utils_iterable.py` & `bigxml-1.0.1/tests/unit/test_utils_iterable.py`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/LICENSE.txt` & `bigxml-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/README.md` & `bigxml-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `bigxml-1.0.0/pyproject.toml` & `bigxml-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -113,75 +113,61 @@
 show_error_context = true
 show_error_codes = true
 # Miscellaneous
 warn_unused_configs = true
 
 
 #
-# pylint
-#
-
-[tool.pylint.DESIGN]
-max-branches = 15
-
-[tool.pylint.'MESSAGE CONTROL']
-disable = [
-    "missing-class-docstring",
-    "missing-function-docstring",
-    "missing-module-docstring",
-    "too-few-public-methods",
-]
-
-
-#
 # pytest
 #
 
 [tool.pytest.ini_options]
-addopts = [
-    "--cov",
-    "--doctest-glob='*.md'",
-    "--doctest-modules",
-    "--strict-markers",
-]
+addopts = """
+    --cov
+    --doctest-glob='*.md'
+    --doctest-modules --strict-markers
+    """
 doctest_optionflags = ["ELLIPSIS", "NORMALIZE_WHITESPACE", "NUMBER"]
 filterwarnings = ["error"]
 markers = ["docs", "integration", "unit"]
 testpaths = ["docs", "tests"]
 
 
 #
 # ruff
 #
 
 [tool.ruff]
-select = ["ALL"]
 src = ["src"]
 target-version = "py38"
+
+[tool.ruff.lint]
+select = ["ALL"]
 ignore = [
     "ANN101",
     "ANN102",
     "C901",
     "COM812",
     "D",
     "E501",
     "EM",
     "ERA001",
     "FA100",
+    "ISC001",
     "PLR0912",
     "TRY003",
     "TRY301",
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "docs/**" = ["D", "INP001", "PTH109"]
 "stubs/**" = ["D"]
 "tests/**" = ["D", "FBT", "INP001", "PLR2004", "S101", "SLF001"]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 force-sort-within-sections = true
 known-first-party = ["bigxml"]
 
-[tool.ruff.flake8-pytest-style]
+[tool.ruff.lint.flake8-pytest-style]
 fixture-parentheses = false
 mark-parentheses = false
 parametrize-names-type = "list"
```

### Comparing `bigxml-1.0.0/PKG-INFO` & `bigxml-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: bigxml
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pythonic xml parser to handle big files or streams
 Project-URL: Homepage, https://github.com/rogdham/bigxml
 Project-URL: Documentation, https://bigxml.rogdham.net/
 Project-URL: Source, https://github.com/rogdham/bigxml
 Author-email: Rogdham <contact@rogdham.net>
 License: The MIT License (MIT)
```

