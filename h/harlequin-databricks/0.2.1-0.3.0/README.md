# Comparing `tmp/harlequin_databricks-0.2.1.tar.gz` & `tmp/harlequin_databricks-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harlequin_databricks-0.2.1.tar", max compression
+gzip compressed data, was "harlequin_databricks-0.3.0.tar", max compression
```

## Comparing `harlequin_databricks-0.2.1.tar` & `harlequin_databricks-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1089 2024-02-15 14:46:02.148060 harlequin_databricks-0.2.1/LICENSE
--rw-r--r--   0        0        0     4538 2024-02-15 14:46:02.148060 harlequin_databricks-0.2.1/README.md
--rw-r--r--   0        0        0     2173 2024-02-15 14:46:02.148060 harlequin_databricks-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      110 2024-02-15 14:46:02.148060 harlequin_databricks-0.2.1/src/harlequin_databricks/__init__.py
--rw-r--r--   0        0        0    14566 2024-02-15 14:46:02.148060 harlequin_databricks-0.2.1/src/harlequin_databricks/adapter.py
--rw-r--r--   0        0        0     2269 2024-02-15 14:46:02.148060 harlequin_databricks-0.2.1/src/harlequin_databricks/cli_options.py
--rw-r--r--   0        0        0     1228 2024-02-15 14:46:02.148060 harlequin_databricks-0.2.1/src/harlequin_databricks/completions.py
--rw-r--r--   0        0        0    39501 2024-02-15 14:46:02.148060 harlequin_databricks-0.2.1/src/harlequin_databricks/functions.csv
--rw-r--r--   0        0        0      814 2024-02-15 14:46:02.148060 harlequin_databricks-0.2.1/src/harlequin_databricks/keywords.csv
--rw-r--r--   0        0        0        0 2024-02-15 14:46:02.148060 harlequin_databricks-0.2.1/src/harlequin_databricks/py.typed
--rw-r--r--   0        0        0     5654 1970-01-01 00:00:00.000000 harlequin_databricks-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-27 14:58:05.501782 harlequin_databricks-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4538 2024-04-27 14:58:05.501782 harlequin_databricks-0.3.0/README.md
+-rw-r--r--   0        0        0     2184 2024-04-27 14:58:05.505782 harlequin_databricks-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      110 2024-04-27 14:58:05.505782 harlequin_databricks-0.3.0/src/harlequin_databricks/__init__.py
+-rw-r--r--   0        0        0    14648 2024-04-27 14:58:05.505782 harlequin_databricks-0.3.0/src/harlequin_databricks/adapter.py
+-rw-r--r--   0        0        0     2269 2024-04-27 14:58:05.505782 harlequin_databricks-0.3.0/src/harlequin_databricks/cli_options.py
+-rw-r--r--   0        0        0     1228 2024-04-27 14:58:05.505782 harlequin_databricks-0.3.0/src/harlequin_databricks/completions.py
+-rw-r--r--   0        0        0    41249 2024-04-27 14:58:05.505782 harlequin_databricks-0.3.0/src/harlequin_databricks/functions.csv
+-rw-r--r--   0        0        0      814 2024-04-27 14:58:05.505782 harlequin_databricks-0.3.0/src/harlequin_databricks/keywords.csv
+-rw-r--r--   0        0        0        0 2024-04-27 14:58:05.505782 harlequin_databricks-0.3.0/src/harlequin_databricks/py.typed
+-rw-r--r--   0        0        0     5654 1970-01-01 00:00:00.000000 harlequin_databricks-0.3.0/PKG-INFO
```

### Comparing `harlequin_databricks-0.2.1/LICENSE` & `harlequin_databricks-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `harlequin_databricks-0.2.1/README.md` & `harlequin_databricks-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `harlequin_databricks-0.2.1/pyproject.toml` & `harlequin_databricks-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "harlequin-databricks"
-version = "0.2.1"
+version = "0.3.0"
 description = "A Harlequin adapter for Databricks."
 authors = [
     "Zach Shirah <zachshirah01@gmail.com>",
     "Alex Malins <github@alexmalinsREMOVETHIS.com>",
 ]
 license = "MIT"
 homepage = "https://harlequin.sh/docs/databricks/index"
@@ -16,31 +16,31 @@
 ]
 
 [tool.poetry.plugins."harlequin.adapter"]
 databricks = "harlequin_databricks:HarlequinDatabricksAdapter"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-harlequin = "^1.14"
+harlequin = "^1.17"
 databricks-sql-connector = "^3.0.3"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.12.1"
