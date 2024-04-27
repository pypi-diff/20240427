# Comparing `tmp/adios4dolfinx-0.8.0.dev0.tar.gz` & `tmp/adios4dolfinx-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adios4dolfinx-0.8.0.dev0.tar", last modified: Wed Mar  6 14:59:42 2024, max compression
+gzip compressed data, was "adios4dolfinx-0.8.1.tar", last modified: Sat Apr 27 08:15:15 2024, max compression
```

## Comparing `adios4dolfinx-0.8.0.dev0.tar` & `adios4dolfinx-0.8.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:59:42.480504 adios4dolfinx-0.8.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-03-06 14:59:42.480504 adios4dolfinx-0.8.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 14:59:42.480504 adios4dolfinx-0.8.0.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:59:42.472504 adios4dolfinx-0.8.0.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:59:42.476504 adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9927 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/adios2_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    26800 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/checkpointing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/comm_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15055 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/legacy_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16177 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/original_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:59:42.476504 adios4dolfinx-0.8.0.dev0/src/adios4dolfinx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-03-06 14:59:42.000000 adios4dolfinx-0.8.0.dev0/src/adios4dolfinx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-06 14:59:42.000000 adios4dolfinx-0.8.0.dev0/src/adios4dolfinx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 14:59:42.000000 adios4dolfinx-0.8.0.dev0/src/adios4dolfinx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-06 14:59:42.000000 adios4dolfinx-0.8.0.dev0/src/adios4dolfinx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-06 14:59:42.000000 adios4dolfinx-0.8.0.dev0/src/adios4dolfinx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:59:42.476504 adios4dolfinx-0.8.0.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/tests/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/tests/test_checkpointing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/tests/test_checkpointing_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/tests/test_legacy_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/tests/test_mesh_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11538 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/tests/test_meshtags.py
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/tests/test_numpy_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    16234 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/tests/test_original_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/tests/test_snapshot_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-06 14:59:37.000000 adios4dolfinx-0.8.0.dev0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:15:15.630074 adios4dolfinx-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9299 2024-04-27 08:15:15.630074 adios4dolfinx-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 08:15:15.630074 adios4dolfinx-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:15:15.622074 adios4dolfinx-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:15:15.626074 adios4dolfinx-0.8.1/src/adios4dolfinx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/src/adios4dolfinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/src/adios4dolfinx/adios2_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28651 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/src/adios4dolfinx/checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/src/adios4dolfinx/comm_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15063 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/src/adios4dolfinx/legacy_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16243 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/src/adios4dolfinx/original_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/src/adios4dolfinx/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/src/adios4dolfinx/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/src/adios4dolfinx/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/src/adios4dolfinx/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/src/adios4dolfinx/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:15:15.630074 adios4dolfinx-0.8.1/src/adios4dolfinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9299 2024-04-27 08:15:15.000000 adios4dolfinx-0.8.1/src/adios4dolfinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-27 08:15:15.000000 adios4dolfinx-0.8.1/src/adios4dolfinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 08:15:15.000000 adios4dolfinx-0.8.1/src/adios4dolfinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-27 08:15:15.000000 adios4dolfinx-0.8.1/src/adios4dolfinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-27 08:15:15.000000 adios4dolfinx-0.8.1/src/adios4dolfinx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:15:15.630074 adios4dolfinx-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/tests/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/tests/test_checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/tests/test_checkpointing_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/tests/test_legacy_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/tests/test_mesh_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11562 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/tests/test_meshtags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/tests/test_numpy_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16234 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/tests/test_original_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/tests/test_snapshot_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-27 08:15:09.000000 adios4dolfinx-0.8.1/tests/test_version.py
```

### Comparing `adios4dolfinx-0.8.0.dev0/LICENSE` & `adios4dolfinx-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adios4dolfinx-0.8.0.dev0/PKG-INFO` & `adios4dolfinx-0.8.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: adios4dolfinx
-Version: 0.8.0.dev0
+Version: 0.8.1
 Summary: Checkpointing functionality for DOLFINx meshes/functions with ADIOS2
 Author-email: "Jørgen S. Dokken" <dokken@simula.no>
 License: Copyright 2023 Jørgen S. Dokken
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fenics-dolfinx>=0.8.0.dev0
+Requires-Dist: fenics-dolfinx>=0.8.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: ipyparallel; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pdbpp; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
@@ -26,47 +26,97 @@
 Provides-Extra: docs
 Requires-Dist: jupyter-book; extra == "docs"
 Requires-Dist: ipyparallel; extra == "docs"
 Requires-Dist: ipywidgets; extra == "docs"
 Provides-Extra: all
 Requires-Dist: adios4dolfinx[dev,docs,test]; extra == "all"
 
-# ADIOS2Wrappers for DOLFINx
+# ADIOS4DOLFINx - A framework for checkpointing in DOLFINx
 
