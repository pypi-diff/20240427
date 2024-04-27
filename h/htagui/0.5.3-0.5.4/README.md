# Comparing `tmp/htagui-0.5.3.tar.gz` & `tmp/htagui-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagui-0.5.3.tar", max compression
+gzip compressed data, was "htagui-0.5.4.tar", max compression
```

## Comparing `htagui-0.5.3.tar` & `htagui-0.5.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1065 2024-04-22 09:40:11.535899 htagui-0.5.3/LICENSE
--rw-r--r--   0        0        0     8233 2024-04-22 09:40:11.535899 htagui-0.5.3/README.md
--rw-r--r--   0        0        0      330 2024-04-22 09:40:11.787900 htagui-0.5.3/htagui/__init__.py
--rw-r--r--   0        0        0      846 2024-04-22 09:40:11.535899 htagui-0.5.3/htagui/all.py
--rw-r--r--   0        0        0      750 2024-04-22 09:40:11.535899 htagui-0.5.3/htagui/basics/__init__.py
--rw-r--r--   0        0        0    10956 2024-04-22 09:40:11.535899 htagui-0.5.3/htagui/basics/bases.py
--rw-r--r--   0        0        0      771 2024-04-22 09:40:11.535899 htagui-0.5.3/htagui/bulma/__init__.py
--rw-r--r--   0        0        0   656003 2024-04-22 09:40:11.539899 htagui-0.5.3/htagui/bulma/bases.py
--rw-r--r--   0        0        0     4268 2024-04-22 09:40:11.539899 htagui-0.5.3/htagui/common.py
--rw-r--r--   0        0        0     3401 2024-04-22 09:40:11.539899 htagui-0.5.3/htagui/dialog.py
--rw-r--r--   0        0        0     1856 2024-04-22 09:40:11.539899 htagui-0.5.3/htagui/flex.py
--rw-r--r--   0        0        0      771 2024-04-22 09:40:11.539899 htagui-0.5.3/htagui/form.py
--rw-r--r--   0        0        0     3795 2024-04-22 09:40:11.539899 htagui-0.5.3/htagui/ifields.py
--rw-r--r--   0        0        0      746 2024-04-22 09:40:11.539899 htagui-0.5.3/htagui/md/__init__.py
--rw-r--r--   0        0        0    10392 2024-04-22 09:40:11.539899 htagui-0.5.3/htagui/md/bases.py
--rw-r--r--   0        0        0      774 2024-04-22 09:40:11.539899 htagui-0.5.3/htagui/shoelace/__init__.py
--rw-r--r--   0        0        0     8108 2024-04-22 09:40:11.539899 htagui-0.5.3/htagui/shoelace/bases.py
--rw-r--r--   0        0        0     9619 2024-04-22 09:40:11.539899 htagui-0.5.3/htagui/splitters.py
--rw-r--r--   0        0        0     1441 2024-04-22 09:40:11.539899 htagui-0.5.3/htagui/tabs.py
--rw-r--r--   0        0        0     1069 2024-04-22 09:40:11.787900 htagui-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     9466 1970-01-01 00:00:00.000000 htagui-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-27 17:10:16.486731 htagui-0.5.4/LICENSE
+-rw-r--r--   0        0        0     8233 2024-04-27 17:10:16.486731 htagui-0.5.4/README.md
+-rw-r--r--   0        0        0      330 2024-04-27 17:10:16.754731 htagui-0.5.4/htagui/__init__.py
+-rw-r--r--   0        0        0      846 2024-04-27 17:10:16.486731 htagui-0.5.4/htagui/all.py
+-rw-r--r--   0        0        0      750 2024-04-27 17:10:16.486731 htagui-0.5.4/htagui/basics/__init__.py
+-rw-r--r--   0        0        0    11352 2024-04-27 17:10:16.486731 htagui-0.5.4/htagui/basics/bases.py
+-rw-r--r--   0        0        0      771 2024-04-27 17:10:16.486731 htagui-0.5.4/htagui/bulma/__init__.py
+-rw-r--r--   0        0        0   656405 2024-04-27 17:10:16.490731 htagui-0.5.4/htagui/bulma/bases.py
+-rw-r--r--   0        0        0     4268 2024-04-27 17:10:16.490731 htagui-0.5.4/htagui/common.py
+-rw-r--r--   0        0        0     3401 2024-04-27 17:10:16.490731 htagui-0.5.4/htagui/dialog.py
+-rw-r--r--   0        0        0     1856 2024-04-27 17:10:16.490731 htagui-0.5.4/htagui/flex.py
+-rw-r--r--   0        0        0      771 2024-04-27 17:10:16.490731 htagui-0.5.4/htagui/form.py
+-rw-r--r--   0        0        0     3795 2024-04-27 17:10:16.490731 htagui-0.5.4/htagui/ifields.py
+-rw-r--r--   0        0        0      922 2024-04-27 17:10:16.490731 htagui-0.5.4/htagui/md/__init__.py
+-rw-r--r--   0        0        0    10884 2024-04-27 17:10:16.490731 htagui-0.5.4/htagui/md/bases.py
+-rw-r--r--   0        0        0      774 2024-04-27 17:10:16.490731 htagui-0.5.4/htagui/shoelace/__init__.py
+-rw-r--r--   0        0        0     8583 2024-04-27 17:10:16.490731 htagui-0.5.4/htagui/shoelace/bases.py
+-rw-r--r--   0        0        0     9619 2024-04-27 17:10:16.490731 htagui-0.5.4/htagui/splitters.py
+-rw-r--r--   0        0        0     1441 2024-04-27 17:10:16.490731 htagui-0.5.4/htagui/tabs.py
+-rw-r--r--   0        0        0     1069 2024-04-27 17:10:16.758731 htagui-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     9466 1970-01-01 00:00:00.000000 htagui-0.5.4/PKG-INFO
```

### Comparing `htagui-0.5.3/LICENSE` & `htagui-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `htagui-0.5.3/README.md` & `htagui-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `htagui-0.5.3/htagui/all.py` & `htagui-0.5.4/htagui/all.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.3/htagui/basics/__init__.py` & `htagui-0.5.4/htagui/basics/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.3/htagui/basics/bases.py` & `htagui-0.5.4/htagui/basics/bases.py`

 * *Files 2% similar despite different names*

```diff
@@ -346,15 +346,28 @@
         self <= Voile(_onmousedown=metatag.stepevent())
         self <= Tag.div( obj ,_style=f"position:fixed;top:{t};bottom:{b};left:{l};right:{r};background:white;border-radius:0px;box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;;z-index:1001;padding:10px")
 
 class Pop(Tag.div):
     def init(self,metatag,obj,xy:tuple):
         x,y=xy
         self <= VoileTransparent(_onmousedown=lambda ev: metatag.popclose())
