# Comparing `tmp/monarchmoney-0.1.8.tar.gz` & `tmp/monarchmoney-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monarchmoney-0.1.8.tar", last modified: Tue Jan  9 00:53:28 2024, max compression
+gzip compressed data, was "monarchmoney-0.1.9.tar", last modified: Sat Jan 20 18:53:38 2024, max compression
```

## Comparing `monarchmoney-0.1.8.tar` & `monarchmoney-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 00:53:28.581858 monarchmoney-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-09 00:53:25.000000 monarchmoney-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-01-09 00:53:28.581858 monarchmoney-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-01-09 00:53:25.000000 monarchmoney-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 00:53:28.581858 monarchmoney-0.1.8/monarchmoney/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-09 00:53:25.000000 monarchmoney-0.1.8/monarchmoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61080 2024-01-09 00:53:25.000000 monarchmoney-0.1.8/monarchmoney/monarchmoney.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 00:53:28.581858 monarchmoney-0.1.8/monarchmoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-01-09 00:53:28.000000 monarchmoney-0.1.8/monarchmoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-01-09 00:53:28.000000 monarchmoney-0.1.8/monarchmoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 00:53:28.000000 monarchmoney-0.1.8/monarchmoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 00:53:28.000000 monarchmoney-0.1.8/monarchmoney.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-09 00:53:28.000000 monarchmoney-0.1.8/monarchmoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-09 00:53:28.000000 monarchmoney-0.1.8/monarchmoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-09 00:53:28.581858 monarchmoney-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-01-09 00:53:25.000000 monarchmoney-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 18:53:38.689271 monarchmoney-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-20 18:53:32.000000 monarchmoney-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-01-20 18:53:38.689271 monarchmoney-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-01-20 18:53:32.000000 monarchmoney-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 18:53:38.689271 monarchmoney-0.1.9/monarchmoney/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-01-20 18:53:32.000000 monarchmoney-0.1.9/monarchmoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70934 2024-01-20 18:53:32.000000 monarchmoney-0.1.9/monarchmoney/monarchmoney.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 18:53:38.689271 monarchmoney-0.1.9/monarchmoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-01-20 18:53:38.000000 monarchmoney-0.1.9/monarchmoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-01-20 18:53:38.000000 monarchmoney-0.1.9/monarchmoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-20 18:53:38.000000 monarchmoney-0.1.9/monarchmoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-20 18:53:38.000000 monarchmoney-0.1.9/monarchmoney.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-20 18:53:38.000000 monarchmoney-0.1.9/monarchmoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-20 18:53:38.000000 monarchmoney-0.1.9/monarchmoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-20 18:53:38.689271 monarchmoney-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-01-20 18:53:32.000000 monarchmoney-0.1.9/setup.py
```

### Comparing `monarchmoney-0.1.8/LICENSE` & `monarchmoney-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `monarchmoney-0.1.8/PKG-INFO` & `monarchmoney-0.1.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: monarchmoney
-Version: 0.1.8
-Summary: Monarch Money API for Python
-Home-page: https://github.com/hammem/monarchmoney
-Author: hammem
-Author-email: hammem@users.noreply.github.com
-License: MIT
-Keywords: monarch money,financial,money,personal finance
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Office/Business :: Financial
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp>=3.8.4
-Requires-Dist: gql>=3.4
-Requires-Dist: oathtool>=2.3.1
-
 # Monarch Money
 
 Python library for accessing [Monarch Money](https://www.monarchmoney.com/referral/ngam2i643l) data.
 
 # Installation
 
 ## From Source Code
@@ -39,36 +18,49 @@
 There are two ways to use this library: interactive and non-interactive.
 
 ## Interactive
 
 If you're using this library in something like iPython or Jupyter, you can run an interactive-login which supports multi-factor authentication:
 
 ```python
+from monarchmoney import MonarchMoney
+
 mm = MonarchMoney()
 await mm.interactive_login()
 ```
 This will prompt you for the email, password and, if needed, the multi-factor token.
 
 ## Non-interactive
 
 For a non-interactive session, you'll need to create an instance and login:
 
 ```python
+from monarchmoney import MonarchMoney
+
 mm = MonarchMoney()
-mm.login(email, password)
+await mm.login(email, password)
 ```
 
 This may throw a `RequireMFAException`.  If it does, you'll need to get a multi-factor token and call the following method:
 
 ```python
