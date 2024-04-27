# Comparing `tmp/PythonicDISORT-0.6.2.tar.gz` & `tmp/pythonicdisort-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonicDISORT-0.6.2.tar", last modified: Tue Mar 19 19:28:05 2024, max compression
+gzip compressed data, was "pythonicdisort-0.7.0.tar", last modified: Sat Apr 27 03:59:06 2024, max compression
```

## Comparing `PythonicDISORT-0.6.2.tar` & `pythonicdisort-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:28:05.693571 PythonicDISORT-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-19 19:27:49.000000 PythonicDISORT-0.6.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-03-19 19:28:05.693571 PythonicDISORT-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-03-19 19:27:49.000000 PythonicDISORT-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-19 19:27:50.000000 PythonicDISORT-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 19:28:05.693571 PythonicDISORT-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:28:05.689571 PythonicDISORT-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:28:05.689571 PythonicDISORT-0.6.2/src/PythonicDISORT/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-19 19:27:50.000000 PythonicDISORT-0.6.2/src/PythonicDISORT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14849 2024-03-19 19:27:50.000000 PythonicDISORT-0.6.2/src/PythonicDISORT/_assemble_solution_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-03-19 19:27:50.000000 PythonicDISORT-0.6.2/src/PythonicDISORT/_diagonalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    15014 2024-03-19 19:27:50.000000 PythonicDISORT-0.6.2/src/PythonicDISORT/_solve_for_coefs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24295 2024-03-19 19:27:50.000000 PythonicDISORT-0.6.2/src/PythonicDISORT/pydisort.py
--rw-r--r--   0 runner    (1001) docker     (127)    13295 2024-03-19 19:27:50.000000 PythonicDISORT-0.6.2/src/PythonicDISORT/subroutines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:28:05.693571 PythonicDISORT-0.6.2/src/PythonicDISORT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-03-19 19:28:05.000000 PythonicDISORT-0.6.2/src/PythonicDISORT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-19 19:28:05.000000 PythonicDISORT-0.6.2/src/PythonicDISORT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 19:28:05.000000 PythonicDISORT-0.6.2/src/PythonicDISORT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-19 19:28:05.000000 PythonicDISORT-0.6.2/src/PythonicDISORT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-19 19:28:05.000000 PythonicDISORT-0.6.2/src/PythonicDISORT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:59:06.037189 pythonicdisort-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-27 03:58:55.000000 pythonicdisort-0.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-27 03:59:06.037189 pythonicdisort-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-27 03:58:55.000000 pythonicdisort-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-27 03:58:55.000000 pythonicdisort-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 03:59:06.037189 pythonicdisort-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:59:06.033189 pythonicdisort-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:59:06.037189 pythonicdisort-0.7.0/src/PythonicDISORT/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-27 03:58:55.000000 pythonicdisort-0.7.0/src/PythonicDISORT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20410 2024-04-27 03:58:55.000000 pythonicdisort-0.7.0/src/PythonicDISORT/_assemble_intensity_and_fluxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19162 2024-04-27 03:58:55.000000 pythonicdisort-0.7.0/src/PythonicDISORT/_solve_for_coeffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12841 2024-04-27 03:58:55.000000 pythonicdisort-0.7.0/src/PythonicDISORT/_solve_for_gen_and_part_sols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27880 2024-04-27 03:58:55.000000 pythonicdisort-0.7.0/src/PythonicDISORT/pydisort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15857 2024-04-27 03:58:55.000000 pythonicdisort-0.7.0/src/PythonicDISORT/subroutines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:59:06.037189 pythonicdisort-0.7.0/src/PythonicDISORT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-27 03:59:06.000000 pythonicdisort-0.7.0/src/PythonicDISORT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-27 03:59:06.000000 pythonicdisort-0.7.0/src/PythonicDISORT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 03:59:06.000000 pythonicdisort-0.7.0/src/PythonicDISORT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-27 03:59:06.000000 pythonicdisort-0.7.0/src/PythonicDISORT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-27 03:59:06.000000 pythonicdisort-0.7.0/src/PythonicDISORT.egg-info/top_level.txt
```

### Comparing `PythonicDISORT-0.6.2/LICENSE.md` & `pythonicdisort-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PythonicDISORT-0.6.2/PKG-INFO` & `pythonicdisort-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonicDISORT
-Version: 0.6.2
+Version: 0.7.0
 Summary: Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere.
 Author-email: Dion HO Jia Xu <dh3065@columbia.edu>
 Project-URL: Homepage, https://github.com/LDEO-CREW/Pythonic-DISORT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -42,31 +42,31 @@
 of our GitHub repository.
 The Jupyter Notebook provides comprehensive documentation, suggested inputs, explanations, 
 mathematical derivations and verification tests.
 We highly recommend reading the non-optional parts of sections 1 and 2 before use.
 
 ## PyTest and examples of how to use PythonicDISORT
 
