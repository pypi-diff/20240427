# Comparing `tmp/qs_codec-0.1.2.tar.gz` & `tmp/qs_codec-0.1.3.tar.gz`

## Comparing `qs_codec-0.1.2.tar` & `qs_codec-0.1.3.tar`

### file list

```diff
@@ -1,36 +1,43 @@
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qs_codec-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 qs_codec-0.1.2/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qs_codec-0.1.2/requirements_dev.txt
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/__init__.py
--rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/decode.py
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/encode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/enums/__init__.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/enums/charset.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/enums/duplicates.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/enums/format.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/enums/list_format.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/enums/sentinel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/models/__init__.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/models/decode_options.py
--rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/models/encode_options.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/models/undefined.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/models/weak_wrapper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/utils/__init__.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/utils/decode_utils.py
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/utils/encode_utils.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/utils/str_utils.py
--rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 qs_codec-0.1.2/src/qs_codec/utils/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.2/tests/e2e/__init__.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 qs_codec-0.1.2/tests/e2e/e2e_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.2/tests/unit/__init__.py
--rw-r--r--   0        0        0    29989 2020-02-02 00:00:00.000000 qs_codec-0.1.2/tests/unit/decode_test.py
--rw-r--r--   0        0        0    50930 2020-02-02 00:00:00.000000 qs_codec-0.1.2/tests/unit/encode_test.py
--rw-r--r--   0        0        0    21897 2020-02-02 00:00:00.000000 qs_codec-0.1.2/tests/unit/example_test.py
--rw-r--r--   0        0        0    14896 2020-02-02 00:00:00.000000 qs_codec-0.1.2/tests/unit/utils_test.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 qs_codec-0.1.2/tests/unit/weakref_test.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 qs_codec-0.1.2/.gitignore
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 qs_codec-0.1.2/LICENSE
--rw-r--r--   0        0        0    24736 2020-02-02 00:00:00.000000 qs_codec-0.1.2/README.md
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 qs_codec-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    26141 2020-02-02 00:00:00.000000 qs_codec-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 qs_codec-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 qs_codec-0.1.3/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qs_codec-0.1.3/requirements_dev.txt
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/__init__.py
+-rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/decode.py
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/encode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/enums/__init__.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/enums/charset.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/enums/duplicates.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/enums/format.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/enums/list_format.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/enums/sentinel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/models/__init__.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/models/decode_options.py
+-rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/models/encode_options.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/models/undefined.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/models/weak_wrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/utils/__init__.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/utils/decode_utils.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/utils/encode_utils.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/utils/str_utils.py
+-rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 qs_codec-0.1.3/src/qs_codec/utils/utils.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 qs_codec-0.1.3/tests/comparison/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.3/tests/comparison/__init__.py
+-rwxr-xr-x   0        0        0      408 2020-02-02 00:00:00.000000 qs_codec-0.1.3/tests/comparison/compare_outputs.sh
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 qs_codec-0.1.3/tests/comparison/package.json
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 qs_codec-0.1.3/tests/comparison/qs.js
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 qs_codec-0.1.3/tests/comparison/qs.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 qs_codec-0.1.3/tests/comparison/test_cases.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.3/tests/e2e/__init__.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 qs_codec-0.1.3/tests/e2e/e2e_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.1.3/tests/unit/__init__.py
+-rw-r--r--   0        0        0    29989 2020-02-02 00:00:00.000000 qs_codec-0.1.3/tests/unit/decode_test.py
+-rw-r--r--   0        0        0    50930 2020-02-02 00:00:00.000000 qs_codec-0.1.3/tests/unit/encode_test.py
+-rw-r--r--   0        0        0    22214 2020-02-02 00:00:00.000000 qs_codec-0.1.3/tests/unit/example_test.py
+-rw-r--r--   0        0        0    14896 2020-02-02 00:00:00.000000 qs_codec-0.1.3/tests/unit/utils_test.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 qs_codec-0.1.3/tests/unit/weakref_test.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 qs_codec-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 qs_codec-0.1.3/LICENSE
+-rw-r--r--   0        0        0    24693 2020-02-02 00:00:00.000000 qs_codec-0.1.3/README.md
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 qs_codec-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    26098 2020-02-02 00:00:00.000000 qs_codec-0.1.3/PKG-INFO
```

