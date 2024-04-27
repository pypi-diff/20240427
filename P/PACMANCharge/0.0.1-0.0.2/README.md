# Comparing `tmp/PACMANCharge-0.0.1.tar.gz` & `tmp/PACMANCharge-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PACMANCharge-0.0.1.tar", last modified: Sat Apr 27 15:17:45 2024, max compression
+gzip compressed data, was "PACMANCharge-0.0.2.tar", last modified: Sat Apr 27 15:22:21 2024, max compression
```

## Comparing `PACMANCharge-0.0.1.tar` & `PACMANCharge-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-27 15:17:45.380518 PACMANCharge-0.0.1/
--rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMANCharge-0.0.1/LICENSE
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-27 15:17:45.283517 PACMANCharge-0.0.1/PACMANCharge/
--rwxrwxrwx   0 root         (0) root         (0)    25236 2024-04-27 15:03:47.000000 PACMANCharge-0.0.1/PACMANCharge/PACMaN.py
--rwxrwxrwx   0 root         (0) root         (0)       31 2024-04-27 15:01:51.000000 PACMANCharge-0.0.1/PACMANCharge/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-27 15:17:45.339517 PACMANCharge-0.0.1/PACMANCharge.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     4191 2024-04-27 15:17:45.000000 PACMANCharge-0.0.1/PACMANCharge.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      286 2024-04-27 15:17:45.000000 PACMANCharge-0.0.1/PACMANCharge.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-27 15:17:45.000000 PACMANCharge-0.0.1/PACMANCharge.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      112 2024-04-27 15:17:45.000000 PACMANCharge-0.0.1/PACMANCharge.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-04-27 15:17:45.000000 PACMANCharge-0.0.1/PACMANCharge.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     4191 2024-04-27 15:17:45.375518 PACMANCharge-0.0.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3606 2024-04-23 07:07:55.000000 PACMANCharge-0.0.1/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-27 15:17:45.381518 PACMANCharge-0.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      961 2024-04-27 15:17:16.000000 PACMANCharge-0.0.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-27 15:17:45.362518 PACMANCharge-0.0.1/test/
--rwxrwxrwx   0 root         (0) root         (0)    34098 2024-03-24 05:52:28.000000 PACMANCharge-0.0.1/test/Cu-BTC.cif
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMANCharge-0.0.1/test/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-27 15:22:21.104868 PACMANCharge-0.0.2/
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMANCharge-0.0.2/LICENSE
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-27 15:22:21.013607 PACMANCharge-0.0.2/PACMANCharge/
+-rwxrwxrwx   0 root         (0) root         (0)    25263 2024-04-27 15:21:48.000000 PACMANCharge-0.0.2/PACMANCharge/PACMaN.py
+-rwxrwxrwx   0 root         (0) root         (0)       31 2024-04-27 15:01:51.000000 PACMANCharge-0.0.2/PACMANCharge/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-27 15:22:21.068867 PACMANCharge-0.0.2/PACMANCharge.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3959 2024-04-27 15:22:20.000000 PACMANCharge-0.0.2/PACMANCharge.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      286 2024-04-27 15:22:20.000000 PACMANCharge-0.0.2/PACMANCharge.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-27 15:22:20.000000 PACMANCharge-0.0.2/PACMANCharge.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      112 2024-04-27 15:22:20.000000 PACMANCharge-0.0.2/PACMANCharge.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-04-27 15:22:20.000000 PACMANCharge-0.0.2/PACMANCharge.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     3959 2024-04-27 15:22:21.103868 PACMANCharge-0.0.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3606 2024-04-23 07:07:55.000000 PACMANCharge-0.0.2/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-27 15:22:21.105868 PACMANCharge-0.0.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      961 2024-04-27 15:22:11.000000 PACMANCharge-0.0.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-27 15:22:21.091867 PACMANCharge-0.0.2/test/
+-rwxrwxrwx   0 root         (0) root         (0)    34098 2024-03-24 05:52:28.000000 PACMANCharge-0.0.2/test/Cu-BTC.cif
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMANCharge-0.0.2/test/__init__.py
```

### Comparing `PACMANCharge-0.0.1/LICENSE` & `PACMANCharge-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PACMANCharge-0.0.1/PACMANCharge/PACMaN.py` & `PACMANCharge-0.0.2/PACMANCharge/PACMaN.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
     
 class CIFData(Dataset):
     def __init__(self,crystal_data,pos,cell,radius,dmin,step):
         self.pos = pos
         self.cell = cell
         self.radius = radius
         self.crystal_data = crystal_data
