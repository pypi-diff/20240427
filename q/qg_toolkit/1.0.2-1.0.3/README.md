# Comparing `tmp/qg_toolkit-1.0.2.tar.gz` & `tmp/qg_toolkit-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qg_toolkit-1.0.2.tar", max compression
+gzip compressed data, was "qg_toolkit-1.0.3.tar", max compression
```

## Comparing `qg_toolkit-1.0.2.tar` & `qg_toolkit-1.0.3.tar`

### file list

```diff
@@ -1,53 +1,73 @@
--rw-r--r--   0        0        0      602 2024-04-27 10:46:21.403031 qg_toolkit-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4871 2024-04-27 05:30:59.226522 qg_toolkit-1.0.2/qtweepy/examples/account_checker.py
--rw-r--r--   0        0        0     2210 2024-04-20 19:48:15.064902 qg_toolkit-1.0.2/qtweepy/examples/follow_each_other.py
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.415935 qg_toolkit-1.0.2/qtweepy/examples/input-output/BAD_TOKEN.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.2/qtweepy/examples/input-output/CONSENT_LOCKED.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.2/qtweepy/examples/input-output/GOOD.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.2/qtweepy/examples/input-output/LOCKED.txt
--rw-r--r--   0        0        0       46 2024-04-27 05:31:06.618786 qg_toolkit-1.0.2/qtweepy/examples/input-output/PROXIES.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.2/qtweepy/examples/input-output/SUSPENDED.txt
--rw-r--r--   0        0        0       40 2024-04-27 05:31:12.415935 qg_toolkit-1.0.2/qtweepy/examples/input-output/UNKNOWN.txt
--rw-r--r--   0        0        0     3581 2024-04-20 19:48:15.065903 qg_toolkit-1.0.2/qtweepy/examples/mavia.py
--rw-r--r--   0        0        0     2332 2024-04-20 19:48:15.066903 qg_toolkit-1.0.2/qtweepy/examples/set_2fa.py
--rw-r--r--   0        0        0     3040 2024-04-20 19:48:15.066903 qg_toolkit-1.0.2/qtweepy/examples/set_avatars_and_banners.py
--rw-r--r--   0        0        0      686 2024-04-20 19:48:15.066903 qg_toolkit-1.0.2/qtweepy/examples/uploading_images.py
--rw-r--r--   0        0        0     2212 2024-04-20 19:48:15.067902 qg_toolkit-1.0.2/qtweepy/examples/voter.py
--rw-r--r--   0        0        0     3079 2024-04-20 19:48:15.067902 qg_toolkit-1.0.2/qtweepy/examples/xai.py
--rw-r--r--   0        0        0      687 2024-04-20 19:57:03.446998 qg_toolkit-1.0.2/qtweepy/pyproject.toml
--rw-r--r--   0        0        0     8720 2024-04-20 19:48:15.063903 qg_toolkit-1.0.2/qtweepy/README.md
--rw-r--r--   0        0        0      132 2024-04-24 18:22:26.184000 qg_toolkit-1.0.2/qtweepy/tea.yaml
--rw-r--r--   0        0        0      732 2024-04-20 19:48:15.068902 qg_toolkit-1.0.2/qtweepy/twitter/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/core/__init__.py
--rw-r--r--   0        0        0     8883 2024-04-20 19:48:15.070903 qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/core/base.py
--rw-r--r--   0        0        0     1054 2024-04-20 19:48:15.070903 qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/core/config.py
--rw-r--r--   0        0        0     1741 2024-04-20 19:48:15.071903 qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/core/enum.py
--rw-r--r--   0        0        0     2602 2024-04-20 19:48:15.071903 qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/core/serializer.py
--rw-r--r--   0        0        0    10974 2024-04-20 19:48:15.072903 qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/fun_captcha.py
--rw-r--r--   0        0        0     3248 2024-04-20 19:48:15.072903 qg_toolkit-1.0.2/qtweepy/twitter/account.py
--rw-r--r--   0        0        0      141 2024-04-20 19:48:15.072903 qg_toolkit-1.0.2/qtweepy/twitter/base/__init__.py
--rw-r--r--   0        0        0      500 2024-04-20 19:48:15.074292 qg_toolkit-1.0.2/qtweepy/twitter/base/client.py
--rw-r--r--   0        0        0     2164 2024-04-20 19:48:15.074413 qg_toolkit-1.0.2/qtweepy/twitter/base/session.py
--rw-r--r--   0        0        0    70738 2024-04-20 19:48:15.075686 qg_toolkit-1.0.2/qtweepy/twitter/client.py
--rw-r--r--   0        0        0      267 2024-04-20 19:48:15.076283 qg_toolkit-1.0.2/qtweepy/twitter/enums.py
--rw-r--r--   0        0        0     5322 2024-04-20 19:48:15.076811 qg_toolkit-1.0.2/qtweepy/twitter/errors.py
--rw-r--r--   0        0        0     4695 2024-04-20 19:48:15.076811 qg_toolkit-1.0.2/qtweepy/twitter/models.py
--rw-r--r--   0        0        0      665 2024-04-20 19:48:15.077920 qg_toolkit-1.0.2/qtweepy/twitter/utils/__init__.py
--rw-r--r--   0        0        0     1152 2024-04-20 19:48:15.077920 qg_toolkit-1.0.2/qtweepy/twitter/utils/file.py
--rw-r--r--   0        0        0     2140 2024-04-20 19:48:15.078463 qg_toolkit-1.0.2/qtweepy/twitter/utils/html.py
--rw-r--r--   0        0        0     1061 2024-04-20 19:48:15.078992 qg_toolkit-1.0.2/qtweepy/twitter/utils/other.py
--rw-r--r--   0        0        0       38 2024-04-20 19:50:56.436133 qg_toolkit-1.0.2/README.md
--rw-r--r--   0        0        0      132 2024-04-27 10:46:21.398031 qg_toolkit-1.0.2/tea.yaml
--rw-r--r--   0        0        0      279 2024-04-24 18:54:00.529601 qg_toolkit-1.0.2/tools/demo.yaml
--rw-r--r--   0        0        0     5432 2024-04-26 20:14:27.357118 qg_toolkit-1.0.2/tools/qg_airdrop.py
--rw-r--r--   0        0        0      985 2024-04-20 20:27:34.147592 qg_toolkit-1.0.2/tools/qg_crypto.py
--rw-r--r--   0        0        0    35634 2024-04-26 20:13:35.014431 qg_toolkit-1.0.2/tools/qg_eth.py
--rw-r--r--   0        0        0     3594 2024-04-20 20:29:00.648873 qg_toolkit-1.0.2/tools/qg_file.py
--rw-r--r--   0        0        0      300 2024-04-24 18:53:34.062471 qg_toolkit-1.0.2/tools/qg_models.py
--rw-r--r--   0        0        0      741 2024-04-20 20:24:22.248041 qg_toolkit-1.0.2/tools/qg_random.py
--rw-r--r--   0        0        0     6143 2024-04-20 20:02:39.286618 qg_toolkit-1.0.2/tools/qg_solana.py
--rw-r--r--   0        0        0     2764 2024-04-24 18:21:31.477405 qg_toolkit-1.0.2/tools/qg_starknet.py
--rw-r--r--   0        0        0     3241 2024-04-20 19:48:15.080086 qg_toolkit-1.0.2/tools/qproxy.py
--rw-r--r--   0        0        0     6050 2024-04-20 21:14:04.319021 qg_toolkit-1.0.2/tools/rpc.py
--rw-r--r--   0        0        0      812 1970-01-01 00:00:00.000000 qg_toolkit-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      605 2024-04-27 11:05:18.150404 qg_toolkit-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-04-27 10:53:56.731750 qg_toolkit-1.0.3/qg_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 18:53:34.039466 qg_toolkit-1.0.3/qg_toolkit/gcaptcha4/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-27 10:54:32.432326 qg_toolkit-1.0.3/qg_toolkit/gcaptcha4/geetest4_fullpage/__init__.py
+-rw-r--r--   0        0        0     5190 2024-04-24 18:53:34.040467 qg_toolkit-1.0.3/qg_toolkit/gcaptcha4/geetest4_fullpage/geetest_v4.py
+-rw-r--r--   0        0        0     5433 2024-04-24 18:53:34.040467 qg_toolkit-1.0.3/qg_toolkit/gcaptcha4/geetest4_fullpage/jiyan.js
+-rw-r--r--   0        0        0     2288 2024-04-27 11:00:05.704720 qg_toolkit-1.0.3/qg_toolkit/gcaptcha4/geetest4_fullpage/mian.py
+-rw-r--r--   0        0        0       94 2024-04-27 10:54:37.081886 qg_toolkit-1.0.3/qg_toolkit/gcaptcha4/geetest4_slide/__init__.py
+-rw-r--r--   0        0        0     2723 2024-04-24 18:53:34.042468 qg_toolkit-1.0.3/qg_toolkit/gcaptcha4/geetest4_slide/gap.py
+-rw-r--r--   0        0        0    35544 2024-04-26 20:18:37.986103 qg_toolkit-1.0.3/qg_toolkit/gcaptcha4/geetest4_slide/geetest_slide_v4.py
+-rw-r--r--   0        0        0    51280 2024-04-24 18:53:34.044476 qg_toolkit-1.0.3/qg_toolkit/gcaptcha4/geetest4_slide/img/bg.png
+-rw-r--r--   0        0        0     4818 2024-04-24 18:53:34.045475 qg_toolkit-1.0.3/qg_toolkit/gcaptcha4/geetest4_slide/img/show_image.png
+-rw-r--r--   0        0        0     9121 2024-04-24 18:53:34.045475 qg_toolkit-1.0.3/qg_toolkit/gcaptcha4/geetest4_slide/img/slide.png
+-rw-r--r--   0        0        0  1793853 2024-04-24 18:53:34.058465 qg_toolkit-1.0.3/qg_toolkit/gcaptcha4/geetest4_slide/img/tracks.json
+-rw-r--r--   0        0        0     2362 2024-04-24 18:53:34.059468 qg_toolkit-1.0.3/qg_toolkit/gcaptcha4/geetest4_slide/jiyan.js
+-rw-r--r--   0        0        0     2343 2024-04-27 10:52:23.248729 qg_toolkit-1.0.3/qg_toolkit/gcaptcha4/geetest4_slide/mian.py
+-rw-r--r--   0        0        0     1043 2024-04-24 18:53:34.060469 qg_toolkit-1.0.3/qg_toolkit/gcaptcha4/geetest4_slide/trace.py
+-rw-r--r--   0        0        0       96 2024-04-27 10:54:21.799092 qg_toolkit-1.0.3/qg_toolkit/qtweepy/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-27 10:52:23.199431 qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/__init__.py
+-rw-r--r--   0        0        0     4880 2024-04-27 10:52:23.276729 qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/account_checker.py
+-rw-r--r--   0        0        0     2251 2024-04-27 10:52:23.208431 qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/follow_each_other.py
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.415935 qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/input-output/BAD_TOKEN.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/input-output/CONSENT_LOCKED.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/input-output/GOOD.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/input-output/LOCKED.txt
+-rw-r--r--   0        0        0       46 2024-04-27 05:31:06.618786 qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/input-output/PROXIES.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/input-output/SUSPENDED.txt
+-rw-r--r--   0        0        0       40 2024-04-27 05:31:12.415935 qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/input-output/UNKNOWN.txt
+-rw-r--r--   0        0        0     3622 2024-04-27 10:52:23.284728 qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/mavia.py
+-rw-r--r--   0        0        0     2373 2024-04-27 10:52:23.217431 qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/set_2fa.py
+-rw-r--r--   0        0        0     3081 2024-04-27 10:52:23.184432 qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py
+-rw-r--r--   0        0        0      697 2024-04-27 10:52:23.174431 qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/uploading_images.py
+-rw-r--r--   0        0        0     2253 2024-04-27 10:52:23.159432 qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/voter.py
+-rw-r--r--   0        0        0     3120 2024-04-27 10:52:23.191432 qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/xai.py
+-rw-r--r--   0        0        0      687 2024-04-20 19:57:03.446998 qg_toolkit-1.0.3/qg_toolkit/qtweepy/pyproject.toml
+-rw-r--r--   0        0        0     8720 2024-04-20 19:48:15.063903 qg_toolkit-1.0.3/qg_toolkit/qtweepy/README.md
+-rw-r--r--   0        0        0      132 2024-04-24 18:22:26.184000 qg_toolkit-1.0.3/qg_toolkit/qtweepy/tea.yaml
+-rw-r--r--   0        0        0      732 2024-04-20 19:48:15.068902 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/_capsolver/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/_capsolver/core/__init__.py
+-rw-r--r--   0        0        0     8883 2024-04-20 19:48:15.070903 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py
+-rw-r--r--   0        0        0     1054 2024-04-20 19:48:15.070903 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py
+-rw-r--r--   0        0        0     1741 2024-04-20 19:48:15.071903 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py
+-rw-r--r--   0        0        0     2602 2024-04-20 19:48:15.071903 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py
+-rw-r--r--   0        0        0    10974 2024-04-20 19:48:15.072903 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py
+-rw-r--r--   0        0        0     3248 2024-04-20 19:48:15.072903 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/account.py
+-rw-r--r--   0        0        0      141 2024-04-20 19:48:15.072903 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/base/__init__.py
+-rw-r--r--   0        0        0      500 2024-04-20 19:48:15.074292 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/base/client.py
+-rw-r--r--   0        0        0     2175 2024-04-27 10:52:23.255728 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/base/session.py
+-rw-r--r--   0        0        0    70738 2024-04-20 19:48:15.075686 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/client.py
+-rw-r--r--   0        0        0      267 2024-04-20 19:48:15.076283 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/enums.py
+-rw-r--r--   0        0        0     5322 2024-04-20 19:48:15.076811 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/errors.py
+-rw-r--r--   0        0        0     4695 2024-04-20 19:48:15.076811 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/models.py
+-rw-r--r--   0        0        0      665 2024-04-20 19:48:15.077920 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/utils/__init__.py
+-rw-r--r--   0        0        0     1152 2024-04-20 19:48:15.077920 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/utils/file.py
+-rw-r--r--   0        0        0     2140 2024-04-20 19:48:15.078463 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/utils/html.py
+-rw-r--r--   0        0        0     1061 2024-04-20 19:48:15.078992 qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/utils/other.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:06:09.049630 qg_toolkit-1.0.3/qg_toolkit/test/test.py
+-rw-r--r--   0        0        0       96 2024-04-27 10:54:04.685704 qg_toolkit-1.0.3/qg_toolkit/tools/__init__.py
+-rw-r--r--   0        0        0      279 2024-04-24 18:54:00.529601 qg_toolkit-1.0.3/qg_toolkit/tools/demo.yaml
+-rw-r--r--   0        0        0     5454 2024-04-27 10:53:33.237906 qg_toolkit-1.0.3/qg_toolkit/tools/qg_airdrop.py
+-rw-r--r--   0        0        0      985 2024-04-20 20:27:34.147592 qg_toolkit-1.0.3/qg_toolkit/tools/qg_crypto.py
+-rw-r--r--   0        0        0    35560 2024-04-27 10:55:26.247249 qg_toolkit-1.0.3/qg_toolkit/tools/qg_eth.py
+-rw-r--r--   0        0        0     3594 2024-04-20 20:29:00.648873 qg_toolkit-1.0.3/qg_toolkit/tools/qg_file.py
+-rw-r--r--   0        0        0      300 2024-04-24 18:53:34.062471 qg_toolkit-1.0.3/qg_toolkit/tools/qg_models.py
+-rw-r--r--   0        0        0      741 2024-04-20 20:24:22.248041 qg_toolkit-1.0.3/qg_toolkit/tools/qg_random.py
+-rw-r--r--   0        0        0     6135 2024-04-27 11:03:13.085956 qg_toolkit-1.0.3/qg_toolkit/tools/qg_solana.py
+-rw-r--r--   0        0        0     2764 2024-04-24 18:21:31.477405 qg_toolkit-1.0.3/qg_toolkit/tools/qg_starknet.py
+-rw-r--r--   0        0        0     3241 2024-04-20 19:48:15.080086 qg_toolkit-1.0.3/qg_toolkit/tools/qproxy.py
+-rw-r--r--   0        0        0     6050 2024-04-20 21:14:04.319021 qg_toolkit-1.0.3/qg_toolkit/tools/rpc.py
+-rw-r--r--   0        0        0       38 2024-04-20 19:50:56.436133 qg_toolkit-1.0.3/README.md
+-rw-r--r--   0        0        0      132 2024-04-27 11:06:18.892535 qg_toolkit-1.0.3/tea.yaml
+-rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 qg_toolkit-1.0.3/PKG-INFO
```

### Comparing `qg_toolkit-1.0.2/pyproject.toml` & `qg_toolkit-1.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "qg_toolkit"
-version = "1.0.2"
+version = "1.0.3"
 description = "qg_toolkit for Python!"
 authors = ["qg <qg@gmail.com>"]
 readme = "README.md"
