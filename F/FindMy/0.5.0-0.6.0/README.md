# Comparing `tmp/findmy-0.5.0.tar.gz` & `tmp/findmy-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmy-0.5.0.tar", max compression
+gzip compressed data, was "findmy-0.6.0.tar", max compression
```

## Comparing `findmy-0.5.0.tar` & `findmy-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1079 2024-02-29 17:20:52.119771 findmy-0.5.0/LICENSE.md
--rw-r--r--   0        0        0     3652 2024-02-29 17:20:52.119771 findmy-0.5.0/README.md
--rw-r--r--   0        0        0      302 2024-02-29 17:20:52.119771 findmy-0.5.0/findmy/__init__.py
--rw-r--r--   0        0        0     5853 2024-02-29 17:20:52.119771 findmy-0.5.0/findmy/accessory.py
--rw-r--r--   0        0        0      537 2024-02-29 17:20:52.119771 findmy-0.5.0/findmy/errors.py
--rw-r--r--   0        0        0     4407 2024-02-29 17:20:52.119771 findmy-0.5.0/findmy/keys.py
--rw-r--r--   0        0        0      431 2024-02-29 17:20:52.119771 findmy-0.5.0/findmy/reports/__init__.py
--rw-r--r--   0        0        0    31175 2024-02-29 17:20:52.119771 findmy-0.5.0/findmy/reports/account.py
--rw-r--r--   0        0        0     3005 2024-02-29 17:20:52.119771 findmy-0.5.0/findmy/reports/anisette.py
--rw-r--r--   0        0        0     7963 2024-02-29 17:20:52.119771 findmy-0.5.0/findmy/reports/reports.py
--rw-r--r--   0        0        0      836 2024-02-29 17:20:52.119771 findmy-0.5.0/findmy/reports/state.py
--rw-r--r--   0        0        0     7151 2024-02-29 17:20:52.119771 findmy-0.5.0/findmy/reports/twofactor.py
--rw-r--r--   0        0        0      148 2024-02-29 17:20:52.119771 findmy-0.5.0/findmy/scanner/__init__.py
--rw-r--r--   0        0        0     6994 2024-02-29 17:20:52.119771 findmy-0.5.0/findmy/scanner/scanner.py
--rw-r--r--   0        0        0      201 2024-02-29 17:20:52.119771 findmy-0.5.0/findmy/util/__init__.py
--rw-r--r--   0        0        0     1043 2024-02-29 17:20:52.119771 findmy-0.5.0/findmy/util/closable.py
--rw-r--r--   0        0        0     1234 2024-02-29 17:20:52.119771 findmy-0.5.0/findmy/util/crypto.py
--rw-r--r--   0        0        0     3603 2024-02-29 17:20:52.119771 findmy-0.5.0/findmy/util/http.py
--rw-r--r--   0        0        0      500 2024-02-29 17:20:52.119771 findmy-0.5.0/findmy/util/parsers.py
--rw-r--r--   0        0        0      120 2024-02-29 17:20:52.119771 findmy-0.5.0/findmy/util/types.py
--rw-r--r--   0        0        0     1316 2024-02-29 17:20:52.119771 findmy-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4395 1970-01-01 00:00:00.000000 findmy-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-27 14:40:52.098734 findmy-0.6.0/LICENSE.md
+-rw-r--r--   0        0        0     3668 2024-04-27 14:40:52.098734 findmy-0.6.0/README.md
+-rw-r--r--   0        0        0      302 2024-04-27 14:40:52.098734 findmy-0.6.0/findmy/__init__.py
+-rw-r--r--   0        0        0     8463 2024-04-27 14:40:52.098734 findmy-0.6.0/findmy/accessory.py
+-rw-r--r--   0        0        0      537 2024-04-27 14:40:52.098734 findmy-0.6.0/findmy/errors.py
+-rw-r--r--   0        0        0     4407 2024-04-27 14:40:52.098734 findmy-0.6.0/findmy/keys.py
+-rw-r--r--   0        0        0      481 2024-04-27 14:40:52.098734 findmy-0.6.0/findmy/reports/__init__.py
+-rw-r--r--   0        0        0    34186 2024-04-27 14:40:52.098734 findmy-0.6.0/findmy/reports/account.py
+-rw-r--r--   0        0        0     7337 2024-04-27 14:40:52.098734 findmy-0.6.0/findmy/reports/anisette.py
+-rw-r--r--   0        0        0     9059 2024-04-27 14:40:52.098734 findmy-0.6.0/findmy/reports/reports.py
+-rw-r--r--   0        0        0      836 2024-04-27 14:40:52.098734 findmy-0.6.0/findmy/reports/state.py
+-rw-r--r--   0        0        0     7151 2024-04-27 14:40:52.098734 findmy-0.6.0/findmy/reports/twofactor.py
+-rw-r--r--   0        0        0      148 2024-04-27 14:40:52.098734 findmy-0.6.0/findmy/scanner/__init__.py
+-rw-r--r--   0        0        0     7217 2024-04-27 14:40:52.098734 findmy-0.6.0/findmy/scanner/scanner.py
+-rw-r--r--   0        0        0      201 2024-04-27 14:40:52.098734 findmy-0.6.0/findmy/util/__init__.py
+-rw-r--r--   0        0        0     1043 2024-04-27 14:40:52.098734 findmy-0.6.0/findmy/util/closable.py
+-rw-r--r--   0        0        0     2417 2024-04-27 14:40:52.098734 findmy-0.6.0/findmy/util/crypto.py
+-rw-r--r--   0        0        0     3603 2024-04-27 14:40:52.098734 findmy-0.6.0/findmy/util/http.py
+-rw-r--r--   0        0        0      500 2024-04-27 14:40:52.098734 findmy-0.6.0/findmy/util/parsers.py
+-rw-r--r--   0        0        0      120 2024-04-27 14:40:52.098734 findmy-0.6.0/findmy/util/types.py
+-rw-r--r--   0        0        0     1350 2024-04-27 14:40:52.102734 findmy-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4411 1970-01-01 00:00:00.000000 findmy-0.6.0/PKG-INFO
```

### Comparing `findmy-0.5.0/LICENSE.md` & `findmy-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `findmy-0.5.0/README.md` & `findmy-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,39 +20,39 @@
 > 
 > You are encouraged to report any issues you can find on the
 > [issue tracker](https://github.com/malmeloo/FindMy.py/)!
 
 ### Features
 
 - [x] Cross-platform: no Mac needed
-- [x] Fetch location reports
-  - [x] Apple acount sign-in
+- [x] Fetch and decrypt location reports
+  - [x] Official accessories (AirTags, iDevices, etc.)
+  - [x] Custom AirTags (OpenHaystack) 
+- [x] Apple account sign-in
   - [x] SMS 2FA support
+  - [x] Trusted Device 2FA support
 - [x] Scan for nearby FindMy-devices
   - [x] Decode their info, such as public keys and status bytes
 - [x] Import or create your own accessory keys
 - [x] Both async and sync APIs
 
 ### Roadmap
 
-- [ ] Trusted device 2FA
-    - Work has been done, but needs testing (I don't own any Apple devices)
 - [ ] Local anisette generation (without server)
-    - Can be done using [pyprovision](https://github.com/Dadoum/pyprovision/),
-      however I want to wait until Python wheels are available.
+    - More information: [#2](https://github.com/malmeloo/FindMy.py/issues/2)
 
 ## Installation
 
 The package can be installed from [PyPi](https://pypi.org/project/findmy/):
 
 ```shell
 pip install findmy
 ```
 
-For usage examples, see the [examples](examples) directory. Documentation coming soon™.
+For usage examples, see the [examples](examples) directory. Documentation can be found [here](http://docs.mikealmel.ooo/FindMy.py/).
 
 ## Contributing
 
 Want to contribute code? That's great! For new features, please open an
 [issue](https://github.com/malmeloo/FindMy.py/issues) first so we can discuss.
 
 This project uses [Ruff](https://docs.astral.sh/ruff/) for linting and formatting.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `findmy-0.5.0/findmy/accessory.py` & `findmy-0.6.0/findmy/accessory.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,26 +2,70 @@
 Module to interact with accessories that implement Find My.
 
 Accessories could be anything ranging from AirTags to iPhones.
 """
 from __future__ import annotations
 
 import logging
-from datetime import datetime, timedelta
-from typing import Generator, overload
+import plistlib
+from abc import ABC, abstractmethod
+from datetime import datetime, timedelta, timezone
+from typing import IO, Generator, overload
 
 from typing_extensions import override
 
 from .keys import KeyGenerator, KeyPair, KeyType
 from .util import crypto
 
 logging.getLogger(__name__)
 
 
-class FindMyAccessory:
+class RollingKeyPairSource(ABC):
+    """A class that generates rolling `KeyPair`s."""
+
+    @property
+    @abstractmethod
+    def interval(self) -> timedelta:
+        """KeyPair rollover interval."""
+
+    @abstractmethod
+    def keys_at(self, ind: int | datetime) -> set[KeyPair]:
+        """Generate potential key(s) occurring at a certain index or timestamp."""
+        raise NotImplementedError
+
+    @overload
+    def keys_between(self, start: int, end: int) -> set[KeyPair]:
+        pass
+
+    @overload
+    def keys_between(self, start: datetime, end: datetime) -> set[KeyPair]:
+        pass
+
+    def keys_between(self, start: int | datetime, end: int | datetime) -> set[KeyPair]:
+        """Generate potential key(s) occurring between two indices or timestamps."""
+        keys: set[KeyPair] = set()
+
+        if isinstance(start, int) and isinstance(end, int):
+            while start < end:
+                keys.update(self.keys_at(start))
+
+                start += 1
+        elif isinstance(start, datetime) and isinstance(end, datetime):
+            while start < end:
+                keys.update(self.keys_at(start))
+
+                start += self.interval
+        else:
+            msg = "Invalid start/end type"
+            raise TypeError(msg)
+
+        return keys
+
+
+class FindMyAccessory(RollingKeyPairSource):
     """A findable Find My-accessory using official key rollover."""
 
     def __init__(  # noqa: PLR0913
         self,
         master_key: bytes,
         skn: bytes,
         sks: bytes,
@@ -43,16 +87,28 @@
             logging.warning(
                 "Pairing datetime is timezone-naive. Assuming system tz: %s.",
                 self._paired_at.tzname(),
             )
 
         self._name = name
 
+    @property
+    @override
+    def interval(self) -> timedelta:
+        """Official FindMy accessory rollover interval (15 minutes)."""
+        return timedelta(minutes=15)
+
+    @override
     def keys_at(self, ind: int | datetime) -> set[KeyPair]:
         """Get the potential primary and secondary keys active at a certain time or index."""
+        if isinstance(ind, datetime) and ind < self._paired_at:
+            return set()
+        if isinstance(ind, int) and ind < 0:
+            return set()
+
         secondary_offset = 0
 
         if isinstance(ind, datetime):
             # number of 15-minute slots since pairing time
             ind = (
                 int(
                     (ind - self._paired_at).total_seconds() / (15 * 60),
@@ -84,14 +140,38 @@
 
         if ind > secondary_offset:
             # after the first 4 am after pairing, we need to account for the first day
             possible_keys.add(self._secondary_gen[(ind - secondary_offset) // 96 + 2])
 
         return possible_keys
 
+    @classmethod
+    def from_plist(cls, plist: IO[bytes]) -> FindMyAccessory:
+        """Create a FindMyAccessory from a .plist file dumped from the FindMy app."""
+        device_data = plistlib.load(plist)
+
+        # PRIVATE master key. 28 (?) bytes.
+        master_key = device_data["privateKey"]["key"]["data"][-28:]
+
+        # "Primary" shared secret. 32 bytes.
+        skn = device_data["sharedSecret"]["key"]["data"]
+
+        # "Secondary" shared secret. 32 bytes.
+        if "secondarySharedSecret" in device_data:
+            # AirTag
+            sks = device_data["secondarySharedSecret"]["key"]["data"]
+        else:
+            # iDevice
+            sks = device_data["secureLocationsSharedSecret"]["key"]["data"]
+
+        # "Paired at" timestamp (UTC)
+        paired_at = device_data["pairingDate"].replace(tzinfo=timezone.utc)
+
+        return cls(master_key, skn, sks, paired_at)
+
 
 class AccessoryKeyGenerator(KeyGenerator[KeyPair]):
     """KeyPair generator. Uses the same algorithm internally as FindMy accessories do."""
 
     def __init__(
         self,
         master_key: bytes,
```

### Comparing `findmy-0.5.0/findmy/errors.py` & `findmy-0.6.0/findmy/errors.py`

 * *Files identical despite different names*

### Comparing `findmy-0.5.0/findmy/keys.py` & `findmy-0.6.0/findmy/keys.py`

 * *Files identical despite different names*

### Comparing `findmy-0.5.0/findmy/reports/account.py` & `findmy-0.6.0/findmy/reports/account.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """Module containing most of the code necessary to interact with an Apple account."""
 from __future__ import annotations
 
 import asyncio
 import base64
-import hashlib
-import hmac
 import json
 import logging
 import plistlib
 import uuid
 from abc import ABC, abstractmethod
 from datetime import datetime, timedelta, timezone
 from functools import wraps
@@ -18,24 +16,23 @@
     Callable,
     Concatenate,
     ParamSpec,
     Sequence,
     TypedDict,
     TypeVar,
     cast,
+    overload,
 )
 
 import bs4
 import srp._pysrp as srp
-from cryptography.hazmat.primitives import hashes, padding
-from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
-from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 from typing_extensions import override
 
 from findmy.errors import InvalidCredentialsError, InvalidStateError, UnhandledProtocolError
+from findmy.util import crypto
 from findmy.util.closable import Closable
 from findmy.util.http import HttpSession, decode_plist
 
 from .reports import LocationReport, LocationReportsFetcher
 from .state import LoginState
 from .twofactor import (
     AsyncSecondFactorMethod,
@@ -44,14 +41,15 @@
     BaseSecondFactorMethod,
     SyncSecondFactorMethod,
     SyncSmsSecondFactor,
     SyncTrustedDeviceSecondFactor,
 )
 
 if TYPE_CHECKING:
+    from findmy.accessory import RollingKeyPairSource
     from findmy.keys import KeyPair
     from findmy.util.types import MaybeCoro
 
     from .anisette import BaseAnisetteProvider
 
 logging.getLogger(__name__)
 
@@ -92,40 +90,14 @@
             return func(acc, *args, **kwargs)
 
         return wrapper
 
     return decorator
 
 
-def _encrypt_password(password: str, salt: bytes, iterations: int) -> bytes:
-    p = hashlib.sha256(password.encode("utf-8")).digest()
-    kdf = PBKDF2HMAC(
-        algorithm=hashes.SHA256(),
-        length=32,
-        salt=salt,
-        iterations=iterations,
-    )
-    return kdf.derive(p)
-
-
-def _decrypt_cbc(session_key: bytes, data: bytes) -> bytes:
-    extra_data_key = hmac.new(session_key, b"extra data key:", hashlib.sha256).digest()
-    extra_data_iv = hmac.new(session_key, b"extra data iv:", hashlib.sha256).digest()
-    # Get only the first 16 bytes of the iv
-    extra_data_iv = extra_data_iv[:16]
-
-    # Decrypt with AES CBC
-    cipher = Cipher(algorithms.AES(extra_data_key), modes.CBC(extra_data_iv))
-    decryptor = cipher.decryptor()
-    data = decryptor.update(data) + decryptor.finalize()
-    # Remove PKCS#7 padding
-    padder = padding.PKCS7(128).unpadder()
-    return padder.update(data) + padder.finalize()
-
-
 def _extract_phone_numbers(html: str) -> list[dict]:
     soup = bs4.BeautifulSoup(html, features="html.parser")
     data_elem = soup.find("script", {"class": "boot_args"})
     if not data_elem:
         msg = "Could not find HTML element containing phone numbers"
         raise RuntimeError(msg)
 
@@ -241,54 +213,129 @@
         """
         Submit a 2FA code that was sent to a trusted device.
 
         Consider using `BaseSecondFactorMethod.submit` instead.
         """
         raise NotImplementedError
 
+    @overload
+    @abstractmethod
+    def fetch_reports(
+        self,
+        keys: KeyPair,
+        date_from: datetime,
+        date_to: datetime | None,
+    ) -> MaybeCoro[list[LocationReport]]:
+        ...
+
+    @overload
     @abstractmethod
     def fetch_reports(
         self,
         keys: Sequence[KeyPair],
         date_from: datetime,
         date_to: datetime | None,
     ) -> MaybeCoro[dict[KeyPair, list[LocationReport]]]:
+        ...
+
+    @overload
+    @abstractmethod
+    def fetch_reports(
+        self,
+        keys: RollingKeyPairSource,
+        date_from: datetime,
+        date_to: datetime | None,
+    ) -> MaybeCoro[list[LocationReport]]:
+        ...
+
+    @abstractmethod
+    def fetch_reports(
+        self,
+        keys: KeyPair | Sequence[KeyPair] | RollingKeyPairSource,
+        date_from: datetime,
+        date_to: datetime | None,
+    ) -> MaybeCoro[list[LocationReport] | dict[KeyPair, list[LocationReport]]]:
         """
         Fetch location reports for a sequence of `KeyPair`s between `date_from` and `date_end`.
 
         Returns a dictionary mapping `KeyPair`s to a list of their location reports.
         """
         raise NotImplementedError
 
+    @overload
+    @abstractmethod
+    def fetch_last_reports(
+        self,
+        keys: KeyPair,
+        hours: int = 7 * 24,
+    ) -> MaybeCoro[list[LocationReport]]:
+        ...
+
+    @overload
     @abstractmethod
     def fetch_last_reports(
         self,
         keys: Sequence[KeyPair],
         hours: int = 7 * 24,
     ) -> MaybeCoro[dict[KeyPair, list[LocationReport]]]:
+        ...
+
+    @overload
+    @abstractmethod
+    def fetch_last_reports(
+        self,
+        keys: RollingKeyPairSource,
+        hours: int = 7 * 24,
+    ) -> MaybeCoro[list[LocationReport]]:
+        ...
+
+    @abstractmethod
+    def fetch_last_reports(
+        self,
+        keys: KeyPair | Sequence[KeyPair] | RollingKeyPairSource,
+        hours: int = 7 * 24,
+    ) -> MaybeCoro[list[LocationReport] | dict[KeyPair, list[LocationReport]]]:
         """
         Fetch location reports for a sequence of `KeyPair`s for the last `hours` hours.
 
         Utility method as an alternative to using `BaseAppleAccount.fetch_reports` directly.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def get_anisette_headers(self, serial: str = "0") -> MaybeCoro[dict[str, str]]:
