# Comparing `tmp/introspection-1.7.9.tar.gz` & `tmp/introspection-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "introspection-1.7.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "introspection-1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `introspection-1.7.9.tar` & `introspection-1.8.tar`

### file list

```diff
@@ -1,109 +1,112 @@
--rw-r--r--   0        0        0     1070 2019-10-05 20:23:15.010707 introspection-1.7.9/LICENSE
--rw-r--r--   0        0        0      423 2020-06-21 16:21:23.702593 introspection-1.7.9/README.md
--rw-r--r--   0        0        0        1 2018-02-07 23:45:28.000000 introspection-1.7.9/docs/.nojekyll
--rw-r--r--   0        0        0     8370 2022-01-11 18:29:27.165570 introspection-1.7.9/docs/Makefile
--rw-r--r--   0        0        0    50309 2023-09-27 09:04:29.286431 introspection-1.7.9/docs/build/doctrees/call_stack.doctree
--rw-r--r--   0        0        0   113126 2023-09-27 09:04:29.472424 introspection-1.7.9/docs/build/doctrees/classes.doctree
--rw-r--r--   0        0        0   123722 2023-09-27 09:04:29.603457 introspection-1.7.9/docs/build/doctrees/dundermethods.doctree
--rw-r--r--   0        0        0   150280 2023-09-27 09:04:30.168939 introspection-1.7.9/docs/build/doctrees/function_signatures.doctree
--rw-r--r--   0        0        0     4054 2023-09-27 09:04:30.173941 introspection-1.7.9/docs/build/doctrees/index.doctree
--rw-r--r--   0        0        0   112020 2023-09-27 09:04:30.356611 introspection-1.7.9/docs/build/doctrees/misc.doctree
--rw-r--r--   0        0        0   132622 2022-07-28 05:12:16.888430 introspection-1.7.9/docs/build/doctrees/typing.doctree
--rw-r--r--   0        0        0      234 2022-07-28 05:12:17.627586 introspection-1.7.9/docs/build/html/.buildinfo
--rw-r--r--   0        0        0     4418 2022-06-30 11:20:55.284834 introspection-1.7.9/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    16132 2022-07-28 05:12:17.556578 introspection-1.7.9/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0      313 2022-01-14 19:00:26.466660 introspection-1.7.9/docs/build/html/_static/check-solid.svg
--rw-r--r--   0        0        0     9031 2022-01-14 19:00:26.467661 introspection-1.7.9/docs/build/html/_static/clipboard.min.js
--rw-r--r--   0        0        0      434 2022-01-14 19:00:26.467661 introspection-1.7.9/docs/build/html/_static/copy-button.svg
--rw-r--r--   0        0        0     1754 2022-01-14 19:00:26.470668 introspection-1.7.9/docs/build/html/_static/copybutton.css
--rw-r--r--   0        0        0     6716 2022-07-28 05:12:17.625587 introspection-1.7.9/docs/build/html/_static/copybutton.js
--rw-r--r--   0        0        0     2198 2022-01-14 19:00:26.473668 introspection-1.7.9/docs/build/html/_static/copybutton_funcs.js
--rw-r--r--   0        0        0     8171 2022-06-30 11:20:55.286835 introspection-1.7.9/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      435 2022-07-28 05:12:17.566583 introspection-1.7.9/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0     2296 2022-01-11 21:41:53.887944 introspection-1.7.9/docs/build/html/_static/favicon.svg
--rw-r--r--   0        0        0      286 2022-01-11 18:34:47.961414 introspection-1.7.9/docs/build/html/_static/file.png
--rw-r--r--   0        0        0   287630 2022-01-11 18:34:47.963413 introspection-1.7.9/docs/build/html/_static/jquery-3.5.1.js
--rw-r--r--   0        0        0   288580 2022-06-30 11:20:55.289835 introspection-1.7.9/docs/build/html/_static/jquery-3.6.0.js
--rw-r--r--   0        0        0    89501 2022-06-30 11:20:55.290835 introspection-1.7.9/docs/build/html/_static/jquery.js
--rw-r--r--   0        0        0     4957 2022-07-28 05:12:17.575582 introspection-1.7.9/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2022-01-11 18:34:47.966416 introspection-1.7.9/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0     9096 2022-01-15 08:34:05.001989 introspection-1.7.9/docs/build/html/_static/nightsky.css
--rw-r--r--   0        0        0    12357 2022-01-15 11:08:27.758930 introspection-1.7.9/docs/build/html/_static/nightsky.styl
--rw-r--r--   0        0        0       85 2021-03-08 19:37:10.079040 introspection-1.7.9/docs/build/html/_static/package-lock.json
--rw-r--r--   0        0        0        3 2021-03-08 19:37:10.080250 introspection-1.7.9/docs/build/html/_static/package.json
--rw-r--r--   0        0        0       90 2022-01-11 18:34:47.967415 introspection-1.7.9/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0     5119 2022-01-14 23:24:17.967774 introspection-1.7.9/docs/build/html/_static/pygments-cobalt2.css
--rw-r--r--   0        0        0     4919 2022-07-28 05:12:17.543568 introspection-1.7.9/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0     4633 2022-07-28 05:12:17.544569 introspection-1.7.9/docs/build/html/_static/pygments_dark.css
--rw-r--r--   0        0        0    17088 2022-06-30 11:20:55.294836 introspection-1.7.9/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     7067 2022-07-28 05:12:17.664594 introspection-1.7.9/docs/build/html/_static/theme_switcher.js
--rw-r--r--   0        0        0    68420 2022-01-11 18:34:47.969416 introspection-1.7.9/docs/build/html/_static/underscore-1.13.1.js
--rw-r--r--   0        0        0    19530 2022-01-11 18:34:47.970415 introspection-1.7.9/docs/build/html/_static/underscore.js
--rw-r--r--   0        0        0    19915 2022-07-28 05:12:17.083464 introspection-1.7.9/docs/build/html/call_stack.html
--rw-r--r--   0        0        0    48881 2022-07-28 05:12:17.141485 introspection-1.7.9/docs/build/html/classes.html
--rw-r--r--   0        0        0    61201 2022-07-28 05:12:17.254511 introspection-1.7.9/docs/build/html/dundermethods.html
--rw-r--r--   0        0        0    62670 2022-07-28 05:12:17.327518 introspection-1.7.9/docs/build/html/function_signatures.html
--rw-r--r--   0        0        0    24122 2022-07-28 05:12:17.499557 introspection-1.7.9/docs/build/html/genindex.html
--rw-r--r--   0        0        0     4965 2022-07-28 05:12:17.340521 introspection-1.7.9/docs/build/html/index.html
--rw-r--r--   0        0        0    54576 2022-07-28 05:12:17.404537 introspection-1.7.9/docs/build/html/misc.html
--rw-r--r--   0        0        0     1394 2022-07-28 05:12:17.632588 introspection-1.7.9/docs/build/html/objects.inv
--rw-r--r--   0        0        0     5636 2022-07-28 05:12:17.525572 introspection-1.7.9/docs/build/html/py-modindex.html
--rw-r--r--   0        0        0     3786 2022-07-28 05:12:17.541568 introspection-1.7.9/docs/build/html/search.html
--rw-r--r--   0        0        0    19468 2022-07-28 05:12:17.629587 introspection-1.7.9/docs/build/html/searchindex.js
--rw-r--r--   0        0        0    62944 2022-07-28 05:12:17.477563 introspection-1.7.9/docs/build/html/typing.html
--rw-r--r--   0        0        0      173 2018-02-07 20:12:32.000000 introspection-1.7.9/docs/index.html
--rwxr-xr-x   0        0        0     7793 2018-02-07 15:05:16.000000 introspection-1.7.9/docs/make.bat
--rw-r--r--   0        0        0      176 2020-06-21 11:11:00.000000 introspection-1.7.9/docs/source/call_stack.rst
--rw-r--r--   0        0        0      144 2020-06-21 11:52:08.000000 introspection-1.7.9/docs/source/classes.rst
--rw-r--r--   0        0        0     3889 2022-01-14 19:30:26.076283 introspection-1.7.9/docs/source/conf.py
--rw-r--r--   0        0        0     1605 2020-07-11 05:40:06.000000 introspection-1.7.9/docs/source/dundermethods.rst
--rw-r--r--   0        0        0     2296 2022-01-11 21:41:53.887944 introspection-1.7.9/docs/source/favicon.svg
--rw-r--r--   0        0        0      579 2022-01-13 20:53:53.587095 introspection-1.7.9/docs/source/function_signatures.rst
--rw-r--r--   0        0        0      496 2020-07-11 05:40:06.000000 introspection-1.7.9/docs/source/index.rst
--rw-r--r--   0        0        0      210 2022-01-15 11:18:12.735064 introspection-1.7.9/docs/source/misc.rst
--rw-r--r--   0        0        0     1672 2022-07-26 08:59:09.533795 introspection-1.7.9/docs/source/typing.rst
--rw-r--r--   0        0        0      704 2024-02-02 13:03:04.036033 introspection-1.7.9/introspection/__init__.py
--rw-r--r--   0        0        0     1668 2024-01-18 08:25:36.597619 introspection-1.7.9/introspection/_utils.py
--rw-r--r--   0        0        0     1306 2024-01-18 08:25:42.808139 introspection-1.7.9/introspection/argument_bundle.py
--rw-r--r--   0        0        0     5213 2024-01-18 10:53:25.579010 introspection-1.7.9/introspection/bound_arguments.py
--rw-r--r--   0        0        0     5388 2024-01-18 23:04:07.035404 introspection-1.7.9/introspection/call_frame.py
--rw-r--r--   0        0        0     2531 2023-12-12 21:17:22.152565 introspection-1.7.9/introspection/call_stack.py
--rw-r--r--   0        0        0    18294 2024-01-19 09:49:33.862993 introspection-1.7.9/introspection/classes.py
--rw-r--r--   0        0        0      718 2022-12-07 10:42:15.146932 introspection-1.7.9/introspection/dunder.py
--rw-r--r--   0        0        0    16502 2024-01-18 23:07:13.842401 introspection-1.7.9/introspection/dundermethods.py
--rw-r--r--   0        0        0     6011 2024-01-18 08:25:41.852978 introspection-1.7.9/introspection/errors.py
--rw-r--r--   0        0        0     1512 2024-01-18 08:25:41.645930 introspection-1.7.9/introspection/exceptions.py
--rw-r--r--   0        0        0     2024 2024-01-18 09:17:05.536726 introspection-1.7.9/introspection/hazmat.py
--rw-r--r--   0        0        0    21330 2024-01-18 23:04:47.391839 introspection-1.7.9/introspection/misc.py
--rw-r--r--   0        0        0    10865 2024-01-19 10:46:29.091164 introspection-1.7.9/introspection/misc2.py
--rw-r--r--   0        0        0     5802 2024-01-18 08:25:40.454662 introspection-1.7.9/introspection/parameter.py
--rw-r--r--   0        0        0    40316 2024-01-18 19:55:08.715620 introspection-1.7.9/introspection/signature_.py
--rw-r--r--   0        0        0     1966 2024-01-18 20:15:05.854391 introspection-1.7.9/introspection/types.py
--rw-r--r--   0        0        0      199 2024-01-19 09:03:29.591495 introspection-1.7.9/introspection/typing/__init__.py
--rw-r--r--   0        0        0      163 2024-01-23 19:52:21.080258 introspection-1.7.9/introspection/typing/_compat.py
--rw-r--r--   0        0        0     2969 2024-01-23 21:51:57.641256 introspection-1.7.9/introspection/typing/_utils.py
--rw-r--r--   0        0        0      365 2024-01-18 20:14:58.591707 introspection-1.7.9/introspection/typing/i_hate_circular_imports.py
--rw-r--r--   0        0        0     9488 2024-01-23 22:09:32.275136 introspection-1.7.9/introspection/typing/instance_check.py
--rw-r--r--   0        0        0    35436 2024-01-19 22:48:36.960074 introspection-1.7.9/introspection/typing/introspection.py
--rw-r--r--   0        0        0    19030 2024-01-31 11:16:09.982816 introspection-1.7.9/introspection/typing/misc.py
--rw-r--r--   0        0        0     4486 2024-01-23 22:19:01.712250 introspection-1.7.9/introspection/typing/subtype_check.py
--rw-r--r--   0        0        0     7831 2024-01-19 21:00:24.103910 introspection-1.7.9/introspection/typing/type_compat.py
--rw-r--r--   0        0        0     2400 2024-01-19 09:02:05.166193 introspection-1.7.9/introspection/typing/type_info.py
--rw-r--r--   0        0        0      667 2022-12-27 16:52:40.582428 introspection-1.7.9/pyproject.toml
--rw-r--r--   0        0        0      702 2024-01-18 23:02:11.112358 introspection-1.7.9/tests/conftest.py
--rw-r--r--   0        0        0      998 2024-01-18 08:25:47.069324 introspection-1.7.9/tests/test_argument_bundle.py
--rw-r--r--   0        0        0     3863 2024-01-18 23:12:45.882041 introspection-1.7.9/tests/test_bound_arguments.py
--rw-r--r--   0        0        0     3620 2024-01-19 09:53:41.199622 introspection-1.7.9/tests/test_call_frame.py
--rw-r--r--   0        0        0      991 2023-09-26 21:21:15.576128 introspection-1.7.9/tests/test_call_stack.py
--rw-r--r--   0        0        0    14394 2024-01-18 23:17:45.860907 introspection-1.7.9/tests/test_class_functions.py
--rw-r--r--   0        0        0      300 2022-07-24 08:46:16.677569 introspection-1.7.9/tests/test_deprecations.py
--rw-r--r--   0        0        0     4548 2024-01-18 23:16:27.846736 introspection-1.7.9/tests/test_dunder_functions.py
--rw-r--r--   0        0        0    11193 2024-01-19 11:49:42.874121 introspection-1.7.9/tests/test_misc_functions.py
--rw-r--r--   0        0        0     3594 2022-12-27 16:52:40.434500 introspection-1.7.9/tests/test_parameter.py
--rw-r--r--   0        0        0    13881 2024-01-18 23:14:31.422176 introspection-1.7.9/tests/test_signature.py
--rw-r--r--   0        0        0    28366 2024-01-19 22:47:49.967274 introspection-1.7.9/tests/test_typing/test_introspection.py
--rw-r--r--   0        0        0     9027 2024-01-30 20:36:10.077258 introspection-1.7.9/tests/test_typing/test_misc.py
--rw-r--r--   0        0        0     3382 2024-01-23 22:15:36.047839 introspection-1.7.9/tests/test_typing/test_type_checks.py
--rw-r--r--   0        0        0     4910 2023-01-15 21:33:46.002055 introspection-1.7.9/tests/test_typing/test_type_compat.py
--rw-r--r--   0        0        0      815 2024-01-19 10:45:51.475169 introspection-1.7.9/tox.ini
--rw-r--r--   0        0        0     1132 1970-01-01 00:00:00.000000 introspection-1.7.9/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2019-10-05 20:23:15.010707 introspection-1.8/LICENSE
+-rwxr-xr-x   0        0        0      423 2020-06-21 16:21:23.702593 introspection-1.8/README.md
+-rwxr-xr-x   0        0        0        1 2018-02-07 23:45:28.000000 introspection-1.8/docs/.nojekyll
+-rwxr-xr-x   0        0        0     8370 2022-01-11 18:29:27.165570 introspection-1.8/docs/Makefile
+-rwxr-xr-x   0        0        0    50309 2023-09-27 09:04:29.286431 introspection-1.8/docs/build/doctrees/call_stack.doctree
+-rwxr-xr-x   0        0        0   113126 2023-09-27 09:04:29.472424 introspection-1.8/docs/build/doctrees/classes.doctree
+-rwxr-xr-x   0        0        0   123722 2023-09-27 09:04:29.603457 introspection-1.8/docs/build/doctrees/dundermethods.doctree
+-rwxr-xr-x   0        0        0   150280 2023-09-27 09:04:30.168939 introspection-1.8/docs/build/doctrees/function_signatures.doctree
+-rwxr-xr-x   0        0        0     4054 2023-09-27 09:04:30.173941 introspection-1.8/docs/build/doctrees/index.doctree
+-rwxr-xr-x   0        0        0   112020 2023-09-27 09:04:30.356611 introspection-1.8/docs/build/doctrees/misc.doctree
+-rwxr-xr-x   0        0        0   132622 2022-07-28 05:12:16.888430 introspection-1.8/docs/build/doctrees/typing.doctree
+-rwxr-xr-x   0        0        0      234 2022-07-28 05:12:17.627586 introspection-1.8/docs/build/html/.buildinfo
+-rwxr-xr-x   0        0        0     4418 2022-06-30 11:20:55.284834 introspection-1.8/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rwxr-xr-x   0        0        0    16132 2022-07-28 05:12:17.556578 introspection-1.8/docs/build/html/_static/basic.css
+-rwxr-xr-x   0        0        0      313 2022-01-14 19:00:26.466660 introspection-1.8/docs/build/html/_static/check-solid.svg
+-rwxr-xr-x   0        0        0     9031 2022-01-14 19:00:26.467661 introspection-1.8/docs/build/html/_static/clipboard.min.js
+-rwxr-xr-x   0        0        0      434 2022-01-14 19:00:26.467661 introspection-1.8/docs/build/html/_static/copy-button.svg
+-rwxr-xr-x   0        0        0     1754 2022-01-14 19:00:26.470668 introspection-1.8/docs/build/html/_static/copybutton.css
+-rwxr-xr-x   0        0        0     6716 2022-07-28 05:12:17.625587 introspection-1.8/docs/build/html/_static/copybutton.js
+-rwxr-xr-x   0        0        0     2198 2022-01-14 19:00:26.473668 introspection-1.8/docs/build/html/_static/copybutton_funcs.js
+-rwxr-xr-x   0        0        0     8171 2022-06-30 11:20:55.286835 introspection-1.8/docs/build/html/_static/doctools.js
+-rwxr-xr-x   0        0        0      435 2022-07-28 05:12:17.566583 introspection-1.8/docs/build/html/_static/documentation_options.js
+-rwxr-xr-x   0        0        0     2296 2022-01-11 21:41:53.887944 introspection-1.8/docs/build/html/_static/favicon.svg
+-rwxr-xr-x   0        0        0      286 2022-01-11 18:34:47.961414 introspection-1.8/docs/build/html/_static/file.png
+-rwxr-xr-x   0        0        0   287630 2022-01-11 18:34:47.963413 introspection-1.8/docs/build/html/_static/jquery-3.5.1.js
+-rwxr-xr-x   0        0        0   288580 2022-06-30 11:20:55.289835 introspection-1.8/docs/build/html/_static/jquery-3.6.0.js
+-rwxr-xr-x   0        0        0    89501 2022-06-30 11:20:55.290835 introspection-1.8/docs/build/html/_static/jquery.js
+-rwxr-xr-x   0        0        0     4957 2022-07-28 05:12:17.575582 introspection-1.8/docs/build/html/_static/language_data.js
+-rwxr-xr-x   0        0        0       90 2022-01-11 18:34:47.966416 introspection-1.8/docs/build/html/_static/minus.png
+-rwxr-xr-x   0        0        0     9096 2022-01-15 08:34:05.001989 introspection-1.8/docs/build/html/_static/nightsky.css
+-rwxr-xr-x   0        0        0    12357 2022-01-15 11:08:27.758930 introspection-1.8/docs/build/html/_static/nightsky.styl
+-rwxr-xr-x   0        0        0       85 2021-03-08 19:37:10.079040 introspection-1.8/docs/build/html/_static/package-lock.json
+-rwxr-xr-x   0        0        0        3 2021-03-08 19:37:10.080250 introspection-1.8/docs/build/html/_static/package.json
+-rwxr-xr-x   0        0        0       90 2022-01-11 18:34:47.967415 introspection-1.8/docs/build/html/_static/plus.png
+-rwxr-xr-x   0        0        0     5119 2022-01-14 23:24:17.967774 introspection-1.8/docs/build/html/_static/pygments-cobalt2.css
+-rwxr-xr-x   0        0        0     4919 2022-07-28 05:12:17.543568 introspection-1.8/docs/build/html/_static/pygments.css
+-rwxr-xr-x   0        0        0     4633 2022-07-28 05:12:17.544569 introspection-1.8/docs/build/html/_static/pygments_dark.css
+-rwxr-xr-x   0        0        0    17088 2022-06-30 11:20:55.294836 introspection-1.8/docs/build/html/_static/searchtools.js
+-rwxr-xr-x   0        0        0     7067 2022-07-28 05:12:17.664594 introspection-1.8/docs/build/html/_static/theme_switcher.js
+-rwxr-xr-x   0        0        0    68420 2022-01-11 18:34:47.969416 introspection-1.8/docs/build/html/_static/underscore-1.13.1.js
+-rwxr-xr-x   0        0        0    19530 2022-01-11 18:34:47.970415 introspection-1.8/docs/build/html/_static/underscore.js
+-rwxr-xr-x   0        0        0    19915 2022-07-28 05:12:17.083464 introspection-1.8/docs/build/html/call_stack.html
+-rwxr-xr-x   0        0        0    48881 2022-07-28 05:12:17.141485 introspection-1.8/docs/build/html/classes.html
+-rwxr-xr-x   0        0        0    61201 2022-07-28 05:12:17.254511 introspection-1.8/docs/build/html/dundermethods.html
+-rwxr-xr-x   0        0        0    62670 2022-07-28 05:12:17.327518 introspection-1.8/docs/build/html/function_signatures.html
+-rwxr-xr-x   0        0        0    24122 2022-07-28 05:12:17.499557 introspection-1.8/docs/build/html/genindex.html
+-rwxr-xr-x   0        0        0     4965 2022-07-28 05:12:17.340521 introspection-1.8/docs/build/html/index.html
+-rwxr-xr-x   0        0        0    54576 2022-07-28 05:12:17.404537 introspection-1.8/docs/build/html/misc.html
+-rwxr-xr-x   0        0        0     1394 2022-07-28 05:12:17.632588 introspection-1.8/docs/build/html/objects.inv
+-rwxr-xr-x   0        0        0     5636 2022-07-28 05:12:17.525572 introspection-1.8/docs/build/html/py-modindex.html
+-rwxr-xr-x   0        0        0     3786 2022-07-28 05:12:17.541568 introspection-1.8/docs/build/html/search.html
+-rwxr-xr-x   0        0        0    19468 2022-07-28 05:12:17.629587 introspection-1.8/docs/build/html/searchindex.js
+-rwxr-xr-x   0        0        0    62944 2022-07-28 05:12:17.477563 introspection-1.8/docs/build/html/typing.html
+-rwxr-xr-x   0        0        0      173 2018-02-07 20:12:32.000000 introspection-1.8/docs/index.html
+-rwxr-xr-x   0        0        0     7793 2018-02-07 15:05:16.000000 introspection-1.8/docs/make.bat
+-rwxr-xr-x   0        0        0      176 2020-06-21 11:11:00.000000 introspection-1.8/docs/source/call_stack.rst
+-rwxr-xr-x   0        0        0      144 2020-06-21 11:52:08.000000 introspection-1.8/docs/source/classes.rst
+-rwxr-xr-x   0        0        0     3889 2022-01-14 19:30:26.076283 introspection-1.8/docs/source/conf.py
+-rwxr-xr-x   0        0        0     1605 2020-07-11 05:40:06.000000 introspection-1.8/docs/source/dundermethods.rst
+-rwxr-xr-x   0        0        0     2296 2022-01-11 21:41:53.887944 introspection-1.8/docs/source/favicon.svg
+-rwxr-xr-x   0        0        0      579 2022-01-13 20:53:53.587095 introspection-1.8/docs/source/function_signatures.rst
+-rwxr-xr-x   0        0        0      496 2020-07-11 05:40:06.000000 introspection-1.8/docs/source/index.rst
+-rwxr-xr-x   0        0        0      210 2022-01-15 11:18:12.735064 introspection-1.8/docs/source/misc.rst
+-rwxr-xr-x   0        0        0     1672 2022-07-26 08:59:09.533795 introspection-1.8/docs/source/typing.rst
+-rwxr-xr-x   0        0        0      721 2024-04-27 18:19:16.645374 introspection-1.8/introspection/__init__.py
+-rwxr-xr-x   0        0        0     1668 2024-01-18 08:25:36.597619 introspection-1.8/introspection/_utils.py
+-rwxr-xr-x   0        0        0     1306 2024-01-18 08:25:42.808139 introspection-1.8/introspection/argument_bundle.py
+-rwxr-xr-x   0        0        0     5229 2024-04-22 15:28:15.662005 introspection-1.8/introspection/bound_arguments.py
+-rwxr-xr-x   0        0        0     5388 2024-01-18 23:04:07.035404 introspection-1.8/introspection/call_frame.py
+-rwxr-xr-x   0        0        0     2531 2023-12-12 21:17:22.152565 introspection-1.8/introspection/call_stack.py
+-rwxr-xr-x   0        0        0    19314 2024-03-30 19:16:42.066223 introspection-1.8/introspection/classes.py
+-rwxr-xr-x   0        0        0      718 2022-12-07 10:42:15.146932 introspection-1.8/introspection/dunder.py
+-rwxr-xr-x   0        0        0    16502 2024-01-18 23:07:13.842401 introspection-1.8/introspection/dundermethods.py
+-rwxr-xr-x   0        0        0     6021 2024-03-27 15:55:39.084807 introspection-1.8/introspection/errors.py
+-rwxr-xr-x   0        0        0     1512 2024-01-18 08:25:41.645930 introspection-1.8/introspection/exceptions.py
+-rwxr-xr-x   0        0        0     2024 2024-01-18 09:17:05.536726 introspection-1.8/introspection/hazmat.py
+-rwxr-xr-x   0        0        0      504 2024-03-03 07:55:07.701629 introspection-1.8/introspection/mark.py
+-rwxr-xr-x   0        0        0    21932 2024-04-12 07:33:59.368217 introspection-1.8/introspection/misc.py
+-rwxr-xr-x   0        0        0    10853 2024-04-22 15:31:00.973509 introspection-1.8/introspection/misc2.py
+-rwxr-xr-x   0        0        0     6051 2024-03-27 15:55:56.452781 introspection-1.8/introspection/parameter.py
+-rwxr-xr-x   0        0        0    23052 2024-04-22 15:31:32.700262 introspection-1.8/introspection/signature_.py
+-rwxr-xr-x   0        0        0    21193 2024-03-01 08:10:43.356161 introspection-1.8/introspection/signature_db.py
+-rwxr-xr-x   0        0        0     2036 2024-04-12 07:30:53.803927 introspection-1.8/introspection/types.py
+-rwxr-xr-x   0        0        0      220 2024-03-10 10:49:14.643553 introspection-1.8/introspection/typing/__init__.py
+-rwxr-xr-x   0        0        0      163 2024-01-23 19:52:21.080258 introspection-1.8/introspection/typing/_compat.py
+-rwxr-xr-x   0        0        0     3014 2024-03-27 16:00:41.694182 introspection-1.8/introspection/typing/_utils.py
+-rwxr-xr-x   0        0        0      365 2024-01-18 20:14:58.591707 introspection-1.8/introspection/typing/i_hate_circular_imports.py
+-rwxr-xr-x   0        0        0     9335 2024-03-27 16:07:53.492118 introspection-1.8/introspection/typing/instance_check.py
+-rwxr-xr-x   0        0        0    35545 2024-03-27 16:07:34.319897 introspection-1.8/introspection/typing/introspection.py
+-rwxr-xr-x   0        0        0    19661 2024-04-22 15:37:54.671244 introspection-1.8/introspection/typing/misc.py
+-rwxr-xr-x   0        0        0      836 2024-03-10 19:27:23.218173 introspection-1.8/introspection/typing/misc2.py
+-rwxr-xr-x   0        0        0     4580 2024-03-27 15:59:52.850405 introspection-1.8/introspection/typing/subtype_check.py
+-rwxr-xr-x   0        0        0     7844 2024-03-27 16:08:13.814762 introspection-1.8/introspection/typing/type_compat.py
+-rwxr-xr-x   0        0        0     2377 2024-03-27 15:57:57.630293 introspection-1.8/introspection/typing/type_info.py
+-rwxr-xr-x   0        0        0      667 2022-12-27 16:52:40.582428 introspection-1.8/pyproject.toml
+-rwxr-xr-x   0        0        0      702 2024-01-18 23:02:11.112358 introspection-1.8/tests/conftest.py
+-rwxr-xr-x   0        0        0      998 2024-01-18 08:25:47.069324 introspection-1.8/tests/test_argument_bundle.py
+-rwxr-xr-x   0        0        0     3863 2024-01-18 23:12:45.882041 introspection-1.8/tests/test_bound_arguments.py
+-rwxr-xr-x   0        0        0     3620 2024-01-19 09:53:41.199622 introspection-1.8/tests/test_call_frame.py
+-rwxr-xr-x   0        0        0      991 2023-09-26 21:21:15.576128 introspection-1.8/tests/test_call_stack.py
+-rwxr-xr-x   0        0        0    14394 2024-01-18 23:17:45.860907 introspection-1.8/tests/test_class_functions.py
+-rwxr-xr-x   0        0        0      300 2022-07-24 08:46:16.677569 introspection-1.8/tests/test_deprecations.py
+-rwxr-xr-x   0        0        0     4548 2024-01-18 23:16:27.846736 introspection-1.8/tests/test_dunder_functions.py
+-rwxr-xr-x   0        0        0    11300 2024-04-12 07:35:04.751265 introspection-1.8/tests/test_misc_functions.py
+-rwxr-xr-x   0        0        0     3594 2022-12-27 16:52:40.434500 introspection-1.8/tests/test_parameter.py
+-rwxr-xr-x   0        0        0    14880 2024-03-03 07:40:40.287143 introspection-1.8/tests/test_signature.py
+-rwxr-xr-x   0        0        0    28366 2024-01-19 22:47:49.967274 introspection-1.8/tests/test_typing/test_introspection.py
+-rwxr-xr-x   0        0        0     9315 2024-04-17 21:17:42.054685 introspection-1.8/tests/test_typing/test_misc.py
+-rwxr-xr-x   0        0        0     3386 2024-03-03 07:41:18.271471 introspection-1.8/tests/test_typing/test_type_checks.py
+-rwxr-xr-x   0        0        0     4910 2023-01-15 21:33:46.002055 introspection-1.8/tests/test_typing/test_type_compat.py
+-rwxr-xr-x   0        0        0      815 2024-01-19 10:45:51.475169 introspection-1.8/tox.ini
+-rw-r--r--   0        0        0     1130 1970-01-01 00:00:00.000000 introspection-1.8/PKG-INFO
```

