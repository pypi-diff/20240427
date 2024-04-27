# Comparing `tmp/clovers_setu_collection-0.1.0.tar.gz` & `tmp/clovers_setu_collection-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers_setu_collection-0.1.0.tar", max compression
+gzip compressed data, was "clovers_setu_collection-0.1.1.tar", max compression
```

## Comparing `clovers_setu_collection-0.1.0.tar` & `clovers_setu_collection-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     5994 2024-04-26 10:07:42.530728 clovers_setu_collection-0.1.0/clovers_setu_collection/__init__.py
--rw-r--r--   0        0        0      698 2024-04-26 09:08:10.615761 clovers_setu_collection-0.1.0/clovers_setu_collection/api/Anosu.py
--rw-r--r--   0        0        0      601 2024-04-26 09:53:37.735616 clovers_setu_collection-0.1.0/clovers_setu_collection/api/Lolicon.py
--rw-r--r--   0        0        0     1300 2024-04-26 09:48:03.121270 clovers_setu_collection-0.1.0/clovers_setu_collection/api/MirlKoi.py
--rw-r--r--   0        0        0      380 2024-04-26 09:54:30.161563 clovers_setu_collection-0.1.0/clovers_setu_collection/config.py
--rw-r--r--   0        0        0     1154 2024-04-26 09:08:10.616761 clovers_setu_collection-0.1.0/clovers_setu_collection/setu_api.py
--rw-r--r--   0        0        0      362 2024-04-26 10:35:16.973478 clovers_setu_collection-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1218 2024-04-26 10:13:09.093611 clovers_setu_collection-0.1.0/README.md
--rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 clovers_setu_collection-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5994 2024-04-27 16:02:34.886118 clovers_setu_collection-0.1.1/clovers_setu_collection/__init__.py
+-rw-r--r--   0        0        0      698 2024-04-27 15:14:36.617849 clovers_setu_collection-0.1.1/clovers_setu_collection/api/Anosu.py
+-rw-r--r--   0        0        0      601 2024-04-27 15:14:36.617849 clovers_setu_collection-0.1.1/clovers_setu_collection/api/Lolicon.py
+-rw-r--r--   0        0        0     1300 2024-04-27 15:14:36.618349 clovers_setu_collection-0.1.1/clovers_setu_collection/api/MirlKoi.py
+-rw-r--r--   0        0        0      380 2024-04-27 15:14:36.618349 clovers_setu_collection-0.1.1/clovers_setu_collection/config.py
+-rw-r--r--   0        0        0     1154 2024-04-27 15:14:36.618849 clovers_setu_collection-0.1.1/clovers_setu_collection/setu_api.py
+-rw-r--r--   0        0        0      362 2024-04-27 16:02:51.430791 clovers_setu_collection-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1798 2024-04-27 16:07:40.620120 clovers_setu_collection-0.1.1/README.md
+-rw-r--r--   0        0        0     2071 1970-01-01 00:00:00.000000 clovers_setu_collection-0.1.1/PKG-INFO
```

### Comparing `clovers_setu_collection-0.1.0/clovers_setu_collection/__init__.py` & `clovers_setu_collection-0.1.1/clovers_setu_collection/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
 apiname_dict = {"1": "Jitsu/MirlKoi API", "2": "Lolicon API"}
 api_dict = {"2": Lolicon_api}
 plugin = Plugin()
 
 
