# Comparing `tmp/landmarkclassifier-2.1.0.tar.gz` & `tmp/landmarkclassifier-2.1.1.tar.gz`

## Comparing `landmarkclassifier-2.1.0.tar` & `landmarkclassifier-2.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/environment.yml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/LANDMark/LANDMark.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/LANDMark/__init__.py
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/LANDMark/lm_dtree_clfs.py
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/LANDMark/lm_linear_clfs.py
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/LANDMark/lm_nnet_clfs.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/LANDMark/lm_oracle_clfs.py
--rw-r--r--   0        0        0    29098 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/LANDMark/tree.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/LANDMark/utils.py
--rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/docs/API.md
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0    38524 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/notebooks/ExampleUsage.ipynb
--rw-r--r--   0        0        0   388411 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/notebooks/ParameterChoices.ipynb
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/notebooks/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/tests/__init__.py
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/tests/test_landmark.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/.gitignore
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/LICENSE
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/README.md
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/environment.yml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    11546 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/LANDMarkClassifier/LANDMark.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/LANDMarkClassifier/__init__.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/LANDMarkClassifier/lm_dtree_clfs.py
+-rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/LANDMarkClassifier/lm_linear_clfs.py
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/LANDMarkClassifier/lm_nnet_clfs.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/LANDMarkClassifier/lm_oracle_clfs.py
+-rw-r--r--   0        0        0    28252 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/LANDMarkClassifier/tree.py
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/LANDMarkClassifier/utils.py
+-rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/docs/API.md
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0    38524 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/notebooks/ExampleUsage.ipynb
+-rw-r--r--   0        0        0   388411 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/notebooks/ParameterChoices.ipynb
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/notebooks/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/tests/test_landmark.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/.gitignore
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/LICENSE
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/README.md
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5466 2020-02-02 00:00:00.000000 landmarkclassifier-2.1.1/PKG-INFO
```

### Comparing `landmarkclassifier-2.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `landmarkclassifier-2.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `landmarkclassifier-2.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.1.0/.github/workflows/ci.yml` & `landmarkclassifier-2.1.1/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     branches: [ main ]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.8, 3.9, 3.10, 3.11]
+        python-version: [3.10, 3.11, 3.12]
 
     steps:
     - uses: actions/checkout@v2
     - uses: conda-incubator/setup-miniconda@v2
       with:
         miniforge-variant: Mambaforge
         miniforge-version: latest