### Comparing `introspection-1.7.9/LICENSE` & `introspection-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/Makefile` & `introspection-1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/doctrees/call_stack.doctree` & `introspection-1.8/docs/build/doctrees/call_stack.doctree`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/doctrees/classes.doctree` & `introspection-1.8/docs/build/doctrees/classes.doctree`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/doctrees/dundermethods.doctree` & `introspection-1.8/docs/build/doctrees/dundermethods.doctree`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/doctrees/function_signatures.doctree` & `introspection-1.8/docs/build/doctrees/function_signatures.doctree`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/doctrees/index.doctree` & `introspection-1.8/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/doctrees/misc.doctree` & `introspection-1.8/docs/build/doctrees/misc.doctree`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/doctrees/typing.doctree` & `introspection-1.8/docs/build/doctrees/typing.doctree`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `introspection-1.8/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/basic.css` & `introspection-1.8/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/clipboard.min.js` & `introspection-1.8/docs/build/html/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/copybutton.css` & `introspection-1.8/docs/build/html/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/copybutton.js` & `introspection-1.8/docs/build/html/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/copybutton_funcs.js` & `introspection-1.8/docs/build/html/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/doctools.js` & `introspection-1.8/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/favicon.svg` & `introspection-1.8/docs/build/html/_static/favicon.svg`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/jquery-3.5.1.js` & `introspection-1.8/docs/build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/jquery-3.6.0.js` & `introspection-1.8/docs/build/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/jquery.js` & `introspection-1.8/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/language_data.js` & `introspection-1.8/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/nightsky.css` & `introspection-1.8/docs/build/html/_static/nightsky.css`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/nightsky.styl` & `introspection-1.8/docs/build/html/_static/nightsky.styl`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/pygments-cobalt2.css` & `introspection-1.8/docs/build/html/_static/pygments-cobalt2.css`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/pygments.css` & `introspection-1.8/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/pygments_dark.css` & `introspection-1.8/docs/build/html/_static/pygments_dark.css`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/searchtools.js` & `introspection-1.8/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/theme_switcher.js` & `introspection-1.8/docs/build/html/_static/theme_switcher.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/underscore-1.13.1.js` & `introspection-1.8/docs/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/_static/underscore.js` & `introspection-1.8/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/call_stack.html` & `introspection-1.8/docs/build/html/call_stack.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/classes.html` & `introspection-1.8/docs/build/html/classes.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/dundermethods.html` & `introspection-1.8/docs/build/html/dundermethods.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/function_signatures.html` & `introspection-1.8/docs/build/html/function_signatures.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/genindex.html` & `introspection-1.8/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/index.html` & `introspection-1.8/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/misc.html` & `introspection-1.8/docs/build/html/misc.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/objects.inv` & `introspection-1.8/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/py-modindex.html` & `introspection-1.8/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/search.html` & `introspection-1.8/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/searchindex.js` & `introspection-1.8/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/build/html/typing.html` & `introspection-1.8/docs/build/html/typing.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/make.bat` & `introspection-1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/source/conf.py` & `introspection-1.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/source/dundermethods.rst` & `introspection-1.8/docs/source/dundermethods.rst`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/source/favicon.svg` & `introspection-1.8/docs/source/favicon.svg`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/source/function_signatures.rst` & `introspection-1.8/docs/source/function_signatures.rst`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/docs/source/typing.rst` & `introspection-1.8/docs/source/typing.rst`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/introspection/__init__.py` & `introspection-1.8/introspection/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 New and improved introspection functions
 """
 
-__version__ = "1.7.9"
+__version__ = "1.8"
 
 from .parameter import *
 from .signature_ import *
 from .argument_bundle import *
 from .bound_arguments import *
 from .call_stack import *
 from .call_frame import *
@@ -16,14 +16,15 @@
 from .dundermethods import *
 from .misc import *
 from .misc2 import *
 from .hazmat import *
 
 from . import dunder
 from . import errors
+from . import mark
 from . import types
 
 # Make sure a ``from introspection import *`` doesn't import the ``typing``
 # submodule
 import types as types_
 
 __all__ = [
```

### Comparing `introspection-1.7.9/introspection/_utils.py` & `introspection-1.8/introspection/_utils.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/introspection/argument_bundle.py` & `introspection-1.8/introspection/argument_bundle.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/introspection/bound_arguments.py` & `introspection-1.8/introspection/bound_arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     .. versionadded:: 1.4
     .. versionchanged: 1.5
         Now implements the :class:`~collections.abc.MutableMapping` interface.
     """
 
     __slots__ = ()
 
