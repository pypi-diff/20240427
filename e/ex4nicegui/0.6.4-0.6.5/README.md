# Comparing `tmp/ex4nicegui-0.6.4.tar.gz` & `tmp/ex4nicegui-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex4nicegui-0.6.4.tar", last modified: Thu Mar 21 07:52:38 2024, max compression
+gzip compressed data, was "ex4nicegui-0.6.5.tar", last modified: Sat Apr 27 11:46:49 2024, max compression
```

## Comparing `ex4nicegui-0.6.4.tar` & `ex4nicegui-0.6.5.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.931112 ex4nicegui-0.6.4/
--rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.6.4/LICENSE
--rw-rw-rw-   0        0        0    27491 2024-03-21 07:52:38.931112 ex4nicegui-0.6.4/PKG-INFO
--rw-rw-rw-   0        0        0    25989 2024-03-05 13:06:09.000000 ex4nicegui-0.6.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.238753 ex4nicegui-0.6.4/ex4nicegui/
--rw-rw-rw-   0        0        0      818 2024-03-21 07:52:03.000000 ex4nicegui-0.6.4/ex4nicegui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.260523 ex4nicegui-0.6.4/ex4nicegui/bi/
--rw-rw-rw-   0        0        0      315 2023-10-18 15:44:54.000000 ex4nicegui-0.6.4/ex4nicegui/bi/__init__.py
--rw-rw-rw-   0        0        0     7691 2024-02-21 17:06:50.000000 ex4nicegui-0.6.4/ex4nicegui/bi/dataSource.py
--rw-rw-rw-   0        0        0     8186 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/bi/dataSourceFacade.py
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.294531 ex4nicegui-0.6.4/ex4nicegui/bi/elements/
--rw-rw-rw-   0        0        0        0 2023-10-18 15:44:54.000000 ex4nicegui-0.6.4/ex4nicegui/bi/elements/__init__.py
--rw-rw-rw-   0        0        0      358 2023-10-18 15:44:54.000000 ex4nicegui-0.6.4/ex4nicegui/bi/elements/containers.py
--rw-rw-rw-   0        0        0      898 2023-10-18 15:44:54.000000 ex4nicegui-0.6.4/ex4nicegui/bi/elements/layouts.py
--rw-rw-rw-   0        0        0     1534 2023-12-04 18:30:56.000000 ex4nicegui-0.6.4/ex4nicegui/bi/elements/models.py
--rw-rw-rw-   0        0        0      808 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/bi/elements/text.py
--rw-rw-rw-   0        0        0     2009 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/bi/elements/ui_aggrid.py
--rw-rw-rw-   0        0        0      852 2023-10-18 15:44:54.000000 ex4nicegui-0.6.4/ex4nicegui/bi/elements/ui_date_picker.js
--rw-rw-rw-   0        0        0     2260 2023-12-06 09:33:56.000000 ex4nicegui-0.6.4/ex4nicegui/bi/elements/ui_date_picker.py
--rw-rw-rw-   0        0        0     2302 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/bi/elements/ui_echarts.py
--rw-rw-rw-   0        0        0     5447 2023-12-06 09:33:56.000000 ex4nicegui-0.6.4/ex4nicegui/bi/elements/ui_radio.py
--rw-rw-rw-   0        0        0     4128 2023-12-06 09:33:56.000000 ex4nicegui-0.6.4/ex4nicegui/bi/elements/ui_range.py
--rw-rw-rw-   0        0        0     3872 2023-12-08 12:43:57.000000 ex4nicegui-0.6.4/ex4nicegui/bi/elements/ui_select.py
--rw-rw-rw-   0        0        0     2165 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/bi/elements/ui_slider.py
--rw-rw-rw-   0        0        0     1810 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/bi/elements/ui_table.py
--rw-rw-rw-   0        0        0     2067 2024-01-07 17:28:53.000000 ex4nicegui-0.6.4/ex4nicegui/bi/index.py
--rw-rw-rw-   0        0        0     4529 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/bi/protocols.py
--rw-rw-rw-   0        0        0      355 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/bi/types.py
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.299395 ex4nicegui-0.6.4/ex4nicegui/experimental_/
--rw-rw-rw-   0        0        0       69 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/experimental_/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.303377 ex4nicegui-0.6.4/ex4nicegui/experimental_/gridLayout/
--rw-rw-rw-   0        0        0      125 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/experimental_/gridLayout/__init__.py
--rw-rw-rw-   0        0        0     4737 2023-10-18 15:44:54.000000 ex4nicegui-0.6.4/ex4nicegui/experimental_/gridLayout/index.py
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.325286 ex4nicegui-0.6.4/ex4nicegui/gsap/
--rw-rw-rw-   0        0        0      218 2024-02-27 20:13:02.000000 ex4nicegui-0.6.4/ex4nicegui/gsap/__init__.py
--rw-rw-rw-   0        0        0     4675 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/gsap/gsap.py
--rw-rw-rw-   0        0        0     1241 2024-02-27 20:13:02.000000 ex4nicegui-0.6.4/ex4nicegui/gsap/timeline.js
--rw-rw-rw-   0        0        0     2421 2024-02-27 20:13:02.000000 ex4nicegui-0.6.4/ex4nicegui/gsap/timeline.py
--rw-rw-rw-   0        0        0     1045 2024-02-02 15:27:35.000000 ex4nicegui-0.6.4/ex4nicegui/gsap/wrapGsap.js
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.336252 ex4nicegui-0.6.4/ex4nicegui/layout/
--rw-rw-rw-   0        0        0      278 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/layout/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.370410 ex4nicegui-0.6.4/ex4nicegui/layout/gridFlex/
--rw-rw-rw-   0        0        0     4468 2023-10-18 15:44:54.000000 ex4nicegui-0.6.4/ex4nicegui/layout/gridFlex/GridFlex.js
--rw-rw-rw-   0        0        0        2 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/layout/gridFlex/__init__.py
--rw-rw-rw-   0        0        0     7194 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/layout/gridFlex/gridFlex.py
--rw-rw-rw-   0        0        0     1236 2023-10-18 15:44:54.000000 ex4nicegui-0.6.4/ex4nicegui/layout/gridFlex/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.379934 ex4nicegui-0.6.4/ex4nicegui/layout/rxFlex/
--rw-rw-rw-   0        0        0        0 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/layout/rxFlex/__init__.py
--rw-rw-rw-   0        0        0     3672 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/layout/rxFlex/index.py
--rw-rw-rw-   0        0        0     1411 2023-10-18 15:44:54.000000 ex4nicegui-0.6.4/ex4nicegui/layout/rxFlex/types.py
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.379934 ex4nicegui-0.6.4/ex4nicegui/libs/
--rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.506974 ex4nicegui-0.6.4/ex4nicegui/libs/d3/
--rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/d3/__init__.py
--rw-rw-rw-   0        0        0    12795 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/d3/d3-color.ems.js
--rw-rw-rw-   0        0        0     2148 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/d3/d3-dispatch.ems.js
--rw-rw-rw-   0        0        0     4822 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/d3/d3-drag.ems.js
--rw-rw-rw-   0        0        0     3883 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/d3/d3-ease.ems.js
--rw-rw-rw-   0        0        0     9903 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/d3/d3-interpolate.ems.js
--rw-rw-rw-   0        0        0    16007 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/d3/d3-selection.ems.js
--rw-rw-rw-   0        0        0     2320 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/d3/d3-timer.ems.js
--rw-rw-rw-   0        0        0    14024 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/d3/d3-transition.ems.js
--rw-rw-rw-   0        0        0    11599 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/d3/d3-zoom.ems.js
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.669643 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/
--rw-rw-rw-   0        0        0    64907 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/CSSPlugin.js
--rw-rw-rw-   0        0        0     3674 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/CSSRulePlugin.js
--rw-rw-rw-   0        0        0    11588 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/CustomEase.js
--rw-rw-rw-   0        0        0   103102 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/Draggable.js
--rw-rw-rw-   0        0        0     5530 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/EasePack.js
--rw-rw-rw-   0        0        0     9125 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/EaselPlugin.js
--rw-rw-rw-   0        0        0    48981 2024-03-07 20:18:40.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/Flip.js
--rw-rw-rw-   0        0        0    12852 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/MotionPathPlugin.js
--rw-rw-rw-   0        0        0    26112 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/Observer.js
--rw-rw-rw-   0        0        0    15404 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/PixiPlugin.js
--rw-rw-rw-   0        0        0     9217 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/ScrollToPlugin.js
--rw-rw-rw-   0        0        0   112584 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/ScrollTrigger.js
--rw-rw-rw-   0        0        0     4877 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/TextPlugin.js
--rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/__init__.py
--rw-rw-rw-   0        0        0     1585 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/all.js
--rw-rw-rw-   0        0        0   175009 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/gsap-core.js
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.711924 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/utils/
--rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/utils/__init__.py
--rw-rw-rw-   0        0        0    15235 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/utils/matrix.js
--rw-rw-rw-   0        0        0    49314 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/utils/paths.js
--rw-rw-rw-   0        0        0    10472 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/libs/gsap/utils/strings.js
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.754994 ex4nicegui-0.6.4/ex4nicegui/reactive/
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.776485 ex4nicegui-0.6.4/ex4nicegui/reactive/EChartsComponent/
--rw-rw-rw-   0        0        0     3326 2024-02-04 23:34:45.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/EChartsComponent/ECharts.js
--rw-rw-rw-   0        0        0     6344 2024-02-04 23:34:45.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/EChartsComponent/ECharts.py
--rw-rw-rw-   0        0        0        0 2023-07-31 07:50:52.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/EChartsComponent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.791858 ex4nicegui-0.6.4/ex4nicegui/reactive/UseDraggable/
--rw-rw-rw-   0        0        0     5473 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/UseDraggable/UseDraggable.js
--rw-rw-rw-   0        0        0     3929 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/UseDraggable/UseDraggable.py
--rw-rw-rw-   0        0        0        0 2023-07-17 16:36:22.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/UseDraggable/__init__.py
--rw-rw-rw-   0        0        0     3714 2024-03-19 12:59:58.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.804765 ex4nicegui-0.6.4/ex4nicegui/reactive/dropZone/
--rw-rw-rw-   0        0        0        0 2023-07-31 07:45:08.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/dropZone/__init__.py
--rw-rw-rw-   0        0        0     2713 2023-07-29 10:16:25.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/dropZone/dropZone.js
--rw-rw-rw-   0        0        0     2590 2023-10-18 15:44:54.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/dropZone/dropZone.py
--rw-rw-rw-   0        0        0       50 2024-03-15 09:54:53.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/empty.js
--rw-rw-rw-   0        0        0      132 2024-03-15 09:54:53.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/empty.py
--rw-rw-rw-   0        0        0     1472 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/fileWatcher.py
--rw-rw-rw-   0        0        0     6225 2024-03-05 13:06:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/local_file_picker.py
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.821623 ex4nicegui-0.6.4/ex4nicegui/reactive/mermaid/
--rw-rw-rw-   0        0        0        0 2023-10-23 17:41:12.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/mermaid/__init__.py
--rw-rw-rw-   0        0        0     2308 2023-10-29 08:33:17.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/mermaid/mermaid.js
--rw-rw-rw-   0        0        0     2144 2024-02-05 16:01:34.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/mermaid/mermaid.py
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.898331 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/
--rw-rw-rw-   0        0        0        2 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/__init__.py
--rw-rw-rw-   0        0        0     2929 2024-03-07 20:18:40.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/aggrid.py
--rw-rw-rw-   0        0        0    10440 2024-03-15 09:54:52.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/base.py
--rw-rw-rw-   0        0        0     1660 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/button.py
--rw-rw-rw-   0        0        0     1275 2023-07-21 14:29:40.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/card.py
--rw-rw-rw-   0        0        0     1562 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/checkbox.py
--rw-rw-rw-   0        0        0     1787 2024-02-29 13:12:44.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/circular_progress.py
--rw-rw-rw-   0        0        0     3402 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/color_picker.py
--rw-rw-rw-   0        0        0     1040 2024-02-29 12:25:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/column.py
--rw-rw-rw-   0        0        0     2681 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/date.py
--rw-rw-rw-   0        0        0     2370 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/drawer.py
--rw-rw-rw-   0        0        0     9696 2024-03-21 07:26:57.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/echarts.py
--rw-rw-rw-   0        0        0      412 2024-03-19 12:59:58.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/element.py
--rw-rw-rw-   0        0        0     1873 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/expansion.py
--rw-rw-rw-   0        0        0      865 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/grid.py
--rw-rw-rw-   0        0        0      119 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/html.js
--rw-rw-rw-   0        0        0      675 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/html.py
--rw-rw-rw-   0        0        0     1559 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/icon.py
--rw-rw-rw-   0        0        0     1120 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/image.py
--rw-rw-rw-   0        0        0     4030 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/input.py
--rw-rw-rw-   0        0        0     2153 2024-02-29 11:46:48.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/knob.py
--rw-rw-rw-   0        0        0     1398 2024-03-04 19:14:43.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/label.py
--rw-rw-rw-   0        0        0     2128 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/linear_progress.py
--rw-rw-rw-   0        0        0     2201 2024-02-29 13:12:44.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/number.py
--rw-rw-rw-   0        0        0     1929 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/radio.py
--rw-rw-rw-   0        0        0     1029 2024-02-29 12:25:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/row.py
--rw-rw-rw-   0        0        0     2980 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/select.py
--rw-rw-rw-   0        0        0     2954 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/slider.py
--rw-rw-rw-   0        0        0     1605 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/switch.py
--rw-rw-rw-   0        0        0     1796 2024-03-15 09:54:52.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/tab.py
--rw-rw-rw-   0        0        0      630 2024-03-15 09:54:52.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/tab_panel.py
--rw-rw-rw-   0        0        0     1375 2024-03-15 09:54:52.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/tab_panels.py
--rw-rw-rw-   0        0        0     6042 2024-03-15 09:54:52.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/table.py
--rw-rw-rw-   0        0        0     1232 2024-03-15 09:54:52.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/tabs.py
--rw-rw-rw-   0        0        0     3044 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/textarea.py
--rw-rw-rw-   0        0        0     2360 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/upload.py
--rw-rw-rw-   0        0        0      213 2024-02-21 13:27:29.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/officials/utils.py
--rw-rw-rw-   0        0        0     1505 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/q_pagination.py
--rw-rw-rw-   0        0        0       31 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/rxui.py
--rw-rw-rw-   0        0        0      898 2024-03-15 09:54:53.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/transitionGroup.js
--rw-rw-rw-   0        0        0      597 2024-03-15 09:54:53.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/transitionGroup.py
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.910262 ex4nicegui-0.6.4/ex4nicegui/reactive/useMouse/
--rw-rw-rw-   0        0        0     2722 2023-07-17 15:14:14.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/useMouse/UseMouse.js
--rw-rw-rw-   0        0        0     2122 2024-02-23 16:33:09.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/useMouse/UseMouse.py
--rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/useMouse/__init__.py
--rw-rw-rw-   0        0        0     2598 2024-03-07 10:39:11.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/usePagination.py
--rw-rw-rw-   0        0        0     4360 2024-03-07 20:18:40.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/utils.py
--rw-rw-rw-   0        0        0      282 2024-03-15 09:54:53.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/vfor.js
--rw-rw-rw-   0        0        0     5786 2024-03-15 10:50:26.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/vfor.py
--rw-rw-rw-   0        0        0     5091 2024-03-05 13:12:27.000000 ex4nicegui-0.6.4/ex4nicegui/reactive/vmodel.py
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.913680 ex4nicegui-0.6.4/ex4nicegui/tools/
--rw-rw-rw-   0        0        0        0 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/tools/__init__.py
--rw-rw-rw-   0        0        0     4868 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/tools/debug.py
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.927116 ex4nicegui-0.6.4/ex4nicegui/utils/
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.6.4/ex4nicegui/utils/__init__.py
--rw-rw-rw-   0        0        0     2527 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/utils/apiEffect.py
--rw-rw-rw-   0        0        0     1505 2024-03-05 13:06:09.000000 ex4nicegui-0.6.4/ex4nicegui/utils/asyncComputed.py
--rw-rw-rw-   0        0        0     1225 2024-02-27 19:38:02.000000 ex4nicegui-0.6.4/ex4nicegui/utils/clientScope.py
--rw-rw-rw-   0        0        0      994 2024-02-20 10:06:17.000000 ex4nicegui-0.6.4/ex4nicegui/utils/common.py
--rw-rw-rw-   0        0        0     2310 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/utils/effect.py
--rw-rw-rw-   0        0        0     1218 2024-02-27 19:00:38.000000 ex4nicegui-0.6.4/ex4nicegui/utils/scheduler.py
--rw-rw-rw-   0        0        0    11346 2024-03-21 07:28:05.000000 ex4nicegui-0.6.4/ex4nicegui/utils/signals.py
-drwxrwxrwx   0        0        0        0 2024-03-21 07:52:38.249096 ex4nicegui-0.6.4/ex4nicegui.egg-info/
--rw-rw-rw-   0        0        0    27491 2024-03-21 07:52:37.000000 ex4nicegui-0.6.4/ex4nicegui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5460 2024-03-21 07:52:37.000000 ex4nicegui-0.6.4/ex4nicegui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 07:52:37.000000 ex4nicegui-0.6.4/ex4nicegui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-21 07:52:37.000000 ex4nicegui-0.6.4/ex4nicegui.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       57 2024-03-21 07:52:37.000000 ex4nicegui-0.6.4/ex4nicegui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-21 07:52:37.000000 ex4nicegui-0.6.4/ex4nicegui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-21 07:52:38.932608 ex4nicegui-0.6.4/setup.cfg
--rw-rw-rw-   0        0        0     1575 2024-03-15 11:10:09.000000 ex4nicegui-0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.941689 ex4nicegui-0.6.5/
+-rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.6.5/LICENSE
+-rw-rw-rw-   0        0        0    27491 2024-04-27 11:46:49.941689 ex4nicegui-0.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0    25989 2024-03-05 13:06:09.000000 ex4nicegui-0.6.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.088757 ex4nicegui-0.6.5/ex4nicegui/
+-rw-rw-rw-   0        0        0      818 2024-04-27 11:46:30.000000 ex4nicegui-0.6.5/ex4nicegui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.123763 ex4nicegui-0.6.5/ex4nicegui/bi/
+-rw-rw-rw-   0        0        0      315 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/bi/__init__.py
+-rw-rw-rw-   0        0        0     7644 2024-04-26 16:54:25.000000 ex4nicegui-0.6.5/ex4nicegui/bi/dataSource.py
+-rw-rw-rw-   0        0        0     8186 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/bi/dataSourceFacade.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.179173 ex4nicegui-0.6.5/ex4nicegui/bi/elements/
+-rw-rw-rw-   0        0        0        0 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/__init__.py
+-rw-rw-rw-   0        0        0      358 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/containers.py
+-rw-rw-rw-   0        0        0      898 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/layouts.py
+-rw-rw-rw-   0        0        0     1534 2023-12-04 18:30:56.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/models.py
+-rw-rw-rw-   0        0        0      808 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/text.py
+-rw-rw-rw-   0        0        0     2009 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_aggrid.py
+-rw-rw-rw-   0        0        0      852 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_date_picker.js
+-rw-rw-rw-   0        0        0     2260 2023-12-06 09:33:56.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_date_picker.py
+-rw-rw-rw-   0        0        0     2302 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_echarts.py
+-rw-rw-rw-   0        0        0     5447 2023-12-06 09:33:56.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_radio.py
+-rw-rw-rw-   0        0        0     4128 2023-12-06 09:33:56.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_range.py
+-rw-rw-rw-   0        0        0     3872 2023-12-08 12:43:57.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_select.py
+-rw-rw-rw-   0        0        0     2165 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_slider.py
+-rw-rw-rw-   0        0        0     1810 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_table.py
+-rw-rw-rw-   0        0        0     2067 2024-01-07 17:28:53.000000 ex4nicegui-0.6.5/ex4nicegui/bi/index.py
+-rw-rw-rw-   0        0        0     4529 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/bi/protocols.py
+-rw-rw-rw-   0        0        0      355 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/bi/types.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.182931 ex4nicegui-0.6.5/ex4nicegui/experimental_/
+-rw-rw-rw-   0        0        0       69 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/experimental_/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.201132 ex4nicegui-0.6.5/ex4nicegui/experimental_/gridLayout/
+-rw-rw-rw-   0        0        0      125 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/experimental_/gridLayout/__init__.py
+-rw-rw-rw-   0        0        0     4737 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/experimental_/gridLayout/index.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.226755 ex4nicegui-0.6.5/ex4nicegui/gsap/
+-rw-rw-rw-   0        0        0      218 2024-02-27 20:13:02.000000 ex4nicegui-0.6.5/ex4nicegui/gsap/__init__.py
+-rw-rw-rw-   0        0        0     4638 2024-04-26 16:54:25.000000 ex4nicegui-0.6.5/ex4nicegui/gsap/gsap.py
+-rw-rw-rw-   0        0        0     1241 2024-02-27 20:13:02.000000 ex4nicegui-0.6.5/ex4nicegui/gsap/timeline.js
+-rw-rw-rw-   0        0        0     2390 2024-04-26 16:54:25.000000 ex4nicegui-0.6.5/ex4nicegui/gsap/timeline.py
+-rw-rw-rw-   0        0        0     1045 2024-02-02 15:27:35.000000 ex4nicegui-0.6.5/ex4nicegui/gsap/wrapGsap.js
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.288398 ex4nicegui-0.6.5/ex4nicegui/layout/
+-rw-rw-rw-   0        0        0      278 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/layout/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.305360 ex4nicegui-0.6.5/ex4nicegui/layout/gridFlex/
+-rw-rw-rw-   0        0        0     4468 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/layout/gridFlex/GridFlex.js
+-rw-rw-rw-   0        0        0        2 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/layout/gridFlex/__init__.py
+-rw-rw-rw-   0        0        0     7194 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/layout/gridFlex/gridFlex.py
+-rw-rw-rw-   0        0        0     1236 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/layout/gridFlex/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.309360 ex4nicegui-0.6.5/ex4nicegui/layout/rxFlex/
+-rw-rw-rw-   0        0        0        0 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/layout/rxFlex/__init__.py
+-rw-rw-rw-   0        0        0     3672 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/layout/rxFlex/index.py
+-rw-rw-rw-   0        0        0     1411 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/layout/rxFlex/types.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.309360 ex4nicegui-0.6.5/ex4nicegui/libs/
+-rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.464670 ex4nicegui-0.6.5/ex4nicegui/libs/d3/
+-rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/__init__.py
+-rw-rw-rw-   0        0        0    12795 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-color.ems.js
+-rw-rw-rw-   0        0        0     2148 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-dispatch.ems.js
+-rw-rw-rw-   0        0        0     4822 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-drag.ems.js
+-rw-rw-rw-   0        0        0     3883 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-ease.ems.js
+-rw-rw-rw-   0        0        0     9903 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-interpolate.ems.js
+-rw-rw-rw-   0        0        0    16007 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-selection.ems.js
+-rw-rw-rw-   0        0        0     2320 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-timer.ems.js
+-rw-rw-rw-   0        0        0    14024 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-transition.ems.js
+-rw-rw-rw-   0        0        0    11599 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-zoom.ems.js
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.668386 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/
+-rw-rw-rw-   0        0        0    64907 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/CSSPlugin.js
+-rw-rw-rw-   0        0        0     3674 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/CSSRulePlugin.js
+-rw-rw-rw-   0        0        0    11588 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/CustomEase.js
+-rw-rw-rw-   0        0        0   103102 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/Draggable.js
+-rw-rw-rw-   0        0        0     5530 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/EasePack.js
+-rw-rw-rw-   0        0        0     9125 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/EaselPlugin.js
+-rw-rw-rw-   0        0        0    48981 2024-03-07 20:18:40.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/Flip.js
+-rw-rw-rw-   0        0        0    12852 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/MotionPathPlugin.js
+-rw-rw-rw-   0        0        0    26112 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/Observer.js
+-rw-rw-rw-   0        0        0    15404 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/PixiPlugin.js
+-rw-rw-rw-   0        0        0     9217 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/ScrollToPlugin.js
+-rw-rw-rw-   0        0        0   112584 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/ScrollTrigger.js
+-rw-rw-rw-   0        0        0     4877 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/TextPlugin.js
+-rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/__init__.py
+-rw-rw-rw-   0        0        0     1585 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/all.js
+-rw-rw-rw-   0        0        0   175009 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/gsap-core.js
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.709381 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/utils/__init__.py
+-rw-rw-rw-   0        0        0    15235 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/utils/matrix.js
+-rw-rw-rw-   0        0        0    49314 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/utils/paths.js
+-rw-rw-rw-   0        0        0    10472 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/libs/gsap/utils/strings.js
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.755703 ex4nicegui-0.6.5/ex4nicegui/reactive/
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.762172 ex4nicegui-0.6.5/ex4nicegui/reactive/EChartsComponent/
+-rw-rw-rw-   0        0        0     3326 2024-04-23 06:45:41.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/EChartsComponent/ECharts.js
+-rw-rw-rw-   0        0        0     6313 2024-04-26 16:54:25.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/EChartsComponent/ECharts.py
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:50:52.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/EChartsComponent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.791785 ex4nicegui-0.6.5/ex4nicegui/reactive/UseDraggable/
+-rw-rw-rw-   0        0        0     5473 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/UseDraggable/UseDraggable.js
+-rw-rw-rw-   0        0        0     3929 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/UseDraggable/UseDraggable.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 16:36:22.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/UseDraggable/__init__.py
+-rw-rw-rw-   0        0        0     3714 2024-03-25 14:45:22.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.807772 ex4nicegui-0.6.5/ex4nicegui/reactive/dropZone/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:45:08.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/dropZone/__init__.py
+-rw-rw-rw-   0        0        0     2713 2023-07-29 10:16:25.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/dropZone/dropZone.js
+-rw-rw-rw-   0        0        0     2590 2023-10-18 15:44:54.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/dropZone/dropZone.py
+-rw-rw-rw-   0        0        0       50 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/empty.js
+-rw-rw-rw-   0        0        0      132 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/empty.py
+-rw-rw-rw-   0        0        0     1472 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/fileWatcher.py
+-rw-rw-rw-   0        0        0     6225 2024-03-05 13:06:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/local_file_picker.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.824726 ex4nicegui-0.6.5/ex4nicegui/reactive/mermaid/
+-rw-rw-rw-   0        0        0        0 2023-10-23 17:41:12.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/mermaid/__init__.py
+-rw-rw-rw-   0        0        0     2308 2023-10-29 08:33:17.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/mermaid/mermaid.js
+-rw-rw-rw-   0        0        0     2144 2024-02-05 16:01:34.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/mermaid/mermaid.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.901962 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/
+-rw-rw-rw-   0        0        0        2 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/__init__.py
+-rw-rw-rw-   0        0        0     2929 2024-03-07 20:18:40.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/aggrid.py
+-rw-rw-rw-   0        0        0    10440 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/base.py
+-rw-rw-rw-   0        0        0     1660 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/button.py
+-rw-rw-rw-   0        0        0     1275 2023-07-21 14:29:40.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/card.py
+-rw-rw-rw-   0        0        0     1562 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/checkbox.py
+-rw-rw-rw-   0        0        0     1787 2024-02-29 13:12:44.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/circular_progress.py
+-rw-rw-rw-   0        0        0     3402 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/color_picker.py
+-rw-rw-rw-   0        0        0     1040 2024-02-29 12:25:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/column.py
+-rw-rw-rw-   0        0        0     2681 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/date.py
+-rw-rw-rw-   0        0        0     2370 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/drawer.py
+-rw-rw-rw-   0        0        0     9696 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/echarts.py
+-rw-rw-rw-   0        0        0      412 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/element.py
+-rw-rw-rw-   0        0        0     1873 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/expansion.py
+-rw-rw-rw-   0        0        0      865 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/grid.py
+-rw-rw-rw-   0        0        0      119 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/html.js
+-rw-rw-rw-   0        0        0      675 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/html.py
+-rw-rw-rw-   0        0        0     1559 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/icon.py
+-rw-rw-rw-   0        0        0     1120 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/image.py
+-rw-rw-rw-   0        0        0     4030 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/input.py
+-rw-rw-rw-   0        0        0     2153 2024-02-29 11:46:48.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/knob.py
+-rw-rw-rw-   0        0        0     1398 2024-03-04 19:14:43.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/label.py
+-rw-rw-rw-   0        0        0     2128 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/linear_progress.py
+-rw-rw-rw-   0        0        0     2201 2024-02-29 13:12:44.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/number.py
+-rw-rw-rw-   0        0        0     1929 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/radio.py
+-rw-rw-rw-   0        0        0     1029 2024-02-29 12:25:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/row.py
+-rw-rw-rw-   0        0        0     2980 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/select.py
+-rw-rw-rw-   0        0        0     2954 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/slider.py
+-rw-rw-rw-   0        0        0     1605 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/switch.py
+-rw-rw-rw-   0        0        0     1796 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/tab.py
+-rw-rw-rw-   0        0        0      630 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/tab_panel.py
+-rw-rw-rw-   0        0        0     1375 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/tab_panels.py
+-rw-rw-rw-   0        0        0     6042 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/table.py
+-rw-rw-rw-   0        0        0     1232 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/tabs.py
+-rw-rw-rw-   0        0        0     3044 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/textarea.py
+-rw-rw-rw-   0        0        0     2360 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/upload.py
+-rw-rw-rw-   0        0        0      213 2024-02-21 13:27:29.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/officials/utils.py
+-rw-rw-rw-   0        0        0     1505 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/q_pagination.py
+-rw-rw-rw-   0        0        0       31 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/rxui.py
+-rw-rw-rw-   0        0        0      898 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/transitionGroup.js
+-rw-rw-rw-   0        0        0      597 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/transitionGroup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.918558 ex4nicegui-0.6.5/ex4nicegui/reactive/useMouse/
+-rw-rw-rw-   0        0        0     2722 2023-07-17 15:14:14.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/useMouse/UseMouse.js
+-rw-rw-rw-   0        0        0     2122 2024-02-23 16:33:09.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/useMouse/UseMouse.py
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/useMouse/__init__.py
+-rw-rw-rw-   0        0        0     2598 2024-03-07 10:39:11.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/usePagination.py
+-rw-rw-rw-   0        0        0     4360 2024-03-07 20:18:40.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/utils.py
+-rw-rw-rw-   0        0        0      282 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/vfor.js
+-rw-rw-rw-   0        0        0     5778 2024-04-26 16:54:25.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/vfor.py
+-rw-rw-rw-   0        0        0     5091 2024-03-05 13:12:27.000000 ex4nicegui-0.6.5/ex4nicegui/reactive/vmodel.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.922558 ex4nicegui-0.6.5/ex4nicegui/tools/
+-rw-rw-rw-   0        0        0        0 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/tools/__init__.py
+-rw-rw-rw-   0        0        0     4868 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/tools/debug.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.938831 ex4nicegui-0.6.5/ex4nicegui/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.6.5/ex4nicegui/utils/__init__.py
+-rw-rw-rw-   0        0        0     2527 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/utils/apiEffect.py
+-rw-rw-rw-   0        0        0     1505 2024-03-05 13:06:09.000000 ex4nicegui-0.6.5/ex4nicegui/utils/asyncComputed.py
+-rw-rw-rw-   0        0        0     1267 2024-04-26 16:54:25.000000 ex4nicegui-0.6.5/ex4nicegui/utils/clientScope.py
+-rw-rw-rw-   0        0        0      994 2024-02-20 10:06:17.000000 ex4nicegui-0.6.5/ex4nicegui/utils/common.py
+-rw-rw-rw-   0        0        0     2310 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/utils/effect.py
+-rw-rw-rw-   0        0        0     1218 2024-02-27 19:00:38.000000 ex4nicegui-0.6.5/ex4nicegui/utils/scheduler.py
+-rw-rw-rw-   0        0        0    11346 2024-03-21 14:24:33.000000 ex4nicegui-0.6.5/ex4nicegui/utils/signals.py
+drwxrwxrwx   0        0        0        0 2024-04-27 11:46:49.106607 ex4nicegui-0.6.5/ex4nicegui.egg-info/
+-rw-rw-rw-   0        0        0    27491 2024-04-27 11:46:48.000000 ex4nicegui-0.6.5/ex4nicegui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5460 2024-04-27 11:46:48.000000 ex4nicegui-0.6.5/ex4nicegui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 11:46:48.000000 ex4nicegui-0.6.5/ex4nicegui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-27 11:46:48.000000 ex4nicegui-0.6.5/ex4nicegui.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       58 2024-04-27 11:46:48.000000 ex4nicegui-0.6.5/ex4nicegui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-27 11:46:48.000000 ex4nicegui-0.6.5/ex4nicegui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 11:46:49.941689 ex4nicegui-0.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1576 2024-04-26 16:54:25.000000 ex4nicegui-0.6.5/setup.py
```

### Comparing `ex4nicegui-0.6.4/LICENSE` & `ex4nicegui-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/PKG-INFO` & `ex4nicegui-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ex4nicegui
-Version: 0.6.4
+Version: 0.6.5
 Summary: Extension library based on nicegui, providing data responsive,BI functionality modules
 Home-page: 
 Author: carson_jia
 Author-email: 568166495@qq.com
 License: MIT license
 Keywords: nicegui,ex4nicegui,webui
 Classifier: Intended Audience :: Developers