```

### Comparing `landmarkclassifier-2.1.0/.github/workflows/python-publish.yml` & `landmarkclassifier-2.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.1.0/LANDMark/LANDMark.py` & `landmarkclassifier-2.1.1/LANDMarkClassifier/LANDMark.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,331 +1,331 @@
-from __future__ import annotations
-
-import numpy as np
-
-from .utils import Ensemble
-from .tree import MTree
-
-from sklearn.base import ClassifierMixin, BaseEstimator
-from sklearn.metrics import balanced_accuracy_score
-from sklearn.utils import check_X_y
-from sklearn.utils.validation import check_is_fitted
-
-from typing import Optional, List
-
-from scipy.sparse import csr_array, issparse
-
-
-class LANDMarkClassifier(BaseEstimator, ClassifierMixin):
-    def __init__(
-        self,
-        n_estimators: int = 64,
-        min_samples_in_leaf: int = 5,
-        max_depth: Optional[int] = None,
-        max_features: float = 0.80,
-        min_gain: float = 0.0,
-        impurity: str = "gain",
-        q: float = 1.5,
-        use_oracle: bool = True,
-        use_lm_l2: bool = True,
-        use_lm_l1: bool = True,
-        minority_sz_lm: int = 6,
-        use_nnet: bool = True,
-        nnet_min_samples: int = 32,
-        minority_sz_nnet: int = 6,
-        use_etc: bool = True,
-        etc_max_depth: int = 5,
-        etc_max_trees: int = 128,
-        resampler=None,
-        use_cascade: bool = False,
-        n_jobs: int = 4,
-    ):
-        # Tree construction parameters
-        self.n_estimators = n_estimators
-        self.min_samples_in_leaf = min_samples_in_leaf
-        self.max_depth = max_depth
-        self.max_features = max_features
-        self.min_gain = min_gain
-        self.impurity = impurity
-        self.q = q
-        self.use_oracle = use_oracle
-        self.use_lm_l2 = use_lm_l2
-        self.use_lm_l1 = use_lm_l1
-        self.minority_sz_lm = minority_sz_lm
-        self.use_nnet = use_nnet
-        self.nnet_min_samples = nnet_min_samples
-        self.minority_sz_nnet = minority_sz_nnet
-        self.use_etc = use_etc
-        self.etc_max_depth = etc_max_depth
-        self.etc_max_trees = etc_max_trees
-        self.resampler = resampler
-        self.use_cascade = use_cascade
-
-        self.n_jobs = n_jobs
-
-    def fit(self, X: np.ndarray, y: np.ndarray) -> LANDMarkClassifier:
-        """
-        Parameters
-        -----------
-        X : Numpy array of samples with shape (n_samples, n_features)
-
-        y : Numpy array of class labels with shape (n_samples,)
-
-        Returns
-        -----------
-        self : object, the fitted model
-        """
-        X_checked, y_checked = self._check_params(X, y)
-
-        self.classes_ = np.unique(y_checked)
-
-        # Fit a model
-        self.estimators_ = Ensemble(
-            base_estimator=MTree(
-                min_samples_in_leaf=self.min_samples_in_leaf,
-                max_depth=self.max_depth,
-                max_features=self.max_features,
-                min_gain=self.min_gain,
-                impurity=self.impurity,
-                q=self.q,
-                use_oracle=self.use_oracle,
-                use_lm_l2=self.use_lm_l2,
-                use_lm_l1=self.use_lm_l1,
-                minority_sz_lm=self.minority_sz_lm,
-                use_nnet=self.use_nnet,
-                nnet_min_samples=self.nnet_min_samples,
-                minority_sz_nnet=self.minority_sz_nnet,
-                use_etc=self.use_etc,
-                etc_max_depth=self.etc_max_depth,
-                etc_max_trees=self.etc_max_trees,
-                resampler=self.resampler,
-                use_cascade=self.use_cascade,
-            ),
-            n_estimators=self.n_estimators,
-            class_names=self.classes_,
-            n_jobs=self.n_jobs,
-        )
-
-        self.estimators_.fit(X_checked, y_checked)
-
-        return self
-
-    def predict(self, X: np.ndarray) -> np.ndarray:
-        """
-        Parameters
-        -----------
-        X : Numpy array of samples with shape (n_samples, n_features)
-
-        Returns
-        -----------
-        predictions : Numpy array of predictions with shape (n_samples,)
-        """
-        check_is_fitted(self, attributes=["classes_", "estimators_"])
-
-        predictions = self.estimators_.predict(X)
-
-        return predictions
-
-    def predict_proba(self, X: np.ndarray) -> np.ndarray:
-        """
-        Parameters
-        -----------
-        X : Numpy array of samples with shape (n_samples, n_features)
-
-        Returns
-        -----------
-        predictions : Numpy array of probabilities with shape (n_samples, n_classes)
-        """
-        check_is_fitted(self, attributes=["classes_", "estimators_"])
-
-        predictions = self.estimators_.predict_proba(X)
-
-        return predictions
-
-    def score(self, X: np.ndarray, y: np.ndarray) -> float:
-        check_is_fitted(self, attributes=["classes_", "estimators_"])
-
-        score = balanced_accuracy_score(y, self.predict(X))
-
-        return score
-
-    def proximity(self, X: np.ndarray, prox_type: str = "path") -> np.ndarray:
-        check_is_fitted(self, attributes=["classes_", "estimators_"])
-
-        if prox_type == "terminal":
-            tree_mats = []
-
-            for estimator in self.estimators_.estimators_:
-                tree_mats.append(estimator.proximity(X, prox_type))
-
-            emb = np.hstack(tree_mats)
-
-            return csr_array(emb.astype(np.uint8))
-
-        elif prox_type == "path":
-            if hasattr(self, "node_set"):
-                embs = [
-                    est.proximity(X, prox_type) for est in self.estimators_.estimators_
-                ]
-
-                if X.ndim == 1:
-                    emb = np.zeros(shape=(1, len(self.node_set)), dtype=np.uint8)
-                else:
-                    emb = np.zeros(
-                        shape=(X.shape[0], len(self.node_set)), dtype=np.uint8
-                    )
-
-                for tree_emb in embs:
-                    for sample, nodes in tree_emb.items():
-                        for node in nodes:
-                            emb[sample, self.node_set[node]] = 1
-
-                return csr_array(emb)
-
-            else:
-                # Get the list of nodes associated with each sample in X
-                embs = [
-                    est.proximity(X, prox_type) for est in self.estimators_.estimators_
-                ]
-
-                # Create a list of all nodes across all trees in the forest
-                node_set = set()
-                [node_set.update(est.all_nodes) for est in self.estimators_.estimators_]
-
-                node_set = list(node_set)
-
-                # Create the embedding matrix
-                emb = np.zeros(shape=(X.shape[0], len(node_set)), dtype=np.uint8)
-
-                # Create a mapping between node id and index in the embedding matrix
-                self.node_set = {node: i for i, node in enumerate(node_set)}
-                
-                # Update the embedding matrix
-                for tree_emb in embs:
-                    for sample, nodes in tree_emb.items():
-                        for node in nodes:
-                            emb[sample, self.node_set[node]] = 1
-
-                return csr_array(emb)
-
-    def _check_params(
-        self, X: np.ndarray, y: np.ndarray
-    ) -> List[np.ndarray, np.ndarray]:
-        SUPPORTED_IMPURITY = {"gain", "gain-ratio", "tsallis", "tsallis-gain-ratio"}
-
-        # Check that X and y meet the minimum requirements
-        X_conv, y_conv = check_X_y(X, y, accept_sparse=True)
-
-        if not issparse(X_conv):
-            sparsity = 1.0 - (np.count_nonzero(X_conv) / X_conv.size)
-
-            if sparsity >= 0.9:
-                X_conv = csr_array(X_conv)
-
-        if not isinstance(self.n_estimators, int):
-            raise TypeError("'n_estimators' must be an integer.")
-
-        if isinstance(self.n_estimators, int):
-            if self.n_estimators <= 0:
-                raise ValueError("'n_estimators' must be greater than zero.")
-
-        if not isinstance(self.min_samples_in_leaf, int):
-            raise TypeError("'min_samples_in_leaf' must be an integer.")
-
-        if isinstance(self.min_samples_in_leaf, int):
-            if self.min_samples_in_leaf <= 0:
-                raise ValueError("'min_samples_in_leaf' must be greater than zero.")
-
-        if isinstance(self.max_depth, type(None)):
-            pass
-
-        elif isinstance(self.max_depth, int):
-            if self.max_depth <= 0:
-                raise ValueError("'max_depth' must be an greater than zero.")
-
-        else:
-            raise TypeError("'max_depth' must be an integer greater than zero or None.")
-
-        if not isinstance(self.max_features, float):
-            raise TypeError("'max_features' must be float.")
-
-        if isinstance(self.max_features, float):
-            if self.max_features <= 0 or self.max_features > 1:
-                raise ValueError(
-                    "'max_features' must be greater than zero but less than or equal to one."
-                )
-
-        if isinstance(self.min_gain, float):
-            if self.min_gain < 0:
-                raise ValueError("'min_gain' must be greater than or equal to zero.")
-
-        else:
-            raise TypeError("'min_gain' must be float.")
-
-        if isinstance(self.impurity, str):
-            if self.impurity not in SUPPORTED_IMPURITY:
-                raise ValueError(
-                    "Supplied 'impurity' is not supported. 'impurity' must be 'gain', 'gain-ratio', 'tsallis', or 'tsallis-gain-ratio'."
-                )
-
-        else:
-            raise TypeError(
-                "'impurity' must be 'gain', 'gain-ratio', 'tsallis', or 'tsallis-gain-ratio'."
-            )
-
-        if not isinstance(self.q, float):
-            raise TypeError("'q' must be float.")
-
-        if not isinstance(self.use_oracle, bool):
-            raise TypeError("'use_oracle' must be True or False.")
-
-        if not isinstance(self.use_lm_l2, bool):
-            raise TypeError("'use_lm_l2' must be True or False.")
-
-        if not isinstance(self.use_lm_l1, bool):
-            raise TypeError("'use_lm_l1' must be True or False.")
-
-        if not isinstance(self.use_nnet, bool):
-            raise TypeError("'use_nnet' must be True or False.")
-
-        if not isinstance(self.nnet_min_samples, int):
-            raise TypeError("'nnet_min_samples' must be an integer.")
-
-        if not isinstance(self.use_cascade, bool):
-            raise TypeError("'use_cascade' must be True or False.")
-
-        if isinstance(self.nnet_min_samples, int):
-            if self.nnet_min_samples <= 0:
-                raise ValueError("'nnet_min_samples' must be greater than zero.")
-
-        if not isinstance(self.use_etc, bool):
-            raise TypeError("'use_etc' must be True or False.")
-
-        if isinstance(self.etc_max_depth, int):
-            if self.etc_max_depth <= 0:
-                raise ValueError("'etc_max_depth' must be greater than zero.")
-
-        else:
-            if not isinstance(self.etc_max_depth, type(None)):
-                raise TypeError("'etc_max_depth' must be an integer.")
-
-        if not isinstance(self.etc_max_trees, int):
-            raise TypeError("'etc_max_trees' must be an integer.")
-
-        if isinstance(self.etc_max_trees, int):
-            if self.etc_max_trees <= 0:
-                raise ValueError("'etc_max_trees' must be greater than zero.")
-
-        if not isinstance(self.n_jobs, int):
-            raise TypeError("'n_jobs' must be an integer.")
-
-        if isinstance(self.n_jobs, int):
-            if self.n_jobs <= 0:
-                raise ValueError("'n_jobs' must be greater than zero.")
-
-        if isinstance(self.resampler, type(None)):
-            pass
-
-        elif hasattr(self.resampler, "fit_transform") is False:
-            raise ValueError("'resampler' must have a 'fit_transform(X, y)' function.")
-
-        return X_conv, y_conv
+from __future__ import annotations
+
+import numpy as np
+
+from .utils import Ensemble
+from .tree import MTree
+
+from sklearn.base import ClassifierMixin, BaseEstimator
+from sklearn.metrics import balanced_accuracy_score
+from sklearn.utils import check_X_y
+from sklearn.utils.validation import check_is_fitted
+
+from typing import Optional, List
+
+from scipy.sparse import csr_array, issparse
+
+
+class LANDMarkClassifier(BaseEstimator, ClassifierMixin):
+    def __init__(
+        self,
+        n_estimators: int = 64,
+        min_samples_in_leaf: int = 5,
+        max_depth: Optional[int] = None,
+        max_features: float = 0.80,
+        min_gain: float = 0.0,
+        impurity: str = "gain",
+        q: float = 1.5,
+        use_oracle: bool = True,
+        use_lm_l2: bool = True,
+        use_lm_l1: bool = True,
+        minority_sz_lm: int = 6,
+        use_nnet: bool = True,
+        nnet_min_samples: int = 32,
+        minority_sz_nnet: int = 6,
+        use_etc: bool = True,
+        etc_max_depth: int = 5,
+        etc_max_trees: int = 128,
+        resampler=None,
+        use_cascade: bool = False,
+        n_jobs: int = 4,
+    ):
+        # Tree construction parameters
+        self.n_estimators = n_estimators
+        self.min_samples_in_leaf = min_samples_in_leaf
+        self.max_depth = max_depth
+        self.max_features = max_features
+        self.min_gain = min_gain
+        self.impurity = impurity
+        self.q = q
+        self.use_oracle = use_oracle
+        self.use_lm_l2 = use_lm_l2
+        self.use_lm_l1 = use_lm_l1
+        self.minority_sz_lm = minority_sz_lm
+        self.use_nnet = use_nnet
+        self.nnet_min_samples = nnet_min_samples
+        self.minority_sz_nnet = minority_sz_nnet
+        self.use_etc = use_etc
+        self.etc_max_depth = etc_max_depth
+        self.etc_max_trees = etc_max_trees
+        self.resampler = resampler
+        self.use_cascade = use_cascade
+
+        self.n_jobs = n_jobs
+
+    def fit(self, X: np.ndarray, y: np.ndarray) -> LANDMarkClassifier:
+        """
+        Parameters
+        -----------
+        X : Numpy array of samples with shape (n_samples, n_features)
+
+        y : Numpy array of class labels with shape (n_samples,)
+
+        Returns
+        -----------
+        self : object, the fitted model
+        """
+        X_checked, y_checked = self._check_params(X, y)
+
+        self.classes_ = np.unique(y_checked)
+
+        # Fit a model
+        self.estimators_ = Ensemble(
+            base_estimator=MTree(
+                min_samples_in_leaf=self.min_samples_in_leaf,
+                max_depth=self.max_depth,
+                max_features=self.max_features,
+                min_gain=self.min_gain,
+                impurity=self.impurity,
+                q=self.q,
+                use_oracle=self.use_oracle,
+                use_lm_l2=self.use_lm_l2,
+                use_lm_l1=self.use_lm_l1,
+                minority_sz_lm=self.minority_sz_lm,
+                use_nnet=self.use_nnet,
+                nnet_min_samples=self.nnet_min_samples,
+                minority_sz_nnet=self.minority_sz_nnet,
+                use_etc=self.use_etc,
+                etc_max_depth=self.etc_max_depth,
+                etc_max_trees=self.etc_max_trees,
+                resampler=self.resampler,
+                use_cascade=self.use_cascade,
+            ),
+            n_estimators=self.n_estimators,
+            class_names=self.classes_,
+            n_jobs=self.n_jobs,
+        )
+
+        self.estimators_.fit(X_checked, y_checked)
+
+        return self
+
+    def predict(self, X: np.ndarray) -> np.ndarray:
+        """
+        Parameters
+        -----------
+        X : Numpy array of samples with shape (n_samples, n_features)
+
+        Returns
+        -----------
+        predictions : Numpy array of predictions with shape (n_samples,)
+        """
+        check_is_fitted(self, attributes=["classes_", "estimators_"])
+
+        predictions = self.estimators_.predict(X)
+
+        return predictions
+
+    def predict_proba(self, X: np.ndarray) -> np.ndarray:
+        """
+        Parameters
+        -----------
+        X : Numpy array of samples with shape (n_samples, n_features)
+
+        Returns
+        -----------
+        predictions : Numpy array of probabilities with shape (n_samples, n_classes)
+        """
+        check_is_fitted(self, attributes=["classes_", "estimators_"])
+
+        predictions = self.estimators_.predict_proba(X)
+
+        return predictions
+
+    def score(self, X: np.ndarray, y: np.ndarray) -> float:
+        check_is_fitted(self, attributes=["classes_", "estimators_"])
+
+        score = balanced_accuracy_score(y, self.predict(X))
+
+        return score
+
+    def proximity(self, X: np.ndarray, prox_type: str = "terminal") -> np.ndarray:
+        check_is_fitted(self, attributes=["classes_", "estimators_"])
+
+        if prox_type == "terminal":
+            tree_mats = []
+
+            for estimator in self.estimators_.estimators_:
+                tree_mats.append(estimator.proximity(X, prox_type))
+
+            emb = np.hstack(tree_mats)
+
+            return csr_array(emb.astype(np.uint8))
+
+        elif prox_type == "path":
+            if hasattr(self, "node_set"):
+                embs = [
+                    est.proximity(X, prox_type) for est in self.estimators_.estimators_
+                ]
+
+                if X.ndim == 1:
+                    emb = np.zeros(shape=(1, len(self.node_set)), dtype=np.uint8)
+                else:
+                    emb = np.zeros(
+                        shape=(X.shape[0], len(self.node_set)), dtype=np.uint8
+                    )
+
+                for tree_emb in embs:
+                    for sample, nodes in tree_emb.items():
+                        for node in nodes:
+                            emb[sample, self.node_set[node]] = 1
+
+                return csr_array(emb)
+
+            else:
+                # Get the list of nodes associated with each sample in X
+                embs = [
+                    est.proximity(X, prox_type) for est in self.estimators_.estimators_
+                ]
+
+                # Create a list of all nodes across all trees in the forest
+                node_set = set()
+                [node_set.update(est.all_nodes) for est in self.estimators_.estimators_]
+
+                node_set = list(node_set)
+
+                # Create the embedding matrix
+                emb = np.zeros(shape=(X.shape[0], len(node_set)), dtype=np.uint8)
+
+                # Create a mapping between node id and index in the embedding matrix
+                self.node_set = {node: i for i, node in enumerate(node_set)}
+                
+                # Update the embedding matrix
+                for tree_emb in embs:
+                    for sample, nodes in tree_emb.items():
+                        for node in nodes:
+                            emb[sample, self.node_set[node]] = 1
+
+                return csr_array(emb)
+
+    def _check_params(
+        self, X: np.ndarray, y: np.ndarray
+    ) -> List[np.ndarray, np.ndarray]:
+        SUPPORTED_IMPURITY = {"gain", "gain-ratio", "tsallis", "tsallis-gain-ratio"}
+
+        # Check that X and y meet the minimum requirements
+        X_conv, y_conv = check_X_y(X, y, accept_sparse=True)
+
+        if not issparse(X_conv):
+            sparsity = 1.0 - (np.count_nonzero(X_conv) / X_conv.size)
+
+            if sparsity >= 0.9:
+                X_conv = csr_array(X_conv)
+
+        if not isinstance(self.n_estimators, int):
+            raise TypeError("'n_estimators' must be an integer.")
+
+        if isinstance(self.n_estimators, int):
+            if self.n_estimators <= 0:
+                raise ValueError("'n_estimators' must be greater than zero.")
+
+        if not isinstance(self.min_samples_in_leaf, int):
+            raise TypeError("'min_samples_in_leaf' must be an integer.")
+
+        if isinstance(self.min_samples_in_leaf, int):
+            if self.min_samples_in_leaf <= 0:
+                raise ValueError("'min_samples_in_leaf' must be greater than zero.")
+
+        if isinstance(self.max_depth, type(None)):
+            pass
+
+        elif isinstance(self.max_depth, int):
+            if self.max_depth <= 0:
+                raise ValueError("'max_depth' must be an greater than zero.")
+
+        else:
+            raise TypeError("'max_depth' must be an integer greater than zero or None.")
+
+        if not isinstance(self.max_features, float):
+            raise TypeError("'max_features' must be float.")
+
+        if isinstance(self.max_features, float):
+            if self.max_features <= 0 or self.max_features > 1:
+                raise ValueError(
+                    "'max_features' must be greater than zero but less than or equal to one."
+                )
+
+        if isinstance(self.min_gain, float):
+            if self.min_gain < 0:
+                raise ValueError("'min_gain' must be greater than or equal to zero.")
+
+        else:
+            raise TypeError("'min_gain' must be float.")
+
+        if isinstance(self.impurity, str):
+            if self.impurity not in SUPPORTED_IMPURITY:
+                raise ValueError(
+                    "Supplied 'impurity' is not supported. 'impurity' must be 'gain', 'gain-ratio', 'tsallis', or 'tsallis-gain-ratio'."
+                )
+
+        else:
+            raise TypeError(
+                "'impurity' must be 'gain', 'gain-ratio', 'tsallis', or 'tsallis-gain-ratio'."
+            )
+
+        if not isinstance(self.q, float):
+            raise TypeError("'q' must be float.")
+
+        if not isinstance(self.use_oracle, bool):
+            raise TypeError("'use_oracle' must be True or False.")
+
+        if not isinstance(self.use_lm_l2, bool):
+            raise TypeError("'use_lm_l2' must be True or False.")
+
+        if not isinstance(self.use_lm_l1, bool):
+            raise TypeError("'use_lm_l1' must be True or False.")
+
+        if not isinstance(self.use_nnet, bool):
+            raise TypeError("'use_nnet' must be True or False.")
+
+        if not isinstance(self.nnet_min_samples, int):
+            raise TypeError("'nnet_min_samples' must be an integer.")
+
+        if not isinstance(self.use_cascade, bool):
+            raise TypeError("'use_cascade' must be True or False.")
+
+        if isinstance(self.nnet_min_samples, int):
+            if self.nnet_min_samples <= 0:
+                raise ValueError("'nnet_min_samples' must be greater than zero.")
+
+        if not isinstance(self.use_etc, bool):
+            raise TypeError("'use_etc' must be True or False.")
+
+        if isinstance(self.etc_max_depth, int):
+            if self.etc_max_depth <= 0:
+                raise ValueError("'etc_max_depth' must be greater than zero.")
+
+        else:
+            if not isinstance(self.etc_max_depth, type(None)):
+                raise TypeError("'etc_max_depth' must be an integer.")
+
+        if not isinstance(self.etc_max_trees, int):
+            raise TypeError("'etc_max_trees' must be an integer.")
+
+        if isinstance(self.etc_max_trees, int):
+            if self.etc_max_trees <= 0:
+                raise ValueError("'etc_max_trees' must be greater than zero.")
+
+        if not isinstance(self.n_jobs, int):
+            raise TypeError("'n_jobs' must be an integer.")
+
+        if isinstance(self.n_jobs, int):
+            if self.n_jobs <= 0:
+                raise ValueError("'n_jobs' must be greater than zero.")
+
+        if isinstance(self.resampler, type(None)):
+            pass
+
+        elif hasattr(self.resampler, "fit_transform") is False:
+            raise ValueError("'resampler' must have a 'fit_transform(X, y)' function.")
+
+        return X_conv, y_conv
```

### Comparing `landmarkclassifier-2.1.0/LANDMark/lm_dtree_clfs.py` & `landmarkclassifier-2.1.1/LANDMarkClassifier/lm_dtree_clfs.py`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.1.0/LANDMark/lm_linear_clfs.py` & `landmarkclassifier-2.1.1/LANDMarkClassifier/lm_linear_clfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             elif self.model_type == "ridge":
                 self.clf = RidgeClassifierCV(
                     alphas=(0.001, 0.01, 0.1, 1.0, 10, 100, 1000), cv=StratifiedKFold(5)
                 ).fit(X_re, y_re)
 
             elif self.model_type == "lsvc":
                 self.cv = GridSearchCV(
-                    LinearSVC(max_iter=2000),
+                    LinearSVC(max_iter=2000, dual="auto"),
                     param_grid={"C": [0.001, 0.01, 0.1, 1.0, 10, 100]},
                     cv=StratifiedKFold(5),
                 ).fit(X_re, y_re)
 
                 self.clf = self.cv.best_estimator_
 
             return self, self.decision_function(X)
```