-    signature: "signature_.Signature"
+    signature: "signature_.Signature"  # type: ignore
 
     @classmethod
     def from_bound_arguments(cls, bound_args: inspect.BoundArguments) -> Self:
         """
         Creates a new ``BoundArguments`` instance from a
         :class:`inspect.BoundArguments` instance.
```

### Comparing `introspection-1.7.9/introspection/call_frame.py` & `introspection-1.8/introspection/call_frame.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/introspection/call_stack.py` & `introspection-1.8/introspection/call_stack.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/introspection/classes.py` & `introspection-1.8/introspection/classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import inspect
 import functools
 from typing import *
 from typing_extensions import *
 
 import sentinel
 
+from .mark import FORWARDS_ARGUMENTS, forwards_arguments
 from .misc import static_vars, is_abstract, static_mro
 from .errors import *
 from .types import Slot, Function, Class
 
 __all__ = [
     "iter_subclasses",
     "get_subclasses",
@@ -276,17 +277,17 @@
     :param thing: The thing whose metadata should be updated
     :param cls: The class to copy the metadata from
     :param name: The name to rename ``thing`` to
     """
     methods: List[Union[type, Function]]
 
     if isinstance(thing, (classmethod, staticmethod)):
-        methods = [thing.__func__]
+        methods = [thing.__func__]  # type: ignore
     elif isinstance(thing, property):
