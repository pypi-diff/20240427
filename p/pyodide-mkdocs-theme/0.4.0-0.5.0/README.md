# Comparing `tmp/pyodide_mkdocs_theme-0.4.0.tar.gz` & `tmp/pyodide_mkdocs_theme-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide_mkdocs_theme-0.4.0.tar", max compression
+gzip compressed data, was "pyodide_mkdocs_theme-0.5.0.tar", max compression
```

## Comparing `pyodide_mkdocs_theme-0.4.0.tar` & `pyodide_mkdocs_theme-0.5.0.tar`

### file list

```diff
@@ -1,75 +1,76 @@
--rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.4.0/LICENSE
--rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.4.0/README.md
--rw-r--r--   0        0        0     1347 2024-04-25 15:11:17.449074 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/__init__.py
--rw-r--r--   0        0        0     2160 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/__main__.py
--rw-r--r--   0        0        0       22 2024-04-25 15:11:17.481075 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/__version__.py
--rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py
--rw-r--r--   0        0        0     1178 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/deprecation.py
--rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
--rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
--rw-r--r--   0        0        0     4974 2024-04-11 09:41:00.019938 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
--rw-r--r--   0        0        0     4967 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
--rw-r--r--   0        0        0    21205 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
--rw-r--r--   0        0        0    14716 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
--rw-r--r--   0        0        0      689 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
--rw-r--r--   0        0        0     6073 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
--rw-r--r--   0        0        0     4093 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
--rw-r--r--   0        0        0    11589 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
--rw-r--r--   0        0        0    13167 2024-04-18 21:29:06.622893 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/messages.py
--rw-r--r--   0        0        0     6945 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
--rw-r--r--   0        0        0     4237 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/parsing.py
--rw-r--r--   0        0        0     4462 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
--rw-r--r--   0        0        0    11593 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
--rw-r--r--   0        0        0    11690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
--rw-r--r--   0        0        0    13032 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py
--rw-r--r--   0        0        0     1614 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
--rw-r--r--   0        0        0     2877 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
--rw-r--r--   0        0        0     9974 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
--rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
--rw-r--r--   0        0        0     1064 2024-04-25 15:11:17.441074 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
--rw-r--r--   0        0        0     6881 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
--rw-r--r--   0        0        0      690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/scripts/__init__.py
--rw-r--r--   0        0        0     1001 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/scripts/custom_lang.py
--rw-r--r--   0        0        0     3983 2024-04-25 15:11:17.449074 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/scripts/custom_lang_src.py
--rw-r--r--   0        0        0     5490 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/__init__.py
--rw-r--r--   0        0        0     4510 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
--rw-r--r--   0        0        0     7349 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
--rw-r--r--   0        0        0     1675 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
--rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
--rw-r--r--   0        0        0     4320 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
--rw-r--r--   0        0        0     3683 2024-04-25 15:10:27.387632 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
--rw-r--r--   0        0        0     1078 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css
--rw-r--r--   0        0        0     6426 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/main.html
--rw-r--r--   0        0        0     1924 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
--rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/partials/copyright.html
--rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/partials/footer.html
--rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/partials/social.html
--rw-r--r--   0        0        0     9776 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
--rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
--rw-r--r--   0        0        0     3459 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css
--rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
--rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
--rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
--rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
--rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
--rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
--rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
--rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
--rw-r--r--   0        0        0     6600 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
--rw-r--r--   0        0        0    16559 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
--rw-r--r--   0        0        0     9657 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
--rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
--rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
--rw-r--r--   0        0        0     9150 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
--rw-r--r--   0        0        0     3629 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css
--rw-r--r--   0        0        0     1651 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css
--rw-r--r--   0        0        0     5373 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
--rw-r--r--   0        0        0     4203 2024-04-25 15:10:27.387632 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
--rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
--rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
--rw-r--r--   0        0        0     3774 2024-04-14 12:10:19.820826 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css
--rw-r--r--   0        0        0    12716 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
--rw-r--r--   0        0        0     1775 2024-04-25 15:11:13.760968 pyodide_mkdocs_theme-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.5.0/LICENSE
+-rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.5.0/README.md
+-rw-r--r--   0        0        0     1347 2024-04-26 21:34:25.787204 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/__init__.py
+-rw-r--r--   0        0        0     2160 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/__main__.py
+-rw-r--r--   0        0        0       22 2024-04-26 21:34:25.827205 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/__version__.py
+-rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py
+-rw-r--r--   0        0        0     1178 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/deprecation.py
+-rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
+-rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
+-rw-r--r--   0        0        0     4974 2024-04-11 09:41:00.019938 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
+-rw-r--r--   0        0        0     4979 2024-04-26 21:24:58.094371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
+-rw-r--r--   0        0        0    21452 2024-04-26 21:24:58.094371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
+-rw-r--r--   0        0        0    14716 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
+-rw-r--r--   0        0        0      689 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
+-rw-r--r--   0        0        0     6062 2024-04-26 21:24:58.094371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
+-rw-r--r--   0        0        0     3928 2024-04-26 21:24:58.094371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
+-rw-r--r--   0        0        0    11742 2024-04-26 21:24:58.094371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
+-rw-r--r--   0        0        0    13167 2024-04-18 21:29:06.622893 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/messages.py
+-rw-r--r--   0        0        0     6945 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
+-rw-r--r--   0        0        0     4237 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/parsing.py
+-rw-r--r--   0        0        0     4451 2024-04-26 21:24:58.094371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
+-rw-r--r--   0        0        0    12435 2024-04-26 21:24:58.094371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
+-rw-r--r--   0        0        0    11679 2024-04-26 21:24:58.094371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
+-rw-r--r--   0        0        0     6152 2024-04-26 21:24:58.102371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py
+-rw-r--r--   0        0        0     1603 2024-04-26 21:24:58.102371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
+-rw-r--r--   0        0        0    10204 2024-04-26 21:34:25.775203 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py
+-rw-r--r--   0        0        0     2877 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
+-rw-r--r--   0        0        0     8198 2024-04-26 21:24:58.102371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
+-rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
+-rw-r--r--   0        0        0     1064 2024-04-26 21:34:25.775203 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
+-rw-r--r--   0        0        0     6881 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
+-rw-r--r--   0        0        0      690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/scripts/__init__.py
+-rw-r--r--   0        0        0     1001 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/scripts/custom_lang.py
+-rw-r--r--   0        0        0     3983 2024-04-26 21:34:25.787204 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/scripts/custom_lang_src.py
+-rw-r--r--   0        0        0     5490 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/__init__.py
+-rw-r--r--   0        0        0     5160 2024-04-26 21:24:58.102371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
+-rw-r--r--   0        0        0     7349 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
+-rw-r--r--   0        0        0     1675 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
+-rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
+-rw-r--r--   0        0        0     4320 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
+-rw-r--r--   0        0        0     3791 2024-04-26 21:24:58.102371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
+-rw-r--r--   0        0        0     1078 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css
+-rw-r--r--   0        0        0     6642 2024-04-26 21:24:58.102371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/main.html
+-rw-r--r--   0        0        0     1924 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
+-rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/partials/copyright.html
+-rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/partials/footer.html
+-rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/partials/social.html
+-rw-r--r--   0        0        0     9830 2024-04-26 21:24:58.102371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
+-rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
+-rw-r--r--   0        0        0     3459 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css
+-rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
+-rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
+-rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
+-rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
+-rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
+-rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
+-rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
+-rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
+-rw-r--r--   0        0        0     6607 2024-04-26 21:24:58.102371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
+-rw-r--r--   0        0        0    16619 2024-04-26 21:24:58.102371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
+-rw-r--r--   0        0        0    10269 2024-04-26 21:24:58.102371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
+-rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
+-rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
+-rw-r--r--   0        0        0     9297 2024-04-26 21:24:58.102371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
+-rw-r--r--   0        0        0     3740 2024-04-26 21:24:58.102371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css
+-rw-r--r--   0        0        0     1651 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css
+-rw-r--r--   0        0        0     5379 2024-04-26 21:24:58.102371 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
+-rw-r--r--   0        0        0     4203 2024-04-25 15:11:28.669398 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
+-rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
+-rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
+-rw-r--r--   0        0        0     3774 2024-04-14 12:10:19.820826 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css
+-rw-r--r--   0        0        0    12716 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
+-rw-r--r--   0        0        0     1775 2024-04-26 21:34:21.923089 pyodide_mkdocs_theme-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.5.0/PKG-INFO
```

### Comparing `pyodide_mkdocs_theme-0.4.0/LICENSE` & `pyodide_mkdocs_theme-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/README.md` & `pyodide_mkdocs_theme-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/__init__.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/__main__.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/__main__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/deprecation.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/deprecation.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     """
 
     @wraps(_IDE_maker)
     def wrapped(
         py_name: str = "",
         MAX: Optional[Union[int, Literal["+"]]] = None,
         SANS: str = "",
-        MAX_SIZE: int = 30,
+        MAX_SIZE: Optional[int] = None,
         ID: Optional[int] = None,
         WHITE: str = "",
         LOGS: Optional[bool] = None,
         REC_LIMIT: int = -1,
         TERM_H: int = 10,
     ) -> str:
         return Ide(
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,16 +164,22 @@
     )
 
 
 
 
     def __post_init__(self):
 
-        if self.max_attempts is None:
-            self.max_attempts = self.my_env.max_attempts_before_corr_available
+        to_globals_if_none = (
+            ('max_attempts', 'max_attempts_before_corr_available'),
+            ('max_size',     'default_ide_height_lines'),
+        )
+        for prop,conf_prop in to_globals_if_none:
+            if getattr(self, prop) is None:
+                def_val = getattr(self.my_env, conf_prop)
+                setattr(self, prop, def_val)
 
         self.files_data = IdeFilesExtractor(self.my_env, self.py_name, self.id)
 
         if 0 <= self.rec_limit < self.my_env.MIN_RECURSION_LIMIT:
             with_id = f' (ID={ self.id })' if self.id is not None else ''
             raise BuildError(
                 f"The recursion limit for {self.my_env.page.file.src_uri}:{self.py_name}"
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 """
 # pylint: disable=unused-argument
 
 import os
 from typing import Union
 from functools import wraps
 from ..paths_utils import get_sibling_of_current_page, to_uri