+    def get_anisette_headers(
+        self,
+        with_client_info: bool = False,
+        serial: str = "0",
+    ) -> MaybeCoro[dict[str, str]]:
         """
         Retrieve a complete dictionary of Anisette headers.
 
         Utility method for `AnisetteProvider.get_headers` using this account's user and device ID.
         """
         raise NotImplementedError
 
 
 class AsyncAppleAccount(BaseAppleAccount):
     """An async implementation of `BaseAppleAccount`."""
 
+    # auth endpoints
+    _ENDPOINT_GSA = "https://gsa.apple.com/grandslam/GsService2"
+    _ENDPOINT_LOGIN_MOBILEME = "https://setup.icloud.com/setup/iosbuddy/loginDelegates"
+
+    # 2fa auth endpoints
+    _ENDPOINT_2FA_METHODS = "https://gsa.apple.com/auth"
+    _ENDPOINT_2FA_SMS_REQUEST = "https://gsa.apple.com/auth/verify/phone"
+    _ENDPOINT_2FA_SMS_SUBMIT = "https://gsa.apple.com/auth/verify/phone/securitycode"
+    _ENDPOINT_2FA_TD_REQUEST = "https://gsa.apple.com/auth/verify/trusteddevice"
+    _ENDPOINT_2FA_TD_SUBMIT = "https://gsa.apple.com/grandslam/GsService2/validate"
+
+    # reports endpoints
+    _ENDPOINT_REPORTS_FETCH = "https://gateway.icloud.com/acsnservice/fetch"
+
     def __init__(
         self,
         anisette: BaseAnisetteProvider,
         user_id: str | None = None,
         device_id: str | None = None,
     ) -> None:
         """
@@ -434,15 +481,15 @@
         if self._account_info is None:
             return []
 
         if self._account_info["trusted_device_2fa"]:
             methods.append(AsyncTrustedDeviceSecondFactor(self))
 
         # sms
-        auth_page = await self._sms_2fa_request("GET", "https://gsa.apple.com/auth")
+        auth_page = await self._sms_2fa_request("GET", self._ENDPOINT_2FA_METHODS)
         try:
             phone_numbers = _extract_phone_numbers(auth_page)
             methods.extend(
                 AsyncSmsSecondFactor(
                     self,
                     number.get("id") or -1,
                     number.get("numberWithDialCode") or "-",
@@ -458,15 +505,15 @@
     @override
     async def sms_2fa_request(self, phone_number_id: int) -> None:
         """See `BaseAppleAccount.sms_2fa_request`."""
         data = {"phoneNumber": {"id": phone_number_id}, "mode": "sms"}
 
         await self._sms_2fa_request(
             "PUT",
-            "https://gsa.apple.com/auth/verify/phone",
+            self._ENDPOINT_2FA_SMS_REQUEST,
             data,
         )
 
     @require_login_state(LoginState.REQUIRE_2FA)
     @override
     async def sms_2fa_submit(self, phone_number_id: int, code: str) -> LoginState:
         """See `BaseAppleAccount.sms_2fa_submit`."""
@@ -474,15 +521,15 @@
             "phoneNumber": {"id": phone_number_id},
             "securityCode": {"code": str(code)},
             "mode": "sms",
         }
 
         await self._sms_2fa_request(
             "POST",
-            "https://gsa.apple.com/auth/verify/phone/securitycode",
+            self._ENDPOINT_2FA_SMS_SUBMIT,
             data,
         )
 
         # REQUIRE_2FA -> AUTHENTICATED
         new_state = await self._gsa_authenticate()
         if new_state != LoginState.AUTHENTICATED:
             msg = f"Unexpected state after submitting 2FA: {new_state}"
@@ -497,30 +544,30 @@
         """See `BaseAppleAccount.td_2fa_request`."""
         headers = {
             "Content-Type": "text/x-xml-plist",
             "Accept": "text/x-xml-plist",
         }
         await self._sms_2fa_request(
             "GET",
-            "https://gsa.apple.com/auth/verify/trusteddevice",
+            self._ENDPOINT_2FA_TD_REQUEST,
             headers=headers,
         )
 
     @require_login_state(LoginState.REQUIRE_2FA)
     @override
     async def td_2fa_submit(self, code: str) -> LoginState:
         """See `BaseAppleAccount.td_2fa_submit`."""
         headers = {
             "security-code": code,
             "Content-Type": "text/x-xml-plist",
             "Accept": "text/x-xml-plist",
         }
         await self._sms_2fa_request(
             "GET",
-            "https://gsa.apple.com/grandslam/GsService2/validate",
+            self._ENDPOINT_2FA_TD_SUBMIT,
             headers=headers,
         )
 
         # REQUIRE_2FA -> AUTHENTICATED
         new_state = await self._gsa_authenticate()
         if new_state != LoginState.AUTHENTICATED:
             msg = f"Unexpected state after submitting 2FA: {new_state}"
@@ -533,51 +580,103 @@
     async def fetch_raw_reports(self, start: int, end: int, ids: list[str]) -> dict[str, Any]:
         """Make a request for location reports, returning raw data."""
         auth = (
             self._login_state_data["dsid"],
             self._login_state_data["mobileme_data"]["tokens"]["searchPartyToken"],
         )
         data = {"search": [{"startDate": start, "endDate": end, "ids": ids}]}
+
         r = await self._http.post(
-            "https://gateway.icloud.com/acsnservice/fetch",
+            self._ENDPOINT_REPORTS_FETCH,
             auth=auth,
             headers=await self.get_anisette_headers(),
             json=data,
         )
         resp = r.json()
         if not r.ok or resp["statusCode"] != "200":
             msg = f"Failed to fetch reports: {resp['statusCode']}"
             raise UnhandledProtocolError(msg)
 
         return resp
 
-    @require_login_state(LoginState.LOGGED_IN)
-    @override
+    @overload
+    async def fetch_reports(
+        self,
+        keys: KeyPair,
+        date_from: datetime,
+        date_to: datetime | None,
+    ) -> list[LocationReport]:
+        ...
+
+    @overload
     async def fetch_reports(
         self,
         keys: Sequence[KeyPair],
         date_from: datetime,
         date_to: datetime | None,
     ) -> dict[KeyPair, list[LocationReport]]:
+        ...
+
+    @overload
+    async def fetch_reports(
+        self,
+        keys: RollingKeyPairSource,
+        date_from: datetime,
+        date_to: datetime | None,
+    ) -> list[LocationReport]:
+        ...
+
+    @require_login_state(LoginState.LOGGED_IN)
+    @override
+    async def fetch_reports(
+        self,
+        keys: KeyPair | Sequence[KeyPair] | RollingKeyPairSource,
+        date_from: datetime,
+        date_to: datetime | None,
+    ) -> list[LocationReport] | dict[KeyPair, list[LocationReport]]:
         """See `BaseAppleAccount.fetch_reports`."""
         date_to = date_to or datetime.now().astimezone()
 
         return await self._reports.fetch_reports(
             date_from,
             date_to,
             keys,
         )
 
-    @require_login_state(LoginState.LOGGED_IN)
-    @override
+    @overload
+    async def fetch_last_reports(
+        self,
+        keys: KeyPair,
+        hours: int = 7 * 24,
+    ) -> list[LocationReport]:
+        ...
+
+    @overload
     async def fetch_last_reports(
         self,
         keys: Sequence[KeyPair],
         hours: int = 7 * 24,
     ) -> dict[KeyPair, list[LocationReport]]:
+        ...
+
+    @overload
+    async def fetch_last_reports(
+        self,
+        keys: RollingKeyPairSource,
+        hours: int = 7 * 24,
+    ) -> list[LocationReport]:
+        ...
+
+    @require_login_state(LoginState.LOGGED_IN)
+    @override
+    async def fetch_last_reports(
+        self,
+        keys: KeyPair | Sequence[KeyPair] | RollingKeyPairSource,
+        hours: int = 7 * 24,
+    ) -> list[LocationReport] | dict[KeyPair, list[LocationReport]]:
         """See `BaseAppleAccount.fetch_last_reports`."""
         end = datetime.now(tz=timezone.utc)
         start = end - timedelta(hours=hours)
 
         return await self.fetch_reports(keys, start, end)
 
     @require_login_state(LoginState.LOGGED_OUT, LoginState.REQUIRE_2FA)
@@ -612,15 +711,15 @@
         sp = r.get("sp")
         if sp != "s2k":
             msg = f"This implementation only supports s2k. Server returned {sp}"
             raise UnhandledProtocolError(msg)
 
         logging.debug("Attempting password challenge")
 
-        usr.p = _encrypt_password(self._password, r["s"], r["i"])
+        usr.p = crypto.encrypt_password(self._password, r["s"], r["i"])
         m1 = usr.process_challenge(r["s"], r["B"])
         if m1 is None:
             msg = "Failed to process challenge"
             raise UnhandledProtocolError(msg)
         r = await self._gsa_request(
             {"c": r["c"], "M1": m1, "u": self._username, "o": "complete"},
         )
@@ -633,16 +732,20 @@
         usr.verify_session(r.get("M2"))
         if not usr.authenticated():
             msg = "Failed to verify session"
             raise UnhandledProtocolError(msg)
 
         logging.debug("Decrypting SPD data in response")
 
-        spd = _decrypt_cbc(usr.get_session_key() or b"", r["spd"])
-        spd = decode_plist(spd)
+        spd = decode_plist(
+            crypto.decrypt_spd_aes_cbc(
+                usr.get_session_key() or b"",
+                r["spd"],
+            ),
+        )
 
         logging.debug("Received account information")
         self._account_info = cast(
             _AccountInfo,
             {
                 "account_name": spd.get("acname"),
                 "first_name": spd.get("fn"),
@@ -651,35 +754,31 @@
             },
         )
 
         au = r["Status"].get("au")
         if au in ("secondaryAuth", "trustedDeviceSecondaryAuth"):
             logging.info("Detected 2FA requirement: %s", au)
 
-            self._account_info.update(
-                {
-                    "trusted_device_2fa": au == "trustedDeviceSecondaryAuth",
-                },
-            )
+            self._account_info["trusted_device_2fa"] = au == "trustedDeviceSecondaryAuth"
 
             return self._set_login_state(
                 LoginState.REQUIRE_2FA,
                 {"adsid": spd["adsid"], "idms_token": spd["GsIdmsToken"]},
             )
-        if au is not None:
-            msg = f"Unknown auth value: {au}"
-            raise UnhandledProtocolError(msg)
+        if au is None:
+            logging.info("GSA authentication successful")
 
-        logging.info("GSA authentication successful")
+            idms_pet = spd.get("t", {}).get("com.apple.gs.idms.pet", {}).get("token", "")
+            return self._set_login_state(
+                LoginState.AUTHENTICATED,
+                {"idms_pet": idms_pet, "adsid": spd["adsid"]},
+            )
 
-        idms_pet = spd.get("t", {}).get("com.apple.gs.idms.pet", {}).get("token", "")
-        return self._set_login_state(
-            LoginState.AUTHENTICATED,
-            {"idms_pet": idms_pet, "adsid": spd["adsid"]},
-        )
+        msg = f"Unknown auth value: {au}"
+        raise UnhandledProtocolError(msg)
 
     @require_login_state(LoginState.AUTHENTICATED)
     async def _login_mobileme(self) -> LoginState:
         logging.info("Logging into com.apple.mobileme")
         data = plistlib.dumps(
             {
                 "apple-id": self._username,
@@ -694,15 +793,15 @@
             "User-Agent": "com.apple.iCloudHelper/282 CFNetwork/1408.0.4 Darwin/22.5.0",
             "X-Mme-Client-Info": "<MacBookPro18,3> <Mac OS X;13.4.1;22F8>"
             " <com.apple.AOSKit/282 (com.apple.accountsd/113)>",
         }
         headers.update(await self.get_anisette_headers())
 
         resp = await self._http.post(
-            "https://setup.icloud.com/setup/iosbuddy/loginDelegates",
+            self._ENDPOINT_LOGIN_MOBILEME,
             auth=(self._username or "", self._login_state_data["idms_pet"]),
             data=data,
             headers=headers,
         )
         data = resp.plist()
 
         mobileme_data = data.get("delegates", {}).get("com.apple.mobileme", {})
@@ -730,74 +829,69 @@
 
         headers = headers or {}
         headers.update(
             {
                 "User-Agent": "Xcode",
                 "Accept-Language": "en-us",
                 "X-Apple-Identity-Token": identity_token,
-                "X-Apple-App-Info": "com.apple.gs.xcode.auth",
-                "X-Xcode-Version": "11.2 (11B41)",
-                "X-Mme-Client-Info": "<MacBookPro18,3> <Mac OS X;13.4.1;22F8>"
-                " <com.apple.AOSKit/282 (com.apple.dt.Xcode/3594.4.19)>",
             },
         )
-        headers.update(await self.get_anisette_headers())
+        headers.update(await self.get_anisette_headers(with_client_info=True))
 
         r = await self._http.request(
             method,
             url,
             json=data,
             headers=headers,
         )
         if not r.ok:
             msg = f"SMS 2FA request failed: {r.status_code}"
             raise UnhandledProtocolError(msg)
 
         return r.text()
 
-    async def _gsa_request(self, params: dict[str, Any]) -> dict[Any, Any]:
-        request_data = {
-            "cpd": {
-                "bootstrap": True,
-                "icscrec": True,
-                "pbe": False,
-                "prkgen": True,
-                "svct": "iCloud",
-            },
-        }
-        request_data["cpd"].update(await self.get_anisette_headers())
-        request_data.update(params)
-
+    async def _gsa_request(self, parameters: dict[str, Any]) -> dict[str, Any]:
         body = {
-            "Header": {"Version": "1.0.1"},
-            "Request": request_data,
+            "Header": {
+                "Version": "1.0.1",
+            },
+            "Request": {
+                "cpd": await self._anisette.get_cpd(
+                    self._uid,
+                    self._devid,
+                ),
+                **parameters,
+            },
         }
 
         headers = {
             "Content-Type": "text/x-xml-plist",
             "Accept": "*/*",
             "User-Agent": "akd/1.0 CFNetwork/978.0.7 Darwin/18.7.0",
-            "X-MMe-Client-Info": "<MacBookPro18,3> <Mac OS X;13.4.1;22F8> "
-            "<com.apple.AOSKit/282 (com.apple.dt.Xcode/3594.4.19)>",
+            "X-MMe-Client-Info": self._anisette.client,
         }
 
         resp = await self._http.post(
-            "https://gsa.apple.com/grandslam/GsService2",
+            self._ENDPOINT_GSA,
             headers=headers,
             data=plistlib.dumps(body),
         )
         if not resp.ok:
             msg = f"Error response for GSA request: {resp.status_code}"
             raise UnhandledProtocolError(msg)
         return resp.plist()["Response"]
 
     @override
-    async def get_anisette_headers(self, serial: str = "0") -> dict[str, str]:
+    async def get_anisette_headers(
+        self,
+        with_client_info: bool = False,
+        serial: str = "0",
+    ) -> dict[str, str]:
         """See `BaseAppleAccount.get_anisette_headers`."""
-        return await self._anisette.get_headers(self._uid, self._devid, serial)
+        return await self._anisette.get_headers(self._uid, self._devid, serial, with_client_info)
 
 
 class AppleAccount(BaseAppleAccount):
     """
     A sync implementation of `BaseappleAccount`.
 
     Uses `AsyncappleAccount` internally.
