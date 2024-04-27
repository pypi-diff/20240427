# Comparing `tmp/bifabrik-0.6.1.tar.gz` & `tmp/bifabrik-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bifabrik-0.6.1.tar", max compression
+gzip compressed data, was "bifabrik-0.7.0.tar", max compression
```

## Comparing `bifabrik-0.6.1.tar` & `bifabrik-0.7.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
--rw-r--r--   0        0        0     1073 2024-04-11 19:20:20.724360 bifabrik-0.6.1/LICENSE
--rw-r--r--   0        0        0     4792 2024-04-11 19:20:20.724360 bifabrik-0.6.1/README.md
--rw-r--r--   0        0        0      575 2024-04-11 19:20:20.728360 bifabrik-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     5095 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/__init__.py
--rw-r--r--   0        0        0     2896 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/base/Pipeline.py
--rw-r--r--   0        0        0     1631 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/base/Task.py
--rw-r--r--   0        0        0     4899 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/CompleteConfiguration.py
--rw-r--r--   0        0        0        0 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/Configuration.py
--rw-r--r--   0        0        0      755 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/CsvSourceConfiguration.py
--rw-r--r--   0        0        0      570 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/DataDestinationConfigurationBase.py
--rw-r--r--   0        0        0      525 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/DataSourceConfigurationBase.py
--rw-r--r--   0        0        0      729 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/ExcelSourceConfiguration.py
--rw-r--r--   0        0        0      715 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/JsonSourceConfiguration.py
--rw-r--r--   0        0        0      512 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/SharePointListSourceConfiguration.py
--rw-r--r--   0        0        0      605 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/TableDestinationConfiguration.py
--rw-r--r--   0        0        0        0 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/__init__.py
--rw-r--r--   0        0        0     5045 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/engine/ConfigContainer.py
--rw-r--r--   0        0        0      411 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/engine/Configuration.py
--rw-r--r--   0        0        0     3895 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/CsvConfiguration.py
--rw-r--r--   0        0        0     1139 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/DestinationStorageConfiguration.py
--rw-r--r--   0        0        0     4700 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/ExcelConfiguration.py
--rw-r--r--   0        0        0     2699 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/FileSourceConfiguration.py
--rw-r--r--   0        0        0     7254 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/JsonConfiguration.py
--rw-r--r--   0        0        0     3782 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/LogConfiguration.py
--rw-r--r--   0        0        0     2159 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py
--rw-r--r--   0        0        0     1472 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/SecurityConfiguration.py
--rw-r--r--   0        0        0     1049 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/SourceStorageConfiguration.py
--rw-r--r--   0        0        0     4638 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/cfg/specific/TableConfiguration.py
--rw-r--r--   0        0        0      931 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/dst/DataDestination.py
--rw-r--r--   0        0        0      909 2024-04-11 19:20:20.728360 bifabrik-0.6.1/src/bifabrik/dst/PandasDfDestination.py
--rw-r--r--   0        0        0      834 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/dst/SparkDfDestination.py
--rw-r--r--   0        0        0    13819 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/dst/TableDestination.py
--rw-r--r--   0        0        0        0 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/dst/__init__.py
--rw-r--r--   0        0        0     3916 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/src/CsvSource.py
--rw-r--r--   0        0        0     2177 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/src/DataSource.py
--rw-r--r--   0        0        0     3925 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/src/ExcelSource.py
--rw-r--r--   0        0        0     3447 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/src/JsonSource.py
--rw-r--r--   0        0        0      919 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/src/PandasDfSource.py
--rw-r--r--   0        0        0     3588 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/src/SharePointListSource.py
--rw-r--r--   0        0        0      914 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/src/SparkDfSource.py
--rw-r--r--   0        0        0      932 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/src/SqlSource.py
--rw-r--r--   0        0        0        0 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/src/__init__.py
--rw-r--r--   0        0        0     2091 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/tsf/DataTransformation.py
--rw-r--r--   0        0        0     1086 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/tsf/PandasDfTransformation.py
--rw-r--r--   0        0        0      916 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/tsf/SparkDfTransformation.py
--rw-r--r--   0        0        0    15243 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/utils/fsUtils.py
--rw-r--r--   0        0        0     7064 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/utils/log.py
--rw-r--r--   0        0        0     2500 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/utils/tableUtils.py
--rw-r--r--   0        0        0     6158 2024-04-11 19:20:20.732360 bifabrik-0.6.1/src/bifabrik/utils/tmslUtils.py
--rw-r--r--   0        0        0     5556 1970-01-01 00:00:00.000000 bifabrik-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-27 16:34:27.127625 bifabrik-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4792 2024-04-27 16:34:27.127625 bifabrik-0.7.0/README.md
+-rw-r--r--   0        0        0      575 2024-04-27 16:34:27.131625 bifabrik-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6451 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/__init__.py
+-rw-r--r--   0        0        0     2896 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/base/Pipeline.py
+-rw-r--r--   0        0        0     1631 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/base/Task.py
+-rw-r--r--   0        0        0     4899 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/CompleteConfiguration.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/Configuration.py
+-rw-r--r--   0        0        0      755 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/CsvSourceConfiguration.py
+-rw-r--r--   0        0        0      570 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/DataDestinationConfigurationBase.py
+-rw-r--r--   0        0        0      525 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/DataSourceConfigurationBase.py
+-rw-r--r--   0        0        0      729 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/ExcelSourceConfiguration.py
+-rw-r--r--   0        0        0      715 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/JsonSourceConfiguration.py
+-rw-r--r--   0        0        0      512 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/SharePointListSourceConfiguration.py
+-rw-r--r--   0        0        0      605 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/TableDestinationConfiguration.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/__init__.py
+-rw-r--r--   0        0        0     5045 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/engine/ConfigContainer.py
+-rw-r--r--   0        0        0      411 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/engine/Configuration.py
+-rw-r--r--   0        0        0     3895 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/CsvConfiguration.py
+-rw-r--r--   0        0        0     2617 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/DestinationStorageConfiguration.py
+-rw-r--r--   0        0        0     4700 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/ExcelConfiguration.py
+-rw-r--r--   0        0        0     2699 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/FileSourceConfiguration.py
+-rw-r--r--   0        0        0     7254 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/JsonConfiguration.py
+-rw-r--r--   0        0        0     3782 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/LogConfiguration.py
+-rw-r--r--   0        0        0     2159 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py
+-rw-r--r--   0        0        0     2350 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/SecurityConfiguration.py
+-rw-r--r--   0        0        0     2421 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/SourceStorageConfiguration.py
+-rw-r--r--   0        0        0     4673 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/TableConfiguration.py
+-rw-r--r--   0        0        0      931 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/dst/DataDestination.py
+-rw-r--r--   0        0        0    13828 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/dst/LakehouseTableDestination.py
+-rw-r--r--   0        0        0      909 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/dst/PandasDfDestination.py
+-rw-r--r--   0        0        0      834 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/dst/SparkDfDestination.py
+-rw-r--r--   0        0        0    24469 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/dst/WarehouseTableDestination.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/dst/__init__.py
+-rw-r--r--   0        0        0     3916 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/CsvSource.py
+-rw-r--r--   0        0        0     3803 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/DataSource.py
+-rw-r--r--   0        0        0     3925 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/ExcelSource.py
+-rw-r--r--   0        0        0     3447 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/JsonSource.py
+-rw-r--r--   0        0        0      919 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/PandasDfSource.py
+-rw-r--r--   0        0        0     3588 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/SharePointListSource.py
+-rw-r--r--   0        0        0      914 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/SparkDfSource.py
+-rw-r--r--   0        0        0      941 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/SparkSqlSource.py
+-rw-r--r--   0        0        0     2844 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/WarehouseSqlSource.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/__init__.py
+-rw-r--r--   0        0        0     3548 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/tsf/DataTransformation.py
+-rw-r--r--   0        0        0     1086 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/tsf/PandasDfTransformation.py
+-rw-r--r--   0        0        0      916 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/tsf/SparkDfTransformation.py
+-rw-r--r--   0        0        0    15243 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/utils/fsUtils.py
+-rw-r--r--   0        0        0     7064 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/utils/log.py
+-rw-r--r--   0        0        0     2500 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/utils/tableUtils.py
+-rw-r--r--   0        0        0     6158 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/utils/tmslUtils.py
+-rw-r--r--   0        0        0     5556 1970-01-01 00:00:00.000000 bifabrik-0.7.0/PKG-INFO
```

### Comparing `bifabrik-0.6.1/LICENSE` & `bifabrik-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/README.md` & `bifabrik-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/pyproject.toml` & `bifabrik-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bifabrik"
-version = "0.6.1"
+version = "0.7.0"
 description = "Microsoft Fabric ETL toolbox"
 authors = ["Radovan Jankovič"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://rjankovic.github.io/bifabrik/"
 documentation = "https://rjankovic.github.io/bifabrik/"
 repository = "https://github.com/rjankovic/bifabrik/"
```

### Comparing `bifabrik-0.6.1/src/bifabrik/__init__.py` & `bifabrik-0.7.0/src/bifabrik/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     >>> bif.fromSql("SELECT * FROM OrdersTable LIMIT 10").toTable('TenOrders').save()
 """
 
 from bifabrik.src.CsvSource import CsvSource
 from bifabrik.src.ExcelSource import ExcelSource
 from bifabrik.src.SharePointListSource import SharePointListSource
 from bifabrik.src.JsonSource import JsonSource
-from bifabrik.src.SqlSource import SqlSource
+from bifabrik.src.SparkSqlSource import SparkSqlSource
+from bifabrik.src.WarehouseSqlSource import WarehouseSqlSource
 from bifabrik.src.SparkDfSource import SparkDfSource
 from bifabrik.src.PandasDfSource import PandasDfSource
 from bifabrik.cfg.CompleteConfiguration import CompleteConfiguration
 import bifabrik.utils.log as log
 from bifabrik.base.Pipeline import Pipeline
 import pyspark.sql.session as pss
 from pyspark.sql.dataframe import DataFrame as SparkDf
@@ -39,15 +40,15 @@
 __version__ = version("bifabrik")
 __loggername__ = "bifabrik_logger"
 
 #import bifabrik
 from bifabrik.utils.fsUtils import getDefaultLakehouseAbfsPath
 
 if getDefaultLakehouseAbfsPath() is None:
-    print('bifabrik warning: the notebook is not attached to a lakehouse - some features of bifabrik will not work correctly.')
+    print('bifabrik warning: the notebook is not attached to a lakehouse - some features will not work correctly.')
 
 
 #from bifabrik.base.Task import Task
 
 __spark = pss.SparkSession.builder.getOrCreate()
 __configuration = CompleteConfiguration()
         #self.__configuration.log.loggingEnabled = False
@@ -99,28 +100,61 @@
     >>> bif.fromExcel.path('ExcelData/factOrderLine.xlsx').sheetName('Sheet1').toTable('FactOrderLine').run()
     """
     ds = ExcelSource(__prepPipeline())
     ds.path(path)
     return ds
 
 
-def fromSql(query: str = None) -> SqlSource:
-    """Load the result of a SQL query to a table
+def fromSql(query: str = None) -> SparkSqlSource:
+    """Load the result of a SparkSQL query to a table
     
     Examples
     --------
     
     >>> import bifabrik as bif
     >>>
     >>> bif.fromSql('SELECT A, B, C FROM Table1 WHERE D = 1').toTable('Table2').run()
     """
-    ds = SqlSource(__prepPipeline())
+    return fromSparkSql(query)
+
+def fromSparkSql(query: str = None) -> SparkSqlSource:
+    """Load the result of a SparkSQL query to a table
+    
+    Examples
+    --------
+    
+    >>> import bifabrik as bif
+    >>>
+    >>> bif.fromSql('SELECT A, B, C FROM Table1 WHERE D = 1').toTable('Table2').run()
+    """
+    ds = SparkSqlSource(__prepPipeline())
     ds.query(query)
     return ds
 
+def fromWarehouseSql(query: str) -> WarehouseSqlSource:
+    """Load the result of a TSQL query from a Fabric warehouse to a table
+    Service principal authentication is used to connect to the warehouse. This needs to be configured as below
+    
+    Examples
+    --------
+    >>> import bifabrik as bif
+    >>>
+    >>> bif.config.security.keyVaultUrl = 'https://kv-contoso.vault.azure.net/'
+    >>> bif.config.security.servicePrincipalClientId = '56712345-1234-7890-abcd-abcd12344d14'
+    >>> bif.config.security.servicePrincipalClientSecretKVSecretName = 'contoso-clientSecret'
+    >>> bif.config.sourceStorage.sourceWarehouseConnectionString = 'dxtxxxxxxbue.datawarehouse.fabric.microsoft.com'
+    >>>
+    >>> bif.fromWarehouseSql('''
+    >>> SELECT CountryOrRegion, Year, PublicHolidayCount FROM [DW1].[dbo].[HolidayCountsYearly]
+    >>> ''').toTable('HolidayCountsYearlyFromDW').run()
+    
+    """
+    ds = WarehouseSqlSource(__prepPipeline(), query)
+    return ds
+
 def fromSparkDf(df: SparkDf) -> SparkDfSource:
     """Use spark dataframe as source
     
     Examples
     --------
     
     >>> import bifabrik as bif
```

### Comparing `bifabrik-0.6.1/src/bifabrik/base/Pipeline.py` & `bifabrik-0.7.0/src/bifabrik/base/Pipeline.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/base/Task.py` & `bifabrik-0.7.0/src/bifabrik/base/Task.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/cfg/CompleteConfiguration.py` & `bifabrik-0.7.0/src/bifabrik/cfg/CompleteConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/cfg/CsvSourceConfiguration.py` & `bifabrik-0.7.0/src/bifabrik/cfg/CsvSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/cfg/DataDestinationConfigurationBase.py` & `bifabrik-0.7.0/src/bifabrik/cfg/DataDestinationConfigurationBase.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/cfg/DataSourceConfigurationBase.py` & `bifabrik-0.7.0/src/bifabrik/cfg/DataSourceConfigurationBase.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/cfg/ExcelSourceConfiguration.py` & `bifabrik-0.7.0/src/bifabrik/cfg/ExcelSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/cfg/JsonSourceConfiguration.py` & `bifabrik-0.7.0/src/bifabrik/cfg/JsonSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/cfg/SharePointListSourceConfiguration.py` & `bifabrik-0.7.0/src/bifabrik/cfg/SharePointListSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/cfg/TableDestinationConfiguration.py` & `bifabrik-0.7.0/src/bifabrik/cfg/TableDestinationConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/cfg/engine/ConfigContainer.py` & `bifabrik-0.7.0/src/bifabrik/cfg/engine/ConfigContainer.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/cfg/specific/CsvConfiguration.py` & `bifabrik-0.7.0/src/bifabrik/cfg/specific/CsvConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/cfg/specific/ExcelConfiguration.py` & `bifabrik-0.7.0/src/bifabrik/cfg/specific/ExcelConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/cfg/specific/FileSourceConfiguration.py` & `bifabrik-0.7.0/src/bifabrik/cfg/specific/FileSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/cfg/specific/JsonConfiguration.py` & `bifabrik-0.7.0/src/bifabrik/cfg/specific/JsonConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/cfg/specific/LogConfiguration.py` & `bifabrik-0.7.0/src/bifabrik/cfg/specific/LogConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py` & `bifabrik-0.7.0/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/cfg/specific/SecurityConfiguration.py` & `bifabrik-0.7.0/src/bifabrik/cfg/specific/SecurityConfiguration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from bifabrik.cfg.engine.Configuration import Configuration
 from bifabrik.cfg.engine.Configuration import CfgProperty
 
 class SecurityConfiguration(Configuration):
-    """Credentials configuration, currently used in the SharePointListSource.
-    (Credentials aren't actually stored here, this configuration only refers to KeyVault secrets.)
+    """Credentials configuration, currently used for connecting to Fabric warehouses and the SharePointListSource.
+    (Passwords aren't actually stored here, this configuration only refers to KeyVault secrets.)
     """
     def __init__(self):
         self._explicitProps = {}
         self.__keyVaultUrl = None
         self.__loginKVSecretName = None
         self.__passwordKVSecretName = None
 
@@ -34,8 +34,26 @@
         """Secret in the Key Vault that contains the password
         """
         return self.__passwordKVSecretName
     @passwordKVSecretName.setter(key='passwordKVSecretName')
     def passwordKVSecretName(self, val):
         self.__passwordKVSecretName = val
 
+    @CfgProperty
+    def servicePrincipalClientId(self) -> str:
+        """Service principal used for connecting to Fabric warehouses
+        """
+        return self.__servicePrincipalClientId
+    @servicePrincipalClientId.setter(key='servicePrincipalClientId')
+    def servicePrincipalClientId(self, val):
+        self.__servicePrincipalClientId = val
+    
+    @CfgProperty
+    def servicePrincipalClientSecretKVSecretName(self) -> str:
+        """Secret in the Key Vault that contains the service principal's client secret
+        """
+        return self.__servicePrincipalClientSecretKVSecretName
+    @servicePrincipalClientSecretKVSecretName.setter(key='servicePrincipalClientSecretKVSecretName')
+    def servicePrincipalClientSecretKVSecretName(self, val):
+        self.__servicePrincipalClientSecretKVSecretName = val
+
```

### Comparing `bifabrik-0.6.1/src/bifabrik/cfg/specific/SourceStorageConfiguration.py` & `bifabrik-0.7.0/src/bifabrik/cfg/specific/SourceStorageConfiguration.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from bifabrik.cfg.engine.Configuration import Configuration
 from bifabrik.cfg.engine.Configuration import CfgProperty
 
 class SourceStorageConfiguration(Configuration):
-    """Defines the data source lakehouse. By default refers to the default lakehouse of the notebook.
+    """Defines the data source lakehouse or warehouse. By default refers to the default lakehouse of the notebook.
     """
     def __init__(self):
         self._explicitProps = {}
         self.__sourceWorkspace = None
         self.__sourceLakehouse = None
+        self.__sourceWarehouseConnectionString = None
+        self.__sourceWarehouseConnectionTimeout = 600
+        self.__sourceWarehouseName = None
 
     @CfgProperty
     def sourceWorkspace(self) -> str:
         """The workspace from which pipeline sources load data - ID or name
         """
         return self.__sourceWorkspace
     @sourceWorkspace.setter(key='sourceWorkspace')
@@ -21,8 +24,36 @@
     @CfgProperty
     def sourceLakehouse(self) -> str:
         """The lakehouse from which pipeline sources load data - ID or name
         """
         return self.__sourceLakehouse
     @sourceLakehouse.setter(key='sourceLakehouse')
     def sourceLakehouse(self, val):
-        self.__sourceLakehouse = val
+        self.__sourceLakehouse = val
+
+    @CfgProperty
+    def sourceWarehouseConnectionString(self) -> str:
+        """Connection string to the source Fabric warehouse (server name like dxt....datawarehouse.fabric.microsoft.com)
+        """
+        return self.__sourceWarehouseConnectionString
+    @sourceWarehouseConnectionString.setter(key='sourceWarehouseConnectionString')
+    def sourceWarehouseConnectionString(self, val):
+        self.__sourceWarehouseConnectionString = val
+
+    @CfgProperty
+    def sourceWarehouseConnectionTimeout(self) -> str:
+        """Warehouse ODBC connection timetout in seconds
+        default 600
+        """
+        return self.__sourceWarehouseConnectionTimeout
+    @sourceWarehouseConnectionTimeout.setter(key='sourceWarehouseConnectionTimeout')
+    def sourceWarehouseConnectionTimeout(self, val):
+        self.__sourceWarehouseConnectionTimeout = val
+
+    @CfgProperty
+    def sourceWarehouseName(self) -> str:
+        """Name of the warehouse from which the pipelines read data
+        """
+        return self.__sourceWarehouseName
+    @sourceWarehouseName.setter(key='sourceWarehouseName')
+    def sourceWarehouseName(self, val):
+        self.__sourceWarehouseName = val
```

### Comparing `bifabrik-0.6.1/src/bifabrik/cfg/specific/TableConfiguration.py` & `bifabrik-0.7.0/src/bifabrik/cfg/specific/TableConfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from bifabrik.cfg.engine.Configuration import Configuration
 from bifabrik.cfg.engine.Configuration import CfgProperty
 
 class TableConfiguration(Configuration):
-    """Configuration related to saving data to delta tables
+    """Configuration related to saving data to delta tables in a Fabric lakehouse or warehouse
     """
     def __init__(self):
         self._explicitProps = {}
         self.__watermarkColumn = None
         self.__increment = None
         self.__identityColumnPattern = None
         self.__insertDateColumn = None
```

### Comparing `bifabrik-0.6.1/src/bifabrik/dst/DataDestination.py` & `bifabrik-0.7.0/src/bifabrik/dst/DataDestination.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/dst/PandasDfDestination.py` & `bifabrik-0.7.0/src/bifabrik/dst/PandasDfDestination.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/dst/SparkDfDestination.py` & `bifabrik-0.7.0/src/bifabrik/dst/SparkDfDestination.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/dst/TableDestination.py` & `bifabrik-0.7.0/src/bifabrik/dst/LakehouseTableDestination.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pyspark.sql.functions import *
 from pyspark.sql.window import Window
 import time
 import datetime
 import notebookutils.mssparkutils.fs
 from bifabrik.utils import tableUtils as tu
 
-class TableDestination(DataDestination, TableDestinationConfiguration):
+class LakehouseTableDestination(DataDestination, TableDestinationConfiguration):
     """Saves data to a lakehouse table.
 
     Examples
     --------
     > import bifabrik as bif
     >
     > bif.fromSql.query('SELECT * FROM SomeTable').toTable('DestinationTable1').run()
@@ -224,15 +224,15 @@
         # print('non-key columns')
         # print(non_key_columns)
         
         if len(key_columns) == 0:
             raise Exception('No key columns set for merge increment. Please set the mergeKeyColumns property in destinationTable configuration to the list of column names.')
         
 
-        # todo: instead of SQL, use pyspark for cross-workspace ETL
+        # TODO: instead of SQL, use pyspark for cross-workspace ETL
         join_condition = " AND ".join([f"src.`{item}` = tgt.`{item}`" for item in key_columns])
         update_list = ", ".join([f"`{item}` = src.`{item}`" for item in non_key_columns])
         insert_list = ", ".join([f"`{item}`" for item in all_columns])
         insert_values = ", ".join([f"src.`{item}`" for item in all_columns])
         
         scd1_update = f"WHEN MATCHED THEN UPDATE SET \
             {update_list} "
```

### Comparing `bifabrik-0.6.1/src/bifabrik/src/CsvSource.py` & `bifabrik-0.7.0/src/bifabrik/src/CsvSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/src/ExcelSource.py` & `bifabrik-0.7.0/src/bifabrik/src/ExcelSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/src/JsonSource.py` & `bifabrik-0.7.0/src/bifabrik/src/JsonSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/src/PandasDfSource.py` & `bifabrik-0.7.0/src/bifabrik/src/PandasDfSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/src/SharePointListSource.py` & `bifabrik-0.7.0/src/bifabrik/src/SharePointListSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/src/SparkDfSource.py` & `bifabrik-0.7.0/src/bifabrik/src/SparkDfSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/src/SqlSource.py` & `bifabrik-0.7.0/src/bifabrik/src/SparkSqlSource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from bifabrik.src.DataSource import DataSource
 from pyspark.sql.dataframe import DataFrame
 
-class SqlSource(DataSource):
+class SparkSqlSource(DataSource):
     """SQL (SparkSQL) data source - executes a SparkSQL query
 
     Examples
     --------
     > import bifabrik as bif
     >
     > bif.fromSql.query('SELECT OrderId, CustomerId  FROM LH1.FactOrderLine WHERE ProductId = 791057').toTable('TransformedOrders1').run()
     """
-
+    
     def __init__(self, parentPipeline):
         super().__init__(parentPipeline)
         self._query = ""
     
     def __str__(self):
         return f'SQL source: {self._query}'
```

### Comparing `bifabrik-0.6.1/src/bifabrik/tsf/PandasDfTransformation.py` & `bifabrik-0.7.0/src/bifabrik/tsf/PandasDfTransformation.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/tsf/SparkDfTransformation.py` & `bifabrik-0.7.0/src/bifabrik/tsf/SparkDfTransformation.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/utils/fsUtils.py` & `bifabrik-0.7.0/src/bifabrik/utils/fsUtils.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/utils/log.py` & `bifabrik-0.7.0/src/bifabrik/utils/log.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/utils/tableUtils.py` & `bifabrik-0.7.0/src/bifabrik/utils/tableUtils.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/src/bifabrik/utils/tmslUtils.py` & `bifabrik-0.7.0/src/bifabrik/utils/tmslUtils.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.6.1/PKG-INFO` & `bifabrik-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bifabrik
-Version: 0.6.1
+Version: 0.7.0
 Summary: Microsoft Fabric ETL toolbox
 Home-page: https://rjankovic.github.io/bifabrik/
 License: MIT
 Author: Radovan Jankovič
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

