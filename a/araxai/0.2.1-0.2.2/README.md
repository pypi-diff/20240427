# Comparing `tmp/araxai-0.2.1.tar.gz` & `tmp/araxai-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "araxai-0.2.1.tar", last modified: Sun Nov 12 21:12:55 2023, max compression
+gzip compressed data, was "araxai-0.2.2.tar", last modified: Sat Apr 27 06:00:28 2024, max compression
```

## Comparing `araxai-0.2.1.tar` & `araxai-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-11-12 21:12:55.082543 araxai-0.2.1/
--rw-rw-rw-   0        0        0     7815 2023-10-31 21:50:02.000000 araxai-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     9538 2023-11-12 21:12:55.082543 araxai-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     8546 2023-11-12 21:10:05.000000 araxai-0.2.1/README.md
--rw-rw-rw-   0        0        0      143 2023-10-31 21:38:48.000000 araxai-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-11-12 21:12:55.082543 araxai-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1293 2023-11-12 21:12:13.000000 araxai-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-12 21:12:55.049836 araxai-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-11-12 21:12:55.066395 araxai-0.2.1/src/araxai/
--rw-rw-rw-   0        0        0       74 2023-11-08 21:42:22.000000 araxai-0.2.1/src/araxai/__init__.py
--rw-rw-rw-   0        0        0    25223 2023-11-08 20:37:36.000000 araxai-0.2.1/src/araxai/ara.py
-drwxrwxrwx   0        0        0        0 2023-11-12 21:12:55.082543 araxai-0.2.1/src/araxai.egg-info/
--rw-rw-rw-   0        0        0     9538 2023-11-12 21:12:55.000000 araxai-0.2.1/src/araxai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-11-12 21:12:55.000000 araxai-0.2.1/src/araxai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-12 21:12:55.000000 araxai-0.2.1/src/araxai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-11-12 21:12:55.000000 araxai-0.2.1/src/araxai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-11-12 21:12:55.000000 araxai-0.2.1/src/araxai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 06:00:28.102384 araxai-0.2.2/
+-rw-rw-rw-   0        0        0     7815 2023-10-31 21:50:02.000000 araxai-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     9538 2024-04-27 06:00:28.102384 araxai-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8546 2023-11-12 21:10:05.000000 araxai-0.2.2/README.md
+-rw-rw-rw-   0        0        0      143 2023-10-31 21:38:48.000000 araxai-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-27 06:00:28.102384 araxai-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1293 2024-04-27 05:58:37.000000 araxai-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 06:00:28.070635 araxai-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-27 06:00:28.086739 araxai-0.2.2/src/araxai/
+-rw-rw-rw-   0        0        0       74 2023-11-08 21:42:22.000000 araxai-0.2.2/src/araxai/__init__.py
+-rw-rw-rw-   0        0        0    26249 2024-04-27 05:59:03.000000 araxai-0.2.2/src/araxai/ara.py
+drwxrwxrwx   0        0        0        0 2024-04-27 06:00:28.102384 araxai-0.2.2/src/araxai.egg-info/
+-rw-rw-rw-   0        0        0     9538 2024-04-27 06:00:28.000000 araxai-0.2.2/src/araxai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-04-27 06:00:28.000000 araxai-0.2.2/src/araxai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 06:00:28.000000 araxai-0.2.2/src/araxai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-04-27 06:00:28.000000 araxai-0.2.2/src/araxai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-27 06:00:28.000000 araxai-0.2.2/src/araxai.egg-info/top_level.txt
```

### Comparing `araxai-0.2.1/LICENSE` & `araxai-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `araxai-0.2.1/PKG-INFO` & `araxai-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: araxai
-Version: 0.2.1
+Version: 0.2.2
 Summary: ARAxai is an expainable AI tool based on association rule analysis (therefore ARA).It can be used as XAI method to describe maininfluencers in data as well as to explain model by simplification using association rule analysis. Key influencers of the target variable are extracted.
 Home-page: https://github.com/petrmasa/araxai
-Author: (C) Copyright 2021 - 2023 Petr Masa
+Author: (C) Copyright 2021 - 2024 Petr Masa
 Author-email: code@cleverminer.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `araxai-0.2.1/README.md` & `araxai-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `araxai-0.2.1/setup.py` & `araxai-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="araxai",
-    version="0.2.1",
-    author="(C) Copyright 2021 - 2023 Petr Masa",
+    version="0.2.2",
+    author="(C) Copyright 2021 - 2024 Petr Masa",
     author_email="code@cleverminer.org",
     description="ARAxai is an expainable AI tool based on association rule analysis (therefore ARA).It can be used as XAI method to describe maininfluencers in data as well as to explain model by simplification using association rule analysis. Key influencers of the target variable are extracted.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/petrmasa/araxai",
     project_urls={
     },
```

