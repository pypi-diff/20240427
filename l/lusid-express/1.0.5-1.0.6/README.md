# Comparing `tmp/lusid_express-1.0.5.tar.gz` & `tmp/lusid_express-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_express-1.0.5.tar", last modified: Thu Apr 25 20:06:07 2024, max compression
+gzip compressed data, was "lusid_express-1.0.6.tar", last modified: Sat Apr 27 19:32:59 2024, max compression
```

## Comparing `lusid_express-1.0.5.tar` & `lusid_express-1.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:06:07.707778 lusid_express-1.0.5/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-25 20:05:26.000000 lusid_express-1.0.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-25 20:05:26.000000 lusid_express-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6659 2024-04-25 20:06:07.707778 lusid_express-1.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6019 2024-04-25 20:05:26.000000 lusid_express-1.0.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 20:06:07.707778 lusid_express-1.0.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-25 20:05:26.000000 lusid_express-1.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:06:07.701778 lusid_express-1.0.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:06:07.703778 lusid_express-1.0.5/src/lusid_express/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-25 20:05:26.000000 lusid_express-1.0.5/src/lusid_express/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5616 2024-04-25 20:05:26.000000 lusid_express-1.0.5/src/lusid_express/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:06:07.704778 lusid_express-1.0.5/src/lusid_express/apis/
--rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-04-25 20:06:07.000000 lusid_express-1.0.5/src/lusid_express/apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:06:07.706777 lusid_express-1.0.5/src/lusid_express/config/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-25 20:05:26.000000 lusid_express-1.0.5/src/lusid_express/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:06:07.707778 lusid_express-1.0.5/src/lusid_express/display/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-25 20:05:26.000000 lusid_express-1.0.5/src/lusid_express/display/PRELOADED_VARS.md
--rw-rw-rw-   0 root         (0) root         (0)     8675 2024-04-25 20:05:26.000000 lusid_express-1.0.5/src/lusid_express/display/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2352 2024-04-25 20:05:26.000000 lusid_express-1.0.5/src/lusid_express/load.le
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:06:07.704778 lusid_express-1.0.5/src/lusid_express.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6659 2024-04-25 20:06:07.000000 lusid_express-1.0.5/src/lusid_express.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      482 2024-04-25 20:06:07.000000 lusid_express-1.0.5/src/lusid_express.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:06:07.000000 lusid_express-1.0.5/src/lusid_express.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-25 20:06:07.000000 lusid_express-1.0.5/src/lusid_express.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-25 20:06:07.000000 lusid_express-1.0.5/src/lusid_express.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:32:59.427700 lusid_express-1.0.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-27 19:32:21.000000 lusid_express-1.0.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-27 19:32:21.000000 lusid_express-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6659 2024-04-27 19:32:59.427700 lusid_express-1.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6019 2024-04-27 19:32:21.000000 lusid_express-1.0.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 19:32:59.427700 lusid_express-1.0.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-27 19:32:21.000000 lusid_express-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:32:59.421700 lusid_express-1.0.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:32:59.423700 lusid_express-1.0.6/src/lusid_express/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-27 19:32:21.000000 lusid_express-1.0.6/src/lusid_express/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5616 2024-04-27 19:32:21.000000 lusid_express-1.0.6/src/lusid_express/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:32:59.425700 lusid_express-1.0.6/src/lusid_express/apis/
+-rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-04-27 19:32:59.000000 lusid_express-1.0.6/src/lusid_express/apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:32:59.426700 lusid_express-1.0.6/src/lusid_express/config/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-27 19:32:21.000000 lusid_express-1.0.6/src/lusid_express/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:32:59.427700 lusid_express-1.0.6/src/lusid_express/display/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-27 19:32:21.000000 lusid_express-1.0.6/src/lusid_express/display/PRELOADED_VARS.md
+-rw-rw-rw-   0 root         (0) root         (0)    10715 2024-04-27 19:32:21.000000 lusid_express-1.0.6/src/lusid_express/display/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2352 2024-04-27 19:32:21.000000 lusid_express-1.0.6/src/lusid_express/load.le
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:32:59.424700 lusid_express-1.0.6/src/lusid_express.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6659 2024-04-27 19:32:59.000000 lusid_express-1.0.6/src/lusid_express.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-27 19:32:59.000000 lusid_express-1.0.6/src/lusid_express.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 19:32:59.000000 lusid_express-1.0.6/src/lusid_express.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-27 19:32:59.000000 lusid_express-1.0.6/src/lusid_express.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-27 19:32:59.000000 lusid_express-1.0.6/src/lusid_express.egg-info/top_level.txt
```

### Comparing `lusid_express-1.0.5/LICENSE` & `lusid_express-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.5/PKG-INFO` & `lusid_express-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid_express
-Version: 1.0.5
+Version: 1.0.6
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_express-1.0.5/README.md` & `lusid_express-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.5/setup.py` & `lusid_express-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 
 
 
 
 setup(
     name='lusid_express',
-    version='1.0.5',
+    version='1.0.6',
     package_dir={'': 'src'},  # tells setuptools that packages are under src
     packages=find_packages(where='src'),  # tells setuptools to look for packages in src
     install_requires=requirements,
     description='lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
```

### Comparing `lusid_express-1.0.5/src/lusid_express/__main__.py` & `lusid_express-1.0.6/src/lusid_express/__main__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.5/src/lusid_express/apis/__init__.py` & `lusid_express-1.0.6/src/lusid_express/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.5/src/lusid_express/display/PRELOADED_VARS.md` & `lusid_express-1.0.6/src/lusid_express/display/PRELOADED_VARS.md`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.5/src/lusid_express/display/__init__.py` & `lusid_express-1.0.6/src/lusid_express/display/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from IPython.display import Markdown as render_markdown, HTML as render_html
 import os as __os
 import json as __json
-import re
-from uuid import uuid4 as UUID
+import re as __re
+from uuid import uuid4 as __UUID
+import uuid as __uuid
 
 with open(__os.path.join(__os.path.dirname(__file__), "PRELOADED_VARS.md"), "r") as __f:
     PRELOADED_VARS_MARKDOWN = __f.read()
 
 
 def data_to_markdown(data, col_name_key="Key", col_name_value="Value", title="table"):
     """
@@ -70,71 +71,85 @@
 .button:focus-visible {
   box-shadow: none;
 }
 </style>
 <button 
 class="button"
 
-onclick='copyTable()'>Copy to Clipboard</button>
+onclick='copyTable("REPLACEMENT_HOOK")'>Copy to Clipboard</button>
  <script>
-        function copyTable() {{
-            var rows = document.querySelectorAll('#data_table tr');
-            var csvContent = '';
-            rows.forEach(function(row, index) {{
-                var cols = row.querySelectorAll('th, td');
-                var rowData = [];
-                cols.forEach(function(col) {{
-                    var text = col.innerText.replace(/(\\r\\n|\\n|\\r)/gm, '');
-                     if (text.startsWith('[') && text.endsWith(']')) {
-                    var listItems = text.slice(1, -1).split(', ');
-                    listItems.forEach(function(item) {
-                        rowData.push(item.replace(/['"]+/g, '')); // Remove quotes from items
-                    });
-                } else {
-                    rowData.push(text);
-                }
-                }});
-                csvContent += rowData.join('\\t') + '\\n';
-            }});
-            var el = document.createElement('textarea');
-            el.value = csvContent;
-            document.body.appendChild(el);
-            el.select();
-            document.execCommand('copy');
-            document.body.removeChild(el);
-            alert('Copied to clipboard');
-        }}
+function copyTable(tableId) {
+    var table = document.getElementById(tableId);
+    if (!table) {
+        alert("Table not found!");
+        return;
+    }
+    var rows = table.querySelectorAll('tr');
+    var csvContent = '';
+    rows.forEach(function(row) {
+        var isExpandableRow = row.classList.contains('expandable');
+        var cols = row.querySelectorAll('th, td');
+        var rowData = [];
+        cols.forEach(function(col) {
+            // Skip cells that contain the 'expand-link' class or are in expandable rows
+            if (!col.querySelector('.expand-link') && !isExpandableRow) {
+                var text = col.innerText.replace(/(\r\n|\n|\r)/gm, '').trim();
+                rowData.push(text);
+            }
+        });
+        // Only add non-empty rows to the CSV content
+        if (rowData.length > 0 && !isExpandableRow) {
+            csvContent += rowData.join('\t') + '\n';
+        }
+    });
+    // Create a temporary textarea element to copy the content
+    var el = document.createElement('textarea');
+    el.value = csvContent;
+    document.body.appendChild(el);
+    el.select();
+    document.execCommand('copy');
+    document.body.removeChild(el);
+    alert('Copied to clipboard');
+}
+
         </script>"""
 
 STYLES = {
     "table": """
 <style>
 @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700&display=swap');
 
 :root {
     --main-color: #00B6DA; /* Light theme color */
     --table-color: #065F82; /* Light theme table color */
     --accent-color: #FF5500; /* Light theme accent color */
     --foreground-color: #777777; /* Light theme background */
 }
+.indent-0 { padding-left: 0em; }
+.indent-1 { padding-left: 1em; }
+.indent-2 { padding-left: 2em; }
+.indent-3 { padding-left: 3em; }
+.indent-4 { padding-left: 4em; }
+.indent-5 { padding-left: 5em; }
+.indent-6 { padding-left: 6em; }
 
 @media (prefers-color-scheme: dark) {
     :root {
         --main-color: #0094AC; /* Dark theme color */
         --table-color: #043A4A; /* Dark theme table color */
         --accent-color: #E76F00; /* Dark theme accent color */
         --foreground-color: #777777; /* Dark theme background */
     }
 }
 
 body, h1, h2, h3, p {
     font-family: 'Montserrat';
 }
 table {
-
+    padding: 4px;
     margin-left: 2px;
     margin-right: 2px;
     border-collapse: collapse;
     text-align: center;
     color: #065F82;
     border: 2px solid #ccc; /* Add border */
     border-radius: 10px; /* Add border radius */
@@ -170,14 +185,16 @@
     line-height: 12px;
     font-weight: 500;
 color: var(--foreground-color);
 
 }
 th, td {
     height: 15px; /* Fixed height for all rows */
+    padding: 8px  !important;
+    text-align: left !important; /* Ensure text is aligned left */
 
 
 }
 th h2, td h3, td p {
     margin: 0;     /* Remove margin from cell contents */
     padding: 5px;  /* Reduce padding */
     text-align: left; 
@@ -190,14 +207,15 @@
 }
     tr:nth-child(odd) td {
     border-color: #415464;
     color: #FF5500;
 }
 
 </style>
+
 """
 }
 
 
 def __convert_data(data):
     """
     Converts a JSON string to a dictionary if necessary.
@@ -235,42 +253,74 @@
         col_name_key (str): Custom name for the column header of the keys.
         col_name_value (str): Custom name for the column header of the values.
         title (str): Title of the table.
     """
 
     table = ""
 
-    # return f"## {title}\n{markdown_table}"
-    def get_row(key, value):
-        return f"<tr><td><h3>{key}</h3></td><td><p>{value}</p></td></tr>"
 
+
+    def get_rows(key, value, depth=0):
+        """ Generate HTML rows for any nested structures, with CSS class and non-breaking spaces for indentation """
+        rows = ""
+        nbsp_indent = "&nbsp;" * (depth * 4)  # Non-breaking spaces for indentation
+        indent_class = f"indent-{depth}"  # CSS class for indentation
+
+        if isinstance(value, dict):
+            # Include the key for the dictionary
+            rows += f"<tr><td class='{indent_class}'>{nbsp_indent}<strong>{key}</strong></td><td></td></tr>"
+            # Recursively handle dictionary items
+            for sub_key, sub_value in value.items():
+                rows += get_rows(sub_key, sub_value, depth + 1)
+        elif isinstance(value, list):
+            # Start with the key for the list
+            rows += f"<tr><td class='{indent_class}'>{nbsp_indent}<strong>{key}</strong></td><td>{str(value[0]) if value else '(empty list)'}</td></tr>"
+            # Continue with the rest of the items without the key
+            for item in value[1:]:
+                rows += f"<tr><td class='{indent_class}'>{nbsp_indent}</td><td>{str(item)}</td></tr>"
+        else:
+            # Handle simple key-value pairs
+            rows += f"<tr><td class='{indent_class}'>{nbsp_indent}<strong>{key}</strong></td><td>{str(value)}</td></tr>"
+        return rows
+
+    
+    def clean(data):
+        if isinstance(data, dict):
+            return {k: clean(v) for k, v in data.items() if v is not None}
+        elif isinstance(data, list):
+            return [clean(item) for item in data if item is not None]
+        else:
+            return data
     
-    id = f"DATA_TABLE-{UUID()}"
     # Add each key-value pair as a row in the table
+    data = clean(data)
+    table = ""
     for key, value in data.items():
-        # Ensure the value is converted to a string if necessary
-        table += get_row(key, value)
-
-    return f"""<h1>{title}</h1> <table id={id}><tr><th><h2>{col_name_key}</h2></th><th><h2>{col_name_value}</h2></th></tr>{table}</table  >{COPY_SCRIPT.replace('data_table', id)}"""
+        table += get_rows(key, value)
 
+    # Ensure the table ID is correctly set and used in the COPY_SCRIPT
+    table_id = f"DATA_TABLE-{__uuid.uuid4()}"  # Unique ID for each table instance
+    html_output = f"""<h1>{title}</h1> <table id='{table_id}'><tr><th>{col_name_key}</th><th>{col_name_value}</th></tr>{table}</table>{COPY_SCRIPT.replace('REPLACEMENT_HOOK', table_id)}"""
+    print(html_output)
+    return html_output
 
 def render_table(data, col_name_key="Key", col_name_value="Value", title="table"):
     """
     Renders table from data.
 
     Parameters:
         data (str or dict): JSON string or dictionary containing the data.
         col_name_key (str): Custom name for the column header of the keys.
         col_name_value (str): Custom name for the column header of the values.
         title (str): Title of the table.
     """
 
     def camel_case_to_spaces(input_string):
         # This regular expression finds all places where a lowercase letter is followed by an uppercase letter
-        result = re.sub(r"(?<=[a-z])(?=[A-Z])", " ", input_string)
+        result = __re.sub(r"(?<=[a-z])(?=[A-Z])", " ", input_string)
         return result
 
     try:
         if str(type(data)).removeprefix("<class '").split(".")[0] == "lusid":
             title = (
                 str(type(data)).split(".")[-1].removesuffix("'>").removeprefix("Create")
             )
```

### Comparing `lusid_express-1.0.5/src/lusid_express/load.le` & `lusid_express-1.0.6/src/lusid_express/load.le`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.5/src/lusid_express.egg-info/PKG-INFO` & `lusid_express-1.0.6/src/lusid_express.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-express
-Version: 1.0.5
+Version: 1.0.6
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

