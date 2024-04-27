# Comparing `tmp/django_utz-0.1.9.tar.gz` & `tmp/django_utz-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_utz-0.1.9.tar", last modified: Sat Feb 10 18:21:34 2024, max compression
+gzip compressed data, was "django_utz-0.2.0.tar", last modified: Fri Apr 26 20:43:50 2024, max compression
```

## Comparing `django_utz-0.1.9.tar` & `django_utz-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-02-10 18:21:34.288978 django_utz-0.1.9/
--rw-rw-rw-   0        0        0     1104 2024-02-04 03:14:29.000000 django_utz-0.1.9/LICENSE
--rw-rw-rw-   0        0        0    22341 2024-02-10 18:21:34.270396 django_utz-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0    21035 2024-02-04 14:43:08.000000 django_utz-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-02-10 18:21:33.955826 django_utz-0.1.9/django_utz/
--rw-rw-rw-   0        0        0      655 2024-02-10 18:21:04.000000 django_utz-0.1.9/django_utz/__init__.py
--rw-rw-rw-   0        0        0      198 2024-02-03 17:21:50.000000 django_utz-0.1.9/django_utz/apps.py
--rw-rw-rw-   0        0        0      208 2024-02-03 20:45:17.000000 django_utz-0.1.9/django_utz/base_exceptions.py
--rw-rw-rw-   0        0        0     1406 2024-02-01 09:14:21.000000 django_utz-0.1.9/django_utz/datetime.py
-drwxrwxrwx   0        0        0        0 2024-02-10 18:21:34.066053 django_utz-0.1.9/django_utz/decorators/
--rw-rw-rw-   0        0        0      141 2024-02-03 21:04:25.000000 django_utz-0.1.9/django_utz/decorators/__init__.py
--rw-rw-rw-   0        0        0     1225 2024-02-03 16:54:19.000000 django_utz-0.1.9/django_utz/decorators/bases.py
-drwxrwxrwx   0        0        0        0 2024-02-10 18:21:34.144635 django_utz-0.1.9/django_utz/decorators/models/
--rw-rw-rw-   0        0        0      141 2024-02-03 17:09:17.000000 django_utz-0.1.9/django_utz/decorators/models/__init__.py
--rw-rw-rw-   0        0        0     3449 2024-02-10 17:58:58.000000 django_utz-0.1.9/django_utz/decorators/models/bases.py
--rw-rw-rw-   0        0        0    10250 2024-02-10 18:05:25.000000 django_utz-0.1.9/django_utz/decorators/models/decorators.py
--rw-rw-rw-   0        0        0      276 2024-02-04 02:15:49.000000 django_utz-0.1.9/django_utz/decorators/models/exceptions.py
--rw-rw-rw-   0        0        0     4799 2024-02-04 02:29:09.000000 django_utz-0.1.9/django_utz/decorators/models/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-10 18:21:34.202151 django_utz-0.1.9/django_utz/decorators/serializers/
--rw-rw-rw-   0        0        0      531 2024-02-03 17:18:11.000000 django_utz-0.1.9/django_utz/decorators/serializers/__init__.py
--rw-rw-rw-   0        0        0     8802 2024-02-10 18:16:42.000000 django_utz-0.1.9/django_utz/decorators/serializers/decorators.py
--rw-rw-rw-   0        0        0      286 2024-02-04 02:15:55.000000 django_utz-0.1.9/django_utz/decorators/serializers/exceptions.py
--rw-rw-rw-   0        0        0     4508 2024-02-10 17:51:21.000000 django_utz-0.1.9/django_utz/decorators/utils.py
--rw-rw-rw-   0        0        0     1575 2024-02-04 03:19:03.000000 django_utz-0.1.9/django_utz/middleware.py
--rw-rw-rw-   0        0        0     3031 2024-02-04 02:43:52.000000 django_utz-0.1.9/django_utz/serializer_fields.py
--rw-rw-rw-   0        0        0     1306 2024-02-04 03:14:58.000000 django_utz-0.1.9/django_utz/signals.py
-drwxrwxrwx   0        0        0        0 2024-02-10 18:21:34.243204 django_utz-0.1.9/django_utz/templatetags/
--rw-rw-rw-   0        0        0       96 2023-08-21 23:07:01.000000 django_utz-0.1.9/django_utz/templatetags/__init__.py
--rw-rw-rw-   0        0        0     5860 2024-02-07 10:40:55.000000 django_utz-0.1.9/django_utz/templatetags/django_utz.py
-drwxrwxrwx   0        0        0        0 2024-02-10 18:21:34.270396 django_utz-0.1.9/django_utz.egg-info/
--rw-rw-rw-   0        0        0    22341 2024-02-10 18:21:33.000000 django_utz-0.1.9/django_utz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      890 2024-02-10 18:21:33.000000 django_utz-0.1.9/django_utz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-10 18:21:33.000000 django_utz-0.1.9/django_utz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-02-10 18:21:33.000000 django_utz-0.1.9/django_utz.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-10 18:21:33.000000 django_utz-0.1.9/django_utz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1450 2024-02-04 15:00:52.000000 django_utz-0.1.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-10 18:21:34.288978 django_utz-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 20:43:50.242676 django_utz-0.2.0/
+-rw-rw-rw-   0        0        0     1104 2024-02-04 03:14:29.000000 django_utz-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0    22577 2024-04-26 20:43:50.239102 django_utz-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    21271 2024-04-26 20:23:13.000000 django_utz-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 20:43:50.022062 django_utz-0.2.0/django_utz/
+-rw-rw-rw-   0        0        0      661 2024-04-26 20:40:16.000000 django_utz-0.2.0/django_utz/__init__.py
+-rw-rw-rw-   0        0        0      198 2024-02-03 17:21:50.000000 django_utz-0.2.0/django_utz/apps.py
+-rw-rw-rw-   0        0        0      208 2024-02-03 20:45:17.000000 django_utz-0.2.0/django_utz/base_exceptions.py
+-rw-rw-rw-   0        0        0     1406 2024-02-01 09:14:21.000000 django_utz-0.2.0/django_utz/datetime.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:43:50.096234 django_utz-0.2.0/django_utz/decorators/
+-rw-rw-rw-   0        0        0      198 2024-04-26 20:12:25.000000 django_utz-0.2.0/django_utz/decorators/__init__.py
+-rw-rw-rw-   0        0        0     1225 2024-02-03 16:54:19.000000 django_utz-0.2.0/django_utz/decorators/bases.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:43:50.156968 django_utz-0.2.0/django_utz/decorators/models/
+-rw-rw-rw-   0        0        0      141 2024-02-03 17:09:17.000000 django_utz-0.2.0/django_utz/decorators/models/__init__.py
+-rw-rw-rw-   0        0        0     3419 2024-04-26 20:40:54.000000 django_utz-0.2.0/django_utz/decorators/models/bases.py
+-rw-rw-rw-   0        0        0    10150 2024-04-26 20:38:40.000000 django_utz-0.2.0/django_utz/decorators/models/decorators.py
+-rw-rw-rw-   0        0        0      276 2024-02-04 02:15:49.000000 django_utz-0.2.0/django_utz/decorators/models/exceptions.py
+-rw-rw-rw-   0        0        0     5721 2024-04-26 20:41:16.000000 django_utz-0.2.0/django_utz/decorators/models/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:43:50.198320 django_utz-0.2.0/django_utz/decorators/serializers/
+-rw-rw-rw-   0        0        0      531 2024-02-03 17:18:11.000000 django_utz-0.2.0/django_utz/decorators/serializers/__init__.py
+-rw-rw-rw-   0        0        0     8803 2024-04-26 04:22:55.000000 django_utz-0.2.0/django_utz/decorators/serializers/decorators.py
+-rw-rw-rw-   0        0        0      286 2024-02-04 02:15:55.000000 django_utz-0.2.0/django_utz/decorators/serializers/exceptions.py
+-rw-rw-rw-   0        0        0     4520 2024-04-26 20:11:31.000000 django_utz-0.2.0/django_utz/decorators/utils.py
+-rw-rw-rw-   0        0        0     1575 2024-02-04 03:19:03.000000 django_utz-0.2.0/django_utz/middleware.py
+-rw-rw-rw-   0        0        0     3031 2024-02-04 02:43:52.000000 django_utz-0.2.0/django_utz/serializer_fields.py
+-rw-rw-rw-   0        0        0     1573 2024-04-26 20:22:15.000000 django_utz-0.2.0/django_utz/signals.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:43:50.231096 django_utz-0.2.0/django_utz/templatetags/
+-rw-rw-rw-   0        0        0       96 2023-08-21 23:07:01.000000 django_utz-0.2.0/django_utz/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     5870 2024-04-26 20:14:11.000000 django_utz-0.2.0/django_utz/templatetags/django_utz.py
+drwxrwxrwx   0        0        0        0 2024-04-26 20:43:50.231096 django_utz-0.2.0/django_utz.egg-info/
+-rw-rw-rw-   0        0        0    22577 2024-04-26 20:43:49.000000 django_utz-0.2.0/django_utz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      890 2024-04-26 20:43:49.000000 django_utz-0.2.0/django_utz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 20:43:49.000000 django_utz-0.2.0/django_utz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-26 20:43:49.000000 django_utz-0.2.0/django_utz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-26 20:43:49.000000 django_utz-0.2.0/django_utz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1450 2024-02-04 15:00:52.000000 django_utz-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 20:43:50.242676 django_utz-0.2.0/setup.cfg
```

### Comparing `django_utz-0.1.9/LICENSE` & `django_utz-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_utz-0.1.9/PKG-INFO` & `django_utz-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_utz
-Version: 0.1.9
+Version: 0.2.0
 Summary: Get datetime values in model instances and model serializers in user's time zone without the need to manually perform timezone conversions for each user.
 Author-email: "Daniel T. Afolayan (ti-oluwa)" <tioluwa.dev@gmail.com>
 Maintainer-email: "Daniel T. Afolayan (ti-oluwa)" <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/django_utz
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/django_utz/issues
 Project-URL: Repository, https://github.com/ti-oluwa/django_utz
 Keywords: User Timezone,Auto Timezone Conversion,Django Timezone