-from ..plugin.maestro_base_and_indent import BaseMaestro
+from ..plugin.maestro_base import BaseMaestro
 from ..plugin.maestro_extras import MaestroExtras
 
 
 
 
 def numworks(env:BaseMaestro):
     """ wut...? """
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,46 +12,40 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
-
-"""
-Simple elements introduced through macros
-(code block with language and indentation, empty terminal, ...)
-"""
 # pylint: disable=unused-argument
 
 
 import re
 from pathlib import Path
 from functools import wraps
 
 from .. import html_builder as Html
 from ..plugin.maestro_IDE import MaestroIDE
-from ..plugin.maestro_base_and_indent import BaseMaestro
 from ..parsing import build_code_fence
 from ..paths_utils import get_sibling_of_current_page
 from ..tools_and_constants import HtmlClass, Prefix, ScriptKind
 
 
 
 
 
 def script(
-    env:MaestroIDE,
-    macro:str,
-    docs_dir:Path,
-    nom:str,
+    env: MaestroIDE,
+    macro: str,
+    docs_dir: Path,
+    nom: str,
     *,
-    lang:str='python',
-    stop=None,
-    ID:int=None
+    lang: str='python',
+    stop= None,
+    ID: int=None
 ) -> str:
     """
     Renvoie le script dans une balise bloc avec langage spécifié
 
     - macro: permet de retrouver le niveau d'indentation de l'appel de macro
     - lang: le nom du lexer pour la coloration syntaxique
     - nom: le chemin du script relativement au .md d'appel
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,22 +69,22 @@
     @ID:int=None:     To disambiguate GCMs macro calls if needed
     @DEBUG=False:     If True, md output will be printed to the console
     """
 
     @wraps(multi_qcm)
     def wrapped(
         *inputs,
-        shuffle:bool=False,
-        hide:bool=False,
-        multi:Optional[bool]=None,
-        admo_kind:str="!!!",
-        admo_class:str="tip",
-        qcm_title:str=None,
-        ID:Optional[int]=None,
-        DEBUG:bool=False,
+        shuffle:    Optional[bool]=None,
+        hide:       Optional[bool]=None,
+        multi:      Optional[bool]=None,
+        admo_kind:  str="!!!",
+        admo_class: str="tip",
+        qcm_title:  Optional[str]=None,
+        ID:         Optional[int]=None,
+        DEBUG:      bool=False,
     ):
         """
         WARNING:    extra closing </p> tags needed here and there to guarantee the
                     final html structure!
 
         Reasons:
         1. THE MD RENDERER GENERATES INVALID HTML, WHEN MIXING html+md PERIOD!
@@ -166,15 +166,15 @@
                 )
 
             # validate "multi" aspect, but without actually updating the value (see multi_kls)
             # (...that's probably a bad idea...?)
             if len(lst_correct) < 2 and multi is None:
                 raise BuildError(
                     "Found a QCM question with only one valid answer, while no information was "
-                    "available to know is it is a multi- or single choice question.\nPlease set "
+                    "available to know if it is a multi or single choice question.\nPlease set "
                     "the `multi` argument either on the macro call (`multi_qcm(...multi=bool)`), "
                     "or on the question itself, with a 4th dict element: "
                     "`[question, choices, answers, {'multi':bool}]`."
                     f"\n\nQuestion:\n{ question }"
                 )
 
         #------------------------------------------------------------------
@@ -195,16 +195,17 @@
         ]
 
         id_pattern = "" if ID is None else rf".*?,\s*ID\s*=\s*{ ID }\b\s*"
         call_pattern = re.compile(rf"multi_qcm[(]{ id_pattern }")
         indent = env.get_indent_in_current_page(call_pattern)
         auto_indent = auto_indenter_factory(indent)
 
-        if multi is None:
-            multi = env.multi
+        if hide is None:    hide    = env.hide
+        if multi is None:   multi   = env.multi
+        if shuffle is None: shuffle = env.shuffle
 
         admonition_lst = qcm_start()
 
         for n, (question, items, lst_answers, extra_dct) in enumerate(questions_data, 1):
 
             is_multi = extra_dct.get('multi', multi)
             if is_multi is None:
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/messages.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/messages.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/parsing.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/parsing.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """
 
 
 from urllib.parse import unquote
 from pathlib import Path
 from typing import Optional, Union
 
