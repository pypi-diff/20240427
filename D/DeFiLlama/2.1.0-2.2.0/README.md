# Comparing `tmp/DeFiLlama-2.1.0.tar.gz` & `tmp/defillama-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeFiLlama-2.1.0.tar", last modified: Thu Apr 11 15:06:33 2024, max compression
+gzip compressed data, was "defillama-2.2.0.tar", last modified: Sat Apr 27 16:49:34 2024, max compression
```

## Comparing `DeFiLlama-2.1.0.tar` & `defillama-2.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:06:33.819090 DeFiLlama-2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:06:33.815089 DeFiLlama-2.1.0/DeFiLlama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-11 15:06:33.000000 DeFiLlama-2.1.0/DeFiLlama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-11 15:06:33.000000 DeFiLlama-2.1.0/DeFiLlama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:06:33.000000 DeFiLlama-2.1.0/DeFiLlama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 15:06:33.000000 DeFiLlama-2.1.0/DeFiLlama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 15:06:33.000000 DeFiLlama-2.1.0/DeFiLlama.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 15:06:26.000000 DeFiLlama-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-11 15:06:33.815089 DeFiLlama-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-11 15:06:26.000000 DeFiLlama-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:06:33.815089 DeFiLlama-2.1.0/defillama/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-11 15:06:26.000000 DeFiLlama-2.1.0/defillama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-11 15:06:26.000000 DeFiLlama-2.1.0/defillama/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-11 15:06:26.000000 DeFiLlama-2.1.0/defillama/defillama.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:06:33.819090 DeFiLlama-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-11 15:06:26.000000 DeFiLlama-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:06:33.815089 DeFiLlama-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-11 15:06:26.000000 DeFiLlama-2.1.0/tests/test_defillama.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:49:34.920696 defillama-2.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:49:34.920696 defillama-2.2.0/DeFiLlama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-27 16:49:34.000000 defillama-2.2.0/DeFiLlama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-27 16:49:34.000000 defillama-2.2.0/DeFiLlama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:49:34.000000 defillama-2.2.0/DeFiLlama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-27 16:49:34.000000 defillama-2.2.0/DeFiLlama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-27 16:49:34.000000 defillama-2.2.0/DeFiLlama.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 16:49:24.000000 defillama-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-27 16:49:34.920696 defillama-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-27 16:49:24.000000 defillama-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:49:34.916696 defillama-2.2.0/defillama/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-27 16:49:24.000000 defillama-2.2.0/defillama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-27 16:49:24.000000 defillama-2.2.0/defillama/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-04-27 16:49:24.000000 defillama-2.2.0/defillama/defillama.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 16:49:34.920696 defillama-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-27 16:49:24.000000 defillama-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:49:34.920696 defillama-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-27 16:49:24.000000 defillama-2.2.0/tests/test_defillama.py
```

### Comparing `DeFiLlama-2.1.0/DeFiLlama.egg-info/PKG-INFO` & `defillama-2.2.0/DeFiLlama.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeFiLlama
-Version: 2.1.0
+Version: 2.2.0
 Summary: Unofficial DeFi Llama API client.
 Home-page: https://github.com/itzmestar/DeFiLlama
 Author: Tarique Anwer
 Author-email: itzmetariq@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `DeFiLlama-2.1.0/LICENSE` & `defillama-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DeFiLlama-2.1.0/PKG-INFO` & `defillama-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeFiLlama
-Version: 2.1.0
+Version: 2.2.0
 Summary: Unofficial DeFi Llama API client.
 Home-page: https://github.com/itzmestar/DeFiLlama
 Author: Tarique Anwer
 Author-email: itzmetariq@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `DeFiLlama-2.1.0/README.md` & `defillama-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `DeFiLlama-2.1.0/defillama/defillama.py` & `defillama-2.2.0/defillama/defillama.py`

 * *Files 21% similar despite different names*