-packages = [{include = "qtweepy"},{include = "tools"}]
+packages = [{include = "qg_toolkit"}]
 include = [{path = "tea.yaml"}]
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 curl_cffi = "0.6.2"
 beautifulsoup4 = "^4"
@@ -16,14 +16,15 @@
 lxml = "^5"
 pyotp = "^2"
 yarl = "^1"
 aiohttp = "^3.9"
 tenacity = "^8"
 requests = "^2"
 loguru = "^0.7"
+solders= "^0.21.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `qg_toolkit-1.0.2/qtweepy/examples/account_checker.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/account_checker.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 from pathlib import Path
 from typing import Iterable
 
 from loguru import logger
 
 from curl_cffi import requests
 
-from qtweepy.twitter import *
-from qtweepy.twitter.utils import load_lines, write_lines
-import qtweepy.twitter
-from tools.qproxy import Proxy
+from qg_toolkit.qtweepy.twitter import *
+from qg_toolkit.qtweepy.twitter.utils import load_lines, write_lines
+from qg_toolkit.tools.qproxy import Proxy
 
 LOGGING_LEVEL = "INFO"
 logger.enable("twitter")
 logger.remove()
 logger.add(sys.stderr, level=LOGGING_LEVEL)
```

### Comparing `qg_toolkit-1.0.2/qtweepy/examples/follow_each_other.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/follow_each_other.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 from itertools import cycle
 import asyncio
 from pathlib import Path
 import random
 
 import curl_cffi
