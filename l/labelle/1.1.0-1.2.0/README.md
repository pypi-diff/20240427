# Comparing `tmp/labelle-1.1.0.tar.gz` & `tmp/labelle-1.2.0.tar.gz`

## Comparing `labelle-1.1.0.tar` & `labelle-1.2.0.tar`

### file list

```diff
@@ -1,82 +1,89 @@
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 labelle-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 labelle-1.1.0/labelle.ini
--rw-r--r--   0        0        0   635825 2020-02-02 00:00:00.000000 labelle-1.1.0/labelle.png
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 labelle-1.1.0/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 labelle-1.1.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 labelle-1.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 labelle-1.1.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 labelle-1.1.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 labelle-1.1.0/.vscode/launch.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 labelle-1.1.0/.vscode/settings.json
--rw-r--r--   0        0        0    43688 2020-02-02 00:00:00.000000 labelle-1.1.0/doc/Labelle_example_1.png
--rw-r--r--   0        0        0    41426 2020-02-02 00:00:00.000000 labelle-1.1.0/doc/Labelle_example_2.png
--rw-r--r--   0        0        0    50874 2020-02-02 00:00:00.000000 labelle-1.1.0/doc/Labelle_example_3.png
--rwxr-xr-x   0        0        0      117 2020-02-02 00:00:00.000000 labelle-1.1.0/scripts/gui_dev.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labelle-1.1.0/src/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_version.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/metadata.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib.pyi
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE
--rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_AMSFONTS
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_BAKOMA
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_CARLOGO
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_COLORBREWER
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_COURIERTEN
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_DEJAVU
--rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_JSXTOOLS_RESIZE_OBSERVER
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_QHULL
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_QT4_EDITOR
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_SOLARIZED
--rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_STIX
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_YORICK
--rw-r--r--   0        0        0     8951 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/_vendor/matplotlib/font_manager.py
--rwxr-xr-x   0        0        0    10454 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/cli/cli.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/gui/common.py
--rw-r--r--   0        0        0     9793 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/gui/gui.py
--rw-r--r--   0        0        0    15048 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/gui/q_dymo_label_widgets.py
--rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/gui/q_dymo_labels_list.py
--rwxr-xr-x   0        0        0     4017 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/barcode_writer.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/config_file.py
--rwxr-xr-x   0        0        0     2508 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/constants.py
--rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/detect.py
--rwxr-xr-x   0        0        0    11650 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/dymo_labeler.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/font_config.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/logger.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/unicode_blocks.py
--rwxr-xr-x   0        0        0     1225 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/utils.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/__init__.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/barcode.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/barcode_with_text.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/empty.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/horizontally_combined.py
--rw-r--r--   0        0        0     5004 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/margins.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/picture.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/print_payload.py
--rw-r--r--   0        0        0     7328 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/print_preview.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/qr.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/render_context.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/render_engine.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/test_pattern.py
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/lib/render_engines/text.py
--rw-r--r--   0        0        0   690516 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/fonts/Carlito-Bold.ttf
--rw-r--r--   0        0        0   816716 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/fonts/Carlito-BoldItalic.ttf
--rw-r--r--   0        0        0   623416 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/fonts/Carlito-Italic.ttf
--rw-r--r--   0        0        0   635996 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/fonts/Carlito-Regular.ttf
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/fonts/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/fonts/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/icons/__init__.py
--rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/icons/barcode_icon.png
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/icons/barcode_text_icon.png
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/icons/img_icon.png
--rw-r--r--   0        0        0    68086 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/icons/logo_small.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/icons/qr_icon.png
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 labelle-1.1.0/src/labelle/resources/icons/txt_icon.png
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 labelle-1.1.0/vendoring/README.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 labelle-1.1.0/vendoring/vendor.txt
--rw-r--r--   0        0        0    47308 2020-02-02 00:00:00.000000 labelle-1.1.0/vendoring/patches/matplotlib.patch
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 labelle-1.1.0/.gitignore
--rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 labelle-1.1.0/LICENSE
--rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 labelle-1.1.0/README.md
--rw-r--r--   0        0        0     5798 2020-02-02 00:00:00.000000 labelle-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     8403 2020-02-02 00:00:00.000000 labelle-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 labelle-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 labelle-1.2.0/labelle.ini
+-rw-r--r--   0        0        0   635825 2020-02-02 00:00:00.000000 labelle-1.2.0/labelle.png
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 labelle-1.2.0/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 labelle-1.2.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 labelle-1.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 labelle-1.2.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 labelle-1.2.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 labelle-1.2.0/.vscode/launch.json
+-rw-r--r--   0        0        0    43688 2020-02-02 00:00:00.000000 labelle-1.2.0/doc/Labelle_example_1.png
+-rw-r--r--   0        0        0    41426 2020-02-02 00:00:00.000000 labelle-1.2.0/doc/Labelle_example_2.png
+-rw-r--r--   0        0        0    50874 2020-02-02 00:00:00.000000 labelle-1.2.0/doc/Labelle_example_3.png
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 labelle-1.2.0/scripts/gui_dev.sh
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/_version.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/metadata.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/_vendor/matplotlib.pyi
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE
+-rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_AMSFONTS
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_BAKOMA
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_CARLOGO
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_COLORBREWER
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_COURIERTEN
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_DEJAVU
+-rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_JSXTOOLS_RESIZE_OBSERVER
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_QHULL
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_QT4_EDITOR
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_SOLARIZED
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_STIX
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_YORICK
+-rw-r--r--   0        0        0     8951 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/_vendor/matplotlib/font_manager.py
+-rwxr-xr-x   0        0        0    11632 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/cli/cli.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/gui/common.py
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/gui/gui.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/gui/q_actions.py
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/gui/q_device_selector.py
+-rw-r--r--   0        0        0    15187 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/gui/q_label_widgets.py
+-rw-r--r--   0        0        0     9477 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/gui/q_labels_list.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/gui/q_render.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/gui/q_settings_toolbar.py
+-rwxr-xr-x   0        0        0     4017 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/barcode_writer.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/config_file.py
+-rwxr-xr-x   0        0        0     3102 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/constants.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/env_config.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/font_config.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/logger.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/outputs.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/unicode_blocks.py
+-rwxr-xr-x   0        0        0     1225 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/devices/__init__.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/devices/device_manager.py
+-rwxr-xr-x   0        0        0    12025 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/devices/dymo_labeler.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/devices/online_device_manager.py
+-rw-r--r--   0        0        0     9909 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/devices/usb_device.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/render_engines/__init__.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/render_engines/barcode.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/render_engines/barcode_with_text.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/render_engines/empty.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/render_engines/horizontally_combined.py
+-rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/render_engines/margins.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/render_engines/picture.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/render_engines/print_payload.py
+-rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/render_engines/print_preview.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/render_engines/qr.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/render_engines/render_context.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/render_engines/render_engine.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/render_engines/test_pattern.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/lib/render_engines/text.py
+-rw-r--r--   0        0        0   690516 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/resources/fonts/Carlito-Bold.ttf
+-rw-r--r--   0        0        0   816716 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/resources/fonts/Carlito-BoldItalic.ttf
+-rw-r--r--   0        0        0   623416 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/resources/fonts/Carlito-Italic.ttf
+-rw-r--r--   0        0        0   635996 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/resources/fonts/Carlito-Regular.ttf
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/resources/fonts/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/resources/fonts/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/resources/icons/__init__.py
+-rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/resources/icons/barcode_icon.png
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/resources/icons/barcode_text_icon.png
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/resources/icons/img_icon.png
+-rw-r--r--   0        0        0    68086 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/resources/icons/logo_small.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/resources/icons/qr_icon.png
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 labelle-1.2.0/src/labelle/resources/icons/txt_icon.png
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 labelle-1.2.0/vendoring/README.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 labelle-1.2.0/vendoring/vendor.txt
+-rw-r--r--   0        0        0    47308 2020-02-02 00:00:00.000000 labelle-1.2.0/vendoring/patches/matplotlib.patch
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 labelle-1.2.0/.gitignore
+-rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 labelle-1.2.0/LICENSE
+-rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 labelle-1.2.0/README.md
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 labelle-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8432 2020-02-02 00:00:00.000000 labelle-1.2.0/PKG-INFO
```

