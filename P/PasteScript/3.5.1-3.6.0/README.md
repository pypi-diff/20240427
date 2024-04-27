# Comparing `tmp/PasteScript-3.5.1.tar.gz` & `tmp/PasteScript-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PasteScript-3.5.1.tar", last modified: Fri Mar 15 16:32:12 2024, max compression
+gzip compressed data, was "PasteScript-3.6.0.tar", last modified: Sat Apr 27 12:05:26 2024, max compression
```

## Comparing `PasteScript-3.5.1.tar` & `PasteScript-3.6.0.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.383965 PasteScript-3.5.1/
--rw-r--r--   0 cdent      (503) staff       (20)      536 2021-04-27 13:47:08.000000 PasteScript-3.5.1/AUTHORS
--rw-r--r--   0 cdent      (503) staff       (20)      403 2021-04-27 13:47:08.000000 PasteScript-3.5.1/MANIFEST.in
--rw-r--r--   0 cdent      (503) staff       (20)     2384 2024-03-15 16:32:12.383803 PasteScript-3.5.1/PKG-INFO
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.383074 PasteScript-3.5.1/PasteScript.egg-info/
--rw-r--r--   0 cdent      (503) staff       (20)     2384 2024-03-15 16:32:12.000000 PasteScript-3.5.1/PasteScript.egg-info/PKG-INFO
--rw-r--r--   0 cdent      (503) staff       (20)     2893 2024-03-15 16:32:12.000000 PasteScript-3.5.1/PasteScript.egg-info/SOURCES.txt
--rw-r--r--   0 cdent      (503) staff       (20)        1 2024-03-15 16:32:12.000000 PasteScript-3.5.1/PasteScript.egg-info/dependency_links.txt
--rw-r--r--   0 cdent      (503) staff       (20)     2197 2024-03-15 16:32:12.000000 PasteScript-3.5.1/PasteScript.egg-info/entry_points.txt
--rw-r--r--   0 cdent      (503) staff       (20)        6 2024-03-15 16:32:12.000000 PasteScript-3.5.1/PasteScript.egg-info/namespace_packages.txt
--rw-r--r--   0 cdent      (503) staff       (20)        1 2021-04-27 13:47:15.000000 PasteScript-3.5.1/PasteScript.egg-info/not-zip-safe
--rw-r--r--   0 cdent      (503) staff       (20)      155 2024-03-15 16:32:12.000000 PasteScript-3.5.1/PasteScript.egg-info/requires.txt
--rw-r--r--   0 cdent      (503) staff       (20)        6 2024-03-15 16:32:12.000000 PasteScript-3.5.1/PasteScript.egg-info/top_level.txt
--rw-r--r--   0 cdent      (503) staff       (20)      837 2021-04-27 13:47:08.000000 PasteScript-3.5.1/README.rst
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.357469 PasteScript-3.5.1/docs/
--rw-r--r--   0 cdent      (503) staff       (20)     3907 2024-03-14 12:37:59.000000 PasteScript-3.5.1/docs/conf.py
--rw-r--r--   0 cdent      (503) staff       (20)     7679 2021-04-27 13:47:08.000000 PasteScript-3.5.1/docs/developer.txt
--rwxr-xr-x   0 cdent      (503) staff       (20)      570 2021-04-27 13:47:08.000000 PasteScript-3.5.1/docs/example_app.ini
--rwxr-xr-x   0 cdent      (503) staff       (20)      111 2021-04-27 13:47:08.000000 PasteScript-3.5.1/docs/example_cgi_app.ini
--rw-r--r--   0 cdent      (503) staff       (20)     7070 2021-04-27 13:47:08.000000 PasteScript-3.5.1/docs/index.txt
--rw-r--r--   0 cdent      (503) staff       (20)     1077 2021-04-27 13:47:08.000000 PasteScript-3.5.1/docs/license.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.359455 PasteScript-3.5.1/docs/modules/
--rw-r--r--   0 cdent      (503) staff       (20)      597 2021-04-27 13:47:08.000000 PasteScript-3.5.1/docs/modules/checkperms.txt
--rw-r--r--   0 cdent      (503) staff       (20)      329 2021-04-27 13:47:08.000000 PasteScript-3.5.1/docs/modules/cherrypy_server.txt
--rw-r--r--   0 cdent      (503) staff       (20)      248 2021-04-27 13:47:08.000000 PasteScript-3.5.1/docs/modules/command.txt
--rw-r--r--   0 cdent      (503) staff       (20)      314 2021-04-27 13:47:08.000000 PasteScript-3.5.1/docs/modules/copydir.txt
--rw-r--r--   0 cdent      (503) staff       (20)      228 2021-04-27 13:47:08.000000 PasteScript-3.5.1/docs/modules/filemaker.txt
--rw-r--r--   0 cdent      (503) staff       (20)      288 2021-04-27 13:47:08.000000 PasteScript-3.5.1/docs/modules/templates.txt
--rw-r--r--   0 cdent      (503) staff       (20)      225 2021-04-27 13:47:08.000000 PasteScript-3.5.1/docs/modules/testapp.txt
--rw-r--r--   0 cdent      (503) staff       (20)      224 2021-04-27 13:47:08.000000 PasteScript-3.5.1/docs/modules/util.secret.txt
--rw-r--r--   0 cdent      (503) staff       (20)    15317 2024-03-15 16:28:22.000000 PasteScript-3.5.1/docs/news.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.359706 PasteScript-3.5.1/paste/
--rw-r--r--   0 cdent      (503) staff       (20)      552 2021-04-27 13:47:08.000000 PasteScript-3.5.1/paste/__init__.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.365975 PasteScript-3.5.1/paste/script/
--rw-r--r--   0 cdent      (503) staff       (20)      171 2021-04-27 13:47:08.000000 PasteScript-3.5.1/paste/script/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)    24769 2024-03-14 12:37:59.000000 PasteScript-3.5.1/paste/script/appinstall.py
--rw-r--r--   0 cdent      (503) staff       (20)     1985 2021-04-27 13:47:08.000000 PasteScript-3.5.1/paste/script/bool_optparse.py
--rw-r--r--   0 cdent      (503) staff       (20)     2388 2024-03-14 12:37:59.000000 PasteScript-3.5.1/paste/script/cgi_server.py
--rw-r--r--   0 cdent      (503) staff       (20)    13375 2021-04-27 13:47:08.000000 PasteScript-3.5.1/paste/script/checkperms.py
--rw-r--r--   0 cdent      (503) staff       (20)     3464 2021-04-27 13:47:08.000000 PasteScript-3.5.1/paste/script/cherrypy_server.py
--rw-r--r--   0 cdent      (503) staff       (20)    29069 2024-03-14 12:37:59.000000 PasteScript-3.5.1/paste/script/command.py
--rw-r--r--   0 cdent      (503) staff       (20)    15372 2024-03-14 12:37:59.000000 PasteScript-3.5.1/paste/script/copydir.py
--rw-r--r--   0 cdent      (503) staff       (20)    16855 2024-03-14 12:37:59.000000 PasteScript-3.5.1/paste/script/create_distro.py
--rw-r--r--   0 cdent      (503) staff       (20)     1416 2021-04-27 13:47:08.000000 PasteScript-3.5.1/paste/script/default_sysconfig.py
--rw-r--r--   0 cdent      (503) staff       (20)     9317 2024-03-14 12:37:59.000000 PasteScript-3.5.1/paste/script/entrypoints.py
--rw-r--r--   0 cdent      (503) staff       (20)     1596 2021-04-27 13:47:08.000000 PasteScript-3.5.1/paste/script/epdesc.py
--rw-r--r--   0 cdent      (503) staff       (20)     3454 2021-04-27 13:47:08.000000 PasteScript-3.5.1/paste/script/exe.py
--rw-r--r--   0 cdent      (503) staff       (20)    13519 2024-03-14 12:37:59.000000 PasteScript-3.5.1/paste/script/filemaker.py
--rw-r--r--   0 cdent      (503) staff       (20)     3685 2021-04-27 13:47:08.000000 PasteScript-3.5.1/paste/script/flup_server.py
--rw-r--r--   0 cdent      (503) staff       (20)     6208 2024-03-14 12:37:59.000000 PasteScript-3.5.1/paste/script/grep.py
--rw-r--r--   0 cdent      (503) staff       (20)     1960 2024-03-14 12:37:59.000000 PasteScript-3.5.1/paste/script/help.py
--rw-r--r--   0 cdent      (503) staff       (20)     1978 2021-04-27 13:47:08.000000 PasteScript-3.5.1/paste/script/interfaces.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.328009 PasteScript-3.5.1/paste/script/paster-templates/
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.366476 PasteScript-3.5.1/paste/script/paster-templates/basic_package/
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.366758 PasteScript-3.5.1/paste/script/paster-templates/basic_package/+package+/
--rw-r--r--   0 cdent      (503) staff       (20)        2 2021-04-27 13:47:08.000000 PasteScript-3.5.1/paste/script/paster-templates/basic_package/+package+/__init__.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.367011 PasteScript-3.5.1/paste/script/paster-templates/basic_package/docs/
--rw-r--r--   0 cdent      (503) staff       (20)    45741 2021-04-27 13:47:08.000000 PasteScript-3.5.1/paste/script/paster-templates/basic_package/docs/license.txt_tmpl
--rw-r--r--   0 cdent      (503) staff       (20)       51 2021-04-27 13:47:08.000000 PasteScript-3.5.1/paste/script/paster-templates/basic_package/setup.cfg
--rw-r--r--   0 cdent      (503) staff       (20)      853 2021-04-27 13:47:08.000000 PasteScript-3.5.1/paste/script/paster-templates/basic_package/setup.py_tmpl
--rw-r--r--   0 cdent      (503) staff       (20)     4287 2024-03-14 12:37:59.000000 PasteScript-3.5.1/paste/script/pluginlib.py
--rw-r--r--   0 cdent      (503) staff       (20)     7434 2024-03-14 12:37:59.000000 PasteScript-3.5.1/paste/script/request.py
--rw-r--r--   0 cdent      (503) staff       (20)    23124 2024-03-14 12:37:59.000000 PasteScript-3.5.1/paste/script/serve.py
--rw-r--r--   0 cdent      (503) staff       (20)    10018 2024-03-14 12:37:59.000000 PasteScript-3.5.1/paste/script/templates.py
--rw-r--r--   0 cdent      (503) staff       (20)     2861 2024-03-14 12:37:59.000000 PasteScript-3.5.1/paste/script/testapp.py
--rw-r--r--   0 cdent      (503) staff       (20)      905 2021-04-27 13:47:08.000000 PasteScript-3.5.1/paste/script/twisted_web2_server.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.368209 PasteScript-3.5.1/paste/script/util/
--rw-r--r--   0 cdent      (503) staff       (20)      171 2021-04-27 13:47:08.000000 PasteScript-3.5.1/paste/script/util/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)    12375 2024-03-14 12:37:59.000000 PasteScript-3.5.1/paste/script/util/logging_config.py
--rw-r--r--   0 cdent      (503) staff       (20)     1045 2024-03-14 12:37:59.000000 PasteScript-3.5.1/paste/script/util/secret.py
--rw-r--r--   0 cdent      (503) staff       (20)      749 2021-04-27 13:47:08.000000 PasteScript-3.5.1/paste/script/wsgiutils_server.py
--rwxr-xr-x   0 cdent      (503) staff       (20)      241 2021-04-27 13:47:08.000000 PasteScript-3.5.1/regen-docs
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.368502 PasteScript-3.5.1/scripts/
--rwxr-xr-x   0 cdent      (503) staff       (20)      289 2021-04-27 13:47:08.000000 PasteScript-3.5.1/scripts/paster
--rw-r--r--   0 cdent      (503) staff       (20)       94 2024-03-15 16:32:12.384289 PasteScript-3.5.1/setup.cfg
--rw-r--r--   0 cdent      (503) staff       (20)     5656 2024-03-15 16:27:49.000000 PasteScript-3.5.1/setup.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.370331 PasteScript-3.5.1/tests/
--rw-r--r--   0 cdent      (503) staff       (20)      954 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/__init__.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.377248 PasteScript-3.5.1/tests/appsetup/
--rw-r--r--   0 cdent      (503) staff       (20)        0 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/appsetup/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)     5246 2024-03-14 12:37:59.000000 PasteScript-3.5.1/tests/appsetup/test_make_project.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.378478 PasteScript-3.5.1/tests/appsetup/testfiles/
--rw-r--r--   0 cdent      (503) staff       (20)       96 2024-03-14 12:37:59.000000 PasteScript-3.5.1/tests/appsetup/testfiles/admin_index.py
--rw-r--r--   0 cdent      (503) staff       (20)      185 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/appsetup/testfiles/conftest.py
--rw-r--r--   0 cdent      (503) staff       (20)      175 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/appsetup/testfiles/iscape.txt
--rw-r--r--   0 cdent      (503) staff       (20)      329 2024-03-14 12:37:59.000000 PasteScript-3.5.1/tests/appsetup/testfiles/test_forbidden.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.330538 PasteScript-3.5.1/tests/fake_packages/
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.378735 PasteScript-3.5.1/tests/fake_packages/FakePlugin.egg/
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.379913 PasteScript-3.5.1/tests/fake_packages/FakePlugin.egg/EGG-INFO/
--rw-r--r--   0 cdent      (503) staff       (20)      182 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/fake_packages/FakePlugin.egg/EGG-INFO/PKG-INFO
--rw-r--r--   0 cdent      (503) staff       (20)       64 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/fake_packages/FakePlugin.egg/EGG-INFO/entry_points.txt
--rw-r--r--   0 cdent      (503) staff       (20)       13 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/fake_packages/FakePlugin.egg/EGG-INFO/paster_plugins.txt
--rw-r--r--   0 cdent      (503) staff       (20)       11 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/fake_packages/FakePlugin.egg/EGG-INFO/top_level.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.381027 PasteScript-3.5.1/tests/fake_packages/FakePlugin.egg/FakePlugin.egg-info/
--rw-r--r--   0 cdent      (503) staff       (20)      182 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/fake_packages/FakePlugin.egg/FakePlugin.egg-info/PKG-INFO
--rw-r--r--   0 cdent      (503) staff       (20)       64 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/fake_packages/FakePlugin.egg/FakePlugin.egg-info/entry_points.txt
--rw-r--r--   0 cdent      (503) staff       (20)       13 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/fake_packages/FakePlugin.egg/FakePlugin.egg-info/paster_plugins.txt
--rw-r--r--   0 cdent      (503) staff       (20)       11 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/fake_packages/FakePlugin.egg/FakePlugin.egg-info/top_level.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.381352 PasteScript-3.5.1/tests/fake_packages/FakePlugin.egg/fakeplugin/
--rw-r--r--   0 cdent      (503) staff       (20)        2 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/fake_packages/FakePlugin.egg/fakeplugin/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)      124 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/fake_packages/FakePlugin.egg/setup.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-15 16:32:12.382639 PasteScript-3.5.1/tests/sample_templates/
--rw-r--r--   0 cdent      (503) staff       (20)       79 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/sample_templates/test1.txt
--rw-r--r--   0 cdent      (503) staff       (20)      123 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/sample_templates/test2.py_tmpl
--rw-r--r--   0 cdent      (503) staff       (20)       50 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/sample_templates/test3.ini_tmpl
--rw-r--r--   0 cdent      (503) staff       (20)       37 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/sample_templates/test4.html_tmpl
--rw-r--r--   0 cdent      (503) staff       (20)     9928 2024-03-14 12:37:59.000000 PasteScript-3.5.1/tests/test_command.py
--rw-r--r--   0 cdent      (503) staff       (20)      858 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/test_egg_finder.py
--rw-r--r--   0 cdent      (503) staff       (20)     6211 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/test_logging_config.py
--rw-r--r--   0 cdent      (503) staff       (20)      736 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/test_plugin_adder.py
--rw-r--r--   0 cdent      (503) staff       (20)      491 2023-01-03 17:45:06.000000 PasteScript-3.5.1/tests/test_template_introspect.py
--rw-r--r--   0 cdent      (503) staff       (20)      397 2021-04-27 13:47:08.000000 PasteScript-3.5.1/tests/test_util.py
--rw-r--r--   0 cdent      (503) staff       (20)      408 2024-03-14 12:37:59.000000 PasteScript-3.5.1/tox.ini
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.559934 PasteScript-3.6.0/
+-rw-r--r--   0 cdent      (503) staff       (20)      536 2021-04-27 13:47:08.000000 PasteScript-3.6.0/AUTHORS
+-rw-r--r--   0 cdent      (503) staff       (20)      403 2021-04-27 13:47:08.000000 PasteScript-3.6.0/MANIFEST.in
+-rw-r--r--   0 cdent      (503) staff       (20)     2814 2024-04-27 12:05:26.559761 PasteScript-3.6.0/PKG-INFO
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.559073 PasteScript-3.6.0/PasteScript.egg-info/
+-rw-r--r--   0 cdent      (503) staff       (20)     2814 2024-04-27 12:05:26.000000 PasteScript-3.6.0/PasteScript.egg-info/PKG-INFO
+-rw-r--r--   0 cdent      (503) staff       (20)     2893 2024-04-27 12:05:26.000000 PasteScript-3.6.0/PasteScript.egg-info/SOURCES.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        1 2024-04-27 12:05:26.000000 PasteScript-3.6.0/PasteScript.egg-info/dependency_links.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     2197 2024-04-27 12:05:26.000000 PasteScript-3.6.0/PasteScript.egg-info/entry_points.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        6 2024-04-27 12:05:26.000000 PasteScript-3.6.0/PasteScript.egg-info/namespace_packages.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        1 2024-04-27 12:05:26.000000 PasteScript-3.6.0/PasteScript.egg-info/not-zip-safe
+-rw-r--r--   0 cdent      (503) staff       (20)      155 2024-04-27 12:05:26.000000 PasteScript-3.6.0/PasteScript.egg-info/requires.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        6 2024-04-27 12:05:26.000000 PasteScript-3.6.0/PasteScript.egg-info/top_level.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     1267 2024-04-27 11:52:45.000000 PasteScript-3.6.0/README.rst
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.531801 PasteScript-3.6.0/docs/
+-rw-r--r--   0 cdent      (503) staff       (20)     3899 2024-04-27 11:54:27.000000 PasteScript-3.6.0/docs/conf.py
+-rw-r--r--   0 cdent      (503) staff       (20)     7679 2021-04-27 13:47:08.000000 PasteScript-3.6.0/docs/developer.txt
+-rwxr-xr-x   0 cdent      (503) staff       (20)      570 2021-04-27 13:47:08.000000 PasteScript-3.6.0/docs/example_app.ini
+-rwxr-xr-x   0 cdent      (503) staff       (20)      111 2021-04-27 13:47:08.000000 PasteScript-3.6.0/docs/example_cgi_app.ini
+-rw-r--r--   0 cdent      (503) staff       (20)     7073 2024-04-27 11:48:40.000000 PasteScript-3.6.0/docs/index.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     1077 2021-04-27 13:47:08.000000 PasteScript-3.6.0/docs/license.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.533955 PasteScript-3.6.0/docs/modules/
+-rw-r--r--   0 cdent      (503) staff       (20)      597 2021-04-27 13:47:08.000000 PasteScript-3.6.0/docs/modules/checkperms.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      329 2021-04-27 13:47:08.000000 PasteScript-3.6.0/docs/modules/cherrypy_server.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      248 2021-04-27 13:47:08.000000 PasteScript-3.6.0/docs/modules/command.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      314 2021-04-27 13:47:08.000000 PasteScript-3.6.0/docs/modules/copydir.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      228 2021-04-27 13:47:08.000000 PasteScript-3.6.0/docs/modules/filemaker.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      288 2021-04-27 13:47:08.000000 PasteScript-3.6.0/docs/modules/templates.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      225 2021-04-27 13:47:08.000000 PasteScript-3.6.0/docs/modules/testapp.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      224 2021-04-27 13:47:08.000000 PasteScript-3.6.0/docs/modules/util.secret.txt
+-rw-r--r--   0 cdent      (503) staff       (20)    15846 2024-04-27 11:52:30.000000 PasteScript-3.6.0/docs/news.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.534217 PasteScript-3.6.0/paste/
+-rw-r--r--   0 cdent      (503) staff       (20)      552 2021-04-27 13:47:08.000000 PasteScript-3.6.0/paste/__init__.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.547233 PasteScript-3.6.0/paste/script/
+-rw-r--r--   0 cdent      (503) staff       (20)      171 2021-04-27 13:47:08.000000 PasteScript-3.6.0/paste/script/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)    24769 2024-03-14 12:37:59.000000 PasteScript-3.6.0/paste/script/appinstall.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1985 2021-04-27 13:47:08.000000 PasteScript-3.6.0/paste/script/bool_optparse.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2388 2024-03-14 12:37:59.000000 PasteScript-3.6.0/paste/script/cgi_server.py
+-rw-r--r--   0 cdent      (503) staff       (20)    13375 2021-04-27 13:47:08.000000 PasteScript-3.6.0/paste/script/checkperms.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3464 2021-04-27 13:47:08.000000 PasteScript-3.6.0/paste/script/cherrypy_server.py
+-rw-r--r--   0 cdent      (503) staff       (20)    29069 2024-03-14 12:37:59.000000 PasteScript-3.6.0/paste/script/command.py
+-rw-r--r--   0 cdent      (503) staff       (20)    15372 2024-03-14 12:37:59.000000 PasteScript-3.6.0/paste/script/copydir.py
+-rw-r--r--   0 cdent      (503) staff       (20)    16855 2024-03-14 12:37:59.000000 PasteScript-3.6.0/paste/script/create_distro.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1416 2021-04-27 13:47:08.000000 PasteScript-3.6.0/paste/script/default_sysconfig.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9317 2024-03-14 12:37:59.000000 PasteScript-3.6.0/paste/script/entrypoints.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1596 2021-04-27 13:47:08.000000 PasteScript-3.6.0/paste/script/epdesc.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3454 2021-04-27 13:47:08.000000 PasteScript-3.6.0/paste/script/exe.py
+-rw-r--r--   0 cdent      (503) staff       (20)    13519 2024-03-14 12:37:59.000000 PasteScript-3.6.0/paste/script/filemaker.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3685 2021-04-27 13:47:08.000000 PasteScript-3.6.0/paste/script/flup_server.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6208 2024-03-14 12:37:59.000000 PasteScript-3.6.0/paste/script/grep.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1960 2024-03-14 12:37:59.000000 PasteScript-3.6.0/paste/script/help.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1978 2021-04-27 13:47:08.000000 PasteScript-3.6.0/paste/script/interfaces.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.522596 PasteScript-3.6.0/paste/script/paster-templates/
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.548017 PasteScript-3.6.0/paste/script/paster-templates/basic_package/
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.548358 PasteScript-3.6.0/paste/script/paster-templates/basic_package/+package+/
+-rw-r--r--   0 cdent      (503) staff       (20)        2 2021-04-27 13:47:08.000000 PasteScript-3.6.0/paste/script/paster-templates/basic_package/+package+/__init__.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.548664 PasteScript-3.6.0/paste/script/paster-templates/basic_package/docs/
+-rw-r--r--   0 cdent      (503) staff       (20)    45741 2021-04-27 13:47:08.000000 PasteScript-3.6.0/paste/script/paster-templates/basic_package/docs/license.txt_tmpl
+-rw-r--r--   0 cdent      (503) staff       (20)       51 2021-04-27 13:47:08.000000 PasteScript-3.6.0/paste/script/paster-templates/basic_package/setup.cfg
+-rw-r--r--   0 cdent      (503) staff       (20)      853 2021-04-27 13:47:08.000000 PasteScript-3.6.0/paste/script/paster-templates/basic_package/setup.py_tmpl
+-rw-r--r--   0 cdent      (503) staff       (20)     4287 2024-03-14 12:37:59.000000 PasteScript-3.6.0/paste/script/pluginlib.py
+-rw-r--r--   0 cdent      (503) staff       (20)     7434 2024-03-14 12:37:59.000000 PasteScript-3.6.0/paste/script/request.py
+-rw-r--r--   0 cdent      (503) staff       (20)    23124 2024-03-14 12:37:59.000000 PasteScript-3.6.0/paste/script/serve.py
+-rw-r--r--   0 cdent      (503) staff       (20)    10018 2024-03-14 12:37:59.000000 PasteScript-3.6.0/paste/script/templates.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2861 2024-03-14 12:37:59.000000 PasteScript-3.6.0/paste/script/testapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)      905 2021-04-27 13:47:08.000000 PasteScript-3.6.0/paste/script/twisted_web2_server.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.549673 PasteScript-3.6.0/paste/script/util/
+-rw-r--r--   0 cdent      (503) staff       (20)      171 2021-04-27 13:47:08.000000 PasteScript-3.6.0/paste/script/util/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)    12375 2024-03-14 12:37:59.000000 PasteScript-3.6.0/paste/script/util/logging_config.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1045 2024-03-14 12:37:59.000000 PasteScript-3.6.0/paste/script/util/secret.py
+-rw-r--r--   0 cdent      (503) staff       (20)      749 2021-04-27 13:47:08.000000 PasteScript-3.6.0/paste/script/wsgiutils_server.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)      241 2021-04-27 13:47:08.000000 PasteScript-3.6.0/regen-docs
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.549943 PasteScript-3.6.0/scripts/
+-rwxr-xr-x   0 cdent      (503) staff       (20)      289 2021-04-27 13:47:08.000000 PasteScript-3.6.0/scripts/paster
+-rw-r--r--   0 cdent      (503) staff       (20)       94 2024-04-27 12:05:26.560250 PasteScript-3.6.0/setup.cfg
+-rw-r--r--   0 cdent      (503) staff       (20)     5684 2024-04-27 12:02:10.000000 PasteScript-3.6.0/setup.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.552292 PasteScript-3.6.0/tests/
+-rw-r--r--   0 cdent      (503) staff       (20)      954 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/__init__.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.552780 PasteScript-3.6.0/tests/appsetup/
+-rw-r--r--   0 cdent      (503) staff       (20)        0 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/appsetup/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)     5246 2024-03-14 12:37:59.000000 PasteScript-3.6.0/tests/appsetup/test_make_project.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.554126 PasteScript-3.6.0/tests/appsetup/testfiles/
+-rw-r--r--   0 cdent      (503) staff       (20)       96 2024-03-14 12:37:59.000000 PasteScript-3.6.0/tests/appsetup/testfiles/admin_index.py
+-rw-r--r--   0 cdent      (503) staff       (20)      185 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/appsetup/testfiles/conftest.py
+-rw-r--r--   0 cdent      (503) staff       (20)      175 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/appsetup/testfiles/iscape.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      329 2024-03-14 12:37:59.000000 PasteScript-3.6.0/tests/appsetup/testfiles/test_forbidden.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.524700 PasteScript-3.6.0/tests/fake_packages/
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.554440 PasteScript-3.6.0/tests/fake_packages/FakePlugin.egg/
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.555809 PasteScript-3.6.0/tests/fake_packages/FakePlugin.egg/EGG-INFO/
+-rw-r--r--   0 cdent      (503) staff       (20)      182 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/fake_packages/FakePlugin.egg/EGG-INFO/PKG-INFO
+-rw-r--r--   0 cdent      (503) staff       (20)       64 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/fake_packages/FakePlugin.egg/EGG-INFO/entry_points.txt
+-rw-r--r--   0 cdent      (503) staff       (20)       13 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/fake_packages/FakePlugin.egg/EGG-INFO/paster_plugins.txt
+-rw-r--r--   0 cdent      (503) staff       (20)       11 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/fake_packages/FakePlugin.egg/EGG-INFO/top_level.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.556997 PasteScript-3.6.0/tests/fake_packages/FakePlugin.egg/FakePlugin.egg-info/
+-rw-r--r--   0 cdent      (503) staff       (20)      182 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/fake_packages/FakePlugin.egg/FakePlugin.egg-info/PKG-INFO
+-rw-r--r--   0 cdent      (503) staff       (20)       64 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/fake_packages/FakePlugin.egg/FakePlugin.egg-info/entry_points.txt
+-rw-r--r--   0 cdent      (503) staff       (20)       13 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/fake_packages/FakePlugin.egg/FakePlugin.egg-info/paster_plugins.txt
+-rw-r--r--   0 cdent      (503) staff       (20)       11 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/fake_packages/FakePlugin.egg/FakePlugin.egg-info/top_level.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.557358 PasteScript-3.6.0/tests/fake_packages/FakePlugin.egg/fakeplugin/
+-rw-r--r--   0 cdent      (503) staff       (20)        2 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/fake_packages/FakePlugin.egg/fakeplugin/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)      124 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/fake_packages/FakePlugin.egg/setup.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-04-27 12:05:26.558660 PasteScript-3.6.0/tests/sample_templates/
+-rw-r--r--   0 cdent      (503) staff       (20)       79 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/sample_templates/test1.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      123 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/sample_templates/test2.py_tmpl
+-rw-r--r--   0 cdent      (503) staff       (20)       50 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/sample_templates/test3.ini_tmpl
+-rw-r--r--   0 cdent      (503) staff       (20)       37 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/sample_templates/test4.html_tmpl
+-rw-r--r--   0 cdent      (503) staff       (20)     9928 2024-03-14 12:37:59.000000 PasteScript-3.6.0/tests/test_command.py
+-rw-r--r--   0 cdent      (503) staff       (20)      858 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/test_egg_finder.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6211 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/test_logging_config.py
+-rw-r--r--   0 cdent      (503) staff       (20)      736 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/test_plugin_adder.py
+-rw-r--r--   0 cdent      (503) staff       (20)      491 2023-01-03 17:45:06.000000 PasteScript-3.6.0/tests/test_template_introspect.py
+-rw-r--r--   0 cdent      (503) staff       (20)      397 2021-04-27 13:47:08.000000 PasteScript-3.6.0/tests/test_util.py
+-rw-r--r--   0 cdent      (503) staff       (20)      408 2024-03-14 12:37:59.000000 PasteScript-3.6.0/tox.ini
```

### Comparing `PasteScript-3.5.1/AUTHORS` & `PasteScript-3.6.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/PKG-INFO` & `PasteScript-3.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PasteScript
-Version: 3.5.1
+Version: 3.6.0
 Summary: A pluggable command-line frontend, including commands to setup package file layouts
 Home-page: https://pastescript.readthedocs.io/
 Author: Ian Bicking
 Author-email: ianb@colorstudy.com
 License: MIT
 Keywords: web wsgi setuptools framework command-line setup
 Classifier: Development Status :: 6 - Mature