-[![MIT](https://img.shields.io/github/license/jorgensd/adios4dolfinx)](LICENSE)
-[Read Latest Documentation](https://jsdokken.com/adios4dolfinx/)
+![MIT](https://img.shields.io/github/license/jorgensd/adios4dolfinx)
+[![status](https://joss.theoj.org/papers/7866cb142db8a803e32d79a109573d25/status.svg)](https://joss.theoj.org/papers/7866cb142db8a803e32d79a109573d25)
 
-This is an extension for [DOLFINx](https://github.com/FEniCS/dolfinx/) to checkpoint meshes, meshtags and functions using [ADIOS2](https://adios2.readthedocs.io/en/latest/).
+ADIOS4DOLFINx is an extension for [DOLFINx](https://github.com/FEniCS/dolfinx/) to checkpoint meshes, meshtags and functions using [ADIOS 2](https://adios2.readthedocs.io/en/latest/).
 
-The code uses the adios2 Python-wrappers to write DOLFINx objects to file, supporting N-to-M (_recoverable_) and N-to-N (_snapshot_) checkpointing.
-See: [Checkpointing in DOLFINx - FEniCS 23](https://jsdokken.com/checkpointing-presentation/#/) for more information.
+The code uses the ADIOS2 Python-wrappers to write DOLFINx objects to file, supporting N-to-M (_recoverable_) and N-to-N (_snapshot_) checkpointing.
+See: [Checkpointing in DOLFINx - FEniCS 23](https://jsdokken.com/checkpointing-presentation/#/) or the examples in the [Documentation](https://jsdokken.com/adios4dolfinx/) for more information.
 
 For scalability, the code uses [MPI Neighbourhood collectives](https://www.mpi-forum.org/docs/mpi-3.1/mpi31-report/node200.htm) for communication across processes.
 
+## Statement of Need
+
+As the usage of high performance computing clusters increases, more and more large-scale, long-running simulations are deployed.
+The need for storing intermediate solutions from such simulations are crucial, as the HPC system might crash, or the simulation might crash or exceed the alloted computational budget.
+Having a checkpoint of related variables, such as the solutions to partial differential equations (PDEs) is therefore essential.
+The `adios4dolfinx` library extends the [DOLFINx](https://github.com/FEniCS/dolfinx/) computational framework for solving PDEs with checkpointing functionality, such that immediate solutions and mesh information can be stored and re-used in another simulation.
+
 ## Installation
 
+Compatibility with DOLFINx:
+
+- ADIOS4DOLFINx v0.7.3 is compatible with DOLFINx v0.7.x
+- ADIOS4DOLFINx v0.8.1 is compatible with DOLFINx v0.8.x
+
+### Dependencies
+
+The library depends on the Python-interface of [DOLFINx](https://github.com/) and an MPI-build of [ADIOS2](https://adios2.readthedocs.io/en/latest/setting_up/setting_up.html#as-package) and can therefore not be installed through PyPi, but has to be installed through Conda, Spack or from source.
+
 ### Docker
 
-ADIOS2 is installed in the official DOLFINx containers.
+An MPI build of ADIOS2 is installed in the official DOLFINx containers, and thus there are no additional dependencies required to install `adios4dolfinx`
+on top of DOLFINx in these images.
+
+Create a Docker container, named for instance `dolfinx-checkpoint`.
+Use the `nightly` tag to get the main branch of DOLFINx, or `stable` to get the latest stable release
 
 ```bash
 docker run -ti -v $(pwd):/root/shared -w /root/shared --name=dolfinx-checkpoint ghcr.io/fenics/dolfinx/dolfinx:nightly
 ```
 
+For the latest version compatible with nightly (with the ability to run the test suite), use
+
+```bash
+python3 -m pip install adios4dolfinx[test]@git+https://github.com/jorgensd/adios4dolfinx@main
+```
+
+If you are using the `stable` image, you can install `adios4dolfinx` from [PYPI](https://pypi.org/project/adios4dolfinx/) with
+
+```bash
+python3 -m pip install adios4dolfinx[test]
+```
+
+This docker container can be opened with
+
+```bash
+docker container start -i dolfinx-checkpoint
+```
+
+at a later instance
+
 ### Conda
 
-To use with conda (DOLFINx release v0.7.0 works with v0.7.3 of ADIOS4DOLFINx)
+> [!NOTE]  
+> Conda supports the stable release of DOLFINx, and thus the appropriate version should be installed, see the section above for more details.
+
+Following is a minimal recipe of how to install adios4dolfinx, given that you have conda installed on your system.
 
 ```bash
 conda create -n dolfinx-checkpoint python=3.10
 conda activate dolfinx-checkpoint
-conda install -c conda-forge fenics-dolfinx pip adios2
-python3 -m pip install git+https://github.com/jorgensd/adios4dolfinx@v0.7.2
+conda install -c conda-forge fenics-dolfinx pip adios2=*=mpi_*
+python3 -m pip install adios4dolfinx[test]@git+https://github.com/jorgensd/adios4dolfinx@v0.8.1
 ```
 
+> [!NOTE]
+> To run the tests or demos associated with the code, install `ipyparallel` in your environment, for instance by calling
+>
+> ```bash
+> python3 -m pip install adios4dolfinx[test]@git+https://github.com/jorgensd/adios4dolfinx@v0.8.1
+> ```
+
 ## Functionality
 
 ### DOLFINx
 
 - Reading and writing meshes, using `adios4dolfinx.read/write_mesh`
 - Reading and writing meshtags associated to meshes `adios4dolfinx.read/write_meshtags`
 - Reading checkpoints for any element (serial and parallel, arbitrary number of functions and timesteps per file). Use `adios4dolfinx.read/write_function`.
@@ -78,14 +128,25 @@
 
 > [!IMPORTANT]  
 > A checkpoint file supports multiple functions and multiple time steps, as long as the functions are associated with the same mesh
 
 > [!IMPORTANT]  
 > Only one mesh per file is allowed
 
+## Example Usage
+
+The repository contains many documented examples of usage, in the `docs`-folder, including
+
+- [Reading and writing mesh checkpoints](./docs/writing_mesh_checkpoint.py)
+- [Storing mesh partitioning data](./docs/partitioned_mesh.py)
+- [Writing mesh-tags to a checkpoint](./docs/meshtags.py)
+- [Reading and writing function checkpoints](./docs/writing_functions_checkpoint.py)
+- [Checkpoint on input mesh](./docs/original_checkpoint.py)
+  Further examples can be found at [ADIOS4DOLFINx examples](https://jsdokken.com/adios4dolfinx/)
+
 ### Backwards compatibility
 
 > [!WARNING]
 > If you are using v0.7.2, you are adviced to upgrade to v0.7.3, as it contains som crucial fixes for openmpi.
 
 ### Legacy DOLFIN
 
@@ -93,53 +154,52 @@
 
 - Reading meshes from the DOLFIN HDF5File-format
 - Reading checkpoints from the DOLFIN HDF5File-format (one checkpoint per file only)
 - Reading checkpoints from the DOLFIN XDMFFile-format (one checkpoint per file only, and only uses the `.h5` file)
 
 See the [API](./docs/api) for more information.
 
-## Long term plan
+## Testing
 
-The long term plan is to get this library merged into DOLFINx (rewritten in C++ with appropriate Python-bindings).
+This library uses `pytest` for testing.
+To execute the tests, one should first install the library and its dependencies, as listed above.
+Then, can execute all tests by calling
 
-# Contributor guidelines
-When contributing to this repository, please first [create an issue](https://github.com/jorgensd/adios4dolfinx/issues/new/choose) containing information about the missing feature or the bug that you would like to fix. Here you can discuss the change you want to make with the maintainers of the repository.
+```bash
+python3 -m pytest .
+```
 
-Please note we have a code of conduct, please follow it in all your interactions with the project.
+### Testing against data from legacy dolfin
 
-## New contributor guide
+Some tests check the capability of reading data created with the legacy version of DOLFIN.
+To create this dataset, start a docker container with legacy DOLFIN, for instance:
 
-To get an overview of the project, read the [documentation](https://jorgensd.github.io/adios4dolfinx). Here are some resources to help you get started with open source contributions:
+```bash
+docker run -ti -v $(pwd):/root/shared -w /root/s
+hared --rm ghcr.io/scientificcomputing/fenics:2024-02-19
+```
 
-- [Finding ways to contribute to open source on GitHub](https://docs.github.com/en/get-started/exploring-projects-on-github/finding-ways-to-contribute-to-open-source-on-github)
-- [Set up Git](https://docs.github.com/en/get-started/quickstart/set-up-git)
-- [GitHub flow](https://docs.github.com/en/get-started/quickstart/github-flow)
-- [Collaborating with pull requests](https://docs.github.com/en/github/collaborating-with-pull-requests)
+Then, inside this container, call
 
-## Pull Request Process
+```bash
+python3 ./tests/create_legacy_data.py --output-dir=legacy
+```
 
+### Testing against data from older versions of ADIOS4DOLFINx
 
-### Pull Request
+Some tests check the capability to read data generated by `adios4dolfinx<0.7.2`.
+To generate data for these tests use the following commands:
 
-- When you're finished with the changes, create a pull request, also known as a PR. It is also OK to create a [draft pull request](https://github.blog/2019-02-14-introducing-draft-pull-requests/) from the very beginning. Once you are done you can click on the ["Ready for review"] button. You can also [request a review](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/requesting-a-pull-request-review) from one of the maintainers.
-- Don't forget to [link PR to the issue that you opened ](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue).
-- Enable the checkbox to [allow maintainer edits](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/allowing-changes-to-a-pull-request-branch-created-from-a-fork) so the branch can be updated for a merge.
-Once you submit your PR, a team member will review your proposal. We may ask questions or request for additional information.
-- We may ask for changes to be made before a PR can be merged, either using [suggested changes](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/incorporating-feedback-in-your-pull-request) or pull request comments. You can apply suggested changes directly through the UI. You can make any other changes in your fork, then commit them to your branch.
-- As you update your PR and apply changes, mark each conversation as [resolved](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/commenting-on-a-pull-request#resolving-conversations).
-- If you run into any merge issues, checkout this [git tutorial](https://lab.github.com/githubtraining/managing-merge-conflicts) to help you resolve merge conflicts and other issues.
-- Please make sure that all tests are passing, github pages renders nicely, and code coverage are are not lower than before your contribution. You see the different github action workflows by clicking the "Action" tab in the GitHub repository.
+```bash
+docker run -ti -v $(pwd):/root/shared -w /root/shared --rm ghcr.io/fenics/dolfinx/dolfinx:v0.7.3
+```
 
-Note that for a pull request to be accepted, it has to pass all the tests on CI, which includes:
-- `mypy`: typechecking
-- `ruff`: Code formatting
-- `pytest`: Successfull execution of all tests in the `tests` folder.
+Then, inside the container, call
 
+```bash
+python3 -m pip install adios4dolfinx==0.7.1
+python3 ./tests/create_legacy_checkpoint.py --output-dir=legacy_checkpoint
+```
 
-### Our Pledge
+## Long term plan
 
-In the interest of fostering an open and welcoming environment, we as
-contributors and maintainers pledge to making participation in our project and
-our community a harassment-free experience for everyone, regardless of age, body
-size, disability, ethnicity, gender identity and expression, level of experience,
-nationality, personal appearance, race, religion, or sexual identity and
-orientation.
+The long term plan is to get this library merged into DOLFINx (rewritten in C++ with appropriate Python-bindings).
```

### Comparing `adios4dolfinx-0.8.0.dev0/README.md` & `adios4dolfinx-0.8.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,90 @@
-# ADIOS2Wrappers for DOLFINx
+# ADIOS4DOLFINx - A framework for checkpointing in DOLFINx
 
-[![MIT](https://img.shields.io/github/license/jorgensd/adios4dolfinx)](LICENSE)
-[Read Latest Documentation](https://jsdokken.com/adios4dolfinx/)
+![MIT](https://img.shields.io/github/license/jorgensd/adios4dolfinx)
+[![status](https://joss.theoj.org/papers/7866cb142db8a803e32d79a109573d25/status.svg)](https://joss.theoj.org/papers/7866cb142db8a803e32d79a109573d25)
 
-This is an extension for [DOLFINx](https://github.com/FEniCS/dolfinx/) to checkpoint meshes, meshtags and functions using [ADIOS2](https://adios2.readthedocs.io/en/latest/).
+ADIOS4DOLFINx is an extension for [DOLFINx](https://github.com/FEniCS/dolfinx/) to checkpoint meshes, meshtags and functions using [ADIOS 2](https://adios2.readthedocs.io/en/latest/).
 
-The code uses the adios2 Python-wrappers to write DOLFINx objects to file, supporting N-to-M (_recoverable_) and N-to-N (_snapshot_) checkpointing.
-See: [Checkpointing in DOLFINx - FEniCS 23](https://jsdokken.com/checkpointing-presentation/#/) for more information.
+The code uses the ADIOS2 Python-wrappers to write DOLFINx objects to file, supporting N-to-M (_recoverable_) and N-to-N (_snapshot_) checkpointing.
+See: [Checkpointing in DOLFINx - FEniCS 23](https://jsdokken.com/checkpointing-presentation/#/) or the examples in the [Documentation](https://jsdokken.com/adios4dolfinx/) for more information.
 
 For scalability, the code uses [MPI Neighbourhood collectives](https://www.mpi-forum.org/docs/mpi-3.1/mpi31-report/node200.htm) for communication across processes.
 
+## Statement of Need
+
+As the usage of high performance computing clusters increases, more and more large-scale, long-running simulations are deployed.
+The need for storing intermediate solutions from such simulations are crucial, as the HPC system might crash, or the simulation might crash or exceed the alloted computational budget.
+Having a checkpoint of related variables, such as the solutions to partial differential equations (PDEs) is therefore essential.
+The `adios4dolfinx` library extends the [DOLFINx](https://github.com/FEniCS/dolfinx/) computational framework for solving PDEs with checkpointing functionality, such that immediate solutions and mesh information can be stored and re-used in another simulation.
+
 ## Installation
 
+Compatibility with DOLFINx:
+
+- ADIOS4DOLFINx v0.7.3 is compatible with DOLFINx v0.7.x
+- ADIOS4DOLFINx v0.8.1 is compatible with DOLFINx v0.8.x
+
+### Dependencies
+
+The library depends on the Python-interface of [DOLFINx](https://github.com/) and an MPI-build of [ADIOS2](https://adios2.readthedocs.io/en/latest/setting_up/setting_up.html#as-package) and can therefore not be installed through PyPi, but has to be installed through Conda, Spack or from source.
+
 ### Docker
 
-ADIOS2 is installed in the official DOLFINx containers.
+An MPI build of ADIOS2 is installed in the official DOLFINx containers, and thus there are no additional dependencies required to install `adios4dolfinx`
+on top of DOLFINx in these images.
+
+Create a Docker container, named for instance `dolfinx-checkpoint`.
+Use the `nightly` tag to get the main branch of DOLFINx, or `stable` to get the latest stable release
 
 ```bash
 docker run -ti -v $(pwd):/root/shared -w /root/shared --name=dolfinx-checkpoint ghcr.io/fenics/dolfinx/dolfinx:nightly
 ```
 
+For the latest version compatible with nightly (with the ability to run the test suite), use
+
+```bash
+python3 -m pip install adios4dolfinx[test]@git+https://github.com/jorgensd/adios4dolfinx@main
+```
+
+If you are using the `stable` image, you can install `adios4dolfinx` from [PYPI](https://pypi.org/project/adios4dolfinx/) with
+
+```bash
+python3 -m pip install adios4dolfinx[test]
+```
+
+This docker container can be opened with
+
+```bash
+docker container start -i dolfinx-checkpoint
+```
+
+at a later instance
+
 ### Conda
 
-To use with conda (DOLFINx release v0.7.0 works with v0.7.3 of ADIOS4DOLFINx)
+> [!NOTE]  
+> Conda supports the stable release of DOLFINx, and thus the appropriate version should be installed, see the section above for more details.
+
+Following is a minimal recipe of how to install adios4dolfinx, given that you have conda installed on your system.
 
 ```bash
 conda create -n dolfinx-checkpoint python=3.10
 conda activate dolfinx-checkpoint
-conda install -c conda-forge fenics-dolfinx pip adios2
-python3 -m pip install git+https://github.com/jorgensd/adios4dolfinx@v0.7.2
+conda install -c conda-forge fenics-dolfinx pip adios2=*=mpi_*
+python3 -m pip install adios4dolfinx[test]@git+https://github.com/jorgensd/adios4dolfinx@v0.8.1
 ```
 
+> [!NOTE]
+> To run the tests or demos associated with the code, install `ipyparallel` in your environment, for instance by calling
+>
+> ```bash
+> python3 -m pip install adios4dolfinx[test]@git+https://github.com/jorgensd/adios4dolfinx@v0.8.1
+> ```
+
 ## Functionality
 
 ### DOLFINx
 
 - Reading and writing meshes, using `adios4dolfinx.read/write_mesh`
 - Reading and writing meshtags associated to meshes `adios4dolfinx.read/write_meshtags`
 - Reading checkpoints for any element (serial and parallel, arbitrary number of functions and timesteps per file). Use `adios4dolfinx.read/write_function`.
@@ -46,14 +96,25 @@
 
 > [!IMPORTANT]  
 > A checkpoint file supports multiple functions and multiple time steps, as long as the functions are associated with the same mesh
 
 > [!IMPORTANT]  
 > Only one mesh per file is allowed
 
+## Example Usage
+
+The repository contains many documented examples of usage, in the `docs`-folder, including
+
+- [Reading and writing mesh checkpoints](./docs/writing_mesh_checkpoint.py)
+- [Storing mesh partitioning data](./docs/partitioned_mesh.py)
+- [Writing mesh-tags to a checkpoint](./docs/meshtags.py)
+- [Reading and writing function checkpoints](./docs/writing_functions_checkpoint.py)
+- [Checkpoint on input mesh](./docs/original_checkpoint.py)
+  Further examples can be found at [ADIOS4DOLFINx examples](https://jsdokken.com/adios4dolfinx/)
+
 ### Backwards compatibility
 
 > [!WARNING]
 > If you are using v0.7.2, you are adviced to upgrade to v0.7.3, as it contains som crucial fixes for openmpi.
 
 ### Legacy DOLFIN
 
@@ -61,53 +122,52 @@
 
 - Reading meshes from the DOLFIN HDF5File-format
 - Reading checkpoints from the DOLFIN HDF5File-format (one checkpoint per file only)
 - Reading checkpoints from the DOLFIN XDMFFile-format (one checkpoint per file only, and only uses the `.h5` file)
 
 See the [API](./docs/api) for more information.
 
-## Long term plan
+## Testing
 
-The long term plan is to get this library merged into DOLFINx (rewritten in C++ with appropriate Python-bindings).
+This library uses `pytest` for testing.
+To execute the tests, one should first install the library and its dependencies, as listed above.
+Then, can execute all tests by calling
 
-# Contributor guidelines
-When contributing to this repository, please first [create an issue](https://github.com/jorgensd/adios4dolfinx/issues/new/choose) containing information about the missing feature or the bug that you would like to fix. Here you can discuss the change you want to make with the maintainers of the repository.
+```bash
+python3 -m pytest .
+```
 
-Please note we have a code of conduct, please follow it in all your interactions with the project.
+### Testing against data from legacy dolfin
 
-## New contributor guide
+Some tests check the capability of reading data created with the legacy version of DOLFIN.
+To create this dataset, start a docker container with legacy DOLFIN, for instance:
 
-To get an overview of the project, read the [documentation](https://jorgensd.github.io/adios4dolfinx). Here are some resources to help you get started with open source contributions:
+```bash
+docker run -ti -v $(pwd):/root/shared -w /root/s
+hared --rm ghcr.io/scientificcomputing/fenics:2024-02-19
+```
 
-- [Finding ways to contribute to open source on GitHub](https://docs.github.com/en/get-started/exploring-projects-on-github/finding-ways-to-contribute-to-open-source-on-github)
-- [Set up Git](https://docs.github.com/en/get-started/quickstart/set-up-git)
-- [GitHub flow](https://docs.github.com/en/get-started/quickstart/github-flow)
-- [Collaborating with pull requests](https://docs.github.com/en/github/collaborating-with-pull-requests)
+Then, inside this container, call
 
-## Pull Request Process
+```bash
+python3 ./tests/create_legacy_data.py --output-dir=legacy
+```
 
+### Testing against data from older versions of ADIOS4DOLFINx
 
-### Pull Request
+Some tests check the capability to read data generated by `adios4dolfinx<0.7.2`.
+To generate data for these tests use the following commands:
 
-- When you're finished with the changes, create a pull request, also known as a PR. It is also OK to create a [draft pull request](https://github.blog/2019-02-14-introducing-draft-pull-requests/) from the very beginning. Once you are done you can click on the ["Ready for review"] button. You can also [request a review](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/requesting-a-pull-request-review) from one of the maintainers.
-- Don't forget to [link PR to the issue that you opened ](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue).
-- Enable the checkbox to [allow maintainer edits](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/allowing-changes-to-a-pull-request-branch-created-from-a-fork) so the branch can be updated for a merge.
-Once you submit your PR, a team member will review your proposal. We may ask questions or request for additional information.
-- We may ask for changes to be made before a PR can be merged, either using [suggested changes](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/incorporating-feedback-in-your-pull-request) or pull request comments. You can apply suggested changes directly through the UI. You can make any other changes in your fork, then commit them to your branch.
-- As you update your PR and apply changes, mark each conversation as [resolved](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/commenting-on-a-pull-request#resolving-conversations).
-- If you run into any merge issues, checkout this [git tutorial](https://lab.github.com/githubtraining/managing-merge-conflicts) to help you resolve merge conflicts and other issues.
-- Please make sure that all tests are passing, github pages renders nicely, and code coverage are are not lower than before your contribution. You see the different github action workflows by clicking the "Action" tab in the GitHub repository.
+```bash
+docker run -ti -v $(pwd):/root/shared -w /root/shared --rm ghcr.io/fenics/dolfinx/dolfinx:v0.7.3
+```
 
-Note that for a pull request to be accepted, it has to pass all the tests on CI, which includes:
-- `mypy`: typechecking
-- `ruff`: Code formatting
-- `pytest`: Successfull execution of all tests in the `tests` folder.
+Then, inside the container, call
 
+```bash
+python3 -m pip install adios4dolfinx==0.7.1
+python3 ./tests/create_legacy_checkpoint.py --output-dir=legacy_checkpoint
+```
 
-### Our Pledge
+## Long term plan
 
-In the interest of fostering an open and welcoming environment, we as
-contributors and maintainers pledge to making participation in our project and
-our community a harassment-free experience for everyone, regardless of age, body
-size, disability, ethnicity, gender identity and expression, level of experience,
-nationality, personal appearance, race, religion, or sexual identity and
-orientation.
+The long term plan is to get this library merged into DOLFINx (rewritten in C++ with appropriate Python-bindings).
```

### Comparing `adios4dolfinx-0.8.0.dev0/pyproject.toml` & `adios4dolfinx-0.8.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system] # Require setuptool version due to https://github.com/pypa/setuptools/issues/2938
 requires = ["setuptools>=61.0.0", "wheel"]
 
 [project]
 name = "adios4dolfinx"
-version = "0.8.0.dev0"
+version = "0.8.1"
 description = "Checkpointing functionality for DOLFINx meshes/functions with ADIOS2"
 authors = [{ name = "Jørgen S. Dokken", email = "dokken@simula.no" }]
 license = { file = "LICENSE" }
 readme = "README.md"
-dependencies = ["fenics-dolfinx>=0.8.0.dev0"]
+dependencies = ["fenics-dolfinx>=0.8.0"]
 
 [project.optional-dependencies]
 test = ["pytest", "coverage", "ipyparallel"]
 dev = ["pdbpp", "ipython", "mypy", "ruff"]
 docs = ["jupyter-book", "ipyparallel", "ipywidgets"]
 all = ["adios4dolfinx[test,dev,docs]"]
```

### Comparing `adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/__init__.py` & `adios4dolfinx-0.8.1/src/adios4dolfinx/__init__.py`

 * *Files identical despite different names*

### Comparing `adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/adios2_helpers.py` & `adios4dolfinx-0.8.1/src/adios4dolfinx/adios2_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from contextlib import contextmanager
 from pathlib import Path
-from typing import NamedTuple
+from typing import NamedTuple, Union
 
 from mpi4py import MPI
 
 import adios2
 import dolfinx.cpp.graph
 import dolfinx.graph
 import numpy as np
@@ -40,15 +40,15 @@
     io: adios2.IO
     file: adios2.Engine
 
 
 @contextmanager
 def ADIOSFile(
     adios: adios2.ADIOS,
-    filename: Path | str,
+    filename: Union[Path, str],
     engine: str,
     mode: adios2.Mode,
     io_name: str,
 ):
     io = adios.DeclareIO(io_name)
     io.SetEngine(engine)
     file = io.Open(str(filename), mode)
@@ -58,15 +58,15 @@
         file.Close()
         adios.RemoveIO(io_name)
 
 
 def read_cell_perms(
     adios: adios2.ADIOS,
     comm: MPI.Intracomm,
-    filename: Path | str,
+    filename: Union[Path, str],
     variable: str,
     num_cells_global: np.int64,
     engine: str,
 ) -> npt.NDArray[np.uint32]:
     """
     Read cell permutation from file with given communicator,
     Split in continuous chunks based on number of cells in the mesh (global).
@@ -122,20 +122,20 @@
 
     return in_perm
 
 
 def read_adjacency_list(
     adios: adios2.ADIOS,
     comm: MPI.Intracomm,
-    filename: Path | str,
+    filename: Union[Path, str],
     dofmap: str,
     dofmap_offsets: str,
     num_cells_global: np.int64,
     engine: str,
-) -> dolfinx.cpp.graph.AdjacencyList_int64 | dolfinx.cpp.graph.AdjacencyList_int32:
+) -> Union[dolfinx.cpp.graph.AdjacencyList_int64, dolfinx.cpp.graph.AdjacencyList_int32]:
     """
     Read an adjacency-list from an ADIOS file with given communicator.
     The adjancency list is split in to a flat array (data) and its corresponding offset.
 
     Args:
         adios: The ADIOS instance
         comm: The MPI communicator used to read the data
@@ -201,15 +201,15 @@
 
     # Return local dofmap
     return dolfinx.graph.adjacencylist(in_dofmap, in_offsets.astype(np.int32))
 
 
 def read_array(
     adios: adios2.ADIOS,
-    filename: Path | str,
+    filename: Union[Path, str],
     array_name: str,
     engine: str,
     comm: MPI.Intracomm,
     time: float = 0.0,
     time_name: str = "",
     legacy: bool = False,
 ) -> tuple[npt.NDArray[valid_function_types], int]:
```

### Comparing `adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/checkpointing.py` & `adios4dolfinx-0.8.1/src/adios4dolfinx/checkpointing.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # This file is part of adios4dolfinx
 #
 # SPDX-License-Identifier:    MIT
 
 from __future__ import annotations
 
+import typing
 from pathlib import Path
 
 from mpi4py import MPI
 
 import adios2
 import basix
 import dolfinx
@@ -26,48 +27,56 @@
 )
 from .comm_helpers import (
     send_and_recv_cell_perm,
     send_dofmap_and_recv_values,
     send_dofs_and_recv_values,
 )
 from .structures import FunctionData, MeshData
-from .utils import compute_dofmap_pos, compute_local_range, index_owner, unroll_dofmap
+from .utils import (
+    compute_dofmap_pos,
+    compute_local_range,
+    index_owner,
+    unroll_dofmap,
+    unroll_insert_position,
+)
 from .writers import write_function as _internal_function_writer
 from .writers import write_mesh as _internal_mesh_writer
 
 adios2 = resolve_adios_scope(adios2)
 
 __all__ = [
+    "read_mesh_data",
     "read_mesh",
     "write_function",
     "read_function",
     "write_mesh",
     "read_meshtags",
     "write_meshtags",
     "read_attributes",
     "write_attributes",
 ]
 
 
 def write_attributes(
-    filename: Path | str,
+    filename: typing.Union[Path, str],
     comm: MPI.Intracomm,
     name: str,
     attributes: dict[str, np.ndarray],
     engine: str = "BP4",
 ):
     """Write attributes to file using ADIOS2.
 
     Args:
         filename: Path to file to write to
         comm: MPI communicator used in storage
         name: Name of the attributes
         attributes: Dictionary of attributes to write to file
         engine: ADIOS2 engine to use
     """
+
     adios = adios2.ADIOS(comm)
     with ADIOSFile(
         adios=adios,
         filename=filename,
         mode=adios2.Mode.Append,
         engine=engine,
         io_name="AttributesWriter",
@@ -78,30 +87,29 @@
             adios_file.io.DefineAttribute(f"{name}_{k}", v)
 
         adios_file.file.PerformPuts()
         adios_file.file.EndStep()
 
 
 def read_attributes(
-    filename: Path | str,
+    filename: typing.Union[Path, str],
     comm: MPI.Intracomm,
     name: str,
     engine: str = "BP4",
 ) -> dict[str, np.ndarray]:
     """Read attributes from file using ADIOS2.
 
     Args:
         filename: Path to file to read from
         comm: MPI communicator used in storage
         name: Name of the attributes
         engine: ADIOS2 engine to use
     Returns:
         The attributes
     """
-
     adios = adios2.ADIOS(comm)
     with ADIOSFile(
         adios=adios,
         filename=filename,
         mode=adios2.Mode.Read,
         engine=engine,
         io_name="AttributesReader",
@@ -113,19 +121,19 @@
                 a = adios_file.io.InquireAttribute(k)
                 attributes[k[len(name) + 1 :]] = a.Data()
         adios_file.file.EndStep()
     return attributes
 
 
 def write_meshtags(
-    filename: Path | str,
+    filename: typing.Union[Path, str],
     mesh: dolfinx.mesh.Mesh,
     meshtags: dolfinx.mesh.MeshTags,
     engine: str = "BP4",
-    meshtag_name: str | None = None,
+    meshtag_name: typing.Optional[str] = None,
 ):
     """
     Write meshtags associated with input mesh to file.
 
     .. note::
         For this checkpoint to work, the mesh must be written to file
         using :func:`write_mesh` before calling this function.
@@ -192,15 +200,15 @@
         adios_file.io.DefineAttribute(name + "_dim", np.array([meshtags.dim], dtype=np.uint8))
 
         adios_file.file.PerformPuts()
         adios_file.file.EndStep()
 
 
 def read_meshtags(
-    filename: Path | str,
+    filename: typing.Union[Path, str],
     mesh: dolfinx.mesh.Mesh,
     meshtag_name: str,
     engine: str = "BP4",
 ) -> dolfinx.mesh.MeshTags:
     """
     Read meshtags from file and return a :class:`dolfinx.mesh.MeshTags` object.
 
@@ -272,16 +280,16 @@
         values.SetSelection([[topology_range[0]], [topology_range[1] - topology_range[0]]])
         tag_values = np.empty((topology_range[1] - topology_range[0]), dtype=np.int32)
         adios_file.file.Get(values, tag_values, adios2.Mode.Deferred)
 
         adios_file.file.PerformGets()
         adios_file.file.EndStep()
 
-    local_entities, local_values = dolfinx.cpp.io.distribute_entity_data(
-        mesh._cpp_object, int(dim), mesh_entities, tag_values
+    local_entities, local_values = dolfinx.io.distribute_entity_data(
+        mesh, int(dim), mesh_entities.astype(np.int32), tag_values
     )
     mesh.topology.create_connectivity(dim, 0)
     mesh.topology.create_connectivity(dim, mesh.topology.dim)
 
     adj = dolfinx.cpp.graph.AdjacencyList_int32(local_entities)
 
     local_values = np.array(local_values, dtype=np.int32)
@@ -289,20 +297,20 @@
     mt = dolfinx.mesh.meshtags_from_entities(mesh, int(dim), adj, local_values)
     mt.name = meshtag_name
 
     return mt
 
 
 def read_function(
-    filename: Path | str,
+    filename: typing.Union[Path, str],
     u: dolfinx.fem.Function,
     engine: str = "BP4",
     time: float = 0.0,
     legacy: bool = False,
-    name: str | None = None,
+    name: typing.Optional[str] = None,
 ):
     """
     Read checkpoint from file and fill it into `u`.
 
     Args:
         filename: Path to checkpoint
         u: Function to fill
@@ -372,26 +380,35 @@
 
         # Read input cell permutations on dofmap process
         local_input_range = compute_local_range(comm, num_cells_global)
         input_local_cell_index = inc_cells - local_input_range[0]
         input_perms = read_cell_perms(
             adios, comm, filename, "CellPermutations", num_cells_global, engine
         )
+        # Start by sorting data array by cell permutation
+        num_dofs_per_cell = input_dofmap.offsets[1:] - input_dofmap.offsets[:-1]
+        assert np.allclose(num_dofs_per_cell, num_dofs_per_cell[0])
+
+        # Sort dofmap by input local cell index
+        input_perms_sorted = input_perms[input_local_cell_index]
+        unrolled_dofmap_position = unroll_insert_position(
+            input_local_cell_index, num_dofs_per_cell[0]
+        )
+        dofmap_sorted_by_input = recv_array[unrolled_dofmap_position]
 
         # First invert input data to reference element then transform to current mesh
-        for i, l_cell in enumerate(input_local_cell_index):
-            start, end = input_dofmap.offsets[l_cell : l_cell + 2]
-            # FIXME: Tempoary cast uint32 to integer as transformations
-            # doesn't support uint32 with the switch to nanobind
-            element.pre_apply_transpose_dof_transformation(
-                recv_array[int(start) : int(end)], int(input_perms[l_cell]), bs
-            )
-            element.pre_apply_inverse_transpose_dof_transformation(
-                recv_array[int(start) : int(end)], int(inc_perms[i]), bs
-            )
+        element.Tt_apply(dofmap_sorted_by_input, input_perms_sorted, bs)
+        element.Tt_inv_apply(dofmap_sorted_by_input, inc_perms, bs)
+        # Compute invert permutation
+        inverted_perm = np.empty_like(unrolled_dofmap_position)
+        inverted_perm[unrolled_dofmap_position] = np.arange(
+            len(unrolled_dofmap_position), dtype=inverted_perm.dtype
+        )
+        recv_array = dofmap_sorted_by_input[inverted_perm]
+
     # ------------------Step 6----------------------------------------
     # For each dof owned by a process, find the local position in the dofmap.
     V = u.function_space
     local_cells, dof_pos = compute_dofmap_pos(V)
     input_cells = V.mesh.topology.original_cell_index[local_cells]
     num_cells_global = V.mesh.topology.index_map(V.mesh.topology.dim).size_global
     owners = index_owner(V.mesh.comm, input_cells, num_cells_global)
@@ -415,37 +432,37 @@
         recv_array,
         input_dofmap.offsets,
     )
     u.x.array[: len(owned_values)] = owned_values
     u.x.scatter_forward()
 
 
-def read_mesh(
-    filename: Path | str,
+def read_mesh_data(
+    filename: typing.Union[Path, str],
     comm: MPI.Intracomm,
     engine: str = "BP4",
     ghost_mode: dolfinx.mesh.GhostMode = dolfinx.mesh.GhostMode.shared_facet,
     time: float = 0.0,
     legacy: bool = False,
     read_from_partition: bool = False,
-) -> dolfinx.mesh.Mesh:
+) -> tuple[np.ndarray, np.ndarray, ufl.Mesh, typing.Callable]:
     """
-    Read an ADIOS2 mesh into DOLFINx.
+    Read an ADIOS2 mesh data for use with DOLFINx.
 
     Args:
         filename: Path to input file
         comm: The MPI communciator to distribute the mesh over
         engine: ADIOS engine to use for reading (BP4, BP5 or HDF5)
         ghost_mode: Ghost mode to use for mesh. If `read_from_partition`
             is set to `True` this option is ignored.
         time: Time stamp associated with mesh
         legacy: If checkpoint was made prior to time-dependent mesh-writer set to True
         read_from_partition: Read mesh with partition from file
     Returns:
-        The distributed mesh
+        The mesh topology, geometry, UFL domain and partition function
     """
     adios = adios2.ADIOS(comm)
 
     with ADIOSFile(
         adios=adios,
         filename=filename,
         mode=adios2.Mode.Read,
@@ -548,15 +565,53 @@
 
         def partitioner(comm: MPI.Intracomm, n, m, topo):
             assert len(partition_graph.offsets) - 1 == topo.num_nodes
             return partition_graph
     else:
         partitioner = dolfinx.cpp.mesh.create_cell_partitioner(ghost_mode)
 
-    return dolfinx.mesh.create_mesh(comm, mesh_topology, mesh_geometry, domain, partitioner)
+    return mesh_topology, mesh_geometry, domain, partitioner
+
+
+def read_mesh(
+    filename: typing.Union[Path, str],
+    comm: MPI.Intracomm,
+    engine: str = "BP4",
+    ghost_mode: dolfinx.mesh.GhostMode = dolfinx.mesh.GhostMode.shared_facet,
+    time: float = 0.0,
+    legacy: bool = False,
+    read_from_partition: bool = False,
+) -> dolfinx.mesh.Mesh:
+    """
+    Read an ADIOS2 mesh into DOLFINx.
+
+    Args:
+        filename: Path to input file
+        comm: The MPI communciator to distribute the mesh over
+        engine: ADIOS engine to use for reading (BP4, BP5 or HDF5)
+        ghost_mode: Ghost mode to use for mesh. If `read_from_partition`
+            is set to `True` this option is ignored.
+        time: Time stamp associated with mesh
+        legacy: If checkpoint was made prior to time-dependent mesh-writer set to True
+        read_from_partition: Read mesh with partition from file
+    Returns:
+        The distributed mesh
+    """
+    return dolfinx.mesh.create_mesh(
+        comm,
+        *read_mesh_data(
+            filename,
+            comm,
+            engine=engine,
+            ghost_mode=ghost_mode,
+            time=time,
+            legacy=legacy,
+            read_from_partition=read_from_partition,
+        ),
+    )
 
 
 def write_mesh(
     filename: Path,
     mesh: dolfinx.mesh.Mesh,
     engine: str = "BP4",
     mode: adios2.Mode = adios2.Mode.Write,
@@ -650,20 +705,20 @@
         mode=mode,
         time=time,
         io_name="MeshWriter",
     )
 
 
 def write_function(
-    filename: Path | str,
+    filename: typing.Union[Path, str],
     u: dolfinx.fem.Function,
     engine: str = "BP4",
     mode: adios2.Mode = adios2.Mode.Append,
     time: float = 0.0,
-    name: str | None = None,
+    name: typing.Optional[str] = None,
 ):
     """
     Write function checkpoint to file.
 
     Args:
         u: Function to write to file
         filename: Path to write to
```

### Comparing `adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/comm_helpers.py` & `adios4dolfinx-0.8.1/src/adios4dolfinx/comm_helpers.py`

 * *Files identical despite different names*

### Comparing `adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/legacy_readers.py` & `adios4dolfinx-0.8.1/src/adios4dolfinx/legacy_readers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # This file is part of adios4dolfinx
 #
 # SPDX-License-Identifier:    MIT
 
 from __future__ import annotations
 
 import pathlib
+import typing
 
 from mpi4py import MPI
 
 import adios2
 import basix
 import dolfinx
 import numpy as np
@@ -272,28 +273,28 @@
 
     Args:
         comm: MPI communicator to distribute mesh over
         filename: Path to `h5` or `xdmf` file
         group: Name of mesh in `h5`-file
         cell_type: What type of cell type, by default tetrahedron.
     """
+    # Make sure we use the HDF5File and check that the file is present
+    filename = pathlib.Path(filename).with_suffix(".h5")
+    if not filename.is_file():
+        raise FileNotFoundError(f"File {filename} does not exist")
+
     # Create ADIOS2 reader
     adios = adios2.ADIOS(comm)
     with ADIOSFile(
         adios=adios,
         filename=filename,
         mode=adios2.Mode.Read,
         io_name="Mesh reader",
         engine="HDF5",
     ) as adios_file:
-        # Make sure we use the HDF5File and check that the file is present
-        filename = pathlib.Path(filename).with_suffix(".h5")
-        if not filename.is_file():
-            raise FileNotFoundError(f"File {filename} does not exist")
-
         # Get mesh topology (distributed)
         if f"{group}/topology" not in adios_file.io.AvailableVariables().keys():
             raise KeyError(f"Mesh topology not found at '{group}/topology'")
         topology = adios_file.io.InquireVariable(f"{group}/topology")
         shape = topology.Shape()
         local_range = compute_local_range(MPI.COMM_WORLD, shape[0])
         topology.SetSelection([[local_range[0], 0], [local_range[1] - local_range[0], shape[1]]])
@@ -325,15 +326,15 @@
 
 
 def read_function_from_legacy_h5(
     filename: pathlib.Path,
     comm: MPI.Intracomm,
     u: dolfinx.fem.Function,
     group: str = "mesh",
-    step: int | None = None,
+    step: typing.Optional[int] = None,
 ):
     """
     Read function from a `h5`-file generated by legacy DOLFIN `HDF5File.write`
     or `XDMF.write_checkpoint`.
 
     Args:
         comm : MPI communicator to distribute mesh over
```

### Comparing `adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/original_checkpoint.py` & `adios4dolfinx-0.8.1/src/adios4dolfinx/original_checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # This file is part of adios4dolfinx
 #
 # SPDX-License-Identifier:    MIT
 
 from __future__ import annotations
 
+import typing
 from pathlib import Path
 
 from mpi4py import MPI
 
 import adios2
 import dolfinx
 import numpy as np
@@ -195,15 +196,15 @@
         ownership_offset=None,
         partition_range=None,
         partition_global=None,
     )
 
 
 def create_function_data_on_original_mesh(
-    u: dolfinx.fem.Function, name: str | None = None
+    u: dolfinx.fem.Function, name: typing.Optional[str] = None
 ) -> FunctionData:
     """
     Create data object to save with ADIOS2
     """
     mesh = u.function_space.mesh
 
     # Compute what cells owned by current process should be sent to what output process
@@ -323,20 +324,20 @@
         dofmap_range=dofmap_imap.local_range,
         global_dofs_in_dofmap=dofmap_imap.size_global,
         name=func_name,
     )
 
 
 def write_function_on_input_mesh(
-    filename: Path | str,
+    filename: typing.Union[Path, str],
     u: dolfinx.fem.Function,
     engine: str = "BP4",
     mode: adios2.Mode = adios2.Mode.Append,
     time: float = 0.0,
-    name: str | None = None,
+    name: typing.Optional[str] = None,
 ):
     """
     Write function checkpoint (to be read with the input mesh).
 
     Parameters:
         u: The function to checkpoint
         filename: The filename to write to
@@ -355,15 +356,17 @@
         engine,
         mode,
         time,
         io_name="OriginalFunctionWriter",
     )
 
 
-def write_mesh_input_order(filename: Path | str, mesh: dolfinx.mesh.Mesh, engine: str = "BP4"):
+def write_mesh_input_order(
+    filename: typing.Union[Path, str], mesh: dolfinx.mesh.Mesh, engine: str = "BP4"
+):
     """
     Write mesh to checkpoint file in original input ordering
     """
 
     mesh_data = create_original_mesh_data(mesh)
     fname = Path(filename)
     write_mesh(fname, mesh.comm, mesh_data, engine, io_name="OriginalMeshWriter")
```

### Comparing `adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/snapshot.py` & `adios4dolfinx-0.8.1/src/adios4dolfinx/snapshot.py`

 * *Files identical despite different names*

### Comparing `adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/structures.py` & `adios4dolfinx-0.8.1/src/adios4dolfinx/structures.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # This file is part of adios4dolfinx
 #
 # SPDX-License-Identifier:    MIT
 
 from __future__ import annotations
 
+import typing
 from dataclasses import dataclass
 
 import numpy as np
 import numpy.typing as npt
 
 """Internal library classes for storing mesh and function data"""
 __all__ = ["MeshData", "FunctionData"]
@@ -29,19 +30,21 @@
 
     cell_type: str
     degree: int
     lagrange_variant: int
 
     # Partitioning_information
     store_partition: bool
-    partition_processes: int | None  # Number of processes in partition
-    ownership_array: npt.NDArray[np.int32] | None  # Ownership array for cells
-    ownership_offset: npt.NDArray[np.int32] | None  # Ownership offset for cells
-    partition_range: tuple[int, int] | None  # Local insert position for partitioning information
-    partition_global: int | None
+    partition_processes: typing.Optional[int]  # Number of processes in partition
+    ownership_array: typing.Optional[npt.NDArray[np.int32]]  # Ownership array for cells
+    ownership_offset: typing.Optional[npt.NDArray[np.int32]]  # Ownership offset for cells
+    partition_range: typing.Optional[
+        tuple[int, int]
+    ]  # Local insert position for partitioning information
+    partition_global: typing.Optional[int]
 
 
 @dataclass
 class FunctionData:
     cell_permutations: npt.NDArray[np.uint32]  # Cell permutations for dofmap
     local_cell_range: tuple[int, int]  # Range of cells on current process
     num_cells_global: int  # Number of cells in global topology
```

### Comparing `adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/utils.py` & `adios4dolfinx-0.8.1/src/adios4dolfinx/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 """
 Vectorized numpy operations used internally in adios4dolfinx
 """
 
 from __future__ import annotations
 
+import typing
+
 from mpi4py import MPI
 
 import dolfinx
 import numpy as np
 import numpy.typing as npt
 
 __all__ = [
@@ -21,16 +23,16 @@
     "index_owner",
     "compute_dofmap_pos",
     "unroll_dofmap",
     "compute_insert_position",
     "unroll_insert_position",
 ]
 
-valid_function_types = np.float32 | np.float64 | np.complex64 | np.complex128
-valid_real_types = np.float32 | np.float64
+valid_function_types = typing.Union[np.float32, np.float64, np.complex64, np.complex128]
+valid_real_types = typing.Union[np.float32, np.float64]
 
 
 def compute_insert_position(
     data_owner: npt.NDArray[np.int32],
     destination_ranks: npt.NDArray[np.int32],
     out_size: npt.NDArray[np.int32],
 ) -> npt.NDArray[np.int32]:
```

### Comparing `adios4dolfinx-0.8.0.dev0/src/adios4dolfinx/writers.py` & `adios4dolfinx-0.8.1/src/adios4dolfinx/writers.py`

 * *Files identical despite different names*

### Comparing `adios4dolfinx-0.8.0.dev0/src/adios4dolfinx.egg-info/PKG-INFO` & `adios4dolfinx-0.8.1/src/adios4dolfinx.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: adios4dolfinx
-Version: 0.8.0.dev0
+Version: 0.8.1
 Summary: Checkpointing functionality for DOLFINx meshes/functions with ADIOS2
 Author-email: "Jørgen S. Dokken" <dokken@simula.no>
 License: Copyright 2023 Jørgen S. Dokken
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fenics-dolfinx>=0.8.0.dev0
+Requires-Dist: fenics-dolfinx>=0.8.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: ipyparallel; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pdbpp; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
@@ -26,47 +26,97 @@
 Provides-Extra: docs
 Requires-Dist: jupyter-book; extra == "docs"
 Requires-Dist: ipyparallel; extra == "docs"
 Requires-Dist: ipywidgets; extra == "docs"
 Provides-Extra: all
 Requires-Dist: adios4dolfinx[dev,docs,test]; extra == "all"
 
-# ADIOS2Wrappers for DOLFINx
+# ADIOS4DOLFINx - A framework for checkpointing in DOLFINx
 
-[![MIT](https://img.shields.io/github/license/jorgensd/adios4dolfinx)](LICENSE)
-[Read Latest Documentation](https://jsdokken.com/adios4dolfinx/)
+![MIT](https://img.shields.io/github/license/jorgensd/adios4dolfinx)
+[![status](https://joss.theoj.org/papers/7866cb142db8a803e32d79a109573d25/status.svg)](https://joss.theoj.org/papers/7866cb142db8a803e32d79a109573d25)
 
-This is an extension for [DOLFINx](https://github.com/FEniCS/dolfinx/) to checkpoint meshes, meshtags and functions using [ADIOS2](https://adios2.readthedocs.io/en/latest/).
+ADIOS4DOLFINx is an extension for [DOLFINx](https://github.com/FEniCS/dolfinx/) to checkpoint meshes, meshtags and functions using [ADIOS 2](https://adios2.readthedocs.io/en/latest/).
 
-The code uses the adios2 Python-wrappers to write DOLFINx objects to file, supporting N-to-M (_recoverable_) and N-to-N (_snapshot_) checkpointing.
-See: [Checkpointing in DOLFINx - FEniCS 23](https://jsdokken.com/checkpointing-presentation/#/) for more information.
+The code uses the ADIOS2 Python-wrappers to write DOLFINx objects to file, supporting N-to-M (_recoverable_) and N-to-N (_snapshot_) checkpointing.
+See: [Checkpointing in DOLFINx - FEniCS 23](https://jsdokken.com/checkpointing-presentation/#/) or the examples in the [Documentation](https://jsdokken.com/adios4dolfinx/) for more information.
 
 For scalability, the code uses [MPI Neighbourhood collectives](https://www.mpi-forum.org/docs/mpi-3.1/mpi31-report/node200.htm) for communication across processes.
 
+## Statement of Need
+
+As the usage of high performance computing clusters increases, more and more large-scale, long-running simulations are deployed.
+The need for storing intermediate solutions from such simulations are crucial, as the HPC system might crash, or the simulation might crash or exceed the alloted computational budget.
+Having a checkpoint of related variables, such as the solutions to partial differential equations (PDEs) is therefore essential.
+The `adios4dolfinx` library extends the [DOLFINx](https://github.com/FEniCS/dolfinx/) computational framework for solving PDEs with checkpointing functionality, such that immediate solutions and mesh information can be stored and re-used in another simulation.
+
 ## Installation
 
+Compatibility with DOLFINx:
+
+- ADIOS4DOLFINx v0.7.3 is compatible with DOLFINx v0.7.x
+- ADIOS4DOLFINx v0.8.1 is compatible with DOLFINx v0.8.x
+
+### Dependencies
+
+The library depends on the Python-interface of [DOLFINx](https://github.com/) and an MPI-build of [ADIOS2](https://adios2.readthedocs.io/en/latest/setting_up/setting_up.html#as-package) and can therefore not be installed through PyPi, but has to be installed through Conda, Spack or from source.
+
 ### Docker
 
-ADIOS2 is installed in the official DOLFINx containers.
+An MPI build of ADIOS2 is installed in the official DOLFINx containers, and thus there are no additional dependencies required to install `adios4dolfinx`
+on top of DOLFINx in these images.
+
+Create a Docker container, named for instance `dolfinx-checkpoint`.
+Use the `nightly` tag to get the main branch of DOLFINx, or `stable` to get the latest stable release
 
 ```bash
 docker run -ti -v $(pwd):/root/shared -w /root/shared --name=dolfinx-checkpoint ghcr.io/fenics/dolfinx/dolfinx:nightly
 ```
 
+For the latest version compatible with nightly (with the ability to run the test suite), use
+
+```bash
+python3 -m pip install adios4dolfinx[test]@git+https://github.com/jorgensd/adios4dolfinx@main
+```
+
+If you are using the `stable` image, you can install `adios4dolfinx` from [PYPI](https://pypi.org/project/adios4dolfinx/) with
+
+```bash
+python3 -m pip install adios4dolfinx[test]
+```
+
+This docker container can be opened with
+
+```bash
+docker container start -i dolfinx-checkpoint
+```
+
+at a later instance
+
 ### Conda
 
-To use with conda (DOLFINx release v0.7.0 works with v0.7.3 of ADIOS4DOLFINx)
+> [!NOTE]  
+> Conda supports the stable release of DOLFINx, and thus the appropriate version should be installed, see the section above for more details.
+
+Following is a minimal recipe of how to install adios4dolfinx, given that you have conda installed on your system.
 
 ```bash
 conda create -n dolfinx-checkpoint python=3.10
 conda activate dolfinx-checkpoint
-conda install -c conda-forge fenics-dolfinx pip adios2
-python3 -m pip install git+https://github.com/jorgensd/adios4dolfinx@v0.7.2
+conda install -c conda-forge fenics-dolfinx pip adios2=*=mpi_*
+python3 -m pip install adios4dolfinx[test]@git+https://github.com/jorgensd/adios4dolfinx@v0.8.1
 ```
 
+> [!NOTE]
+> To run the tests or demos associated with the code, install `ipyparallel` in your environment, for instance by calling
+>
+> ```bash
+> python3 -m pip install adios4dolfinx[test]@git+https://github.com/jorgensd/adios4dolfinx@v0.8.1
+> ```
+
 ## Functionality
 
 ### DOLFINx
 
 - Reading and writing meshes, using `adios4dolfinx.read/write_mesh`
 - Reading and writing meshtags associated to meshes `adios4dolfinx.read/write_meshtags`
 - Reading checkpoints for any element (serial and parallel, arbitrary number of functions and timesteps per file). Use `adios4dolfinx.read/write_function`.
@@ -78,14 +128,25 @@
 
 > [!IMPORTANT]  
 > A checkpoint file supports multiple functions and multiple time steps, as long as the functions are associated with the same mesh
 
 > [!IMPORTANT]  
 > Only one mesh per file is allowed
 
+## Example Usage
+
+The repository contains many documented examples of usage, in the `docs`-folder, including
+
+- [Reading and writing mesh checkpoints](./docs/writing_mesh_checkpoint.py)
+- [Storing mesh partitioning data](./docs/partitioned_mesh.py)
+- [Writing mesh-tags to a checkpoint](./docs/meshtags.py)
+- [Reading and writing function checkpoints](./docs/writing_functions_checkpoint.py)
+- [Checkpoint on input mesh](./docs/original_checkpoint.py)
+  Further examples can be found at [ADIOS4DOLFINx examples](https://jsdokken.com/adios4dolfinx/)
+
 ### Backwards compatibility
 
 > [!WARNING]
 > If you are using v0.7.2, you are adviced to upgrade to v0.7.3, as it contains som crucial fixes for openmpi.
 
 ### Legacy DOLFIN
 
@@ -93,53 +154,52 @@
 
 - Reading meshes from the DOLFIN HDF5File-format
 - Reading checkpoints from the DOLFIN HDF5File-format (one checkpoint per file only)
 - Reading checkpoints from the DOLFIN XDMFFile-format (one checkpoint per file only, and only uses the `.h5` file)
 
 See the [API](./docs/api) for more information.
 
-## Long term plan
+## Testing
 
-The long term plan is to get this library merged into DOLFINx (rewritten in C++ with appropriate Python-bindings).
+This library uses `pytest` for testing.
+To execute the tests, one should first install the library and its dependencies, as listed above.
+Then, can execute all tests by calling
 
-# Contributor guidelines
-When contributing to this repository, please first [create an issue](https://github.com/jorgensd/adios4dolfinx/issues/new/choose) containing information about the missing feature or the bug that you would like to fix. Here you can discuss the change you want to make with the maintainers of the repository.
+```bash
+python3 -m pytest .
+```
 
-Please note we have a code of conduct, please follow it in all your interactions with the project.
+### Testing against data from legacy dolfin
 
-## New contributor guide
+Some tests check the capability of reading data created with the legacy version of DOLFIN.
+To create this dataset, start a docker container with legacy DOLFIN, for instance:
 
-To get an overview of the project, read the [documentation](https://jorgensd.github.io/adios4dolfinx). Here are some resources to help you get started with open source contributions:
+```bash
+docker run -ti -v $(pwd):/root/shared -w /root/s
+hared --rm ghcr.io/scientificcomputing/fenics:2024-02-19
+```
 
-- [Finding ways to contribute to open source on GitHub](https://docs.github.com/en/get-started/exploring-projects-on-github/finding-ways-to-contribute-to-open-source-on-github)
-- [Set up Git](https://docs.github.com/en/get-started/quickstart/set-up-git)
-- [GitHub flow](https://docs.github.com/en/get-started/quickstart/github-flow)
-- [Collaborating with pull requests](https://docs.github.com/en/github/collaborating-with-pull-requests)
+Then, inside this container, call
 
-## Pull Request Process
+```bash
+python3 ./tests/create_legacy_data.py --output-dir=legacy
+```
 
+### Testing against data from older versions of ADIOS4DOLFINx
 
-### Pull Request
+Some tests check the capability to read data generated by `adios4dolfinx<0.7.2`.
+To generate data for these tests use the following commands:
 
-- When you're finished with the changes, create a pull request, also known as a PR. It is also OK to create a [draft pull request](https://github.blog/2019-02-14-introducing-draft-pull-requests/) from the very beginning. Once you are done you can click on the ["Ready for review"] button. You can also [request a review](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/requesting-a-pull-request-review) from one of the maintainers.
-- Don't forget to [link PR to the issue that you opened ](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue).
-- Enable the checkbox to [allow maintainer edits](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/allowing-changes-to-a-pull-request-branch-created-from-a-fork) so the branch can be updated for a merge.
-Once you submit your PR, a team member will review your proposal. We may ask questions or request for additional information.
-- We may ask for changes to be made before a PR can be merged, either using [suggested changes](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/incorporating-feedback-in-your-pull-request) or pull request comments. You can apply suggested changes directly through the UI. You can make any other changes in your fork, then commit them to your branch.
-- As you update your PR and apply changes, mark each conversation as [resolved](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/commenting-on-a-pull-request#resolving-conversations).
-- If you run into any merge issues, checkout this [git tutorial](https://lab.github.com/githubtraining/managing-merge-conflicts) to help you resolve merge conflicts and other issues.
-- Please make sure that all tests are passing, github pages renders nicely, and code coverage are are not lower than before your contribution. You see the different github action workflows by clicking the "Action" tab in the GitHub repository.
+```bash
+docker run -ti -v $(pwd):/root/shared -w /root/shared --rm ghcr.io/fenics/dolfinx/dolfinx:v0.7.3
+```
 
-Note that for a pull request to be accepted, it has to pass all the tests on CI, which includes:
-- `mypy`: typechecking
-- `ruff`: Code formatting
-- `pytest`: Successfull execution of all tests in the `tests` folder.
+Then, inside the container, call
 
+```bash
+python3 -m pip install adios4dolfinx==0.7.1
+python3 ./tests/create_legacy_checkpoint.py --output-dir=legacy_checkpoint
+```
 
-### Our Pledge
+## Long term plan
 
-In the interest of fostering an open and welcoming environment, we as
-contributors and maintainers pledge to making participation in our project and
-our community a harassment-free experience for everyone, regardless of age, body
-size, disability, ethnicity, gender identity and expression, level of experience,
-nationality, personal appearance, race, religion, or sexual identity and
-orientation.
+The long term plan is to get this library merged into DOLFINx (rewritten in C++ with appropriate Python-bindings).
```

### Comparing `adios4dolfinx-0.8.0.dev0/src/adios4dolfinx.egg-info/SOURCES.txt` & `adios4dolfinx-0.8.1/src/adios4dolfinx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adios4dolfinx-0.8.0.dev0/tests/test_attributes.py` & `adios4dolfinx-0.8.1/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `adios4dolfinx-0.8.0.dev0/tests/test_checkpointing.py` & `adios4dolfinx-0.8.1/tests/test_checkpointing.py`

 * *Files identical despite different names*

### Comparing `adios4dolfinx-0.8.0.dev0/tests/test_checkpointing_vector.py` & `adios4dolfinx-0.8.1/tests/test_checkpointing_vector.py`

 * *Files identical despite different names*

### Comparing `adios4dolfinx-0.8.0.dev0/tests/test_legacy_readers.py` & `adios4dolfinx-0.8.1/tests/test_legacy_readers.py`

 * *Files identical despite different names*

### Comparing `adios4dolfinx-0.8.0.dev0/tests/test_mesh_writer.py` & `adios4dolfinx-0.8.1/tests/test_mesh_writer.py`

 * *Files identical despite different names*

### Comparing `adios4dolfinx-0.8.0.dev0/tests/test_meshtags.py` & `adios4dolfinx-0.8.1/tests/test_meshtags.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import itertools
+import typing
 from collections import ChainMap
 
 from mpi4py import MPI
 
 import dolfinx
 import numpy as np
 import numpy.typing as npt
@@ -63,15 +64,15 @@
 
 
 def generate_reference_map(
     mesh: dolfinx.mesh.Mesh,
     meshtag: dolfinx.mesh.MeshTags,
     comm: MPI.Intracomm,
     root: int,
-) -> None | dict[str, tuple[int, npt.NDArray]]:
+) -> typing.Optional[dict[str, tuple[int, npt.NDArray]]]:
     """
     Helper function to generate map from meshtag value to its corresponding index and midpoint.
 
     Args:
         mesh: The mesh
         meshtag: The associated meshtag
         comm: MPI communicator to gather the map from all processes with
```

### Comparing `adios4dolfinx-0.8.0.dev0/tests/test_numpy_vectorization.py` & `adios4dolfinx-0.8.1/tests/test_numpy_vectorization.py`

 * *Files identical despite different names*

### Comparing `adios4dolfinx-0.8.0.dev0/tests/test_original_checkpoint.py` & `adios4dolfinx-0.8.1/tests/test_original_checkpoint.py`

 * *Files identical despite different names*

### Comparing `adios4dolfinx-0.8.0.dev0/tests/test_snapshot_checkpoint.py` & `adios4dolfinx-0.8.1/tests/test_snapshot_checkpoint.py`

 * *Files identical despite different names*