### Comparing `labelle-1.1.0/.pre-commit-config.yaml` & `labelle-1.2.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   - id: check-yaml
   - id: debug-statements
   - id: end-of-file-fixer
   - id: mixed-line-ending
     args: ['--fix=lf']
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.3.7
+  rev: v0.4.1
   hooks:
   - id: ruff
     args: [--fix, --exit-non-zero-on-fix]
   - id: ruff-format
 
 - repo: https://gitlab.com/bmares/check-json5
   rev: v1.0.0
@@ -33,12 +33,13 @@
 
 - repo: https://github.com/pre-commit/mirrors-mypy
   rev: v1.9.0
   hooks:
   - id: mypy
     additional_dependencies:
     - types-pillow
+    - types-cffi
 
 - repo: https://github.com/igorshubovych/markdownlint-cli
   rev: v0.39.0
   hooks:
   - id: markdownlint
```

### Comparing `labelle-1.1.0/labelle.png` & `labelle-1.2.0/labelle.png`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/.devcontainer/Dockerfile` & `labelle-1.2.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/.devcontainer/devcontainer.json` & `labelle-1.2.0/.devcontainer/devcontainer.json`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,21 @@
 		"vscode": {
 			"extensions": [
 				"charliermarsh.ruff",
 				"eamodio.gitlens",
 				"github.vscode-github-actions",
 				"ms-azuretools.vscode-docker",
 				"ms-python.mypy-type-checker",
+				"ms-python.python",
 				"tamasfe.even-better-toml",
 				"zhoufeng.pyqt-integration"
-			]
+			],
+			"settings": {
+				"editor.rulers": [88]
+			}
 		}
 	},
 	// Uncomment to connect as root instead. More info: https://aka.ms/dev-containers-non-root.
 	// "remoteUser": "root"
 	"runArgs": [
 		"--net",
 		"host",
```

### Comparing `labelle-1.1.0/.github/workflows/pypi-publish.yml` & `labelle-1.2.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/.github/workflows/tests.yml` & `labelle-1.2.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/.vscode/launch.json` & `labelle-1.2.0/.vscode/launch.json`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 {
     // Use IntelliSense to learn about possible attributes.
     // Hover to view descriptions of existing attributes.
     // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
     "version": "0.2.0",
     "configurations": [
         {
-            "name": "Python: Module",
+            "name": "CLI",
             "type": "debugpy",
             "request": "launch",
-            "module": "labelle.command_line",
+            "module": "labelle.cli.cli",
             "args": [
+                "--preview",
                 "hi",
             ],
-            "justMyCode": true
+            "justMyCode": false,
+        },
+        {
+            "name": "GUI",
+            "type": "debugpy",
+            "request": "launch",
+            "module": "labelle.gui.gui",
+            "justMyCode": false,
         }
     ]
 }
```

### Comparing `labelle-1.1.0/doc/Labelle_example_1.png` & `labelle-1.2.0/doc/Labelle_example_1.png`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/doc/Labelle_example_2.png` & `labelle-1.2.0/doc/Labelle_example_2.png`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/doc/Labelle_example_3.png` & `labelle-1.2.0/doc/Labelle_example_3.png`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE` & `labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_AMSFONTS` & `labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_AMSFONTS`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_BAKOMA` & `labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_BAKOMA`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_CARLOGO` & `labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_CARLOGO`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_COLORBREWER` & `labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_COLORBREWER`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_COURIERTEN` & `labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_COURIERTEN`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_DEJAVU` & `labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_DEJAVU`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_JSXTOOLS_RESIZE_OBSERVER` & `labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_JSXTOOLS_RESIZE_OBSERVER`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_QHULL` & `labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_QHULL`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_QT4_EDITOR` & `labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_QT4_EDITOR`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_SOLARIZED` & `labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_SOLARIZED`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_STIX` & `labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_STIX`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/_vendor/matplotlib/LICENSE_YORICK` & `labelle-1.2.0/src/labelle/_vendor/matplotlib/LICENSE_YORICK`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/_vendor/matplotlib/font_manager.py` & `labelle-1.2.0/src/labelle/_vendor/matplotlib/font_manager.py`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/gui/q_dymo_label_widgets.py` & `labelle-1.2.0/src/labelle/gui/q_label_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,25 +13,27 @@
     QPlainTextEdit,
     QPushButton,
     QSpinBox,
     QWidget,
 )
 
 from labelle.gui.common import crash_msg_box
-from labelle.lib.constants import AVAILABLE_BARCODES, ICON_DIR
+from labelle.lib.constants import ICON_DIR, BarcodeType, Direction
+from labelle.lib.env_config import is_dev_mode_no_margins
 from labelle.lib.font_config import get_available_fonts
 from labelle.lib.render_engines import (
     BarcodeRenderEngine,
     BarcodeWithTextRenderEngine,
     EmptyRenderEngine,
     NoContentError,
     NoPictureFilePath,
     PictureRenderEngine,
     QrRenderEngine,
     RenderContext,
+    RenderEngine,
     TextRenderEngine,
 )
 from labelle.lib.render_engines.render_engine import RenderEngineException
 
 
 class FontStyle(QComboBox):
     def __init__(self):
@@ -40,15 +42,15 @@
         for font_path in get_available_fonts():
             name = font_path.stem
             absolute_path = font_path.absolute()
             self.addItem(name, absolute_path)
             self.setCurrentText("Carlito-Regular")
 
 
