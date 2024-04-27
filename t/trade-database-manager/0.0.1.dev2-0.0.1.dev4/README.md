# Comparing `tmp/trade_database_manager-0.0.1.dev2.tar.gz` & `tmp/trade_database_manager-0.0.1.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trade_database_manager-0.0.1.dev2.tar", last modified: Mon Apr 22 13:37:29 2024, max compression
+gzip compressed data, was "trade_database_manager-0.0.1.dev4.tar", last modified: Sat Apr 27 03:09:37 2024, max compression
```

## Comparing `trade_database_manager-0.0.1.dev2.tar` & `trade_database_manager-0.0.1.dev4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 13:37:29.624081 trade_database_manager-0.0.1.dev2/
--rw-rw-rw-   0        0        0    35184 2023-12-24 12:12:27.000000 trade_database_manager-0.0.1.dev2/LICENSE
--rw-rw-rw-   0        0        0     3205 2024-04-22 13:37:29.623081 trade_database_manager-0.0.1.dev2/PKG-INFO
--rw-rw-rw-   0        0        0     2333 2024-04-09 11:51:28.000000 trade_database_manager-0.0.1.dev2/README.md
--rw-rw-rw-   0        0        0     1547 2024-04-22 12:39:40.000000 trade_database_manager-0.0.1.dev2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-22 13:37:29.624081 trade_database_manager-0.0.1.dev2/setup.cfg
--rw-rw-rw-   0        0        0       41 2024-04-22 12:39:40.000000 trade_database_manager-0.0.1.dev2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 13:37:29.613080 trade_database_manager-0.0.1.dev2/trade_database_manager/
--rw-rw-rw-   0        0        0        0 2023-12-24 12:22:34.000000 trade_database_manager-0.0.1.dev2/trade_database_manager/__init__.py
--rw-rw-rw-   0        0        0      184 2023-12-24 14:33:56.000000 trade_database_manager-0.0.1.dev2/trade_database_manager/config.py
-drwxrwxrwx   0        0        0        0 2024-04-22 13:37:29.618082 trade_database_manager-0.0.1.dev2/trade_database_manager/core/
--rw-rw-rw-   0        0        0        0 2023-12-24 12:22:34.000000 trade_database_manager-0.0.1.dev2/trade_database_manager/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 13:37:29.618082 trade_database_manager-0.0.1.dev2/trade_database_manager/core/kdb/
--rw-rw-rw-   0        0        0        0 2023-12-24 12:22:34.000000 trade_database_manager-0.0.1.dev2/trade_database_manager/core/kdb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 13:37:29.620081 trade_database_manager-0.0.1.dev2/trade_database_manager/core/sql/
--rw-rw-rw-   0        0        0        0 2023-12-24 12:22:34.000000 trade_database_manager-0.0.1.dev2/trade_database_manager/core/sql/__init__.py
--rw-rw-rw-   0        0        0     9482 2024-04-22 12:39:40.000000 trade_database_manager-0.0.1.dev2/trade_database_manager/core/sql/sqlmanager.py
--rw-rw-rw-   0        0        0        0 2023-12-24 12:22:34.000000 trade_database_manager-0.0.1.dev2/trade_database_manager/core/sql/sqlreader.py
--rw-rw-rw-   0        0        0        0 2023-12-24 12:22:34.000000 trade_database_manager-0.0.1.dev2/trade_database_manager/core/sql/sqlwriter.py
--rw-rw-rw-   0        0        0      524 2024-04-22 12:39:40.000000 trade_database_manager-0.0.1.dev2/trade_database_manager/core/typedefs.py
-drwxrwxrwx   0        0        0        0 2024-04-22 13:37:29.622081 trade_database_manager-0.0.1.dev2/trade_database_manager/manager/
--rw-rw-rw-   0        0        0      117 2024-04-22 12:39:40.000000 trade_database_manager-0.0.1.dev2/trade_database_manager/manager/__init__.py
--rw-rw-rw-   0        0        0      601 2024-04-22 12:39:40.000000 trade_database_manager-0.0.1.dev2/trade_database_manager/manager/fields_data_type.py
--rw-rw-rw-   0        0        0     6696 2024-04-22 12:39:40.000000 trade_database_manager-0.0.1.dev2/trade_database_manager/manager/metadata_sql.py
--rw-rw-rw-   0        0        0      910 2024-04-22 12:39:40.000000 trade_database_manager-0.0.1.dev2/trade_database_manager/manager/typedefs.py
-drwxrwxrwx   0        0        0        0 2024-04-22 13:37:29.622081 trade_database_manager-0.0.1.dev2/trade_database_manager.egg-info/
--rw-rw-rw-   0        0        0     3205 2024-04-22 13:37:29.000000 trade_database_manager-0.0.1.dev2/trade_database_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      826 2024-04-22 13:37:29.000000 trade_database_manager-0.0.1.dev2/trade_database_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 13:37:29.000000 trade_database_manager-0.0.1.dev2/trade_database_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-22 13:37:29.000000 trade_database_manager-0.0.1.dev2/trade_database_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-04-22 13:37:29.000000 trade_database_manager-0.0.1.dev2/trade_database_manager.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 03:09:37.755499 trade_database_manager-0.0.1.dev4/
+-rw-rw-rw-   0        0        0    35184 2023-12-24 12:12:27.000000 trade_database_manager-0.0.1.dev4/LICENSE
+-rw-rw-rw-   0        0        0     3205 2024-04-27 03:09:37.755499 trade_database_manager-0.0.1.dev4/PKG-INFO
+-rw-rw-rw-   0        0        0     2333 2024-04-09 11:51:28.000000 trade_database_manager-0.0.1.dev4/README.md
+-rw-rw-rw-   0        0        0     1614 2024-04-27 03:08:33.000000 trade_database_manager-0.0.1.dev4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-27 03:09:37.756497 trade_database_manager-0.0.1.dev4/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-04-22 12:39:40.000000 trade_database_manager-0.0.1.dev4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:09:37.744497 trade_database_manager-0.0.1.dev4/trade_database_manager/
+-rw-rw-rw-   0        0        0        0 2023-12-24 12:22:34.000000 trade_database_manager-0.0.1.dev4/trade_database_manager/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-12-24 14:33:56.000000 trade_database_manager-0.0.1.dev4/trade_database_manager/config.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:09:37.749497 trade_database_manager-0.0.1.dev4/trade_database_manager/core/
+-rw-rw-rw-   0        0        0        0 2023-12-24 12:22:34.000000 trade_database_manager-0.0.1.dev4/trade_database_manager/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:09:37.749497 trade_database_manager-0.0.1.dev4/trade_database_manager/core/kdb/
+-rw-rw-rw-   0        0        0        0 2023-12-24 12:22:34.000000 trade_database_manager-0.0.1.dev4/trade_database_manager/core/kdb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:09:37.751497 trade_database_manager-0.0.1.dev4/trade_database_manager/core/sql/
+-rw-rw-rw-   0        0        0        0 2023-12-24 12:22:34.000000 trade_database_manager-0.0.1.dev4/trade_database_manager/core/sql/__init__.py
+-rw-rw-rw-   0        0        0    13485 2024-04-27 02:59:53.000000 trade_database_manager-0.0.1.dev4/trade_database_manager/core/sql/sqlmanager.py
+-rw-rw-rw-   0        0        0        0 2023-12-24 12:22:34.000000 trade_database_manager-0.0.1.dev4/trade_database_manager/core/sql/sqlreader.py
+-rw-rw-rw-   0        0        0        0 2023-12-24 12:22:34.000000 trade_database_manager-0.0.1.dev4/trade_database_manager/core/sql/sqlwriter.py
+-rw-rw-rw-   0        0        0      524 2024-04-22 12:39:40.000000 trade_database_manager-0.0.1.dev4/trade_database_manager/core/typedefs.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:09:37.753497 trade_database_manager-0.0.1.dev4/trade_database_manager/manager/
+-rw-rw-rw-   0        0        0      188 2024-04-27 02:59:53.000000 trade_database_manager-0.0.1.dev4/trade_database_manager/manager/__init__.py
+-rw-rw-rw-   0        0        0      601 2024-04-22 12:39:40.000000 trade_database_manager-0.0.1.dev4/trade_database_manager/manager/fields_data_type.py
+-rw-rw-rw-   0        0        0    10051 2024-04-27 02:59:53.000000 trade_database_manager-0.0.1.dev4/trade_database_manager/manager/metadata_sql.py
+-rw-rw-rw-   0        0        0      910 2024-04-22 12:39:40.000000 trade_database_manager-0.0.1.dev4/trade_database_manager/manager/typedefs.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:09:37.754497 trade_database_manager-0.0.1.dev4/trade_database_manager.egg-info/
+-rw-rw-rw-   0        0        0     3205 2024-04-27 03:09:37.000000 trade_database_manager-0.0.1.dev4/trade_database_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      826 2024-04-27 03:09:37.000000 trade_database_manager-0.0.1.dev4/trade_database_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 03:09:37.000000 trade_database_manager-0.0.1.dev4/trade_database_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-27 03:09:37.000000 trade_database_manager-0.0.1.dev4/trade_database_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-04-27 03:09:37.000000 trade_database_manager-0.0.1.dev4/trade_database_manager.egg-info/top_level.txt
```

### Comparing `trade_database_manager-0.0.1.dev2/LICENSE` & `trade_database_manager-0.0.1.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `trade_database_manager-0.0.1.dev2/PKG-INFO` & `trade_database_manager-0.0.1.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trade_database_manager
-Version: 0.0.1.dev2
+Version: 0.0.1.dev4
 Summary: A wrapper of kdb and sql for convenient trade data management.
 Author-email: "Y.Q. Cui" <qianyun210603@hotmail.com>
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trade_database_manager Version: 0.0.1.dev2 Summary:
+Metadata-Version: 2.1 Name: trade_database_manager Version: 0.0.1.dev4 Summary:
 A wrapper of kdb and sql for convenient trade data management. Author-email:
 "Y.Q. Cui"
 hotmail.com> Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: GNU Affero General Public License v3 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `trade_database_manager-0.0.1.dev2/README.md` & `trade_database_manager-0.0.1.dev4/README.md`

 * *Files identical despite different names*

### Comparing `trade_database_manager-0.0.1.dev2/pyproject.toml` & `trade_database_manager-0.0.1.dev4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "trade_database_manager"
-version = "0.0.1.dev2"
+version = "0.0.1.dev4"
 description = "A wrapper of kdb and sql for convenient trade data management."
 readme = "README.md"
 authors = [
     {name = "Y.Q. Cui", email = "qianyun210603@hotmail.com"},
 ]
 dependencies = ["pandas>=2.0.0", "numpy", "ruamel.yaml", "sqlalchemy", "psycopg2"]
 classifiers = [
@@ -39,7 +39,11 @@
 [tool.black]
 line-length = 120
 target-version = ['py310']
 
 [tool.isort]
 profile = "black"
 line_length = 120
+
+[tool.flake8]
+max-line-length = 120
+ignore = "E203,E501,W503"
```

### Comparing `trade_database_manager-0.0.1.dev2/trade_database_manager/core/sql/sqlmanager.py` & `trade_database_manager-0.0.1.dev4/trade_database_manager/core/sql/sqlmanager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from collections.abc import Container
 from functools import partial, reduce
 from typing import Any, Literal, Sequence, Type, Union
 
 import pandas as pd
-from sqlalchemy import Float, Index, Integer, MetaData, String, Table, create_engine, inspect, select, sql, text
+from sqlalchemy import REAL, Index, Integer, MetaData, String, Table, create_engine, inspect, select, sql, text
 from sqlalchemy.dialects.postgresql import insert
 
 from ...config import CONFIG
 from ..typedefs import FILTERFIELD_TYPE, QUERYFIELD_TYPE
 
 
 def _insert_on_conflict_update(table, conn, keys, data_iter, indexes):
@@ -23,44 +23,74 @@
     data = [dict(zip(keys, row)) for row in data_iter]
     stmt = insert(table.table).values(data).on_conflict_do_nothing(index_elements=keys)
     result = conn.execute(stmt)
     return result.rowcount
 
 
 class SqlManager:
+    """
+    This class is used to manage SQL operations.
+
+    :ivar sqlalchemy.engine.Engine engine: An instance of the SQLAlchemy Engine class for executing SQL operations.
+    """
+
     def __init__(self):
         self.engine = create_engine(CONFIG["sqlconnstr"])
 
     def _execute(self, sql_executable: Union[str, sql.base.Executable]) -> Any:
         if isinstance(sql_executable, str):
             sql_executable = text(sql_executable)
         with self.engine.begin() as conn:
             return conn.execute(sql_executable)
 
     def add_index(self, table_name: str, columns: Union[str, list[str]], unique: bool = True):
+        """
+        Adds an index to a table.
+
+        :param table_name: The name of the table to add the index to.
+        :type table_name: str
+        :param columns: The column(s) to include in the index. It can be a single column name or a list of column names.
+        :type columns: Union[str, list[str]]
+        :param unique: Whether the index should enforce unique values. Defaults to True.
+        :type unique: bool
+        """
         if isinstance(columns, str):
             columns = [columns]
 
         index_name = f"uix_{table_name}_{'_'.join(columns)}"
-        columns_str = ", ".join(columns)
-        unique_str = "UNIQUE" if unique else ""
         table_meta = MetaData()
         table = Table(table_name, table_meta, autoload_with=self.engine)
         columns = [getattr(table.c, colname) for colname in columns if colname in table.c.keys()]
         index = Index(index_name, *columns, unique=unique)
         index.create(bind=self.engine)
 
     def insert(
         self,
         table_name: str,
         df: pd.DataFrame,
         upsert: bool = True,
         other_unique_index_columns: Sequence[str] = (),
         other_non_unique_index_columns: Sequence[str] = (),
     ):
+        """
+        Inserts data into a table.
+
+        :param table_name: The name of the table to insert data into.
+        :type table_name: str
+        :param df: The data to insert. It should be a DataFrame where the column names match the table columns.
+        :type df: pd.DataFrame
+        :param upsert: Whether to update the table if the data already exists. Defaults to True.
+        :type upsert: bool
+        :param other_unique_index_columns: Other columns to enforce unique values on. Defaults to an empty sequence.
+        :type other_unique_index_columns: Sequence[str]
+        :param other_non_unique_index_columns: Other columns to add non-unique indexes to. Defaults to an empty sequence.
+        :type other_non_unique_index_columns: Sequence[str]
+        :return: The number of rows inserted.
+        :rtype: int
+        """
         if_exists: Literal["replace", "append"] = "append"
         inspector = inspect(self.engine)
         new_table = not inspector.has_table(table_name)
         method = partial(_insert_on_conflict_update, indexes=df.index.names) if upsert and not new_table else None
         num_rows = df.to_sql(
             table_name,
             self.engine,
@@ -74,33 +104,63 @@
             for column in other_unique_index_columns:
                 self.add_index(table_name, column, unique=True)
             for column in other_non_unique_index_columns:
                 self.add_index(table_name, column, unique=False)
         return num_rows
 
     def _convert_to_sqlalchemy_type(self, column_type: Type, **kwargs):
-        if isinstance(column_type, str):
-            column_type = type(column_type)
-        if column_type == str:
+        if isinstance(column_type, type):
+            column_type = column_type.__name__
+        if column_type == "str":
             return String(**kwargs)
-        if column_type == int:
+        if column_type == "int":
             return Integer()
-        if column_type == float:
-            return Float()
+        if column_type == "float":
+            return REAL()
         raise ValueError(f"Unsupported column type {column_type}")
 
     def insert_column(self, table_name: str, column_name: str, column_type: Union[str, Type], type_kwargs: dict = None):
+        """
+        Inserts a new column into a table.
+
+        :param table_name: The name of the table to insert the column into.
+        :type table_name: str
+        :param column_name: The name of the new column.
+        :type column_name: str
+        :param column_type: The data type of the new column. It can be a string or a Python type.
+        :type column_type: Union[str, Type]
+        :param type_kwargs: Additional keyword arguments for the data type. Defaults to None.
+        :type type_kwargs: dict, optional
+        """
         type_kwargs = type_kwargs or {}
         sql_code = f"ALTER TABLE {table_name} ADD COLUMN {column_name} {str(self._convert_to_sqlalchemy_type(column_type, **type_kwargs))}"
         self._execute(sql_code)
 
     def delete_column(self, table_name: str, column_name: str):
+        """
+        Deletes a column from a table.
+
+        :param table_name: The name of the table to delete the column from.
+        :type table_name: str
+        :param column_name: The name of the column to delete.
+        :type column_name: str
+        """
         self._execute(f"ALTER TABLE {table_name} DROP COLUMN {column_name}")
 
     def rename_column(self, table_name: str, old_column_name: str, new_column_name: str):
+        """
+        Renames a column in a table.
+
+        :param table_name: The name of the table containing the column to rename.
+        :type table_name: str
+        :param old_column_name: The current name of the column.
+        :type old_column_name: str
+        :param new_column_name: The new name for the column.
+        :type new_column_name: str
+        """
         # check if any index is referring to the column
         sql_code = f"SELECT indexname, indexdef FROM pg_indexes WHERE indexdef LIKE '%%(%%{old_column_name}%%)%%' and tablename = '{table_name}'"
         index_refering_column = dict(self.engine.execute(sql_code).fetchall())
 
         # drop indexes referring to the column
         for index_name in index_refering_column:
             self._execute(f"DROP INDEX IF EXISTS {index_name}")
@@ -150,14 +210,27 @@
                 ]
             )
         stmt = stmt.where(sql.and_(*conditions))
         res = self._execute(stmt)
         return pd.DataFrame(res.fetchall(), columns=res.keys())
 
     def read_data(self, table_name: str, query_fields: QUERYFIELD_TYPE = "*", filter_fields=None):