-@plugin.handle({"涩图，色图"}, ["to_me"])
+@plugin.handle({"涩图","色图"}, ["to_me"])
 async def _(event: Event):
     if not event.kwargs["to_me"]:
         return
     msg = (
         "发送【来一张xx涩图】可获得一张随机色图。"
         "群聊图片取自：\n"
         "Jitsu：https://image.anosu.top/\n"
```

### Comparing `clovers_setu_collection-0.1.0/clovers_setu_collection/api/Anosu.py` & `clovers_setu_collection-0.1.1/clovers_setu_collection/api/Anosu.py`

 * *Files identical despite different names*

### Comparing `clovers_setu_collection-0.1.0/clovers_setu_collection/api/Lolicon.py` & `clovers_setu_collection-0.1.1/clovers_setu_collection/api/Lolicon.py`

 * *Files identical despite different names*

### Comparing `clovers_setu_collection-0.1.0/clovers_setu_collection/api/MirlKoi.py` & `clovers_setu_collection-0.1.1/clovers_setu_collection/api/MirlKoi.py`

 * *Files identical despite different names*

### Comparing `clovers_setu_collection-0.1.0/clovers_setu_collection/setu_api.py` & `clovers_setu_collection-0.1.1/clovers_setu_collection/setu_api.py`

 * *Files identical despite different names*

### Comparing `clovers_setu_collection-0.1.0/README.md` & `clovers_setu_collection-0.1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,77 +1,113 @@
 00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
 00000010: 6572 223e 0d0a 0d0a 2320 636c 6f76 6572  er">....# clover
 00000020: 732d 7365 7475 2d63 6f6c 6c65 6374 696f  s-setu-collectio
-00000030: 6e0d 0a0d 0a3c 2f64 6976 3e0d 0a0d 0ae4  n....</div>.....
-00000040: bdbf e794 a8e7 9a84 2041 5049 3a0d 0a0d  ........ API:...
-00000050: 0a5b 4a69 7473 755d 2868 7474 7073 3a2f  .[Jitsu](https:/
-00000060: 2f69 6d61 6765 2e61 6e6f 7375 2e74 6f70  /image.anosu.top
-00000070: 2f29 20e7 ae80 e58d 95e5 a5bd e794 a8e7  /) .............
-00000080: 9a84 e889 b2e5 9bbe 2061 7069 0d0a 0d0a  ........ api....
-00000090: 5b4d 6972 6c4b 6f69 2041 5049 5d28 6874  [MirlKoi API](ht
-000000a0: 7470 733a 2f2f 6977 3233 332e 636e 2f29  tps://iw233.cn/)
-000000b0: 20e5 8faf e4bb a5e9 81bf e585 8d20 626f   ............ bo
-000000c0: 7420 e8a2 abe5 b081 e79a 84e8 b685 e5ae  t ..............
-000000d0: 89e5 85a8 efbc 88e4 bf9d e8af 81e5 a5bd  ................
-000000e0: e79c 8be4 bd86 e698 afe4 b88d e680 8ee4  ................
-000000f0: b988 e6b6 a9ef bc89 e889 b2e5 9bbe 2061  .............. a
-00000100: 7069 0d0a 0d0a 5b4c 6f6c 6963 6f6e 2041  pi....[Lolicon A
-00000110: 5049 5d28 6874 7470 733a 2f2f 6170 692e  PI](https://api.
-00000120: 6c6f 6c69 636f 6e2e 6170 702f 2920 e4bd  lolicon.app/) ..
-00000130: bfe7 94a8 e8bf 99e4 b8aa e79a 84e6 97b6  ................
-00000140: e580 99e8 afb7 e6b3 a8e6 848f e8ba abe4  ................
-00000150: bd93 0d0a 0d0a 2323 20f0 9f92 bf20 e5ae  ......## .... ..
-00000160: 89e8 a385 0d0a 0d0a 6060 6062 6173 680d  ........```bash.
-00000170: 0a70 6970 2069 6e73 7461 6c6c 2063 6c6f  .pip install clo
-00000180: 7665 7273 2d73 6574 752d 636f 6c6c 6563  vers-setu-collec
-00000190: 7469 6f6e 0d0a 6060 600d 0a0d 0a23 2320  tion..```....## 
-000001a0: e29a 99ef b88f 20e9 858d e7bd ae0d 0a0d  ...... .........
-000001b0: 0a60 6060 746f 6d6c 0d0a 5b63 6c6f 7665  .```toml..[clove
-000001c0: 7273 5f73 6574 755f 636f 6c6c 6563 7469  rs_setu_collecti
-000001d0: 6f6e 5d0d 0a23 20e6 98af e590 a6e4 bf9d  on]..# .........
-000001e0: e5ad 98e4 bb8e 6170 69e8 8eb7 e58f 96e7  ......api.......
-000001f0: 9a84 e59b bee7 8987 0d0a 7361 7665 5f69  ..........save_i
-00000200: 6d61 6765 203d 2074 7275 650d 0a23 20e4  mage = true..# .
-00000210: b8bb e8b7 afe5 be84 0d0a 7061 7468 203d  ..........path =
-00000220: 2022 6461 7461 5c5c 7365 7475 5f63 6f6c   "data\\setu_col
-00000230: 6c65 6374 696f 6e22 0d0a 2320 e7a7 81e8  lection"..# ....
-00000240: 818a e59b bee7 8987 e999 90e5 88b6 0d0a  ................
-00000250: 7072 6976 6174 655f 7365 7475 5f6c 696d  private_setu_lim
-00000260: 6974 203d 2066 616c 7365 0d0a 2320 e7be  it = false..# ..
-00000270: a4e8 818a e59b bee7 8987 e999 90e5 88b6  ................
-00000280: efbc 88e5 88ab e585 b3ef bc89 0d0a 7075  ..............pu
-00000290: 626c 6963 5f73 6574 755f 6c69 6d69 7420  blic_setu_limit 
-000002a0: 3d20 7472 7565 0d0a 6060 600d 0a0d 0a23  = true..```....#
-000002b0: 2320 f09f 8e89 20e4 bb8b e7bb 8d0d 0a0d  # .... .........
-000002c0: 0a2a 2ae6 8c87 e4bb a42a 2aef bc9a 60e6  .**......**...`.
-000002d0: 9da5 4ee5 bca0 7878 e889 b2e5 9bbe 6020  ..N...xx......` 
-000002e0: 60e6 9da5 4ee5 bca0 7878 6020 60e6 9da5  `...N...xx` `...
-000002f0: 4ee5 bca0 7231 3878 78e8 89b2 e59b be60  N...r18xx......`
-00000300: 0d0a 0d0a 2a2a e68c 87e4 bba4 efbc 88e4  ....**..........
-00000310: bb85 e7a7 81e8 818a efbc 892a 2aef bc9a  ...........**...
-00000320: e588 87e6 8da2 2061 7069 0d0a 0d0a e58d  ...... api......
-00000330: 95e6 aca1 e69c 80e5 a49a e58f 91e9 8081  ................
-00000340: 2035 20e5 bca0 e889 b2e5 9bbe 0d0a 0d0a   5 .............
-00000350: e7be a4e8 818a e694 afe6 8c81 e58d 95e4  ................
-00000360: b8aa 2074 6167 efbc 8ce7 a781 e881 8ae6  .. tag..........
-00000370: 94af e68c 8120 3320 e4b8 aa20 7461 67ef  ..... 3 ... tag.
-00000380: bc88 e59b a0e4 b8ba e7a7 81e8 818a e794  ................
-00000390: a820 4c6f 6c69 636f 6eef bc89 efbc 8ce7  . Lolicon.......
-000003a0: 94a8 e7a9 bae6 a0bc e99a 94e5 bc80 e380  ................
-000003b0: 820d 0a0d 0a23 2320 f09f 939e 20e8 8194  .....## .... ...
-000003c0: e7b3 bb0d 0a0d 0ae5 a682 e69c 89e5 bbba  ................
-000003d0: e8ae aeef bc8c 6275 6720 e58f 8de9 a688  ......bug ......
-000003e0: e7ad 89e5 8faf e4bb a5e5 8aa0 e7be a40d  ................
-000003f0: 0a0d 0ae6 9cba e599 a8e4 baba 2062 7567  ............ bug
-00000400: 20e7 a094 e7a9 b6e4 b8ad e5bf 83ef bc88   ...............
-00000410: e997 b2e8 818a e7be a4ef bc89 2037 3434  ............ 744
-00000420: 3735 3131 3739 0d0a 0d0a e6b0 b8e6 8192  751179..........
-00000430: e4b9 8be5 9f8e efbc 88e6 b58b e8af 95e7  ................
-00000440: bea4 efbc 8920 3732 3430 3234 3831 300d  ..... 724024810.
-00000450: 0a0d 0a21 5be7 bea4 e58f b75d 2868 7474  ...![......](htt
-00000460: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000470: 636c 6f76 6572 732d 7072 6f6a 6563 742f  clovers-project/
-00000480: 636c 6f76 6572 732f 626c 6f62 2f6d 6173  clovers/blob/mas
-00000490: 7465 722f 2545 3925 3939 2538 3425 4534  ter/%E9%99%84%E4
-000004a0: 2542 4225 4236 2f71 7263 6f64 655f 3136  %BB%B6/qrcode_16
-000004b0: 3736 3533 3837 3432 3232 312e 6a70 6729  76538742221.jpg)
-000004c0: 0d0a                                     ..
+00000030: 6e0d 0a0d 0a5f e29c a820 e4bb 8ee5 a49a  n...._... ......
+00000040: e4b8 aa20 6170 6920 e88e b7e5 8f96 e889  ... api ........
+00000050: b2e5 9bbe e5b9 b6e6 a0b9 e68d aee5 9cba  ................
+00000060: e699 afe6 95b4 e590 88e7 9a84 e889 b2e5  ................
+00000070: 9bbe e68f 92e4 bbb6 20e2 9ca8 5f0d 0a0d  ........ ..._...
+00000080: 0a3c 696d 6720 7372 633d 2268 7474 7073  .<img src="https
+00000090: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000000a0: 6f2f 6261 6467 652f 7079 7468 6f6e 2d33  o/badge/python-3
+000000b0: 2e31 322b 2d62 6c75 652e 7376 6722 2061  .12+-blue.svg" a
+000000c0: 6c74 3d22 7079 7468 6f6e 223e 0d0a 3c61  lt="python">..<a
+000000d0: 2068 7265 663d 222e 2f4c 4943 454e 5345   href="./LICENSE
+000000e0: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+000000f0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000100: 696f 2f67 6974 6875 622f 6c69 6365 6e73  io/github/licens
+00000110: 652f 4b61 7269 7341 7961 2f63 6c6f 7665  e/KarisAya/clove
+00000120: 7273 5f73 6574 755f 636f 6c6c 6563 7469  rs_setu_collecti
+00000130: 6f6e 2e73 7667 2220 616c 743d 226c 6963  on.svg" alt="lic
+00000140: 656e 7365 223e 3c2f 613e 0d0a 3c61 2068  ense"></a>..<a h
+00000150: 7265 663d 2268 7474 7073 3a2f 2f70 7970  ref="https://pyp
+00000160: 692e 7079 7468 6f6e 2e6f 7267 2f70 7970  i.python.org/pyp
+00000170: 692f 636c 6f76 6572 735f 7365 7475 5f63  i/clovers_setu_c
+00000180: 6f6c 6c65 6374 696f 6e22 3e3c 696d 6720  ollection"><img 
+00000190: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+000001a0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+000001b0: 2f76 2f63 6c6f 7665 7273 5f73 6574 755f  /v/clovers_setu_
+000001c0: 636f 6c6c 6563 7469 6f6e 2e73 7667 2220  collection.svg" 
+000001d0: 616c 743d 2270 7970 6922 3e3c 2f61 3e0d  alt="pypi"></a>.
+000001e0: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+000001f0: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
+00000200: 672f 7079 7069 2f63 6c6f 7665 7273 5f73  g/pypi/clovers_s
+00000210: 6574 755f 636f 6c6c 6563 7469 6f6e 223e  etu_collection">
+00000220: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000230: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000240: 2f70 7970 692f 646d 2f63 6c6f 7665 7273  /pypi/dm/clovers
+00000250: 5f73 6574 755f 636f 6c6c 6563 7469 6f6e  _setu_collection
+00000260: 2220 616c 743d 2270 7970 6920 646f 776e  " alt="pypi down
+00000270: 6c6f 6164 223e 3c2f 613e 0d0a 0d0a 3c2f  load"></a>....</
+00000280: 6469 763e 0d0a 0d0a 2323 20f0 9f92 bf20  div>....## .... 
+00000290: e5ae 89e8 a385 0d0a 0d0a 6060 6062 6173  ..........```bas
+000002a0: 680d 0a70 6970 2069 6e73 7461 6c6c 2063  h..pip install c
+000002b0: 6c6f 7665 7273 2d73 6574 752d 636f 6c6c  lovers-setu-coll
+000002c0: 6563 7469 6f6e 0d0a 6060 600d 0a0d 0a23  ection..```....#
+000002d0: 2320 e29a 99ef b88f 20e9 858d e7bd ae0d  # ...... .......
+000002e0: 0a0d 0a60 6060 746f 6d6c 0d0a 5b63 6c6f  ...```toml..[clo
+000002f0: 7665 7273 5f73 6574 755f 636f 6c6c 6563  vers_setu_collec
+00000300: 7469 6f6e 5d0d 0a23 20e6 98af e590 a6e4  tion]..# .......
+00000310: bf9d e5ad 98e4 bb8e 6170 69e8 8eb7 e58f  ........api.....
+00000320: 96e7 9a84 e59b bee7 8987 0d0a 7361 7665  ............save
+00000330: 5f69 6d61 6765 203d 2074 7275 650d 0a23  _image = true..#
+00000340: 20e4 b8bb e8b7 afe5 be84 0d0a 7061 7468   ...........path
+00000350: 203d 2022 6461 7461 5c5c 7365 7475 5f63   = "data\\setu_c
+00000360: 6f6c 6c65 6374 696f 6e22 0d0a 2320 e7a7  ollection"..# ..
+00000370: 81e8 818a e59b bee7 8987 e999 90e5 88b6  ................
+00000380: 0d0a 7072 6976 6174 655f 7365 7475 5f6c  ..private_setu_l
+00000390: 696d 6974 203d 2066 616c 7365 0d0a 2320  imit = false..# 
+000003a0: e7be a4e8 818a e59b bee7 8987 e999 90e5  ................
+000003b0: 88b6 efbc 88e5 88ab e585 b3ef bc89 0d0a  ................
+000003c0: 7075 626c 6963 5f73 6574 755f 6c69 6d69  public_setu_limi
+000003d0: 7420 3d20 7472 7565 0d0a 6060 600d 0a0d  t = true..```...
+000003e0: 0a23 2320 f09f 8e89 20e4 bb8b e7bb 8d0d  .## .... .......
+000003f0: 0a0d 0a2a 2ae6 8c87 e4bb a42a 2aef bc9a  ...**......**...
+00000400: 60e6 9da5 4ee5 bca0 7878 e889 b2e5 9bbe  `...N...xx......
+00000410: 6020 60e6 9da5 4ee5 bca0 7878 6020 60e6  ` `...N...xx` `.
+00000420: 9da5 4ee5 bca0 7231 3878 78e8 89b2 e59b  ..N...r18xx.....
+00000430: be60 0d0a 0d0a 2a2a e68c 87e4 bba4 efbc  .`....**........
+00000440: 88e4 bb85 e7a7 81e8 818a efbc 892a 2aef  .............**.
+00000450: bc9a e588 87e6 8da2 2061 7069 0d0a 0d0a  ........ api....
+00000460: e58d 95e6 aca1 e69c 80e5 a49a e58f 91e9  ................
+00000470: 8081 2035 20e5 bca0 e889 b2e5 9bbe 0d0a  .. 5 ...........
+00000480: 0d0a e7be a4e8 818a e694 afe6 8c81 e58d  ................
+00000490: 95e4 b8aa 2074 6167 efbc 8ce7 a781 e881  .... tag........
+000004a0: 8ae6 94af e68c 8120 3320 e4b8 aa20 7461  ....... 3 ... ta
+000004b0: 67ef bc88 e59b a0e4 b8ba e7a7 81e8 818a  g...............
+000004c0: e794 a820 4c6f 6c69 636f 6eef bc89 efbc  ... Lolicon.....
+000004d0: 8ce7 94a8 e7a9 bae6 a0bc e99a 94e5 bc80  ................
+000004e0: e380 820d 0a0d 0a23 2320 f09f 939e 20e8  .......## .... .
+000004f0: 8194 e7b3 bb0d 0a0d 0ae5 a682 e69c 89e5  ................
+00000500: bbba e8ae aeef bc8c 6275 6720 e58f 8de9  ........bug ....
+00000510: a688 e7ad 89e5 8faf e4bb a5e5 8aa0 e7be  ................
+00000520: a40d 0a0d 0ae6 9cba e599 a8e4 baba 2062  .............. b
+00000530: 7567 20e7 a094 e7a9 b6e4 b8ad e5bf 83ef  ug .............
+00000540: bc88 e997 b2e8 818a e7be a4ef bc89 2037  .............. 7
+00000550: 3434 3735 3131 3739 0d0a 0d0a e6b0 b8e6  44751179........
+00000560: 8192 e4b9 8be5 9f8e efbc 88e6 b58b e8af  ................
+00000570: 95e7 bea4 efbc 8920 3732 3430 3234 3831  ....... 72402481
+00000580: 300d 0a0d 0a21 5be7 bea4 e58f b75d 2868  0....![......](h
+00000590: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000005a0: 6d2f 636c 6f76 6572 732d 7072 6f6a 6563  m/clovers-projec
+000005b0: 742f 636c 6f76 6572 732f 626c 6f62 2f6d  t/clovers/blob/m
+000005c0: 6173 7465 722f 2545 3925 3939 2538 3425  aster/%E9%99%84%
+000005d0: 4534 2542 4225 4236 2f71 7263 6f64 655f  E4%BB%B6/qrcode_
+000005e0: 3136 3736 3533 3837 3432 3232 312e 6a70  1676538742221.jp
+000005f0: 6729 0d0a 0d0a 2323 20f0 9f92 a120 e4bd  g)....## .... ..
+00000600: bfe7 94a8 e79a 8420 4150 490d 0a0d 0a5b  ....... API....[
+00000610: 4a69 7473 755d 2868 7474 7073 3a2f 2f69  Jitsu](https://i
+00000620: 6d61 6765 2e61 6e6f 7375 2e74 6f70 2f29  mage.anosu.top/)
+00000630: 20e7 ae80 e58d 95e5 a5bd e794 a8e7 9a84   ...............
+00000640: e889 b2e5 9bbe 2061 7069 0d0a 0d0a 5b4d  ...... api....[M
+00000650: 6972 6c4b 6f69 2041 5049 5d28 6874 7470  irlKoi API](http
+00000660: 733a 2f2f 6977 3233 332e 636e 2f29 20e5  s://iw233.cn/) .
+00000670: 8faf e4bb a5e9 81bf e585 8d20 626f 7420  ........... bot 
+00000680: e8a2 abe5 b081 e79a 84e8 b685 e5ae 89e5  ................
+00000690: 85a8 efbc 88e5 a5bd e79c 8be4 bd86 e698  ................
+000006a0: afe4 b88d e6b6 a9ef bc89 e889 b2e5 9bbe  ................
+000006b0: 2061 7069 0d0a 0d0a 5b4c 6f6c 6963 6f6e   api....[Lolicon
+000006c0: 2041 5049 5d28 6874 7470 733a 2f2f 6170   API](https://ap
+000006d0: 692e 6c6f 6c69 636f 6e2e 6170 702f 2920  i.lolicon.app/) 
+000006e0: e4bd bfe7 94a8 e8bf 99e4 b8aa e79a 84e6  ................
+000006f0: 97b6 e580 99e8 afb7 e6b3 a8e6 848f e8ba  ................
+00000700: abe4 bd93 0d0a                           ......
```

### Comparing `clovers_setu_collection-0.1.0/PKG-INFO` & `clovers_setu_collection-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,130 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 636c 6f76  : 2.1.Name: clov
 00000020: 6572 735f 7365 7475 5f63 6f6c 6c65 6374  ers_setu_collect
 00000030: 696f 6e0a 5665 7273 696f 6e3a 2030 2e31  ion.Version: 0.1
-00000040: 2e30 0a53 756d 6d61 7279 3a20 0a41 7574  .0.Summary: .Aut
+00000040: 2e31 0a53 756d 6d61 7279 3a20 0a41 7574  .1.Summary: .Aut
 00000050: 686f 723a 206b 6172 6973 6179 610a 4175  hor: karisaya.Au
 00000060: 7468 6f72 2d65 6d61 696c 3a20 3130 3438  thor-email: 1048
 00000070: 3832 3734 3234 4071 712e 636f 6d0a 5265  827424@qq.com.Re
 00000080: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
 00000090: 3d33 2e31 322c 3c34 2e30 0a43 6c61 7373  =3.12,<4.0.Class
 000000a0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
 000000b0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
 000000c0: 7974 686f 6e20 3a3a 2033 0a52 6571 7569  ython :: 3.Requi
 000000d0: 7265 732d 4469 7374 3a20 636c 6f76 6572  res-Dist: clover
 000000e0: 735b 746f 6f6c 735d 2028 3e3d 302e 312e  s[tools] (>=0.1.
-000000f0: 352c 3c30 2e32 2e30 290a 5265 7175 6972  5,<0.2.0).Requir
+000000f0: 382c 3c30 2e32 2e30 290a 5265 7175 6972  8,<0.2.0).Requir
 00000100: 6573 2d44 6973 743a 2070 7964 616e 7469  es-Dist: pydanti
 00000110: 6320 283e 3d32 2e37 2e31 2c3c 332e 302e  c (>=2.7.1,<3.0.
 00000120: 3029 0a44 6573 6372 6970 7469 6f6e 2d43  0).Description-C
 00000130: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
 00000140: 742f 6d61 726b 646f 776e 0a0a 3c64 6976  t/markdown..<div
 00000150: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
 00000160: 0a0a 2320 636c 6f76 6572 732d 7365 7475  ..# clovers-setu
-00000170: 2d63 6f6c 6c65 6374 696f 6e0a 0a3c 2f64  -collection..</d
-00000180: 6976 3e0a 0ae4 bdbf e794 a8e7 9a84 2041  iv>........... A
-00000190: 5049 3a0a 0a5b 4a69 7473 755d 2868 7474  PI:..[Jitsu](htt
-000001a0: 7073 3a2f 2f69 6d61 6765 2e61 6e6f 7375  ps://image.anosu
-000001b0: 2e74 6f70 2f29 20e7 ae80 e58d 95e5 a5bd  .top/) .........
-000001c0: e794 a8e7 9a84 e889 b2e5 9bbe 2061 7069  ............ api
-000001d0: 0a0a 5b4d 6972 6c4b 6f69 2041 5049 5d28  ..[MirlKoi API](
-000001e0: 6874 7470 733a 2f2f 6977 3233 332e 636e  https://iw233.cn
-000001f0: 2f29 20e5 8faf e4bb a5e9 81bf e585 8d20  /) ............ 
-00000200: 626f 7420 e8a2 abe5 b081 e79a 84e8 b685  bot ............
-00000210: e5ae 89e5 85a8 efbc 88e4 bf9d e8af 81e5  ................
-00000220: a5bd e79c 8be4 bd86 e698 afe4 b88d e680  ................
-00000230: 8ee4 b988 e6b6 a9ef bc89 e889 b2e5 9bbe  ................
-00000240: 2061 7069 0a0a 5b4c 6f6c 6963 6f6e 2041   api..[Lolicon A
-00000250: 5049 5d28 6874 7470 733a 2f2f 6170 692e  PI](https://api.
-00000260: 6c6f 6c69 636f 6e2e 6170 702f 2920 e4bd  lolicon.app/) ..
-00000270: bfe7 94a8 e8bf 99e4 b8aa e79a 84e6 97b6  ................
-00000280: e580 99e8 afb7 e6b3 a8e6 848f e8ba abe4  ................
-00000290: bd93 0a0a 2323 20f0 9f92 bf20 e5ae 89e8  ....## .... ....
-000002a0: a385 0a0a 6060 6062 6173 680a 7069 7020  ....```bash.pip 
-000002b0: 696e 7374 616c 6c20 636c 6f76 6572 732d  install clovers-
-000002c0: 7365 7475 2d63 6f6c 6c65 6374 696f 6e0a  setu-collection.
-000002d0: 6060 600a 0a23 2320 e29a 99ef b88f 20e9  ```..## ...... .
-000002e0: 858d e7bd ae0a 0a60 6060 746f 6d6c 0a5b  .......```toml.[
-000002f0: 636c 6f76 6572 735f 7365 7475 5f63 6f6c  clovers_setu_col
-00000300: 6c65 6374 696f 6e5d 0a23 20e6 98af e590  lection].# .....
-00000310: a6e4 bf9d e5ad 98e4 bb8e 6170 69e8 8eb7  ..........api...
-00000320: e58f 96e7 9a84 e59b bee7 8987 0a73 6176  .............sav
-00000330: 655f 696d 6167 6520 3d20 7472 7565 0a23  e_image = true.#
-00000340: 20e4 b8bb e8b7 afe5 be84 0a70 6174 6820   ..........path 
-00000350: 3d20 2264 6174 615c 5c73 6574 755f 636f  = "data\\setu_co
-00000360: 6c6c 6563 7469 6f6e 220a 2320 e7a7 81e8  llection".# ....
-00000370: 818a e59b bee7 8987 e999 90e5 88b6 0a70  ...............p
-00000380: 7269 7661 7465 5f73 6574 755f 6c69 6d69  rivate_setu_limi
-00000390: 7420 3d20 6661 6c73 650a 2320 e7be a4e8  t = false.# ....
-000003a0: 818a e59b bee7 8987 e999 90e5 88b6 efbc  ................
-000003b0: 88e5 88ab e585 b3ef bc89 0a70 7562 6c69  ...........publi
-000003c0: 635f 7365 7475 5f6c 696d 6974 203d 2074  c_setu_limit = t
-000003d0: 7275 650a 6060 600a 0a23 2320 f09f 8e89  rue.```..## ....
-000003e0: 20e4 bb8b e7bb 8d0a 0a2a 2ae6 8c87 e4bb   ........**.....
-000003f0: a42a 2aef bc9a 60e6 9da5 4ee5 bca0 7878  .**...`...N...xx
-00000400: e889 b2e5 9bbe 6020 60e6 9da5 4ee5 bca0  ......` `...N...
-00000410: 7878 6020 60e6 9da5 4ee5 bca0 7231 3878  xx` `...N...r18x
-00000420: 78e8 89b2 e59b be60 0a0a 2a2a e68c 87e4  x......`..**....
-00000430: bba4 efbc 88e4 bb85 e7a7 81e8 818a efbc  ................
-00000440: 892a 2aef bc9a e588 87e6 8da2 2061 7069  .**......... api
-00000450: 0a0a e58d 95e6 aca1 e69c 80e5 a49a e58f  ................
-00000460: 91e9 8081 2035 20e5 bca0 e889 b2e5 9bbe  .... 5 .........
-00000470: 0a0a e7be a4e8 818a e694 afe6 8c81 e58d  ................
-00000480: 95e4 b8aa 2074 6167 efbc 8ce7 a781 e881  .... tag........
-00000490: 8ae6 94af e68c 8120 3320 e4b8 aa20 7461  ....... 3 ... ta
-000004a0: 67ef bc88 e59b a0e4 b8ba e7a7 81e8 818a  g...............
-000004b0: e794 a820 4c6f 6c69 636f 6eef bc89 efbc  ... Lolicon.....
-000004c0: 8ce7 94a8 e7a9 bae6 a0bc e99a 94e5 bc80  ................
-000004d0: e380 820a 0a23 2320 f09f 939e 20e8 8194  .....## .... ...
-000004e0: e7b3 bb0a 0ae5 a682 e69c 89e5 bbba e8ae  ................
-000004f0: aeef bc8c 6275 6720 e58f 8de9 a688 e7ad  ....bug ........
-00000500: 89e5 8faf e4bb a5e5 8aa0 e7be a40a 0ae6  ................
-00000510: 9cba e599 a8e4 baba 2062 7567 20e7 a094  ........ bug ...
-00000520: e7a9 b6e4 b8ad e5bf 83ef bc88 e997 b2e8  ................
-00000530: 818a e7be a4ef bc89 2037 3434 3735 3131  ........ 7447511
-00000540: 3739 0a0a e6b0 b8e6 8192 e4b9 8be5 9f8e  79..............
-00000550: efbc 88e6 b58b e8af 95e7 bea4 efbc 8920  ............... 
-00000560: 3732 3430 3234 3831 300a 0a21 5be7 bea4  724024810..![...
-00000570: e58f b75d 2868 7474 7073 3a2f 2f67 6974  ...](https://git
-00000580: 6875 622e 636f 6d2f 636c 6f76 6572 732d  hub.com/clovers-
-00000590: 7072 6f6a 6563 742f 636c 6f76 6572 732f  project/clovers/
-000005a0: 626c 6f62 2f6d 6173 7465 722f 2545 3925  blob/master/%E9%
-000005b0: 3939 2538 3425 4534 2542 4225 4236 2f71  99%84%E4%BB%B6/q
-000005c0: 7263 6f64 655f 3136 3736 3533 3837 3432  rcode_1676538742
-000005d0: 3232 312e 6a70 6729 0a0a                 221.jpg)..
+00000170: 2d63 6f6c 6c65 6374 696f 6e0a 0a5f e29c  -collection.._..
+00000180: a820 e4bb 8ee5 a49a e4b8 aa20 6170 6920  . ......... api 
+00000190: e88e b7e5 8f96 e889 b2e5 9bbe e5b9 b6e6  ................
+000001a0: a0b9 e68d aee5 9cba e699 afe6 95b4 e590  ................
+000001b0: 88e7 9a84 e889 b2e5 9bbe e68f 92e4 bbb6  ................
+000001c0: 20e2 9ca8 5f0a 0a3c 696d 6720 7372 633d   ..._..<img src=
+000001d0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+000001e0: 656c 6473 2e69 6f2f 6261 6467 652f 7079  elds.io/badge/py
+000001f0: 7468 6f6e 2d33 2e31 322b 2d62 6c75 652e  thon-3.12+-blue.
+00000200: 7376 6722 2061 6c74 3d22 7079 7468 6f6e  svg" alt="python
+00000210: 223e 0a3c 6120 6872 6566 3d22 2e2f 4c49  ">.<a href="./LI
+00000220: 4345 4e53 4522 3e3c 696d 6720 7372 633d  CENSE"><img src=
+00000230: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00000240: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
+00000250: 6963 656e 7365 2f4b 6172 6973 4179 612f  icense/KarisAya/
+00000260: 636c 6f76 6572 735f 7365 7475 5f63 6f6c  clovers_setu_col
+00000270: 6c65 6374 696f 6e2e 7376 6722 2061 6c74  lection.svg" alt
+00000280: 3d22 6c69 6365 6e73 6522 3e3c 2f61 3e0a  ="license"></a>.
+00000290: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000002a0: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
+000002b0: 2f70 7970 692f 636c 6f76 6572 735f 7365  /pypi/clovers_se
+000002c0: 7475 5f63 6f6c 6c65 6374 696f 6e22 3e3c  tu_collection"><
+000002d0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+000002e0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000002f0: 7079 7069 2f76 2f63 6c6f 7665 7273 5f73  pypi/v/clovers_s
+00000300: 6574 755f 636f 6c6c 6563 7469 6f6e 2e73  etu_collection.s
+00000310: 7667 2220 616c 743d 2270 7970 6922 3e3c  vg" alt="pypi"><
+00000320: 2f61 3e0a 3c61 2068 7265 663d 2268 7474  /a>.<a href="htt
+00000330: 7073 3a2f 2f70 7970 692e 7079 7468 6f6e  ps://pypi.python
+00000340: 2e6f 7267 2f70 7970 692f 636c 6f76 6572  .org/pypi/clover
+00000350: 735f 7365 7475 5f63 6f6c 6c65 6374 696f  s_setu_collectio
+00000360: 6e22 3e3c 696d 6720 7372 633d 2268 7474  n"><img src="htt
+00000370: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000380: 2e69 6f2f 7079 7069 2f64 6d2f 636c 6f76  .io/pypi/dm/clov
+00000390: 6572 735f 7365 7475 5f63 6f6c 6c65 6374  ers_setu_collect
+000003a0: 696f 6e22 2061 6c74 3d22 7079 7069 2064  ion" alt="pypi d
+000003b0: 6f77 6e6c 6f61 6422 3e3c 2f61 3e0a 0a3c  ownload"></a>..<
+000003c0: 2f64 6976 3e0a 0a23 2320 f09f 92bf 20e5  /div>..## .... .
+000003d0: ae89 e8a3 850a 0a60 6060 6261 7368 0a70  .......```bash.p
+000003e0: 6970 2069 6e73 7461 6c6c 2063 6c6f 7665  ip install clove
+000003f0: 7273 2d73 6574 752d 636f 6c6c 6563 7469  rs-setu-collecti
+00000400: 6f6e 0a60 6060 0a0a 2323 20e2 9a99 efb8  on.```..## .....
+00000410: 8f20 e985 8de7 bdae 0a0a 6060 6074 6f6d  . ........```tom
+00000420: 6c0a 5b63 6c6f 7665 7273 5f73 6574 755f  l.[clovers_setu_
+00000430: 636f 6c6c 6563 7469 6f6e 5d0a 2320 e698  collection].# ..
+00000440: afe5 90a6 e4bf 9de5 ad98 e4bb 8e61 7069  .............api
+00000450: e88e b7e5 8f96 e79a 84e5 9bbe e789 870a  ................
+00000460: 7361 7665 5f69 6d61 6765 203d 2074 7275  save_image = tru
+00000470: 650a 2320 e4b8 bbe8 b7af e5be 840a 7061  e.# ..........pa
+00000480: 7468 203d 2022 6461 7461 5c5c 7365 7475  th = "data\\setu
+00000490: 5f63 6f6c 6c65 6374 696f 6e22 0a23 20e7  _collection".# .
+000004a0: a781 e881 8ae5 9bbe e789 87e9 9990 e588  ................
+000004b0: b60a 7072 6976 6174 655f 7365 7475 5f6c  ..private_setu_l
+000004c0: 696d 6974 203d 2066 616c 7365 0a23 20e7  imit = false.# .
+000004d0: bea4 e881 8ae5 9bbe e789 87e9 9990 e588  ................
+000004e0: b6ef bc88 e588 abe5 85b3 efbc 890a 7075  ..............pu
+000004f0: 626c 6963 5f73 6574 755f 6c69 6d69 7420  blic_setu_limit 
+00000500: 3d20 7472 7565 0a60 6060 0a0a 2323 20f0  = true.```..## .
+00000510: 9f8e 8920 e4bb 8be7 bb8d 0a0a 2a2a e68c  ... ........**..
+00000520: 87e4 bba4 2a2a efbc 9a60 e69d a54e e5bc  ....**...`...N..
+00000530: a078 78e8 89b2 e59b be60 2060 e69d a54e  .xx......` `...N
+00000540: e5bc a078 7860 2060 e69d a54e e5bc a072  ...xx` `...N...r
+00000550: 3138 7878 e889 b2e5 9bbe 600a 0a2a 2ae6  18xx......`..**.
+00000560: 8c87 e4bb a4ef bc88 e4bb 85e7 a781 e881  ................
+00000570: 8aef bc89 2a2a efbc 9ae5 8887 e68d a220  ....**......... 
+00000580: 6170 690a 0ae5 8d95 e6ac a1e6 9c80 e5a4  api.............
+00000590: 9ae5 8f91 e980 8120 3520 e5bc a0e8 89b2  ....... 5 ......
+000005a0: e59b be0a 0ae7 bea4 e881 8ae6 94af e68c  ................
+000005b0: 81e5 8d95 e4b8 aa20 7461 67ef bc8c e7a7  ....... tag.....
+000005c0: 81e8 818a e694 afe6 8c81 2033 20e4 b8aa  .......... 3 ...
+000005d0: 2074 6167 efbc 88e5 9ba0 e4b8 bae7 a781   tag............
+000005e0: e881 8ae7 94a8 204c 6f6c 6963 6f6e efbc  ...... Lolicon..
+000005f0: 89ef bc8c e794 a8e7 a9ba e6a0 bce9 9a94  ................
+00000600: e5bc 80e3 8082 0a0a 2323 20f0 9f93 9e20  ........## .... 
+00000610: e881 94e7 b3bb 0a0a e5a6 82e6 9c89 e5bb  ................
+00000620: bae8 aeae efbc 8c62 7567 20e5 8f8d e9a6  .......bug .....
+00000630: 88e7 ad89 e58f afe4 bba5 e58a a0e7 bea4  ................
+00000640: 0a0a e69c bae5 99a8 e4ba ba20 6275 6720  ........... bug 
+00000650: e7a0 94e7 a9b6 e4b8 ade5 bf83 efbc 88e9  ................
+00000660: 97b2 e881 8ae7 bea4 efbc 8920 3734 3437  ........... 7447
+00000670: 3531 3137 390a 0ae6 b0b8 e681 92e4 b98b  51179...........
+00000680: e59f 8eef bc88 e6b5 8be8 af95 e7be a4ef  ................
+00000690: bc89 2037 3234 3032 3438 3130 0a0a 215b  .. 724024810..![
+000006a0: e7be a4e5 8fb7 5d28 6874 7470 733a 2f2f  ......](https://
+000006b0: 6769 7468 7562 2e63 6f6d 2f63 6c6f 7665  github.com/clove
+000006c0: 7273 2d70 726f 6a65 6374 2f63 6c6f 7665  rs-project/clove
+000006d0: 7273 2f62 6c6f 622f 6d61 7374 6572 2f25  rs/blob/master/%
+000006e0: 4539 2539 3925 3834 2545 3425 4242 2542  E9%99%84%E4%BB%B
+000006f0: 362f 7172 636f 6465 5f31 3637 3635 3338  6/qrcode_1676538
+00000700: 3734 3232 3231 2e6a 7067 290a 0a23 2320  742221.jpg)..## 
+00000710: f09f 92a1 20e4 bdbf e794 a8e7 9a84 2041  .... ......... A
+00000720: 5049 0a0a 5b4a 6974 7375 5d28 6874 7470  PI..[Jitsu](http
+00000730: 733a 2f2f 696d 6167 652e 616e 6f73 752e  s://image.anosu.
+00000740: 746f 702f 2920 e7ae 80e5 8d95 e5a5 bde7  top/) ..........
+00000750: 94a8 e79a 84e8 89b2 e59b be20 6170 690a  ........... api.
+00000760: 0a5b 4d69 726c 4b6f 6920 4150 495d 2868  .[MirlKoi API](h
+00000770: 7474 7073 3a2f 2f69 7732 3333 2e63 6e2f  ttps://iw233.cn/
+00000780: 2920 e58f afe4 bba5 e981 bfe5 858d 2062  ) ............ b
+00000790: 6f74 20e8 a2ab e5b0 81e7 9a84 e8b6 85e5  ot .............
+000007a0: ae89 e585 a8ef bc88 e5a5 bde7 9c8b e4bd  ................
+000007b0: 86e6 98af e4b8 8de6 b6a9 efbc 89e8 89b2  ................
+000007c0: e59b be20 6170 690a 0a5b 4c6f 6c69 636f  ... api..[Lolico
+000007d0: 6e20 4150 495d 2868 7474 7073 3a2f 2f61  n API](https://a
+000007e0: 7069 2e6c 6f6c 6963 6f6e 2e61 7070 2f29  pi.lolicon.app/)
+000007f0: 20e4 bdbf e794 a8e8 bf99 e4b8 aae7 9a84   ...............
+00000800: e697 b6e5 8099 e8af b7e6 b3a8 e684 8fe8  ................
+00000810: baab e4bd 930a 0a                        .......
```