-        atom_init_file = resource_filename('GCNCharge', 'atom_init.json')
+        atom_init_file = resource_filename('PACMANCharge', 'atom_init.json')
         self.ari = AtomCustomJSONInitializer(atom_init_file)
         self.gdf = GaussianDistance(dmin=dmin, dmax=self.radius, step=step)
     def __len__(self):
         return 1
     @functools.lru_cache(maxsize=None) 
     def __getitem__(self,_):
         nums = self.crystal_data['numbers']
@@ -464,19 +464,19 @@
             nbr_fea,atom_fea,global_fea = conv_func(atom_fea,nbr_fea,nbr_fea_idx1,nbr_fea_idx2,num_nbrs,crystal_atom_idx)          
         global_fea = global_fea / atom_nums
         z = self.phi_u(global_fea)
         return z
 
 def predict(cif_file,model_name,digits,atom_type,neutral):
     if model_name == "MOF":
-        model_ddec_name = resource_filename('PACMAN', 'mof.pth')
-        ddec_nor_name = resource_filename('PACMAN', 'mof.pkl')
+        model_ddec_name = resource_filename('PACMANCharge', 'mof.pth')
+        ddec_nor_name = resource_filename('PACMANCharge', 'mof.pkl')
     elif model_name == "COF":
-        model_ddec_name = resource_filename('PACMAN', 'cof.pth')
-        ddec_nor_name = resource_filename('PACMAN', 'cof.pkl')
+        model_ddec_name = resource_filename('PACMANCharge', 'cof.pth')
+        ddec_nor_name = resource_filename('PACMANCharge', 'cof.pkl')
     with open(ddec_nor_name, 'rb') as f:
         ddec_nor = pickle.load(f)
     f.close()
     try:
         struc = ase_format(cif_file)
         crystal_data = CIF2json(struc,cif_file)
         cell,pos=pre4pre(cif_file)
```

### Comparing `PACMANCharge-0.0.1/PACMANCharge.egg-info/PKG-INFO` & `PACMANCharge-0.0.2/PACMANCharge.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 Metadata-Version: 2.1
 Name: PACMANCharge
-Version: 0.0.1
+Version: 0.0.2
 Summary: A partial atomic charge of nanoporous materials predicter
 Home-page: https://github.com/sxm13/GCNCharges
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.13.3
-Requires-Dist: pymatgen>=2018.6.11
-Requires-Dist: ase>=3.19
-Requires-Dist: tqdm>=4.15
-Requires-Dist: pandas>=0.20.3
-Requires-Dist: scikit-learn>=0.19.1
-Requires-Dist: joblib>=0.13.2
-Requires-Dist: torch
 
 <h1 align="center">PACMAN</h1>
 
 <h4 align="center">
 
 </h4>
```

### Comparing `PACMANCharge-0.0.1/PKG-INFO` & `PACMANCharge-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 Metadata-Version: 2.1
 Name: PACMANCharge
-Version: 0.0.1
+Version: 0.0.2
 Summary: A partial atomic charge of nanoporous materials predicter
 Home-page: https://github.com/sxm13/GCNCharges
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.13.3
-Requires-Dist: pymatgen>=2018.6.11
-Requires-Dist: ase>=3.19
-Requires-Dist: tqdm>=4.15
-Requires-Dist: pandas>=0.20.3
-Requires-Dist: scikit-learn>=0.19.1
-Requires-Dist: joblib>=0.13.2
-Requires-Dist: torch
 
 <h1 align="center">PACMAN</h1>
 
 <h4 align="center">
 
 </h4>
```

### Comparing `PACMANCharge-0.0.1/README.md` & `PACMANCharge-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `PACMANCharge-0.0.1/setup.py` & `PACMANCharge-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="PACMANCharge",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(),
     description="A partial atomic charge of nanoporous materials predicter",
     author="Guobin Zhao",
     author_email="sxmzhaogb@gmai.com",
     url="https://github.com/sxm13/GCNCharges",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `PACMANCharge-0.0.1/test/Cu-BTC.cif` & `PACMANCharge-0.0.2/test/Cu-BTC.cif`

 * *Files identical despite different names*

