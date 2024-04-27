# Comparing `tmp/python_trading212-0.2.0.tar.gz` & `tmp/python_trading212-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_trading212-0.2.0.tar", max compression
+gzip compressed data, was "python_trading212-1.0.0.tar", max compression
```

## Comparing `python_trading212-0.2.0.tar` & `python_trading212-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1015 2024-04-26 09:57:15.316482 python_trading212-0.2.0/README.md
--rw-r--r--   0        0        0      449 2024-04-26 09:57:15.316482 python_trading212-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       98 2024-04-26 09:57:15.316482 python_trading212-0.2.0/python_trading212/__init__.py
--rw-r--r--   0        0        0     3836 2024-04-26 09:57:15.316482 python_trading212-0.2.0/python_trading212/models.py
--rw-r--r--   0        0        0     8054 2024-04-26 09:57:15.316482 python_trading212-0.2.0/python_trading212/trading212.py
--rw-r--r--   0        0        0     1470 1970-01-01 00:00:00.000000 python_trading212-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-27 13:55:45.063219 python_trading212-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0     2090 2024-04-27 13:55:45.063219 python_trading212-1.0.0/README.md
+-rw-r--r--   0        0        0      449 2024-04-27 13:55:45.063219 python_trading212-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      324 2024-04-27 13:55:45.063219 python_trading212-1.0.0/python_trading212/__init__.py
+-rw-r--r--   0        0        0     5287 2024-04-27 13:55:45.063219 python_trading212-1.0.0/python_trading212/models.py
+-rw-r--r--   0        0        0    12528 2024-04-27 13:55:45.063219 python_trading212-1.0.0/python_trading212/trading212.py
+-rw-r--r--   0        0        0     2545 1970-01-01 00:00:00.000000 python_trading212-1.0.0/PKG-INFO
```

### Comparing `python_trading212-0.2.0/python_trading212/models.py` & `python_trading212-1.0.0/python_trading212/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -98,24 +98,35 @@
     investedValue: float
     result: float
     resultCoef: float
     value: float
 
 
 class Pie(BaseModel):
-    cash: float
-    dividendDetails: DividendDetails
-    id: int
-    progress: float
-    result: Result
-    status: str
+    # Pie Out
+    cash: Optional[float] = None
+    dividendDetails: Optional[DividendDetails] = None
+    id: Optional[int] = None
+    progress: Optional[float] = None
+    result: Optional[Result] = None
+    status: Optional[str] = None
+    # New Pie Input
+    name: Optional[str] = None
+    dividendCashAction: Optional[str] = None
+    endDate: Optional[datetime] = None
+    goal: Optional[float] = None
+    icon: Optional[Icon] = None
+    instrumentShares: Optional[Dict[str, float]] = None
+    # New Pie Output
+    instruments: Optional[List[Instrument]] = None
+    settings: Optional[Settings] = None
 
 
 class Order(BaseModel):
-    creationTime: str
+    creationTime: datetime
     filledQuantity: float
     filledValue: float
     id: int
     limitPrice: float
     quantity: float
     status: str
     stopPrice: float
@@ -136,23 +147,14 @@
 
 
 class AccountMetadata(BaseModel):
     currencyCode: str
     id: int
 
 
-class NewPieIn(BaseModel):
-    name: str
-    dividendCashAction: str
-    endDate: datetime
-    goal: float
-    icon: Optional[Icon]
-    instrumentShares: Dict[str, float]
-
-
 class Issue(BaseModel):
     name: str
     severity: str
 
 
 class Settings(BaseModel):
     creationDate: str
@@ -163,19 +165,14 @@
     id: int
     initialInvestment: int
     instrumentShares: Dict[str, float]
     name: str
     pubicUrl: str
 
 
-class NewPieOut(BaseModel):
-    instruments: List[Instrument]
-    settings: Settings
-
-
 class Tax(BaseModel):
     fillId: str
     name: str
     quantity: float
     timeCharged: datetime
 
 
@@ -203,7 +200,82 @@
     timeValidity: str
     type: str
 
 
 class HistoricalOrderData(BaseModel):
     items: List[HistoryItem]
     nextPagePath: str
+
+
+class LimitOrder(BaseModel):
+    limitPrice: float
+    quantity: float
+    ticker: str
+    timeValidity: str
+
+
+class MarketOrder(BaseModel):
+    quantity: float
+    ticker: str
+
+
+class StopOrder(BaseModel):
+    ticker: str
+    quantity: float
+    stopPrice: float
+    timeValidity: str
+
+
+class StopLimitOrder(BaseModel):
+    ticker: str
+    quantity: float
+    stopPrice: float
+    limitPrice: float
+    timeValidity: str
+
+
+class Dividend(BaseModel):
+    amount: int
+    amountInEuro: int
+    grossAmountPerShare: int
+    paidOn: str
+    quantity: int
+    reference: str
+    ticker: str
+    type: str
+
+
+class PaidOutDividends(BaseModel):
+    items: List[Dividend]
+    nextPagePath: str
+
+
+class DataIncluded(BaseModel):
+    includeDividends: bool
+    includeInterest: bool
+    includeOrders: bool
+    includeTransactions: bool
+
+
+class Export(BaseModel):
+    dataIncluded: DataIncluded
+    downloadLink: str
+    reportId: int
+    status: str
+    timeFrom: datetime
+    timeTo: datetime
+
+
+class Report(BaseModel):
+    reportId: int
+
+
+class Transaction(BaseModel):
+    amount: int
+    dateTime: datetime
+    reference: str
+    type: str
+
+
+class TransactionList(BaseModel):
+    items: List[Transaction]
+    nextPagePath: str
```

