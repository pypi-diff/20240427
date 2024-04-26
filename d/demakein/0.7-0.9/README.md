# Comparing `tmp/demakein-0.7.tar.gz` & `tmp/demakein-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/demakein-0.7.tar", last modified: Tue Apr 23 08:59:54 2013, max compression
+gzip compressed data, was "dist/demakein-0.9.tar", last modified: Sat May 18 06:40:12 2013, max compression
```

## Comparing `demakein-0.7.tar` & `demakein-0.9.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxrwxr-x   0 pfh       (1000) pfh       (1000)        0 2013-04-23 08:59:54.000000 demakein-0.7/
--rw-rw-r--   0 pfh       (1000) pfh       (1000)      364 2013-04-23 08:36:38.000000 demakein-0.7/CHANGES
-drwxrwxr-x   0 pfh       (1000) pfh       (1000)        0 2013-04-23 08:59:54.000000 demakein-0.7/demakein.egg-info/
--rw-rw-r--   0 pfh       (1000) pfh       (1000)       44 2013-04-23 08:59:54.000000 demakein-0.7/demakein.egg-info/entry_points.txt
--rw-rw-r--   0 pfh       (1000) pfh       (1000)      380 2013-04-23 08:59:54.000000 demakein-0.7/demakein.egg-info/PKG-INFO
--rw-rw-r--   0 pfh       (1000) pfh       (1000)        1 2013-04-23 08:59:54.000000 demakein-0.7/demakein.egg-info/dependency_links.txt
--rw-rw-r--   0 pfh       (1000) pfh       (1000)        9 2013-04-23 08:59:54.000000 demakein-0.7/demakein.egg-info/top_level.txt
--rw-rw-r--   0 pfh       (1000) pfh       (1000)       11 2013-04-23 08:59:54.000000 demakein-0.7/demakein.egg-info/requires.txt
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     1658 2013-04-23 08:59:54.000000 demakein-0.7/demakein.egg-info/SOURCES.txt
--rw-rw-r--   0 pfh       (1000) pfh       (1000)      380 2013-04-23 08:59:54.000000 demakein-0.7/PKG-INFO
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     2460 2013-04-23 08:35:55.000000 demakein-0.7/README
-drwxrwxr-x   0 pfh       (1000) pfh       (1000)        0 2013-04-23 08:59:54.000000 demakein-0.7/doc/
--rw-rw-r--   0 pfh       (1000) pfh       (1000)    45298 2013-02-05 09:56:41.000000 demakein-0.7/doc/folk-flute-and-whistle-fingering.pdf
--rw-rw-r--   0 pfh       (1000) pfh       (1000)    14268 2012-11-18 01:45:29.000000 demakein-0.7/doc/folk-shawm-fingering.odt
--rw-rw-r--   0 pfh       (1000) pfh       (1000)    43046 2012-11-18 01:45:29.000000 demakein-0.7/doc/pflute-fingering.pdf
--rw-rw-r--   0 pfh       (1000) pfh       (1000)    14654 2012-11-18 01:45:29.000000 demakein-0.7/doc/shawm-fingering.odt
--rw-rw-r--   0 pfh       (1000) pfh       (1000)    21279 2013-02-05 09:56:41.000000 demakein-0.7/doc/folk-flute-and-whistle-fingering.odt
--rw-rw-r--   0 pfh       (1000) pfh       (1000)    19986 2012-11-18 01:45:29.000000 demakein-0.7/doc/pflute-fingering.odt
--rw-rw-r--   0 pfh       (1000) pfh       (1000)       66 2013-04-08 07:06:07.000000 demakein-0.7/MANIFEST.in
-drwxrwxr-x   0 pfh       (1000) pfh       (1000)        0 2013-04-23 08:59:54.000000 demakein-0.7/examples/
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     1404 2013-04-08 07:06:07.000000 demakein-0.7/examples/simple_shawm.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)      251 2013-02-05 09:56:41.000000 demakein-0.7/examples/mywhistle.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     1454 2013-04-08 07:06:07.000000 demakein-0.7/examples/drinking_straw.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)      929 2013-02-04 23:26:17.000000 demakein-0.7/setup.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)       59 2013-04-23 08:59:54.000000 demakein-0.7/setup.cfg
-drwxrwxr-x   0 pfh       (1000) pfh       (1000)        0 2013-04-23 08:59:54.000000 demakein-0.7/demakein/
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     1593 2013-04-23 08:59:51.000000 demakein-0.7/demakein/__init__.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     4401 2012-12-22 03:39:59.000000 demakein-0.7/demakein/all.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)    14647 2012-11-26 21:38:02.000000 demakein-0.7/demakein/geom.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     3207 2012-11-18 02:18:22.000000 demakein-0.7/demakein/make_mouthpiece.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)    13519 2013-02-04 23:26:17.000000 demakein-0.7/demakein/cpp.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)    14427 2013-04-23 08:48:33.000000 demakein-0.7/demakein/make.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     4019 2012-11-18 01:45:29.000000 demakein-0.7/demakein/sketch.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)    17831 2013-04-18 08:33:19.000000 demakein-0.7/demakein/shape.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     5277 2012-12-17 08:23:25.000000 demakein-0.7/demakein/optimize.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)    27615 2013-04-08 07:06:07.000000 demakein-0.7/demakein/design.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     3528 2012-11-18 01:45:29.000000 demakein-0.7/demakein/svg.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     6456 2013-04-13 05:57:49.000000 demakein-0.7/demakein/design_whistle.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     8831 2013-02-04 23:26:17.000000 demakein-0.7/demakein/make_flute.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)    14491 2013-04-08 07:06:07.000000 demakein-0.7/demakein/pack.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     8391 2013-02-04 23:26:17.000000 demakein-0.7/demakein/profile.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     1599 2013-04-19 22:53:11.000000 demakein-0.7/demakein/make_reed.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)    11223 2013-04-12 03:52:30.000000 demakein-0.7/demakein/make_whistle.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)    22389 2012-11-18 02:18:22.000000 demakein-0.7/demakein/cgal.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     8242 2012-12-16 01:47:06.000000 demakein-0.7/demakein/make_shawm.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)      783 2012-11-18 01:45:29.000000 demakein-0.7/demakein/make_cork.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     6545 2012-11-18 01:45:29.000000 demakein-0.7/demakein/design_flute.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     5760 2013-04-08 07:06:07.000000 demakein-0.7/demakein/design_shawm.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     7171 2013-04-23 08:33:32.000000 demakein-0.7/demakein/make_panpipe.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     2427 2012-11-18 02:18:22.000000 demakein-0.7/demakein/make_bauble.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)       66 2013-02-04 23:26:17.000000 demakein-0.7/demakein/__main__.py
-drwxrwxr-x   0 pfh       (1000) pfh       (1000)        0 2013-04-23 08:59:54.000000 demakein-0.7/demakein/raphs_curves/
--rw-rw-r--   0 pfh       (1000) pfh       (1000)       79 2012-11-18 01:45:29.000000 demakein-0.7/demakein/raphs_curves/__init__.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)    27850 2012-11-18 01:45:29.000000 demakein-0.7/demakein/raphs_curves/mecsolve.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     5265 2012-11-18 01:45:29.000000 demakein-0.7/demakein/raphs_curves/bezfigs.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     1664 2012-11-18 01:45:29.000000 demakein-0.7/demakein/raphs_curves/polymat-bad.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)    21245 2012-11-18 01:45:29.000000 demakein-0.7/demakein/raphs_curves/bigmat.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     5123 2012-11-18 01:45:29.000000 demakein-0.7/demakein/raphs_curves/numintsynth.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)      560 2012-11-18 01:45:29.000000 demakein-0.7/demakein/raphs_curves/offset.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)    14558 2012-11-18 01:45:29.000000 demakein-0.7/demakein/raphs_curves/tocubic.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)    12668 2012-11-18 01:45:29.000000 demakein-0.7/demakein/raphs_curves/polymat.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     1876 2012-11-18 01:45:29.000000 demakein-0.7/demakein/raphs_curves/clothoid.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     7031 2012-11-18 01:45:29.000000 demakein-0.7/demakein/raphs_curves/fromcubic.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     5928 2012-11-18 01:45:29.000000 demakein-0.7/demakein/raphs_curves/mvc.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     3140 2012-11-18 01:45:29.000000 demakein-0.7/demakein/raphs_curves/cornu.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     5614 2012-11-18 01:45:29.000000 demakein-0.7/demakein/raphs_curves/pcorn.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     4757 2012-11-18 01:45:29.000000 demakein-0.7/demakein/raphs_curves/plot_solve_clothoid.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)       64 2012-11-18 01:45:29.000000 demakein-0.7/demakein/raphs_curves/cloth_off.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     2061 2012-11-18 01:45:29.000000 demakein-0.7/demakein/raphs_curves/band.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)     4706 2012-11-18 01:45:29.000000 demakein-0.7/demakein/raphs_curves/poly3.py
--rw-rw-r--   0 pfh       (1000) pfh       (1000)      786 2012-11-18 01:45:29.000000 demakein-0.7/demakein/raphs_curves/euler-elastica.py
+drwxrwxr-x   0 pfh       (1000) pfh       (1000)        0 2013-05-18 06:40:12.000000 demakein-0.9/
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)      537 2013-05-18 06:39:27.000000 demakein-0.9/CHANGES
+drwxrwxr-x   0 pfh       (1000) pfh       (1000)        0 2013-05-18 06:40:12.000000 demakein-0.9/demakein.egg-info/
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)       44 2013-05-18 06:40:12.000000 demakein-0.9/demakein.egg-info/entry_points.txt
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)      380 2013-05-18 06:40:12.000000 demakein-0.9/demakein.egg-info/PKG-INFO
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)        1 2013-05-18 06:40:12.000000 demakein-0.9/demakein.egg-info/dependency_links.txt
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)        9 2013-05-18 06:40:12.000000 demakein-0.9/demakein.egg-info/top_level.txt
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)       11 2013-05-18 06:40:12.000000 demakein-0.9/demakein.egg-info/requires.txt
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     1675 2013-05-18 06:40:12.000000 demakein-0.9/demakein.egg-info/SOURCES.txt
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)      380 2013-05-18 06:40:12.000000 demakein-0.9/PKG-INFO
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     4829 2013-04-24 11:11:00.000000 demakein-0.9/README
+drwxrwxr-x   0 pfh       (1000) pfh       (1000)        0 2013-05-18 06:40:12.000000 demakein-0.9/doc/
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)    45298 2013-02-05 09:56:41.000000 demakein-0.9/doc/folk-flute-and-whistle-fingering.pdf
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)    14268 2012-11-18 01:45:29.000000 demakein-0.9/doc/folk-shawm-fingering.odt
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)    43046 2012-11-18 01:45:29.000000 demakein-0.9/doc/pflute-fingering.pdf
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)    14654 2012-11-18 01:45:29.000000 demakein-0.9/doc/shawm-fingering.odt
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)    21279 2013-02-05 09:56:41.000000 demakein-0.9/doc/folk-flute-and-whistle-fingering.odt
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)    19986 2012-11-18 01:45:29.000000 demakein-0.9/doc/pflute-fingering.odt
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)       66 2013-04-08 07:06:07.000000 demakein-0.9/MANIFEST.in
+drwxrwxr-x   0 pfh       (1000) pfh       (1000)        0 2013-05-18 06:40:12.000000 demakein-0.9/examples/
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     1404 2013-04-08 07:06:07.000000 demakein-0.9/examples/simple_shawm.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)      251 2013-02-05 09:56:41.000000 demakein-0.9/examples/mywhistle.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     1454 2013-04-08 07:06:07.000000 demakein-0.9/examples/drinking_straw.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)      929 2013-02-04 23:26:17.000000 demakein-0.9/setup.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)       59 2013-05-18 06:40:12.000000 demakein-0.9/setup.cfg
+drwxrwxr-x   0 pfh       (1000) pfh       (1000)        0 2013-05-18 06:40:12.000000 demakein-0.9/demakein/
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     1673 2013-05-18 06:39:35.000000 demakein-0.9/demakein/__init__.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     4401 2012-12-22 03:39:59.000000 demakein-0.9/demakein/all.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)    14647 2012-11-26 21:38:02.000000 demakein-0.9/demakein/geom.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     3207 2012-11-18 02:18:22.000000 demakein-0.9/demakein/make_mouthpiece.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)    13519 2013-02-04 23:26:17.000000 demakein-0.9/demakein/cpp.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)    15179 2013-05-17 09:11:03.000000 demakein-0.9/demakein/make.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     4019 2012-11-18 01:45:29.000000 demakein-0.9/demakein/sketch.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)    17956 2013-04-25 04:44:06.000000 demakein-0.9/demakein/shape.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     5279 2013-05-11 07:25:42.000000 demakein-0.9/demakein/optimize.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)    27658 2013-05-14 12:58:31.000000 demakein-0.9/demakein/design.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     3528 2012-11-18 01:45:29.000000 demakein-0.9/demakein/svg.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     8201 2013-05-17 07:10:10.000000 demakein-0.9/demakein/design_whistle.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     8831 2013-02-04 23:26:17.000000 demakein-0.9/demakein/make_flute.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)    14491 2013-04-08 07:06:07.000000 demakein-0.9/demakein/pack.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     8391 2013-02-04 23:26:17.000000 demakein-0.9/demakein/profile.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     3281 2013-05-15 00:30:41.000000 demakein-0.9/demakein/tune.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     1599 2013-04-19 22:53:11.000000 demakein-0.9/demakein/make_reed.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)    11466 2013-05-16 00:46:34.000000 demakein-0.9/demakein/make_whistle.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)    22389 2012-11-18 02:18:22.000000 demakein-0.9/demakein/cgal.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     8242 2012-12-16 01:47:06.000000 demakein-0.9/demakein/make_shawm.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)      783 2012-11-18 01:45:29.000000 demakein-0.9/demakein/make_cork.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     6545 2012-11-18 01:45:29.000000 demakein-0.9/demakein/design_flute.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     5760 2013-04-08 07:06:07.000000 demakein-0.9/demakein/design_shawm.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     7171 2013-04-23 08:33:32.000000 demakein-0.9/demakein/make_panpipe.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     2427 2012-11-18 02:18:22.000000 demakein-0.9/demakein/make_bauble.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)       66 2013-02-04 23:26:17.000000 demakein-0.9/demakein/__main__.py
+drwxrwxr-x   0 pfh       (1000) pfh       (1000)        0 2013-05-18 06:40:12.000000 demakein-0.9/demakein/raphs_curves/
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)       79 2012-11-18 01:45:29.000000 demakein-0.9/demakein/raphs_curves/__init__.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)    27850 2012-11-18 01:45:29.000000 demakein-0.9/demakein/raphs_curves/mecsolve.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     5265 2012-11-18 01:45:29.000000 demakein-0.9/demakein/raphs_curves/bezfigs.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     1664 2012-11-18 01:45:29.000000 demakein-0.9/demakein/raphs_curves/polymat-bad.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)    21245 2012-11-18 01:45:29.000000 demakein-0.9/demakein/raphs_curves/bigmat.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     5123 2012-11-18 01:45:29.000000 demakein-0.9/demakein/raphs_curves/numintsynth.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)      560 2012-11-18 01:45:29.000000 demakein-0.9/demakein/raphs_curves/offset.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)    14558 2012-11-18 01:45:29.000000 demakein-0.9/demakein/raphs_curves/tocubic.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)    12668 2012-11-18 01:45:29.000000 demakein-0.9/demakein/raphs_curves/polymat.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     1876 2012-11-18 01:45:29.000000 demakein-0.9/demakein/raphs_curves/clothoid.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     7031 2012-11-18 01:45:29.000000 demakein-0.9/demakein/raphs_curves/fromcubic.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     5928 2012-11-18 01:45:29.000000 demakein-0.9/demakein/raphs_curves/mvc.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     3140 2012-11-18 01:45:29.000000 demakein-0.9/demakein/raphs_curves/cornu.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     5614 2012-11-18 01:45:29.000000 demakein-0.9/demakein/raphs_curves/pcorn.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     4757 2012-11-18 01:45:29.000000 demakein-0.9/demakein/raphs_curves/plot_solve_clothoid.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)       64 2012-11-18 01:45:29.000000 demakein-0.9/demakein/raphs_curves/cloth_off.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     2061 2012-11-18 01:45:29.000000 demakein-0.9/demakein/raphs_curves/band.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)     4706 2012-11-18 01:45:29.000000 demakein-0.9/demakein/raphs_curves/poly3.py
+-rw-rw-r--   0 pfh       (1000) pfh       (1000)      786 2012-11-18 01:45:29.000000 demakein-0.9/demakein/raphs_curves/euler-elastica.py
```

### Comparing `demakein-0.7/demakein.egg-info/SOURCES.txt` & `demakein-0.9/demakein.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 demakein/make_whistle.py
 demakein/optimize.py
 demakein/pack.py
 demakein/profile.py
 demakein/shape.py
 demakein/sketch.py
 demakein/svg.py