-from qtweepy import twitter
-from tools.qproxy import Proxy
+from qg_toolkit.qtweepy import twitter
+from qg_toolkit.tools.qproxy import Proxy
 
 TWITTERS_TXT = Path("twitters.txt")
 PROXIES_TXT = Path("proxies.txt")
 
 for filepath in (
     TWITTERS_TXT,
     PROXIES_TXT,
 ):
     filepath.touch(exist_ok=True)
 
 
-TWITTER_ACCOUNTS = twitter.account.load_accounts_from_file(TWITTERS_TXT)
+TWITTER_ACCOUNTS = qg_toolkit.qtweepy.twitter.account.load_accounts_from_file(TWITTERS_TXT)
 PROXIES = Proxy.from_file(PROXIES_TXT)
 
 if not PROXIES:
     PROXIES = [None]
 
 CAPSOLVER_API_KEY = None  # 用于自动解锁
 MAX_FOLLOWERS = 10
```

### Comparing `qg_toolkit-1.0.2/qtweepy/examples/mavia.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/mavia.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from itertools import cycle
 import asyncio
 from pathlib import Path
 
 import curl_cffi
-from qtweepy import twitter
-from tools.qproxy import Proxy
+from qg_toolkit.qtweepy import twitter
+from qg_toolkit.tools.qproxy import Proxy
 
 TWITTERS_TXT = Path("twitters.txt")
 PROXIES_TXT = Path("proxies.txt")
 RESULTS_TXT = Path("results.txt")
 DYM_MESSAGES_TXT = Path("dym_messages.txt")
 MAVIA_MESSAGES_TXT = Path("mavia_messages.txt")
 
