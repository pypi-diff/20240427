# Comparing `tmp/dnevnik-mos-ru-api-1.2.8.tar.gz` & `tmp/dnevnik-mos-ru-api-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnevnik-mos-ru-api-1.2.8.tar", last modified: Fri Mar  1 20:06:13 2024, max compression
+gzip compressed data, was "dnevnik-mos-ru-api-1.2.9.tar", last modified: Sat Apr 27 21:37:08 2024, max compression
```

## Comparing `dnevnik-mos-ru-api-1.2.8.tar` & `dnevnik-mos-ru-api-1.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-03-01 20:06:13.917960 dnevnik-mos-ru-api-1.2.8/
--rw-rw-rw-   0        0        0      516 2024-03-01 20:06:13.916961 dnevnik-mos-ru-api-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-02-29 20:52:56.000000 dnevnik-mos-ru-api-1.2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-01 20:06:13.896963 dnevnik-mos-ru-api-1.2.8/dnevnik/
--rw-rw-rw-   0        0        0     1091 2024-02-29 18:33:31.000000 dnevnik-mos-ru-api-1.2.8/dnevnik/Authenticator.py
--rw-rw-rw-   0        0        0    34651 2024-03-01 20:05:08.000000 dnevnik-mos-ru-api-1.2.8/dnevnik/Client.py
--rw-rw-rw-   0        0        0      581 2024-02-29 18:39:19.000000 dnevnik-mos-ru-api-1.2.8/dnevnik/FileAuthenticator.py
--rw-rw-rw-   0        0        0       52 2024-02-29 19:21:48.000000 dnevnik-mos-ru-api-1.2.8/dnevnik/IncorrectLoginPassword.py
--rw-rw-rw-   0        0        0     9060 2024-03-01 16:55:47.000000 dnevnik-mos-ru-api-1.2.8/dnevnik/PlayWrightAuthenticator.py
--rw-rw-rw-   0        0        0      522 2024-02-29 18:42:33.000000 dnevnik-mos-ru-api-1.2.8/dnevnik/PredefinedAuthenticator.py
--rw-rw-rw-   0        0        0       41 2024-02-29 19:12:37.000000 dnevnik-mos-ru-api-1.2.8/dnevnik/TOTPRequested.py
--rw-rw-rw-   0        0        0      359 2024-03-01 15:53:12.000000 dnevnik-mos-ru-api-1.2.8/dnevnik/Utils.py
--rw-rw-rw-   0        0        0      397 2024-03-01 19:47:59.000000 dnevnik-mos-ru-api-1.2.8/dnevnik/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-01 20:06:13.915962 dnevnik-mos-ru-api-1.2.8/dnevnik_mos_ru_api.egg-info/
--rw-rw-rw-   0        0        0      516 2024-03-01 20:06:13.000000 dnevnik-mos-ru-api-1.2.8/dnevnik_mos_ru_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2024-03-01 20:06:13.000000 dnevnik-mos-ru-api-1.2.8/dnevnik_mos_ru_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-01 20:06:13.000000 dnevnik-mos-ru-api-1.2.8/dnevnik_mos_ru_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-03-01 20:06:13.000000 dnevnik-mos-ru-api-1.2.8/dnevnik_mos_ru_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-01 20:06:13.000000 dnevnik-mos-ru-api-1.2.8/dnevnik_mos_ru_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-01 20:06:13.917960 dnevnik-mos-ru-api-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      454 2024-03-01 19:47:59.000000 dnevnik-mos-ru-api-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 21:37:08.195047 dnevnik-mos-ru-api-1.2.9/
+-rw-rw-rw-   0        0        0      516 2024-04-27 21:37:08.194048 dnevnik-mos-ru-api-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-02-29 20:52:56.000000 dnevnik-mos-ru-api-1.2.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 21:37:08.177046 dnevnik-mos-ru-api-1.2.9/dnevnik/
+-rw-rw-rw-   0        0        0     1091 2024-02-29 18:33:31.000000 dnevnik-mos-ru-api-1.2.9/dnevnik/Authenticator.py
+-rw-rw-rw-   0        0        0    36225 2024-04-27 21:35:02.000000 dnevnik-mos-ru-api-1.2.9/dnevnik/DnevnikClient.py
+-rw-rw-rw-   0        0        0      581 2024-02-29 18:39:19.000000 dnevnik-mos-ru-api-1.2.9/dnevnik/FileAuthenticator.py
+-rw-rw-rw-   0        0        0       52 2024-02-29 19:21:48.000000 dnevnik-mos-ru-api-1.2.9/dnevnik/IncorrectLoginPassword.py
+-rw-rw-rw-   0        0        0     9060 2024-03-01 16:55:47.000000 dnevnik-mos-ru-api-1.2.9/dnevnik/PlayWrightAuthenticator.py
+-rw-rw-rw-   0        0        0      522 2024-02-29 18:42:33.000000 dnevnik-mos-ru-api-1.2.9/dnevnik/PredefinedAuthenticator.py
+-rw-rw-rw-   0        0        0       41 2024-02-29 19:12:37.000000 dnevnik-mos-ru-api-1.2.9/dnevnik/TOTPRequested.py
+-rw-rw-rw-   0        0        0      359 2024-03-01 15:53:12.000000 dnevnik-mos-ru-api-1.2.9/dnevnik/Utils.py
+-rw-rw-rw-   0        0        0      411 2024-04-27 21:35:42.000000 dnevnik-mos-ru-api-1.2.9/dnevnik/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 21:37:08.193046 dnevnik-mos-ru-api-1.2.9/dnevnik_mos_ru_api.egg-info/
+-rw-rw-rw-   0        0        0      516 2024-04-27 21:37:08.000000 dnevnik-mos-ru-api-1.2.9/dnevnik_mos_ru_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2024-04-27 21:37:08.000000 dnevnik-mos-ru-api-1.2.9/dnevnik_mos_ru_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 21:37:08.000000 dnevnik-mos-ru-api-1.2.9/dnevnik_mos_ru_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-27 21:37:08.000000 dnevnik-mos-ru-api-1.2.9/dnevnik_mos_ru_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-27 21:37:08.000000 dnevnik-mos-ru-api-1.2.9/dnevnik_mos_ru_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 21:37:08.195047 dnevnik-mos-ru-api-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      454 2024-04-27 21:35:42.000000 dnevnik-mos-ru-api-1.2.9/setup.py
```

### Comparing `dnevnik-mos-ru-api-1.2.8/PKG-INFO` & `dnevnik-mos-ru-api-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnevnik-mos-ru-api
-Version: 1.2.8
+Version: 1.2.9
 Summary: API for dnevnik.mos.ru
 Author: RedGuy
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: playwright==1.41.2
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: mintotp==0.3.0
```

### Comparing `dnevnik-mos-ru-api-1.2.8/dnevnik/Authenticator.py` & `dnevnik-mos-ru-api-1.2.9/dnevnik/Authenticator.py`

 * *Files identical despite different names*

### Comparing `dnevnik-mos-ru-api-1.2.8/dnevnik/Client.py` & `dnevnik-mos-ru-api-1.2.9/dnevnik/DnevnikClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import aiohttp
 from datetime import datetime, timezone
 from . import Authenticator, Utils
 import json
 import pytz
 
 
