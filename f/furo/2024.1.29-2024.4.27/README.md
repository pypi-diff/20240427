# Comparing `tmp/furo-2024.1.29.tar.gz` & `tmp/furo-2024.4.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furo-2024.1.29.tar", last modified: Mon Jan 29 22:52:04 2024, max compression
+gzip compressed data, was "furo-2024.4.27.tar", last modified: Sat Apr 27 10:31:33 2024, max compression
```

## Comparing `furo-2024.1.29.tar` & `furo-2024.4.27.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-01-29 22:52:04.046539 furo-2024.1.29/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     5212 2022-12-07 02:12:20.980461 furo-2024.1.29/CODE_OF_CONDUCT.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1078 2022-12-07 02:12:20.980570 furo-2024.1.29/LICENSE
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3578 2023-04-26 22:26:30.335543 furo-2024.1.29/README.md
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-12-10 17:15:53.819908 furo-2024.1.29/docs/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:20.992187 furo-2024.1.29/docs/_static/
--rw-r--r--   0 pradyunsg   (501) staff       (20)   476986 2022-12-07 02:12:20.984051 furo-2024.1.29/docs/_static/demo-dark.png
--rw-r--r--   0 pradyunsg   (501) staff       (20)   452305 2022-12-07 02:12:20.986929 furo-2024.1.29/docs/_static/demo-light.png
--rw-r--r--   0 pradyunsg   (501) staff       (20)   775827 2022-12-07 02:12:20.991994 furo-2024.1.29/docs/_static/demo.png
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2110 2022-12-07 02:12:20.992140 furo-2024.1.29/docs/_static/pied-piper-admonition.css
--rw-r--r--   0 pradyunsg   (501) staff       (20)      182 2022-12-07 02:12:20.992240 furo-2024.1.29/docs/_static/readthedocs-dummy.js
--rw-r--r--   0 pradyunsg   (501) staff       (20)    19783 2024-01-29 22:50:26.856018 furo-2024.1.29/docs/changelog.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     4931 2023-08-18 23:24:40.358672 furo-2024.1.29/docs/conf.py
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:20.994013 furo-2024.1.29/docs/contributing/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      961 2022-12-07 02:12:20.993810 furo-2024.1.29/docs/contributing/design.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      869 2022-12-07 02:12:20.993895 furo-2024.1.29/docs/contributing/index.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     4790 2022-12-07 02:12:20.993972 furo-2024.1.29/docs/contributing/internals.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3178 2022-12-07 02:12:20.994069 furo-2024.1.29/docs/contributing/workflow.md
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-12-10 17:13:56.071941 furo-2024.1.29/docs/customisation/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      716 2022-12-07 02:12:20.994295 furo-2024.1.29/docs/customisation/announcement.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2199 2022-12-07 02:12:20.994465 furo-2024.1.29/docs/customisation/colors.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1646 2022-12-07 02:12:20.994613 furo-2024.1.29/docs/customisation/edit-button.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      832 2022-12-07 02:12:20.994707 furo-2024.1.29/docs/customisation/fonts.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     5208 2023-12-10 17:13:56.071813 furo-2024.1.29/docs/customisation/footer.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3577 2023-05-20 06:29:53.184453 furo-2024.1.29/docs/customisation/index.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1630 2022-12-07 02:12:20.995041 furo-2024.1.29/docs/customisation/injecting.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      965 2023-12-10 17:13:56.072135 furo-2024.1.29/docs/customisation/landing-page.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1799 2023-05-20 06:29:53.184857 furo-2024.1.29/docs/customisation/logo.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      495 2022-12-07 02:12:20.995279 furo-2024.1.29/docs/customisation/sidebar-title.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3989 2022-12-07 02:12:20.995372 furo-2024.1.29/docs/customisation/sidebar.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      563 2022-12-07 02:12:20.995440 furo-2024.1.29/docs/customisation/toc.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      404 2022-12-07 02:12:20.995513 furo-2024.1.29/docs/index.md
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-12-10 17:13:56.072300 furo-2024.1.29/docs/kitchen-sink/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1317 2023-07-15 10:12:04.480639 furo-2024.1.29/docs/kitchen-sink/admonitions.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1153 2022-12-07 02:12:20.995774 furo-2024.1.29/docs/kitchen-sink/api.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     8423 2023-12-10 17:13:56.072569 furo-2024.1.29/docs/kitchen-sink/blocks.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     8978 2023-04-13 21:50:39.135508 furo-2024.1.29/docs/kitchen-sink/generic.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3070 2022-12-07 02:12:20.996156 furo-2024.1.29/docs/kitchen-sink/images.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)      778 2022-12-07 02:12:20.996263 furo-2024.1.29/docs/kitchen-sink/index.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     6177 2022-12-07 02:12:20.996359 furo-2024.1.29/docs/kitchen-sink/lists.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)    12941 2023-07-02 07:54:47.884930 furo-2024.1.29/docs/kitchen-sink/really-long.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2584 2022-12-07 02:12:20.996549 furo-2024.1.29/docs/kitchen-sink/sphinx-design.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     6376 2022-12-07 02:12:20.996637 furo-2024.1.29/docs/kitchen-sink/structure.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     5200 2023-07-15 08:51:23.625580 furo-2024.1.29/docs/kitchen-sink/tables.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2668 2022-12-07 02:12:20.996837 furo-2024.1.29/docs/kitchen-sink/typography.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)       66 2023-11-06 23:31:33.042578 furo-2024.1.29/docs/license.rst
--rw-r--r--   0 pradyunsg   (501) staff       (20)      121 2022-12-07 02:12:20.996995 furo-2024.1.29/docs/quickstart.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3271 2022-12-07 02:12:20.997091 furo-2024.1.29/docs/recommendations.md
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-04-09 14:47:21.361291 furo-2024.1.29/docs/reference/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     5455 2022-12-07 02:12:20.997257 furo-2024.1.29/docs/reference/admonitions.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      817 2023-04-09 14:47:21.362077 furo-2024.1.29/docs/reference/api.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1549 2022-12-26 12:21:17.347462 furo-2024.1.29/docs/reference/code-blocks.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1069 2022-12-07 02:12:20.997543 furo-2024.1.29/docs/reference/hyperlinks.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2350 2023-07-15 09:18:08.114960 furo-2024.1.29/docs/reference/images.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)      554 2022-12-07 02:12:20.997740 furo-2024.1.29/docs/reference/index.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1606 2022-12-07 02:12:20.997824 furo-2024.1.29/docs/reference/lists.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1372 2022-12-07 02:12:20.997898 furo-2024.1.29/docs/reference/tables.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1020 2022-12-07 02:12:20.997976 furo-2024.1.29/docs/reference/tabs.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1321 2022-12-07 02:12:20.998057 furo-2024.1.29/docs/reference/text-formatting.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)       75 2022-12-07 02:12:20.998128 furo-2024.1.29/docs/requirements.txt
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1967 2023-04-13 16:48:43.861620 furo-2024.1.29/docs/stability.md
--rw-r--r--   0 pradyunsg   (501) staff       (20)     5058 2024-01-29 22:37:21.766593 furo-2024.1.29/noxfile.py
--rw-r--r--   0 pradyunsg   (501) staff       (20)   123493 2024-01-29 22:49:02.105328 furo-2024.1.29/package-lock.json
--rw-r--r--   0 pradyunsg   (501) staff       (20)      421 2023-03-27 12:04:35.297935 furo-2024.1.29/package.json
--rw-r--r--   0 pradyunsg   (501) staff       (20)       60 2022-12-07 02:12:21.002171 furo-2024.1.29/postcss.config.js
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1394 2023-09-09 22:47:19.676842 furo-2024.1.29/pyproject.toml
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2021-11-11 18:55:23.538711 furo-2024.1.29/src/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-12-10 17:15:53.835190 furo-2024.1.29/src/furo/
--rw-r--r--   0 pradyunsg   (501) staff       (20)    12518 2024-01-29 22:51:56.520187 furo-2024.1.29/src/furo/__init__.py
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1389 2023-09-10 15:04:01.605148 furo-2024.1.29/src/furo/_demo_module.py
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.003273 furo-2024.1.29/src/furo/assets/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-12-10 17:13:56.072666 furo-2024.1.29/src/furo/assets/scripts/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     4987 2022-12-07 02:12:21.003092 furo-2024.1.29/src/furo/assets/scripts/furo.js
--rw-r--r--   0 pradyunsg   (501) staff       (20)    12995 2023-12-10 17:13:56.072855 furo-2024.1.29/src/furo/assets/scripts/gumshoe-patched.js
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-10-11 08:48:22.837263 furo-2024.1.29/src/furo/assets/styles/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     9677 2023-10-11 08:48:22.838875 furo-2024.1.29/src/furo/assets/styles/_scaffold.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      309 2022-12-07 02:12:21.003686 furo-2024.1.29/src/furo/assets/styles/_shame.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.004106 furo-2024.1.29/src/furo/assets/styles/base/
--rw-r--r--   0 pradyunsg   (501) staff       (20)       78 2022-12-07 02:12:21.003806 furo-2024.1.29/src/furo/assets/styles/base/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1403 2022-12-07 02:12:21.003891 furo-2024.1.29/src/furo/assets/styles/base/_print.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      300 2022-12-07 02:12:21.003967 furo-2024.1.29/src/furo/assets/styles/base/_screen-readers.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1307 2022-12-07 02:12:21.004063 furo-2024.1.29/src/furo/assets/styles/base/_theme.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1549 2022-12-07 02:12:21.004155 furo-2024.1.29/src/furo/assets/styles/base/_typography.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-02-25 11:33:38.919529 furo-2024.1.29/src/furo/assets/styles/components/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1978 2023-02-25 11:33:38.920044 furo-2024.1.29/src/furo/assets/styles/components/_footer.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)       80 2022-12-07 02:12:21.004909 furo-2024.1.29/src/furo/assets/styles/components/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      328 2022-12-07 02:12:21.004994 furo-2024.1.29/src/furo/assets/styles/components/_search.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     6094 2022-12-07 02:12:21.005360 furo-2024.1.29/src/furo/assets/styles/components/_sidebar.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1832 2023-07-02 07:57:06.099329 furo-2024.1.29/src/furo/assets/styles/components/_table_of_contents.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-04-13 21:50:43.172691 furo-2024.1.29/src/furo/assets/styles/content/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1945 2023-07-15 08:52:07.005777 furo-2024.1.29/src/furo/assets/styles/content/_admonitions.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2281 2023-07-02 07:57:07.496021 furo-2024.1.29/src/furo/assets/styles/content/_api.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      140 2022-12-07 02:12:21.005982 furo-2024.1.29/src/furo/assets/styles/content/_blocks.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      385 2022-12-07 02:12:21.006058 furo-2024.1.29/src/furo/assets/styles/content/_captions.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3231 2023-07-15 10:15:52.575334 furo-2024.1.29/src/furo/assets/styles/content/_code.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      846 2022-12-07 02:12:21.006385 furo-2024.1.29/src/furo/assets/styles/content/_footnotes.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      210 2022-12-07 02:12:21.006461 furo-2024.1.29/src/furo/assets/styles/content/_gui-labels.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      571 2022-12-07 02:12:21.006547 furo-2024.1.29/src/furo/assets/styles/content/_images.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      279 2022-12-07 02:12:21.006627 furo-2024.1.29/src/furo/assets/styles/content/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      312 2022-12-07 02:12:21.006705 furo-2024.1.29/src/furo/assets/styles/content/_indexes.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1090 2022-12-07 02:12:21.006795 furo-2024.1.29/src/furo/assets/styles/content/_lists.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      320 2023-04-13 21:50:43.173530 furo-2024.1.29/src/furo/assets/styles/content/_math.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1139 2022-12-07 02:12:21.006958 furo-2024.1.29/src/furo/assets/styles/content/_misc.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      318 2022-12-07 02:12:21.007281 furo-2024.1.29/src/furo/assets/styles/content/_rubrics.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      562 2022-12-07 02:12:21.007361 furo-2024.1.29/src/furo/assets/styles/content/_sidebar.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      944 2022-12-07 02:12:21.007587 furo-2024.1.29/src/furo/assets/styles/content/_tables.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1927 2022-12-07 02:12:21.007844 furo-2024.1.29/src/furo/assets/styles/content/_target.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.008365 furo-2024.1.29/src/furo/assets/styles/extensions/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      946 2022-12-07 02:12:21.007971 furo-2024.1.29/src/furo/assets/styles/extensions/_copybutton.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      120 2022-12-07 02:12:21.008050 furo-2024.1.29/src/furo/assets/styles/extensions/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1774 2022-12-07 02:12:21.008134 furo-2024.1.29/src/furo/assets/styles/extensions/_readthedocs.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1895 2022-12-07 02:12:21.008211 furo-2024.1.29/src/furo/assets/styles/extensions/_sphinx-design.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      832 2022-12-07 02:12:21.008305 furo-2024.1.29/src/furo/assets/styles/extensions/_sphinx-inline-tabs.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      604 2022-12-07 02:12:21.008415 furo-2024.1.29/src/furo/assets/styles/extensions/_sphinx-panels.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)       21 2022-12-07 02:12:21.008490 furo-2024.1.29/src/furo/assets/styles/furo-extensions.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      136 2022-12-07 02:12:21.008564 furo-2024.1.29/src/furo/assets/styles/furo.sass
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-02-25 11:33:38.920180 furo-2024.1.29/src/furo/assets/styles/variables/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1386 2023-02-19 16:58:48.371772 furo-2024.1.29/src/furo/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     6355 2022-12-26 19:15:34.355902 furo-2024.1.29/src/furo/assets/styles/variables/_colors.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1366 2022-12-07 02:12:21.008944 furo-2024.1.29/src/furo/assets/styles/variables/_fonts.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3396 2023-02-25 11:33:38.920423 furo-2024.1.29/src/furo/assets/styles/variables/_icons.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)      177 2022-12-07 02:12:21.009133 furo-2024.1.29/src/furo/assets/styles/variables/_index.sass
--rw-r--r--   0 pradyunsg   (501) staff       (20)      334 2022-12-07 02:12:21.009218 furo-2024.1.29/src/furo/assets/styles/variables/_layout.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1211 2023-02-19 17:00:37.502919 furo-2024.1.29/src/furo/assets/styles/variables/_spacing.scss
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2831 2023-04-13 21:46:27.392172 furo-2024.1.29/src/furo/navigation.py
--rw-r--r--   0 pradyunsg   (501) staff       (20)     2425 2023-09-09 22:19:15.862233 furo-2024.1.29/src/furo/sphinxext.py
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2021-11-07 20:44:58.042467 furo-2024.1.29/src/furo/theme/
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-08-18 23:16:51.465851 furo-2024.1.29/src/furo/theme/furo/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3245 2023-08-18 23:16:51.465972 furo-2024.1.29/src/furo/theme/furo/base.html
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.010035 furo-2024.1.29/src/furo/theme/furo/components/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1290 2022-12-07 02:12:21.011302 furo-2024.1.29/src/furo/theme/furo/components/edit-this-page.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1792 2022-12-07 02:12:21.011392 furo-2024.1.29/src/furo/theme/furo/domainindex.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1683 2022-12-07 02:12:21.011474 furo-2024.1.29/src/furo/theme/furo/genindex.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      298 2022-12-07 02:12:21.011555 furo-2024.1.29/src/furo/theme/furo/globaltoc.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      506 2022-12-07 02:12:21.011633 furo-2024.1.29/src/furo/theme/furo/layout.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      297 2022-12-07 02:12:21.011707 furo-2024.1.29/src/furo/theme/furo/localtoc.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)    11025 2023-02-19 17:22:59.452178 furo-2024.1.29/src/furo/theme/furo/page.html
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.012166 furo-2024.1.29/src/furo/theme/furo/partials/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      870 2022-12-07 02:12:21.012118 furo-2024.1.29/src/furo/theme/furo/partials/_head_css_variables.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3342 2023-02-19 17:22:58.491744 furo-2024.1.29/src/furo/theme/furo/partials/icons.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      758 2022-12-07 02:12:21.012606 furo-2024.1.29/src/furo/theme/furo/search.html
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.013631 furo-2024.1.29/src/furo/theme/furo/sidebar/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1076 2022-12-07 02:12:21.012734 furo-2024.1.29/src/furo/theme/furo/sidebar/brand.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      267 2022-12-07 02:12:21.012818 furo-2024.1.29/src/furo/theme/furo/sidebar/ethical-ads.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       63 2022-12-07 02:12:21.012894 furo-2024.1.29/src/furo/theme/furo/sidebar/navigation.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1174 2022-12-07 02:12:21.012981 furo-2024.1.29/src/furo/theme/furo/sidebar/rtd-versions.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)        7 2022-12-07 02:12:21.013057 furo-2024.1.29/src/furo/theme/furo/sidebar/scroll-end.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)       29 2022-12-07 02:12:21.013131 furo-2024.1.29/src/furo/theme/furo/sidebar/scroll-start.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)      350 2022-12-07 02:12:21.013585 furo-2024.1.29/src/furo/theme/furo/sidebar/search.html
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1171 2022-12-07 02:12:21.013671 furo-2024.1.29/src/furo/theme/furo/sidebar/variant-selector.html
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.013729 furo-2024.1.29/src/furo/theme/furo/static/
--rw-r--r--   0 pradyunsg   (501) staff       (20)      112 2022-12-07 02:12:21.013760 furo-2024.1.29/src/furo/theme/furo/static/.gitignore
--rw-r--r--   0 pradyunsg   (501) staff       (20)      574 2022-12-07 02:12:21.014346 furo-2024.1.29/src/furo/theme/furo/theme.conf
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-11-07 21:23:47.887523 furo-2024.1.29/tests/
--rw-r--r--   0 pradyunsg   (501) staff       (20)       54 2023-09-01 22:33:56.796743 furo-2024.1.29/tests/requirements.txt
-drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-12-10 17:15:53.837542 furo-2024.1.29/tests/workflow/
--rw-r--r--   0 pradyunsg   (501) staff       (20)     3023 2023-09-01 22:31:55.015509 furo-2024.1.29/tests/workflow/test_sphinx_versions.py
--rw-r--r--   0 pradyunsg   (501) staff       (20)     1017 2022-12-07 02:12:21.014428 furo-2024.1.29/webpack.config.js
--rw-r--r--   0        0        0     5917 1970-01-01 00:00:00.000000 furo-2024.1.29/PKG-INFO
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-04-27 10:31:33.841484 furo-2024.4.27/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     5212 2022-12-07 02:12:20.980461 furo-2024.4.27/CODE_OF_CONDUCT.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1078 2022-12-07 02:12:20.980570 furo-2024.4.27/LICENSE
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3578 2023-04-26 22:26:30.335543 furo-2024.4.27/README.md
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-04-27 10:23:38.977274 furo-2024.4.27/docs/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:20.992187 furo-2024.4.27/docs/_static/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)   476986 2022-12-07 02:12:20.984051 furo-2024.4.27/docs/_static/demo-dark.png
+-rw-r--r--   0 pradyunsg   (501) staff       (20)   452305 2022-12-07 02:12:20.986929 furo-2024.4.27/docs/_static/demo-light.png
+-rw-r--r--   0 pradyunsg   (501) staff       (20)   775827 2022-12-07 02:12:20.991994 furo-2024.4.27/docs/_static/demo.png
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2110 2022-12-07 02:12:20.992140 furo-2024.4.27/docs/_static/pied-piper-admonition.css
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      182 2022-12-07 02:12:20.992240 furo-2024.4.27/docs/_static/readthedocs-dummy.js
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    20299 2024-04-27 10:27:15.767102 furo-2024.4.27/docs/changelog.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     4931 2024-01-30 01:39:25.360621 furo-2024.4.27/docs/conf.py
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:20.994013 furo-2024.4.27/docs/contributing/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      961 2022-12-07 02:12:20.993810 furo-2024.4.27/docs/contributing/design.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      869 2022-12-07 02:12:20.993895 furo-2024.4.27/docs/contributing/index.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     4790 2022-12-07 02:12:20.993972 furo-2024.4.27/docs/contributing/internals.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3178 2022-12-07 02:12:20.994069 furo-2024.4.27/docs/contributing/workflow.md
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-12-10 17:13:56.071941 furo-2024.4.27/docs/customisation/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      716 2022-12-07 02:12:20.994295 furo-2024.4.27/docs/customisation/announcement.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2199 2022-12-07 02:12:20.994465 furo-2024.4.27/docs/customisation/colors.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1646 2022-12-07 02:12:20.994613 furo-2024.4.27/docs/customisation/edit-button.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      832 2022-12-07 02:12:20.994707 furo-2024.4.27/docs/customisation/fonts.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     5208 2023-12-10 17:13:56.071813 furo-2024.4.27/docs/customisation/footer.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3577 2023-05-20 06:29:53.184453 furo-2024.4.27/docs/customisation/index.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1630 2022-12-07 02:12:20.995041 furo-2024.4.27/docs/customisation/injecting.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      965 2023-12-10 17:13:56.072135 furo-2024.4.27/docs/customisation/landing-page.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1799 2023-05-20 06:29:53.184857 furo-2024.4.27/docs/customisation/logo.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      495 2022-12-07 02:12:20.995279 furo-2024.4.27/docs/customisation/sidebar-title.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3989 2022-12-07 02:12:20.995372 furo-2024.4.27/docs/customisation/sidebar.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      563 2022-12-07 02:12:20.995440 furo-2024.4.27/docs/customisation/toc.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      404 2022-12-07 02:12:20.995513 furo-2024.4.27/docs/index.md
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-12-10 17:13:56.072300 furo-2024.4.27/docs/kitchen-sink/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1317 2023-07-15 10:12:04.480639 furo-2024.4.27/docs/kitchen-sink/admonitions.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1153 2022-12-07 02:12:20.995774 furo-2024.4.27/docs/kitchen-sink/api.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     8423 2023-12-10 17:13:56.072569 furo-2024.4.27/docs/kitchen-sink/blocks.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     8978 2023-04-13 21:50:39.135508 furo-2024.4.27/docs/kitchen-sink/generic.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3070 2022-12-07 02:12:20.996156 furo-2024.4.27/docs/kitchen-sink/images.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      778 2022-12-07 02:12:20.996263 furo-2024.4.27/docs/kitchen-sink/index.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     6177 2022-12-07 02:12:20.996359 furo-2024.4.27/docs/kitchen-sink/lists.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    12941 2023-07-02 07:54:47.884930 furo-2024.4.27/docs/kitchen-sink/really-long.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2584 2022-12-07 02:12:20.996549 furo-2024.4.27/docs/kitchen-sink/sphinx-design.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     6376 2022-12-07 02:12:20.996637 furo-2024.4.27/docs/kitchen-sink/structure.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     5200 2023-07-15 08:51:23.625580 furo-2024.4.27/docs/kitchen-sink/tables.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2668 2022-12-07 02:12:20.996837 furo-2024.4.27/docs/kitchen-sink/typography.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       66 2023-11-06 23:31:33.042578 furo-2024.4.27/docs/license.rst
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      121 2022-12-07 02:12:20.996995 furo-2024.4.27/docs/quickstart.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3271 2022-12-07 02:12:20.997091 furo-2024.4.27/docs/recommendations.md
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-04-09 14:47:21.361291 furo-2024.4.27/docs/reference/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     5455 2022-12-07 02:12:20.997257 furo-2024.4.27/docs/reference/admonitions.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      817 2023-04-09 14:47:21.362077 furo-2024.4.27/docs/reference/api.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1549 2022-12-26 12:21:17.347462 furo-2024.4.27/docs/reference/code-blocks.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1069 2022-12-07 02:12:20.997543 furo-2024.4.27/docs/reference/hyperlinks.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2350 2023-07-15 09:18:08.114960 furo-2024.4.27/docs/reference/images.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      554 2022-12-07 02:12:20.997740 furo-2024.4.27/docs/reference/index.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1606 2022-12-07 02:12:20.997824 furo-2024.4.27/docs/reference/lists.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1372 2022-12-07 02:12:20.997898 furo-2024.4.27/docs/reference/tables.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1020 2022-12-07 02:12:20.997976 furo-2024.4.27/docs/reference/tabs.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1321 2022-12-07 02:12:20.998057 furo-2024.4.27/docs/reference/text-formatting.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       75 2022-12-07 02:12:20.998128 furo-2024.4.27/docs/requirements.txt
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1967 2023-04-13 16:48:43.861620 furo-2024.4.27/docs/stability.md
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     4973 2024-01-30 01:36:38.605170 furo-2024.4.27/noxfile.py
+-rw-r--r--   0 pradyunsg   (501) staff       (20)   123797 2024-04-27 10:23:07.241777 furo-2024.4.27/package-lock.json
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      422 2024-04-27 10:23:07.242305 furo-2024.4.27/package.json
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       60 2022-12-07 02:12:21.002171 furo-2024.4.27/postcss.config.js
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1394 2024-02-16 11:01:24.612304 furo-2024.4.27/pyproject.toml
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2021-11-11 18:55:23.538711 furo-2024.4.27/src/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-04-27 10:31:29.593578 furo-2024.4.27/src/furo/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    12715 2024-04-27 10:31:27.583826 furo-2024.4.27/src/furo/__init__.py
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1764 2024-02-14 21:57:37.106174 furo-2024.4.27/src/furo/_demo_module.py
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.003273 furo-2024.4.27/src/furo/assets/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-01-30 01:36:38.279679 furo-2024.4.27/src/furo/assets/scripts/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     4987 2024-01-30 01:36:38.279984 furo-2024.4.27/src/furo/assets/scripts/furo.js
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    12995 2023-12-10 17:13:56.072855 furo-2024.4.27/src/furo/assets/scripts/gumshoe-patched.js
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-10-11 08:48:22.837263 furo-2024.4.27/src/furo/assets/styles/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    10020 2024-01-30 01:32:10.312810 furo-2024.4.27/src/furo/assets/styles/_scaffold.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      309 2022-12-07 02:12:21.003686 furo-2024.4.27/src/furo/assets/styles/_shame.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.004106 furo-2024.4.27/src/furo/assets/styles/base/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       78 2022-12-07 02:12:21.003806 furo-2024.4.27/src/furo/assets/styles/base/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1403 2022-12-07 02:12:21.003891 furo-2024.4.27/src/furo/assets/styles/base/_print.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      387 2024-01-30 01:45:45.842282 furo-2024.4.27/src/furo/assets/styles/base/_screen-readers.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1307 2022-12-07 02:12:21.004063 furo-2024.4.27/src/furo/assets/styles/base/_theme.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1986 2024-01-30 00:59:20.983828 furo-2024.4.27/src/furo/assets/styles/base/_typography.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-04-27 10:23:07.243569 furo-2024.4.27/src/furo/assets/styles/components/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1978 2023-02-25 11:33:38.920044 furo-2024.4.27/src/furo/assets/styles/components/_footer.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       80 2022-12-07 02:12:21.004909 furo-2024.4.27/src/furo/assets/styles/components/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      328 2022-12-07 02:12:21.004994 furo-2024.4.27/src/furo/assets/styles/components/_search.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     6138 2024-01-30 01:36:38.418271 furo-2024.4.27/src/furo/assets/styles/components/_sidebar.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1835 2024-04-27 10:23:07.243741 furo-2024.4.27/src/furo/assets/styles/components/_table_of_contents.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-04-27 10:23:07.243894 furo-2024.4.27/src/furo/assets/styles/content/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1945 2023-07-15 08:52:07.005777 furo-2024.4.27/src/furo/assets/styles/content/_admonitions.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2282 2024-01-29 23:46:50.094207 furo-2024.4.27/src/furo/assets/styles/content/_api.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      140 2022-12-07 02:12:21.005982 furo-2024.4.27/src/furo/assets/styles/content/_blocks.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      385 2022-12-07 02:12:21.006058 furo-2024.4.27/src/furo/assets/styles/content/_captions.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3231 2023-07-15 10:15:52.575334 furo-2024.4.27/src/furo/assets/styles/content/_code.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      856 2024-04-27 10:23:07.244044 furo-2024.4.27/src/furo/assets/styles/content/_footnotes.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      210 2022-12-07 02:12:21.006461 furo-2024.4.27/src/furo/assets/styles/content/_gui-labels.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      571 2022-12-07 02:12:21.006547 furo-2024.4.27/src/furo/assets/styles/content/_images.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      279 2022-12-07 02:12:21.006627 furo-2024.4.27/src/furo/assets/styles/content/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      312 2022-12-07 02:12:21.006705 furo-2024.4.27/src/furo/assets/styles/content/_indexes.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1090 2022-12-07 02:12:21.006795 furo-2024.4.27/src/furo/assets/styles/content/_lists.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      320 2023-04-13 21:50:43.173530 furo-2024.4.27/src/furo/assets/styles/content/_math.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1139 2022-12-07 02:12:21.006958 furo-2024.4.27/src/furo/assets/styles/content/_misc.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      318 2022-12-07 02:12:21.007281 furo-2024.4.27/src/furo/assets/styles/content/_rubrics.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      562 2022-12-07 02:12:21.007361 furo-2024.4.27/src/furo/assets/styles/content/_sidebar.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      944 2022-12-07 02:12:21.007587 furo-2024.4.27/src/furo/assets/styles/content/_tables.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1927 2024-01-30 01:32:03.792174 furo-2024.4.27/src/furo/assets/styles/content/_target.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.008365 furo-2024.4.27/src/furo/assets/styles/extensions/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      946 2022-12-07 02:12:21.007971 furo-2024.4.27/src/furo/assets/styles/extensions/_copybutton.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      120 2022-12-07 02:12:21.008050 furo-2024.4.27/src/furo/assets/styles/extensions/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1774 2022-12-07 02:12:21.008134 furo-2024.4.27/src/furo/assets/styles/extensions/_readthedocs.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1895 2022-12-07 02:12:21.008211 furo-2024.4.27/src/furo/assets/styles/extensions/_sphinx-design.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      832 2022-12-07 02:12:21.008305 furo-2024.4.27/src/furo/assets/styles/extensions/_sphinx-inline-tabs.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      604 2022-12-07 02:12:21.008415 furo-2024.4.27/src/furo/assets/styles/extensions/_sphinx-panels.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       21 2022-12-07 02:12:21.008490 furo-2024.4.27/src/furo/assets/styles/furo-extensions.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      136 2022-12-07 02:12:21.008564 furo-2024.4.27/src/furo/assets/styles/furo.sass
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-02-14 21:56:45.361121 furo-2024.4.27/src/furo/assets/styles/variables/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1386 2023-02-19 16:58:48.371772 furo-2024.4.27/src/furo/assets/styles/variables/_admonitions.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     6676 2024-02-14 21:56:45.343355 furo-2024.4.27/src/furo/assets/styles/variables/_colors.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1411 2024-01-30 00:53:16.184455 furo-2024.4.27/src/furo/assets/styles/variables/_fonts.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3396 2023-02-25 11:33:38.920423 furo-2024.4.27/src/furo/assets/styles/variables/_icons.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      177 2022-12-07 02:12:21.009133 furo-2024.4.27/src/furo/assets/styles/variables/_index.sass
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      334 2022-12-07 02:12:21.009218 furo-2024.4.27/src/furo/assets/styles/variables/_layout.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1211 2023-02-19 17:00:37.502919 furo-2024.4.27/src/furo/assets/styles/variables/_spacing.scss
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2831 2023-04-13 21:46:27.392172 furo-2024.4.27/src/furo/navigation.py
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     2425 2023-09-09 22:19:15.862233 furo-2024.4.27/src/furo/sphinxext.py
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2021-11-07 20:44:58.042467 furo-2024.4.27/src/furo/theme/
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-04-27 10:23:07.244176 furo-2024.4.27/src/furo/theme/furo/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3245 2023-08-18 23:16:51.465972 furo-2024.4.27/src/furo/theme/furo/base.html
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.010035 furo-2024.4.27/src/furo/theme/furo/components/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1290 2022-12-07 02:12:21.011302 furo-2024.4.27/src/furo/theme/furo/components/edit-this-page.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1792 2022-12-07 02:12:21.011392 furo-2024.4.27/src/furo/theme/furo/domainindex.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1683 2022-12-07 02:12:21.011474 furo-2024.4.27/src/furo/theme/furo/genindex.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      298 2022-12-07 02:12:21.011555 furo-2024.4.27/src/furo/theme/furo/globaltoc.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      506 2022-12-07 02:12:21.011633 furo-2024.4.27/src/furo/theme/furo/layout.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      297 2022-12-07 02:12:21.011707 furo-2024.4.27/src/furo/theme/furo/localtoc.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)    11172 2024-01-30 00:59:20.037638 furo-2024.4.27/src/furo/theme/furo/page.html
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.012166 furo-2024.4.27/src/furo/theme/furo/partials/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      870 2022-12-07 02:12:21.012118 furo-2024.4.27/src/furo/theme/furo/partials/_head_css_variables.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3342 2023-02-19 17:22:58.491744 furo-2024.4.27/src/furo/theme/furo/partials/icons.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      861 2024-04-27 10:23:07.244436 furo-2024.4.27/src/furo/theme/furo/search.html
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.013631 furo-2024.4.27/src/furo/theme/furo/sidebar/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1076 2022-12-07 02:12:21.012734 furo-2024.4.27/src/furo/theme/furo/sidebar/brand.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      267 2022-12-07 02:12:21.012818 furo-2024.4.27/src/furo/theme/furo/sidebar/ethical-ads.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       63 2022-12-07 02:12:21.012894 furo-2024.4.27/src/furo/theme/furo/sidebar/navigation.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1174 2022-12-07 02:12:21.012981 furo-2024.4.27/src/furo/theme/furo/sidebar/rtd-versions.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)        7 2022-12-07 02:12:21.013057 furo-2024.4.27/src/furo/theme/furo/sidebar/scroll-end.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       29 2022-12-07 02:12:21.013131 furo-2024.4.27/src/furo/theme/furo/sidebar/scroll-start.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      350 2022-12-07 02:12:21.013585 furo-2024.4.27/src/furo/theme/furo/sidebar/search.html
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1171 2022-12-07 02:12:21.013671 furo-2024.4.27/src/furo/theme/furo/sidebar/variant-selector.html
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2022-12-07 02:12:21.013729 furo-2024.4.27/src/furo/theme/furo/static/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      112 2022-12-07 02:12:21.013760 furo-2024.4.27/src/furo/theme/furo/static/.gitignore
+-rw-r--r--   0 pradyunsg   (501) staff       (20)      574 2022-12-07 02:12:21.014346 furo-2024.4.27/src/furo/theme/furo/theme.conf
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2023-11-07 21:23:47.887523 furo-2024.4.27/tests/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)       54 2023-09-01 22:33:56.796743 furo-2024.4.27/tests/requirements.txt
+drwxr-xr-x   0 pradyunsg   (501) staff       (20)        0 2024-02-14 21:57:44.566705 furo-2024.4.27/tests/workflow/
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     3023 2023-09-01 22:31:55.015509 furo-2024.4.27/tests/workflow/test_sphinx_versions.py
+-rw-r--r--   0 pradyunsg   (501) staff       (20)     1017 2022-12-07 02:12:21.014428 furo-2024.4.27/webpack.config.js
+-rw-r--r--   0        0        0     5917 1970-01-01 00:00:00.000000 furo-2024.4.27/PKG-INFO
```

### Comparing `furo-2024.1.29/CODE_OF_CONDUCT.md` & `furo-2024.4.27/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/LICENSE` & `furo-2024.4.27/LICENSE`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/README.md` & `furo-2024.4.27/README.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/_static/demo-dark.png` & `furo-2024.4.27/docs/_static/demo-dark.png`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/_static/demo-light.png` & `furo-2024.4.27/docs/_static/demo-light.png`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/_static/demo.png` & `furo-2024.4.27/docs/_static/demo.png`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/_static/pied-piper-admonition.css` & `furo-2024.4.27/docs/_static/pied-piper-admonition.css`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/changelog.md` & `furo-2024.4.27/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,27 @@
 date "+## %Y.%m.%d -- {adjective} {colorname}" | pbcopy
 
 https://patternbasedwriting.com/elementary_writing_success/list-4800-adjectives/
 https://en.wikipedia.org/wiki/Lists_of_colors
 
 -->
 
+## 2024.04.27 -- Bold Burgundy
+
+- Add a skip to content link.
+- Add `--font-stack--headings`.
+- Add `:visited` colour and enforce uniform contrast between light/dark.
+- Add an offset of `:target` to reduce back-to-top overlap.
+- Improve dark mode colours.
+- Fix outstanding colour contrast warnings on Firefox.
+- Fix bad indent in footnotes.
+- Tweak handling of default configuration options in a more resilient manner.
+- Tweak length and sizing of API `source` links.
+- Stop search engine indexing on search page.
+
 ## 2024.01.29 -- Amazing Amethyst
 
 - Fix canonical url when building with `dirhtml`.
 - Relicense the demo module.
 
 ## 2023.09.10 -- Zesty Zaffre
```