+demakein/tune.py
 demakein.egg-info/PKG-INFO
 demakein.egg-info/SOURCES.txt
 demakein.egg-info/dependency_links.txt
 demakein.egg-info/entry_points.txt
 demakein.egg-info/requires.txt
 demakein.egg-info/top_level.txt
 demakein/raphs_curves/__init__.py
```

### Comparing `demakein-0.7/doc/folk-flute-and-whistle-fingering.pdf` & `demakein-0.9/doc/folk-flute-and-whistle-fingering.pdf`

 * *Files identical despite different names*

### Comparing `demakein-0.7/doc/folk-shawm-fingering.odt` & `demakein-0.9/doc/folk-shawm-fingering.odt`

 * *Files identical despite different names*

### Comparing `demakein-0.7/doc/pflute-fingering.pdf` & `demakein-0.9/doc/pflute-fingering.pdf`

 * *Files identical despite different names*

### Comparing `demakein-0.7/doc/shawm-fingering.odt` & `demakein-0.9/doc/shawm-fingering.odt`

 * *Files identical despite different names*

### Comparing `demakein-0.7/doc/folk-flute-and-whistle-fingering.odt` & `demakein-0.9/doc/folk-flute-and-whistle-fingering.odt`

 * *Files identical despite different names*

### Comparing `demakein-0.7/doc/pflute-fingering.odt` & `demakein-0.9/doc/pflute-fingering.odt`

 * *Files identical despite different names*

### Comparing `demakein-0.7/examples/simple_shawm.py` & `demakein-0.9/examples/simple_shawm.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/examples/drinking_straw.py` & `demakein-0.9/examples/drinking_straw.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/setup.py` & `demakein-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/__init__.py` & `demakein-0.9/demakein/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = '0.7'
+VERSION = '0.9'
 
 from .design_flute import Design_tapered_pflute, Design_straight_pflute, Design_tapered_folk_flute, Design_straight_folk_flute
 from .make_flute import Make_flute
 from .make_cork import Make_cork
 
 from .design_shawm import Design_shawm, Design_folk_shawm
 from .make_shawm import Make_shawm