@@ -47,19 +47,20 @@
 ```python
 INSTALLED_APPS = [
     ...,
     'django_utz',
 ]
 ```
 
-Add `django_utz.middleware.DjangoUTZMiddleware` to `MIDDLEWARE`
+Add `django_utz.middleware.DjangoUTZMiddleware` to `MIDDLEWARE` just below `AuthenticationMiddleware`:
 
 ```python
 MIDDLEWARE = [
     ...,
+    'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django_utz.middleware.DjangoUTZMiddleware',
 ]
 ```
 
 You can then import and use the required user model decorator
 
 ```python
@@ -411,26 +412,28 @@
     class Meta:
         model = Post
         fields = "__all__"
 ```
 
 ## Signals
 
-The `django_utz.signals` module contains signals that are sent when an event occurs on a user's timezone. The signals are:
+The `django_utz.signals` module contain signals that are sent when an event occurs on a user's timezone. The signals are:
 
 - `user_timezone_changed`: Sent when a user's timezone is updated.
 
+> These signals are disabled by default. To ensure that the signals are sent set `ENABLE_UTZ_SIGNALS` to `True` in your settings.py file.
+
 In your receiver, you can access the user object, its previous timezone and current timezone with the `instance`, `previous_timezone`and `current_timezone` keyword arguments respectively.
 
 ```python
 from django.dispatch import receiver
 from django_utz.signals import user_timezone_changed
 
 @receiver(user_timezone_changed)
-def user_timezone_changed_receiver(sender, **kwargs):
+def timezone_change_handler(sender, **kwargs):
     old_timezone = kwargs.get("previous_timezone")
     new_timezone = kwargs.get("current_timezone")
     print(old_timezone, new_timezone)
 ```
 
 ## Templates