-Not only do we have verification tests in the Jupyter Notebook, we also used PyTest to recreate most of the test problems in Stamnes' `disotest.f90`; 
+Not only do we have verification tests in the Jupyter Notebook, we have also recreated most of the test problems in Stamnes' `disotest.f90`; 
 `disotest.f90` is included in the `disort4.0.99_f2py` directory of our GitHub repository. In these tests, the solutions from PythonicDISORT are compared 
 against solutions from our F2PY-wrapped Stamnes' DISORT (version 4.0.99). With PyTest installed, execute the console command `pytest` 
 in the `pydisotest` directory to run these tests. The `pydisotest` directory also contains Jupyter Notebooks, one for each test, 
 to show how the tests were implemented. These notebooks double up as examples of how to use PythonicDISORT.
 
 # Installation
 
 * From PyPI: `pip install PythonicDISORT`
 * From Conda-forge: (TODO: we need to first publish on Conda-forge)
-* By cloning repository: `pip install .` in the `Pythonic-DISORT` directory; `pip install -r all_optional_dependencies.txt` to install all optional dependencies
+* By cloning repository: `pip install .` in the `Pythonic-DISORT` directory; `pip install -r all_optional_dependencies.txt` to install all optional dependencies (see *Requirements to run PythonicDISORT*)
 
 ## Requirements to run PythonicDISORT
 * Python 3.8+
 * `numpy >= 1.8.0`
 * `scipy >= 1.8.0`
-* (OPTIONAL) `pytest >= 6.2.5` (Required for non-Notebook tests)
+* (OPTIONAL) `pytest >= 6.2.5` (Required to use the command `pytest`, see *PyTest and examples of how to use PythonicDISORT*)
 
 ## Additional requirements to run the Jupyter Notebook
 * `autograd >= 1.5`
 * `jupyter > 1.0.0`
 * `notebook > 6.5.2`
 
 In addition, our F2PY-wrapped Stamnes' DISORT (in the `disort4.0.99_f2py` directory), or equivalent,
```

### Comparing `PythonicDISORT-0.6.2/README.md` & `pythonicdisort-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,31 +21,31 @@
 of our GitHub repository.
 The Jupyter Notebook provides comprehensive documentation, suggested inputs, explanations, 
 mathematical derivations and verification tests.
 We highly recommend reading the non-optional parts of sections 1 and 2 before use.
 
 ## PyTest and examples of how to use PythonicDISORT
 
-Not only do we have verification tests in the Jupyter Notebook, we also used PyTest to recreate most of the test problems in Stamnes' `disotest.f90`; 
+Not only do we have verification tests in the Jupyter Notebook, we have also recreated most of the test problems in Stamnes' `disotest.f90`; 
 `disotest.f90` is included in the `disort4.0.99_f2py` directory of our GitHub repository. In these tests, the solutions from PythonicDISORT are compared 
 against solutions from our F2PY-wrapped Stamnes' DISORT (version 4.0.99). With PyTest installed, execute the console command `pytest` 
 in the `pydisotest` directory to run these tests. The `pydisotest` directory also contains Jupyter Notebooks, one for each test, 
 to show how the tests were implemented. These notebooks double up as examples of how to use PythonicDISORT.
 
 # Installation
 
 * From PyPI: `pip install PythonicDISORT`
 * From Conda-forge: (TODO: we need to first publish on Conda-forge)
-* By cloning repository: `pip install .` in the `Pythonic-DISORT` directory; `pip install -r all_optional_dependencies.txt` to install all optional dependencies
+* By cloning repository: `pip install .` in the `Pythonic-DISORT` directory; `pip install -r all_optional_dependencies.txt` to install all optional dependencies (see *Requirements to run PythonicDISORT*)
 
 ## Requirements to run PythonicDISORT
 * Python 3.8+
 * `numpy >= 1.8.0`
 * `scipy >= 1.8.0`
-* (OPTIONAL) `pytest >= 6.2.5` (Required for non-Notebook tests)
+* (OPTIONAL) `pytest >= 6.2.5` (Required to use the command `pytest`, see *PyTest and examples of how to use PythonicDISORT*)
 
 ## Additional requirements to run the Jupyter Notebook
 * `autograd >= 1.5`
 * `jupyter > 1.0.0`
 * `notebook > 6.5.2`
 
 In addition, our F2PY-wrapped Stamnes' DISORT (in the `disort4.0.99_f2py` directory), or equivalent,
```

### Comparing `PythonicDISORT-0.6.2/pyproject.toml` & `pythonicdisort-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 dependencies = [
   "numpy>=1.8.0",
   "scipy>=1.8.0",
 ]
 name = "PythonicDISORT"
-version = "0.6.2"
+version = "0.7.0"
 authors = [
   { name="Dion HO Jia Xu", email="dh3065@columbia.edu" },
 ]
 description = "Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `PythonicDISORT-0.6.2/src/PythonicDISORT/pydisort.py` & `pythonicdisort-0.7.0/src/PythonicDISORT/pydisort.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from PythonicDISORT import subroutines