@@ -22,15 +22,15 @@
     filepath.touch(exist_ok=True)
 
 SCREENSHOTS_DIR = Path("screenshots")
 
 for dirpath in (SCREENSHOTS_DIR,):
     dirpath.mkdir(exist_ok=True)
 
-TWITTER_ACCOUNTS = twitter.account.load_accounts_from_file(TWITTERS_TXT)
+TWITTER_ACCOUNTS = qg_toolkit.qtweepy.twitter.account.load_accounts_from_file(TWITTERS_TXT)
 PROXIES = Proxy.from_file(PROXIES_TXT)
 
 if not PROXIES:
     PROXIES = [None]
 
 QUOT_MAVIA_TWEET_URL = "https://twitter.com/Bybit_Official/status/1754416124207181938"
 QUOT_DYM_TWEET_URL = "https://twitter.com/Bybit_Official/status/1760246614252286288"
```

### Comparing `qg_toolkit-1.0.2/qtweepy/examples/set_2fa.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/set_2fa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from itertools import cycle
 import asyncio
 from pathlib import Path
 from typing import Optional
 
-from qtweepy import twitter
-from tools.qproxy import Proxy
+from qg_toolkit.qtweepy import twitter
+from qg_toolkit.tools.qproxy import Proxy
 
 TWITTERS_TXT = Path("twitters.txt")
 PROXIES_TXT = Path("proxies.txt")
 RESULTS_TXT = Path("results.txt")
 
 for filepath in (TWITTERS_TXT, PROXIES_TXT, RESULTS_TXT):
     filepath.touch(exist_ok=True)
 
 FIELDS = ("auth_token", "username", "password")