@@ -12,14 +12,16 @@
 from .design_whistle import Design_folk_whistle, Design_recorder, Design_three_hole_whistle
 from .make_whistle import Make_whistle
 
 from .make_panpipe import Make_panpipe
 
 from .make_reed import Make_reed
 
+from .tune import Tune
+
 from .all import All
 
 def main():
     """ Command line interface. """
     import nesoni    
     nesoni.run_toolbox([
             'Demakein '+VERSION,
@@ -44,14 +46,17 @@
             Make_mouthpiece,
             Make_bauble,
             #Make_reed,
             
             'Panpipes',        
             Make_panpipe,
             
+            'Utilities',
+            Tune,
+            
             #'Everything',        
             #All,
             #'"demakein all:" uses the nesoni make system, see flags below.',
         ],
         show_make_flags=False,
         )
```

### Comparing `demakein-0.7/demakein/all.py` & `demakein-0.9/demakein/all.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/geom.py` & `demakein-0.9/demakein/geom.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/make_mouthpiece.py` & `demakein-0.9/demakein/make_mouthpiece.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/cpp.py` & `demakein-0.9/demakein/cpp.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/make.py` & `demakein-0.9/demakein/make.py`

 * *Files 7% similar despite different names*

```diff
@@ -253,16 +253,19 @@
             assert False, 'Unknown join type: '+self.join
         
         shapes = [ ]
         for cut in cuts:
             d1 = inner(cut)
             d4 = outer(cut)
             d5 = outer.maximum() * 2.0