@@ -906,33 +1000,88 @@
 
     @override
     def td_2fa_submit(self, code: str) -> LoginState:
         """See `AsyncAppleAccount.td_2fa_submit`."""
         coro = self._asyncacc.td_2fa_submit(code)
         return self._evt_loop.run_until_complete(coro)
 
-    @override
+    @overload
+    def fetch_reports(
+        self,
+        keys: KeyPair,
+        date_from: datetime,
+        date_to: datetime | None,
+    ) -> list[LocationReport]:
+        ...
+
+    @overload
     def fetch_reports(
         self,
         keys: Sequence[KeyPair],
         date_from: datetime,
         date_to: datetime | None,
     ) -> dict[KeyPair, list[LocationReport]]:
+        ...
+
+    @overload
+    def fetch_reports(
+        self,
+        keys: RollingKeyPairSource,
+        date_from: datetime,
+        date_to: datetime | None,
+    ) -> list[LocationReport]:
+        ...
+
+    @override
+    def fetch_reports(
+        self,
+        keys: KeyPair | Sequence[KeyPair] | RollingKeyPairSource,
+        date_from: datetime,
+        date_to: datetime | None,
+    ) -> list[LocationReport] | dict[KeyPair, list[LocationReport]]:
         """See `AsyncAppleAccount.fetch_reports`."""
         coro = self._asyncacc.fetch_reports(keys, date_from, date_to)
         return self._evt_loop.run_until_complete(coro)
 