-        self <= Tag.div( obj ,_style=f"position:fixed;top:{y}px;left:{x}px;z-index:2001;background:white")
+
+        js="""(function(tag,x,y) {
+            tag.style="position:fixed;z-index:2001;padding:2px;left:"+x+"px;top:"+y+"px";
+            let bw=window.innerWidth;
+            let bh=window.innerHeight;
+            let w=tag.clientWidth;
+            let h=tag.clientHeight;
+            if(x+w > bw) x=bw-w;
+            if(y+h > bh) y=bh-h;
+            tag.style="position:fixed;z-index:2001;padding:2px;left:"+x+"px;top:"+y+"px";
+        })(self,%s,%s)""" % (x,y)
+
+        self <= Tag.div( obj ,js=js)
+
 
 class Toast(Tag.div):
     def init(self,main_non_used,obj,timeout=1000):
         self <= Tag.div(obj,_style="position:fixed;right:10px;bottom:10px;z-index:1001;background:white;padding:10px;border:2px solid black;border-radius:10px;min-width:200px")
         self.js="setTimeout( function() {self.remove()} , %s)" % timeout
 
 ######################################################################################
```

### Comparing `htagui-0.5.3/htagui/bulma/__init__.py` & `htagui-0.5.4/htagui/bulma/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.3/htagui/bulma/bases.py` & `htagui-0.5.4/htagui/bulma/bases.py`

 * *Files 0% similar despite different names*

```diff
@@ -40939,63 +40939,88 @@
 0009fea0: 7461 672c 6f62 6a2c 7879 3a74 7570 6c65  tag,obj,xy:tuple
 0009feb0: 293a 0a20 2020 2020 2020 2078 2c79 3d78  ):.        x,y=x
 0009fec0: 790a 2020 2020 2020 2020 7365 6c66 203c  y.        self <
 0009fed0: 3d20 566f 696c 6554 7261 6e73 7061 7265  = VoileTranspare
 0009fee0: 6e74 285f 6f6e 6d6f 7573 6564 6f77 6e3d  nt(_onmousedown=
 0009fef0: 6c61 6d62 6461 2065 763a 206d 6574 6174  lambda ev: metat
 0009ff00: 6167 2e70 6f70 636c 6f73 6528 2929 0a20  ag.popclose()). 