-            p1 = cut-d4*0.4
-            p3 = cut+d4*0.4
+            #p1 = cut-d4*0.4
+            #p3 = cut+d4*0.4
+            
+            p1 = cut-d4*0.8
+            p3 = cut
             
             if self.thick_sockets:
                 d4_orig = d4
                 d4 += min(d4*0.2, (d4-d1)*0.5)
                 prof_thicker = profile.Profile(
                     [ p1-(d4-d4_orig), p1, p3 ],
                     [ (d1+d4)*0.5, d4, d4 ],
@@ -291,19 +294,21 @@
         shapes = shapes[::-1]
         
         for i, item in enumerate(shapes):
             item.rotate(0,1,0, 180)
             item.position_nicely()
             self.save(item, '%d-piece-%d' % (len(shapes),i+1))
         
-        size = outer.maximum() * 4.0
-        template = pack.Pack(size,size,5000.0)
-        packables = [ [pack.Packable([item], 0.0, 1.0)] for item in shapes ]
-        [ packed ] = pack.pack(template, packables)
-        self.save(packed.render_print(), '%d-piece-all' % len(shapes))
+        #size = outer.maximum() * 4.0
+        #template = pack.Pack(size,size,5000.0)
+        #packables = [ [pack.Packable([item], 0.0, 1.0)] for item in shapes ]
+        #[ packed ] = pack.pack(template, packables)
+        #render = packed.render_print()
+        #render.position_nicely()
+        #self.save(render, '%d-piece-all' % len(shapes))
         
         #self.working.segments = shapes
 
     def _straight_socket(
                 self,
                 p1,
                 p3,
@@ -374,33 +379,46 @@
             return mask_inside, mask_outside
 
     def _weld_join(self,z0,z1,zmax,d0,d1,dmax):
         prof = profile.Profile(
             [ z1, zmax+50 ],
             [ dmax, dmax]
             )
-        mask = shape.extrude_profile(prof)
+        mask_upper = shape.extrude_profile(prof)
+        mask_lower = mask_upper.copy()
         
         triangle = shape.Loop([
             (0.5, 0.0),
-            (-0.5, 0.0),
             (0.0, math.sqrt(0.75)),
-            ]).scale(d0*0.5)
-        dstart = (d0+d1)*0.5
+            (-0.5, 0.0),
+            ])
+        triangle_upper = triangle.scale(d0*0.5+self.gap)
+        triangle_lower  = triangle.scale(d0*0.5-self.gap)
+        d1_3 = d0*0.6666+d1*0.3334
+        d2_3 = d0*0.3334+d1*0.6666
         for i in xrange(1,5):
             bump = shape.extrusion(
-                [ dstart*0.5, dmax*0.5 ],
-                [ triangle, triangle ]
+                [ d1_3*0.5-self.gap*0.5, d2_3*0.5-self.gap*0.5, dmax*0.5 ],
+                [ triangle_upper.scale(0.0), triangle_upper, triangle_upper ]
+                )
+            bump.rotate(1,0,0,-90)
+            bump.rotate(0,0,1,180+360.0/5*i)
+            bump.move(0,0,z1)
+            mask_upper.add(bump)
+
+            bump = shape.extrusion(
+                [ d1_3*0.5+self.gap*0.5, d2_3*0.5+self.gap*0.5, dmax*0.5 ],
+                [ triangle_lower.scale(0.0), triangle_lower, triangle_lower ]
                 )
             bump.rotate(1,0,0,-90)
             bump.rotate(0,0,1,180+360.0/5*i)
             bump.move(0,0,z1)