-from .plugin.maestro_base_and_indent import BaseMaestro
+from .plugin.maestro_base import BaseMaestro
 
 
 
 
 PathOrStr = Union[str,Path]
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,14 +113,31 @@
     If true, any failure when running the user code during a validation will decrease the number
     of attempts left. Note this means even syntax errors will decrease the count.
 
     When this option is set to True, any error raised within the code of the editor will stop
     the validation process without modifying the number of attempts left.
     """
 
+    default_ide_height_lines = C.Type(int, default=30)
+    """
+    Max height of the editor (in number of lines). For the macro IDEv, this takes precedence on
+    the TERM_H argument.
+    """
+
+    deactivate_stdout_for_secrets = C.Type(bool, default=True)
+    """
+    Define if the stdout will be shown to the user or not, for the secret tests.
+    """
+
+    show_only_assertion_errors_for_secrets = C.Type(bool, default=False)
+    """
+    If True, the stack trace of all error messages will be suppressed and only assertion messages
+    will be left unchanged, when an error is raised during the secret tests.
+    """
+
 
 
 
 
 
 
 class BuildConfig(Config):
@@ -231,22 +248,32 @@
     """
 
 
 
 class QcmsConfig(Config):
     """ Options specific to the QCMs or QCSs"""
 
+    hide = C.Type(bool, default=False)
+    """
+    Global choice for the `shuffle` argument of QCMs.
+    """
+
     multi = C.Optional(C.Choice((True, False, None), default=None))
     """
     Global choice for the `multi` argument.
 
     If this option is set to `True` or `False`, it will act as a documentation-wide setting to
     disambiguate questions having 0 or 1 correct answers only.
     """
 
+    shuffle = C.Type(bool, default=False)
+    """
+    Global choice for the `shuffle` argument of QCMs.
+    """
+
 
 
 # This only defines the values exposed to the user in mkdocs.yml.
 # When a property is declared here, don't forgot to add the related extractor on the
 # BaseMaestro class.
 class PyodideMacrosConfig(Config):
     """ Configuration for the main pyodide-mkdocs-theme plugin. """
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     ScriptKind
 )
 from ..pyodide_logger import logger
 from ..parsing import eat, encrypt_string
 from ..scripts_templates import SCRIPTS_TEMPLATES
 
 from .maestro_tools import AutoCounter
-from .maestro_base_and_indent import BaseMaestro
+from .maestro_base import BaseMaestro
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,103 +12,46 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
-# pylint: disable=multiple-statements
 
 
 import re
-from typing import Dict, List, Optional, Union
+from typing import Dict, Optional, Union
 from pathlib import Path
 
-from mkdocs.plugins import BasePlugin
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.structure.pages import Page
 from mkdocs.exceptions import BuildError
 
+
 from ..deprecation import deprecation_warning
-from ..messages import Lang, Msg, Tip
+from ..messages import  Msg, Tip
 
-from ...__version__ import __version__
 from ..tools_and_constants import PageUrl
 from ..pyodide_logger import logger
 from ..parsing import eat
 
-from .maestro_tools import ConfigExtractor
-from .config import PyodideMacrosConfig
-
-
-
-
+from .maestro_base import BaseMaestro
 
 
 
 
-class BaseMaestro( BasePlugin[PyodideMacrosConfig] ):
-    """
-    Main class, regrouping the basic configurations, properties, getters and/or constants
-    for the different children classes: each of them will inherit from MaestroConfig.
-    It is also used as "sink" for the super calls of other classes that are not implemented
-    on the MacrosPlugin class.
-
-    Note that, for the ConfigExtractor for to properly work, the class hierarchy has to
-    extend MacrosPlugin at some point.
-    """
-
-    ignore_macros_plugin_diffs:             bool = ConfigExtractor('build')
-    skip_py_md_paths_names_validation:      bool = ConfigExtractor('build')
-    check_python_files:                     bool = ConfigExtractor('build')
-    soft_check:                             bool = ConfigExtractor('build')
-    load_yaml_encoding:                     str  = ConfigExtractor('build')
-    bypass_indent_errors:                   bool = ConfigExtractor('build')
-    encrypt_corrections_and_rems:           bool = ConfigExtractor('build')
-    macros_with_indents:               List[str] = ConfigExtractor('build')
-
-    show_assertion_code_on_failed_test:     bool = ConfigExtractor("ides")
-    max_attempts_before_corr_available:     bool = ConfigExtractor("ides")
-    decrease_attempts_on_user_code_failure: bool = ConfigExtractor("ides")
 