### Comparing `landmarkclassifier-2.1.0/LANDMark/lm_nnet_clfs.py` & `landmarkclassifier-2.1.1/LANDMarkClassifier/lm_nnet_clfs.py`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.1.0/LANDMark/lm_oracle_clfs.py` & `landmarkclassifier-2.1.1/LANDMarkClassifier/lm_oracle_clfs.py`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.1.0/LANDMark/tree.py` & `landmarkclassifier-2.1.1/LANDMarkClassifier/tree.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,843 +1,843 @@
-import numpy as np
-
-from scipy.stats import entropy
-
-from random import choice
-
-from sklearn.base import ClassifierMixin, BaseEstimator, clone
-from sklearn.metrics import balanced_accuracy_score
-
-from .lm_linear_clfs import LMClassifier
-from .lm_oracle_clfs import RandomOracle
-from .lm_dtree_clfs import ETClassifier
-from .lm_nnet_clfs import ANNClassifier
-
-
-def tsallis_fun(N, N_lab, L, R, y, mode, q):
-    if q == 1:  # Special case
-        if "ratio" in mode.split("-"):
-            return entropy_fun(N, N_lab, L, R, y, "gain-ratio")
-
-        else:
-            return entropy_fun(N, N_lab, L, R, y, "gain")
-
-    scaler = 1 / (1 - q)
-
-    L_outcome, L_counts = np.unique(y[L], return_counts=True)
-    L_prob = L_counts / L_counts.sum()
-    H_L = (L_counts.sum() / N) * (scaler * (np.power(L_prob, q).sum() - 1))
-
-    R_outcome, R_counts = np.unique(y[R], return_counts=True)
-    R_prob = R_counts / R_counts.sum()
-    H_R = (R_counts.sum() / N) * (scaler * (np.power(R_prob, q).sum() - 1))
-
-    H_parent = scaler * (np.power(N_lab, q).sum() - 1)
-
-    IG = H_parent - H_R - H_L
-
-    if mode == "tsallis":
-        return IG
-
-    else:
-        norm_factor = np.asarray([(L_counts.sum() / N), (R_counts.sum() / N)])
-        norm_factor = 1 + (scaler * (np.power(norm_factor, q).sum() - 1))
-
-        GR = IG / norm_factor
-
-        return GR
-
-
-def entropy_fun(N, N_lab, L, R, y, mode):
-    L_outcome, L_counts = np.unique(y[L], return_counts=True)
-    L_prob = L_counts / L_counts.sum()
-    H_L = entropy(L_prob) * (L_counts.sum() / N)
-
-    R_outcome, R_counts = np.unique(y[R], return_counts=True)
-    R_prob = R_counts / R_counts.sum()
-    H_R = entropy(R_prob) * (R_counts.sum() / N)
-
-    H_parent = entropy(N_lab)
-
-    IG = H_parent - H_L - H_R
-
-    if mode == "gain":
-        return IG
-
-    else:
-        norm_factor = np.asarray([(L_counts.sum() / N), (R_counts.sum() / N)])
-        norm_factor = 1 + entropy(norm_factor)
-
-        GR = IG / norm_factor
-
-        return GR
-
-
-def purity_function(N, N_lab, L, R, y, purity_fun, q):
-    if purity_fun == "gain" or purity_fun == "gain-ratio":
-        return entropy_fun(N, N_lab, L, R, y, purity_fun)
-
-    elif purity_fun == "tsallis-gain-ratio" or purity_fun == "tsallis":
-        return tsallis_fun(N, N_lab, L, R, y, purity_fun, q)
-
-
-class PredictData:
-    def __init__(self, node_lab):
-        self.node_lab = node_lab
-
-    def predict(self, X):
-        predictions = np.asarray([self.node_lab for i in range(X.shape[0])])
-
-        return predictions
-
-
-class Node:
-    def __init__(self):
-        # Node parameters
-        self.c_choice = None
-
-        self.left = None
-        self.right = None
-
-        self.splitter = None
-        self.features = None
-        self.gain = None
-        self.split_type = None
-
-        self.terminal = False
-        self.label = None
-        self.node_id = None
-
-    # Select the best split point for a dataset
-    def get_split(
-        self,
-        X,
-        y,
-        min_samples_in_leaf,
-        max_depth,
-        max_features,
-        min_gain,
-        impurity,
-        q,
-        use_lm_l2,
-        use_lm_l1,
-        minority_sz_lm,
-        use_nnet,
-        nnet_min_samples,
-        minority_sz_nnet,
-        use_etc,
-        etc_max_depth,
-        etc_max_trees,
-        N,
-        current_depth,
-        use_oracle,
-        use_cascade,
-    ):
-        # Get the ID of the node
-        self.node_id = id(self)
-
-        # Prepare the list of hyperplanes, gains, and model types
-        hyperplane_list = []
-        gains = []
-        model_type = []
-
-        # Determine the counts of each class at this node
-        outcomes, counts_tr = np.unique(y, return_counts=True)
-        counts_sum = counts_tr.sum()
-        counts_prob = counts_tr / counts_sum
-        counts_min = np.min(counts_tr)
-
-        # Check if stopping criteria are met
-        if entropy(counts_prob) == 0:
-            leaf_predictions = PredictData(outcomes[np.argmax(counts_prob)])
-
-            self.label = leaf_predictions.predict
-            self.terminal = True
-
-            return self
-
-        if counts_sum < min_samples_in_leaf:
-            leaf_predictions = PredictData(outcomes[np.argmax(counts_prob)])
-
-            self.label = leaf_predictions.predict
-            self.terminal = True
-
-            return self
-
-        if counts_min <= 1:
-            leaf_predictions = PredictData(outcomes[np.argmax(counts_prob)])
-
-            self.label = leaf_predictions.predict
-            self.terminal = True
-
-            return self
-
-        if not isinstance(max_depth, type(None)) and current_depth >= max_depth:
-            leaf_predictions = PredictData(outcomes[np.argmax(counts_prob)])
-
-            self.label = leaf_predictions.predict
-            self.terminal = True
-
-            return self
-
-        # Otherwise split
-        else:
-            # Create a Random Oracle Splitter
-            if use_oracle:
-                self.splitter = RandomOracle(n_feat=max_features).fit(X, y)
-
-                D = self.splitter.decision_function(X)
-
-                # Extend X using the output of the decision function, D, if the cascade parameter is True
-                if use_cascade:
-                    X = np.hstack((X, D.reshape(-1, 1)))
-
-                L = np.where(D > 0, True, False)
-                R = np.where(D <= 0, True, False)
-
-                IG = purity_function(counts_sum, counts_prob, L, R, y, impurity, q)
-
-                self.gain = IG
-
-                # Recursivly split
-                self.left = Node().get_split(
-                    X[L],
-                    y[L],
-                    min_samples_in_leaf=min_samples_in_leaf,
-                    max_depth=max_depth,
-                    max_features=max_features,
-                    min_gain=min_gain,
-                    impurity=impurity,
-                    q=q,
-                    use_lm_l2=use_lm_l2,
-                    use_lm_l1=use_lm_l1,
-                    minority_sz_lm=minority_sz_lm,
-                    use_nnet=use_nnet,
-                    nnet_min_samples=nnet_min_samples,
-                    minority_sz_nnet=minority_sz_nnet,
-                    use_etc=use_etc,
-                    etc_max_depth=etc_max_depth,
-                    etc_max_trees=etc_max_trees,
-                    N=X.shape[0],
-                    current_depth=current_depth + 1,
-                    use_oracle=False,
-                    use_cascade=use_cascade,
-                )
-
-                self.right = Node().get_split(
-                    X[R],
-                    y[R],
-                    min_samples_in_leaf=min_samples_in_leaf,
-                    max_depth=max_depth,
-                    max_features=max_features,
-                    min_gain=min_gain,
-                    impurity=impurity,
-                    q=q,
-                    use_lm_l2=use_lm_l2,
-                    use_lm_l1=use_lm_l1,
-                    minority_sz_lm=minority_sz_lm,
-                    use_nnet=use_nnet,
-                    nnet_min_samples=nnet_min_samples,
-                    minority_sz_nnet=minority_sz_nnet,
-                    use_etc=use_etc,
-                    etc_max_depth=etc_max_depth,
-                    etc_max_trees=etc_max_trees,
-                    N=X.shape[0],
-                    current_depth=current_depth + 1,
-                    use_oracle=False,
-                    use_cascade=use_cascade,
-                )
-
-                return self
-
-            # Split using a Linear, Tree, or Neural Network Models
-            else:
-                self.c_choice = choice([i for i in range(outcomes.shape[0])])
-
-                # Train Linear Models - L2
-                if use_lm_l2:
-                    for clf in [
-                        LMClassifier(
-                            model_type="lr_l2",
-                            n_feat=max_features,
-                            minority=minority_sz_lm,
-                        ),
-                        LMClassifier(
-                            model_type="sgd_l2",
-                            n_feat=max_features,
-                            minority=minority_sz_lm,
-                        ),
-                        LMClassifier(
-                            model_type="ridge",
-                            n_feat=max_features,
-                            minority=minority_sz_lm,
-                        ),
-                        LMClassifier(
-                            model_type="lsvc",
-                            n_feat=max_features,
-                            minority=minority_sz_lm,
-                        ),
-                    ]:
-                        model, D = clf.fit(X, y)
-
-                        if not isinstance(D, type(None)):
-                            if D.ndim > 1:
-                                D = D[:, self.c_choice]
-
-                            L = np.where(D > 0, True, False)
-                            R = np.where(D <= 0, True, False)
-
-                            X_L_n = X[L].shape[0]
-                            X_R_n = X[R].shape[0]
-
-                            # Calculate Information Gain
-                            if X_L_n > 0 and X_R_n > 0:
-                                IG = purity_function(
-                                    counts_sum, counts_prob, L, R, y, impurity, q
-                                )
-
-                                gains.append(IG)
-                                hyperplane_list.append((model, L, R))
-                                model_type.append(model.model_type)
-
-                # Train Linear Models - L1 / ElasticNet
-                if use_lm_l1:
-                    for clf in [
-                        LMClassifier(
-                            model_type="lr_l1",
-                            n_feat=max_features,
-                            minority=minority_sz_lm,
-                        ),
-                        LMClassifier(
-                            model_type="sgd_l1",
-                            n_feat=max_features,
-                            minority=minority_sz_lm,
-                        ),
-                    ]:
-                        model, D = clf.fit(X, y)
-
-                        if not isinstance(D, type(None)):
-                            if D.ndim > 1:
-                                D = D[:, self.c_choice]
-
-                            L = np.where(D > 0, True, False)
-                            R = np.where(D <= 0, True, False)
-
-                            X_L_n = X[L].shape[0]
-                            X_R_n = X[R].shape[0]
-
-                            # Calculate Information Gain
-                            if X_L_n > 0 and X_R_n > 0:
-                                IG = purity_function(
-                                    counts_sum, counts_prob, L, R, y, impurity, q
-                                )
-
-                                gains.append(IG)
-                                hyperplane_list.append((model, L, R))
-                                model_type.append(model.model_type)
-
-                # Train a Neural Network
-                if use_nnet:
-                    if X.shape[0] >= nnet_min_samples:
-                        for clf in [
-                            ANNClassifier(
-                                n_feat=max_features,
-                                minority=minority_sz_nnet,
-                            )
-                        ]:
-                            model, D = clf.fit(X, y)
-
-                            if not isinstance(D, type(None)):
-                                if D.ndim > 1:
-                                    D = D[:, self.c_choice]
-
-                                L = np.where(D > 0, True, False)
-                                R = np.where(D <= 0, True, False)
-
-                                X_L_n = X[L].shape[0]
-                                X_R_n = X[R].shape[0]
-
-                                # Calculate Information Gain
-                                if X_L_n > 0 and X_R_n > 0:
-                                    IG = purity_function(
-                                        counts_sum, counts_prob, L, R, y, impurity, q
-                                    )
-
-                                    gains.append(IG)
-                                    hyperplane_list.append((model, L, R))
-                                    model_type.append(model.model_type)
-
-                # Train Decision Tree Models
-                if use_etc:
-                    for clf in [
-                        ETClassifier(
-                            n_feat=max_features,
-                            max_depth=etc_max_depth,
-                            max_trees=etc_max_trees,
-                        )
-                    ]:
-                        model, D = clf.fit(X, y)
-
-                        if not isinstance(D, type(None)):
-                            if D.ndim > 1:
-                                D = D[:, self.c_choice]
-
-                            L = np.where(D > 0, True, False)
-                            R = np.where(D <= 0, True, False)
-
-                            X_L_n = X[L].shape[0]
-                            X_R_n = X[R].shape[0]
-
-                            # Calculate Information Gain
-                            if X_L_n > 0 and X_R_n > 0:
-                                IG = purity_function(
-                                    counts_sum, counts_prob, L, R, y, impurity, q
-                                )
-
-                                gains.append(IG)
-                                hyperplane_list.append((model, L, R))
-                                model_type.append(model.model_type)
-
-                gains = np.asarray(gains)
-                hyperplane_list = np.asarray(hyperplane_list, dtype="object")
-                model_type = np.asarray(model_type, dtype=np.str)
-
-                # Ensure that there is at least one set of splits that meets the minimum gain criteria
-                gain_mask = np.where(gains >= min_gain, True, False)
-
-                # Split the node
-                if np.any(gain_mask):
-                    # Filter models using gain
-                    best_index = np.argmax(gains)
-                    best_gain = gains[best_index]
-                    best_gains = np.where(gains == best_gain, True, False)
-
-                    hyperplane_list = hyperplane_list[best_gains]
-
-                    best_hyperplane = choice(hyperplane_list)
-                    L = best_hyperplane[1]
-                    R = best_hyperplane[2]
-
-                    self.gain = best_gain
-                    self.splitter = best_hyperplane[0]
-
-                    # Append the output of the decision function to each dataframe
-                    if use_cascade:
-                        if isinstance(self.splitter, LMClassifier):
-                            X_cascade = self.splitter.decision_function(X)
-
-                            if X_cascade.ndim == 1:
-                                X_cascade = X_cascade.reshape(-1, 1)
-
-                        else:
-                            X_cascade = self.splitter.predict_proba(X)
-
-                        X_new = np.hstack((X, X_cascade))
-
-                    else:
-                        X_new = X
-
-                    # Recursivly split
-                    self.left = Node().get_split(
-                        X_new[L],
-                        y[L],
-                        min_samples_in_leaf=min_samples_in_leaf,
-                        max_depth=max_depth,
-                        max_features=max_features,
-                        min_gain=min_gain,
-                        impurity=impurity,
-                        q=q,
-                        use_lm_l2=use_lm_l2,
-                        use_lm_l1=use_lm_l1,
-                        minority_sz_lm=minority_sz_lm,
-                        use_nnet=use_nnet,
-                        nnet_min_samples=nnet_min_samples,
-                        minority_sz_nnet=minority_sz_nnet,
-                        use_etc=use_etc,
-                        etc_max_depth=etc_max_depth,
-                        etc_max_trees=etc_max_trees,
-                        N=X.shape[0],
-                        current_depth=current_depth + 1,
-                        use_oracle=use_oracle,
-                        use_cascade=use_cascade,
-                    )
-
-                    self.right = Node().get_split(
-                        X_new[R],
-                        y[R],
-                        min_samples_in_leaf=min_samples_in_leaf,
-                        max_depth=max_depth,
-                        max_features=max_features,
-                        min_gain=min_gain,
-                        impurity=impurity,
-                        q=q,
-                        use_lm_l2=use_lm_l2,
-                        use_lm_l1=use_lm_l1,
-                        minority_sz_lm=minority_sz_lm,
-                        use_nnet=use_nnet,
-                        nnet_min_samples=nnet_min_samples,
-                        minority_sz_nnet=minority_sz_nnet,
-                        use_etc=use_etc,
-                        etc_max_depth=etc_max_depth,
-                        etc_max_trees=etc_max_trees,
-                        N=X.shape[0],
-                        current_depth=current_depth + 1,
-                        use_oracle=use_oracle,
-                        use_cascade=use_cascade,
-                    )
-
-                    return self
-
-                # Create a Leaf
-                else:
-                    leaf_predictions = PredictData(outcomes[np.argmax(counts_prob)])
-
-                    self.label = leaf_predictions.predict
-                    self.terminal = True
-
-                    return self
-
-
-class MTree(ClassifierMixin, BaseEstimator):
-    def __init__(
-        self,
-        min_samples_in_leaf,
-        max_depth,
-        max_features,
-        min_gain,
-        impurity,
-        q,
-        use_oracle,
-        use_lm_l2,
-        use_lm_l1,
-        minority_sz_lm,
-        use_nnet,
-        nnet_min_samples,
-        minority_sz_nnet,
-        use_etc,
-        etc_max_depth,
-        etc_max_trees,
-        resampler,
-        use_cascade,
-    ):
-        self.min_samples_in_leaf = min_samples_in_leaf
-        self.max_depth = max_depth
-        self.max_features = max_features
-        self.min_gain = min_gain
-        self.impurity = impurity
-        self.q = q
-        self.use_oracle = use_oracle
-        self.use_lm_l2 = use_lm_l2
-        self.use_lm_l1 = use_lm_l1
-        self.minority_sz_lm = minority_sz_lm
-        self.use_nnet = use_nnet
-        self.nnet_min_samples = nnet_min_samples
-        self.minority_sz_nnet = minority_sz_nnet
-        self.use_etc = use_etc
-        self.etc_max_depth = etc_max_depth
-        self.etc_max_trees = etc_max_trees
-        self.resampler = resampler
-        self.use_cascade = use_cascade
-
-    def fit(self, X, y):
-        self.classes_ = np.unique(y)
-
-        # Increase diversity by resampling
-        if isinstance(self.resampler, type(None)):
-            X_re = X
-            y_re = y
-
-        else:
-            self.resampler = clone(self.resampler)
-
-            X_re, y_re = self.resampler.fit_resample(X, y)
-
-        # Create the root node
-        tree = Node()
-
-        # Begin Splitting
-        tree.get_split(
-            X=X_re,
-            y=y_re,
-            min_samples_in_leaf=self.min_samples_in_leaf,
-            max_depth=self.max_depth,
-            max_features=self.max_features,
-            min_gain=self.min_gain,
-            impurity=self.impurity,
-            q=self.q,
-            use_lm_l2=self.use_lm_l2,
-            use_lm_l1=self.use_lm_l1,
-            minority_sz_lm=self.minority_sz_lm,
-            use_nnet=self.use_nnet,
-            nnet_min_samples=self.nnet_min_samples,
-            minority_sz_nnet=self.minority_sz_nnet,
-            use_etc=self.use_etc,
-            etc_max_depth=self.etc_max_depth,
-            etc_max_trees=self.etc_max_trees,
-            N=X.shape[0],
-            current_depth=1,
-            use_oracle=self.use_oracle,
-            use_cascade=self.use_cascade,
-        )
-
-        self.LMTree = tree
-
-        self.all_nodes = self._get_all_nodes(self.LMTree)
-
-        self.terminal_nodes = [x[0] for x in self.all_nodes if x[1] == 1]
-        self.all_nodes = [x[0] for x in self.all_nodes]
-
-        return self
-
-    def _predict(self, X, current_node=None, samp_idx=None):
-        final_predictions = []
-
-        # Get a list of sample IDs if sample_index is not provided and set the node to the root of the tree
-        if isinstance(samp_idx, type(None)):
-            samp_idx = np.asarray([i for i in range(X.shape[0])])
-
-            current_node = self.LMTree
-
-        if current_node.terminal is False:
-            # Determine where each sample goes
-            D = current_node.splitter.decision_function(X)
-
-            if D.ndim > 1:
-                D = D[:, current_node.c_choice]
-
-            L = np.where(D > 0, True, False)
-            R = np.where(D <= 0, True, False)
-
-            # Append decision function data
-            if self.use_cascade:
-                if isinstance(current_node.splitter, LMClassifier) or isinstance(
-                    current_node.splitter, RandomOracle
-                ):
-                    C = current_node.splitter.decision_function(X)
-
-                    if C.ndim == 1:
-                        C = C.reshape(-1, 1)
-
-                else:
-                    C = current_node.splitter.predict_proba(X)
-
-                X_new = np.hstack((X, C))
-
-            else:
-                X_new = X
-
-            X_L = X_new[L]
-            left = samp_idx[L]
-
-            X_R = X_new[R]
-            right = samp_idx[R]
-
-            if left.shape[0] > 0:
-                predictions_left = self._predict(X_L, current_node.left, left)
-                final_predictions.extend(predictions_left)
-
-            if right.shape[0] > 0:
-                predictions_right = self._predict(X_R, current_node.right, right)
-                final_predictions.extend(predictions_right)
-
-        elif current_node.terminal:
-            predictions = current_node.label(X)
-            predictions = np.asarray(
-                [(samp_idx[i], prediction) for i, prediction in enumerate(predictions)]
-            )
-
-            return predictions
-
-        return final_predictions
-
-    def predict(self, X):
-        if hasattr(self.resampler, "transform"):
-            X_trf = self.resampler.transform(X)
-
-        else:
-            X_trf = X
-
-        tree_predictions = self._predict(X_trf)
-
-        tree_predictions = [(int(entry[0]), entry[1]) for entry in tree_predictions]
-        tree_predictions.sort()
-
-        return np.asarray(tree_predictions)[:, 1]
-
-    def score(self, X, y):
-        score = balanced_accuracy_score(y, self.predict(X))
-
-        return score
-
-    def _get_all_nodes(self, node):
-        node_list = set()
-
-        if node.terminal is False:
-            node_list.update([(node.node_id, 0)])
-
-            node_list = node_list.union(self._get_all_nodes(node.left))
-            node_list = node_list.union(self._get_all_nodes(node.right))
-
-        elif node.terminal:
-            node_list.update([(node.node_id, 1)])
-
-            return node_list
-
-        return node_list
-
-    def _proximity(self, X, current_node=None, samp_idx=None):
-        final_predictions = []
-
-        # Get a list of sample IDs if sample_index is not provided and set the node to the root of the tree
-        if isinstance(samp_idx, type(None)):
-            samp_idx = np.asarray([i for i in range(X.shape[0])])
-
-            current_node = self.LMTree
-
-        # Check if the node is a terminal node
-        if current_node.terminal is False:
-            # Determine where each sample goes
-            D = current_node.splitter.decision_function(X)
-
-            if D.ndim > 1:
-                D = D[:, current_node.c_choice]
-
-            L = np.where(D > 0, True, False)
-            R = np.where(D <= 0, True, False)
-
-            # Append decision function data
-            if self.use_cascade:
-                if isinstance(current_node.splitter, LMClassifier) or isinstance(
-                    current_node.splitter, RandomOracle
-                ):
-                    C = current_node.splitter.decision_function(X)
-
-                    if C.ndim == 1:
-                        C = C.reshape(-1, 1)
-
-                else:
-                    C = current_node.splitter.predict_proba(X)
-
-                X_new = np.hstack((X, C))
-
-            else:
-                X_new = X
-
-            X_L = X_new[L]
-            left = samp_idx[L]
-
-            X_R = X_new[R]
-            right = samp_idx[R]
-
-            if left.shape[0] > 0:
-                predictions_left = self._proximity(X_L, current_node.left, left)
-                final_predictions.extend(predictions_left)
-
-            if right.shape[0] > 0:
-                predictions_right = self._proximity(X_R, current_node.right, right)
-                final_predictions.extend(predictions_right)
-
-        elif current_node.terminal:
-            return [(entry, current_node.node_id) for entry in samp_idx]
-
-        return final_predictions
-
-    def _proximity_path(self, X, current_node=None, samp_idx=None):
-        final_predictions = []
-
-        # Get a list of sample IDs if sample_index is not provided and set the node to the root of the tree
-        if isinstance(samp_idx, type(None)):
-            samp_idx = np.asarray([i for i in range(X.shape[0])])
-
-            current_node = self.LMTree
-
-        # Check if the node is a terminal node
-        if current_node.terminal is False:
-            # Determine where each sample goes
-            D = current_node.splitter.decision_function(X)
-
-            if D.ndim > 1:
-                D = D[:, current_node.c_choice]
-
-            L = np.where(D > 0, True, False)
-            R = np.where(D <= 0, True, False)
-
-            # Append decision function data
-            if self.use_cascade:
-                if isinstance(current_node.splitter, LMClassifier) or isinstance(
-                    current_node.splitter, RandomOracle
-                ):
-                    C = current_node.splitter.decision_function(X)
-
-                    if C.ndim == 1:
-                        C = C.reshape(-1, 1)
-
-                else:
-                    C = current_node.splitter.predict_proba(X)
-
-                X_new = np.hstack((X, C))
-
-            else:
-                X_new = X
-
-            X_L = X_new[L]
-            left = samp_idx[L]
-
-            X_R = X_new[R]
-            right = samp_idx[R]
-
-            if left.shape[0] > 0:
-                final_predictions.extend(
-                    [(entry, current_node.node_id) for entry in samp_idx[L]]
-                )
-                predictions_left = self._proximity_path(X_L, current_node.left, left)
-                final_predictions.extend(predictions_left)
-
-            if right.shape[0] > 0:
-                final_predictions.extend(
-                    [(entry, current_node.node_id) for entry in samp_idx[R]]
-                )
-                predictions_right = self._proximity_path(X_R, current_node.right, right)
-                final_predictions.extend(predictions_right)
-
-        elif current_node.terminal:
-            return [(entry, current_node.node_id) for entry in samp_idx]
-
-        return final_predictions
-
-    def proximity(self, X, prox_type="path"):
-        if hasattr(self.resampler, "transform"):
-            X_trf = self.resampler.transform(X)
-
-        else:
-            X_trf = X
-
-        if prox_type == "terminal":
-            tree_predictions = self._proximity(X_trf)
-
-            tree_predictions.sort()
-
-            col_dict = {col: i for i, col in enumerate(self.terminal_nodes)}
-
-            emb_matrix = np.zeros(
-                shape=(X.shape[0], len(self.terminal_nodes)), dtype=np.ushort
-            )
-
-            for entry in tree_predictions:
-                row = entry[0]
-                col = col_dict[entry[1]]
-
-                emb_matrix[row, col] = 1
-
-            return emb_matrix
-
-        elif prox_type == "path":
-            tree_predictions = self._proximity_path(X_trf)
-
-            emb_matrix = {}
-            for sample in tree_predictions:
-                if sample[0] not in emb_matrix:
-                    emb_matrix[sample[0]] = set()
-
-                emb_matrix[sample[0]].add(sample[1])
-
-            return emb_matrix
+import numpy as np
+
+from scipy.stats import entropy
+
+from random import choice
+
+from sklearn.base import ClassifierMixin, BaseEstimator, clone
+from sklearn.metrics import balanced_accuracy_score
+
+from .lm_linear_clfs import LMClassifier
+from .lm_oracle_clfs import RandomOracle
+from .lm_dtree_clfs import ETClassifier
+from .lm_nnet_clfs import ANNClassifier
+
+
+def tsallis_fun(N, N_lab, L, R, y, mode, q):
+    if q == 1:  # Special case
+        if "ratio" in mode.split("-"):
+            return entropy_fun(N, N_lab, L, R, y, "gain-ratio")
+
+        else:
+            return entropy_fun(N, N_lab, L, R, y, "gain")
+
+    scaler = 1 / (1 - q)
+
+    L_outcome, L_counts = np.unique(y[L], return_counts=True)
+    L_prob = L_counts / L_counts.sum()
+    H_L = (L_counts.sum() / N) * (scaler * (np.power(L_prob, q).sum() - 1))
+
+    R_outcome, R_counts = np.unique(y[R], return_counts=True)
+    R_prob = R_counts / R_counts.sum()
+    H_R = (R_counts.sum() / N) * (scaler * (np.power(R_prob, q).sum() - 1))
+
+    H_parent = scaler * (np.power(N_lab, q).sum() - 1)
+
+    IG = H_parent - H_R - H_L
+
+    if mode == "tsallis":
+        return IG
+
+    else:
+        norm_factor = np.asarray([(L_counts.sum() / N), (R_counts.sum() / N)])
+        norm_factor = 1 + (scaler * (np.power(norm_factor, q).sum() - 1))
+
+        GR = IG / norm_factor
+
+        return GR
+
+
+def entropy_fun(N, N_lab, L, R, y, mode):
+    L_outcome, L_counts = np.unique(y[L], return_counts=True)
+    L_prob = L_counts / L_counts.sum()
+    H_L = entropy(L_prob) * (L_counts.sum() / N)
+
+    R_outcome, R_counts = np.unique(y[R], return_counts=True)
+    R_prob = R_counts / R_counts.sum()
+    H_R = entropy(R_prob) * (R_counts.sum() / N)
+
+    H_parent = entropy(N_lab)
+
+    IG = H_parent - H_L - H_R
+
+    if mode == "gain":
+        return IG
+
+    else:
+        norm_factor = np.asarray([(L_counts.sum() / N), (R_counts.sum() / N)])
+        norm_factor = 1 + entropy(norm_factor)
+
+        GR = IG / norm_factor
+
+        return GR
+
+
+def purity_function(N, N_lab, L, R, y, purity_fun, q):
+    if purity_fun == "gain" or purity_fun == "gain-ratio":
+        return entropy_fun(N, N_lab, L, R, y, purity_fun)
+
+    elif purity_fun == "tsallis-gain-ratio" or purity_fun == "tsallis":
+        return tsallis_fun(N, N_lab, L, R, y, purity_fun, q)
+
+
+class PredictData:
+    def __init__(self, node_lab):
+        self.node_lab = node_lab
+
+    def predict(self, X):
+        predictions = np.asarray([self.node_lab for i in range(X.shape[0])])
+
+        return predictions
+
+
+class Node:
+    def __init__(self):
+        # Node parameters
+        self.c_choice = None
+
+        self.left = None
+        self.right = None
+
+        self.splitter = None
+        self.features = None
+        self.gain = None
+        self.split_type = None
+
+        self.terminal = False
+        self.label = None
+        self.node_id = None
+
+    # Select the best split point for a dataset
+    def get_split(
+        self,
+        X,
+        y,
+        min_samples_in_leaf,
+        max_depth,
+        max_features,
+        min_gain,
+        impurity,
+        q,
+        use_lm_l2,
+        use_lm_l1,
+        minority_sz_lm,
+        use_nnet,
+        nnet_min_samples,
+        minority_sz_nnet,
+        use_etc,
+        etc_max_depth,
+        etc_max_trees,
+        N,
+        current_depth,
+        use_oracle,
+        use_cascade,
+    ):
+        # Get the ID of the node
+        self.node_id = id(self)
+
+        # Prepare the list of hyperplanes, gains, and model types
+        hyperplane_list = []
+        gains = []
+        model_type = []
+
+        # Determine the counts of each class at this node
+        outcomes, counts_tr = np.unique(y, return_counts=True)
+        counts_sum = counts_tr.sum()
+        counts_prob = counts_tr / counts_sum
+        counts_min = np.min(counts_tr)
+
+        # Check if stopping criteria are met
+        if entropy(counts_prob) == 0:
+            leaf_predictions = PredictData(outcomes[np.argmax(counts_prob)])
+
+            self.label = leaf_predictions.predict
+            self.terminal = True
+
+            return self
+
+        if counts_sum < min_samples_in_leaf:
+            leaf_predictions = PredictData(outcomes[np.argmax(counts_prob)])
+
+            self.label = leaf_predictions.predict
+            self.terminal = True
+
+            return self
+
+        if counts_min <= 1:
+            leaf_predictions = PredictData(outcomes[np.argmax(counts_prob)])
+
+            self.label = leaf_predictions.predict
+            self.terminal = True
+
+            return self
+
+        if not isinstance(max_depth, type(None)) and current_depth >= max_depth:
+            leaf_predictions = PredictData(outcomes[np.argmax(counts_prob)])
+
+            self.label = leaf_predictions.predict
+            self.terminal = True
+
+            return self
+
+        # Otherwise split
+        else:
+            # Create a Random Oracle Splitter
+            if use_oracle:
+                self.splitter = RandomOracle(n_feat=max_features).fit(X, y)
+
+                D = self.splitter.decision_function(X)
+
+                # Extend X using the output of the decision function, D, if the cascade parameter is True
+                if use_cascade:
+                    X = np.hstack((X, D.reshape(-1, 1)))
+
+                L = np.where(D > 0, True, False)
+                R = np.where(D <= 0, True, False)
+
+                IG = purity_function(counts_sum, counts_prob, L, R, y, impurity, q)
+
+                self.gain = IG
+
+                # Recursivly split
+                self.left = Node().get_split(
+                    X[L],
+                    y[L],
+                    min_samples_in_leaf=min_samples_in_leaf,
+                    max_depth=max_depth,
+                    max_features=max_features,
+                    min_gain=min_gain,
+                    impurity=impurity,
+                    q=q,
+                    use_lm_l2=use_lm_l2,
+                    use_lm_l1=use_lm_l1,
+                    minority_sz_lm=minority_sz_lm,
+                    use_nnet=use_nnet,
+                    nnet_min_samples=nnet_min_samples,
+                    minority_sz_nnet=minority_sz_nnet,
+                    use_etc=use_etc,
+                    etc_max_depth=etc_max_depth,
+                    etc_max_trees=etc_max_trees,
+                    N=X.shape[0],
+                    current_depth=current_depth + 1,
+                    use_oracle=False,
+                    use_cascade=use_cascade,
+                )
+
+                self.right = Node().get_split(
+                    X[R],
+                    y[R],
+                    min_samples_in_leaf=min_samples_in_leaf,
+                    max_depth=max_depth,
+                    max_features=max_features,
+                    min_gain=min_gain,
+                    impurity=impurity,
+                    q=q,
+                    use_lm_l2=use_lm_l2,
+                    use_lm_l1=use_lm_l1,
+                    minority_sz_lm=minority_sz_lm,
+                    use_nnet=use_nnet,
+                    nnet_min_samples=nnet_min_samples,
+                    minority_sz_nnet=minority_sz_nnet,
+                    use_etc=use_etc,
+                    etc_max_depth=etc_max_depth,
+                    etc_max_trees=etc_max_trees,
+                    N=X.shape[0],
+                    current_depth=current_depth + 1,
+                    use_oracle=False,
+                    use_cascade=use_cascade,
+                )
+
+                return self
+
+            # Split using a Linear, Tree, or Neural Network Models
+            else:
+                self.c_choice = choice([i for i in range(outcomes.shape[0])])
+
+                # Train Linear Models - L2
+                if use_lm_l2:
+                    for clf in [
+                        LMClassifier(
+                            model_type="lr_l2",
+                            n_feat=max_features,
+                            minority=minority_sz_lm,
+                        ),
+                        LMClassifier(
+                            model_type="sgd_l2",
+                            n_feat=max_features,
+                            minority=minority_sz_lm,
+                        ),
+                        LMClassifier(
+                            model_type="ridge",
+                            n_feat=max_features,
+                            minority=minority_sz_lm,
+                        ),
+                        LMClassifier(
+                            model_type="lsvc",
+                            n_feat=max_features,
+                            minority=minority_sz_lm,
+                        ),
+                    ]:
+                        model, D = clf.fit(X, y)
+
+                        if not isinstance(D, type(None)):
+                            if D.ndim > 1:
+                                D = D[:, self.c_choice]
+
+                            L = np.where(D > 0, True, False)
+                            R = np.where(D <= 0, True, False)
+
+                            X_L_n = X[L].shape[0]
+                            X_R_n = X[R].shape[0]
+
+                            # Calculate Information Gain
+                            if X_L_n > 0 and X_R_n > 0:
+                                IG = purity_function(
+                                    counts_sum, counts_prob, L, R, y, impurity, q
+                                )
+
+                                gains.append(IG)
+                                hyperplane_list.append((model, L, R))
+                                model_type.append(model.model_type)
+
+                # Train Linear Models - L1 / ElasticNet
+                if use_lm_l1:
+                    for clf in [
+                        LMClassifier(
+                            model_type="lr_l1",
+                            n_feat=max_features,
+                            minority=minority_sz_lm,
+                        ),
+                        LMClassifier(
+                            model_type="sgd_l1",
+                            n_feat=max_features,
+                            minority=minority_sz_lm,
+                        ),
+                    ]:
+                        model, D = clf.fit(X, y)
+
+                        if not isinstance(D, type(None)):
+                            if D.ndim > 1:
+                                D = D[:, self.c_choice]
+
+                            L = np.where(D > 0, True, False)
+                            R = np.where(D <= 0, True, False)
+
+                            X_L_n = X[L].shape[0]
+                            X_R_n = X[R].shape[0]
+
+                            # Calculate Information Gain
+                            if X_L_n > 0 and X_R_n > 0:
+                                IG = purity_function(
+                                    counts_sum, counts_prob, L, R, y, impurity, q
+                                )
+
+                                gains.append(IG)
+                                hyperplane_list.append((model, L, R))
+                                model_type.append(model.model_type)
+
+                # Train a Neural Network
+                if use_nnet:
+                    if X.shape[0] >= nnet_min_samples:
+                        for clf in [
+                            ANNClassifier(
+                                n_feat=max_features,
+                                minority=minority_sz_nnet,
+                            )
+                        ]:
+                            model, D = clf.fit(X, y)
+
+                            if not isinstance(D, type(None)):
+                                if D.ndim > 1:
+                                    D = D[:, self.c_choice]
+
+                                L = np.where(D > 0, True, False)
+                                R = np.where(D <= 0, True, False)
+
+                                X_L_n = X[L].shape[0]
+                                X_R_n = X[R].shape[0]
+
+                                # Calculate Information Gain
+                                if X_L_n > 0 and X_R_n > 0:
+                                    IG = purity_function(
+                                        counts_sum, counts_prob, L, R, y, impurity, q
+                                    )
+
+                                    gains.append(IG)
+                                    hyperplane_list.append((model, L, R))
+                                    model_type.append(model.model_type)
+
+                # Train Decision Tree Models
+                if use_etc:
+                    for clf in [
+                        ETClassifier(
+                            n_feat=max_features,
+                            max_depth=etc_max_depth,
+                            max_trees=etc_max_trees,
+                        )
+                    ]:
+                        model, D = clf.fit(X, y)
+
+                        if not isinstance(D, type(None)):
+                            if D.ndim > 1:
+                                D = D[:, self.c_choice]
+
+                            L = np.where(D > 0, True, False)
+                            R = np.where(D <= 0, True, False)
+
+                            X_L_n = X[L].shape[0]
+                            X_R_n = X[R].shape[0]
+
+                            # Calculate Information Gain
+                            if X_L_n > 0 and X_R_n > 0:
+                                IG = purity_function(
+                                    counts_sum, counts_prob, L, R, y, impurity, q
+                                )
+
+                                gains.append(IG)
+                                hyperplane_list.append((model, L, R))
+                                model_type.append(model.model_type)
+
+                gains = np.asarray(gains)
+                hyperplane_list = np.asarray(hyperplane_list, dtype="object")
+                model_type = np.asarray(model_type, dtype=str)
+
+                # Ensure that there is at least one set of splits that meets the minimum gain criteria
+                gain_mask = np.where(gains >= min_gain, True, False)
+
+                # Split the node
+                if np.any(gain_mask):
+                    # Filter models using gain
+                    best_index = np.argmax(gains)
+                    best_gain = gains[best_index]
+                    best_gains = np.where(gains == best_gain, True, False)
+
+                    hyperplane_list = hyperplane_list[best_gains]
+
+                    best_hyperplane = choice(hyperplane_list)
+                    L = best_hyperplane[1]
+                    R = best_hyperplane[2]
+
+                    self.gain = best_gain
+                    self.splitter = best_hyperplane[0]
+
+                    # Append the output of the decision function to each dataframe
+                    if use_cascade:
+                        if isinstance(self.splitter, LMClassifier):
+                            X_cascade = self.splitter.decision_function(X)
+
+                            if X_cascade.ndim == 1:
+                                X_cascade = X_cascade.reshape(-1, 1)
+
+                        else:
+                            X_cascade = self.splitter.predict_proba(X)
+
+                        X_new = np.hstack((X, X_cascade))
+
+                    else:
+                        X_new = X
+
+                    # Recursivly split
+                    self.left = Node().get_split(
+                        X_new[L],
+                        y[L],
+                        min_samples_in_leaf=min_samples_in_leaf,
+                        max_depth=max_depth,
+                        max_features=max_features,
+                        min_gain=min_gain,
+                        impurity=impurity,
+                        q=q,
+                        use_lm_l2=use_lm_l2,
+                        use_lm_l1=use_lm_l1,
+                        minority_sz_lm=minority_sz_lm,
+                        use_nnet=use_nnet,
+                        nnet_min_samples=nnet_min_samples,
+                        minority_sz_nnet=minority_sz_nnet,
+                        use_etc=use_etc,
+                        etc_max_depth=etc_max_depth,
+                        etc_max_trees=etc_max_trees,
+                        N=X.shape[0],
+                        current_depth=current_depth + 1,
+                        use_oracle=use_oracle,
+                        use_cascade=use_cascade,
+                    )
+
+                    self.right = Node().get_split(
+                        X_new[R],
+                        y[R],
+                        min_samples_in_leaf=min_samples_in_leaf,
+                        max_depth=max_depth,
+                        max_features=max_features,
+                        min_gain=min_gain,
+                        impurity=impurity,
+                        q=q,
+                        use_lm_l2=use_lm_l2,
+                        use_lm_l1=use_lm_l1,
+                        minority_sz_lm=minority_sz_lm,
+                        use_nnet=use_nnet,
+                        nnet_min_samples=nnet_min_samples,
+                        minority_sz_nnet=minority_sz_nnet,
+                        use_etc=use_etc,
+                        etc_max_depth=etc_max_depth,
+                        etc_max_trees=etc_max_trees,
+                        N=X.shape[0],
+                        current_depth=current_depth + 1,
+                        use_oracle=use_oracle,
+                        use_cascade=use_cascade,
+                    )
+
+                    return self
+
+                # Create a Leaf
+                else:
+                    leaf_predictions = PredictData(outcomes[np.argmax(counts_prob)])
+
+                    self.label = leaf_predictions.predict
+                    self.terminal = True
+
+                    return self
+
+
+class MTree(ClassifierMixin, BaseEstimator):
+    def __init__(
+        self,
+        min_samples_in_leaf,
+        max_depth,
+        max_features,
+        min_gain,
+        impurity,
+        q,
+        use_oracle,
+        use_lm_l2,
+        use_lm_l1,
+        minority_sz_lm,
+        use_nnet,
+        nnet_min_samples,
+        minority_sz_nnet,
+        use_etc,
+        etc_max_depth,
+        etc_max_trees,
+        resampler,
+        use_cascade,
+    ):
+        self.min_samples_in_leaf = min_samples_in_leaf
+        self.max_depth = max_depth
+        self.max_features = max_features
+        self.min_gain = min_gain
+        self.impurity = impurity
+        self.q = q
+        self.use_oracle = use_oracle
+        self.use_lm_l2 = use_lm_l2
+        self.use_lm_l1 = use_lm_l1
+        self.minority_sz_lm = minority_sz_lm
+        self.use_nnet = use_nnet
+        self.nnet_min_samples = nnet_min_samples
+        self.minority_sz_nnet = minority_sz_nnet
+        self.use_etc = use_etc
+        self.etc_max_depth = etc_max_depth
+        self.etc_max_trees = etc_max_trees
+        self.resampler = resampler
+        self.use_cascade = use_cascade
+
+    def fit(self, X, y):
+        self.classes_ = np.unique(y)
+
+        # Increase diversity by resampling
+        if isinstance(self.resampler, type(None)):
+            X_re = X
+            y_re = y
+
+        else:
+            self.resampler = clone(self.resampler)
+
+            X_re, y_re = self.resampler.fit_resample(X, y)
+
+        # Create the root node
+        tree = Node()
+
+        # Begin Splitting
+        tree.get_split(
+            X=X_re,
+            y=y_re,
+            min_samples_in_leaf=self.min_samples_in_leaf,
+            max_depth=self.max_depth,
+            max_features=self.max_features,
+            min_gain=self.min_gain,
+            impurity=self.impurity,
+            q=self.q,
+            use_lm_l2=self.use_lm_l2,
+            use_lm_l1=self.use_lm_l1,
+            minority_sz_lm=self.minority_sz_lm,
+            use_nnet=self.use_nnet,
+            nnet_min_samples=self.nnet_min_samples,
+            minority_sz_nnet=self.minority_sz_nnet,
+            use_etc=self.use_etc,
+            etc_max_depth=self.etc_max_depth,
+            etc_max_trees=self.etc_max_trees,
+            N=X.shape[0],
+            current_depth=1,
+            use_oracle=self.use_oracle,
+            use_cascade=self.use_cascade,
+        )
+
+        self.LMTree = tree
+
+        self.all_nodes = self._get_all_nodes(self.LMTree)
+
+        self.terminal_nodes = [x[0] for x in self.all_nodes if x[1] == 1]
+        self.all_nodes = [x[0] for x in self.all_nodes]
+
+        return self
+
+    def _predict(self, X, current_node=None, samp_idx=None):
+        final_predictions = []
+
+        # Get a list of sample IDs if sample_index is not provided and set the node to the root of the tree
+        if isinstance(samp_idx, type(None)):
+            samp_idx = np.asarray([i for i in range(X.shape[0])])
+
+            current_node = self.LMTree
+
+        if current_node.terminal is False:
+            # Determine where each sample goes
+            D = current_node.splitter.decision_function(X)
+
+            if D.ndim > 1:
+                D = D[:, current_node.c_choice]
+
+            L = np.where(D > 0, True, False)
+            R = np.where(D <= 0, True, False)
+
+            # Append decision function data
+            if self.use_cascade:
+                if isinstance(current_node.splitter, LMClassifier) or isinstance(
+                    current_node.splitter, RandomOracle
+                ):
+                    C = current_node.splitter.decision_function(X)
+
+                    if C.ndim == 1:
+                        C = C.reshape(-1, 1)
+
+                else:
+                    C = current_node.splitter.predict_proba(X)
+
+                X_new = np.hstack((X, C))
+
+            else:
+                X_new = X
+
+            X_L = X_new[L]
+            left = samp_idx[L]
+
+            X_R = X_new[R]
+            right = samp_idx[R]
+
+            if left.shape[0] > 0:
+                predictions_left = self._predict(X_L, current_node.left, left)
+                final_predictions.extend(predictions_left)
+
+            if right.shape[0] > 0:
+                predictions_right = self._predict(X_R, current_node.right, right)
+                final_predictions.extend(predictions_right)
+
+        elif current_node.terminal:
+            predictions = current_node.label(X)
+            predictions = np.asarray(
+                [(samp_idx[i], prediction) for i, prediction in enumerate(predictions)]
+            )
+
+            return predictions
+
+        return final_predictions
+
+    def predict(self, X):
+        if hasattr(self.resampler, "transform"):
+            X_trf = self.resampler.transform(X)
+
+        else:
+            X_trf = X
+
+        tree_predictions = self._predict(X_trf)
+
+        tree_predictions = [(int(entry[0]), entry[1]) for entry in tree_predictions]
+        tree_predictions.sort()
+
+        return np.asarray(tree_predictions)[:, 1]
+
+    def score(self, X, y):
+        score = balanced_accuracy_score(y, self.predict(X))
+
+        return score
+
+    def _get_all_nodes(self, node):
+        node_list = set()
+
+        if node.terminal is False:
+            node_list.update([(node.node_id, 0)])
+
+            node_list = node_list.union(self._get_all_nodes(node.left))
+            node_list = node_list.union(self._get_all_nodes(node.right))
+
+        elif node.terminal:
+            node_list.update([(node.node_id, 1)])
+
+            return node_list
+
+        return node_list
+
+    def _proximity(self, X, current_node=None, samp_idx=None):
+        final_predictions = []
+
+        # Get a list of sample IDs if sample_index is not provided and set the node to the root of the tree
+        if isinstance(samp_idx, type(None)):
+            samp_idx = np.asarray([i for i in range(X.shape[0])])
+
+            current_node = self.LMTree
+
+        # Check if the node is a terminal node
+        if current_node.terminal is False:
+            # Determine where each sample goes
+            D = current_node.splitter.decision_function(X)
+
+            if D.ndim > 1:
+                D = D[:, current_node.c_choice]
+
+            L = np.where(D > 0, True, False)
+            R = np.where(D <= 0, True, False)
+
+            # Append decision function data
+            if self.use_cascade:
+                if isinstance(current_node.splitter, LMClassifier) or isinstance(
+                    current_node.splitter, RandomOracle
+                ):
+                    C = current_node.splitter.decision_function(X)
+
+                    if C.ndim == 1:
+                        C = C.reshape(-1, 1)
+
+                else:
+                    C = current_node.splitter.predict_proba(X)
+
+                X_new = np.hstack((X, C))
+
+            else:
+                X_new = X
+
+            X_L = X_new[L]
+            left = samp_idx[L]
+
+            X_R = X_new[R]
+            right = samp_idx[R]
+
+            if left.shape[0] > 0:
+                predictions_left = self._proximity(X_L, current_node.left, left)
+                final_predictions.extend(predictions_left)
+
+            if right.shape[0] > 0:
+                predictions_right = self._proximity(X_R, current_node.right, right)
+                final_predictions.extend(predictions_right)
+
+        elif current_node.terminal:
+            return [(entry, current_node.node_id) for entry in samp_idx]
+
+        return final_predictions
+
+    def _proximity_path(self, X, current_node=None, samp_idx=None):
+        final_predictions = []
+
+        # Get a list of sample IDs if sample_index is not provided and set the node to the root of the tree
+        if isinstance(samp_idx, type(None)):
+            samp_idx = np.asarray([i for i in range(X.shape[0])])
+
+            current_node = self.LMTree
+
+        # Check if the node is a terminal node
+        if current_node.terminal is False:
+            # Determine where each sample goes
+            D = current_node.splitter.decision_function(X)
+
+            if D.ndim > 1:
+                D = D[:, current_node.c_choice]
+
+            L = np.where(D > 0, True, False)
+            R = np.where(D <= 0, True, False)
+
+            # Append decision function data
+            if self.use_cascade:
+                if isinstance(current_node.splitter, LMClassifier) or isinstance(
+                    current_node.splitter, RandomOracle
+                ):
+                    C = current_node.splitter.decision_function(X)
+
+                    if C.ndim == 1:
+                        C = C.reshape(-1, 1)
+
+                else:
+                    C = current_node.splitter.predict_proba(X)
+
+                X_new = np.hstack((X, C))
+
+            else:
+                X_new = X
+
+            X_L = X_new[L]
+            left = samp_idx[L]
+
+            X_R = X_new[R]
+            right = samp_idx[R]
+
+            if left.shape[0] > 0:
+                final_predictions.extend(
+                    [(entry, current_node.node_id) for entry in samp_idx[L]]
+                )
+                predictions_left = self._proximity_path(X_L, current_node.left, left)
+                final_predictions.extend(predictions_left)
+
+            if right.shape[0] > 0:
+                final_predictions.extend(
+                    [(entry, current_node.node_id) for entry in samp_idx[R]]
+                )
+                predictions_right = self._proximity_path(X_R, current_node.right, right)
+                final_predictions.extend(predictions_right)
+
+        elif current_node.terminal:
+            return [(entry, current_node.node_id) for entry in samp_idx]
+
+        return final_predictions
+
+    def proximity(self, X, prox_type="path"):
+        if hasattr(self.resampler, "transform"):
+            X_trf = self.resampler.transform(X)
+
+        else:
+            X_trf = X
+
+        if prox_type == "terminal":
+            tree_predictions = self._proximity(X_trf)
+
+            tree_predictions.sort()
+
+            col_dict = {col: i for i, col in enumerate(self.terminal_nodes)}
+
+            emb_matrix = np.zeros(
+                shape=(X.shape[0], len(self.terminal_nodes)), dtype=np.ushort
+            )
+
+            for entry in tree_predictions:
+                row = entry[0]
+                col = col_dict[entry[1]]
+
+                emb_matrix[row, col] = 1
+
+            return emb_matrix
+
+        elif prox_type == "path":
+            tree_predictions = self._proximity_path(X_trf)
+
+            emb_matrix = {}
+            for sample in tree_predictions:
+                if sample[0] not in emb_matrix:
+                    emb_matrix[sample[0]] = set()
+
+                emb_matrix[sample[0]].add(sample[1])
+
+            return emb_matrix
```

### Comparing `landmarkclassifier-2.1.0/LANDMark/utils.py` & `landmarkclassifier-2.1.1/LANDMarkClassifier/utils.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-import numpy as np
-
-##########################################################################################
-# For Bagging Classifier
-from sklearn.base import ClassifierMixin, BaseEstimator, clone
-from scipy.special import softmax
-from joblib import Parallel, delayed
-
-
-def _parallel_build(estimator, X, y):
-    return estimator.fit(X, y)
-
-
-class Ensemble(ClassifierMixin, BaseEstimator):
-    def __init__(self, base_estimator, n_estimators, class_names, n_jobs):
-        self.base_estimator = base_estimator
-        self.n_estimators = n_estimators
-        self.classes_ = class_names
-        self.n_jobs = n_jobs
-
-    def fit(self, X, y):
-        self.estimators_ = Parallel(n_jobs=self.n_jobs)(
-            delayed(_parallel_build)(clone(self.base_estimator), X, y)
-            for i in range(self.n_estimators)
-        )
-
-        return self
-
-    def predict(self, X):
-        prediction_probs = self.predict_proba(X)
-
-        max_probs = np.argmax(prediction_probs, axis=1)
-
-        predictions = [self.classes_[idx] for idx in max_probs]
-
-        predictions = np.asarray(predictions)
-
-        return predictions
-
-    def predict_proba(self, X):
-        class_map = {class_name: i for i, class_name in enumerate(self.classes_)}
-
-        # Returns an array that of shape (n_estimators, n_samples)
-        prediction_results = [
-            self.estimators_[i].predict(X) for i in range(self.n_estimators)
-        ]
-
-        prediction_results = np.asarray(prediction_results)
-
-        # Create an array that will hold all probabilities
-        prediction_probs = np.zeros(
-            shape=(X.shape[0], self.classes_.shape[0]), dtype=float
-        )
-
-        # Loop over samples and record the probabilities
-        for sample_num in range(prediction_results.shape[1]):
-            sample_pred = prediction_results[:, sample_num]
-
-            class_names, counts = np.unique(sample_pred, return_counts=True)
-            probs = counts / np.sum(counts)
-
-            if probs.shape[0] == self.classes_.shape[0]:
-                prediction_probs[sample_num] = probs
-
-            elif probs.shape[0] == 1:
-                index = class_map[class_names[0]]
-                prediction_probs[sample_num, index] = 1.0
-
-            else:
-                for idx, prob in enumerate(probs):
-                    index = class_map[class_names[idx]]
-                    prediction_probs[sample_num, index] = prob
-
-        # Ensure all probabilities sum to one
-        prediction_probs = softmax(prediction_probs, axis=1)
-
-        return prediction_probs
+import numpy as np
+
+##########################################################################################
+# For Bagging Classifier
+from sklearn.base import ClassifierMixin, BaseEstimator, clone
+from scipy.special import softmax
+from joblib import Parallel, delayed
+
+
+def _parallel_build(estimator, X, y):
+    return estimator.fit(X, y)
+
+
+class Ensemble(ClassifierMixin, BaseEstimator):
+    def __init__(self, base_estimator, n_estimators, class_names, n_jobs):
+        self.base_estimator = base_estimator
+        self.n_estimators = n_estimators
+        self.classes_ = class_names
+        self.n_jobs = n_jobs
+
+    def fit(self, X, y):
+        self.estimators_ = Parallel(n_jobs=self.n_jobs)(
+            delayed(_parallel_build)(clone(self.base_estimator), X, y)
+            for i in range(self.n_estimators)
+        )
+
+        return self
+
+    def predict(self, X):
+        prediction_probs = self.predict_proba(X)
+
+        max_probs = np.argmax(prediction_probs, axis=1)
+
+        predictions = [self.classes_[idx] for idx in max_probs]
+
+        predictions = np.asarray(predictions)
+
+        return predictions
+
+    def predict_proba(self, X):
+        class_map = {class_name: i for i, class_name in enumerate(self.classes_)}
+
+        # Returns an array that of shape (n_estimators, n_samples)
+        prediction_results = [
+            self.estimators_[i].predict(X) for i in range(self.n_estimators)
+        ]
+
+        prediction_results = np.asarray(prediction_results)
+
+        # Create an array that will hold all probabilities
+        prediction_probs = np.zeros(
+            shape=(X.shape[0], self.classes_.shape[0]), dtype=float
+        )
+
+        # Loop over samples and record the probabilities
+        for sample_num in range(prediction_results.shape[1]):
+            sample_pred = prediction_results[:, sample_num]
+
+            class_names, counts = np.unique(sample_pred, return_counts=True)
+            probs = counts / np.sum(counts)
+
+            if probs.shape[0] == self.classes_.shape[0]:
+                prediction_probs[sample_num] = probs
+
+            elif probs.shape[0] == 1:
+                index = class_map[class_names[0]]
+                prediction_probs[sample_num, index] = 1.0
+
+            else:
+                for idx, prob in enumerate(probs):
+                    index = class_map[class_names[idx]]
+                    prediction_probs[sample_num, index] = prob
+
+        # Ensure all probabilities sum to one
+        prediction_probs = softmax(prediction_probs, axis=1)
+
+        return prediction_probs
```

### Comparing `landmarkclassifier-2.1.0/docs/API.md` & `landmarkclassifier-2.1.1/docs/API.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.1.0/docs/CONTRIBUTING.md` & `landmarkclassifier-2.1.1/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.1.0/notebooks/ExampleUsage.ipynb` & `landmarkclassifier-2.1.1/notebooks/ExampleUsage.ipynb`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.1.0/notebooks/ParameterChoices.ipynb` & `landmarkclassifier-2.1.1/notebooks/ParameterChoices.ipynb`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.1.0/tests/test_landmark.py` & `landmarkclassifier-2.1.1/tests/test_landmark.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from LANDMark import LANDMarkClassifier
-from LANDMark.lm_nnet_clfs import ANNClassifier
-from LANDMark.lm_linear_clfs import LMClassifier
-from LANDMark.lm_oracle_clfs import RandomOracle
-from LANDMark.lm_dtree_clfs import ETClassifier
+from LANDMarkClassifier import LANDMarkClassifier
+from LANDMarkClassifier.lm_nnet_clfs import ANNClassifier
+from LANDMarkClassifier.lm_linear_clfs import LMClassifier
+from LANDMarkClassifier.lm_oracle_clfs import RandomOracle
+from LANDMarkClassifier.lm_dtree_clfs import ETClassifier
 
 from sklearn.datasets import load_wine, load_breast_cancer
 from sklearn.preprocessing import StandardScaler
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import balanced_accuracy_score
 
 from pathlib import Path