-TWITTER_ACCOUNTS = twitter.account.load_accounts_from_file(TWITTERS_TXT, fields=FIELDS)
+TWITTER_ACCOUNTS = qg_toolkit.qtweepy.twitter.account.load_accounts_from_file(TWITTERS_TXT, fields=FIELDS)
 PROXIES = Proxy.from_file(PROXIES_TXT)
 
 if not PROXIES:
     PROXIES = [None]
 
 semaphore = asyncio.Semaphore(10)  # 限制同时执行 10 个任务
```

### Comparing `qg_toolkit-1.0.2/qtweepy/examples/set_avatars_and_banners.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from itertools import cycle
 import asyncio
 from pathlib import Path
 from typing import Optional
 
-from tools.qproxy import Proxy
-from qtweepy import twitter
+from qg_toolkit.tools.qproxy import Proxy
+from qg_toolkit.qtweepy import twitter
 
 TWITTERS_TXT = Path("twitters.txt")
 PROXIES_TXT = Path("proxies.txt")
 
 for filepath in (TWITTERS_TXT, PROXIES_TXT):
     filepath.touch(exist_ok=True)
 
 AVATARS_DIR = Path("avatars")
 BANNERS_DIR = Path("banners")
 
 for dirpath in (AVATARS_DIR, BANNERS_DIR):
     dirpath.mkdir(exist_ok=True)
 
