# Comparing `tmp/yggdrasil_mc-0.2.3.tar.gz` & `tmp/yggdrasil_mc-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yggdrasil_mc-0.2.3.tar", max compression
+gzip compressed data, was "yggdrasil_mc-0.2.4.tar", max compression
```

## Comparing `yggdrasil_mc-0.2.3.tar` & `yggdrasil_mc-0.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    34514 2024-01-19 15:05:07.449824 yggdrasil_mc-0.2.3/LICENSE
--rw-r--r--   0        0        0     1097 2024-01-19 15:05:07.449824 yggdrasil_mc-0.2.3/README.md
--rw-r--r--   0        0        0     1570 2024-01-19 15:05:07.449824 yggdrasil_mc-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-19 15:05:07.449824 yggdrasil_mc-0.2.3/yggdrasil_mc/__init__.py
--rw-r--r--   0        0        0     3383 2024-01-19 15:05:07.449824 yggdrasil_mc-0.2.3/yggdrasil_mc/client.py
--rw-r--r--   0        0        0       47 2024-01-19 15:05:07.449824 yggdrasil_mc-0.2.3/yggdrasil_mc/exceptions.py
--rw-r--r--   0        0        0     1212 2024-01-19 15:05:07.449824 yggdrasil_mc-0.2.3/yggdrasil_mc/models.py
--rw-r--r--   0        0        0       89 2024-01-19 15:05:07.449824 yggdrasil_mc-0.2.3/yggdrasil_mc/utils.py
--rw-r--r--   0        0        0     2446 1970-01-01 00:00:00.000000 yggdrasil_mc-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    34514 2024-04-27 03:20:22.070627 yggdrasil_mc-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1419 2024-04-27 03:20:22.070627 yggdrasil_mc-0.2.4/README.md
+-rw-r--r--   0        0        0     1570 2024-04-27 03:20:22.070627 yggdrasil_mc-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-27 03:20:22.070627 yggdrasil_mc-0.2.4/yggdrasil_mc/__init__.py
+-rw-r--r--   0        0        0     3589 2024-04-27 03:20:22.070627 yggdrasil_mc-0.2.4/yggdrasil_mc/client.py
+-rw-r--r--   0        0        0       47 2024-04-27 03:20:22.070627 yggdrasil_mc-0.2.4/yggdrasil_mc/exceptions.py
+-rw-r--r--   0        0        0     1282 2024-04-27 03:20:22.070627 yggdrasil_mc-0.2.4/yggdrasil_mc/models.py
+-rw-r--r--   0        0        0       89 2024-04-27 03:20:22.070627 yggdrasil_mc-0.2.4/yggdrasil_mc/utils.py
+-rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 yggdrasil_mc-0.2.4/PKG-INFO
```

### Comparing `yggdrasil_mc-0.2.3/LICENSE` & `yggdrasil_mc-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yggdrasil_mc-0.2.3/pyproject.toml` & `yggdrasil_mc-0.2.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yggdrasil-mc"
-version = "0.2.3"
+version = "0.2.4"
 description = "A simple Python lib to get player info and texture from Mojang and Yggdrasil APIs. / 一个简单的 Python 库，可从 Mojang 和 Yggdrasil APIs 获取玩家的信息和材质。"
 license = "AGPL-3.0-or-later"
 authors = ["SerinaNya <34389622+SerinaNya@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/SerinaNya/yggdrasil-mc"
 repository = "https://github.com/SerinaNya/yggdrasil-mc"
 keywords = ["yggdrasil", "mc", "api", "mcapi", "mojang", "minecraft", "littleskin", "blessing skin"]
@@ -36,12 +36,12 @@
 pytest = "^7.4.3"
 pytest-asyncio = "^0.21.1"
 
 
 [[tool.poetry.source]]
 name = "sjtu"
 url = "https://mirror.sjtu.edu.cn/pypi/web/simple"
-priority = "default"
+priority = "primary"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `yggdrasil_mc-0.2.3/yggdrasil_mc/models.py` & `yggdrasil_mc-0.2.4/yggdrasil_mc/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,52 @@
-from typing import Literal
+from typing import Literal, Annotated
 
-from pydantic import AliasPath, BaseModel, Field, HttpUrl
+from pydantic import AliasPath, BaseModel, Field, AnyHttpUrl
 
 
 class PlayerUuid(BaseModel):
-    id: str | None
-    name: str | None
+    id: str
+    name: str
 
     @property
     def existed(self) -> bool:
         """
         Returns a boolean value indicating whether the player is existed.
         """
         return self.id is not None
 
 
 class PlayerSkin_MetaData(BaseModel):
-    model: Literal["default", "slim"] = Field(default="default")
+    model: Literal["default", "slim"] = "default"
 
 
 class PlayerTexutureBase(BaseModel):
-    url: HttpUrl | None
+    url: AnyHttpUrl
 
     @property
     def hash(self) -> str | None:
         """
         Returns the hash part of the texture URL.
         """
         return str(self.url).split("/")[-1] if self.url else None
 
 
 class PlayerSkin(PlayerTexutureBase):
-    metadata: PlayerSkin_MetaData | None = Field(default_factory=PlayerSkin_MetaData)
+    metadata: Annotated[PlayerSkin_MetaData, Field(default_factory=PlayerSkin_MetaData)]
 
 
 class PlayerCape(PlayerTexutureBase):
     ...
 
 
 class PlayerProfile(BaseModel):
-    id: str = Field(..., validation_alias="profileId")
-    name: str =  Field(..., validation_alias="profileName")
-    skin: PlayerSkin | None = Field(default=None, validation_alias=AliasPath("textures", "SKIN"))
-    cape: PlayerCape | None = Field(default=None, validation_alias=AliasPath("textures", "CAPE"))
+    id: Annotated[str, Field(..., validation_alias="profileId")]
+    name: Annotated[str, Field(..., validation_alias="profileName")]
+
+    skin: Annotated[
+        PlayerSkin | None,
+        Field(default=None, validation_alias=AliasPath("textures", "SKIN")),
+    ]
+    cape: Annotated[
+        PlayerCape | None,
+        Field(default=None, validation_alias=AliasPath("textures", "CAPE")),
+    ]
```

### Comparing `yggdrasil_mc-0.2.3/PKG-INFO` & `yggdrasil_mc-0.2.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yggdrasil-mc
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple Python lib to get player info and texture from Mojang and Yggdrasil APIs. / 一个简单的 Python 库，可从 Mojang 和 Yggdrasil APIs 获取玩家的信息和材质。
 Home-page: https://github.com/SerinaNya/yggdrasil-mc
 License: AGPL-3.0-or-later
 Keywords: yggdrasil,mc,api,mcapi,mojang,minecraft,littleskin,blessing skin
 Author: SerinaNya
 Author-email: 34389622+SerinaNya@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
@@ -43,24 +43,33 @@
 <img src="https://img.shields.io/pypi/pyversions/yggdrasil-mc?style=flat-square" alt="PyPI - Python Version">
 <img src="https://img.shields.io/github/last-commit/SerinaNya/yggdrasil-mc/main?style=flat-square" alt="GitHub last commit (branch)">
 <img src="https://img.shields.io/github/license/SerinaNya/yggdrasil-mc?style=flat-square" alt="GitHub">
 
 </p>
 
 
-## Attention
+## ⚠️ Attention
 
-This package can be used with **Python 3.10+ ONLY**.
+This package can be used with **Python 3.10+**.
 
 ## Usage
 
 ``` shell
 pip3 install yggdrasil-mc
 ```
 
 ``` python
 from yggdrasil_mc.client import YggdrasilMC
 
 ygg = YggdrasilMC()
 await ygg.by_name_async("SerinaNya")
+
+# return PlayerProfile
+PlayerProfile(
+    id='8705a5560b7447e8ba869169c31fb5ef', 
+    name='SerinaNya', 
+    skin=PlayerSkin(
+        url=Url('http://textures.minecraft.net/texture/7781fa8ed3e2aa907944ec0f1ec391ad05955eb9c6424d911d409b00a69ea516'), 
+        metadata=PlayerSkin_MetaData(model='slim')), 
+    cape=None)
 ```
```