### Comparing `qs_codec-0.1.2/CODE-OF-CONDUCT.md` & `qs_codec-0.1.3/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/src/qs_codec/decode.py` & `qs_codec-0.1.3/src/qs_codec/decode.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/src/qs_codec/encode.py` & `qs_codec-0.1.3/src/qs_codec/encode.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/src/qs_codec/enums/format.py` & `qs_codec-0.1.3/src/qs_codec/enums/format.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/src/qs_codec/enums/list_format.py` & `qs_codec-0.1.3/src/qs_codec/enums/list_format.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/src/qs_codec/enums/sentinel.py` & `qs_codec-0.1.3/src/qs_codec/enums/sentinel.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/src/qs_codec/models/decode_options.py` & `qs_codec-0.1.3/src/qs_codec/models/decode_options.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/src/qs_codec/models/encode_options.py` & `qs_codec-0.1.3/src/qs_codec/models/encode_options.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/src/qs_codec/models/weak_wrapper.py` & `qs_codec-0.1.3/src/qs_codec/models/weak_wrapper.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/src/qs_codec/utils/decode_utils.py` & `qs_codec-0.1.3/src/qs_codec/utils/decode_utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/src/qs_codec/utils/encode_utils.py` & `qs_codec-0.1.3/src/qs_codec/utils/encode_utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/src/qs_codec/utils/str_utils.py` & `qs_codec-0.1.3/src/qs_codec/utils/str_utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/src/qs_codec/utils/utils.py` & `qs_codec-0.1.3/src/qs_codec/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/tests/e2e/e2e_test.py` & `qs_codec-0.1.3/tests/e2e/e2e_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/tests/unit/decode_test.py` & `qs_codec-0.1.3/tests/unit/decode_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/tests/unit/encode_test.py` & `qs_codec-0.1.3/tests/unit/encode_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/tests/unit/example_test.py` & `qs_codec-0.1.3/tests/unit/example_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,17 @@
         assert qs_codec.decode("a%5Bb%5D=c") == {"a": {"b": "c"}}
 
         # You can also nest your `dict`s, like 'foo[bar][baz]=foobarbaz':
         assert qs_codec.decode("foo[bar][baz]=foobarbaz") == {"foo": {"bar": {"baz": "foobarbaz"}}}
 
         # By default, when nesting `dict`s qs_codec will only decode up to 5 children deep. This means if you attempt to
         # decode a string like 'a[b][c][d][e][f][g][h][i]=j' your resulting `dict` will be:
-        assert qs_codec.decode("a[b][c][d][e][f][g][h][i]=j") == {"a": {"b": {"c": {"d": {"e": {"f": {"[g][h][i]": "j"}}}}}}}
+        assert qs_codec.decode("a[b][c][d][e][f][g][h][i]=j") == {
+            "a": {"b": {"c": {"d": {"e": {"f": {"[g][h][i]": "j"}}}}}}
+        }
 
         # This depth can be overridden by passing a depth option to `DecodeOptions.depth`:
         assert qs_codec.decode("a[b][c][d][e][f][g][h][i]=j", qs_codec.DecodeOptions(depth=1)) == {
             "a": {"b": {"[c][d][e][f][g][h][i]": "j"}}
         }
 
         # The depth limit helps mitigate abuse when **qs_codec** is used to parse user input, and it is recommended to keep
@@ -57,23 +59,30 @@
         # **Note:** it implies `DecodeOptions.allow_dots`, so `decode` will error if you set
         # `DecodeOptions.decode_dot_in_keys` to `True`, and `DecodeOptions.allow_dots` to `False`.
         assert qs_codec.decode(
             "name%252Eobj.first=John&name%252Eobj.last=Doe", qs_codec.DecodeOptions(decode_dot_in_keys=True)
         ) == {"name.obj": {"first": "John", "last": "Doe"}}
 
         # Option `DecodeOptions.allow_empty_lists` can be used to allowing empty `list` values in `dict`