### Comparing `furo-2024.1.29/docs/conf.py` & `furo-2024.4.27/docs/conf.py`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/contributing/design.md` & `furo-2024.4.27/docs/contributing/design.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/contributing/index.md` & `furo-2024.4.27/docs/contributing/index.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/contributing/internals.md` & `furo-2024.4.27/docs/contributing/internals.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/contributing/workflow.md` & `furo-2024.4.27/docs/contributing/workflow.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/customisation/announcement.md` & `furo-2024.4.27/docs/customisation/announcement.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/customisation/colors.md` & `furo-2024.4.27/docs/customisation/colors.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/customisation/edit-button.md` & `furo-2024.4.27/docs/customisation/edit-button.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/customisation/fonts.md` & `furo-2024.4.27/docs/customisation/fonts.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/customisation/footer.md` & `furo-2024.4.27/docs/customisation/footer.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/customisation/index.md` & `furo-2024.4.27/docs/customisation/index.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/customisation/injecting.md` & `furo-2024.4.27/docs/customisation/injecting.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/customisation/landing-page.md` & `furo-2024.4.27/docs/customisation/landing-page.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/customisation/logo.md` & `furo-2024.4.27/docs/customisation/logo.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/customisation/sidebar.md` & `furo-2024.4.27/docs/customisation/sidebar.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/customisation/toc.md` & `furo-2024.4.27/docs/customisation/toc.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/kitchen-sink/admonitions.rst` & `furo-2024.4.27/docs/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/kitchen-sink/api.rst` & `furo-2024.4.27/docs/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/kitchen-sink/blocks.rst` & `furo-2024.4.27/docs/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/kitchen-sink/generic.rst` & `furo-2024.4.27/docs/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/kitchen-sink/images.rst` & `furo-2024.4.27/docs/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/kitchen-sink/index.md` & `furo-2024.4.27/docs/kitchen-sink/index.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/kitchen-sink/lists.rst` & `furo-2024.4.27/docs/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/kitchen-sink/really-long.md` & `furo-2024.4.27/docs/kitchen-sink/really-long.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/kitchen-sink/sphinx-design.md` & `furo-2024.4.27/docs/kitchen-sink/sphinx-design.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/kitchen-sink/structure.rst` & `furo-2024.4.27/docs/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/kitchen-sink/tables.rst` & `furo-2024.4.27/docs/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/kitchen-sink/typography.rst` & `furo-2024.4.27/docs/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/recommendations.md` & `furo-2024.4.27/docs/recommendations.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/reference/admonitions.md` & `furo-2024.4.27/docs/reference/admonitions.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/reference/api.md` & `furo-2024.4.27/docs/reference/api.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/reference/code-blocks.md` & `furo-2024.4.27/docs/reference/code-blocks.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/reference/hyperlinks.md` & `furo-2024.4.27/docs/reference/hyperlinks.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/reference/images.md` & `furo-2024.4.27/docs/reference/images.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/reference/index.md` & `furo-2024.4.27/docs/reference/index.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/reference/lists.md` & `furo-2024.4.27/docs/reference/lists.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/reference/tables.md` & `furo-2024.4.27/docs/reference/tables.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/reference/tabs.md` & `furo-2024.4.27/docs/reference/tabs.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/reference/text-formatting.md` & `furo-2024.4.27/docs/reference/text-formatting.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/docs/stability.md` & `furo-2024.4.27/docs/stability.md`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/noxfile.py` & `furo-2024.4.27/noxfile.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,51 +61,51 @@
 
     return _determine_versions(current_version, date=datetime.date.today())
 
 
 #
 # Development Sessions
 #