@@ -42,22 +42,30 @@
 PasteScript is a pluggable command-line tool.
 
 **Note**: Paste Script is being maintained on life support. That
 means that critical bugs will be fixed, and support for new versions
 of Python will be handled, but other than that new features are not
 being considered.
 
+**With version 3.6.0 pastescript development moves to the pasteorg GitHub
+organization and will be going deeper into maintenance mode unless
+more active maintainers step forward to take over. "Deeper" in this
+case means that releases will be much less frequent and patches
+will only be accepted for security issues or major problems. Current
+consumers of pastescript should prepare to migrate away to more modern
+solutions.**
+
 It includes some built-in features;
 
 * Create file layouts for packages.  For instance, ``paster create
   --template=basic_package MyPackage`` will create a `setuptools
   <https://pythonhosted.org/setuptools/>`_-ready
   file layout.
 
 * Serving up web applications, with configuration based on
   `paste.deploy <https://docs.pylonsproject.org/projects/pastedeploy>`_.
 
 The latest version is available in a `GitHub repository
-<https://github.com/cdent/pastescript/>`_.
+<https://github.com/pasteorg/pastescript/>`_.
 
 For the latest changes see the `news file
 <https://pastescript.readthedocs.io/en/latest/news.html>`_.
```

### Comparing `PasteScript-3.5.1/PasteScript.egg-info/PKG-INFO` & `PasteScript-3.6.0/PasteScript.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PasteScript
-Version: 3.5.1
+Version: 3.6.0
 Summary: A pluggable command-line frontend, including commands to setup package file layouts
 Home-page: https://pastescript.readthedocs.io/
 Author: Ian Bicking
 Author-email: ianb@colorstudy.com
 License: MIT
 Keywords: web wsgi setuptools framework command-line setup
 Classifier: Development Status :: 6 - Mature