@@ -131,7 +131,8 @@
     D = clf.decision_function(X_test)
 
 
 test_models()
 
 test_landmark()
 
+fdfd = 5
```

### Comparing `landmarkclassifier-2.1.0/.gitignore` & `landmarkclassifier-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.1.0/LICENSE` & `landmarkclassifier-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.1.0/README.md` & `landmarkclassifier-2.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -31,14 +31,28 @@
 
 Examples of how to use `LANDMark` can be found [here](notebooks/README.md).
 
 ## Contributing
 
 To contribute to the development of `LANDMark` please read our [contributing guide](docs/CONTRIBUTING.md)
 
+### Projects Using LANDMark
+
+    Rudar J, Kruczkiewicz P, Vernygora O, Golding GB, Hajibabaei M, Lung O. Sequence signatures 
+    within the genome of SARS-CoV-2 can be used to predict host source. Microbiol Spectr. 
+    2024 Apr 2;12(4):e0358423. doi: 10.1128/spectrum.03584-23. Epub 2024 Mar 4. PMID: 38436242.
+
+    Rudar J, Golding GB, Kremer SC, Hajibabaei M. Decision Tree Ensembles Utilizing Multivariate 
+    Splits Are Effective at Investigating Beta Diversity in Medically Relevant 16S Amplicon 
+    Sequencing Data. Microbiol Spectr. 2023 Mar 6;11(2):e0206522. doi: 10.1128/spectrum.02065-22. 
+    Epub ahead of print. PMID: 36877086; PMCID: PMC10100742.
+
+    Rudar, J., Porter, T.M., Wright, M., Golding G.B., Hajibabaei, M. LANDMark: an ensemble 
+    approach to the supervised selection of biomarkers in high-throughput sequencing data. 
+    BMC Bioinformatics 23, 110 (2022). https://doi.org/10.1186/s12859-022-04631-z
 
 ### References
 
     Rudar, J., Porter, T.M., Wright, M., Golding G.B., Hajibabaei, M. LANDMark: an ensemble 
     approach to the supervised selection of biomarkers in high-throughput sequencing data. 
     BMC Bioinformatics 23, 110 (2022). https://doi.org/10.1186/s12859-022-04631-z