```

### Comparing `ex4nicegui-0.6.4/README.md` & `ex4nicegui-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/__init__.py` & `ex4nicegui-0.6.5/ex4nicegui/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,8 +41,8 @@
     "reactive",
     "deep_ref",
     "batch",
     "to_raw",
     "is_setter_ref",
 ]
 
-__version__ = "0.6.4"
+__version__ = "0.6.5"
```

### Comparing `ex4nicegui-0.6.4/ex4nicegui/bi/dataSource.py` & `ex4nicegui-0.6.5/ex4nicegui/bi/dataSource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from typing import Callable, Dict, List, Optional, Set, cast, TYPE_CHECKING
 from ex4nicegui import to_ref, ref_computed, on, batch, effect
-from nicegui import context as ng_context, Client, ui
+from nicegui import Client, ui
 
 from dataclasses import dataclass, field
 from . import types
 from .protocols import IDataSourceAble
 
 
 if TYPE_CHECKING:
@@ -145,15 +145,15 @@
                 if current_info.uiResult:
                     current_info.uiResult._reset_state()
 
             # nodify every component
             self.__notify_update()
 
     def get_component_info_key(self, element_id: types._TElementID):
-        client_id = ng_context.get_client().id
+        client_id = ui.context.client.id
         return ComponentInfoKey(client_id, element_id)
 
     def get_filtered_data(self, element: ui.element):
         data = self._idataSource.get_data()
 
         # note:must be use client id of the element
         key = ComponentInfoKey(element.client.id, element.id)