-            mask.add(bump)
+            mask_lower.add(bump)
         
-        return mask, mask      
+        return mask_lower, mask_upper
         
 @config.Bool_flag('mill', 'Create shapes for milling (rather than 3D printing).')
 @config.Float_flag('mill_diameter', 'Milling: Bit diameter for milling (affects gap size when packing pieces).')
 @config.Float_flag('mill_length', 'Milling: Wood length for milling.')
 @config.Float_flag('mill_width', 'Milling: Wood width for milling.')
 @config.Float_flag('mill_thickness', 'Milling: Wood thickness for milling.')
 class Make_millable_instrument(Make_instrument):
```

### Comparing `demakein-0.7/demakein/sketch.py` & `demakein-0.9/demakein/sketch.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/shape.py` & `demakein-0.9/demakein/shape.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,22 @@
     area = math.pi + xpad*ypad + xpad*2 + ypad*2
     want = math.pi * (diameter*0.5)**2
     scale = math.sqrt( want/area )
     result = [ (x*scale,y*scale) for x,y in result ]
     
     return Loop(result)
 
+def rectangle(x0,x1,y0,y1):
+    return Loop([
+        (x0,y0),
+        (x1,y0),
+        (x1,y1),
+        (x0,y1)
+        ])
+
 def rounded_rectangle(x0,x1,y0,y1, diameter):    
     radius = min(diameter,x1-x0,y1-y0)*0.5 
     result = [ ]
     for i in range(QUALITY):
         a = (i+0.5)*math.pi*2.0/QUALITY
         x = math.cos(a)*radius
         if x < 0: x += x0+radius
```

### Comparing `demakein-0.7/demakein/optimize.py` & `demakein-0.9/demakein/optimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             val+random.normalvariate(0.0, extra) 
             for val in update 
             ]
     
     return update
 
 
