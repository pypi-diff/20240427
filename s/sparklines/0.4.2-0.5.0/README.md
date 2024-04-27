# Comparing `tmp/sparklines-0.4.2.tar.gz` & `tmp/sparklines-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sparklines-0.4.2.tar", last modified: Fri Jul 27 09:45:55 2018, max compression
+gzip compressed data, was "sparklines-0.5.0.tar", last modified: Sat Apr 27 09:23:21 2024, max compression
```

## Comparing `sparklines-0.4.2.tar` & `sparklines-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxr-xr-x   0 dinu       (501) staff       (20)        0 2018-07-27 09:45:55.000000 sparklines-0.4.2/
--rw-r--r--   0 dinu       (501) staff       (20)     1004 2018-07-27 09:26:28.000000 sparklines-0.4.2/CHANGELOG.txt
--rw-r--r--   0 dinu       (501) staff       (20)      121 2018-07-27 09:28:35.000000 sparklines-0.4.2/CONTRIBUTORS.txt
--rw-r--r--   0 dinu       (501) staff       (20)    35142 2018-07-27 09:15:33.000000 sparklines-0.4.2/LICENSE.txt
--rw-r--r--   0 dinu       (501) staff       (20)      102 2018-07-27 09:15:33.000000 sparklines-0.4.2/MANIFEST.in
--rw-r--r--   0 dinu       (501) staff       (20)     8038 2018-07-27 09:45:55.000000 sparklines-0.4.2/PKG-INFO
--rw-r--r--   0 dinu       (501) staff       (20)     6074 2018-07-27 09:15:33.000000 sparklines-0.4.2/README.rst
--rw-r--r--   0 dinu       (501) staff       (20)      101 2018-07-27 09:45:55.000000 sparklines-0.4.2/setup.cfg
--rw-r--r--   0 dinu       (501) staff       (20)     1409 2018-07-27 09:27:08.000000 sparklines-0.4.2/setup.py
-drwxr-xr-x   0 dinu       (501) staff       (20)        0 2018-07-27 09:45:55.000000 sparklines-0.4.2/sparklines/
--rw-r--r--   0 dinu       (501) staff       (20)      175 2018-07-27 09:15:33.000000 sparklines-0.4.2/sparklines/__init__.py
--rw-r--r--   0 dinu       (501) staff       (20)     4439 2018-07-27 09:40:28.000000 sparklines-0.4.2/sparklines/__main__.py
--rw-r--r--   0 dinu       (501) staff       (20)     7006 2018-07-27 09:15:33.000000 sparklines-0.4.2/sparklines/sparklines.py
-drwxr-xr-x   0 dinu       (501) staff       (20)        0 2018-07-27 09:45:55.000000 sparklines-0.4.2/sparklines.egg-info/
--rw-r--r--   0 dinu       (501) staff       (20)        1 2018-07-27 09:45:55.000000 sparklines-0.4.2/sparklines.egg-info/dependency_links.txt
--rw-r--r--   0 dinu       (501) staff       (20)       57 2018-07-27 09:45:55.000000 sparklines-0.4.2/sparklines.egg-info/entry_points.txt
--rw-r--r--   0 dinu       (501) staff       (20)     8038 2018-07-27 09:45:55.000000 sparklines-0.4.2/sparklines.egg-info/PKG-INFO
--rw-r--r--   0 dinu       (501) staff       (20)        7 2018-07-27 09:45:55.000000 sparklines-0.4.2/sparklines.egg-info/requires.txt
--rw-r--r--   0 dinu       (501) staff       (20)      426 2018-07-27 09:45:55.000000 sparklines-0.4.2/sparklines.egg-info/SOURCES.txt
--rw-r--r--   0 dinu       (501) staff       (20)       16 2018-07-27 09:45:55.000000 sparklines-0.4.2/sparklines.egg-info/top_level.txt
-drwxr-xr-x   0 dinu       (501) staff       (20)        0 2018-07-27 09:45:55.000000 sparklines-0.4.2/test/
--rw-r--r--   0 dinu       (501) staff       (20)        0 2018-07-27 09:15:33.000000 sparklines-0.4.2/test/__init__.py
--rw-r--r--   0 dinu       (501) staff       (20)   265540 2018-07-27 09:15:33.000000 sparklines-0.4.2/test/runtests.py
--rw-r--r--   0 dinu       (501) staff       (20)     5517 2018-07-27 09:15:33.000000 sparklines-0.4.2/test/test_sparkline.py
--rw-r--r--   0 dinu       (501) staff       (20)       97 2018-07-27 09:26:47.000000 sparklines-0.4.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:23:21.419784 sparklines-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-27 09:23:11.000000 sparklines-0.5.0/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-27 09:23:11.000000 sparklines-0.5.0/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35142 2024-04-27 09:23:11.000000 sparklines-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-27 09:23:11.000000 sparklines-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-27 09:23:21.419784 sparklines-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-04-27 09:23:11.000000 sparklines-0.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-27 09:23:21.423784 sparklines-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-27 09:23:11.000000 sparklines-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:23:21.419784 sparklines-0.5.0/sparklines/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-27 09:23:11.000000 sparklines-0.5.0/sparklines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-27 09:23:11.000000 sparklines-0.5.0/sparklines/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-27 09:23:11.000000 sparklines-0.5.0/sparklines/sparklines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:23:21.419784 sparklines-0.5.0/sparklines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-27 09:23:21.000000 sparklines-0.5.0/sparklines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-27 09:23:21.000000 sparklines-0.5.0/sparklines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 09:23:21.000000 sparklines-0.5.0/sparklines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-27 09:23:21.000000 sparklines-0.5.0/sparklines.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-27 09:23:21.000000 sparklines-0.5.0/sparklines.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:23:21.419784 sparklines-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 09:23:11.000000 sparklines-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-27 09:23:11.000000 sparklines-0.5.0/tests/test_sparkline.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sparklines-0.4.2/CHANGELOG.txt` & `sparklines-0.5.0/CHANGELOG.txt`

 * *Files 25% similar despite different names*

```diff
@@ -20,13 +20,20 @@
 - added filter to unclutter input numbers (remove commas, etc.)
 - added tox support
 - added more tests
 - added asciicast to README.rst
 
 0.4.1: Fourth release:
 
-- improved command-line option -e/--emphasise to take only one argument,
+- improved command-line option -e/--emphasize to take only one argument,
   but can be used repeatedly now, which reduces unexpected behaviour
 
 0.4.2: Fifth release:
 
 - fixed a buglet preventing pip install without future already installed
+
+0.5.0: Sixth release:
+
+- dropped Python 2 support
+- replaced Travis build with GitHub build action
+- removed minified pytest code
+- added a fix regarding regex for Python 3.12
```

### Comparing `sparklines-0.4.2/LICENSE.txt` & `sparklines-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sparklines-0.4.2/PKG-INFO` & `sparklines-0.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,185 +1,203 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: sparklines
-Version: 0.4.2
+Version: 0.5.0
 Summary: Generate sparklines for numbers using Unicode characters only.
 Home-page: https://github.com/deeplook/sparklines
 Author: Dinu Gherman
 Author-email: gherman@darwin.in-berlin.de
 License: GPL
