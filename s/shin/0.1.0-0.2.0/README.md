# Comparing `tmp/shin-0.1.0.tar.gz` & `tmp/shin-0.2.0.tar.gz`

## Comparing `shin-0.1.0.tar` & `shin-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0      332 1970-01-01 00:00:00.000000 shin-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     1506 2023-11-03 16:54:04.000000 shin-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     1079 2023-11-03 16:54:04.000000 shin-0.1.0/.github/workflows/test.yml
--rw-r--r--   0     1001      127      334 2023-11-03 16:54:04.000000 shin-0.1.0/.gitignore
--rw-r--r--   0     1001      127      386 2023-11-03 16:54:04.000000 shin-0.1.0/HISTORY.md
--rw-r--r--   0     1001      127     1074 2023-11-03 16:54:04.000000 shin-0.1.0/LICENSE
--rw-r--r--   0     1001      127     5904 2023-11-03 16:54:04.000000 shin-0.1.0/README.md
--rw-r--r--   0     1001      127      653 2023-11-03 16:54:04.000000 shin-0.1.0/pyproject.toml
--rw-r--r--   0     1001      127     2529 2023-11-03 16:54:04.000000 shin-0.1.0/python/shin/__init__.py
--rw-r--r--   0     1001      127       28 2023-11-03 16:54:04.000000 shin-0.1.0/requirements-test.txt
--rw-r--r--   0     1001      127      954 2023-11-03 16:54:04.000000 shin-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127     2557 2023-11-03 16:54:04.000000 shin-0.1.0/tests/test_shin.py
--rw-r--r--   0     1001      127     7181 2023-11-03 16:54:04.000000 shin-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     6453 1970-01-01 00:00:00.000000 shin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      332 1970-01-01 00:00:00.000000 shin-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      127     1606 2024-04-27 06:52:04.000000 shin-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     1139 2024-04-27 06:52:04.000000 shin-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      356 2024-04-27 06:52:04.000000 shin-0.2.0/.gitignore
+-rw-r--r--   0     1001      127      574 2024-04-27 06:52:04.000000 shin-0.2.0/HISTORY.md
+-rw-r--r--   0     1001      127     1074 2024-04-27 06:52:04.000000 shin-0.2.0/LICENSE
+-rw-r--r--   0     1001      127     7949 2024-04-27 06:52:04.000000 shin-0.2.0/README.md
+-rw-r--r--   0     1001      127     1049 2024-04-27 06:52:04.000000 shin-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      127     4841 2024-04-27 06:52:04.000000 shin-0.2.0/python/shin/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-27 06:52:04.000000 shin-0.2.0/python/shin/py.typed
+-rw-r--r--   0     1001      127      194 2024-04-27 06:52:04.000000 shin-0.2.0/python/shin/shin.pyi
+-rw-r--r--   0     1001      127       67 2024-04-27 06:52:04.000000 shin-0.2.0/requirements-test.txt
+-rw-r--r--   0     1001      127      954 2024-04-27 06:52:04.000000 shin-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      127     3141 2024-04-27 06:52:04.000000 shin-0.2.0/tests/test_shin.py
+-rw-r--r--   0     1001      127     2823 2024-04-27 06:52:04.000000 shin-0.2.0/typesafety/test_shin.yml
+-rw-r--r--   0     1001      127     7181 2024-04-27 06:52:04.000000 shin-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     8498 1970-01-01 00:00:00.000000 shin-0.2.0/PKG-INFO
```

### Comparing `shin-0.1.0/.github/workflows/CI.yml` & `shin-0.2.0/.github/workflows/CI.yml`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 
 on:
   push:
   pull_request:
 
 jobs:
   linux:
+    strategy:
+      matrix:
+        target: [x86_64, aarch64]
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - uses: messense/maturin-action@v1
       with:
         manylinux: auto
         command: build
+        target: ${{ matrix.target }}
         args: --release --sdist -o dist --find-interpreter
     - name: Upload wheels
       uses: actions/upload-artifact@v2
       with:
         name: wheels
         path: dist
 
@@ -59,8 +63,8 @@
           name: wheels
       - name: Publish to PyPI
         uses: messense/maturin-action@v1
         env:
           MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
         with:
           command: upload
-          args: --skip-existing *
+          args: --skip-existing *
```

### Comparing `shin-0.1.0/.github/workflows/test.yml` & `shin-0.2.0/.github/workflows/test.yml`

 * *Files 7% similar despite different names*