-        assert qs_codec.decode("foo[]&bar=baz", qs_codec.DecodeOptions(allow_empty_lists=True)) == {"foo": [], "bar": "baz"}
+        assert qs_codec.decode("foo[]&bar=baz", qs_codec.DecodeOptions(allow_empty_lists=True)) == {
+            "foo": [],
+            "bar": "baz",
+        }
 
         # Option `DecodeOptions.duplicates` can be used to change the behavior when duplicate keys are encountered
         assert qs_codec.decode("foo=bar&foo=baz") == {"foo": ["bar", "baz"]}
         assert qs_codec.decode("foo=bar&foo=baz", qs_codec.DecodeOptions(duplicates=qs_codec.Duplicates.COMBINE)) == {
             "foo": ["bar", "baz"]
         }
-        assert qs_codec.decode("foo=bar&foo=baz", qs_codec.DecodeOptions(duplicates=qs_codec.Duplicates.FIRST)) == {"foo": "bar"}
-        assert qs_codec.decode("foo=bar&foo=baz", qs_codec.DecodeOptions(duplicates=qs_codec.Duplicates.LAST)) == {"foo": "baz"}
+        assert qs_codec.decode("foo=bar&foo=baz", qs_codec.DecodeOptions(duplicates=qs_codec.Duplicates.FIRST)) == {
+            "foo": "bar"
+        }
+        assert qs_codec.decode("foo=bar&foo=baz", qs_codec.DecodeOptions(duplicates=qs_codec.Duplicates.LAST)) == {
+            "foo": "baz"
+        }
 
         # If you have to deal with legacy browsers or services, there's also support for decoding percent-encoded octets
         # as `Charset.LATIN1`:
         assert qs_codec.decode("a=%A7", qs_codec.DecodeOptions(charset=qs_codec.Charset.LATIN1)) == {"a": "§"}
 
         # Some services add an initial `utf8=✓` value to forms so that old Internet Explorer versions are more likely to
         # submit the form as utf-8. Additionally, the server can check the value against wrong encodings of the
@@ -148,16 +157,18 @@
         assert qs_codec.encode({"a": {"b": "c"}}) == "a%5Bb%5D=c"
 
         # This encoding can be disabled by setting the `EncodeOptions.encode` option to `False`:
         assert qs_codec.encode({"a": {"b": "c"}}, qs_codec.EncodeOptions(encode=False)) == "a[b]=c"
 
         # Encoding can be disabled for keys by setting the `EncodeOptions.encode_values_only` option to `True`:
         assert (
-                qs_codec.encode({"a": "b", "c": ["d", "e=f"], "f": [["g"], ["h"]]}, qs_codec.EncodeOptions(encode_values_only=True))
-                == "a=b&c[0]=d&c[1]=e%3Df&f[0][0]=g&f[1][0]=h"
+            qs_codec.encode(
+                {"a": "b", "c": ["d", "e=f"], "f": [["g"], ["h"]]}, qs_codec.EncodeOptions(encode_values_only=True)
+            )
+            == "a=b&c[0]=d&c[1]=e%3Df&f[0][0]=g&f[1][0]=h"
         )
 
         # This encoding can also be replaced by a custom `Encoder` set as `EncodeOptions.encoder` option:
         # (Note: the `EncodeOptions.encoder` option does not apply if `EncodeOptions.encode` is `False`)
         def custom_encoder(value: str, charset: t.Optional[qs_codec.Charset], format: t.Optional[qs_codec.Format]):
             if value == "č":
                 return "c"
@@ -177,56 +188,71 @@
 
         # When `list`s are encoded, they follow the `EncodeOptions.list_format` option, which defaults to
         # `ListFormat.INDICES`:
         assert qs_codec.encode({"a": ["b", "c", "d"]}, qs_codec.EncodeOptions(encode=False)) == "a[0]=b&a[1]=c&a[2]=d"
 
         # You may use the `EncodeOptions.list_format` option to specify the format of the output `list`:
         assert (
-                qs_codec.encode({"a": ["b", "c"]}, qs_codec.EncodeOptions(encode=False, list_format=qs_codec.ListFormat.INDICES))
-                == "a[0]=b&a[1]=c"
+            qs_codec.encode(
+                {"a": ["b", "c"]}, qs_codec.EncodeOptions(encode=False, list_format=qs_codec.ListFormat.INDICES)
+            )
+            == "a[0]=b&a[1]=c"
+        )
+        assert (
+            qs_codec.encode(
+                {"a": ["b", "c"]}, qs_codec.EncodeOptions(encode=False, list_format=qs_codec.ListFormat.BRACKETS)
+            )
+            == "a[]=b&a[]=c"
         )
         assert (
-                qs_codec.encode({"a": ["b", "c"]}, qs_codec.EncodeOptions(encode=False, list_format=qs_codec.ListFormat.BRACKETS))
-                == "a[]=b&a[]=c"
+            qs_codec.encode(
+                {"a": ["b", "c"]}, qs_codec.EncodeOptions(encode=False, list_format=qs_codec.ListFormat.REPEAT)
+            )
+            == "a=b&a=c"
         )
         assert (
-                qs_codec.encode({"a": ["b", "c"]}, qs_codec.EncodeOptions(encode=False, list_format=qs_codec.ListFormat.REPEAT)) == "a=b&a=c"
+            qs_codec.encode(
+                {"a": ["b", "c"]}, qs_codec.EncodeOptions(encode=False, list_format=qs_codec.ListFormat.COMMA)
+            )
+            == "a=b,c"
         )