-Description: Sparklines
-        ==========
-        
-        |ci| |pypi|
-        
-        .. |ci| image:: http://img.shields.io/travis/deeplook/sparklines.svg
-          :target: https://travis-ci.org/deeplook/sparklines
-        
-        .. |pypi| image:: https://img.shields.io/pypi/v/sparklines.svg
-          :target: https://pypi.python.org/pypi/sparklines
-        
-        This Python package implements Edward Tufte's concept of sparklines_, but
-        limited to text only e.g. like this: ▃▁▄▁▅█▂▅ (this I likely not displayed
-        correctly in every browser). You can find more information about sparklines
-        `on Wikipedia`_. This code was mainly developed for running simple
-        plausibility tests in sensor networks as shown in fig. 1 below:
-        
-        .. figure:: https://raw.githubusercontent.com/deeplook/sparklines/master/example_sensors.png
-           :width: 75%
-           :alt: example usecase with sensor values
-           :align: center
-        
-           Fig. 1: Example usecase for such "sparklines" on the command-line,
-           showing IoT sensor values (generating code not included here).
-        
-        Due to limitations of available Unicode characters this works best when all
-        values are positive. And even then true sparklines that look more like lines
-        and less like bars are a real challenge, because they would need multiple
-        characters with a single horizontal line on different vertical positions. This
-        would work only with a dedicated font, which is way beyond the scope of this
-        tool and which would significantly complicate its usage. So we stick to these
-        characters: "▁▂▃▄▅▆▇█", and use a blank for missing values.
-        
-        This code was tested ok for Python 2.6 to 2.7 and 3.2 to 3.5.
-        
-        
-        Sample output
-        -------------
-        
-        This is a recorded sample session illustrating how to use ``sparklines`` (as
-        GitHub doesn't render embedded Asciinema_ recordings you'll see here an image
-        pointing to the respective
-        `asciicast <https://asciinema.org/a/5xwfvcrrk09fy3ml3a8n67hep>`_):
-        
-        .. image:: https://asciinema.org/a/5xwfvcrrk09fy3ml3a8n67hep.png
-           :target: https://asciinema.org/a/5xwfvcrrk09fy3ml3a8n67hep
-        
-        Here is some example output on the command-line (please note that in some
-        browsers the vertical alignment of these block characters might be displayed
-        slightly wrong, the same effect can be seen for other repos referenced below):
-        
-        Examples for the code below:
-        
-        .. code-block:: bash
-        
-            $ sparklines 2 7 1 8 2 8 1 8
-            ▂▇▁█▂█▁█
-            $ echo 2 7 1 8 2 8 1 8 | sparklines
-            ▂▇▁█▂█▁█
-            $ sparklines < numbers.txt
-            ▂▇▁█▂█▁█
-            $ sparklines 0 2. 1e0
-            ▁█▅
-        
-        
-        Installation
-        ------------
-        
-        You can install this package using ``pip install sparklines`` from the `Python
-        Package Index`_.
-        You can also clone this repository and install it via ``python setup.py install``
-        or ``pip install -e .``.
-        After installing, you will have access system-wide (or in your virtualenv
-        if you have used that) to ``sparklines``, programmatically as well as via a
-        command-line tool with the same name.
-        
-        Test
-        ----
-        
-        To run the (still very small) "test suite", download and unpack this repository
-        or clone it, and run the command ``python setup.py test`` in the unpacked
-        archive. This will use a minified version of the ``pytest`` package included
-        in this package in the file ``test/runtests.py``. If you have the excellent
-        ``pytest`` package installed you can also run ``py.test test`` from the 
-        downloaded repository's root folder.
-        
-        
-        Usage
-        -----
-        
-        Please note that the samples below might look a little funky (misaligned or 
-        even colored) in some browsers, but it should be totally fine when you print
-        this in your terminal, Python or IPython session or your Python IDE of choice.
-        Figure 2 below might sshow better what you should expect than the copied sample
-        code thereafter:
-        
-        .. figure:: https://raw.githubusercontent.com/deeplook/sparklines/master/example_python.png
-           :width: 65%
-           :alt: example interactive invocation
-           :align: center
-        
-           Fig. 2: Example invocation from a Python and an IPython session.
-        
-        
-        Command-Line
-        ............
-        
-        Here are two sample invocations from the command-line, copied into this README:
-        
-        .. code-block:: console
-        
-            $ sparklines 1 2 3 4 5.0 null 3 2 1
-            ▁▃▅▆█ ▅▃▁
-        
-            $ sparklines -n 2 1 2 3 4 5.0 null 3 2 1
-              ▁▅█ ▁  
-            ▁▅███ █▅▁
-        
-        
-        Programmatic
-        ............
-        
-        And here are sample invocations from interactive Python sessions, copied into
-        this README. The main function to use programmatically is 
-        ``sparklines.sparklines()``:
-        
-        .. code-block:: python
-        
-            In [1]: from sparklines import sparklines
-        
-            In [2]: for line in sparklines([1, 2, 3, 4, 5.0, None, 3, 2, 1]):
-               ...:     print(line)
-               ...:     
-            ▁▃▅▆█ ▅▃▁
-        
-            In [3]: for line in sparklines([1, 2, 3, 4, 5.0, None, 3, 2, 1], num_lines=2):
-                print(line)
-               ...:     
-              ▁▅█ ▁  
-            ▁▅███ █▅▁
-        
-        
-        References
-        ----------
-        
-        This code was inspired by Zach Holman's `spark 
-        <https://github.com/holman/spark>`_, converted to a Python module 
-        by Kenneth Reitz as `spark.py 
-        <https://raw.githubusercontent.com/kennethreitz/spark.py/master/spark.py>`_ 
-        and by RegKrieg to a Python package named `pysparklines <https://github.com/RedKrieg/pysparklines>`_.
-        And Roger Allen provides an even `shorter spark.py 
-        <https://gist.githubusercontent.com/rogerallen/1368454/raw/b17e96b56ae881621a9f3b1508ca2e7fde3ec93e/spark.py>`_.
-        
-        But since it is so short and easy to code in Python we can add a few nice
-        extra features I was missing, like:
-        
-        - increasing resolution with multiple output lines per sparkline
-        - showing gaps in input numbers for missing data
-        - issuing warnings for negative values (allowed, but misleading)
-        - highlighting values exceeding some threshold with a different
-          color (if ``termcolor`` package is available)
-        - wrapping long sparklines at some max. length
-        - (todo) adding separator characters like ``:`` at regular intervals
-        
-        .. _Asciinema: https://asciinema.org
-        .. _Python Package Index: https://pypi.python.org/pypi/sparklines/
-        .. _sparklines: http://www.edwardtufte.com/bboard/q-and-a-fetch-msg?msg_id=0001OR
-        .. _on Wikipedia: https://en.wikipedia.org/wiki/Sparkline
-        
 Keywords: visualization,chart,tool
-Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Other Audience
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+License-File: LICENSE.txt
+
+Sparklines
+==========
+
+.. image:: https://img.shields.io/github/actions/workflow/status/deeplook/sparklines/python-package.yml
+  :target: https://pypi.org/project/sparklines
+
+.. image:: https://img.shields.io/pypi/pyversions/sparklines.svg
+  :target: https://pypi.org/project/sparklines
+  
+.. image:: https://img.shields.io/pypi/v/sparklines.svg
+  :target: https://pypi.org/project/sparklines/
+
+.. image:: https://static.pepy.tech/badge/sparklines/month
+  :target: https://pepy.tech/project/sparklines
+
+.. image:: https://img.shields.io/pypi/status/sparklines.svg
+  :target: https://pypi.org/project/sparklines
+
+.. image:: https://img.shields.io/pypi/format/sparklines.svg
+  :target: https://pypi.org/project/sparklines
+
+.. image:: https://img.shields.io/pypi/l/sparklines.svg
+  :target: https://pypi.org/project/sparklines
+  
+This Python package implements Edward Tufte's concept of sparklines_, but
+limited to text only e.g. like this: ▃▁▄▁▅█▂▅ (this I likely not displayed
+correctly in every browser). You can find more information about sparklines
+`on Wikipedia`_. This code was mainly developed for running simple
+plausibility tests in sensor networks as shown in fig. 1 below:
+
+.. figure:: https://raw.githubusercontent.com/deeplook/sparklines/main/example_sensors.png
+   :width: 75%
+   :alt: example usecase with sensor values
+   :align: center
+
+   Fig. 1: Example usecase for such "sparklines" on the command-line,
+   showing IoT sensor values (generating code not included here).
+
+Due to limitations of available Unicode characters this works best when all
+values are positive. And even then true sparklines that look more like lines
+and less like bars are a real challenge, because they would need multiple
+characters with a single horizontal line on different vertical positions. This
+would work only with a dedicated font, which is way beyond the scope of this
+tool and which would significantly complicate its usage. So we stick to these
+characters: "▁▂▃▄▅▆▇█", and use a blank for missing values.
+
+This code was tested ok at some point for Python 2.6 and 2.7, but no longer
+supports Python 2 after it reached end-of-life. Now Python 3.5 to 3.8 as well
+as PyPy 3 are all tested via Travis-CI.
+
+
+Sample output
+-------------
+
+This is a recorded sample session illustrating how to use ``sparklines`` (as
+GitHub doesn't render embedded Asciinema_ recordings you'll see here an image
+pointing to the respective
+`asciicast <https://asciinema.org/a/5xwfvcrrk09fy3ml3a8n67hep>`_):
+
+.. image:: https://asciinema.org/a/5xwfvcrrk09fy3ml3a8n67hep.png
+   :target: https://asciinema.org/a/5xwfvcrrk09fy3ml3a8n67hep
+
+Here is some example output on the command-line (please note that in some
+browsers the vertical alignment of these block characters might be displayed
+slightly wrong, the same effect can be seen for other repos referenced below):
+
+Examples for the code below:
+
+.. code-block:: bash
+
+    $ sparklines 2 7 1 8 2 8 1 8
+    ▂▇▁█▂█▁█
+    $ echo 2 7 1 8 2 8 1 8 | sparklines
+    ▂▇▁█▂█▁█
+    $ sparklines < numbers.txt
+    ▂▇▁█▂█▁█
+    $ sparklines 0 2. 1e0
+    ▁█▅
+
+
+Installation
+------------
+
+You can install this package using ``pip install sparklines`` from the `Python
+Package Index`_.
+You can also clone this repository and install it via ``python setup.py install``
+or ``pip install -e .``.
+After installing, you will have access system-wide (or in your virtualenv
+if you have used that) to ``sparklines``, programmatically as well as via a
+command-line tool with the same name.
+
+Test
+----
+
+To run the test suite, download and unpack this repository or clone it,
+run `pip inastall pytest`, and run the command ``pytest tests`` in the
+unpacked archive. from the downloaded repository's root folder.
+
+
+Usage
+-----
+
+Please note that the samples below might look a little funky (misaligned or 
+even colored) in some browsers, but it should be totally fine when you print
+this in your terminal, Python or IPython session or your Python IDE of choice.
+Figure 2 below might show better what you should expect than the copied sample
+code thereafter:
+
+.. figure:: https://raw.githubusercontent.com/deeplook/sparklines/main/example_python.png
+   :width: 65%
+   :alt: example interactive invocation
+   :align: center
+
+   Fig. 2: Example invocation from a Python and an IPython session.
+
+
+Command-Line
+............
+
+Here are two sample invocations from the command-line, copied into this README:
+
+.. code-block:: console
+
+    $ sparklines 1 2 3 4 5.0 null 3 2 1
+    ▁▃▅▆█ ▅▃▁
+
+    $ sparklines -n 2 1 2 3 4 5.0 null 3 2 1
+      ▁▅█ ▁  
+    ▁▅███ █▅▁
+
+
+Programmatic
+............
+
+And here are sample invocations from interactive Python sessions, copied into
+this README. The main function to use programmatically is 
+``sparklines.sparklines()``:
+
+.. code-block:: python
+
+    In [1]: from sparklines import sparklines
+
+    In [2]: for line in sparklines([1, 2, 3, 4, 5.0, None, 3, 2, 1]):
+       ...:     print(line)
+       ...:     
+    ▁▃▅▆█ ▅▃▁
+
+    In [3]: for line in sparklines([1, 2, 3, 4, 5.0, None, 3, 2, 1], num_lines=2):
+        print(line)
+       ...:     
+      ▁▅█ ▁  
+    ▁▅███ █▅▁
+
+
+References
+----------
+
+This code was inspired by Zach Holman's `spark 
+<https://github.com/holman/spark>`_, converted to a Python module 
+by Kenneth Reitz as `spark.py 
+<https://raw.githubusercontent.com/kennethreitz/spark.py/master/spark.py>`_ 
+and by RegKrieg to a Python package named `pysparklines <https://github.com/RedKrieg/pysparklines>`_.
+And Roger Allen provides an even `shorter spark.py 
+<https://gist.githubusercontent.com/rogerallen/1368454/raw/b17e96b56ae881621a9f3b1508ca2e7fde3ec93e/spark.py>`_.
+
+But since it is so short and easy to code in Python we can add a few nice
+extra features I was missing, like:
+
+- increasing resolution with multiple output lines per sparkline
+- showing gaps in input numbers for missing data
+- issuing warnings for negative values (allowed, but misleading)
+- highlighting values exceeding some threshold with a different
+  color (if ``termcolor`` package is available)
+- wrapping long sparklines at some max. length
+- (todo) adding separator characters like ``:`` at regular intervals
+
+.. _Asciinema: https://asciinema.org
+.. _Python Package Index: https://pypi.python.org/pypi/sparklines/
+.. _sparklines: http://www.edwardtufte.com/bboard/q-and-a-fetch-msg?msg_id=0001OR
+.. _on Wikipedia: https://en.wikipedia.org/wiki/Sparkline
```

### Comparing `sparklines-0.4.2/README.rst` & `sparklines-0.5.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,38 @@
 Sparklines
 ==========
 
-|ci| |pypi|
-
-.. |ci| image:: http://img.shields.io/travis/deeplook/sparklines.svg
-  :target: https://travis-ci.org/deeplook/sparklines
-
-.. |pypi| image:: https://img.shields.io/pypi/v/sparklines.svg
-  :target: https://pypi.python.org/pypi/sparklines
+.. image:: https://img.shields.io/github/actions/workflow/status/deeplook/sparklines/python-package.yml
+  :target: https://pypi.org/project/sparklines
 
+.. image:: https://img.shields.io/pypi/pyversions/sparklines.svg
+  :target: https://pypi.org/project/sparklines
+  
+.. image:: https://img.shields.io/pypi/v/sparklines.svg
+  :target: https://pypi.org/project/sparklines/
+
+.. image:: https://static.pepy.tech/badge/sparklines/month
+  :target: https://pepy.tech/project/sparklines
+
+.. image:: https://img.shields.io/pypi/status/sparklines.svg
+  :target: https://pypi.org/project/sparklines
+
+.. image:: https://img.shields.io/pypi/format/sparklines.svg
+  :target: https://pypi.org/project/sparklines
+
+.. image:: https://img.shields.io/pypi/l/sparklines.svg
+  :target: https://pypi.org/project/sparklines
+  
 This Python package implements Edward Tufte's concept of sparklines_, but
 limited to text only e.g. like this: ▃▁▄▁▅█▂▅ (this I likely not displayed
 correctly in every browser). You can find more information about sparklines
 `on Wikipedia`_. This code was mainly developed for running simple
 plausibility tests in sensor networks as shown in fig. 1 below:
 