```

### Comparing `landmarkclassifier-2.1.0/pyproject.toml` & `landmarkclassifier-2.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "LANDMarkClassifier"
-version = "2.1.0"
+version = "2.1.1"
 authors = [
     {name = "Josip Rudar", email = "rudarj@uoguelph.ca"},
     {name = "Teresita M. Porter"},
     {name = "Michael Wright"},
     {name = "G. Brian Golding"},
     {name = "Mehrdad Hajibabaei", email = "mhajibab@uoguelph.ca"}
 ]
@@ -17,30 +17,29 @@
     "ecology",
     "multivariate statistics",
     "machine learning",
     "classification"
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
-    "numpy == 1.23.5",
+    "numpy >= 1.26",
     "scikit-learn >= 1.1.2",
     "joblib >= 1.2.0",
     "pandas >= 1.5.0",
     "scipy >= 1.8.1",
     "skorch >= 0.13.0",
     "torch >= 2.0.1"
 ]
@@ -60,14 +59,14 @@
 
 test = [
     "pytest",
     "pytest-cov"
 ]
 
 [tool.setuptools]
-py-modules = ["LANDMark"]
+py-modules = ["LANDMarkClassifier"]
 
 [tool.pytest.ini_options]
 addopts = "--cov --cov-report html --cov-report term-missing --cov-fail-under 30"
 
 [tool.coverage.run]
