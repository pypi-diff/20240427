# Comparing `tmp/careamics_portfolio-0.0.8.tar.gz` & `tmp/careamics_portfolio-0.0.9.tar.gz`

## Comparing `careamics_portfolio-0.0.8.tar` & `careamics_portfolio-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/.copier-answers.yml
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/.github/dependabot.yml
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/.github/PR_TEMPLATE/pull_request.md
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/.github/workflows/datasets_ci.yml
--rw-r--r--   0        0        0    12056 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/datasets/datasets.json
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/examples/example.ipynb
--rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/scripts/update_json.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/scripts/update_registry.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/__init__.py
--rw-r--r--   0        0        0    11114 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/denoiseg_datasets.py
--rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/denoising_datasets.py
--rw-r--r--   0        0        0    13269 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/portfolio.py
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/portfolio_entry.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/py.typed
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/registry/registry.txt
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/utils/__init__.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/utils/download_utils.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/utils/pale_blue_dot.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/src/careamics_portfolio/utils/pale_blue_dot_zip.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/tests/conftest.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/tests/test_denoiseg_datasets.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/tests/test_denoising_datasets.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/tests/test_download_utils.py
--rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/tests/test_portfolio.py
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/tests/test_portfolio_entry.py
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/tests/utils.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/.gitignore
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/LICENSE
--rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/README.md
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/.copier-answers.yml
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/.github/dependabot.yml
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/.github/PR_TEMPLATE/pull_request.md
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/.github/workflows/datasets_ci.yml
+-rw-r--r--   0        0        0    12056 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/datasets/datasets.json
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/examples/example.ipynb
+-rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/scripts/update_json.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/scripts/update_registry.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/src/careamics_portfolio/__init__.py
+-rw-r--r--   0        0        0    11114 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/src/careamics_portfolio/denoiseg_datasets.py
+-rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/src/careamics_portfolio/denoising_datasets.py
+-rw-r--r--   0        0        0    13269 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/src/careamics_portfolio/portfolio.py
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/src/careamics_portfolio/portfolio_entry.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/src/careamics_portfolio/py.typed
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/src/careamics_portfolio/registry/registry.txt
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/src/careamics_portfolio/utils/__init__.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/src/careamics_portfolio/utils/download_utils.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/src/careamics_portfolio/utils/pale_blue_dot.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/src/careamics_portfolio/utils/pale_blue_dot_zip.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/tests/conftest.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/tests/test_denoiseg_datasets.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/tests/test_denoising_datasets.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/tests/test_download_utils.py
+-rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/tests/test_portfolio.py
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/tests/test_portfolio_entry.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/tests/utils.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/LICENSE
+-rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/README.md
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 careamics_portfolio-0.0.9/PKG-INFO
```

### Comparing `careamics_portfolio-0.0.8/.copier-answers.yml` & `careamics_portfolio-0.0.9/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/.pre-commit-config.yaml` & `careamics_portfolio-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md` & `careamics_portfolio-0.0.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md` & `careamics_portfolio-0.0.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/.github/PR_TEMPLATE/pull_request.md` & `careamics_portfolio-0.0.9/.github/PR_TEMPLATE/pull_request.md`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/.github/workflows/ci.yml` & `careamics_portfolio-0.0.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/.github/workflows/datasets_ci.yml` & `careamics_portfolio-0.0.9/.github/workflows/datasets_ci.yml`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/datasets/datasets.json` & `careamics_portfolio-0.0.9/datasets/datasets.json`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/examples/example.ipynb` & `careamics_portfolio-0.0.9/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/src/careamics_portfolio/__init__.py` & `careamics_portfolio-0.0.9/src/careamics_portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/src/careamics_portfolio/denoiseg_datasets.py` & `careamics_portfolio-0.0.9/src/careamics_portfolio/denoiseg_datasets.py`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/src/careamics_portfolio/denoising_datasets.py` & `careamics_portfolio-0.0.9/src/careamics_portfolio/denoising_datasets.py`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/src/careamics_portfolio/portfolio.py` & `careamics_portfolio-0.0.9/src/careamics_portfolio/portfolio.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,15 +348,15 @@
         -------
         N2V_RGB
             RGB dataset.
         """
         return self._N2V_RGB
 
     @property
-    def flywing(self) -> Flywing:
+    def Flywing(self) -> Flywing:
         """Flywing dataset.
 
         Returns
         -------
         Flywing
             Flywing dataset.
         """
```

