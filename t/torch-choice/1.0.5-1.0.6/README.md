# Comparing `tmp/torch_choice-1.0.5.tar.gz` & `tmp/torch_choice-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_choice-1.0.5.tar", last modified: Mon Sep 18 07:31:33 2023, max compression
+gzip compressed data, was "torch_choice-1.0.6.tar", last modified: Sat Apr 27 03:13:17 2024, max compression
```

## Comparing `torch_choice-1.0.5.tar` & `torch_choice-1.0.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 07:31:33.572891 torch_choice-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-09-18 07:31:10.000000 torch_choice-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15905 2023-09-18 07:31:33.572891 torch_choice-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15215 2023-09-18 07:31:10.000000 torch_choice-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-18 07:31:33.572891 torch_choice-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2023-09-18 07:31:10.000000 torch_choice-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 07:31:33.568891 torch_choice-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9406 2023-09-18 07:31:10.000000 torch_choice-1.0.5/tests/test_choice_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2023-09-18 07:31:10.000000 torch_choice-1.0.5/tests/test_conditional_logit_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2023-09-18 07:31:10.000000 torch_choice-1.0.5/tests/test_nested_logit_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 07:31:33.568891 torch_choice-1.0.5/torch_choice/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-18 07:31:10.000000 torch_choice-1.0.5/torch_choice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 07:31:33.568891 torch_choice-1.0.5/torch_choice/data/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-09-18 07:31:10.000000 torch_choice-1.0.5/torch_choice/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24641 2023-09-18 07:31:10.000000 torch_choice-1.0.5/torch_choice/data/choice_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2023-09-18 07:31:10.000000 torch_choice-1.0.5/torch_choice/data/example_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2023-09-18 07:31:10.000000 torch_choice-1.0.5/torch_choice/data/joint_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2023-09-18 07:31:10.000000 torch_choice-1.0.5/torch_choice/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 07:31:33.568891 torch_choice-1.0.5/torch_choice/model/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-09-18 07:31:10.000000 torch_choice-1.0.5/torch_choice/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10032 2023-09-18 07:31:10.000000 torch_choice-1.0.5/torch_choice/model/coefficient.py
--rw-r--r--   0 runner    (1001) docker     (127)    18464 2023-09-18 07:31:10.000000 torch_choice-1.0.5/torch_choice/model/conditional_logit_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2023-09-18 07:31:10.000000 torch_choice-1.0.5/torch_choice/model/formula_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    24480 2023-09-18 07:31:10.000000 torch_choice-1.0.5/torch_choice/model/nested_logit_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 07:31:33.568891 torch_choice-1.0.5/torch_choice/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-09-18 07:31:10.000000 torch_choice-1.0.5/torch_choice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23594 2023-09-18 07:31:10.000000 torch_choice-1.0.5/torch_choice/utils/easy_data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2023-09-18 07:31:10.000000 torch_choice-1.0.5/torch_choice/utils/run_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11762 2023-09-18 07:31:10.000000 torch_choice-1.0.5/torch_choice/utils/run_helper_lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2023-09-18 07:31:10.000000 torch_choice-1.0.5/torch_choice/utils/std.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 07:31:33.568891 torch_choice-1.0.5/torch_choice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15905 2023-09-18 07:31:33.000000 torch_choice-1.0.5/torch_choice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      858 2023-09-18 07:31:33.000000 torch_choice-1.0.5/torch_choice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-18 07:31:33.000000 torch_choice-1.0.5/torch_choice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-09-18 07:31:33.000000 torch_choice-1.0.5/torch_choice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-09-18 07:31:33.000000 torch_choice-1.0.5/torch_choice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:13:17.604479 torch_choice-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-27 03:13:13.000000 torch_choice-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16268 2024-04-27 03:13:17.604479 torch_choice-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15578 2024-04-27 03:13:13.000000 torch_choice-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 03:13:17.604479 torch_choice-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-27 03:13:13.000000 torch_choice-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:13:17.600479 torch_choice-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9406 2024-04-27 03:13:13.000000 torch_choice-1.0.6/tests/test_choice_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-27 03:13:13.000000 torch_choice-1.0.6/tests/test_conditional_logit_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-27 03:13:13.000000 torch_choice-1.0.6/tests/test_nested_logit_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:13:17.600479 torch_choice-1.0.6/torch_choice/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-27 03:13:13.000000 torch_choice-1.0.6/torch_choice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:13:17.600479 torch_choice-1.0.6/torch_choice/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-27 03:13:13.000000 torch_choice-1.0.6/torch_choice/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29168 2024-04-27 03:13:13.000000 torch_choice-1.0.6/torch_choice/data/choice_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-27 03:13:13.000000 torch_choice-1.0.6/torch_choice/data/example_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-27 03:13:13.000000 torch_choice-1.0.6/torch_choice/data/joint_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-27 03:13:13.000000 torch_choice-1.0.6/torch_choice/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:13:17.600479 torch_choice-1.0.6/torch_choice/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-27 03:13:13.000000 torch_choice-1.0.6/torch_choice/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10032 2024-04-27 03:13:13.000000 torch_choice-1.0.6/torch_choice/model/coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20351 2024-04-27 03:13:13.000000 torch_choice-1.0.6/torch_choice/model/conditional_logit_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-27 03:13:13.000000 torch_choice-1.0.6/torch_choice/model/formula_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26686 2024-04-27 03:13:13.000000 torch_choice-1.0.6/torch_choice/model/nested_logit_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:13:17.604479 torch_choice-1.0.6/torch_choice/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-27 03:13:13.000000 torch_choice-1.0.6/torch_choice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24572 2024-04-27 03:13:13.000000 torch_choice-1.0.6/torch_choice/utils/easy_data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-04-27 03:13:13.000000 torch_choice-1.0.6/torch_choice/utils/run_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13293 2024-04-27 03:13:13.000000 torch_choice-1.0.6/torch_choice/utils/run_helper_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-27 03:13:13.000000 torch_choice-1.0.6/torch_choice/utils/std.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:13:17.604479 torch_choice-1.0.6/torch_choice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16268 2024-04-27 03:13:17.000000 torch_choice-1.0.6/torch_choice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-27 03:13:17.000000 torch_choice-1.0.6/torch_choice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 03:13:17.000000 torch_choice-1.0.6/torch_choice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-27 03:13:17.000000 torch_choice-1.0.6/torch_choice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-27 03:13:17.000000 torch_choice-1.0.6/torch_choice.egg-info/top_level.txt
```

### Comparing `torch_choice-1.0.5/LICENSE` & `torch_choice-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.5/PKG-INFO` & `torch_choice-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_choice
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Pytorch Backend Library for Choice Modelling
 Home-page: https://gsbdbi.github.io/torch-choice/
 Author: Tianyu Du, Ayush Kanodia, and Susan Athey
 Author-email: tianyudu@stanford.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -227,7 +227,22 @@
 We note the shapes/sizes of each of the components in the above model. Suppose there are U users, I items and S sessions; in this case, an item is one of the 10 possible digits, so I = 10; there is one user per session, so that U=S; and each session is an image being classified.
 Then,
 - $X^{session:pixelvalues}_{t}$ is a matrix of size (S) x (H x W) where H x W are the dimensions of the image being classified; its coefficient $\beta_i$ has item level vartiation and is of size (I) x (1)
 
 This is a classic problem used for exposition in Computer Science to motivate various Machine Learning models. There is no concept of a user in this setup. Our package allows for models of this nature and is fully usable for Machine Learning problems with added flexibility over [scikit-learn logistic regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html)
  -->
 We highly recommend users to go through [tutorials](https://github.com/gsbDBI/torch-choice/blob/main/tutorials) we prepared to get a better understanding of what the package offers. We present multiple examples, and for each case we specify the utility form.
+
+## Reproducibility
+The `torch-choice` package is built upon several dependencies that introduce randomness, you would need to fix random seeds for these packages for reproducibility:
+
+```python
+import random
+import numpy as np
+import torch
+
+SEED = 12345
+random.seed(SEED)
+np.random.seed(SEED)
+torch.manual_seed(SEED)
+torch.use_deterministic_algorithms(True)
+```
```

### Comparing `torch_choice-1.0.5/README.md` & `torch_choice-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -206,7 +206,22 @@
 We note the shapes/sizes of each of the components in the above model. Suppose there are U users, I items and S sessions; in this case, an item is one of the 10 possible digits, so I = 10; there is one user per session, so that U=S; and each session is an image being classified.
 Then,
 - $X^{session:pixelvalues}_{t}$ is a matrix of size (S) x (H x W) where H x W are the dimensions of the image being classified; its coefficient $\beta_i$ has item level vartiation and is of size (I) x (1)
 
 This is a classic problem used for exposition in Computer Science to motivate various Machine Learning models. There is no concept of a user in this setup. Our package allows for models of this nature and is fully usable for Machine Learning problems with added flexibility over [scikit-learn logistic regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html)
  -->
 We highly recommend users to go through [tutorials](https://github.com/gsbDBI/torch-choice/blob/main/tutorials) we prepared to get a better understanding of what the package offers. We present multiple examples, and for each case we specify the utility form.
+
+## Reproducibility
+The `torch-choice` package is built upon several dependencies that introduce randomness, you would need to fix random seeds for these packages for reproducibility:
+
+```python
+import random
+import numpy as np
+import torch
+
+SEED = 12345
+random.seed(SEED)
+np.random.seed(SEED)
+torch.manual_seed(SEED)
+torch.use_deterministic_algorithms(True)
+```
```

### Comparing `torch_choice-1.0.5/setup.py` & `torch_choice-1.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="torch_choice",
-    version="1.0.5",
+    version="1.0.6",
     description="A Pytorch Backend Library for Choice Modelling",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://gsbdbi.github.io/torch-choice/",
     author="Tianyu Du, Ayush Kanodia, and Susan Athey",
     author_email="tianyudu@stanford.edu",
     license="MIT",
```

### Comparing `torch_choice-1.0.5/tests/test_choice_dataset.py` & `torch_choice-1.0.6/tests/test_choice_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.5/tests/test_conditional_logit_model.py` & `torch_choice-1.0.6/tests/test_conditional_logit_model.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.5/tests/test_nested_logit_model.py` & `torch_choice-1.0.6/tests/test_nested_logit_model.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.5/torch_choice/data/choice_dataset.py` & `torch_choice-1.0.6/torch_choice/data/choice_dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 The dataset object for management large scale consumer choice datasets.
 Please refer to the documentation and tutorials for more details on using `ChoiceDataset`.
 
 Author: Tianyu Du
 Update: Jan. 2, 2023
 """
 import copy
+import warnings
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import torch
 
 
@@ -202,15 +203,22 @@
 
         Returns:
             int: the number of users involved in this dataset.
         """
         if self._num_users is not None:
             return self._num_users
         elif self.user_index is not None:
-            # infer from the number of unique items in  user_index.
+            num_unique = len(torch.unique(self.user_index))
+            expected_num_users = int(self.user_index.max()) + 1
+            if num_unique != expected_num_users:
+                warnings.warn(f"The number of users is inferred from the number of unique users in the user_index tensor. The user_index tensor in the ChoiceDataset ranges from {int(self.user_index.min())} to {int(self.user_index.max())}. The ChoiceDataset assumes user_index to be 0-indexed and encoded using consecutive integers. There are {expected_num_users} users expected given max(user_index). However, there are {num_unique} unique values in the user_index . This could be caused by missing users in the dataset (i.e., some users are not in user_index at all). If this is not expected, please check the user_index tensor. For a safer behavior, please provide the number of users explicitly by using the num_users keyword while initializing the ChoiceDataset class.")
+            else:
+                warnings.warn(f"The number of users is inferred from the number of unique users in the user_index tensor. This might lead to unexpected behaviors if some users never appeared in the user_index tensor. For a safer behavior, please provide the number of users explicitly by using the num_users keyword while initializing the ChoiceDataset class.")
+
+            # infer from the number of unique users using the user_index.
             return len(torch.unique(self.user_index))
         else:
             return 1
 
     @property
     def num_items(self) -> int:
         """Returns the number of items involved in this dataset.
@@ -219,27 +227,41 @@
             int: the number of items involved in this dataset.
         """
         if self._num_items is not None:
             # return the _num_items provided in the constructor.
             return self._num_items
         else:
             # infer the number of items from item_index.
-            return len(torch.unique(self.item_index))
+            # the -1 is an optional special symbol for outside option, do not count it towards the number of items.
+            num_unique = len(torch.unique(self.item_index[self.item_index != -1]))
+            expected_num_items = int(self.item_index[self.item_index != -1].max()) + 1
+            if num_unique != expected_num_items:
+                warnings.warn(f"The number of items is inferred from the number of unique items, excluding -1's denoting outside options, in the item_index tensor. The item_index tensor in the ChoiceDataset ranges from {int(self.item_index[self.item_index != -1].min())} to {int(self.item_index[self.item_index != -1].max())}, excluding -1's. The ChoiceDataset assumes item_index to be 0-indexed and encoded using consecutive integers. There are {expected_num_items} items expected given max(item_index). However, there are {num_unique} unique values in item_index. This could be caused by missing items in the dataset (i.e., some items are not in item_index at all). If this is not expected, please check the item_index tensor. For a safer behavior, please provide the number of items explicitly by using the num_items keyword while initializing the ChoiceDataset class.")
+            else:
+                warnings.warn(f"The number of items is inferred from the number of unique items, excluding -1's denoting outside options, in the item_index tensor. This might lead to unexpected behaviors if some items never appeared in the item_index tensor. For a safer behavior, please provide the number of items explicitly by using the num_items keyword while initializing the ChoiceDataset class.")
+
+            return len(torch.unique(self.item_index[self.item_index != -1]))
 
     @property
     def num_sessions(self) -> int:
         """Returns the number of sessions involved in this dataset.
 
         Returns:
             int: the number of sessions involved in this dataset.
         """
         if self._num_sessions is not None:
             # return the _num_sessions provided in the constructor.
             return self._num_sessions
         else:
+            num_unique = len(torch.unique(self.session_index))
+            expected_num_sessions = int(self.session_index.max()) + 1
+            if num_unique != expected_num_sessions:
+                warnings.warn(f"The number of sessions is inferred from the number of unique sessions in the session_index tensor. The session_index tensor in the ChoiceDataset ranges from {int(self.session_index.min())} to {int(self.session_index.max())}. The ChoiceDataset assumes session_index to be 0-indexed and encoded using consecutive integers. There are {expected_num_sessions} sessions expected given max(session_index). However, there are {num_unique} unique values in the session_index . This could be caused by missing sessions in the dataset (i.e., some sessions are not in session_index at all). If this is not expected, please check the session_index tensor. For a safer behavior, please provide the number of sessions explicitly by using the num_sessions keyword while initializing the ChoiceDataset class.")
+            else:
+                warnings.warn(f"The number of sessions is inferred from the number of unique sessions in the session_index tensor. This might lead to unexpected behaviors if some sessions never appeared in the session_index tensor. For a safer behavior, please provide the number of sessions explicitly by using the num_sessions keyword while initializing the ChoiceDataset class.")
             # infer the number of sessions from session_index.
             return len(torch.unique(self.session_index))
 
     @property
     def x_dict(self) -> Dict[object, torch.Tensor]:
         """Formats attributes of in this dataset into shape (num_sessions, num_items, num_params) and returns in a dictionary format.
         Models in this package are expecting this dictionary based data format.
@@ -447,15 +469,15 @@
         elif self._is_usersessionitem_attribute(key):
             # usersessionitem_attribute has shape (num_users, num_sessions, num_items, *)
             out = val[self.user_index, self.session_index, :, :]  # (len(self), num_items, *)
 
         else:
             raise ValueError(f'Warning: the input key {key} is not an attribute of the dataset, will NOT modify the provided tensor.')
 
-        assert out.shape == (len(self), self.num_items, num_params)
+        assert out.shape == (len(self), self.num_items, num_params), f'Error: the output shape {out.shape} is not correct, expected: {(len(self), self.num_items, num_params)}.'
         return out
 
     @staticmethod
     def unique(tensor: torch.Tensor) -> Tuple[np.ndarray]:
         arr = tensor.cpu().numpy()
         unique, counts = np.unique(arr, return_counts=True)
         count_sort_ind = np.argsort(-counts)
```

### Comparing `torch_choice-1.0.5/torch_choice/data/example_datasets.py` & `torch_choice-1.0.6/torch_choice/data/example_datasets.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.5/torch_choice/data/joint_dataset.py` & `torch_choice-1.0.6/torch_choice/data/joint_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.5/torch_choice/data/utils.py` & `torch_choice-1.0.6/torch_choice/data/utils.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.5/torch_choice/model/coefficient.py` & `torch_choice-1.0.6/torch_choice/model/coefficient.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.5/torch_choice/model/conditional_logit_model.py` & `torch_choice-1.0.6/torch_choice/model/conditional_logit_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,15 +44,16 @@
                  dataset: Optional[ChoiceDataset]=None,
                  coef_variation_dict: Optional[Dict[str, str]]=None,
                  num_param_dict: Optional[Dict[str, int]]=None,
                  num_items: Optional[int]=None,
                  num_users: Optional[int]=None,
                  regularization: Optional[str]=None,
                  regularization_weight: Optional[float]=None,
-                 weight_initialization: Optional[Union[str, Dict[str, str]]]=None
+                 weight_initialization: Optional[Union[str, Dict[str, str]]]=None,
+                 model_outside_option: Optional[bool]=False
                  ) -> None:
         """
         Args:
             formula (str): a string representing the utility formula.
                 The formula consists of '(variable_name|variation)'s separated by '+', for example:
                 "(var1|item) + (var2|user) + (var3|constant)"
                 where the first part of each term is the name of the variable
@@ -102,14 +103,20 @@
                 is not None.
                 Defaults to None.
             weight_initialization (Optional[Union[str, Dict[str, str]]]): controls for how coefficients are initialized;
                 users can pass a string from {'normal', 'uniform', 'zero'} to initialize all coefficients in the same way.
                 Alternatively, users can pass a dictionary with keys exactly the same as the `coef_variation_dict` dictionary,
                 and values from {'normal', 'uniform', 'zero'} to initialize coefficients of different types of variables differently.
                 By default, all coefficients are initialized following a standard normal distribution.
+            model_outside_option (Optional[bool]): whether to explicitly model the outside option (i.e., the consumer did not buy anything).
+                To enable modeling outside option, the outside option is indicated by `item_index[n] == -1` in the item-index-tensor.
+                In this case, the item-index-tensor can contain values in `{-1, 0, 1, ..., num_items-1}`.
+                Otherwise, if the outside option is not modelled, the item-index-tensor should only contain values in `{0, 1, ..., num_items-1}`.
+                The utility of the outside option is always set to 0 while computing the probability.
+                By default, model_outside_option is set to False and the model does not model the outside option.
         """
         # ==============================================================================================================
         # Check that the model received a valid combination of inputs so that it can be initialized.
         # ==============================================================================================================
         if coef_variation_dict is None and formula is None:
             raise ValueError("Either coef_variation_dict or formula should be provided to specify the model.")
 
@@ -193,14 +200,15 @@
                                               num_items=self.num_items,
                                               num_users=self.num_users,
                                               num_params=self.num_param_dict[var_type],
                                               init=init)
         # A ModuleDict is required to properly register all trainable parameters.
         # self.parameter() will fail if a python dictionary is used instead.
         self.coef_dict = nn.ModuleDict(coef_dict)
+        self.model_outside_option = model_outside_option
 
     def __repr__(self) -> str:
         """Return a string representation of the model.
 
         Returns:
             str: the string representation of the model.
         """
@@ -271,14 +279,21 @@
                 manual_coef_value=None if manual_coef_value_dict is None else manual_coef_value_dict[var_type])
 
         assert total_utility.shape == (len(batch), self.num_items)
 
         if batch.item_availability is not None:
             # mask out unavailable items.
             total_utility[~batch.item_availability[batch.session_index, :]] = torch.finfo(total_utility.dtype).min / 2
+
+        # accommodate the outside option.
+        if self.model_outside_option:
+            # the outside option has zero utility.
+            util_zero = torch.zeros(total_utility.size(0), 1, device=batch.device)  # (len(batch), 1)  zero tensor.
+            # outside option is indicated by item_index == -1, we put it at the end.
+            total_utility = torch.cat((total_utility, util_zero), dim=1)  # (len(batch), num_items+1)
         return total_utility
 
 
     def negative_log_likelihood(self, batch: ChoiceDataset, y: torch.Tensor, is_train: bool=True) -> torch.Tensor:
         """Computes the log-likelihood for the batch and label.
         TODO: consider remove y, change to label.
         TODO: consider move this method outside the model, the role of the model is to compute the utility.
@@ -293,15 +308,23 @@
         """
         if is_train:
             self.train()
         else:
             self.eval()
         # (num_trips, num_items)
         total_utility = self.forward(batch)
+        # check shapes.
+        if self.model_outside_option:
+            assert total_utility.shape == (len(batch), self.num_items+1)
+            assert torch.all(total_utility[:, -1] == 0), "The last column of total_utility should be all zeros, which corresponds to the outside option."
+        else:
+            assert total_utility.shape == (len(batch), self.num_items)
         logP = torch.log_softmax(total_utility, dim=1)
+        # since y == -1 indicates the outside option and the last column of total_utility is the outside option, the following
+        # indexing should correctly retrieve the log-likelihood even for outside options.
         nll = - logP[torch.arange(len(y)), y].sum()
         return nll
 
     def loss(self, *args, **kwargs):
         """The loss function to be optimized. This is a wrapper of `negative_log_likelihood` + regularization loss if required."""
         nll = self.negative_log_likelihood(*args, **kwargs)
         if self.regularization is not None:
```

### Comparing `torch_choice-1.0.5/torch_choice/model/formula_parser.py` & `torch_choice-1.0.6/torch_choice/model/formula_parser.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.5/torch_choice/model/nested_logit_model.py` & `torch_choice-1.0.6/torch_choice/model/nested_logit_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,16 @@
                  nest_formula: Optional[str]=None,
                  dataset: Optional[JointDataset]=None,
                  num_users: Optional[int]=None,
                  shared_lambda: bool=False,
                  regularization: Optional[str]=None,
                  regularization_weight: Optional[float]=None,
                  nest_weight_initialization: Optional[Union[str, Dict[str, str]]]=None,
-                 item_weight_initialization: Optional[Union[str, Dict[str, str]]]=None
+                 item_weight_initialization: Optional[Union[str, Dict[str, str]]]=None,
+                 model_outside_option: Optional[bool]=False
                  ) -> None:
         """Initialization method of the nested logit model.
 
         Args:
             nest_to_item (Dict[object, List[int]]): a dictionary maps a nest ID to a list
                 of items IDs of the queried nest.
 
@@ -87,14 +88,21 @@
             regularization_weight (Optional[float]): the weight of parameter norm subtracted from the log-likelihood.
                 This term controls the strength of regularization. This argument is required if and only if regularization
                 is not None.
                 Defaults to None.
 
             {nest, item}_weight_initialization (Optional[Union[str, Dict[str, str]]]): methods to initialize the weights of
                 coefficients for {nest, item} level model. Please refer to the `weight_initialization` keyword in ConditionalLogitModel's documentation for more details.
+
+            model_outside_option (Optional[bool]): whether to explicitly model the outside option (i.e., the consumer did not buy anything).
+                To enable modeling outside option, the outside option is indicated by `item_index[n] == -1` in the item-index-tensor.
+                In this case, the item-index-tensor can contain values in `{-1, 0, 1, ..., num_items-1}`.
+                Otherwise, if the outside option is not modelled, the item-index-tensor should only contain values in `{0, 1, ..., num_items-1}`.
+                The utility of the outside option is always set to 0 while computing the probability.
+                By default, model_outside_option is set to False and the model does not model the outside option.
         """
         # handle nest level model.
         using_formula_to_initiate = (item_formula is not None) and (nest_formula is not None)
         if using_formula_to_initiate:
             # make sure that the research does not specify duplicated information, which might cause conflict.
             if (nest_coef_variation_dict is not None) or (item_coef_variation_dict is not None):
                 raise ValueError('You specify the {item, nest}_formula to initiate the model, you should not specify the {item, nest}_coef_variation_dict at the same time.')
@@ -154,14 +162,16 @@
         assert self.regularization in ['L1', 'L2', None], f"Provided regularization={self.regularization} is not allowed, allowed values are ['L1', 'L2', None]."
         self.regularization_weight = regularization_weight
         if (self.regularization is not None) and (self.regularization_weight is None):
             raise ValueError(f'You specified regularization type {self.regularization} without providing regularization_weight.')
         if (self.regularization is None) and (self.regularization_weight is not None):
             raise ValueError(f'You specified no regularization but you provide regularization_weight={self.regularization_weight}, you should leave regularization_weight as None if you do not want to regularize the model.')
 
+        self.model_outside_option = model_outside_option
+
     @property
     def num_params(self) -> int:
         """Get the total number of parameters. For example, if there is only an user-specific coefficient to be multiplied
         with the K-dimensional observable, then the total number of parameters would be K x number of users, assuming no
         intercept is involved.
 
         Returns:
@@ -297,15 +307,15 @@
         # compute item-specific utility (T, num_items).
         Y = torch.zeros(T, self.num_items).to(device)
         for var_type, coef in self.item_coef_dict.items():
             corresponding_observable = var_type.split("[")[0]
             Y += coef(item_x_dict[corresponding_observable], user_index)
 
         if item_availability is not None:
-            Y[~item_availability] =torch.finfo(Y.dtype).min / 2
+            Y[~item_availability] = torch.finfo(Y.dtype).min / 2
 
         # =============================================================================
         # compute the inclusive value of each nest.
         inclusive_value = dict()
         for k, Bk in self.nest_to_item.items():
             # for nest k, divide the Y of all items in Bk by lambda_k.
             Y[:, Bk] /= self.lambdas[k]
@@ -317,24 +327,37 @@
         I = torch.zeros(T, self.num_items).to(device)
         for k, Bk in self.nest_to_item.items():
             I[:, Bk] = inclusive_value[k].view(-1, 1)  # (T, |Bk|)
 
         # logP_item[t, i] = log P(ni|Bk), where Bk is the nest item i is in, n is the user in trip t.
         logP_item = Y - I  # (T, num_items)
 
+        if self.model_outside_option:
+            # if the model explicitly models the outside option, we need to add a column of zeros to logP_item.
+            # log P(ni|Bk) = 0 for the outside option since Y = 0 and the outside option has its own nest.
+            logP_item = torch.cat((logP_item, torch.zeros(T, 1).to(device)), dim=1)
+            assert logP_item.shape == (T, self.num_items+1)
+            assert torch.all(logP_item[:, -1] == 0)
+
         # =============================================================================
         # logP_nest[t, i] = log P(Bk), for item i in trip t, the probability of choosing the nest/bucket
         # item i belongs to. logP_nest has shape (T, num_items)
         # logit[t, i] = W[n, k] + lambda[k] I[n, k], where n is the user involved in trip t, k is
         # the nest item i belongs to.
         logit = torch.zeros(T, self.num_items).to(device)
         for k, Bk in self.nest_to_item.items():
             logit[:, Bk] = (W[:, k] + self.lambdas[k] * inclusive_value[k]).view(-1, 1)  # (T, |Bk|)
         # only count each nest once in the logsumexp within the nest level model.
         cols = [x[0] for x in self.nest_to_item.values()]
+        if self.model_outside_option:
+            # the last column corresponds to the outside option, which has W+lambda*I = 0 since W = I = Y = 0 for the outside option.
+            logit = torch.cat((logit, torch.zeros(T, 1).to(device)), dim=1)
+            assert logit.shape == (T, self.num_items+1)
+            # we have already added W+lambda*I for each "actual" nest, now we add the "fake" nest for the outside option.
+            cols.append(-1)
         logP_nest = logit - torch.logsumexp(logit[:, cols], dim=1, keepdim=True)
 
         # =============================================================================
         # compute the joint log P_{ni} as in the textbook.
         logP = logP_item + logP_nest
         self._clamp_called_flag = False
         return logP
@@ -368,14 +391,21 @@
         # compute the negative log-likelihood loss directly.
         if is_train:
             self.train()
         else:
             self.eval()
         # (num_trips, num_items)
         logP = self.forward(batch)
+        # check shapes
+        if self.model_outside_option:
+            assert logP.shape == (len(batch['item']), self.num_items+1)
+        else:
+            assert logP.shape == (len(batch['item']), self.num_items)
+        # since y == -1 indicates the outside option and the last column of total_utility is the outside option, the following
+        # indexing should correctly retrieve the log-likelihood even for outside options.
         nll = - logP[torch.arange(len(y)), y].sum()
         return nll
 
     def loss(self, *args, **kwargs):
         """The loss function to be optimized. This is a wrapper of `negative_log_likelihood` + regularization loss if required."""
         nll = self.negative_log_likelihood(*args, **kwargs)
         if self.regularization is not None:
```

### Comparing `torch_choice-1.0.5/torch_choice/utils/easy_data_wrapper.py` & `torch_choice-1.0.6/torch_choice/utils/easy_data_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,17 @@
                  user_observable_columns: Optional[List[str]] = None,
                  item_observable_columns: Optional[List[str]] = None,
                  useritem_observable_columns: Optional[List[str]] = None,
                  session_observable_columns: Optional[List[str]] = None,
                  price_observable_columns: Optional[List[str]] = None,
                  itemsession_observable_columns: Optional[List[str]] = None,
                  useritemsession_observable_columns: Optional[List[str]] = None,
+                 num_items: Optional[int] = None,
+                 num_users: Optional[int] = None,
+                 num_sessions: Optional[int] = None,
                  # Misc.
                  device: str = 'cpu'):
         """The initialization method of EasyDatasetWrapper.
 
         Args:
             main_data (pd.DataFrame): the main dataset holding all purchase records in a "long-format", each row of the
                 dataset is an item in a purchase record.
@@ -86,14 +89,20 @@
                 data-frame. The data wrapper will derive observable data from the main_data data-frame.
                 For example, with `user_observable_columns = ['feature_A', 'feature_B']`, this wrapper will create two user-specific
                 observable tensors derived from main_data['feature_A'] and main_data['feature_B'].
 
             The itemsession_observable_column is an alias for the `price_observable_column` argument for backward compatibility,
                 all elements of `itemsession_observable_columns` will be appended to `price_observable_column`.
 
+            num_items (Optional[int], optional): the number of items in the dataset to pass to the ChoiceDataset. Defaults to None.
+
+            num_users (Optional[int], optional): the number of users in the dataset to pass to the ChoiceDataset. Defaults to None.
+
+            num_sessions (Optional[int], optional): the number of sessions in the dataset to pass to the ChoiceDataset. Defaults to None.
+
         Raises:
             ValueError: _description_
         """
         if (useritem_observable_data is not None) or (useritemsession_observable_data is not None) or (useritem_observable_columns is not None) or (useritemsession_observable_columns is not None):
             raise NotImplementedError("The user-item and user-item-session observables are not yet supported in easy data wrapper. Please construct ChoiceDataset objects directly with tensors using the ChoiceDataset class to include these observables.")
 
         # read in data.
@@ -135,14 +144,18 @@
         self.derive_observable_from_main_data(item_observable_columns,
                                               user_observable_columns,
                                               session_observable_columns,
                                               price_observable_columns)
 
         self.observable_data_to_observable_tensors()
 
+        # read in explicit numbers of items, users, and sessions.
+        self._num_items = num_items
+        self._num_users = num_users
+        self._num_sessions = num_sessions
         self.create_choice_dataset()
         print('Finished Creating Choice Dataset.')
 
     def encode(self) -> None:
         """
         Encodes item names, user names, and session names to {0, 1, 2, ...} integers, item/user/session are encoded
         in alphabetical order.
@@ -330,27 +343,30 @@
             self.session_index = self.main_data.groupby(self.purchase_record_column)[self.session_index_column].first().loc[self.purchase_record_index].values
             self.session_index = self.session_name_encoder.transform(self.session_index)
 
         self.choice_dataset = ChoiceDataset(item_index=torch.LongTensor(self.item_index),
                                             user_index=torch.LongTensor(self.user_index) if self.user_index is not None else None,
                                             session_index=torch.LongTensor(self.session_index) if self.session_index is not None else None,
                                             item_availability=self.item_availability,
+                                            num_items=self._num_items,
+                                            num_users=self._num_users,
+                                            num_sessions=self._num_sessions,
                                             # keyword arguments for observables.
                                             **self.item_observable_tensors,
                                             **self.user_observable_tensors,
                                             **self.session_observable_tensors,
                                             **self.price_observable_tensors)
 
         self.choice_dataset.to(self.device)
 
     def get_item_availability_tensor(self) -> torch.BoolTensor:
         """Get the item availability tensor from the main_data data-frame."""
         if self.session_index_column is None:
             raise ValueError(f'Item availability cannot be constructed without session index column.')
-        A = self.main_data.pivot(self.session_index_column, self.item_name_column, self.choice_column)
+        A = self.main_data.pivot(index=self.session_index_column, columns=self.item_name_column, values=self.choice_column)
         return torch.BoolTensor(~np.isnan(A.values))
 
     def __len__(self):
         return len(self.purchase_record_index)
 
     def summary(self):
         print(f'* purchase record index range:', self.purchase_record_index[:3], '...', self.purchase_record_index[-3:])
```

### Comparing `torch_choice-1.0.5/torch_choice/utils/run_helper.py` & `torch_choice-1.0.6/torch_choice/utils/run_helper.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.5/torch_choice/utils/run_helper_lightning.py` & `torch_choice-1.0.6/torch_choice/utils/run_helper_lightning.py`

 * *Files 12% similar despite different names*

```diff
@@ -168,28 +168,46 @@
         return model
 
     # ==================================================================================================================
     # Construct standard error, z-value, and p-value of coefficients.
     # ==================================================================================================================
     # current methods of computing standard deviation will corrupt the model, load weights into another model for returning.
     state_dict = deepcopy(lightning_model.model.state_dict())
-    model_clone.load_state_dict(state_dict)
+    if "lambdas" in state_dict:
+        # if the model is using a specific lambda for each nest, it will create an additional `lambdas` tensor in the forward process.
+        # the forward method on `model_clone` has never been called, so it does not have the `lambdas` tensor.
+        # we need to drop the `lambdas` tensor from the state_dict to avoid the error while loading the state dict.
+        # The lambdas tensor is simply a copy of the lambda_weight in this case.
+        assert torch.all(state_dict["lambdas"] == state_dict["lambda_weight"]), \
+            f"lambdas and lambda_weight should be the same, maximum difference: {torch.max(torch.abs(state_dict['lambdas'] - state_dict['lambda_weight']))}: {state_dict['lambdas']=:}, {state_dict['lambda_weight']=:}"
+        state_dict.pop("lambdas")
+    model_clone.load_state_dict(state_dict, strict=True)
 
     # get mean of estimation.
     mean_dict = dict()
     for k, v in lightning_model.model.named_parameters():
         mean_dict[k] = v.clone()
 
     # estimate the standard error of the model.
     dataset_for_std = dataset_train.clone()
 
     if isinstance(model, ConditionalLogitModel):
         def nll_loss(model):
             y_pred = model(dataset_for_std)
-            return F.cross_entropy(y_pred, dataset_for_std.item_index, reduction='sum')
+            item_index = dataset_for_std.item_index.clone()
+            if model.model_outside_option:
+                assert y_pred.shape == (len(dataset_for_std), model.num_items+1)
+                # y_pred has shape (len(dataset_for_std.choice_set), model.num_items+1) since the last column is the probability of the outside option.
+                # F.cross_entropy is not smart enough to handle the -1 outside option in y.
+                # Even though y_pred[:, -1] nad y_pred[:, model.num_items] are the same, F.cross_entropy does not know.
+                # We need to fix it manually.
+                # manually modify the index for the outside option.
+                item_index[item_index == -1] = model.num_items
+
+            return F.cross_entropy(y_pred, item_index, reduction='sum')
     elif isinstance(model, NestedLogitModel):
         def nll_loss(model):
             d = dataset_for_std[torch.arange(len(dataset_for_std))]
             return model.negative_log_likelihood(d, d['item'].item_index)
     std_dict = parameter_std(model_clone, nll_loss)
 
     print('=' * 20, 'model results', '=' * 20)
```

### Comparing `torch_choice-1.0.5/torch_choice/utils/std.py` & `torch_choice-1.0.6/torch_choice/utils/std.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.5/torch_choice.egg-info/PKG-INFO` & `torch_choice-1.0.6/torch_choice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: torch-choice
-Version: 1.0.5
+Name: torch_choice
+Version: 1.0.6
 Summary: A Pytorch Backend Library for Choice Modelling
 Home-page: https://gsbdbi.github.io/torch-choice/
 Author: Tianyu Du, Ayush Kanodia, and Susan Athey
 Author-email: tianyudu@stanford.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -227,7 +227,22 @@
 We note the shapes/sizes of each of the components in the above model. Suppose there are U users, I items and S sessions; in this case, an item is one of the 10 possible digits, so I = 10; there is one user per session, so that U=S; and each session is an image being classified.
 Then,
 - $X^{session:pixelvalues}_{t}$ is a matrix of size (S) x (H x W) where H x W are the dimensions of the image being classified; its coefficient $\beta_i$ has item level vartiation and is of size (I) x (1)
 
 This is a classic problem used for exposition in Computer Science to motivate various Machine Learning models. There is no concept of a user in this setup. Our package allows for models of this nature and is fully usable for Machine Learning problems with added flexibility over [scikit-learn logistic regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html)
  -->
 We highly recommend users to go through [tutorials](https://github.com/gsbDBI/torch-choice/blob/main/tutorials) we prepared to get a better understanding of what the package offers. We present multiple examples, and for each case we specify the utility form.
+
+## Reproducibility
+The `torch-choice` package is built upon several dependencies that introduce randomness, you would need to fix random seeds for these packages for reproducibility:
+
+```python
+import random
+import numpy as np
+import torch
+
+SEED = 12345
+random.seed(SEED)
+np.random.seed(SEED)
+torch.manual_seed(SEED)
+torch.use_deterministic_algorithms(True)
+```
```

### Comparing `torch_choice-1.0.5/torch_choice.egg-info/SOURCES.txt` & `torch_choice-1.0.6/torch_choice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