-        methods = [method for method in (thing.fget, thing.fset, thing.fdel) if method is not None]
+        methods = [method for method in (thing.fget, thing.fset, thing.fdel) if method is not None]  # type: ignore
     else:
         methods = [thing]
 
     for method in methods:
         if name is None:
             method_name = method.__name__
         else:
@@ -331,28 +332,45 @@
 
     if method_type is not None:
         method = method_type(method)  # type: ignore
 
     setattr(cls, method_name, method)
 
 
+@overload
 def wrap_method(
-    method: Callable[..., Any],
     cls: type,
+    method: Callable[..., object],
+    name: Optional[str] = None,
+    method_type: Union[None, Type[staticmethod], Type[classmethod]] = auto,  # type: ignore
+) -> None: ...
+
+
+@overload  # Deprecated signature
+def wrap_method(
+    method: Callable[..., object],
+    cls: type,
+    name: Optional[str] = None,
+    method_type: Union[None, Type[staticmethod], Type[classmethod]] = auto,  # type: ignore
+) -> None: ...
+
+
+def wrap_method(  # type: ignore[wtf]
+    cls: Union[type, Callable[..., object]],
+    method: Union[type, Callable[..., object]],
     name: Optional[str] = None,
     method_type: Union[None, Type[staticmethod], Type[classmethod]] = auto,  # type: ignore
 ) -> None:
     r"""
-    Adds ``method`` to ``cls``\ 's namespace under the given ``name``,
-    wrapping the existing method (if one exists).
+    Adds ``method`` to ``cls``\ 's namespace under the given ``name``, wrapping the existing method
+    (if one exists).
 
-    The replaced method will be passed in as the first positional argument
-    (even before the implicit ``self``). If the class previously didn't
-    implement this method, an appropriate dummy method will be passed
-    in instead, which merely sends the call further up the MRO.
+    The replaced method will be passed in as the first positional argument (even before the implicit
+    ``self``). If the class previously didn't implement this method, an appropriate dummy method
+    will be passed in instead, which merely sends the call further up the MRO.
 
     ``method_type`` has the same meaning as it does in :func:`~introspection.add_method_to_class`.
 
     Example::
 
         class Foo:
             def __init__(self, foo):
@@ -366,21 +384,20 @@
             print('Initialized instance:', self)
 
         wrap_method(custom_init, Foo, '__init__')
 
         Foo(5)  # prints "Initialized instance: <Foo object with foo=5>"
 
     .. note::
-        Adding a ``__new__`` method to a class can lead to unexpected
-        problems because of the way ``object.__new__`` works.
+        Adding a ``__new__`` method to a class can lead to unexpected problems because of the way
+        ``object.__new__`` works.
 
-        If a class doesn't implement a ``__new__`` method at all,
-        ``object.__new__`` silently discards any arguments it receives.
-        But if a class does implement a custom ``__new__`` method,
-        passing arguments into ``object.__new__`` will throw an exception::
+        If a class doesn't implement a ``__new__`` method at all, ``object.__new__`` silently
+        discards any arguments it receives. But if a class does implement a custom ``__new__``
+        method, passing arguments into ``object.__new__`` will throw an exception::
 
             class ThisWorks:
                 def __init__(self, some_arg):
                     pass
 
             class ThisDoesntWork:
                 def __new__(cls, *args, **kwargs):
@@ -388,36 +405,33 @@
 
                 def __init__(self, some_arg):
                     pass
 
             ThisWorks(5)  # works
             ThisDoesntWork(5)  # throws TypeError: object.__new__() takes exactly one argument
 
-        This is why, when this function is used to add a ``__new__``
-        method to a class that previously didn't have one, it
-        automatically generates a dummy ``__new__`` that *attempts*
-        to figure out whether it should forward its arguments to
-        the base class's ``__new__`` method or not. This is why
-        the following code will work just fine::
+        This is why, when this function is used to add a ``__new__`` method to a class that
+        previously didn't have one, it automatically generates a dummy ``__new__`` that *attempts*
+        to figure out whether it should forward its arguments to the base class's ``__new__`` method
+        or not. This is why the following code will work just fine::
 
             class ThisWorks:
                 def __init__(self, some_arg):
                     pass
 
             def __new__(original_new, cls, *args, **kwargs):
                 return original_new(cls, *args, **kwargs)
 
             wrap_method(__new__, ThisWorks)
 
             ThisWorks(5)  # works!
 
-        However, it is impossible to always correctly figure out
-        if the arguments should be passed on or not. If there is
-        another ``__new__`` method that passes on its arguments,
-        things will go wrong::
+        However, it is impossible to always correctly figure out if the arguments should be passed
+        on or not. If there is another ``__new__`` method that passes on its arguments, things will
+        go wrong::
 
             class Parent:
                 def __init__(self, some_arg):
                     pass
 
             class Child(Parent):
                 def __new__(cls, *args, **kwargs):
@@ -427,34 +441,43 @@
                 return original_new(cls, *args, **kwargs)
 
             wrap_method(__new__, Parent)
 
             Parent(5)  # works!
             Child(5)  # throws TypeError
 
-        In such a scenario, the method sees that ``Child.__new__``
-        exists, and therefore it is ``Child.__new__``\ 's responsibility
-        to handle the arguments correctly. It should consume all the
-        arguments, but doesn't, so an exception is raised.
-
-        As a workaround, you can mark ``Child.__new__`` as a
-        method that forwards its arguments. This is done by
-        setting its ``_forwards_args`` attribute to ``True``::
+        In such a scenario, the method sees that ``Child.__new__`` exists, and therefore it is
+        ``Child.__new__``\ 's responsibility to handle the arguments correctly. It should consume
+        all the arguments, but doesn't, so an exception is raised.
+
+        As a workaround, you can mark ``Child.__new__`` as a method that forwards its arguments.
+        This is done by decorating it with ``@introspection.mark.forwards_arguments`::
+
+            @introspection.mark.forwards_arguments
+            def __new__(original_new, cls, *args, **kwargs):
+                return original_new(cls, *args, **kwargs)
 
-            Child.__new__._forwards_args = True
+            wrap_method(__new__, Parent)
 
             Child(5)  # works!
 
     .. versionadded:: 1.3
+    .. versionchanged:: 1.7.13
+        Swapped the first two parameters. Passing the function as the first argument is still
+        possible, but deprecated.
 
     :param method: The method to add to the class
     :param cls: The class to which to add the method
     :param name: The name under which the method is registered in the class namespace
     :param method_type: One of :class:`staticmethod`, :class:`classmethod`, or ``None`` (or omitted)
     """
+    # Deprecated call signature: Swap the first two arguments
+    if not isinstance(cls, type):
+        cls, method = method, cls
+
     if not isinstance(cls, type):
         raise InvalidArgumentType("cls", cls, type)
 
     if name is None:
         name = method.__name__
 
     if method_type is auto:
@@ -509,60 +532,53 @@
     return original_method, wrap_original
 
 
 def _make_original_new_method(cls: type):
     def original_method(class_: type, *args, **kwargs):
         super_new = super(cls, class_).__new__  # type: ignore[wtf]
 
-        # object.__new__ accepts no arguments if the class
-        # implements its own __new__ method, so we must
-        # take care to not pass it any if this is the only
-        # __new__ method in the whole MRO. But if there's
-        # no __init__ method either, then receiving any
-        # arguments should results in an exception.
-
-        # If super_new is not object.__new__, then it's
-        # their responsibility to deal with the arguments.
-        # In this case, we always forward them.
-        # If the class implements no __init__ method at all,
-        # we forward them as well.
+        # object.__new__ accepts no arguments if the class implements its own __new__ method, so we
+        # must take care to not pass it any if this is the only __new__ method in the whole MRO. But
+        # if there's no __init__ method either, then receiving any arguments should results in an
+        # exception.
+
+        # If super_new is not object.__new__, then it's their responsibility to deal with the
+        # arguments. In this case, we always forward them. If the class implements no __init__
+        # method at all, we forward them as well.
         if super_new is object.__new__ and class_.__init__ is not object.__init__:
-            # At this point, we know that the next __new__
-            # method in the MRO is object.__new__, so we
-            # must decide how to handle the arguments.
-
-            # If there's a __new__ method in the MRO that
-            # is not object.__new__ and is not marked as
-            # ._forwards_args, then that method should've
-            # consumed all the arguments.
+            # At this point, we know that the next __new__ method in the MRO is object.__new__, so
+            # we must decide how to handle the arguments.
+
+            # If there's a __new__ method in the MRO that is not object.__new__ and is not marked as
+            # `@forwards_arguments`, then that method should've consumed all the arguments.
             forward_args = False
 
             for c in static_mro(class_):  # pragma: no branch
                 if c is object:
                     break
 
                 try:
                     # __new__ is always wrapped in `staticmethod`
                     new = static_vars(c)["__new__"].__func__  # type: ignore
                 except KeyError:
                     continue
 
-                if getattr(new, "_forwards_args", False):
+                if new in FORWARDS_ARGUMENTS:
+                    continue
+
+                if getattr(new, "_forwards_args", False):  # Legacy version of `@forwards_arguments`
                     continue
 
                 forward_args = True
                 break
 
             if not forward_args:
                 args = ()
                 kwargs = {}
 
         return super_new(class_, *args, **kwargs)  # type: ignore
 
-    # We're just gonna assume that the user is going to properly
-    # call our original_method, because if not, they should've
-    # just used add_method_to_class instead.
-    def wrap_original(func):
-        func._forwards_args = True
-        return func
+    # We're just gonna assume that the user is going to properly call our original_method, because
+    # if not, they should've just used `add_method_to_class` instead.
+    wrap_original = forwards_arguments
 
     return original_method, wrap_original
```

### Comparing `introspection-1.7.9/introspection/dunder.py` & `introspection-1.8/introspection/dunder.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/introspection/dundermethods.py` & `introspection-1.8/introspection/dundermethods.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/introspection/errors.py` & `introspection-1.8/introspection/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
             f"TypeVar {self.type_var} of {self.base_type!r} doesn't have a concrete value in"
             f" {self.type!r}; it is set to {self.final_var!r}"
         )
 
 
 class CannotResolveForwardref(Error, ValueError):
     forward_ref: ForwardReference
-    context: ForwardRefContext
+    context: Optional[ForwardRefContext]
 
     def __str__(self) -> str:
         return f"Cannot resolve forward reference {self.forward_ref!r} in context {self.context!r}"
 
 
 class NoTypingEquivalent(Error, ValueError):
     type: type
```

### Comparing `introspection-1.7.9/introspection/exceptions.py` & `introspection-1.8/introspection/exceptions.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/introspection/hazmat.py` & `introspection-1.8/introspection/hazmat.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/introspection/misc.py` & `introspection-1.8/introspection/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import builtins
 import copy
 import inspect
 import sys
 import types
+import warnings
 
 from collections import defaultdict, deque
 from typing import *
 from typing_extensions import ParamSpec, TypeAlias
 
 from .errors import *
-from .types import ObjectWithQualname
+from .types import ObjectWithQualname, Case
 
 __all__ = [
     "common_ancestor",
     "create_class",
     "resolve_bases",
     "static_vars",
     "static_copy",
@@ -31,15 +32,14 @@
     "snake_to_camel",
     "detect_case",
     "convert_case",
 ]
 
 P = ParamSpec("P")
 T = TypeVar("T")
