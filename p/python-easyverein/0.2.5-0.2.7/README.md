# Comparing `tmp/python_easyverein-0.2.5.tar.gz` & `tmp/python_easyverein-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_easyverein-0.2.5.tar", max compression
+gzip compressed data, was "python_easyverein-0.2.7.tar", max compression
```

## Comparing `python_easyverein-0.2.5.tar` & `python_easyverein-0.2.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1063 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/LICENSE
--rw-r--r--   0        0        0     5062 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/README.md
--rw-r--r--   0        0        0      338 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/__init__.py
--rw-r--r--   0        0        0     1338 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/api.py
--rw-r--r--   0        0        0        0 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/core/__init__.py
--rw-r--r--   0        0        0    11386 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/core/client.py
--rw-r--r--   0        0        0      747 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/core/exceptions.py
--rw-r--r--   0        0        0      533 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/core/protocol.py
--rw-r--r--   0        0        0     1094 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/core/types.py
--rw-r--r--   0        0        0      144 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/core/validators.py
--rw-r--r--   0        0        0      835 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/models/__init__.py
--rw-r--r--   0        0        0      720 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/models/base.py
--rw-r--r--   0        0        0     6390 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/models/contact_details.py
--rw-r--r--   0        0        0     3574 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/models/custom_field.py
--rw-r--r--   0        0        0     4442 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/models/invoice.py
--rw-r--r--   0        0        0     2608 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/models/invoice_item.py
--rw-r--r--   0        0        0     7938 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/models/member.py
--rw-r--r--   0        0        0     2587 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/models/member_custom_field.py
--rw-r--r--   0        0        0        0 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/models/mixins/__init__.py
--rw-r--r--   0        0        0      621 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/models/mixins/empty_strings_mixin.py
--rw-r--r--   0        0        0     1477 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/models/mixins/required_attributes.py
--rw-r--r--   0        0        0        0 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/modules/__init__.py
--rw-r--r--   0        0        0      723 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/modules/contact_details.py
--rw-r--r--   0        0        0      696 2024-01-21 19:46:16.180409 python_easyverein-0.2.5/easyverein/modules/custom_field.py
--rw-r--r--   0        0        0     6990 2024-01-21 19:46:16.184409 python_easyverein-0.2.5/easyverein/modules/invoice.py
--rw-r--r--   0        0        0      581 2024-01-21 19:46:16.184409 python_easyverein-0.2.5/easyverein/modules/invoice_item.py
--rw-r--r--   0        0        0      571 2024-01-21 19:46:16.184409 python_easyverein-0.2.5/easyverein/modules/member.py
--rw-r--r--   0        0        0     4106 2024-01-21 19:46:16.184409 python_easyverein-0.2.5/easyverein/modules/member_custom_field.py
--rw-r--r--   0        0        0        0 2024-01-21 19:46:16.184409 python_easyverein-0.2.5/easyverein/modules/mixins/__init__.py
--rw-r--r--   0        0        0     7117 2024-01-21 19:46:16.184409 python_easyverein-0.2.5/easyverein/modules/mixins/crud.py
--rw-r--r--   0        0        0     1707 2024-01-21 19:46:16.184409 python_easyverein-0.2.5/easyverein/modules/mixins/recycle_bin.py
--rw-r--r--   0        0        0     1212 2024-01-21 19:46:16.184409 python_easyverein-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     5575 1970-01-01 00:00:00.000000 python_easyverein-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/LICENSE
+-rw-r--r--   0        0        0     5062 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/README.md
+-rw-r--r--   0        0        0      338 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/__init__.py
+-rw-r--r--   0        0        0     1399 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/api.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/core/__init__.py
+-rw-r--r--   0        0        0    11964 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/core/client.py
+-rw-r--r--   0        0        0      747 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/core/exceptions.py
+-rw-r--r--   0        0        0      493 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/core/protocol.py
+-rw-r--r--   0        0        0     1095 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/core/types.py
+-rw-r--r--   0        0        0      144 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/core/validators.py
+-rw-r--r--   0        0        0      835 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/models/__init__.py
+-rw-r--r--   0        0        0      720 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/models/base.py
+-rw-r--r--   0        0        0     6391 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/models/contact_details.py
+-rw-r--r--   0        0        0     3609 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/models/custom_field.py
+-rw-r--r--   0        0        0     4548 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/models/invoice.py
+-rw-r--r--   0        0        0     2609 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/models/invoice_item.py
+-rw-r--r--   0        0        0     7939 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/models/member.py
+-rw-r--r--   0        0        0     2587 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/models/member_custom_field.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/models/mixins/__init__.py
+-rw-r--r--   0        0        0      622 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/models/mixins/empty_strings_mixin.py
+-rw-r--r--   0        0        0     1478 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/models/mixins/required_attributes.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/modules/__init__.py
+-rw-r--r--   0        0        0      724 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/modules/contact_details.py
+-rw-r--r--   0        0        0      697 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/modules/custom_field.py
+-rw-r--r--   0        0        0     7359 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/modules/invoice.py
+-rw-r--r--   0        0        0      582 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/modules/invoice_item.py
+-rw-r--r--   0        0        0      572 2024-04-27 16:41:46.384312 python_easyverein-0.2.7/easyverein/modules/member.py
+-rw-r--r--   0        0        0     4107 2024-04-27 16:41:46.388312 python_easyverein-0.2.7/easyverein/modules/member_custom_field.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:41:46.388312 python_easyverein-0.2.7/easyverein/modules/mixins/__init__.py
+-rw-r--r--   0        0        0     7117 2024-04-27 16:41:46.388312 python_easyverein-0.2.7/easyverein/modules/mixins/crud.py
+-rw-r--r--   0        0        0     1707 2024-04-27 16:41:46.388312 python_easyverein-0.2.7/easyverein/modules/mixins/recycle_bin.py
+-rw-r--r--   0        0        0     1212 2024-04-27 16:41:46.388312 python_easyverein-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     5575 1970-01-01 00:00:00.000000 python_easyverein-0.2.7/PKG-INFO
```

### Comparing `python_easyverein-0.2.5/LICENSE` & `python_easyverein-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_easyverein-0.2.5/README.md` & `python_easyverein-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `python_easyverein-0.2.5/easyverein/api.py` & `python_easyverein-0.2.7/easyverein/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Main EasyVerein API class
 """
+
 import logging
 
 from .core.client import EasyvereinClient
 from .modules.contact_details import ContactDetailsMixin
 from .modules.custom_field import CustomFieldMixin
 from .modules.invoice import InvoiceMixin
 from .modules.invoice_item import InvoiceItemMixin
@@ -15,27 +16,30 @@
 class EasyvereinAPI:
     def __init__(
         self,
         api_key,
         api_version="v1.7",
         base_url: str = "https://hexa.easyverein.com/api/",
         logger: logging.Logger = None,
+        auto_retry=False,
     ):
         """
         Constructor setting API key and logger. Test
         """
 
         super().__init__()
 
         if logger:
             self.logger = logger
         else:
             self.logger = logging.getLogger("easyverein")
 
-        self.c = EasyvereinClient(api_key, api_version, base_url, self.logger, self)
+        self.c = EasyvereinClient(
+            api_key, api_version, base_url, self.logger, self, auto_retry
+        )
 
         # Add methods
 
         self.contact_details = ContactDetailsMixin(self.c, self.logger)
         self.custom_field = CustomFieldMixin(self.c, self.logger)
         self.invoice = InvoiceMixin(self.c, self.logger)
         self.invoice_item = InvoiceItemMixin(self.c, self.logger)
```

