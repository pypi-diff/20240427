# Comparing `tmp/pathologyfoundation-0.1.9.tar.gz` & `tmp/pathologyfoundation-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathologyfoundation-0.1.9.tar", last modified: Thu Aug 17 05:09:27 2023, max compression
+gzip compressed data, was "pathologyfoundation-0.2.tar", last modified: Fri Apr 26 22:07:35 2024, max compression
```

## Comparing `pathologyfoundation-0.1.9.tar` & `pathologyfoundation-0.2.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2023-08-17 05:09:27.492191 pathologyfoundation-0.1.9/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1048 2023-08-16 21:26:47.000000 pathologyfoundation-0.1.9/LICENSE
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      542 2023-08-17 05:09:27.492191 pathologyfoundation-0.1.9/PKG-INFO
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2721 2023-08-17 05:02:26.000000 pathologyfoundation-0.1.9/README.md
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2023-08-17 05:09:27.488191 pathologyfoundation-0.1.9/models/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       64 2023-08-17 05:05:17.000000 pathologyfoundation-0.1.9/models/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)    10833 2023-08-17 04:36:25.000000 pathologyfoundation-0.1.9/models/finetuner.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6619 2023-08-17 04:35:41.000000 pathologyfoundation-0.1.9/models/plip_vit.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2023-08-17 05:09:27.492191 pathologyfoundation-0.1.9/pathologyfoundation.egg-info/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      542 2023-08-17 05:09:27.000000 pathologyfoundation-0.1.9/pathologyfoundation.egg-info/PKG-INFO
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      298 2023-08-17 05:09:27.000000 pathologyfoundation-0.1.9/pathologyfoundation.egg-info/SOURCES.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        1 2023-08-17 05:09:27.000000 pathologyfoundation-0.1.9/pathologyfoundation.egg-info/dependency_links.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       92 2023-08-17 05:09:27.000000 pathologyfoundation-0.1.9/pathologyfoundation.egg-info/requires.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        7 2023-08-17 05:09:27.000000 pathologyfoundation-0.1.9/pathologyfoundation.egg-info/top_level.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       38 2023-08-17 05:09:27.492191 pathologyfoundation-0.1.9/setup.cfg
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      981 2023-08-17 05:09:14.000000 pathologyfoundation-0.1.9/setup.py
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-04-26 22:07:35.243886 pathologyfoundation-0.2/
+-rw-r--r--   0 zhihuang   (501) staff       (20)     1048 2024-04-26 21:38:18.000000 pathologyfoundation-0.2/LICENSE
+-rw-r--r--   0 zhihuang   (501) staff       (20)      540 2024-04-26 22:07:35.242998 pathologyfoundation-0.2/PKG-INFO
+-rw-r--r--   0 zhihuang   (501) staff       (20)     2730 2024-04-26 21:38:18.000000 pathologyfoundation-0.2/README.md
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-04-26 22:07:35.218821 pathologyfoundation-0.2/pathologyfoundation/
+-rw-r--r--   0 zhihuang   (501) staff       (20)      112 2024-04-26 21:38:18.000000 pathologyfoundation-0.2/pathologyfoundation/__init__.py
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-04-26 22:07:35.240489 pathologyfoundation-0.2/pathologyfoundation/dataset/
+-rw-r--r--   0 zhihuang   (501) staff       (20)       25 2024-04-26 21:38:18.000000 pathologyfoundation-0.2/pathologyfoundation/dataset/__init__.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)     2813 2024-04-26 21:38:18.000000 pathologyfoundation-0.2/pathologyfoundation/dataset/load_data.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)      460 2024-04-26 21:38:18.000000 pathologyfoundation-0.2/pathologyfoundation/model_zoo.py
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-04-26 22:07:35.242314 pathologyfoundation-0.2/pathologyfoundation/models/
+-rw-r--r--   0 zhihuang   (501) staff       (20)       64 2024-04-26 21:38:18.000000 pathologyfoundation-0.2/pathologyfoundation/models/__init__.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)    11065 2024-04-26 21:40:33.000000 pathologyfoundation-0.2/pathologyfoundation/models/finetuner.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)     6619 2024-04-26 21:38:18.000000 pathologyfoundation-0.2/pathologyfoundation/models/plip_vit.py
+-rw-r--r--   0 zhihuang   (501) staff       (20)      700 2024-04-26 21:38:18.000000 pathologyfoundation-0.2/pathologyfoundation/utils.py
+drwxr-xr-x   0 zhihuang   (501) staff       (20)        0 2024-04-26 22:07:35.230251 pathologyfoundation-0.2/pathologyfoundation.egg-info/
+-rw-r--r--   0 zhihuang   (501) staff       (20)      540 2024-04-26 22:07:35.000000 pathologyfoundation-0.2/pathologyfoundation.egg-info/PKG-INFO
+-rw-r--r--   0 zhihuang   (501) staff       (20)      533 2024-04-26 22:07:35.000000 pathologyfoundation-0.2/pathologyfoundation.egg-info/SOURCES.txt
+-rw-r--r--   0 zhihuang   (501) staff       (20)        1 2024-04-26 22:07:35.000000 pathologyfoundation-0.2/pathologyfoundation.egg-info/dependency_links.txt
+-rw-r--r--   0 zhihuang   (501) staff       (20)       92 2024-04-26 22:07:35.000000 pathologyfoundation-0.2/pathologyfoundation.egg-info/requires.txt
+-rw-r--r--   0 zhihuang   (501) staff       (20)       20 2024-04-26 22:07:35.000000 pathologyfoundation-0.2/pathologyfoundation.egg-info/top_level.txt
+-rw-r--r--   0 zhihuang   (501) staff       (20)       38 2024-04-26 22:07:35.243987 pathologyfoundation-0.2/setup.cfg
+-rw-r--r--   0 zhihuang   (501) staff       (20)      979 2024-04-26 22:00:28.000000 pathologyfoundation-0.2/setup.py
```

### Comparing `pathologyfoundation-0.1.9/LICENSE` & `pathologyfoundation-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.1.9/PKG-INFO` & `pathologyfoundation-0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pathologyfoundation
-Version: 0.1.9
+Version: 0.2
 Summary: A package of pathology foundation models.