-Case = Literal["snake", "upper snake", "camel", "pascal", "kebab", "upper kebab"]
 
 
 TYPE_GET_DICT = cast(Callable[[type], Mapping[str, Any]], type.__dict__["__dict__"].__get__)  # type: ignore
 TYPE_GET_MRO = cast(Callable[[type], Tuple[type, ...]], type.__dict__["__mro__"].__get__)  # type: ignore
 
 
 def create_class(
@@ -569,15 +569,22 @@
 
         >>> camel_to_snake('FooBar')
         'foo_bar'
         >>> camel_to_snake('HTTPAdapater')
         'http_adapter'
 
     .. versionadded:: 1.5
+    .. deprecated:: 1.7.12
+        Use :func:`convert_case` instead.
     """
+    warnings.warn(
+        "The `camel_to_snake` function is deprecated in favor of `convert_case`",
+        DeprecationWarning,
+    )
+
     chars: List[str] = []
     last_char_was_upper = True
 
     for i, char in enumerate(camel):
         is_upper = char.isupper()
 
         if is_upper:
@@ -603,15 +610,22 @@
 
         >>> snake_to_camel('foo_bar')
         'FooBar'
         >>> snake_to_camel('http_adapter')
         'HttpAdapter'
 
     .. versionadded:: 1.5
+    .. deprecated:: 1.7.12
+        Use :func:`convert_case` instead.
     """
+    warnings.warn(
+        "The `snake_to_camel` function is deprecated in favor of `convert_case`",
+        DeprecationWarning,
+    )
+
     chars: List[str] = []
     last_char_was_underscore = True
 
     for char in snake:
         if char == "_":
             last_char_was_underscore = True
             continue
@@ -621,62 +635,72 @@
             last_char_was_underscore = False
 
         chars.append(char)
 
     return "".join(chars)
 
 
-def detect_case(name: str) -> Case:
+def detect_case(name: str) -> Union[Case, Literal["mixed"]]:
     """
     Detects the case of a name, for example::
 
         >>> detect_case('foo_bar')
         'snake'
         >>> detect_case('FooBar')
         'pascal'
+        >>> detect_case('foo_bar-qux')
+        'mixed'
     """
-    if name[0].islower():
-        if "-" in name:
-            return "kebab"
-        elif name.islower():
-            return "snake"
-        else:
-            return "camel"
+    has_upper = has_lower = False
+    has_dash = has_underscore = has_whitespace = False
 
-    if "-" in name:
-        return "upper kebab"
-    elif "_" in name:
-        return "upper snake"
+    for char in name:
+        if char == "-":
+            has_dash = True
+        elif char == "_":
+            has_underscore = True
+        elif char.isspace():
+            has_whitespace = True
+        elif char.isupper():
+            has_upper = True
+        elif char.islower():
+            has_lower = True
+
+    if has_upper and has_lower:
+        return "mixed"
+
+    if has_dash + has_underscore + has_whitespace != 1:
+        return "mixed"
+
+    if has_dash:
+        return "upper kebab" if has_upper else "kebab"
+    elif has_underscore:
+        return "upper snake" if has_upper else "snake"
     else:
-        return "pascal"
-
-
-def _split_snake(name: str) -> List[str]:
-    return name.split("_")
-
+        return "pascal" if name[0].isupper() else "camel"
 
-def _split_kebab(name: str) -> List[str]:
-    return name.split("-")
 
-
-def _split_camel_and_pascal(name: str) -> List[str]:
+def _split_name(name: str) -> List[str]:
     words: List[str] = []
     word: List[str] = []
     last_char_was_upper = True
 
     for i, char in enumerate(name):
+        if char in "-_" or char.isspace():
+            words.append("".join(word))
+            word.clear()
+            last_char_was_upper = False
+            continue
+
         is_upper = char.isupper()
 
         if (
             word
             and is_upper
-            and (
-                not last_char_was_upper
-                or (i > 0 and i + 1 < len(name) and not name[i + 1].isupper())
-            )
+            and (not last_char_was_upper or (i > 0 and i + 1 < len(name) and name[i + 1].islower()))
         ):
             words.append("".join(word))
             word.clear()
 
         word.append(char)
         last_char_was_upper = is_upper
 
@@ -712,28 +736,19 @@
     return "".join(word.title() for word in words)
 
 
 def convert_case(name: str, to: Case) -> str:
     """
     Converts a name to a different case, for example::
 
-        >>> convert_case('FooBar', 'snake')
-        'foo_bar'
+        >>> convert_case('HTMLParser', 'snake')
+        'html_parser'
     """
     case_ = detect_case(name)
-
-    split_func = {
-        "snake": _split_snake,
-        "upper snake": _split_snake,
-        "kebab": _split_kebab,
-        "upper kebab": _split_kebab,
-        "camel": _split_camel_and_pascal,
-        "pascal": _split_camel_and_pascal,
-    }[case_]
-    words = split_func(name)
+    words = _split_name(name)
 
     # Special case conversions between pascal and camel so that capitalization is preserved. For
     # example, `FancyHTML` should become `fancyHTML`, not `fancyHtml`.
     if case_ == "pascal" and to == "camel":
         words[0] = words[0].lower()
         return "".join(words)
     elif case_ == "camel" and to == "pascal":
```

### Comparing `introspection-1.7.9/introspection/misc2.py` & `introspection-1.8/introspection/misc2.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,101 +24,93 @@
 # Unchanged signature
 @overload
 def set_signature(
     signature: Union[Callable[P, T], inspect.Signature],
     *,
     remove_parameters: None = None,
     add_self: Literal[False] = False,
-) -> Callable[[Callable[..., object]], Callable[P, T]]:
-    ...
+) -> Callable[[Callable[..., object]], Callable[P, T]]: ...
 
 
 # Self parameter added
 @overload
 def set_signature(
     signature: Union[Callable[P, T], inspect.Signature],
     *,
     remove_parameters: None = None,
     add_self: Literal[True],
-) -> Callable[[Callable[..., object]], Callable[Concatenate[Any, P], T]]:
-    ...
+) -> Callable[[Callable[..., object]], Callable[Concatenate[Any, P], T]]: ...
 
 
 # Return annotation changed
 @overload
 def set_signature(
     signature: Union[Callable[P, object], inspect.Signature],
     *,
     remove_parameters: None = None,
     add_self: Literal[False] = False,
     return_annotation: Type[T],
-) -> Callable[[Callable[..., object]], Callable[P, T]]:
-    ...
+) -> Callable[[Callable[..., object]], Callable[P, T]]: ...
 
 
 # Self parameter added and return annotation changed
 @overload
 def set_signature(
     signature: Union[Callable[P, object], inspect.Signature],
     *,
     remove_parameters: None = None,
     add_self: Literal[True],
     return_annotation: Type[T],
-) -> Callable[[Callable[..., object]], Callable[Concatenate[Any, P], T]]:
-    ...
+) -> Callable[[Callable[..., object]], Callable[Concatenate[Any, P], T]]: ...
 
 
 # Parameters removed
 @overload
 def set_signature(
     signature: Union[Callable[..., T], inspect.Signature],
     *,
     remove_parameters: Iterable[Union[str, int, inspect._ParameterKind]],
     add_self: Literal[False] = False,
-) -> Callable[[Callable[..., object]], Callable[..., T]]:
-    ...
+) -> Callable[[Callable[..., object]], Callable[..., T]]: ...
 
 
 # Parameters removed and Self added
 @overload
 def set_signature(
     signature: Union[Callable[..., T], inspect.Signature],
     *,
     remove_parameters: Iterable[Union[str, int, inspect._ParameterKind]],
     add_self: Literal[True],
     # The return type should ideally be Callable[Concatenate[Self, ...], T], but
     # that crashes in 3.10
-) -> Callable[[Callable[..., object]], Callable[..., T]]:
-    ...
+) -> Callable[[Callable[..., object]], Callable[..., T]]: ...
 
 
 # Parameters removed and return annotation changed
 @overload
 def set_signature(
     signature: Union[Callable[..., object], inspect.Signature],
     *,
     remove_parameters: Iterable[Union[str, int, inspect._ParameterKind]],
     add_self: Literal[False] = False,
     return_annotation: Type[T],
-) -> Callable[[Callable[..., object]], Callable[..., T]]:
-    ...
+) -> Callable[[Callable[..., object]], Callable[..., T]]: ...
 
 
 # Parameters removed, return annotation changed and Self added
 @overload
 def set_signature(
     signature: Union[Callable[..., object], inspect.Signature],
     *,
     remove_parameters: Iterable[Union[str, int, inspect._ParameterKind]],
     add_self: Literal[True],
     return_annotation: Type[T],
     # The return type should ideally be Callable[Concatenate[Self, ...], T], but
     # that crashes in 3.10
-) -> Callable[[Callable[..., object]], Callable[..., T]]:
-    ...
+) -> Callable[[Callable[..., object]], Callable[..., T]]: ...
 
 
 def set_signature(  # type: ignore[wtf]
     signature: Union[Callable[P, T], inspect.Signature],
     *,
     remove_parameters: Optional[Iterable[Union[str, int, inspect._ParameterKind]]] = None,
     return_annotation: Type_ = NONE,  # type: ignore
@@ -138,15 +130,15 @@
             0, Parameter("self", Parameter.POSITIONAL_ONLY, annotation=Self)
         )
 
     if return_annotation is not NONE:
         signature = signature.replace(return_annotation=return_annotation)
 
     def decorator(func: Callable) -> Callable[P, T]:
-        func.__signature__ = signature
+        func.__signature__ = signature  # type: ignore
         return func  # type: ignore
 
     return decorator
 
 
 @set_signature(Signature.from_callable)
 def signature(*args, **kwargs) -> Signature:
@@ -172,68 +164,64 @@
 ) -> Callable[[Callable[..., object]], Callable[..., T]]:
     def decorator(func: Callable[..., T]) -> Callable[..., T]:
         merged_signature = Signature.from_callable(func).replace_varargs(signature)
 
         if remove_parameters:
             merged_signature = merged_signature.without_parameters(*remove_parameters)
 