```

### Comparing `django_utz-0.1.9/README.md` & `django_utz-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,19 +19,20 @@
 ```python
 INSTALLED_APPS = [
     ...,
     'django_utz',
 ]
 ```
 
-Add `django_utz.middleware.DjangoUTZMiddleware` to `MIDDLEWARE`
+Add `django_utz.middleware.DjangoUTZMiddleware` to `MIDDLEWARE` just below `AuthenticationMiddleware`:
 
 ```python
 MIDDLEWARE = [
     ...,
+    'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django_utz.middleware.DjangoUTZMiddleware',
 ]
 ```
 
 You can then import and use the required user model decorator
 
 ```python
@@ -383,26 +384,28 @@
     class Meta:
         model = Post
         fields = "__all__"
 ```
 
 ## Signals
 
-The `django_utz.signals` module contains signals that are sent when an event occurs on a user's timezone. The signals are:
+The `django_utz.signals` module contain signals that are sent when an event occurs on a user's timezone. The signals are:
 
 - `user_timezone_changed`: Sent when a user's timezone is updated.
 
+> These signals are disabled by default. To ensure that the signals are sent set `ENABLE_UTZ_SIGNALS` to `True` in your settings.py file.
+
 In your receiver, you can access the user object, its previous timezone and current timezone with the `instance`, `previous_timezone`and `current_timezone` keyword arguments respectively.
 
 ```python
 from django.dispatch import receiver
 from django_utz.signals import user_timezone_changed
 
 @receiver(user_timezone_changed)
-def user_timezone_changed_receiver(sender, **kwargs):
+def timezone_change_handler(sender, **kwargs):
     old_timezone = kwargs.get("previous_timezone")
     new_timezone = kwargs.get("current_timezone")
     print(old_timezone, new_timezone)
 ```
 
 ## Templates
