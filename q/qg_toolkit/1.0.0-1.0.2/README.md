# Comparing `tmp/qg_toolkit-1.0.0.tar.gz` & `tmp/qg_toolkit-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qg_toolkit-1.0.0.tar", max compression
+gzip compressed data, was "qg_toolkit-1.0.2.tar", max compression
```

## Comparing `qg_toolkit-1.0.0.tar` & `qg_toolkit-1.0.2.tar`

### file list

```diff
@@ -1,47 +1,53 @@
--rw-r--r--   0        0        0      602 2024-04-24 18:35:01.907492 qg_toolkit-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4852 2024-04-20 19:48:15.063903 qg_toolkit-1.0.0/qtweepy/examples/account_checker.py
--rw-r--r--   0        0        0     2210 2024-04-20 19:48:15.064902 qg_toolkit-1.0.0/qtweepy/examples/follow_each_other.py
--rw-r--r--   0        0        0        0 2024-04-20 20:13:46.959521 qg_toolkit-1.0.0/qtweepy/examples/input-output/PROXIES.txt
--rw-r--r--   0        0        0        0 2024-04-20 20:13:46.959521 qg_toolkit-1.0.0/qtweepy/examples/input-output/UNKNOWN.txt
--rw-r--r--   0        0        0     3581 2024-04-20 19:48:15.065903 qg_toolkit-1.0.0/qtweepy/examples/mavia.py
--rw-r--r--   0        0        0     2332 2024-04-20 19:48:15.066903 qg_toolkit-1.0.0/qtweepy/examples/set_2fa.py
--rw-r--r--   0        0        0     3040 2024-04-20 19:48:15.066903 qg_toolkit-1.0.0/qtweepy/examples/set_avatars_and_banners.py
--rw-r--r--   0        0        0      686 2024-04-20 19:48:15.066903 qg_toolkit-1.0.0/qtweepy/examples/uploading_images.py
--rw-r--r--   0        0        0     2212 2024-04-20 19:48:15.067902 qg_toolkit-1.0.0/qtweepy/examples/voter.py
--rw-r--r--   0        0        0     3079 2024-04-20 19:48:15.067902 qg_toolkit-1.0.0/qtweepy/examples/xai.py
--rw-r--r--   0        0        0      687 2024-04-20 19:57:03.446998 qg_toolkit-1.0.0/qtweepy/pyproject.toml
--rw-r--r--   0        0        0     8720 2024-04-20 19:48:15.063903 qg_toolkit-1.0.0/qtweepy/README.md
--rw-r--r--   0        0        0      132 2024-04-24 18:22:26.184000 qg_toolkit-1.0.0/qtweepy/tea.yaml
--rw-r--r--   0        0        0      732 2024-04-20 19:48:15.068902 qg_toolkit-1.0.0/qtweepy/twitter/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.0/qtweepy/twitter/_capsolver/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.0/qtweepy/twitter/_capsolver/core/__init__.py
--rw-r--r--   0        0        0     8883 2024-04-20 19:48:15.070903 qg_toolkit-1.0.0/qtweepy/twitter/_capsolver/core/base.py
--rw-r--r--   0        0        0     1054 2024-04-20 19:48:15.070903 qg_toolkit-1.0.0/qtweepy/twitter/_capsolver/core/config.py
--rw-r--r--   0        0        0     1741 2024-04-20 19:48:15.071903 qg_toolkit-1.0.0/qtweepy/twitter/_capsolver/core/enum.py
--rw-r--r--   0        0        0     2602 2024-04-20 19:48:15.071903 qg_toolkit-1.0.0/qtweepy/twitter/_capsolver/core/serializer.py
--rw-r--r--   0        0        0    10974 2024-04-20 19:48:15.072903 qg_toolkit-1.0.0/qtweepy/twitter/_capsolver/fun_captcha.py
--rw-r--r--   0        0        0     3248 2024-04-20 19:48:15.072903 qg_toolkit-1.0.0/qtweepy/twitter/account.py
--rw-r--r--   0        0        0      141 2024-04-20 19:48:15.072903 qg_toolkit-1.0.0/qtweepy/twitter/base/__init__.py
--rw-r--r--   0        0        0      500 2024-04-20 19:48:15.074292 qg_toolkit-1.0.0/qtweepy/twitter/base/client.py
--rw-r--r--   0        0        0     2164 2024-04-20 19:48:15.074413 qg_toolkit-1.0.0/qtweepy/twitter/base/session.py
--rw-r--r--   0        0        0    70738 2024-04-20 19:48:15.075686 qg_toolkit-1.0.0/qtweepy/twitter/client.py
--rw-r--r--   0        0        0      267 2024-04-20 19:48:15.076283 qg_toolkit-1.0.0/qtweepy/twitter/enums.py
--rw-r--r--   0        0        0     5322 2024-04-20 19:48:15.076811 qg_toolkit-1.0.0/qtweepy/twitter/errors.py
--rw-r--r--   0        0        0     4695 2024-04-20 19:48:15.076811 qg_toolkit-1.0.0/qtweepy/twitter/models.py
--rw-r--r--   0        0        0      665 2024-04-20 19:48:15.077920 qg_toolkit-1.0.0/qtweepy/twitter/utils/__init__.py
--rw-r--r--   0        0        0     1152 2024-04-20 19:48:15.077920 qg_toolkit-1.0.0/qtweepy/twitter/utils/file.py
--rw-r--r--   0        0        0     2140 2024-04-20 19:48:15.078463 qg_toolkit-1.0.0/qtweepy/twitter/utils/html.py
--rw-r--r--   0        0        0     1061 2024-04-20 19:48:15.078992 qg_toolkit-1.0.0/qtweepy/twitter/utils/other.py
--rw-r--r--   0        0        0       38 2024-04-20 19:50:56.436133 qg_toolkit-1.0.0/README.md
--rw-r--r--   0        0        0      132 2024-04-24 18:33:41.150515 qg_toolkit-1.0.0/tea.yaml
--rw-r--r--   0        0        0      360 2024-04-24 18:22:05.368911 qg_toolkit-1.0.0/tools/galxe_qg.yaml
--rw-r--r--   0        0        0     5653 2024-04-20 21:44:47.711324 qg_toolkit-1.0.0/tools/qg_airdrop.py
--rw-r--r--   0        0        0      985 2024-04-20 20:27:34.147592 qg_toolkit-1.0.0/tools/qg_crypto.py
--rw-r--r--   0        0        0    35670 2024-04-20 21:42:00.231604 qg_toolkit-1.0.0/tools/qg_eth.py
--rw-r--r--   0        0        0     3594 2024-04-20 20:29:00.648873 qg_toolkit-1.0.0/tools/qg_file.py
--rw-r--r--   0        0        0      741 2024-04-20 20:24:22.248041 qg_toolkit-1.0.0/tools/qg_random.py
--rw-r--r--   0        0        0     6143 2024-04-20 20:02:39.286618 qg_toolkit-1.0.0/tools/qg_solana.py
--rw-r--r--   0        0        0     2764 2024-04-24 18:21:31.477405 qg_toolkit-1.0.0/tools/qg_starknet.py
--rw-r--r--   0        0        0     3241 2024-04-20 19:48:15.080086 qg_toolkit-1.0.0/tools/qproxy.py
--rw-r--r--   0        0        0     6050 2024-04-20 21:14:04.319021 qg_toolkit-1.0.0/tools/rpc.py
--rw-r--r--   0        0        0      812 1970-01-01 00:00:00.000000 qg_toolkit-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      602 2024-04-27 10:46:21.403031 qg_toolkit-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4871 2024-04-27 05:30:59.226522 qg_toolkit-1.0.2/qtweepy/examples/account_checker.py
+-rw-r--r--   0        0        0     2210 2024-04-20 19:48:15.064902 qg_toolkit-1.0.2/qtweepy/examples/follow_each_other.py
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.415935 qg_toolkit-1.0.2/qtweepy/examples/input-output/BAD_TOKEN.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.2/qtweepy/examples/input-output/CONSENT_LOCKED.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.2/qtweepy/examples/input-output/GOOD.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.2/qtweepy/examples/input-output/LOCKED.txt
+-rw-r--r--   0        0        0       46 2024-04-27 05:31:06.618786 qg_toolkit-1.0.2/qtweepy/examples/input-output/PROXIES.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.2/qtweepy/examples/input-output/SUSPENDED.txt
+-rw-r--r--   0        0        0       40 2024-04-27 05:31:12.415935 qg_toolkit-1.0.2/qtweepy/examples/input-output/UNKNOWN.txt
+-rw-r--r--   0        0        0     3581 2024-04-20 19:48:15.065903 qg_toolkit-1.0.2/qtweepy/examples/mavia.py
+-rw-r--r--   0        0        0     2332 2024-04-20 19:48:15.066903 qg_toolkit-1.0.2/qtweepy/examples/set_2fa.py
+-rw-r--r--   0        0        0     3040 2024-04-20 19:48:15.066903 qg_toolkit-1.0.2/qtweepy/examples/set_avatars_and_banners.py
+-rw-r--r--   0        0        0      686 2024-04-20 19:48:15.066903 qg_toolkit-1.0.2/qtweepy/examples/uploading_images.py
+-rw-r--r--   0        0        0     2212 2024-04-20 19:48:15.067902 qg_toolkit-1.0.2/qtweepy/examples/voter.py
+-rw-r--r--   0        0        0     3079 2024-04-20 19:48:15.067902 qg_toolkit-1.0.2/qtweepy/examples/xai.py
+-rw-r--r--   0        0        0      687 2024-04-20 19:57:03.446998 qg_toolkit-1.0.2/qtweepy/pyproject.toml
+-rw-r--r--   0        0        0     8720 2024-04-20 19:48:15.063903 qg_toolkit-1.0.2/qtweepy/README.md
+-rw-r--r--   0        0        0      132 2024-04-24 18:22:26.184000 qg_toolkit-1.0.2/qtweepy/tea.yaml
+-rw-r--r--   0        0        0      732 2024-04-20 19:48:15.068902 qg_toolkit-1.0.2/qtweepy/twitter/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/core/__init__.py
+-rw-r--r--   0        0        0     8883 2024-04-20 19:48:15.070903 qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/core/base.py
+-rw-r--r--   0        0        0     1054 2024-04-20 19:48:15.070903 qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/core/config.py
+-rw-r--r--   0        0        0     1741 2024-04-20 19:48:15.071903 qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/core/enum.py
+-rw-r--r--   0        0        0     2602 2024-04-20 19:48:15.071903 qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/core/serializer.py
+-rw-r--r--   0        0        0    10974 2024-04-20 19:48:15.072903 qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/fun_captcha.py
+-rw-r--r--   0        0        0     3248 2024-04-20 19:48:15.072903 qg_toolkit-1.0.2/qtweepy/twitter/account.py
+-rw-r--r--   0        0        0      141 2024-04-20 19:48:15.072903 qg_toolkit-1.0.2/qtweepy/twitter/base/__init__.py
+-rw-r--r--   0        0        0      500 2024-04-20 19:48:15.074292 qg_toolkit-1.0.2/qtweepy/twitter/base/client.py
+-rw-r--r--   0        0        0     2164 2024-04-20 19:48:15.074413 qg_toolkit-1.0.2/qtweepy/twitter/base/session.py
+-rw-r--r--   0        0        0    70738 2024-04-20 19:48:15.075686 qg_toolkit-1.0.2/qtweepy/twitter/client.py
+-rw-r--r--   0        0        0      267 2024-04-20 19:48:15.076283 qg_toolkit-1.0.2/qtweepy/twitter/enums.py
+-rw-r--r--   0        0        0     5322 2024-04-20 19:48:15.076811 qg_toolkit-1.0.2/qtweepy/twitter/errors.py
+-rw-r--r--   0        0        0     4695 2024-04-20 19:48:15.076811 qg_toolkit-1.0.2/qtweepy/twitter/models.py
+-rw-r--r--   0        0        0      665 2024-04-20 19:48:15.077920 qg_toolkit-1.0.2/qtweepy/twitter/utils/__init__.py
+-rw-r--r--   0        0        0     1152 2024-04-20 19:48:15.077920 qg_toolkit-1.0.2/qtweepy/twitter/utils/file.py
+-rw-r--r--   0        0        0     2140 2024-04-20 19:48:15.078463 qg_toolkit-1.0.2/qtweepy/twitter/utils/html.py
+-rw-r--r--   0        0        0     1061 2024-04-20 19:48:15.078992 qg_toolkit-1.0.2/qtweepy/twitter/utils/other.py
+-rw-r--r--   0        0        0       38 2024-04-20 19:50:56.436133 qg_toolkit-1.0.2/README.md
+-rw-r--r--   0        0        0      132 2024-04-27 10:46:21.398031 qg_toolkit-1.0.2/tea.yaml
+-rw-r--r--   0        0        0      279 2024-04-24 18:54:00.529601 qg_toolkit-1.0.2/tools/demo.yaml
+-rw-r--r--   0        0        0     5432 2024-04-26 20:14:27.357118 qg_toolkit-1.0.2/tools/qg_airdrop.py
+-rw-r--r--   0        0        0      985 2024-04-20 20:27:34.147592 qg_toolkit-1.0.2/tools/qg_crypto.py
+-rw-r--r--   0        0        0    35634 2024-04-26 20:13:35.014431 qg_toolkit-1.0.2/tools/qg_eth.py
+-rw-r--r--   0        0        0     3594 2024-04-20 20:29:00.648873 qg_toolkit-1.0.2/tools/qg_file.py
+-rw-r--r--   0        0        0      300 2024-04-24 18:53:34.062471 qg_toolkit-1.0.2/tools/qg_models.py
+-rw-r--r--   0        0        0      741 2024-04-20 20:24:22.248041 qg_toolkit-1.0.2/tools/qg_random.py
+-rw-r--r--   0        0        0     6143 2024-04-20 20:02:39.286618 qg_toolkit-1.0.2/tools/qg_solana.py
+-rw-r--r--   0        0        0     2764 2024-04-24 18:21:31.477405 qg_toolkit-1.0.2/tools/qg_starknet.py
+-rw-r--r--   0        0        0     3241 2024-04-20 19:48:15.080086 qg_toolkit-1.0.2/tools/qproxy.py
+-rw-r--r--   0        0        0     6050 2024-04-20 21:14:04.319021 qg_toolkit-1.0.2/tools/rpc.py
+-rw-r--r--   0        0        0      812 1970-01-01 00:00:00.000000 qg_toolkit-1.0.2/PKG-INFO
```

### Comparing `qg_toolkit-1.0.0/pyproject.toml` & `qg_toolkit-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qg_toolkit"
-version = "1.0.0"
+version = "1.0.2"
 description = "qg_toolkit for Python!"
 authors = ["qg <qg@gmail.com>"]
 readme = "README.md"
 packages = [{include = "qtweepy"},{include = "tools"}]
 include = [{path = "tea.yaml"}]
