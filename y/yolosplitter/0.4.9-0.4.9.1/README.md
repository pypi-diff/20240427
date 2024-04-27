# Comparing `tmp/yolosplitter-0.4.9.tar.gz` & `tmp/yolosplitter-0.4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolosplitter-0.4.9.tar", last modified: Tue Jan 30 02:35:34 2024, max compression
+gzip compressed data, was "yolosplitter-0.4.9.1.tar", last modified: Sat Apr 27 09:39:49 2024, max compression
```

## Comparing `yolosplitter-0.4.9.tar` & `yolosplitter-0.4.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 wpnx      (1000) wpnx      (1000)        0 2024-01-30 02:35:34.791698 yolosplitter-0.4.9/
--rw-r--r--   0 wpnx      (1000) wpnx      (1000)     3538 2024-01-30 02:35:34.791698 yolosplitter-0.4.9/PKG-INFO
--rw-rw-r--   0 wpnx      (1000) wpnx      (1000)     2972 2024-01-30 02:30:10.000000 yolosplitter-0.4.9/README.md
--rw-rw-r--   0 wpnx      (1000) wpnx      (1000)       38 2024-01-30 02:35:34.791698 yolosplitter-0.4.9/setup.cfg
--rw-rw-r--   0 wpnx      (1000) wpnx      (1000)      923 2024-01-04 17:21:47.000000 yolosplitter-0.4.9/setup.py
-drwxrwxr-x   0 wpnx      (1000) wpnx      (1000)        0 2024-01-30 02:35:34.787698 yolosplitter-0.4.9/src/
-drwxrwxr-x   0 wpnx      (1000) wpnx      (1000)        0 2024-01-30 02:35:34.791698 yolosplitter-0.4.9/src/yolosplitter.egg-info/
--rw-r--r--   0 wpnx      (1000) wpnx      (1000)     3538 2024-01-30 02:35:34.000000 yolosplitter-0.4.9/src/yolosplitter.egg-info/PKG-INFO
--rw-rw-r--   0 wpnx      (1000) wpnx      (1000)      237 2024-01-30 02:35:34.000000 yolosplitter-0.4.9/src/yolosplitter.egg-info/SOURCES.txt
--rw-rw-r--   0 wpnx      (1000) wpnx      (1000)        1 2024-01-30 02:35:34.000000 yolosplitter-0.4.9/src/yolosplitter.egg-info/dependency_links.txt
--rw-rw-r--   0 wpnx      (1000) wpnx      (1000)       19 2024-01-30 02:35:34.000000 yolosplitter-0.4.9/src/yolosplitter.egg-info/requires.txt
--rw-rw-r--   0 wpnx      (1000) wpnx      (1000)       13 2024-01-30 02:35:34.000000 yolosplitter-0.4.9/src/yolosplitter.egg-info/top_level.txt
--rw-rw-r--   0 wpnx      (1000) wpnx      (1000)     8843 2024-01-30 02:24:01.000000 yolosplitter-0.4.9/src/yolosplitter.py
+drwxrwxr-x   0 wpnx      (1000) wpnx      (1000)        0 2024-04-27 09:39:49.751839 yolosplitter-0.4.9.1/
+-rw-r--r--   0 wpnx      (1000) wpnx      (1000)     3760 2024-04-27 09:39:49.751839 yolosplitter-0.4.9.1/PKG-INFO
+-rw-rw-r--   0 wpnx      (1000) wpnx      (1000)     3191 2024-04-27 09:38:47.000000 yolosplitter-0.4.9.1/README.md
+-rw-rw-r--   0 wpnx      (1000) wpnx      (1000)       38 2024-04-27 09:39:49.751839 yolosplitter-0.4.9.1/setup.cfg
+-rw-rw-r--   0 wpnx      (1000) wpnx      (1000)      925 2024-04-27 09:28:40.000000 yolosplitter-0.4.9.1/setup.py
+drwxrwxr-x   0 wpnx      (1000) wpnx      (1000)        0 2024-04-27 09:39:49.751839 yolosplitter-0.4.9.1/src/
+drwxrwxr-x   0 wpnx      (1000) wpnx      (1000)        0 2024-04-27 09:39:49.751839 yolosplitter-0.4.9.1/src/yolosplitter.egg-info/
+-rw-r--r--   0 wpnx      (1000) wpnx      (1000)     3760 2024-04-27 09:39:49.000000 yolosplitter-0.4.9.1/src/yolosplitter.egg-info/PKG-INFO
+-rw-rw-r--   0 wpnx      (1000) wpnx      (1000)      237 2024-04-27 09:39:49.000000 yolosplitter-0.4.9.1/src/yolosplitter.egg-info/SOURCES.txt
+-rw-rw-r--   0 wpnx      (1000) wpnx      (1000)        1 2024-04-27 09:39:49.000000 yolosplitter-0.4.9.1/src/yolosplitter.egg-info/dependency_links.txt
+-rw-rw-r--   0 wpnx      (1000) wpnx      (1000)       19 2024-04-27 09:39:49.000000 yolosplitter-0.4.9.1/src/yolosplitter.egg-info/requires.txt
+-rw-rw-r--   0 wpnx      (1000) wpnx      (1000)       13 2024-04-27 09:39:49.000000 yolosplitter-0.4.9.1/src/yolosplitter.egg-info/top_level.txt
+-rw-rw-r--   0 wpnx      (1000) wpnx      (1000)     9431 2024-04-27 09:27:15.000000 yolosplitter-0.4.9.1/src/yolosplitter.py
```

### Comparing `yolosplitter-0.4.9/PKG-INFO` & `yolosplitter-0.4.9.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: yolosplitter
-Version: 0.4.9
-Summary: Tool to Create,Modify YOLO dataset and much more...
-Home-page: https://github.com/sandeshkharat87/yolo-splitter
-Author: wpnx
-Keywords: yolo splitter,split datasets,yolo split,yolos split dataset,yolo,yolosplitter,yolo-splitter
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: pandas
-Requires-Dist: tqdm
-Requires-Dist: PyYAML
-
 # yolo-splitter
 Tool to create,modify YOLO dataset.
 
 ## Installation
 ```bash
 pip install yolosplitter
 ```
