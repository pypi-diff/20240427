# Comparing `tmp/phbuilder-1.2.4.tar.gz` & `tmp/phbuilder-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phbuilder-1.2.4.tar", last modified: Thu Feb 22 11:46:18 2024, max compression
+gzip compressed data, was "phbuilder-1.2.5.tar", last modified: Sat Apr 27 17:09:17 2024, max compression
```

## Comparing `phbuilder-1.2.4.tar` & `phbuilder-1.2.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2024-02-22 11:46:18.366519 phbuilder-1.2.4/
--rw-rw-r--   0 anton     (1000) anton     (1000)    35148 2023-08-11 14:36:04.000000 phbuilder-1.2.4/LICENSE
--rw-r--r--   0 anton     (1000) anton     (1000)    41013 2024-02-22 11:46:18.366519 phbuilder-1.2.4/PKG-INFO
--rw-rw-r--   0 anton     (1000) anton     (1000)    40154 2024-02-21 14:43:37.000000 phbuilder-1.2.4/README.md
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2024-02-22 11:46:18.362519 phbuilder-1.2.4/phbuilder/
--rw-rw-r--   0 anton     (1000) anton     (1000)      377 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/__init__.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2024-02-22 11:46:18.362519 phbuilder-1.2.4/phbuilder/ffield/
--rw-rw-r--   0 anton     (1000) anton     (1000)      659 2024-02-22 11:33:36.000000 phbuilder-1.2.4/phbuilder/ffield/README.md
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2024-02-22 11:46:18.366519 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/
--rw-rw-r--   0 anton     (1000) anton     (1000)    24234 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/atomtypes.atp
--rw-rw-r--   0 anton     (1000) anton     (1000)   116897 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/cmap.itp
--rw-rw-r--   0 anton     (1000) anton     (1000)  1470200 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/ffbonded.itp
--rw-rw-r--   0 anton     (1000) anton     (1000)  1923615 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/ffnonbonded.itp
--rw-rw-r--   0 anton     (1000) anton     (1000)    10332 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/forcefield.doc
--rw-rw-r--   0 anton     (1000) anton     (1000)      650 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/forcefield.itp
--rw-rw-r--   0 anton     (1000) anton     (1000)     1873 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/gb.itp
--rw-rw-r--   0 anton     (1000) anton     (1000)     1942 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/ions.itp
--rw-rw-r--   0 anton     (1000) anton     (1000)       78 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.arn
--rw-rw-r--   0 anton     (1000) anton     (1000)     1377 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.c.tdb
--rw-rw-r--   0 anton     (1000) anton     (1000)     8077 2023-10-05 10:56:49.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.hdb
--rw-rw-r--   0 anton     (1000) anton     (1000)     1480 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.n.tdb
--rw-rw-r--   0 anton     (1000) anton     (1000)      161 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.r2b
--rw-rw-r--   0 anton     (1000) anton     (1000)  2303819 2023-10-05 10:56:49.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.rtp
--rw-rw-r--   0 anton     (1000) anton     (1000)     4292 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.vsd
--rw-rw-r--   0 anton     (1000) anton     (1000)     4727 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/nbfix.itp
--rw-rw-r--   0 anton     (1000) anton     (1000)    54970 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/old_c36_cmap.itp
--rw-rw-r--   0 anton     (1000) anton     (1000)    38535 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/popc.itp
--rw-rw-r--   0 anton     (1000) anton     (1000)      484 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/spc.itp
--rw-rw-r--   0 anton     (1000) anton     (1000)      490 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/spce.itp
--rw-rw-r--   0 anton     (1000) anton     (1000)      817 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/tip3p.itp
--rw-rw-r--   0 anton     (1000) anton     (1000)     1011 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/tip4p.itp
--rw-rw-r--   0 anton     (1000) anton     (1000)      198 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/watermodels.dat
--rw-rw-r--   0 anton     (1000) anton     (1000)     2659 2024-02-22 11:33:36.000000 phbuilder-1.2.4/phbuilder/ffield/lambdagrouptypes.dat
--rw-rw-r--   0 anton     (1000) anton     (1000)     2779 2023-10-05 10:56:49.000000 phbuilder-1.2.4/phbuilder/ffield/residuetypes.dat
--rw-rw-r--   0 anton     (1000) anton     (1000)     4398 2023-10-05 10:56:49.000000 phbuilder-1.2.4/phbuilder/mdp.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    11556 2024-02-22 11:34:41.000000 phbuilder-1.2.4/phbuilder/parsecmdline.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    66237 2024-02-21 13:54:33.000000 phbuilder-1.2.4/phbuilder/phbuilder.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     6409 2023-08-30 13:10:43.000000 phbuilder-1.2.4/phbuilder/sanitize.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    11479 2023-09-15 14:32:43.000000 phbuilder-1.2.4/phbuilder/structure.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     4202 2023-08-11 14:36:04.000000 phbuilder-1.2.4/phbuilder/user.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2024-02-22 11:46:18.366519 phbuilder-1.2.4/phbuilder.egg-info/
--rw-r--r--   0 anton     (1000) anton     (1000)    41013 2024-02-22 11:46:18.000000 phbuilder-1.2.4/phbuilder.egg-info/PKG-INFO
--rw-rw-r--   0 anton     (1000) anton     (1000)     1815 2024-02-22 11:46:18.000000 phbuilder-1.2.4/phbuilder.egg-info/SOURCES.txt
--rw-rw-r--   0 anton     (1000) anton     (1000)        1 2024-02-22 11:46:18.000000 phbuilder-1.2.4/phbuilder.egg-info/dependency_links.txt
--rw-rw-r--   0 anton     (1000) anton     (1000)       54 2024-02-22 11:46:18.000000 phbuilder-1.2.4/phbuilder.egg-info/entry_points.txt
--rw-rw-r--   0 anton     (1000) anton     (1000)       39 2024-02-22 11:46:18.000000 phbuilder-1.2.4/phbuilder.egg-info/requires.txt
--rw-rw-r--   0 anton     (1000) anton     (1000)       10 2024-02-22 11:46:18.000000 phbuilder-1.2.4/phbuilder.egg-info/top_level.txt
--rw-rw-r--   0 anton     (1000) anton     (1000)      105 2023-08-11 14:36:04.000000 phbuilder-1.2.4/pyproject.toml
--rw-rw-r--   0 anton     (1000) anton     (1000)     1117 2024-02-22 11:46:18.370519 phbuilder-1.2.4/setup.cfg
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2024-04-27 17:09:17.329450 phbuilder-1.2.5/
+-rw-rw-r--   0 anton     (1000) anton     (1000)    35148 2023-08-11 14:36:04.000000 phbuilder-1.2.5/LICENSE
+-rw-r--r--   0 anton     (1000) anton     (1000)    40932 2024-04-27 17:09:17.329450 phbuilder-1.2.5/PKG-INFO
+-rw-rw-r--   0 anton     (1000) anton     (1000)    40025 2024-04-27 17:06:23.000000 phbuilder-1.2.5/README.md
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2024-04-27 17:09:17.313450 phbuilder-1.2.5/phbuilder/
+-rw-rw-r--   0 anton     (1000) anton     (1000)      377 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/__init__.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2024-04-27 17:09:17.317450 phbuilder-1.2.5/phbuilder/ffield/
+-rw-rw-r--   0 anton     (1000) anton     (1000)      659 2024-04-09 11:36:31.000000 phbuilder-1.2.5/phbuilder/ffield/README.md
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2024-04-27 17:09:17.329450 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/
+-rw-rw-r--   0 anton     (1000) anton     (1000)    24234 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/atomtypes.atp
+-rw-rw-r--   0 anton     (1000) anton     (1000)   116897 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/cmap.itp
+-rw-rw-r--   0 anton     (1000) anton     (1000)  1470200 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/ffbonded.itp
+-rw-rw-r--   0 anton     (1000) anton     (1000)  1923615 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/ffnonbonded.itp
+-rw-rw-r--   0 anton     (1000) anton     (1000)    10332 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/forcefield.doc
+-rw-rw-r--   0 anton     (1000) anton     (1000)      650 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/forcefield.itp
+-rw-rw-r--   0 anton     (1000) anton     (1000)     1873 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/gb.itp
+-rw-rw-r--   0 anton     (1000) anton     (1000)     1942 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/ions.itp
+-rw-rw-r--   0 anton     (1000) anton     (1000)       78 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.arn
+-rw-rw-r--   0 anton     (1000) anton     (1000)     1377 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.c.tdb
+-rw-rw-r--   0 anton     (1000) anton     (1000)     8077 2023-10-05 10:56:49.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.hdb
+-rw-rw-r--   0 anton     (1000) anton     (1000)     1480 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.n.tdb
+-rw-rw-r--   0 anton     (1000) anton     (1000)      161 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.r2b
+-rw-rw-r--   0 anton     (1000) anton     (1000)  2303819 2023-10-05 10:56:49.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.rtp
+-rw-rw-r--   0 anton     (1000) anton     (1000)     4292 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.vsd
+-rw-rw-r--   0 anton     (1000) anton     (1000)     4727 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/nbfix.itp
+-rw-rw-r--   0 anton     (1000) anton     (1000)    54970 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/old_c36_cmap.itp
+-rw-rw-r--   0 anton     (1000) anton     (1000)    38535 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/popc.itp
+-rw-rw-r--   0 anton     (1000) anton     (1000)      484 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/spc.itp
+-rw-rw-r--   0 anton     (1000) anton     (1000)      490 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/spce.itp
+-rw-rw-r--   0 anton     (1000) anton     (1000)      817 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/tip3p.itp
+-rw-rw-r--   0 anton     (1000) anton     (1000)     1011 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/tip4p.itp
+-rw-rw-r--   0 anton     (1000) anton     (1000)      198 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/watermodels.dat
+-rw-rw-r--   0 anton     (1000) anton     (1000)     2658 2024-04-27 17:06:23.000000 phbuilder-1.2.5/phbuilder/ffield/lambdagrouptypes.dat
+-rw-rw-r--   0 anton     (1000) anton     (1000)     2779 2023-10-05 10:56:49.000000 phbuilder-1.2.5/phbuilder/ffield/residuetypes.dat
+-rw-rw-r--   0 anton     (1000) anton     (1000)     4398 2023-10-05 10:56:49.000000 phbuilder-1.2.5/phbuilder/mdp.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    11975 2024-04-27 17:08:10.000000 phbuilder-1.2.5/phbuilder/parsecmdline.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    67483 2024-04-27 17:06:23.000000 phbuilder-1.2.5/phbuilder/phbuilder.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     7731 2024-04-27 17:06:23.000000 phbuilder-1.2.5/phbuilder/sanitize.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    11479 2023-09-15 14:32:43.000000 phbuilder-1.2.5/phbuilder/structure.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     4202 2023-08-11 14:36:04.000000 phbuilder-1.2.5/phbuilder/user.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2024-04-27 17:09:17.329450 phbuilder-1.2.5/phbuilder.egg-info/
+-rw-r--r--   0 anton     (1000) anton     (1000)    40932 2024-04-27 17:09:17.000000 phbuilder-1.2.5/phbuilder.egg-info/PKG-INFO
+-rw-rw-r--   0 anton     (1000) anton     (1000)     1815 2024-04-27 17:09:17.000000 phbuilder-1.2.5/phbuilder.egg-info/SOURCES.txt
+-rw-rw-r--   0 anton     (1000) anton     (1000)        1 2024-04-27 17:09:17.000000 phbuilder-1.2.5/phbuilder.egg-info/dependency_links.txt
+-rw-rw-r--   0 anton     (1000) anton     (1000)       54 2024-04-27 17:09:17.000000 phbuilder-1.2.5/phbuilder.egg-info/entry_points.txt
+-rw-rw-r--   0 anton     (1000) anton     (1000)       57 2024-04-27 17:09:17.000000 phbuilder-1.2.5/phbuilder.egg-info/requires.txt
+-rw-rw-r--   0 anton     (1000) anton     (1000)       10 2024-04-27 17:09:17.000000 phbuilder-1.2.5/phbuilder.egg-info/top_level.txt
+-rw-rw-r--   0 anton     (1000) anton     (1000)      118 2024-04-27 17:06:23.000000 phbuilder-1.2.5/pyproject.toml
+-rw-rw-r--   0 anton     (1000) anton     (1000)     1137 2024-04-27 17:09:17.329450 phbuilder-1.2.5/setup.cfg
```

### Comparing `phbuilder-1.2.4/LICENSE` & `phbuilder-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/PKG-INFO` & `phbuilder-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phbuilder
-Version: 1.2.4
+Version: 1.2.5
 Summary: System builder for constant-pH simulations in GROMACS.
 Home-page: https://gitlab.com/gromacs-constantph/phbuilder
 Author: Anton Jansen
 Author-email: anton.jansen@scilifelab.se
 Project-URL: Bug Tracker, https://gitlab.com/gromacs-constantph/phbuilder/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -14,14 +14,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argcomplete>=3.1.1
 Requires-Dist: configparser>=6.0.0