-from PythonicDISORT._assemble_solution_functions import _assemble_solution_functions
+from PythonicDISORT._assemble_intensity_and_fluxes import _assemble_intensity_and_fluxes
 
 import numpy as np
 import scipy as sc
 from math import pi
 from numpy.polynomial.legendre import Legendre
 from scipy import integrate
     
@@ -18,48 +18,50 @@
     b_pos=0, 
     b_neg=0,
     only_flux=False,
     f_arr=0, 
     NT_cor=False,
     BDRF_Fourier_modes=[],
     s_poly_coeffs=np.array([[]]),
-    use_sparse_NLayers=13,
-    _is_compatible_with_autograd = False,
+    NLayers_to_use_sparse=13,
+    _autograd_compatible = False,
 ):
     """Solves the 1D RTE for the fluxes, and optionally intensity,
     of a multi-layer atmosphere with the specified optical properties, boundary conditions
     and sources. Optionally performs delta-M scaling and NT corrections. 
     
         See https://pythonic-disort.readthedocs.io/en/latest/Pythonic-DISORT.html#1.-USER-INPUT-REQUIRED:-Choose-parameters
         for a more detailed explanation of each parameter.
         See https://pythonic-disort.readthedocs.io/en/latest/Pythonic-DISORT.html#2.-PythonicDISORT-modules-and-outputs
         for a more detailed explanation of each output.
         The notebook also has numerous examples of this function being called.
 
     Parameters
     ----------
-    tau_arr : array
+    tau_arr : array or float
         Optical depth of the lower boundary of each atmospheric layer.
-    omega_arr : array
+    omega_arr : array or float
         Single-scattering albedo of each atmospheric layer.
     NQuad : int
         Number of `mu` quadrature nodes.
-    Leg_coeffs_all : ndarray
-        All available unweighted phase function Legendre coefficients. 
+    Leg_coeffs_all : 2darray
+        All available unweighted phase function Legendre coefficients.
+        Each row of coefficients pertain to an atmospheric layer.
         Each coefficient should be between 0 and 1 inclusive.
     mu0 : float
         Cosine of polar angle of the incident beam.
     I0 : float
         Intensity of the incident beam.
     phi0 : float
         Azimuthal angle of the incident beam.
     NLeg : optional, int
-        Number of phase function Legendre coefficients.
+        Number of phase function Legendre coefficients
+        to use in the pre-correction solver.
     NFourier : optional, int
-        Number of Fourier modes to use in the intensity function.
+        Number of Fourier modes to use to construct the intensity function.
     b_pos : optional, 2darray or float
         Dirichlet boundary condition for the upward direction.
     b_neg : optional, 2darray or float
         Dirichlet boundary condition for the downward direction.
     only_flux : optional, bool
         Do NOT compute the intensity function?
     f_arr : optional, array
@@ -68,41 +70,88 @@
         Perform Nakajima-Tanaka intensity corrections?
     BDRF_Fourier_modes : optional, list
         BDRF Fourier modes, each a function with arguments `mu, -mu_p` of type array
         and which output has the same dimensions as the outer product of the two arrays.
     s_poly_coeffs : optional, array
         Polynomial coefficients of isotropic internal sources.
         Arrange coefficients from lowest order term to highest.
-    use_sparse_NLayers : optional, int
+    NLayers_to_use_sparse : optional, int
         At or above how many atmospheric layers should SciPy's sparse matrix framework be used?
 
     Returns
     -------
-    array
+    mu_arr : array
         All `mu` (cosine of polar angle) quadrature nodes.
-    function
+    Fp(tau) : function, function
         (Energetic) Flux function with argument `tau` (type: array) for positive (upward) `mu` values.
         Returns the diffuse flux magnitudes (type: array).
-    function
+    Fm(tau) : function
         (Energetic) Flux function with argument `tau` (type: array) for negative (downward) `mu` values.
         Returns a tuple of the diffuse and direct flux magnitudes respectively (type: (array, array)).
-    function
+    u0(tau) : function
         Zeroth Fourier mode of the intensity with argument `tau` (type: array).
         Returns an ndarray with axes corresponding to variation with `mu` and `tau` respectively.
         This function is useful for calculating actinic fluxes and other quantities of interest,
         but reclassification of delta-scaled flux and other corrections must be done manually
         (for actinic flux `generate_diff_act_flux_funcs` will automatically perform the reclassification).
-    function, optional
+    u(tau, phi) : function, optional
         Intensity function with arguments `(tau, phi, return_Fourier_error=False)` of types `(array, array, bool)`.
         Returns an ndarray with axes corresponding to variation with `mu, tau, phi` respectively.
         The optional flag `return_Fourier_error` determines whether the function will also return
         the Cauchy / Fourier convergence evaluation (type: float) for the last Fourier term.
 
     """