-TWITTER_ACCOUNTS = twitter.account.load_accounts_from_file(TWITTERS_TXT)
+TWITTER_ACCOUNTS = qg_toolkit.qtweepy.twitter.account.load_accounts_from_file(TWITTERS_TXT)
 PROXIES = Proxy.from_file(PROXIES_TXT)
 
 if not PROXIES:
     PROXIES = [None]
 
 semaphore = asyncio.Semaphore(10)  # 最多同时执行 10 个任务
```

### Comparing `qg_toolkit-1.0.2/qtweepy/examples/uploading_images.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/uploading_images.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncio
-from qtweepy import twitter
+from qg_toolkit.qtweepy import twitter
 
 ACCOUNT = twitter.Account(auth_token="auth_token")
 IMAGE = open(f"image.png", "rb").read()
 
 
 async def update_profile_images(account: twitter.Account, image: bytes):
     async with twitter.Client(account) as twitter_client:
```

### Comparing `qg_toolkit-1.0.2/qtweepy/examples/voter.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/voter.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 """
 
 import asyncio
 from itertools import cycle
 from pathlib import Path
 from typing import Iterable
 
-from qtweepy import twitter
-from tools.qproxy import Proxy
+from qg_toolkit.qtweepy import twitter
+from qg_toolkit.tools.qproxy import Proxy
 
 TwitterAccountWithAdditionalData = tuple[str, twitter.Account]
 SortedAccounts = dict[twitter.AccountStatus: TwitterAccountWithAdditionalData]
 
 INPUT_OUTPUT_DIR = Path("input-output")
 INPUT_OUTPUT_DIR.mkdir(exist_ok=True)
 
@@ -54,15 +54,15 @@
 if __name__ == '__main__':
     proxies = Proxy.from_file(PROXIES_TXT)
     print(f"代理数量：{len(proxies)}")
     if not proxies:
         print(f"(可选) 在任何格式中添加代理 "
               f"\n\t到文件 {PROXIES_TXT}")
 
-    accounts = twitter.account.load_accounts_from_file(ACCOUNTS_TXT)
+    accounts = qg_toolkit.qtweepy.twitter.account.load_accounts_from_file(ACCOUNTS_TXT)
     if not accounts:
         print(f"以 {SEPARATOR.join(FIELDS)} 格式添加帐户"
               f" (auth_token 为必填项，其他为可选项)"
               f"\n\t到文件 {ACCOUNTS_TXT}")
         quit()
 
     asyncio.run(vote(proxies, accounts, TWEET_ID, CARD_ID, CHOICE_NUMBER))
```

### Comparing `qg_toolkit-1.0.2/qtweepy/examples/xai.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/examples/xai.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 """
 
 from itertools import cycle
 import asyncio
 from pathlib import Path
 
 import curl_cffi