-0009ff10: 2020 2020 2020 2073 656c 6620 3c3d 2054         self <= T
-0009ff20: 6167 2e64 6976 2820 6f62 6a20 2c5f 7374  ag.div( obj ,_st
-0009ff30: 796c 653d 6622 706f 7369 7469 6f6e 3a66  yle=f"position:f
-0009ff40: 6978 6564 3b74 6f70 3a7b 797d 7078 3b6c  ixed;top:{y}px;l
-0009ff50: 6566 743a 7b78 7d70 783b 7a2d 696e 6465  eft:{x}px;z-inde
-0009ff60: 783a 3230 3031 3b62 6163 6b67 726f 756e  x:2001;backgroun
-0009ff70: 643a 7768 6974 6522 290a 0a63 6c61 7373  d:white")..class
-0009ff80: 2054 6f61 7374 2854 6167 2e64 6976 293a   Toast(Tag.div):
-0009ff90: 0a20 2020 2064 6566 2069 6e69 7428 7365  .    def init(se
-0009ffa0: 6c66 2c6d 6169 6e5f 6e6f 6e5f 7573 6564  lf,main_non_used
-0009ffb0: 2c6f 626a 2c74 696d 656f 7574 3d31 3030  ,obj,timeout=100
-0009ffc0: 3029 3a0a 2020 2020 2020 2020 7365 6c66  0):.        self
-0009ffd0: 203c 3d20 5461 672e 6469 7628 6f62 6a2c   <= Tag.div(obj,
-0009ffe0: 5f73 7479 6c65 3d22 706f 7369 7469 6f6e  _style="position
-0009fff0: 3a66 6978 6564 3b72 6967 6874 3a31 3070  :fixed;right:10p
-000a0000: 783b 626f 7474 6f6d 3a31 3070 783b 7a2d  x;bottom:10px;z-
-000a0010: 696e 6465 783a 3130 3031 3b22 2c20 5f63  index:1001;", _c
-000a0020: 6c61 7373 3d22 6e6f 7469 6669 6361 7469  lass="notificati
-000a0030: 6f6e 2069 732d 6c69 6e6b 2069 732d 6c69  on is-link is-li
-000a0040: 6768 7422 290a 2020 2020 2020 2020 7365  ght").        se
-000a0050: 6c66 2e6a 733d 2273 6574 5469 6d65 6f75  lf.js="setTimeou
-000a0060: 7428 2066 756e 6374 696f 6e28 2920 7b73  t( function() {s
-000a0070: 656c 662e 7265 6d6f 7665 2829 7d20 2c20  elf.remove()} , 
-000a0080: 2573 2922 2025 2074 696d 656f 7574 0a0a  %s)" % timeout..
-000a0090: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000a00a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000a00b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000a00c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000a00d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000a00e0: 2323 2323 2323 0a0a 636c 6173 7320 5461  ######..class Ta
-000a00f0: 6273 2854 6167 2e64 6976 293a 0a20 2020  bs(Tag.div):.   
-000a0100: 2064 6566 2069 6e69 7428 7365 6c66 2c6d   def init(self,m
-000a0110: 6574 6174 6167 2c73 656c 6563 7465 643d  etatag,selected=
-000a0120: 3029 3a0a 2020 2020 2020 2020 756c 203d  0):.        ul =
-000a0130: 2054 6167 2e75 6c28 290a 2020 2020 2020   Tag.ul().      
-000a0140: 2020 666f 7220 6964 782c 6920 696e 2065    for idx,i in e
-000a0150: 6e75 6d65 7261 7465 286d 6574 6174 6167  numerate(metatag
-000a0160: 2e5f 7461 6273 293a 0a20 2020 2020 2020  ._tabs):.       
-000a0170: 2020 2020 206e 616d 6520 3d20 6861 7361       name = hasa
-000a0180: 7474 7228 692c 226e 616d 6522 2920 616e  ttr(i,"name") an
-000a0190: 6420 692e 6e61 6d65 206f 7220 223f 286e  d i.name or "?(n
-000a01a0: 616d 6529 3f22 0a20 2020 2020 2020 2020  ame)?".         
-000a01b0: 2020 2075 6c2b 3d54 6167 2e6c 6928 2054     ul+=Tag.li( T
-000a01c0: 6167 2e61 286e 616d 6529 2c20 5f6f 6e63  ag.a(name), _onc
-000a01d0: 6c69 636b 203d 206d 6574 6174 6167 2e73  lick = metatag.s
-000a01e0: 7465 7065 7665 6e74 2873 656c 6563 743d  tepevent(select=
-000a01f0: 6964 7829 2c20 5f63 6c61 7373 3d22 6973  idx), _class="is
-000a0200: 2d61 6374 6976 6522 2069 6620 6964 783d  -active" if idx=
-000a0210: 3d73 656c 6563 7465 6420 656c 7365 2022  =selected else "
-000a0220: 2229 0a20 2020 2020 2020 2073 656c 663c  ").        self<
-000a0230: 3d54 6167 2e64 6976 2875 6c2c 5f63 6c61  =Tag.div(ul,_cla
-000a0240: 7373 3d22 7461 6273 2229 0a20 2020 2020  ss="tabs").     
-000a0250: 2020 2069 6620 6d65 7461 7461 672e 5f74     if metatag._t
-000a0260: 6162 733a 2073 656c 663c 3d6d 6574 6174  abs: self<=metat
-000a0270: 6167 2e5f 7461 6273 5b73 656c 6563 7465  ag._tabs[selecte
-000a0280: 645d 0a                                  d].
+0009ff10: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+0009ff20: 6a73 3d22 2222 2866 756e 6374 696f 6e28  js="""(function(
+0009ff30: 7461 672c 782c 7929 207b 0a20 2020 2020  tag,x,y) {.     
+0009ff40: 2020 2020 2020 2074 6167 2e73 7479 6c65         tag.style
+0009ff50: 3d22 706f 7369 7469 6f6e 3a66 6978 6564  ="position:fixed
+0009ff60: 3b7a 2d69 6e64 6578 3a32 3030 313b 7061  ;z-index:2001;pa
+0009ff70: 6464 696e 673a 3270 783b 6c65 6674 3a22  dding:2px;left:"
+0009ff80: 2b78 2b22 7078 3b74 6f70 3a22 2b79 2b22  +x+"px;top:"+y+"
+0009ff90: 7078 223b 0a20 2020 2020 2020 2020 2020  px";.           
+0009ffa0: 206c 6574 2062 773d 7769 6e64 6f77 2e69   let bw=window.i
+0009ffb0: 6e6e 6572 5769 6474 683b 0a20 2020 2020  nnerWidth;.     
+0009ffc0: 2020 2020 2020 206c 6574 2062 683d 7769         let bh=wi
+0009ffd0: 6e64 6f77 2e69 6e6e 6572 4865 6967 6874  ndow.innerHeight
+0009ffe0: 3b0a 2020 2020 2020 2020 2020 2020 6c65  ;.            le
+0009fff0: 7420 773d 7461 672e 636c 6965 6e74 5769  t w=tag.clientWi
+000a0000: 6474 683b 0a20 2020 2020 2020 2020 2020  dth;.           
+000a0010: 206c 6574 2068 3d74 6167 2e63 6c69 656e   let h=tag.clien
+000a0020: 7448 6569 6768 743b 0a20 2020 2020 2020  tHeight;.       
+000a0030: 2020 2020 2069 6628 782b 7720 3e20 6277       if(x+w > bw
+000a0040: 2920 783d 6277 2d77 3b0a 2020 2020 2020  ) x=bw-w;.      
+000a0050: 2020 2020 2020 6966 2879 2b68 203e 2062        if(y+h > b
+000a0060: 6829 2079 3d62 682d 683b 0a20 2020 2020  h) y=bh-h;.     
+000a0070: 2020 2020 2020 2074 6167 2e73 7479 6c65         tag.style
+000a0080: 3d22 706f 7369 7469 6f6e 3a66 6978 6564  ="position:fixed
+000a0090: 3b7a 2d69 6e64 6578 3a32 3030 313b 7061  ;z-index:2001;pa
+000a00a0: 6464 696e 673a 3270 783b 6c65 6674 3a22  dding:2px;left:"
+000a00b0: 2b78 2b22 7078 3b74 6f70 3a22 2b79 2b22  +x+"px;top:"+y+"
+000a00c0: 7078 223b 0a20 2020 2020 2020 207d 2928  px";.        })(
+000a00d0: 7365 6c66 2c25 732c 2573 2922 2222 2025  self,%s,%s)""" %
+000a00e0: 2028 782c 7929 0a0a 2020 2020 2020 2020   (x,y)..        
+000a00f0: 7365 6c66 203c 3d20 5461 672e 6469 7628  self <= Tag.div(
+000a0100: 206f 626a 202c 6a73 3d6a 7329 0a63 6c61   obj ,js=js).cla
+000a0110: 7373 2054 6f61 7374 2854 6167 2e64 6976  ss Toast(Tag.div
+000a0120: 293a 0a20 2020 2064 6566 2069 6e69 7428  ):.    def init(
+000a0130: 7365 6c66 2c6d 6169 6e5f 6e6f 6e5f 7573  self,main_non_us
+000a0140: 6564 2c6f 626a 2c74 696d 656f 7574 3d31  ed,obj,timeout=1
+000a0150: 3030 3029 3a0a 2020 2020 2020 2020 7365  000):.        se
+000a0160: 6c66 203c 3d20 5461 672e 6469 7628 6f62  lf <= Tag.div(ob
+000a0170: 6a2c 5f73 7479 6c65 3d22 706f 7369 7469  j,_style="positi
+000a0180: 6f6e 3a66 6978 6564 3b72 6967 6874 3a31  on:fixed;right:1
+000a0190: 3070 783b 626f 7474 6f6d 3a31 3070 783b  0px;bottom:10px;
+000a01a0: 7a2d 696e 6465 783a 3130 3031 3b22 2c20  z-index:1001;", 
+000a01b0: 5f63 6c61 7373 3d22 6e6f 7469 6669 6361  _class="notifica
+000a01c0: 7469 6f6e 2069 732d 6c69 6e6b 2069 732d  tion is-link is-
+000a01d0: 6c69 6768 7422 290a 2020 2020 2020 2020  light").        
+000a01e0: 7365 6c66 2e6a 733d 2273 6574 5469 6d65  self.js="setTime
+000a01f0: 6f75 7428 2066 756e 6374 696f 6e28 2920  out( function() 
+000a0200: 7b73 656c 662e 7265 6d6f 7665 2829 7d20  {self.remove()} 
+000a0210: 2c20 2573 2922 2025 2074 696d 656f 7574  , %s)" % timeout
+000a0220: 0a0a 2323 2323 2323 2323 2323 2323 2323  ..##############
+000a0230: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000a0240: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000a0250: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000a0260: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000a0270: 2323 2323 2323 2323 0a0a 636c 6173 7320  ########..class 
+000a0280: 5461 6273 2854 6167 2e64 6976 293a 0a20  Tabs(Tag.div):. 
+000a0290: 2020 2064 6566 2069 6e69 7428 7365 6c66     def init(self
+000a02a0: 2c6d 6574 6174 6167 2c73 656c 6563 7465  ,metatag,selecte
+000a02b0: 643d 3029 3a0a 2020 2020 2020 2020 756c  d=0):.        ul
+000a02c0: 203d 2054 6167 2e75 6c28 290a 2020 2020   = Tag.ul().    
+000a02d0: 2020 2020 666f 7220 6964 782c 6920 696e      for idx,i in
+000a02e0: 2065 6e75 6d65 7261 7465 286d 6574 6174   enumerate(metat
+000a02f0: 6167 2e5f 7461 6273 293a 0a20 2020 2020  ag._tabs):.     
+000a0300: 2020 2020 2020 206e 616d 6520 3d20 6861         name = ha
+000a0310: 7361 7474 7228 692c 226e 616d 6522 2920  sattr(i,"name") 
+000a0320: 616e 6420 692e 6e61 6d65 206f 7220 223f  and i.name or "?
+000a0330: 286e 616d 6529 3f22 0a20 2020 2020 2020  (name)?".       
+000a0340: 2020 2020 2075 6c2b 3d54 6167 2e6c 6928       ul+=Tag.li(
+000a0350: 2054 6167 2e61 286e 616d 6529 2c20 5f6f   Tag.a(name), _o
+000a0360: 6e63 6c69 636b 203d 206d 6574 6174 6167  nclick = metatag
+000a0370: 2e73 7465 7065 7665 6e74 2873 656c 6563  .stepevent(selec
+000a0380: 743d 6964 7829 2c20 5f63 6c61 7373 3d22  t=idx), _class="
+000a0390: 6973 2d61 6374 6976 6522 2069 6620 6964  is-active" if id
+000a03a0: 783d 3d73 656c 6563 7465 6420 656c 7365  x==selected else
+000a03b0: 2022 2229 0a20 2020 2020 2020 2073 656c   "").        sel
+000a03c0: 663c 3d54 6167 2e64 6976 2875 6c2c 5f63  f<=Tag.div(ul,_c
+000a03d0: 6c61 7373 3d22 7461 6273 2229 0a20 2020  lass="tabs").   
+000a03e0: 2020 2020 2069 6620 6d65 7461 7461 672e       if metatag.
+000a03f0: 5f74 6162 733a 2073 656c 663c 3d6d 6574  _tabs: self<=met
+000a0400: 6174 6167 2e5f 7461 6273 5b73 656c 6563  atag._tabs[selec
+000a0410: 7465 645d 0a                             ted].
```

### Comparing `htagui-0.5.3/htagui/common.py` & `htagui-0.5.4/htagui/common.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.3/htagui/dialog.py` & `htagui-0.5.4/htagui/dialog.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.3/htagui/flex.py` & `htagui-0.5.4/htagui/flex.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.3/htagui/form.py` & `htagui-0.5.4/htagui/form.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.3/htagui/ifields.py` & `htagui-0.5.4/htagui/ifields.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.3/htagui/md/__init__.py` & `htagui-0.5.4/htagui/shoelace/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 #
 # MIT licence
 #
 # https://github.com/manatlan/htag
 # #############################################################################
 
 import __main__
-__main__.htaguimodule = "htagui.md.bases"
+__main__.htaguimodule = "htagui.shoelace.bases"
+
+from htag import Tag
 
 ########################################################################################
 from .bases import Button,Input,Textarea,Menu,Spinner,Select,Radios
 ########################################################################################
 from ..all import *
 
 ALL.extend( [Button,Input,Textarea,Select,Radios,Menu,Spinner] )
```

### Comparing `htagui-0.5.3/htagui/md/bases.py` & `htagui-0.5.4/htagui/md/bases.py`

 * *Files 3% similar despite different names*

```diff
@@ -291,16 +291,28 @@
         self <= Voile(_onmousedown=metatag.stepevent())
         self <= Tag.div( obj ,_style=f"position:fixed;top:{t};bottom:{b};left:{l};right:{r};background:white;border-radius:0px;box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;;z-index:1001;padding:10px")
 
 class Pop(Tag.div):
     def init(self,metatag,obj,xy:tuple):
         x,y=xy
         self <= VoileTransparent(_onmousedown=lambda ev: metatag.popclose())
-        self <= Tag.div( obj ,_style=f"position:fixed;top:{y}px;left:{x}px;z-index:2001;background:white")
+        js="""(function(tag,x,y) {
+            tag.style="position:fixed;z-index:2001;padding:2px;left:"+x+"px;top:"+y+"px";
+            setTimeout(function() {
+                let bw=window.innerWidth;
+                let bh=window.innerHeight;
+                let w=tag.clientWidth;
+                let h=tag.clientHeight;
+                if(x+w > bw) x=bw-w;
+                if(y+h > bh) y=bh-h;
+                tag.style="position:fixed;z-index:2001;padding:2px;left:"+x+"px;top:"+y+"px;background:white";
+            },0);
+        })(self,%s,%s)""" % (x,y)
 
+        self <= Tag.div( obj ,js=js)
 class Toast(Tag.div):
     def init(self,main_non_used,obj,timeout=1000):
         self["style"]="position:fixed;right:10px;bottom:10px;z-index:1001;border:2px solid black;background:white;padding:10px";
         self <= obj
         self.js="setTimeout( function() {self.remove()} , %s)" % timeout
 
 ######################################################################################
```

### Comparing `htagui-0.5.3/htagui/shoelace/bases.py` & `htagui-0.5.4/htagui/shoelace/bases.py`

 * *Files 11% similar despite different names*

```diff
@@ -218,16 +218,28 @@
 
 
 
 class Pop(Tag.div):
     def init(self,metatag,obj,xy:tuple):
         x,y=xy
         self <= VoileTransparent(_onmousedown=lambda ev: metatag.popclose())
-        self <= Tag.div( obj ,_style=f"position:fixed;top:{y}px;left:{x}px;z-index:2001;background:white")
+        js="""(function(tag,x,y) {
+            tag.style="position:fixed;z-index:2001;padding:2px;left:"+x+"px;top:"+y+"px";
+            setTimeout(function() {
+                let bw=window.innerWidth;
+                let bh=window.innerHeight;
+                let w=tag.clientWidth;
+                let h=tag.clientHeight;
+                if(x+w > bw) x=bw-w;
+                if(y+h > bh) y=bh-h;
+                tag.style="position:fixed;z-index:2001;padding:2px;left:"+x+"px;top:"+y+"px";
+            },0);
+        })(self,%s,%s)""" % (x,y)
 
+        self <= Tag.div( obj ,js=js)
 class Toast(Tag.sl_alert):
     def init(self,main_non_used,obj,timeout=1000):
         self["duration"]=timeout
         self <= obj
         self.js = "window.customElements.whenDefined('sl-alert').then( function() { document.getElementById('%s').toast() })" % id(self)
 ######################################################################################
```

### Comparing `htagui-0.5.3/htagui/splitters.py` & `htagui-0.5.4/htagui/splitters.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.3/htagui/tabs.py` & `htagui-0.5.4/htagui/tabs.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.3/pyproject.toml` & `htagui-0.5.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagui"
-version = "0.5.3" # auto-updated
+version = "0.5.4" # auto-updated
 description = "GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','gui', 'electron', "cef", "asyncio", "guy", "desktop", "web", "mobile", "http", "websocket", "html", "pyscript"]
 homepage = "https://github.com/manatlan/htagui"
 repository = "https://github.com/manatlan/htagui"
```

### Comparing `htagui-0.5.3/PKG-INFO` & `htagui-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagui
-Version: 0.5.3
+Version: 0.5.4
 Summary: GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase
 Home-page: https://github.com/manatlan/htagui
 License: MIT
 Keywords: htag,gui,electron,cef,asyncio,guy,desktop,web,mobile,http,websocket,html,pyscript
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.7,<4.0
```