@@ -171,15 +171,15 @@
 
     def _register_component(
         self,
         element_id: types._TElementID,
         update_callback: Optional[_TComponentUpdateCallback] = None,
         ui_result: Optional[UiResult] = None,
     ):
-        ng_client = ng_context.get_client()
+        ng_client = ui.context.client
         client_id = ng_client.id
 
         if not self._component_map.has_client_record(client_id):
 
             @ng_client.on_disconnect
             def _(e: Client):
                 if not e.shared:
@@ -194,15 +194,15 @@
 
     def send_filter(
         self,
         element_id: types._TElementID,
         filter: Optional[Filter],
         notify_update=True,
     ):
-        client_id = ng_context.get_client().id
+        client_id = ui.context.client.id
         key = ComponentInfoKey(client_id, element_id)
 
         if not self._component_map.has_record(key):
             raise ValueError("element not register")
 
         self._component_map.set_filter(client_id, element_id, filter)
 
@@ -212,15 +212,15 @@
 
         if notify_update:
             self.__notify_update([trigger_info])
 
         return self
 
     def notify_update(self, exclude: Optional[List[UiResult]] = None):
-        client_id = ng_context.get_client().id
+        client_id = ui.context.client.id
         exclude_infos = [
             self._component_map.get_info(ComponentInfoKey(client_id, ur.id))
             for ur in (exclude or [])
         ]
 
         return self.__notify_update(exclude_infos)