-source = ["LANDMark"]
+source = ["LANDMarkClassifier"]
```

### Comparing `landmarkclassifier-2.1.0/PKG-INFO` & `landmarkclassifier-2.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: LANDMarkClassifier
-Version: 2.1.0
+Version: 2.1.1
 Summary: LANDMark: An ensemble approach to the supervised selection of biomarkers in high-throughput sequencing data
 Project-URL: Homepage, https://github.com/jrudar/LANDMark
 Project-URL: Repository, https://github.com/jrudar/LANDMark.git
 Project-URL: Bug Tracker, https://github.com/jrudar/LANDMark/issues
 Author: Teresita M. Porter, Michael Wright, G. Brian Golding
 Author-email: Josip Rudar <rudarj@uoguelph.ca>, Mehrdad Hajibabaei <mhajibab@uoguelph.ca>
 License: MIT License
@@ -33,21 +33,20 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
 Requires-Dist: joblib>=1.2.0
-Requires-Dist: numpy==1.23.5
+Requires-Dist: numpy>=1.26
 Requires-Dist: pandas>=1.5.0
 Requires-Dist: scikit-learn>=1.1.2
 Requires-Dist: scipy>=1.8.1
 Requires-Dist: skorch>=0.13.0
 Requires-Dist: torch>=2.0.1
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
@@ -92,14 +91,28 @@
 
 Examples of how to use `LANDMark` can be found [here](notebooks/README.md).
 
 ## Contributing
 
 To contribute to the development of `LANDMark` please read our [contributing guide](docs/CONTRIBUTING.md)
 
