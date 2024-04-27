# Comparing `tmp/lektor-chameleon-0.7.tar.gz` & `tmp/lektor_chameleon-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lektor-chameleon-0.7.tar", last modified: Thu Jun 29 18:21:23 2023, max compression
+gzip compressed data, was "lektor_chameleon-0.8.tar", last modified: Sat Apr 27 19:46:38 2024, max compression
```

## Comparing `lektor-chameleon-0.7.tar` & `lektor_chameleon-0.8.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-06-29 18:21:23.395638 lektor-chameleon-0.7/
--rw-------   0 uyar      (1000) uyar      (1000)     1496 2023-06-29 18:01:38.000000 lektor-chameleon-0.7/LICENSE.txt
--rw-------   0 uyar      (1000) uyar      (1000)     4181 2023-06-29 18:21:23.391638 lektor-chameleon-0.7/PKG-INFO
--rw-------   0 uyar      (1000) uyar      (1000)     1486 2023-06-29 18:07:38.000000 lektor-chameleon-0.7/README.rst
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-06-29 18:21:23.391638 lektor-chameleon-0.7/lektor_chameleon/
--rw-------   0 uyar      (1000) uyar      (1000)     3156 2023-06-29 18:14:47.000000 lektor-chameleon-0.7/lektor_chameleon/__init__.py
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-06-29 18:21:23.391638 lektor-chameleon-0.7/lektor_chameleon.egg-info/
--rw-------   0 uyar      (1000) uyar      (1000)     4181 2023-06-29 18:21:23.000000 lektor-chameleon-0.7/lektor_chameleon.egg-info/PKG-INFO
--rw-------   0 uyar      (1000) uyar      (1000)      308 2023-06-29 18:21:23.000000 lektor-chameleon-0.7/lektor_chameleon.egg-info/SOURCES.txt
--rw-------   0 uyar      (1000) uyar      (1000)        1 2023-06-29 18:21:23.000000 lektor-chameleon-0.7/lektor_chameleon.egg-info/dependency_links.txt
--rw-------   0 uyar      (1000) uyar      (1000)       62 2023-06-29 18:21:23.000000 lektor-chameleon-0.7/lektor_chameleon.egg-info/entry_points.txt
--rw-------   0 uyar      (1000) uyar      (1000)       79 2023-06-29 18:21:23.000000 lektor-chameleon-0.7/lektor_chameleon.egg-info/requires.txt
--rw-------   0 uyar      (1000) uyar      (1000)       17 2023-06-29 18:21:23.000000 lektor-chameleon-0.7/lektor_chameleon.egg-info/top_level.txt
--rw-------   0 uyar      (1000) uyar      (1000)     1377 2023-06-29 18:04:25.000000 lektor-chameleon-0.7/pyproject.toml
--rw-------   0 uyar      (1000) uyar      (1000)       38 2023-06-29 18:21:23.395638 lektor-chameleon-0.7/setup.cfg
+drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-04-27 19:46:38.594599 lektor_chameleon-0.8/
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     1496 2024-04-27 16:35:46.000000 lektor_chameleon-0.8/LICENSE.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     4072 2024-04-27 19:46:38.594599 lektor_chameleon-0.8/PKG-INFO
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     1130 2024-04-27 19:18:39.000000 lektor_chameleon-0.8/README.rst
+drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-04-27 19:46:38.594599 lektor_chameleon-0.8/lektor_chameleon.egg-info/
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     4072 2024-04-27 19:46:38.000000 lektor_chameleon-0.8/lektor_chameleon.egg-info/PKG-INFO
+-rw-r--r--   0 uyar      (1000) uyar      (1000)      323 2024-04-27 19:46:38.000000 lektor_chameleon-0.8/lektor_chameleon.egg-info/SOURCES.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)        1 2024-04-27 19:46:38.000000 lektor_chameleon-0.8/lektor_chameleon.egg-info/dependency_links.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)       62 2024-04-27 19:46:38.000000 lektor_chameleon-0.8/lektor_chameleon.egg-info/entry_points.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)      100 2024-04-27 19:46:38.000000 lektor_chameleon-0.8/lektor_chameleon.egg-info/requires.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)       17 2024-04-27 19:46:38.000000 lektor_chameleon-0.8/lektor_chameleon.egg-info/top_level.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     2920 2024-04-27 19:18:39.000000 lektor_chameleon-0.8/lektor_chameleon.py
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     1964 2024-04-27 16:45:38.000000 lektor_chameleon-0.8/pyproject.toml
+-rw-r--r--   0 uyar      (1000) uyar      (1000)       38 2024-04-27 19:46:38.594599 lektor_chameleon-0.8/setup.cfg
+drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-04-27 19:46:38.594599 lektor_chameleon-0.8/tests/
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     1885 2024-04-27 19:18:39.000000 lektor_chameleon-0.8/tests/test_chameleon.py
```

### Comparing `lektor-chameleon-0.7/LICENSE.txt` & `lektor_chameleon-0.8/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2018-2023 H. Turgut Uyar <uyar@tekir.org>
+Copyright 2018-2024 H. Turgut Uyar <uyar@tekir.org>
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
```

### Comparing `lektor-chameleon-0.7/PKG-INFO` & `lektor_chameleon-0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lektor-chameleon
-Version: 0.7
+Version: 0.8
 Summary: Chameleon template support for Lektor.
 Author-email: "H. Turgut Uyar" <uyar@tekir.org>