```

### Comparing `ex4nicegui-0.6.4/ex4nicegui/bi/dataSourceFacade.py` & `ex4nicegui-0.6.5/ex4nicegui/bi/dataSourceFacade.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/bi/elements/layouts.py` & `ex4nicegui-0.6.5/ex4nicegui/bi/elements/layouts.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/bi/elements/models.py` & `ex4nicegui-0.6.5/ex4nicegui/bi/elements/models.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/bi/elements/text.py` & `ex4nicegui-0.6.5/ex4nicegui/bi/elements/text.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/bi/elements/ui_aggrid.py` & `ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_aggrid.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/bi/elements/ui_date_picker.js` & `ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_date_picker.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/bi/elements/ui_date_picker.py` & `ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_date_picker.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/bi/elements/ui_echarts.py` & `ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_echarts.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/bi/elements/ui_radio.py` & `ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_radio.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/bi/elements/ui_range.py` & `ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_range.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/bi/elements/ui_select.py` & `ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_select.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/bi/elements/ui_slider.py` & `ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_slider.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/bi/elements/ui_table.py` & `ex4nicegui-0.6.5/ex4nicegui/bi/elements/ui_table.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/bi/index.py` & `ex4nicegui-0.6.5/ex4nicegui/bi/index.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/bi/protocols.py` & `ex4nicegui-0.6.5/ex4nicegui/bi/protocols.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/experimental_/gridLayout/index.py` & `ex4nicegui-0.6.5/ex4nicegui/experimental_/gridLayout/index.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/gsap/gsap.py` & `ex4nicegui-0.6.5/ex4nicegui/gsap/gsap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from pathlib import Path
 from typing import Dict, Optional, Union
 from nicegui.element import Element
