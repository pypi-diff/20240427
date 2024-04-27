# Comparing `tmp/ALLM-1.0.1-py3-none-any.whl.zip` & `tmp/ALLM-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,15 @@
-Zip file size: 6726 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-21 10:37 ALLM/__init__.py
--rw-rw-rw-  2.0 fat     1911 b- defN 24-Apr-21 16:12 ALLM/api.py
--rw-rw-rw-  2.0 fat      757 b- defN 24-Apr-21 10:37 ALLM/cli.py
--rw-rw-rw-  2.0 fat     2579 b- defN 24-Apr-21 10:37 ALLM/generate.py
--rw-rw-rw-  2.0 fat    10338 b- defN 24-Apr-21 17:50 ALLM/instruct.py
--rw-rw-rw-  2.0 fat     2372 b- defN 24-Apr-23 04:58 ALLM-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-23 04:58 ALLM-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       75 b- defN 24-Apr-23 04:58 ALLM-1.0.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-23 04:58 ALLM-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      730 b- defN 24-Apr-23 04:58 ALLM-1.0.1.dist-info/RECORD
-10 files, 18898 bytes uncompressed, 5498 bytes compressed:  70.9%
+Zip file size: 11497 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-27 04:39 ALLM/__init__.py
+-rw-rw-rw-  2.0 fat     3096 b- defN 24-Apr-27 04:39 ALLM/agent_rag.py
+-rw-rw-rw-  2.0 fat     3440 b- defN 24-Apr-27 04:39 ALLM/agent_ragrun.py
+-rw-rw-rw-  2.0 fat      757 b- defN 24-Apr-27 04:39 ALLM/cli.py
+-rw-rw-rw-  2.0 fat     1945 b- defN 24-Apr-27 04:39 ALLM/fasty.py
+-rw-rw-rw-  2.0 fat     2579 b- defN 24-Apr-27 04:39 ALLM/generate.py
+-rw-rw-rw-  2.0 fat    10334 b- defN 24-Apr-27 04:39 ALLM/instruct.py
+-rw-rw-rw-  2.0 fat     3490 b- defN 24-Apr-27 04:39 ALLM/ragserve.py
+-rw-rw-rw-  2.0 fat     3790 b- defN 24-Apr-27 10:23 ALLM-1.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-27 10:23 ALLM-1.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      186 b- defN 24-Apr-27 10:23 ALLM-1.0.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-27 10:23 ALLM-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      957 b- defN 24-Apr-27 10:23 ALLM-1.0.2.dist-info/RECORD
+13 files, 30710 bytes uncompressed, 9931 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -1,31 +1,40 @@
 Filename: ALLM/__init__.py
 Comment: 
 
-Filename: ALLM/api.py
+Filename: ALLM/agent_rag.py
+Comment: 
+
+Filename: ALLM/agent_ragrun.py
 Comment: 
 
 Filename: ALLM/cli.py
 Comment: 
 
+Filename: ALLM/fasty.py
+Comment: 
+
 Filename: ALLM/generate.py
 Comment: 
 
 Filename: ALLM/instruct.py
 Comment: 
 
-Filename: ALLM-1.0.1.dist-info/METADATA
+Filename: ALLM/ragserve.py
+Comment: 
+
+Filename: ALLM-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: ALLM-1.0.1.dist-info/WHEEL
+Filename: ALLM-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: ALLM-1.0.1.dist-info/entry_points.txt
+Filename: ALLM-1.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: ALLM-1.0.1.dist-info/top_level.txt
+Filename: ALLM-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: ALLM-1.0.1.dist-info/RECORD
+Filename: ALLM-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ALLM/instruct.py

```diff
@@ -148,15 +148,15 @@
             verbose=False,
         )
 
         # Start the chat loop
         while True:
             try:
                 # Prompt user for input
-                user_input = input("\n\nUser: ")
+                user_input = input("User: ")
                 
                 # Exit loop if user types "exit"
                 if user_input.lower() == "exit":
                     print("Exiting chat.")
                     break
                 
                 # Construct prompt with user input
```

## Comparing `ALLM-1.0.1.dist-info/RECORD` & `ALLM-1.0.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 ALLM/__init__.py,sha256=8XSO2SVH9cZ_Iut8rNwcDxtEaBp4LIdXP6hAKGRgeaI,39
-ALLM/api.py,sha256=wkihJbxEWe69LL66RuiDJqZYWiLR2nnQ7rb1AVMhFiQ,1911
+ALLM/agent_rag.py,sha256=BzdKTA6gutbZbJS3nL1aWZqmTxe7QABkrLz9zpxlQZc,3096
+ALLM/agent_ragrun.py,sha256=UHLn4mVEBz6C77G8aaf3DWrzuVPfA-PCEp6uFZpcGyM,3440
 ALLM/cli.py,sha256=wWOt7Uv_DmQKT821rEIaEVh9MFJVz0n19BXgwTHsdDY,757
+ALLM/fasty.py,sha256=9YSkUcPnZUW2B2JrkHZaH75FcNYLZL5JNJI9ZmqkBCw,1945
 ALLM/generate.py,sha256=bjvXRrlHpe_-TsWDAL-OoivuTO9225gOK15FKRlBvIg,2579
-ALLM/instruct.py,sha256=2tasQjI3gQOmTudcVCg04Y1Wu9EICZTHNCDxEmF61GA,10338
-ALLM-1.0.1.dist-info/METADATA,sha256=oZBwc6HK5DHN6OBSn-2geOb33X3JZcyxO76SKc7iJJw,2372
-ALLM-1.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ALLM-1.0.1.dist-info/entry_points.txt,sha256=bRVlAhmjDquIZd9PRF-QVLXaA7gGWr9F9TOMkX4lGgA,75
-ALLM-1.0.1.dist-info/top_level.txt,sha256=7I9ZpiXpdc4mz6ZgmIvmsbw5M2OC1m99v28mTvj1qEM,5
-ALLM-1.0.1.dist-info/RECORD,,
+ALLM/instruct.py,sha256=9cjx7CnIc-C-LXxVl2THdlrNX3WXcZ0rXKXWVpZ0BXY,10334
+ALLM/ragserve.py,sha256=MD6Tq0W45IIhbnEqCUypB3Vf2P1kxldm6fwl-DypG7I,3490
+ALLM-1.0.2.dist-info/METADATA,sha256=DrqIOEOekF9yq4wj27nI64q_SmCWiE4q1Y5McBdTdxg,3790
+ALLM-1.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ALLM-1.0.2.dist-info/entry_points.txt,sha256=fm1Uz1aVfoYycTrPBgRVy_cUkbTiud-eC_lhvV9blgY,186
+ALLM-1.0.2.dist-info/top_level.txt,sha256=7I9ZpiXpdc4mz6ZgmIvmsbw5M2OC1m99v28mTvj1qEM,5
+ALLM-1.0.2.dist-info/RECORD,,
```