@@ -42,22 +42,30 @@
 PasteScript is a pluggable command-line tool.
 
 **Note**: Paste Script is being maintained on life support. That
 means that critical bugs will be fixed, and support for new versions
 of Python will be handled, but other than that new features are not
 being considered.
 
+**With version 3.6.0 pastescript development moves to the pasteorg GitHub
+organization and will be going deeper into maintenance mode unless
+more active maintainers step forward to take over. "Deeper" in this
+case means that releases will be much less frequent and patches
+will only be accepted for security issues or major problems. Current
+consumers of pastescript should prepare to migrate away to more modern
+solutions.**
+
 It includes some built-in features;
 
 * Create file layouts for packages.  For instance, ``paster create
   --template=basic_package MyPackage`` will create a `setuptools
   <https://pythonhosted.org/setuptools/>`_-ready
   file layout.
 
 * Serving up web applications, with configuration based on
   `paste.deploy <https://docs.pylonsproject.org/projects/pastedeploy>`_.
 
 The latest version is available in a `GitHub repository
-<https://github.com/cdent/pastescript/>`_.
+<https://github.com/pasteorg/pastescript/>`_.
 
 For the latest changes see the `news file
 <https://pastescript.readthedocs.io/en/latest/news.html>`_.
```

### Comparing `PasteScript-3.5.1/PasteScript.egg-info/SOURCES.txt` & `PasteScript-3.6.0/PasteScript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/PasteScript.egg-info/entry_points.txt` & `PasteScript-3.6.0/PasteScript.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/README.rst` & `PasteScript-3.6.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 PasteScript is a pluggable command-line tool.
 
 **Note**: Paste Script is being maintained on life support. That
 means that critical bugs will be fixed, and support for new versions
 of Python will be handled, but other than that new features are not
 being considered.
 