```

### Comparing `django_utz-0.1.9/django_utz/__init__.py` & `django_utz-0.2.0/django_utz/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 Decorators for Django models and DRF model serializers, custom serializer fields, 
 template tags and filters that aid easy conversion of timezone aware fields to a user's timezone.
 
 @Author: Daniel T. Afolayan (ti-oluwa.github.io)
 """
 
-__version__ = "0.1.9"
+__version__ = "0.2.0"
 __author__ = "Daniel T. Afolayan"
 
 alias = "django-user-timezone"
 
 try:
     import zoneinfo
 except ImportError:
     from backports import zoneinfo
-except:
+except Exception:
     raise Exception(
         "django_utz couldn't import the zoneinfo module.\
          Perhaps you are on an older version of Python, run `pip install backports.zoneinfo` to continue."
-        )
+    )
```

### Comparing `django_utz-0.1.9/django_utz/datetime.py` & `django_utz-0.2.0/django_utz/datetime.py`

 * *Files identical despite different names*

### Comparing `django_utz-0.1.9/django_utz/decorators/bases.py` & `django_utz-0.2.0/django_utz/decorators/bases.py`

 * *Files identical despite different names*

### Comparing `django_utz-0.1.9/django_utz/decorators/models/bases.py` & `django_utz-0.2.0/django_utz/decorators/models/bases.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from abc import ABC, abstractmethod
 import inspect
 from typing import Any, TypeVar
 from django.db import models
-from django.db import models
 
 from ..bases import UTZDecorator
 from .exceptions import ModelConfigurationError
 
 DjangoModel = TypeVar("DjangoModel", bound=models.Model)
```

### Comparing `django_utz-0.1.9/django_utz/decorators/models/decorators.py` & `django_utz-0.2.0/django_utz/decorators/models/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from django.db import models
 import pytz
 import datetime
-from django.db import models
 from django.conf import settings
-
 try:
     import zoneinfo
-except:
+except ImportError:
     from backports import zoneinfo
 from django.contrib.auth.models import AbstractBaseUser
 from typing import TypeVar, List
 from django.core.exceptions import FieldDoesNotExist
 from typing import Callable
 
 
 from ..utils import is_datetime_field, is_timezone_valid, validate_timezone, transform_utz_decorator
 from ...datetime import utzdatetime
 from .exceptions import ModelError, ModelConfigurationError
 from .bases import ModelDecorator, DjangoModel
-from .utils import get_user, is_user_model, FunctionAttribute
+from .utils import get_user, is_user_model, FunctionAttribute, get_datetime_fields
 
 
 
 class UserModelUTZMixin:
-    """Adds neccessary methods and properties to the User Model"""
+    """Adds necessary utz methods and properties to a User Model"""
     
     @property
     def utz(self):
         """
         The user's timezone info as a `pytz.tzinfo` or `zoneinfo.ZoneInfo` object.
 
         if settings.USE_DEPRECATED_PYTZ is True, then the user's timezone info is returned as a pytz.tzinfo object.