-    multi:                        Optional[bool] = ConfigExtractor("qcms")
 
-    _dev_mode:                              bool = ConfigExtractor()
 
-    scripts_url: str = ConfigExtractor("_others")
-    site_root:   str = ConfigExtractor("_others")
 
-    # global mkdocs config data:
-    docs_dir:    str = ConfigExtractor(root='_conf')
-    repo_url:    str = ConfigExtractor(root='_conf')
-    site_name:   str = ConfigExtractor(root='_conf')
-    site_url:    str = ConfigExtractor(root='_conf')
 
-    page: Page  # just as a reminder: defined by MacrosPlugin
 
-    #----------------------------------------------------------------------------
-    # WARNING: the following properties are assigned from the PyodideMacrosPlugin
 
-    docs_dir_path: Path
-    """ Current docs_dir of the project as a Path object (ABSOLUTE path) """
-
-    docs_dir_cwd_rel: Path
-    """ docs_dir Path object, but relative to the CWD, at runtime """
-
-    _macro_with_indent_pattern:re.Pattern = None
-    """
-    Pattern to re.match macro calls that will need to handle indentation levels.
-    Built at runtime (depends on `macro_with_indents`)
-    """
-
-    #----------------------------------------------------------------------------
-
-    version:str = __version__
-
-    pmt_url:str = 'https://gitlab.com/frederic-zinelli/pyodide-mkdocs-theme'
+class MaestroIndent(BaseMaestro):
+    """ Manage Indentation logistic """
 
 
     _pages_indents: 'PageIndents'
     """
     Cache storing the indentations for each jinja/macro template in a Page.
     A page is entirely studied the first time it's seen and the result of the indentation levels
     are stored.
@@ -117,24 +60,19 @@
     """
 
     _running_macro: Optional[str] = None
     """
     Name of the macro currently running (or the last one called. None if no macro called yet).
     """
 
-    lang: Lang = None
-
 
 
     def on_config(self, config:MkDocsConfig):
         # pylint: disable=unused-argument, no-member, missing-function-docstring
         self._pages_indents = PageIndents()
-        self.lang = Lang()
-        self.lang.register_env(self)
-
         super().on_config(config)     # MacrosPlugin is actually "next in line" and has the method
 
 
     def override_messages(self, dct_lang: Dict[str, Union[Msg,Tip]]):
         """ Replace some default messages or configurations with the given content """
         self.lang.overload(dct_lang)
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """
 # pylint: disable=multiple-statements
 
 
 from mkdocs.config.defaults import MkDocsConfig
 
 from ..tools_and_constants import Prefix
-from .maestro_base_and_indent import BaseMaestro
+from .maestro_base import BaseMaestro
 from .maestro_tools import AutoCounter
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,63 +14,52 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
 
-import json
 import os
 import re
 from collections import defaultdict
 from functools import wraps
 from pathlib import Path
 
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.exceptions import BuildError
 from mkdocs_macros.plugin import MacrosPlugin
 
-from pyodide_mkdocs_theme.pyodide_macros.messages import Lang
-from pyodide_mkdocs_theme.pyodide_macros.plugin.maestro_tools import dump_and_dumper
+
 
 
 from ...__version__ import __version__
 from ..exceptions import PyodideConfigurationError
 from ..pyodide_logger import logger
 from ..macros import (
     autres,
     IDEs,
     isolated_components,
     qcm,
 )
 from .config import MISSING_MACROS_PROPS, EXTRAS_MACROS_PROPS
-from .maestro_base_and_indent import BaseMaestro
+from .maestro_base import BaseMaestro
+from .maestro_indent import MaestroIndent
 from .maestro_IDE import MaestroIDE
 from .maestro_extras import MaestroExtras
 
 
 
-ICONS_FROM_TEMPLATES = Path("pyodide-mkdocs/IDE-and-buttons/images/")
-
-TO_DUMP_TO_JD_CONFIG = """
-    button_icons_directory
-    decrease_attempts_on_user_code_failure
-    encrypt_corrections_and_rems
-    show_assertion_code_on_failed_test
-    site_name
-    version
-""".split()
-
 
 
 
 
 class PyodideMacrosPlugin(
     MaestroIDE,
     MaestroExtras,
+    MaestroIndent,
     BaseMaestro,
     MacrosPlugin,    # Always last, so that other classes may trigger super methods appropriately.
 ):
     """
     Class centralizing all the behaviors of the different parent classes.
 
     This is kinda the "controller", linking all the behaviors to mkdocs machinery, while the