+**With version 3.6.0 pastescript development moves to the pasteorg GitHub
+organization and will be going deeper into maintenance mode unless
+more active maintainers step forward to take over. "Deeper" in this
+case means that releases will be much less frequent and patches
+will only be accepted for security issues or major problems. Current
+consumers of pastescript should prepare to migrate away to more modern
+solutions.**
+
 It includes some built-in features;
 
 * Create file layouts for packages.  For instance, ``paster create
   --template=basic_package MyPackage`` will create a `setuptools
   <https://pythonhosted.org/setuptools/>`_-ready
   file layout.
 
 * Serving up web applications, with configuration based on
   `paste.deploy <https://docs.pylonsproject.org/projects/pastedeploy>`_.
 
 The latest version is available in a `GitHub repository
-<https://github.com/cdent/pastescript/>`_.
+<https://github.com/pasteorg/pastescript/>`_.
 
 For the latest changes see the `news file
 <https://pastescript.readthedocs.io/en/latest/news.html>`_.
```

### Comparing `PasteScript-3.5.1/docs/conf.py` & `PasteScript-3.6.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 project = 'Paste Script'
 copyright = '2011, Ian Bicking'
 
 # The default replacements for |version| and |release|, also used in various
 # other places throughout the built documents.
 #
 # The short X.Y version.