-    if _is_compatible_with_autograd:
+    
+    """
+    Arguments of pydisort
+    |         Variable        |            Type / Shape            |
+    | ----------------------- | ---------------------------------- |
+    | `tau_arr`               | `NLayers`                          |
+    | `omega_arr`             | `NLayers`                          |
+    | `NQuad`                 | scalar                             |
+    | `Leg_coeffs_all`        | `NLeg_all`                         |
+    | `mu0`                   | scalar                             |
+    | `I0`                    | scalar                             |
+    | `phi0`                  | scalar                             |
+    | `NLeg`                  | scalar                             |
+    | `NFourier`              | scalar                             |
+    | `b_pos`                 | `NQuad/2 x NFourier` or scalar     |
+    | `b_neg`                 | `NQuad/2 x NFourier` or scalar     |              
+    | `only_flux`             | boolean                            |
+    | `f_arr`                 | `NLayers` or scalar                |
+    | `NT_cor`                | boolean                            |
+    | `BDRF_Fourier_modes`    | `NBDRF`                            |
+    | `s_poly_coeffs`         | `NLayers x Nscoeffs` or `Nscoeffs` |
+    | `NLayers_to_use_sparse` | scalar                             |
+    
+    Notable internal variables of pydisort
+    |          Variable            |     Type / Shape     |
+    | ---------------------------- | -------------------- |
+    | `I0_orig`                    | scalar               |
+    | `thickness_arr`              | `NLayers`            |
+    | `weighted_Leg_coeffs_all`    | `NLayers x NLeg_all` |
+    | `Leg_coeffs`                 | `NLayers x NLeg`     |
+    | `weighted_scaled_Leg_coeffs` | `NLayers x NLeg`     |
+    | `mu_arr_pos`                 | `NQuad/2`            |
+    | `W`                          | `NQuad/2`            |
+    | `mu_arr`                     | `NQuad`              |
+    | `M_inv`                      | `NQuad/2`            |
+    | `scale_tau`                  | `NLayers`            |
+    | `scaled_tau_arr_with_0`      | `NLayers + 1`        |
+    | `scaled_omega_arr`           | `NLayers`            |
+    | `sum1`                       | scalar               |
+    | `omega_avg`                  | scalar               |
+    | `sum2`                       | scalar               |
+    | `f_avg`                      | scalar               |
+    | `Leg_coeffs_residue`         | `NLayers x NLeg_all` |
+    | `Leg_coeffs_residue_avg`     | `NLeg_all`           |
+    | `scaled_mu0`                 | scalar               |
+    """
+
+    if _autograd_compatible:
         import autograd.numpy as np
     else:
         import numpy as np
     
     # Turn scalars into arrays
     # --------------------------------------------------------------------------------------------------------------------------
     tau_arr = np.atleast_1d(tau_arr)
@@ -130,18 +179,18 @@
     b_pos_is_scalar = False
     b_neg_is_scalar = False
     thickness_arr = np.concatenate([[tau_arr[0]], np.diff(tau_arr)])
     NLeg_all = np.shape(Leg_coeffs_all)[1]
     N = NQuad // 2
     there_is_beam_source = I0 > 0
     there_is_iso_source = Nscoeffs > 0
-    atmos_is_multilayered = NLayers > 1
+    is_atmos_multilayered = NLayers > 1
     # --------------------------------------------------------------------------------------------------------------------------
 
-    # Input checks
+    # Input checks (refer to Section 1 of the Comprehensive Documentation)
     # --------------------------------------------------------------------------------------------------------------------------
     # Optical depths and thickness must be positive
     assert np.all(tau_arr > 0)
     assert np.all(thickness_arr > 0)
     # Single-scattering albedo must be between 0 and 1, excluding 1
     assert np.all(omega_arr >= 0)
     assert np.all(omega_arr < 1)
@@ -179,41 +228,43 @@
     if len(np.atleast_1d(b_neg)) == 1:
         b_neg_is_scalar = True
     else:
         assert np.shape(b_neg) == (N, NFourier)
     # The fractional scattering must be between 0 and 1
     assert np.all(0 <= f_arr) and np.all(f_arr <= 1)
     # The minimum threshold is the minimum numbers of layers: 1
-    assert(use_sparse_NLayers >= 1)
+    assert(NLayers_to_use_sparse >= 1)
     # --------------------------------------------------------------------------------------------------------------------------
     
     # Some more setup
     # --------------------------------------------------------------------------------------------------------------------------
     NBDRF = len(BDRF_Fourier_modes)
     weighted_Leg_coeffs_all = (2 * np.arange(NLeg_all) + 1) * Leg_coeffs_all
     Leg_coeffs = Leg_coeffs_all[:, :NLeg]
