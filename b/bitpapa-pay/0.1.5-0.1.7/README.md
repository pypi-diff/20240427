# Comparing `tmp/bitpapa_pay-0.1.5.tar.gz` & `tmp/bitpapa_pay-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitpapa_pay-0.1.5.tar", max compression
+gzip compressed data, was "bitpapa_pay-0.1.7.tar", max compression
```

## Comparing `bitpapa_pay-0.1.5.tar` & `bitpapa_pay-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0     1155 2024-04-09 10:23:59.770129 bitpapa_pay-0.1.5/README.md
--rw-r--r--   0        0        0       50 2024-04-09 08:50:44.260698 bitpapa_pay-0.1.5/bitpapa_pay/__init__.py
--rw-r--r--   0        0        0     3562 2024-04-09 10:22:00.217588 bitpapa_pay-0.1.5/bitpapa_pay/client.py
--rw-r--r--   0        0        0      473 2024-04-09 09:47:14.505171 bitpapa_pay-0.1.5/bitpapa_pay/methods/base.py
--rw-r--r--   0        0        0      625 2024-04-09 09:55:00.185493 bitpapa_pay-0.1.5/bitpapa_pay/methods/exchange_rates.py
--rw-r--r--   0        0        0     2325 2024-04-09 09:55:17.053511 bitpapa_pay-0.1.5/bitpapa_pay/methods/telegram.py
--rw-r--r--   0        0        0       18 2024-04-09 10:43:21.713081 bitpapa_pay-0.1.5/bitpapa_pay/version.py
--rw-r--r--   0        0        0      353 2024-04-09 10:43:41.709007 bitpapa_pay-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 bitpapa_pay-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1138 2024-04-12 18:48:56.761770 bitpapa_pay-0.1.7/README.md
+-rw-r--r--   0        0        0       42 2024-04-11 08:47:40.794934 bitpapa_pay-0.1.7/bitpapa_pay/__init__.py
+-rw-r--r--   0        0        0     6522 2024-04-24 17:55:52.551475 bitpapa_pay-0.1.7/bitpapa_pay/client.py
+-rw-r--r--   0        0        0     3814 2024-04-24 17:55:43.319650 bitpapa_pay-0.1.7/bitpapa_pay/methods/addresses.py
+-rw-r--r--   0        0        0      608 2024-04-12 20:23:58.411916 bitpapa_pay-0.1.7/bitpapa_pay/methods/base.py
+-rw-r--r--   0        0        0      686 2024-04-12 20:26:00.463851 bitpapa_pay-0.1.7/bitpapa_pay/methods/exchange_rates.py
+-rw-r--r--   0        0        0     2405 2024-04-24 16:33:12.237628 bitpapa_pay-0.1.7/bitpapa_pay/methods/telegram.py
+-rw-r--r--   0        0        0      261 2024-04-12 20:22:45.616006 bitpapa_pay-0.1.7/bitpapa_pay/types/base.py
+-rw-r--r--   0        0        0      124 2024-04-12 20:25:33.931857 bitpapa_pay-0.1.7/bitpapa_pay/types/exchange_rates.py
+-rw-r--r--   0        0        0      816 2024-04-24 16:36:05.257339 bitpapa_pay-0.1.7/bitpapa_pay/types/telegram.py
+-rw-r--r--   0        0        0       18 2024-04-27 17:24:11.552517 bitpapa_pay-0.1.7/bitpapa_pay/version.py
+-rw-r--r--   0        0        0      371 2024-04-27 17:23:58.888122 bitpapa_pay-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1794 1970-01-01 00:00:00.000000 bitpapa_pay-0.1.7/PKG-INFO
```

### Comparing `bitpapa_pay-0.1.5/README.md` & `bitpapa_pay-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 ```
     
 ## Usage/Examples
 
 ```python
 import asyncio
 
-from bitpapa_pay import TelegramBitpapaPay
+from bitpapa_pay import BitpapaPay
 
 
 async def main():