-version = '1.7'
+version = ''
 # The full version, including alpha/beta/rc tags.
-release = '1.7.5'
+release = ''
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 #today = ''
 # Else, today_fmt is used as the format for a strftime call.
 today_fmt = '%B %d, %Y'
```

### Comparing `PasteScript-3.5.1/docs/developer.txt` & `PasteScript-3.6.0/docs/developer.txt`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/docs/example_app.ini` & `PasteScript-3.6.0/docs/example_app.ini`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/docs/index.txt` & `PasteScript-3.6.0/docs/index.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 Warning
 -------
 
 Paste Script is being maintained on life support. That means that
 critical bugs will be fixed, and support for new versions of Python
 will be handled, but other than that new features are not being
 considered. Development has moved to `GitHub
-<https://github.com/cdent/pastescript>`_.
+<https://github.com/pasteorg/pastescript>`_.
 
 Introduction
 ------------
 
 If you are developer, see the `Developer Documentation
 <developer.html>`_; this will tell you how to add commands and
 templates to ``paster``.  For a list of updates see the `news file
```

### Comparing `PasteScript-3.5.1/docs/license.txt` & `PasteScript-3.6.0/docs/license.txt`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/docs/modules/checkperms.txt` & `PasteScript-3.6.0/docs/modules/checkperms.txt`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/docs/news.txt` & `PasteScript-3.6.0/docs/news.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 News: Paste Script
 ==================
 
 .. contents::
 