-from nicegui import context as ng_context
+from nicegui import ui
 from weakref import WeakKeyDictionary
 
 
 class Gsap(
     Element,
     component="wrapGsap.js",
     exposed_libraries=["../libs/gsap/gsap.mjs"],
@@ -41,36 +41,36 @@
         self.__try_run_script_task(script)
         return self
 
     def __try_run_script_task(self, script: str):
         def fn():
             self.run_method("runScript", script)
 
-        if ng_context.get_client().has_socket_connection:
+        if ui.context.client.has_socket_connection:
             fn()
         else:
             tasks = self._props["scriptTasks"]
             tasks.append(script)
 
     def __try_run_task(self, name: str, targets: str, vars: Dict):
         def fn():
             self.run_method(name, targets, vars)
 
-        if ng_context.get_client().has_socket_connection:
+        if ui.context.client.has_socket_connection:
             fn()
         else:
             tasks = self._props["tasks"]
             tasks.append({"method": name, "targets": targets, "vars": vars})
 
 
 __instance_map = WeakKeyDictionary()
 
 
 def _get_instance():
-    current_client = ng_context.get_client()
+    current_client = ui.context.client
     ins = __instance_map.get(current_client)
 
     if not ins:
         ins = Gsap()
         __instance_map[current_client] = ins
 
     return ins
```

### Comparing `ex4nicegui-0.6.4/ex4nicegui/gsap/timeline.js` & `ex4nicegui-0.6.5/ex4nicegui/gsap/timeline.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/gsap/timeline.py` & `ex4nicegui-0.6.5/ex4nicegui/gsap/timeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from pathlib import Path
 from typing import Dict, Optional, Union
 from nicegui.element import Element
-from nicegui import context as ng_context
+from nicegui import ui
 
 
 class Timeline(
     Element,
     component="timeline.js",
     exposed_libraries=["../libs/gsap/gsap.mjs"],
     extra_libraries=["../libs/gsap/*.js", "../libs/gsap/utils/*.js"],
@@ -36,27 +36,27 @@
         self.__try_run_script_task(script)
         return self
 
     def __try_run_script_task(self, script: str):
         def fn():
             self.run_method("runScript", script)
 
-        if ng_context.get_client().has_socket_connection:
+        if ui.context.client.has_socket_connection:
             fn()
         else:
             tasks = self._props["scriptTasks"]
             tasks.append(script)
 
     def __try_run_task(
         self, name: str, targets: str, vars: Dict, position: Optional[str] = None
     ):
         def fn():
             self.run_method(name, targets, vars)
 
-        if ng_context.get_client().has_socket_connection:
+        if ui.context.client.has_socket_connection:
             fn()
         else:
             tasks = self._props["tasks"]
             tasks.append(
                 {"method": name, "targets": targets, "vars": vars, "position": position}
             )
```

### Comparing `ex4nicegui-0.6.4/ex4nicegui/gsap/wrapGsap.js` & `ex4nicegui-0.6.5/ex4nicegui/gsap/wrapGsap.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/layout/gridFlex/GridFlex.js` & `ex4nicegui-0.6.5/ex4nicegui/layout/gridFlex/GridFlex.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/layout/gridFlex/gridFlex.py` & `ex4nicegui-0.6.5/ex4nicegui/layout/gridFlex/gridFlex.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/layout/gridFlex/utils.py` & `ex4nicegui-0.6.5/ex4nicegui/layout/gridFlex/utils.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/layout/rxFlex/index.py` & `ex4nicegui-0.6.5/ex4nicegui/layout/rxFlex/index.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/layout/rxFlex/types.py` & `ex4nicegui-0.6.5/ex4nicegui/layout/rxFlex/types.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/d3/d3-color.ems.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-color.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/d3/d3-dispatch.ems.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-dispatch.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/d3/d3-drag.ems.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-drag.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/d3/d3-ease.ems.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-ease.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/d3/d3-interpolate.ems.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-interpolate.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/d3/d3-selection.ems.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-selection.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/d3/d3-timer.ems.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-timer.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/d3/d3-transition.ems.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-transition.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/d3/d3-zoom.ems.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/d3/d3-zoom.ems.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/gsap/CSSPlugin.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/CSSPlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/gsap/CSSRulePlugin.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/CSSRulePlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/gsap/CustomEase.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/CustomEase.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/gsap/Draggable.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/Draggable.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/gsap/EasePack.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/EasePack.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/gsap/EaselPlugin.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/EaselPlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/gsap/Flip.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/Flip.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/gsap/MotionPathPlugin.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/MotionPathPlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/gsap/Observer.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/Observer.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/gsap/PixiPlugin.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/PixiPlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/gsap/ScrollToPlugin.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/ScrollToPlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/gsap/ScrollTrigger.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/ScrollTrigger.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/gsap/TextPlugin.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/TextPlugin.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/gsap/all.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/all.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/gsap/gsap-core.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/gsap-core.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/gsap/utils/matrix.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/utils/matrix.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/gsap/utils/paths.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/utils/paths.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/libs/gsap/utils/strings.js` & `ex4nicegui-0.6.5/ex4nicegui/libs/gsap/utils/strings.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/EChartsComponent/ECharts.js` & `ex4nicegui-0.6.5/ex4nicegui/reactive/EChartsComponent/ECharts.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/EChartsComponent/ECharts.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/EChartsComponent/ECharts.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from nicegui.dataclasses import KWONLY_SLOTS
 from nicegui.events import (
     handle_event,
     UiEventArguments,
 )
 from nicegui.element import Element
 from nicegui.awaitable_response import AwaitableResponse
-from nicegui import context as ng_context
+from nicegui import ui
 from pathlib import Path
 import nicegui
 import uuid
 
 NG_ROOT = Path(nicegui.__file__).parent / "elements"
 libraries = [NG_ROOT / "lib/echarts/echarts.min.js"]
 
@@ -98,15 +98,15 @@
             await client.connected()
 
             for func in self._echarts_on_tasks:
                 func()
 
             client.connect_handlers.remove(on_client_connect)  # type: ignore
 
-        ng_context.get_client().on_connect(on_client_connect)
+        ui.context.client.on_connect(on_client_connect)
 
         def echartsOn_handler(e):
             callbackId = e.args["callbackId"]
             params: Dict = e.args["params"]
             params["dataType"] = params.get("dataType")
 
             if callbackId in self._echarts_on_callback_map:
@@ -172,15 +172,15 @@
 
     def echarts_on(
         self,
         event_name: _T_mouse_event_name,
         handler: _T_echats_on_callback,
         query: Optional[Union[str, Dict]] = None,
     ):
-        if not ng_context.get_client().has_socket_connection:
+        if not ui.context.client.has_socket_connection:
 
             def task_func():
                 self.echarts_on(event_name, handler, query)
 
             self._echarts_on_tasks.append(task_func)
             return
```

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/UseDraggable/UseDraggable.js` & `ex4nicegui-0.6.5/ex4nicegui/reactive/UseDraggable/UseDraggable.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/UseDraggable/UseDraggable.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/UseDraggable/UseDraggable.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/__init__.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/__init__.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/dropZone/dropZone.js` & `ex4nicegui-0.6.5/ex4nicegui/reactive/dropZone/dropZone.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/dropZone/dropZone.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/dropZone/dropZone.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/fileWatcher.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/fileWatcher.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/local_file_picker.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/local_file_picker.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/mermaid/mermaid.js` & `ex4nicegui-0.6.5/ex4nicegui/reactive/mermaid/mermaid.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/mermaid/mermaid.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/mermaid/mermaid.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/aggrid.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/aggrid.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/base.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/base.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/button.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/button.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/card.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/card.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/checkbox.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/checkbox.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/circular_progress.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/circular_progress.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/color_picker.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/color_picker.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/column.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/column.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/date.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/date.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/drawer.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/drawer.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/echarts.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/echarts.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/expansion.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/expansion.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/grid.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/grid.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/html.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/html.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/icon.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/icon.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/image.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/image.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/input.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/input.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/knob.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/knob.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/label.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/label.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/linear_progress.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/linear_progress.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/number.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/number.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/radio.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/radio.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/row.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/row.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/select.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/select.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/slider.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/slider.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/switch.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/switch.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/tab.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/tab.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/tab_panel.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/tab_panel.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/tab_panels.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/tab_panels.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/table.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/table.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/tabs.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/tabs.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/textarea.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/textarea.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/officials/upload.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/officials/upload.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/q_pagination.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/q_pagination.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/transitionGroup.js` & `ex4nicegui-0.6.5/ex4nicegui/reactive/transitionGroup.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/transitionGroup.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/transitionGroup.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/useMouse/UseMouse.js` & `ex4nicegui-0.6.5/ex4nicegui/reactive/useMouse/UseMouse.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/useMouse/UseMouse.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/useMouse/UseMouse.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/usePagination.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/usePagination.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/utils.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/utils.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/vfor.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/vfor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 from nicegui.element import Element
-from nicegui import context
+from nicegui import ui
 from ex4nicegui.utils.clientScope import _CLIENT_SCOPE_MANAGER
 from ex4nicegui.utils.signals import (
     TReadonlyRef,
     on,
     to_ref,
     to_ref_wrapper,
     TGetterOrReadonlyRef,
@@ -154,15 +154,15 @@
 
             return key, element, store, scope
 
         for idx, value in enumerate(to_value(self._data)):  # type: ignore
             key, element, store, scope = build_element(idx, value)
             self._store_map[key] = StoreItem(store, element.id, scope)
 
-        ng_client = context.get_client()
+        ng_client = ui.context.client
 
         @on(self._data, deep=True)
         def _():
             data_map = {
                 self._get_key(idx, d): d for idx, d in enumerate(to_value(self._data))
             }
```

### Comparing `ex4nicegui-0.6.4/ex4nicegui/reactive/vmodel.py` & `ex4nicegui-0.6.5/ex4nicegui/reactive/vmodel.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/tools/debug.py` & `ex4nicegui-0.6.5/ex4nicegui/tools/debug.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/utils/apiEffect.py` & `ex4nicegui-0.6.5/ex4nicegui/utils/apiEffect.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/utils/asyncComputed.py` & `ex4nicegui-0.6.5/ex4nicegui/utils/asyncComputed.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/utils/clientScope.py` & `ex4nicegui-0.6.5/ex4nicegui/utils/clientScope.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict
 from signe.core.scope import ScopeSuite
-from nicegui import Client, context as ng_context
+from nicegui import Client, ui
 
 
 _TClientID = str
 
 
 class NgScopeSuite(ScopeSuite):
     def __init__(self) -> None:
@@ -20,24 +20,25 @@
     def new_scope(self, detached: bool = False):
         return self.get_current_scope().scope(detached)
 
     def get_current_scope(self):
         # if len(ng_context.get_slot_stack()) <= 0:
         #     return
 
-        client = ng_context.get_client()
-        # if client.shared:
-        #     return
+        client = ui.context.client
 
         if client.id not in self._client_scope_map:
             self._client_scope_map[client.id] = NgScopeSuite()
 
-            @client.on_disconnect
-            def _(e: Client):
-                if e.id in self._client_scope_map:
-                    self._client_scope_map[e.id]._top_scope.dispose()
-                    del self._client_scope_map[e.id]
+            # shared clients always not dispose their scope
+            if not client.shared:
+
+                @client.on_disconnect
+                def _(e: Client):
+                    if e.id in self._client_scope_map:
+                        self._client_scope_map[e.id]._top_scope.dispose()
+                        del self._client_scope_map[e.id]
 
         return self._client_scope_map[client.id]
 
 
 _CLIENT_SCOPE_MANAGER = NgClientScopeManager()
```

### Comparing `ex4nicegui-0.6.4/ex4nicegui/utils/common.py` & `ex4nicegui-0.6.5/ex4nicegui/utils/common.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/utils/effect.py` & `ex4nicegui-0.6.5/ex4nicegui/utils/effect.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/utils/scheduler.py` & `ex4nicegui-0.6.5/ex4nicegui/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui/utils/signals.py` & `ex4nicegui-0.6.5/ex4nicegui/utils/signals.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/ex4nicegui.egg-info/PKG-INFO` & `ex4nicegui-0.6.5/ex4nicegui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ex4nicegui
-Version: 0.6.4
+Version: 0.6.5
 Summary: Extension library based on nicegui, providing data responsive,BI functionality modules
 Home-page: 
 Author: carson_jia
 Author-email: 568166495@qq.com
 License: MIT license
 Keywords: nicegui,ex4nicegui,webui
 Classifier: Intended Audience :: Developers
```

### Comparing `ex4nicegui-0.6.4/ex4nicegui.egg-info/SOURCES.txt` & `ex4nicegui-0.6.5/ex4nicegui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.6.4/setup.py` & `ex4nicegui-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     return list(all_infos)
 
 
 readme = Path("README.en.md").read_text("utf8")
 
 
-requirements = ["signe>=0.4.14", "nicegui>=1.4.0", "typing_extensions", "executing"]
+requirements = ["signe>=0.4.14", "nicegui>=1.4.23", "typing_extensions", "executing"]
 
 test_requirements = ["pytest>=3", "playwright", "pandas", "executing"]
 
 setup(
     author="carson_jia",
     author_email="568166495@qq.com",
     python_requires=">=3.8",
```