-mm.multi_factor_authenticate(email, password, multi_factor_code)
+from monarchmoney import MonarchMoney, RequireMFAException
+
+mm = MonarchMoney()
+try:
+        await mm.login(email, password)
+except RequireMFAException:
+        await mm.multi_factor_authenticate(email, password, multi_factor_code)
 ```
 
 Alternatively, you can provide the MFA Secret Key. The MFA Secret Key is found when setting up the MFA in Monarch Money by going to Settings -> Security -> Enable MFA -> and copy the "Two-factor text code". Then provide it in the login() method:
 ```python
+from monarchmoney import MonarchMoney, RequireMFAException
+
+mm = MonarchMoney()
 await mm.login(
         email=email,
         password=password,
         save_session=False,
         use_saved_session=False,
         mfa_secret_key=mfa_secret_key,
     )
@@ -80,14 +72,16 @@
 As of writing this README, the following methods are supported:
 
 ## Non-Mutating Methods
 
 - `get_accounts` - gets all the accounts linked to Monarch Money
 - `get_account_holdings` - gets all of the securities in a brokerage or similar type of account
 - `get_account_type_options` - all account types and their subtypes available in Monarch Money- 
+- `get_account_history` - gets all daily account history for the specified account
+- `get_institutions` -- gets institutions linked to Monarch Money
 - `get_budgets` — all the budgets and the corresponding actual amounts
 - `get_subscription_details` - gets the Monarch Money account's status (e.g. paid or trial)
 - `get_transactions_summary` - gets the transaction summary data from the transactions page
 - `get_transactions` - gets transaction data, defaults to returning the last 100 transactions; can also be searched by date range
 - `get_transaction_categories` - gets all of the categories configured in the account
 - `get_transaction_category_groups` all category groups configured in the account- 
 - `get_transaction_details` - gets detailed transaction data for a single transaction
@@ -105,14 +99,15 @@
 - `request_accounts_refresh_and_wait` - requests a synchronization / refresh of all accounts linked to Monarch Money. This is a **blocking call** and will not return until the refresh is complete or no longer running.
 - `create_transaction` - creates a transaction with the given attributes
 - `update_transaction` - modifies one or more attributes for an existing transaction
 - `delete_transaction` - deletes a given transaction by the provided transaction id
 - `update_transaction_splits` - modifies how a transaction is split (or not)
 - `set_budget_amount` - sets a budget's value to the given amount (date allowed, will only apply to month specified by default). A zero amount value will "unset" or "clear" the budget for the given category.
 - `create_manual_account` - creates a new manual account
+- `upload_account_balance_history` - uploads account history csv file for a given account
 
 # Contributing
 
 Any and all contributions -- code, documentation, feature requests, feedback -- are welcome!
 
 If you plan to submit up a pull request, you can expect a timely review.  There aren't any strict requirements around the environment you need to configure aside from using [Black](https://github.com/psf/black) to auto-format the code.  An action is configured in this repo to run against all PRs and merges and will block them from being committed.