-from qtweepy import twitter
-from tools.qproxy import Proxy
+from qg_toolkit.qtweepy import twitter
+from qg_toolkit.tools.qproxy import Proxy
 
 TWITTERS_TXT = Path("twitters.txt")
 PROXIES_TXT = Path("proxies.txt")
 RESULTS_TXT = Path("results.txt")
 XAI_MESSAGES_TXT = Path("xai_messages.txt")
 
 for filepath in (
@@ -20,15 +20,15 @@
     PROXIES_TXT,
     RESULTS_TXT,
     XAI_MESSAGES_TXT,
 ):
     filepath.touch(exist_ok=True)
 
 
-TWITTER_ACCOUNTS = twitter.account.load_accounts_from_file(TWITTERS_TXT)
+TWITTER_ACCOUNTS = qg_toolkit.qtweepy.twitter.account.load_accounts_from_file(TWITTERS_TXT)
 PROXIES = Proxy.from_file(PROXIES_TXT)
 
 if not PROXIES:
     PROXIES = [None]
 
 QUOT_TWEET_URL = "https://twitter.com/Bybit_Official/status/1767120261961097328"
 USER_IDS_TO_FOLLOW = [
```

### Comparing `qg_toolkit-1.0.2/qtweepy/pyproject.toml` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/qtweepy/README.md` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/README.md`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/qtweepy/twitter/__init__.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/core/base.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/core/config.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/core/enum.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/core/serializer.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/qtweepy/twitter/_capsolver/fun_captcha.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/qtweepy/twitter/account.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/account.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/qtweepy/twitter/base/session.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/base/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Union
 
 from curl_cffi import requests
 
-from tools.qproxy import Proxy
+from qg_toolkit.tools.qproxy import Proxy
 
 
 # from better_proxy import Proxy
 
 
 class BaseAsyncSession(requests.AsyncSession):
     """
```

### Comparing `qg_toolkit-1.0.2/qtweepy/twitter/client.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/client.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/qtweepy/twitter/errors.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/errors.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/qtweepy/twitter/models.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/models.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/qtweepy/twitter/utils/__init__.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/qtweepy/twitter/utils/file.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/utils/file.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/qtweepy/twitter/utils/html.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/utils/html.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/qtweepy/twitter/utils/other.py` & `qg_toolkit-1.0.3/qg_toolkit/qtweepy/twitter/utils/other.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/tools/qg_airdrop.py` & `qg_toolkit-1.0.3/qg_toolkit/tools/qg_airdrop.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import concurrent.futures
 import copy
 from threading import Lock
 
 from web3 import Web3
 
-from tools.qg_eth import QGEth
-from tools.qg_file import QGFile
+from qg_toolkit.tools.qg_eth import QGEth
+from qg_toolkit.tools.qg_file import QGFile
 
 
 class QGAirDrop(QGEth):
     lock = Lock()
 
     def __init__(self, chain_name=None, per_value=None, left_value=None, is_check_receiver=False, check_balance=0.0000001, receiver_accounts=[], **kwargs):
         super().__init__(**kwargs)
```

### Comparing `qg_toolkit-1.0.2/tools/qg_crypto.py` & `qg_toolkit-1.0.3/qg_toolkit/tools/qg_crypto.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/tools/qg_eth.py` & `qg_toolkit-1.0.3/qg_toolkit/tools/qg_eth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import base64
 import binascii
 import inspect
 import random
-from dataclasses import dataclass, field
 from decimal import Decimal
 from pathlib import Path
-from typing import Union, Dict
 
 import requests
 from eth_account import Account
 from eth_account.messages import encode_defunct, encode_typed_data
 from retry import retry
 from web3 import Web3
 from web3.auto import w3
```

### Comparing `qg_toolkit-1.0.2/tools/qg_file.py` & `qg_toolkit-1.0.3/qg_toolkit/tools/qg_file.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/tools/qg_random.py` & `qg_toolkit-1.0.3/qg_toolkit/tools/qg_random.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/tools/qg_solana.py` & `qg_toolkit-1.0.3/qg_toolkit/tools/qg_solana.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import base64
 import concurrent
 import struct
 from threading import Lock
 
-import requests
 from solana.rpc.api import Client
 from solana.rpc.commitment import Commitment
 from solana.transaction import Transaction
 from solders.instruction import AccountMeta, Instruction
 from solders.keypair import Keypair
 from solders.pubkey import Pubkey
-
-from tools.qg_util import QGUtil
+from qg_toolkit.tools.qg_file import QGFile
 
 
 class QGSolana:
     # rpc
     endpoints = {
         "mainnet": "https://mainnet.infura.io/v3/257c5f3bdfed414b88a4908b0f999377",
         "mainnet2": "https://api.mainnet-beta.solana.com",
@@ -118,27 +116,27 @@
 
     @staticmethod
     def generate_wallet(num):
         for i in range(num):
             keypair = Keypair()
             log = f'{keypair.pubkey()}----{keypair}----{keypair.to_bytes_array()}'
             print(log)
-            QGUtil.save_to_file('kun_sol-100.txt', log)
+            QGFile.save_to_file('kun_sol-100.txt', log)
 
 
 def qg_task(index, addr, pk, mn):
     qg = QGSolana(index=index, address=addr, private_key=pk)
     qg.batch_transfer(recept_accounts, 0.1, is_check=True, check_balance=0.01)
 
 
 
 if __name__ == '__main__':
     arr = []
-    accounts = QGUtil.txt_to_array("../wallets/solana/qg-solana.txt")
-    recept_accounts = [x[0] for x in QGUtil.txt_to_array("../wallets/solana/qg_sol-100.txt")][0:9]
+    accounts = QGFile.txt_to_array("../wallets/solana/qg-solana.txt")
+    recept_accounts = [x[0] for x in QGFile.txt_to_array("../wallets/solana/qg_sol-100.txt")][0:9]
     executor = concurrent.futures.ThreadPoolExecutor(max_workers=2)
     results = []
     for i, account in enumerate(accounts, start=1):
         addr1 = account[0]
         pk1 = ""
         mn1 = ""
         email1 = ""
```

### Comparing `qg_toolkit-1.0.2/tools/qg_starknet.py` & `qg_toolkit-1.0.3/qg_toolkit/tools/qg_starknet.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/tools/qproxy.py` & `qg_toolkit-1.0.3/qg_toolkit/tools/qproxy.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/tools/rpc.py` & `qg_toolkit-1.0.3/qg_toolkit/tools/rpc.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.2/PKG-INFO` & `qg_toolkit-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qg_toolkit
-Version: 1.0.2
+Version: 1.0.3
 Summary: qg_toolkit for Python!
 Author: qg
 Author-email: qg@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,14 +14,15 @@
 Requires-Dist: beautifulsoup4 (>=4,<5)
 Requires-Dist: curl_cffi (==0.6.2)
 Requires-Dist: loguru (>=0.7,<0.8)
 Requires-Dist: lxml (>=5,<6)
 Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: pyotp (>=2,<3)
 Requires-Dist: requests (>=2,<3)
+Requires-Dist: solders (>=0.21.0,<0.22.0)
 Requires-Dist: tenacity (>=8,<9)
 Requires-Dist: yarl (>=1,<2)
 Description-Content-Type: text/markdown
 
 # QG_TOOLKIT
 
 some tool in Python.
```