-ruff = "^0.1.6"
-pytest = "^7.4.3"
-mypy = "^1.7.0"
+black = "^24.4.2"
+ruff = "^0.4.2"
+pytest = "^8.1.2"
+mypy = "^1.10.0"
 pre-commit = "^3.5.0"
-importlib_metadata = { version = ">=4.6.0", python = "<3.10.0" }
+importlib_metadata = { version = ">=7.1.0", python = "<3.10.0" }
 beautifulsoup4 = "^4.12.3"
 types-beautifulsoup4 = "^4.12.0.0"
-lxml = "^5.1.0"
+lxml = "^5.2.1"
 pandas = "^2.0.0"
 pandas-stubs = "^2.0.0.230412"
-requests = "^2.0.0"
-types-requests = "^2.25.0"
+requests = "^2.31.0"
+types-requests = "^2.31.0.20240406"
 
 [tool.poetry.urls]
 Changelog = "https://github.com/alexmalins/harlequin-databricks/blob/main/CHANGELOG.md"
 Discussions = "https://github.com/alexmalins/harlequin-databricks/discussions"
 Issues = "https://github.com/alexmalins/harlequin-databricks/issues"
 
 [build-system]
@@ -75,12 +75,12 @@
 disallow_incomplete_defs = true
 disallow_subclassing_any = true
 strict_optional = true
 
 warn_return_any = true
 warn_no_return = true
 warn_redundant_casts = true
-warn_unused_ignores = true
+warn_unused_ignores = false
 warn_unused_configs = true
 
 no_implicit_reexport = true
 strict_equality = true
```

### Comparing `harlequin_databricks-0.2.1/src/harlequin_databricks/adapter.py` & `harlequin_databricks-0.3.0/src/harlequin_databricks/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,14 +330,18 @@
                     )
                 )
             return catalog_items, unity_catalogs.to_pylist()
 
     def get_completions(self) -> list[HarlequinCompletion]:
         return load_completions()
 