+3.6.0 (2024-04-27)
+------------------
+
+* Pastescript is moved to https://github.com/pasteorg/pastescript
+
+With version 3.6.0 pastescript development moves to the pasteorg GitHub
+organization and will be going deeper into maintenance mode unless
+more active maintainers step forward to take over. "Deeper" in this
+case means that releases will be much less frequent and patches
+will only be accepted for security issues or major problems. Current
+consumers of pastescript should prepare to migrate away to more modern
+solutions.
+
 3.5.1 (2024-03-15)
 ------------------
 
 * Be explicit about Python 3 being required.
 
 3.5.0 (2024-03-14)
 ------------------
```

### Comparing `PasteScript-3.5.1/paste/__init__.py` & `PasteScript-3.6.0/paste/__init__.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/appinstall.py` & `PasteScript-3.6.0/paste/script/appinstall.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/bool_optparse.py` & `PasteScript-3.6.0/paste/script/bool_optparse.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/cgi_server.py` & `PasteScript-3.6.0/paste/script/cgi_server.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/checkperms.py` & `PasteScript-3.6.0/paste/script/checkperms.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/cherrypy_server.py` & `PasteScript-3.6.0/paste/script/cherrypy_server.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/command.py` & `PasteScript-3.6.0/paste/script/command.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/copydir.py` & `PasteScript-3.6.0/paste/script/copydir.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/create_distro.py` & `PasteScript-3.6.0/paste/script/create_distro.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/default_sysconfig.py` & `PasteScript-3.6.0/paste/script/default_sysconfig.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/entrypoints.py` & `PasteScript-3.6.0/paste/script/entrypoints.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/epdesc.py` & `PasteScript-3.6.0/paste/script/epdesc.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/exe.py` & `PasteScript-3.6.0/paste/script/exe.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/filemaker.py` & `PasteScript-3.6.0/paste/script/filemaker.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/flup_server.py` & `PasteScript-3.6.0/paste/script/flup_server.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/grep.py` & `PasteScript-3.6.0/paste/script/grep.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/help.py` & `PasteScript-3.6.0/paste/script/help.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/interfaces.py` & `PasteScript-3.6.0/paste/script/interfaces.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/paster-templates/basic_package/docs/license.txt_tmpl` & `PasteScript-3.6.0/paste/script/paster-templates/basic_package/docs/license.txt_tmpl`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/paster-templates/basic_package/setup.py_tmpl` & `PasteScript-3.6.0/paste/script/paster-templates/basic_package/setup.py_tmpl`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/pluginlib.py` & `PasteScript-3.6.0/paste/script/pluginlib.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/request.py` & `PasteScript-3.6.0/paste/script/request.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/serve.py` & `PasteScript-3.6.0/paste/script/serve.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/templates.py` & `PasteScript-3.6.0/paste/script/templates.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/testapp.py` & `PasteScript-3.6.0/paste/script/testapp.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/twisted_web2_server.py` & `PasteScript-3.6.0/paste/script/twisted_web2_server.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/util/logging_config.py` & `PasteScript-3.6.0/paste/script/util/logging_config.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/util/secret.py` & `PasteScript-3.6.0/paste/script/util/secret.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/paste/script/wsgiutils_server.py` & `PasteScript-3.6.0/paste/script/wsgiutils_server.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/setup.py` & `PasteScript-3.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,29 +11,30 @@
 # - git tag -s VERSION
 # - git push
 # - python setup.py sdist bdist_wheel upload --sign
 
 from setuptools import setup, find_packages
 import os
 import re