```

### Comparing `qg_toolkit-1.0.0/qtweepy/examples/account_checker.py` & `qg_toolkit-1.0.2/qtweepy/examples/account_checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     await asyncio.gather(*(sem_task(task) for task in tasks))
 
 
 def sort_accounts(
     accounts: Iterable[TwitterAccountWithAdditionalData],
 ) -> SortedAccounts:
     status_to_account_with_additional_data = {
-        status: list() for status in qtweepy.AccountStatus
+        f'{status}': list() for status in qtweepy.twitter.AccountStatus
     }
     for additional_data, account in accounts:
         status_to_account_with_additional_data[account.status].append(
             (additional_data, account)
         )
     return status_to_account_with_additional_data
 
@@ -115,15 +115,15 @@
         proxies = [None]
 
     proxy_to_account_list = list(zip(cycle(proxies), accounts))
 
     tasks = []
     for proxy, account_with_additional_data in proxy_to_account_list:
         account = account_with_additional_data[1]
-        if account.status == AccountStatus.UNKNOWN:
+        if account.status == AccountStatus.UNKNOWN.value:
             tasks.append(establish_account_status(account, proxy=proxy))
     try:
         await limited_gather(tasks, limit=MAX_TASKS)
     finally:
         sorted_accounts = sort_accounts(accounts)
         save_sorted_accounts_with_additional_data(sorted_accounts)
         print_statistic(sorted_accounts)