+    def close(self) -> None:
+        if self.conn:
+            self.conn.close()
+
 
 class HarlequinDatabricksAdapter(HarlequinAdapter):
     ADAPTER_OPTIONS = DATABRICKS_ADAPTER_OPTIONS
 
     def __init__(
         self,
         server_hostname: str | None = None,
```

### Comparing `harlequin_databricks-0.2.1/src/harlequin_databricks/cli_options.py` & `harlequin_databricks-0.3.0/src/harlequin_databricks/cli_options.py`

 * *Files identical despite different names*

### Comparing `harlequin_databricks-0.2.1/src/harlequin_databricks/completions.py` & `harlequin_databricks-0.3.0/src/harlequin_databricks/completions.py`

 * *Files identical despite different names*

### Comparing `harlequin_databricks-0.2.1/src/harlequin_databricks/functions.csv` & `harlequin_databricks-0.3.0/src/harlequin_databricks/functions.csv`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,27 @@
 abs,abs(expr),Returns the absolute value of the numeric value in expr.
 acos,acos(expr),Returns the inverse cosine (arccosine) of expr.
 acosh,acosh(expr),Returns the inverse hyperbolic cosine of expr.
 add_months,"add_months(startDate,numMonths)",Returns the date that is numMonths after startDate.
 aes_decrypt,"aes_decrypt(expr, key[, mode[, padding[, aad]]])",Decrypts a binary expr using AES encryption.
 aes_encrypt,"aes_encrypt(expr, key[, mode[, padding[, iv[, aad]]]])",Encrypts a binary expr using AES encryption.
 aggregate,"aggregate(expr,start,merge[,finish])",Aggregates elements in an array using a custom aggregator.
-ai_generate_text,"ai_generate_text(prompt, modelName[, param1, value1] […])",Returns text generated by a selected large language model (LLM) given the prompt.
+ai_analyze_sentiment,ai_analyze_sentiment(content),Returns the sentiment of a text.
+ai_classify,"ai_classify(content, labels)",Classifies the provided content into one of the provided labels.
+ai_extract,"ai_extract(content, labels)",Extracts entities specified by labels from a given text.
+ai_fix_grammar,ai_fix_grammar(content),Corrects grammatical errors in a given text.
+ai_gen,ai_gen(content),Invokes a state-of-the-art generative AI model from Databricks Foundation Model APIs to answer the user-provided prompt.
+ai_generate_text,"ai_generate_text(prompt, modelName[, param1, value1] […])",Deprecated: Returns text generated by a selected large language model (LLM) given the prompt.
+ai_mask,"ai_mask(content, labels)",Masks specified entities within a given text.
 ai_query,"ai_query(endpointName, request, returnType)",Invokes an existing Databricks Model Serving endpoint and parses and returns its response.
+ai_similarity,"ai_similarity(strExpr1, strExpr2)",Compares two strings and computes the semantic similarity score.
+ai_summarize,"ai_summarize(content[, max_words])",Generates a summary of a given text.
+ai_translate,"ai_translate(content, to_lang)",Translates text to a specified target language.
 any,any(expr),Returns true if at least one value of expr in the group is true.
-any_value,"any_value(expr[,ignoreNull])",Returns any random value of expr for a group of rows.
+any_value,"any_value(expr[,ignoreNull])",Returns some value of expr for a group of rows.
 approx_count_distinct,"approx_count_distinct(expr[,relativeSD])",Returns the estimated number of distinct values in expr within the group.
 approx_percentile,"approx_percentile(expr,percentage[,accuracy])",Returns the approximate percentile of the expr within the group.
 approx_top_k,"approx_top_k(expr[,k[,maxItemsTracked]])",Returns the top k most frequently occurring item values in an expr along with their approximate counts.
 array,"array([expr [, …]])",Returns an array with the elements in expr.
 array_agg,array_agg(expr),Returns an array consisting of all values in expr within the group.
 array_append,"array_append(array, elem)",Returns array appended by elem.
 array_compact,array_compact(array),Removes NULL values from array.
@@ -154,14 +163,15 @@
 from_json,"from_json(jsonStr, schema[, options])",Returns a struct value with the jsonStr and schema.
 from_unixtime,"from_unixtime(unixTime,fmt)",Returns unixTime in fmt.
 from_utc_timestamp,"from_utc_timestamp(expr,timezone)",Returns a timestamp in expr specified in UTC in the timezone timeZone.
 from_xml,"from_xml(xmlStr, schema[, options])",Returns a struct value parsed from the xmlStr using schema.
 get,"get(arrayExpr, index)","Returns the element of an arrayExpr at index, starting at 0."
 get_json_object,"get_json_object(expr, path)",Extracts a JSON object from path.
 getbit,"getbit(expr, pos)",Returns the value of a bit in a binary representation of an integral numeric.
+getdate,getdate(),Returns the current timestamp at the start of query evaluation.
 greatest,"greatest(expr1, expr2 [, …])","Returns the largest value of all arguments, skipping null values."
 grouping,grouping(col),"Indicates whether a specified column in a GROUPING SET, ROLLUP, or CUBE represents a subtotal."
 grouping_id,"grouping_id([col1 [, …]])",Returns the level of grouping for a set of columns.
 hash,"hash(expr1 [, …])",Returns a hashed value of the arguments.
 hex,hex(expr),Converts expr to hexadecimal.
 hll_sketch_agg,"hll_sketch_agg(expr[,lgConfigK])",Returns a HyperLogLog sketch used to approximate a distinct values count.
 hll_sketch_estimate,hll_sketch_estimate(expr),Etimates number of distinct values collected in a HyperLogLog sketch.
@@ -192,15 +202,15 @@
 kurtosis,kurtosis(expr),Returns the kurtosis value calculated from values of a group.
 lag,"lag(expr[,offset[,default]])",Returns the value of expr from a preceding row within the partition.
 last,"last(expr[,ignoreNull])",Returns the last value of expr for the group of rows.
 last_day,last_day(expr),Returns the last day of the month that the date belongs to.
 last_value,"last_value(expr[,ignoreNull])",Returns the last value of expr for the group of rows.
 lcase,lcase(expr),Returns expr with all characters changed to lowercase.
 lead,"lead(expr[,offset[,default]])",Returns the value of expr from a subsequent row within the partition.
-least,"least(expr1 [, …])","Returns the smallest value of all arguments, skipping null values."
+least,"least(expr1, expr2 [, …])","Returns the smallest value of all arguments, skipping null values."
 left,"left(str, len)",Returns the leftmost len characters from str.
 len,len(expr),Returns the character length of string data or number of bytes of binary data.
 length,length(expr),Returns the character length of string data or number of bytes of binary data.
 levenshtein,"levenshtein(str1, str2)",Returns the Levenshtein distance between the strings str1 and str2.
 list_secrets,list_secrets(),Returns the keys which the user is authorized to see from Databricks secret service.
 ln,ln(expr),Returns the natural logarithm (base e) of expr.
 locate,"locate(substr, str[, pos])",Returns the position of the first occurrence of substr in str after position pos.
@@ -274,14 +284,19 @@
 rand,rand([seed]),Returns a random value between 0 and 1.
 randn,randn([seed]),Returns a random value from a standard normal distribution.
 random,random([seed]),Returns a random value between 0 and 1.
 range,range(end),Returns a table of values within a specified range.
 rank,rank(),Returns the rank of a value compared to all values in the partition.
 read_files,"read_files(path, [optionKey => optionValue] [, …])",Reads data files on cloud storage and returns it in tabular format.
 read_kafka,"read_kafka([optionKey => optionValue] [, …])",Reads records from an Apache Kafka cluster and returns it in tabular format.
+read_kinesis,"read_kinesis({parameter => value} [, …])",Returns a table with records read from Kinesis from one or more streams.
+read_pubsub,"read_pubsub([parameter => value] [, …])",A table valued function for reading records from Pub/Sub from a topic.
+read_pulsar,"read_pulsar({optionKey => optionValue} [, …])",Returns a table with records read from Pulsar.
+read_state_metadata,read_state_metadata(path),Returns a table with rows that represent the metadata of a streaming query state.
+read_statestore,"read_statestore(path [, option_key => option_value] […])",Returns records from the state store of streaming queries.
 reduce,"reduce(expr,start,merge[,finish])",Aggregates elements in an array using a custom aggregator.
 reflect,"reflect(class, method[, arg1 [, …]])",Calls a method with reflection.
 regexp_count,"regexp_count(str, regexp)",Returns the number of times str matches the regexp pattern.
 regexp_extract,"regexp_extract(str, regexp[, idx])",Extracts the first string in str that matches the regexp expression and corresponds to the regex group index.
 regexp_extract_all,"regexp_extract_all(str, regexp[, idx])",Extracts the all strings in str that matches the regexp expression and corresponds to the regex group index.
 regexp_instr,"regexp_instr(str, regexp)",Returns the position of the first substring in str that matches regexp.
 regexp_replace,"regexp_replace(str, regexp, rep[, position])",Replaces all substrings of str that match regexp with rep.
@@ -302,14 +317,15 @@
 rint,rint(expr),Returns expr rounded to a whole number as a DOUBLE.
 round,"round(expr[,targetScale])",Returns the rounded expr using HALF_UP rounding mode.
 row_number,row_number(),"Assigns a unique, sequential number to each row, starting with one, according to the ordering of rows within the window partition."
 rpad,"rpad(expr, len[, pad])","Returns expr, right-padded with pad to a length of len."
 rtrim,"rtrim([trimStr,] str)",Returns str with trailing characters removed.
 schema_of_csv,"schema_of_csv(csv[, options])",Returns the schema of a CSV string in DDL format.
 schema_of_json,"schema_of_json(jsonStr[, options])",Returns the schema of a JSON string in DDL format.
+schema_of_json_agg,"schema_of_json_agg(json[, options])",Returns the combined schema of JSON strings in a group in DDL format.
 schema_of_xml,"schema_of_xml(xmlStr[, options])",Returns the schema of a XML string in DDL format.
 sec,sec(expr),Returns the secant of expr.
 second,second(expr),Returns the second component of the timestamp in expr.
 secret,"secret(scope, key)",Extracts a secret value with the given scope and key from Databricks secret service.
 sentences,"sentences(str[, lang, country])",Splits str into an array of array of words.
 sequence,"sequence(start,stop,step)","Generates an array of elements from start to stop (inclusive), incrementing by step."
 session_user,session_user(),Returns the user connected to Databricks.
```

### Comparing `harlequin_databricks-0.2.1/src/harlequin_databricks/keywords.csv` & `harlequin_databricks-0.3.0/src/harlequin_databricks/keywords.csv`

 * *Files identical despite different names*

### Comparing `harlequin_databricks-0.2.1/PKG-INFO` & `harlequin_databricks-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: harlequin-databricks
-Version: 0.2.1
+Version: 0.3.0
 Summary: A Harlequin adapter for Databricks.
 Home-page: https://harlequin.sh/docs/databricks/index
 License: MIT
 Author: Zach Shirah
 Author-email: zachshirah01@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: databricks-sql-connector (>=3.0.3,<4.0.0)
-Requires-Dist: harlequin (>=1.14,<2.0)
+Requires-Dist: harlequin (>=1.17,<2.0)
 Project-URL: Changelog, https://github.com/alexmalins/harlequin-databricks/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://harlequin.sh/docs/databricks/index
 Project-URL: Discussions, https://github.com/alexmalins/harlequin-databricks/discussions
 Project-URL: Issues, https://github.com/alexmalins/harlequin-databricks/issues
 Project-URL: Repository, https://github.com/alexmalins/harlequin-databricks
 Description-Content-Type: text/markdown
```