-@nox.session(reuse_venv=True)
+@nox.session
 def docs(session):
     session.install("-r", "docs/requirements.txt")
     session.install(".")
 
     # Generate documentation into `build/docs`
     session.run("sphinx-build", "-b", "dirhtml", "-v", "docs/", "build/docs")
 
 
-@nox.session(name="docs-live", reuse_venv=True)
+@nox.session(name="docs-live")
 def docs_live(session):
     session.install("-r", "docs/requirements.txt")
     session.install("-e", ".", "sphinx-theme-builder[cli]")
 
     # Generate documentation into `build/docs`
     session.run("stb", "serve", "docs/", *session.posargs)
 
 
-@nox.session(reuse_venv=True)
+@nox.session
 def lint(session):
     session.notify("lint-pre-commit")
     session.notify("lint-mypy")
 
 
-@nox.session(reuse_venv=True, name="lint-pre-commit")
+@nox.session(name="lint-pre-commit")
 def lint_pre_commit(session):
     session.install("pre-commit")
 
     args = list(session.posargs)
     args.append("--all-files")
     if "CI" in os.environ:
         args.append("--show-diff-on-failure")
 
     session.run("pre-commit", "run", *args)
 
 
-@nox.session(reuse_venv=True, name="lint-mypy")
+@nox.session(name="lint-mypy")
 def lint_mypy(session):
     session.install(
         "-e", ".", "mypy", "types-docutils", "types-Pygments", "types-beautifulsoup4"
     )
     session.run("mypy", "src")