```

### Comparing `qg_toolkit-1.0.0/qtweepy/examples/follow_each_other.py` & `qg_toolkit-1.0.2/qtweepy/examples/follow_each_other.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/examples/mavia.py` & `qg_toolkit-1.0.2/qtweepy/examples/mavia.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/examples/set_2fa.py` & `qg_toolkit-1.0.2/qtweepy/examples/set_2fa.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/examples/set_avatars_and_banners.py` & `qg_toolkit-1.0.2/qtweepy/examples/set_avatars_and_banners.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/examples/uploading_images.py` & `qg_toolkit-1.0.2/qtweepy/examples/uploading_images.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/examples/voter.py` & `qg_toolkit-1.0.2/qtweepy/examples/voter.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/examples/xai.py` & `qg_toolkit-1.0.2/qtweepy/examples/xai.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/pyproject.toml` & `qg_toolkit-1.0.2/qtweepy/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/README.md` & `qg_toolkit-1.0.2/qtweepy/README.md`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/twitter/__init__.py` & `qg_toolkit-1.0.2/qtweepy/twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/twitter/_capsolver/core/base.py` & `qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/core/base.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/twitter/_capsolver/core/config.py` & `qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/core/config.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/twitter/_capsolver/core/enum.py` & `qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/core/enum.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/twitter/_capsolver/core/serializer.py` & `qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/core/serializer.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/twitter/_capsolver/fun_captcha.py` & `qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/fun_captcha.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/twitter/account.py` & `qg_toolkit-1.0.2/qtweepy/twitter/account.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/twitter/base/session.py` & `qg_toolkit-1.0.2/qtweepy/twitter/base/session.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/twitter/client.py` & `qg_toolkit-1.0.2/qtweepy/twitter/client.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/twitter/errors.py` & `qg_toolkit-1.0.2/qtweepy/twitter/errors.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/twitter/models.py` & `qg_toolkit-1.0.2/qtweepy/twitter/models.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/twitter/utils/__init__.py` & `qg_toolkit-1.0.2/qtweepy/twitter/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/twitter/utils/file.py` & `qg_toolkit-1.0.2/qtweepy/twitter/utils/file.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/twitter/utils/html.py` & `qg_toolkit-1.0.2/qtweepy/twitter/utils/html.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/qtweepy/twitter/utils/other.py` & `qg_toolkit-1.0.2/qtweepy/twitter/utils/other.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/tools/qg_airdrop.py` & `qg_toolkit-1.0.2/tools/qg_airdrop.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,50 @@
 import concurrent.futures
 import copy
-from typing import List
+from threading import Lock
 
-from pydantic import Field
 from web3 import Web3
 
 from tools.qg_eth import QGEth
 from tools.qg_file import QGFile
 
 
 class QGAirDrop(QGEth):
-    # 每个号留多少
-    chain_name: str = None
-    # 每个号转多少
-    per_value: float = None
-    # 自己号留多少
-    left_value: float = None
-    # 是否检查接受账户余额
-    is_check_receiver: bool = False
-    # 检查接受账户余额是否有足够的量，不足就转，足够不转
-    check_balance: float = 0.0000001
-    receiver_accounts: List = Field(None, validate=False)
-
-    #
-    class Config:
-        avalidate_assignment = True
+    lock = Lock()
 
-    def __init__(self, **kwargs):
+    def __init__(self, chain_name=None, per_value=None, left_value=None, is_check_receiver=False, check_balance=0.0000001, receiver_accounts=[], **kwargs):
         super().__init__(**kwargs)
-        self.receiver_accounts = []
-        self.contract_map = {
+        self.chain_name = chain_name
+        self.per_value = per_value
+        self.left_value = left_value
+        self.is_check_receiver = is_check_receiver
+        self.check_balance = check_balance
+        self.receiver_accounts = receiver_accounts or []
+
+        self.init_chains(self.chain_name)
+        self.w3 = getattr(self, f"{self.chain_name}_w3", None)
+        self.w3_balance = getattr(self, f"{self.chain_name}_balance", None)
+        self.fenpei()
+
+    @property
+    def contract_map(self):
+        return {
             "polygon": "0xDCB4a16EB4F5F8214962357c96584F6955B9b525",
             "bsc": "0x0Ff88bdD9BE134F29dD660C4F220DD1e392e49E4",
             "opbnb": "0x501Ab65Ec2E89aB6e9CBfE6eE3AED423995b1aef",
             "goerli": "0x9680D1e126bBeF521F97b6FFB2fe39Da5c88C290",
             "sepolia": "0xEf50B70800f0D5D89b7a0056A0746845C2Dbe7b7",
             "linea": "0x2Ce164CbdBFb8fA0BEbf1f2dCD2F364481Fa86d3",
             "mantle": "0x601074C151C229d04D339F807817e8cB87E6CF1e",
             "berachain": "0xaB06c32FCE992B423F17e57BCC78C1cA80dd7AaA",
             "blast": "0x8B4a4AA2fD4bB59eBBEB987D229A3eb01f987E7b",
             "zeta": "0xBc4A4b3846C3F2F8085689F0A4A09D76627b6c2E",
             "holesky": "0x42d5f4D80dC931644627127385F51F07eb8a485D",
             "xter": "0x7347Ae5a53F7b80A7eF6654E3b8eA0c0E396a4D3"
         }
-        self.init_chains(self.chain_name)
-        self.w3 = getattr(self, f"{self.chain_name}_w3", None)
-        self.w3_balance = getattr(self, f"{self.chain_name}_balance", None)
-        self.fenpei()
 
     def batch_send_eth_by_lian(self):
         print(f'【{self.address}】【{self.index}】接收地址数量：{len(self.receiver_accounts)}')
         if len(self.receiver_accounts) == 0:
             return
         address_arr = self.receiver_accounts
         value = self.per_value
@@ -79,50 +73,50 @@
         # self.sent_tx_with_assembled(self.w3, to_address, to_value, input_data, action_name)
         self.sent_tx_with_assembled_by_type0(self.w3, to_address, to_value, input_data, action_name)
 
     def fenpei(self):
         can_num = int(float(float(self.w3_balance) - self.left_value) / float(self.per_value))
         if can_num < 0:
             can_num = 0
-        global receiver_accounts
+        global rs
         QGAirDrop.lock.acquire()
         if self.is_check_receiver:
-            rs = copy.deepcopy(receiver_accounts)
+            rs = copy.deepcopy(rs)
             for addr in rs:
                 if self.get_balance_from_web3(self.w3, addr) < self.check_balance:
                     self.receiver_accounts.append(addr)
-                receiver_accounts.pop(0)
+                rs.pop(0)
                 if len(self.receiver_accounts) >= can_num:
                     break
         else:
-            self.receiver_accounts = receiver_accounts[:can_num]
-            receiver_accounts = receiver_accounts[can_num:]
+            self.receiver_accounts = rs[:can_num]
+            rs = rs[can_num:]
         QGAirDrop.lock.release()
         print(f'{self.address} 分配账号数量{len(self.receiver_accounts)}:{self.receiver_accounts}')
 
 
 def qg_task(index, address, private_key, mnemonic):
     chain_name = "opbnb"
     # 每个号空投多少
     per_value = "0.00015"
     # 给自己号剩余多少
-    left_value = 0.01
+    left_value = 1
     # 是否检查接收者余额
     is_check_receiver = True
     # 检查接收者余额是否大于N
     check_balance = 0.0001
     batch = QGAirDrop(index=index, address=address, private_key=private_key, mnemonic=mnemonic,
                       chain_name=chain_name, per_value=per_value, left_value=left_value,
                       is_check_receiver=is_check_receiver, check_balance=check_balance)
     batch.batch_send_eth_by_lian()
 
 
 if __name__ == '__main__':
-    accounts = QGFile.read_yaml("galxe_qg.yaml")["accounts"]
-    receiver_accounts = [x["address"] for x in QGFile.read_yaml("galxe_qg.yaml")["accounts"]][1:]
+    accounts = QGFile.read_yaml("demo.yaml")["accounts"]
+    rs = [x["address"] for x in QGFile.read_yaml("demo.yaml")["accounts"]][1:]
     executor = concurrent.futures.ThreadPoolExecutor(max_workers=1)
     for i, account in enumerate(accounts, start=1):
         if not isinstance(account, list):
             addr1 = account.get('address')
             pk1 = account.get('private_key')
         else:
             addr1 = account[0]
```