-        func.__signature__ = merged_signature
+        func.__signature__ = merged_signature  # type: ignore
         return func
 
     return decorator  # type: ignore
 
 
 # Case 1: No parameters removed, return annotation unchanged
 @overload
 def wraps(
     wrapped_func: Callable[P, T],
     *,
     name: Optional[str] = None,
     signature: Union[None, inspect.Signature, Callable] = None,
     remove_parameters: None = None,
-) -> Callable[[Callable[P, T]], Callable[P, T]]:
-    ...
+) -> Callable[[Callable[P, T]], Callable[P, T]]: ...
 
 
 # Case 2: No parameters removed, return annotation changed
 @overload
 def wraps(
     wrapped_func: Callable[P, Any],
     *,
     name: Optional[str] = None,
     signature: Union[None, inspect.Signature, Callable[..., object]] = None,
     remove_parameters: None = None,
     return_annotation: Type[T],
-) -> Callable[[Callable[P, T]], Callable[P, T]]:
-    ...
+) -> Callable[[Callable[P, T]], Callable[P, T]]: ...
 
 
 # Case 3: Parameters removed, return annotation unchanged
 @overload
 def wraps(
     wrapped_func: Callable[..., T],
     *,
     name: Optional[str] = None,
     signature: Union[None, inspect.Signature, Callable[..., object]] = None,
     remove_parameters: Iterable[Union[str, int, inspect._ParameterKind]],
-) -> Callable[[Callable[P, T]], Callable[P, T]]:
-    ...
+) -> Callable[[Callable[P, T]], Callable[P, T]]: ...
 
 
 # Case 4: Parameters removed, return annotation changed
 @overload
 def wraps(
     wrapped_func: Callable[..., Any],
     *,
     name: Optional[str] = None,
     signature: Union[None, inspect.Signature, Callable[..., object]] = None,
     remove_parameters: Iterable[Union[str, int, inspect._ParameterKind]],
     return_annotation: Type[T],
-) -> Callable[[Callable[P, T]], Callable[P, T]]:
-    ...
+) -> Callable[[Callable[P, T]], Callable[P, T]]: ...
 
 
 def wraps(  # type: ignore
     wrapped_func: Callable,
     *,
     name: Optional[str] = None,
     signature: Union[None, inspect.Signature, Callable[..., object]] = None,
@@ -269,15 +257,15 @@
 
             if remove_parameters:
                 sig = sig.without_parameters(*remove_parameters)
 
             if return_annotation is not NONE:
                 sig = sig.replace(return_annotation=return_annotation)
 
-            wrapper_func.__signature__ = sig
+            wrapper_func.__signature__ = sig  # type: ignore
 
         return wrapper_func
 
     return wrapper
 
 
 def split_arguments(
```

### Comparing `introspection-1.7.9/introspection/parameter.py` & `introspection-1.8/introspection/parameter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import inspect
 from typing import *
 from typing_extensions import Self
 
 from ._utils import PARAM_EMPTY
+from .types import ForwardRefContext
 
 __all__ = ["Parameter"]
 
 
 #: Enum of parameter kinds (POSITIONAL_ONLY, etc.)
 ParameterKind = inspect._ParameterKind
 
@@ -16,15 +17,15 @@
     An :class:`inspect.Parameter` subclass that represents a function parameter.
 
     Instances of this class are immutable.
 
     This class adds a new special value for the ``default`` attribute: :attr:`Parameter.missing`.
     """
 
-    __slots__ = ()
+    __slots__ = ("forward_ref_context",)
 
     #: A special class-level marker that can be used to specify
     #: that the parameter is optional, but doesn't have a (known)
     #: default value.
     #:
     #: This is commonly used by signatures for builtin functions.
     #: For example, the signature of the :class:`range` function
@@ -42,14 +43,15 @@
 
     def __init__(
         self,
         name: str,
         kind: inspect._ParameterKind = inspect.Parameter.POSITIONAL_OR_KEYWORD,
         default: Any = PARAM_EMPTY,
         annotation: Any = PARAM_EMPTY,
+        forward_ref_context: Optional[ForwardRefContext] = None,
     ):
         """
         :param name: The parameter's name
         :param kind: The parameter's kind. See :attr:`inspect.Parameter.kind` for details.
         :param default: The parameter's default value, or one of the special values :attr:`inspect.Parameter.empty` and :attr:`Parameter.missing`
         :param annotation: The parameter's type annotation
         """
@@ -57,22 +59,27 @@
             default = inspect.Parameter.empty
 
         if annotation is PARAM_EMPTY:
             annotation = inspect.Parameter.empty
 
         super().__init__(name, kind, default=default, annotation=annotation)
 
+        self.forward_ref_context = forward_ref_context
+
     @classmethod
     def from_parameter(cls, parameter: inspect.Parameter) -> Self:
         """
         Creates a new :class:`Parameter` instance from an :class:`inspect.Parameter` instance.
 
         :param parameter: An :class:`inspect.Parameter` instance
         :return: A new :class:`Parameter` instance
         """
+        if isinstance(parameter, cls):
+            return parameter
+
         return cls(
             parameter.name,
             kind=parameter.kind,
             default=parameter.default,
             annotation=parameter.annotation,
         )
```

### Comparing `introspection-1.7.9/introspection/types.py` & `introspection-1.8/introspection/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import typing
 import typing_extensions
 
 import sentinel
 
 
 __all__ = [
+    "Case",
     "TypeParameter",
     "Type_",
     "ParameterizedGeneric",
     "ForwardReference",
     "TypeAnnotation",
     "ForwardRefContext",
 ]
@@ -27,22 +28,23 @@
 )
 
 
 T = typing.TypeVar("T")
 P = typing_extensions.ParamSpec("P")
 Class = typing.TypeVar("Class", bound=type)
 
+Case = typing.Literal["snake", "upper snake", "camel", "pascal", "kebab", "upper kebab"]
 TypeParameter = typing.Union[typing.TypeVar, typing_extensions.TypeVarTuple]
 Function = types.FunctionType
 ParameterizedGeneric: typing_extensions.TypeAlias = "types.GenericAlias"
 Type_ = typing.Union[type, typing.TypeVar, ParameterizedGeneric, None]
 ForwardReference = typing.Union[str, typing.ForwardRef]
 TypeAnnotation = typing.Union[Type_, ForwardReference]
 ForwardRefContext = typing.Union[
-    None, type, types.FunctionType, types.ModuleType, str, typing.Mapping[str, object]
+    type, types.FunctionType, types.ModuleType, str, typing.Mapping[str, object]
 ]
 
 
 # class _MetaGeneric(typing_extensions.Protocol[T]):  # type: ignore
 #     def __getitem__(self, subtypes: typing.Union[T, typing.Tuple[T, ...]]) -> ParameterizedGeneric:
 #         ...
 
@@ -54,20 +56,17 @@
 #         ...
 
 
 # GenericType = typing.Union[_MetaGeneric[T], typing.Type[_ClassGeneric[T]]]
 
 
 class Slot(typing.Protocol[T]):  # type: ignore[variance]
-    def __get__(self, instance: T, owner: typing.Optional[typing.Type[T]]) -> object:
-        ...
+    def __get__(self, instance: T, owner: typing.Optional[typing.Type[T]]) -> object: ...
 
-    def __set__(self, instance: T, value: object) -> None:
-        ...
+    def __set__(self, instance: T, value: object) -> None: ...
 
-    def __delete__(self, instance: T) -> None:
-        ...
+    def __delete__(self, instance: T) -> None: ...
 
 
 class ObjectWithQualname(typing.Protocol):
     __name__: str
     __qualname__: str
```

### Comparing `introspection-1.7.9/introspection/typing/_utils.py` & `introspection-1.8/introspection/typing/_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,27 +32,29 @@
         for name, value in mapping.items()
         for obj in resolve_name_in_all_typing_modules(name)
     }
 
 
 @dataclasses.dataclass
 class TypeCheckingConfig:
-    forward_ref_context: ForwardRefContext
+    forward_ref_context: typing.Optional[ForwardRefContext]
     treat_name_errors_as_imports: bool
 
     def resolve_at_least_1_level_of_forward_refs(self, annotation: TypeAnnotation) -> Type_:
         return resolve_at_least_1_level_of_forward_refs(
             annotation,
             self.forward_ref_context,  # type: ignore[wtf]
             self.treat_name_errors_as_imports,
         )
 
 
 def resolve_at_least_1_level_of_forward_refs(
-    annotation: TypeAnnotation, context: ForwardRefContext, treat_name_errors_as_imports: bool
+    annotation: TypeAnnotation,
+    context: typing.Optional[ForwardRefContext],
+    treat_name_errors_as_imports: bool,
 ) -> Type_:
     # Given a forward reference as input, this function resolves the outermost type, but may leave
     # subtypes unevaluated. If the input isn't a forward reference, it is returned as-is.
     if not isinstance(annotation, (str, typing.ForwardRef)):
         return annotation
 
     # We could set max_depth=1, but that would probably be a waste. There's a good chance that the
```

### Comparing `introspection-1.7.9/introspection/typing/instance_check.py` & `introspection-1.8/introspection/typing/instance_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from ._utils import (
     NOT_INSTANCE_OR_SUBTYPE_CHECKED,
     TypeCheckingConfig,
     resolve_names_in_all_typing_modules,
 )
 from .subtype_check import _is_subtype
 from .type_compat import to_python
-from ..errors import CannotResolveForwardref
 from ..parameter import Parameter
 from ..signature_ import Signature
 from .._utils import eval_or_discard
 from ..types import Type_, TypeAnnotation, ForwardRefContext
 
 __all__ = ["is_instance"]
 
@@ -31,15 +30,15 @@
 T = TypeVar("T")
 
 
 def is_instance(
     obj: object,
     type_: Union[Type[T], TypeAnnotation],
     *,
-    forward_ref_context: ForwardRefContext = None,
+    forward_ref_context: Optional[ForwardRefContext] = None,
     treat_name_errors_as_imports: bool = False,
 ) -> typing_extensions.TypeGuard[T]:
     """
     Returns whether ``obj`` is an instance of ``type_``. Unlike the builtin
     ``isinstance``, this function supports generics.
 
     .. warning::
@@ -55,18 +54,15 @@
 
 def _is_instance(
     config: TypeCheckingConfig,
     obj: object,
     type_: TypeAnnotation,
 ) -> bool:
     # Make sure we're working with an actual type, not a forward reference
-    try:
-        type_ = config.resolve_at_least_1_level_of_forward_refs(type_)
-    except CannotResolveForwardref:
-        return False
+    type_ = config.resolve_at_least_1_level_of_forward_refs(type_)
 
     # Find out if the type has type parameters
     if not is_parameterized_generic(type_):
         if type_ in TESTS:
             test = TESTS[type_]
             return test(obj)
 
@@ -177,22 +173,19 @@
 
 def _test_callable_subtypes(
     config: TypeCheckingConfig,
     obj: Callable,
     param_types: Union[List[Type_], types.EllipsisType],
     return_type: Type_,
 ) -> bool:
-    try:
-        context = sys.modules[obj.__module__]
-    except AttributeError:
-        context = None
-
-    new_config = TypeCheckingConfig(context, config.treat_name_errors_as_imports)
-
     signature = Signature.from_callable(obj)
+    new_config = TypeCheckingConfig(
+        signature.forward_ref_context,  # type: ignore[wtf]
+        config.treat_name_errors_as_imports,
+    )
 
     if signature.return_annotation is not Signature.empty:
         if not _is_subtype(new_config, signature.return_annotation, return_type):
             return False
 
     if param_types is ...:
         # I thought functions with keyword-only arguments wouldn't match, but they do. So this is
```

### Comparing `introspection-1.7.9/introspection/typing/introspection.py` & `introspection-1.8/introspection/typing/introspection.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,26 +57,23 @@
     for attr in attrs:
         obj = getattr(obj, attr)
 
     return obj
 
 
 @overload
-def _resolve_dotted_names(names: Dict[str, T]) -> Dict[object, T]:
-    ...
+def _resolve_dotted_names(names: Dict[str, T]) -> Dict[object, T]: ...
 
 
 @overload
-def _resolve_dotted_names(names: Tuple[str, ...]) -> Tuple[object, ...]:
-    ...
+def _resolve_dotted_names(names: Tuple[str, ...]) -> Tuple[object, ...]: ...
 
 
 @overload
-def _resolve_dotted_names(names: Iterable[str]) -> Iterable[object]:
-    ...
+def _resolve_dotted_names(names: Iterable[str]) -> Iterable[object]: ...
 
 
 def _resolve_dotted_names(
     names: Union[Dict[str, T], Iterable[str]]
 ) -> Union[Dict[object, T], Iterable[object]]:
     """
     ::
@@ -290,15 +287,15 @@
 
 
 def _get_type_parameters(type_):
     if sys.version_info >= (3, 10):
         if isinstance(type_, types.UnionType):
             return type_.__parameters__  # type: ignore
 
-    if safe_is_subclass(type_, Generic):
+    if safe_is_subclass(type_, Generic):  # type: ignore[wtf]
         # Classes that inherit from Generic directly (like
         # ``class Protocol(Generic):``) and Generic itself don't
         # have __orig_bases__, while classes that have type
         # parameters do.
         if not hasattr(type_, "__orig_bases__"):
             return None
 
@@ -417,15 +414,15 @@
     except AttributeError:
         return cls._name
 
 
 if sys.version_info >= (3, 9):
 
     def _is_generic_base_class(cls):
-        if safe_is_subclass(cls, Generic):
+        if safe_is_subclass(cls, Generic):  # type: ignore[wtf]
             return bool(cls.__parameters__)  # type: ignore
 
         return False
 
     def _is_parameterized_generic(cls):
         if sys.version_info >= (3, 10) and isinstance(cls, types.UnionType):
             return True
@@ -814,15 +811,15 @@
         args = _get_type_args(type_)
 
         args = tuple(arg for arg in args if arg not in {None, NoneType})
 
         if len(args) == 1:
             base = Optional
 
-    return base
+    return base  # type: ignore[wtf]
 
 
 def get_type_arguments(type_: Type_) -> Tuple[object, ...]:
     """
     Given a parameterized generic type as input, returns a tuple of its type
     arguments.
 
@@ -1066,15 +1063,15 @@
     for params, args in reversed(stack):
         i = params.index(current_var)
 
         try:
             arg = args[i]
         except IndexError:
             if assume_any:
-                return Any
+                return Any  # type: ignore
 
             raise TypeVarNotSet(type_var, base_type, type_)  # type: ignore
 
         if not isinstance(arg, TypeVar):
             return arg
 
         current_var = arg
@@ -1146,19 +1143,19 @@
     # then `__bases__` only contains `Parent`. To find `Parent[int]`, we have to
     # look in `__orig_bases__`. *However*, when inheriting from a generic type
     # without parameterizing it, then `__orig_bases__` will contain `Generic`
     # for some godforsaken reason.
     try:
         orig_bases = type_.__orig_bases__  # type: ignore
     except AttributeError:
-        return type_.__bases__
+        return type_.__bases__  # type: ignore[wtf]
 
     parent_types = []
 
-    for base, orig_base in zip(type_.__bases__, orig_bases):
+    for base, orig_base in zip(type_.__bases__, orig_bases):  # type: ignore[wtf]
         # Non-generic types show up as-is in both tuples
         if base is orig_base:
             parent_types.append(base)
         else:
             generic_base = get_generic_base_class(orig_base)
             if base is generic_base:
                 parent_types.append(orig_base)
```

### Comparing `introspection-1.7.9/introspection/typing/misc.py` & `introspection-1.8/introspection/typing/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import ast
 import builtins
 import collections.abc
+import dataclasses
 import importlib
 import types
 import typing
 import warnings
 from typing import *
 
 import typing_extensions
@@ -29,46 +30,49 @@
     "is_forward_ref",
     "resolve_forward_refs",
     "annotation_to_string",
     "annotation_for_callable",
 ]
 
 
-def is_forward_ref(annotation: TypeAnnotation) -> typing_extensions.TypeGuard[ForwardReference]:
+KW_ONLY = getattr(dataclasses, "KW_ONLY", object())
+
+
+def is_forward_ref(
+    annotation: TypeAnnotation,
+) -> typing_extensions.TypeGuard[ForwardReference]:
     """ """
     return isinstance(annotation, (str, ForwardRef))
 
 
 @overload
 def resolve_forward_refs(
     annotation: TypeAnnotation,
-    context: ForwardRefContext = None,
+    context: Optional[ForwardRefContext] = None,
     *,
     mode: Literal["eval", "getattr", "ast"] = "eval",
     strict: bool = True,
     max_depth: Optional[int] = None,
     extra_globals: Mapping[str, object] = {},
     treat_name_errors_as_imports: bool = False,
-) -> TypeAnnotation:
-    ...
+) -> TypeAnnotation: ...
 
 
 @overload
 def resolve_forward_refs(
     annotation: TypeAnnotation,
     module: typing.Optional[types.ModuleType] = None,
     eval_: bool = True,
     strict: bool = True,
-) -> TypeAnnotation:
-    ...
+) -> TypeAnnotation: ...
 
 
 def resolve_forward_refs(  # type: ignore
     annotation: TypeAnnotation,
-    context: ForwardRefContext = None,
+    context: Optional[ForwardRefContext] = None,
     eval_: Optional[bool] = None,
     strict: bool = True,
     *,
     module: typing.Optional[types.ModuleType] = None,
     mode: Literal["eval", "getattr", "ast"] = "eval",
     max_depth: Optional[int] = None,
     extra_globals: Mapping[str, object] = {},
@@ -149,15 +153,16 @@
             return annotation
         _currently_evaluating = _currently_evaluating | {key}
 
         scope: collections.ChainMap[str, object] = collections.ChainMap()
 
         if context is None:
             scope.maps.extend(
-                vars(module) for module in (collections.abc, collections, typing, typing_extensions)  # type: ignore
+                vars(module)
+                for module in (collections.abc, collections, typing, typing_extensions)  # type: ignore
             )
         elif isinstance(context, types.ModuleType):
             scope.maps.append(vars(context))
         elif isinstance(context, str):
             module = importlib.import_module(context)
             scope.maps.append(vars(module))
         elif isinstance(context, collections.abc.Mapping):
@@ -387,17 +392,19 @@
     raise NotImplementedError(f"Can't evaluate AST node {node}")
 
 
 def annotation_to_string(
     annotation: TypeAnnotation,
     *,
     implicit_typing: bool = True,
+    implicit_dataclasses: bool = True,
     new_style_unions: bool = True,
     optional_as_union: bool = True,
     variance_prefixes: bool = False,
+    aliases: Mapping[object, str] = {},
 ) -> str:
     """
     Converts a type annotation to string. The result is valid python code
     (unless ``variance_prefixes`` is set to ``True``).
 
     Examples::
 
@@ -407,43 +414,56 @@
         'None'
         >>> annotation_to_string(typing.List[int])
         'List[int]'
 
     :param annotation: A class or type annotation
     :param implicit_typing: Whether to omit the "typing." prefix from ``typing``
         types' names
+    :param implicit_dataclasses: Whether to omit the "dataclasses." prefix from ``dataclasses.KW_ONLY``
     :param new_style_unions: Whether to use the new-style ``typing.Union`` syntax
         ``int | str`` instead of ``Union[int, str]``
     :param variance_prefixes: Whether `TypeVars` and `ParamSpecs` should be
         prefixed with ``+``, ``-``, or ``~`` to indicate variance
     :return: A string that, when evaluated, returns ``annotation``
     """
 
     def recurse(annotation: TypeAnnotation) -> str:
         return annotation_to_string(
             annotation,
             implicit_typing=implicit_typing,
             new_style_unions=new_style_unions,
             optional_as_union=optional_as_union,
             variance_prefixes=variance_prefixes,
+            aliases=aliases,
         )
 
     def process_nested(prefix: str, elems: Iterable[TypeAnnotation]):
         elems = ", ".join(recurse(ann) for ann in elems)
         return "{}[{}]".format(prefix, elems)
 
     if isinstance(annotation, ForwardRef):
         return _get_forward_ref_code(annotation)
 
     if isinstance(annotation, str):
         return annotation
 
+    try:
+        return aliases[annotation]
+    except KeyError:
+        pass
+
     if annotation is ...:
         return "..."
 
+    if annotation is KW_ONLY:
+        if implicit_dataclasses:
+            return "KW_ONLY"
+        else:
+            return "dataclasses.KW_ONLY"
+
     if annotation in (None, type(None)):
         return "None"
 
     if is_parameterized_generic(annotation, raising=False):
         base = get_generic_base_class(annotation)
         subtypes = get_type_arguments(annotation)
 
@@ -453,39 +473,39 @@
 
         if base is typing.Union and new_style_unions:
             return " | ".join(recurse(sub) for sub in subtypes)  # type: ignore
 
         if base in (typing.Callable, collections.abc.Callable):
             param_types, return_type = subtypes
 
-            prefix = recurse(base)
+            prefix = recurse(base)  # type: ignore[wtf]
             return_str = recurse(return_type)  # type: ignore
 
             if isinstance(param_types, list):
                 params = ", ".join(recurse(param_type) for param_type in param_types)
                 params = f"[{params}]"
             else:
                 params = "..."
 
             return f"{prefix}[{params}, {return_str}]"
 
         if base in LITERAL_TYPES:
             literals = ", ".join(repr(value) for value in subtypes)
-            prefix = recurse(base)
+            prefix = recurse(base)  # type: ignore[wtf]
             return f"{prefix}[{literals}]"
 
         if base is typing_extensions.Annotated:
             sub_type, *annotations = subtypes
             sub_strs = [recurse(sub_type)]  # type: ignore
             sub_strs.extend(repr(ann) for ann in annotations)
 
-            prefix = recurse(base)
+            prefix = recurse(base)  # type: ignore[wtf]
             return f'{prefix}[{", ".join(sub_strs)}]'
 
-        prefix = recurse(base)
+        prefix = recurse(base)  # type: ignore[wtf]
         return process_nested(prefix, subtypes)  # type: ignore
 
     if isinstance(annotation, (typing.TypeVar, typing_extensions.ParamSpec)):
         result = annotation.__name__
 
         if variance_prefixes:
             if annotation.__covariant__:
```

### Comparing `introspection-1.7.9/introspection/typing/subtype_check.py` & `introspection-1.8/introspection/typing/subtype_check.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import types
-import typing
+from typing import Any, Callable, List, Mapping, Optional, Tuple, Type, TypeVar
 from typing_extensions import TypeGuard
 
 from ._utils import (
     NOT_INSTANCE_OR_SUBTYPE_CHECKED,
     TypeCheckingConfig,
     resolve_names_in_all_typing_modules,
 )
@@ -11,24 +11,24 @@
 from .type_compat import to_python
 from ..errors import CannotResolveForwardref, NotAParameterizedGeneric
 from ..types import Type_, TypeAnnotation, ForwardRefContext
 
 __all__ = ["is_subtype"]
 
 
-Type_Variable = typing.TypeVar("Type_Variable", bound=Type_)
+Type_Variable = TypeVar("Type_Variable", bound=Type_)
 
 
 def is_subtype(
     subtype: TypeAnnotation,
     supertype: Type_Variable,
     *,
-    forward_ref_context: ForwardRefContext = None,
+    forward_ref_context: Optional[ForwardRefContext] = None,
     treat_name_errors_as_imports: bool = False,
-) -> TypeGuard[typing.Type[Type_Variable]]:
+) -> TypeGuard[Type[Type_Variable]]:
     """
     Returns whether ``subtype`` is a subtype of ``supertype``. Unlike the
     builtin ``issubclass``, this function supports generics.
 
     .. warning::
         This function is a work-in-progress and only supports a subset of all
         generic types. If it encounters a type it can't handle, it will throw a
@@ -42,24 +42,21 @@
 
 def _is_subtype(
     config: TypeCheckingConfig,
     subtype: TypeAnnotation,
     supertype: TypeAnnotation,
 ) -> bool:
     # Make sure we're working with actual types, not forward references
-    try:
-        subtype = config.resolve_at_least_1_level_of_forward_refs(subtype)
-        supertype = config.resolve_at_least_1_level_of_forward_refs(supertype)  # type: ignore
-    except CannotResolveForwardref:
-        return False
+    subtype = config.resolve_at_least_1_level_of_forward_refs(subtype)
+    supertype = config.resolve_at_least_1_level_of_forward_refs(supertype)  # type: ignore
 
-    if subtype is typing.Any:
+    if subtype is Any:
         return True
 
-    if supertype in (typing.Any, object):
+    if supertype in (Any, object):
         return True
 
     if not is_parameterized_generic(supertype):
         return _unparameterized_supertype_check(subtype, supertype)
 
     super_base = get_generic_base_class(supertype)
     if not _unparameterized_supertype_check(subtype, super_base):
@@ -92,41 +89,47 @@
     try:
         return issubclass(subtype, supertype)  # type: ignore
     except TypeError:
         raise NotImplementedError(f"is_subtype({subtype!r}, {supertype!r}) isn't supported yet")
 
 
 def _test_union_subtypes(config: TypeCheckingConfig, subtype: Type_, union_types: tuple) -> bool:
+    errors: List[Exception] = []
+
     for union_type in union_types:
         try:
             union_type = config.resolve_at_least_1_level_of_forward_refs(union_type)
-        except CannotResolveForwardref:
+        except CannotResolveForwardref as error:
+            errors.append(error)
             continue
 
         if _is_subtype(config, subtype, union_type):
             return True
 
+    if errors:
+        raise errors[0]
+
     return False
 
 
 def _test_optional_subtypes(
     config: TypeCheckingConfig,
     subtype: Type_,
     optional_type: tuple,  # this is a 1-element tuple
 ) -> bool:
     if subtype is None or subtype is type(None):
         return True
 
     return _test_union_subtypes(config, subtype, optional_type)
 
 
-TYPE_ARGS_TESTS: typing.Mapping[
-    Type_, typing.Callable[[TypeCheckingConfig, Type_, typing.Tuple[object, ...]], bool]
-] = resolve_names_in_all_typing_modules(
-    {
-        "Union": _test_union_subtypes,
-        "Optional": _test_optional_subtypes,
-    }
+TYPE_ARGS_TESTS: Mapping[Type_, Callable[[TypeCheckingConfig, Type_, Tuple[object, ...]], bool]] = (
+    resolve_names_in_all_typing_modules(
+        {
+            "Union": _test_union_subtypes,
+            "Optional": _test_optional_subtypes,
+        }
+    )
 )
 
 if hasattr(types, "UnionType"):
     TYPE_ARGS_TESTS[types.UnionType] = _test_union_subtypes  # type: ignore
```

### Comparing `introspection-1.7.9/introspection/typing/type_compat.py` & `introspection-1.8/introspection/typing/type_compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,21 +62,19 @@
     except AttributeError:
         continue
 
     PYTHON_TO_TYPING[key] = value
 
 
 @typing.overload
-def to_python(type_: Type_, strict: typing.Literal[True]) -> type:
-    ...
+def to_python(type_: Type_, strict: typing.Literal[True]) -> type: ...
 
 
 @typing.overload
-def to_python(type_: Type_, strict: bool = False) -> Type_:
-    ...
+def to_python(type_: Type_, strict: bool = False) -> Type_: ...
 
 
 def to_python(type_: Type_, strict: bool = False) -> Type_:
     """
     Given a ``typing`` type as input, returns the corresponding "regular" python
     class.
 