-    bitpapa_pay = TelegramBitpapaPay(api_token="api_token")
-    result = await bitpapa_pay.create_invoice("USDT", -100)
+    bitpapa_pay = BitpapaPay(api_token="api_token")
+    result = await bitpapa_pay.create_invoice("USDT", 100)
     print(result.model_dump())
     print(
         result.invoice.id,
         result.invoice.currency_code,
         result.invoice.amount,
         result.invoice.status,
         result.invoice.created_at,
```

### Comparing `bitpapa_pay-0.1.5/bitpapa_pay/methods/exchange_rates.py` & `bitpapa_pay-0.1.7/bitpapa_pay/methods/exchange_rates.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from typing import Dict, Type
-
-from pydantic import BaseModel
+from typing import Literal, Type
 
 from bitpapa_pay.methods.base import BaseMethod, BaseOutData
-
-
-class GetExchangeRatesOut(BaseModel):
-    rates: Dict[str, float]
+from bitpapa_pay.types.exchange_rates import GetExchangeRatesOut
 
 
 class GetExchangeRates(BaseMethod):
-    def __init__(self) -> None:
-        self.returning_model: Type[GetExchangeRatesOut] = GetExchangeRatesOut
-
     @property
     def endpoint(self) -> str:
         return "/api/v1/exchange_rates/all"
 
+    @property
+    def request_type(self) -> Literal["GET"]:
+        return "GET"
+
+    @property
+    def returning_model(self) -> Type[GetExchangeRatesOut]:
+        return GetExchangeRatesOut
+
     def get_data(self) -> BaseOutData:
         return BaseOutData(
             endpoint=self.endpoint,
-            request_type="GET",
+            request_type=self.request_type,
             returning_model=self.returning_model
         )
```

### Comparing `bitpapa_pay-0.1.5/bitpapa_pay/methods/telegram.py` & `bitpapa_pay-0.1.7/bitpapa_pay/methods/telegram.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,91 +1,76 @@
-from typing import List, Type, Union
-
-from pydantic import BaseModel, computed_field
+from typing import Literal, Type, Union, Optional
 
 from bitpapa_pay.methods.base import BaseMethod, BaseOutData
-
-
-class TelegramInvoice(BaseModel):
-    id: str
-    currency_code: str
-    amount: Union[int, float]
-    status: str
-    created_at: str
-    updated_at: str
-
-    @computed_field
-    def url(self) -> str:
-        return f"https://t.me/bitpapa_bot?start={self.id}"
-
-
-class TelegramInvoices(BaseModel):
-    invoices: List[TelegramInvoice]
-
-
-class TelegramInvoiceIn(BaseModel):
-    currency_code: str
-    amount: Union[int, float]
-
-
-class CreateTelegramInvoiceJD(BaseModel):
-    api_token: str
-    invoice: TelegramInvoiceIn
-
-
-class CreateTelegramInvoiceOut(BaseModel):
-    invoice: TelegramInvoice
-
-
-class GetTelegramInvoicesParams(BaseModel):
-    api_token: str
+from bitpapa_pay.types.telegram import (CreateTelegramInvoiceInputData,
+                                        CreateTelegramInvoiceOutputData,
+                                        GetTelegramInvoicesInputParams,
+                                        TelegramInvoiceInputData,
+                                        TelegramInvoices)
 
 
 class CreateTelegramInvoice(BaseMethod):
     def __init__(
         self,
         api_token: str,
         currency_code: str,
-        amount: Union[int, float]
+        amount: Union[int, float],
+        crypto_address: Optional[str] = None
     ) -> None:
-        self.returning_model: Type[CreateTelegramInvoiceOut] = CreateTelegramInvoiceOut
         self.api_token = api_token
         self.currency_code = currency_code
         self.amount = amount
+        self.crypto_address = crypto_address
 
     @property
     def endpoint(self) -> str:
         return "/api/v1/invoices/public"
 
+    @property
+    def request_type(self) -> Literal["POST"]:
+        return "POST"
+
+    @property
+    def returning_model(self) -> Type[CreateTelegramInvoiceOutputData]:
+        return CreateTelegramInvoiceOutputData
+
     def get_data(self) -> BaseOutData:
         return BaseOutData(
             endpoint=self.endpoint,
-            request_type="POST",
-            json_data=CreateTelegramInvoiceJD(
+            request_type=self.request_type,
+            json_data=CreateTelegramInvoiceInputData(
                 api_token=self.api_token,
-                invoice=TelegramInvoiceIn(
+                invoice=TelegramInvoiceInputData(
                     currency_code=self.currency_code,
-                    amount=self.amount
-                )
+                    amount=self.amount,
+                    crypto_address=self.crypto_address
+                ),
             ).model_dump(),
             returning_model=self.returning_model
         )
 
 
 class GetTelegramInvoices(BaseMethod):
     def __init__(self, api_token: str) -> None:
-        self.returning_model: Type[TelegramInvoices] = TelegramInvoices
         self.api_token = api_token
 
     @property
     def endpoint(self) -> str:
         return "/api/v1/invoices/public"
 
+    @property
+    def request_type(self) -> Literal["GET"]:
+        return "GET"
+
+    @property
+    def returning_model(self) -> Type[TelegramInvoices]:
+        return TelegramInvoices
+
     def get_data(self) -> BaseOutData:
         return BaseOutData(
             endpoint=self.endpoint,
-            request_type="GET",
-            params=GetTelegramInvoicesParams(
+            request_type=self.request_type,
+            params=GetTelegramInvoicesInputParams(
                 api_token=self.api_token
             ).model_dump(),
             returning_model=self.returning_model
         )
```

### Comparing `bitpapa_pay-0.1.5/PKG-INFO` & `bitpapa_pay-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: bitpapa-pay
-Version: 0.1.5
+Version: 0.1.7
 Summary: Bitpapa Pay async python wrapper
 Author: VasilevAlexandr97
 Author-email: vasilev.alex.work@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.8.6,<4.0.0)
+Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: pydantic (>=2.4.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 
 # Bitpapa Pay asynchronous api wrapper
 
 **Docs**: https://apidocs.bitpapa.com/docs/apidocs/wvea40l9be95f-integracziya-bitpapa-pay
@@ -31,20 +32,20 @@
 ```
     
 ## Usage/Examples
 
 ```python
 import asyncio
 
-from bitpapa_pay import TelegramBitpapaPay
+from bitpapa_pay import BitpapaPay
 
 
 async def main():
-    bitpapa_pay = TelegramBitpapaPay(api_token="api_token")
-    result = await bitpapa_pay.create_invoice("USDT", -100)
+    bitpapa_pay = BitpapaPay(api_token="api_token")
+    result = await bitpapa_pay.create_invoice("USDT", 100)
     print(result.model_dump())
     print(
         result.invoice.id,
         result.invoice.currency_code,
         result.invoice.amount,
         result.invoice.status,
         result.invoice.created_at,
```