### Comparing `qg_toolkit-1.0.0/tools/qg_crypto.py` & `qg_toolkit-1.0.2/tools/qg_crypto.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/tools/qg_eth.py` & `qg_toolkit-1.0.2/tools/qg_eth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,55 +1,48 @@
 import base64
 import binascii
 import inspect
 import random
+from dataclasses import dataclass, field
 from decimal import Decimal
 from pathlib import Path
-from typing import Union
+from typing import Union, Dict
 
 import requests
 from eth_account import Account
-from eth_account.messages import encode_defunct, encode_structured_data
-from pydantic import BaseModel
+from eth_account.messages import encode_defunct, encode_typed_data
 from retry import retry
 from web3 import Web3
 from web3.auto import w3
 
 from loguru import logger
 from rpc import endpoints, bases, apis
 
 
-class QGEth(BaseModel):
-    index: int
-    address: str = None
-    private_key: Union[str,int,None] = None
-    mnemonic: str = None
-    chain_instances: dict = {}
-
-    class Config:
-        arbitrary_types_allowed = True
-        validate_default = False
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        if 'address' not in kwargs:
-            self.address = Web3.to_checksum_address(self.address)
-
+class QGEth:
+    def __init__(self, index, address=None, private_key=None, mnemonic=None, chain_instances=None):
+        self.index = index
+        self.address = address
+        self.private_key = private_key
+        self.mnemonic = mnemonic
+        self.chain_instances = chain_instances or {}
+        if self.address is None:
+            self.address = Account.from_key(private_key).address
 
     @retry(tries=2, delay=1, backoff=1, max_delay=3)
     def init_chains(self, *chain_names):
         try:
             for name in chain_names:
                 web3 = getattr(self, f"{name}_w3", None)
                 if web3 is None:
                     self.add_chain(name)
                     self.add_balance(name)
             chains_info = []
             for chain_name, web3_instance in self.chain_instances.items():