-        assert qs_codec.encode({"a": ["b", "c"]}, qs_codec.EncodeOptions(encode=False, list_format=qs_codec.ListFormat.COMMA)) == "a=b,c"
 
         # **Note:** When using `EncodeOptions.list_format` set to `ListFormat.COMMA`, you can also pass the
         # `EncodeOptions.comma_round_trip` option set to `True` or `False`, to append `[]` on single-item `list`s, so
         # that they can round trip through a parse.
 
         # When `dict`s are encoded, by default they use bracket notation:
-        assert qs_codec.encode({"a": {"b": {"c": "d", "e": "f"}}}, qs_codec.EncodeOptions(encode=False)) == "a[b][c]=d&a[b][e]=f"
+        assert (
+            qs_codec.encode({"a": {"b": {"c": "d", "e": "f"}}}, qs_codec.EncodeOptions(encode=False))
+            == "a[b][c]=d&a[b][e]=f"
+        )
 
         # You may override this to use dot notation by setting the `EncodeOptions.allow_dots` option to `True`:
         assert (
-                qs_codec.encode({"a": {"b": {"c": "d", "e": "f"}}}, qs_codec.EncodeOptions(encode=False, allow_dots=True))
-                == "a.b.c=d&a.b.e=f"
+            qs_codec.encode({"a": {"b": {"c": "d", "e": "f"}}}, qs_codec.EncodeOptions(encode=False, allow_dots=True))
+            == "a.b.c=d&a.b.e=f"
         )
 
         # You may encode the dot notation in the keys of `dict` with option `EncodeOptions.encode_dot_in_keys` by
         # setting it to `True`:
         assert (
-                qs_codec.encode(
+            qs_codec.encode(
                 {"name.obj": {"first": "John", "last": "Doe"}},
                 qs_codec.EncodeOptions(allow_dots=True, encode_dot_in_keys=True),
             )
-                == "name%252Eobj.first=John&name%252Eobj.last=Doe"
+            == "name%252Eobj.first=John&name%252Eobj.last=Doe"
         )
 
         # **Caveat:** when `EncodeOptions.encode_values_only` is `True` as well as `EncodeOptions.encode_dot_in_keys`,
         # only dots in keys and nothing else will be encoded.
 
         # You may allow empty `list` values by setting the `EncodeOptions.allow_empty_lists` option to `True`:
         assert (
-                qs_codec.encode({"foo": [], "bar": "baz"}, qs_codec.EncodeOptions(encode=False, allow_empty_lists=True))
-                == "foo[]&bar=baz"
+            qs_codec.encode({"foo": [], "bar": "baz"}, qs_codec.EncodeOptions(encode=False, allow_empty_lists=True))
+            == "foo[]&bar=baz"
         )
 
         # Empty strings and null values will omit the value, but the equals sign (`=`) remains in place:
         assert qs_codec.encode({"a": ""}) == "a="
 
         # Key with no values (such as an empty `dict` or `list`) will return nothing:
         assert qs_codec.encode({"a": []}) == ""
@@ -258,44 +284,44 @@
                 qs_codec.EncodeOptions(encode=False),
             )
             == "a=1970-01-01T00:00:07+00:00"
             if version_info.major == 3 and version_info.minor >= 11
             else "a=1970-01-01T00:00:07"
         )
         assert (
-                qs_codec.encode(
+            qs_codec.encode(
                 {
                     "a": (
                         datetime.datetime.fromtimestamp(7, datetime.UTC)
                         if version_info.major == 3 and version_info.minor >= 11
                         else datetime.datetime.utcfromtimestamp(7)
                     )
                 },
                 qs_codec.EncodeOptions(encode=False, serialize_date=lambda date: str(int(date.timestamp()))),
             )
-                == "a=7"
+            == "a=7"
         )
 
         # You may use the `EncodeOptions.sort` option to affect the order of parameter keys:
         assert (
-                qs_codec.encode(
+            qs_codec.encode(
                 {"a": "c", "z": "y", "b": "f"},
                 qs_codec.EncodeOptions(
                     encode=False,
                     sort=lambda a, b: (a > b) - (a < b),
                 ),
             )
-                == "a=c&b=f&z=y"
+            == "a=c&b=f&z=y"
         )
 
         # Finally, you can use the `EncodeOptions.filter` option to restrict which keys will be included in the encoded
         # output. If you pass a `Callable`, it will be called for each key to obtain the replacement value.
         # Otherwise, if you pass a `list`, it will be used to select properties and `list` indices to be encoded:
         assert (
-                qs_codec.encode(
+            qs_codec.encode(
                 {
                     "a": "b",
                     "c": "d",
                     "e": {
                         "f": (
                             datetime.datetime.fromtimestamp(123, datetime.UTC)
                             if version_info.major == 3 and version_info.minor >= 11
@@ -309,20 +335,23 @@
                     filter=lambda prefix, value: {
                         "b": None,
                         "e[f]": int(value.timestamp()) if isinstance(value, datetime.datetime) else value,
                         "e[g][0]": value * 2 if isinstance(value, int) else value,
                     }.get(prefix, value),
                 ),
             )
-                == "a=b&c=d&e[f]=123&e[g][0]=4"
+            == "a=b&c=d&e[f]=123&e[g][0]=4"
+        )
+        assert (
+            qs_codec.encode({"a": "b", "c": "d", "e": "f"}, qs_codec.EncodeOptions(encode=False, filter=["a", "e"]))
+            == "a=b&e=f"
         )
-        assert qs_codec.encode({"a": "b", "c": "d", "e": "f"}, qs_codec.EncodeOptions(encode=False, filter=["a", "e"])) == "a=b&e=f"
         assert (
-                qs_codec.encode({"a": ["b", "c", "d"], "e": "f"}, qs_codec.EncodeOptions(encode=False, filter=["a", 0, 2]))
-                == "a[0]=b&a[2]=d"
+            qs_codec.encode({"a": ["b", "c", "d"], "e": "f"}, qs_codec.EncodeOptions(encode=False, filter=["a", 0, 2]))
+            == "a[0]=b&a[2]=d"
         )
 
     def test_none_values(self):
         # By default, `None` values are treated like empty strings:
         assert qs_codec.encode({"a": None, "b": ""}) == "a=&b="
 
         # To distinguish between `None` values and empty `str`s use the `EncodeOptions.strict_null_handling` flag.
@@ -342,35 +371,39 @@
         # Characters that don't exist in `Charset.LATIN1` will be converted to numeric entities, similar to what
         # browsers do:
         assert qs_codec.encode({"a": "☺"}, qs_codec.EncodeOptions(charset=qs_codec.Charset.LATIN1)) == "a=%26%239786%3B"
 
         # You can use the `EncodeOptions.charset_sentinel` option to announce the character by including an `utf8=✓`
         # parameter with the proper encoding of the checkmark, similar to what Ruby on Rails and others do when
         # submitting forms.
-        assert qs_codec.encode({"a": "☺"}, qs_codec.EncodeOptions(charset_sentinel=True)) == "utf8=%E2%9C%93&a=%E2%98%BA"
         assert (
-                qs_codec.encode({"a": "æ"}, qs_codec.EncodeOptions(charset=qs_codec.Charset.LATIN1, charset_sentinel=True))
-                == "utf8=%26%2310003%3B&a=%E6"
+            qs_codec.encode({"a": "☺"}, qs_codec.EncodeOptions(charset_sentinel=True)) == "utf8=%E2%9C%93&a=%E2%98%BA"
+        )
+        assert (
+            qs_codec.encode({"a": "æ"}, qs_codec.EncodeOptions(charset=qs_codec.Charset.LATIN1, charset_sentinel=True))
+            == "utf8=%26%2310003%3B&a=%E6"
         )
 
         # By default, the encoding and decoding of characters is done in `Charset.UTF8`, and `Charset.LATIN1` support is
         # also built in via the `EncodeOptions.charset` and `DecodeOptions.charset` parameter, respectively.
         #
         # If you wish to encode query strings to a different character set (i.e.
         # [Shift JIS](https://en.wikipedia.org/wiki/Shift_JIS))
-        def custom_encoder(string: str, charset: t.Optional[qs_codec.Charset], format: t.Optional[qs_codec.Format]) -> str:
+        def custom_encoder(
+            string: str, charset: t.Optional[qs_codec.Charset], format: t.Optional[qs_codec.Format]
+        ) -> str:
             if string:
                 buf: bytes = codecs.encode(string, "shift_jis")
                 result: t.List[str] = ["{:02x}".format(b) for b in buf]
                 return "%" + "%".join(result)
             return ""
 
         assert (
-                qs_codec.encode({"a": "こんにちは！"}, qs_codec.EncodeOptions(encoder=custom_encoder))
-                == "%61=%82%b1%82%f1%82%c9%82%bf%82%cd%81%49"
+            qs_codec.encode({"a": "こんにちは！"}, qs_codec.EncodeOptions(encoder=custom_encoder))
+            == "%61=%82%b1%82%f1%82%c9%82%bf%82%cd%81%49"
         )
 
         # This also works for decoding of query strings:
         def custom_decoder(string: str, charset: t.Optional[qs_codec.Charset]) -> t.Optional[str]:
             if string:
                 result: t.List[int] = []
                 while string:
@@ -380,17 +413,17 @@
                         string = string[match.end() :]
                     else:
                         break
                 buf: bytes = bytes(result)
                 return codecs.decode(buf, "shift_jis")
             return None
 
-        assert qs_codec.decode("%61=%82%b1%82%f1%82%c9%82%bf%82%cd%81%49", qs_codec.DecodeOptions(decoder=custom_decoder)) == {
-            "a": "こんにちは！"
-        }
+        assert qs_codec.decode(
+            "%61=%82%b1%82%f1%82%c9%82%bf%82%cd%81%49", qs_codec.DecodeOptions(decoder=custom_decoder)
+        ) == {"a": "こんにちは！"}
 
     def test_rfc3986_and_rfc1738(self):
         # The default `EncodeOptions.format` is `Format.RFC3986` which encodes `' '` to `%20` which is backward
         # compatible. You can also set the `EncodeOptions.format` to `Format.RFC1738` which encodes `' '` to `+`.
         assert qs_codec.encode({"a": "b c"}, qs_codec.EncodeOptions(format=qs_codec.Format.RFC3986)) == "a=b%20c"
         assert qs_codec.encode({"a": "b c"}, qs_codec.EncodeOptions(format=qs_codec.Format.RFC3986)) == "a=b%20c"
         assert qs_codec.encode({"a": "b c"}, qs_codec.EncodeOptions(format=qs_codec.Format.RFC1738)) == "a=b+c"
```

### Comparing `qs_codec-0.1.2/tests/unit/utils_test.py` & `qs_codec-0.1.3/tests/unit/utils_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/tests/unit/weakref_test.py` & `qs_codec-0.1.3/tests/unit/weakref_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/.gitignore` & `qs_codec-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/LICENSE` & `qs_codec-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/README.md` & `qs_codec-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from typing import Listfrom re import Matchfrom typing import List
-
 # qs_codec
 
 A query string encoding and decoding library for Python.
 
 Ported from [qs](https://www.npmjs.com/package/qs) for JavaScript.
 
-![PyPI - Version](https://img.shields.io/pypi/v/qs_codec)
+[![PyPI - Version](https://img.shields.io/pypi/v/qs_codec)](https://pypi.org/project/qs-codec/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/qs_codec)
 ![PyPI - Status](https://img.shields.io/pypi/status/qs_codec)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qs_codec)
-![PyPI - Implementation](https://img.shields.io/pypi/implementation/qs_codec)
 ![PyPI - Format](https://img.shields.io/pypi/format/qs_codec)
 [![Test](https://github.com/techouse/qs_codec/actions/workflows/test.yml/badge.svg)](https://github.com/techouse/qs_codec/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/techouse/qs_codec/graph/badge.svg?token=Vp0z05yj2l)](https://codecov.io/gh/techouse/qs_codec)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/7ead208221ae4f6785631043064647e4)](https://app.codacy.com/gh/techouse/qs_codec/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![GitHub](https://img.shields.io/github/license/techouse/qs_codec)](LICENSE)
 [![GitHub Sponsors](https://img.shields.io/github/sponsors/techouse)](https://github.com/sponsors/techouse)
 [![GitHub Repo stars](https://img.shields.io/github/stars/techouse/qs_codec)](https://github.com/techouse/qs_codec/stargazers)
@@ -914,10 +912,10 @@
     {'a': 'b c'},
     qs_codec.EncodeOptions(format=qs_codec.Format.RFC1738)
 ) == 'a=b+c'
 ```
 
 ---
 
-Special thanks to the authors of [qs](https://github.com/ljharb/qs) for JavaScript:
+Special thanks to the authors of [qs](https://www.npmjs.com/package/qs) for JavaScript:
 - [Jordan Harband](https://github.com/ljharb)
 - [TJ Holowaychuk](https://github.com/visionmedia/node-querystring)
```

### Comparing `qs_codec-0.1.2/pyproject.toml` & `qs_codec-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qs_codec-0.1.2/PKG-INFO` & `qs_codec-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: qs-codec
-Version: 0.1.2
+Version: 0.1.3
 Summary: A query string encoding and decoding library for Python. Ported from qs for JavaScript.
 Project-URL: Source, https://github.com/techouse/qs_codec
 Project-URL: Changelog, https://github.com/techouse/qs_codec/blob/master/CHANGELOG.md
 Project-URL: Sponsor, https://github.com/sponsors/techouse
 Project-URL: PayPal, https://paypal.me/ktusar
 Author-email: Klemen Tusar <techouse@gmail.com>
 License: BSD-3-Clause
@@ -25,26 +25,24 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-from typing import Listfrom re import Matchfrom typing import List
-
 # qs_codec
 
 A query string encoding and decoding library for Python.
 
 Ported from [qs](https://www.npmjs.com/package/qs) for JavaScript.
 
-![PyPI - Version](https://img.shields.io/pypi/v/qs_codec)
+[![PyPI - Version](https://img.shields.io/pypi/v/qs_codec)](https://pypi.org/project/qs-codec/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/qs_codec)
 ![PyPI - Status](https://img.shields.io/pypi/status/qs_codec)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qs_codec)
-![PyPI - Implementation](https://img.shields.io/pypi/implementation/qs_codec)
 ![PyPI - Format](https://img.shields.io/pypi/format/qs_codec)
 [![Test](https://github.com/techouse/qs_codec/actions/workflows/test.yml/badge.svg)](https://github.com/techouse/qs_codec/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/techouse/qs_codec/graph/badge.svg?token=Vp0z05yj2l)](https://codecov.io/gh/techouse/qs_codec)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/7ead208221ae4f6785631043064647e4)](https://app.codacy.com/gh/techouse/qs_codec/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![GitHub](https://img.shields.io/github/license/techouse/qs_codec)](LICENSE)
 [![GitHub Sponsors](https://img.shields.io/github/sponsors/techouse)](https://github.com/sponsors/techouse)
 [![GitHub Repo stars](https://img.shields.io/github/stars/techouse/qs_codec)](https://github.com/techouse/qs_codec/stargazers)
@@ -945,10 +943,10 @@
     {'a': 'b c'},
     qs_codec.EncodeOptions(format=qs_codec.Format.RFC1738)
 ) == 'a=b+c'
 ```
 
 ---
 
-Special thanks to the authors of [qs](https://github.com/ljharb/qs) for JavaScript:
+Special thanks to the authors of [qs](https://www.npmjs.com/package/qs) for JavaScript:
 - [Jordan Harband](https://github.com/ljharb)
 - [TJ Holowaychuk](https://github.com/visionmedia/node-querystring)
```