@@ -39,15 +37,15 @@
             zone_str = str(utz)
 
         elif utz and isinstance(utz, str):
             if not is_timezone_valid(utz):
                 raise ValueError(f"Invalid timezone: {utz}.")
             zone_str = utz
 
-        if getattr(settings, "USE_DEPRECATED_PYTZ", False):
+        if getattr(settings, "USE_DEPRECATED_PYTZ", False) is True:
             return pytz.timezone(zone_str)
 
         return zoneinfo.ZoneInfo(zone_str)
 
 
     def to_local_timezone(self, _datetime: datetime.datetime) -> utzdatetime:
         """
@@ -85,15 +83,18 @@
     def __init__(self, model: UserModel) -> None:
         super().__init__(model)
 
 
     def check_model(self, model: UserModel) -> UserModel:
         """Ensures that the model in which this mixin is used is the project's user model"""
         if not is_user_model(model):
-            raise ModelError(f"Model '{model.__name__}' is not the project's user model")  
+            raise ModelError(
+                f"Model '{model.__name__}' is not the project's user model"
+                "Ensure that the decorated model is the one defined in settings.AUTH_USER_MODEL"
+            )  
         return super().check_model(model) 
     
 
     def validate_timezone_field(self, value: str) -> None:
         if not isinstance(value, str):
             raise ModelConfigurationError("Value for 'timezone_field' should be of type str")
         return None
@@ -126,29 +127,29 @@
         if related_user and not isinstance(related_user, str):
             raise ModelConfigurationError("'related_user' should be of type str")
         return model
     
 
     def prepare_model(self) -> DjangoModel:
         if self.get_config("datetime_fields") == "__all__":
-            self.set_config("datetime_fields", self.get_datetime_fields(self.model))
+            self.set_config("datetime_fields", get_datetime_fields(self.model))
 
         if not self.get_config("attribute_suffix"):
             self.set_config("attribute_suffix", "utz")
 
         if not self.get_config("use_related_user_timezone"):
             self.set_config("use_related_user_timezone", False)
 
         return self.update_model_attrs(self.model)
     
 
     def validate_datetime_fields(self, value: str | List[str] | tuple[str]) -> None:
         if value != "__all__" and not isinstance(value, (list, tuple)):
             raise ModelConfigurationError(
-                f"'datetime_fields' should be a list, tuple or '__all__'"
+                "'datetime_fields' should be a list, tuple or '__all__'"
             )
         return None
     
 
     def validate_attribute_suffix(self, value: str) -> None:
         if not isinstance(value, str):
             raise ModelConfigurationError("'attribute_suffix' should be of type str")
@@ -157,30 +158,25 @@
 
     def validate_use_related_user_timezone(self, value: bool) -> None:
         if not isinstance(value, bool):
             raise ModelConfigurationError("'use_related_user_timezone' should be of type bool")
         return None
     
 