+        """
+        Reads data from a table.
+
+        :param table_name: The name of the table to read data from.
+        :type table_name: str
+        :param query_fields: The fields to query. By default, it queries all fields. Defaults to "*".
+        :type query_fields: QUERYFIELD_TYPE, optional
+        :param filter_fields: Additional fields to filter by. The keys are the field names and the values are the filter values. Defaults to None.
+        :type filter_fields: dict, optional
+        :return: A DataFrame containing the queried data.
+        :rtype: pd.DataFrame
+        """
+
         meta = MetaData()
         table = Table(table_name, meta, autoload_with=self.engine)
 
         if query_fields != "*":
             query_fields = [table.columns[field] for field in query_fields]
             stmt = select(*query_fields)
         else:
@@ -173,23 +246,38 @@
                 )
                 for field, filter_values in filter_fields.items()
             ]
             stmt = stmt.where(sql.and_(*conditions))
 
         # cannot use pandas.read_sql here as it discards timezone info
         res = self._execute(stmt)
+        pd.read_sql_query()
         return pd.DataFrame(res.fetchall(), columns=res.keys())
 
     def read_data_across_tables(
         self,
         table_names: Sequence[str],
         joined_columns: Sequence[str],
         query_fields: QUERYFIELD_TYPE = "*",
         filter_fields: FILTERFIELD_TYPE = None,
     ):