-    @override
+    @overload
+    def fetch_last_reports(
+        self,
+        keys: KeyPair,
+        hours: int = 7 * 24,
+    ) -> list[LocationReport]:
+        ...
+
+    @overload
     def fetch_last_reports(
         self,
         keys: Sequence[KeyPair],
         hours: int = 7 * 24,
     ) -> dict[KeyPair, list[LocationReport]]:
+        ...
+
+    @overload
+    def fetch_last_reports(
+        self,
+        keys: RollingKeyPairSource,
+        hours: int = 7 * 24,
+    ) -> list[LocationReport]:
+        ...
+
+    @override
+    def fetch_last_reports(
+        self,
+        keys: KeyPair | Sequence[KeyPair] | RollingKeyPairSource,
+        hours: int = 7 * 24,
+    ) -> list[LocationReport] | dict[KeyPair, list[LocationReport]]:
         """See `AsyncAppleAccount.fetch_last_reports`."""
         coro = self._asyncacc.fetch_last_reports(keys, hours)
         return self._evt_loop.run_until_complete(coro)
 
     @override
-    def get_anisette_headers(self, serial: str = "0") -> dict[str, str]:
+    def get_anisette_headers(
+        self,
+        with_client_info: bool = False,
+        serial: str = "0",
+    ) -> dict[str, str]:
         """See `AsyncAppleAccount.get_anisette_headers`."""