-Home-page: https://github.com/PathologyFoundation/PathologyFoundation
+Home-page: https://github.com/PathologyFoundation/pathologyfoundation
 Author: Zhi Huang
 Author-email: hz9423@gmail.com
 Keywords: Pathology,Foundation model,PLIP,OpenPath
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
```

### Comparing `pathologyfoundation-0.1.9/README.md` & `pathologyfoundation-0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                            )
 ```
 
 Step 3. Start training the model.
 
 ```python
 clf.train(df_image_label,
-          validation_split=0,
+          validation_split=0.1,
           batch_size=32,
           num_workers=1,
           lr=1e-5,
           nepochs=10
           )
 ```
 
@@ -94,15 +94,15 @@
 
 
 Optional 2: Predict a single image.
 
 ```python
 image = Image.open(df_image_label["image"].values[0])
 proba = clf.predict(image)
-predicted_class_name = df.loc[df['label'] == torch.argmax(proba).item(), 'class'][0]
+predicted_class_name = df.loc[df['label'] == torch.argmax(proba).item(), 'class'].values[0]
 print(f"Prediction: {predicted_class_name}")
 ```
 
 Optional 3: Generate image embedding.
 
 ```python
 image = Image.open(df_image_label["image"].values[0])
```

### Comparing `pathologyfoundation-0.1.9/models/finetuner.py` & `pathologyfoundation-0.2/pathologyfoundation/models/finetuner.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,29 +90,33 @@
         classifier = nn.Linear(in_features = self.in_features,
                                     out_features = self.num_classes)
         self.model = BackboneProber(backbone, classifier)
         if checkpoint is not None:
             self.load_model(checkpoint)
         self.train_init()
     
-    def predict(self, image):
+    def predict(self, image, force_to_device=True):
         # image can be either PIL Image or a list of PIL Image
         x = self.preprocess(image)
         # Convert the list of NumPy arrays to a PyTorch tensor
         tensor_list = [torch.tensor(arr) for arr in x]
+        if force_to_device:
+            tensor_list = [tsr.to(device) for tsr in tensor_list]
         # Convert the list of PyTorch tensors to a single tensor
         x = torch.stack(tensor_list)
         out, _ = self.model(x)
         return out
     
-    def extract_embedding(self, image):
+    def extract_embedding(self, image, force_to_device=True):
         # image can be either PIL Image or a list of PIL Image
         x = self.preprocess(image)
         # Convert the list of NumPy arrays to a PyTorch tensor
         tensor_list = [torch.tensor(arr) for arr in x]
+        if force_to_device:
+            tensor_list = [tsr.to(device) for tsr in tensor_list]
         # Convert the list of PyTorch tensors to a single tensor
         x = torch.stack(tensor_list)
         _, embedding = self.model(x)
         return embedding
         
     def train_init(self):
         np.random.seed(self.random_state)
```

### Comparing `pathologyfoundation-0.1.9/models/plip_vit.py` & `pathologyfoundation-0.2/pathologyfoundation/models/plip_vit.py`

 * *Files identical despite different names*

### Comparing `pathologyfoundation-0.1.9/pathologyfoundation.egg-info/PKG-INFO` & `pathologyfoundation-0.2/pathologyfoundation.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pathologyfoundation
-Version: 0.1.9
+Version: 0.2
 Summary: A package of pathology foundation models.
-Home-page: https://github.com/PathologyFoundation/PathologyFoundation
+Home-page: https://github.com/PathologyFoundation/pathologyfoundation
 Author: Zhi Huang
 Author-email: hz9423@gmail.com
 Keywords: Pathology,Foundation model,PLIP,OpenPath
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
```

### Comparing `pathologyfoundation-0.1.9/setup.py` & `pathologyfoundation-0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,20 +11,20 @@
         "appdirs",
         "pandas",
         "numpy",
         "tqdm",
         "gdown",
         "scikit-learn",
     ],
-    version = '0.1.9',  # Ideally should be same as the GitHub release tag varsion
+    version = '0.2',  # Ideally should be same as the GitHub release tag varsion
     description="A package of pathology foundation models.",
     long_description="Please check our github page: https://github.com/PathologyFoundation/pathologyfoundation",
     author = 'Zhi Huang',
     author_email = 'hz9423@gmail.com',
-    url = 'https://github.com/PathologyFoundation/PathologyFoundation',
+    url = 'https://github.com/PathologyFoundation/pathologyfoundation',
     keywords = ['Pathology', 'Foundation model', "PLIP", "OpenPath"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