-    def get_datetime_fields(self, model: DjangoModel) -> List[str]:
-        """Returns the datetime fields in the given model."""
-        return [field.name for field in model._meta.fields if isinstance(field, models.DateTimeField)]
-    
-
     def make_func_for_field(self, datetime_field: str) -> Callable[[models.Model], utzdatetime]:
         """
         Makes and returns a function that returns the value of the datetime field on a model instance
         in the user's local timezone.
 
         :param datetime_field: The name of the datetime field for which to make the function
         """
         func_name = f"get_{datetime_field}_{self.get_config('attribute_suffix')}"
 
         def func(model_instance: models.Model) -> utzdatetime:
-            user: UserModel = get_user(model_instance)
+            user: UTZUserModel | None = get_user(model_instance)
             if user is None:
                 return utzdatetime.from_datetime(getattr(model_instance, datetime_field))
             return user.to_local_timezone(getattr(model_instance, datetime_field))
         
         func.__name__ = func_name
         func.__qualname__ = func_name
         return func
```

### Comparing `django_utz-0.1.9/django_utz/decorators/models/utils.py` & `django_utz-0.2.0/django_utz/decorators/models/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import Callable
+from typing import Callable, List, Any
 from django.db import models
 from django.conf import settings
 
 from ..utils import get_attr_by_traversal
 from ...middleware import get_request_user
-from ...datetime import utzdatetime
 from .exceptions import ModelError, ModelConfigurationError
 
 
 def get_model_traversal_path(model: type[models.Model]) -> str:
     """Returns the traversal path to the model."""
     return f"{model.__module__}.{model.__name__}"
 
@@ -23,21 +22,20 @@
 
 
 def is_user_model(model: type[models.Model]) -> bool:
     """Check if the model is the project's user model."""
     return get_project_user_model() == get_model_traversal_path(model)
 
 
-
 class FunctionAttribute:
     """
     A descriptor class that returns the result of 
     passing an object into a function as an attribute.
     """
-    def __init__(self, func: Callable[..., utzdatetime]):
+    def __init__(self, func: Callable[..., Any]):
         if not callable(func):
             raise TypeError("Value must be a function.")
         self.func = func
 
 
     def __set_name__(self, objtype, name: str):
         if not isinstance(name, str):
@@ -45,15 +43,14 @@
         self.name = name
 
 
     def __get__(self, obj, objtype):
         return self.func(obj)
 
 