@@ -80,60 +69,14 @@
         - on_config
         - on_nav
         - on_page_markdown  (+ on_pre_page_macros + on_post_page_macros)
         - on_post_build     (on_post_build macros)
         - on_serve
     """
 
-    version: str = __version__
-
-
-    def rebase(self, base_url:str):
-        """
-        Necessary for development only (to replace the wrong base_url value during a serve in the
-        theme project)
-        NOTE: Keep in mind the bas_url SOMETIMES ends with a slash...
-        """
-        return base_url if base_url!='/' else '.'
-
-
-
-    def dump_to_js_config(self, base_url):
-        """
-        Create the <script> tag that will add all the CONFIG properties needed in the JS global.
-        """
-        if self:
-            base_url = self.rebase(base_url).rstrip('/')
-            # temporary property:
-            self.button_icons_directory = f"{base_url}/{ICONS_FROM_TEMPLATES}"  # pylint: disable=w0201
-
-
-        dct = dump_and_dumper(TO_DUMP_TO_JD_CONFIG, self, json.dumps)
-        dct['lang'] = Lang.dump_as_str(self and self.lang)
-
-
-        if self is None:    # HACK!
-            # Dump to config.js (helper):
-            dumping = [ f"\n    { prop }: { val }," for prop,val in dct.items() ]
-            return ''.join(dumping)
-
-
-        # Dump to main.html:
-        dumping = [ f"\n  CONFIG.{ prop } = { val }" for prop,val in dct.items() ]
-
-        del self.button_icons_directory
-
-        out = f'''\
-<script type="application/javascript">
-{ "".join(dumping) }
-CONFIG.lang.tests.as_pattern = new RegExp(CONFIG.lang.tests.as_pattern, 'i')
-</script>'''
-        return out
-
-
 
     def _check_docs_paths_validity(self) -> None :
         """
         Travel through all paths in the docs_dir and raises an BuildError if "special characters"
         are found in directory, py, or md file names (accepted characters are: r'[\\w.-]+' )
         """
         if self.skip_py_md_paths_names_validation:
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/scripts/__init__.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/scripts/custom_lang.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/scripts/custom_lang.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/scripts/custom_lang_src.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/scripts/custom_lang_src.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/__init__.py` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -28,19 +28,40 @@
 
 const CONFIG = {
 
     /*
     The following values are passed from python to JS through the main.html,
     once this script got loaded */
     //CONFIG_DUMP
-    buttonIconsDirectory: null,
-    decreaseAttemptsOnUserCodeFailure: null,
+    ignoreMacrosPluginDiffs: null,
+    skipPyMdPathsNamesValidation: null,
+    checkPythonFiles: null,
+    softCheck: null,
+    loadYamlEncoding: null,
+    bypassIndentErrors: null,
     encryptCorrectionsAndRems: null,
+    macrosWithIndents: null,
     showAssertionCodeOnFailedTest: null,
+    maxAttemptsBeforeCorrAvailable: null,
+    decreaseAttemptsOnUserCodeFailure: null,
+    defaultIdeHeightLines: null,
+    deactivateStdoutForSecrets: null,
+    showOnlyAssertionErrorsForSecrets: null,
+    hide: null,
+    multi: null,
+    shuffle: null,
+    scriptsUrl: null,
+    siteRoot: null,
+    docsDir: null,
+    repoUrl: null,
     siteName: null,
+    siteUrl: null,
+    buttonIconsDirectory: null,
+    baseUrl: null,
+    pmtUrl: null,
     version: null,
     lang: {
         comments: null,
         tests: null,
         runScript: null,
         successMsg: null,
         installStart: null,
@@ -77,14 +98,16 @@
     ideProp: {}, // filled dynamically
 
     onDoneEvent: 'unload', // unused, so far...
 
     // Various UI elements identifiers
     element: {
         searchBlock: "div.md-search",
+        searchBtnsLeft: "#search-btns-left",
+        searchBtnsRight: "#search-btns-right",
         dayNight: "form.md-header__option",
         stdoutCtrlId: "#stdout-controller-btn",
         cutFeedbackSvg: "#cut-feedback-svg",
         hourGlass: "#header-hourglass-svg",
         qcm_admos: ".py_mk_admonition_qcm",
         qcmInnerDiv: ".py_mk_admonition_qcm-inner",
         qcmCounterCls: ".qcm-counter",
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -38,15 +38,16 @@
         const trashBtnOptions = {
             shift: 90,
             tipText: CONFIG.lang.tipTrash.msg,
             tipWidth: CONFIG.lang.tipTrash.em
         }
 
         const trashButtonCode = buttonWithTooltip(trashBtnOptions, TRASH_SVG)
-        $(trashButtonCode).insertAfter(CONFIG.element.searchBlock).on('click', function() {
+        const wrappingDiv = `<div id="${ CONFIG.element.searchBtnsRight.slice(1) }">${ trashButtonCode }</div>`
+        $(wrappingDiv).insertAfter(CONFIG.element.searchBlock).on('click', function() {
 
             const data = Object.keys(localStorage)
             const codes = data.filter(s => /^editor_[\da-f]{16,}$/.test(s))
             const cmds = data.filter(s => /^\d+_commands$/.test(s))
 
 
             if (!codes.length) {
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/main.html` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/main.html`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 -->
 
 {% extends "base.html" %}
 
 <!-- Load CDNs : Pyodide (Python in WASM), Ace (Editor) and JQuery (Terminal) and mathJax, then local scripts. -->
 <!-- WARNING: the mathjax tex-mml-chtml.js cdn must be loaded AFTER the pmt config-libs.js file has been loaded. -->
 {% block libs %}
+{% include "hooks/libsBefore.html" ignore missing %}
 {{ super() }}
 <script src="https://cdn.jsdelivr.net/npm/lodash@4.17.20/lodash.min.js" type="text/javascript"></script>
 <script src="https://cdnjs.cloudflare.com/ajax/libs/ace/1.32.7/ace.min.js" charset="utf-8" type="text/javascript" integrity="sha512-GQpIYSKNIPIC763JKTNALj+t18/nfLdzw5gITgFGa31aK/4NmjyPKsfqrjh7CuzpJaG3nqEleeVcWUhHad9Axg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
 <script src="https://cdnjs.cloudflare.com/ajax/libs/ace/1.32.7/ext-language_tools.min.js" charset="utf-8" type="text/javascript" integrity="sha512-iK7yTkCkv7MbFwTqRgHTbmIqoiiLq6BsyNjymnFyB5a7pEQwYThj9QIgqBy9+XPPwj7+hAEHyR2npOHL1bz4Qg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
 <script src="https://cdn.jsdelivr.net/npm/jquery"></script>
 <script src="https://cdn.jsdelivr.net/npm/jquery.terminal/js/jquery.terminal.min.js"></script>
 <link href="https://cdn.jsdelivr.net/npm/jquery.terminal/css/jquery.terminal.min.css" rel="stylesheet"/>
@@ -41,14 +42,15 @@
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/IDE-and-buttons/ide-libs.css">
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/pyoditeur-libs.css">
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/qcm/qcm-libs.css">
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/terminal/css/terminal-libs.css">
 <link rel="stylesheet" href="{{ config.plugins.pyodide_macros.rebase(base_url) }}/js-libs/z_header-btns-libs.css">
 <!-- PYODIDE - insertion token -->
 <script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js" type="text/javascript" charset="utf-8"></script>
+{% include "hooks/libsAfter.html" ignore missing %}
 {% endblock %}
 
 
 {% block extrahead %}
 
 {% if config.extra.ace_style %}
   {% if config.extra.ace_style['slate'] and config.extra.ace_style['default'] %}
@@ -69,21 +71,23 @@
         data-ace-dark-mode="tomorrow_night_bright"
         data-ace-light-mode="crimson_editor">
 {% endif %}
 {% endblock %}
 
 
 {% block scripts %}
+{% include "hooks/scriptsBefore.html" ignore missing %}
 {{ super() }}
 <!-- PYODIDE - insertion token -->
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js"></script>
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/actions/0_tasks-scripts.js"></script>
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js"></script>
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/error-logs-generator-scripts.js"></script>
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/actions/genericCodeRunner-scripts.js"></script>
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/qcm/qcm-scripts.js"></script>
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/terminal/terminal-helpers-scripts.js"></script>
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/terminal/terminal-scripts.js"></script>
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js"></script>
 <script type="application/javascript" src="{{ config.plugins.pyodide_macros.rebase(base_url) }}/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js"></script>
 <!-- PYODIDE - insertion token -->
+{% include "hooks/scriptsAfter.html" ignore missing %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,10 @@
-{% extends "base.html" %} {% block libs %} {{ super() }}
+{% extends "base.html" %} {% block libs %} {% include "hooks/libsBefore.html"
+ignore missing %} {{ super() }}
 {{ config.plugins.pyodide_macros.dump_to_js_config(base_url) }}
-{% endblock %} {% block extrahead %} {% if config.extra.ace_style %} {% if
-config.extra.ace_style['slate'] and config.extra.ace_style['default'] %} ??{%
-elif config.extra.ace_style['slate'] %} ??{% elif config.extra.ace_style
-['default'] %} ??{% endif %} {% else %} ??{% endif %} {% endblock %} {% block
-scripts %} {{ super() }}
-{% endblock %}
+{% include "hooks/libsAfter.html" ignore missing %} {% endblock %} {% block
+extrahead %} {% if config.extra.ace_style %} {% if config.extra.ace_style
+['slate'] and config.extra.ace_style['default'] %} ??{% elif
+config.extra.ace_style['slate'] %} ??{% elif config.extra.ace_style['default']
+%} ??{% endif %} {% else %} ??{% endif %} {% endblock %} {% block scripts %} {%
+include "hooks/scriptsBefore.html" ignore missing %} {{ super() }}
+{% include "hooks/scriptsAfter.html" ignore missing %} {% endblock %}
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/partials/copyright.html` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/partials/footer.html` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/partials/footer.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/partials/social.html` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/partials/social.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -29,15 +29,15 @@
     await waitForPyodideReady();
     jsLogger("[Play]")
 
     let [code, terminal, options] = await setupRuntimeAndTerminal(editorName);
     let stdErr = ""
 
     try {
-        stdErr = await runPythonCodeWithOptions(code, terminal, options)
+        stdErr = await runPythonCodeWithOptions(code, terminal, options, true)
     } finally {
         tearDownRuntimeAndTerminal(terminal, stdErr)
     }
     $.terminal.active().focus()
 
 }, 'play')
 
@@ -57,15 +57,15 @@
     let [code, terminal, options] = await setupRuntimeAndTerminal(editorName);
     let finalMsg = "",
         stdErr = ""
     let decrease_count = false
 
     try {
         // Define the user's code in the environment and run the public tests (if any)
-        stdErr = await runPythonCodeWithOptions(code, terminal, options)
+        stdErr = await runPythonCodeWithOptions(code, terminal, options, true)
 
         decrease_count = CONFIG.decreaseAttemptsOnUserCodeFailure && stdErr
 
         // Run the validation tests only if the user's code succeeded at the previous step
         if (!stdErr) {
 
             // If still running, run the original public tests and the secret ones...
@@ -74,18 +74,18 @@
 
             // ...unless there are no secret tests (this may happen when using KB shortcuts, while
             // there is no validation to do => just quit the testing process right away)
             if (!secretTests) return
 
             const autoLogAssert = securedExtraction(editorName, CONFIG.ideProp.autoLogAssert)
             options.autoLogAssert = autoLogAssert !== null ? autoLogAssert : CONFIG.showAssertionCodeOnFailedTest
-            options.withStdOut = false
+            options.withStdOut = !CONFIG.deactivateStdoutForSecrets
 
             const fullTests = `${ publicTests }\n\n${ secretTests }`
-            decrease_count = stdErr = await runPythonCodeWithOptions(fullTests, terminal, options)
+            decrease_count = stdErr = await runPythonCodeWithOptions(fullTests, terminal, options, false)
         }
 
         // On error, manage the counter of tries and the revelation of the solution, otherwise
         // reveal the solutions + setup success message (displayed in teardown step):
         if (!stdErr) {
             unhideSolutionAndRem(editorName)
             if (getAttemptsLeft(editorName) > 0) {
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -48,15 +48,15 @@
 
     // Run before clearing the terminal, in case someone forgot a print:
     setupStdIO()
     let stdErr = ''
     try {
         await runHdrContent(editorName, options, terminal)
     } catch (err) {
-        stdErr = generateErrorLog(err, "", false)
+        stdErr = generateErrorLog(err, "", false, false)
     } finally {
         let someMsg = (getFullStdIO() || "") + stdErr
         if (someMsg) terminal.echo(someMsg)
     }
 
     return [aceCode, terminal, options]
 }
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -104,15 +104,15 @@
  * NOTE:
  *    - Pyodide itself is using eval, so replacing globally the builtin will cause a lot of
  *      troubles and just won't work.
  *    - This function doesn't take in charge the pyodide environment setup, (preparation,
  *      rebuilding the setup, ...).
  *    - On the other hand it DOES take in charge installation of missing modules/packages.
  */
-async function runPythonCodeWithOptions(code, terminal, options) {
+async function runPythonCodeWithOptions(code, terminal, options, isPublicRun) {
 
     try {
         // Do first the methods exclusions check, to gain some time (avoids loading modules if
         // the error would show up anyway after loading them)
         const nope = options.excludedMethods.filter(methodCall => code.includes(methodCall))
         if (nope.length) {
             const plural = nope.length > 1 ? "s" : ""
@@ -121,16 +121,16 @@
             throw new PythonError(msg)
         }
 
         // Detect possible user imports and install the packages to allow their imports:
         await installAndImportMissingModules(code, options, terminal)
 
     } catch (err) {
-        const strErr = generateErrorLog(err, code)
-        terminal.echo(strErr);
+        const strErr = generateErrorLog(err, code, false, !isPublicRun)
+        terminal.echo(strErr)
         return strErr
     }
 
     const withExclusions = options.excluded.length > 0 || options.recLimit > 0
 
     // Setup stdout capture. WARNING: this must always be done even if it's not shown to the user.
     // If not done, a previous execution might have close the StringIO and if ever the user prints
@@ -155,29 +155,29 @@
         // finally close, and they also must be protected against failure, so in their own
         // try/catch/finally construct:
         try {
             if (withExclusions) restoreOriginalFunctions(options.excluded)
 
             // Now only, compute the error message if needed.
             if (delayedErr) {
-                stdErr = generateErrorLog(delayedErr, code, options.autoLogAssert)
+                stdErr = generateErrorLog(delayedErr, code, options.autoLogAssert, !isPublicRun)
             }
 
             // Always extract the stdout and close the buffer (avoid memory leaks)
             let captured = getFullStdIO() || ""
 
             // Send stdout feedback to the user only if allowed:
             if (options.withStdOut) {
                 stdOut = escapeSquareBrackets(textShortener(captured))
             }
 
         } catch (err) {
             // This second catch is there so that the user can see the JS error in the terminal.
             // (Note: maybe I should actually throw them again...?)
-            stdErr = generateErrorLog(err, code)
+            stdErr = generateErrorLog(err, code, true, false)
 
         } finally {
             const someMsg = stdOut + stdErr
             if (someMsg) {
                 terminal.echo(someMsg);
             }
             return stdErr
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -87,15 +87,15 @@
  *        File "/lib/python311.zip/_pyodide/_base.py", line 339, in run
  *          coroutine = eval(self.code, globals, locals)
  *                      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  *        File "<exec>", line 1, in <module>
  *      AssertionError: This message...
  *
  * */
-function generateErrorLog(err, code, allowCodeExtraction = true) {
+function generateErrorLog(err, code, allowAssertionCodeExtraction, purgeErr) {
 
     const msg = String(err).trimEnd() // Note: err has a trailing linefeed, s trim it...
 
     // Return directly non python errors. => allows to also see JS errors.
     if (!msg.startsWith('PythonError')) {
         return youAreInTroubles(err)
     }
@@ -132,56 +132,74 @@
     const isMultiLineError = iError + 1 < errLines.length
     const cleaned = (errLines[iError] || "").replace("AssertionError", "").trim()
     const hasNoMsg = !isMultiLineError && !cleaned
 
     // WARNING: working by mutation, so successive splices are done 'from the end".
 
     // Rebuild the assertion message first, if needed:
-    if (isAssertErr && hasNoMsg && allowCodeExtraction) {
+    if (isAssertErr && hasNoMsg && allowAssertionCodeExtraction) {
         buildAssertionMsg(code, errLines, iError)
+
+    } else if (!isAssertErr && purgeErr && CONFIG.showOnlyAssertionErrorsForSecrets) {
+        // Reformat error message if needed
+        const errKind = errLines[iError].split(':')[0]
+        errLines.splice(iError, errLines.length)
+        errLines.push(`${errKind} has been raised.`)
     }
 
     // Shorten the error code section (if multiline assertion message), and then the stacktrace.
-    shortenArrSection('err', errLines, iError, errLines.length - 1)
+    shortenArrSection('err', errLines, iError, errLines.length - 1, iModule, purgeErr)
 
     // Remove pyodide related information from the stacktrace (the user doesn't need to know) if
     // it's the user's code that is run, otherwise, keep the full stack trace to ease debugging:
     if (isFromUserCode) {
-        shortenArrSection('trace', errLines, iModule, iError - 1)
-
-        errLines.splice(1, iModule - 1)
-        errLines[0] = errLines[0].slice('PythonError: '.length)
+        shortenArrSection('trace', errLines, iModule, iError - 1, iModule, purgeErr)
 
     } else {
         errLines.push(CONFIG.MSG.bigFail)
     }
 
     return error(errLines.join('\n'))
 }
 
 
 
 /**Mutate the content of the given array, if the section identified by the original `from` and
  * `to` indices is considered too long.
  * Both indices arguments are inclusive.
  * */
-const shortenArrSection = (kind, errLines, from, to) => {
-    if (!CONFIG.cutFeedback) return
+const shortenArrSection = (kind, errLines, from, to, iModule, purgeErr) => {
+
+    if (kind == 'trace' && CONFIG.showOnlyAssertionErrorsForSecrets && purgeErr) {
+        errLines.splice(0, to + 1)
+        return
+    }
 
-    const [limit, head, tail] = "Limit Head Tail".split(' ').map(prop => CONFIG.feedbackShortener[kind + prop])
-    if (to - from > limit) {
-        from += head
-        to -= tail
-        let middle = CONFIG.feedbackShortener.msg
-        if (kind == 'trace') {
-            middle = middle.replace(CONFIG.MSG.rightSafeSqbr,
-                `, ${ to-from-1 } more lines here...${ CONFIG.MSG.rightSafeSqbr }`)
+    if (!CONFIG.cutFeedback) {
+
+        const [limit, head, tail] = "Limit Head Tail".split(' ').map(prop => CONFIG.feedbackShortener[kind + prop])
+        if (to - from > limit) {
+            from += head
+            to -= tail
+            let middle = CONFIG.feedbackShortener.msg
+            if (kind == 'trace') {
+                middle = middle.replace(
+                    CONFIG.MSG.rightSafeSqbr,
+                    `, ${ to-from-1 } more lines here...${ CONFIG.MSG.rightSafeSqbr }`
+                )
+            }
+            errLines.splice(from, to - from + 1, middle)
         }
-        errLines.splice(from, to - from + 1, middle)
     }
+
+    if (kind != 'trace') return
+
+    // Then remove or reformat pyodide specific lines (nly if this is the last operation, aka "trace")
+    errLines.splice(1, iModule - 1)
+    errLines[0] = errLines[0].slice('PythonError: '.length)
 }
 
 
 
 
 /**Travel through the lines of an error message from the end, and spot the line index of the
  * raised Error, assuming it will be preceded by a line starting with `  File "<(exec|console)>"`
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -22,30 +22,34 @@
  * but the header doesn't exist yet, so the subscription delay is used, and it's done from here
  * so that the hourglass cannot show up in pages tht do not need it.
  * */
 subscribeWhenReady(
     "HourGlass",
     function() {
         jsLogger('[HourGlass]')
-        $(`
+
+        const hourGlassSvg = `
 <svg viewBox="0 0 512 512" id="${ CONFIG.element.hourGlass.slice(1) }"
     height="24px" width="24px" version="1.1" xmlns="http://www.w3.org/2000/svg"
     xmlns:xlink="http://www.w3.org/1999/xlink" xml:space="preserve" fill="#ffffff">
     <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
     <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
     <g id="SVGRepo_iconCarrier">
         <g>
             <path class="st0" d="M329.368,237.908l42.55-39.905c25.237-23.661,39.56-56.701,39.56-91.292V49.156 c0.009-13.514-5.538-25.918-14.402-34.754C388.24,5.529,375.828-0.009,362.314,0H149.677c-13.514-0.009-25.918,5.529-34.754,14.401 c-8.872,8.837-14.41,21.24-14.402,34.754v57.554c0,34.591,14.315,67.632,39.552,91.292l42.55,39.888 c2.352,2.205,3.678,5.272,3.678,8.493v19.234c0,3.221-1.326,6.279-3.67,8.475l-42.558,39.905 c-25.237,23.653-39.552,56.702-39.552,91.292v57.554c-0.009,13.514,5.529,25.918,14.402,34.755 c8.836,8.871,21.24,14.409,34.754,14.401h212.636c13.514,0.008,25.926-5.53,34.763-14.401c8.863-8.838,14.41-21.241,14.402-34.755 v-57.554c0-34.59-14.324-67.64-39.56-91.292l-42.55-39.896c-2.344-2.205-3.678-5.263-3.678-8.484v-19.234 C325.69,243.162,327.025,240.095,329.368,237.908z M373.942,462.844c-0.009,3.273-1.266,6.055-3.403,8.218 c-2.162,2.135-4.952,3.402-8.226,3.41H149.677c-3.273-0.009-6.055-1.275-8.225-3.41c-2.128-2.163-3.394-4.945-3.402-8.218v-57.554 c0-24.212,10.026-47.356,27.691-63.91l42.55-39.906c9.914-9.285,15.538-22.274,15.538-35.857v-19.234 c0-13.592-5.624-26.58-15.547-35.866l-42.541-39.896c-17.666-16.555-27.691-39.69-27.691-63.91V49.156 c0.008-3.273,1.274-6.055,3.402-8.226c2.17-2.127,4.952-3.394,8.225-3.402h212.636c3.273,0.009,6.064,1.275,8.226,3.402 c2.136,2.171,3.394,4.952,3.403,8.226v57.554c0,24.22-10.026,47.355-27.683,63.91l-42.55,39.896 c-9.922,9.286-15.547,22.274-15.547,35.866v19.234c0,13.583,5.625,26.572,15.547,35.874l42.55,39.88 c17.658,16.563,27.683,39.707,27.683,63.918V462.844z"></path>
             <path class="st0" d="M256,248.674c10.017,0,18.131-8.122,18.131-18.139c3.032-12.051,9.397-23.161,18.578-31.757l42.542-39.888 c13.592-12.739,21.602-30.448,22.446-48.984H154.302c0.844,18.536,8.854,36.245,22.438,48.984l42.541,39.888 c9.19,8.596,15.547,19.706,18.579,31.757C237.861,240.552,245.983,248.674,256,248.674z"></path>
             <path class="st0" d="M256,267.796c-10.017,0-18.139,8.122-18.139,18.139c0,10.009,8.122,18.131,18.139,18.131 c10.017,0,18.131-8.122,18.131-18.131C274.131,275.918,266.017,267.796,256,267.796z"></path>
             <path class="st0" d="M256,332.137c-10.017,0-18.139,8.122-18.139,18.14c0,10.009,8.122,18.131,18.139,18.131 c10.017,0,18.131-8.122,18.131-18.131C274.131,340.259,266.017,332.137,256,332.137z"></path>
             <path class="st0" d="M239.876,389.742l-66.538,66.538h165.315l-66.537-66.538C263.21,380.845,248.782,380.845,239.876,389.742z"></path>
         </g>
     </g>
-</svg>`).insertBefore(CONFIG.element.dayNight)
+</svg>`
+
+        const wrappingDiv = `<div id="${ CONFIG.element.searchBtnsLeft.slice(1) }">${ hourGlassSvg }</div>`
+        $(wrappingDiv).insertBefore(CONFIG.element.dayNight)
     }, {
         waitFor: CONFIG.element.dayNight
     },
 )
 
 
 
@@ -188,15 +192,15 @@
     found to enforce them to release focus without action from the user is:
         1. Override onBlur on each terminal (otherwise they never lose focus)
         2. Enforce scrolling back to the position before creation of the terminal
         3. Use an hidden input button and its click event to make sure the last textarea
             defined loses the focus... (note: it _doesn't_ work with a text input or autofocus)
     */
     const [x, y] = CONFIG.currentScroll
-    jsLogger('[Scroll] meh', x, y)
+    jsLogger('[Scroll]', x, y)
     $('body').append(`
         <input type="button" id="py_mk_pin_scroll_input"
             style="
                 position:absolute; left:${x}px; top:${y}px;
                 width:50px; height:20px; color: red;background-color: red; z-index: 20;
                 visibility:hidden;
         ">`.replace(/\s+/g, " "))
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css`

 * *Files 2% similar despite different names*

```diff
@@ -160,7 +160,15 @@
   text-shadow: 0px 0px rgba(87, 147, 240, 0);
   position: relative;
   left: 1px;
   top: 1px;
   font-size: 2em;
   box-shadow: 0px 0px rgba(87, 147, 240, 0);
 }
+
+
+#search-btns-left, #search-btns-right {
+  height: 40px;
+  display: flex;
+  align-items: center;
+  gap: 5px;
+}
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -92,15 +92,15 @@
                 editorName, {
                     runCodeAsync: commandRunnerAsync(term)
                 }
             )
         }
         term.pause();
         try {
-            await runPythonCodeWithOptions(command, term, options)
+            await runPythonCodeWithOptions(command, term, options, true)
         } finally {
             // Release the terminal to the user:
             term.resume();
             await sleep(); // Enforce the UI update, going through the next tick
         }
     }
 }
```

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js` & `pyodide_mkdocs_theme-0.5.0/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.4.0/pyproject.toml` & `pyodide_mkdocs_theme-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyodide-mkdocs-theme"
-version = "0.4.0"
+version = "0.5.0"
 description = "Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations"
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 readme = "README.md"
 keywords = [
     "mkdocs", "mkdocs-plugin", "pyodide", "IDE", "terminal"
 ]
 classifiers = [
```

### Comparing `pyodide_mkdocs_theme-0.4.0/PKG-INFO` & `pyodide_mkdocs_theme-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-mkdocs-theme
-Version: 0.4.0
+Version: 0.5.0
 Summary: Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations
 Keywords: mkdocs,mkdocs-plugin,pyodide,IDE,terminal
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