+Requires-Dist: sympy>=1.12
+Requires-Dist: numpy
 
 <div style="width: 830px">
 
 [![GitLab issues](https://img.shields.io/badge/issue_tracking-gitlab-blue.svg)](https://gitlab.com/gromacs-constantph/phbuilder/-/issues)
 
 <p align="center">
   <img src="figures/logo.png" width="600"/>
@@ -235,37 +237,29 @@
 
 ```
 gmx cphmd -s MD.tpr -e MD.edr -numplot 1
 ```
 
 # Performing titrations
 
-Performing a computational titration is helpful for determining the microscopic pKas of titratable sites. After steps 1 to 9 of the basic workflow have been completed, one can use the included [create_titration.py](scripts/create_titration.py) to setup a titration. For example, the command:
+Performing a computational titration is helpful for determining the pKa shifts of titratable sites. After steps 1 to 9 of the basic workflow have been completed, one can use the included [create_titration.py](scripts/create_titration.py) to setup a titration. For example, the command:
 
 ```
 create_titration.py -f MD.mdp -c NPT.pdb -p topol.top -n index.ndx -pH 1:10:1 -nr 2
 ```
 
 creates directories corresponding to pH 1 to 9, with each subdirectory containing two replicates (each containing the appropriate input files for `gmx mdrun`).
 
-**NOTE** `create_titration.py` currently requires small modifications of `MD.mdp` file. In case of multisite groups (e.g. histidine), one of the $\lambda$-coordinates (usually the first coordinate associated with the multisite group) should have pH value equal to $\text{p}K_\text{a}$ (check [manual](https://gitlab.com/gromacs-constantph/constantph/-/blob/main/manual/constantph_usage.md)). To achieve this, `create_titration.py` searches through the **.mdp** file, and if it sees pH and $\text{p}K_\text{a}$ in one line, it replaces pH with actual numeric value. This will ensure the correct set up at all pH values. To give an example:
-```
-lambda-dynamics-group-type3-state-1-reference-pka      = pH
-```
-this line will be sequentially changed to 
+The minor change is at step 7. When parameters are generated, `phbuilder genparams` needs to be called with the `-titr` option:
+
 ```
-lambda-dynamics-group-type3-state-1-reference-pka      = 1.0
-lambda-dynamics-group-type3-state-1-reference-pka      = 2.0
-lambda-dynamics-group-type3-state-1-reference-pka      = 3.0
-...
+phbuilder genparams -f phneutral.pdb -ph 4.0 -titr
 ```
-in the corresponding folders.
-
 
-**NOTE** This behaviour will change in the next release of the code.
+This will set the pH value to the string "ph", as well as all pH-dependent terms for pKa values in multisite groups (e.g. $\lambda_1$ of histidine). Those pH-dependent strings will be read by `create_titration.py` and modified according to the pH value for a particular somulation. Note however that a pH value is still required to be passed as input to `phbuilder genparams`. Minimization and equilibration files will be generated for this provided pH.
 
 # Performing parameterizations
 
 As mentioned, out of the box phbuilder comes with the topology and parameterization parameters (`lambdagrouptypes.dat`) required for setting up CpHMD simulation with Asp, Glu, Arg, Lys, and His in CHARMM36m. Although we expect this to be sufficient for most purposes, we recognize that scenarios (titratable ligands, titratable lipids, different force fields, etc.) exist for which CpHMD could be beneficial, but for which no parameterization is currently available.
 
 The following section describes a procedure for *single-site* parameterizations of ligands. For convenience, we will use the word "ligand" to refer to any new lambdagrouptype. Here, we consider parameterizing arginine as an example. As in [our previous work](https://pubs.acs.org/doi/full/10.1021/acs.jctc.2c00517), for amino acid parameterization we use capped tripeptides. Note that performing parameterizations correctly is relatively complicated, and the reader is advised to check [Scalable Constant pH Molecular Dynamics in GROMACS](https://pubs.acs.org/doi/10.1021/acs.jctc.2c00516) for more information on parameterization in CpHMD as well as [phbuilder: A Tool for Efficiently Setting up Constant pH Molecular Dynamics Simulations in GROMACS](https://pubs.acs.org/doi/full/10.1021/acs.jcim.3c01313). Here, we will use a two-step procedure, introduced in the phbuilder paper.
 
@@ -563,15 +557,15 @@
 
 OPTIONS
 
 | Flag__       | Description    |
 |--------------|----------------|
 | `-f`         | [\<.pdb/.gro>] (required) <br /> Specify input structure file. | 
 | `-o`         | [\<.pdb/.gro>] (phprocessed.pdb) <br /> Specify output structure file. | 
-| `-ph`        | [\<float>] <br /> Specify intended simulation pH. Will be used together with the macroscopic pKas of the titratable sites to auto set the initial lambdas. |
+| `-ph`        | [\<float>] <br /> Specify intended simulation pH. Will be used together with the reference pKas of the titratable sites to auto set the initial lambdas. |
 | `-v`         | (no) <br /> Be more verbose. |
 
 # Synopsis `phbuilder neutralize`
 
 ```
 phbuilder neutralize [-h] -f FILE [-p TOPOL] [-o OUTPUT] [-solname SOLNAME] [-pname PNAME] [-nname NNAME] [-conc CONC] [-nbufs NBUFS] [-rmin RMIN] [-ignw] [-v]
 ```
@@ -600,15 +594,15 @@
 | `-rmin`      | [\<float>] (0.6) <br /> Set the minimum distance the ions and buffers should be placed from the solute.
 | `-ignw`      | (no) <br /> Ignore all gmx grompp warnings. |
 | `-v`         | (no) <br /> Be more verbose. |
 
 # Synopsis `phbuilder genparams`
 
 ```
-phbuilder genparams [-h] -f FILE -ph PH [-mdp MDP] [-ndx NDX] [-nstout NSTOUT] [-dwpE DWPE] [-inter] [-cal] [-v]
+phbuilder genparams [-h] -f FILE -ph PH [-mdp MDP] [-ndx NDX] [-nstout NSTOUT] [-dwpE DWPE] [-inter] [-titr] [-cal] [-v]
 ```
 
 ### DESCRIPTION
 
 Generates the CpHMD-specific `.mdp` and `.ndx` files. Will write generic EM.mdp EQ.mdp, and MD.mdp files for CHARMM36m and append the CpHMD parameters at the bottom. genparams requires the existence of a phrecord.dat file, which contains the initial lambda values and is created during the gentopol step. Note: if you previously used the auto feature (`-ph` flag) for gentopol, the pH you specify for genparams should reflect this.
 
 ### OPTIONS
@@ -618,14 +612,15 @@
 | `-f`         | [\<.pdb/.gro>] (required) <br /> Specify input structure file. |
 | `-ph`        | [\<float>] (required) <br /> Specify simulation pH. |
 | `-mdp`       | [\<.mdp>] (MD.mdp) <br /> Specify `.mdp` file for the constant-pH parameters to be appended to. If the specified file does not exist, the `.mdp` file will be generated from scratch. Note that this only applies to production (MD), for energy minimization (EM) and equilibration (NVT/NPT), the .mdp files will be generated from scratch regardless. |
 | `-ndx`       | [\<.idx>] (index.ndx) <br /> Specify `.ndx` file to append the CpHMD index groups to. If not set or the specified file does not exist, a generic `index.ndx` will be created first. |
 | `-nstout`    | [\<int>] (500) <br /> Specify lambda coordinate output frequency. 500 is large enough for subsequent frames to be uncoupled (with a $dt = 0.002$).
 | `-dwpE`      | [\<float>] (7.5) <br /> Specify default height of bias potential barrier (kJ/mol).
 | `-inter`     | (no) <br /> Interactively set the height of the bias potential barrier (kJ/mol) for every titratable site.
+| `-titr`       | (no) <br /> Prepare files for running titrations with CpHMD: forces pH to be set to "ph" and ph-dependent pKa values to be written to MD.mdp as string. The `create_titration.py` script will further modify those entries according to the currently set ph. |
 | `-cal`       | (no) <br /> Run CpHMD simulation in calibration mode: forces on the lambda coordinates are computed, but their positions won't be updated. This is only used for parameterization purposes. |
 | `-v`         | (no) <br /> Be more verbose. |
 
 # Tips, Tricks, and FAQ
 
 * One can use the experimental [EQ_smart.py](scripts/EQ_smart.py) to perform a more sound CpHMD equilibration. When using this script, the lambda coordinates from the last frame of an equilibration step are extracted from the `.edr` file and inserted in the `.mdp` file for the next equilibration step.
```

### Comparing `phbuilder-1.2.4/README.md` & `phbuilder-1.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -214,37 +214,29 @@
 
 ```
 gmx cphmd -s MD.tpr -e MD.edr -numplot 1
 ```
 
 # Performing titrations
 
-Performing a computational titration is helpful for determining the microscopic pKas of titratable sites. After steps 1 to 9 of the basic workflow have been completed, one can use the included [create_titration.py](scripts/create_titration.py) to setup a titration. For example, the command:
+Performing a computational titration is helpful for determining the pKa shifts of titratable sites. After steps 1 to 9 of the basic workflow have been completed, one can use the included [create_titration.py](scripts/create_titration.py) to setup a titration. For example, the command:
 
 ```
 create_titration.py -f MD.mdp -c NPT.pdb -p topol.top -n index.ndx -pH 1:10:1 -nr 2
 ```
 
 creates directories corresponding to pH 1 to 9, with each subdirectory containing two replicates (each containing the appropriate input files for `gmx mdrun`).
 
-**NOTE** `create_titration.py` currently requires small modifications of `MD.mdp` file. In case of multisite groups (e.g. histidine), one of the $\lambda$-coordinates (usually the first coordinate associated with the multisite group) should have pH value equal to $\text{p}K_\text{a}$ (check [manual](https://gitlab.com/gromacs-constantph/constantph/-/blob/main/manual/constantph_usage.md)). To achieve this, `create_titration.py` searches through the **.mdp** file, and if it sees pH and $\text{p}K_\text{a}$ in one line, it replaces pH with actual numeric value. This will ensure the correct set up at all pH values. To give an example:
-```
-lambda-dynamics-group-type3-state-1-reference-pka      = pH
-```
-this line will be sequentially changed to 
+The minor change is at step 7. When parameters are generated, `phbuilder genparams` needs to be called with the `-titr` option:
+
 ```
-lambda-dynamics-group-type3-state-1-reference-pka      = 1.0
-lambda-dynamics-group-type3-state-1-reference-pka      = 2.0
-lambda-dynamics-group-type3-state-1-reference-pka      = 3.0
-...
+phbuilder genparams -f phneutral.pdb -ph 4.0 -titr
 ```
-in the corresponding folders.
-
 
-**NOTE** This behaviour will change in the next release of the code.
+This will set the pH value to the string "ph", as well as all pH-dependent terms for pKa values in multisite groups (e.g. $\lambda_1$ of histidine). Those pH-dependent strings will be read by `create_titration.py` and modified according to the pH value for a particular somulation. Note however that a pH value is still required to be passed as input to `phbuilder genparams`. Minimization and equilibration files will be generated for this provided pH.
 
 # Performing parameterizations
 
 As mentioned, out of the box phbuilder comes with the topology and parameterization parameters (`lambdagrouptypes.dat`) required for setting up CpHMD simulation with Asp, Glu, Arg, Lys, and His in CHARMM36m. Although we expect this to be sufficient for most purposes, we recognize that scenarios (titratable ligands, titratable lipids, different force fields, etc.) exist for which CpHMD could be beneficial, but for which no parameterization is currently available.
 
 The following section describes a procedure for *single-site* parameterizations of ligands. For convenience, we will use the word "ligand" to refer to any new lambdagrouptype. Here, we consider parameterizing arginine as an example. As in [our previous work](https://pubs.acs.org/doi/full/10.1021/acs.jctc.2c00517), for amino acid parameterization we use capped tripeptides. Note that performing parameterizations correctly is relatively complicated, and the reader is advised to check [Scalable Constant pH Molecular Dynamics in GROMACS](https://pubs.acs.org/doi/10.1021/acs.jctc.2c00516) for more information on parameterization in CpHMD as well as [phbuilder: A Tool for Efficiently Setting up Constant pH Molecular Dynamics Simulations in GROMACS](https://pubs.acs.org/doi/full/10.1021/acs.jcim.3c01313). Here, we will use a two-step procedure, introduced in the phbuilder paper.
 
@@ -542,15 +534,15 @@
 
 OPTIONS
 
 | Flag__       | Description    |
 |--------------|----------------|
 | `-f`         | [\<.pdb/.gro>] (required) <br /> Specify input structure file. | 
 | `-o`         | [\<.pdb/.gro>] (phprocessed.pdb) <br /> Specify output structure file. | 
-| `-ph`        | [\<float>] <br /> Specify intended simulation pH. Will be used together with the macroscopic pKas of the titratable sites to auto set the initial lambdas. |
+| `-ph`        | [\<float>] <br /> Specify intended simulation pH. Will be used together with the reference pKas of the titratable sites to auto set the initial lambdas. |
 | `-v`         | (no) <br /> Be more verbose. |
 
 # Synopsis `phbuilder neutralize`
 
 ```
 phbuilder neutralize [-h] -f FILE [-p TOPOL] [-o OUTPUT] [-solname SOLNAME] [-pname PNAME] [-nname NNAME] [-conc CONC] [-nbufs NBUFS] [-rmin RMIN] [-ignw] [-v]
 ```
@@ -579,15 +571,15 @@
 | `-rmin`      | [\<float>] (0.6) <br /> Set the minimum distance the ions and buffers should be placed from the solute.
 | `-ignw`      | (no) <br /> Ignore all gmx grompp warnings. |
 | `-v`         | (no) <br /> Be more verbose. |
 
 # Synopsis `phbuilder genparams`
 
 ```
-phbuilder genparams [-h] -f FILE -ph PH [-mdp MDP] [-ndx NDX] [-nstout NSTOUT] [-dwpE DWPE] [-inter] [-cal] [-v]
+phbuilder genparams [-h] -f FILE -ph PH [-mdp MDP] [-ndx NDX] [-nstout NSTOUT] [-dwpE DWPE] [-inter] [-titr] [-cal] [-v]
 ```
 
 ### DESCRIPTION
 
 Generates the CpHMD-specific `.mdp` and `.ndx` files. Will write generic EM.mdp EQ.mdp, and MD.mdp files for CHARMM36m and append the CpHMD parameters at the bottom. genparams requires the existence of a phrecord.dat file, which contains the initial lambda values and is created during the gentopol step. Note: if you previously used the auto feature (`-ph` flag) for gentopol, the pH you specify for genparams should reflect this.
 
 ### OPTIONS
@@ -597,14 +589,15 @@
 | `-f`         | [\<.pdb/.gro>] (required) <br /> Specify input structure file. |
 | `-ph`        | [\<float>] (required) <br /> Specify simulation pH. |
 | `-mdp`       | [\<.mdp>] (MD.mdp) <br /> Specify `.mdp` file for the constant-pH parameters to be appended to. If the specified file does not exist, the `.mdp` file will be generated from scratch. Note that this only applies to production (MD), for energy minimization (EM) and equilibration (NVT/NPT), the .mdp files will be generated from scratch regardless. |
 | `-ndx`       | [\<.idx>] (index.ndx) <br /> Specify `.ndx` file to append the CpHMD index groups to. If not set or the specified file does not exist, a generic `index.ndx` will be created first. |
 | `-nstout`    | [\<int>] (500) <br /> Specify lambda coordinate output frequency. 500 is large enough for subsequent frames to be uncoupled (with a $dt = 0.002$).
 | `-dwpE`      | [\<float>] (7.5) <br /> Specify default height of bias potential barrier (kJ/mol).
 | `-inter`     | (no) <br /> Interactively set the height of the bias potential barrier (kJ/mol) for every titratable site.
+| `-titr`       | (no) <br /> Prepare files for running titrations with CpHMD: forces pH to be set to "ph" and ph-dependent pKa values to be written to MD.mdp as string. The `create_titration.py` script will further modify those entries according to the currently set ph. |
 | `-cal`       | (no) <br /> Run CpHMD simulation in calibration mode: forces on the lambda coordinates are computed, but their positions won't be updated. This is only used for parameterization purposes. |
 | `-v`         | (no) <br /> Be more verbose. |
 
 # Tips, Tricks, and FAQ
 
 * One can use the experimental [EQ_smart.py](scripts/EQ_smart.py) to perform a more sound CpHMD equilibration. When using this script, the lambda coordinates from the last frame of an equilibration step are extracted from the `.edr` file and inserted in the `.mdp` file for the next equilibration step.
```

### Comparing `phbuilder-1.2.4/phbuilder/ffield/README.md` & `phbuilder-1.2.5/phbuilder/ffield/README.md`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/atomtypes.atp` & `phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/cmap.itp` & `phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/cmap.itp`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/ffbonded.itp` & `phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/ffnonbonded.itp` & `phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/forcefield.doc` & `phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/forcefield.doc`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/forcefield.itp` & `phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/gb.itp` & `phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/gb.itp`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/ions.itp` & `phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.c.tdb` & `phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.c.tdb`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.hdb` & `phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.hdb`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.n.tdb` & `phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.n.tdb`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.rtp` & `phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.rtp`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.vsd` & `phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/merged.vsd`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/nbfix.itp` & `phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/nbfix.itp`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/old_c36_cmap.itp` & `phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/old_c36_cmap.itp`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/popc.itp` & `phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/popc.itp`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/tip3p.itp` & `phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/ffield/charmm36-mar2019-cphmd.ff/tip4p.itp` & `phbuilder-1.2.5/phbuilder/ffield/charmm36-mar2019-cphmd.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/ffield/lambdagrouptypes.dat` & `phbuilder-1.2.5/phbuilder/ffield/lambdagrouptypes.dat`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 qqB_1  = -0.28 0.62 -0.76 -0.76 0.00
 dvdl_1 = 59.636 -429.770 514.370 -204.910 -558.210 27.157
 
 [ HSPT ]
 incl   = HIS HIS1 HISA HISB HISH HISD HISE HISP HSD HSE HSP
 atoms  = CB CD2 HD2 CG NE2 HE2 ND1 HD1 CE1 HE1
 qqA    = 0.00 0.00 0.00 0.00 0.00 0.00 0.00 0.00 0.00 0.00
-pKa_1  = 0.0
+pKa_1  = ph
 qqB_1  = -0.05 0.19 0.13 0.19 -0.51 0.44 -0.51 0.44 0.32 0.18
 dvdl_1 = -3015.4 -13444.1 -34779. -44335.5 -31383.1 -13684.4 -4905.57 106.148 -484.107 11865.5 48985.4 104163. 103612. 59628.7 25794.9 3490.9 2180.34 -18552.6 -70083.6 -117174. -91492.5 -47959.2 -12542.4 -3968.74 14751.8 49997.8 63417.3 42048.3 16441.1 3929.98 -6193.44 -18113.5 -17591.7 -9832.74 -2246.33 934.809 2225.21 1887.54 594.263 402.485 604.077 158.757 -463.471 -193.458 82.6296
 pKa_2  = 6.53
 qqB_2  = -0.08 -0.05 0.09 0.22 -0.36 0.32 -0.7 0.0 0.25 0.13
 dvdl_2 = -1695.49 -8107.68 -22614.3 -40090.6 -39319.4 -21686.8 -5816.32 -1663.43 -1231.35 7080.8 30409.5 75205.7 105063. 78113.9 30391.7 8898.15 5178.6 -12000.8 -45996.4 -95996.2 -101472. -54848.1 -18185.2 -8896.93 10595.2 35922. 59318.7 45645. 18480.3 8030.77 -5015.37 -14771.9 -17941.8 -9642.21 -3996.01 894.376 2282.28 1905.97 857.662 264.085 372.239 128.992 -135.244 -299.418 -28.5093
 pKa_3 = 6.92
 qqB_3  = -0.09 0.22 0.1 -0.05 -0.7 0.0 -0.36 0.32 0.25 0.13
```

### Comparing `phbuilder-1.2.4/phbuilder/ffield/residuetypes.dat` & `phbuilder-1.2.5/phbuilder/ffield/residuetypes.dat`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/mdp.py` & `phbuilder-1.2.5/phbuilder/mdp.py`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/parsecmdline.py` & `phbuilder-1.2.5/phbuilder/parsecmdline.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         CLI: object containing all the parsed key-value pairs.
     """
 
     # phbuilder main description.
     desc_1 = "System builder for constant-pH simulations in GROMACS. phbuilder consists of three tools: gentopol, neutralize, and genparams. Each tool performs a specific task for preparing a constant-pH simulation. Functionality for setting up titrations and parameterizations is provided with the help of stand-alone Python scripts, provided on the gitlab. Out of the box, phbuilder comes with the force field and CpHMD topology parameters required for setting up titratable Arg, Lys, Asp, Glu, and His residues in CHARMM36m."
 
     # Epilogue. Also used by subcommands.
-    desc_2 = "phbuilder VERSION 1.2.4. For the user manual visit https://gitlab.com/gromacs-constantph/phbuilder."
+    desc_2 = "phbuilder VERSION 1.2.5. For the user manual visit https://gitlab.com/gromacs-constantph/phbuilder."
 
     # gentopol main description.
     desc_3 = "Allows you to select which residues to make titratable and which initial lambda (protonation) state they should have. Also (re)generates the system topology using the modified CHARMM36m force field. If you don't want to manually set initial lambda values, you can use the -ph flag to have gentopol automatically choose the appropriate initial lambda values, based on the criterion: pH > pKa means start deprotonated, else start protonated."
 
     # neutralize main description.
     desc_4 = "Adds the appropriate number of ions to ensure a net-neutral system at t=0, and adds buffer particles in order to maintain a net-neutral system at t>0. The system charge a t=0 depends on the chosen initial lambda (protonation) states. At t>0, protonation states can change dynamically, meaning the resulting charge difference needs to be 'absorbed' by buffer particles. Each buffer particle can absorb up to ±0.5 charge, and charge is distributed evenly across all buffers (-10 system charge and 100 BUF implies every BUF +0.1). The GROMACS CpHMD beta MUST be sourced/loaded for neutralize to work correctly."
 
@@ -47,15 +47,15 @@
                           default='phprocessed.pdb',
                           help='[<.pdb/.gro>] (phprocessed.pdb) Specify output structure file.')
 
     parser_1.add_argument('-ph',
                           required=False,
                           dest='ph',
                           action='store',
-                          help='[<float>] Specify intended simulation pH. Will be used together with the macroscopic pKas of the titratable sites to auto set the initial lambdas.',
+                          help='[<float>] Specify intended simulation pH. Will be used together with the reference pKas of the titratable sites to auto set the initial lambdas.',
                           type=float)
 
     parser_1.add_argument('-v',
                           required=False,
                           dest='verbosity',
                           action='store_const',
                           const=1,
@@ -193,14 +193,21 @@
     parser_3.add_argument('-inter',
                           required=False,
                           dest='inter',
                           action='store_const',
                           const=1,
                           help='(no) Interactively set the height of the bias potential barrier (kJ/mol) for every titratable site.')
 
+    parser_3.add_argument('-titr',
+                          required=False,
+                          dest='titr',
+                          action='store_const',
+                          const=1,
+                          help="(no) Prepare files for CpHMD titration. This will leave all pH-dependent pKa values as they are in lambdagrouptypes.dat. Those will be further modified by the create_titration.py script.")
+
     parser_3.add_argument('-cal',
                           required=False,
                           dest='cal',
                           action='store_const',
                           const=1,
                           help="(no) Run CpHMD simulation in calibration mode: forces on the lambda coordinates are computed, but their positions won't be updated. This is only used for parameterization purposes.")
```

### Comparing `phbuilder-1.2.4/phbuilder/phbuilder.py` & `phbuilder-1.2.5/phbuilder/phbuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import configparser
 import subprocess
 import os
 
+from sympy.parsing.sympy_parser import parse_expr
+from sympy import symbols
+
 from .user import User
 from .sanitize import Sanitize
 from .structure import Structure
 from .mdp import gen_mdp
 
 
 class LambdaType:
@@ -102,14 +105,20 @@
 
             # Process whether the -inter flag was or wasn't set.
             if CLI.inter is not None:
                 self.ph_inter = True
             else:
                 self.ph_inter = False
 
+            # Process whether the -titr flag was or wasn't set.
+            if CLI.titr is not None:
+                self.titr = True
+            else:
+                self.titr = False
+
             # Process whether the -cal flag was or wasn't set.
             if CLI.cal is not None:
                 self.ph_cal = True
             else:
                 self.ph_cal = False
 
         # User information.
@@ -219,18 +228,21 @@
 
             # Parse qqA
             qqA = str2floatList(parser.get(sect, 'qqA'))
 
             pKa  = []
             qqB  = []
             dvdl = []
-            for idx in range(1, 11):  # Max 10 multisites
+            # We iterate over the residue description as we don't know how many states we have.
+            # for loop over max 100 multistates. Do not use while True to prevent potential infinite loop.
+            for idx in range(1, 101):
                 try:
-                    # Parse pKa(s)
-                    pKa.append(float(parser.get(sect, 'pKA_{}'.format(idx))))
+                    # Parse pKa(s). Note: we are not converting pKa values here
+                    # as there might be a dependence on pH.
+                    pKa.append(parser.get(sect, 'pKA_{}'.format(idx)).lower())
 
                     # Parse qqB(s)
                     qqB.append(str2floatList(parser.get(sect, 'qqB_{}'.format(idx))))
 
                     # Parse dvdl(s)
                     dvdl.append(str2floatList(parser.get(sect, 'dvdl_{}'.format(idx))))
                 except configparser.NoOptionError:
@@ -238,15 +250,15 @@
 
             # SANITIZE INPUT
 
             groupname = Sanitize(groupname, "groupname in lambdagrouptypes.dat").string(Range=[2, 4], upper=True)
             incl      = [Sanitize(val, f"incl for {groupname} in lambdagrouptypes.dat").string(Range=[2, 4], upper=True) for val in incl]
             atoms     = [Sanitize(val, f"atoms for {groupname} in lambdagrouptypes.dat").string(Range=[1, 4], upper=True) for val in atoms]
             qqA       = [Sanitize(val, f"qqA for {groupname} in lambdagrouptypes.dat").num() for val in qqA]
-            pKa       = [Sanitize(val, f"pKa for {groupname} in lambdagrouptypes.dat").num(Range=[0, 14]) for val in pKa]
+            pKa       = [Sanitize(val, f"pKa for {groupname} in lambdagrouptypes.dat").pka_string(Range=[0, 14]) for val in pKa]
 
             for array in qqB:
                 for val in array:
                     Sanitize(val, f"qqB for {groupname} in lambdagrouptypes.dat").num()
 
             # Call function that constructs the LambdaType object.
             defineLambdaType(groupname, incl, pKa, atoms, qqA, qqB, dvdl)
@@ -1051,15 +1063,18 @@
             file.write("{:54s} = {:13s}\n".format(name, str(value)))
 
         # PART 1 - WRITE GENERAL PARAMETERS
 
         file.write("\n; CONSTANT PH\n")
 
         addParam('lambda-dynamics', 'yes')
-        addParam('lambda-dynamics-simulation-ph', self.ph_ph)
+        if Type == "MD" and self.titr:
+            addParam('lambda-dynamics-simulation-ph', 'ph')
+        else:
+            addParam('lambda-dynamics-simulation-ph', self.ph_ph)
         addParam('lambda-dynamics-lambda-particle-mass', "{:.1f}".format(5.0))  # lmass is hardcoded to 5.0 (amu).
         addParam('lambda-dynamics-tau', "{:.1f}".format(2.0))  # ltau is hardcoded to 2.0 (ps).
         addParam('lambda-dynamics-update-nst', self.ph_nstout)
 
         # If we use charge constraining...
         if constrainCharge:
             addParam('lambda-dynamics-charge-constraints', 'yes')
@@ -1119,18 +1134,22 @@
             addParam('lambda-dynamics-group-type{}-name'.format(number), name)
             addParam('lambda-dynamics-group-type{}-n-states'.format(number), multistates)
             addParam('lambda-dynamics-group-type{}-state-0-charges'.format(number), to_string(qqA))
 
             for idx in range(1, multistates + 1):
                 # When we have a multistate lambdagrouptype, one of the pKas should
                 # be equal to the simulation-pH. This is done by setting this pKa
-                # to zero in the lambdagrouptypes.dat file.
-                pKaNew = pKa[idx - 1]
-                if multistates > 1 and float(pKaNew) == 0.0:
-                    pKaNew = self.ph_ph
+                # to ph in the lambdagrouptypes.dat file.
+
+                if Type == "MD" and self.titr:
+                    pKaNew = pKa[idx - 1]
+                else:
+                    # Do some symbol maths
+                    ph = symbols("ph")
+                    pKaNew = float(parse_expr(pKa[idx - 1], evaluate=False).subs(ph, self.ph_ph))
 
                 addParam('lambda-dynamics-group-type{}-state-{}-charges'.format(number, idx), to_string(qqB[idx - 1]))
                 addParam('lambda-dynamics-group-type{}-state-{}-reference-pka'.format(number, idx), pKaNew)
                 addParam('lambda-dynamics-group-type{}-state-{}-dvdl-coefficients'.format(number, idx), to_string(dvdl[idx - 1]))
 
             file.write('\n')
 
@@ -1161,15 +1180,15 @@
 
             writeLambdaGroupTypeBlock(
                 number,
                 'BUF',
                 1,
                 [qqA],
                 [[qqB]],
-                [0],
+                ['0'],
                 [self.ph_BUF_dvdl]
             )
 
         # PART 3 - WRITE LAMBDA GROUPS
 
         def writeResBlock(number: int, name: str, initList: list, Edwp: float):
             """Writes the block for a specific residue."""
@@ -1255,17 +1274,27 @@
             if residue.d_resname in LambdaTypeNames:
                 LambdasFoundinProtein.append(residue.d_resname)
 
         file = open(fileName, 'a')
 
         def writeTheGroup(number, atomIndexList):
             """Formatting function for writing the index block."""
+
             file.write('\n[ LAMBDA{} ]\n'.format(number))
+
+            idxPerLine = 0
+
             for index in atomIndexList:
                 file.write('{} '.format(index))
+
+                idxPerLine += 1
+                if idxPerLine == 15:
+                    file.write('\n')
+                    idxPerLine = 0
+
             file.write('\n')
 
         atomCount   = 1
         groupNumber = 1
         bufferIndexList = []
 
         # Write the lambda index groups for the titratable residues.
@@ -1391,24 +1420,33 @@
 
         Returns:
             int: initial lambda value.
         """
         # multistate case
         if len(pKaList) > 1:
 
+            # Do some symbol maths
+            ph = symbols("ph")
+            pKa_vals = [
+                float(
+                    parse_expr(x, evaluate=False).subs(ph, systempH)
+                ) for x in pKaList
+            ]
+
             highest = 0
-            for pKa in pKaList:
+            for pKa in pKa_vals:
+
                 if pKa <= systempH and pKa > highest:
                     highest = pKa
 
-            return pKaList.index(highest) + 1
+            return pKa_vals.index(highest) + 1
 
         #2state case
         else:
-            if systempH >= pKaList[0]:
+            if systempH >= float(pKaList[0]):
                 return 1  # if pH >= pKa, we are in deproto = 1 state.
 
             return 0  # if pH < pKa, we are in the proto = 0 state.
 
     def pleaseCite(self):
         """Print citation request.
         """
```

### Comparing `phbuilder-1.2.4/phbuilder/sanitize.py` & `phbuilder-1.2.5/phbuilder/sanitize.py`

 * *Files 10% similar despite different names*

```diff
@@ -87,14 +87,48 @@
 
             # Check signed versus unsigned.
             if signed and self.var < 0:
                 self.__error('cannot be negative')
 
         return self.__endbehavior()
 
+    def pka_string(self, Range: list = []):
+        """Sanitize strings that describe pka values for lambda coordinate.
+        The rule is, if <ph> not in string, then we should be within range.
+
+        Args:
+            Type (Any, optional): (list of) acceptable type(s). Defaults to None.
+            Range (list, optional): acceptable interval. Defaults to [].
+            signed (bool, optional): Signed or unsigned. Defaults to False.
+
+        Returns:
+            int: exitcode.
+        """
+
+        # Confirm whether var is a string.
+        if not isinstance(self.var, str):
+            self.__error(f'should be of type {str}')
+
+        # Check if ph in var
+        if 'ph' in self.var:
+            # Do nothing
+            return self.__endbehavior()
+
+        # Try converting to string
+        try:
+            float(self.var)
+        except ValueError:
+            self.__error('should be convertible to float or have "ph"')
+
+        # Check range.
+        if Range and (float(self.var) < Range[0] or float(self.var) > Range[1]):
+            self.__error(f'outside of acceptable interval {Range}')
+
+        return self.__endbehavior()
+
     def string(self, Range: list = [], upper: bool = False, lower: bool = False, ws: bool = True):
         """sanitize strings (str).
 
         Args:
             Range (list, optional): acceptable string length. Defaults to [].
             upper (bool, optional): all uppercase. Defaults to False.
             lower (bool, optional): all lowercase. Defaults to False.
@@ -157,24 +191,27 @@
         # Check extension.
         if ext:
             tail = os.path.split(self.var)[1]
 
             if type(ext) != list:
                 ext = [ext]
 
-            if tail.count(' ') != 0:
-                self.__error('cannot contain whitespace')
-
-            if (tail.count('.') == 0) or (tail.count('.') > 1) or (tail[-1] == '.'):
-                self.__error(f'ambiguous extension (should be {ext})')
+            # Add "." to extensions if not present.
+            for idx in range(len(ext)):
+                if ext[idx][0] != ".":
+                    ext[idx] = "." + ext[idx]
+
+            # Comment this because file names can contain whitespace in linux.
+            # if tail.count(" ") != 0:
+            #     self.__error("cannot contain whitespace")
 
-            elif tail.index('.') == 0:
-                self.__error('cannot be just an extension')
+            if "." not in tail or (tail.index(".") == 0 and tail.count(".") == 1):
+                self.__error(f"does not have a file extension (should be {ext})")
 
-            elif tail[tail.index('.'):] not in ext:
-                self.__error(f'should have extension {ext}')
+            elif "." + tail.split(".")[-1] not in ext:
+                self.__error(f"should have extension {ext}")
 
         # Check absolute file path.
         if abs and not os.path.isabs(self.var):
             self.__error('should be an absolute file path')
 
         return self.__endbehavior()
```

### Comparing `phbuilder-1.2.4/phbuilder/structure.py` & `phbuilder-1.2.5/phbuilder/structure.py`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder/user.py` & `phbuilder-1.2.5/phbuilder/user.py`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/phbuilder.egg-info/PKG-INFO` & `phbuilder-1.2.5/phbuilder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phbuilder
-Version: 1.2.4
+Version: 1.2.5
 Summary: System builder for constant-pH simulations in GROMACS.
 Home-page: https://gitlab.com/gromacs-constantph/phbuilder
 Author: Anton Jansen
 Author-email: anton.jansen@scilifelab.se
 Project-URL: Bug Tracker, https://gitlab.com/gromacs-constantph/phbuilder/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -14,14 +14,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argcomplete>=3.1.1
 Requires-Dist: configparser>=6.0.0
+Requires-Dist: sympy>=1.12
+Requires-Dist: numpy
 
 <div style="width: 830px">
 
 [![GitLab issues](https://img.shields.io/badge/issue_tracking-gitlab-blue.svg)](https://gitlab.com/gromacs-constantph/phbuilder/-/issues)
 
 <p align="center">
   <img src="figures/logo.png" width="600"/>
@@ -235,37 +237,29 @@
 
 ```
 gmx cphmd -s MD.tpr -e MD.edr -numplot 1
 ```
 
 # Performing titrations
 
-Performing a computational titration is helpful for determining the microscopic pKas of titratable sites. After steps 1 to 9 of the basic workflow have been completed, one can use the included [create_titration.py](scripts/create_titration.py) to setup a titration. For example, the command:
+Performing a computational titration is helpful for determining the pKa shifts of titratable sites. After steps 1 to 9 of the basic workflow have been completed, one can use the included [create_titration.py](scripts/create_titration.py) to setup a titration. For example, the command:
 
 ```
 create_titration.py -f MD.mdp -c NPT.pdb -p topol.top -n index.ndx -pH 1:10:1 -nr 2
 ```
 
 creates directories corresponding to pH 1 to 9, with each subdirectory containing two replicates (each containing the appropriate input files for `gmx mdrun`).
 
-**NOTE** `create_titration.py` currently requires small modifications of `MD.mdp` file. In case of multisite groups (e.g. histidine), one of the $\lambda$-coordinates (usually the first coordinate associated with the multisite group) should have pH value equal to $\text{p}K_\text{a}$ (check [manual](https://gitlab.com/gromacs-constantph/constantph/-/blob/main/manual/constantph_usage.md)). To achieve this, `create_titration.py` searches through the **.mdp** file, and if it sees pH and $\text{p}K_\text{a}$ in one line, it replaces pH with actual numeric value. This will ensure the correct set up at all pH values. To give an example:
-```
-lambda-dynamics-group-type3-state-1-reference-pka      = pH
-```
-this line will be sequentially changed to 
+The minor change is at step 7. When parameters are generated, `phbuilder genparams` needs to be called with the `-titr` option:
+
 ```
-lambda-dynamics-group-type3-state-1-reference-pka      = 1.0
-lambda-dynamics-group-type3-state-1-reference-pka      = 2.0
-lambda-dynamics-group-type3-state-1-reference-pka      = 3.0
-...
+phbuilder genparams -f phneutral.pdb -ph 4.0 -titr
 ```
-in the corresponding folders.
-
 
-**NOTE** This behaviour will change in the next release of the code.
+This will set the pH value to the string "ph", as well as all pH-dependent terms for pKa values in multisite groups (e.g. $\lambda_1$ of histidine). Those pH-dependent strings will be read by `create_titration.py` and modified according to the pH value for a particular somulation. Note however that a pH value is still required to be passed as input to `phbuilder genparams`. Minimization and equilibration files will be generated for this provided pH.
 
 # Performing parameterizations
 
 As mentioned, out of the box phbuilder comes with the topology and parameterization parameters (`lambdagrouptypes.dat`) required for setting up CpHMD simulation with Asp, Glu, Arg, Lys, and His in CHARMM36m. Although we expect this to be sufficient for most purposes, we recognize that scenarios (titratable ligands, titratable lipids, different force fields, etc.) exist for which CpHMD could be beneficial, but for which no parameterization is currently available.
 
 The following section describes a procedure for *single-site* parameterizations of ligands. For convenience, we will use the word "ligand" to refer to any new lambdagrouptype. Here, we consider parameterizing arginine as an example. As in [our previous work](https://pubs.acs.org/doi/full/10.1021/acs.jctc.2c00517), for amino acid parameterization we use capped tripeptides. Note that performing parameterizations correctly is relatively complicated, and the reader is advised to check [Scalable Constant pH Molecular Dynamics in GROMACS](https://pubs.acs.org/doi/10.1021/acs.jctc.2c00516) for more information on parameterization in CpHMD as well as [phbuilder: A Tool for Efficiently Setting up Constant pH Molecular Dynamics Simulations in GROMACS](https://pubs.acs.org/doi/full/10.1021/acs.jcim.3c01313). Here, we will use a two-step procedure, introduced in the phbuilder paper.
 
@@ -563,15 +557,15 @@
 
 OPTIONS
 
 | Flag__       | Description    |
 |--------------|----------------|
 | `-f`         | [\<.pdb/.gro>] (required) <br /> Specify input structure file. | 
 | `-o`         | [\<.pdb/.gro>] (phprocessed.pdb) <br /> Specify output structure file. | 
-| `-ph`        | [\<float>] <br /> Specify intended simulation pH. Will be used together with the macroscopic pKas of the titratable sites to auto set the initial lambdas. |
+| `-ph`        | [\<float>] <br /> Specify intended simulation pH. Will be used together with the reference pKas of the titratable sites to auto set the initial lambdas. |
 | `-v`         | (no) <br /> Be more verbose. |
 
 # Synopsis `phbuilder neutralize`
 
 ```
 phbuilder neutralize [-h] -f FILE [-p TOPOL] [-o OUTPUT] [-solname SOLNAME] [-pname PNAME] [-nname NNAME] [-conc CONC] [-nbufs NBUFS] [-rmin RMIN] [-ignw] [-v]
 ```
@@ -600,15 +594,15 @@
 | `-rmin`      | [\<float>] (0.6) <br /> Set the minimum distance the ions and buffers should be placed from the solute.
 | `-ignw`      | (no) <br /> Ignore all gmx grompp warnings. |
 | `-v`         | (no) <br /> Be more verbose. |
 
 # Synopsis `phbuilder genparams`
 
 ```
-phbuilder genparams [-h] -f FILE -ph PH [-mdp MDP] [-ndx NDX] [-nstout NSTOUT] [-dwpE DWPE] [-inter] [-cal] [-v]
+phbuilder genparams [-h] -f FILE -ph PH [-mdp MDP] [-ndx NDX] [-nstout NSTOUT] [-dwpE DWPE] [-inter] [-titr] [-cal] [-v]
 ```
 
 ### DESCRIPTION
 
 Generates the CpHMD-specific `.mdp` and `.ndx` files. Will write generic EM.mdp EQ.mdp, and MD.mdp files for CHARMM36m and append the CpHMD parameters at the bottom. genparams requires the existence of a phrecord.dat file, which contains the initial lambda values and is created during the gentopol step. Note: if you previously used the auto feature (`-ph` flag) for gentopol, the pH you specify for genparams should reflect this.
 
 ### OPTIONS
@@ -618,14 +612,15 @@
 | `-f`         | [\<.pdb/.gro>] (required) <br /> Specify input structure file. |
 | `-ph`        | [\<float>] (required) <br /> Specify simulation pH. |
 | `-mdp`       | [\<.mdp>] (MD.mdp) <br /> Specify `.mdp` file for the constant-pH parameters to be appended to. If the specified file does not exist, the `.mdp` file will be generated from scratch. Note that this only applies to production (MD), for energy minimization (EM) and equilibration (NVT/NPT), the .mdp files will be generated from scratch regardless. |
 | `-ndx`       | [\<.idx>] (index.ndx) <br /> Specify `.ndx` file to append the CpHMD index groups to. If not set or the specified file does not exist, a generic `index.ndx` will be created first. |
 | `-nstout`    | [\<int>] (500) <br /> Specify lambda coordinate output frequency. 500 is large enough for subsequent frames to be uncoupled (with a $dt = 0.002$).
 | `-dwpE`      | [\<float>] (7.5) <br /> Specify default height of bias potential barrier (kJ/mol).
 | `-inter`     | (no) <br /> Interactively set the height of the bias potential barrier (kJ/mol) for every titratable site.
+| `-titr`       | (no) <br /> Prepare files for running titrations with CpHMD: forces pH to be set to "ph" and ph-dependent pKa values to be written to MD.mdp as string. The `create_titration.py` script will further modify those entries according to the currently set ph. |
 | `-cal`       | (no) <br /> Run CpHMD simulation in calibration mode: forces on the lambda coordinates are computed, but their positions won't be updated. This is only used for parameterization purposes. |
 | `-v`         | (no) <br /> Be more verbose. |
 
 # Tips, Tricks, and FAQ
 
 * One can use the experimental [EQ_smart.py](scripts/EQ_smart.py) to perform a more sound CpHMD equilibration. When using this script, the lambda coordinates from the last frame of an equilibration step are extracted from the `.edr` file and inserted in the `.mdp` file for the next equilibration step.
```

### Comparing `phbuilder-1.2.4/phbuilder.egg-info/SOURCES.txt` & `phbuilder-1.2.5/phbuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phbuilder-1.2.4/setup.cfg` & `phbuilder-1.2.5/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = phbuilder
-version = 1.2.4
+version = 1.2.5
 author = Anton Jansen
 author_email = anton.jansen@scilifelab.se
 description = System builder for constant-pH simulations in GROMACS.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/gromacs-constantph/phbuilder
 project_urls = 
@@ -23,14 +23,16 @@
 package_dir = 
 	= .
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	argcomplete>=3.1.1
 	configparser>=6.0.0
+	sympy>=1.12
+	numpy
 
 [options.package_data]
 phbuilder = ffield/*, ffield/charmm36-mar2019-cphmd.ff/*
 
 [options.entry_points]
 console_scripts = 
 	phbuilder = phbuilder:entryFunction
```

