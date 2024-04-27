# Comparing `tmp/qg_toolkit-1.0.6.tar.gz` & `tmp/qg_toolkit-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qg_toolkit-1.0.6.tar", max compression
+gzip compressed data, was "qg_toolkit-1.0.7.tar", max compression
```

## Comparing `qg_toolkit-1.0.6.tar` & `qg_toolkit-1.0.7.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0      778 2024-04-27 11:59:41.708134 qg_toolkit-1.0.6/pyproject.toml
--rw-r--r--   0        0        0       94 2024-04-27 10:53:56.731750 qg_toolkit-1.0.6/qg_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 18:53:34.039466 qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/__init__.py
--rw-r--r--   0        0        0       94 2024-04-27 10:54:32.432326 qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_fullpage/__init__.py
--rw-r--r--   0        0        0     5190 2024-04-24 18:53:34.040467 qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py
--rw-r--r--   0        0        0     5433 2024-04-24 18:53:34.040467 qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js
--rw-r--r--   0        0        0     2288 2024-04-27 11:00:05.704720 qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py
--rw-r--r--   0        0        0       94 2024-04-27 10:54:37.081886 qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_slide/__init__.py
--rw-r--r--   0        0        0     2723 2024-04-24 18:53:34.042468 qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_slide/gap.py
--rw-r--r--   0        0        0    35544 2024-04-26 20:18:37.986103 qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py
--rw-r--r--   0        0        0    51280 2024-04-24 18:53:34.044476 qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png
--rw-r--r--   0        0        0     4818 2024-04-24 18:53:34.045475 qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png
--rw-r--r--   0        0        0     9121 2024-04-24 18:53:34.045475 qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png
--rw-r--r--   0        0        0  1793853 2024-04-24 18:53:34.058465 qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json
--rw-r--r--   0        0        0     2362 2024-04-24 18:53:34.059468 qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js
--rw-r--r--   0        0        0     2349 2024-04-27 11:14:05.254088 qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_slide/mian.py
--rw-r--r--   0        0        0     1043 2024-04-24 18:53:34.060469 qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_slide/trace.py
--rw-r--r--   0        0        0       96 2024-04-27 10:54:21.799092 qg_toolkit-1.0.6/qg_toolkit/qtweepy/__init__.py
--rw-r--r--   0        0        0      103 2024-04-27 10:52:23.199431 qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/__init__.py
--rw-r--r--   0        0        0     4880 2024-04-27 10:52:23.276729 qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/account_checker.py
--rw-r--r--   0        0        0     2251 2024-04-27 10:52:23.208431 qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/follow_each_other.py
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.415935 qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/input-output/BAD_TOKEN.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/input-output/CONSENT_LOCKED.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/input-output/GOOD.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/input-output/LOCKED.txt
--rw-r--r--   0        0        0       46 2024-04-27 05:31:06.618786 qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/input-output/PROXIES.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/input-output/SUSPENDED.txt
--rw-r--r--   0        0        0       40 2024-04-27 05:31:12.415935 qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/input-output/UNKNOWN.txt
--rw-r--r--   0        0        0     3622 2024-04-27 10:52:23.284728 qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/mavia.py
--rw-r--r--   0        0        0     2373 2024-04-27 10:52:23.217431 qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/set_2fa.py
--rw-r--r--   0        0        0     3081 2024-04-27 10:52:23.184432 qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py
--rw-r--r--   0        0        0      697 2024-04-27 10:52:23.174431 qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/uploading_images.py
--rw-r--r--   0        0        0     2253 2024-04-27 10:52:23.159432 qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/voter.py
--rw-r--r--   0        0        0     3120 2024-04-27 10:52:23.191432 qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/xai.py
--rw-r--r--   0        0        0      687 2024-04-20 19:57:03.446998 qg_toolkit-1.0.6/qg_toolkit/qtweepy/pyproject.toml
--rw-r--r--   0        0        0     8720 2024-04-20 19:48:15.063903 qg_toolkit-1.0.6/qg_toolkit/qtweepy/README.md
--rw-r--r--   0        0        0      132 2024-04-24 18:22:26.184000 qg_toolkit-1.0.6/qg_toolkit/qtweepy/tea.yaml
--rw-r--r--   0        0        0      732 2024-04-20 19:48:15.068902 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/_capsolver/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/_capsolver/core/__init__.py
--rw-r--r--   0        0        0     8883 2024-04-20 19:48:15.070903 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py
--rw-r--r--   0        0        0     1054 2024-04-20 19:48:15.070903 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py
--rw-r--r--   0        0        0     1741 2024-04-20 19:48:15.071903 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py
--rw-r--r--   0        0        0     2602 2024-04-20 19:48:15.071903 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py
--rw-r--r--   0        0        0    10974 2024-04-20 19:48:15.072903 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py
--rw-r--r--   0        0        0     3248 2024-04-20 19:48:15.072903 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/account.py
--rw-r--r--   0        0        0      141 2024-04-20 19:48:15.072903 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/base/__init__.py
--rw-r--r--   0        0        0      500 2024-04-20 19:48:15.074292 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/base/client.py
--rw-r--r--   0        0        0     2175 2024-04-27 10:52:23.255728 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/base/session.py
--rw-r--r--   0        0        0    70738 2024-04-20 19:48:15.075686 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/client.py
--rw-r--r--   0        0        0      267 2024-04-20 19:48:15.076283 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/enums.py
--rw-r--r--   0        0        0     5322 2024-04-20 19:48:15.076811 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/errors.py
--rw-r--r--   0        0        0     4695 2024-04-20 19:48:15.076811 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/models.py
--rw-r--r--   0        0        0      665 2024-04-20 19:48:15.077920 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/utils/__init__.py
--rw-r--r--   0        0        0     1152 2024-04-20 19:48:15.077920 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/utils/file.py
--rw-r--r--   0        0        0     2140 2024-04-20 19:48:15.078463 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/utils/html.py
--rw-r--r--   0        0        0     1061 2024-04-20 19:48:15.078992 qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/utils/other.py
--rw-r--r--   0        0        0        0 2024-04-27 11:06:09.049630 qg_toolkit-1.0.6/qg_toolkit/test/test.py
--rw-r--r--   0        0        0       96 2024-04-27 10:54:04.685704 qg_toolkit-1.0.6/qg_toolkit/tools/__init__.py
--rw-r--r--   0        0        0      279 2024-04-24 18:54:00.529601 qg_toolkit-1.0.6/qg_toolkit/tools/demo.yaml
--rw-r--r--   0        0        0     5454 2024-04-27 10:53:33.237906 qg_toolkit-1.0.6/qg_toolkit/tools/qg_airdrop.py
--rw-r--r--   0        0        0      985 2024-04-20 20:27:34.147592 qg_toolkit-1.0.6/qg_toolkit/tools/qg_crypto.py
--rw-r--r--   0        0        0    35560 2024-04-27 10:55:26.247249 qg_toolkit-1.0.6/qg_toolkit/tools/qg_eth.py
--rw-r--r--   0        0        0     3594 2024-04-20 20:29:00.648873 qg_toolkit-1.0.6/qg_toolkit/tools/qg_file.py
--rw-r--r--   0        0        0      300 2024-04-24 18:53:34.062471 qg_toolkit-1.0.6/qg_toolkit/tools/qg_models.py
--rw-r--r--   0        0        0      741 2024-04-20 20:24:22.248041 qg_toolkit-1.0.6/qg_toolkit/tools/qg_random.py
--rw-r--r--   0        0        0     6135 2024-04-27 11:03:13.085956 qg_toolkit-1.0.6/qg_toolkit/tools/qg_solana.py
--rw-r--r--   0        0        0     2764 2024-04-24 18:21:31.477405 qg_toolkit-1.0.6/qg_toolkit/tools/qg_starknet.py
--rw-r--r--   0        0        0     3241 2024-04-20 19:48:15.080086 qg_toolkit-1.0.6/qg_toolkit/tools/qproxy.py
--rw-r--r--   0        0        0     6050 2024-04-20 21:14:04.319021 qg_toolkit-1.0.6/qg_toolkit/tools/rpc.py
--rw-r--r--   0        0        0       38 2024-04-20 19:50:56.436133 qg_toolkit-1.0.6/README.md
--rw-r--r--   0        0        0      132 2024-04-27 11:59:41.702131 qg_toolkit-1.0.6/tea.yaml
--rw-r--r--   0        0        0     1211 1970-01-01 00:00:00.000000 qg_toolkit-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      778 2024-04-27 12:04:27.972774 qg_toolkit-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-04-27 10:53:56.731750 qg_toolkit-1.0.7/qg_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 18:53:34.039466 qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-27 10:54:32.432326 qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_fullpage/__init__.py
+-rw-r--r--   0        0        0     5190 2024-04-24 18:53:34.040467 qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py
+-rw-r--r--   0        0        0     5433 2024-04-24 18:53:34.040467 qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js
+-rw-r--r--   0        0        0     2288 2024-04-27 11:00:05.704720 qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py
+-rw-r--r--   0        0        0       94 2024-04-27 10:54:37.081886 qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_slide/__init__.py
+-rw-r--r--   0        0        0     2723 2024-04-24 18:53:34.042468 qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_slide/gap.py
+-rw-r--r--   0        0        0    35544 2024-04-26 20:18:37.986103 qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py
+-rw-r--r--   0        0        0    51280 2024-04-24 18:53:34.044476 qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png
+-rw-r--r--   0        0        0     4818 2024-04-24 18:53:34.045475 qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png
+-rw-r--r--   0        0        0     9121 2024-04-24 18:53:34.045475 qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png
+-rw-r--r--   0        0        0  1793853 2024-04-24 18:53:34.058465 qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json
+-rw-r--r--   0        0        0     2362 2024-04-24 18:53:34.059468 qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js
+-rw-r--r--   0        0        0     2349 2024-04-27 11:14:05.254088 qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_slide/mian.py
+-rw-r--r--   0        0        0     1043 2024-04-24 18:53:34.060469 qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_slide/trace.py
+-rw-r--r--   0        0        0       96 2024-04-27 10:54:21.799092 qg_toolkit-1.0.7/qg_toolkit/qtweepy/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-27 10:52:23.199431 qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/__init__.py
+-rw-r--r--   0        0        0     4880 2024-04-27 10:52:23.276729 qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/account_checker.py
+-rw-r--r--   0        0        0     2251 2024-04-27 10:52:23.208431 qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/follow_each_other.py
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.415935 qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/input-output/BAD_TOKEN.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/input-output/CONSENT_LOCKED.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/input-output/GOOD.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/input-output/LOCKED.txt
+-rw-r--r--   0        0        0       46 2024-04-27 05:31:06.618786 qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/input-output/PROXIES.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/input-output/SUSPENDED.txt
+-rw-r--r--   0        0        0       40 2024-04-27 05:31:12.415935 qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/input-output/UNKNOWN.txt
+-rw-r--r--   0        0        0     3622 2024-04-27 10:52:23.284728 qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/mavia.py
+-rw-r--r--   0        0        0     2373 2024-04-27 10:52:23.217431 qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/set_2fa.py
+-rw-r--r--   0        0        0     3081 2024-04-27 10:52:23.184432 qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py
+-rw-r--r--   0        0        0      697 2024-04-27 10:52:23.174431 qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/uploading_images.py
+-rw-r--r--   0        0        0     2253 2024-04-27 10:52:23.159432 qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/voter.py
+-rw-r--r--   0        0        0     3120 2024-04-27 10:52:23.191432 qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/xai.py
+-rw-r--r--   0        0        0      687 2024-04-20 19:57:03.446998 qg_toolkit-1.0.7/qg_toolkit/qtweepy/pyproject.toml
+-rw-r--r--   0        0        0     8720 2024-04-20 19:48:15.063903 qg_toolkit-1.0.7/qg_toolkit/qtweepy/README.md
+-rw-r--r--   0        0        0      132 2024-04-24 18:22:26.184000 qg_toolkit-1.0.7/qg_toolkit/qtweepy/tea.yaml
+-rw-r--r--   0        0        0      732 2024-04-20 19:48:15.068902 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/_capsolver/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/_capsolver/core/__init__.py
+-rw-r--r--   0        0        0     8883 2024-04-20 19:48:15.070903 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py
+-rw-r--r--   0        0        0     1054 2024-04-20 19:48:15.070903 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py
+-rw-r--r--   0        0        0     1741 2024-04-20 19:48:15.071903 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py
+-rw-r--r--   0        0        0     2602 2024-04-20 19:48:15.071903 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py
+-rw-r--r--   0        0        0    10974 2024-04-20 19:48:15.072903 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py
+-rw-r--r--   0        0        0     3248 2024-04-20 19:48:15.072903 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/account.py
+-rw-r--r--   0        0        0      141 2024-04-20 19:48:15.072903 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/base/__init__.py
+-rw-r--r--   0        0        0      500 2024-04-20 19:48:15.074292 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/base/client.py
+-rw-r--r--   0        0        0     2175 2024-04-27 10:52:23.255728 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/base/session.py
+-rw-r--r--   0        0        0    70738 2024-04-20 19:48:15.075686 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/client.py
+-rw-r--r--   0        0        0      267 2024-04-20 19:48:15.076283 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/enums.py
+-rw-r--r--   0        0        0     5322 2024-04-20 19:48:15.076811 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/errors.py
+-rw-r--r--   0        0        0     4695 2024-04-20 19:48:15.076811 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/models.py
+-rw-r--r--   0        0        0      665 2024-04-20 19:48:15.077920 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/utils/__init__.py
+-rw-r--r--   0        0        0     1152 2024-04-20 19:48:15.077920 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/utils/file.py
+-rw-r--r--   0        0        0     2140 2024-04-20 19:48:15.078463 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/utils/html.py
+-rw-r--r--   0        0        0     1061 2024-04-20 19:48:15.078992 qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/utils/other.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:06:09.049630 qg_toolkit-1.0.7/qg_toolkit/test/test.py
+-rw-r--r--   0        0        0       96 2024-04-27 10:54:04.685704 qg_toolkit-1.0.7/qg_toolkit/tools/__init__.py
+-rw-r--r--   0        0        0      279 2024-04-24 18:54:00.529601 qg_toolkit-1.0.7/qg_toolkit/tools/demo.yaml
+-rw-r--r--   0        0        0     5454 2024-04-27 10:53:33.237906 qg_toolkit-1.0.7/qg_toolkit/tools/qg_airdrop.py
+-rw-r--r--   0        0        0      985 2024-04-20 20:27:34.147592 qg_toolkit-1.0.7/qg_toolkit/tools/qg_crypto.py
+-rw-r--r--   0        0        0    35560 2024-04-27 10:55:26.247249 qg_toolkit-1.0.7/qg_toolkit/tools/qg_eth.py
+-rw-r--r--   0        0        0     3594 2024-04-20 20:29:00.648873 qg_toolkit-1.0.7/qg_toolkit/tools/qg_file.py
+-rw-r--r--   0        0        0      300 2024-04-24 18:53:34.062471 qg_toolkit-1.0.7/qg_toolkit/tools/qg_models.py
+-rw-r--r--   0        0        0      741 2024-04-20 20:24:22.248041 qg_toolkit-1.0.7/qg_toolkit/tools/qg_random.py
+-rw-r--r--   0        0        0     6135 2024-04-27 11:03:13.085956 qg_toolkit-1.0.7/qg_toolkit/tools/qg_solana.py
+-rw-r--r--   0        0        0     2764 2024-04-24 18:21:31.477405 qg_toolkit-1.0.7/qg_toolkit/tools/qg_starknet.py
+-rw-r--r--   0        0        0     3241 2024-04-20 19:48:15.080086 qg_toolkit-1.0.7/qg_toolkit/tools/qproxy.py
+-rw-r--r--   0        0        0     6050 2024-04-20 21:14:04.319021 qg_toolkit-1.0.7/qg_toolkit/tools/rpc.py
+-rw-r--r--   0        0        0       38 2024-04-20 19:50:56.436133 qg_toolkit-1.0.7/README.md
+-rw-r--r--   0        0        0      132 2024-04-27 12:04:27.967776 qg_toolkit-1.0.7/tea.yaml
+-rw-r--r--   0        0        0     1211 1970-01-01 00:00:00.000000 qg_toolkit-1.0.7/PKG-INFO
```

### Comparing `qg_toolkit-1.0.6/pyproject.toml` & `qg_toolkit-1.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qg_toolkit"
-version = "1.0.6"
+version = "1.0.7"
 description = "qg_toolkit for Python!"
 authors = ["qg <qg@gmail.com>"]
 readme = "README.md"
 packages = [{include = "qg_toolkit"}]
 include = [{path = "tea.yaml"}]
 
 