### Comparing `python_easyverein-0.2.5/easyverein/core/client.py` & `python_easyverein-0.2.7/easyverein/core/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Main EasyVerein API class
 """
+
 from __future__ import annotations
 
 import logging
 from pathlib import Path
+from time import sleep
 from typing import TYPE_CHECKING, Any, TypeVar
 
 import requests
 from pydantic import BaseModel
 from requests.structures import CaseInsensitiveDict
 
 from .exceptions import (
@@ -31,23 +33,25 @@
     def __init__(
         self,
         api_key,
         api_version,
         base_url,
         logger: logging.Logger,
         instance: EasyvereinAPI,
+        auto_retry=False,
     ):
         """
         Constructor setting API key and logger
         """
         self.api_key = api_key
         self.base_url = base_url
         self.api_version = api_version
         self.logger = logger
         self.api_instance = instance
+        self.auto_retry = auto_retry
 
     def _get_header(self):
         """
         Constructs a header for the API request
         """
         return {"Authorization": "Bearer " + self.api_key}
 
@@ -114,18 +118,29 @@
                 self.logger.debug("Retry-After header: %s", retry_after)
                 retry_after = 0
 
             self.logger.warning(
                 "Request returned status code 429, too many requests. Wait %d seconds",
                 retry_after,
             )
-            raise EasyvereinAPITooManyRetriesException(
-                f"Too many requests, please wait {retry_after} seconds and try again.",
-                retry_after=retry_after,
-            )
+            if self.auto_retry:
+                self.logger.warning("Retrying after %d seconds sleep.", retry_after)
+                sleep(retry_after)
+                if files:
+                    for v in files.values():
+                        v.seek(
+                            0
+                        )  # reset file seek, as it has been moved by the previous call
+
+                return self._do_request(method, url, binary, data, headers, files)
+            else:
+                raise EasyvereinAPITooManyRetriesException(
+                    f"Too many requests, please wait {retry_after} seconds and try again.",
+                    retry_after=retry_after,
+                )
 
         if res.status_code == 404:
             self.logger.warning("Request returned status code 404, resource not found")
             raise EasyvereinAPINotFoundException("Requested resource not found")
 
         # In some cases (for example on 204 delete) the response is empty
         if res.content == b"":
```

### Comparing `python_easyverein-0.2.5/easyverein/core/exceptions.py` & `python_easyverein-0.2.7/easyverein/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_easyverein-0.2.5/easyverein/core/types.py` & `python_easyverein-0.2.7/easyverein/core/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Custom types used for model validation
 """