-                chains_info.append(f"{chain_name}余额:{self.get_balance_from_attr(chain_name)}")
+                chains_info.append(f"{chain_name}余额:{self.get_balance_by_chain(chain_name)}")
             print(f"【{self.index}】【{self.address}】余额情况 {','.join(chains_info)}")
         except Exception as e:
             print(e)
             raise Exception("初始化失败！")
 
     def add_chain(self, chain_name):
         endpoint = endpoints.get(chain_name)
@@ -76,15 +69,15 @@
             return None
 
     def get_balance_from_web3(self, w3, addr):
         """获取指定地址的余额"""
         balance = Web3.from_wei(w3.eth.get_balance(addr), 'ether')
         return balance
 
-    def get_balance_from_attr(self, chain_name):
+    def get_balance_by_chain(self, chain_name):
         web3_balance = getattr(self, f"{chain_name}_balance", None)
         return web3_balance
 
     def get_token_balance(self, w3, contract_address):
         """
         查询指定代币的余额
         """
@@ -343,15 +336,15 @@
         message = encode_defunct(text=msg)
         signed_message = w3.eth.account.sign_message(message, private_key=self.private_key)
         signed_data = signed_message.signature
         # print("签名后:" + signed_data.hex())
         return signed_data.hex()
 
     def sign_712(self, data):