+    # The following is explained in Section 1.4 of the Comprehensive Documentation
     if (b_pos_is_scalar and b_pos == 0) and (b_neg_is_scalar and b_neg == 0) and not there_is_iso_source and there_is_beam_source:
         I0_orig = I0
         I0 = 1
     else:
         I0_orig = 1
     # --------------------------------------------------------------------------------------------------------------------------
     
-    # Generation of Double Gauss-Legendre quadrature weights and points
+    # Generation of "double-Gauss" quadrature weights and points (refer to Section 3.4 of the Comprehensive Documentation)
     # --------------------------------------------------------------------------------------------------------------------------
     # For positive mu values (the weights are identical for both domains)
     mu_arr_pos, W = subroutines.Gauss_Legendre_quad(N)  # mu_arr_neg = -mu_arr_pos
     mu_arr = np.concatenate([mu_arr_pos, -mu_arr_pos])
     M_inv = 1 / mu_arr_pos
     
     # We do not allow mu0 to equal a quadrature / computational angle
     assert not np.any(np.abs(mu_arr_pos - mu0) < 1e-8)
     # --------------------------------------------------------------------------------------------------------------------------
 
     # Delta-M scaling; there is no scaling if f = 0
+    # Refer to Sections 1.3.1 and 3.3 of the Comprehensive Documentation
     # --------------------------------------------------------------------------------------------------------------------------
     if np.any(f_arr > 0):
         scale_tau = 1 - omega_arr * f_arr
         scaled_thickness_arr = scale_tau * thickness_arr
         scaled_tau_arr_with_0 = np.array(
             list(map(lambda l: np.sum(scaled_thickness_arr[:l]), range(NLayers + 1)))
         )
@@ -227,39 +278,40 @@
         scaled_tau_arr_with_0 = np.concatenate([[0], tau_arr])
         weighted_scaled_Leg_coeffs = Leg_coeffs * (2 * np.arange(NLeg) + 1)[None, :]
         scaled_omega_arr = omega_arr
     # --------------------------------------------------------------------------------------------------------------------------
     
     if NT_cor and not only_flux and there_is_beam_source and np.any(f_arr > 0) and NLeg < NLeg_all:
         
-        ############################### Perform NT corrections on the intensity but not the flux ###################################
+        ############################### Perform NT corrections on the intensity but not the flux ###############################
+        ############################### Refer to Section 3.7.2 of the Comprehensive Documentation ##############################
         
         # Delta-M scaled solution; no further corrections to the flux
-        flux_up, flux_down, u0, u_star = _assemble_solution_functions(
+        flux_up, flux_down, u0, u_star = _assemble_intensity_and_fluxes(
             scaled_omega_arr,
             tau_arr,
             scaled_tau_arr_with_0,
             mu_arr_pos, mu_arr,
             M_inv, W,
-            N, NQuad, NLeg, NFourier,
-            NLayers, NBDRF,
-            atmos_is_multilayered,
+            N, NQuad, NLeg,
+            NFourier, NLayers, NBDRF,
+            is_atmos_multilayered,
             weighted_scaled_Leg_coeffs,
             BDRF_Fourier_modes,
             mu0, I0, I0_orig, phi0,
             there_is_beam_source,
             b_pos, b_neg,
             b_pos_is_scalar, b_neg_is_scalar,
             s_poly_coeffs,
             Nscoeffs,
             there_is_iso_source,
             scale_tau,
             only_flux,
-            use_sparse_NLayers,
-            _is_compatible_with_autograd,
+            NLayers_to_use_sparse,
+            _autograd_compatible,
         )
         
         # TMS correction
         # --------------------------------------------------------------------------------------------------------------------------
         def TMS_correction(tau, phi):
             Ntau = len(tau)
             Nphi = len(phi)
@@ -320,24 +372,33 @@
                 )
             )
             
             ## Contribution from other layers
             # TODO: Despite being vectorized and despite many attempts at further optimization,
             # this block of code is slower than desired and is the bottleneck for the TMS correction.
             # --------------------------------------------------------------------------------------------------------------------------
-            if atmos_is_multilayered:
+            solution = (
+                mathscr_B[:, l, :] * np.vstack((TMS_correction_pos, TMS_correction_neg))[:, :, None]
+            )
+            
+            if is_atmos_multilayered:
                 layers_arr = np.arange(NLayers)[:, None]
                 pos_contribution_mask = (l[None, :] < layers_arr).ravel()
                 neg_contribution_mask = (l[None, :] > layers_arr).ravel()
+                any_pos_contribution = np.any(pos_contribution_mask)
+                any_neg_contribution = np.any(neg_contribution_mask)
+            
+                if not (any_pos_contribution or any_neg_contribution):
+                    return solution
 
                 layers_arr_repeat = np.repeat(layers_arr, Ntau)
                 scaled_tau_tile = np.tile(scaled_tau, NLayers)
                 scaled_tau_arr_with_0_repeat = np.repeat(scaled_tau_arr_with_0, Ntau)
 