-.. figure:: https://raw.githubusercontent.com/deeplook/sparklines/master/example_sensors.png
+.. figure:: https://raw.githubusercontent.com/deeplook/sparklines/main/example_sensors.png
    :width: 75%
    :alt: example usecase with sensor values
    :align: center
 
    Fig. 1: Example usecase for such "sparklines" on the command-line,
    showing IoT sensor values (generating code not included here).
 
@@ -27,15 +40,17 @@
 values are positive. And even then true sparklines that look more like lines
 and less like bars are a real challenge, because they would need multiple
 characters with a single horizontal line on different vertical positions. This
 would work only with a dedicated font, which is way beyond the scope of this
 tool and which would significantly complicate its usage. So we stick to these
 characters: "▁▂▃▄▅▆▇█", and use a blank for missing values.
 
-This code was tested ok for Python 2.6 to 2.7 and 3.2 to 3.5.
+This code was tested ok at some point for Python 2.6 and 2.7, but no longer
+supports Python 2 after it reached end-of-life. Now Python 3.5 to 3.8 as well
+as PyPy 3 are all tested via Travis-CI.
 
 
 Sample output
 -------------
 
 This is a recorded sample session illustrating how to use ``sparklines`` (as
 GitHub doesn't render embedded Asciinema_ recordings you'll see here an image
@@ -73,32 +88,29 @@
 After installing, you will have access system-wide (or in your virtualenv
 if you have used that) to ``sparklines``, programmatically as well as via a
 command-line tool with the same name.
 
 Test
 ----
 
-To run the (still very small) "test suite", download and unpack this repository
-or clone it, and run the command ``python setup.py test`` in the unpacked
-archive. This will use a minified version of the ``pytest`` package included
-in this package in the file ``test/runtests.py``. If you have the excellent
-``pytest`` package installed you can also run ``py.test test`` from the 
-downloaded repository's root folder.
+To run the test suite, download and unpack this repository or clone it,
+run `pip inastall pytest`, and run the command ``pytest tests`` in the
+unpacked archive. from the downloaded repository's root folder.
 
 
 Usage
 -----
 
 Please note that the samples below might look a little funky (misaligned or 
 even colored) in some browsers, but it should be totally fine when you print
 this in your terminal, Python or IPython session or your Python IDE of choice.
-Figure 2 below might sshow better what you should expect than the copied sample
+Figure 2 below might show better what you should expect than the copied sample
 code thereafter:
 
-.. figure:: https://raw.githubusercontent.com/deeplook/sparklines/master/example_python.png
+.. figure:: https://raw.githubusercontent.com/deeplook/sparklines/main/example_python.png
    :width: 65%
    :alt: example interactive invocation
    :align: center
 
    Fig. 2: Example invocation from a Python and an IPython session.
```

### Comparing `sparklines-0.4.2/sparklines/sparklines.py` & `sparklines-0.5.0/sparklines/sparklines.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,81 +1,68 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 """
 Text-based sparklines, e.g. on the command-line like this: ▃▁▄▁▄█▂▅.
 
 Please read the file README.rst for more information.
 """
 
-from __future__ import unicode_literals, print_function, division
-
-import itertools
 import re
 import sys
 import warnings
 
-from future.builtins import round # bankers' rounding for Python 2
-
-
-# handle different file types in Python 2 and 3
-try:
-    import io
-    file = io.IOBase
-except ImportError:
-    pass
-
 try:
     import termcolor
+
     HAVE_TERMCOLOR = True
 except ImportError:
     HAVE_TERMCOLOR = False
 
 
 blocks = " ▁▂▃▄▅▆▇█"
 
 
 def _check_negatives(numbers):
-    "Raise warning for negative numbers."
+    """Raise warning for negative numbers."""
 
     negatives = filter(lambda x: x < 0, filter(None, numbers))
     if any(negatives):
-        neg_values = ', '.join(map(str, negatives))
-        msg = 'Found negative value(s): {0!s}. '.format(neg_values)
-        msg += 'While not forbidden, the output will look unexpected.'
+        neg_values = ", ".join(map(str, negatives))
+        msg = "Found negative value(s): {0!s}. ".format(neg_values)
+        msg += "While not forbidden, the output will look unexpected."
         warnings.warn(msg)
 
 
 def _check_emphasis(numbers, emph):
-    "Find index postions in list of numbers to be emphasized according to emph."
+    """Find index postions in list of numbers to be emphasized according to emph."""
 
-    pat = '(\w+)\:(eq|gt|ge|lt|le)\:(.+)'
+    pat = r"(\w+)\:(eq|gt|ge|lt|le)\:(.+)"
     # find values to be highlighted
-    emphasized = {} # index: color
+    emphasized = {}  # index: color
     for (i, n) in enumerate(numbers):
         if n is None:
             continue
         for em in emph:
             color, op, value = re.match(pat, em).groups()
             value = float(value)
-            if op == 'eq' and n == value:
+            if op == "eq" and n == value:
                 emphasized[i] = color
-            elif op == 'gt' and n > value:
+            elif op == "gt" and n > value:
                 emphasized[i] = color
-            elif op == 'ge' and n >= value:
+            elif op == "ge" and n >= value:
                 emphasized[i] = color
-            elif op == 'lt' and n < value:
+            elif op == "lt" and n < value:
                 emphasized[i] = color
-            elif op == 'le' and n <= value:
+            elif op == "le" and n <= value:
                 emphasized[i] = color
     return emphasized
 
 
 def scale_values(numbers, num_lines=1, minimum=None, maximum=None):
-    "Scale input numbers to appropriate range."
+    """Scale input numbers to appropriate range."""
 
     # find min/max values, ignoring Nones
     filtered = [n for n in numbers if n is not None]
     min_ = min(filtered) if minimum is None else minimum
     max_ = max(filtered) if maximum is None else maximum
     dv = max_ - min_
 
@@ -83,28 +70,37 @@
     numbers = [max(min(n, max_), min_) if n is not None else None for n in numbers]
 
     if dv == 0:
         values = [4 * num_lines if x is not None else None for x in numbers]
     elif dv > 0:
         num_blocks = len(blocks) - 1
 
-        min_index = 1.
+        min_index = 1.0
         max_index = num_lines * num_blocks
 
         values = [
             ((max_index - min_index) * (x - min_)) / dv + min_index
-            if not x is None else None for x in numbers
+            if x is not None
+            else None
+            for x in numbers
         ]
 
-        values = [round(v) or 1 if not v is None else None for v in values]
+        values = [round(v) or 1 if v is not None else None for v in values]
     return values
 
 
-def sparklines(numbers=[], num_lines=1, emph=None, verbose=False,
-        minimum=None, maximum=None, wrap=None):
+def sparklines(
+    numbers=None,
+    num_lines=1,
+    emph=None,
+    verbose=False,
+    minimum=None,
+    maximum=None,
+    wrap=None,
+):
     """
     Return a list of 'sparkline' strings for a given list of input numbers.
 
     The list of input numbers may contain None values, too, for which the
     resulting sparkline will contain a blank character (a space).
 
     Examples:
@@ -113,56 +109,67 @@
         -> ['▃▁▄▁▄█▂▅']
         sparklines([3, 1, 4, 1, 5, 9, 2, 6], num_lines=2)
         -> [
             '     █ ▂',
             '▅▁▆▁██▃█'
         ]
     """
+    if numbers is None:
+        numbers = []
 
     assert num_lines > 0
 
     if len(numbers) == 0:
-        return ['']
+        return [""]
 
     # raise warning for negative numbers
     _check_negatives(numbers)
 
-    values = scale_values(numbers, num_lines=num_lines, minimum=minimum, maximum=maximum)
+    values = scale_values(
+        numbers, num_lines=num_lines, minimum=minimum, maximum=maximum
+    )
 
     # find values to be highlighted
     emphasized = _check_emphasis(numbers, emph) if emph else {}
 
     point_index = 0
     subgraphs = []
     for subgraph_values in batch(wrap, values):
         multi_values = []
         for i in range(num_lines):
-            multi_values.append([
-                min(v, 8) if not v is None else None
-                for v in subgraph_values
-            ])
-            subgraph_values = [max(0, v-8) if not v is None else None for v in subgraph_values]
+            multi_values.append(
+                [min(v, 8) if v is not None else None for v in subgraph_values]
+            )
+            subgraph_values = [
+                max(0, v - 8) if v is not None else None for v in subgraph_values
+            ]
         multi_values.reverse()
         lines = []
         for subgraph_values in multi_values:
             if HAVE_TERMCOLOR and emphasized:
                 tc = termcolor.colored
-                res = [tc(blocks[int(v)], emphasized.get(point_index + i, 'white')) if not v is None else ' ' for (i, v) in enumerate(subgraph_values)]
+                res = [
+                    tc(blocks[int(v)], emphasized.get(point_index + i, "white"))
+                    if v is not None
+                    else " "
+                    for (i, v) in enumerate(subgraph_values)
+                ]
             else:
-                res = [blocks[int(v)] if not v is None else ' ' for v in subgraph_values]
-            lines.append(''.join(res))
+                res = [
+                    blocks[int(v)] if v is not None else " " for v in subgraph_values
+                ]
+            lines.append("".join(res))
         subgraphs.append(lines)
         point_index += len(subgraph_values)
 
-    return list_join('', subgraphs)
-
+    return list_join("", subgraphs)
 
 
 def batch(batch_size, items):
-    "Batch items into groups of batch_size"
+    """Batch items into groups of batch_size."""
     items = list(items)
     if batch_size is None:
         return [items]
     MISSING = object()
     padded_items = items + [MISSING] * (batch_size - 1)
     groups = zip(*[padded_items[i::batch_size] for i in range(batch_size)])
     return [[item for item in group if item != MISSING] for group in groups]
@@ -175,51 +182,61 @@
         result.append(separator)
 
     if lists:
         result.extend(lists[-1])
     return result
 
 
-def demo(nums=[]):
-    "Print a few usage examples on stdout."
+def demo(nums=None):
+    """Print a few usage examples on stdout."""
+    if nums is None:
+        nums = []
 
     nums = nums or [3, 1, 4, 1, 5, 9, 2, 6]
-    fmt = lambda num: '{0:g}'.format(num) if isinstance(num, (float, int)) else 'None'
+
+    def fmt(num):
+        return "{0:g}".format(num) if isinstance(num, (float, int)) else "None"
+
     nums1 = list(map(fmt, nums))
 
-    if __name__ == '__main__':
+    if __name__ == "__main__":
         prog = sys.argv[0]
     else:
-        prog = 'sparklines'
+        prog = "sparklines"
 
     result = []
 
+    result.append("Usage examples (command-line and programmatic use):")
+    result.append("")
 
-    result.append('Usage examples (command-line and programmatic use):')
-    result.append('')
-
-    result.append('- Standard one-line sparkline')
-    result.append('{0!s} {1!s}'.format(prog, ' '.join(nums1)))
-    result.append('>>> print(sparklines([{0!s}])[0])'.format(', '.join(nums1)))
+    result.append("- Standard one-line sparkline")
+    result.append("{0!s} {1!s}".format(prog, " ".join(nums1)))
+    result.append(">>> print(sparklines([{0!s}])[0])".format(", ".join(nums1)))
     result.append(sparklines(nums)[0])
-    result.append('')
+    result.append("")
 
-    result.append('- Multi-line sparkline (n=2)')
-    result.append('{0!s} -n 2 {1!s}'.format(prog, ' '.join(nums1)))
-    result.append('>>> for line in sparklines([{0!s}], num_lines=2): print(line)'.format(', '.join(nums1)))
+    result.append("- Multi-line sparkline (n=2)")
+    result.append("{0!s} -n 2 {1!s}".format(prog, " ".join(nums1)))
+    result.append(
+        ">>> for line in sparklines"
+        "([{0!s}], num_lines=2): print(line)".format(", ".join(nums1))
+    )
     for line in sparklines(nums, num_lines=2):
         result.append(line)
-    result.append('')
+    result.append("")
 
-    result.append('- Multi-line sparkline (n=3)')
-    result.append('{0!s} -n 3 {1!s}'.format(prog, ' '.join(nums1)))
-    result.append('>>> for line in sparklines([{0!s}], num_lines=3): print(line)'.format(', '.join(nums1)))
+    result.append("- Multi-line sparkline (n=3)")
+    result.append("{0!s} -n 3 {1!s}".format(prog, " ".join(nums1)))
+    result.append(
+        ">>> for line in sparklines"
+        "([{0!s}], num_lines=3): print(line)".format(", ".join(nums1))
+    )
     for line in sparklines(nums, num_lines=3):
         result.append(line)
-    result.append('')
+    result.append("")
 
     nums = nums + [None] + list(reversed(nums[:]))
-    result.append('- Standard one-line sparkline with gap')
-    result.append('{0!s} {1!s}'.format(prog, ' '.join(map(str, nums))))
-    result.append('>>> print(sparklines([{0!s}])[0])'.format(', '.join(map(str, nums))))
+    result.append("- Standard one-line sparkline with gap")
+    result.append("{0!s} {1!s}".format(prog, " ".join(map(str, nums))))
+    result.append(">>> print(sparklines([{0!s}])[0])".format(", ".join(map(str, nums))))
     result.append(sparklines(nums)[0])
-    return '\n'.join(result) + '\n'
+    return "\n".join(result) + "\n"
```

### Comparing `sparklines-0.4.2/sparklines.egg-info/PKG-INFO` & `sparklines-0.5.0/sparklines.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,185 +1,203 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: sparklines
-Version: 0.4.2
+Version: 0.5.0
 Summary: Generate sparklines for numbers using Unicode characters only.
 Home-page: https://github.com/deeplook/sparklines
 Author: Dinu Gherman
 Author-email: gherman@darwin.in-berlin.de
 License: GPL
-Description: Sparklines
-        ==========
-        
-        |ci| |pypi|
-        
-        .. |ci| image:: http://img.shields.io/travis/deeplook/sparklines.svg
-          :target: https://travis-ci.org/deeplook/sparklines
-        
-        .. |pypi| image:: https://img.shields.io/pypi/v/sparklines.svg
-          :target: https://pypi.python.org/pypi/sparklines
-        
-        This Python package implements Edward Tufte's concept of sparklines_, but
-        limited to text only e.g. like this: ▃▁▄▁▅█▂▅ (this I likely not displayed
-        correctly in every browser). You can find more information about sparklines
-        `on Wikipedia`_. This code was mainly developed for running simple
-        plausibility tests in sensor networks as shown in fig. 1 below:
-        
-        .. figure:: https://raw.githubusercontent.com/deeplook/sparklines/master/example_sensors.png
-           :width: 75%
-           :alt: example usecase with sensor values
-           :align: center
-        
-           Fig. 1: Example usecase for such "sparklines" on the command-line,
-           showing IoT sensor values (generating code not included here).
-        
-        Due to limitations of available Unicode characters this works best when all
-        values are positive. And even then true sparklines that look more like lines
-        and less like bars are a real challenge, because they would need multiple
-        characters with a single horizontal line on different vertical positions. This
-        would work only with a dedicated font, which is way beyond the scope of this
-        tool and which would significantly complicate its usage. So we stick to these
-        characters: "▁▂▃▄▅▆▇█", and use a blank for missing values.
-        
-        This code was tested ok for Python 2.6 to 2.7 and 3.2 to 3.5.
-        
-        
-        Sample output
-        -------------
-        
-        This is a recorded sample session illustrating how to use ``sparklines`` (as
-        GitHub doesn't render embedded Asciinema_ recordings you'll see here an image
-        pointing to the respective
-        `asciicast <https://asciinema.org/a/5xwfvcrrk09fy3ml3a8n67hep>`_):
-        
-        .. image:: https://asciinema.org/a/5xwfvcrrk09fy3ml3a8n67hep.png
-           :target: https://asciinema.org/a/5xwfvcrrk09fy3ml3a8n67hep
-        
-        Here is some example output on the command-line (please note that in some
-        browsers the vertical alignment of these block characters might be displayed
-        slightly wrong, the same effect can be seen for other repos referenced below):
-        
-        Examples for the code below:
-        
-        .. code-block:: bash
-        
-            $ sparklines 2 7 1 8 2 8 1 8
-            ▂▇▁█▂█▁█
-            $ echo 2 7 1 8 2 8 1 8 | sparklines
-            ▂▇▁█▂█▁█
-            $ sparklines < numbers.txt
-            ▂▇▁█▂█▁█
-            $ sparklines 0 2. 1e0
-            ▁█▅
-        
-        
-        Installation
-        ------------
-        
-        You can install this package using ``pip install sparklines`` from the `Python
-        Package Index`_.
-        You can also clone this repository and install it via ``python setup.py install``
-        or ``pip install -e .``.
-        After installing, you will have access system-wide (or in your virtualenv
-        if you have used that) to ``sparklines``, programmatically as well as via a
-        command-line tool with the same name.
-        
-        Test
-        ----
-        
-        To run the (still very small) "test suite", download and unpack this repository
-        or clone it, and run the command ``python setup.py test`` in the unpacked
-        archive. This will use a minified version of the ``pytest`` package included
-        in this package in the file ``test/runtests.py``. If you have the excellent
-        ``pytest`` package installed you can also run ``py.test test`` from the 
-        downloaded repository's root folder.
-        
-        
-        Usage
-        -----
-        
-        Please note that the samples below might look a little funky (misaligned or 
-        even colored) in some browsers, but it should be totally fine when you print
-        this in your terminal, Python or IPython session or your Python IDE of choice.
-        Figure 2 below might sshow better what you should expect than the copied sample
-        code thereafter:
-        
-        .. figure:: https://raw.githubusercontent.com/deeplook/sparklines/master/example_python.png
-           :width: 65%
-           :alt: example interactive invocation
-           :align: center
-        
-           Fig. 2: Example invocation from a Python and an IPython session.
-        
-        
-        Command-Line
-        ............
-        
-        Here are two sample invocations from the command-line, copied into this README:
-        
-        .. code-block:: console
-        
-            $ sparklines 1 2 3 4 5.0 null 3 2 1
-            ▁▃▅▆█ ▅▃▁
-        
-            $ sparklines -n 2 1 2 3 4 5.0 null 3 2 1
-              ▁▅█ ▁  
-            ▁▅███ █▅▁
-        
-        
-        Programmatic
-        ............
-        
-        And here are sample invocations from interactive Python sessions, copied into
-        this README. The main function to use programmatically is 
-        ``sparklines.sparklines()``:
-        
-        .. code-block:: python
-        
-            In [1]: from sparklines import sparklines
-        
-            In [2]: for line in sparklines([1, 2, 3, 4, 5.0, None, 3, 2, 1]):
-               ...:     print(line)
-               ...:     
-            ▁▃▅▆█ ▅▃▁
-        
-            In [3]: for line in sparklines([1, 2, 3, 4, 5.0, None, 3, 2, 1], num_lines=2):
-                print(line)
-               ...:     
-              ▁▅█ ▁  
-            ▁▅███ █▅▁
-        
-        
-        References
-        ----------
-        
-        This code was inspired by Zach Holman's `spark 
-        <https://github.com/holman/spark>`_, converted to a Python module 
-        by Kenneth Reitz as `spark.py 
-        <https://raw.githubusercontent.com/kennethreitz/spark.py/master/spark.py>`_ 
-        and by RegKrieg to a Python package named `pysparklines <https://github.com/RedKrieg/pysparklines>`_.
-        And Roger Allen provides an even `shorter spark.py 
-        <https://gist.githubusercontent.com/rogerallen/1368454/raw/b17e96b56ae881621a9f3b1508ca2e7fde3ec93e/spark.py>`_.
-        
-        But since it is so short and easy to code in Python we can add a few nice
-        extra features I was missing, like:
-        
-        - increasing resolution with multiple output lines per sparkline
-        - showing gaps in input numbers for missing data
-        - issuing warnings for negative values (allowed, but misleading)
-        - highlighting values exceeding some threshold with a different
-          color (if ``termcolor`` package is available)
-        - wrapping long sparklines at some max. length
-        - (todo) adding separator characters like ``:`` at regular intervals
-        
-        .. _Asciinema: https://asciinema.org
-        .. _Python Package Index: https://pypi.python.org/pypi/sparklines/
-        .. _sparklines: http://www.edwardtufte.com/bboard/q-and-a-fetch-msg?msg_id=0001OR
-        .. _on Wikipedia: https://en.wikipedia.org/wiki/Sparkline
-        
 Keywords: visualization,chart,tool
-Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Other Audience
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+License-File: LICENSE.txt
+
+Sparklines
+==========
+
+.. image:: https://img.shields.io/github/actions/workflow/status/deeplook/sparklines/python-package.yml
+  :target: https://pypi.org/project/sparklines
+
+.. image:: https://img.shields.io/pypi/pyversions/sparklines.svg
+  :target: https://pypi.org/project/sparklines
+  
+.. image:: https://img.shields.io/pypi/v/sparklines.svg
+  :target: https://pypi.org/project/sparklines/
+
+.. image:: https://static.pepy.tech/badge/sparklines/month
+  :target: https://pepy.tech/project/sparklines
+
+.. image:: https://img.shields.io/pypi/status/sparklines.svg
+  :target: https://pypi.org/project/sparklines
+
+.. image:: https://img.shields.io/pypi/format/sparklines.svg
+  :target: https://pypi.org/project/sparklines
+
+.. image:: https://img.shields.io/pypi/l/sparklines.svg
+  :target: https://pypi.org/project/sparklines
+  
+This Python package implements Edward Tufte's concept of sparklines_, but
+limited to text only e.g. like this: ▃▁▄▁▅█▂▅ (this I likely not displayed
+correctly in every browser). You can find more information about sparklines
+`on Wikipedia`_. This code was mainly developed for running simple
+plausibility tests in sensor networks as shown in fig. 1 below:
+
+.. figure:: https://raw.githubusercontent.com/deeplook/sparklines/main/example_sensors.png
+   :width: 75%
+   :alt: example usecase with sensor values
+   :align: center
+
+   Fig. 1: Example usecase for such "sparklines" on the command-line,
+   showing IoT sensor values (generating code not included here).
+
+Due to limitations of available Unicode characters this works best when all
+values are positive. And even then true sparklines that look more like lines
+and less like bars are a real challenge, because they would need multiple
+characters with a single horizontal line on different vertical positions. This
+would work only with a dedicated font, which is way beyond the scope of this
+tool and which would significantly complicate its usage. So we stick to these
+characters: "▁▂▃▄▅▆▇█", and use a blank for missing values.
+
+This code was tested ok at some point for Python 2.6 and 2.7, but no longer
+supports Python 2 after it reached end-of-life. Now Python 3.5 to 3.8 as well
+as PyPy 3 are all tested via Travis-CI.
+
+
+Sample output
+-------------
+
+This is a recorded sample session illustrating how to use ``sparklines`` (as
+GitHub doesn't render embedded Asciinema_ recordings you'll see here an image
+pointing to the respective
+`asciicast <https://asciinema.org/a/5xwfvcrrk09fy3ml3a8n67hep>`_):
+
+.. image:: https://asciinema.org/a/5xwfvcrrk09fy3ml3a8n67hep.png
+   :target: https://asciinema.org/a/5xwfvcrrk09fy3ml3a8n67hep
+
+Here is some example output on the command-line (please note that in some
+browsers the vertical alignment of these block characters might be displayed
+slightly wrong, the same effect can be seen for other repos referenced below):
+
+Examples for the code below:
+
+.. code-block:: bash
+
+    $ sparklines 2 7 1 8 2 8 1 8
+    ▂▇▁█▂█▁█
+    $ echo 2 7 1 8 2 8 1 8 | sparklines
+    ▂▇▁█▂█▁█
+    $ sparklines < numbers.txt
+    ▂▇▁█▂█▁█
+    $ sparklines 0 2. 1e0
+    ▁█▅
+
+
+Installation
+------------
+
+You can install this package using ``pip install sparklines`` from the `Python
+Package Index`_.
+You can also clone this repository and install it via ``python setup.py install``
+or ``pip install -e .``.
+After installing, you will have access system-wide (or in your virtualenv
+if you have used that) to ``sparklines``, programmatically as well as via a
+command-line tool with the same name.
+
+Test
+----
+
+To run the test suite, download and unpack this repository or clone it,
+run `pip inastall pytest`, and run the command ``pytest tests`` in the
+unpacked archive. from the downloaded repository's root folder.
+
+
+Usage
+-----
+
+Please note that the samples below might look a little funky (misaligned or 
+even colored) in some browsers, but it should be totally fine when you print
+this in your terminal, Python or IPython session or your Python IDE of choice.
+Figure 2 below might show better what you should expect than the copied sample
+code thereafter:
+
+.. figure:: https://raw.githubusercontent.com/deeplook/sparklines/main/example_python.png
+   :width: 65%
+   :alt: example interactive invocation
+   :align: center
+
+   Fig. 2: Example invocation from a Python and an IPython session.
+
+
+Command-Line
+............
+
+Here are two sample invocations from the command-line, copied into this README:
+
+.. code-block:: console
+
+    $ sparklines 1 2 3 4 5.0 null 3 2 1
+    ▁▃▅▆█ ▅▃▁
+
+    $ sparklines -n 2 1 2 3 4 5.0 null 3 2 1
+      ▁▅█ ▁  
+    ▁▅███ █▅▁
+
+
+Programmatic
+............
+
+And here are sample invocations from interactive Python sessions, copied into
+this README. The main function to use programmatically is 
+``sparklines.sparklines()``:
+
+.. code-block:: python
+
+    In [1]: from sparklines import sparklines
+
+    In [2]: for line in sparklines([1, 2, 3, 4, 5.0, None, 3, 2, 1]):
+       ...:     print(line)
+       ...:     
+    ▁▃▅▆█ ▅▃▁
+
+    In [3]: for line in sparklines([1, 2, 3, 4, 5.0, None, 3, 2, 1], num_lines=2):
+        print(line)
+       ...:     
+      ▁▅█ ▁  
+    ▁▅███ █▅▁
+
+
+References
+----------
+
+This code was inspired by Zach Holman's `spark 
+<https://github.com/holman/spark>`_, converted to a Python module 
+by Kenneth Reitz as `spark.py 
+<https://raw.githubusercontent.com/kennethreitz/spark.py/master/spark.py>`_ 
+and by RegKrieg to a Python package named `pysparklines <https://github.com/RedKrieg/pysparklines>`_.
+And Roger Allen provides an even `shorter spark.py 
+<https://gist.githubusercontent.com/rogerallen/1368454/raw/b17e96b56ae881621a9f3b1508ca2e7fde3ec93e/spark.py>`_.
+
+But since it is so short and easy to code in Python we can add a few nice
+extra features I was missing, like:
+
+- increasing resolution with multiple output lines per sparkline
+- showing gaps in input numbers for missing data
+- issuing warnings for negative values (allowed, but misleading)
+- highlighting values exceeding some threshold with a different
+  color (if ``termcolor`` package is available)
+- wrapping long sparklines at some max. length
+- (todo) adding separator characters like ``:`` at regular intervals
+
+.. _Asciinema: https://asciinema.org
+.. _Python Package Index: https://pypi.python.org/pypi/sparklines/
+.. _sparklines: http://www.edwardtufte.com/bboard/q-and-a-fetch-msg?msg_id=0001OR
+.. _on Wikipedia: https://en.wikipedia.org/wiki/Sparkline
```

### Comparing `sparklines-0.4.2/test/test_sparkline.py` & `sparklines-0.5.0/tests/test_sparkline.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,222 +1,229 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 """
 Run from the root folder with either 'python setup.py test' or
 'py.test test/test_sparkline.py'.
 """
 
-from __future__ import print_function, unicode_literals
-
 import os
 import re
 
 import pytest
 
 from sparklines import batch, scale_values, sparklines, demo
 from sparklines.__main__ import test_valid_number as is_valid_number
 
 
 def strip_ansi(text):
+    """Remove ANSI escape sequences from a text."""
     # http://stackoverflow.com/questions/14693701/how-can-i-remove-the-ansi-escape-sequences-from-a-string-in-python#14693789
-    ansi_escape = re.compile(r'\x1b[^m]*m')
-    return ansi_escape.sub('', text)
+    ansi_escape = re.compile(r"\x1b[^m]*m")
+    return ansi_escape.sub("", text)
 
 
 def test_parse_float():
-    "Test parsing input numbers."
+    """Test parsing input numbers."""
 
     t = is_valid_number
 
-    assert t('4.5') == '4.5'
-    assert t('-4.5') == '-4.5'
-    assert t('4.') == '4.'
-    assert t('.5') == '.5'
-    assert t('4.5e0') == '4.5e0'
-    assert t('-4.5e0') == '-4.5e0'
-    assert t('-4.5e-2') == '-4.5e-2'
-    assert t('-.5e-2') == '-.5e-2'
-
-    assert t('4.5,') == '4.5'
-    assert t('4.5;') == '4.5'
-    assert t('"4.5"') == '4.5'
-    assert t('(4.5)') == '4.5'
-
-    assert t('null') == 'null'
-    assert t('Null') == 'null'
-    assert t('none') == 'none'
-    assert t('None') == 'none'
+    assert t("4.5") == "4.5"
+    assert t("-4.5") == "-4.5"
+    assert t("4.") == "4."
+    assert t(".5") == ".5"
+    assert t("4.5e0") == "4.5e0"
+    assert t("-4.5e0") == "-4.5e0"
+    assert t("-4.5e-2") == "-4.5e-2"
+    assert t("-.5e-2") == "-.5e-2"
+
+    assert t("4.5,") == "4.5"
+    assert t("4.5;") == "4.5"
+    assert t('"4.5"') == "4.5"
+    assert t("(4.5)") == "4.5"
+
+    assert t("null") == "null"
+    assert t("Null") == "null"
+    assert t("none") == "none"
+    assert t("None") == "none"
 
-    assert t('None,') == 'none'
+    assert t("None,") == "none"
 
     with pytest.raises(ValueError):
-        t(',')
+        t(",")
     with pytest.raises(ValueError):
-        t('invalid')
+        t("invalid")
 
 
 def test_scale0():
-    "Test scale..."
+    """Test scale..."""
 
     res = scale_values([1, 2, 3])
-    exp = [1., 4., 8.]
+    exp = [1.0, 4.0, 8.0]
     assert res == exp
 
 
 def test_scale1():
-    "Test scale..."
+    """Test scale..."""
 
     res = scale_values([1, 2, 3], num_lines=2)
-    exp = [1., 8., 16.]
+    exp = [1.0, 8.0, 16.0]
     assert res == exp
 
 
 def test_batch():
     batches = batch(3, range(10))
     assert batches == [[0, 1, 2], [3, 4, 5], [6, 7, 8], [9]], batches
 
     batches = batch(None, range(3))
     assert batches == [[0, 1, 2]]
 
 
 def test_scale_pi():
-    "Test scale Pi."
+    """Test scale Pi."""
 
     res = scale_values([3, 1, 4, 1, 5, 9, 2, 6])
     exp = [3, 1, 4, 1, 4, 8, 2, 5]
     assert res == exp
 
 
 def test_pi():
-    "Test first eight digits of Pi."
+    """Test first eight digits of Pi."""
 
     res = sparklines([3, 1, 4, 1, 5, 9, 2, 6])
-    exp = ['▃▁▄▁▄█▂▅']
+    exp = ["▃▁▄▁▄█▂▅"]
     assert res == exp
 
 
 def test_minmax():
-    "Test two values, min and max."
+    """Test two values, min and max."""
 
     res = sparklines([1, 8])
-    exp = ['▁█'] # 1, 8
+    exp = ["▁█"]  # 1, 8
     assert res == exp
 
 
 def test_rounding0():
-    "Test two values, min and max."
+    """Test two values, min and max."""
 
     res = sparklines([1, 5, 8])
-    exp = ['▁▅█'] # 1, 5, 8
+    exp = ["▁▅█"]  # 1, 5, 8
     assert res == exp
 
+
 def test_maximum():
     res = sparklines([1, 2, 3, 10, 10], maximum=3)
-    exp = ['▁▄███']
+    exp = ["▁▄███"]
     assert res == exp
 
+
 def test_maximum_internal_consistency():
     res = sparklines([1, 2, 3, 10, 10, 1], maximum=3)
     exp = sparklines([1, 2, 3, 3, 3, 1], maximum=3)
     assert res == exp
 
 
 def test_minimum():
     res = sparklines([0, 0, 11, 12, 13], minimum=10)
-    exp = ['▁▁▃▆█']
+    exp = ["▁▁▃▆█"]
     assert res == exp
 
+
 def test_minimum_internal_consistency():
     res = sparklines([0, 0, 11, 12, 13], minimum=10)
     exp = sparklines([10, 10, 11, 12, 13], minimum=10)
     assert res == exp
 
+
 def test1():
-    "Test single values all have the same four pixel high output character."
+    """Test single values all have the same four pixel high output character."""
 
     for i in range(10):
         res = sparklines([i])
-        exp = ['▄']
+        exp = ["▄"]
         assert res == exp
 
 
 def test_empty():
-    "Make sure degenerate cases don't fail"
+    """Make sure degenerate cases don't fail."""
+
     res = sparklines([])
-    exp = ['']
+    exp = [""]
     # Produces an empty line from the command line
     #   we might prefer empty output
     assert res == exp
 
 
 def test_multiline():
     res = sparklines([1, 5, 8], num_lines=3)
-    exp = [
-        "  █",
-        " ▆█",
-        "▁██"]
+    exp = ["  █", " ▆█", "▁██"]
     assert res == exp
 
 
 def test_wrap():
-    res = sparklines([1,2, 3, 1, 2, 3, 1, 2], wrap=3)
+    res = sparklines([1, 2, 3, 1, 2, 3, 1, 2], wrap=3)
     exp = ["▁▄█", "", "▁▄█", "", "▁▄"]
     assert res == exp
 
 
 def test_wrap_scale():
     res = sparklines([100, 50, 100, 20, 50, 20, 1, 1, 1], wrap=3)
     exp = ["█▄█", "", "▂▄▂", "", "▁▁▁"]
     assert res == exp
 
 
 def test_wrap_consistency():
-    res = sparklines([1,2, 3, 1, 2, 3, 1, 2], wrap=3)
+    res = sparklines([1, 2, 3, 1, 2, 3, 1, 2], wrap=3)
     exp = (
         sparklines([1, 2, 3], maximum=3, minimum=1)
-        + ['']
+        + [""]
         + sparklines([1, 2, 3], maximum=3, minimum=1)
-        + ['']
-        + sparklines([1, 2], maximum=3, minimum=1))
+        + [""]
+        + sparklines([1, 2], maximum=3, minimum=1)
+    )
     assert res == exp
 
 
 def test_wrap_escaping_consistency():