-License: Copyright 2018-2023 H. Turgut Uyar <uyar@tekir.org>
+License: Copyright 2018-2024 H. Turgut Uyar <uyar@tekir.org>
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice,
            this list of conditions and the following disclaimer.
         
@@ -33,54 +33,48 @@
 Project-URL: repository, https://github.com/uyar/lektor-chameleon
 Keywords: lektor,plugin,chameleon,template
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Framework :: Lektor
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+Requires-Dist: lektor
+Requires-Dist: chameleon
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
 Provides-Extra: style
+Requires-Dist: ruff; extra == "style"
 Provides-Extra: dev
-License-File: LICENSE.txt
+Requires-Dist: lektor-chameleon[style,tests]; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: tox; extra == "dev"
 
 lektor-chameleon
 ================
 
 lektor-chameleon is a plugin for the `Lektor <https://www.getlektor.com>`_
 static site generator
 that makes is possible to write the templates
 using the `Chameleon <https://chameleon.readthedocs.io/>`_ template engine.
 
 To use the plugin, add it to your project::
 
   lektor plugin add lektor-chameleon
 
-Since the plugin modifies the default environment,
-it requires that it will be explicitly enabled.
-To enable the plugin, create the file ``configs/chameleon.ini``
-and put the following lines into it::
-
-  [chameleon]
-  enabled = yes
-
-If you don't want to use the ".html" extension for your template files,
-you can set a different one in the configuration::
-
-  [chameleon]
-  enabled = yes
-  file_ext = .pt
+Templates must have the ``.pt`` file extension.
 
 Usage examples:
 
 .. code:: html
 
    <html lang="${this.alt}">
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: lektor-chameleon Version: 0.7 Summary: Chameleon
+Metadata-Version: 2.1 Name: lektor-chameleon Version: 0.8 Summary: Chameleon
 template support for Lektor. Author-email: "H. Turgut Uyar"
-tekir.org> License: Copyright 2018-2023 H. Turgut Uyar
+tekir.org> License: Copyright 2018-2024 H. Turgut Uyar
 tekir.org> Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
 following disclaimer in the documentation and/or other materials provided with
 the distribution. 3. Neither the name of the copyright holder nor the names of