-
 def get_user(model_obj: models.Model) -> models.Model | None:
     """
     Gets and returns the user object whose timezone is to be used by the model instance.
     
     If  the `use_related_user_timezone` config is True and `related_user` is not set, the first
     user object found that is related to the model instance is returned.
 
@@ -70,15 +67,15 @@
         if model_obj_cls.UTZMeta.use_related_user_timezone:
             # Get the user object as specified by the `related_user` config 
             # or by finding the user field in the model and its related models
             related_user = getattr(model_obj_cls.UTZMeta, "related_user", None) or find_user_field(model_obj_cls)
             if not related_user:
                 if getattr(model_obj_cls.UTZMeta, "related_user", None):
                     raise ModelConfigurationError(
-                        f"Please set the `related_user` config to the name or traversal path of the user field in {model_obj_cls.__name__}."
+                        f"Make sure to set the `related_user` config to the name or traversal path of the user field in {model_obj_cls.__name__}."
                     )
                 raise ModelError(f"No relation to the User model was found in {model_obj_cls.__name__}")
             
             user = get_attr_by_traversal(obj=model_obj, traversal_path=related_user)
 
         else:
             user = get_request_user()
@@ -88,36 +85,53 @@
         if not user_model_is_decorated:
             raise ModelError(
                 f"Model '{user.__class__.__name__}', has not been decorated with a `ModelDecorator`"
             )
     return user
 
 
-
 def find_user_field(model: type[models.Model]) -> str | None:
     """
     Finds and returns the traversal path to the first user field found
     in the model or its related models.
 
     This method assumes that the user is a foreign key or one-to-one field.
     """
     field_paths = []
-
+    
     def find_user_related_field(model: type[models.Model]) -> str | None:
         """
         Finds and returns the user related field traversal path 
         in the given model or its related models.
         """
+        # First check all the fields in the model for the user field
+        # If the user field is found, return the field path (Surface-level search)
+        for field in model._meta.fields:
+            if not is_user_model(field.related_model):
+                continue
+            field_paths.append(field.name)
+            return ".".join(field_paths)
+
+        # If the user field was not found at surface level, check each field's related model (if any).
         for field in model._meta.fields:
             related_model = field.related_model
             if related_model and isinstance(field, (models.ForeignKey, models.OneToOneField)):
                 field_paths.append(field.name)
 
                 if is_user_model(related_model):
                     return ".".join(field_paths)
                 else:
-                    # if the field is not the user model, recursively check the field's related_model for the user field
-                    return find_user_related_field(related_model)  
-        field_paths.pop()
-        return None
-            
+                    # If the field is not the user field, recursively check the field's 
+                    # related model for the user field, both at surface level and in its related models (if any).
+                    return find_user_related_field(related_model) 
+                
+        # If the user field was not found in the model or its related models, pop the last field path and return. 
+        if field_paths:
+            field_paths.pop()
+        return
+         
     return find_user_related_field(model)
+
+
+def get_datetime_fields(self, model: type[models.Model]) -> List[str]:
+    """Returns a list of the datetime fields in the given model."""
+    return [field.name for field in model._meta.fields if isinstance(field, models.DateTimeField)]
```

### Comparing `django_utz-0.1.9/django_utz/decorators/serializers/__init__.py` & `django_utz-0.2.0/django_utz/decorators/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `django_utz-0.1.9/django_utz/decorators/serializers/decorators.py` & `django_utz-0.2.0/django_utz/decorators/serializers/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
         val = getattr(self.serializer.UTZMeta, attr, default)
         if val is not None and hasattr(self, f"validate_{attr}"):
             getattr(self, f"validate_{attr}")(val)
         return val
 
 
 
-# Funtion-type decorator for `rest_framework.serializers.ModelSerializer` classes
+# Function-type decorator for `rest_framework.serializers.ModelSerializer` classes
 
 def modelserializer(serializer: DRFModelSerializer) -> DRFModelSerializer:
     """
     #### `django_utz` decorator for `reest_framework.serializers.ModelSerializer` classes.
 
     This decorator auto adds user timezone aware datetime fields to the serializer class 
     in-place of the normal datetime fields, if `auto_add_fields` config is set as True.