```

### Comparing `furo-2024.1.29/package-lock.json` & `furo-2024.4.27/package-lock.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9924107670278909%*

 * *Differences: {"'packages'": "{'': {'devDependencies': {'autoprefixer': '^10.4.19', 'css-loader': '^6.10.0', "*

 * *               "'css-minimizer-webpack-plugin': '^6.0.0', 'mini-css-extract-plugin': '^2.8.1', "*

 * *               "'postcss-loader': '^8.1.1', 'sass': '^1.72.0', 'sass-loader': '^14.1.1', "*

 * *               "'webpack': '^5.91.0'}}, 'node_modules/@webassemblyjs/ast': {'version': '1.12.1', "*

 * *               "'resolved': 'https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.12.1.tgz', "*

 * *               "'integrity': "*

 * *  […]*

```diff
@@ -1,23 +1,23 @@
 {
     "lockfileVersion": 3,
     "name": "furo",
     "packages": {
         "": {
             "devDependencies": {
-                "autoprefixer": "^10.4.14",
-                "css-loader": "^6.7.3",
-                "css-minimizer-webpack-plugin": "^4.2.2",
-                "mini-css-extract-plugin": "^2.7.5",
+                "autoprefixer": "^10.4.19",
+                "css-loader": "^6.10.0",
+                "css-minimizer-webpack-plugin": "^6.0.0",
+                "mini-css-extract-plugin": "^2.8.1",
                 "normalize.css": "^8.0.1",
-                "postcss-loader": "^7.1.0",
-                "sass": "^1.60.0",
-                "sass-loader": "^13.2.1",
+                "postcss-loader": "^8.1.1",
+                "sass": "^1.72.0",
+                "sass-loader": "^14.1.1",
                 "style-loader": "^3.3.2",
-                "webpack": "^5.76.3",
+                "webpack": "^5.91.0",
                 "webpack-cli": "^5.0.1"
             }
         },
         "node_modules/@babel/code-frame": {
             "dependencies": {
                 "@babel/highlight": "^7.23.4",
                 "chalk": "^2.4.2"
@@ -370,17 +370,17 @@
         },
         "node_modules/@webassemblyjs/ast": {
             "dependencies": {
                 "@webassemblyjs/helper-numbers": "1.11.6",
                 "@webassemblyjs/helper-wasm-bytecode": "1.11.6"
             },
             "dev": true,
-            "integrity": "sha512-IN1xI7PwOvLPgjcf180gC1bqn3q/QaOCwYUahIOhbYUu8KA/3tw2RT/T0Gidi1l7Hhj5D/INhJxiICObqpMu4Q==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.6.tgz",
-            "version": "1.11.6"
+            "integrity": "sha512-EKfMUOPRRUTy5UII4qJDGPpqfwjOmZ5jeGFwid9mnoqIFK+e0vqoi1qH56JpmZSzEL53jKnNzScdmftJyG5xWg==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.12.1.tgz",
+            "version": "1.12.1"
         },
         "node_modules/@webassemblyjs/floating-point-hex-parser": {
             "dev": true,
             "integrity": "sha512-ejAj9hfRJ2XMsNHk/v6Fu2dGS+i4UaXBXGemOfQ/JfQ6mdQg/WXtwleQRLLS4OvfDhv8rYnVwH27YJLMyYsxhw==",
             "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.6.tgz",
             "version": "1.11.6"
         },
@@ -388,17 +388,17 @@
             "dev": true,
             "integrity": "sha512-o0YkoP4pVu4rN8aTJgAyj9hC2Sv5UlkzCHhxqWj8butaLvnpdc2jOwh4ewE6CX0txSfLn/UYaV/pheS2Txg//Q==",
             "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.6.tgz",
             "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/helper-buffer": {
             "dev": true,
-            "integrity": "sha512-z3nFzdcp1mb8nEOFFk8DrYLpHvhKC3grJD2ardfKOzmbmJvEf/tPIqCY+sNcwZIY8ZD7IkB2l7/pqhUhqm7hLA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.6.tgz",
-            "version": "1.11.6"
+            "integrity": "sha512-nzJwQw99DNDKr9BVCOZcLuJJUlqkJh+kVzVl6Fmq/tI5ZtEyWT1KZMyOXltXLZJmDtvLCDgwsyrkohEtopTXCw==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.12.1.tgz",
+            "version": "1.12.1"
         },
         "node_modules/@webassemblyjs/helper-numbers": {
             "dependencies": {
                 "@webassemblyjs/floating-point-hex-parser": "1.11.6",
                 "@webassemblyjs/helper-api-error": "1.11.6",
                 "@xtuc/long": "4.2.2"
             },
@@ -411,23 +411,23 @@
             "dev": true,
             "integrity": "sha512-sFFHKwcmBprO9e7Icf0+gddyWYDViL8bpPjJJl0WHxCdETktXdmtWLGVzoHbqUcY4Be1LkNfwTmXOJUFZYSJdA==",
             "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.6.tgz",
             "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/helper-wasm-section": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.6",
-                "@webassemblyjs/helper-buffer": "1.11.6",
+                "@webassemblyjs/ast": "1.12.1",
+                "@webassemblyjs/helper-buffer": "1.12.1",
                 "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
-                "@webassemblyjs/wasm-gen": "1.11.6"
+                "@webassemblyjs/wasm-gen": "1.12.1"
             },
             "dev": true,
-            "integrity": "sha512-LPpZbSOwTpEC2cgn4hTydySy1Ke+XEu+ETXuoyvuyezHO3Kjdu90KK95Sh9xTbmjrCsUwvWwCOQQNta37VrS9g==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.6.tgz",
-            "version": "1.11.6"
+            "integrity": "sha512-Jif4vfB6FJlUlSbgEMHUyk1j234GTNG9dBJ4XJdOySoj518Xj0oGsNi59cUQF4RRMS9ouBUxDDdyBVfPTypa5g==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.12.1.tgz",
+            "version": "1.12.1"
         },
         "node_modules/@webassemblyjs/ieee754": {
             "dependencies": {
                 "@xtuc/ieee754": "^1.2.0"
             },
             "dev": true,
             "integrity": "sha512-LM4p2csPNvbij6U1f19v6WR56QZ8JcHg3QIJTlSwzFcmx6WSORicYj6I63f9yU1kEUtrpG+kjkiIAkevHpDXrg==",
@@ -447,76 +447,76 @@
             "dev": true,
             "integrity": "sha512-vtXf2wTQ3+up9Zsg8sa2yWiQpzSsMyXj0qViVP6xKGCUT8p8YJ6HqI7l5eCnWx1T/FYdsv07HQs2wTFbbof/RA==",
             "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.6.tgz",
             "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/wasm-edit": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.6",
-                "@webassemblyjs/helper-buffer": "1.11.6",
+                "@webassemblyjs/ast": "1.12.1",
+                "@webassemblyjs/helper-buffer": "1.12.1",
                 "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
-                "@webassemblyjs/helper-wasm-section": "1.11.6",
-                "@webassemblyjs/wasm-gen": "1.11.6",
-                "@webassemblyjs/wasm-opt": "1.11.6",
-                "@webassemblyjs/wasm-parser": "1.11.6",
-                "@webassemblyjs/wast-printer": "1.11.6"
+                "@webassemblyjs/helper-wasm-section": "1.12.1",
+                "@webassemblyjs/wasm-gen": "1.12.1",
+                "@webassemblyjs/wasm-opt": "1.12.1",
+                "@webassemblyjs/wasm-parser": "1.12.1",
+                "@webassemblyjs/wast-printer": "1.12.1"
             },
             "dev": true,
-            "integrity": "sha512-Ybn2I6fnfIGuCR+Faaz7YcvtBKxvoLV3Lebn1tM4o/IAJzmi9AWYIPWpyBfU8cC+JxAO57bk4+zdsTjJR+VTOw==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.6.tgz",
-            "version": "1.11.6"
+            "integrity": "sha512-1DuwbVvADvS5mGnXbE+c9NfA8QRcZ6iKquqjjmR10k6o+zzsRVesil54DKexiowcFCPdr/Q0qaMgB01+SQ1u6g==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.12.1.tgz",
+            "version": "1.12.1"
         },
         "node_modules/@webassemblyjs/wasm-gen": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/ast": "1.12.1",
                 "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
                 "@webassemblyjs/ieee754": "1.11.6",
                 "@webassemblyjs/leb128": "1.11.6",
                 "@webassemblyjs/utf8": "1.11.6"
             },
             "dev": true,
-            "integrity": "sha512-3XOqkZP/y6B4F0PBAXvI1/bky7GryoogUtfwExeP/v7Nzwo1QLcq5oQmpKlftZLbT+ERUOAZVQjuNVak6UXjPA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.6.tgz",
-            "version": "1.11.6"
+            "integrity": "sha512-TDq4Ojh9fcohAw6OIMXqiIcTq5KUXTGRkVxbSo1hQnSy6lAM5GSdfwWeSxpAo0YzgsgF182E/U0mDNhuA0tW7w==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.12.1.tgz",
+            "version": "1.12.1"
         },
         "node_modules/@webassemblyjs/wasm-opt": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.6",
-                "@webassemblyjs/helper-buffer": "1.11.6",
-                "@webassemblyjs/wasm-gen": "1.11.6",
-                "@webassemblyjs/wasm-parser": "1.11.6"
+                "@webassemblyjs/ast": "1.12.1",
+                "@webassemblyjs/helper-buffer": "1.12.1",
+                "@webassemblyjs/wasm-gen": "1.12.1",
+                "@webassemblyjs/wasm-parser": "1.12.1"
             },
             "dev": true,
-            "integrity": "sha512-cOrKuLRE7PCe6AsOVl7WasYf3wbSo4CeOk6PkrjS7g57MFfVUF9u6ysQBBODX0LdgSvQqRiGz3CXvIDKcPNy4g==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.6.tgz",
-            "version": "1.11.6"
+            "integrity": "sha512-Jg99j/2gG2iaz3hijw857AVYekZe2SAskcqlWIZXjji5WStnOpVoat3gQfT/Q5tb2djnCjBtMocY/Su1GfxPBg==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.12.1.tgz",
+            "version": "1.12.1"
         },
         "node_modules/@webassemblyjs/wasm-parser": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/ast": "1.12.1",
                 "@webassemblyjs/helper-api-error": "1.11.6",
                 "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
                 "@webassemblyjs/ieee754": "1.11.6",
                 "@webassemblyjs/leb128": "1.11.6",
                 "@webassemblyjs/utf8": "1.11.6"
             },
             "dev": true,
-            "integrity": "sha512-6ZwPeGzMJM3Dqp3hCsLgESxBGtT/OeCvCZ4TA1JUPYgmhAx38tTPR9JaKy0S5H3evQpO/h2uWs2j6Yc/fjkpTQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.6.tgz",
-            "version": "1.11.6"
+            "integrity": "sha512-xikIi7c2FHXysxXe3COrVUPSheuBtpcfhbpFj4gmu7KRLYOzANztwUU0IbsqvMqzuNK2+glRGWCEqZo1WCLyAQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.12.1.tgz",
+            "version": "1.12.1"
         },
         "node_modules/@webassemblyjs/wast-printer": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/ast": "1.12.1",
                 "@xtuc/long": "4.2.2"
             },
             "dev": true,
-            "integrity": "sha512-JM7AhRcE+yW2GWYaKeHL5vt4xqee5N2WcezptmgyhNS+ScggqcT1OtXykhAb13Sn5Yas0j2uv9tHgrjwvzAP4A==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.6.tgz",
-            "version": "1.11.6"
+            "integrity": "sha512-+X4WAlOisVWQMikjbcvY2e0rwPsKQ9F688lksZhBcPycBBuii3O7m8FACbDMWDojpAqvjIncrG8J0XHKyQfVeA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.12.1.tgz",
+            "version": "1.12.1"
         },
         "node_modules/@webpack-cli/configtest": {
             "dev": true,
             "engines": {
                 "node": ">=14.15.0"
             },
             "integrity": "sha512-wy0mglZpDSiSS0XHrVR+BAdId2+yxPSoJW8fsna3ZpYSlufjvxnP4YbKTCBZnNIcGN4r6ZPXV55X4mYExOfLmw==",
@@ -671,16 +671,16 @@
             "version": "2.0.1"
         },
         "node_modules/autoprefixer": {
             "bin": {
                 "autoprefixer": "bin/autoprefixer"
             },
             "dependencies": {
-                "browserslist": "^4.22.2",
-                "caniuse-lite": "^1.0.30001578",
+                "browserslist": "^4.23.0",
+                "caniuse-lite": "^1.0.30001599",
                 "fraction.js": "^4.3.7",
                 "normalize-range": "^0.1.2",
                 "picocolors": "^1.0.0",
                 "postcss-value-parser": "^4.2.0"
             },
             "dev": true,
             "engines": {
@@ -696,20 +696,20 @@
                     "url": "https://tidelift.com/funding/github/npm/autoprefixer"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-/cpVNRLSfhOtcGflT13P2794gVSgmPgTR+erw5ifnMLZb0UnSlkK4tquLmkd3BhA+nLo5tX8Cu0upUsGKvKbmg==",
+            "integrity": "sha512-BaENR2+zBZ8xXhM4pUaKUxlVdxZ0EZhjvbopwnXmxRUfqDmwSpC2lAi/QXvx7NRdPCo1WKEcEF6mV64si1z4Ew==",
             "peerDependencies": {
                 "postcss": "^8.1.0"
             },
-            "resolved": "https://registry.npmjs.org/autoprefixer/-/autoprefixer-10.4.17.tgz",
-            "version": "10.4.17"
+            "resolved": "https://registry.npmjs.org/autoprefixer/-/autoprefixer-10.4.19.tgz",
+            "version": "10.4.19"
         },
         "node_modules/binary-extensions": {
             "dev": true,
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-jDctJ/IVQbZoJykoeHbhXpOlNBqGNcwXJKJog42E5HDPUwQTSdjCHdihjj0DlnheQ7blbT6dHOafNAiS8ooQKA==",
@@ -735,16 +735,16 @@
             "version": "3.0.2"
         },
         "node_modules/browserslist": {
             "bin": {
                 "browserslist": "cli.js"
             },
             "dependencies": {
-                "caniuse-lite": "^1.0.30001580",
-                "electron-to-chromium": "^1.4.648",
+                "caniuse-lite": "^1.0.30001587",
+                "electron-to-chromium": "^1.4.668",
                 "node-releases": "^2.0.14",
                 "update-browserslist-db": "^1.0.13"
             },
             "dev": true,
             "engines": {
                 "node": "^6 || ^7 || ^8 || ^9 || ^10 || ^11 || ^12 || >=13.7"
             },
@@ -758,17 +758,17 @@
                     "url": "https://tidelift.com/funding/github/npm/browserslist"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-UAp55yfwNv0klWNapjs/ktHoguxuQNGnOzxYmfnXIS+8AsRDZkSDxg7R1AX3GKzn078SBI5dzwzj/Yx0Or0e3A==",
-            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.22.3.tgz",
-            "version": "4.22.3"
+            "integrity": "sha512-QW8HiM1shhT2GuzkvklfjcKDiWFXHOeFCIA/huJPwHsslwcydgk7X+z2zXpEijP98UCY7HbubZt5J2Zgvf0CaQ==",
+            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.23.0.tgz",
+            "version": "4.23.0"
         },
         "node_modules/buffer-from": {
             "dev": true,
             "integrity": "sha512-E+XQCRwSbaaiChtv6k6Dwgc+bx+Bs6vuKJHHl5kox/BaKbhiXzqQOwK4cO22yElGp2OCmjwVhT3HmxgyPGnJfQ==",
             "resolved": "https://registry.npmjs.org/buffer-from/-/buffer-from-1.1.2.tgz",
             "version": "1.1.2"
         },
@@ -805,17 +805,17 @@
                     "url": "https://tidelift.com/funding/github/npm/caniuse-lite"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-whlTkwhqV2tUmP3oYhtNfaWGYHDdS3JYFQBKXxcUR9qqPWsRhFHhoISO2Xnl/g0xyKzht9mI1LZpiNWfMzHixQ==",
-            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001581.tgz",
-            "version": "1.0.30001581"
+            "integrity": "sha512-iL2iSS0eDILMb9n5yKQoTBim9jMZ0Yrk8g0N9K7UzYyWnfIKzXBZD5ngpM37ZcL/cv0Mli8XtVMRYMQAfFpi5Q==",
+            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001603.tgz",
+            "version": "1.0.30001603"
         },
         "node_modules/chalk": {
             "dependencies": {
                 "ansi-styles": "^4.1.0",
                 "supports-color": "^7.1.0"
             },
             "dev": true,
@@ -943,37 +943,37 @@
             },
             "integrity": "sha512-QrWXB+ZQSVPmIWIhtEO9H+gwHaMGYiF5ChvoJ+K9ZGHG/sVsa6yiesAD1GC/x46sET00Xlwo1u49RVVVzvcSkw==",
             "resolved": "https://registry.npmjs.org/commander/-/commander-7.2.0.tgz",
             "version": "7.2.0"
         },
         "node_modules/cosmiconfig": {
             "dependencies": {
+                "env-paths": "^2.2.1",
                 "import-fresh": "^3.3.0",
                 "js-yaml": "^4.1.0",
-                "parse-json": "^5.2.0",
-                "path-type": "^4.0.0"
+                "parse-json": "^5.2.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=14"
             },
             "funding": {
                 "url": "https://github.com/sponsors/d-fischer"
             },
-            "integrity": "sha512-kcZ6+W5QzcJ3P1Mt+83OUv/oHFqZHIx8DuxG6eZ5RGMERoLqp4BuGjhHLYGK+Kf5XVkQvqBSmAy/nGWN3qDgEA==",
+            "integrity": "sha512-itvL5h8RETACmOTFc4UfIyB2RfEHi71Ax6E/PivVxq9NseKbOWpeyHEOIbmAw1rs8Ak0VursQNww7lf7YtUwzg==",
             "peerDependencies": {
                 "typescript": ">=4.9.5"
             },
             "peerDependenciesMeta": {
                 "typescript": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/cosmiconfig/-/cosmiconfig-8.3.6.tgz",
-            "version": "8.3.6"
+            "resolved": "https://registry.npmjs.org/cosmiconfig/-/cosmiconfig-9.0.0.tgz",
+            "version": "9.0.0"
         },
         "node_modules/cross-spawn": {
             "dependencies": {
                 "path-key": "^3.1.0",
                 "shebang-command": "^2.0.0",
                 "which": "^2.0.1"
             },
@@ -984,22 +984,22 @@
             "integrity": "sha512-iRDPJKUPVEND7dHPO8rkbOnPpyDygcDFtWjpeWNCgy8WP2rXcxXL8TskReQl6OrB2G7+UJrags1q15Fudc7G6w==",
             "resolved": "https://registry.npmjs.org/cross-spawn/-/cross-spawn-7.0.3.tgz",
             "version": "7.0.3"
         },
         "node_modules/css-declaration-sorter": {
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14"
+                "node": "^14 || ^16 || >=18"
             },
-            "integrity": "sha512-rtdthzxKuyq6IzqX6jEcIzQF/YqccluefyCYheovBOLhFT/drQA9zj/UbRAa9J7C0o6EG6u3E6g+vKkay7/k3g==",
+            "integrity": "sha512-dZ3bVTEEc1vxr3Bek9vGwfB5Z6ESPULhcRvO472mfjVnj8jRcTnKO8/JTczlvxM10Myb+wBM++1MtdO76eWcaQ==",
             "peerDependencies": {
                 "postcss": "^8.0.9"
             },
-            "resolved": "https://registry.npmjs.org/css-declaration-sorter/-/css-declaration-sorter-6.4.1.tgz",
-            "version": "6.4.1"
+            "resolved": "https://registry.npmjs.org/css-declaration-sorter/-/css-declaration-sorter-7.1.1.tgz",
+            "version": "7.1.1"
         },
         "node_modules/css-loader": {
             "dependencies": {
                 "icss-utils": "^5.1.0",
                 "postcss": "^8.4.33",
                 "postcss-modules-extract-imports": "^3.0.0",
                 "postcss-modules-local-by-default": "^4.0.4",
@@ -1012,39 +1012,48 @@
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-OzABOh0+26JKFdMzlK6PY1u5Zx8+Ck7CVRlcGNZoY9qwJjdfu2VWFuprTIpPW+Av5TZTVViYWcFQaEEQURLknQ==",
+            "integrity": "sha512-LTSA/jWbwdMlk+rhmElbDR2vbtQoTBPr7fkJE+mxrHj+7ru0hUmHafDRzWIjIHTwpitWVaqY2/UWGRca3yUgRw==",
             "peerDependencies": {
+                "@rspack/core": "0.x || 1.x",
                 "webpack": "^5.0.0"
             },
-            "resolved": "https://registry.npmjs.org/css-loader/-/css-loader-6.9.1.tgz",
-            "version": "6.9.1"
+            "peerDependenciesMeta": {
+                "@rspack/core": {
+                    "optional": true
+                },
+                "webpack": {
+                    "optional": true
+                }
+            },
+            "resolved": "https://registry.npmjs.org/css-loader/-/css-loader-6.10.0.tgz",
+            "version": "6.10.0"
         },
         "node_modules/css-minimizer-webpack-plugin": {
             "dependencies": {
-                "cssnano": "^5.1.8",
-                "jest-worker": "^29.1.2",
-                "postcss": "^8.4.17",
-                "schema-utils": "^4.0.0",
-                "serialize-javascript": "^6.0.0",
-                "source-map": "^0.6.1"
+                "@jridgewell/trace-mapping": "^0.3.21",
+                "cssnano": "^6.0.3",
+                "jest-worker": "^29.7.0",
+                "postcss": "^8.4.33",
+                "schema-utils": "^4.2.0",
+                "serialize-javascript": "^6.0.2"
             },
             "dev": true,
             "engines": {
-                "node": ">= 14.15.0"
+                "node": ">= 18.12.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-s3Of/4jKfw1Hj9CxEO1E5oXhQAxlayuHO2y/ML+C6I9sQ7FdzfEV6QgMLN3vI+qFsjJGIAFLKtQK7t8BOXAIyA==",
+            "integrity": "sha512-BLpR9CCDkKvhO3i0oZQgad6v9pCxUuhSc5RT6iUEy9M8hBXi4TJb5vqF2GQ2deqYHmRi3O6IR9hgAZQWg0EBwA==",
             "peerDependencies": {
                 "webpack": "^5.0.0"
             },
             "peerDependenciesMeta": {
                 "@parcel/css": {
                     "optional": true
                 },
@@ -1060,45 +1069,45 @@
                 "esbuild": {
                     "optional": true
                 },
                 "lightningcss": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/css-minimizer-webpack-plugin/-/css-minimizer-webpack-plugin-4.2.2.tgz",
-            "version": "4.2.2"
+            "resolved": "https://registry.npmjs.org/css-minimizer-webpack-plugin/-/css-minimizer-webpack-plugin-6.0.0.tgz",
+            "version": "6.0.0"
         },
         "node_modules/css-select": {
             "dependencies": {
                 "boolbase": "^1.0.0",
-                "css-what": "^6.0.1",
-                "domhandler": "^4.3.1",
-                "domutils": "^2.8.0",
+                "css-what": "^6.1.0",
+                "domhandler": "^5.0.2",
+                "domutils": "^3.0.1",
                 "nth-check": "^2.0.1"
             },
             "dev": true,
             "funding": {
                 "url": "https://github.com/sponsors/fb55"
             },
-            "integrity": "sha512-wPpOYtnsVontu2mODhA19JrqWxNsfdatRKd64kmpRbQgh1KtItko5sTnEpPdpSaJszTOhEMlF/RPz28qj4HqhQ==",
-            "resolved": "https://registry.npmjs.org/css-select/-/css-select-4.3.0.tgz",
-            "version": "4.3.0"
+            "integrity": "sha512-nwoRF1rvRRnnCqqY7updORDsuqKzqYJ28+oSMaJMMgOauh3fvwHqMS7EZpIPqK8GL+g9mKxF1vP/ZjSeNjEVHg==",
+            "resolved": "https://registry.npmjs.org/css-select/-/css-select-5.1.0.tgz",
+            "version": "5.1.0"
         },
         "node_modules/css-tree": {
             "dependencies": {
-                "mdn-data": "2.0.14",
-                "source-map": "^0.6.1"
+                "mdn-data": "2.0.30",
+                "source-map-js": "^1.0.1"
             },
             "dev": true,
             "engines": {
-                "node": ">=8.0.0"
+                "node": "^10 || ^12.20.0 || ^14.13.0 || >=15.0.0"
             },
-            "integrity": "sha512-tRpdppF7TRazZrjJ6v3stzv93qxRcSsFmW6cX0Zm2NVKpxE1WV1HblnghVv9TreireHkqI/VDEsfolRF1p6y7Q==",
-            "resolved": "https://registry.npmjs.org/css-tree/-/css-tree-1.1.3.tgz",
-            "version": "1.1.3"
+            "integrity": "sha512-6Fv1DV/TYw//QF5IzQdqsNDjx/wc8TrMBZsqjL9eW01tWb7R7k/mq+/VXfJCl7SoD5emsJop9cOByJZfs8hYIw==",
+            "resolved": "https://registry.npmjs.org/css-tree/-/css-tree-2.3.1.tgz",
+            "version": "2.3.1"
         },
         "node_modules/css-what": {
             "dev": true,
             "engines": {
                 "node": ">= 6"
             },
             "funding": {
@@ -1118,113 +1127,133 @@
             },
             "integrity": "sha512-/Tb/JcjK111nNScGob5MNtsntNM1aCNUDipB/TkwZFhyDrrE47SOx/18wF2bbjgc3ZzCSKW1T5nt5EbFoAz/Vg==",
             "resolved": "https://registry.npmjs.org/cssesc/-/cssesc-3.0.0.tgz",
             "version": "3.0.0"
         },
         "node_modules/cssnano": {
             "dependencies": {
-                "cssnano-preset-default": "^5.2.14",
-                "lilconfig": "^2.0.3",
-                "yaml": "^1.10.2"
+                "cssnano-preset-default": "^6.0.3",
+                "lilconfig": "^3.0.0"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/cssnano"
             },
-            "integrity": "sha512-j+BKgDcLDQA+eDifLx0EO4XSA56b7uut3BQFH+wbSaSTuGLuiyTa/wbRYthUXX8LC9mLg+WWKe8h+qJuwTAbHw==",
+            "integrity": "sha512-MRq4CIj8pnyZpcI2qs6wswoYoDD1t0aL28n+41c1Ukcpm56m1h6mCexIHBGjfZfnTqtGSSCP4/fB1ovxgjBOiw==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/cssnano/-/cssnano-5.1.15.tgz",
-            "version": "5.1.15"
+            "resolved": "https://registry.npmjs.org/cssnano/-/cssnano-6.0.3.tgz",
+            "version": "6.0.3"
         },
         "node_modules/cssnano-preset-default": {
             "dependencies": {
-                "css-declaration-sorter": "^6.3.1",
-                "cssnano-utils": "^3.1.0",
-                "postcss-calc": "^8.2.3",
-                "postcss-colormin": "^5.3.1",
-                "postcss-convert-values": "^5.1.3",
-                "postcss-discard-comments": "^5.1.2",
-                "postcss-discard-duplicates": "^5.1.0",
-                "postcss-discard-empty": "^5.1.1",
-                "postcss-discard-overridden": "^5.1.0",
-                "postcss-merge-longhand": "^5.1.7",
-                "postcss-merge-rules": "^5.1.4",
-                "postcss-minify-font-values": "^5.1.0",
-                "postcss-minify-gradients": "^5.1.1",
-                "postcss-minify-params": "^5.1.4",
-                "postcss-minify-selectors": "^5.2.1",
-                "postcss-normalize-charset": "^5.1.0",
-                "postcss-normalize-display-values": "^5.1.0",
-                "postcss-normalize-positions": "^5.1.1",
-                "postcss-normalize-repeat-style": "^5.1.1",
-                "postcss-normalize-string": "^5.1.0",
-                "postcss-normalize-timing-functions": "^5.1.0",
-                "postcss-normalize-unicode": "^5.1.1",
-                "postcss-normalize-url": "^5.1.0",
-                "postcss-normalize-whitespace": "^5.1.1",
-                "postcss-ordered-values": "^5.1.3",
-                "postcss-reduce-initial": "^5.1.2",
-                "postcss-reduce-transforms": "^5.1.0",
-                "postcss-svgo": "^5.1.0",
-                "postcss-unique-selectors": "^5.1.1"
+                "css-declaration-sorter": "^7.1.1",
+                "cssnano-utils": "^4.0.1",
+                "postcss-calc": "^9.0.1",
+                "postcss-colormin": "^6.0.2",
+                "postcss-convert-values": "^6.0.2",
+                "postcss-discard-comments": "^6.0.1",
+                "postcss-discard-duplicates": "^6.0.1",
+                "postcss-discard-empty": "^6.0.1",
+                "postcss-discard-overridden": "^6.0.1",
+                "postcss-merge-longhand": "^6.0.2",
+                "postcss-merge-rules": "^6.0.3",
+                "postcss-minify-font-values": "^6.0.1",
+                "postcss-minify-gradients": "^6.0.1",
+                "postcss-minify-params": "^6.0.2",
+                "postcss-minify-selectors": "^6.0.2",
+                "postcss-normalize-charset": "^6.0.1",
+                "postcss-normalize-display-values": "^6.0.1",
+                "postcss-normalize-positions": "^6.0.1",
+                "postcss-normalize-repeat-style": "^6.0.1",
+                "postcss-normalize-string": "^6.0.1",
+                "postcss-normalize-timing-functions": "^6.0.1",
+                "postcss-normalize-unicode": "^6.0.2",
+                "postcss-normalize-url": "^6.0.1",
+                "postcss-normalize-whitespace": "^6.0.1",
+                "postcss-ordered-values": "^6.0.1",
+                "postcss-reduce-initial": "^6.0.2",
+                "postcss-reduce-transforms": "^6.0.1",
+                "postcss-svgo": "^6.0.2",
+                "postcss-unique-selectors": "^6.0.2"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-t0SFesj/ZV2OTylqQVOrFgEh5uanxbO6ZAdeCrNsUQ6fVuXwYTxJPNAGvGTxHbD68ldIJNec7PyYZDBrfDQ+6A==",
+            "integrity": "sha512-4y3H370aZCkT9Ev8P4SO4bZbt+AExeKhh8wTbms/X7OLDo5E7AYUUy6YPxa/uF5Grf+AJwNcCnxKhZynJ6luBA==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/cssnano-preset-default/-/cssnano-preset-default-5.2.14.tgz",
-            "version": "5.2.14"
+            "resolved": "https://registry.npmjs.org/cssnano-preset-default/-/cssnano-preset-default-6.0.3.tgz",
+            "version": "6.0.3"
         },
         "node_modules/cssnano-utils": {
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-JQNR19/YZhz4psLX/rQ9M83e3z2Wf/HdJbryzte4a3NSuafyp9w/I4U+hx5C2S9g41qlstH7DEWnZaaj83OuEA==",
+            "integrity": "sha512-6qQuYDqsGoiXssZ3zct6dcMxiqfT6epy7x4R0TQJadd4LWO3sPR6JH6ZByOvVLoZ6EdwPGgd7+DR1EmX3tiXQQ==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/cssnano-utils/-/cssnano-utils-3.1.0.tgz",
-            "version": "3.1.0"
+            "resolved": "https://registry.npmjs.org/cssnano-utils/-/cssnano-utils-4.0.1.tgz",
+            "version": "4.0.1"
         },
         "node_modules/csso": {
             "dependencies": {
-                "css-tree": "^1.1.2"
+                "css-tree": "~2.2.0"
             },
             "dev": true,
             "engines": {
-                "node": ">=8.0.0"
+                "node": "^10 || ^12.20.0 || ^14.13.0 || >=15.0.0",
+                "npm": ">=7.0.0"
             },
-            "integrity": "sha512-wvlcdIbf6pwKEk7vHj8/Bkc0B4ylXZruLvOgs9doS5eOsOpuodOV2zJChSpkp+pRpYQLQMeF04nr3Z68Sta9jA==",
-            "resolved": "https://registry.npmjs.org/csso/-/csso-4.2.0.tgz",
-            "version": "4.2.0"
+            "integrity": "sha512-0LrrStPOdJj+SPCCrGhzryycLjwcgUSHBtxNA8aIDxf0GLsRh1cKYhB00Gd1lDOS4yGH69+SNn13+TWbVHETFQ==",
+            "resolved": "https://registry.npmjs.org/csso/-/csso-5.0.5.tgz",
+            "version": "5.0.5"
+        },
+        "node_modules/csso/node_modules/css-tree": {
+            "dependencies": {
+                "mdn-data": "2.0.28",
+                "source-map-js": "^1.0.1"
+            },
+            "dev": true,
+            "engines": {
+                "node": "^10 || ^12.20.0 || ^14.13.0 || >=15.0.0",
+                "npm": ">=7.0.0"
+            },
+            "integrity": "sha512-OA0mILzGc1kCOCSJerOeqDxDQ4HOh+G8NbOJFOTgOCzpw7fCBubk0fEyxp8AgOL/jvLgYA/uV0cMbe43ElF1JA==",
+            "resolved": "https://registry.npmjs.org/css-tree/-/css-tree-2.2.1.tgz",
+            "version": "2.2.1"
+        },
+        "node_modules/csso/node_modules/mdn-data": {
+            "dev": true,
+            "integrity": "sha512-aylIc7Z9y4yzHYAJNuESG3hfhC+0Ibp/MAMiaOZgNv4pmEdFyfZhhhny4MNiAfWdBQ1RQ2mfDWmM1x8SvGyp8g==",
+            "resolved": "https://registry.npmjs.org/mdn-data/-/mdn-data-2.0.28.tgz",
+            "version": "2.0.28"
         },
         "node_modules/dom-serializer": {
             "dependencies": {
-                "domelementtype": "^2.0.1",
-                "domhandler": "^4.2.0",
-                "entities": "^2.0.0"
+                "domelementtype": "^2.3.0",
+                "domhandler": "^5.0.2",
+                "entities": "^4.2.0"
             },
             "dev": true,
             "funding": {
                 "url": "https://github.com/cheeriojs/dom-serializer?sponsor=1"
             },
-            "integrity": "sha512-VHwB3KfrcOOkelEG2ZOfxqLZdfkil8PtJi4P8N2MMXucZq2yLp75ClViUlOVwyoHEDjYU433Aq+5zWP61+RGag==",
-            "resolved": "https://registry.npmjs.org/dom-serializer/-/dom-serializer-1.4.1.tgz",
-            "version": "1.4.1"
+            "integrity": "sha512-wIkAryiqt/nV5EQKqQpo3SToSOV9J0DnbJqwK7Wv/Trc92zIAYZ4FlMu+JPFW1DfGFt81ZTCGgDEabffXeLyJg==",
+            "resolved": "https://registry.npmjs.org/dom-serializer/-/dom-serializer-2.0.0.tgz",
+            "version": "2.0.0"
         },
         "node_modules/domelementtype": {
             "dev": true,
             "funding": [
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/fb55"
@@ -1232,68 +1261,80 @@
             ],
             "integrity": "sha512-OLETBj6w0OsagBwdXnPdN0cnMfF9opN69co+7ZrbfPGrdpPVNBUj02spi6B1N7wChLQiPn4CSH/zJvXw56gmHw==",
             "resolved": "https://registry.npmjs.org/domelementtype/-/domelementtype-2.3.0.tgz",
             "version": "2.3.0"
         },
         "node_modules/domhandler": {
             "dependencies": {
-                "domelementtype": "^2.2.0"
+                "domelementtype": "^2.3.0"
             },
             "dev": true,
             "engines": {
                 "node": ">= 4"
             },
             "funding": {
                 "url": "https://github.com/fb55/domhandler?sponsor=1"
             },
-            "integrity": "sha512-GrwoxYN+uWlzO8uhUXRl0P+kHE4GtVPfYzVLcUxPL7KNdHKj66vvlhiweIHqYYXWlw+T8iLMp42Lm67ghw4WMQ==",
-            "resolved": "https://registry.npmjs.org/domhandler/-/domhandler-4.3.1.tgz",
-            "version": "4.3.1"
+            "integrity": "sha512-cgwlv/1iFQiFnU96XXgROh8xTeetsnJiDsTc7TYCLFd9+/WNkIqPTxiM/8pSd8VIrhXGTf1Ny1q1hquVqDJB5w==",
+            "resolved": "https://registry.npmjs.org/domhandler/-/domhandler-5.0.3.tgz",
+            "version": "5.0.3"
         },
         "node_modules/domutils": {
             "dependencies": {
-                "dom-serializer": "^1.0.1",
-                "domelementtype": "^2.2.0",
-                "domhandler": "^4.2.0"
+                "dom-serializer": "^2.0.0",
+                "domelementtype": "^2.3.0",
+                "domhandler": "^5.0.3"
             },
             "dev": true,
             "funding": {
                 "url": "https://github.com/fb55/domutils?sponsor=1"
             },
-            "integrity": "sha512-w96Cjofp72M5IIhpjgobBimYEfoPjx1Vx0BSX9P30WBdZW2WIKU0T1Bd0kz2eNZ9ikjKgHbEyKx8BB6H1L3h3A==",
-            "resolved": "https://registry.npmjs.org/domutils/-/domutils-2.8.0.tgz",
-            "version": "2.8.0"
+            "integrity": "sha512-H78uMmQtI2AhgDJjWeQmHwJJ2bLPD3GMmO7Zja/ZZh84wkm+4ut+IUnUdRa8uCGX88DiVx1j6FRe1XfxEgjEZA==",
+            "resolved": "https://registry.npmjs.org/domutils/-/domutils-3.1.0.tgz",
+            "version": "3.1.0"
         },
         "node_modules/electron-to-chromium": {
             "dev": true,
-            "integrity": "sha512-dq/owIaALxZGqWm5RXpKQ4baX6aDC19e2Z16c8SXYN+I71PyEKjbVqQUgm7kcuk8CRqljTKXbolo0XXDjxnh2w==",
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.649.tgz",
-            "version": "1.4.649"
+            "integrity": "sha512-5nLE0TWFFpZ80Crhtp4pIp8LXCztjYX41yUcV6b+bKR2PqzjskTMOOlBi1VjBHlvHwS+4gar7kNKOrsbsewEZQ==",
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.722.tgz",
+            "version": "1.4.722"
         },
         "node_modules/enhanced-resolve": {
             "dependencies": {
                 "graceful-fs": "^4.2.4",
                 "tapable": "^2.2.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=10.13.0"
             },
-            "integrity": "sha512-LXYT42KJ7lpIKECr2mAXIaMldcNCh/7E0KBKOu4KSfkHmP+mZmSs+8V5gBAqisWBy0OO4W5Oyys0GO1Y8KtdKg==",
-            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.15.0.tgz",
-            "version": "5.15.0"
+            "integrity": "sha512-O+QWCviPNSSLAD9Ucn8Awv+poAkqn3T1XY5/N7kR7rQO9yfSGWkYZDwpJ+iKF7B8rxaQKWngSqACpgzeapSyoA==",
+            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.16.0.tgz",
+            "version": "5.16.0"
         },
         "node_modules/entities": {
             "dev": true,
+            "engines": {
+                "node": ">=0.12"
+            },
             "funding": {
                 "url": "https://github.com/fb55/entities?sponsor=1"
             },
-            "integrity": "sha512-p92if5Nz619I0w+akJrLZH0MX0Pb5DX39XOwQTtXSdQQOaYH03S1uIQp4mhOZtAXrxq4ViO67YTiLBo2638o9A==",
-            "resolved": "https://registry.npmjs.org/entities/-/entities-2.2.0.tgz",
-            "version": "2.2.0"
+            "integrity": "sha512-V0hjH4dGPh9Ao5p0MoRY6BVqtwCjhz6vI5LT8AJ55H+4g9/4vbHx1I54fS0XuclLhDHArPQCiMjDxjaL8fPxhw==",
+            "resolved": "https://registry.npmjs.org/entities/-/entities-4.5.0.tgz",
+            "version": "4.5.0"
+        },
+        "node_modules/env-paths": {
+            "dev": true,
+            "engines": {
+                "node": ">=6"
+            },
+            "integrity": "sha512-+h1lkLKhZMTYjog1VEpJNG7NZJWcuc2DDk/qsqSTRRCOXiLjeQ1d1/udrUGhqMxUgAlwKNZ0cf2uqan5GLuS2A==",
+            "resolved": "https://registry.npmjs.org/env-paths/-/env-paths-2.2.1.tgz",
+            "version": "2.2.1"
         },
         "node_modules/envinfo": {
             "bin": {
                 "envinfo": "dist/cli.js"
             },
             "dev": true,
             "engines": {
@@ -1752,19 +1793,19 @@
             "integrity": "sha512-dcS1ul+9tmeD95T+x28/ehLgd9mENa3LsvDTtzm3vyBEO7RPptvAD+t44WVXaUjTBRcrpFeFlC8WCruUR456hw==",
             "resolved": "https://registry.npmjs.org/kind-of/-/kind-of-6.0.3.tgz",
             "version": "6.0.3"
         },
         "node_modules/lilconfig": {
             "dev": true,
             "engines": {
-                "node": ">=10"
+                "node": ">=14"
             },
-            "integrity": "sha512-utWOt/GHzuUxnLKxB6dk81RoOeoNeHgbrXiuGk4yyF5qlRz+iIVWu56E2fqGHFrXz0QNUhLB/8nKqvRH66JKGQ==",
-            "resolved": "https://registry.npmjs.org/lilconfig/-/lilconfig-2.1.0.tgz",
-            "version": "2.1.0"
+            "integrity": "sha512-K2U4W2Ff5ibV7j7ydLr+zLAkIg5JJ4lPn1Ltsdt+Tz/IjQ8buJ55pZAxoP34lqIiwtF9iAvtLv3JGv7CAyAg+g==",
+            "resolved": "https://registry.npmjs.org/lilconfig/-/lilconfig-3.0.0.tgz",
+            "version": "3.0.0"
         },
         "node_modules/lines-and-columns": {
             "dev": true,
             "integrity": "sha512-7ylylesZQ/PV29jhEDl3Ufjo6ZX7gCqJr5F7PKrqc93v7fzSymt1BpwEU8nAUXs8qzzvqhbjhK5QZg6Mt/HkBg==",
             "resolved": "https://registry.npmjs.org/lines-and-columns/-/lines-and-columns-1.2.4.tgz",
             "version": "1.2.4"
         },
@@ -1811,17 +1852,17 @@
             },
             "integrity": "sha512-Jo6dJ04CmSjuznwJSS3pUeWmd/H0ffTlkXXgwZi+eq1UCmqQwCh+eLsYOYCwY991i2Fah4h1BEMCx4qThGbsiA==",
             "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
             "version": "6.0.0"
         },
         "node_modules/mdn-data": {
             "dev": true,
-            "integrity": "sha512-dn6wd0uw5GsdswPFfsgMp5NSB0/aDe6fK94YJV/AJDYXL6HVLWBsxeq7js7Ad+mU2K9LAlwpk6kN2D5mwCPVow==",
-            "resolved": "https://registry.npmjs.org/mdn-data/-/mdn-data-2.0.14.tgz",
-            "version": "2.0.14"
+            "integrity": "sha512-GaqWWShW4kv/G9IEucWScBx9G1/vsFZZJUO+tD26M8J8z3Kw5RDQjaoZe03YAClgeS/SWPOcb4nkFBTEi5DUEA==",
+            "resolved": "https://registry.npmjs.org/mdn-data/-/mdn-data-2.0.30.tgz",
+            "version": "2.0.30"
         },
         "node_modules/merge-stream": {
             "dev": true,
             "integrity": "sha512-abv/qOcuPfk3URPfDzmZU1LKmuw8kT+0nIHvKrKgFrwifol/doWcdA4ZqsWQ8ENrFKkd67Mfpo/LovbIUsbt3w==",
             "resolved": "https://registry.npmjs.org/merge-stream/-/merge-stream-2.0.0.tgz",
             "version": "2.0.0"
         },
@@ -1844,30 +1885,31 @@
             },
             "integrity": "sha512-ZDY+bPm5zTTF+YpCrAU9nK0UgICYPT0QtT1NZWFv4s++TNkcgVaT0g6+4R2uI4MjQjzysHB1zxuWL50hzaeXiw==",
             "resolved": "https://registry.npmjs.org/mime-types/-/mime-types-2.1.35.tgz",
             "version": "2.1.35"
         },
         "node_modules/mini-css-extract-plugin": {
             "dependencies": {
-                "schema-utils": "^4.0.0"
+                "schema-utils": "^4.0.0",
+                "tapable": "^2.2.1"
             },
             "dev": true,
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-+0n11YGyRavUR3IlaOzJ0/4Il1avMvJ1VJfhWfCn24ITQXhRr1gghbhhrda6tgtNcpZaWKdSuwKq20Jb7fnlyw==",
+            "integrity": "sha512-/1HDlyFRxWIZPI1ZpgqlZ8jMw/1Dp/dl3P0L1jtZ+zVcHqwPhGwaJwKL00WVgfnBy6PWCde9W65or7IIETImuA==",
             "peerDependencies": {
                 "webpack": "^5.0.0"
             },
-            "resolved": "https://registry.npmjs.org/mini-css-extract-plugin/-/mini-css-extract-plugin-2.7.7.tgz",
-            "version": "2.7.7"
+            "resolved": "https://registry.npmjs.org/mini-css-extract-plugin/-/mini-css-extract-plugin-2.8.1.tgz",
+            "version": "2.8.1"
         },
         "node_modules/nanoid": {
             "bin": {
                 "nanoid": "bin/nanoid.cjs"
             },
             "dev": true,
             "engines": {
@@ -1909,26 +1951,14 @@
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-bdok/XvKII3nUpklnV6P2hxtMNrCboOjAcyBuQnWEhO665FwrSNRxU+AqpsyvO6LgGYPspN+lu5CLtw4jPRKNA==",
             "resolved": "https://registry.npmjs.org/normalize-range/-/normalize-range-0.1.2.tgz",
             "version": "0.1.2"
         },
-        "node_modules/normalize-url": {
-            "dev": true,
-            "engines": {
-                "node": ">=10"
-            },
-            "funding": {
-                "url": "https://github.com/sponsors/sindresorhus"
-            },
-            "integrity": "sha512-DlL+XwOy3NxAQ8xuC0okPgK46iuVNAK01YN7RueYBqqFeGsBjV9XmCAzAdgt+667bCl5kPh9EqKKDwnaPG1I7A==",
-            "resolved": "https://registry.npmjs.org/normalize-url/-/normalize-url-6.1.0.tgz",
-            "version": "6.1.0"
-        },
         "node_modules/normalize.css": {
             "dev": true,
             "integrity": "sha512-qizSNPO93t1YUuUhP22btGOo3chcvDFqFaj2TRybP0DMxkHOCTYwp3n34fel4a31ORXy4m1Xq0Gyqpb5m33qIg==",
             "resolved": "https://registry.npmjs.org/normalize.css/-/normalize.css-8.0.1.tgz",
             "version": "8.0.1"
         },
         "node_modules/nth-check": {
@@ -2029,23 +2059,14 @@
         },
         "node_modules/path-parse": {
             "dev": true,
             "integrity": "sha512-LDJzPVEEEPR+y48z93A0Ed0yXb8pAByGWo/k5YYdYgpY2/2EsOsksJrq7lOHxryrVOn1ejG6oAp8ahvOIQD8sw==",
             "resolved": "https://registry.npmjs.org/path-parse/-/path-parse-1.0.7.tgz",
             "version": "1.0.7"
         },
-        "node_modules/path-type": {
-            "dev": true,
-            "engines": {
-                "node": ">=8"
-            },
-            "integrity": "sha512-gDKb8aZMDeD/tZWs9P6+q0J9Mwkdl6xMV8TjnGP3qJVJ06bdMgkbBlLU8IdfOsIsFz2BW1rNVT3XuNEl8zPAvw==",
-            "resolved": "https://registry.npmjs.org/path-type/-/path-type-4.0.0.tgz",
-            "version": "4.0.0"
-        },
         "node_modules/picocolors": {
             "dev": true,
             "integrity": "sha512-1fygroTLlHu66zi26VoTDv8yRgm0Fccecssto+MhsZ0D/DGW2sm8E8AjW7NU5VVTRt5GxbeZ5qBuJr+HyLYkjQ==",
             "resolved": "https://registry.npmjs.org/picocolors/-/picocolors-1.0.0.tgz",
             "version": "1.0.0"
         },
         "node_modules/picomatch": {
@@ -2098,226 +2119,238 @@
             ],
             "integrity": "sha512-Kkpbhhdjw2qQs2O2DGX+8m5OVqEcbB9HRBvuYM9pgrjEFUg30A9LmXNlTAUj4S9kgtGyrMbTzVjH7E+s5Re2yg==",
             "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.33.tgz",
             "version": "8.4.33"
         },
         "node_modules/postcss-calc": {
             "dependencies": {
-                "postcss-selector-parser": "^6.0.9",
+                "postcss-selector-parser": "^6.0.11",
                 "postcss-value-parser": "^4.2.0"
             },
             "dev": true,
-            "integrity": "sha512-SmWMSJmB8MRnnULldx0lQIyhSNvuDl9HfrZkaqqE/WHAhToYsAvDq+yAsA/kIyINDszOp3Rh0GFoNuH5Ypsm3Q==",
+            "engines": {
+                "node": "^14 || ^16 || >=18.0"
+            },
+            "integrity": "sha512-TipgjGyzP5QzEhsOZUaIkeO5mKeMFpebWzRogWG/ysonUlnHcq5aJe0jOjpfzUU8PeSaBQnrE8ehR0QA5vs8PQ==",
             "peerDependencies": {
                 "postcss": "^8.2.2"
             },
-            "resolved": "https://registry.npmjs.org/postcss-calc/-/postcss-calc-8.2.4.tgz",
-            "version": "8.2.4"
+            "resolved": "https://registry.npmjs.org/postcss-calc/-/postcss-calc-9.0.1.tgz",
+            "version": "9.0.1"
         },
         "node_modules/postcss-colormin": {
             "dependencies": {
-                "browserslist": "^4.21.4",
+                "browserslist": "^4.22.2",
                 "caniuse-api": "^3.0.0",
                 "colord": "^2.9.1",
                 "postcss-value-parser": "^4.2.0"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-UsWQG0AqTFQmpBegeLLc1+c3jIqBNB0zlDGRWR+dQ3pRKJL1oeMzyqmH3o2PIfn9MBdNrVPWhDbT769LxCTLJQ==",
+            "integrity": "sha512-TXKOxs9LWcdYo5cgmcSHPkyrLAh86hX1ijmyy6J8SbOhyv6ua053M3ZAM/0j44UsnQNIWdl8gb5L7xX2htKeLw==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-colormin/-/postcss-colormin-5.3.1.tgz",
-            "version": "5.3.1"
+            "resolved": "https://registry.npmjs.org/postcss-colormin/-/postcss-colormin-6.0.2.tgz",
+            "version": "6.0.2"
         },
         "node_modules/postcss-convert-values": {
             "dependencies": {
-                "browserslist": "^4.21.4",
+                "browserslist": "^4.22.2",
                 "postcss-value-parser": "^4.2.0"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-82pC1xkJZtcJEfiLw6UXnXVXScgtBrjlO5CBmuDQc+dlb88ZYheFsjTn40+zBVi3DkfF7iezO0nJUPLcJK3pvA==",
+            "integrity": "sha512-aeBmaTnGQ+NUSVQT8aY0sKyAD/BaLJenEKZ03YK0JnDE1w1Rr8XShoxdal2V2H26xTJKr3v5haByOhJuyT4UYw==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-convert-values/-/postcss-convert-values-5.1.3.tgz",
-            "version": "5.1.3"
+            "resolved": "https://registry.npmjs.org/postcss-convert-values/-/postcss-convert-values-6.0.2.tgz",
+            "version": "6.0.2"
         },
         "node_modules/postcss-discard-comments": {
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-+L8208OVbHVF2UQf1iDmRcbdjJkuBF6IS29yBDSiWUIzpYaAhtNl6JYnYm12FnkeCwQqF5LeklOu6rAqgfBZqQ==",
+            "integrity": "sha512-f1KYNPtqYLUeZGCHQPKzzFtsHaRuECe6jLakf/RjSRqvF5XHLZnM2+fXLhb8Qh/HBFHs3M4cSLb1k3B899RYIg==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-discard-comments/-/postcss-discard-comments-5.1.2.tgz",
-            "version": "5.1.2"
+            "resolved": "https://registry.npmjs.org/postcss-discard-comments/-/postcss-discard-comments-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "node_modules/postcss-discard-duplicates": {
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-zmX3IoSI2aoenxHV6C7plngHWWhUOV3sP1T8y2ifzxzbtnuhk1EdPwm0S1bIUNaJ2eNbWeGLEwzw8huPD67aQw==",
+            "integrity": "sha512-1hvUs76HLYR8zkScbwyJ8oJEugfPV+WchpnA+26fpJ7Smzs51CzGBHC32RS03psuX/2l0l0UKh2StzNxOrKCYg==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-discard-duplicates/-/postcss-discard-duplicates-5.1.0.tgz",
-            "version": "5.1.0"
+            "resolved": "https://registry.npmjs.org/postcss-discard-duplicates/-/postcss-discard-duplicates-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "node_modules/postcss-discard-empty": {
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-zPz4WljiSuLWsI0ir4Mcnr4qQQ5e1Ukc3i7UfE2XcrwKK2LIPIqE5jxMRxO6GbI3cv//ztXDsXwEWT3BHOGh3A==",
+            "integrity": "sha512-yitcmKwmVWtNsrrRqGJ7/C0YRy53i0mjexBDQ9zYxDwTWVBgbU4+C9jIZLmQlTDT9zhml+u0OMFJh8+31krmOg==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-discard-empty/-/postcss-discard-empty-5.1.1.tgz",
-            "version": "5.1.1"
+            "resolved": "https://registry.npmjs.org/postcss-discard-empty/-/postcss-discard-empty-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "node_modules/postcss-discard-overridden": {
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-21nOL7RqWR1kasIVdKs8HNqQJhFxLsyRfAnUDm4Fe4t4mCWL9OJiHvlHPjcd8zc5Myu89b/7wZDnOSjFgeWRtw==",
+            "integrity": "sha512-qs0ehZMMZpSESbRkw1+inkf51kak6OOzNRaoLd/U7Fatp0aN2HQ1rxGOrJvYcRAN9VpX8kUF13R2ofn8OlvFVA==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-discard-overridden/-/postcss-discard-overridden-5.1.0.tgz",
-            "version": "5.1.0"
+            "resolved": "https://registry.npmjs.org/postcss-discard-overridden/-/postcss-discard-overridden-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "node_modules/postcss-loader": {
             "dependencies": {
-                "cosmiconfig": "^8.3.5",
+                "cosmiconfig": "^9.0.0",
                 "jiti": "^1.20.0",
                 "semver": "^7.5.4"
             },
             "dev": true,
             "engines": {
-                "node": ">= 14.15.0"
+                "node": ">= 18.12.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-iW5WTTBSC5BfsBJ9daFMPVrLT36MrNiC6fqOZTTaHjBNX6Pfd5p+hSBqe/fEeNd7pc13QiAyGt7VdGMw4eRC4A==",
+            "integrity": "sha512-0IeqyAsG6tYiDRCYKQJLAmgQr47DX6N7sFSWvQxt6AcupX8DIdmykuk/o/tx0Lze3ErGHJEp5OSRxrelC6+NdQ==",
             "peerDependencies": {
+                "@rspack/core": "0.x || 1.x",
                 "postcss": "^7.0.0 || ^8.0.1",
                 "webpack": "^5.0.0"
             },
-            "resolved": "https://registry.npmjs.org/postcss-loader/-/postcss-loader-7.3.4.tgz",
-            "version": "7.3.4"
+            "peerDependenciesMeta": {
+                "@rspack/core": {
+                    "optional": true
+                },
+                "webpack": {
+                    "optional": true
+                }
+            },
+            "resolved": "https://registry.npmjs.org/postcss-loader/-/postcss-loader-8.1.1.tgz",
+            "version": "8.1.1"
         },
         "node_modules/postcss-merge-longhand": {
             "dependencies": {
                 "postcss-value-parser": "^4.2.0",
-                "stylehacks": "^5.1.1"
+                "stylehacks": "^6.0.2"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-YCI9gZB+PLNskrK0BB3/2OzPnGhPkBEwmwhfYk1ilBHYVAZB7/tkTHFBAnCrvBBOmeYyMYw3DMjT55SyxMBzjQ==",
+            "integrity": "sha512-+yfVB7gEM8SrCo9w2lCApKIEzrTKl5yS1F4yGhV3kSim6JzbfLGJyhR1B6X+6vOT0U33Mgx7iv4X9MVWuaSAfw==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-merge-longhand/-/postcss-merge-longhand-5.1.7.tgz",
-            "version": "5.1.7"
+            "resolved": "https://registry.npmjs.org/postcss-merge-longhand/-/postcss-merge-longhand-6.0.2.tgz",
+            "version": "6.0.2"
         },
         "node_modules/postcss-merge-rules": {
             "dependencies": {
-                "browserslist": "^4.21.4",
+                "browserslist": "^4.22.2",
                 "caniuse-api": "^3.0.0",
-                "cssnano-utils": "^3.1.0",
-                "postcss-selector-parser": "^6.0.5"
+                "cssnano-utils": "^4.0.1",
+                "postcss-selector-parser": "^6.0.15"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-0R2IuYpgU93y9lhVbO/OylTtKMVcHb67zjWIfCiKR9rWL3GUk1677LAqD/BcHizukdZEjT8Ru3oHRoAYoJy44g==",
+            "integrity": "sha512-yfkDqSHGohy8sGYIJwBmIGDv4K4/WrJPX355XrxQb/CSsT4Kc/RxDi6akqn5s9bap85AWgv21ArcUWwWdGNSHA==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-merge-rules/-/postcss-merge-rules-5.1.4.tgz",
-            "version": "5.1.4"
+            "resolved": "https://registry.npmjs.org/postcss-merge-rules/-/postcss-merge-rules-6.0.3.tgz",
+            "version": "6.0.3"
         },
         "node_modules/postcss-minify-font-values": {
             "dependencies": {
                 "postcss-value-parser": "^4.2.0"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-el3mYTgx13ZAPPirSVsHqFzl+BBBDrXvbySvPGFnQcTI4iNslrPaFq4muTkLZmKlGk4gyFAYUBMH30+HurREyA==",
+            "integrity": "sha512-tIwmF1zUPoN6xOtA/2FgVk1ZKrLcCvE0dpZLtzyyte0j9zUeB8RTbCqrHZGjJlxOvNWKMYtunLrrl7HPOiR46w==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-minify-font-values/-/postcss-minify-font-values-5.1.0.tgz",
-            "version": "5.1.0"
+            "resolved": "https://registry.npmjs.org/postcss-minify-font-values/-/postcss-minify-font-values-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "node_modules/postcss-minify-gradients": {
             "dependencies": {
                 "colord": "^2.9.1",
-                "cssnano-utils": "^3.1.0",
+                "cssnano-utils": "^4.0.1",
                 "postcss-value-parser": "^4.2.0"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-VGvXMTpCEo4qHTNSa9A0a3D+dxGFZCYwR6Jokk+/3oB6flu2/PnPXAh2x7x52EkY5xlIHLm+Le8tJxe/7TNhzw==",
+            "integrity": "sha512-M1RJWVjd6IOLPl1hYiOd5HQHgpp6cvJVLrieQYS9y07Yo8itAr6jaekzJphaJFR0tcg4kRewCk3kna9uHBxn/w==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-minify-gradients/-/postcss-minify-gradients-5.1.1.tgz",
-            "version": "5.1.1"
+            "resolved": "https://registry.npmjs.org/postcss-minify-gradients/-/postcss-minify-gradients-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "node_modules/postcss-minify-params": {
             "dependencies": {
-                "browserslist": "^4.21.4",
-                "cssnano-utils": "^3.1.0",
+                "browserslist": "^4.22.2",
+                "cssnano-utils": "^4.0.1",
                 "postcss-value-parser": "^4.2.0"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-+mePA3MgdmVmv6g+30rn57USjOGSAyuxUmkfiWpzalZ8aiBkdPYjXWtHuwJGm1v5Ojy0Z0LaSYhHaLJQB0P8Jw==",
+            "integrity": "sha512-zwQtbrPEBDj+ApELZ6QylLf2/c5zmASoOuA4DzolyVGdV38iR2I5QRMsZcHkcdkZzxpN8RS4cN7LPskOkTwTZw==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-minify-params/-/postcss-minify-params-5.1.4.tgz",
-            "version": "5.1.4"
+            "resolved": "https://registry.npmjs.org/postcss-minify-params/-/postcss-minify-params-6.0.2.tgz",
+            "version": "6.0.2"
         },
         "node_modules/postcss-minify-selectors": {
             "dependencies": {
-                "postcss-selector-parser": "^6.0.5"
+                "postcss-selector-parser": "^6.0.15"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-nPJu7OjZJTsVUmPdm2TcaiohIwxP+v8ha9NehQ2ye9szv4orirRU3SDdtUmKH+10nzn0bAyOXZ0UEr7OpvLehg==",
+            "integrity": "sha512-0b+m+w7OAvZejPQdN2GjsXLv5o0jqYHX3aoV0e7RBKPCsB7TYG5KKWBFhGnB/iP3213Ts8c5H4wLPLMm7z28Sg==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-minify-selectors/-/postcss-minify-selectors-5.2.1.tgz",
-            "version": "5.2.1"
+            "resolved": "https://registry.npmjs.org/postcss-minify-selectors/-/postcss-minify-selectors-6.0.2.tgz",
+            "version": "6.0.2"
         },
         "node_modules/postcss-modules-extract-imports": {
             "dev": true,
             "engines": {
                 "node": "^10 || ^12 || >= 14"
             },
             "integrity": "sha512-bdHleFnP3kZ4NYDhuGlVK+CMrQ/pqUm8bx/oGL93K6gVwiclvX5x0n76fYMKuIGKzlABOy13zsvqjb0f92TEXw==",
@@ -2373,191 +2406,190 @@
             },
             "resolved": "https://registry.npmjs.org/postcss-modules-values/-/postcss-modules-values-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/postcss-normalize-charset": {
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-mSgUJ+pd/ldRGVx26p2wz9dNZ7ji6Pn8VWBajMXFf8jk7vUoSrZ2lt/wZR7DtlZYKesmZI680qjr2CeFF2fbUg==",
+            "integrity": "sha512-aW5LbMNRZ+oDV57PF9K+WI1Z8MPnF+A8qbajg/T8PP126YrGX1f9IQx21GI2OlGz7XFJi/fNi0GTbY948XJtXg==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-normalize-charset/-/postcss-normalize-charset-5.1.0.tgz",
-            "version": "5.1.0"
+            "resolved": "https://registry.npmjs.org/postcss-normalize-charset/-/postcss-normalize-charset-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "node_modules/postcss-normalize-display-values": {
             "dependencies": {
                 "postcss-value-parser": "^4.2.0"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-WP4KIM4o2dazQXWmFaqMmcvsKmhdINFblgSeRgn8BJ6vxaMyaJkwAzpPpuvSIoG/rmX3M+IrRZEz2H0glrQNEA==",
+            "integrity": "sha512-mc3vxp2bEuCb4LgCcmG1y6lKJu1Co8T+rKHrcbShJwUmKJiEl761qb/QQCfFwlrvSeET3jksolCR/RZuMURudw==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-normalize-display-values/-/postcss-normalize-display-values-5.1.0.tgz",
-            "version": "5.1.0"
+            "resolved": "https://registry.npmjs.org/postcss-normalize-display-values/-/postcss-normalize-display-values-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "node_modules/postcss-normalize-positions": {
             "dependencies": {
                 "postcss-value-parser": "^4.2.0"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-6UpCb0G4eofTCQLFVuI3EVNZzBNPiIKcA1AKVka+31fTVySphr3VUgAIULBhxZkKgwLImhzMR2Bw1ORK+37INg==",
+            "integrity": "sha512-HRsq8u/0unKNvm0cvwxcOUEcakFXqZ41fv3FOdPn916XFUrympjr+03oaLkuZENz3HE9RrQE9yU0Xv43ThWjQg==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-normalize-positions/-/postcss-normalize-positions-5.1.1.tgz",
-            "version": "5.1.1"
+            "resolved": "https://registry.npmjs.org/postcss-normalize-positions/-/postcss-normalize-positions-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "node_modules/postcss-normalize-repeat-style": {
             "dependencies": {
                 "postcss-value-parser": "^4.2.0"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-mFpLspGWkQtBcWIRFLmewo8aC3ImN2i/J3v8YCFUwDnPu3Xz4rLohDO26lGjwNsQxB3YF0KKRwspGzE2JEuS0g==",
+            "integrity": "sha512-Gbb2nmCy6tTiA7Sh2MBs3fj9W8swonk6lw+dFFeQT68B0Pzwp1kvisJQkdV6rbbMSd9brMlS8I8ts52tAGWmGQ==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-normalize-repeat-style/-/postcss-normalize-repeat-style-5.1.1.tgz",
-            "version": "5.1.1"
+            "resolved": "https://registry.npmjs.org/postcss-normalize-repeat-style/-/postcss-normalize-repeat-style-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "node_modules/postcss-normalize-string": {
             "dependencies": {
                 "postcss-value-parser": "^4.2.0"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-oYiIJOf4T9T1N4i+abeIc7Vgm/xPCGih4bZz5Nm0/ARVJ7K6xrDlLwvwqOydvyL3RHNf8qZk6vo3aatiw/go3w==",
+            "integrity": "sha512-5Fhx/+xzALJD9EI26Aq23hXwmv97Zfy2VFrt5PLT8lAhnBIZvmaT5pQk+NuJ/GWj/QWaKSKbnoKDGLbV6qnhXg==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-normalize-string/-/postcss-normalize-string-5.1.0.tgz",
-            "version": "5.1.0"
+            "resolved": "https://registry.npmjs.org/postcss-normalize-string/-/postcss-normalize-string-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "node_modules/postcss-normalize-timing-functions": {
             "dependencies": {
                 "postcss-value-parser": "^4.2.0"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-DOEkzJ4SAXv5xkHl0Wa9cZLF3WCBhF3o1SKVxKQAa+0pYKlueTpCgvkFAHfk+Y64ezX9+nITGrDZeVGgITJXjg==",
+            "integrity": "sha512-4zcczzHqmCU7L5dqTB9rzeqPWRMc0K2HoR+Bfl+FSMbqGBUcP5LRfgcH4BdRtLuzVQK1/FHdFoGT3F7rkEnY+g==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-normalize-timing-functions/-/postcss-normalize-timing-functions-5.1.0.tgz",
-            "version": "5.1.0"
+            "resolved": "https://registry.npmjs.org/postcss-normalize-timing-functions/-/postcss-normalize-timing-functions-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "node_modules/postcss-normalize-unicode": {
             "dependencies": {
-                "browserslist": "^4.21.4",
+                "browserslist": "^4.22.2",
                 "postcss-value-parser": "^4.2.0"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-qnCL5jzkNUmKVhZoENp1mJiGNPcsJCs1aaRmURmeJGES23Z/ajaln+EPTD+rBeNkSryI+2WTdW+lwcVdOikrpA==",
+            "integrity": "sha512-Ff2VdAYCTGyMUwpevTZPZ4w0+mPjbZzLLyoLh/RMpqUqeQKZ+xMm31hkxBavDcGKcxm6ACzGk0nBfZ8LZkStKA==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-normalize-unicode/-/postcss-normalize-unicode-5.1.1.tgz",
-            "version": "5.1.1"
+            "resolved": "https://registry.npmjs.org/postcss-normalize-unicode/-/postcss-normalize-unicode-6.0.2.tgz",
+            "version": "6.0.2"
         },
         "node_modules/postcss-normalize-url": {
             "dependencies": {
-                "normalize-url": "^6.0.1",
                 "postcss-value-parser": "^4.2.0"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-5upGeDO+PVthOxSmds43ZeMeZfKH+/DKgGRD7TElkkyS46JXAUhMzIKiCa7BabPeIy3AQcTkXwVVN7DbqsiCew==",
+            "integrity": "sha512-jEXL15tXSvbjm0yzUV7FBiEXwhIa9H88JOXDGQzmcWoB4mSjZIsmtto066s2iW9FYuIrIF4k04HA2BKAOpbsaQ==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-normalize-url/-/postcss-normalize-url-5.1.0.tgz",
-            "version": "5.1.0"
+            "resolved": "https://registry.npmjs.org/postcss-normalize-url/-/postcss-normalize-url-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "node_modules/postcss-normalize-whitespace": {
             "dependencies": {
                 "postcss-value-parser": "^4.2.0"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-83ZJ4t3NUDETIHTa3uEg6asWjSBYL5EdkVB0sDncx9ERzOKBVJIUeDO9RyA9Zwtig8El1d79HBp0JEi8wvGQnA==",
+            "integrity": "sha512-76i3NpWf6bB8UHlVuLRxG4zW2YykF9CTEcq/9LGAiz2qBuX5cBStadkk0jSkg9a9TCIXbMQz7yzrygKoCW9JuA==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-normalize-whitespace/-/postcss-normalize-whitespace-5.1.1.tgz",
-            "version": "5.1.1"
+            "resolved": "https://registry.npmjs.org/postcss-normalize-whitespace/-/postcss-normalize-whitespace-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "node_modules/postcss-ordered-values": {
             "dependencies": {
-                "cssnano-utils": "^3.1.0",
+                "cssnano-utils": "^4.0.1",
                 "postcss-value-parser": "^4.2.0"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-9UO79VUhPwEkzbb3RNpqqghc6lcYej1aveQteWY+4POIwlqkYE21HKWaLDF6lWNuqCobEAyTovVhtI32Rbv2RQ==",
+            "integrity": "sha512-XXbb1O/MW9HdEhnBxitZpPFbIvDgbo9NK4c/5bOfiKpnIGZDoL2xd7/e6jW5DYLsWxBbs+1nZEnVgnjnlFViaA==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-ordered-values/-/postcss-ordered-values-5.1.3.tgz",
-            "version": "5.1.3"
+            "resolved": "https://registry.npmjs.org/postcss-ordered-values/-/postcss-ordered-values-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "node_modules/postcss-reduce-initial": {
             "dependencies": {
-                "browserslist": "^4.21.4",
+                "browserslist": "^4.22.2",
                 "caniuse-api": "^3.0.0"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-dE/y2XRaqAi6OvjzD22pjTUQ8eOfc6m/natGHgKFBK9DxFmIm69YmaRVQrGgFlEfc1HePIurY0TmDeROK05rIg==",
+            "integrity": "sha512-YGKalhNlCLcjcLvjU5nF8FyeCTkCO5UtvJEt0hrPZVCTtRLSOH4z00T1UntQPj4dUmIYZgMj8qK77JbSX95hSw==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-reduce-initial/-/postcss-reduce-initial-5.1.2.tgz",
-            "version": "5.1.2"
+            "resolved": "https://registry.npmjs.org/postcss-reduce-initial/-/postcss-reduce-initial-6.0.2.tgz",
+            "version": "6.0.2"
         },
         "node_modules/postcss-reduce-transforms": {
             "dependencies": {
                 "postcss-value-parser": "^4.2.0"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-2fbdbmgir5AvpW9RLtdONx1QoYG2/EtqpNQbFASDlixBbAYuTcJ0dECwlqNqH7VbaUnEnh8SrxOe2sRIn24XyQ==",
+            "integrity": "sha512-fUbV81OkUe75JM+VYO1gr/IoA2b/dRiH6HvMwhrIBSUrxq3jNZQZitSnugcTLDi1KkQh1eR/zi+iyxviUNBkcQ==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-reduce-transforms/-/postcss-reduce-transforms-5.1.0.tgz",
-            "version": "5.1.0"
+            "resolved": "https://registry.npmjs.org/postcss-reduce-transforms/-/postcss-reduce-transforms-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "node_modules/postcss-selector-parser": {
             "dependencies": {
                 "cssesc": "^3.0.0",
                 "util-deprecate": "^1.0.2"
             },
             "dev": true,
@@ -2567,41 +2599,41 @@
             "integrity": "sha512-rEYkQOMUCEMhsKbK66tbEU9QVIxbhN18YiniAwA7XQYTVBqrBy+P2p5JcdqsHgKM2zWylp8d7J6eszocfds5Sw==",
             "resolved": "https://registry.npmjs.org/postcss-selector-parser/-/postcss-selector-parser-6.0.15.tgz",
             "version": "6.0.15"
         },
         "node_modules/postcss-svgo": {
             "dependencies": {
                 "postcss-value-parser": "^4.2.0",
-                "svgo": "^2.7.0"
+                "svgo": "^3.2.0"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >= 18"
             },
-            "integrity": "sha512-D75KsH1zm5ZrHyxPakAxJWtkyXew5qwS70v56exwvw542d9CRtTo78K0WeFxZB4G7JXKKMbEZtZayTGdIky/eA==",
+            "integrity": "sha512-IH5R9SjkTkh0kfFOQDImyy1+mTCb+E830+9SV1O+AaDcoHTvfsvt6WwJeo7KwcHbFnevZVCsXhDmjFiGVuwqFQ==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-svgo/-/postcss-svgo-5.1.0.tgz",
-            "version": "5.1.0"
+            "resolved": "https://registry.npmjs.org/postcss-svgo/-/postcss-svgo-6.0.2.tgz",
+            "version": "6.0.2"
         },
         "node_modules/postcss-unique-selectors": {
             "dependencies": {
-                "postcss-selector-parser": "^6.0.5"
+                "postcss-selector-parser": "^6.0.15"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-5JiODlELrz8L2HwxfPnhOWZYWDxVHWL83ufOv84NrcgipI7TaeRsatAhK4Tr2/ZiYldpK/wBvw5BD3qfaK96GA==",
+            "integrity": "sha512-8IZGQ94nechdG7Y9Sh9FlIY2b4uS8/k8kdKRX040XHsS3B6d1HrJAkXrBSsSu4SuARruSsUjW3nlSw8BHkaAYQ==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/postcss-unique-selectors/-/postcss-unique-selectors-5.1.1.tgz",
-            "version": "5.1.1"
+            "resolved": "https://registry.npmjs.org/postcss-unique-selectors/-/postcss-unique-selectors-6.0.2.tgz",
+            "version": "6.0.2"
         },
         "node_modules/postcss-value-parser": {
             "dev": true,
             "integrity": "sha512-1NNCs6uurfkVbeXG4S8JFT9t19m45ICnif8zWLd5oPSZ50QnwMfK+H3jv408d4jw/7Bttv5axS5IiHoLaVNHeQ==",
             "resolved": "https://registry.npmjs.org/postcss-value-parser/-/postcss-value-parser-4.2.0.tgz",
             "version": "4.2.0"
         },
@@ -2732,54 +2764,57 @@
                 "immutable": "^4.0.0",
                 "source-map-js": ">=0.6.2 <2.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=14.0.0"
             },
-            "integrity": "sha512-uUxNQ3zAHeAx5nRFskBnrWzDUJrrvpCPD5FNAoRvTi0WwremlheES3tg+56PaVtCs5QDRX5CBLxxKMDJMEa1WQ==",
-            "resolved": "https://registry.npmjs.org/sass/-/sass-1.70.0.tgz",
-            "version": "1.70.0"
+            "integrity": "sha512-Gpczt3WA56Ly0Mn8Sl21Vj94s1axi9hDIzDFn9Ph9x3C3p4nNyvsqJoQyVXKou6cBlfFWEgRW4rT8Tb4i3XnVA==",
+            "resolved": "https://registry.npmjs.org/sass/-/sass-1.72.0.tgz",
+            "version": "1.72.0"
         },
         "node_modules/sass-loader": {
             "dependencies": {
                 "neo-async": "^2.6.2"
             },
             "dev": true,
             "engines": {
-                "node": ">= 14.15.0"
+                "node": ">= 18.12.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-mt5YN2F1MOZr3d/wBRcZxeFgwgkH44wVc2zohO2YF6JiOMkiXe4BYRZpSu2sO1g71mo/j16txzUhsKZlqjVGzA==",
+            "integrity": "sha512-QX8AasDg75monlybel38BZ49JP5Z+uSKfKwF2rO7S74BywaRmGQMUBw9dtkS+ekyM/QnP+NOrRYq8ABMZ9G8jw==",
             "peerDependencies": {
-                "fibers": ">= 3.1.0",
+                "@rspack/core": "0.x || 1.x",
                 "node-sass": "^4.0.0 || ^5.0.0 || ^6.0.0 || ^7.0.0 || ^8.0.0 || ^9.0.0",
                 "sass": "^1.3.0",
                 "sass-embedded": "*",
                 "webpack": "^5.0.0"
             },
             "peerDependenciesMeta": {
-                "fibers": {
+                "@rspack/core": {
                     "optional": true
                 },
                 "node-sass": {
                     "optional": true
                 },
                 "sass": {
                     "optional": true
                 },
                 "sass-embedded": {
                     "optional": true
+                },
+                "webpack": {
+                    "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/sass-loader/-/sass-loader-13.3.3.tgz",
-            "version": "13.3.3"
+            "resolved": "https://registry.npmjs.org/sass-loader/-/sass-loader-14.1.1.tgz",
+            "version": "14.1.1"
         },
         "node_modules/schema-utils": {
             "dependencies": {
                 "@types/json-schema": "^7.0.9",
                 "ajv": "^8.9.0",
                 "ajv-formats": "^2.1.1",
                 "ajv-keywords": "^5.1.0"
@@ -2877,21 +2912,14 @@
                 "source-map": "^0.6.0"
             },
             "dev": true,
             "integrity": "sha512-uBHU3L3czsIyYXKX88fdrGovxdSCoTGDRZ6SYXtSRxLZUzHg5P/66Ht6uoUlHu9EZod+inXhKo3qQgwXUT/y1w==",
             "resolved": "https://registry.npmjs.org/source-map-support/-/source-map-support-0.5.21.tgz",
             "version": "0.5.21"
         },
-        "node_modules/stable": {
-            "deprecated": "Modern JS already guarantees Array#sort() is a stable sort, so this library is deprecated. See the compatibility table on MDN: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort#browser_compatibility",
-            "dev": true,
-            "integrity": "sha512-ji9qxRnOVfcuLDySj9qzhGSEFVobyt1kIOSkj1qZzYLzq7Tos/oUUWvotUPQLlrsidqsK6tBH89Bc9kL5zHA6w==",
-            "resolved": "https://registry.npmjs.org/stable/-/stable-0.1.8.tgz",
-            "version": "0.1.8"
-        },
         "node_modules/style-loader": {
             "dev": true,
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
@@ -2902,27 +2930,27 @@
                 "webpack": "^5.0.0"
             },
             "resolved": "https://registry.npmjs.org/style-loader/-/style-loader-3.3.4.tgz",
             "version": "3.3.4"
         },
         "node_modules/stylehacks": {
             "dependencies": {
-                "browserslist": "^4.21.4",
-                "postcss-selector-parser": "^6.0.4"
+                "browserslist": "^4.22.2",
+                "postcss-selector-parser": "^6.0.15"
             },
             "dev": true,
             "engines": {
-                "node": "^10 || ^12 || >=14.0"
+                "node": "^14 || ^16 || >=18.0"
             },
-            "integrity": "sha512-sBpcd5Hx7G6seo7b1LkpttvTz7ikD0LlH5RmdcBNb6fFR0Fl7LQwHDFr300q4cwUqi+IYrFGmsIHieMBfnN/Bw==",
+            "integrity": "sha512-00zvJGnCu64EpMjX8b5iCZ3us2Ptyw8+toEkb92VdmkEaRaSGBNKAoK6aWZckhXxmQP8zWiTaFaiMGIU8Ve8sg==",
             "peerDependencies": {
-                "postcss": "^8.2.15"
+                "postcss": "^8.4.31"
             },
-            "resolved": "https://registry.npmjs.org/stylehacks/-/stylehacks-5.1.1.tgz",
-            "version": "5.1.1"
+            "resolved": "https://registry.npmjs.org/stylehacks/-/stylehacks-6.0.2.tgz",
+            "version": "6.0.2"
         },
         "node_modules/supports-color": {
             "dependencies": {
                 "has-flag": "^4.0.0"
             },
             "dev": true,
             "engines": {
@@ -2950,27 +2978,31 @@
         "node_modules/svgo": {
             "bin": {
                 "svgo": "bin/svgo"
             },
             "dependencies": {
                 "@trysound/sax": "0.2.0",
                 "commander": "^7.2.0",
-                "css-select": "^4.1.3",
-                "css-tree": "^1.1.3",
-                "csso": "^4.2.0",
-                "picocolors": "^1.0.0",
-                "stable": "^0.1.8"
+                "css-select": "^5.1.0",
+                "css-tree": "^2.3.1",
+                "css-what": "^6.1.0",
+                "csso": "^5.0.5",
+                "picocolors": "^1.0.0"
             },
             "dev": true,
             "engines": {
-                "node": ">=10.13.0"
+                "node": ">=14.0.0"
             },
-            "integrity": "sha512-+N/Q9kV1+F+UeWYoSiULYo4xYSDQlTgb+ayMobAXPwMnLvop7oxKMo9OzIrX5x3eS4L4f2UHhc9axXwY8DpChg==",
-            "resolved": "https://registry.npmjs.org/svgo/-/svgo-2.8.0.tgz",
-            "version": "2.8.0"
+            "funding": {
+                "type": "opencollective",
+                "url": "https://opencollective.com/svgo"
+            },
+            "integrity": "sha512-4PP6CMW/V7l/GmKRKzsLR8xxjdHTV4IMvhTnpuHwwBazSIlw5W/5SmPjN8Dwyt7lKbSJrRDgp4t9ph0HgChFBQ==",
+            "resolved": "https://registry.npmjs.org/svgo/-/svgo-3.2.0.tgz",
+            "version": "3.2.0"
         },
         "node_modules/tapable": {
             "dev": true,
             "engines": {
                 "node": ">=6"
             },
             "integrity": "sha512-GNzQvQTOIP6RyTfE2Qxb8ZVlNmw0n88vp1szwWRimP02mnTsx3Wtn5qRdqY9w2XduFNUgvOwhNnQsjwCp+kqaQ==",
@@ -3166,64 +3198,64 @@
                 "glob-to-regexp": "^0.4.1",
                 "graceful-fs": "^4.1.2"
             },
             "dev": true,
             "engines": {
                 "node": ">=10.13.0"
             },
-            "integrity": "sha512-Lcvm7MGST/4fup+ifyKi2hjyIAwcdI4HRgtvTpIUxBRhB+RFtUh8XtDOxUfctVCnhVi+QQj49i91OyvzkJl6cg==",
-            "resolved": "https://registry.npmjs.org/watchpack/-/watchpack-2.4.0.tgz",
-            "version": "2.4.0"
+            "integrity": "sha512-8wrBCMtVhqcXP2Sup1ctSkga6uc2Bx0IIvKyT7yTFier5AXHooSI+QyQQAtTb7+E0IUCCKyTFmXqdqgum2XWGg==",
+            "resolved": "https://registry.npmjs.org/watchpack/-/watchpack-2.4.1.tgz",
+            "version": "2.4.1"
         },
         "node_modules/webpack": {
             "bin": {
                 "webpack": "bin/webpack.js"
             },
             "dependencies": {
                 "@types/eslint-scope": "^3.7.3",
                 "@types/estree": "^1.0.5",
-                "@webassemblyjs/ast": "^1.11.5",
-                "@webassemblyjs/wasm-edit": "^1.11.5",
-                "@webassemblyjs/wasm-parser": "^1.11.5",
+                "@webassemblyjs/ast": "^1.12.1",
+                "@webassemblyjs/wasm-edit": "^1.12.1",
+                "@webassemblyjs/wasm-parser": "^1.12.1",
                 "acorn": "^8.7.1",
                 "acorn-import-assertions": "^1.9.0",
                 "browserslist": "^4.21.10",
                 "chrome-trace-event": "^1.0.2",
-                "enhanced-resolve": "^5.15.0",
+                "enhanced-resolve": "^5.16.0",
                 "es-module-lexer": "^1.2.1",
                 "eslint-scope": "5.1.1",
                 "events": "^3.2.0",
                 "glob-to-regexp": "^0.4.1",
-                "graceful-fs": "^4.2.9",
+                "graceful-fs": "^4.2.11",
                 "json-parse-even-better-errors": "^2.3.1",
                 "loader-runner": "^4.2.0",
                 "mime-types": "^2.1.27",
                 "neo-async": "^2.6.2",
                 "schema-utils": "^3.2.0",
                 "tapable": "^2.1.1",
                 "terser-webpack-plugin": "^5.3.10",
-                "watchpack": "^2.4.0",
+                "watchpack": "^2.4.1",
                 "webpack-sources": "^3.2.3"
             },
             "dev": true,
             "engines": {
                 "node": ">=10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-bdmyXRCXeeNIePv6R6tGPyy20aUobw4Zy8r0LUS2EWO+U+Ke/gYDgsCh7bl5rB6jPpr4r0SZa6dPxBxLooDT3w==",
+            "integrity": "sha512-rzVwlLeBWHJbmgTC/8TvAcu5vpJNII+MelQpylD4jNERPwpBJOE2lEcko1zJX3QJeLjTTAnQxn/OJ8bjDzVQaw==",
             "peerDependenciesMeta": {
                 "webpack-cli": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.90.0.tgz",
-            "version": "5.90.0"
+            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.91.0.tgz",
+            "version": "5.91.0"
         },
         "node_modules/webpack-cli": {
             "bin": {
                 "webpack-cli": "bin/cli.js"
             },
             "dependencies": {
                 "@discoveryjs/json-ext": "^0.5.0",
@@ -3369,20 +3401,11 @@
             "version": "2.0.1"
         },
         "node_modules/yallist": {
             "dev": true,
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
-        },
-        "node_modules/yaml": {
-            "dev": true,
-            "engines": {
-                "node": ">= 6"
-            },
-            "integrity": "sha512-r3vXyErRCYJ7wg28yvBY5VSoAF8ZvlcW9/BwUzEtUsjvX/DKs24dIkuwjtuprwJJHsbyUbLApepYTR1BN4uHrg==",
-            "resolved": "https://registry.npmjs.org/yaml/-/yaml-1.10.2.tgz",
-            "version": "1.10.2"
         }
     },
     "requires": true
 }
```

### Comparing `furo-2024.1.29/pyproject.toml` & `furo-2024.4.27/pyproject.toml`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/__init__.py` & `furo-2024.4.27/src/furo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A clean customisable Sphinx documentation theme."""
 
-__version__ = "2024.01.29"
+__version__ = "2024.04.27"
 
 import hashlib
 import logging
 import os
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, Iterator, List, Optional, cast
@@ -279,15 +279,21 @@
     ), "there should be a default style known to Sphinx"
     assert (
         builder.dark_highlighter is None  # type: ignore[attr-defined]
     ), "this shouldn't be a dark style known to Sphinx"
     update_known_styles_state(app)
 
     def _update_default(key: str, *, new_default: Any) -> None:
-        app.config.values[key] = (new_default, *app.config.values[key][1:])
+        try:
+            conf_py_settings = app.config._raw_config
+        except AttributeError:
+            pass  # Sphinx's config has changed.
+        else:
+            if key not in conf_py_settings:
+                app.config._raw_config.setdefault(key, new_default)
 
     # Change the default permalinks icon
     _update_default("html_permalinks_icon", new_default="#")
 
 
 def update_known_styles_state(app: sphinx.application.Sphinx) -> None:
     """Update a global store of known styles of this application."""
```

### Comparing `furo-2024.1.29/src/furo/assets/scripts/furo.js` & `furo-2024.4.27/src/furo/assets/scripts/furo.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -137,15 +137,15 @@
     // Scrollspy -- highlight table on contents, based on scroll
     new Gumshoe(".toc-tree a", {
         reflow: true,
         recursive: true,
         navClass: "scroll-current",
         offset: () => {
             let rem = parseFloat(getComputedStyle(document.documentElement).fontSize);
-            return header.getBoundingClientRect().height + 0.5 * rem + 1;
+            return header.getBoundingClientRect().height + 2.5 * rem + 1;
         },
     });
 }
 
 function setupTheme() {
     // Attach event handlers for toggling themes
     const buttons = document.getElementsByClassName("theme-toggle");
```

### Comparing `furo-2024.1.29/src/furo/assets/scripts/gumshoe-patched.js` & `furo-2024.4.27/src/furo/assets/scripts/gumshoe-patched.js`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/assets/styles/_scaffold.sass` & `furo-2024.4.27/src/furo/assets/styles/_scaffold.sass`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,30 @@
 //
 html,
 body
   height: 100%
   color: var(--color-foreground-primary)
   background: var(--color-background-primary)
 
+.skip-to-content
+  position: fixed
+  padding: 1rem
+  border-radius: 1rem
+  left: 0.25rem
+  top: 0.25rem
+  z-index: 40
+  background: var(--color-background-primary)
+  color: var(--color-foreground-primary)
+
+  transform: translateY(-200%)
+  transition: transform 300ms ease-in-out
+
+  &:focus-within
+    transform: translateY(0%)
+
 article
   color: var(--color-content-foreground)
   background: var(--color-content-background)
   overflow-wrap: break-word
 
 .page
   display: flex
@@ -386,15 +402,15 @@
   .nav-overlay-icon .icon,
   .theme-toggle svg
     height: 1.25rem
     width: 1.25rem
 
   // Add a scroll margin for the content
   :target
-    scroll-margin-top: var(--header-height)
+    scroll-margin-top: calc(var(--header-height) + 2.5rem)
 
   // Show back-to-top below the header
   .back-to-top
     top: calc(var(--header-height) + 0.5rem)
 
   // Center the page, and accommodate for the header.
   .page
```

### Comparing `furo-2024.1.29/src/furo/assets/styles/base/_print.sass` & `furo-2024.4.27/src/furo/assets/styles/base/_print.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/assets/styles/base/_theme.sass` & `furo-2024.4.27/src/furo/assets/styles/base/_theme.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/assets/styles/components/_footer.sass` & `furo-2024.4.27/src/furo/assets/styles/components/_footer.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/assets/styles/components/_sidebar.sass` & `furo-2024.4.27/src/furo/assets/styles/components/_sidebar.sass`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,15 @@
 
     height: 100%
     width: 100%
 
     padding: var(--sidebar-item-spacing-vertical) var(--sidebar-item-spacing-horizontal)
 
     &:hover
+      color: var(--color-sidebar-link-text)
       background: var(--color-sidebar-item-background--hover)
 
     // Add a nice little "external-link" arrow here.
     &.external::after
       content: url('data:image/svg+xml,<svg width="12" height="12" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" stroke-width="1.5" stroke="%23607D8B" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z"/><path d="M11 7h-5a2 2 0 0 0 -2 2v9a2 2 0 0 0 2 2h9a2 2 0 0 0 2 -2v-5" /><line x1="10" y1="14" x2="20" y2="4" /><polyline points="15 4 20 4 20 9" /></svg>')
       margin: 0 0.25rem
       vertical-align: middle
```

### Comparing `furo-2024.1.29/src/furo/assets/styles/components/_table_of_contents.sass` & `furo-2024.4.27/src/furo/assets/styles/components/_table_of_contents.sass`

 * *Files 12% similar despite different names*

```diff
@@ -36,26 +36,26 @@
     list-style-type: none
     margin-top: 0
     margin-bottom: 0
     padding-left: var(--toc-item-spacing-horizontal)
   li
     padding-top: var(--toc-item-spacing-vertical)
 
-    &.scroll-current >.reference
+    &.scroll-current > .reference
       color: var(--color-toc-item-text--active)
       font-weight: bold
 
-  .reference
+  a.reference
     color: var(--color-toc-item-text)
     text-decoration: none
     overflow-wrap: anywhere
 
 .toc-scroll
   max-height: 100vh
   overflow-y: scroll
 
 // Be very annoying when someone includes the table of contents
 .contents:not(.this-will-duplicate-information-and-it-is-still-useful-here)
   color: var(--color-problematic)
   background: rgba(255, 0, 0, 0.25)
   &::before
-    content: "ERROR: Adding a table of contents in Furo-based documentation is unnecessary, and does not work well with existing styling.Add a 'this-will-duplicate-information-and-it-is-still-useful-here' class, if you want an escape hatch."
+    content: "ERROR: Adding a table of contents in Furo-based documentation is unnecessary, and does not work well with existing styling. Add a 'this-will-duplicate-information-and-it-is-still-useful-here' class, if you want an escape hatch."
```

### Comparing `furo-2024.1.29/src/furo/assets/styles/content/_admonitions.sass` & `furo-2024.4.27/src/furo/assets/styles/content/_admonitions.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/assets/styles/content/_api.sass` & `furo-2024.4.27/src/furo/assets/styles/content/_api.sass`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
   &:hover
     background: var(--color-api-background-hover)
 
   // adjust the size of the [source] link on the right.
   a.reference
     .viewcode-link
       font-weight: normal
-      width: 3.5rem
+      width: 4.25rem
 
 em.property
   font-style: normal
   &:first-child
     color: var(--color-api-keyword)
 .sig-name
   color: var(--color-api-name)
```

### Comparing `furo-2024.1.29/src/furo/assets/styles/content/_code.sass` & `furo-2024.4.27/src/furo/assets/styles/content/_code.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/assets/styles/content/_footnotes.sass` & `furo-2024.4.27/src/furo/assets/styles/content/_footnotes.sass`

 * *Files 13% similar despite different names*

```diff
@@ -36,10 +36,10 @@
 
 aside.footnote > span,
 div.citation > span
   float: left
   font-weight: 500
   padding-right: 0.25rem
 
-aside.footnote > p,
+aside.footnote > *:not(span),
 div.citation > p
   margin-left: 2rem
```

### Comparing `furo-2024.1.29/src/furo/assets/styles/content/_images.sass` & `furo-2024.4.27/src/furo/assets/styles/content/_images.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/assets/styles/content/_lists.sass` & `furo-2024.4.27/src/furo/assets/styles/content/_lists.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/assets/styles/content/_misc.sass` & `furo-2024.4.27/src/furo/assets/styles/content/_misc.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/assets/styles/content/_sidebar.sass` & `furo-2024.4.27/src/furo/assets/styles/content/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/assets/styles/content/_tables.sass` & `furo-2024.4.27/src/furo/assets/styles/content/_tables.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/assets/styles/content/_target.sass` & `furo-2024.4.27/src/furo/assets/styles/content/_target.sass`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 :target
-  scroll-margin-top: 0.5rem
+  scroll-margin-top: 2.5rem
 
 @media (max-width: $full-width - $sidebar-width)
   :target
-    scroll-margin-top: calc(0.5rem + var(--header-height))
+    scroll-margin-top: calc(2.5rem + var(--header-height))
 
   // When a heading is selected
   section > span:target
-    scroll-margin-top: calc(0.8rem + var(--header-height))
+    scroll-margin-top: calc(2.8rem + var(--header-height))
 
 // Permalinks
 .headerlink
   font-weight: 100
   user-select: none
 
 h1,
```

### Comparing `furo-2024.1.29/src/furo/assets/styles/extensions/_copybutton.sass` & `furo-2024.4.27/src/furo/assets/styles/extensions/_copybutton.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/assets/styles/extensions/_readthedocs.sass` & `furo-2024.4.27/src/furo/assets/styles/extensions/_readthedocs.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/assets/styles/extensions/_sphinx-design.sass` & `furo-2024.4.27/src/furo/assets/styles/extensions/_sphinx-design.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/assets/styles/extensions/_sphinx-inline-tabs.sass` & `furo-2024.4.27/src/furo/assets/styles/extensions/_sphinx-inline-tabs.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/assets/styles/extensions/_sphinx-panels.sass` & `furo-2024.4.27/src/furo/assets/styles/extensions/_sphinx-panels.sass`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/assets/styles/variables/_admonitions.scss` & `furo-2024.4.27/src/furo/assets/styles/variables/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/assets/styles/variables/_colors.scss` & `furo-2024.4.27/src/furo/assets/styles/variables/_colors.scss`

 * *Files 2% similar despite different names*

```diff
@@ -8,31 +8,32 @@
 
 @mixin colors {
   --color-problematic: #b30000;
 
   // Base Colors
   --color-foreground-primary: black; // for main text and headings
   --color-foreground-secondary: #5a5c63; // for secondary text
-  --color-foreground-muted: #646776; // for muted text
+  --color-foreground-muted: #6b6f76; // for muted text
   --color-foreground-border: #878787; // for content borders
 
   --color-background-primary: white; // for content
   --color-background-secondary: #f8f9fb; // for navigation + ToC
   --color-background-hover: #efeff4ff; // for navigation-item hover
   --color-background-hover--transparent: #efeff400;
   --color-background-border: #eeebee; // for UI borders
   --color-background-item: #ccc; // for "background" items (eg: copybutton)
 
   // Announcements
   --color-announcement-background: #000000dd;
   --color-announcement-text: #eeebee;
 
   // Brand colors
-  --color-brand-primary: #2962ff;
-  --color-brand-content: #2a5adf;
+  --color-brand-primary: #0a4bff;
+  --color-brand-content: #2757dd;
+  --color-brand-visited: #872ee0;
 
   // API documentation
   --color-api-background: var(--color-background-hover--transparent);
   --color-api-background-hover: var(--color-background-hover);
   --color-api-overall: var(--color-foreground-secondary);
   --color-api-name: var(--color-problematic);
   --color-api-pre-name: var(--color-problematic);
@@ -116,24 +117,29 @@
 
   // Actual page contents
   --color-content-foreground: var(--color-foreground-primary);
   --color-content-background: transparent;
 
   // Links
   --color-link: var(--color-brand-content);
-  --color-link--hover: var(--color-brand-content);
   --color-link-underline: var(--color-background-border);
+  --color-link--hover: var(--color-brand-content);
   --color-link-underline--hover: var(--color-foreground-border);
+
+  --color-link--visited: var(--color-brand-visited);
+  --color-link-underline--visited: var(--color-background-border);
+  --color-link--visited--hover: var(--color-brand-visited);
+  --color-link-underline--visited--hover: var(--color-foreground-border);
 }
 
 @mixin colors-dark {
   --color-problematic: #ee5151;
 
   // Base Colors
-  --color-foreground-primary: #ffffffcc; // for main text and headings
+  --color-foreground-primary: #cfd0d0; // for main text and headings
   --color-foreground-secondary: #9ca0a5; // for secondary text
   --color-foreground-muted: #81868d; // for muted text
   --color-foreground-border: #666666; // for content borders
 
   --color-background-primary: #131416; // for content
   --color-background-secondary: #1a1c1e; // for navigation + ToC
   --color-background-hover: #1e2124ff; // for navigation-item hover
@@ -142,16 +148,17 @@
   --color-background-item: #444; // for "background" items (eg: copybutton)
 
   // Announcements
   --color-announcement-background: #000000dd;
   --color-announcement-text: #eeebee;
 
   // Brand colors
-  --color-brand-primary: #2b8cee;
-  --color-brand-content: #368ce2;
+  --color-brand-primary: #3d94ff;
+  --color-brand-content: #5ca5ff;
+  --color-brand-visited: #b27aeb;
 
   // Highlighted text (search)
   --color-highlighted-background: #083563;
 
   // GUI Labels
   --color-guilabel-background: #08356380;
   --color-guilabel-border: #13395f80;
```

### Comparing `furo-2024.1.29/src/furo/assets/styles/variables/_fonts.scss` & `furo-2024.4.27/src/furo/assets/styles/variables/_fonts.scss`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 @mixin fonts {
   // These are adapted from https://systemfontstack.com/
   --font-stack: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial,
     sans-serif, Apple Color Emoji, Segoe UI Emoji;
   --font-stack--monospace: "SFMono-Regular", Menlo, Consolas, Monaco,
     Liberation Mono, Lucida Console, monospace;
+  --font-stack--headings: var(--font-stack);
 
   --font-size--normal: 100%;
   --font-size--small: 87.5%;
   --font-size--small--2: 81.25%;
   --font-size--small--3: 75%;
   --font-size--small--4: 62.5%;
```

### Comparing `furo-2024.1.29/src/furo/assets/styles/variables/_icons.scss` & `furo-2024.4.27/src/furo/assets/styles/variables/_icons.scss`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/assets/styles/variables/_spacing.scss` & `furo-2024.4.27/src/furo/assets/styles/variables/_spacing.scss`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/navigation.py` & `furo-2024.4.27/src/furo/navigation.py`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/sphinxext.py` & `furo-2024.4.27/src/furo/sphinxext.py`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/theme/furo/base.html` & `furo-2024.4.27/src/furo/theme/furo/base.html`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/theme/furo/components/edit-this-page.html` & `furo-2024.4.27/src/furo/theme/furo/components/edit-this-page.html`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/theme/furo/domainindex.html` & `furo-2024.4.27/src/furo/theme/furo/domainindex.html`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/theme/furo/genindex.html` & `furo-2024.4.27/src/furo/theme/furo/genindex.html`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/theme/furo/page.html` & `furo-2024.4.27/src/furo/theme/furo/page.html`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 <label class="overlay sidebar-overlay" for="__navigation">
   <div class="visually-hidden">Hide navigation sidebar</div>
 </label>
 <label class="overlay toc-overlay" for="__toc">
   <div class="visually-hidden">Hide table of contents sidebar</div>
 </label>
 
+<a class="skip-to-content muted-link" href="#furo-main-content">
+  {%- trans -%}
+  Skip to content
+  {%- endtrans -%}
+</a>
+
 {% if theme_announcement -%}
 <div class="announcement">
   <aside class="announcement-content">
     {% block announcement %} {{ theme_announcement }} {% endblock announcement %}
   </aside>
 </div>
 {%- endif %}
@@ -83,15 +89,15 @@
             </button>
           </div>
           <label class="toc-overlay-icon toc-content-icon{% if furo_hide_toc %} no-toc{% endif %}" for="__toc">
             <div class="visually-hidden">Toggle table of contents sidebar</div>
             <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
           </label>
         </div>
-        <article role="main">
+        <article role="main" id="furo-main-content">
           {% block content %}{{ body }}{% endblock %}
         </article>
       </div>
       <footer>
         {% block footer %}
         <div class="related-pages">
           {% if next -%}
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% extends "base.html" %} {% block body -%} {{ super() }} {% include "partials/
 icons.html" %}????
 Hide navigation sidebar
 Hide table of contents sidebar
-{% if theme_announcement -%}
+_{_%_-_ _t_r_a_n_s_ _-_%_}_ _S_k_i_p_ _t_o_ _c_o_n_t_e_n_t_ _{_%_-_ _e_n_d_t_r_a_n_s_ _-_%_}_ {% if theme_announcement -%}
 {% block announcement %} {{ theme_announcement }} {% endblock announcement %}
 {%- endif %}
 Toggle site navigation sidebar
 _{_{_ _d_o_c_s_t_i_t_l_e_ _i_f_ _d_o_c_s_t_i_t_l_e_ _e_l_s_e_ _p_r_o_j_e_c_t_ _}_}
 Toggle Light / Dark / Auto color theme
 Toggle table of contents sidebar
 {% block left_sidebar %}
```

### Comparing `furo-2024.1.29/src/furo/theme/furo/partials/_head_css_variables.html` & `furo-2024.4.27/src/furo/theme/furo/partials/_head_css_variables.html`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/theme/furo/partials/icons.html` & `furo-2024.4.27/src/furo/theme/furo/partials/icons.html`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/theme/furo/search.html` & `furo-2024.4.27/src/furo/theme/furo/search.html`

 * *Files 14% similar despite different names*

```diff
@@ -23,7 +23,12 @@
 <div id="search-results"></div>
 {% endblock %}
 
 {% block scripts -%}
 {{ super() }}
 <script src="{{ pathto('searchindex.js', 1) }}"></script>
 {%- endblock scripts %}
+
+{% block site_meta %}
+{{ super() }}
+<meta name="robots" content="noindex" />
+{% endblock site_meta %}
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
 {% extends "page.html" %} {%- block regular_scripts -%} {{ super() }}
 {%- endblock regular_scripts-%} {%- block htmltitle -%}
 {%- endblock htmltitle -%} {% block content %}
 {% trans %}Error{% endtrans %}
 {% trans %}Please activate JavaScript to enable the search functionality.{%
 endtrans %}
 {% endblock %} {% block scripts -%} {{ super() }}
-{%- endblock scripts %}
+{%- endblock scripts %} {% block site_meta %} {{ super() }}
+{% endblock site_meta %}
```

### Comparing `furo-2024.1.29/src/furo/theme/furo/sidebar/brand.html` & `furo-2024.4.27/src/furo/theme/furo/sidebar/brand.html`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/theme/furo/sidebar/rtd-versions.html` & `furo-2024.4.27/src/furo/theme/furo/sidebar/rtd-versions.html`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/theme/furo/sidebar/variant-selector.html` & `furo-2024.4.27/src/furo/theme/furo/sidebar/variant-selector.html`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/src/furo/theme/furo/theme.conf` & `furo-2024.4.27/src/furo/theme/furo/theme.conf`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/tests/workflow/test_sphinx_versions.py` & `furo-2024.4.27/tests/workflow/test_sphinx_versions.py`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/webpack.config.js` & `furo-2024.4.27/webpack.config.js`

 * *Files identical despite different names*

### Comparing `furo-2024.1.29/PKG-INFO` & `furo-2024.4.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furo
-Version: 2024.1.29
+Version: 2024.4.27
 Summary: A clean customisable Sphinx documentation theme.
 Author-Email: Pradyun Gedam <mail@pradyunsg.me>
 License: Copyright (c) 2020 Pradyun Gedam <mail@pradyunsg.me>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to
         deal in the Software without restriction, including without limitation the
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: furo Version: 2024.1.29 Summary: A clean
+Metadata-Version: 2.1 Name: furo Version: 2024.4.27 Summary: A clean
 customisable Sphinx documentation theme. Author-Email: Pradyun Gedam
 pradyunsg.me> License: Copyright (c) 2020 Pradyun Gedam
 pradyunsg.me> Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
```

