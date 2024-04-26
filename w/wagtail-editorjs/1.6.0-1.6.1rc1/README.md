# Comparing `tmp/wagtail_editorjs-1.6.0.tar.gz` & `tmp/wagtail_editorjs-1.6.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_editorjs-1.6.0.tar", last modified: Fri Apr 19 16:16:26 2024, max compression
+gzip compressed data, was "wagtail_editorjs-1.6.1rc1.tar", last modified: Fri Apr 26 23:56:32 2024, max compression
```

## Comparing `wagtail_editorjs-1.6.0.tar` & `wagtail_editorjs-1.6.1rc1.tar`

### file list

```diff
@@ -1,138 +1,146 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.104594 wagtail_editorjs-1.6.0/
--rw-rw-rw-   0        0        0    18429 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.0/LICENSE
--rw-rw-rw-   0        0        0      272 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4946 2024-04-19 16:16:26.104594 wagtail_editorjs-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     3687 2024-04-08 19:47:07.000000 wagtail_editorjs-1.6.0/README.md
--rw-rw-rw-   0        0        0       90 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.0/pyproject.toml
--rw-rw-rw-   0        0        0     1186 2024-04-19 16:16:26.116310 wagtail_editorjs-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-03-27 00:40:18.000000 wagtail_editorjs-1.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.948499 wagtail_editorjs-1.6.0/wagtail_editorjs/
--rw-rw-rw-   0        0        0      312 2024-04-19 16:16:23.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/__init__.py
--rw-rw-rw-   0        0        0      169 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/apps.py
--rw-rw-rw-   0        0        0     1985 2024-03-29 17:31:47.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/blocks.py
--rw-rw-rw-   0        0        0     2569 2024-04-08 19:06:41.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/django_editor.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.977420 wagtail_editorjs-1.6.0/wagtail_editorjs/features/
--rw-rw-rw-   0        0        0      588 2024-04-18 08:53:25.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/features/__init__.py
--rw-rw-rw-   0        0        0    10474 2024-04-18 21:16:10.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/features/blocks.py
--rw-rw-rw-   0        0        0     6818 2024-03-31 07:04:36.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/features/documents.py
--rw-rw-rw-   0        0        0     9823 2024-04-16 19:24:08.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/features/images.py
--rw-rw-rw-   0        0        0     5486 2024-04-18 22:08:22.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/features/inlines.py
--rw-rw-rw-   0        0        0     5164 2024-03-27 20:40:47.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/features/lists.py
--rw-rw-rw-   0        0        0     3983 2024-04-18 21:15:27.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/features/tunes.py
--rw-rw-rw-   0        0        0     1785 2024-04-16 12:46:42.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/fields.py
--rw-rw-rw-   0        0        0     6632 2024-04-16 13:02:46.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/forms.py
--rw-rw-rw-   0        0        0      319 2024-03-27 21:25:26.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.978420 wagtail_editorjs-1.6.0/wagtail_editorjs/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.980420 wagtail_editorjs-1.6.0/wagtail_editorjs/migrations/__pycache__/
--rw-rw-rw-   0        0        0      218 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/migrations/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.985422 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/
--rw-rw-rw-   0        0        0      906 2024-04-18 21:15:11.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.993563 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/element/
--rw-rw-rw-   0        0        0      229 2024-03-29 10:32:13.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/element/__init__.py
--rw-rw-rw-   0        0        0     2073 2024-03-28 19:01:37.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/element/attrs.py
--rw-rw-rw-   0        0        0     3494 2024-03-29 14:48:28.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/element/element.py
--rw-rw-rw-   0        0        0     1525 2024-03-27 14:19:36.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/element/utils.py
--rw-rw-rw-   0        0        0     7265 2024-03-27 21:04:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/feature_registry.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.005565 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/
--rw-rw-rw-   0        0        0      340 2024-04-18 21:14:51.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/__init__.py
--rw-rw-rw-   0        0        0     6980 2024-04-18 21:22:23.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/base.py
--rw-rw-rw-   0        0        0     2235 2024-04-18 09:40:47.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/basic.py
--rw-rw-rw-   0        0        0     8940 2024-04-18 22:02:25.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/inlines.py
--rw-rw-rw-   0        0        0      674 2024-04-18 21:56:20.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/snippets_inlines.py
--rw-rw-rw-   0        0        0     1258 2024-03-27 20:13:06.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/view.py
--rw-rw-rw-   0        0        0     3311 2024-04-16 12:34:49.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/value.py
--rw-rw-rw-   0        0        0     5353 2024-04-18 10:11:04.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/render.py
--rw-rw-rw-   0        0        0     1042 2024-04-08 19:04:03.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.913613 wagtail_editorjs-1.6.0/wagtail_editorjs/static/
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.916612 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.007560 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/css/
--rw-rw-rw-   0        0        0     9983 2024-04-18 19:17:32.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css
--rw-rw-rw-   0        0        0    13978 2024-04-18 10:03:45.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.013562 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/
--rw-rw-rw-   0        0        0     1371 2024-03-29 17:29:46.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js
--rw-rw-rw-   0        0        0     1155 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js
--rw-rw-rw-   0        0        0     2913 2024-03-29 23:54:47.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.017094 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/init/
--rw-rw-rw-   0        0        0       86 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/init/drag-drop.js
--rw-rw-rw-   0        0        0       94 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/init/undo-redo.js
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.028490 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/
--rw-rw-rw-   0        0        0      364 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/attaches.js
--rw-rw-rw-   0        0        0    12378 2024-04-18 09:49:54.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js
--rw-rw-rw-   0        0        0     5510 2024-04-18 21:24:20.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js
--rw-rw-rw-   0        0        0     3695 2024-04-18 21:50:35.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js
--rw-rw-rw-   0        0        0    11260 2024-04-18 09:47:53.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js
--rw-rw-rw-   0        0        0     3277 2024-03-26 20:38:45.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js
--rw-rw-rw-   0        0        0     7883 2024-04-18 08:43:02.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js
--rw-rw-rw-   0        0        0    16447 2024-04-18 09:47:21.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js
--rw-rw-rw-   0        0        0     6225 2024-04-18 22:11:04.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.919052 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.032678 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/
--rw-rw-rw-   0        0        0   208234 2024-03-28 10:17:35.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.061879 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/
--rw-rw-rw-   0        0        0    34797 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js
--rw-rw-rw-   0        0        0     7233 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js
--rw-rw-rw-   0        0        0     3222 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js
--rw-rw-rw-   0        0        0     1864 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js
--rw-rw-rw-   0        0        0    10151 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js
--rw-rw-rw-   0        0        0     6946 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js
--rw-rw-rw-   0        0        0    29531 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js
--rw-rw-rw-   0        0        0     2440 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js
--rw-rw-rw-   0        0        0    33560 2024-03-27 17:16:55.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js
--rw-rw-rw-   0        0        0    30466 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js
--rw-rw-rw-   0        0        0     2550 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js
--rw-rw-rw-   0        0        0    10575 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js
--rw-rw-rw-   0        0        0     3142 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js
--rw-rw-rw-   0        0        0     5481 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js
--rw-rw-rw-   0        0        0     3198 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js
--rw-rw-rw-   0        0        0    23954 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js
--rw-rw-rw-   0        0        0     9463 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js
--rw-rw-rw-   0        0        0     9644 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js
--rw-rw-rw-   0        0        0     8007 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js
--rw-rw-rw-   0        0        0    19237 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js
--rw-rw-rw-   0        0        0     3713 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js
--rw-rw-rw-   0        0        0    20734 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.063877 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/
--rw-rw-rw-   0        0        0    44137 2024-04-16 19:19:37.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.920052 wagtail_editorjs-1.6.0/wagtail_editorjs/templates/
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.065009 wagtail_editorjs-1.6.0/wagtail_editorjs/templates/wagtail_editorjs/
--rw-rw-rw-   0        0        0      123 2024-03-29 14:30:09.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/templates/wagtail_editorjs/rich_text.html
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.067013 wagtail_editorjs-1.6.0/wagtail_editorjs/templates/wagtail_editorjs/widgets/
--rw-rw-rw-   0        0        0      555 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.069585 wagtail_editorjs-1.6.0/wagtail_editorjs/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.072389 wagtail_editorjs-1.6.0/wagtail_editorjs/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      220 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      892 2024-03-28 09:30:53.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc
--rw-rw-rw-   0        0        0      349 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/templatetags/editorjs.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.074398 wagtail_editorjs-1.6.0/wagtail_editorjs/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.077397 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/__init__.py
--rw-rw-rw-   0        0        0      168 2024-04-08 18:30:48.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.078396 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.086681 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-03-26 23:51:58.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     2310 2024-04-08 19:05:43.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/base.py
--rw-rw-rw-   0        0        0     2585 2024-04-08 18:38:20.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/test_attrs.py
--rw-rw-rw-   0        0        0     2041 2024-04-08 18:42:47.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/test_inlines.py
--rw-rw-rw-   0        0        0     5862 2024-04-08 18:58:38.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/test_render.py
--rw-rw-rw-   0        0        0      707 2024-04-08 18:29:14.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.094849 wagtail_editorjs-1.6.0/wagtail_editorjs/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3826 2024-04-08 19:17:04.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/testapp/settings.py
--rw-rw-rw-   0        0        0     1176 2024-04-08 18:42:23.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/testapp/urls.py
--rw-rw-rw-   0        0        0      429 2024-04-08 18:29:49.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.101599 wagtail_editorjs-1.6.0/wagtail_editorjs/wagtail_hooks/
--rw-rw-rw-   0        0        0       74 2024-04-16 12:19:31.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     7231 2024-04-18 10:12:16.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/wagtail_hooks/features.py
--rw-rw-rw-   0        0        0      646 2024-03-27 20:14:22.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0      777 2024-04-16 12:19:25.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.103596 wagtail_editorjs-1.6.0/wagtail_editorjs.egg-info/
--rw-rw-rw-   0        0        0     4946 2024-04-19 16:16:25.000000 wagtail_editorjs-1.6.0/wagtail_editorjs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5464 2024-04-19 16:16:25.000000 wagtail_editorjs-1.6.0/wagtail_editorjs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 16:16:25.000000 wagtail_editorjs-1.6.0/wagtail_editorjs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-04-19 16:16:25.000000 wagtail_editorjs-1.6.0/wagtail_editorjs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-19 16:16:25.000000 wagtail_editorjs-1.6.0/wagtail_editorjs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:32.859429 wagtail_editorjs-1.6.1rc1/
+-rw-rw-rw-   0        0        0    18429 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.1rc1/LICENSE
+-rw-rw-rw-   0        0        0      272 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.1rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4987 2024-04-26 23:56:32.859429 wagtail_editorjs-1.6.1rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     3850 2024-04-26 23:55:47.000000 wagtail_editorjs-1.6.1rc1/README.md
+-rw-rw-rw-   0        0        0       90 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.1rc1/pyproject.toml
+-rw-rw-rw-   0        0        0     1189 2024-04-26 23:56:32.871946 wagtail_editorjs-1.6.1rc1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-03-27 00:40:18.000000 wagtail_editorjs-1.6.1rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:31.691428 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/
+-rw-rw-rw-   0        0        0      315 2024-04-26 23:56:28.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/__init__.py
+-rw-rw-rw-   0        0        0      169 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/apps.py
+-rw-rw-rw-   0        0        0     1985 2024-03-29 17:31:47.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/blocks.py
+-rw-rw-rw-   0        0        0     2569 2024-04-08 19:06:41.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/django_editor.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:31.749355 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/features/
+-rw-rw-rw-   0        0        0      609 2024-04-26 08:36:30.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/features/__init__.py
+-rw-rw-rw-   0        0        0    10474 2024-04-18 21:16:10.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/features/blocks.py
+-rw-rw-rw-   0        0        0     6818 2024-03-31 07:04:36.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/features/documents.py
+-rw-rw-rw-   0        0        0     9823 2024-04-16 19:24:08.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/features/images.py
+-rw-rw-rw-   0        0        0     6849 2024-04-26 22:00:46.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/features/inlines.py
+-rw-rw-rw-   0        0        0     5164 2024-03-27 20:40:47.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/features/lists.py
+-rw-rw-rw-   0        0        0     3983 2024-04-18 21:15:27.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/features/tunes.py
+-rw-rw-rw-   0        0        0     1785 2024-04-16 12:46:42.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/fields.py
+-rw-rw-rw-   0        0        0     6874 2024-04-26 08:34:08.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/forms.py
+-rw-rw-rw-   0        0        0      319 2024-03-27 21:25:26.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:31.750356 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:31.752867 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      218 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/migrations/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:31.755874 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/
+-rw-rw-rw-   0        0        0      906 2024-04-18 21:15:11.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:31.760877 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/element/
+-rw-rw-rw-   0        0        0      229 2024-03-29 10:32:13.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/element/__init__.py
+-rw-rw-rw-   0        0        0     2073 2024-03-28 19:01:37.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/element/attrs.py
+-rw-rw-rw-   0        0        0     3494 2024-03-29 14:48:28.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/element/element.py
+-rw-rw-rw-   0        0        0     1525 2024-03-27 14:19:36.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/element/utils.py
+-rw-rw-rw-   0        0        0     7265 2024-03-27 21:04:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/feature_registry.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:31.770396 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/features/
+-rw-rw-rw-   0        0        0      340 2024-04-18 21:14:51.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/features/__init__.py
+-rw-rw-rw-   0        0        0     7487 2024-04-26 08:32:56.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/features/base.py
+-rw-rw-rw-   0        0        0     2235 2024-04-18 09:40:47.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/features/basic.py
+-rw-rw-rw-   0        0        0     8877 2024-04-26 13:03:15.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/features/inlines.py
+-rw-rw-rw-   0        0        0      674 2024-04-18 21:56:20.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/features/snippets_inlines.py
+-rw-rw-rw-   0        0        0     1258 2024-03-27 20:13:06.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/features/view.py
+-rw-rw-rw-   0        0        0     3311 2024-04-16 12:34:49.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/value.py
+-rw-rw-rw-   0        0        0     5353 2024-04-18 10:11:04.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/render.py
+-rw-rw-rw-   0        0        0     1042 2024-04-08 19:04:03.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:31.645011 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:31.648009 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:31.793012 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/css/
+-rw-rw-rw-   0        0        0    10098 2024-04-26 12:36:15.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css
+-rw-rw-rw-   0        0        0    14154 2024-04-26 13:11:26.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:31.860010 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/
+-rw-rw-rw-   0        0        0     1371 2024-03-29 17:29:46.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js
+-rw-rw-rw-   0        0        0     1155 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js
+-rw-rw-rw-   0        0        0     2913 2024-04-26 11:54:42.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:31.885269 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/init/
+-rw-rw-rw-   0        0        0       86 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/init/drag-drop.js
+-rw-rw-rw-   0        0        0       94 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/init/undo-redo.js
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:32.041019 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/
+-rw-rw-rw-   0        0        0      364 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/attaches.js
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:32.047543 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/
+-rw-rw-rw-   0        0        0     2460 2024-04-26 21:59:35.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/frontend.js
+-rw-rw-rw-   0        0        0     4464 2024-04-26 12:37:59.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/wagtail-tooltips.js
+-rw-rw-rw-   0        0        0    12378 2024-04-18 09:49:54.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js
+-rw-rw-rw-   0        0        0     5510 2024-04-18 21:24:20.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js
+-rw-rw-rw-   0        0        0     3595 2024-04-26 10:29:04.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js
+-rw-rw-rw-   0        0        0    11260 2024-04-18 09:47:53.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js
+-rw-rw-rw-   0        0        0     3277 2024-03-26 20:38:45.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js
+-rw-rw-rw-   0        0        0     7883 2024-04-18 08:43:02.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js
+-rw-rw-rw-   0        0        0    16447 2024-04-18 09:47:21.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js
+-rw-rw-rw-   0        0        0     4197 2024-04-26 12:35:50.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-inline-tool.js
+-rw-rw-rw-   0        0        0     6225 2024-04-18 22:11:04.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:31.649011 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:32.151696 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/
+-rw-rw-rw-   0        0        0   208234 2024-03-28 10:17:35.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:32.709198 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/
+-rw-rw-rw-   0        0        0    34797 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js
+-rw-rw-rw-   0        0        0     7233 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js
+-rw-rw-rw-   0        0        0     3222 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js
+-rw-rw-rw-   0        0        0     1864 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js
+-rw-rw-rw-   0        0        0    10151 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js
+-rw-rw-rw-   0        0        0     6946 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js
+-rw-rw-rw-   0        0        0    29531 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js
+-rw-rw-rw-   0        0        0     2440 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js
+-rw-rw-rw-   0        0        0    33560 2024-03-27 17:16:55.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js
+-rw-rw-rw-   0        0        0    30466 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js
+-rw-rw-rw-   0        0        0     2550 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js
+-rw-rw-rw-   0        0        0    10575 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js
+-rw-rw-rw-   0        0        0     3142 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js
+-rw-rw-rw-   0        0        0     5481 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js
+-rw-rw-rw-   0        0        0     3198 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js
+-rw-rw-rw-   0        0        0    23954 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js
+-rw-rw-rw-   0        0        0     9463 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js
+-rw-rw-rw-   0        0        0     9644 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js
+-rw-rw-rw-   0        0        0     8007 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js
+-rw-rw-rw-   0        0        0    19237 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js
+-rw-rw-rw-   0        0        0     3713 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js
+-rw-rw-rw-   0        0        0    20734 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:32.740390 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/
+-rw-rw-rw-   0        0        0    44137 2024-04-16 19:19:37.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:32.812999 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/
+-rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/LICENSE
+-rw-rw-rw-   0        0        0    20122 2024-04-23 14:51:23.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/popper.min.js
+-rw-rw-rw-   0        0        0    25717 2024-04-23 14:51:31.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/tippy-bundle.min.js
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:31.651009 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/templates/
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:32.821051 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/templates/wagtail_editorjs/
+-rw-rw-rw-   0        0        0      123 2024-03-29 14:30:09.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/templates/wagtail_editorjs/rich_text.html
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:32.831230 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/templates/wagtail_editorjs/widgets/
+-rw-rw-rw-   0        0        0      555 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:32.834744 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:32.837743 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      220 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2309 2024-04-25 19:47:38.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1497 2024-04-25 19:47:36.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/templatetags/editorjs.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:32.839743 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:32.841744 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/core/__init__.py
+-rw-rw-rw-   0        0        0      168 2024-04-08 18:30:48.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:32.842743 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/core/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:32.847918 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-26 23:51:58.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     2310 2024-04-08 19:05:43.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     2585 2024-04-08 18:38:20.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/core/tests/test_attrs.py
+-rw-rw-rw-   0        0        0     2041 2024-04-08 18:42:47.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/core/tests/test_inlines.py
+-rw-rw-rw-   0        0        0     5862 2024-04-08 18:58:38.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/core/tests/test_render.py
+-rw-rw-rw-   0        0        0      707 2024-04-08 18:29:14.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:32.852918 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3826 2024-04-08 19:17:04.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/testapp/settings.py
+-rw-rw-rw-   0        0        0     1176 2024-04-08 18:42:23.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      429 2024-04-08 18:29:49.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:32.858429 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/wagtail_hooks/
+-rw-rw-rw-   0        0        0       74 2024-04-16 12:19:31.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     7364 2024-04-26 09:19:37.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/wagtail_hooks/features.py
+-rw-rw-rw-   0        0        0      646 2024-03-27 20:14:22.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0      777 2024-04-16 12:19:25.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:56:31.741126 wagtail_editorjs-1.6.1rc1/wagtail_editorjs.egg-info/
+-rw-rw-rw-   0        0        0     4987 2024-04-26 23:56:31.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5891 2024-04-26 23:56:31.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 23:56:31.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-04-26 23:56:31.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-26 23:56:31.000000 wagtail_editorjs-1.6.1rc1/wagtail_editorjs.egg-info/top_level.txt
```

### Comparing `wagtail_editorjs-1.6.0/LICENSE` & `wagtail_editorjs-1.6.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/PKG-INFO` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wagtail_editorjs
-Version: 1.6.0
+Name: wagtail-editorjs
+Version: 1.6.1rc1
 Summary: EditorJS as a widget for Wagtail, with Page- and Image chooser support
 Home-page: https://github.com/Nigel2392/wagtail_editorjs
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -21,18 +21,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django>=4.2
-Requires-Dist: Wagtail>=5.0
-Requires-Dist: beautifulsoup4>=4.9.3
-Requires-Dist: bleach>=6.0.0
 
 wagtail_editorjs
 ================
 
 *Check out [Awesome Wagtail](https://github.com/springload/awesome-wagtail) for more awesome packages and resources from the Wagtail community.*
 
 A Wagtail EditorJS widget with page/image chooser support, document support and more!
@@ -54,15 +50,22 @@
    ]
    ```
 2. Add the HTML to your template:
 
    ```django-html
    <link rel="stylesheet" href="{% static 'wagtail_editorjs/css/frontend.css' %}">
    {% load editorjs %}
+
+   {# CSS files for features #}
+   {% editorjs_static "css" %}
+
    {% editorjs self.editor_field %}
+
+    {# JS files for features #}
+    {% editorjs_static "js" %}
    ```
 3. Add the field to your model:
 
    ```python
    ...
    from wagtail_editorjs.fields import EditorJSField
    from wagtail_editorjs.blocks import EditorJSBlock
@@ -72,39 +75,41 @@
        content_panels = [
            FieldPanel("editor_field"),
            FieldPanel("content"),
        ]
        editor_field = EditorJSField(
            # All supported features
            features=[
-                'attaches',
-                'checklist',
-                'code',
-                'delimiter',
-                'header',
-                'inline-code',
-                'marker',
-                'nested-list',
-                'paragraph',
-                'quote',
-                'raw',
-                'table',
-                'underline',
-                'warning',
-                'link-autocomplete',
-                'link',
-                'image',
-                'images',
-                'document',
-                'text-alignment-tune',
-                'text-variant-tune',
-                'background-color-tune',
-                'text-color-tune',
-                'undo-redo',
-                'drag-drop',
+               'attaches',
+               'checklist',
+               'code',
+               'delimiter',
+               'header',
+               'inline-code',
+               'marker',
+               'nested-list',
+               'paragraph',
+               'quote',
+               'raw',
+               'table',
+               'underline',
+               'warning',
+               'link-autocomplete',
+               'button',
+               'tooltip',
+               'link',
+               'image',
+               'images',
+               'document',
+               'text-alignment-tune',
+               'text-variant-tune',
+               'background-color-tune',
+               'text-color-tune',
+               'undo-redo',
+               'drag-drop'
             ],
            blank=True,
            null=True,
        )
 
        # Or as a block
        content = fields.StreamField([
```