```

### Comparing `monarchmoney-0.1.8/README.md` & `monarchmoney-0.1.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: monarchmoney
+Version: 0.1.9
+Summary: Monarch Money API for Python
+Home-page: https://github.com/hammem/monarchmoney
+Author: hammem
+Author-email: hammem@users.noreply.github.com
+License: MIT
+Keywords: monarch money,financial,money,personal finance
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Office/Business :: Financial
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp>=3.8.4
+Requires-Dist: gql>=3.4
+Requires-Dist: oathtool>=2.3.1
+
 # Monarch Money
 
 Python library for accessing [Monarch Money](https://www.monarchmoney.com/referral/ngam2i643l) data.
 
 # Installation
 
 ## From Source Code
@@ -18,36 +39,49 @@
 There are two ways to use this library: interactive and non-interactive.
 
 ## Interactive
 
 If you're using this library in something like iPython or Jupyter, you can run an interactive-login which supports multi-factor authentication:
 
 ```python
+from monarchmoney import MonarchMoney
+
 mm = MonarchMoney()
 await mm.interactive_login()
 ```
 This will prompt you for the email, password and, if needed, the multi-factor token.
 
 ## Non-interactive
 
 For a non-interactive session, you'll need to create an instance and login:
 
 ```python
+from monarchmoney import MonarchMoney
+
 mm = MonarchMoney()
-mm.login(email, password)
+await mm.login(email, password)
 ```
 
 This may throw a `RequireMFAException`.  If it does, you'll need to get a multi-factor token and call the following method:
 
 ```python
-mm.multi_factor_authenticate(email, password, multi_factor_code)
+from monarchmoney import MonarchMoney, RequireMFAException
+
+mm = MonarchMoney()
+try:
+        await mm.login(email, password)
+except RequireMFAException:
+        await mm.multi_factor_authenticate(email, password, multi_factor_code)
 ```
 
 Alternatively, you can provide the MFA Secret Key. The MFA Secret Key is found when setting up the MFA in Monarch Money by going to Settings -> Security -> Enable MFA -> and copy the "Two-factor text code". Then provide it in the login() method:
 ```python
+from monarchmoney import MonarchMoney, RequireMFAException
+
+mm = MonarchMoney()
 await mm.login(
         email=email,
         password=password,
         save_session=False,
         use_saved_session=False,
         mfa_secret_key=mfa_secret_key,
     )
@@ -59,14 +93,16 @@
 As of writing this README, the following methods are supported:
 
 ## Non-Mutating Methods
 
 - `get_accounts` - gets all the accounts linked to Monarch Money
 - `get_account_holdings` - gets all of the securities in a brokerage or similar type of account
 - `get_account_type_options` - all account types and their subtypes available in Monarch Money- 
+- `get_account_history` - gets all daily account history for the specified account
+- `get_institutions` -- gets institutions linked to Monarch Money
 - `get_budgets` — all the budgets and the corresponding actual amounts
 - `get_subscription_details` - gets the Monarch Money account's status (e.g. paid or trial)
 - `get_transactions_summary` - gets the transaction summary data from the transactions page
 - `get_transactions` - gets transaction data, defaults to returning the last 100 transactions; can also be searched by date range
 - `get_transaction_categories` - gets all of the categories configured in the account
 - `get_transaction_category_groups` all category groups configured in the account- 
 - `get_transaction_details` - gets detailed transaction data for a single transaction
@@ -84,14 +120,15 @@
 - `request_accounts_refresh_and_wait` - requests a synchronization / refresh of all accounts linked to Monarch Money. This is a **blocking call** and will not return until the refresh is complete or no longer running.
 - `create_transaction` - creates a transaction with the given attributes
 - `update_transaction` - modifies one or more attributes for an existing transaction
 - `delete_transaction` - deletes a given transaction by the provided transaction id
 - `update_transaction_splits` - modifies how a transaction is split (or not)
 - `set_budget_amount` - sets a budget's value to the given amount (date allowed, will only apply to month specified by default). A zero amount value will "unset" or "clear" the budget for the given category.
 - `create_manual_account` - creates a new manual account
+- `upload_account_balance_history` - uploads account history csv file for a given account
 
 # Contributing
 
 Any and all contributions -- code, documentation, feature requests, feedback -- are welcome!
 
 If you plan to submit up a pull request, you can expect a timely review.  There aren't any strict requirements around the environment you need to configure aside from using [Black](https://github.com/psf/black) to auto-format the code.  An action is configured in this repo to run against all PRs and merges and will block them from being committed.
```

### Comparing `monarchmoney-0.1.8/monarchmoney/monarchmoney.py` & `monarchmoney-0.1.9/monarchmoney/monarchmoney.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import calendar
 from datetime import datetime
+import json
 import os
 import pickle
 import oathtool
 import time
 from typing import Any, Dict, Optional, List
 
-from aiohttp import ClientSession
+from aiohttp import ClientSession, FormData
 from aiohttp.client import DEFAULT_TIMEOUT
 import asyncio
 from gql import gql, Client
 from gql.transport.aiohttp import AIOHTTPTransport
 from graphql import DocumentNode
 
 
@@ -29,14 +30,18 @@
     def getLoginEndpoint(cls) -> str:
         return cls.BASE_URL + "/auth/login/"
 
     @classmethod
     def getGraphQL(cls) -> str:
         return cls.BASE_URL + "/graphql"
 
+    @classmethod
+    def getAccountBalanceHistoryUploadEndpoint(cls) -> str:
+        return cls.BASE_URL + "/account-balance-history/upload/"
+
 
 class RequireMFAException(Exception):
     pass
 
 
 class LoginFailedException(Exception):
     pass
@@ -480,14 +485,334 @@
 
         return await self.gql_call(
             operation="Web_GetHoldings",
             graphql_query=query,
             variables=variables,
         )
 
+    async def get_account_history(self, account_id: int) -> Dict[str, Any]:
+        """
+        Gets historical account snapshot data for the requested account
+
+        Args:
+          account_id: Monarch account ID as an integer
+
+        Returns:
+          json object with all historical snapshots of requested account's balances
+        """
+
+        query = gql(
+            """
+            query AccountDetails_getAccount($id: UUID!, $filters: TransactionFilterInput) {
+              account(id: $id) {
+                id
+                ...AccountFields
+                ...EditAccountFormFields
+                isLiability
+                credential {
+                  id
+                  hasSyncInProgress
+                  canBeForceRefreshed
+                  disconnectedFromDataProviderAt
+                  dataProvider
+                  institution {
+                    id
+                    plaidInstitutionId
+                    url
+                    ...InstitutionStatusFields
+                    __typename
+                  }
+                  __typename
+                }
+                institution {
+                  id
+                  plaidInstitutionId
+                  url
+                  ...InstitutionStatusFields
+                  __typename
+                }
+                __typename
+              }
+              transactions: allTransactions(filters: $filters) {
+                totalCount
+                results(limit: 20) {
+                  id
+                  ...TransactionsListFields
+                  __typename
+                }
+                __typename
+              }
+              snapshots: snapshotsForAccount(accountId: $id) {
+                date
+                signedBalance
+                __typename
+              }
+            }
+
+            fragment AccountFields on Account {
+              id
+              displayName
+              syncDisabled
+              deactivatedAt
+              isHidden
+              isAsset
+              mask
+              createdAt
+              updatedAt
+              displayLastUpdatedAt
+              currentBalance
+              displayBalance
+              includeInNetWorth
+              hideFromList
+              hideTransactionsFromReports
+              includeBalanceInNetWorth
+              includeInGoalBalance
+              dataProvider
+              dataProviderAccountId
+              isManual
+              transactionsCount
+              holdingsCount
+              manualInvestmentsTrackingMethod
+              order
+              icon
+              logoUrl
+              type {
+                name
+                display
+                group
+                __typename
+              }
+              subtype {
+                name
+                display
+                __typename
+              }
+              credential {
+                id
+                updateRequired
+                disconnectedFromDataProviderAt
+                dataProvider
+                institution {
+                  id
+                  plaidInstitutionId
+                  name
+                  status
+                  logo
+                  __typename
+                }
+                __typename
+              }
+              institution {
+                id
+                name
+                logo
+                primaryColor
+                url
+                __typename
+              }
+              __typename
+            }
+
+            fragment EditAccountFormFields on Account {
+              id
+              displayName
+              deactivatedAt
+              displayBalance
+              includeInNetWorth
+              hideFromList
+              hideTransactionsFromReports
+              dataProvider
+              dataProviderAccountId
+              isManual
+              manualInvestmentsTrackingMethod
+              isAsset
+              invertSyncedBalance
+              canInvertBalance
+              type {
+                name
+                display
+                __typename
+              }
+              subtype {
+                name
+                display
+                __typename
+              }
+              __typename
+            }
+
+            fragment InstitutionStatusFields on Institution {
+              id
+              hasIssuesReported
+              hasIssuesReportedMessage
+              plaidStatus
+              status
+              balanceStatus
+              transactionsStatus
+              __typename
+            }
+
+            fragment TransactionsListFields on Transaction {
+              id
+              ...TransactionOverviewFields
+              __typename
+            }
+
+            fragment TransactionOverviewFields on Transaction {
+              id
+              amount
+              pending
+              date
+              hideFromReports
+              plaidName
+              notes
+              isRecurring
+              reviewStatus
+              needsReview
+              dataProviderDescription
+              attachments {
+                id
+                __typename
+              }
+              isSplitTransaction
+              category {
+                id
+                name
+                icon
+                group {
+                  id
+                  type
+                  __typename
+                }
+                __typename
+              }
+              merchant {
+                name
+                id
+                transactionsCount
+                __typename
+              }
+              tags {
+                id
+                name
+                color
+                order
+                __typename
+              }
+              __typename
+            }
+            """
+        )
+
+        variables = {"id": str(account_id)}
+
+        account_details = await self.gql_call(
+            operation="AccountDetails_getAccount",
+            graphql_query=query,
+            variables=variables,
+        )
+
+        # Parse JSON
+        account_name = account_details["account"]["displayName"]
+        account_balance_history = account_details["snapshots"]
+
+        # Append account identification data to account balance history
+        for i in account_balance_history:
+            i.update(dict(accountId=str(account_id)))
+            i.update(dict(accountName=account_name))
+
+        return account_balance_history
+
+    async def get_institutions(self) -> Dict[str, Any]:
+        """
+        Gets institution data from the account.
+        """
+
+        query = gql(
+            """
+            query Web_GetInstitutionSettings {
+              credentials {
+                id
+                ...CredentialSettingsCardFields
+                __typename
+              }
+              accounts(filters: {includeDeleted: true}) {
+                id
+                displayName
+                subtype {
+                  display
+                  __typename
+                }
+                mask
+                credential {
+                  id
+                  __typename
+                }
+                deletedAt
+                __typename
+              }
+              subscription {
+                isOnFreeTrial
+                hasPremiumEntitlement
+                __typename
+              }
+            }
+
+            fragment CredentialSettingsCardFields on Credential {
+              id
+              updateRequired
+              disconnectedFromDataProviderAt
+              ...InstitutionInfoFields
+              institution {
+                id
+                name
+                logo
+                url
+                __typename
+              }
+              __typename
+            }
+
+            fragment InstitutionInfoFields on Credential {
+              id
+              displayLastUpdatedAt
+              dataProvider
+              updateRequired
+              disconnectedFromDataProviderAt
+              ...InstitutionLogoWithStatusFields
+              institution {
+                id
+                name
+                hasIssuesReported
+                hasIssuesReportedMessage
+                __typename
+              }
+              __typename
+            }
+
+            fragment InstitutionLogoWithStatusFields on Credential {
+              dataProvider
+              updateRequired
+              institution {
+                hasIssuesReported
+                logo
+                status
+                balanceStatus
+                transactionsStatus
+                __typename
+              }
+              __typename
+            }
+        """
+        )
+        return await self.gql_call(
+            operation="Web_GetInstitutionSettings",
+            graphql_query=query,
+        )
+
     async def get_budgets(
         self,
         start_date: Optional[str] = None,
         end_date: Optional[str] = None,
         use_legacy_goals: Optional[bool] = False,
         use_v2_goals: Optional[bool] = True,
     ) -> Dict[str, Any]:
@@ -1860,14 +2185,39 @@
 
         return await self.gql_call(
             operation="Common_UpdateBudgetItem",
             variables=variables,
             graphql_query=query,
         )
 
+    async def upload_account_balance_history(
+        self, account_id: str, csv_content: str
+    ) -> None:
+        """
+        Uploads the account balance history csv for a given account.
+
+        :param account_id: The account ID to apply the history to.
+        :param csv_content: CSV representation of the balance history.
+        """
+        if not account_id or not csv_content:
+            raise RequestFailedException("account_id and csv_content cannot be empty")
+
+        filename = "upload.csv"
+        form = FormData()
+        form.add_field("files", csv_content, filename=filename, content_type="text/csv")
+        form.add_field("account_files_mapping", json.dumps({filename: account_id}))
+
+        async with ClientSession(headers=self._headers) as session:
+            resp = await session.post(
+                MonarchMoneyEndpoints.getAccountBalanceHistoryUploadEndpoint(),
+                data=form,
+            )
+            if resp.status != 200:
+                raise RequestFailedException(f"HTTP Code {resp.status}: {resp.reason}")
+
     async def gql_call(
         self,
         operation: str,
         graphql_query: DocumentNode,
         variables: Dict[str, Any] = {},
     ) -> Dict[str, Any]:
         """
```

### Comparing `monarchmoney-0.1.8/monarchmoney.egg-info/PKG-INFO` & `monarchmoney-0.1.9/monarchmoney.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monarchmoney
-Version: 0.1.8
+Version: 0.1.9
 Summary: Monarch Money API for Python
 Home-page: https://github.com/hammem/monarchmoney
 Author: hammem
 Author-email: hammem@users.noreply.github.com
 License: MIT
 Keywords: monarch money,financial,money,personal finance
 Platform: any
@@ -39,36 +39,49 @@
 There are two ways to use this library: interactive and non-interactive.
 
 ## Interactive
 
 If you're using this library in something like iPython or Jupyter, you can run an interactive-login which supports multi-factor authentication:
 
 ```python
+from monarchmoney import MonarchMoney
+
 mm = MonarchMoney()
 await mm.interactive_login()
 ```
 This will prompt you for the email, password and, if needed, the multi-factor token.
 
 ## Non-interactive
 
 For a non-interactive session, you'll need to create an instance and login:
 
 ```python
+from monarchmoney import MonarchMoney
+
 mm = MonarchMoney()
-mm.login(email, password)
+await mm.login(email, password)
 ```
 
 This may throw a `RequireMFAException`.  If it does, you'll need to get a multi-factor token and call the following method:
 
 ```python
-mm.multi_factor_authenticate(email, password, multi_factor_code)
+from monarchmoney import MonarchMoney, RequireMFAException
+
+mm = MonarchMoney()
+try:
+        await mm.login(email, password)
+except RequireMFAException:
+        await mm.multi_factor_authenticate(email, password, multi_factor_code)
 ```
 
 Alternatively, you can provide the MFA Secret Key. The MFA Secret Key is found when setting up the MFA in Monarch Money by going to Settings -> Security -> Enable MFA -> and copy the "Two-factor text code". Then provide it in the login() method:
 ```python
+from monarchmoney import MonarchMoney, RequireMFAException
+
+mm = MonarchMoney()
 await mm.login(
         email=email,
         password=password,
         save_session=False,
         use_saved_session=False,
         mfa_secret_key=mfa_secret_key,
     )
@@ -80,14 +93,16 @@
 As of writing this README, the following methods are supported:
 
 ## Non-Mutating Methods
 
 - `get_accounts` - gets all the accounts linked to Monarch Money
 - `get_account_holdings` - gets all of the securities in a brokerage or similar type of account
 - `get_account_type_options` - all account types and their subtypes available in Monarch Money- 
+- `get_account_history` - gets all daily account history for the specified account
+- `get_institutions` -- gets institutions linked to Monarch Money
 - `get_budgets` — all the budgets and the corresponding actual amounts
 - `get_subscription_details` - gets the Monarch Money account's status (e.g. paid or trial)
 - `get_transactions_summary` - gets the transaction summary data from the transactions page
 - `get_transactions` - gets transaction data, defaults to returning the last 100 transactions; can also be searched by date range
 - `get_transaction_categories` - gets all of the categories configured in the account
 - `get_transaction_category_groups` all category groups configured in the account- 
 - `get_transaction_details` - gets detailed transaction data for a single transaction
@@ -105,14 +120,15 @@
 - `request_accounts_refresh_and_wait` - requests a synchronization / refresh of all accounts linked to Monarch Money. This is a **blocking call** and will not return until the refresh is complete or no longer running.
 - `create_transaction` - creates a transaction with the given attributes
 - `update_transaction` - modifies one or more attributes for an existing transaction
 - `delete_transaction` - deletes a given transaction by the provided transaction id
 - `update_transaction_splits` - modifies how a transaction is split (or not)
 - `set_budget_amount` - sets a budget's value to the given amount (date allowed, will only apply to month specified by default). A zero amount value will "unset" or "clear" the budget for the given category.
 - `create_manual_account` - creates a new manual account
+- `upload_account_balance_history` - uploads account history csv file for a given account
 
 # Contributing
 
 Any and all contributions -- code, documentation, feature requests, feedback -- are welcome!
 
 If you plan to submit up a pull request, you can expect a timely review.  There aren't any strict requirements around the environment you need to configure aside from using [Black](https://github.com/psf/black) to auto-format the code.  An action is configured in this repo to run against all PRs and merges and will block them from being committed.
```

### Comparing `monarchmoney-0.1.8/setup.py` & `monarchmoney-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 install_requires = ["aiohttp>=3.8.4", "gql>=3.4", "oathtool>=2.3.1"]
 
 setup(
     name="monarchmoney",
-    version="0.1.8",
+    version="0.1.9",
     description="Monarch Money API for Python",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/hammem/monarchmoney",
     author="hammem",
     author_email="hammem@users.noreply.github.com",
     license="MIT",
```