-        coro = self._asyncacc.get_anisette_headers(serial)
+        coro = self._asyncacc.get_anisette_headers(with_client_info, serial)
         return self._evt_loop.run_until_complete(coro)
```

### Comparing `findmy-0.5.0/findmy/reports/reports.py` & `findmy-0.6.0/findmy/reports/reports.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 """Module providing functionality to look up location reports."""
 from __future__ import annotations
 
 import base64
 import hashlib
+import logging
 import struct
-from datetime import datetime, timezone
-from typing import TYPE_CHECKING, Sequence, TypedDict, overload
+from datetime import datetime, timedelta, timezone
+from typing import TYPE_CHECKING, Sequence, overload
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
-from typing_extensions import Unpack, override
+from typing_extensions import override
 
+from findmy.accessory import RollingKeyPairSource
 from findmy.keys import KeyPair
-from findmy.util.http import HttpSession
 
 if TYPE_CHECKING:
     from .account import AsyncAppleAccount
 
-_session = HttpSession()
-
-
-class _FetcherConfig(TypedDict):
-    user_id: str
-    device_id: str
-    dsid: str
-    search_party_token: str
+logging.getLogger(__name__)
 
 
 def _decrypt_payload(payload: bytes, key: KeyPair) -> bytes:
     eph_key = ec.EllipticCurvePublicKey.from_encoded_point(
         ec.SECP224R1(),
         payload[5:62],
     )