### Comparing `araxai-0.2.1/src/araxai/ara.py` & `araxai-0.2.2/src/araxai/ara.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,51 @@
+
 from cleverminer import cleverminer
 
 import pandas
 import time
 import os
 
 from matplotlib import pyplot as plt
+from pandas.core.dtypes.common import is_categorical_dtype
 
 
 class ara:
     """
     Categorical Lift-based Association Rules Analysis.
     Suitable for data profiling (what influences the target and how) as well as XAI method for explaining the model by simplification (how the model estimates a target).
     """
 
-    version_string = "0.2.1"
+    version_string = "0.2.2"
     max_depth = 2
     min_base = 20
     print_rules_on_the_fly = 0
     default_boundaries = [2,5,10]
     boundaries = [2, 5, 10]
     auto_boundaries = False
     min_rules=2
     max_rules=10
     max_iter=10
     init_stepping=2
+    max_seq_len=3
+    font_size_big = 40
+    font_size_normal=30
+
 
     dir = None
 
     res={}
 
     stats={}
 
     start_time = None
     end_time = None
 
     clms=[]
+    is_var_ordered ={}
 
     def __init__(self,df:pandas.DataFrame=None,target=None,target_class=None,options=None,CL=None):
         """
         Categorical Lift-based Association Rules Analysis. Can be used for data / dependency profiling as well as XAI method for interpreting the model
         :param pandas.DataFrame df: pandas dataframe with input data
         :param string target: target variable of the dataset (profiling) or target prediction (for model explanation task)
         :param string target_class: target class of interest (when profiling more classes is needed, you can run this procedure in loop for all classes)
@@ -118,14 +125,18 @@
                     if "max_depth" in options:
                         ara.max_depth=options.get("max_depth")
                     if "min_base" in options:
                         ara.min_base = options.get("min_base")
                     if "print_rules_on_the_fly" in options:
                         ara.print_rules_on_the_fly = options.get("print_rules_on_the_fly")
                         print("WARNING: this option is marked as experimental. Will be replaced.")
+                    if "font_size_big" in options:
+                        ara.font_size_big = options.get("font_size_big")
+                    if "font_size_normal" in options:
+                        ara.font_size_normal = options.get("font_size_normal")
                     if "boundaries" in options:
                         if forced_boundaries is None:
                             b = options.get("boundaries")
                             if not(len(b)==3):
                                 print("WARNING: boundaries parameter must have length of 3. Parameter will be ignored.")
                             else:
                                 if b[0]<b[1] and b[1]<b[2]:
@@ -139,30 +150,41 @@
                     print("ERROR: options must be a dictionary")
                     return
             ara.clms = []
             for i in range(ara.max_depth):
                 print(f"..will initialize CLM#{i+1}")
                 clm_l=cleverminer(df=df)
                 ara.clms.append(clm_l)
+                for colname in df.columns:
+                    is_ordered = False
+                    if is_categorical_dtype(df[colname]):
+                        if df[colname].cat.ordered:
+                            is_ordered = True
+                    ara.is_var_ordered[colname] = is_ordered
         res_ara = []
         if (df is None):
             print("Dataframe is missing")
             return
         if (target is None):
             print("Target is missing")
             return
         if not(target in df.columns):
             print(f"{target} is not present in the dataframe.")
             return
         def var_str_to_literal(name):
             d = {}
             d['name']=name
-            d['type']='subset'
             d['minlen']=1
-            d['maxlen']=1
+            is_ordered = ara.is_var_ordered[name]
+            if is_ordered:
+                d['type'] = 'seq'
+                d['maxlen'] = ara.max_seq_len
+            else:
+                d['type']='subset'
+                d['maxlen']=1
             return d
         an=[]
         def cond_str_lst(cond):
             res=[]
             if cond is None:
                 return res
             attr= cond['attributes']
@@ -171,14 +193,15 @@
                 res.append(i['name'])
             return res
 
 
         cCL=[]
         if cond_CL is not None:
             for cl in cond_CL:
+
                 cCL.append(var_str_to_literal(cl))
 #            cond_lst = cond_str_lst(cond)
 #            cond_dic['attributes']=cond_lst
 #            cond_dic['minlen']=1
 #            cond_dic['maxlen'] = len(cond)
 #            cond_dic['type'] = 'con'
         for nm in df.columns:
@@ -503,19 +526,19 @@
             colr.append(col)
 
         px = 1/plt.rcParams['figure.dpi']
         font = {'size'   : 8}
 
         plt.rc('font', **font)
         plt.figure(figsize=(1920*px,1080*px))
-        plt.title("Overall dataset profiles/global model properties\n Lift of literals that most influence the target class",fontsize = 40)
+        plt.title("Overall dataset profiles/global model properties\n Lift of literals that most influence the target class",fontsize = ara.font_size_big)
         barlist=plt.barh(x,y)
         for i in range(len(colr)):
             barlist[i].set_color(colr[i])
-        plt.tick_params(axis='y', labelsize=30)
+        plt.tick_params(axis='y', labelsize=ara.font_size_normal)
         plt.tight_layout()
         plt.savefig(os.path.join(ara.dir,"total.png"),bbox_inches='tight')
         plt.clf()
         self._draw_result_sub(res=res)
         print(f"Done. Your results are in {ara.dir}")
 
     # prepare and show deep dive subgraphs for every single most important literal and all variables/literals that influence target class the most for important ones
@@ -563,30 +586,30 @@
 
             if len(item['sub'])>0:
                 x_sub,y_sub,y_sub_loc,col_sub,col_sub_loc = self._draw_result_sub(res=item['sub'],pre=pre+" "+lbl,mult=total_lift,init=False)
                 x_grp = x_grp + x_sub
                 y_grp = y_grp + y_sub
                 colr_grp = colr_grp + col_sub
                 fig, axs = plt.subplots(2,figsize=(1920*px,1080*px))
-                fig.suptitle('Local and global profiling of/with '+pre+" "+lbl,fontsize = 40)
+                fig.suptitle('Local and global profiling of/with '+pre+" "+lbl,fontsize = ara.font_size_big)
                 barlist2 = axs[1].barh(x_sub, y_sub)
                 barlist3 = axs[0].barh(x_sub, y_sub_loc)
                 for i in range(len(col_sub)):
                     barlist2[i].set_color(col_sub[i])
                     barlist3[i].set_color(col_sub_loc[i])
                 if not(init):
                     x2 = range(5)
                     y2 = []
                     for ii in x2:
                         y2.append(mult)
-                axs[1].set_title("GLOBAL LIFT VALUE WITH "+pre+" "+lbl+ " (baseline="+str("{:.1f}".format(mult3))+")",fontsize = 40)
-                axs[0].set_title("LOCAL LIFT CHANGE FROM "+ pre+" "+lbl+ " (baseline="+str("{:.1f}".format(mult3))+")",fontsize = 40)
+                axs[1].set_title("GLOBAL LIFT VALUE WITH "+pre+" "+lbl+ " (baseline="+str("{:.1f}".format(mult3))+")",fontsize = ara.font_size_big)
+                axs[0].set_title("LOCAL LIFT CHANGE FROM "+ pre+" "+lbl+ " (baseline="+str("{:.1f}".format(mult3))+")",fontsize = ara.font_size_big)
                 #axs[1].yticks(fontsize=20)
-                axs[0].tick_params(axis='y', labelsize=30)
-                axs[1].tick_params(axis='y', labelsize=30)
+                axs[0].tick_params(axis='y', labelsize=ara.font_size_normal)
+                axs[1].tick_params(axis='y', labelsize=ara.font_size_normal)
                 #axs[0].yticks(fontsize=20)
                 fname = "".join(x if x.isalnum() else "_" for x in pre+" "+lbl)
                 fname = os.path.join(ara.dir,fname+".png")
                 fig.tight_layout()
                 plt.savefig(fname,bbox_inches='tight')
                 plt.clf()
         return x,y,y_loc,colr,colr_loc
```

### Comparing `araxai-0.2.1/src/araxai.egg-info/PKG-INFO` & `araxai-0.2.2/src/araxai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: araxai
-Version: 0.2.1
+Version: 0.2.2
 Summary: ARAxai is an expainable AI tool based on association rule analysis (therefore ARA).It can be used as XAI method to describe maininfluencers in data as well as to explain model by simplification using association rule analysis. Key influencers of the target variable are extracted.
 Home-page: https://github.com/petrmasa/araxai
-Author: (C) Copyright 2021 - 2023 Petr Masa
+Author: (C) Copyright 2021 - 2024 Petr Masa
 Author-email: code@cleverminer.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

