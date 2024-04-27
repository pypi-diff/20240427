# Comparing `tmp/xm_slurm-0.2-py3-none-any.whl.zip` & `tmp/xm_slurm-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 49213 bytes, number of entries: 36
--rw-r--r--  2.0 unx      901 b- defN 16-Jan-01 00:00 xm_slurm-0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 xm_slurm-0.2.dist-info/WHEEL
+Zip file size: 49214 bytes, number of entries: 36
+-rw-r--r--  2.0 unx      903 b- defN 16-Jan-01 00:00 xm_slurm-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 xm_slurm-0.2.1.dist-info/WHEEL
 -rw-r--r--  2.0 unx     1019 b- defN 16-Jan-01 00:00 xm_slurm/__init__.py
 -rw-r--r--  2.0 unx     9105 b- defN 16-Jan-01 00:00 xm_slurm/api.py
 -rw-r--r--  2.0 unx     4379 b- defN 16-Jan-01 00:00 xm_slurm/batching.py
 -rw-r--r--  2.0 unx     3394 b- defN 16-Jan-01 00:00 xm_slurm/config.py
 -rw-r--r--  2.0 unx       54 b- defN 16-Jan-01 00:00 xm_slurm/console.py
 -rw-r--r--  2.0 unx     5762 b- defN 16-Jan-01 00:00 xm_slurm/executables.py
--rw-r--r--  2.0 unx    18884 b- defN 16-Jan-01 00:00 xm_slurm/execution.py
+-rw-r--r--  2.0 unx    18847 b- defN 16-Jan-01 00:00 xm_slurm/execution.py
 -rw-r--r--  2.0 unx     4723 b- defN 16-Jan-01 00:00 xm_slurm/executors.py
 -rw-r--r--  2.0 unx    25033 b- defN 16-Jan-01 00:00 xm_slurm/experiment.py
 -rw-r--r--  2.0 unx      482 b- defN 16-Jan-01 00:00 xm_slurm/job_blocks.py
 -rw-r--r--  2.0 unx    11216 b- defN 16-Jan-01 00:00 xm_slurm/packageables.py
 -rw-r--r--  2.0 unx      233 b- defN 16-Jan-01 00:00 xm_slurm/packaging/__init__.py
 -rw-r--r--  2.0 unx     2474 b- defN 16-Jan-01 00:00 xm_slurm/packaging/docker/__init__.py
 -rw-r--r--  2.0 unx     3830 b- defN 16-Jan-01 00:00 xm_slurm/packaging/docker/abc.py
@@ -30,9 +30,9 @@
 -rw-r--r--  2.0 unx      814 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/fragments/proxy.bash.j2
 -rw-r--r--  2.0 unx      599 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/job-array.bash.j2
 -rw-r--r--  2.0 unx     1120 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/job-group.bash.j2
 -rw-r--r--  2.0 unx     1852 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/job.bash.j2
 -rw-r--r--  2.0 unx     2884 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/runtimes/apptainer.bash.j2
 -rw-r--r--  2.0 unx     1317 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/runtimes/podman.bash.j2
 -rw-r--r--  2.0 unx     1930 b- defN 16-Jan-01 00:00 xm_slurm/utils.py
-?rw-------  2.0 unx     3097 b- defN 16-Jan-01 00:00 xm_slurm-0.2.dist-info/RECORD
-36 files, 159481 bytes uncompressed, 44241 bytes compressed:  72.3%
+?rw-------  2.0 unx     3103 b- defN 16-Jan-01 00:00 xm_slurm-0.2.1.dist-info/RECORD
+36 files, 159452 bytes uncompressed, 44230 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
-Filename: xm_slurm-0.2.dist-info/METADATA
+Filename: xm_slurm-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: xm_slurm-0.2.dist-info/WHEEL
+Filename: xm_slurm-0.2.1.dist-info/WHEEL
 Comment: 
 
 Filename: xm_slurm/__init__.py
 Comment: 
 
 Filename: xm_slurm/api.py
 Comment: 
@@ -99,11 +99,11 @@
 
 Filename: xm_slurm/templates/slurm/runtimes/podman.bash.j2
 Comment: 
 
 Filename: xm_slurm/utils.py
 Comment: 
 
-Filename: xm_slurm-0.2.dist-info/RECORD
+Filename: xm_slurm-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xm_slurm/execution.py

```diff
@@ -230,15 +230,14 @@
             async with self._connection_lock:
                 try:
                     conn, _ = await asyncssh.create_connection(
                         NoKBAuthSSHClient,
                         host=cluster.host,
                         port=cluster.port or (),
                         username=cluster.user,
-                        config=None,
                     )
                     await self._setup_remote_connection(conn)
                     self._connections[cluster] = conn
                 except asyncssh.misc.PermissionDenied as ex:
                     raise RuntimeError(f"Permission denied connecting to {cluster.host}") from ex
         return self._connections[cluster]
```