+        """
+        Reads data from multiple tables.
+
+        :param table_names: The names of the tables to read data from.
+        :type table_names: Sequence[str]
+        :param joined_columns: The columns to join the tables on.
+        :type joined_columns: Sequence[str]
+        :param query_fields: The fields to query. By default, it queries all fields. Defaults to "*".
+        :type query_fields: QUERYFIELD_TYPE, optional
+        :param filter_fields: Additional fields to filter by. The keys are the field names and the values are the filter values. Defaults to None.
+        :type filter_fields: FILTERFIELD_TYPE, optional
+        :return: A DataFrame containing the queried data.
+        :rtype: pd.DataFrame
+        """
         meta = MetaData()
         tables = {table_name: Table(table_name, meta, autoload_with=self.engine) for table_name in table_names}
 
         joined_table = reduce(
             lambda x, y: x.join(y, sql.and_(*[x.columns[col] == y.columns[col] for col in joined_columns])),
             tables.values(),
         )
```

### Comparing `trade_database_manager-0.0.1.dev2/trade_database_manager/core/typedefs.py` & `trade_database_manager-0.0.1.dev4/trade_database_manager/core/typedefs.py`

 * *Files identical despite different names*

### Comparing `trade_database_manager-0.0.1.dev2/trade_database_manager/manager/fields_data_type.py` & `trade_database_manager-0.0.1.dev4/trade_database_manager/manager/fields_data_type.py`

 * *Files identical despite different names*

### Comparing `trade_database_manager-0.0.1.dev2/trade_database_manager/manager/typedefs.py` & `trade_database_manager-0.0.1.dev4/trade_database_manager/manager/typedefs.py`

 * *Files identical despite different names*

### Comparing `trade_database_manager-0.0.1.dev2/trade_database_manager.egg-info/PKG-INFO` & `trade_database_manager-0.0.1.dev4/trade_database_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trade_database_manager
-Version: 0.0.1.dev2
+Version: 0.0.1.dev4
 Summary: A wrapper of kdb and sql for convenient trade data management.
 Author-email: "Y.Q. Cui" <qianyun210603@hotmail.com>
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trade_database_manager Version: 0.0.1.dev2 Summary:
+Metadata-Version: 2.1 Name: trade_database_manager Version: 0.0.1.dev4 Summary:
 A wrapper of kdb and sql for convenient trade data management. Author-email:
 "Y.Q. Cui"
 hotmail.com> Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: GNU Affero General Public License v3 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `trade_database_manager-0.0.1.dev2/trade_database_manager.egg-info/SOURCES.txt` & `trade_database_manager-0.0.1.dev4/trade_database_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