```diff
@@ -34,8 +34,11 @@
       - name: Install package
         run: python3 -m pip install --user dist/shin*.tar.gz
       - name: Lint with black
         run: |
           black . --check
       - name: Test with pytest
         run: |
-          pytest
+          pytest
+      - name: Test with mypy
+        run: |
+          mypy
```

### Comparing `shin-0.1.0/LICENSE` & `shin-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shin-0.1.0/README.md` & `shin-0.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -33,23 +33,23 @@
 ```python
 import shin
 
 shin.calculate_implied_probabilities([2.6, 2.4, 4.3], full_output=True)
 ```
 
 ```
-{'implied_probabilities': [0.37299406033208965,
-  0.4047794109200184,
-  0.2222265287474275],
- 'iterations': 425,
- 'delta': 9.667822098435863e-13,
- 'z': 0.01694251276407055}
+ShinOptimisationDetails(
+    implied_probabilities=[0.37299406033208965, 0.4047794109200184, 0.2222265287474275],
+    iterations=426,
+    delta=9.667822098435863e-13,
+    z=0.01694251276407055
+)
 ```
 
-The returned `dict` contains the following fields:
+The returned object contains the following fields:
 
 * `implied_probablities`
 * `iterations` - compare this value to the `max_iterations` argument (default = `1000`) to check for failed convergence
 * `delta` - the final change in `z` for the final iteration. Compare with the `convergence_threshold` argument
   (default = `1e-12`) to assess convergence
 * `z` - the estimated proportion of theoretical betting volume coming from insider traders
 
@@ -59,22 +59,68 @@
 ```python
 import shin
 
 shin.calculate_implied_probabilities([1.5, 2.74], full_output=True)
 ```
 
 ```
-{'implied_probabilities': [0.6508515815085157, 0.3491484184914841],
- 'iterations': 0,
- 'delta': 0,
- 'z': 0.03172728540646625}
+ShinOptimisationDetails(
+    implied_probabilities=[0.6508515815085157, 0.3491484184914841],
+    iterations=0.0,
+    delta=0.0,
+    z=0.03172728540646625
+)
 ```
 
 Note that with two outcomes, Shin's method is equivalent to the Additive Method of [[5](#5)].
 