## Comparing `xm_slurm-0.2.dist-info/METADATA` & `xm_slurm-0.2.1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xm-slurm
-Version: 0.2
+Version: 0.2.1
 Summary: Slurm backend for XManager.
 Author-Email: Jesse Farebrother <jfarebro@cs.mcgill.ca>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: xmanager>=0.4.0
 Requires-Dist: asyncssh>=2.13.2
 Requires-Dist: humanize>=4.8.0
```

## Comparing `xm_slurm-0.2.dist-info/RECORD` & `xm_slurm-0.2.1.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-xm_slurm-0.2.dist-info/METADATA,sha256=5WbD-v6HdF8Uq_TQfpODdDVwXpTUnV-K9KLl0VZNoiA,901
-xm_slurm-0.2.dist-info/WHEEL,sha256=N2J68yzZqJh3mI_Wg92rwhw0rtJDFpZj9bwQIMJgaVg,90
+xm_slurm-0.2.1.dist-info/METADATA,sha256=HQOrO0uhBPim-mvuhOP0THwUzAagAfiyUdoRRMrAl1k,903
+xm_slurm-0.2.1.dist-info/WHEEL,sha256=7sv5iXvIiTVJSnAxCz2tGBm9DHsb2vPSzeYeT7pvGUY,90
 xm_slurm/__init__.py,sha256=J5FkaAXbcT7yWmcNgBq3mDLOmnNZW7c4WekSt7JVoFc,1019
 xm_slurm/api.py,sha256=5C9bgqSosqNHXwUb-7HoBqnyo6qW53BZiV70w8UD2BQ,9105
 xm_slurm/batching.py,sha256=mGVvccehsC4dfjtg7QqrtxuoxYI_Fs8o1GLJIGVyvyo,4379
 xm_slurm/config.py,sha256=Vdn83DVIZDfppegpg2yObdffDwCJd_AUMxO9D6UiGgI,3394
 xm_slurm/console.py,sha256=UpMqeJ0C8i0pkue1AHnnyyX0bFJ9zZeJ7HBR6yhuA8A,54
 xm_slurm/executables.py,sha256=4SVn6obIvOKh54RXYccixUx993Xma0rLGanD3TfXNS4,5762
-xm_slurm/execution.py,sha256=wt00zpVB5NjreUup8ymiiRSWcRP-usnMcRMaPT1uLL4,18884
+xm_slurm/execution.py,sha256=Si4VUcPRAsrEzc22aeqbgZobXu3QjlhQNFYZ2Y6TKvw,18847
 xm_slurm/executors.py,sha256=vilogTjlxHLfZDms4aYOZWUW8w-2IdxU7xh-9vcW1Y0,4723
 xm_slurm/experiment.py,sha256=bWdzYOglKdvNVMwlE7H3-eQRsP0KTUdef3mKC8jaM5M,25033
 xm_slurm/job_blocks.py,sha256=1H1eZ5gbEGEoDYcoSh8S_gvp04MLXP7G128crDJlMYo,482
 xm_slurm/packageables.py,sha256=nzmkREacDPJXmo6D1mk4bKjUrLTjHj3rue-PoO_EATk,11216
 xm_slurm/packaging/__init__.py,sha256=dh307yLpUT9KN7rJ1e9fYC6hegGKfZcGboUq9nGpDVQ,233
 xm_slurm/packaging/docker/__init__.py,sha256=SQxaDtomYc4NwZ5lSoCiMoy2S2lRmc0sgwVMbENIatU,2474
 xm_slurm/packaging/docker/abc.py,sha256=f8XvUA_FusIpXI45PR5isA2msxM003ycW5mWbAyiKfk,3830
@@ -29,8 +29,8 @@
 xm_slurm/templates/slurm/fragments/proxy.bash.j2,sha256=VJLglZo-Nvx9R-qe3rHTxr07CylTQ6Z9NwBzvIpAZrA,814
 xm_slurm/templates/slurm/job-array.bash.j2,sha256=d4twfV1PATGQwTIleFBUIGmMAIHH-F7RjBsdfaAIQko,599
 xm_slurm/templates/slurm/job-group.bash.j2,sha256=UkjfBE7jg9mepcUWaHZEAjkiXsIM1j_sLxLzxkteD-Y,1120
 xm_slurm/templates/slurm/job.bash.j2,sha256=EUeq3P2xqTIqlHi2SVhFBT7NL4lUj8okYUa3GnlaIIc,1852
 xm_slurm/templates/slurm/runtimes/apptainer.bash.j2,sha256=HYs9FIjRYehGjJwhZKFgT_aMvL9xMetjXdhaB5TT-jw,2884
 xm_slurm/templates/slurm/runtimes/podman.bash.j2,sha256=J_iGoAaW30bbjhSaN0t9wOwbzT0Oc_KRHjuxxOr-lWE,1317
 xm_slurm/utils.py,sha256=PNd0vTn33UKm5LpC41TdO9QIFe21V5A0RbYEhQIMjrA,1930
-xm_slurm-0.2.dist-info/RECORD,,
+xm_slurm-0.2.1.dist-info/RECORD,,
```

