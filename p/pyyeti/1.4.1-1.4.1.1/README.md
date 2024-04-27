# Comparing `tmp/pyyeti-1.4.1.tar.gz` & `tmp/pyyeti-1.4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyyeti-1.4.1.tar", last modified: Sat Mar 30 17:44:51 2024, max compression
+gzip compressed data, was "pyyeti-1.4.1.1.tar", last modified: Sat Apr 27 19:48:41 2024, max compression
```

## Comparing `pyyeti-1.4.1.tar` & `pyyeti-1.4.1.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-03-30 17:44:51.535298 pyyeti-1.4.1/
--rw-rw-r--   0 macro     (1000) macro     (1000)     1545 2024-03-30 16:48:11.000000 pyyeti-1.4.1/LICENSE.txt
--rw-rw-r--   0 macro     (1000) macro     (1000)      333 2024-01-24 22:45:59.000000 pyyeti-1.4.1/MANIFEST.in
--rw-r--r--   0 macro     (1000) macro     (1000)     4069 2024-03-30 17:44:51.535298 pyyeti-1.4.1/PKG-INFO
--rw-rw-r--   0 macro     (1000) macro     (1000)     3189 2024-03-30 16:48:01.000000 pyyeti-1.4.1/README.md
--rw-rw-r--   0 macro     (1000) macro     (1000)       89 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyproject.toml
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-03-30 17:44:51.527298 pyyeti-1.4.1/pyyeti/
--rw-rw-r--   0 macro     (1000) macro     (1000)     1035 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/__init__.py
--rw-rw-r--   0 macro     (1000) macro     (1000)   106855 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/cb.py
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-03-30 17:44:51.527298 pyyeti-1.4.1/pyyeti/cla/
--rw-rw-r--   0 macro     (1000) macro     (1000)      478 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/cla/__init__.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    15306 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/cla/_magpct.py
--rw-rw-r--   0 macro     (1000) macro     (1000)     4520 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/cla/_rptext1.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    36237 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/cla/_rptpct1.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    10341 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/cla/_rpttab1.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    21512 2024-03-30 16:35:32.000000 pyyeti-1.4.1/pyyeti/cla/_utilities.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    50944 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/cla/dr_def.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    27609 2024-01-28 18:47:10.000000 pyyeti-1.4.1/pyyeti/cla/dr_event.py
--rw-rw-r--   0 macro     (1000) macro     (1000)   111343 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/cla/dr_results.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    22910 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/cla/dr_results_plots.py
--rw-rw-r--   0 macro     (1000) macro     (1000)     7083 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/cla/rel_disp_dtm.py
--rw-rw-r--   0 macro     (1000) macro     (1000)     3912 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/column_plotter.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    24375 2024-03-30 16:14:58.000000 pyyeti-1.4.1/pyyeti/cyclecount.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    28432 2024-02-03 17:54:03.000000 pyyeti-1.4.1/pyyeti/datacursor.py
--rw-rw-r--   0 macro     (1000) macro     (1000)   127401 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/dsp.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    71114 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/era.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    42924 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/expmint.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    29847 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/fdepsd.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    48733 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/frclim.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    16400 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/guitools.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    16361 2024-01-28 18:47:10.000000 pyyeti-1.4.1/pyyeti/locate.py
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-03-30 17:44:51.527298 pyyeti-1.4.1/pyyeti/nastran/
--rw-rw-r--   0 macro     (1000) macro     (1000)      138 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/nastran/__init__.py
--rw-rw-r--   0 macro     (1000) macro     (1000)   189330 2024-03-30 16:12:46.000000 pyyeti-1.4.1/pyyeti/nastran/bulk.py
--rw-rw-r--   0 macro     (1000) macro     (1000)   136739 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/nastran/n2p.py
--rw-rw-r--   0 macro     (1000) macro     (1000)   177827 2024-02-25 16:48:06.000000 pyyeti-1.4.1/pyyeti/nastran/op2.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    91364 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/nastran/op4.py
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-03-30 17:44:51.531298 pyyeti-1.4.1/pyyeti/ode/
--rw-rw-r--   0 macro     (1000) macro     (1000)      869 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/ode/__init__.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    18978 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/ode/_base_ode_class.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    39142 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/ode/_utilities.py
--rw-rw-r--   0 macro     (1000) macro     (1000)     9992 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/ode/freqdirect.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    17472 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/ode/frf_mode_participation.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    10065 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/ode/solvecdf.py
--rw-rw-r--   0 macro     (1000) macro     (1000)     5653 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/ode/solveexp1.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    28080 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/ode/solveexp2.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    27510 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/ode/solvenewmark.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    71837 2024-02-25 16:48:06.000000 pyyeti-1.4.1/pyyeti/ode/solveunc.py
--rw-rw-r--   0 macro     (1000) macro     (1000)     9390 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/pp.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    43921 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/psd.py
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-03-30 17:44:51.531298 pyyeti-1.4.1/pyyeti/rainflow/
--rw-rw-r--   0 macro     (1000) macro     (1000)      195 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/rainflow/__init__.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    13898 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/rainflow/c_rain.c
--rw-rw-r--   0 macro     (1000) macro     (1000)     6540 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/rainflow/py_rain.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    75180 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/srs.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    11892 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/ssmodel.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    14070 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/stats.py
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-03-30 17:44:51.523298 pyyeti-1.4.1/pyyeti/tests/
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-03-30 17:44:51.531298 pyyeti-1.4.1/pyyeti/tests/nas2cam_csuper/
--rw-rw-r--   0 macro     (1000) macro     (1000)     1622 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_csuper/inboard.asm
--rw-rw-r--   0 macro     (1000) macro     (1000)    25840 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_csuper/inboard.op4
--rw-rw-r--   0 macro     (1000) macro     (1000)     4727 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_csuper/inboard.pch
--rw-rw-r--   0 macro     (1000) macro     (1000)    15736 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_csuper/nas2cam.op2
--rw-rw-r--   0 macro     (1000) macro     (1000)   147552 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_csuper/nas2cam.op4
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-03-30 17:44:51.531298 pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/
--rw-rw-r--   0 macro     (1000) macro     (1000)     2432 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/assemble.dat
--rw-rw-r--   0 macro     (1000) macro     (1000)   133180 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/assemble.op2
--rw-rw-r--   0 macro     (1000) macro     (1000)   162313 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/assemble.out
--rw-rw-r--   0 macro     (1000) macro     (1000)     1622 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/inboard.asm
--rw-rw-r--   0 macro     (1000) macro     (1000)     5827 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/inboard.blk
--rw-rw-r--   0 macro     (1000) macro     (1000)     6894 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/inboard.dat
--rw-rw-r--   0 macro     (1000) macro     (1000)    24052 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/inboard.op2
--rw-rw-r--   0 macro     (1000) macro     (1000)    36504 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/inboard.op4
--rw-rw-r--   0 macro     (1000) macro     (1000)   134889 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/inboard.out
--rw-rw-r--   0 macro     (1000) macro     (1000)     8939 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/inboard.pch
--rw-rw-r--   0 macro     (1000) macro     (1000)     2012 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/outboard.asm
--rw-rw-r--   0 macro     (1000) macro     (1000)     4946 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/outboard.blk
--rw-rw-r--   0 macro     (1000) macro     (1000)      767 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/outboard.dat
--rw-rw-r--   0 macro     (1000) macro     (1000)    38384 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/outboard.op4
--rw-rw-r--   0 macro     (1000) macro     (1000)    74780 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/outboard.out
--rw-rw-r--   0 macro     (1000) macro     (1000)     5944 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/outboard.pch
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-03-30 17:44:51.535298 pyyeti-1.4.1/pyyeti/tests/nastran_drm12/
--rw-rw-r--   0 macro     (1000) macro     (1000)    13464 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nastran_drm12/drm12.op2
--rw-rw-r--   0 macro     (1000) macro     (1000)    77852 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nastran_drm12/drm12.op4
--rw-rw-r--   0 macro     (1000) macro     (1000)    17160 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nastran_drm12/inboard_nas2cam.op2
--rw-rw-r--   0 macro     (1000) macro     (1000)    51624 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/tests/nastran_drm12/inboard_nas2cam.op4
--rw-rw-r--   0 macro     (1000) macro     (1000)    12371 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/writer.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    61169 2024-01-24 22:45:59.000000 pyyeti-1.4.1/pyyeti/ytools.py
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-03-30 17:44:51.527298 pyyeti-1.4.1/pyyeti.egg-info/
--rw-r--r--   0 macro     (1000) macro     (1000)     4069 2024-03-30 17:44:51.000000 pyyeti-1.4.1/pyyeti.egg-info/PKG-INFO
--rw-rw-r--   0 macro     (1000) macro     (1000)     2311 2024-03-30 17:44:51.000000 pyyeti-1.4.1/pyyeti.egg-info/SOURCES.txt
--rw-rw-r--   0 macro     (1000) macro     (1000)        1 2024-03-30 17:44:51.000000 pyyeti-1.4.1/pyyeti.egg-info/dependency_links.txt
--rw-rw-r--   0 macro     (1000) macro     (1000)        7 2024-03-30 17:44:51.000000 pyyeti-1.4.1/pyyeti.egg-info/top_level.txt
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-03-30 17:44:51.535298 pyyeti-1.4.1/scripts/
--rwxrwxr-x   0 macro     (1000) macro     (1000)      861 2024-02-25 16:48:06.000000 pyyeti-1.4.1/scripts/lsop2
--rwxrwxr-x   0 macro     (1000) macro     (1000)      561 2024-02-25 16:48:06.000000 pyyeti-1.4.1/scripts/lsop4
--rw-rw-r--   0 macro     (1000) macro     (1000)      198 2024-03-30 17:44:51.535298 pyyeti-1.4.1/setup.cfg
--rw-rw-r--   0 macro     (1000) macro     (1000)     5159 2024-03-30 17:27:02.000000 pyyeti-1.4.1/setup.py
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.229643 pyyeti-1.4.1.1/
+-rw-rw-r--   0 macro     (1000) macro     (1000)     1545 2024-03-30 16:48:11.000000 pyyeti-1.4.1.1/LICENSE.txt
+-rw-rw-r--   0 macro     (1000) macro     (1000)      333 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/MANIFEST.in
+-rw-r--r--   0 macro     (1000) macro     (1000)     4071 2024-04-27 19:48:41.229643 pyyeti-1.4.1.1/PKG-INFO
+-rw-rw-r--   0 macro     (1000) macro     (1000)     3189 2024-03-30 16:48:01.000000 pyyeti-1.4.1.1/README.md
+-rw-rw-r--   0 macro     (1000) macro     (1000)       89 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyproject.toml
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.209642 pyyeti-1.4.1.1/pyyeti/
+-rw-rw-r--   0 macro     (1000) macro     (1000)     1035 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/__init__.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)   106855 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/cb.py
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.213642 pyyeti-1.4.1.1/pyyeti/cla/
+-rw-rw-r--   0 macro     (1000) macro     (1000)      478 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/cla/__init__.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    15306 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/cla/_magpct.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)     4520 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/cla/_rptext1.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    36575 2024-04-27 19:48:26.000000 pyyeti-1.4.1.1/pyyeti/cla/_rptpct1.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    10341 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/cla/_rpttab1.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    21512 2024-03-30 16:35:32.000000 pyyeti-1.4.1.1/pyyeti/cla/_utilities.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    50944 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/cla/dr_def.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    27609 2024-01-28 18:47:10.000000 pyyeti-1.4.1.1/pyyeti/cla/dr_event.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)   111343 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/cla/dr_results.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    22910 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/cla/dr_results_plots.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)     7083 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/cla/rel_disp_dtm.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)     3912 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/column_plotter.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    24375 2024-03-30 16:14:58.000000 pyyeti-1.4.1.1/pyyeti/cyclecount.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    28432 2024-02-03 17:54:03.000000 pyyeti-1.4.1.1/pyyeti/datacursor.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)   127401 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/dsp.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    71114 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/era.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    42924 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/expmint.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    29847 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/fdepsd.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    48733 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/frclim.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    16400 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/guitools.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    16361 2024-01-28 18:47:10.000000 pyyeti-1.4.1.1/pyyeti/locate.py
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.217642 pyyeti-1.4.1.1/pyyeti/nastran/
+-rw-rw-r--   0 macro     (1000) macro     (1000)      138 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/nastran/__init__.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)   189330 2024-03-30 16:12:46.000000 pyyeti-1.4.1.1/pyyeti/nastran/bulk.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)   136739 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/nastran/n2p.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)   177827 2024-02-25 16:48:06.000000 pyyeti-1.4.1.1/pyyeti/nastran/op2.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    91364 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/nastran/op4.py
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.217642 pyyeti-1.4.1.1/pyyeti/ode/
+-rw-rw-r--   0 macro     (1000) macro     (1000)      869 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ode/__init__.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    18978 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ode/_base_ode_class.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    39142 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ode/_utilities.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)     9992 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ode/freqdirect.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    17472 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ode/frf_mode_participation.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    10065 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ode/solvecdf.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)     5653 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ode/solveexp1.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    28080 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ode/solveexp2.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    27510 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ode/solvenewmark.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    71837 2024-02-25 16:48:06.000000 pyyeti-1.4.1.1/pyyeti/ode/solveunc.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)     9390 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/pp.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    43921 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/psd.py
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.217642 pyyeti-1.4.1.1/pyyeti/rainflow/
+-rw-rw-r--   0 macro     (1000) macro     (1000)      195 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/rainflow/__init__.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    13898 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/rainflow/c_rain.c
+-rw-rw-r--   0 macro     (1000) macro     (1000)     6540 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/rainflow/py_rain.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    75180 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/srs.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    11892 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ssmodel.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    14070 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/stats.py
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.205642 pyyeti-1.4.1.1/pyyeti/tests/
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.221643 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/
+-rw-rw-r--   0 macro     (1000) macro     (1000)     1622 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/inboard.asm
+-rw-rw-r--   0 macro     (1000) macro     (1000)    25840 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/inboard.op4
+-rw-rw-r--   0 macro     (1000) macro     (1000)     4727 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/inboard.pch
+-rw-rw-r--   0 macro     (1000) macro     (1000)    15736 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/nas2cam.op2
+-rw-rw-r--   0 macro     (1000) macro     (1000)   147552 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/nas2cam.op4
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.225643 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/
+-rw-rw-r--   0 macro     (1000) macro     (1000)     2432 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/assemble.dat
+-rw-rw-r--   0 macro     (1000) macro     (1000)   133180 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/assemble.op2
+-rw-rw-r--   0 macro     (1000) macro     (1000)   162313 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/assemble.out
+-rw-rw-r--   0 macro     (1000) macro     (1000)     1622 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.asm
+-rw-rw-r--   0 macro     (1000) macro     (1000)     5827 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.blk
+-rw-rw-r--   0 macro     (1000) macro     (1000)     6894 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.dat
+-rw-rw-r--   0 macro     (1000) macro     (1000)    24052 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.op2
+-rw-rw-r--   0 macro     (1000) macro     (1000)    36504 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.op4
+-rw-rw-r--   0 macro     (1000) macro     (1000)   134889 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.out
+-rw-rw-r--   0 macro     (1000) macro     (1000)     8939 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.pch
+-rw-rw-r--   0 macro     (1000) macro     (1000)     2012 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.asm
+-rw-rw-r--   0 macro     (1000) macro     (1000)     4946 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.blk
+-rw-rw-r--   0 macro     (1000) macro     (1000)      767 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.dat
+-rw-rw-r--   0 macro     (1000) macro     (1000)    38384 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.op4
+-rw-rw-r--   0 macro     (1000) macro     (1000)    74780 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.out
+-rw-rw-r--   0 macro     (1000) macro     (1000)     5944 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.pch
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.225643 pyyeti-1.4.1.1/pyyeti/tests/nastran_drm12/
+-rw-rw-r--   0 macro     (1000) macro     (1000)    13464 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nastran_drm12/drm12.op2
+-rw-rw-r--   0 macro     (1000) macro     (1000)    77852 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nastran_drm12/drm12.op4
+-rw-rw-r--   0 macro     (1000) macro     (1000)    17160 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nastran_drm12/inboard_nas2cam.op2
+-rw-rw-r--   0 macro     (1000) macro     (1000)    51624 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nastran_drm12/inboard_nas2cam.op4
+-rw-rw-r--   0 macro     (1000) macro     (1000)    12371 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/writer.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    61169 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ytools.py
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.209642 pyyeti-1.4.1.1/pyyeti.egg-info/
+-rw-r--r--   0 macro     (1000) macro     (1000)     4071 2024-04-27 19:48:41.000000 pyyeti-1.4.1.1/pyyeti.egg-info/PKG-INFO
+-rw-rw-r--   0 macro     (1000) macro     (1000)     2311 2024-04-27 19:48:41.000000 pyyeti-1.4.1.1/pyyeti.egg-info/SOURCES.txt
+-rw-rw-r--   0 macro     (1000) macro     (1000)        1 2024-04-27 19:48:41.000000 pyyeti-1.4.1.1/pyyeti.egg-info/dependency_links.txt
+-rw-rw-r--   0 macro     (1000) macro     (1000)        7 2024-04-27 19:48:41.000000 pyyeti-1.4.1.1/pyyeti.egg-info/top_level.txt
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.225643 pyyeti-1.4.1.1/scripts/
+-rwxrwxr-x   0 macro     (1000) macro     (1000)      861 2024-02-25 16:48:06.000000 pyyeti-1.4.1.1/scripts/lsop2
+-rwxrwxr-x   0 macro     (1000) macro     (1000)      561 2024-02-25 16:48:06.000000 pyyeti-1.4.1.1/scripts/lsop4
+-rw-rw-r--   0 macro     (1000) macro     (1000)      198 2024-04-27 19:48:41.229643 pyyeti-1.4.1.1/setup.cfg
+-rw-rw-r--   0 macro     (1000) macro     (1000)     5161 2024-04-27 19:48:26.000000 pyyeti-1.4.1.1/setup.py
```

### Comparing `pyyeti-1.4.1/LICENSE.txt` & `pyyeti-1.4.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/PKG-INFO` & `pyyeti-1.4.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyeti
-Version: 1.4.1
+Version: 1.4.1.1
 Summary: Tools mostly related to structural dynamics
 Home-page: http://github.com/twmacro/pyyeti/
 Author: Tim Widrick
 Author-email: twmacro@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: pyyeti Version: 1.4.1 Summary: Tools mostly related