@@ -37,15 +21,15 @@
 # To see train/test/val split size, total error files, all class names from annotation files
 ys.info()
 
 # !!! changed show_dataframe to get_dataframe()
 # to see dataframe
 ys.get_dataframe()
 ```
-![2023-10-08_23-28](https://github.com/sandeshkharat87/yolo-splitter/assets/47347413/6e08285d-59c5-4856-8bb5-2eac5f1ec3da)
+![2024-01-30_08-19](https://github.com/sandeshkharat87/yolo-splitter/assets/47347413/b2475cde-cbb7-410f-a4df-dd2622698ee1)
 
 
 
 ```python
 ys.save_split(output_dir="potholes")
 ```
 
@@ -121,20 +105,23 @@
         ├── 02.txt
         ├── 06.txt
         └── 11.txt
 ```
 # Change Log
 ## Stable
 
+* 2023-04-25 version 4.9.1
+    * Fixed. "Having a newline at the end of the file causes an error:
+      ValueError('invalid literal for int() with base 10: ''')". Thanks to [https://github.com/Maxvgrad] for finding bug.
+
 * 2023-01-30 version 4.9
     * Fixed Fixes Annotation Parse Error. Thanks to [https://github.com/Xiteed] 
        
 * 2023-12-20 version 4.8
     * Changed yaml file style
 
 * 2023-12-19 version 4.7
     * Fix output dir of `val` to `valid` thanks to [https://github.com/AndreasFridh]
     * Added `ys.info()` To see train/test/val split size, total error files, all class names from annotation files
     * Changed `ys.show_dataframe` to `ys.get_dataframe()`
     * small bug fixes
-    
-
+
```

### Comparing `yolosplitter-0.4.9/setup.py` & `yolosplitter-0.4.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='yolosplitter',
-    version='0.4.9',
+    version='0.4.9.1',
     description="Tool to Create,Modify YOLO dataset and much more...",
     author= 'wpnx',
     url = 'https://github.com/sandeshkharat87/yolo-splitter',
     long_description = long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     keywords=['yolo splitter', "split datasets", 'yolo split','yolos split dataset','yolo','yolosplitter','yolo-splitter'],
```

### Comparing `yolosplitter-0.4.9/src/yolosplitter.egg-info/PKG-INFO` & `yolosplitter-0.4.9.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolosplitter
-Version: 0.4.9
+Version: 0.4.9.1
 Summary: Tool to Create,Modify YOLO dataset and much more...
 Home-page: https://github.com/sandeshkharat87/yolo-splitter
 Author: wpnx
 Keywords: yolo splitter,split datasets,yolo split,yolos split dataset,yolo,yolosplitter,yolo-splitter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -37,15 +37,15 @@
 # To see train/test/val split size, total error files, all class names from annotation files
 ys.info()
 
 # !!! changed show_dataframe to get_dataframe()
 # to see dataframe
 ys.get_dataframe()
 ```
-![2023-10-08_23-28](https://github.com/sandeshkharat87/yolo-splitter/assets/47347413/6e08285d-59c5-4856-8bb5-2eac5f1ec3da)
+![2024-01-30_08-19](https://github.com/sandeshkharat87/yolo-splitter/assets/47347413/b2475cde-cbb7-410f-a4df-dd2622698ee1)
 
 
 
 ```python
 ys.save_split(output_dir="potholes")
 ```
 
@@ -121,20 +121,23 @@
         ├── 02.txt
         ├── 06.txt
         └── 11.txt
 ```
 # Change Log
 ## Stable
 
+* 2023-04-25 version 4.9.1
+    * Fixed. "Having a newline at the end of the file causes an error:
+      ValueError('invalid literal for int() with base 10: ''')". Thanks to [https://github.com/Maxvgrad] for finding bug.
+
 * 2023-01-30 version 4.9
     * Fixed Fixes Annotation Parse Error. Thanks to [https://github.com/Xiteed] 
        
 * 2023-12-20 version 4.8
     * Changed yaml file style
 
 * 2023-12-19 version 4.7
     * Fix output dir of `val` to `valid` thanks to [https://github.com/AndreasFridh]
     * Added `ys.info()` To see train/test/val split size, total error files, all class names from annotation files
     * Changed `ys.show_dataframe` to `ys.get_dataframe()`
     * small bug fixes
     
-
```

### Comparing `yolosplitter-0.4.9/src/yolosplitter.py` & `yolosplitter-0.4.9.1/src/yolosplitter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,240 +1,274 @@
 import pandas as pd
 import os
 import tqdm
 import shutil as sh
 import yaml
 import random
+import click
 
 
-class YoloSplitter():
-    """
-    imgFormat:[".jpg", ".jpeg", ".png"]
-    Give image format in the list
-
-    lableFormat:[".txt"]
-    Give label format in th list
-    """
-    def __init__(self,imgFormat= [".jpg", ".jpeg", ".png"],labelFormat=[".txt"]):
+class YoloSplitter:
+    def __init__(self, imgFormat=[".jpg", ".jpeg", ".png"], labelFormat=[".txt"]):
+        """
+        Args:
+            imgFormat (list, optional): _description_. Defaults to [".jpg", ".jpeg", ".png"].
+            labelFormat (list, optional): _description_. Defaults to [".txt"].
+
+        Note: Please add image file extensions to the imgFormat list if they are not already listed.
+        """
         self.imgFormat = imgFormat
         self.labelFormat = labelFormat
         self.__DATAFRAME = None
         self.__error_files = []
-        self.__req_cols = ['images', 'labels',  'annots', 'cls_names', 'set', 'new_set']
+        self.__req_cols = ["images", "labels", "annots", "cls_names", "set", "new_set"]
         self.__info = None
 
         # {"train":None,"val":None,"test":None,"cls_names":None}
 
-    def from_mixed_dir(self,input_dir,ratio=(0.70,0.20,0.10),return_df=False):
+    def from_mixed_dir(self, input_dir, ratio=(0.70, 0.20, 0.10), return_df=False):
         """
         input_dir : Provide directory path
         ratio: rato of split train/val/test (0.70,0.20,0.10)
         """
         self.__DATAFRAME = None
         self.__error_files = []
 
         dataset = self.get_data(image_dir=input_dir, label_dir=input_dir)
         input_df = pd.DataFrame.from_dict(dataset).copy()
         input_df["set"] = ""
-        
-        
+
         if self.__error_files:
             print(f"Total Error Files: {len(self.__error_files)} ")
-    
+
         # Splitted df (train/test/val)
-        splitted_df = self.__make_split(input_df,ratio=ratio)
-        
-        
+        splitted_df = self.__make_split(input_df, ratio=ratio)
+
         self.__DATAFRAME = splitted_df
 
         print(self.info())
 
         if return_df:
             return self.__DATAFRAME[self.__req_cols]
         return None
 
-        
-        
-    
-    def from_yolo_dir(self,input_dir,ratio=(0.70,0.20,0.10),return_df=False):
+    def from_yolo_dir(self, input_dir, ratio=(0.70, 0.20, 0.10), return_df=False):
         """
         input_dir : Provide directory path
         ratio: rato of split train/val/test (0.70,0.20,0.10)
         """
         self.__DATAFRAME = None
         self.__error_files = []
         self.__input_dir = input_dir
-        
-        set_dir_names = [i  for i in  os.listdir(input_dir) if i in  ["train","test","valid"]]        
+
+        set_dir_names = [
+            i for i in os.listdir(input_dir) if i in ["train", "test", "valid"]
+        ]
         all_dataframes = []
-        
+
         for folder_name in set_dir_names:
-            os.path.join(input_dir,folder_name)
-            image_dir = os.path.join(input_dir,folder_name,"images")
-            label_dir = os.path.join(input_dir,folder_name,"labels")
+            os.path.join(input_dir, folder_name)
+            image_dir = os.path.join(input_dir, folder_name, "images")
+            label_dir = os.path.join(input_dir, folder_name, "labels")
             dataset = self.get_data(image_dir=image_dir, label_dir=label_dir)
             temp_df = pd.DataFrame.from_dict(dataset)
             temp_df["set"] = folder_name
             all_dataframes.append(temp_df)
-            
+
         if self.__error_files:
             print(f"Total Error Files: {len(self.__error_files)} ")
-        
-        input_df = pd.concat(all_dataframes,ignore_index=True,sort=False)
-        
+
+        input_df = pd.concat(all_dataframes, ignore_index=True, sort=False)
+
         # splitted df (train/test/val)
-        splitted_df = self.__make_split(input_df,ratio=ratio)
-        
+        splitted_df = self.__make_split(input_df, ratio=ratio)
+
         self.__DATAFRAME = splitted_df
-        
+
         print(self.info())
 
         if return_df:
             return self.__DATAFRAME[self.__req_cols]
 
         return None
-        
-    
-    def get_data(self,image_dir,label_dir):
-        dataset = {"images":[], "labels":[], "images_path":[], "labels_path":[] , "annots":[],"cls_names":[] }
-        
-        All_Images = [i for i in os.listdir(
-            f"{image_dir}") if os.path.splitext(i)[-1] in self.imgFormat]
-        All_Labels = [i for i in os.listdir(
-            f"{label_dir}") if os.path.splitext(i)[-1] in self.labelFormat]
+
+    def get_data(self, image_dir, label_dir):
+        dataset = {
+            "images": [],
+            "labels": [],
+            "images_path": [],
+            "labels_path": [],
+            "annots": [],
+            "cls_names": [],
+        }
+
+        All_Images = [
+            i
+            for i in os.listdir(f"{image_dir}")
+            if os.path.splitext(i)[-1] in self.imgFormat
+        ]
+        All_Labels = [
+            i
+            for i in os.listdir(f"{label_dir}")
+            if os.path.splitext(i)[-1] in self.labelFormat
+        ]
 
         for iname in All_Images:
             for lname in All_Labels:
                 if os.path.splitext(iname)[0] == os.path.splitext(lname)[0]:
                     try:
-                        annot_data,cls_names = self.__read_annot(os.path.join(label_dir,lname))
-                        dataset["images_path"].append(os.path.join(image_dir,iname))
-                        dataset["labels_path"].append(os.path.join(label_dir,lname))
+                        annot_data, cls_names = self.__read_annot(
+                            os.path.join(label_dir, lname)
+                        )
+                        dataset["images_path"].append(os.path.join(image_dir, iname))
+                        dataset["labels_path"].append(os.path.join(label_dir, lname))
                         dataset["images"].append(os.path.join(iname))
                         dataset["labels"].append(os.path.join(lname))
                         dataset["annots"].append(annot_data)
                         dataset["cls_names"].append(cls_names)
                     except Exception as e:
-                       self.__error_files.append([os.path.join(label_dir,lname),e])
+                        self.__error_files.append([os.path.join(label_dir, lname), e])
                 else:
                     continue
 
         return dataset
-    
-    
-    def __read_annot(self,path):
+
+    def __read_annot(self, path):
         annot_data = []
         all_cls_names = []
-        with open(path,"r") as f:
+        with open(path, "r") as f:
             f_data = f.read().split("\n")
+            f_data = [line for line in f_data if line.strip()]
             for i in f_data:
                 i = i.strip().split(" ")
                 cls_name = int(i[0])
                 cls_annot = [float(i) for i in i[1:]]
-                annot_data.append([cls_name,cls_annot])
+                annot_data.append([cls_name, cls_annot])
                 all_cls_names.append(cls_name)
-        return annot_data,list(set(all_cls_names))
-    
-    
-    def __make_split(self,input_df,ratio):
-        
-        if round(sum(ratio),5)!=1:
+        return annot_data, list(set(all_cls_names))
+
+    def __make_split(self, input_df, ratio):
+        if round(sum(ratio), 5) != 1:
             raise ValueError("Ratio sum should be equal to 1")
-        
-        if len(ratio)==2:
-            train_ratio,val_ratio = ratio
+
+        if len(ratio) == 2:
+            train_ratio, val_ratio = ratio
             test_ratio = 0
-        
+
         elif len(ratio) == 3:
-            train_ratio,val_ratio,test_ratio = ratio
-        
+            train_ratio, val_ratio, test_ratio = ratio
+
         else:
             raise ValueError("ratio must be tuple length of 2 or 3")
-            
+
         total_length = len(input_df)
         train_length = round(train_ratio * len(input_df))
         val_length = round(val_ratio * total_length)
-        test_length = total_length-train_length-val_length
+        test_length = total_length - train_length - val_length
 
         train_df = input_df.iloc[:train_length].copy()
-        val_df = input_df.iloc[train_length:train_length+val_length].copy()
-        test_df = input_df.iloc[train_length + val_length:].copy()
+        val_df = input_df.iloc[train_length : train_length + val_length].copy()
+        test_df = input_df.iloc[train_length + val_length :].copy()
 
         # Shuffle new_set column to new set
-        set_names = ['train'] * train_length + ['valid'] * val_length + ['test'] * test_length
+        set_names = (
+            ["train"] * train_length + ["valid"] * val_length + ["test"] * test_length
+        )
         random.shuffle(set_names)
-        
-        train_df["new_set"] = set_names[:train_length]
-        val_df["new_set"] = set_names[train_length:train_length + val_length]
-        test_df["new_set"] = set_names[train_length + val_length:]
 
-        
-        splitted_df = pd.concat([train_df,val_df,test_df],ignore_index=True,sort=False)
-        print(f"\nTrain size:{train_length},Validation size:{val_length},Test size :{test_length}\n")
-
-        _cls_names =set([ name for name_list in  splitted_df["cls_names"]
-                              for name in name_list ])
+        train_df["new_set"] = set_names[:train_length]
+        val_df["new_set"] = set_names[train_length : train_length + val_length]
+        test_df["new_set"] = set_names[train_length + val_length :]
 
-        self.__info = {"train":train_length,"val":val_length,"test":test_length,"cls_names":_cls_names,"errors":len(self.show_errors())}
+        splitted_df = pd.concat(
+            [train_df, val_df, test_df], ignore_index=True, sort=False
+        )
+        print(
+            f"\nTrain size:{train_length},Validation size:{val_length},Test size :{test_length}\n"
+        )
+
+        _cls_names = set(
+            [name for name_list in splitted_df["cls_names"] for name in name_list]
+        )
+
+        self.__info = {
+            "train": train_length,
+            "val": val_length,
+            "test": test_length,
+            "cls_names": _cls_names,
+            "errors": len(self.show_errors()),
+        }
 
-        
         return splitted_df
-    
-    def show_errors(self):    
+
+    def show_errors(self):
         return self.__error_files
-    
+
     def get_dataframe(self):
         return self.__DATAFRAME[self.__req_cols]
-    
+
     def info(self):
         return self.__info
 
-    def save_split(self,output_dir):
+    def save_split(self, output_dir):
         """
         output_dir: Oupt dir path
         """
         if os.path.exists(output_dir):
             raise FileExistsError("Folder already exists ...")
 
         input_df = self.__DATAFRAME
-        
+
         print(f"Saving New split in '{output_dir}' dir")
 
         if input_df is None:
-            raise ValueError("Dataframe is not created. Plase ran from_yolo_dir or from_mixed_dir first")
-        
-        
-        for idx,row in tqdm.tqdm(input_df.iterrows(),total=len(input_df)):
-            os.makedirs(os.path.join(output_dir,row["new_set"],"images"), exist_ok=True)
-            os.makedirs(os.path.join(output_dir,row["new_set"],"labels"), exist_ok=True)
-            
-            
-            #Images
+            raise ValueError(
+                "Dataframe is not created. Plase ran from_yolo_dir or from_mixed_dir first"
+            )
+
+        for idx, row in tqdm.tqdm(input_df.iterrows(), total=len(input_df)):
+            os.makedirs(
+                os.path.join(output_dir, row["new_set"], "images"), exist_ok=True
+            )
+            os.makedirs(
+                os.path.join(output_dir, row["new_set"], "labels"), exist_ok=True
+            )
+
+            # Images
             input_image_name = os.path.join(row["images_path"])
-            output_image_name = os.path.join(output_dir,row["new_set"],"images",row["images"])
-            #labels
+            output_image_name = os.path.join(
+                output_dir, row["new_set"], "images", row["images"]
+            )
+            # labels
             input_label_name = os.path.join(row["labels_path"])
-            output_label_name = os.path.join(output_dir,row["new_set"],"labels",row["labels"])
-            
-            #Copying Images --
-            sh.copy2(input_image_name,output_image_name)
-            #Copying labels --
-            sh.copy2(input_label_name,output_label_name)
-        
+            output_label_name = os.path.join(
+                output_dir, row["new_set"], "labels", row["labels"]
+            )
+
+            # Copying Images --
+            sh.copy2(input_image_name, output_image_name)
+            # Copying labels --
+            sh.copy2(input_label_name, output_label_name)
+
         # SAVING YAML FILE
         yamlFile = {"train": "", "nc": 0, "names": ""}
-        flat_list = [item for sublist in input_df["cls_names"].to_list() for item in sublist]
+        flat_list = [
+            item for sublist in input_df["cls_names"].to_list() for item in sublist
+        ]
         cls_names = list(set(flat_list))
-        train_set,valid_set,test_set = [self.__DATAFRAME.new_set.value_counts().to_dict()[i] if i in self.__DATAFRAME.new_set.value_counts().to_dict()  else 0 for i in ["train","valid","test"]]
+        train_set, valid_set, test_set = [
+            self.__DATAFRAME.new_set.value_counts().to_dict()[i]
+            if i in self.__DATAFRAME.new_set.value_counts().to_dict()
+            else 0
+            for i in ["train", "valid", "test"]
+        ]
 
         yamlFile["nc"] = len(cls_names)
         yamlFile["names"] = cls_names
         yamlFile["train"] = os.path.join(output_dir, "train")
         if valid_set != 0:
             yamlFile["val"] = os.path.join(output_dir, "valid")
         if test_set != 0:
             yamlFile["test"] = os.path.join(output_dir, "test")
 
         with open(os.path.join(output_dir, "data.yaml"), "w") as f:
-            yaml.dump(yamlFile, f, indent=2,default_flow_style=None)
-
- 
+            yaml.dump(yamlFile, f, indent=2, default_flow_style=None)
```