-class Client:
+class DnevnikClient:
     _authenticator: Authenticator
 
     def __init__(self, authenticator: Authenticator):
         self._authenticator = authenticator
 
     async def get_profile(self, with_groups=False, with_parents=False, with_assignments=False,
                           with_ec_attendances=False, with_ae_attendances=False,
@@ -85,14 +85,35 @@
                     final_mark["updated_at"] = None if "updated_at" not in final_mark else datetime.strptime(
                         final_mark["updated_at"], "%d.%m.%Y %H:%M")
                     final_mark["deleted_at"] = None if "deleted_at" not in final_mark else datetime.strptime(
                         final_mark["deleted_at"], "%d.%m.%Y %H:%M")
 
                 return res
 
+    async def get_profile_v2(self):
+        async with aiohttp.ClientSession() as session:
+            async with await session.get("https://school.mos.ru/api/family/web/v1/profile/", headers={
+                "Auth-Token": await self._authenticator.get_token(),
+                "Profile-Id": await self._authenticator.get_student_id(),
+                "x-mes-subsystem": "familyweb"
+            }) as response:
+                res = await response.json()
+
+                if res["profile"] is None:
+                    res["profile"] = {}
+                res["profile"]["birth_date"] = datetime.strptime(res["profile"]["birth_date"], '%Y-%m-%d')
+
+                for child in res["children"]:
+                    child["birth_date"] = datetime.strptime(child["birth_date"], '%Y-%m-%d')
+                    child["enrollment_date"] = datetime.strptime(child["enrollment_date"], '%Y-%m-%d')
+
+                    for representative in child["representatives"]:
+                        representative["birth_date"] = datetime.strptime(representative["birth_date"], '%Y-%m-%d') if representative['birth_date'] else None
+                return res
+
     async def get_average_marks(self):
         async with aiohttp.ClientSession() as session:
             async with session.get("https://dnevnik.mos.ru/reports/api/progress/json?academic_year_id=" + str(
                     (await self.get_current_academic_year())["id"]) + "&student_profile_id=" + str(
                 await self._authenticator.get_student_id()), headers={
                 "Auth-Token": await self._authenticator.get_token(),
                 "Profile-Id": await self._authenticator.get_student_id()
@@ -468,25 +489,35 @@
                 notification['new_date_assigned_on'] = datetime.strptime(notification['new_date_assigned_on'],
                                                                          "%Y-%m-%d %H:%M:%S")
                 notification['new_date_prepared_for'] = datetime.strptime(notification['new_date_prepared_for'],
                                                                           "%Y-%m-%d %H:%M:%S")
 
         return report
 
-    async def get_visits(self, from_date=datetime.now(), to_date=datetime.now()):
+    async def get_visits(self, from_date=datetime.now(), to_date=datetime.now(), use_v2_profile=True):
         from_date_str = from_date.astimezone(pytz.timezone('Europe/Moscow')).strftime("%Y-%m-%d")
         to_date_str = to_date.astimezone(pytz.timezone('Europe/Moscow')).strftime("%Y-%m-%d")
-        profile = await self.get_profile()
+        ispp = ""
+        if use_v2_profile:
+            profile = await self.get_profile_v2()
+            for child in profile["children"]:
+                if child["contract_id"] is not None:
+                    ispp = child["contract_id"]
+                    break
+        else:
+            profile = await self.get_profile()
+            ispp = profile['ispp_account']
         async with aiohttp.ClientSession() as session:
             async with session.get(
-                    f"https://dnevnik.mos.ru/mobile/api/visits?from={from_date_str}&to={to_date_str}&contract_id={profile['ispp_account']}",
+                    f"https://school.mos.ru/api/family/web/v1/visits?from={from_date_str}&to={to_date_str}&contract_id={ispp}",
                     headers={
                         "Cookie": f"auth_token={await self._authenticator.get_token()}; student_id={await self._authenticator.get_student_id()};",
                         "Auth-Token": await self._authenticator.get_token(),
-                        "Profile-Id": await self._authenticator.get_student_id()
+                        "Profile-Id": await self._authenticator.get_student_id(),
+                "x-mes-subsystem": "familyweb"
                     }) as response:
                 report = await response.json()
 
         for visit in report['payload']:
             visit['date'] = datetime.strptime(visit['date'], "%Y-%m-%d")
             for enter in visit['visits']:
                 if ":" in enter['in']:
@@ -627,12 +658,12 @@
             year['begin_date'] = datetime.strptime(year['begin_date'], "%y-%m-%d")
             year['end_date'] = datetime.strptime(year['end_date'], "%y-%m-%d")
 
         return res
 
     @staticmethod
     async def get_current_academic_year():
-        res = await Client.get_academic_years()
+        res = await DnevnikClient.get_academic_years()
         for year in res:
             if year['current_year']:
                 return year
         return None
```

### Comparing `dnevnik-mos-ru-api-1.2.8/dnevnik/FileAuthenticator.py` & `dnevnik-mos-ru-api-1.2.9/dnevnik/FileAuthenticator.py`

 * *Files identical despite different names*

### Comparing `dnevnik-mos-ru-api-1.2.8/dnevnik/PlayWrightAuthenticator.py` & `dnevnik-mos-ru-api-1.2.9/dnevnik/PlayWrightAuthenticator.py`

 * *Files identical despite different names*

### Comparing `dnevnik-mos-ru-api-1.2.8/dnevnik/PredefinedAuthenticator.py` & `dnevnik-mos-ru-api-1.2.9/dnevnik/PredefinedAuthenticator.py`

 * *Files identical despite different names*

### Comparing `dnevnik-mos-ru-api-1.2.8/dnevnik_mos_ru_api.egg-info/PKG-INFO` & `dnevnik-mos-ru-api-1.2.9/dnevnik_mos_ru_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnevnik-mos-ru-api
-Version: 1.2.8
+Version: 1.2.9
 Summary: API for dnevnik.mos.ru
 Author: RedGuy
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: playwright==1.41.2
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: mintotp==0.3.0
```