@@ -143,15 +141,15 @@
         return to_python(base, strict)
     elif base in (type, typing.Type) and args[0] is object:
         return type
     elif base in (collections.abc.Callable, typing.Callable) and args == (
         ...,
         typing.Any,
     ):
-        return collections.abc.Callable
+        return collections.abc.Callable  # type: ignore[wtf]
 
     # At this point we know that the type arguments aren't redundant, so if
     # python doesn't have a generic equivalent of the base type, then we can't
     # convert it
     py_base = to_python(base, strict=strict)
 
     # I don't think there is a single class that would fail this is_generic
```

### Comparing `introspection-1.7.9/introspection/typing/type_info.py` & `introspection-1.8/introspection/typing/type_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
-import typing
-import typing_extensions
+from typing import Optional, List, Tuple
+from typing_extensions import Annotated
 
 from ._utils import resolve_at_least_1_level_of_forward_refs
 from .introspection import (
     is_parameterized_generic,
     get_type_arguments,
     get_generic_base_class,
     get_type_parameters,
@@ -20,57 +20,59 @@
 
 
 class TypeInfo:
     def __init__(
         self,
         type_: TypeAnnotation,
         *,
-        forward_ref_context: ForwardRefContext = None,
+        forward_ref_context: Optional[ForwardRefContext] = None,
         treat_name_errors_as_imports: bool = False,
     ):
+        self.raw = type_
+
         resolved_type: Type_ = resolve_at_least_1_level_of_forward_refs(
             type_, forward_ref_context, treat_name_errors_as_imports
         )
 
-        self.annotations = []
+        annotations: List[object] = []
 
         args = None
         while is_parameterized_generic(resolved_type):
             args = get_type_arguments(resolved_type)
             resolved_type = get_generic_base_class(resolved_type)
 
-            if resolved_type is typing_extensions.Annotated:
-                self.annotations += args[1:]
+            if resolved_type is Annotated:
+                annotations += args[1:]
                 resolved_type = resolve_at_least_1_level_of_forward_refs(
                     args[0],  # type: ignore
                     forward_ref_context,
                     treat_name_errors_as_imports,
                 )
+                args = None
 
+        self.annotations = tuple(annotations)
         self.type: Type_ = to_python(resolved_type, strict=False)
         self._arguments = args
         self._context = forward_ref_context
 
     @cached_property
-    def parameters(self) -> typing.Optional[typing.Tuple[TypeParameter, ...]]:
+    def parameters(self) -> Optional[Tuple[TypeParameter, ...]]:
         try:
             return get_type_parameters(self.type)
         except NotAGeneric:
             return None
 
-    # @cached_property
-    # def arguments(self) -> typing.Optional[typing.Tuple[object, ...]]:
-    #     if self._arguments is None:
-    #         return None
-
-    #     return tuple(Annotation(arg, context=self._context) for arg in self._arguments)
     @property
-    def arguments(self) -> typing.Optional[typing.Tuple[object, ...]]:
+    def arguments(self) -> Optional[Tuple[object, ...]]:
         return self._arguments
 
     @property
     def is_generic(self) -> bool:
         return self.parameters is not None
 
     @property
     def is_fully_parameterized_generic(self) -> bool:
         return self.parameters == ()
+
+    def __repr__(self) -> str:
+        cls_name = type(self).__qualname__
+        return f"{cls_name}({self.raw})"
```

### Comparing `introspection-1.7.9/pyproject.toml` & `introspection-1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/tests/conftest.py` & `introspection-1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/tests/test_argument_bundle.py` & `introspection-1.8/tests/test_argument_bundle.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/tests/test_bound_arguments.py` & `introspection-1.8/tests/test_bound_arguments.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/tests/test_call_frame.py` & `introspection-1.8/tests/test_call_frame.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/tests/test_call_stack.py` & `introspection-1.8/tests/test_call_stack.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/tests/test_class_functions.py` & `introspection-1.8/tests/test_class_functions.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/tests/test_dunder_functions.py` & `introspection-1.8/tests/test_dunder_functions.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/tests/test_misc_functions.py` & `introspection-1.8/tests/test_misc_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import abc
 import collections
 import sys
 import typing
 
 from introspection import *
 from introspection import errors
+from introspection.types import Case
 import introspection
 
 
 def test_get_parameters():
     def func(a: int, b=True):
         pass
 
@@ -496,31 +497,24 @@
         ("foo", "foo", True),
         ("foo.bar", "foo", True),
         ("foo.bar", "foo.bar", True),
         ("foo", "foo.bar", False),
         ("foo", "bar.foo", False),
     ],
 )
