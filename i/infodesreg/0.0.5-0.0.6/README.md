# Comparing `tmp/infodesreg-0.0.5.tar.gz` & `tmp/infodesreg-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infodesreg-0.0.5.tar", last modified: Fri Apr 26 18:35:50 2024, max compression
+gzip compressed data, was "infodesreg-0.0.6.tar", last modified: Sat Apr 27 17:46:32 2024, max compression
```

## Comparing `infodesreg-0.0.5.tar` & `infodesreg-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:35:50.767770 infodesreg-0.0.5/
--rw-r--r--   0 firuzjuraev   (501) staff       (20)     1073 2024-04-26 17:42:23.000000 infodesreg-0.0.5/LICENSE
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      713 2024-04-26 18:35:50.767606 infodesreg-0.0.5/PKG-INFO
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      202 2024-04-26 17:42:07.000000 infodesreg-0.0.5/README.md
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      491 2024-04-26 18:33:19.000000 infodesreg-0.0.5/pyproject.toml
--rw-r--r--   0 firuzjuraev   (501) staff       (20)       38 2024-04-26 18:35:50.767804 infodesreg-0.0.5/setup.cfg
-drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:35:50.765664 infodesreg-0.0.5/src/
-drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:35:50.766654 infodesreg-0.0.5/src/infodesreg/
--rw-r--r--   0 firuzjuraev   (501) staff       (20)       43 2024-04-26 18:34:05.000000 infodesreg-0.0.5/src/infodesreg/__init__.py
--rw-r--r--   0 firuzjuraev   (501) staff       (20)     4994 2024-04-26 18:27:53.000000 infodesreg-0.0.5/src/infodesreg/base.py
-drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-26 18:35:50.767465 infodesreg-0.0.5/src/infodesreg.egg-info/
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      713 2024-04-26 18:35:50.000000 infodesreg-0.0.5/src/infodesreg.egg-info/PKG-INFO
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      234 2024-04-26 18:35:50.000000 infodesreg-0.0.5/src/infodesreg.egg-info/SOURCES.txt
--rw-r--r--   0 firuzjuraev   (501) staff       (20)        1 2024-04-26 18:35:50.000000 infodesreg-0.0.5/src/infodesreg.egg-info/dependency_links.txt
--rw-r--r--   0 firuzjuraev   (501) staff       (20)       11 2024-04-26 18:35:50.000000 infodesreg-0.0.5/src/infodesreg.egg-info/top_level.txt
+drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-27 17:46:32.345905 infodesreg-0.0.6/
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)     1073 2024-04-26 17:42:23.000000 infodesreg-0.0.6/LICENSE
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)      713 2024-04-27 17:46:32.345715 infodesreg-0.0.6/PKG-INFO
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)      202 2024-04-26 17:42:07.000000 infodesreg-0.0.6/README.md
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)      491 2024-04-27 17:46:12.000000 infodesreg-0.0.6/pyproject.toml
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)       38 2024-04-27 17:46:32.345981 infodesreg-0.0.6/setup.cfg
+drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-27 17:46:32.343755 infodesreg-0.0.6/src/
+drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-27 17:46:32.344703 infodesreg-0.0.6/src/infodesreg/
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)       41 2024-04-27 17:45:56.000000 infodesreg-0.0.6/src/infodesreg/__init__.py
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)     6346 2024-04-27 17:45:20.000000 infodesreg-0.0.6/src/infodesreg/des.py
+drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-27 17:46:32.345563 infodesreg-0.0.6/src/infodesreg.egg-info/
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)      713 2024-04-27 17:46:32.000000 infodesreg-0.0.6/src/infodesreg.egg-info/PKG-INFO
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)      233 2024-04-27 17:46:32.000000 infodesreg-0.0.6/src/infodesreg.egg-info/SOURCES.txt
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)        1 2024-04-27 17:46:32.000000 infodesreg-0.0.6/src/infodesreg.egg-info/dependency_links.txt
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)       11 2024-04-27 17:46:32.000000 infodesreg-0.0.6/src/infodesreg.egg-info/top_level.txt
```

### Comparing `infodesreg-0.0.5/LICENSE` & `infodesreg-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `infodesreg-0.0.5/PKG-INFO` & `infodesreg-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infodesreg
-Version: 0.0.5
+Version: 0.0.6
 Summary: Dynamic Ensemble Selectio for Regression tasks
 Author-email: Panda <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `infodesreg-0.0.5/src/infodesreg/base.py` & `infodesreg-0.0.6/src/infodesreg/des.py`

 * *Files 16% similar despite different names*

```diff
@@ -52,14 +52,17 @@
 
 class DES(BaseDER): 
     def __init__(self, pool_regressors=None, k=7, knn_metric='minkowski', metrics='mse', threshold=0.2):
         super(DES, self).__init__(pool_regressors=pool_regressors, k=k, knn_metric=knn_metric, metrics=metrics, threshold=threshold) 
         
 
     def fit(self, X_dsel=None, y_dsel=None):
+        X_dsel = X_dsel.reset_index(drop=True)
+        y_dsel = y_dsel.reset_index(drop=True)  
+
         self.X_dsel = X_dsel 
         self.y_dsel = y_dsel  
 
     
     def select(self, competences):
         criteria = self.threshold 
         selected_models_indices = []  
@@ -71,14 +74,56 @@
             
             if len(selected_models_indices) == 0: 
                 criteria = criteria + 0.05 
             
         
         self.selected_models_indices = selected_models_indices   
 
+    
+    def predict_xai(self, query): 
+        # 1) define region of competence 
+        self.get_region_of_competence(query) 
+
+        # 2) estimate competence  
+        competences = self.estimate_competence() 
+
+        # 3) select models 
+        self.select(competences) 
+
+        final_prediction = 0 
+        weight_total = 0 
+
+        model_names = [] 
+        individual_predictions = [] 
+        weights = [] 
+
+        
+        for i in self.selected_models_indices: 
+            pred = get_value(self.pool_regressors[i].predict(query))  
+            final_prediction += pred * competences[i] 
+            weight_total += competences[i]  
+
+            model_names.append(self.pool_regressors[i].__class__.__name__)
+            individual_predictions.append(pred) 
+            weights.append(competences[i])
+
+        final_prediction = final_prediction/weight_total
+
+        contribution_dict = {"selected_models": model_names, "predictions": individual_predictions, "competences": weights}
+
+        contribution_df = pd.DataFrame.from_dict(contribution_dict) 
+
+        self.roc['target'] = self.roc_labels 
+        neighbors_df = self.roc
+
+        print(self.roc_labels)
+        
+        return final_prediction, contribution_df, neighbors_df
+
+
 
     def predict_single_sample(self, query): 
         # 1) define region of competence 
         self.get_region_of_competence(query) 
 
         # 2) estimate competence  
         competences = self.estimate_competence()
```

### Comparing `infodesreg-0.0.5/src/infodesreg.egg-info/PKG-INFO` & `infodesreg-0.0.6/src/infodesreg.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infodesreg
-Version: 0.0.5
+Version: 0.0.6
 Summary: Dynamic Ensemble Selectio for Regression tasks
 Author-email: Panda <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