-                if np.any(pos_contribution_mask):
+                if any_pos_contribution:
                     contribution_from_each_other_layer_pos = np.zeros((N, NLayers * Ntau, Nphi))
                     scaled_tau_l_tile_pos = scaled_tau_tile[pos_contribution_mask]
                     mathscr_B_l_repeat_posmasked = mathscr_B[
                         :N, layers_arr_repeat[pos_contribution_mask], :
                     ]
                     scaled_tau_arr_with_0_l_tile_posmasked = scaled_tau_arr_with_0_repeat[:-Ntau][
                         pos_contribution_mask
@@ -361,15 +422,15 @@
                             )
                         )[:, :, None]
                     )
                     contribution_from_other_layers_pos = np.sum(
                         contribution_from_each_other_layer_pos.reshape((N, NLayers, Ntau, Nphi)),
                         axis=1,
                     )
-                if np.any(neg_contribution_mask):
+                if any_neg_contribution:
                     contribution_from_each_other_layer_neg = np.zeros((N, NLayers * Ntau, Nphi))
                     scaled_tau_l_tile_neg = scaled_tau_tile[neg_contribution_mask]
                     mathscr_B_l_repeat_negmasked = mathscr_B[
                         N:, layers_arr_repeat[neg_contribution_mask], :
                     ]
                     scaled_tau_arr_with_0_l_tile_negmasked = scaled_tau_arr_with_0_repeat[:-Ntau][
                         neg_contribution_mask
@@ -394,38 +455,34 @@
                         )[:, :, None]
                     )
                     contribution_from_other_layers_neg = np.sum(
                         contribution_from_each_other_layer_neg.reshape((N, NLayers, Ntau, Nphi)),
                         axis=1,
                     )
 