@@ -17,20 +17,20 @@
 pyotp = "^2"
 yarl = "^1"
 aiohttp = "^3.9"
 tenacity = "^8"
 requests = "^2"
 loguru = "^0.7"
 solders= "^0.21.0"
+solana= "^0.34.0"
 retry= "^0.9.2"
 rsa= "^4.9"
 pycryptodome= "^3.20.0"
 pillow= "^10.3.0"
 ImageHash= "^4.3.1"
-solana= "^0.31.0"
 PyYAML= "^6.0.1"
 PySocks= "^1.7.1"
 websockets= "11.0.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24"
```

### Comparing `qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py` & `qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js` & `qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py` & `qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_slide/gap.py` & `qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_slide/gap.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py` & `qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png` & `qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png` & `qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png` & `qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json` & `qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js` & `qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_slide/mian.py` & `qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_slide/mian.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/geetest_captcha/geetest4_slide/trace.py` & `qg_toolkit-1.0.7/qg_toolkit/geetest_captcha/geetest4_slide/trace.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/account_checker.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/account_checker.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/follow_each_other.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/follow_each_other.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/mavia.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/mavia.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/set_2fa.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/set_2fa.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/uploading_images.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/uploading_images.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/voter.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/voter.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/examples/xai.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/examples/xai.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/pyproject.toml` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/README.md` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/README.md`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/__init__.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/account.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/account.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/base/session.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/base/session.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/client.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/client.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/errors.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/errors.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/models.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/models.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/utils/__init__.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/utils/file.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/utils/file.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/utils/html.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/utils/html.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/qtweepy/twitter/utils/other.py` & `qg_toolkit-1.0.7/qg_toolkit/qtweepy/twitter/utils/other.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/tools/qg_airdrop.py` & `qg_toolkit-1.0.7/qg_toolkit/tools/qg_airdrop.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/tools/qg_crypto.py` & `qg_toolkit-1.0.7/qg_toolkit/tools/qg_crypto.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/tools/qg_eth.py` & `qg_toolkit-1.0.7/qg_toolkit/tools/qg_eth.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/tools/qg_file.py` & `qg_toolkit-1.0.7/qg_toolkit/tools/qg_file.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/tools/qg_random.py` & `qg_toolkit-1.0.7/qg_toolkit/tools/qg_random.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/tools/qg_solana.py` & `qg_toolkit-1.0.7/qg_toolkit/tools/qg_solana.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/tools/qg_starknet.py` & `qg_toolkit-1.0.7/qg_toolkit/tools/qg_starknet.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/tools/qproxy.py` & `qg_toolkit-1.0.7/qg_toolkit/tools/qproxy.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/qg_toolkit/tools/rpc.py` & `qg_toolkit-1.0.7/qg_toolkit/tools/rpc.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.6/PKG-INFO` & `qg_toolkit-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qg_toolkit
-Version: 1.0.6
+Version: 1.0.7
 Summary: qg_toolkit for Python!
 Author: qg
 Author-email: qg@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -21,15 +21,15 @@
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: pycryptodome (>=3.20.0,<4.0.0)
 Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: pyotp (>=2,<3)
 Requires-Dist: requests (>=2,<3)
 Requires-Dist: retry (>=0.9.2,<0.10.0)
 Requires-Dist: rsa (>=4.9,<5.0)
-Requires-Dist: solana (>=0.31.0,<0.32.0)
+Requires-Dist: solana (>=0.34.0,<0.35.0)
 Requires-Dist: solders (>=0.21.0,<0.22.0)
 Requires-Dist: tenacity (>=8,<9)
 Requires-Dist: websockets (==11.0.3)
 Requires-Dist: yarl (>=1,<2)
 Description-Content-Type: text/markdown
 
 # QG_TOOLKIT
```