@@ -20,32 +20,30 @@
 LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. Project-URL: repository, https://
 github.com/uyar/lektor-chameleon Keywords: lektor,plugin,chameleon,template
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Plugins
 Classifier: Framework :: Lektor Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Internet
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management Requires-Python:
-~=3.8 Description-Content-Type: text/x-rst Provides-Extra: style Provides-
-Extra: dev License-File: LICENSE.txt lektor-chameleon ================ lektor-
-chameleon is a plugin for the `Lektor
+~=3.8 Description-Content-Type: text/x-rst License-File: LICENSE.txt Requires-
+Dist: lektor Requires-Dist: chameleon Provides-Extra: tests Requires-Dist:
+pytest; extra == "tests" Provides-Extra: style Requires-Dist: ruff; extra ==
+"style" Provides-Extra: dev Requires-Dist: lektor-chameleon[style,tests]; extra
+== "dev" Requires-Dist: build; extra == "dev" Requires-Dist: twine; extra ==
+"dev" Requires-Dist: tox; extra == "dev" lektor-chameleon ================
+lektor-chameleon is a plugin for the `Lektor
 www.getlektor.com>`_ static site generator that makes is possible to write the
 templates using the `Chameleon
 chameleon.readthedocs.io/>`_ template engine. To use the plugin, add it to your
-project:: lektor plugin add lektor-chameleon Since the plugin modifies the
-default environment, it requires that it will be explicitly enabled. To enable
-the plugin, create the file ``configs/chameleon.ini`` and put the following
-lines into it:: [chameleon] enabled = yes If you don't want to use the ".html"
-extension for your template files, you can set a different one in the
-configuration:: [chameleon] enabled = yes file_ext = .pt Usage examples: ..
-code:: html
+project:: lektor plugin add lektor-chameleon Templates must have the ``.pt``
+file extension. Usage examples: .. code:: html
 ************ PPaaggee ttiittllee ************
 message Many Lektor and Jinja filters are available using the ``>>`` operator:
 .. code:: html _H_o_m_e_ _p_a_g_e
 Filters also accept parameters: .. code:: html _l_i_n_k_ _t_e_x_t But filter parameters
 must be given as keyword parameters: .. code:: html
 Page body
 Page body
```

### Comparing `lektor-chameleon-0.7/README.rst` & `lektor_chameleon-0.8/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,15 @@
 that makes is possible to write the templates
 using the `Chameleon <https://chameleon.readthedocs.io/>`_ template engine.
 
 To use the plugin, add it to your project::
 
   lektor plugin add lektor-chameleon
 
-Since the plugin modifies the default environment,
-it requires that it will be explicitly enabled.
-To enable the plugin, create the file ``configs/chameleon.ini``
-and put the following lines into it::
-
-  [chameleon]
-  enabled = yes
-
-If you don't want to use the ".html" extension for your template files,
-you can set a different one in the configuration::
-
-  [chameleon]
-  enabled = yes
-  file_ext = .pt
+Templates must have the ``.pt`` file extension.
 
 Usage examples:
 
 .. code:: html
 
    <html lang="${this.alt}">
```

#### html2text {}

```diff
@@ -1,18 +1,13 @@
 lektor-chameleon ================ lektor-chameleon is a plugin for the `Lektor
 www.getlektor.com>`_ static site generator that makes is possible to write the
 templates using the `Chameleon
 chameleon.readthedocs.io/>`_ template engine. To use the plugin, add it to your
-project:: lektor plugin add lektor-chameleon Since the plugin modifies the
-default environment, it requires that it will be explicitly enabled. To enable
-the plugin, create the file ``configs/chameleon.ini`` and put the following
-lines into it:: [chameleon] enabled = yes If you don't want to use the ".html"
-extension for your template files, you can set a different one in the
-configuration:: [chameleon] enabled = yes file_ext = .pt Usage examples: ..
-code:: html
+project:: lektor plugin add lektor-chameleon Templates must have the ``.pt``
+file extension. Usage examples: .. code:: html
 ************ PPaaggee ttiittllee ************
 message Many Lektor and Jinja filters are available using the ``>>`` operator:
 .. code:: html _H_o_m_e_ _p_a_g_e
 Filters also accept parameters: .. code:: html _l_i_n_k_ _t_e_x_t But filter parameters
 must be given as keyword parameters: .. code:: html
 Page body
 Page body
```

### Comparing `lektor-chameleon-0.7/lektor_chameleon/__init__.py` & `lektor_chameleon-0.8/lektor_chameleon.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-# Copyright (C) 2018-2023 H. Turgut Uyar <uyar@tekir.org>
+# Copyright (C) 2018-2024 H. Turgut Uyar <uyar@tekir.org>
 #
 # lektor-chameleon is released under the BSD license.
 # Read the included LICENSE.txt file for details.
 