-def test_is_sub_qualname(sub_name, super_name, expected):
+def test_is_sub_qualname(sub_name: str, super_name: str, expected: bool):
     assert is_sub_qualname(sub_name, super_name) == expected
 
 
 @pytest.mark.parametrize(
-    "camel, expected",
+    "original, case, expected",
     [
-        ("FooBar", "foo_bar"),
-        ("HTTPAdapter", "http_adapter"),
+        ("FooBar", "upper snake", "FOO_BAR"),
+        ("HTTPAdapter", "snake", "http_adapter"),
+        ("foo_bar", "pascal", "FooBar"),
+        ("http_adapter", "camel", "httpAdapter"),
+        ("remoteCode_execution", "kebab", "remote-code-execution"),
+        ("EXAMPLE_PROJECT", "snake", "example_project"),
     ],
 )
-def test_camel_to_snake(camel, expected):
-    assert camel_to_snake(camel) == expected
-
-
-@pytest.mark.parametrize(
-    "snake, expected",
-    [
-        ("foo_bar", "FooBar"),
-        ("http_adapter", "HttpAdapter"),
-    ],
-)
-def test_snake_to_camel(snake, expected):
-    assert snake_to_camel(snake) == expected
+def test_convert_case(original: str, case: Case, expected: str):
+    assert convert_case(original, case) == expected
```

### Comparing `introspection-1.7.9/tests/test_parameter.py` & `introspection-1.8/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/tests/test_signature.py` & `introspection-1.8/tests/test_signature.py`

 * *Files 10% similar despite different names*

```diff
@@ -215,14 +215,57 @@
     assert list(sig.parameters) == ["self", "foo"]
     assert sig.return_annotation is None
     assert sig.parameters["foo"].annotation is float
     assert sig.parameters["foo"].default == 3.5
     assert sig.parameters["foo"].kind is Parameter.KEYWORD_ONLY
 
 
+def test_class_signature():
+    class Cls:
+        def __init__(self, init):
+            pass
+
+    sig = Signature.from_callable(Cls)
+    assert list(sig.parameters) == ["init"]
+
+
+def test_class_signature_with_metaclass():
+    class Meta(type):
+        def __call__(self, meta):
+            pass
+
+    class Cls(metaclass=Meta):
+        def __new__(cls, new):
+            pass
+
+        def __init__(self, init):
+            pass
+
+    sig = Signature.from_callable(Cls)
+    assert list(sig.parameters) == ["meta"]
+
+
+def test_builtin_class_signature():
+    # Just make sure it doesn't crash
+    _ = Signature.from_callable(float, use_signature_db=False)
+
+
+def test_doesnt_alter_signature_mark():
+    class Cls:
+        @introspection.mark.does_not_alter_signature
+        def __new__(cls, *args, **kwargs):
+            return super().__new__(cls, *args, **kwargs)
+
+        def __init__(self, init):
+            pass
+
+    sig = Signature.from_callable(Cls)
+    assert list(sig.parameters) == ["init"]
+
+
 def test_replace():
     sig = Signature([Parameter("foo")], return_annotation=int)
 
     expected = Signature(return_annotation=str)
 
     result = sig.replace(parameters=[], return_annotation=str)
     assert isinstance(result, Signature)
```

### Comparing `introspection-1.7.9/tests/test_typing/test_introspection.py` & `introspection-1.8/tests/test_typing/test_introspection.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/tests/test_typing/test_misc.py` & `introspection-1.8/tests/test_typing/test_misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 
 import builtins
+import dataclasses
 import io
 import sys
 import typing
 from typing import *
 from typing_extensions import ParamSpec
 
 from introspection.typing.misc import *
@@ -40,19 +41,28 @@
         "expected",
         [
             "int | str",
             "int | None",
             "int | str | None",
         ],
     )
-    def test_annotation_to_string_simple_py310(expected):
+    def test_annotation_to_string_simple_py310(expected: str):
         annotation = eval(expected)
 
         assert annotation_to_string(annotation) == expected
 
+    @pytest.mark.parametrize(
+        "annotation, expected",
+        [
+            (dataclasses.KW_ONLY, "KW_ONLY"),
+        ],
+    )
+    def test_annotation_to_string_py310(annotation, expected: str):
+        assert annotation_to_string(annotation) == expected
+
 
 @pytest.mark.parametrize(
     "expected",
     [
         "Union[int, str]",
         "Union[int, str, None]",
     ],
```

### Comparing `introspection-1.7.9/tests/test_typing/test_type_checks.py` & `introspection-1.8/tests/test_typing/test_type_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,18 @@
 from introspection.typing import is_instance, is_subtype
 
 
 T = TypeVar("T")
 
 
 class AwaitableObject:
-    def __await__(self) -> Iterator[None]:
-        ...
+    def __await__(self) -> Iterator[None]: ...
 
 
-def func_with_forwardrefs(arg: "int") -> "str":
-    ...
+def func_with_forwardrefs(arg: "int") -> "str": ...
 
 
 @pytest.mark.parametrize(
     "obj, type_, expected",
     [
         (3, int, True),
         (True, int, True),
@@ -62,23 +60,23 @@
         (func_with_forwardrefs, Callable[[int], bytes], False),
     ],
 )
 def test_is_instance(obj, type_, expected):
     assert is_instance(obj, type_) == expected
 
 
-@pytest.mark.parametrize(
-    "obj, type_, expected",
-    [
-        (3, "ThisIsAnInvalidForwardRef", False),
-        # (3, "datetime", False),  # This is interesting because `datetime` is a module
-    ],
-)
-def test_is_instance_with_forwardref_type(obj, type_, expected):
-    assert is_instance(obj, type_, treat_name_errors_as_imports=True) == expected
+# @pytest.mark.parametrize(
+#     "obj, type_, expected",
+#     [
+#         (3, "ThisIsAnInvalidForwardRef", False),
+#         # (3, "datetime", False),  # This is interesting because `datetime` is a module
+#     ],
+# )
+# def test_is_instance_with_forwardref_type(obj, type_, expected):
+#     assert is_instance(obj, type_, treat_name_errors_as_imports=True) == expected
 
 
 @pytest.mark.parametrize(
     "subtype, supertype, expected",
     [
         (dict, Any, True),
         (Any, dict, True),
```

### Comparing `introspection-1.7.9/tests/test_typing/test_type_compat.py` & `introspection-1.8/tests/test_typing/test_type_compat.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/tox.ini` & `introspection-1.8/tox.ini`

 * *Files identical despite different names*

### Comparing `introspection-1.7.9/PKG-INFO` & `introspection-1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: introspection
-Version: 1.7.9
+Version: 1.8
 Summary: New and improved introspection functions
 Author: Paul Pinterits
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: ordered-set
 Requires-Dist: renumerate
 Requires-Dist: sentinel
```