+### Projects Using LANDMark
+
+    Rudar J, Kruczkiewicz P, Vernygora O, Golding GB, Hajibabaei M, Lung O. Sequence signatures 
+    within the genome of SARS-CoV-2 can be used to predict host source. Microbiol Spectr. 
+    2024 Apr 2;12(4):e0358423. doi: 10.1128/spectrum.03584-23. Epub 2024 Mar 4. PMID: 38436242.
+
+    Rudar J, Golding GB, Kremer SC, Hajibabaei M. Decision Tree Ensembles Utilizing Multivariate 
+    Splits Are Effective at Investigating Beta Diversity in Medically Relevant 16S Amplicon 
+    Sequencing Data. Microbiol Spectr. 2023 Mar 6;11(2):e0206522. doi: 10.1128/spectrum.02065-22. 
+    Epub ahead of print. PMID: 36877086; PMCID: PMC10100742.
+
+    Rudar, J., Porter, T.M., Wright, M., Golding G.B., Hajibabaei, M. LANDMark: an ensemble 
+    approach to the supervised selection of biomarkers in high-throughput sequencing data. 
+    BMC Bioinformatics 23, 110 (2022). https://doi.org/10.1186/s12859-022-04631-z
 
 ### References
 
     Rudar, J., Porter, T.M., Wright, M., Golding G.B., Hajibabaei, M. LANDMark: an ensemble 
     approach to the supervised selection of biomarkers in high-throughput sequencing data. 
     BMC Bioinformatics 23, 110 (2022). https://doi.org/10.1186/s12859-022-04631-z
```