```

### Comparing `django_utz-0.1.9/django_utz/decorators/utils.py` & `django_utz-0.2.0/django_utz/decorators/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Utility functions for `django_utz` decorators"""
 try:
     import zoneinfo
-except:
+except ImportError:
     from backports import zoneinfo
 from typing import Any, Callable, TypeVar
 import pytz
 import datetime
 from django.db import models
 from django.core.exceptions import ValidationError
 import functools
```

### Comparing `django_utz-0.1.9/django_utz/middleware.py` & `django_utz-0.2.0/django_utz/middleware.py`

 * *Files identical despite different names*

### Comparing `django_utz-0.1.9/django_utz/serializer_fields.py` & `django_utz-0.2.0/django_utz/serializer_fields.py`

 * *Files identical despite different names*

### Comparing `django_utz-0.1.9/django_utz/signals.py` & `django_utz-0.2.0/django_utz/signals.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from django.contrib.auth import get_user_model
-from django.dispatch import Signal, receiver
+from django.dispatch import Signal
 from django.db.models.signals import pre_save
-
+from django.conf import settings
 
 
 ProjectUserModel = get_user_model()
 
 user_timezone_changed = Signal()
 # ----------------------------------------------------
 # This signal is sent when a user's timezone is changed.
 # kwargs: instance, previous_timezone, current_timezone
 # ----------------------------------------------------
 
-@receiver(pre_save, sender=ProjectUserModel)
 def utz_change_handler(sender, **kwargs) -> None:
     """Signal handler for user timezone changes"""
     user = kwargs["instance"]
     utz_meta = getattr(sender, "UTZMeta", None)
 
     if utz_meta and utz_meta._decorated:
         tz_field = getattr(utz_meta, "timezone_field")
@@ -30,7 +29,14 @@
             user_timezone_changed.send(
                 sender=sender, 
                 instance=user, 
                 previous_timezone=previous_timezone, 
                 current_timezone=current_timezone
             )
     return None
+
+
+# ----------------------------------------------------
+# Connect the signal handler to the user model
+# ----------------------------------------------------
+if getattr(settings, "ENABLE_UTZ_SIGNALS", False) is True:
+    pre_save.connect(utz_change_handler, sender=ProjectUserModel)
```

### Comparing `django_utz-0.1.9/django_utz/templatetags/django_utz.py` & `django_utz-0.2.0/django_utz/templatetags/django_utz.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,10 +170,10 @@
     utz_meta = getattr(user, "UTZMeta", None)
     is_decorated = utz_meta and utz_meta._decorated and issubclass(user.__class__, UserModelUTZMixin)
     # If the user model was not decorated with the `usermodel` decorator, return the value as is
     if not is_decorated:
         return value
     try:
         return user.to_local_timezone(value)
-    except:
+    except Exception:
         return value
```

### Comparing `django_utz-0.1.9/django_utz.egg-info/PKG-INFO` & `django_utz-0.2.0/django_utz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_utz
-Version: 0.1.9
+Version: 0.2.0
 Summary: Get datetime values in model instances and model serializers in user's time zone without the need to manually perform timezone conversions for each user.
 Author-email: "Daniel T. Afolayan (ti-oluwa)" <tioluwa.dev@gmail.com>
 Maintainer-email: "Daniel T. Afolayan (ti-oluwa)" <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/django_utz
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/django_utz/issues
 Project-URL: Repository, https://github.com/ti-oluwa/django_utz
 Keywords: User Timezone,Auto Timezone Conversion,Django Timezone
@@ -47,19 +47,20 @@
 ```python
 INSTALLED_APPS = [
     ...,
     'django_utz',
 ]
 ```
 
-Add `django_utz.middleware.DjangoUTZMiddleware` to `MIDDLEWARE`
+Add `django_utz.middleware.DjangoUTZMiddleware` to `MIDDLEWARE` just below `AuthenticationMiddleware`:
 
 ```python
 MIDDLEWARE = [
     ...,
+    'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django_utz.middleware.DjangoUTZMiddleware',
 ]
 ```
 
 You can then import and use the required user model decorator
 
 ```python
@@ -411,26 +412,28 @@
     class Meta:
         model = Post
         fields = "__all__"
 ```
 
 ## Signals
 
-The `django_utz.signals` module contains signals that are sent when an event occurs on a user's timezone. The signals are:
+The `django_utz.signals` module contain signals that are sent when an event occurs on a user's timezone. The signals are:
 
 - `user_timezone_changed`: Sent when a user's timezone is updated.
 
+> These signals are disabled by default. To ensure that the signals are sent set `ENABLE_UTZ_SIGNALS` to `True` in your settings.py file.
+
 In your receiver, you can access the user object, its previous timezone and current timezone with the `instance`, `previous_timezone`and `current_timezone` keyword arguments respectively.
 
 ```python
 from django.dispatch import receiver
 from django_utz.signals import user_timezone_changed
 
 @receiver(user_timezone_changed)
-def user_timezone_changed_receiver(sender, **kwargs):
+def timezone_change_handler(sender, **kwargs):
     old_timezone = kwargs.get("previous_timezone")
     new_timezone = kwargs.get("current_timezone")
     print(old_timezone, new_timezone)
 ```
 
 ## Templates
```

### Comparing `django_utz-0.1.9/django_utz.egg-info/SOURCES.txt` & `django_utz-0.2.0/django_utz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_utz-0.1.9/pyproject.toml` & `django_utz-0.2.0/pyproject.toml`

 * *Files identical despite different names*