+import sys
 
-version = '3.5.1'
+version = '3.6.0'
 
 news = os.path.join(os.path.dirname(__file__), 'docs', 'news.txt')
 found_news = ''
 if os.path.exists(news):
     with open(news) as fp:
         news = fp.read()
     parts = re.split(r'([0-9\.]+)\s*\n\r?-+\n\r?', news)
     for i in range(len(parts)-1):
         if parts[i] == version:
             found_news = parts[i+i]
             break
 if not found_news:
-    print('Warning: no news for this version found')
+    print('Warning: no news for this version found', file=sys.stderr)
 
 with open("README.rst") as fp:
     long_description = fp.read().strip()
 
 if found_news:
     title = 'Changes in %s' % version
     long_description += "\n%s\n%s\n" % (title, '-'*len(title))
```

### Comparing `PasteScript-3.5.1/tests/__init__.py` & `PasteScript-3.6.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/tests/appsetup/test_make_project.py` & `PasteScript-3.6.0/tests/appsetup/test_make_project.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/tests/test_command.py` & `PasteScript-3.6.0/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/tests/test_egg_finder.py` & `PasteScript-3.6.0/tests/test_egg_finder.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/tests/test_logging_config.py` & `PasteScript-3.6.0/tests/test_logging_config.py`

 * *Files identical despite different names*

### Comparing `PasteScript-3.5.1/tests/test_plugin_adder.py` & `PasteScript-3.6.0/tests/test_plugin_adder.py`

 * *Files identical despite different names*