-                if _is_compatible_with_autograd:
-                    solution = (
-                        mathscr_B[:, l, :]
-                        * np.vstack((TMS_correction_pos, TMS_correction_neg))[:, :, None]
-                    )
-                    solution[:N, :, :] += contribution_from_other_layers_pos
-                    solution[N:, :, :] += contribution_from_other_layers_neg
-                    return solution
-
-                else:
-                    return mathscr_B[:, l, :] * np.vstack((TMS_correction_pos, TMS_correction_neg))[
-                        :, :, None
-                    ] + np.concatenate(
+                if _autograd_compatible:
+                    if not any_pos_contribution:
+                        TMS_correction_pos = np.zeros((N, Ntau, Nphi))
+                    if not any_neg_contribution:
+                        TMS_correction_neg = np.zeros((N, Ntau, Nphi))
+                    return solution + np.concatenate(
                         (contribution_from_other_layers_pos, contribution_from_other_layers_neg),
                         axis=0,
                     )
+                else:
+                    if any_pos_contribution:
+                        solution[:N, :, :] += contribution_from_other_layers_pos
+                    if any_neg_contribution:
+                        solution[N:, :, :] += contribution_from_other_layers_neg
+                    return solution
                     
             # --------------------------------------------------------------------------------------------------------------------------
             
             else:
-                return (
-                    mathscr_B[:, l, :]
-                    * np.vstack((TMS_correction_pos, TMS_correction_neg))[:, :, None]
-                )
+                return solution
         # --------------------------------------------------------------------------------------------------------------------------
 
         # IMS correction
         # --------------------------------------------------------------------------------------------------------------------------
         sum1 = np.sum(omega_arr * tau_arr)
         omega_avg = sum1 / np.sum(tau_arr)
         sum2 = np.sum(f_arr * omega_arr * tau_arr)
@@ -462,15 +519,15 @@
         # The corrected intensity
         # --------------------------------------------------------------------------------------------------------------------------
         def u_corrected(tau, phi, return_Fourier_error=False):
             tau = np.atleast_1d(tau)
             phi = np.atleast_1d(phi)
             NT_corrections = TMS_correction(tau, phi)
 
-            if _is_compatible_with_autograd:
+            if _autograd_compatible:
                 NT_corrections = NT_corrections + np.concatenate(
                     [np.zeros((N, len(tau), len(phi))), IMS_correction(tau, phi)], axis=0
                 )
             else:
                 NT_corrections[N:, :, :] += IMS_correction(tau, phi)
                
             if return_Fourier_error:
@@ -484,30 +541,30 @@
         # --------------------------------------------------------------------------------------------------------------------------
 
         return mu_arr, flux_up, flux_down, u0, u_corrected
         
     else:
         if only_flux:
             NFourier = 1 # We only need to solve for the 0th Fourier mode to compute the flux
-        return (mu_arr,) + _assemble_solution_functions(
+        return (mu_arr,) + _assemble_intensity_and_fluxes(
             scaled_omega_arr,
             tau_arr,
             scaled_tau_arr_with_0,
             mu_arr_pos, mu_arr,
             M_inv, W,
-            N, NQuad, NLeg, NFourier,
-            NLayers, NBDRF,
-            atmos_is_multilayered,
+            N, NQuad, NLeg,
+            NFourier, NLayers, NBDRF,
+            is_atmos_multilayered,
             weighted_scaled_Leg_coeffs,
             BDRF_Fourier_modes,
             mu0, I0, I0_orig, phi0,
             there_is_beam_source,
             b_pos, b_neg,
             b_pos_is_scalar, b_neg_is_scalar,
             s_poly_coeffs,
             Nscoeffs,
             there_is_iso_source,
             scale_tau,
             only_flux,
-            use_sparse_NLayers,
-            _is_compatible_with_autograd,
+            NLayers_to_use_sparse,
+            _autograd_compatible,
         )
```

### Comparing `PythonicDISORT-0.6.2/src/PythonicDISORT/subroutines.py` & `pythonicdisort-0.7.0/src/PythonicDISORT/subroutines.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import scipy as sc
 from math import pi
 from numpy.polynomial.legendre import leggauss
 
 
-def transform_interval(arr, c, d, a=-1, b=1):
+def transform_interval(arr, c, d, a, b):
     """Affine transformation of an array from interval [a, b] to [c, d].
 
     Parameters
     ----------
     arr : array
         The 1D array to transform.
     c : float
@@ -25,15 +25,15 @@
     array
         The transformed 1D array.
 
     """
     return (((arr - a) * (d - c)) / (b - a)) + c
 
 
-def transform_weights(weights, c, d, a=-1, b=1):
+def transform_weights(weights, c, d, a, b):
     """Transforms an array of quadrature weights from interval [a, b] to [c, d].
 
     Parameters
     ----------
     weights : array
         The weights to transform.
     c : float
@@ -102,15 +102,15 @@
         Quadrature zero points.
     array
         Quadrature weights.
 
     """
     mu_arr_pos, W = leggauss(int(N))
 
-    return transform_interval(mu_arr_pos, c, d), transform_weights(W, c, d)
+    return transform_interval(mu_arr_pos, c, d, -1, 1), transform_weights(W, c, d, -1, 1)
 
 
 def Clenshaw_Curtis_quad(Nphi, c=0, d=(2 * pi)):
     """Generates Clenshaw-Curtis quadrature zero points and weights for integration from c to d.
 
     Parameters
     ----------
@@ -138,15 +138,15 @@
     phi_arr_pos = np.cos(pi * np.arange(Nphi_pos) / Nphi)
     phi_arr = np.concatenate([-phi_arr_pos, [0], np.flip(phi_arr_pos)])
     diff = np.concatenate([[2], 2 / (1 - 4 * np.arange(1, Nphi_pos + 1) ** 2)])
     weights_phi_pos = sc.fft.idct(diff, type=1)
     weights_phi_pos[0] /= 2
     full_weights_phi = np.hstack((weights_phi_pos, np.flip(weights_phi_pos[:-1])))
 
-    return transform_interval(phi_arr, c, d), transform_weights(full_weights_phi, c, d)
+    return transform_interval(phi_arr, c, d, -1, 1), transform_weights(full_weights_phi, c, d, -1, 1)
 
 
 def generate_FD_mat(Ntau, a, b):
     """Generates a sparse first derivative central difference (second-order accuracy) 
     matrix on [a,b] in `csr` format with `Ntau` grid points.
     Second order forward or backward differences are used at the boundaries.
 
@@ -252,26 +252,66 @@
         u0_cache, act_dscale_reclassification = u0(tau, True)
         result_without_reclassification = 2 * pi * GL_weights @ u0_cache[N:]
         return result_without_reclassification + act_dscale_reclassification
     
     return flux_act_up, flux_act_down_diffuse
 
 
-def _mathscr_v(tau, l, s_poly_coeffs, Nscoeffs, G, K, G_inv, mu_arr, _is_compatible_with_autograd=False):
+def _mathscr_v(tau,                         # Input optical depths
+                l,                          # Layer index of each input optical depth
+                s_poly_coeffs,              # Polynomial coefficients of isotropic source
+                Nscoeffs,                   # Number of isotropic source polynomial coefficients
+                G,                          # Eigenvector matrices
+                K,                          # Eigenvalues
+                G_inv,                      # Inverse of eigenvector matrix
+                mu_arr,                     # Quadrature nodes for both hemispheres
+                _autograd_compatible=False  # Should the output functions be compatible with autograd?
+                ):
     """Particular solution for isotropic internal sources.
-    It has many seemingly redundant arguments to maximize precomputation
-    in the `pydisort` function which calls it.
-
+    Refer to Section 3.6.1 of the Comprehensive Documentation.
+    It has many seemingly redundant arguments to maximize 
+    precomputation in the `_assemble_intensity_and_fluxes` 
+    and `_solve_for_coeffs` functions which call it.
+    
+    Arguments of _mathscr_v
+    |        Variable        |                 Shape                 |
+    | ---------------------- | ------------------------------------- |
+    | `tau`                  | `Ntau`                                |
+    | `l`                    | `Ntau`                                |
+    | `s_poly_coeffs`        | `NLayers x Nscoeffs` or `Nscoeffs`    |
+    | `G`                    | `NLayers<= x NQuad x NQuad`           |
+    | `K`                    | `NLayers<= x NQuad`                   |
+    | `G_inv`                | `NLayers<= x NQuad x NQuad` or `None` |
+    | `mu_arr`               | `NQuad`                               |
+    | `_autograd_compatible` | boolean                               |
+    
+    Notable internal variables of _mathscr_v
+    |     Variable     |                Shape                | 
+    | ---------------- | ----------------------------------- |
+    | i_arr            | `Nscoeffs`                          |
+    | i_arr_repeat     | `Nscoeffs*(Nscoeffs+1)/2`           | Using triangular number formula
+    | j_arr            | `Nscoeffs*(Nscoeffs+1)/2`           | Using triangular number formula
+    | s_poly_coeffs_nj | `NLayers x Nscoeffs*(Nscoeffs+1)/2` |
+    | OUTPUT           | `NQuad x Ntau`                      |
     """
     n = Nscoeffs - 1
     
-    if _is_compatible_with_autograd:
+    if _autograd_compatible:
         import autograd.numpy as np
     
         def mathscr_b(i):
+            """
+            Notable internal variables of mathscr_b
+            |     Variable     |                 Shape                 |
+            | ---------------- | ------------------------------------- |
+            | j_arr            | `i + 1`                               |
+            | s_poly_coeffs_nj | `i + 1`                               |
+            | OUTPUT           | `Nscoeffs x (i + 1) x NQuad`          |
+            """
+        
             j_arr = np.arange(i + 1)
             s_poly_coeffs_nj = s_poly_coeffs[:, n - j_arr]
             return np.sum(
                 (sc.special.factorial(n - j_arr) / sc.special.factorial(n - i))[None, None, :]
                 * K[:, :, None] ** -(i - j_arr + 1)[None, None, :]
                 * s_poly_coeffs_nj[:, None, :],
                 axis=-1,
```

### Comparing `PythonicDISORT-0.6.2/src/PythonicDISORT.egg-info/PKG-INFO` & `pythonicdisort-0.7.0/src/PythonicDISORT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonicDISORT
-Version: 0.6.2
+Version: 0.7.0
 Summary: Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere.
 Author-email: Dion HO Jia Xu <dh3065@columbia.edu>
 Project-URL: Homepage, https://github.com/LDEO-CREW/Pythonic-DISORT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -42,31 +42,31 @@
 of our GitHub repository.
 The Jupyter Notebook provides comprehensive documentation, suggested inputs, explanations, 
 mathematical derivations and verification tests.
 We highly recommend reading the non-optional parts of sections 1 and 2 before use.
 
 ## PyTest and examples of how to use PythonicDISORT
 
-Not only do we have verification tests in the Jupyter Notebook, we also used PyTest to recreate most of the test problems in Stamnes' `disotest.f90`; 
+Not only do we have verification tests in the Jupyter Notebook, we have also recreated most of the test problems in Stamnes' `disotest.f90`; 
 `disotest.f90` is included in the `disort4.0.99_f2py` directory of our GitHub repository. In these tests, the solutions from PythonicDISORT are compared 
 against solutions from our F2PY-wrapped Stamnes' DISORT (version 4.0.99). With PyTest installed, execute the console command `pytest` 
 in the `pydisotest` directory to run these tests. The `pydisotest` directory also contains Jupyter Notebooks, one for each test, 
 to show how the tests were implemented. These notebooks double up as examples of how to use PythonicDISORT.
 
 # Installation
 
 * From PyPI: `pip install PythonicDISORT`
 * From Conda-forge: (TODO: we need to first publish on Conda-forge)
-* By cloning repository: `pip install .` in the `Pythonic-DISORT` directory; `pip install -r all_optional_dependencies.txt` to install all optional dependencies
+* By cloning repository: `pip install .` in the `Pythonic-DISORT` directory; `pip install -r all_optional_dependencies.txt` to install all optional dependencies (see *Requirements to run PythonicDISORT*)
 
 ## Requirements to run PythonicDISORT
 * Python 3.8+
 * `numpy >= 1.8.0`
 * `scipy >= 1.8.0`
-* (OPTIONAL) `pytest >= 6.2.5` (Required for non-Notebook tests)
+* (OPTIONAL) `pytest >= 6.2.5` (Required to use the command `pytest`, see *PyTest and examples of how to use PythonicDISORT*)
 
 ## Additional requirements to run the Jupyter Notebook
 * `autograd >= 1.5`
 * `jupyter > 1.0.0`
 * `notebook > 6.5.2`
 
 In addition, our F2PY-wrapped Stamnes' DISORT (in the `disort4.0.99_f2py` directory), or equivalent,
```