-    no_emph = sparklines([1,2, 3, 1, 2, 3, 1, 2], wrap=3)
-    stripped_emph = map(strip_ansi, sparklines([1,2, 3, 1, 2, 3, 1, 2], wrap=3, emph=['green:le:1.0']))
+    no_emph = sparklines([1, 2, 3, 1, 2, 3, 1, 2], wrap=3)
+    stripped_emph = map(
+        strip_ansi, sparklines([1, 2, 3, 1, 2, 3, 1, 2], wrap=3, emph=["green:le:1.0"])
+    )
     assert no_emph == list(stripped_emph)
 
 
 def _test_wrap_escaping():
-    res = sparklines([1, 10, 1, 10, 1, 10], emph=['green:ge:2.0'], wrap=3)
-    exp = ["\x1b[37m▁\x1b[0m\x1b[32m█\x1b[0m\x1b[37m▁\x1b[0m", "", "\x1b[32m█\x1b[0m\x1b[37m▁\x1b[0m\x1b[32m█\x1b[0m"]
+    res = sparklines([1, 10, 1, 10, 1, 10], emph=["green:ge:2.0"], wrap=3)
+    exp = [
+        "\x1b[37m▁\x1b[0m\x1b[32m█\x1b[0m\x1b[37m▁\x1b[0m",
+        "",
+        "\x1b[32m█\x1b[0m\x1b[37m▁\x1b[0m\x1b[32m█\x1b[0m",
+    ]
     assert exp == res, (exp, res)
 
 
 def test_gaps():
     res = sparklines([1, None, 1, 2])
     exp = ["▁ ▁█"]
     assert exp == res
     res = sparklines([1, None, 1])
     exp = ["▄ ▄"]
     assert exp == res, (exp, res)
 
 
 def test_demo_consistency():
     ## todo: remove encoding hacks
-    toplevel = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
-    with open(os.path.join(toplevel, 'test', 'demo-output')) as stream:
+    toplevel = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
+    with open(os.path.join(toplevel, "tests", "demo-output")) as stream:
         exp = stream.read()
         try:
-            exp = exp.decode('utf8')
+            exp = exp.decode("utf8")
         except AttributeError:
             pass
     res = demo([])
 
-    with open('/tmp/blah', 'w') as stream:
+    with open("/tmp/blah", "w") as stream:
         try:
-            stream.write(res) # .encode('utf8'))
+            stream.write(res)  # .encode('utf8'))
         except UnicodeEncodeError:
-            stream.write(res.encode('utf8'))
+            stream.write(res.encode("utf8"))
 
-    assert exp == res, 'Demo output has changed. Verify it and update demo-output!'
+    assert exp == res, "Demo output has changed. Verify it and update demo-output!"
```