-class BaseDymoLabelWidget(QWidget):
+class BaseLabelWidget(QWidget):
     """A base class for creating Dymo label widgets.
 
     Signals:
     --------
     itemRenderSignal : PyQtSignal
         Signal emitted when the content of the label is changed.
 
@@ -79,15 +81,15 @@
         try:
             return self.render_engine_impl
         except RenderEngineException as err:
             crash_msg_box(self, "Render Engine Failed!", err)
             return EmptyRenderEngine()
 
 
-class TextDymoLabelWidget(BaseDymoLabelWidget):
+class TextDymoLabelWidget(BaseLabelWidget):
     """A widget for rendering text on a Dymo label.
 
     Args:
     ----
         render_context (RenderContext): The rendering context to use.
         parent (QWidget): The parent widget of this widget.
 
@@ -109,15 +111,16 @@
     font_size: QSpinBox
     frame_width_px: QSpinBox
 
     def __init__(self, render_context: RenderContext, parent: Optional[QWidget] = None):
         super().__init__(parent)
         self.render_context = render_context
 
-        self.label = QPlainTextEdit("text")
+        default_label_text = "." if is_dev_mode_no_margins() else "text"
+        self.label = QPlainTextEdit(default_label_text)
         self.label.setFixedHeight(15 * (len(self.label.toPlainText().splitlines()) + 2))
         self.setFixedHeight(self.label.height() + 10)
         self.font_style = FontStyle()
         self.font_size = QSpinBox()
         self.font_size.setMaximum(150)
         self.font_size.setMinimum(0)
         self.font_size.setSingleStep(1)
@@ -163,26 +166,25 @@
         """Get the render engine for the text label using the current settings.
 
         Returns
         -------
             TextRenderEngine: The rendered engine.
 
         """
-        selected_alignment = self.align.currentText()
-        assert selected_alignment in ("left", "center", "right")
+        selected_alignment = Direction(self.align.currentText())
         return TextRenderEngine(
             text_lines=self.label.toPlainText().splitlines(),
             font_file_name=self.font_style.currentData(),
             frame_width_px=self.frame_width_px.value(),
             font_size_ratio=self.font_size.value() / 100.0,
             align=selected_alignment,
         )
 
 
-class QrDymoLabelWidget(BaseDymoLabelWidget):
+class QrDymoLabelWidget(BaseLabelWidget):
     """A widget for rendering QR codes on Dymo labels.
 
     Args:
     ----
         render_context (RenderContext): The render context to use for rendering
             the QR code.
         parent (QWidget, optional): The parent widget. Defaults to None.
@@ -223,15 +225,15 @@
         """
         try:
             return QrRenderEngine(content=self.label.text())
         except NoContentError:
             return EmptyRenderEngine()
 
 
-class BarcodeDymoLabelWidget(BaseDymoLabelWidget):
+class BarcodeDymoLabelWidget(BaseLabelWidget):
     """A widget for rendering barcode labels using the Dymo label printer.
 
     Args:
     ----
         render_context (RenderContext): An instance of the RenderContext class.
         parent (QWidget): The parent widget of this widget.
 
@@ -299,15 +301,15 @@
 
         self.set_text_fields_visibility(True)
 
         layout = QHBoxLayout()
 
         self.barcode_type_label = QLabel("Type:")
         self.barcode_type = QComboBox()
-        self.barcode_type.addItems(AVAILABLE_BARCODES)
+        self.barcode_type.addItems(bt.value for bt in BarcodeType)
 
         # Checkbox for toggling text fields
         self.show_text_label = QLabel("Text:")
         self.show_text_checkbox = QCheckBox()
         self.show_text_checkbox.setChecked(True)
         self.show_text_checkbox.stateChanged.connect(
             self.toggle_text_fields_and_rerender
@@ -366,14 +368,15 @@
 
         Returns
         -------
             RenderEngine: The rendered engine (either BarcodeRenderEngine or
             BarcodeWithTextRenderEngine).
 
         """
+        render_engine: RenderEngine
         if self.show_text_checkbox.isChecked():
             render_engine = BarcodeWithTextRenderEngine(
                 content=self.label.text(),
                 barcode_type=self.barcode_type.currentText(),
                 font_file_name=self.font_style.currentData(),
                 frame_width_px=self.frame_width_px.value(),
                 font_size_ratio=self.font_size.value() / 100.0,
@@ -383,15 +386,15 @@
             render_engine = BarcodeRenderEngine(
                 content=self.label.text(),
                 barcode_type=self.barcode_type.currentText(),
             )
         return render_engine
 
 
-class ImageDymoLabelWidget(BaseDymoLabelWidget):
+class ImageDymoLabelWidget(BaseLabelWidget):
     """A widget for rendering image-based Dymo labels.
 
     Args:
     ----
         context (RenderContext): The render context to use for rendering the label.
         parent (QWidget, optional): The parent widget. Defaults to None.
```

### Comparing `labelle-1.1.0/src/labelle/gui/q_dymo_labels_list.py` & `labelle-1.2.0/src/labelle/gui/q_labels_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import logging
-from typing import Literal, Optional
+from typing import Optional
 
 from PIL import Image
 from PyQt6 import QtCore
 from PyQt6.QtGui import QAction
 from PyQt6.QtWidgets import QAbstractItemView, QListWidget, QListWidgetItem, QMenu
 
 from labelle.gui.common import crash_msg_box
-from labelle.gui.q_dymo_label_widgets import (
+from labelle.gui.q_label_widgets import (
     BarcodeDymoLabelWidget,
     EmptyRenderEngine,
     ImageDymoLabelWidget,
     QrDymoLabelWidget,
     TextDymoLabelWidget,
 )
-from labelle.lib.dymo_labeler import DymoLabeler
+from labelle.lib.constants import Direction
+from labelle.lib.devices.dymo_labeler import DymoLabeler
 from labelle.lib.render_engines import (
     HorizontallyCombinedRenderEngine,
     PrintPayloadRenderEngine,
     PrintPreviewRenderEngine,
     RenderContext,
 )
 from labelle.lib.render_engines.render_engine import (
     RenderEngineException,
 )
 from labelle.lib.utils import mm_to_px
 
 LOG = logging.getLogger(__name__)
 
 
-class QDymoLabelList(QListWidget):
+class QLabelList(QListWidget):
     """A custom QListWidget for displaying and managing Dymo label widgets.
 
     Args:
     ----
         render_context (RenderContext): The render context to use for rendering the
         label.
         parent (QWidget): The parent widget of this QListWidget.
@@ -69,30 +70,31 @@
         Image.Image, name="renderPrintPreviewSignal"
     )
     renderPrintPayloadSignal = QtCore.pyqtSignal(
         Image.Image, name="renderPrintPayloadSignal"
     )
     render_context: Optional[RenderContext]
     itemWidget: TextDymoLabelWidget
