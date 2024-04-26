# Comparing `tmp/xian_py-0.1.6.tar.gz` & `tmp/xian_py-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xian_py-0.1.6.tar", max compression
+gzip compressed data, was "xian_py-0.1.7.tar", max compression
```

## Comparing `xian_py-0.1.6.tar` & `xian_py-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     4472 2024-02-21 22:59:58.766214 xian_py-0.1.6/README.md
--rw-r--r--   0        0        0      344 2024-04-12 12:11:45.288569 xian_py-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4755 2024-02-21 22:59:58.766680 xian_py-0.1.6/xian_py/encoding.py
--rw-r--r--   0        0        0      198 2024-04-10 23:20:44.689826 xian_py-0.1.6/xian_py/exception.py
--rw-r--r--   0        0        0     2320 2024-02-21 22:59:58.766767 xian_py-0.1.6/xian_py/formating.py
--rw-r--r--   0        0        0     4797 2024-04-12 11:07:12.108348 xian_py-0.1.6/xian_py/transactions.py
--rw-r--r--   0        0        0      387 2024-04-08 21:58:01.758197 xian_py-0.1.6/xian_py/utils.py
--rw-r--r--   0        0        0     1906 2024-02-21 22:59:58.767011 xian_py-0.1.6/xian_py/wallet.py
--rw-r--r--   0        0        0     7231 2024-04-12 11:45:10.473448 xian_py-0.1.6/xian_py/xian.py
--rw-r--r--   0        0        0     7299 2024-02-21 22:59:58.767235 xian_py-0.1.6/xian_py/xian_datetime.py
--rw-r--r--   0        0        0     4683 2024-02-21 22:59:58.767344 xian_py-0.1.6/xian_py/xian_decimal.py
--rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 xian_py-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     4472 2024-02-21 22:59:58.766214 xian_py-0.1.7/README.md
+-rw-r--r--   0        0        0      344 2024-04-26 23:47:01.673532 xian_py-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4755 2024-02-21 22:59:58.766680 xian_py-0.1.7/xian_py/encoding.py
+-rw-r--r--   0        0        0      198 2024-04-10 23:20:44.689826 xian_py-0.1.7/xian_py/exception.py
+-rw-r--r--   0        0        0     2320 2024-02-21 22:59:58.766767 xian_py-0.1.7/xian_py/formating.py
+-rw-r--r--   0        0        0     5329 2024-04-26 23:43:49.744182 xian_py-0.1.7/xian_py/transactions.py
+-rw-r--r--   0        0        0      387 2024-04-08 21:58:01.758197 xian_py-0.1.7/xian_py/utils.py
+-rw-r--r--   0        0        0     1906 2024-02-21 22:59:58.767011 xian_py-0.1.7/xian_py/wallet.py
+-rw-r--r--   0        0        0     7779 2024-04-26 23:29:03.455598 xian_py-0.1.7/xian_py/xian.py
+-rw-r--r--   0        0        0     7299 2024-02-21 22:59:58.767235 xian_py-0.1.7/xian_py/xian_datetime.py
+-rw-r--r--   0        0        0     4683 2024-02-21 22:59:58.767344 xian_py-0.1.7/xian_py/xian_decimal.py
+-rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 xian_py-0.1.7/PKG-INFO
```

### Comparing `xian_py-0.1.6/README.md` & `xian_py-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `xian_py-0.1.6/xian_py/encoding.py` & `xian_py-0.1.7/xian_py/encoding.py`

 * *Files identical despite different names*

### Comparing `xian_py-0.1.6/xian_py/formating.py` & `xian_py-0.1.7/xian_py/formating.py`

 * *Files identical despite different names*

### Comparing `xian_py-0.1.6/xian_py/transactions.py` & `xian_py-0.1.7/xian_py/transactions.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,14 +55,31 @@
         if data['result']['tx_result']['data'] is not None:
             decoded = decode_str(data['result']['tx_result']['data'])
             data['result']['tx_result']['data'] = json.loads(decoded)
 
     return data
 
 
+def estimate_stamps(node_url: str, tx: Dict[str, Any]) -> int:
+    """ Estimate the amount of stamps a tx will cost """
+    payload = json.dumps(tx).encode().hex()
+
+    try:
+        r = requests.post(f'{node_url}/abci_query?path="/estimate_stamps/{payload}"')
+        r.raise_for_status()
+    except Exception as e:
+        raise XianException(e)
+
+    data = r.json()['result']['response']['value']
+    decoded_json = json.loads(decode_str(data))
+    stamps = decoded_json['stamps_used']
+
+    return int(stamps)
+
+
 def create_tx(
         contract: str,
         function: str,
         kwargs: Dict[str, Any],
         stamps: int,
         chain_id: str,
         private_key: str,
@@ -100,59 +117,59 @@
         }
     }
 
     tx = encode(format_dictionary(tx))
     return json.loads(tx)
 
 
-def broadcast_tx_sync(node_url: str, tx: Dict[str, Any]) -> Dict[str, Any]:
+def broadcast_tx_commit(node_url: str, tx: Dict[str, Any]) -> Dict[str, Any]:
     """
-    Submits a transaction to be included in the blockchain and returns
-    the response from CheckTx. Does not wait for DeliverTx result.
+    DO NOT USE IN PRODUCTION - ONLY FOR TESTS IN DEVELOPMENT!
+    Submits a transaction to be included in the blockchain and
+    returns the response from CheckTx and DeliverTx.
     :param node_url: Node URL in format 'http://<IP>:<Port>'
     :param tx: Transaction data in JSON format (dict)
-    :return: JSON data with tx hash and CheckTx result
+    :return: JSON data with tx hash, CheckTx and DeliverTx results
     """
     payload = json.dumps(tx).encode().hex()
 
     try:
-        r = requests.post(f'{node_url}/broadcast_tx_sync?tx="{payload}"')
+        r = requests.post(f'{node_url}/broadcast_tx_commit?tx="{payload}"')
     except Exception as e:
         raise XianException(e)
 
     data = r.json()
     return data
 
 
-def broadcast_tx_async(node_url: str, tx: Dict[str, Any]):
+def broadcast_tx_sync(node_url: str, tx: Dict[str, Any]) -> Dict[str, Any]:
     """
     Submits a transaction to be included in the blockchain and returns
-    immediately. Does not wait for CheckTx or DeliverTx results.
+    the response from CheckTx. Does not wait for DeliverTx result.
     :param node_url: Node URL in format 'http://<IP>:<Port>'
     :param tx: Transaction data in JSON format (dict)
+    :return: JSON data with tx hash and CheckTx result
     """
     payload = json.dumps(tx).encode().hex()
 
     try:
-        requests.post(f'{node_url}/broadcast_tx_async?tx="{payload}"')
+        r = requests.post(f'{node_url}/broadcast_tx_sync?tx="{payload}"')
     except Exception as e:
         raise XianException(e)
 
+    data = r.json()
+    return data
+
 
-def broadcast_tx_commit(node_url: str, tx: Dict[str, Any]):
+def broadcast_tx_async(node_url: str, tx: Dict[str, Any]):
     """
-    DO NOT USE IN PRODUCTION - ONLY FOR TESTS IN DEVELOPMENT!
-    Submits a transaction to be included in the blockchain and
-    returns the response from CheckTx and DeliverTx.
+    Submits a transaction to be included in the blockchain and returns
+    immediately. Does not wait for CheckTx or DeliverTx results.
     :param node_url: Node URL in format 'http://<IP>:<Port>'
     :param tx: Transaction data in JSON format (dict)
-    :return: JSON data with tx hash, CheckTx and DeliverTx results
     """
     payload = json.dumps(tx).encode().hex()
 
     try:
-        r = requests.post(f'{node_url}/broadcast_tx_commit?tx="{payload}"')
+        requests.post(f'{node_url}/broadcast_tx_async?tx="{payload}"')
     except Exception as e:
         raise XianException(e)
-
-    data = r.json()
-    return data
```

### Comparing `xian_py-0.1.6/xian_py/wallet.py` & `xian_py-0.1.7/xian_py/wallet.py`

 * *Files identical despite different names*

### Comparing `xian_py-0.1.6/xian_py/xian.py` & `xian_py-0.1.7/xian_py/xian.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,23 +64,40 @@
         return balance
 
     def send_tx(
             self,
             contract: str,
             function: str,
             kwargs: dict,
-            stamps: int | str = 500,
+            stamps: str | int = 0,
             chain_id: str = None,
             synchronous: bool = True) -> Optional[Dict[str, Any]]:
         """ Send a transaction to the network """
 
         if chain_id is None:
             if self.chain_id:
                 chain_id = self.chain_id
 
+        if stamps == 0:
+            stamps = tr.estimate_stamps(
+                self.node_url,
+                tr.create_tx(
+                    contract=contract,
+                    function=function,
+                    kwargs=kwargs,
+                    stamps=int(stamps),
+                    chain_id=chain_id,
+                    private_key=self.wallet.private_key,
+                    nonce=tr.get_nonce(
+                        self.node_url,
+                        self.wallet.public_key
+                    )
+                )
+            )
+
         tx = tr.create_tx(
             contract=contract,
             function=function,
             kwargs=kwargs,
             stamps=int(stamps),
             chain_id=chain_id,
             private_key=self.wallet.private_key,
@@ -117,15 +134,15 @@
             tr.broadcast_tx_async(self.node_url, tx)
 
     def send(
             self,
             amount: int | float | str,
             to_address: str,
             token: str = "currency",
-            stamps: int | str = 100,
+            stamps: int | str = 0,
             chain_id: str = None,
             synchronous: bool = True) -> Optional[Dict[str, Any]]:
         """ Send a token to a given address """
 
         return self.send_tx(
             token,
             "transfer",
@@ -198,24 +215,24 @@
             synchronous: bool = True) -> Optional[Dict[str, Any]]:
         """ Approve smart contract to spend max token amount """
 
         return self.send_tx(
             token,
             "approve",
             {"amount": float(amount), "to": contract},
-            50,
+            0,
             chain_id,
             synchronous
         )
 
     def submit_contract(
             self,
             name: str,
             code: str,
-            stamps: int | str = 1000,
+            stamps: str | int = 0,
             chain_id: str = None,
             synchronous: bool = True) -> Optional[Dict[str, Any]]:
         """ Deploy a contract to the network """
 
         return self.send_tx(
             'submission',
             'submit_contract',
```

### Comparing `xian_py-0.1.6/xian_py/xian_datetime.py` & `xian_py-0.1.7/xian_py/xian_datetime.py`

 * *Files identical despite different names*

### Comparing `xian_py-0.1.6/xian_py/xian_decimal.py` & `xian_py-0.1.7/xian_py/xian_decimal.py`

 * *Files identical despite different names*

### Comparing `xian_py-0.1.6/PKG-INFO` & `xian_py-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xian-py
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python tools to interact with the Xian blockchain
 License: MIT
 Author: endogen
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