-        encoded_message = encode_structured_data(data)
+        encoded_message = encode_typed_data(data)
         signed_message = Account.sign_message(encoded_message, private_key=self.private_key)
         # print('Signature:', signed_message.signature.hex())
         return signed_message.signature.hex()
 
     @retry(tries=5, delay=1, backoff=2, max_delay=5)
     def get_data(self, chain_name, req_type, *params):
         url = f"{bases.get(chain_name)}{apis.get(req_type).format(*params)}&page=1&offset=1000&sort=asc"
```

### Comparing `qg_toolkit-1.0.0/tools/qg_file.py` & `qg_toolkit-1.0.2/tools/qg_file.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/tools/qg_random.py` & `qg_toolkit-1.0.2/tools/qg_random.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/tools/qg_solana.py` & `qg_toolkit-1.0.2/tools/qg_solana.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/tools/qg_starknet.py` & `qg_toolkit-1.0.2/tools/qg_starknet.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/tools/qproxy.py` & `qg_toolkit-1.0.2/tools/qproxy.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/tools/rpc.py` & `qg_toolkit-1.0.2/tools/rpc.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.0/PKG-INFO` & `qg_toolkit-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qg_toolkit
-Version: 1.0.0
+Version: 1.0.2
 Summary: qg_toolkit for Python!
 Author: qg
 Author-email: qg@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