### Comparing `careamics_portfolio-0.0.8/src/careamics_portfolio/portfolio_entry.py` & `careamics_portfolio-0.0.9/src/careamics_portfolio/portfolio_entry.py`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/src/careamics_portfolio/registry/registry.txt` & `careamics_portfolio-0.0.9/src/careamics_portfolio/registry/registry.txt`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/src/careamics_portfolio/utils/download_utils.py` & `careamics_portfolio-0.0.9/src/careamics_portfolio/utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/src/careamics_portfolio/utils/pale_blue_dot.py` & `careamics_portfolio-0.0.9/src/careamics_portfolio/utils/pale_blue_dot.py`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/src/careamics_portfolio/utils/pale_blue_dot_zip.py` & `careamics_portfolio-0.0.9/src/careamics_portfolio/utils/pale_blue_dot_zip.py`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/tests/conftest.py` & `careamics_portfolio-0.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/tests/test_denoiseg_datasets.py` & `careamics_portfolio-0.0.9/tests/test_denoiseg_datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     unique_hash_checker,
     unique_url_checker,
 )
 
 DATASETS = list(PortfolioManager().denoiseg)
 
 
-def all_datasets_getters(portfolio: PortfolioManager):
+def test_all_datasets_getters(portfolio: PortfolioManager):
     assert isinstance(portfolio.denoiseg.DSB2018_n0, PortfolioEntry)
     assert isinstance(portfolio.denoiseg.DSB2018_n10, PortfolioEntry)
     assert isinstance(portfolio.denoiseg.DSB2018_n20, PortfolioEntry)
     assert isinstance(portfolio.denoiseg.Flywing_n0, PortfolioEntry)
     assert isinstance(portfolio.denoiseg.Flywing_n10, PortfolioEntry)
     assert isinstance(portfolio.denoiseg.Flywing_n20, PortfolioEntry)
     assert isinstance(portfolio.denoiseg.MouseNuclei_n0, PortfolioEntry)
```

### Comparing `careamics_portfolio-0.0.8/tests/test_denoising_datasets.py` & `careamics_portfolio-0.0.9/tests/test_denoising_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,19 +9,19 @@
     unique_hash_checker,
     unique_url_checker,
 )
 
 DATASETS = list(PortfolioManager().denoising)
 
 
-def all_datasets_getters(portfolio: PortfolioManager):
+def test_all_datasets_getters(portfolio: PortfolioManager):
     assert isinstance(portfolio.denoising.N2V_SEM, PortfolioEntry)
     assert isinstance(portfolio.denoising.N2V_BSD68, PortfolioEntry)
     assert isinstance(portfolio.denoising.N2V_RGB, PortfolioEntry)
-    assert isinstance(portfolio.denoising.flywing, PortfolioEntry)
+    assert isinstance(portfolio.denoising.Flywing, PortfolioEntry)
     assert isinstance(portfolio.denoising.Convallaria, PortfolioEntry)
 
 
 @pytest.mark.dataset
 @pytest.mark.parametrize("dataset", DATASETS)
 def test_datasets(tmp_path, dataset: PortfolioEntry):
     """Test that all denoising datasets download properly.
```

### Comparing `careamics_portfolio-0.0.8/tests/test_download_utils.py` & `careamics_portfolio-0.0.9/tests/test_download_utils.py`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/tests/test_portfolio.py` & `careamics_portfolio-0.0.9/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/tests/test_portfolio_entry.py` & `careamics_portfolio-0.0.9/tests/test_portfolio_entry.py`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/tests/utils.py` & `careamics_portfolio-0.0.9/tests/utils.py`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/.gitignore` & `careamics_portfolio-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/LICENSE` & `careamics_portfolio-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/README.md` & `careamics_portfolio-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/pyproject.toml` & `careamics_portfolio-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `careamics_portfolio-0.0.8/PKG-INFO` & `careamics_portfolio-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: careamics-portfolio
-Version: 0.0.8
+Version: 0.0.9
 Summary: A helper package to download example datasets used in various publications and deep-learning algorithms, including data featured in N2V, P(P)N2V, DivNoising, HDN, EmbedSeg, etc.
 Project-URL: homepage, https://github.com/juglab-torch/careamics-portfolio
 Project-URL: repository, https://github.com/juglab-torch/careamics-portfolio
 Author-email: Joran Deschamps <joran.deschamps@fht.org>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