-to structural dynamics Home-page: http://github.com/twmacro/pyyeti/ Author: Tim
-Widrick Author-email: twmacro@gmail.com License: BSD Platform: any Classifier:
-Development Status :: 4 - Beta Classifier: Programming Language :: C
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: Implementation :: CPython Classifier: Natural Language :: English
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: BSD License Classifier: Operating System :: OS Independent
+Metadata-Version: 2.1 Name: pyyeti Version: 1.4.1.1 Summary: Tools mostly
+related to structural dynamics Home-page: http://github.com/twmacro/pyyeti/
+Author: Tim Widrick Author-email: twmacro@gmail.com License: BSD Platform: any
+Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
+C Classifier: Programming Language :: Python Classifier: Programming Language
+:: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
+Language :: Python :: Implementation :: CPython Classifier: Natural Language ::
+English Classifier: Intended Audience :: Science/Research Classifier: License
+:: OSI Approved :: BSD License Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering Description-Content-Type: text/
 markdown License-File: LICENSE.txt
  _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_:_ _B_S_D_ _3_-_C_l_a_u_s_e_]
                            _[_P_y_P_I_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
 # pyYeti pyYeti has tools mostly related to structural dynamics: * Solve matrix
 equations of motion in the time and frequency domains * Shock response spectrum
 (SRS) * Fatigue damage equivalent power spectral densities (PSD) * Hurty-Craig-
```

### Comparing `pyyeti-1.4.1/README.md` & `pyyeti-1.4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/__init__.py` & `pyyeti-1.4.1.1/pyyeti/__init__.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/cb.py` & `pyyeti-1.4.1.1/pyyeti/cb.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/cla/_magpct.py` & `pyyeti-1.4.1.1/pyyeti/cla/_magpct.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/cla/_rptext1.py` & `pyyeti-1.4.1.1/pyyeti/cla/_rptext1.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/cla/_rptpct1.py` & `pyyeti-1.4.1.1/pyyeti/cla/_rptpct1.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 Low level tool for writing percent difference reports. Typically, this
 is called via: :func:`cla.DR_Results.rptpct`.
 """
 from io import StringIO
 from types import SimpleNamespace
 import warnings
 import numpy as np
+
 import matplotlib.pyplot as plt
+from matplotlib.backends.backend_agg import FigureCanvasAgg
+from matplotlib.figure import Figure
+
 from pyyeti import ytools, locate, writer, guitools
 from ._utilities import _get_rpt_headers, _get_numform, _proc_filterval
 from ._magpct import magpct
 
 
 __all__ = ["rptpct1"]
 
@@ -288,32 +292,35 @@
 
 
 def _figure_on(name, doabsmax, show_figures):
     figsize = [8.5, 11.0]
     if doabsmax:
         figsize[1] /= 3.0
     if show_figures:
-        plt.figure(name, figsize=figsize)
-        plt.clf()
+        fig = plt.figure(name, figsize=figsize, clear=True)
     else:
-        plt.figure(figsize=figsize)
+        fig = Figure(figsize=figsize)
+        FigureCanvasAgg(fig)
+    return fig
 
 
 def _figure_off(show_figures):
-    if not show_figures:
-        plt.close()
+    pass
+    # if not show_figures:
+    #     plt.close()
 
 
-def _prep_subplot(pctinfo, sp):
+def _prep_subplot(pctinfo, fig, sp):
     if "mx" in pctinfo:
         # if not just doing absmax
         if sp > 311:
-            plt.subplot(sp, sharex=plt.gca())
-        else:
-            plt.subplot(sp)
+            prev_axes = fig.gca()
+            return fig.add_subplot(sp, sharex=prev_axes)
+        return fig.add_subplot(sp)
+    return fig.add_subplot()
 
 
 def _plot_magpct(
     pctinfo,
     names,
     desc,
     doabsmax,
@@ -325,42 +332,43 @@
     absmhdr,
     show_figures,
     tight_layout_args,
 ):
     ptitle = f"{desc} - {{}} Comparison vs Magnitude"
     xl = f"{names[1]} Magnitude"
     yl = f"% Diff of {names[0]} vs {names[1]}"
-    _figure_on("Magpct - " + desc, doabsmax, show_figures)
+    fig = _figure_on("Magpct - " + desc, doabsmax, show_figures)
     try:
         for lbl, hdr, sp, ismax in (
             ("mx", maxhdr, 311, True),
             ("mn", minhdr, 312, False),
             ("amx", absmhdr, 313, True),
         ):
-            _prep_subplot(pctinfo, sp)
+            axes = _prep_subplot(pctinfo, fig, sp)
             if lbl in pctinfo:
                 if use_range:
                     ref = pctinfo["amx"]["mag"][1]
                 else:
                     ref = None
                 magpct(
                     pctinfo[lbl]["mag"][0],
                     pctinfo[lbl]["mag"][1],
                     Ref=ref,
                     ismax=ismax,
                     filterval=pctinfo[lbl]["magfilt"],
+                    ax=axes,
                     **magpct_options,
                 )
-                plt.title(ptitle.format(hdr))
-                plt.xlabel(xl)
-                plt.ylabel(yl)
-            plt.grid(True)
-        plt.tight_layout(**tight_layout_args)
+                axes.set_title(ptitle.format(hdr))
+                axes.set_xlabel(xl)
+                axes.set_ylabel(yl)
+            axes.grid(True)
+        fig.tight_layout(**tight_layout_args)
         if isinstance(filename, str):
-            plt.savefig(filename + ".magpct.png")
+            fig.savefig(filename + ".magpct.png")
     finally:
         _figure_off(show_figures)
 
 
 def _plot_histogram(
     pctinfo,
     names,
@@ -373,44 +381,44 @@
     absmhdr,
     show_figures,
     tight_layout_args,
 ):
     ptitle = f"{desc} - {{}} Comparison Histogram"
     xl = f"% Diff of {names[0]} vs {names[1]}"
     yl = "Percent Occurrence (%)"
-    _figure_on("Histogram - " + desc, doabsmax, show_figures)
+    fig = _figure_on("Histogram - " + desc, doabsmax, show_figures)
     try:
         for lbl, hdr, sp in (
             ("mx", maxhdr, 311),
             ("mn", minhdr, 312),
             ("amx", absmhdr, 313),
         ):
-            _prep_subplot(pctinfo, sp)
+            axes = _prep_subplot(pctinfo, fig, sp)
             if lbl in pctinfo:
                 width = histogram_inc
                 x = pctinfo[lbl]["hsto"][:, 0]
                 y = pctinfo[lbl]["hsto"][:, 2]
                 colors = ["b"] * len(x)
                 ax = abs(x)
                 pv1 = ((ax > 5) & (ax <= 10)).nonzero()[0]
                 pv2 = (ax > 10).nonzero()[0]
                 for pv, c in ((pv1, "m"), (pv2, "r")):
                     for i in pv:
                         colors[i] = c
-                plt.bar(x, y, width=width, color=colors, align="center")
-                plt.title(ptitle.format(hdr))
-                plt.xlabel(xl)
-                plt.ylabel(yl)
-                x = abs(max(plt.xlim(), key=abs))
+                axes.bar(x, y, width=width, color=colors, align="center")
+                axes.set_title(ptitle.format(hdr))
+                axes.set_xlabel(xl)
+                axes.set_ylabel(yl)
+                x = abs(max(axes.get_xlim(), key=abs))
                 if x < 5:
-                    plt.xlim(-5, 5)
-            plt.grid(True)
-        plt.tight_layout(**tight_layout_args)
+                    axes.set_xlim(-5, 5)
+            axes.grid(True)
+        fig.tight_layout(**tight_layout_args)
         if isinstance(filename, str):
-            plt.savefig(filename + ".histogram.png")
+            fig.savefig(filename + ".histogram.png")
     finally:
         _figure_off(show_figures)
 
 
 def rptpct1(
     mxmn1,
     mxmn2,
```

### Comparing `pyyeti-1.4.1/pyyeti/cla/_rpttab1.py` & `pyyeti-1.4.1.1/pyyeti/cla/_rpttab1.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/cla/_utilities.py` & `pyyeti-1.4.1.1/pyyeti/cla/_utilities.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/cla/dr_def.py` & `pyyeti-1.4.1.1/pyyeti/cla/dr_def.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/cla/dr_event.py` & `pyyeti-1.4.1.1/pyyeti/cla/dr_event.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/cla/dr_results.py` & `pyyeti-1.4.1.1/pyyeti/cla/dr_results.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/cla/dr_results_plots.py` & `pyyeti-1.4.1.1/pyyeti/cla/dr_results_plots.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/cla/rel_disp_dtm.py` & `pyyeti-1.4.1.1/pyyeti/cla/rel_disp_dtm.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/column_plotter.py` & `pyyeti-1.4.1.1/pyyeti/column_plotter.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/cyclecount.py` & `pyyeti-1.4.1.1/pyyeti/cyclecount.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/datacursor.py` & `pyyeti-1.4.1.1/pyyeti/datacursor.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/dsp.py` & `pyyeti-1.4.1.1/pyyeti/dsp.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/era.py` & `pyyeti-1.4.1.1/pyyeti/era.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/expmint.py` & `pyyeti-1.4.1.1/pyyeti/expmint.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/fdepsd.py` & `pyyeti-1.4.1.1/pyyeti/fdepsd.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/frclim.py` & `pyyeti-1.4.1.1/pyyeti/frclim.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/guitools.py` & `pyyeti-1.4.1.1/pyyeti/guitools.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/locate.py` & `pyyeti-1.4.1.1/pyyeti/locate.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/nastran/bulk.py` & `pyyeti-1.4.1.1/pyyeti/nastran/bulk.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/nastran/n2p.py` & `pyyeti-1.4.1.1/pyyeti/nastran/n2p.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/nastran/op2.py` & `pyyeti-1.4.1.1/pyyeti/nastran/op2.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/nastran/op4.py` & `pyyeti-1.4.1.1/pyyeti/nastran/op4.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/ode/__init__.py` & `pyyeti-1.4.1.1/pyyeti/ode/__init__.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/ode/_base_ode_class.py` & `pyyeti-1.4.1.1/pyyeti/ode/_base_ode_class.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/ode/_utilities.py` & `pyyeti-1.4.1.1/pyyeti/ode/_utilities.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/ode/freqdirect.py` & `pyyeti-1.4.1.1/pyyeti/ode/freqdirect.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/ode/frf_mode_participation.py` & `pyyeti-1.4.1.1/pyyeti/ode/frf_mode_participation.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/ode/solvecdf.py` & `pyyeti-1.4.1.1/pyyeti/ode/solvecdf.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/ode/solveexp1.py` & `pyyeti-1.4.1.1/pyyeti/ode/solveexp1.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/ode/solveexp2.py` & `pyyeti-1.4.1.1/pyyeti/ode/solveexp2.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/ode/solvenewmark.py` & `pyyeti-1.4.1.1/pyyeti/ode/solvenewmark.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/ode/solveunc.py` & `pyyeti-1.4.1.1/pyyeti/ode/solveunc.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/pp.py` & `pyyeti-1.4.1.1/pyyeti/pp.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/psd.py` & `pyyeti-1.4.1.1/pyyeti/psd.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/rainflow/c_rain.c` & `pyyeti-1.4.1.1/pyyeti/rainflow/c_rain.c`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/rainflow/py_rain.py` & `pyyeti-1.4.1.1/pyyeti/rainflow/py_rain.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/srs.py` & `pyyeti-1.4.1.1/pyyeti/srs.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/ssmodel.py` & `pyyeti-1.4.1.1/pyyeti/ssmodel.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/stats.py` & `pyyeti-1.4.1.1/pyyeti/stats.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_csuper/inboard.asm` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/inboard.asm`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_csuper/inboard.op4` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/inboard.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_csuper/inboard.pch` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/inboard.pch`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_csuper/nas2cam.op2` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/nas2cam.op2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_csuper/nas2cam.op4` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/nas2cam.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/assemble.dat` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/assemble.dat`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/assemble.op2` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/assemble.op2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/assemble.out` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/assemble.out`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/inboard.asm` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.asm`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/inboard.blk` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.blk`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/inboard.dat` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.dat`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/inboard.op2` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.op2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/inboard.op4` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/inboard.out` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.out`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/inboard.pch` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.pch`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/outboard.asm` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.asm`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/outboard.blk` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.blk`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/outboard.dat` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.dat`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/outboard.op4` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/outboard.out` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.out`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nas2cam_extseout/outboard.pch` & `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.pch`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nastran_drm12/drm12.op2` & `pyyeti-1.4.1.1/pyyeti/tests/nastran_drm12/drm12.op2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nastran_drm12/drm12.op4` & `pyyeti-1.4.1.1/pyyeti/tests/nastran_drm12/drm12.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nastran_drm12/inboard_nas2cam.op2` & `pyyeti-1.4.1.1/pyyeti/tests/nastran_drm12/inboard_nas2cam.op2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/tests/nastran_drm12/inboard_nas2cam.op4` & `pyyeti-1.4.1.1/pyyeti/tests/nastran_drm12/inboard_nas2cam.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/writer.py` & `pyyeti-1.4.1.1/pyyeti/writer.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti/ytools.py` & `pyyeti-1.4.1.1/pyyeti/ytools.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/pyyeti.egg-info/PKG-INFO` & `pyyeti-1.4.1.1/pyyeti.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyeti
-Version: 1.4.1
+Version: 1.4.1.1
 Summary: Tools mostly related to structural dynamics
 Home-page: http://github.com/twmacro/pyyeti/
 Author: Tim Widrick
 Author-email: twmacro@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: pyyeti Version: 1.4.1 Summary: Tools mostly related
-to structural dynamics Home-page: http://github.com/twmacro/pyyeti/ Author: Tim
-Widrick Author-email: twmacro@gmail.com License: BSD Platform: any Classifier:
-Development Status :: 4 - Beta Classifier: Programming Language :: C
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: Implementation :: CPython Classifier: Natural Language :: English
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: BSD License Classifier: Operating System :: OS Independent
+Metadata-Version: 2.1 Name: pyyeti Version: 1.4.1.1 Summary: Tools mostly
+related to structural dynamics Home-page: http://github.com/twmacro/pyyeti/
+Author: Tim Widrick Author-email: twmacro@gmail.com License: BSD Platform: any
+Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
+C Classifier: Programming Language :: Python Classifier: Programming Language
+:: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
+Language :: Python :: Implementation :: CPython Classifier: Natural Language ::
+English Classifier: Intended Audience :: Science/Research Classifier: License
+:: OSI Approved :: BSD License Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering Description-Content-Type: text/
 markdown License-File: LICENSE.txt
  _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_:_ _B_S_D_ _3_-_C_l_a_u_s_e_]
                            _[_P_y_P_I_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
 # pyYeti pyYeti has tools mostly related to structural dynamics: * Solve matrix
 equations of motion in the time and frequency domains * Shock response spectrum
 (SRS) * Fatigue damage equivalent power spectral densities (PSD) * Hurty-Craig-
```

### Comparing `pyyeti-1.4.1/pyyeti.egg-info/SOURCES.txt` & `pyyeti-1.4.1.1/pyyeti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/scripts/lsop2` & `pyyeti-1.4.1.1/scripts/lsop2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/scripts/lsop4` & `pyyeti-1.4.1.1/scripts/lsop4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1/setup.py` & `pyyeti-1.4.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         )
     else:
         kw = {}
 
     install_requires = check_dependencies()
     setup(
         name="pyyeti",
-        version="1.4.1",
+        version="1.4.1.1",
         url="http://github.com/twmacro/pyyeti/",
         license="BSD",
         author="Tim Widrick",
         install_requires=install_requires,
         author_email="twmacro@gmail.com",
         description=("Tools mostly related to structural dynamics"),
         long_description=long_description,
```