+__version__ = "0.8"
+
 from functools import partial
 
 from chameleon import PageTemplateLoader
 from chameleon.loader import TemplateLoader
 from lektor.context import get_ctx
 from lektor.pluginsystem import Plugin
+from lektor.reporter import reporter
 from markupsafe import Markup
 
 
 _CONTEXT_FILTERS = {
     "url", "asseturl", "markdown",
 }
 
@@ -45,56 +48,44 @@
 
 
 chameleon_load = TemplateLoader.load
 
 
 def load_template(self, filename, *args, **kwargs):
     ctx = get_ctx()
-    pt_ext = self.__class__.file_ext
-    if (pt_ext is not None) and \
-            (filename == ctx.source.datamodel.id + ".html"):
-        filename = ctx.source.datamodel.id + pt_ext
+    if filename == ctx.source.datamodel.id + ".html":
+        filename = ctx.source.datamodel.id + ".pt"
     template = chameleon_load(self, filename, *args, **kwargs)
     ctx.record_dependency(template.filename)
     return template
 
 
 def render_template(self, name, pad=None, this=None, values=None, alt=None):
     if isinstance(name, list):
         name = name[0]
     ctx = self.make_default_tmpl_values(pad, this, values, alt, template=name)
-    ctx.update(self.jinja_env.globals)
-    for f_name, f_filter in self.chameleon_filters.items():
+    ctx.update(self.chameleon_env.globals)
+    for f_name, f_filter in self.chameleon_env.filters.items():
         ctx[f_name] = f_filter(ctx) if f_filter.ctx else f_filter
-    template = self.chameleon_loader.load(name)
+    template = self.chameleon_env.loader.load(name)
     return template(**ctx)
 
 
+class ChameleonEnvironment:
+    def __init__(self, jinja_env) -> None:
+        self.loader = PageTemplateLoader(jinja_env.loader.searchpath,
+                                         auto_reload=True)
+        self.globals = jinja_env.globals
+        self.filters = {n: Filter(n, f) for n, f in jinja_env.filters.items()}
+        for f_name in _JINJA_ENV_FILTERS:
+            self.filters[f_name] = self.filters[f_name](jinja_env)
+
+
 class ChameleonPlugin(Plugin):
     name = "chameleon"
     description = "Chameleon support for templating"
 
-    def __init__(self, *args, **kwargs):
-        Plugin.__init__(self, *args, **kwargs)
-
-        config = self.get_config()
-        self.enabled = config.get_bool("chameleon.enabled", False)
-
-        if self.enabled:
-            TemplateLoader.file_ext = config.get("chameleon.file_ext")
-            TemplateLoader.load = load_template
-
     def on_setup_env(self, **extra):
-        if not self.enabled:
-            return
-
-        template_paths = self.env.jinja_env.loader.searchpath
-        self.env.chameleon_loader = PageTemplateLoader(template_paths,
-                                                       auto_reload=True)
-
-        filters = {n: Filter(n, f)
-                   for n, f in self.env.jinja_env.filters.items()}
-        for f_name in _JINJA_ENV_FILTERS:
-            filters[f_name] = filters[f_name](self.env.jinja_env)
-        self.env.chameleon_filters = filters
-
+        reporter.report_generic("Setting up to use Chameleon templates")
+        TemplateLoader.load = load_template
         self.env.__class__.render_template = render_template
+        self.env.chameleon_env = ChameleonEnvironment(self.env.jinja_env)
```

### Comparing `lektor-chameleon-0.7/lektor_chameleon.egg-info/PKG-INFO` & `lektor_chameleon-0.8/lektor_chameleon.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lektor-chameleon
-Version: 0.7
+Version: 0.8
 Summary: Chameleon template support for Lektor.
 Author-email: "H. Turgut Uyar" <uyar@tekir.org>
-License: Copyright 2018-2023 H. Turgut Uyar <uyar@tekir.org>
+License: Copyright 2018-2024 H. Turgut Uyar <uyar@tekir.org>
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice,
            this list of conditions and the following disclaimer.
         