+
 import datetime
 import json
 from typing import Annotated
 
 from pydantic import Field, PlainSerializer, UrlConstraints
 from pydantic_core import Url
```

### Comparing `python_easyverein-0.2.5/easyverein/models/__init__.py` & `python_easyverein-0.2.7/easyverein/models/__init__.py`

 * *Files identical despite different names*

### Comparing `python_easyverein-0.2.5/easyverein/models/base.py` & `python_easyverein-0.2.7/easyverein/models/base.py`

 * *Files identical despite different names*

### Comparing `python_easyverein-0.2.5/easyverein/models/contact_details.py` & `python_easyverein-0.2.7/easyverein/models/contact_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contact Details related models
 """
+
 from __future__ import annotations
 
 from typing import Any, Literal
 
 from pydantic import BaseModel, EmailStr, Field
 
 from ..core.types import Date, DateTime, FilterIntList
```

### Comparing `python_easyverein-0.2.5/easyverein/models/custom_field.py` & `python_easyverein-0.2.7/easyverein/models/custom_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Member related models
 """
+
 from __future__ import annotations
 
 from typing import Literal
 
 from pydantic import BaseModel, Field
 
 from ..core.types import (
@@ -32,17 +33,17 @@
         This endpoint manages the custom fields themselves, not their values.
     """
 
     name: str | None = Field(default=None, max_length=200)
     color: HexColor = None
     short: str | None = Field(default=None, max_length=4)
     orderSequence: PositiveIntWithZero | None = None
-    settings_type: Literal[
-        "t", "f", "z", "d", "c", "r", "s", "a", "b", "m"
-    ] | None = None
+    settings_type: Literal["t", "f", "z", "d", "c", "r", "s", "a", "b", "m"] | None = (
+        None
+    )
     """
     Settings type defines which type of field this custom field should be. Possible values:
 
     - t: Single line text field
     - f: Multiline text field
     - z: Digit text field
     - d: Date field
@@ -51,17 +52,20 @@
     - s: Select field
     - a: Multiselect field
     - b: File upload
     - m: reminder
 
     If type is set to s or a, the possible options need to be defined in the additional field
     """
-    kind: Literal[
-        "a", "b", "ba", "ca", "iv", "t", "u", "ic", "c", "e", "h", "j", "i", "k"
-    ] | None = None
+    kind: (
+        Literal[
+            "a", "b", "ba", "ca", "iv", "t", "u", "ic", "c", "e", "h", "j", "i", "k"
+        ]
+        | None
+    ) = None
     """
     Kind defines in which context this custom field is used. Unfortunately only some possible values are
     documented in the API spec:
 
     - e: for members
     - h: for events
     - j: for contact details
```

### Comparing `python_easyverein-0.2.5/easyverein/models/invoice.py` & `python_easyverein-0.2.7/easyverein/models/invoice.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Invoice related models
 """
+
 from __future__ import annotations
 
 from typing import Literal
 
 from pydantic import BaseModel
 
 from ..core.types import (
@@ -38,17 +39,26 @@
     description: str | None = None
     totalPrice: float | None = None
     tax: float | None = None
     taxRate: float | None = None
     taxName: str | None = None
     relatedAddress: ContactDetails | EasyVereinReference | None = None
     path: EasyVereinReference | None = None
-    kind: Literal[
-        "balance", "donation", "membership", "revenue", "expense", "cancel", "credit"
-    ] | None = None
+    kind: (
+        Literal[
+            "balance",
+            "donation",
+            "membership",
+            "revenue",
+            "expense",
+            "cancel",
+            "credit",
+        ]
+        | None
+    ) = None
     # TODO: Add reference to BillingAccount once implemented
     selectionAcc: EasyVereinReference | None = None
     refNumber: str | None = None
     paymentDifference: float | None = None
     isDraft: bool | None = None
     isTemplate: bool | None = None
     paymentInformation: str | None = None
```

### Comparing `python_easyverein-0.2.5/easyverein/models/invoice_item.py` & `python_easyverein-0.2.7/easyverein/models/invoice_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Invoice Item model
 """
+
 from __future__ import annotations
 
 from typing import Annotated
 
 from pydantic import BaseModel, PositiveInt, StringConstraints
 
 from ..core.types import EasyVereinReference, FilterIntList
```

### Comparing `python_easyverein-0.2.5/easyverein/models/member.py` & `python_easyverein-0.2.7/easyverein/models/member.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Member related models
 """
+
 from __future__ import annotations
 
 from typing import Literal
 
 from pydantic import BaseModel, Field, PositiveInt
 
 from ..core.types import (
```

### Comparing `python_easyverein-0.2.5/easyverein/models/member_custom_field.py` & `python_easyverein-0.2.7/easyverein/models/member_custom_field.py`

 * *Files identical despite different names*

### Comparing `python_easyverein-0.2.5/easyverein/models/mixins/empty_strings_mixin.py` & `python_easyverein-0.2.7/easyverein/models/mixins/empty_strings_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This module contains a generic plugin for Pydantic models that removes
 empty strings and converts them to None.
 """
+
 from typing import Any
 
 from pydantic import model_validator
 
 
 class EmptyStringsToNone:
     """
```

### Comparing `python_easyverein-0.2.5/easyverein/models/mixins/required_attributes.py` & `python_easyverein-0.2.7/easyverein/models/mixins/required_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This module contains a class factory returning a Mixin class
 """
+
 from typing import Self
 
 from pydantic import BaseModel, model_validator
 
 
 def required_mixin(required_attributes: list[str | list[str]]):
     """
```

### Comparing `python_easyverein-0.2.5/easyverein/modules/contact_details.py` & `python_easyverein-0.2.7/easyverein/modules/contact_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 All methods related to contact details
 """
+
 import logging
 
 from ..core.client import EasyvereinClient
 from ..models import ContactDetails, ContactDetailsCreate, ContactDetailsUpdate
 from ..models.contact_details import ContactDetailsFilter
 from .mixins.crud import CRUDMixin
 from .mixins.recycle_bin import RecycleBinMixin
```

### Comparing `python_easyverein-0.2.5/easyverein/modules/custom_field.py` & `python_easyverein-0.2.7/easyverein/modules/custom_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 All methods related to custom fields
 """
+
 import logging
 
 from ..core.client import EasyvereinClient
 from ..models.custom_field import (
     CustomField,
     CustomFieldCreate,
     CustomFieldFilter,
```

### Comparing `python_easyverein-0.2.5/easyverein/modules/invoice.py` & `python_easyverein-0.2.7/easyverein/modules/invoice.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import logging
+import re
+import urllib
 from pathlib import Path
 from typing import List
 
 from requests.structures import CaseInsensitiveDict
 
 from ..core.client import EasyvereinClient
 from ..core.exceptions import EasyvereinAPIException
@@ -165,8 +167,14 @@
             path = fetched_invoice.path
 
         if not path:
             raise EasyvereinAPIException(
                 "Unable to obtain a valid path for given invoice."
             )
 
-        return self.c.fetch_file(path)
+        # Fix for unencoded characters - should probably be fixed in easyverein API
+        m = re.fullmatch(r"^(.*\&path=)(.*)(&storedInS3=True)$", path.unicode_string())
+        url_components = list(m.groups())
+        if "%" not in url_components[1]:
+            url_components[1] = urllib.parse.quote(url_components[1])
+
+        return self.c.fetch_file("".join(url_components))
```

### Comparing `python_easyverein-0.2.5/easyverein/modules/invoice_item.py` & `python_easyverein-0.2.7/easyverein/modules/invoice_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 All methods related to invoices
 """
+
 import logging
 
 from ..core.client import EasyvereinClient
 from ..models.invoice_item import (
     InvoiceItem,
     InvoiceItemCreate,
     InvoiceItemFilter,
```

### Comparing `python_easyverein-0.2.5/easyverein/modules/member.py` & `python_easyverein-0.2.7/easyverein/modules/member.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 All methods related to invoices
 """
+
 import logging
 
 from ..core.client import EasyvereinClient
 from ..models.member import Member, MemberCreate, MemberFilter, MemberUpdate
 from .mixins.crud import CRUDMixin
 from .mixins.recycle_bin import RecycleBinMixin
```

### Comparing `python_easyverein-0.2.5/easyverein/modules/member_custom_field.py` & `python_easyverein-0.2.7/easyverein/modules/member_custom_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 All methods related to invoices
 """
+
 import logging
 
 from ..core.client import EasyvereinClient
 from ..core.protocol import IsEVClientProtocol
 from ..models import MemberCustomField, MemberCustomFieldCreate, MemberCustomFieldUpdate
 from ..models.member_custom_field import MemberCustomFieldFilter
 from .mixins.crud import CRUDMixin
```

### Comparing `python_easyverein-0.2.5/easyverein/modules/mixins/crud.py` & `python_easyverein-0.2.7/easyverein/modules/mixins/crud.py`

 * *Files identical despite different names*

### Comparing `python_easyverein-0.2.5/easyverein/modules/mixins/recycle_bin.py` & `python_easyverein-0.2.7/easyverein/modules/mixins/recycle_bin.py`

 * *Files identical despite different names*

### Comparing `python_easyverein-0.2.5/pyproject.toml` & `python_easyverein-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-easyverein"
-version = "0.2.5"
+version = "0.2.7"
 description = "Python library to interact with the EasyVerein API"
 authors = ["Daniel Herrmann <daniel.herrmann1@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "easyverein" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `python_easyverein-0.2.5/PKG-INFO` & `python_easyverein-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-easyverein
-Version: 0.2.5
+Version: 0.2.7
 Summary: Python library to interact with the EasyVerein API
 Author: Daniel Herrmann
 Author-email: daniel.herrmann1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