@@ -127,15 +121,15 @@
     ) -> LocationReport:
         """
         Create a `KeyReport` from fields and a payload as reported by Apple.
 
         Requires a `KeyPair` to decrypt the report's payload.
         """
         timestamp_int = int.from_bytes(payload[0:4], "big") + (60 * 60 * 24 * 11323)
-        timestamp = datetime.fromtimestamp(timestamp_int, tz=timezone.utc)
+        timestamp = datetime.fromtimestamp(timestamp_int, tz=timezone.utc).astimezone()
 
         data = _decrypt_payload(payload, key)
         latitude = struct.unpack(">i", data[0:4])[0] / 10000000
         longitude = struct.unpack(">i", data[4:8])[0] / 10000000
         confidence = int.from_bytes(data[8:9], "big")
         status = int.from_bytes(data[9:10], "big")
 
@@ -177,22 +171,14 @@
         """
         Initialize the fetcher.
 
         :param account: Apple account.
         """
         self._account: AsyncAppleAccount = account
 
-        self._http: HttpSession = HttpSession()
-
-        self._config: _FetcherConfig | None = None
-
-    def apply_config(self, **conf: Unpack[_FetcherConfig]) -> None:
-        """Configure internal variables necessary to make reports fetching calls."""
-        self._config = conf
-
     @overload
     async def fetch_reports(
         self,
         date_from: datetime,
         date_to: datetime,
         device: KeyPair,
     ) -> list[LocationReport]:
@@ -203,57 +189,100 @@
         self,
         date_from: datetime,
         date_to: datetime,
         device: Sequence[KeyPair],
     ) -> dict[KeyPair, list[LocationReport]]:
         ...
 
+    @overload
     async def fetch_reports(
         self,
         date_from: datetime,
         date_to: datetime,
-        device: KeyPair | Sequence[KeyPair],
+        device: RollingKeyPairSource,
+    ) -> list[LocationReport]:
+        ...
+
+    async def fetch_reports(
+        self,
+        date_from: datetime,
+        date_to: datetime,
+        device: KeyPair | Sequence[KeyPair] | RollingKeyPairSource,
     ) -> list[LocationReport] | dict[KeyPair, list[LocationReport]]:
         """
         Fetch location reports for a certain device.
 
         When ``device`` is a single :class:`.KeyPair`, this method will return
         a list of location reports corresponding to that pair.
         When ``device`` is a sequence of :class:`.KeyPair`s, it will return a dictionary
         with the :class:`.KeyPair` as key, and a list of location reports as value.
         """
         # single KeyPair
         if isinstance(device, KeyPair):
             return await self._fetch_reports(date_from, date_to, [device])
 
-        # sequence of KeyPairs
-        reports = await self._fetch_reports(date_from, date_to, device)
-        res: dict[KeyPair, list[LocationReport]] = {key: [] for key in device}
+        # KeyPair generator
+        #   add 12h margin to the generator
+        if isinstance(device, RollingKeyPairSource):
+            keys = list(
+                device.keys_between(
+                    date_from - timedelta(hours=12),
+                    date_to + timedelta(hours=12),
+                ),
+            )
+        else:
+            keys = device
+
+        # sequence of KeyPairs (fetch 256 max at a time)
+        reports: list[LocationReport] = []
+        for key_offset in range(0, len(keys), 256):
+            chunk = keys[key_offset : key_offset + 256]
+            reports.extend(await self._fetch_reports(date_from, date_to, chunk))
+
+        if isinstance(device, RollingKeyPairSource):
+            return reports
+
+        res: dict[KeyPair, list[LocationReport]] = {key: [] for key in keys}
         for report in reports:
             res[report.key].append(report)
         return res
 
     async def _fetch_reports(
         self,
         date_from: datetime,
         date_to: datetime,
         keys: Sequence[KeyPair],
     ) -> list[LocationReport]:
+        logging.debug("Fetching reports for %s keys", len(keys))
+
         start_date = int(date_from.timestamp() * 1000)
         end_date = int(date_to.timestamp() * 1000)
         ids = [key.hashed_adv_key_b64 for key in keys]
         data = await self._account.fetch_raw_reports(start_date, end_date, ids)
 
         id_to_key: dict[str, KeyPair] = {key.hashed_adv_key_b64: key for key in keys}
         reports: list[LocationReport] = []
         for report in data.get("results", []):
             key = id_to_key[report["id"]]
             date_published = datetime.fromtimestamp(
                 report.get("datePublished", 0) / 1000,
                 tz=timezone.utc,
-            )
+            ).astimezone()
             description = report.get("description", "")
             payload = base64.b64decode(report["payload"])
 