-def improve(comment, constrainer, scorer, start_x, ftol=1e-4, initial_accuracy=0.001, monitor = lambda x: None):
+def improve(comment, constrainer, scorer, start_x, ftol=1e-4, initial_accuracy=0.001, monitor = lambda x,y: None):
     pool_size = legion.coordinator().get_cores()
     
     worker_futs = [ legion.coordinator().new_future() for i in xrange(pool_size) ]
     reply_futs = [ ]
     
     workers = [
         legion.future(worker,scorer,fut)
```

### Comparing `demakein-0.7/demakein/design.py` & `demakein-0.9/demakein/design.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,22 +129,24 @@
 def hole_length_correction(hole_diameter, bore_diameter, closed):
     # No inner correction even, for closed holes.
     # Not sure why, but including an inner correction
     # for closed holes is wrong (I've tried this).
     
     # Maybe better to treat as bore deviation?
     
-    if closed: return 0.0
+    if closed: 
+       return 0.0
     
     # As per p.63-64 of Nederveen
     outer_correction = 0.7
     inner_correction = 1.3 - 0.9 * hole_diameter/bore_diameter
     a = hole_diameter / 2.0
     
     result = a * (inner_correction+outer_correction)
+
     return result
 
 
 
 # ================ Instruments and classes of instruments =================
 
 class Instrument:
@@ -326,15 +328,14 @@
 def sqrt_scaler(value):
     @property
     def func(self):
         scale = math.sqrt(self.scale)
         return [ item*scale if item is not None else None for item in value ]
     return func
 
-
 @config.Int_flag('transpose', 'Transpose instrument by this many semitones.')
 class Instrument_designer(config.Action_with_output_dir):
     instrument_class = Instrument
 
     cone_step = 0.125  #diameter step size when approximating cones
 
     closed_top = False
@@ -636,14 +637,15 @@
         for pos in instrument.outer_kinks:
             diagram.line([(tick_x-10,-pos),(tick_x-15,-pos)], color)
         for pos in instrument.outer.pos[1:-1]:
             diagram.line([(tick_x-12,-pos),(tick_x-13,-pos)], color)
 
     
     def _save(self, state_vec, other_vecs=[]):
+        self.state_vec = state_vec
         self.instrument = self.unpack( state_vec )
         
         with open(os.path.join(self.output_dir, 'data.pickle'), 'wb') as f:
             if sys.version_info.major == 3:
                 pickle.dump(self, f, fix_imports=True)
             else:
                 pickle.dump(self, f)
```

### Comparing `demakein-0.7/demakein/svg.py` & `demakein-0.9/demakein/svg.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/design_whistle.py` & `demakein-0.9/demakein/design_whistle.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 import math, copy
 
 from nesoni import config
 
 from . import design, profile
 
 @config.Float_flag('tweak_gapextra')
+#@config.Float_flag('tweak_bulgediameter')
+#@config.Float_flag('tweak_bulgepos1')
+#@config.Float_flag('tweak_bulgepos2')
+@config.Float_flag('tweak_boreless')
 class Design_whistle(design.Instrument_designer):
     def get_whistle_maker(self):
         from . import make_whistle
         bore = self.inner_diameters[-1]
         outside = self.outer_diameters[-1]
         if self.outer_add: outside += bore
         return make_whistle.Make_whistle_head(
@@ -20,30 +24,50 @@
     closed_top = False
     
     divisions = [ ]
 
     # For gap_width 0.5, gap_length 0.25, from soprano
     # tweak_gapextra = 0.37
     
-    # For gap_width 0.666, gap_length 0.4, from soprano
-    tweak_gapextra = 0.01
+    # From soprano recorder
+    tweak_gapextra = 0.75 #0.71
+    #tweak_bulgediameter = 1.0
+    #tweak_bulgepos1 = 0.5
+    #tweak_bulgepos2 = 0.9
+    tweak_boreless = 0.65 #0.49
     
     def patch_instrument(self, inst):
         inst = copy.copy(inst)
         inst.true_length = inst.length
         inst.true_inner = inst.inner
         
+        bore_diameter = inst.inner(inst.length)
+        inst.length -= bore_diameter * self.tweak_boreless
+        inst.inner = inst.inner.clipped(0.0,inst.length)
+
+        #bulge_pos1 = self.tweak_bulgepos1 * inst.length
+        #bulge_pos2 = self.tweak_bulgepos2 * inst.length
+        #if bulge_pos1 > bulge_pos2:
+        #    bulge_pos1, bulge_pos2 = bulge_pos2, bulge_pos1
+        #bulge_amount = (self.tweak_bulgediameter-1.0) * bore_diameter
+        #inst.inner = inst.inner + profile.Profile(
+        #    [ bulge_pos1, bulge_pos2 ],
+        #    [ 0.0, bulge_amount ],
+        #    [ bulge_amount, 0.0 ],
+        #    )
+        
         maker = self.get_whistle_maker()
-        diameter = maker.effective_gap_diameter()                
-        length = maker.effective_gap_height()
-        length += diameter * self.tweak_gapextra  # Virtual extra length seems to be needed, as with flute
-                                                  # Not so much if hole is large though
+        diameter = maker.effective_gap_diameter()             
+        length = maker.effective_gap_height() / 2.0
+        #        ^ The gap is this high on one side and a blade on the other side
+        #          split the difference.
+        length += diameter * self.tweak_gapextra
         
         inst.inner = profile.Profile(
-            inst.inner.pos + [ inst.length + length ],
+            inst.inner.pos + [ inst.length+length ],
             inst.inner.low + [ diameter ],
             inst.inner.high[:-1] + [ diameter, diameter ],
             )
         inst.length += length
         return inst
 
 
@@ -69,23 +93,25 @@
     balance = [ 0.2 ]*4
     @property
     def min_hole_spacing(self):
         b = self.inner_diameters[-1]
         return [ b*1.15 ] * 5 #[ b,b,b*1.25,b,b ]
 
     inner_diameters = design.sqrt_scaler([ 24.0, 20.0, 20.0, 22.0, 20.0, 20.0 ])
-    outer_diameters = design.sqrt_scaler([ 38.0, 28.0, 28.0 ])
-    
     initial_inner_fractions = [ 0.2, 0.6,0.65,0.7 ]
-    
-    initial_outer_fractions = [ 0.15 ]
-    min_outer_fraction_sep = [ 0.15, 0.8 ]
-    
     min_inner_fraction_sep = [ 0.02 ] * 5
 
+#    outer_diameters = design.sqrt_scaler([ 38.0, 28.0, 28.0 ])    
+#    initial_outer_fractions = [ 0.15 ]
+#    min_outer_fraction_sep = [ 0.15, 0.8 ]
+
+    outer_diameters = design.sqrt_scaler([ 40.0, 28.0, 28.0, 32.0, 32.0 ])    
+    initial_outer_fractions = [ 0.15, 0.5, 0.85 ]
+    min_outer_fraction_sep = [ 0.15, 0.3, 0.35, 0.15 ]
+    
     #min_outer_fraction_sep = [ 0.01, 0.5 ]
 
     fingerings = [
         ('D4',   [1,1,1,1,1,1]),
         ('E4',   [0,1,1,1,1,1]),
         ('F#4',  [0,0,1,1,1,1]),
         ('G4',   [0,0,0,1,1,1]),
@@ -111,76 +137,91 @@
 """)
 class Design_recorder(Design_whistle):
     divisions = [
         [(7,0)],
         [(0,0),(7,0)],
         [(0,0),(3,0),(7,0)],
         [(0,0),(3,0),(7,0),(7,0.5)],
+        [(0,0),(2,0),(4,0),(7,0),(7,0.5)],
         ]
     
     initial_length = design.wavelength('C4') * 0.5
     
     min_hole_diameters = design.sqrt_scaler([ 3.0 ]*8)
-    max_hole_diameters = design.sqrt_scaler([ 15.0 ]*8)
+    max_hole_diameters = design.sqrt_scaler([ 12.0 ] + [ 14.0 ]*7)
+    min_hole_spacing = design.sqrt_scaler([ 0.0 ]*6+[-50.0])
 
-    horiz_angles = [ -20.0 ] + [ 0.0 ] * 6 + [ 180.0 ]
-    mid_cut = 3
+    horiz_angles = [ -15.0 ] + [ 0.0 ] * 6 + [ 180.0 ]
+    hole_angles = [ -30, 30, -30, 30, 0, 0, 0, 0 ]
 
     balance = [ 0.1, 0.05, None, None, 0.05, None ]
     #balance = [ 0.2 ]*4
     #@property
     #def min_hole_spacing(self):
     #    b = self.inner_diameters[-1]
     #    return [ b*1.15 ] * 5 #[ b,b,b*1.25,b,b ]
 
-    inner_diameters = design.sqrt_scaler([ 20.0, 20.0, 23.0, 20.0, 20.0 ])
-    outer_diameters = design.sqrt_scaler([ 40.0, 30.0, 30.0 ])
-    
-    initial_inner_fractions = [ 0.6,0.65,0.7 ]
-    
-    initial_outer_fractions = [ 0.15 ]
-    min_outer_fraction_sep = [ 0.15, 0.8 ]
-    
-    min_inner_fraction_sep = [ 0.4 ] + [ 0.01 ] * 5
+#    inner_diameters = design.sqrt_scaler([ 17.0, 20.0, 20.0, 23.0, 20.0, 20.0 ])
+    inner_diameters = design.sqrt_scaler([ 20.0, 20.0, 19.0, 23.0, 23.0, 20.0, 20.0 ])
+    initial_inner_fractions = [ 0.6,0.65,0.7,0.75,0.8 ]
+    min_inner_fraction_sep = [ 0.3,0.01,0.01,0.01,0.01,0.01 ]
+
+    outer_diameters = design.sqrt_scaler([ 40.0, 28.0, 28.0, 32.0, 32.0 ])    
+    initial_outer_fractions = [ 0.15, 0.6, 0.85 ]
+    min_outer_fraction_sep = [ 0.15, 0.3, 0.35, 0.15 ]
 
-    #min_outer_fraction_sep = [ 0.01, 0.5 ]
 
     fingerings = [
         ('C4',   [1,1,1,1,1,1,1,1]),
+        # Inter-register locking
+        ('C5',   [1,1,1,1,1,1,1,1]),
+        ('G5',   [1,1,1,1,1,1,1,1]),
+
         ('D4',   [0,1,1,1,1,1,1,1]),
+        # Inter-register locking
+        ('D5',   [0,1,1,1,1,1,1,1]),
+        ('A5',   [0,1,1,1,1,1,1,1]),
+
         ('E4',   [0,0,1,1,1,1,1,1]),
+        # Inter-register locking
+        ('B5',   [0,0,1,1,1,1,1,1]),
+        
+        #Tendency to be sharp, due to inter register locking?
         ('F4',   [1,1,0,1,1,1,1,1]),
+        ('F4',   [0,1,0,1,1,1,1,1]),
+        
         ('F#4',  [0,1,1,0,1,1,1,1]),
         ('G4',   [0,0,0,0,1,1,1,1]),
         ('G#4',  [0,1,1,1,0,1,1,1]),
         ('A4',   [0,0,0,0,0,1,1,1]),
         ('Bb4',  [0,0,0,1,1,0,1,1]),
         ('B4',   [0,0,0,0,0,0,1,1]),
         ('C5',   [0,0,0,0,0,1,0,1]),
         ('C#5',  [0,0,0,0,0,1,1,0]),
         ('D5',   [0,0,0,0,0,1,0,0]),
 
+
         ('Eb5',  [0,1,1,1,1,1,0,0]),
         
         ('E5',   [0,0,1,1,1,1,1,0]),
         ('E5',   [0,0,1,1,1,1,1,1]),
         
         ('F5',   [0,1,0,1,1,1,1,0]),
         ('F5',   [0,1,0,1,1,1,1,1]),
         
         ('F#5',  [0,0,1,0,1,1,1,0]),
         ('F#5',  [0,0,1,0,1,1,1,1]),
 
         #('G5',   [0,0,0,0,1,1,1,0]),
         ('G5',   [0,0,0,0,1,1,1,1]),
 
-        ('G#5',  [0,0,0,1,0,1,1,1]),
+        #('G#5',  [0,0,0,1,0,1,1,1]),
         ('A5',   [0,0,0,0,0,1,1,1]),
-        ('Bb5',  [0,1,1,1,0,1,1,1]),
-        ('B5',   [0,0,1,1,0,1,1,1]),
+#        ('Bb5',  [0,1,1,1,0,1,1,1]),
+#        ('B5',   [0,0,1,1,0,1,1,1]),
     ]
     
 
 @config.help("""\
 Design a three hole pipe, i.e. the pipe in pipe-and-tabor.
 """)
 class Design_three_hole_whistle(Design_whistle):
@@ -189,32 +230,31 @@
         [(2,0.05),(2,0.5)],
         [(2,0),(2,0.333),(2,0.666)],
         ]
     
     initial_length = design.wavelength('D3') * 0.5
     
     min_hole_diameters = design.sqrt_scaler([ 3.0 ]*3)
-    max_hole_diameters = design.sqrt_scaler([ 20.0 ]*3)
+    max_hole_diameters = design.sqrt_scaler([ 14.0 ]*3)
     
     horiz_angles = [ 0.0, 0.0, 180.0 ]
     mid_cut = 2
     
     #min_hole_spacing = [ -20.0, -20.0 ]
     
     initial_hole_fractions = [ 0.1,0.15,0.2 ]
     
-    inner_diameters = design.sqrt_scaler([ 20.0, 20.0 ])
+    inner_diameters = design.sqrt_scaler([ 15.0, 15.0, 20.0, 20.0 ])
+    initial_inner_fractions = [ 0.1, 0.75 ]
     
-    outer_add = True
-    outer_diameters = design.sqrt_scaler([ 8.0, 8.0 ])
+    outer_diameters = design.sqrt_scaler([ 40.0, 28.0, 28.0, 32.0, 32.0 ])
+    min_outer_fraction_sep = [ 0.1, 0.45, 0.3, 0.1 ]
+    initial_outer_fractions = [ 0.1, 0.6, 0.9 ]
     
-    initial_inner_fractions = [ ]
     
-    initial_outer_fractions = [ ]
-    #min_outer_fraction_sep = [ 0.15, 0.8 ]
     
     min_inner_fraction_sep = [ 0.01 ] * 8
 
     fingerings = [
         ('D4', [1,1,1]),
         ('E4', [0,1,1]),
         ('F#4',[0,0,1]),
```

### Comparing `demakein-0.7/demakein/make_flute.py` & `demakein-0.9/demakein/make_flute.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/pack.py` & `demakein-0.9/demakein/pack.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/profile.py` & `demakein-0.9/demakein/profile.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/make_reed.py` & `demakein-0.9/demakein/make_reed.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/make_whistle.py` & `demakein-0.9/demakein/make_whistle.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,25 @@
 @config.Float_flag('outside')
 @config.Float_flag('gap_width')
 @config.Float_flag('gap_length')
 class Make_whistle_head(make.Make):
     bore = 15.0
     outside = 21.0
     
-    gap_width = 0.666 #Formerly 0.5
-    gap_length = 0.4 #Formerly 0.25
+    gap_width = 0.6 #0.5 #0.666 #Formerly 0.5
+    gap_length = 0.25 #0.3 #0.4 #Formerly 0.25
+    # (as a proportion of bore diameter)
 
     def effective_gap_diameter(self):
-        # gap_length * airway_ysize
-        area = (self.bore*0.25) * (self.bore*self.gap_width)
+        area = (self.bore*self.gap_length) * (self.bore*self.gap_width)
         return math.sqrt(area/math.pi) * 2.0
     
     def effective_gap_height(self):
         # TODO: further adjustment
-        return self.bore*(1.4-1.0) * 0.5
+        return (self.outside-self.bore) * 0.5
 
     def construct(self):
         bore = self.bore
         outside = self.outside
         #outside = bore * 1.4
         
         bore_length = bore*2.0        
@@ -50,18 +50,21 @@
         z_gap_1 = z_min + bore_length
         z_windcutter_0 = z_gap_0 - windcutter_length
         z_windcutter_1 = z_gap_0
         z_airway_0 = z_gap_1
         z_airway_1 = z_airway_0 + airway_length
         z_max = z_airway_1
         
-        airway_xsize = bore * 0.15
+        #airway_xsize = bore * 0.15
+        #airway_xsize = (outside-bore) * 0.4
+        airway_xsize = 2.0 #Constant!
+        
         airway_ysize = bore * self.gap_width
         
-        print 'Note mill bit diameter must be less than: %.1fmm' % (airway_xsize*2.0)
+        #print 'Note mill bit diameter must be less than: %.1fmm' % (airway_xsize*2.0)
         
         windcutter_rounding = bore * 0.1
         windcutter_ysize = airway_ysize + windcutter_rounding
         windcutter_lip = bore * 0.02
 
         airway_x_low  = bore*0.5-airway_xsize*0.5+windcutter_lip*0.5
         airway_x_high = bore*0.5+airway_xsize*0.5+windcutter_lip*0.5
@@ -75,15 +78,15 @@
              (z_airway_1, airway_x_high)])
         
         windcutter_line = profile.make_profile(
             [(z_windcutter_0, outside*0.5),
              (z_windcutter_1, bore*0.5+windcutter_lip)])
         
         undercutter_line = profile.make_profile(
-            [(z_windcutter_0, bore*0.4),
+            [(z_windcutter_0, bore*0.35),
              (z_windcutter_1, bore*0.5)])
         
         body = shape.extrude_profile(
             profile.make_profile([(z_min,outside),(z_max,outside)]),
             )
         
         bore_space = shape.extrude_profile(
@@ -102,26 +105,27 @@
             )
         body.remove(windcutter_space)
         #space.add(windcutter_space)
         
         undercutter_space = shape.extrude_profile(
             undercutter_line.clipped(z_windcutter_0,z_gap_1),
             cross_section = lambda x:
-                shape.halfrounded_rectangle(
+#                shape.halfrounded_rectangle(
+                shape.rectangle(
                     x-airway_xsize, x,
                     airway_ysize*-0.5,airway_ysize*0.5)
             )
         #body.remove(undercutter_space)
         space.add(undercutter_space)
                
         airway_space = shape.extrude_profile(
             airway_line_0.clipped(z_gap_0,z_airway_1+ airway_xsize*2), #Make longer, for milling inside
             airway_line_1.clipped(z_gap_0,z_airway_1+ airway_xsize*2),
             cross_section = lambda x0, x1:
-                shape.halfrounded_rectangle(
+                shape.rectangle(
                     x0, x1,
                     airway_ysize*-0.5,airway_ysize*0.5)
             )
         body.remove(airway_space)
         space.add(airway_space)
         
         gap_space = shape.block(
@@ -254,17 +258,20 @@
             #self.segment([ cut1, cut2 ], spec.length, up=True)
             #self.segment([ cut0, cut1, cut3 ], spec.length, up=True)
         
             for division in designer.divisions:
                 cuts = [ ]
                 for hole, above in division:
                     cut = spec.hole_positions[hole] + spec.hole_diameters[hole]*0.75
-                    cut += spec.inner(cut)*0.5
+                    #cut += spec.outer(cut)*0.5
                     cut += (true_length-cut)*above
                     cuts.append(cut)
+                    
+                cuts.append(spec.length)
+                    
                 self.segment(cuts, true_length, up=True)
         
         else:
             mid1 = spec.hole_positions[2]*0.5+spec.hole_diameters[2]*0.5-spec.hole_diameters[3]*0.5+spec.hole_positions[3]*0.5
             mid2 = spec.hole_positions[5]+spec.hole_diameters[5]
         
             upper_segments, lower_segments = pack.plan_segments([mid1/true_length,mid2/true_length], self.mill_length / true_length)
```

### Comparing `demakein-0.7/demakein/cgal.py` & `demakein-0.9/demakein/cgal.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/make_shawm.py` & `demakein-0.9/demakein/make_shawm.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/make_cork.py` & `demakein-0.9/demakein/make_cork.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/design_flute.py` & `demakein-0.9/demakein/design_flute.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/design_shawm.py` & `demakein-0.9/demakein/design_shawm.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/make_panpipe.py` & `demakein-0.9/demakein/make_panpipe.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/make_bauble.py` & `demakein-0.9/demakein/make_bauble.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/raphs_curves/mecsolve.py` & `demakein-0.9/demakein/raphs_curves/mecsolve.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/raphs_curves/bezfigs.py` & `demakein-0.9/demakein/raphs_curves/bezfigs.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/raphs_curves/polymat-bad.py` & `demakein-0.9/demakein/raphs_curves/polymat-bad.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/raphs_curves/bigmat.py` & `demakein-0.9/demakein/raphs_curves/bigmat.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/raphs_curves/numintsynth.py` & `demakein-0.9/demakein/raphs_curves/numintsynth.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/raphs_curves/offset.py` & `demakein-0.9/demakein/raphs_curves/offset.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/raphs_curves/tocubic.py` & `demakein-0.9/demakein/raphs_curves/tocubic.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/raphs_curves/polymat.py` & `demakein-0.9/demakein/raphs_curves/polymat.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/raphs_curves/clothoid.py` & `demakein-0.9/demakein/raphs_curves/clothoid.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/raphs_curves/fromcubic.py` & `demakein-0.9/demakein/raphs_curves/fromcubic.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/raphs_curves/mvc.py` & `demakein-0.9/demakein/raphs_curves/mvc.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/raphs_curves/cornu.py` & `demakein-0.9/demakein/raphs_curves/cornu.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/raphs_curves/pcorn.py` & `demakein-0.9/demakein/raphs_curves/pcorn.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/raphs_curves/plot_solve_clothoid.py` & `demakein-0.9/demakein/raphs_curves/plot_solve_clothoid.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/raphs_curves/band.py` & `demakein-0.9/demakein/raphs_curves/band.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/raphs_curves/poly3.py` & `demakein-0.9/demakein/raphs_curves/poly3.py`

 * *Files identical despite different names*

### Comparing `demakein-0.7/demakein/raphs_curves/euler-elastica.py` & `demakein-0.9/demakein/raphs_curves/euler-elastica.py`

 * *Files identical despite different names*