+# What's New in Version 0.2.0?
+
+The latest version improves support for static typing and includes a breaking change.
+
+## Breaking Change To `calculate_implied_probabilities()` Signature
+
+All arguments to `calculate_implied_probabilities()` other than `odds` are now keyword only arguments. This change
+simplified declaration of overloads to support typing the function's return value and will allow for more flexibility
+in the API.
+
+```py
+from shin import calculate_implied_probabilities
+
+# still works
+calculate_implied_probabilities([2.0, 2.0])
+calculate_implied_probabilities(odds=[2.0, 2.0])
+calculate_implied_probabilities([2.0, 2.0], full_output=True)
+## also any other combination of passing arguments as keyword args remains the same
+
+# passing any arg other than `odds` as positional is now an error
+calculate_implied_probabilibies([2.0, 2.0], 1000)  # Error
+calculate_implied_probabilities([2.0, 2.0], max_iterations=1000)  # OK
+
+
+calculate_impolied_probabilities([2.0, 2.0], 1000, 1e-12, True) # Error
+calculate_implied_probabilities([2.0, 2.0], max_iterations=1000, convergence_threshold=1e-12, full_output=True)  # OK
+```
+
+See [this commit](https://github.com/mberk/shin/commit/06a4ce90fc9bb047cef4e70d8a429b69a6cfd181) for more details.
+
+## Full Output Type
+
+The `full_output` argument now returns a `ShinOptimisationDetails` object instead of a `dict`. This object is a
+`dataclass` with the same fields as the `dict` that was previously returned.
+
+For the read-only case, the `ShinOptimisationDetails` object can be used as a drop-in replacement for the `dict` that
+was previously returned as it supports `__getitem__()`.
+
+This change was introduced to support generic typing of the `implied_probabilities`, currently not supported by
+`TypedDict` in versions of Python < 3.11.
+
+See [this](https://github.com/mberk/shin/commit/467d88954d5ca958b6a1b73c9c4af412725b4d4a) and
+[this](https://github.com/mberk/shin/commit/c9b6e42b9d791fa4e4219a993f0dd2524ceaa1b5) for more details.
+
 # What's New in Version 0.1.0?
 
 The latest version introduces some substantial changes and breaking API changes.
 
 ## Default Return Value Behaviour
 
 Previously `shin.calculate_implied_probabilities` would return a `dict` that contained convergence details of the
```

### Comparing `shin-0.1.0/src/lib.rs` & `shin-0.2.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `shin-0.1.0/Cargo.lock` & `shin-0.2.0/Cargo.lock`

 * *Files identical despite different names*

### Comparing `shin-0.1.0/PKG-INFO` & `shin-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shin
-Version: 0.1.0
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
 Summary: Python implementation of Shin's method for calculating implied probabilities from bookmaker odds
@@ -46,23 +46,23 @@
 ```python
 import shin
 
 shin.calculate_implied_probabilities([2.6, 2.4, 4.3], full_output=True)
 ```
 
 ```
-{'implied_probabilities': [0.37299406033208965,
-  0.4047794109200184,
-  0.2222265287474275],
- 'iterations': 425,
- 'delta': 9.667822098435863e-13,
- 'z': 0.01694251276407055}
+ShinOptimisationDetails(
+    implied_probabilities=[0.37299406033208965, 0.4047794109200184, 0.2222265287474275],
+    iterations=426,
+    delta=9.667822098435863e-13,
+    z=0.01694251276407055
+)
 ```
 
-The returned `dict` contains the following fields:
+The returned object contains the following fields:
 
 * `implied_probablities`
 * `iterations` - compare this value to the `max_iterations` argument (default = `1000`) to check for failed convergence
 * `delta` - the final change in `z` for the final iteration. Compare with the `convergence_threshold` argument
   (default = `1e-12`) to assess convergence
 * `z` - the estimated proportion of theoretical betting volume coming from insider traders
 
@@ -72,22 +72,68 @@
 ```python
 import shin
 
 shin.calculate_implied_probabilities([1.5, 2.74], full_output=True)
 ```
 
 ```
-{'implied_probabilities': [0.6508515815085157, 0.3491484184914841],
- 'iterations': 0,
- 'delta': 0,
- 'z': 0.03172728540646625}
+ShinOptimisationDetails(
+    implied_probabilities=[0.6508515815085157, 0.3491484184914841],
+    iterations=0.0,
+    delta=0.0,
+    z=0.03172728540646625
+)
 ```
 
 Note that with two outcomes, Shin's method is equivalent to the Additive Method of [[5](#5)].
 
+# What's New in Version 0.2.0?
+
+The latest version improves support for static typing and includes a breaking change.
+
+## Breaking Change To `calculate_implied_probabilities()` Signature
+
+All arguments to `calculate_implied_probabilities()` other than `odds` are now keyword only arguments. This change
+simplified declaration of overloads to support typing the function's return value and will allow for more flexibility
+in the API.
+
+```py
+from shin import calculate_implied_probabilities
+
+# still works
+calculate_implied_probabilities([2.0, 2.0])
+calculate_implied_probabilities(odds=[2.0, 2.0])
+calculate_implied_probabilities([2.0, 2.0], full_output=True)
+## also any other combination of passing arguments as keyword args remains the same
+
+# passing any arg other than `odds` as positional is now an error
+calculate_implied_probabilibies([2.0, 2.0], 1000)  # Error
+calculate_implied_probabilities([2.0, 2.0], max_iterations=1000)  # OK
+
+
+calculate_impolied_probabilities([2.0, 2.0], 1000, 1e-12, True) # Error
+calculate_implied_probabilities([2.0, 2.0], max_iterations=1000, convergence_threshold=1e-12, full_output=True)  # OK
+```
+
+See [this commit](https://github.com/mberk/shin/commit/06a4ce90fc9bb047cef4e70d8a429b69a6cfd181) for more details.
+
+## Full Output Type
+
+The `full_output` argument now returns a `ShinOptimisationDetails` object instead of a `dict`. This object is a
+`dataclass` with the same fields as the `dict` that was previously returned.
+
+For the read-only case, the `ShinOptimisationDetails` object can be used as a drop-in replacement for the `dict` that
+was previously returned as it supports `__getitem__()`.
+
+This change was introduced to support generic typing of the `implied_probabilities`, currently not supported by
+`TypedDict` in versions of Python < 3.11.
+
+See [this](https://github.com/mberk/shin/commit/467d88954d5ca958b6a1b73c9c4af412725b4d4a) and
+[this](https://github.com/mberk/shin/commit/c9b6e42b9d791fa4e4219a993f0dd2524ceaa1b5) for more details.
+
 # What's New in Version 0.1.0?
 
 The latest version introduces some substantial changes and breaking API changes.
 
 ## Default Return Value Behaviour
 
 Previously `shin.calculate_implied_probabilities` would return a `dict` that contained convergence details of the
```