-            reports.append(LocationReport.from_payload(key, date_published, description, payload))
+            try:
+                loc_report = LocationReport.from_payload(key, date_published, description, payload)
+            except ValueError as e:
+                logging.warning(
+                    "Location report was not decodable. Some payloads have unknown"
+                    " variations leading to this error. Please report this full message"
+                    " at https://github.com/malmeloo/FindMy.py/issues/27. "
+                    "Payload: %s, Original error: %s",
+                    payload.hex(),
+                    e,
+                )
+                continue
+
+            reports.append(loc_report)
 
         return reports
```

### Comparing `findmy-0.5.0/findmy/reports/state.py` & `findmy-0.6.0/findmy/reports/state.py`

 * *Files identical despite different names*

### Comparing `findmy-0.5.0/findmy/reports/twofactor.py` & `findmy-0.6.0/findmy/reports/twofactor.py`

 * *Files identical despite different names*

### Comparing `findmy-0.5.0/findmy/scanner/scanner.py` & `findmy-0.6.0/findmy/scanner/scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     def __init__(self, loop: asyncio.AbstractEventLoop) -> None:
         """
         Initialize an instance of the Scanner using an event loop.
 
         You most likely do not want to use this yourself;
         check out `OfflineFindingScanner.create` instead.
         """
-        self._scanner: BleakScanner = BleakScanner(self._scan_callback, cb=dict(use_bdaddr=True))
+        self._scanner: BleakScanner = BleakScanner(self._scan_callback, cb={"use_bdaddr": True})
 
         self._loop = loop
         self._device_fut: asyncio.Future[tuple[BLEDevice, AdvertisementData]] = loop.create_future()
 
         self._scanner_count: int = 0
 
     @classmethod
@@ -169,15 +169,20 @@
     async def _wait_for_device(self, timeout: float) -> OfflineFindingDevice | None:
         device, data = await asyncio.wait_for(self._device_fut, timeout=timeout)
 
         apple_data = data.manufacturer_data.get(self.BLE_COMPANY_APPLE, b"")
         if not apple_data:
             return None
 
-        additional_data = device.details.get("props", {})
+        try:
+            additional_data = device.details.get("props", {})
+        except AttributeError:
+            # Likely Windows host, where details is a '_RawAdvData' object.
+            # See: https://github.com/malmeloo/FindMy.py/issues/24
+            additional_data = {}
         return OfflineFindingDevice.from_payload(device.address, apple_data, additional_data)
 
     async def scan_for(
         self,
         timeout: float = 10,
         *,
         extend_timeout: bool = False,
```

### Comparing `findmy-0.5.0/findmy/util/closable.py` & `findmy-0.6.0/findmy/util/closable.py`

 * *Files identical despite different names*

### Comparing `findmy-0.5.0/findmy/util/http.py` & `findmy-0.6.0/findmy/util/http.py`

 * *Files identical despite different names*

### Comparing `findmy-0.5.0/pyproject.toml` & `findmy-0.6.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "FindMy"
-version = "0.5.0"
+version = "v0.6.0"
 description = "Everything you need to work with Apple's Find My network!"
 authors = ["Mike Almeloo <git@mikealmel.ooo>"]
 readme = "README.md"
 packages = [{ include = "findmy" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
@@ -45,14 +45,15 @@
     "FIX002", # resolving TODOs
 
     "D203", # one blank line before class docstring
     "D212", # multi-line docstring start at first line
     "D105", # docstrings in magic methods
 
     "PLR2004", # "magic" values >.>
+    "FBT",     # boolean "traps"
 ]
 
 line-length = 100
 
 [tool.ruff.lint.per-file-ignores]
 "examples/*" = [
     "T201",  # use of "print"
```

### Comparing `findmy-0.5.0/PKG-INFO` & `findmy-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindMy
-Version: 0.5.0
+Version: 0.6.0
 Summary: Everything you need to work with Apple's Find My network!
 Author: Mike Almeloo
 Author-email: git@mikealmel.ooo
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -40,39 +40,39 @@
 > 
 > You are encouraged to report any issues you can find on the
 > [issue tracker](https://github.com/malmeloo/FindMy.py/)!
 
 ### Features
 
 - [x] Cross-platform: no Mac needed
-- [x] Fetch location reports
-  - [x] Apple acount sign-in
+- [x] Fetch and decrypt location reports
+  - [x] Official accessories (AirTags, iDevices, etc.)
+  - [x] Custom AirTags (OpenHaystack) 
+- [x] Apple account sign-in
   - [x] SMS 2FA support
+  - [x] Trusted Device 2FA support
 - [x] Scan for nearby FindMy-devices
   - [x] Decode their info, such as public keys and status bytes
 - [x] Import or create your own accessory keys
 - [x] Both async and sync APIs
 
 ### Roadmap
 
-- [ ] Trusted device 2FA
-    - Work has been done, but needs testing (I don't own any Apple devices)
 - [ ] Local anisette generation (without server)
-    - Can be done using [pyprovision](https://github.com/Dadoum/pyprovision/),
-      however I want to wait until Python wheels are available.
+    - More information: [#2](https://github.com/malmeloo/FindMy.py/issues/2)
 
 ## Installation
 
 The package can be installed from [PyPi](https://pypi.org/project/findmy/):
 
 ```shell
 pip install findmy
 ```
 
-For usage examples, see the [examples](examples) directory. Documentation coming soon™.
+For usage examples, see the [examples](examples) directory. Documentation can be found [here](http://docs.mikealmel.ooo/FindMy.py/).
 
 ## Contributing
 
 Want to contribute code? That's great! For new features, please open an
 [issue](https://github.com/malmeloo/FindMy.py/issues) first so we can discuss.
 
 This project uses [Ruff](https://docs.astral.sh/ruff/) for linting and formatting.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