```diff
@@ -113,14 +113,103 @@
         
         :return: JSON response
         """
         path = f'/v2/chains'
 
         return self._get(path)
 
+    # ##### Coins EPs ###### #
+    def get_token_current_prices(self, coins: str, searchWidth: str = '4h'):
+        """
+        Get current prices of tokens by contract address
+        """
+        path = f'/prices/current/{coins}'
+        params = {
+            'searchWidth': searchWidth
+        }
+
+        return self._get(path, params=params)
+
+    def get_token_historical_prices(self, coins: str, timestamp: int, searchWidth: str = '4h'):
+        """
+        Get historical prices of tokens by contract address
+        """
+        path = f'/prices/historical/{timestamp}/{coins}'
+        params = {
+            'searchWidth': searchWidth
+        }
+
+        return self._get(path, params=params)
+
+    def get_batch_historical_prices(self, coins: str, searchWidth: str = '600'):
+        """
+        Get historical prices of tokens by contract address
+        """
+        path = f'https://coins.llama.fi/batchHistorical'
+        params = {
+            'coins': coins,
+            'searchWidth': searchWidth
+        }
+
+        return self._get(path, params=params, full_url=True)
+
+    def get_token_prices_at_intervals(
+            self,
+            coins: str,
+            start: int,
+            end: int,
+            span: int = 0,
+            period: str = '2d',
+            searchWidth: str = '600'
+    ):
+        """
+        Get token prices at regular time intervals
+        """
+        path = f"/chart/{coins}"
+
+        params = {
+            'start': start,
+            'end': end,
+            'span': span,
+            'period': period,
+            'searchWidth': searchWidth
+        }
+
+        return self._get(path, params=params)
+
+    def get_percentage_price_change(self, coins: str, timestamp: int, lookForward: bool = False, period: str = '3w'):
+        """
+        Get percentage change in price over time
+        """
+        path = f"/percentage/{coins}"
+
+        params = {
+            'timestamp': timestamp,
+            'lookForward': lookForward,
+            'period': period
+        }
+
+        return self._get(path, params=params)
+
+    def get_earliest_ts_price(self, coins: str):
+        """
+        Get earliest timestamp price record for coins
+        """
+        path = f"/percentage/{coins}"
+
+        return self._get(path)
+
+    def get_closest_ts_block(self, chain: str, timestamp: int):
+        """
+        Get the closest block to a timestamp
+        """
+        path = f"/block/{chain}/{timestamp}"
+
+        return self._get(path)
+
     # ##### Yields EPs ###### #
 
     def get_pools(self):
         """
         Get the latest data for all pools
         """
         path = 'https://yields.llama.fi/pools'
@@ -208,7 +297,46 @@
         """
         path = f'/summary/options/{protocol}'
         params = {
             'dataType': dataType
         }
 
         return self._get(path, params=params)
+
+    # ##### Fees & Revenue EPs ###### #
+
+    def get_fees(self, excludeTotalDataChart=True, excludeTotalDataChartBreakdown=True, dataType='dailyFees'):
+        """
+                list all protocols along with summaries of their fees & revenue & dataType history data
+        """
+        path = f'/overview/fees'
+        params = {
+            'excludeTotalDataChart': excludeTotalDataChart,
+            'excludeTotalDataChartBreakdown': excludeTotalDataChartBreakdown,
+            'dataType': dataType
+        }
+
+        return self._get(path, params=params)
+
+    def get_fees_chain(self, chain, excludeTotalDataChart=True, excludeTotalDataChartBreakdown=True, dataType='dailyFees'):
+        """
+            list all protocols along with summaries of their fees & revenue & dataType history data by chain
+        """
+        path = f'/overview/fees/{chain}'
+        params = {
+            'excludeTotalDataChart': excludeTotalDataChart,
+            'excludeTotalDataChartBreakdown': excludeTotalDataChartBreakdown,
+            'dataType': dataType
+        }
+
+        return self._get(path, params=params)
+
+    def get_fees_protocol(self, protocol, dataType='dailyFees'):
+        """
+            Get summary of protocol fees and revenue with historical data
+        """
+        path = f'/overview/fees/{protocol}'
+        params = {
+            'dataType': dataType
+        }
+
+        return self._get(path, params=params)
```

### Comparing `DeFiLlama-2.1.0/setup.py` & `defillama-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `DeFiLlama-2.1.0/tests/test_defillama.py` & `defillama-2.2.0/tests/test_defillama.py`

 * *Files identical despite different names*