@@ -33,54 +33,48 @@
 Project-URL: repository, https://github.com/uyar/lektor-chameleon
 Keywords: lektor,plugin,chameleon,template
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Framework :: Lektor
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+Requires-Dist: lektor
+Requires-Dist: chameleon
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
 Provides-Extra: style
+Requires-Dist: ruff; extra == "style"
 Provides-Extra: dev
-License-File: LICENSE.txt
+Requires-Dist: lektor-chameleon[style,tests]; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: tox; extra == "dev"
 
 lektor-chameleon
 ================
 
 lektor-chameleon is a plugin for the `Lektor <https://www.getlektor.com>`_
 static site generator
 that makes is possible to write the templates
 using the `Chameleon <https://chameleon.readthedocs.io/>`_ template engine.
 
 To use the plugin, add it to your project::
 
   lektor plugin add lektor-chameleon
 
-Since the plugin modifies the default environment,
-it requires that it will be explicitly enabled.
-To enable the plugin, create the file ``configs/chameleon.ini``
-and put the following lines into it::
-
-  [chameleon]
-  enabled = yes
-
-If you don't want to use the ".html" extension for your template files,
-you can set a different one in the configuration::
-
-  [chameleon]
-  enabled = yes
-  file_ext = .pt
+Templates must have the ``.pt`` file extension.
 
 Usage examples:
 
 .. code:: html
 
    <html lang="${this.alt}">
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: lektor-chameleon Version: 0.7 Summary: Chameleon
+Metadata-Version: 2.1 Name: lektor-chameleon Version: 0.8 Summary: Chameleon
 template support for Lektor. Author-email: "H. Turgut Uyar"
-tekir.org> License: Copyright 2018-2023 H. Turgut Uyar
+tekir.org> License: Copyright 2018-2024 H. Turgut Uyar
 tekir.org> Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
 following disclaimer in the documentation and/or other materials provided with
 the distribution. 3. Neither the name of the copyright holder nor the names of
@@ -20,32 +20,30 @@
 LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. Project-URL: repository, https://
 github.com/uyar/lektor-chameleon Keywords: lektor,plugin,chameleon,template
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Plugins
 Classifier: Framework :: Lektor Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Internet
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management Requires-Python:
-~=3.8 Description-Content-Type: text/x-rst Provides-Extra: style Provides-
-Extra: dev License-File: LICENSE.txt lektor-chameleon ================ lektor-
-chameleon is a plugin for the `Lektor
+~=3.8 Description-Content-Type: text/x-rst License-File: LICENSE.txt Requires-
+Dist: lektor Requires-Dist: chameleon Provides-Extra: tests Requires-Dist:
+pytest; extra == "tests" Provides-Extra: style Requires-Dist: ruff; extra ==
+"style" Provides-Extra: dev Requires-Dist: lektor-chameleon[style,tests]; extra
+== "dev" Requires-Dist: build; extra == "dev" Requires-Dist: twine; extra ==
+"dev" Requires-Dist: tox; extra == "dev" lektor-chameleon ================
+lektor-chameleon is a plugin for the `Lektor
 www.getlektor.com>`_ static site generator that makes is possible to write the
 templates using the `Chameleon
 chameleon.readthedocs.io/>`_ template engine. To use the plugin, add it to your
-project:: lektor plugin add lektor-chameleon Since the plugin modifies the
-default environment, it requires that it will be explicitly enabled. To enable
-the plugin, create the file ``configs/chameleon.ini`` and put the following
-lines into it:: [chameleon] enabled = yes If you don't want to use the ".html"
-extension for your template files, you can set a different one in the
-configuration:: [chameleon] enabled = yes file_ext = .pt Usage examples: ..
-code:: html
+project:: lektor plugin add lektor-chameleon Templates must have the ``.pt``
+file extension. Usage examples: .. code:: html
 ************ PPaaggee ttiittllee ************
 message Many Lektor and Jinja filters are available using the ``>>`` operator:
 .. code:: html _H_o_m_e_ _p_a_g_e
 Filters also accept parameters: .. code:: html _l_i_n_k_ _t_e_x_t But filter parameters
 must be given as keyword parameters: .. code:: html
 Page body
 Page body
```