-    dymo_labeler: DymoLabeler
+    dymo_labeler: Optional[DymoLabeler]
     h_margin_mm: float
     min_label_width_mm: Optional[float]
-    justify: str
+    justify: Direction
 
     def __init__(self, parent=None):
         super().__init__(parent)
         self.dymo_labeler = None
-        self.margin_px = None
+        self.h_margin_mm = 0.0
         self.min_label_width_mm = None
-        self.justify = "center"
+        self.justify = Direction.CENTER
         self.render_context = None
         self.setAlternatingRowColors(True)
         self.setDragDropMode(QAbstractItemView.DragDropMode.InternalMove)
 
     def populate(self):
+        assert self.render_context is not None
         for item_widget in [TextDymoLabelWidget(self.render_context)]:
             item = QListWidgetItem(self)
             item.setSizeHint(item_widget.sizeHint())
             self.addItem(item)
             self.setItemWidget(item, item_widget)
             item_widget.itemRenderSignal.connect(self.render_label)
 
@@ -109,15 +111,15 @@
 
     def update_params(
         self,
         dymo_labeler: DymoLabeler,
         h_margin_mm: float,
         min_label_width_mm: float,
         render_context: RenderContext,
-        justify: Literal["left", "center", "right"] = "center",
+        justify: Direction = Direction.CENTER,
     ):
         """Update the render context used for rendering the label.
 
         Args:
         ----
             dymo_labeler: an instance of DymoLabeler object
             h_margin_mm: horizontal margin [mm]
@@ -144,14 +146,16 @@
             item_widget = self.itemWidget(self.item(i))
             if item_widget and item:
                 item.setSizeHint(item_widget.sizeHint())
                 render_engines.append(item_widget.render_engine)
         return HorizontallyCombinedRenderEngine(render_engines=render_engines)
 
     def render_preview(self):
+        assert self.dymo_labeler is not None
+        assert self.render_context is not None
         render_engine = PrintPreviewRenderEngine(
             render_engine=self._payload_render_engine,
             justify=self.justify,
             visible_horizontal_margin_px=mm_to_px(self.h_margin_mm),
             labeler_margin_px=self.dymo_labeler.labeler_margin_px,
             max_width_px=None,
             min_width_px=mm_to_px(self.min_label_width_mm),
@@ -161,24 +165,26 @@
         except RenderEngineException as err:
             crash_msg_box(self, "Render Engine Failed!", err)
             bitmap = EmptyRenderEngine().render(self.render_context)
 
         self.renderPrintPreviewSignal.emit(bitmap)
 
     def render_print(self):
+        assert self.dymo_labeler is not None
+        assert self.render_context is not None
         render_engine = PrintPayloadRenderEngine(
             render_engine=self._payload_render_engine,
             justify=self.justify,
             visible_horizontal_margin_px=mm_to_px(self.h_margin_mm),
             labeler_margin_px=self.dymo_labeler.labeler_margin_px,
             max_width_px=None,
             min_width_px=mm_to_px(self.min_label_width_mm),
         )
         try:
-            bitmap, _ = render_engine.render(self.render_context)
+            bitmap, _ = render_engine.render_with_meta(self.render_context)
         except RenderEngineException as err:
             crash_msg_box(self, "Render Engine Failed!", err)
             bitmap = EmptyRenderEngine().render(self.render_context)
 
         self.renderPrintPayloadSignal.emit(bitmap)
 
     def render_label(self):
@@ -189,14 +195,15 @@
         """Override the default context menu event to add or delete label widgets.
 
         Args:
         ----
             event (QContextMenuEvent): The context menu event.
 
         """
+        assert self.render_context is not None
         contextMenu = QMenu(self)
         add_text: Optional[QAction] = contextMenu.addAction("Add Text")
         add_qr: Optional[QAction] = contextMenu.addAction("Add QR")
         add_barcode: Optional[QAction] = contextMenu.addAction("Add Barcode")
         add_img: Optional[QAction] = contextMenu.addAction("Add Image")
         delete: Optional[QAction] = contextMenu.addAction("Delete")
         menu_click = contextMenu.exec(event.globalPos())
```

### Comparing `labelle-1.1.0/src/labelle/lib/barcode_writer.py` & `labelle-1.2.0/src/labelle/lib/barcode_writer.py`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/lib/config_file.py` & `labelle-1.2.0/src/labelle/lib/config_file.py`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/lib/dymo_labeler.py` & `labelle-1.2.0/src/labelle/lib/devices/dymo_labeler.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 import math
 
 import usb
 from PIL import Image
 from usb.core import NoBackendError, USBError
 
 from labelle.lib.constants import ESC, SYN
-from labelle.lib.detect import DetectedDevice, DymoUSBError, detect_device
+from labelle.lib.devices.usb_device import UsbDevice, UsbDeviceError
 from labelle.lib.utils import mm_to_px
 
 LOG = logging.getLogger(__name__)
-POSSIBLE_USB_ERRORS = (DymoUSBError, NoBackendError, USBError)
+POSSIBLE_USB_ERRORS = (UsbDeviceError, NoBackendError, USBError)
 
 
 class DymoLabelerDetectError(Exception):
     def __init__(self, error: str):
         msg = f"Detection error: {error}"
         super().__init__(msg)
 
@@ -231,46 +231,47 @@
             self._line(line)
         self._status_request()
         status = self._get_status()
         LOG.debug(f"Post-send response: {status}")
 
 
 class DymoLabeler:
-    device: DetectedDevice
+    _device: UsbDevice | None
     tape_size_mm: int
 
     LABELER_DISTANCE_BETWEEN_PRINT_HEAD_AND_CUTTER_MM = 8.1
     LABELER_PRINT_HEAD_HEIGHT_MM = 8.2
     SUPPORTED_TAPE_SIZES_MM = (19, 12, 9, 6)
     DEFAULT_TAPE_SIZE_MM = 12
 
     def __init__(
         self,
-        tape_size_mm: int = DEFAULT_TAPE_SIZE_MM,
+        tape_size_mm: int | None = None,
+        device: UsbDevice | None = None,
     ):
+        if tape_size_mm is None:
+            tape_size_mm = self.DEFAULT_TAPE_SIZE_MM
         if tape_size_mm not in self.SUPPORTED_TAPE_SIZES_MM:
             raise ValueError(
                 f"Unsupported tape size {tape_size_mm}mm. "
                 f"Supported sizes: {self.SUPPORTED_TAPE_SIZES_MM}"
             )
         self.tape_size_mm = tape_size_mm
-        self.device = None
+        self._device = device
 
     @property
     def height_px(self):
         return DymoLabelerFunctions.height_px(self.tape_size_mm)
 
     @property
-    def _functions(self):
-        if not self.device:
-            self.detect()
-        assert self.device is not None
+    def _functions(self) -> DymoLabelerFunctions:
+        assert self._device is not None
         return DymoLabelerFunctions(
-            devout=self.device.devout,
-            devin=self.device.devin,
+            devout=self._device.devout,
+            devin=self._device.devin,
             synwait=64,
         )
 
     @property
     def minimum_horizontal_margin_mm(self):
         return self.LABELER_DISTANCE_BETWEEN_PRINT_HEAD_AND_CUTTER_MM
 
@@ -281,33 +282,45 @@
         )
 
         return (
             mm_to_px(self.minimum_horizontal_margin_mm),
             mm_to_px(vertical_margin_mm),
         )
 
-    def detect(self):
+    @property
+    def device(self) -> UsbDevice | None:
+        return self._device
+
+    @device.setter
+    def device(self, device: UsbDevice | None):
         try:
-            self.device = detect_device()
-        except POSSIBLE_USB_ERRORS as e:
-            raise DymoLabelerDetectError(str(e)) from e
+            if device:
+                device.setup()
+        except UsbDeviceError as e:
+            device = None
+            LOG.error(e)
+        self._device = device
+
+    @property
+    def is_ready(self) -> bool:
+        return self.device is not None
 
     def print(
         self,
         bitmap: Image.Image,
     ) -> None:
         """Print a label bitmap to the detected printer.
 
         The label bitmap is a PIL image in 1-bit format (mode=1), and pixels with value
         equal to 1 are burned.
         """
         # Convert the image to the proper matrix for the dymo labeler object so that
         # rows span the width of the label, and the first row corresponds to the left
         # edge of the label.
-        rotated_bitmap = bitmap.transpose(Image.ROTATE_270)
+        rotated_bitmap = bitmap.transpose(Image.Transpose.ROTATE_270)
 
         # Convert the image to raw bytes. Pixels along rows are chunked into groups of
         # 8 pixels, and subsequent rows are concatenated.
         stream: bytes = rotated_bitmap.tobytes()
 
         # Regather the bytes into rows
         stream_row_length = int(math.ceil(bitmap.height / 8))
@@ -326,11 +339,12 @@
             array.array("B", label_row).tolist() for label_row in label_rows
         ]
 
         try:
             LOG.debug("Printing label..")
             self._functions.print_label(label_matrix)
             LOG.debug("Done printing.")
-            usb.util.dispose_resources(self.device.dev)
+            if self._device is not None:
+                self._device.dispose()
             LOG.debug("Cleaned up.")
         except POSSIBLE_USB_ERRORS as e:
             raise DymoLabelerPrintError(str(e)) from e
```

### Comparing `labelle-1.1.0/src/labelle/lib/font_config.py` & `labelle-1.2.0/src/labelle/lib/font_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from enum import Enum
 from pathlib import Path
 from typing import Dict, List, Optional
 
 import labelle.resources.fonts
 from labelle._vendor.matplotlib import font_manager
 from labelle.lib.config_file import get_config_section
 
@@ -27,14 +28,24 @@
     "regular": _DEFAULT_FONTS_DIR / "Carlito-Regular.ttf",
     "bold": _DEFAULT_FONTS_DIR / "Carlito-Bold.ttf",
     "italic": _DEFAULT_FONTS_DIR / "Carlito-Italic.ttf",
     "narrow": _DEFAULT_FONTS_DIR / "Carlito-BoldItalic.ttf",
 }
 
 
+class FontStyle(str, Enum):
+    REGULAR = "regular"
+    BOLD = "bold"
+    ITALIC = "italic"
+    NARROW = "narrow"
+
+
+DefaultFontStyle = FontStyle(_DEFAULT_STYLE)
+
+
 def _get_styles_to_font_path_lookup() -> Dict[str, Path]:
     """Get a lookup table for styles to font paths.
 
     The lookup table is read from the config file, if available.
     """
     styles_to_font_path = _DEFAULT_STYLES_TO_FONT_PATH.copy()
     fonts_config = get_config_section("FONTS")
```

### Comparing `labelle-1.1.0/src/labelle/lib/unicode_blocks.py` & `labelle-1.2.0/src/labelle/lib/unicode_blocks.py`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/lib/utils.py` & `labelle-1.2.0/src/labelle/lib/utils.py`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/lib/render_engines/__init__.py` & `labelle-1.2.0/src/labelle/lib/render_engines/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 from labelle.lib.render_engines.qr import NoContentError, QrRenderEngine
 from labelle.lib.render_engines.render_context import RenderContext
 from labelle.lib.render_engines.render_engine import RenderEngine
 from labelle.lib.render_engines.test_pattern import TestPatternRenderEngine
 from labelle.lib.render_engines.text import TextRenderEngine
 
 __all__ = [
-    BarcodeRenderEngine,
-    BarcodeWithTextRenderEngine,
-    EmptyRenderEngine,
-    HorizontallyCombinedRenderEngine,
-    MarginsRenderEngine,
-    NoContentError,
-    NoPictureFilePath,
-    PictureRenderEngine,
-    PrintPayloadRenderEngine,
-    PrintPreviewRenderEngine,
-    QrRenderEngine,
-    RenderContext,
-    RenderEngine,
-    TestPatternRenderEngine,
-    TextRenderEngine,
+    "BarcodeRenderEngine",
+    "BarcodeWithTextRenderEngine",
+    "EmptyRenderEngine",
+    "HorizontallyCombinedRenderEngine",
+    "MarginsRenderEngine",
+    "NoContentError",
+    "NoPictureFilePath",
+    "PictureRenderEngine",
+    "PrintPayloadRenderEngine",
+    "PrintPreviewRenderEngine",
+    "QrRenderEngine",
+    "RenderContext",
+    "RenderEngine",
+    "TestPatternRenderEngine",
+    "TextRenderEngine",
 ]
```

### Comparing `labelle-1.1.0/src/labelle/lib/render_engines/barcode.py` & `labelle-1.2.0/src/labelle/lib/render_engines/barcode.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,32 @@
+from __future__ import annotations
+
 import barcode as barcode_module
 from PIL import Image
 
 from labelle.lib.barcode_writer import BarcodeImageWriter
+from labelle.lib.constants import DEFAULT_BARCODE_TYPE
 from labelle.lib.render_engines.render_context import RenderContext
 from labelle.lib.render_engines.render_engine import (
     RenderEngine,
     RenderEngineException,
 )
 
 
 class BarcodeRenderError(RenderEngineException):
     def __init__(self):
         msg = "Barcode render error"
         super().__init__(msg)
 
 
 class BarcodeRenderEngine(RenderEngine):
-    def __init__(self, content, barcode_type):
+    def __init__(self, content: str, barcode_type: str | None):
         super().__init__()
         self.content = content
-        self.barcode_type = barcode_type
+        self.barcode_type = barcode_type or DEFAULT_BARCODE_TYPE
 
     def render(self, context: RenderContext) -> Image.Image:
         code = barcode_module.get(
             self.barcode_type, self.content, writer=BarcodeImageWriter()
         )
         try:
             bitmap = code.render(
```

### Comparing `labelle-1.1.0/src/labelle/lib/render_engines/barcode_with_text.py` & `labelle-1.2.0/src/labelle/lib/render_engines/barcode_with_text.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Literal
 
 from PIL import Image
 
+from labelle.lib.constants import Direction
 from labelle.lib.render_engines.barcode import BarcodeRenderEngine
 from labelle.lib.render_engines.render_context import RenderContext
 from labelle.lib.render_engines.render_engine import (
     RenderEngine,
     RenderEngineException,
 )
 from labelle.lib.render_engines.text import TextRenderEngine
@@ -16,19 +16,19 @@
 
 class BarcodeWithTextRenderEngine(RenderEngine):
     TEXT_HEIGHT_SCALE_FACTOR = 0.4
 
     def __init__(
         self,
         content: str,
-        barcode_type,
+        barcode_type: str | None,
         font_file_name: Path | str,
-        frame_width_px: int,
+        frame_width_px: int | None,
         font_size_ratio: float = 0.9,
-        align: Literal["left", "center", "right"] = "center",
+        align: Direction = Direction.CENTER,
     ):
         super().__init__()
         self._barcode = BarcodeRenderEngine(content, barcode_type)
         self._text = TextRenderEngine(
             content, font_file_name, frame_width_px, font_size_ratio, align
         )
         self.align = align
```

### Comparing `labelle-1.1.0/src/labelle/lib/render_engines/horizontally_combined.py` & `labelle-1.2.0/src/labelle/lib/render_engines/horizontally_combined.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 
+from typing import Sequence
+
 from PIL import Image
 
 from labelle.lib.render_engines.empty import EmptyRenderEngine
 from labelle.lib.render_engines.render_context import RenderContext
 from labelle.lib.render_engines.render_engine import RenderEngine
 
 
 class HorizontallyCombinedRenderEngine(RenderEngine):
     PADDING = 4
 
     def __init__(
         self,
-        render_engines: list[RenderEngine],
+        render_engines: Sequence[RenderEngine],
     ):
         super().__init__()
         self.render_engines = render_engines
 
     def render(self, context: RenderContext) -> Image.Image:
         render_engines = self.render_engines or [EmptyRenderEngine()]
         bitmaps = [engine.render(context) for engine in render_engines]
```

### Comparing `labelle-1.1.0/src/labelle/lib/render_engines/margins.py` & `labelle-1.2.0/src/labelle/lib/render_engines/margins.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import math
 from typing import Literal
 
 from PIL import Image
 
+from labelle.lib.constants import Direction
+from labelle.lib.env_config import is_dev_mode_no_margins
 from labelle.lib.render_engines.render_context import RenderContext
 from labelle.lib.render_engines.render_engine import (
     RenderEngine,
     RenderEngineException,
 )
 
 
@@ -19,60 +21,72 @@
 
 
 class MarginsRenderEngine(RenderEngine):
     def __init__(
         self,
         render_engine: RenderEngine,
         mode: Literal["print", "preview"],
-        justify: Literal["left", "center", "right"] = "center",
+        justify: Direction = Direction.CENTER,
         visible_horizontal_margin_px: float = 0,
         labeler_margin_px: tuple[float, float] = (0, 0),
         max_width_px: float | None = None,
-        min_width_px: float = 0,
+        min_width_px: float | None = 0,
     ):
         super().__init__()
         labeler_horizontal_margin_px, labeler_vertical_margin_px = labeler_margin_px
         assert visible_horizontal_margin_px >= 0
         assert labeler_horizontal_margin_px >= 0
         assert labeler_vertical_margin_px >= 0
         assert not max_width_px or max_width_px >= 0
+        if min_width_px is None:
+            min_width_px = 0
         assert min_width_px >= 0
         self.mode = mode
         self.justify = justify
-        self.visible_horizontal_margin_px = visible_horizontal_margin_px
-        self.labeler_horizontal_margin_px = labeler_horizontal_margin_px
+        if is_dev_mode_no_margins():
+            self.visible_horizontal_margin_px = 0.0
+            self.labeler_horizontal_margin_px = 0.0
+            self.min_width_px = 0.0
+        else:
+            self.visible_horizontal_margin_px = visible_horizontal_margin_px
+            self.labeler_horizontal_margin_px = labeler_horizontal_margin_px
+            self.min_width_px = min_width_px
         self.labeler_vertical_margin_px = labeler_vertical_margin_px
         self.max_width_px = max_width_px
-        self.min_width_px = min_width_px
         self.render_engine = render_engine
 
-    def calculate_visible_width(self, payload_width_px: int) -> float:
+    def _calculate_visible_width(self, payload_width_px: int) -> float:
         minimal_label_width_px = (
-            payload_width_px + self.visible_horizontal_margin_px * 2
+            payload_width_px + self.visible_horizontal_margin_px * 2.0
         )
         if self.max_width_px is not None and minimal_label_width_px > self.max_width_px:
             raise BitmapTooBigError(minimal_label_width_px, self.max_width_px)
 
         if self.min_width_px > minimal_label_width_px:
             label_width_px = self.min_width_px
         else:
             label_width_px = minimal_label_width_px
         return label_width_px
 
-    def render(self, context: RenderContext) -> tuple[Image.Image, dict[str, float]]:
+    def render(self, _: RenderContext) -> Image.Image:
+        raise RuntimeError("This should never be called")
+
+    def render_with_meta(
+        self, context: RenderContext
+    ) -> tuple[Image.Image, dict[str, float]]:
         payload_bitmap = self.render_engine.render(context)
         payload_width_px = payload_bitmap.width
-        label_width_px = self.calculate_visible_width(payload_width_px)
+        label_width_px = self._calculate_visible_width(payload_width_px)
         padding_px = label_width_px - payload_width_px  # sum of margins from both sides
 
-        if self.justify == "left":
+        if self.justify == Direction.LEFT:
             horizontal_offset_px = self.visible_horizontal_margin_px
-        elif self.justify == "center":
+        elif self.justify == Direction.CENTER:
             horizontal_offset_px = padding_px / 2
-        elif self.justify == "right":
+        elif self.justify == Direction.RIGHT:
             horizontal_offset_px = padding_px - self.visible_horizontal_margin_px
         assert horizontal_offset_px >= self.visible_horizontal_margin_px
 
         # In print mode:
         # ==============
         # There is a gap between the printer head and the cutter (for the sake of this
         # example, let us say it is DX pixels wide).
@@ -92,18 +106,20 @@
         # edge
 
         vertical_offset_px: float = 0
         if self.mode == "print":
             # print head is already in offset from label's edge under the cutter
             horizontal_offset_px -= self.labeler_horizontal_margin_px
             # no need to add vertical margins to bitmap
-            bitmap_height = payload_bitmap.height
+            bitmap_height = float(payload_bitmap.height)
         elif self.mode == "preview":
             # add vertical margins to bitmap
-            bitmap_height = payload_bitmap.height + self.labeler_vertical_margin_px * 2
+            bitmap_height = (
+                float(payload_bitmap.height) + self.labeler_vertical_margin_px * 2.0
+            )
             vertical_offset_px = self.labeler_vertical_margin_px
 
         bitmap = Image.new("1", (math.ceil(label_width_px), math.ceil(bitmap_height)))
         bitmap.paste(
             payload_bitmap, box=(round(horizontal_offset_px), round(vertical_offset_px))
         )
         meta = {
```

### Comparing `labelle-1.1.0/src/labelle/lib/render_engines/picture.py` & `labelle-1.2.0/src/labelle/lib/render_engines/picture.py`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/lib/render_engines/print_payload.py` & `labelle-1.2.0/src/labelle/lib/render_engines/print_payload.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 from __future__ import annotations
 
-from typing import Literal
-
 from PIL import Image
 
+from labelle.lib.constants import Direction
 from labelle.lib.render_engines.margins import MarginsRenderEngine
 from labelle.lib.render_engines.render_context import RenderContext
 from labelle.lib.render_engines.render_engine import RenderEngine
 
 
 class PrintPayloadRenderEngine(RenderEngine):
     def __init__(
         self,
         render_engine: RenderEngine,
-        justify: Literal["left", "center", "right"] = "center",
+        justify: Direction = Direction.CENTER,
         visible_horizontal_margin_px: float = 0,
         labeler_margin_px: tuple[float, float] = (0, 0),
         max_width_px: float | None = None,
-        min_width_px: float = 0,
+        min_width_px: float | None = 0,
     ):
         super().__init__()
         self.render_engine = MarginsRenderEngine(
             render_engine=render_engine,
             mode="print",
             justify=justify,
             visible_horizontal_margin_px=visible_horizontal_margin_px,
             labeler_margin_px=labeler_margin_px,
             max_width_px=max_width_px,
             min_width_px=min_width_px,
         )
 
-    def render(self, context: RenderContext) -> tuple[Image.Image, dict[str, float]]:
-        return self.render_engine.render(context)
+    def render(self, _: RenderContext) -> Image.Image:
+        raise RuntimeError("This should never be called")
+
+    def render_with_meta(
+        self, context: RenderContext
+    ) -> tuple[Image.Image, dict[str, float]]:
+        return self.render_engine.render_with_meta(context)
```

### Comparing `labelle-1.1.0/src/labelle/lib/render_engines/print_preview.py` & `labelle-1.2.0/src/labelle/lib/render_engines/print_preview.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
-from typing import Literal
-
 from darkdetect import isDark
 from PIL import Image, ImageColor, ImageDraw, ImageOps
 
+from labelle.lib.constants import Direction
 from labelle.lib.render_engines.margins import MarginsRenderEngine
 from labelle.lib.render_engines.render_context import RenderContext
 from labelle.lib.render_engines.render_engine import RenderEngine
 from labelle.lib.utils import px_to_mm
 
 
 class PrintPreviewRenderEngine(RenderEngine):
@@ -16,15 +15,15 @@
     Y_MARGIN_PX = 30
     DX = X_MARGIN_PX * 0.3
     DY = Y_MARGIN_PX * 0.3
 
     def __init__(
         self,
         render_engine: RenderEngine,
-        justify: Literal["left", "center", "right"] = "center",
+        justify: Direction = Direction.CENTER,
         visible_horizontal_margin_px: float = 0,
         labeler_margin_px: tuple[float, float] = (0, 0),
         max_width_px: float | None = None,
         min_width_px: float = 0,
     ):
         super().__init__()
         self.render_engine = MarginsRenderEngine(
@@ -46,15 +45,15 @@
         return "yellow" if isDark() else "red"
 
     @staticmethod
     def _get_text_color():
         return "white" if isDark() else "blue"
 
     def _get_label_bitmap(self, context: RenderContext):
-        render_bitmap, meta = self.render_engine.render(context)
+        render_bitmap, meta = self.render_engine.render_with_meta(context)
         bitmap = ImageOps.invert(render_bitmap.convert("L")).convert("RGBA")
         pixel_map = {
             "black": context.foreground_color,
             "white": context.background_color,
         }
         pixel_color_map = {
             ImageColor.getcolor(k, "RGBA"): ImageColor.getcolor(v, "RGBA")
```

### Comparing `labelle-1.1.0/src/labelle/lib/render_engines/qr.py` & `labelle-1.2.0/src/labelle/lib/render_engines/qr.py`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/lib/render_engines/test_pattern.py` & `labelle-1.2.0/src/labelle/lib/render_engines/test_pattern.py`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/lib/render_engines/text.py` & `labelle-1.2.0/src/labelle/lib/render_engines/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Literal
 
 from PIL import Image, ImageFont
 
+from labelle.lib.constants import Direction
 from labelle.lib.render_engines.render_context import RenderContext
 from labelle.lib.render_engines.render_engine import RenderEngine
 from labelle.lib.utils import draw_image
 
 
 class TextRenderEngine(RenderEngine):
     def __init__(
         self,
         text_lines: str | list[str],
         font_file_name: Path | str,
-        frame_width_px: int,
+        frame_width_px: int | None,
         font_size_ratio: float = 0.9,
-        align: Literal["left", "center", "right"] = "left",
+        align: Direction = Direction.CENTER,
     ):
         if isinstance(text_lines, str):
             text_lines = [text_lines]
 
         if len(text_lines) == 0:
             text_lines = [" "]
 
         self.text_lines = text_lines
         self.font_file_name = font_file_name
-        self.frame_width_px = frame_width_px
+        self.frame_width_px = frame_width_px or 0
         self.font_size_ratio = font_size_ratio
         self.align = align
 
         super().__init__()
 
     def render(self, context: RenderContext) -> Image.Image:
         height_px = context.height_px
         line_height = float(height_px) / len(self.text_lines)
         font_size_px = int(round(line_height * self.font_size_ratio))
 
         font_offset_px = int((line_height - font_size_px) / 2)
         if self.frame_width_px:
-            frame_width_px = min(self.frame_width_px, font_offset_px, 3)
+            frame_width_px = self.frame_width_px or min(
+                self.frame_width_px, font_offset_px, 3
+            )
         else:
             frame_width_px = self.frame_width_px
 
         font = ImageFont.truetype(str(self.font_file_name), font_size_px)
         boxes = (font.getbbox(line) for line in self.text_lines)
         line_widths = (right - left for left, _, right, _ in boxes)
         label_width_px = max(line_widths) + (font_offset_px * 2)
@@ -65,13 +67,13 @@
                 )
 
             # write the text into the empty image
             multiline_text = "\n".join(self.text_lines)
             draw.multiline_text(
                 (label_width_px / 2, height_px / 2),
                 multiline_text,
-                align=self.align,
+                align=self.align.value,
                 anchor="mm",
                 font=font,
                 fill=1,
             )
         return bitmap
```

### Comparing `labelle-1.1.0/src/labelle/resources/fonts/Carlito-Bold.ttf` & `labelle-1.2.0/src/labelle/resources/fonts/Carlito-Bold.ttf`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/resources/fonts/Carlito-BoldItalic.ttf` & `labelle-1.2.0/src/labelle/resources/fonts/Carlito-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/resources/fonts/Carlito-Italic.ttf` & `labelle-1.2.0/src/labelle/resources/fonts/Carlito-Italic.ttf`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/resources/fonts/Carlito-Regular.ttf` & `labelle-1.2.0/src/labelle/resources/fonts/Carlito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/resources/fonts/LICENSE` & `labelle-1.2.0/src/labelle/resources/fonts/LICENSE`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/resources/icons/barcode_icon.png` & `labelle-1.2.0/src/labelle/resources/icons/barcode_icon.png`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/resources/icons/img_icon.png` & `labelle-1.2.0/src/labelle/resources/icons/img_icon.png`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/resources/icons/logo_small.png` & `labelle-1.2.0/src/labelle/resources/icons/logo_small.png`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/src/labelle/resources/icons/txt_icon.png` & `labelle-1.2.0/src/labelle/resources/icons/txt_icon.png`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/vendoring/patches/matplotlib.patch` & `labelle-1.2.0/vendoring/patches/matplotlib.patch`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/.gitignore` & `labelle-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/LICENSE` & `labelle-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `labelle-1.1.0/README.md` & `labelle-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -234,12 +234,12 @@
 
 ## Disclaimers
 
 * This software is provided as-is, without any warranty. Please see [LICENSE](LICENSE)
   for details.
 * Labelle is not affiliated, associated, authorized, endorsed by, or in any way
   officially connected with DYMO, or any of its subsidiaries or its affiliates.
-  The official DYMO website can be found at [www.dymo.com](www.dymo.com).
+  The official DYMO website can be found at [www.dymo.com](https://www.dymo.com).
   The name DYMO®, as well as related names, marks, emblems, and images, are registered
   trademarks of their respective owners. Currently, Labelle software is designed
   to support certain devices manufactured by DYMO; however, no endorsement or
   partnership is implied.
```

### Comparing `labelle-1.1.0/pyproject.toml` & `labelle-1.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     "platformdirs",
     "Pillow>=8.1.2,<11",
     "PyQRCode>=1.2.1,<2",
     "python-barcode>=0.13.1,<1",
     "pyusb",
     "PyQt6",
     "darkdetect",
+    "typer",
 ]
 classifiers = [
     "Operating System :: POSIX :: Linux",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -78,21 +79,22 @@
 
 [testenv]
 commands =
   pip check
   pip freeze
   labelle --version
   labelle --help
-  labelle --preview "single line"
-  labelle --preview-inverted "single line"
-  labelle --preview multiple lines
-  labelle --preview -qr "qr text"
-  labelle --preview -c code128 "bc txt"
-  labelle --preview -qr "qr text" qr caption
-  labelle --preview -c code128 "bc txt" barcode caption
+  labelle --output console "single line"
+  labelle --output console_inverted "inverted"
+  labelle --output console multiple lines
+  labelle --output console --barcode "Barcode" --barcode-type code128
+  labelle --output console --barcode-with-text "Barcode" --barcode-type code128 Caption
+  labelle --output console --qr QR
+  labelle --output console --qr QR Caption
+  labelle --output console --picture ./labelle.png
 
 [testenv:{clean,build}]
 description =
     Build (or clean) the package in isolation according to instructions in:
     https://setuptools.readthedocs.io/en/latest/build_meta.html#how-to-use-it
     https://github.com/pypa/pep517/issues/91
     https://github.com/pypa/build
@@ -187,10 +189,15 @@
     "COM812", # missing-trailing-comma
     "COM819", # prohibited-trailing-comma
     "ISC001", # single-line-implicit-string-concatenation
     "ISC002", # multi-line-implicit-string-concatenation
 ]
 
 [tool.mypy]
-exclude = ["_vendor"]
 check_untyped_defs = true
 install_types = true
+mypy_path = "src/"
+packages = ["labelle"]
+
+[[tool.mypy.overrides]]
+module="labelle._vendor.*"
+ignore_errors = true
```

### Comparing `labelle-1.1.0/PKG-INFO` & `labelle-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: labelle
-Version: 1.1.0
+Version: 1.2.0
 Summary: Open-source label printing software
 Project-URL: Homepage, https://github.com/labelle-org/labelle
 Project-URL: source, https://github.com/labelle-org/labelle
 Project-URL: tracker, https://github.com/labelle-org/labelle/issues
 Author-email: "Sebastian J. Bronner" <waschtl@sbronner.com>
 Maintainer-email: Tomer Shalev <tshalev@proofpoint.com>, Ben Mares <services-labelle@tensorial.com>, Tomek Szczęsny <mctom@tlen.pl>
 License-Expression: Apache-2.0
@@ -22,14 +22,15 @@
 Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: pillow<11,>=8.1.2
 Requires-Dist: platformdirs
 Requires-Dist: pyqrcode<2,>=1.2.1
 Requires-Dist: pyqt6
 Requires-Dist: python-barcode<1,>=0.13.1
 Requires-Dist: pyusb
+Requires-Dist: typer
 Description-Content-Type: text/markdown
 
 # Labelle
 
 [![GitHub Actions (Tests)](https://github.com/labelle-org/labelle/workflows/Tests/badge.svg)](https://github.com/labelle-org/labelle)
 [![PyPI version](https://img.shields.io/pypi/v/labelle.svg)](https://pypi.org/project/labelle/)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/labelle-org/labelle/main.svg)](https://results.pre-commit.ci/latest/github/labelle-org/labelle/main)
@@ -264,12 +265,12 @@
 
 ## Disclaimers
 
 * This software is provided as-is, without any warranty. Please see [LICENSE](LICENSE)
   for details.
 * Labelle is not affiliated, associated, authorized, endorsed by, or in any way
   officially connected with DYMO, or any of its subsidiaries or its affiliates.
-  The official DYMO website can be found at [www.dymo.com](www.dymo.com).
+  The official DYMO website can be found at [www.dymo.com](https://www.dymo.com).
   The name DYMO®, as well as related names, marks, emblems, and images, are registered
   trademarks of their respective owners. Currently, Labelle software is designed
   to support certain devices manufactured by DYMO; however, no endorsement or
   partnership is implied.
```