### Comparing `wagtail_editorjs-1.6.0/README.md` & `wagtail_editorjs-1.6.1rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,22 @@
    ]
    ```
 2. Add the HTML to your template:
 
    ```django-html
    <link rel="stylesheet" href="{% static 'wagtail_editorjs/css/frontend.css' %}">
    {% load editorjs %}
+
+   {# CSS files for features #}
+   {% editorjs_static "css" %}
+
    {% editorjs self.editor_field %}
+
+    {# JS files for features #}
+    {% editorjs_static "js" %}
    ```
 3. Add the field to your model:
 
    ```python
    ...
    from wagtail_editorjs.fields import EditorJSField
    from wagtail_editorjs.blocks import EditorJSBlock
@@ -40,39 +47,41 @@
        content_panels = [
            FieldPanel("editor_field"),
            FieldPanel("content"),
        ]
        editor_field = EditorJSField(
            # All supported features
            features=[
-                'attaches',
-                'checklist',
-                'code',
-                'delimiter',
-                'header',
-                'inline-code',
-                'marker',
-                'nested-list',
-                'paragraph',
-                'quote',
-                'raw',
-                'table',
-                'underline',
-                'warning',
-                'link-autocomplete',
-                'link',
-                'image',
-                'images',
-                'document',
-                'text-alignment-tune',
-                'text-variant-tune',
-                'background-color-tune',
-                'text-color-tune',
-                'undo-redo',
-                'drag-drop',
+               'attaches',
+               'checklist',
+               'code',
+               'delimiter',
+               'header',
+               'inline-code',
+               'marker',
+               'nested-list',
+               'paragraph',
+               'quote',
+               'raw',
+               'table',
+               'underline',
+               'warning',
+               'link-autocomplete',
+               'button',
+               'tooltip',
+               'link',
+               'image',
+               'images',
+               'document',
+               'text-alignment-tune',
+               'text-variant-tune',
+               'background-color-tune',
+               'text-color-tune',
+               'undo-redo',
+               'drag-drop'
             ],
            blank=True,
            null=True,
        )
 
        # Or as a block
        content = fields.StreamField([
```

### Comparing `wagtail_editorjs-1.6.0/setup.cfg` & `wagtail_editorjs-1.6.1rc1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f65 6469 746f   = wagtail_edito
 00000020: 726a 730d 0a76 6572 7369 6f6e 203d 2031  rjs..version = 1
-00000030: 2e36 2e30 0d0a 6465 7363 7269 7074 696f  .6.0..descriptio
-00000040: 6e20 3d20 4564 6974 6f72 4a53 2061 7320  n = EditorJS as 
-00000050: 6120 7769 6467 6574 2066 6f72 2057 6167  a widget for Wag
-00000060: 7461 696c 2c20 7769 7468 2050 6167 652d  tail, with Page-
-00000070: 2061 6e64 2049 6d61 6765 2063 686f 6f73   and Image choos
-00000080: 6572 2073 7570 706f 7274 0d0a 6c6f 6e67  er support..long
-00000090: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
-000000a0: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
-000000b0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000c0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
-000000d0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a61  text/markdown..a
-000000e0: 7574 686f 7220 3d20 4e69 6765 6c0d 0a61  uthor = Nigel..a
-000000f0: 7574 686f 725f 656d 6169 6c20 3d20 6e69  uthor_email = ni
-00000100: 6765 6c40 676f 6f64 6164 7669 6365 2e69  gel@goodadvice.i
-00000110: 740d 0a75 726c 203d 2068 7474 7073 3a2f  t..url = https:/
-00000120: 2f67 6974 6875 622e 636f 6d2f 4e69 6765  /github.com/Nige
-00000130: 6c32 3339 322f 7761 6774 6169 6c5f 6564  l2392/wagtail_ed
-00000140: 6974 6f72 6a73 0d0a 6c69 6365 6e73 6520  itorjs..license 
-00000150: 3d20 4750 4c2d 332e 302d 6f6e 6c79 0d0a  = GPL-3.0-only..
-00000160: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-00000170: 0945 6e76 6972 6f6e 6d65 6e74 203a 3a20  .Environment :: 
-00000180: 5765 6220 456e 7669 726f 6e6d 656e 740d  Web Environment.
-00000190: 0a09 4672 616d 6577 6f72 6b20 3a3a 2044  ..Framework :: D
-000001a0: 6a61 6e67 6f0d 0a09 4672 616d 6577 6f72  jango...Framewor
-000001b0: 6b20 3a3a 2044 6a61 6e67 6f20 3a3a 2034  k :: Django :: 4
-000001c0: 2e32 0d0a 0946 7261 6d65 776f 726b 203a  .2...Framework :
-000001d0: 3a20 5761 6774 6169 6c0d 0a09 4672 616d  : Wagtail...Fram
-000001e0: 6577 6f72 6b20 3a3a 2057 6167 7461 696c  ework :: Wagtail
-000001f0: 203a 3a20 350d 0a09 4672 616d 6577 6f72   :: 5...Framewor
-00000200: 6b20 3a3a 2057 6167 7461 696c 203a 3a20  k :: Wagtail :: 
-00000210: 360d 0a09 496e 7465 6e64 6564 2041 7564  6...Intended Aud
-00000220: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
-00000230: 6572 730d 0a09 4c69 6365 6e73 6520 3a3a  ers...License ::
-00000240: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-00000250: 2047 4e55 2047 656e 6572 616c 2050 7562   GNU General Pub
-00000260: 6c69 6320 4c69 6365 6e73 6520 7633 206f  lic License v3 o
-00000270: 7220 6c61 7465 7220 2847 504c 7633 2b29  r later (GPLv3+)
-00000280: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
-00000290: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
-000002a0: 6e64 656e 740d 0a09 5072 6f67 7261 6d6d  ndent...Programm
-000002b0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000002c0: 5079 7468 6f6e 0d0a 0950 726f 6772 616d  Python...Program
-000002d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000002e0: 2050 7974 686f 6e20 3a3a 2033 0d0a 0950   Python :: 3...P
-000002f0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000300: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000310: 2033 203a 3a20 4f6e 6c79 0d0a 0950 726f   3 :: Only...Pro
-00000320: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000330: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000340: 2e38 0d0a 0950 726f 6772 616d 6d69 6e67  .8...Programming
-00000350: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000360: 686f 6e20 3a3a 2033 2e39 0d0a 0954 6f70  hon :: 3.9...Top
-00000370: 6963 203a 3a20 496e 7465 726e 6574 203a  ic :: Internet :
-00000380: 3a20 5757 572f 4854 5450 0d0a 0954 6f70  : WWW/HTTP...Top
-00000390: 6963 203a 3a20 496e 7465 726e 6574 203a  ic :: Internet :
-000003a0: 3a20 5757 572f 4854 5450 203a 3a20 4479  : WWW/HTTP :: Dy
-000003b0: 6e61 6d69 6320 436f 6e74 656e 740d 0a0d  namic Content...
-000003c0: 0a5b 6f70 7469 6f6e 735d 0d0a 696e 636c  .[options]..incl
-000003d0: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
-000003e0: 203d 2074 7275 650d 0a70 6163 6b61 6765   = true..package
-000003f0: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
-00000400: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000410: 2e38 0d0a 696e 7374 616c 6c5f 7265 7175  .8..install_requ
-00000420: 6972 6573 203d 200d 0a09 446a 616e 676f  ires = ...Django
-00000430: 203e 3d20 342e 320d 0a09 5761 6774 6169   >= 4.2...Wagtai
-00000440: 6c20 3e3d 2035 2e30 0d0a 0962 6561 7574  l >= 5.0...beaut
-00000450: 6966 756c 736f 7570 3420 3e3d 2034 2e39  ifulsoup4 >= 4.9
-00000460: 2e33 0d0a 0962 6c65 6163 6820 3e3d 2036  .3...bleach >= 6
-00000470: 2e30 2e30 0d0a 0d0a 5b65 6767 5f69 6e66  .0.0....[egg_inf
-00000480: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000490: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-000004a0: 0d0a                                     ..
+00000030: 2e36 2e31 7263 310d 0a64 6573 6372 6970  .6.1rc1..descrip
+00000040: 7469 6f6e 203d 2045 6469 746f 724a 5320  tion = EditorJS 
+00000050: 6173 2061 2077 6964 6765 7420 666f 7220  as a widget for 
+00000060: 5761 6774 6169 6c2c 2077 6974 6820 5061  Wagtail, with Pa
+00000070: 6765 2d20 616e 6420 496d 6167 6520 6368  ge- and Image ch
+00000080: 6f6f 7365 7220 7375 7070 6f72 740d 0a6c  ooser support..l
+00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
+000000a0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
+000000b0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
+000000c0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
+000000d0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
+000000e0: 0d0a 6175 7468 6f72 203d 204e 6967 656c  ..author = Nigel
+000000f0: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
+00000100: 206e 6967 656c 4067 6f6f 6461 6476 6963   nigel@goodadvic
+00000110: 652e 6974 0d0a 7572 6c20 3d20 6874 7470  e.it..url = http
+00000120: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4e  s://github.com/N
+00000130: 6967 656c 3233 3932 2f77 6167 7461 696c  igel2392/wagtail
+00000140: 5f65 6469 746f 726a 730d 0a6c 6963 656e  _editorjs..licen
+00000150: 7365 203d 2047 504c 2d33 2e30 2d6f 6e6c  se = GPL-3.0-onl
+00000160: 790d 0a63 6c61 7373 6966 6965 7273 203d  y..classifiers =
+00000170: 200d 0a09 456e 7669 726f 6e6d 656e 7420   ...Environment 
+00000180: 3a3a 2057 6562 2045 6e76 6972 6f6e 6d65  :: Web Environme
+00000190: 6e74 0d0a 0946 7261 6d65 776f 726b 203a  nt...Framework :
+000001a0: 3a20 446a 616e 676f 0d0a 0946 7261 6d65  : Django...Frame
+000001b0: 776f 726b 203a 3a20 446a 616e 676f 203a  work :: Django :
+000001c0: 3a20 342e 320d 0a09 4672 616d 6577 6f72  : 4.2...Framewor
+000001d0: 6b20 3a3a 2057 6167 7461 696c 0d0a 0946  k :: Wagtail...F
+000001e0: 7261 6d65 776f 726b 203a 3a20 5761 6774  ramework :: Wagt
+000001f0: 6169 6c20 3a3a 2035 0d0a 0946 7261 6d65  ail :: 5...Frame
+00000200: 776f 726b 203a 3a20 5761 6774 6169 6c20  work :: Wagtail 
+00000210: 3a3a 2036 0d0a 0949 6e74 656e 6465 6420  :: 6...Intended 
+00000220: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
+00000230: 6c6f 7065 7273 0d0a 094c 6963 656e 7365  lopers...License
+00000240: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+00000250: 203a 3a20 474e 5520 4765 6e65 7261 6c20   :: GNU General 
+00000260: 5075 626c 6963 204c 6963 656e 7365 2076  Public License v
+00000270: 3320 6f72 206c 6174 6572 2028 4750 4c76  3 or later (GPLv
+00000280: 332b 290d 0a09 4f70 6572 6174 696e 6720  3+)...Operating 
+00000290: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+000002a0: 6570 656e 6465 6e74 0d0a 0950 726f 6772  ependent...Progr
+000002b0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000002c0: 3a3a 2050 7974 686f 6e0d 0a09 5072 6f67  :: Python...Prog
+000002d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000002e0: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
+000002f0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000300: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000310: 203a 3a20 3320 3a3a 204f 6e6c 790d 0a09   :: 3 :: Only...
+00000320: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000330: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000340: 3a20 332e 380d 0a09 5072 6f67 7261 6d6d  : 3.8...Programm
+00000350: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000360: 5079 7468 6f6e 203a 3a20 332e 390d 0a09  Python :: 3.9...
+00000370: 546f 7069 6320 3a3a 2049 6e74 6572 6e65  Topic :: Interne
+00000380: 7420 3a3a 2057 5757 2f48 5454 500d 0a09  t :: WWW/HTTP...
+00000390: 546f 7069 6320 3a3a 2049 6e74 6572 6e65  Topic :: Interne
+000003a0: 7420 3a3a 2057 5757 2f48 5454 5020 3a3a  t :: WWW/HTTP ::
+000003b0: 2044 796e 616d 6963 2043 6f6e 7465 6e74   Dynamic Content
+000003c0: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a69  ....[options]..i
+000003d0: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
+000003e0: 6174 6120 3d20 7472 7565 0d0a 7061 636b  ata = true..pack
+000003f0: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
+00000400: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+00000410: 3e3d 332e 380d 0a69 6e73 7461 6c6c 5f72  >=3.8..install_r
+00000420: 6571 7569 7265 7320 3d20 0d0a 0944 6a61  equires = ...Dja
+00000430: 6e67 6f20 3e3d 2034 2e32 0d0a 0957 6167  ngo >= 4.2...Wag
+00000440: 7461 696c 203e 3d20 352e 300d 0a09 6265  tail >= 5.0...be
+00000450: 6175 7469 6675 6c73 6f75 7034 203e 3d20  autifulsoup4 >= 
+00000460: 342e 392e 330d 0a09 626c 6561 6368 203e  4.9.3...bleach >
+00000470: 3d20 362e 302e 300d 0a0d 0a5b 6567 675f  = 6.0.0....[egg_
+00000480: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000490: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+000004a0: 300d 0a0d 0a                             0....
```

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/blocks.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/django_editor.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/django_editor.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/features/__init__.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/features/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     AttachesFeature,
 )
 from .images import (
     ImageFeature,
     ImageRowFeature,
 )
 from .inlines import (
+    TooltipFeature,
     LinkFeature,
     LinkAutoCompleteFeature,
     DocumentFeature,
 )
 from .tunes import (
     AlignmentBlockTune,
     TextVariantTune,
```

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/features/blocks.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/features/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/features/documents.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/features/documents.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/features/images.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/features/images.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/features/inlines.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/features/inlines.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,26 +5,73 @@
 from wagtail.admin.widgets import AdminPageChooser
 from wagtail.documents.widgets import AdminDocumentChooser
 from wagtail.documents import get_document_model
 from wagtail import hooks
 
 from ..registry import (
     PageChooserURLsMixin,
+    InlineEditorJSFeature,
     ModelInlineEditorJSFeature,
     FeatureViewMixin,
 )
 from django.http import (
     HttpResponse,
     JsonResponse,
 )
 
 
 Document = get_document_model()
 
 
+class TooltipFeature(InlineEditorJSFeature):
+    allowed_tags = ["span"]
+    allowed_attributes = [
+        "class",
+        "data-tippy-content",
+        "data-tippy-placement",
+        "data-tippy-follow-cursor",
+    ]
+    tag_name = "span"
+    must_have_attrs = {
+        "class": "wagtail-tooltip",
+        "data-w-tooltip-content-value": None,
+    }
+    can_have_attrs = {
+        "data-w-tooltip-placement-value": None,
+    }
+    
+    klass = "WagtailTooltip"
+    js = [
+        "wagtail_editorjs/js/tools/tooltips/wagtail-tooltips.js",
+    ]
+    frontend_js = [
+        "wagtail_editorjs/vendor/tippy/popper.min.js",
+        "wagtail_editorjs/vendor/tippy/tippy-bundle.min.js",
+        "wagtail_editorjs/js/tools/tooltips/frontend.js",
+    ]
+
+    @classmethod
+    def get_test_data(cls):
+        return []
+
+    def build_elements(self, inline_data: list, context: dict[str, Any] = None) -> list:
+        for element, attrs in inline_data:
+
+            element["data-tippy-follow-cursor"] = "horizontal"
+
+            for k, v in attrs.items():
+                if not k.startswith("data-w-tooltip-") or not k.endswith("-value"):
+                    continue
+
+                k = k.replace("data-w-tooltip-", "data-tippy-")
+                k = k[:-6]
+
+                element[k] = v
+
+
 class BasePageLinkMixin(PageChooserURLsMixin):
     allowed_attributes = ["target", "rel"]
     can_have_attrs = {
         "data-target": None,
         "data-rel": None,
     }
```

#### html2text {}

```diff
@@ -1,37 +1,51 @@
 from typing import Any from django.urls import reverse from
 django.utils.translation import gettext_lazy as _ from wagtail.models import
 Page from wagtail.admin.widgets import AdminPageChooser from
 wagtail.documents.widgets import AdminDocumentChooser from wagtail.documents
 import get_document_model from wagtail import hooks from ..registry import
-( PageChooserURLsMixin, ModelInlineEditorJSFeature, FeatureViewMixin, ) from
-django.http import ( HttpResponse, JsonResponse, ) Document =
-get_document_model() class BasePageLinkMixin(PageChooserURLsMixin):
-allowed_attributes = ["target", "rel"] can_have_attrs = { "data-target": None,
-"data-rel": None, } def build_element(self, item, obj, context: dict[str, Any]
-= None, data: dict[str, Any] = None): """Build the element from the object."""
-super().build_element(item, obj, context, data) if "data-target" in data and
-data["data-target"]: item["target"] = data["data-target"] if "data-rel" in data
-and data["data-rel"]: item["rel"] = data["data-rel"] @classmethod def get_url
-(cls, instance): return instance.get_url() @classmethod def get_full_url(cls,
-instance, request): return instance.get_full_url(request) @classmethod def
-get_test_queryset(cls): return super().get_test_queryset().filter(depth__gt=1)
-class LinkFeature(BasePageLinkMixin, ModelInlineEditorJSFeature): allowed_tags
-= ["a"] allowed_attributes = BasePageLinkMixin.allowed_attributes + [ "class",
-"href", "data-id" ] must_have_attrs = { "data-parent-id": None, } chooser_class
-= AdminPageChooser model = Page klass="WagtailLinkTool" js =
-[ "wagtail_editorjs/js/tools/wagtail-chooser-tool.js", "wagtail_editorjs/js/
-tools/wagtail-link.js", ] @classmethod def get_test_data(cls): models =
-cls.get_test_queryset()[0:5] return [ ( # Override to add data-autocomplete.
-f"", f"", ) for model in models ] SEARCH_QUERY_PARAM = "search"
-CONSTRUCT_PAGE_QUERYSET = "construct_page_queryset" BUILD_PAGE_DATA =
-"build_page_data" class LinkAutoCompleteFeature(FeatureViewMixin,
-BasePageLinkMixin, ModelInlineEditorJSFeature): allowed_tags = ["a"]
+( PageChooserURLsMixin, InlineEditorJSFeature, ModelInlineEditorJSFeature,
+FeatureViewMixin, ) from django.http import ( HttpResponse, JsonResponse, )
+Document = get_document_model() class TooltipFeature(InlineEditorJSFeature):
+allowed_tags = ["span"] allowed_attributes = [ "class", "data-tippy-content",
+"data-tippy-placement", "data-tippy-follow-cursor", ] tag_name = "span"
+must_have_attrs = { "class": "wagtail-tooltip", "data-w-tooltip-content-value":
+None, } can_have_attrs = { "data-w-tooltip-placement-value": None, } klass =
+"WagtailTooltip" js = [ "wagtail_editorjs/js/tools/tooltips/wagtail-
+tooltips.js", ] frontend_js = [ "wagtail_editorjs/vendor/tippy/popper.min.js",
+"wagtail_editorjs/vendor/tippy/tippy-bundle.min.js", "wagtail_editorjs/js/
+tools/tooltips/frontend.js", ] @classmethod def get_test_data(cls): return []
+def build_elements(self, inline_data: list, context: dict[str, Any] = None) -
+> list: for element, attrs in inline_data: element["data-tippy-follow-cursor"]
+= "horizontal" for k, v in attrs.items(): if not k.startswith("data-w-tooltip-
+") or not k.endswith("-value"): continue k = k.replace("data-w-tooltip-",
+"data-tippy-") k = k[:-6] element[k] = v class BasePageLinkMixin
+(PageChooserURLsMixin): allowed_attributes = ["target", "rel"] can_have_attrs =
+{ "data-target": None, "data-rel": None, } def build_element(self, item, obj,
+context: dict[str, Any] = None, data: dict[str, Any] = None): """Build the
+element from the object.""" super().build_element(item, obj, context, data) if
+"data-target" in data and data["data-target"]: item["target"] = data["data-
+target"] if "data-rel" in data and data["data-rel"]: item["rel"] = data["data-
+rel"] @classmethod def get_url(cls, instance): return instance.get_url()
+@classmethod def get_full_url(cls, instance, request): return
+instance.get_full_url(request) @classmethod def get_test_queryset(cls): return
+super().get_test_queryset().filter(depth__gt=1) class LinkFeature
+(BasePageLinkMixin, ModelInlineEditorJSFeature): allowed_tags = ["a"]
 allowed_attributes = BasePageLinkMixin.allowed_attributes + [ "class", "href",
-"data-id" ] must_have_attrs = { "data-autocomplete": "page", } chooser_class =
+"data-id" ] must_have_attrs = { "data-parent-id": None, } chooser_class =
+AdminPageChooser model = Page klass="WagtailLinkTool" js = [ "wagtail_editorjs/
+js/tools/wagtail-chooser-tool.js", "wagtail_editorjs/js/tools/wagtail-link.js",
+] @classmethod def get_test_data(cls): models = cls.get_test_queryset()[0:5]
+return [ ( # Override to add data-autocomplete. f"", f"", ) for model in models
+] SEARCH_QUERY_PARAM = "search" CONSTRUCT_PAGE_QUERYSET =
+"construct_page_queryset" BUILD_PAGE_DATA = "build_page_data" class
+LinkAutoCompleteFeature(FeatureViewMixin, BasePageLinkMixin,
+ModelInlineEditorJSFeature): allowed_tags = ["a"] allowed_attributes =
+BasePageLinkMixin.allowed_attributes + [ "class", "href", "data-id" ]
+must_have_attrs = { "data-autocomplete": "page", } chooser_class =
 AdminPageChooser model = Page klass="LinkAutocomplete" js =
 [ "wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js", ] def
 get_config(self, context: dict[str, Any]): config = super
 (ModelInlineEditorJSFeature, self).get_config(context) config.setdefault
 ("config", {}) config["config"]["endpoint"] = reverse(f"wagtail_editorjs:
 {self.tool_name}") config["config"]["queryParam"] = "search" return config
 @classmethod def get_test_data(cls): models = cls.get_test_queryset()[0:5]
```

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/features/lists.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/features/lists.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/features/tunes.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/features/tunes.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/fields.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/forms.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/forms.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,31 @@
 )
 from .registry import (
     EDITOR_JS_FEATURES,
     get_features,
     TemplateNotSpecifiedError,
 )
 
+def _get_feature_scripts(feature, method, *args, list_obj = None, **kwargs):
+    get_scripts = getattr(feature, method, None)
+    if get_scripts is None:
+        raise AttributeError(f"Feature {feature} does not have a {method} method")
+    
+    scripts = get_scripts(*args, **kwargs)
+
+    if list_obj is None:
+        list_obj = []
 
+    for file in get_scripts():
+        if file not in list_obj:
+            if isinstance(file, (list, tuple)):
+                list_obj.extend(file)
+            else:
+                list_obj.append(file)
+    return scripts
 
 class EditorJSWidget(widgets.Input):
     """
         A widget which renders the EditorJS editor.
 
         All features are allowed to register CSS and JS files.
 
@@ -79,38 +95,28 @@
     
     @cached_property
     def media(self):
         js = [
             "wagtail_editorjs/vendor/editorjs/editorjs.umd.js",
             "wagtail_editorjs/js/editorjs-widget.js",
             "wagtail_editorjs/js/tools/wagtail-block-tool.js",
+            "wagtail_editorjs/js/tools/wagtail-inline-tool.js",
         ]
         css = [
             "wagtail_editorjs/css/editorjs-widget.css",
             # "wagtail_editorjs/css/frontend.css",
         ]
 
         feature_mapping = EDITOR_JS_FEATURES.get_by_weight(
             self.features,
         )
 
         for feature in feature_mapping.values():
-            for js_file in feature.get_js():
-                if js_file not in js:
-                    if isinstance(js_file, (list, tuple)):
-                        js.extend(js_file)
-                    else:
-                        js.append(js_file)
-
-            for css_file in feature.get_css():
-                if css_file not in css:
-                    if isinstance(css_file, (list, tuple)):
-                        css.extend(css_file)
-                    else:
-                        css.append(css_file)
+            _get_feature_scripts(feature, "get_js", list_obj=js)
+            _get_feature_scripts(feature, "get_css", list_obj=css)
 
         js.extend([
             "wagtail_editorjs/js/editorjs-widget-controller.js",
         ])
 
         return widgets.Media(
             js=js,
```

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/__init__.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/element/attrs.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/element/attrs.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/element/element.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/element/element.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/element/utils.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/element/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/feature_registry.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/feature_registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/base.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/features/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 
 class BaseEditorJSFeature:
     allowed_tags: list[str] = None
     allowed_attributes: dict[str, list[str]] = None
     klass: str = None
     js: list[str] = None
     css: list[str] = None
+    frontend_css: list[str] = []
+    frontend_js: list[str] = []
     # cleaner_funcs: dict[str, dict[str, Callable[[str], bool]]] = {}
     
     def __init__(self,
             tool_name: str,
             klass: str = None,
             js: Union[str, list[str]] = None,
             css: Union[str, list[str]] = None,
@@ -170,26 +172,44 @@
 
         return config
 
     def get_js(self):
         """
             Return any javascript files required for this feature to work.
         """
+        if not self.js:
+            return []
+            
         if isinstance(self.js, str):
             return [self.js]
         return self.js
     
     def get_css(self):
         """
             Return any css files required for this feature to work.
         """
+        if not self.css:
+            return []
+            
         if isinstance(self.css, str):
             return [self.css]
         return self.css
     
+    def get_frontend_css(self):
+        """
+            Returns the css files required for the frontend.
+        """
+        return self.frontend_css
+    
+    def get_frontend_js(self):
+        """
+            Returns the js files required for the frontend.
+        """
+        return self.frontend_js
+
     def validate(self, data: Any):
         """
             Validate any data coming from editorJS
             for completeness and correctness.
         """
         pass
```

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/basic.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/features/basic.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/inlines.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/features/inlines.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 
 import bs4
 
 
 class InlineEditorJSFeature(BaseEditorJSFeature):
     must_have_attrs = None
     can_have_attrs = None
+    tag_name = None
 
     def __init__(
         self,
         tool_name: str,
-        tag_name: str,
+        tag_name: str = None,
         klass: str = None,
         must_have_attrs: dict = None,
         can_have_attrs: dict = None,
         js: Union[str, list[str]] = None,
         css: Union[str, list[str]] = None,
         include_template: str = None,
         config: dict = None,
@@ -45,15 +46,15 @@
 
         if self.must_have_attrs:
             must_have_attrs.update(self.must_have_attrs)
 
         if self.can_have_attrs:
             can_have_attrs.update(self.can_have_attrs)
 
-        self.tag_name = tag_name
+        self.tag_name = tag_name or self.tag_name
         self.must_have_attrs = must_have_attrs
         self.can_have_attrs = can_have_attrs
 
     def build_elements(self, inline_data: list, context: dict[str, Any] = None) -> list:
         """
         Builds the elements for the inline data.
 
@@ -216,18 +217,16 @@
         for data in inline_data:
             # soup: BeautifulSoup
             # element: EditorJSElement
             # matches: dict[bs4.elementType, dict[str, Any]]
             # data: dict[str, Any] # Block data.
             item, data = data
 
-            # # Store element and soup for later replacement of content.
-            # element_soups.append((soup, element))
 
-            # Item is bs4 tag, attrs are must_have_attrs
+            # Item is bs4 tag, attrs are must_have_attrs and can_have_attrs
 
             id = self.get_id(item, data, context)
             ids.append((item, id, data))
 
             # delete all attributes
             for key in list(item.attrs.keys()):
                 del item[key]
```

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/snippets_inlines.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/features/snippets_inlines.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/view.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/features/view.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/value.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/registry/value.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/render.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/render.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/settings.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css`

 * *Files 4% similar despite different names*

```diff
@@ -328,8 +328,13 @@
     height: 16px;
 }
 
 .wagtail-button-wrapper .wagtail-button-icon {
     background-color: unset;
     color: var(--w-color-text-link-default);
     padding: 0;
+}
+
+span.wagtail-tooltip {
+    color: var(--w-color-text-link-default);
+    text-decoration: dotted underline;
 }
```

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 .wagtail-editorjs-richtext.wagtail-editorjs-richtext > * {
     /* margin: 0.75rem 0; */
     margin-top: 0;
     margin-bottom: 0;
     padding-top: calc(var(--editor-richtext-padding-vertical) / 2);
     padding-bottom: calc(var(--editor-richtext-padding-vertical) / 2);
 }
-.wagtail-editorjs-richtext.wagtail-editorjs-richtext > :not(.stretched, .bg-stretched) {
+.wagtail-editorjs-richtext.wagtail-editorjs-richtext > :not(.stretched):is(.bg-stretched) {
     padding-left: calc(var(--editor-margin-x) / 5);
     padding-right: calc(var(--editor-margin-x) / 5);
 }
 
 .wagtail-editorjs-color-tuned {
     color: var(--text-color, inherit) !important;
     background-color: var(--background-color, inherit) !important;
@@ -432,8 +432,15 @@
     border: 1px solid rgba(var(--editor-button-bg), min(calc(var(--editor-button-bg-opacity) / 10), 1));
     background-color: rgba(var(--editor-button-bg), calc(var(--editor-button-bg-opacity) / 100));
     color: var(--editor-button-text);
 }
 .wagtail-editorjs-richtext .editor-button:hover {
     background-color: rgba(var(--editor-button-bg-hover), calc(var(--editor-button-bg-hover-opacity) / 100));
     color: var(--editor-button-text-hover);
+}
+
+.wagtail-tooltip {
+    cursor: help;
+    color: rgba(var(--editor-accent-color-rgb), 1);
+    text-decoration: dotted underline;
+    text-underline-offset: 0.15em;
 }
```

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -113,19 +113,14 @@
         const text = range.extractContents();
         wrapperTag.remove();
         range.insertNode(text);
     }
 
     checkState() {
         const wrapperTag = this.api.selection.findParentTag(this.tag, this.tagClass);
-        this.wrapperTag = wrapperTag;
-        if (!wrapperTag) {
-            return
-        }
-
 
         this.state = !!wrapperTag;
 
         if (this.state) {
             this.showActions(wrapperTag);
         } else {
             this.hideActions();
```

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/base.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/test_attrs.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/core/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/test_inlines.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/core/tests/test_inlines.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/test_render.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/core/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/test/manage.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/test/testapp/settings.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/test/testapp/urls.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/wagtail_hooks/features.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/wagtail_hooks/features.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     DelimiterFeature,
     WarningFeature,
     HeaderFeature,
     HTMLFeature,
     ImageFeature,
     ImageRowFeature,
     ButtonFeature,
+    TooltipFeature,
     LinkFeature,
     LinkAutoCompleteFeature,
     DocumentFeature,
     NestedListFeature,
     TableFeature,
     AlignmentBlockTune,
     TextVariantTune,
@@ -171,14 +172,20 @@
     registry.register(
         "button",
         ButtonFeature(
             "button",
         )
     )
     registry.register(
+        "tooltip",
+        TooltipFeature(
+            "tooltip",
+        ),
+    )
+    registry.register(
         "link",
         LinkFeature(
             "link",
             inlineToolbar = True,
         ),
     )
     registry.register(
```

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/wagtail_hooks/urls.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/wagtail_hooks/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs.egg-info/PKG-INFO` & `wagtail_editorjs-1.6.1rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_editorjs
-Version: 1.6.0
+Version: 1.6.1rc1
 Summary: EditorJS as a widget for Wagtail, with Page- and Image chooser support
 Home-page: https://github.com/Nigel2392/wagtail_editorjs
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -21,18 +21,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django>=4.2
-Requires-Dist: Wagtail>=5.0
-Requires-Dist: beautifulsoup4>=4.9.3
-Requires-Dist: bleach>=6.0.0
 
 wagtail_editorjs
 ================
 
 *Check out [Awesome Wagtail](https://github.com/springload/awesome-wagtail) for more awesome packages and resources from the Wagtail community.*
 
 A Wagtail EditorJS widget with page/image chooser support, document support and more!
@@ -54,15 +50,22 @@
    ]
    ```
 2. Add the HTML to your template:
 
    ```django-html
    <link rel="stylesheet" href="{% static 'wagtail_editorjs/css/frontend.css' %}">
    {% load editorjs %}
+
+   {# CSS files for features #}
+   {% editorjs_static "css" %}
+
    {% editorjs self.editor_field %}
+
+    {# JS files for features #}
+    {% editorjs_static "js" %}
    ```
 3. Add the field to your model:
 
    ```python
    ...
    from wagtail_editorjs.fields import EditorJSField
    from wagtail_editorjs.blocks import EditorJSBlock
@@ -72,39 +75,41 @@
        content_panels = [
            FieldPanel("editor_field"),
            FieldPanel("content"),
        ]
        editor_field = EditorJSField(
            # All supported features
            features=[
-                'attaches',
-                'checklist',
-                'code',
-                'delimiter',
-                'header',
-                'inline-code',
-                'marker',
-                'nested-list',
-                'paragraph',
-                'quote',
-                'raw',
-                'table',
-                'underline',
-                'warning',
-                'link-autocomplete',
-                'link',
-                'image',
-                'images',
-                'document',
-                'text-alignment-tune',
-                'text-variant-tune',
-                'background-color-tune',
-                'text-color-tune',
-                'undo-redo',
-                'drag-drop',
+               'attaches',
+               'checklist',
+               'code',
+               'delimiter',
+               'header',
+               'inline-code',
+               'marker',
+               'nested-list',
+               'paragraph',
+               'quote',
+               'raw',
+               'table',
+               'underline',
+               'warning',
+               'link-autocomplete',
+               'button',
+               'tooltip',
+               'link',
+               'image',
+               'images',
+               'document',
+               'text-alignment-tune',
+               'text-variant-tune',
+               'background-color-tune',
+               'text-color-tune',
+               'undo-redo',
+               'drag-drop'
             ],
            blank=True,
            null=True,
        )
 
        # Or as a block
        content = fields.StreamField([
```

### Comparing `wagtail_editorjs-1.6.0/wagtail_editorjs.egg-info/SOURCES.txt` & `wagtail_editorjs-1.6.1rc1/wagtail_editorjs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,18 @@
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js
+wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-inline-tool.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js
+wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/frontend.js
+wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/wagtail-tooltips.js
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js
@@ -76,14 +79,17 @@
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js
 wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js
+wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/LICENSE
+wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/popper.min.js
+wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/tippy-bundle.min.js
 wagtail_editorjs/templates/wagtail_editorjs/rich_text.html
 wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html
 wagtail_editorjs/templatetags/__init__.py
 wagtail_editorjs/templatetags/editorjs.py
 wagtail_editorjs/templatetags/__pycache__/__init__.cpython-311.pyc
 wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc
 wagtail_editorjs/test/__init__.py
```

