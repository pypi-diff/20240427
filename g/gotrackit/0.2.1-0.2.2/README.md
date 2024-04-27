# Comparing `tmp/gotrackit-0.2.1.tar.gz` & `tmp/gotrackit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotrackit-0.2.1.tar", last modified: Thu Apr 18 13:37:55 2024, max compression
+gzip compressed data, was "gotrackit-0.2.2.tar", last modified: Sat Apr 27 14:32:17 2024, max compression
```

## Comparing `gotrackit-0.2.1.tar` & `gotrackit-0.2.2.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.916367 gotrackit-0.2.1/
--rw-rw-rw-   0        0        0     1085 2024-01-01 15:23:01.000000 gotrackit-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     4833 2024-04-18 13:37:55.915368 gotrackit-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4087 2024-04-18 13:20:15.000000 gotrackit-0.2.1/README.md
--rw-rw-rw-   0        0        0      795 2024-04-18 13:35:20.000000 gotrackit-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 13:37:55.916367 gotrackit-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.807293 gotrackit-0.2.1/src/
--rw-rw-rw-   0        0        0      101 2023-12-09 00:21:11.000000 gotrackit-0.2.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.812836 gotrackit-0.2.1/src/gotrackit/
--rw-rw-rw-   0        0        0    15660 2024-04-18 05:53:17.000000 gotrackit-0.2.1/src/gotrackit/GlobalVal.py
--rw-rw-rw-   0        0        0    11926 2024-04-18 13:10:23.000000 gotrackit-0.2.1/src/gotrackit/MapMatch.py
--rw-rw-rw-   0        0        0      624 2023-12-31 13:24:06.000000 gotrackit-0.2.1/src/gotrackit/WrapsFunc.py
--rw-rw-rw-   0        0        0      102 2024-01-18 03:53:10.000000 gotrackit-0.2.1/src/gotrackit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.817859 gotrackit-0.2.1/src/gotrackit/generation/
--rw-rw-rw-   0        0        0    25084 2024-03-27 15:57:38.000000 gotrackit-0.2.1/src/gotrackit/generation/GpsGen.py
--rw-rw-rw-   0        0        0      103 2023-12-30 07:52:41.000000 gotrackit-0.2.1/src/gotrackit/generation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.829264 gotrackit-0.2.1/src/gotrackit/gps/
--rw-rw-rw-   0        0        0     4259 2024-04-18 12:43:12.000000 gotrackit-0.2.1/src/gotrackit/gps/GpsArray.py
--rw-rw-rw-   0        0        0     8007 2024-04-14 02:50:11.000000 gotrackit-0.2.1/src/gotrackit/gps/GpsTrip.py
--rw-rw-rw-   0        0        0     3888 2024-04-16 14:22:42.000000 gotrackit-0.2.1/src/gotrackit/gps/GpsXfer.py
--rw-rw-rw-   0        0        0    22376 2024-04-18 06:27:36.000000 gotrackit-0.2.1/src/gotrackit/gps/LocGps.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.1/src/gotrackit/gps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.831283 gotrackit-0.2.1/src/gotrackit/map/
--rw-rw-rw-   0        0        0    19341 2024-04-18 02:38:44.000000 gotrackit-0.2.1/src/gotrackit/map/Link.py
--rw-rw-rw-   0        0        0    23345 2024-04-18 12:46:18.000000 gotrackit-0.2.1/src/gotrackit/map/Net.py
--rw-rw-rw-   0        0        0     4607 2024-04-09 00:43:47.000000 gotrackit-0.2.1/src/gotrackit/map/Node.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.1/src/gotrackit/map/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.835290 gotrackit-0.2.1/src/gotrackit/model/
--rw-rw-rw-   0        0        0    55598 2024-04-18 13:18:05.000000 gotrackit-0.2.1/src/gotrackit/model/Markov.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.1/src/gotrackit/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.841865 gotrackit-0.2.1/src/gotrackit/netreverse/
--rw-rw-rw-   0        0        0     1657 2024-01-31 02:46:45.000000 gotrackit-0.2.1/src/gotrackit/netreverse/GlobalVal.py
--rw-rw-rw-   0        0        0    26881 2024-04-12 03:06:11.000000 gotrackit-0.2.1/src/gotrackit/netreverse/NetGen.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.845738 gotrackit-0.2.1/src/gotrackit/netreverse/Parse/
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/Parse/__init__.py
--rw-rw-rw-   0        0        0    19151 2024-04-10 05:04:41.000000 gotrackit-0.2.1/src/gotrackit/netreverse/Parse/gd_car_path.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.849740 gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/
--rw-rw-rw-   0        0        0     3697 2024-01-27 14:10:52.000000 gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/GeoProcess.py
--rw-rw-rw-   0        0        0     1024 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/GraphAna.py
--rw-rw-rw-   0        0        0     1649 2024-01-28 14:46:20.000000 gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/IndexAna.py
--rw-rw-rw-   0        0        0      221 2024-01-28 14:46:20.000000 gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/MapProcess.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/__init__.py
--rw-rw-rw-   0        0        0     4362 2024-03-07 05:54:15.000000 gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/od.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.853738 gotrackit-0.2.1/src/gotrackit/netreverse/Request/
--rw-rw-rw-   0        0        0        0 2023-12-12 03:03:06.000000 gotrackit-0.2.1/src/gotrackit/netreverse/Request/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.857739 gotrackit-0.2.1/src/gotrackit/netreverse/Request/api/
--rw-rw-rw-   0        0        0     3812 2024-01-29 14:05:19.000000 gotrackit-0.2.1/src/gotrackit/netreverse/Request/api/WebApi.py
--rw-rw-rw-   0        0        0      103 2023-12-12 04:05:25.000000 gotrackit-0.2.1/src/gotrackit/netreverse/Request/api/__init__.py
--rw-rw-rw-   0        0        0     3093 2024-01-29 11:43:10.000000 gotrackit-0.2.1/src/gotrackit/netreverse/Request/request_path.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.862703 gotrackit-0.2.1/src/gotrackit/netreverse/Request/usage/
--rw-rw-rw-   0        0        0      103 2023-12-12 04:10:22.000000 gotrackit-0.2.1/src/gotrackit/netreverse/Request/usage/__init__.py
--rw-rw-rw-   0        0        0     7809 2024-01-28 14:46:20.000000 gotrackit-0.2.1/src/gotrackit/netreverse/Request/usage/bd_ts.py
--rw-rw-rw-   0        0        0    11231 2024-01-31 07:13:59.000000 gotrackit-0.2.1/src/gotrackit/netreverse/Request/usage/gd_car_path.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.869965 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.875968 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/DupProcess/
--rw-rw-rw-   0        0        0    21741 2024-03-18 03:07:20.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/DupProcess/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.882864 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/
--rw-rw-rw-   0        0        0      103 2023-12-18 12:14:41.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/__init__.py
--rw-rw-rw-   0        0        0     6874 2024-01-27 07:40:20.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.889779 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/__init__.py
--rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py
--rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py
--rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py
--rw-rw-rw-   0        0        0     9459 2024-01-27 07:40:20.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py
--rw-rw-rw-   0        0        0    12225 2024-03-06 12:24:39.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py
--rw-rw-rw-   0        0        0    15086 2024-01-27 08:21:05.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.889779 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/
--rw-rw-rw-   0        0        0      102 2024-03-17 11:27:43.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.897275 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/__init__.py
--rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py
--rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py
--rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py
--rw-rw-rw-   0        0        0     8948 2024-04-08 05:51:27.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py
--rw-rw-rw-   0        0        0    21559 2024-04-12 02:47:41.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.898273 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/SaveStreets/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/SaveStreets/__init__.py
--rw-rw-rw-   0        0        0    21115 2024-03-15 13:54:11.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.900268 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Split/
--rw-rw-rw-   0        0        0     4266 2024-01-29 13:44:04.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Split/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.902413 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Tools/
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Tools/__init__.py
--rw-rw-rw-   0        0        0     5745 2024-04-08 08:18:36.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Tools/process.py
--rw-rw-rw-   0        0        0      133 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/__init__.py
--rw-rw-rw-   0        0        0     9629 2024-03-27 15:52:33.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/conn.py
--rw-rw-rw-   0        0        0    18855 2024-03-09 13:07:40.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/increment.py
--rw-rw-rw-   0        0        0     9043 2024-04-08 07:19:18.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/net_reverse.py
--rw-rw-rw-   0        0        0     5765 2024-04-12 02:47:41.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/optimize_net.py
--rw-rw-rw-   0        0        0     1188 2024-03-05 08:17:38.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/save_file.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/__init__.py
--rw-rw-rw-   0        0        0     2654 2024-01-29 14:01:55.000000 gotrackit-0.2.1/src/gotrackit/netreverse/book_mark.py
--rw-rw-rw-   0        0        0     1868 2024-01-27 14:19:15.000000 gotrackit-0.2.1/src/gotrackit/netreverse/format_od.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.904216 gotrackit-0.2.1/src/gotrackit/netxfer/
--rw-rw-rw-   0        0        0    17197 2024-04-16 10:06:45.000000 gotrackit-0.2.1/src/gotrackit/netxfer/SumoConvert.py
--rw-rw-rw-   0        0        0      101 2024-03-30 00:52:12.000000 gotrackit-0.2.1/src/gotrackit/netxfer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.905960 gotrackit-0.2.1/src/gotrackit/solver/
--rw-rw-rw-   0        0        0     9181 2024-04-03 02:13:18.000000 gotrackit-0.2.1/src/gotrackit/solver/Viterbi.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.1/src/gotrackit/solver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.912248 gotrackit-0.2.1/src/gotrackit/tools/
--rw-rw-rw-   0        0        0      102 2024-01-10 02:23:14.000000 gotrackit-0.2.1/src/gotrackit/tools/__init__.py
--rw-rw-rw-   0        0        0    10646 2024-03-05 06:26:07.000000 gotrackit-0.2.1/src/gotrackit/tools/coord_trans.py
--rw-rw-rw-   0        0        0    12119 2024-04-08 08:18:36.000000 gotrackit-0.2.1/src/gotrackit/tools/geo_process.py
--rw-rw-rw-   0        0        0      812 2024-04-12 02:40:08.000000 gotrackit-0.2.1/src/gotrackit/tools/group.py
--rw-rw-rw-   0        0        0     1121 2024-01-31 04:02:14.000000 gotrackit-0.2.1/src/gotrackit/tools/save_file.py
--rw-rw-rw-   0        0        0     9708 2024-04-18 13:24:10.000000 gotrackit-0.2.1/src/gotrackit/visualization.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.914372 gotrackit-0.2.1/src/gotrackit.egg-info/
--rw-rw-rw-   0        0        0     4833 2024-04-18 13:37:55.000000 gotrackit-0.2.1/src/gotrackit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3695 2024-04-18 13:37:55.000000 gotrackit-0.2.1/src/gotrackit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 13:37:55.000000 gotrackit-0.2.1/src/gotrackit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-18 13:37:55.000000 gotrackit-0.2.1/src/gotrackit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-18 13:37:55.000000 gotrackit-0.2.1/src/gotrackit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.790742 gotrackit-0.2.2/
+-rw-rw-rw-   0        0        0     1085 2024-01-01 15:23:01.000000 gotrackit-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     7664 2024-04-27 14:32:17.789766 gotrackit-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6918 2024-04-27 00:03:13.000000 gotrackit-0.2.2/README.md
+-rw-rw-rw-   0        0        0      795 2024-04-27 14:31:39.000000 gotrackit-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-27 14:32:17.790742 gotrackit-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.697977 gotrackit-0.2.2/src/
+-rw-rw-rw-   0        0        0      101 2023-12-09 00:21:11.000000 gotrackit-0.2.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.702964 gotrackit-0.2.2/src/gotrackit/
+-rw-rw-rw-   0        0        0    15805 2024-04-25 09:18:31.000000 gotrackit-0.2.2/src/gotrackit/GlobalVal.py
+-rw-rw-rw-   0        0        0    15773 2024-04-27 14:03:24.000000 gotrackit-0.2.2/src/gotrackit/MapMatch.py
+-rw-rw-rw-   0        0        0      624 2023-12-31 13:24:06.000000 gotrackit-0.2.2/src/gotrackit/WrapsFunc.py
+-rw-rw-rw-   0        0        0      102 2024-01-18 03:53:10.000000 gotrackit-0.2.2/src/gotrackit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.708948 gotrackit-0.2.2/src/gotrackit/generation/
+-rw-rw-rw-   0        0        0    25084 2024-03-27 15:57:38.000000 gotrackit-0.2.2/src/gotrackit/generation/GpsGen.py
+-rw-rw-rw-   0        0        0      103 2023-12-30 07:52:41.000000 gotrackit-0.2.2/src/gotrackit/generation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.715937 gotrackit-0.2.2/src/gotrackit/gps/
+-rw-rw-rw-   0        0        0     4259 2024-04-18 12:43:12.000000 gotrackit-0.2.2/src/gotrackit/gps/GpsArray.py
+-rw-rw-rw-   0        0        0     8007 2024-04-14 02:50:11.000000 gotrackit-0.2.2/src/gotrackit/gps/GpsTrip.py
+-rw-rw-rw-   0        0        0     3888 2024-04-16 14:22:42.000000 gotrackit-0.2.2/src/gotrackit/gps/GpsXfer.py
+-rw-rw-rw-   0        0        0    22508 2024-04-22 09:39:54.000000 gotrackit-0.2.2/src/gotrackit/gps/LocGps.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.2/src/gotrackit/gps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.719926 gotrackit-0.2.2/src/gotrackit/map/
+-rw-rw-rw-   0        0        0    18317 2024-04-25 15:48:16.000000 gotrackit-0.2.2/src/gotrackit/map/Link.py
+-rw-rw-rw-   0        0        0    35933 2024-04-27 14:20:15.000000 gotrackit-0.2.2/src/gotrackit/map/Net.py
+-rw-rw-rw-   0        0        0     4607 2024-04-09 00:43:47.000000 gotrackit-0.2.2/src/gotrackit/map/Node.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.2/src/gotrackit/map/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.720924 gotrackit-0.2.2/src/gotrackit/model/
+-rw-rw-rw-   0        0        0    64510 2024-04-27 14:30:20.000000 gotrackit-0.2.2/src/gotrackit/model/Markov.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.2/src/gotrackit/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.727910 gotrackit-0.2.2/src/gotrackit/netreverse/
+-rw-rw-rw-   0        0        0     1657 2024-01-31 02:46:45.000000 gotrackit-0.2.2/src/gotrackit/netreverse/GlobalVal.py
+-rw-rw-rw-   0        0        0    26847 2024-04-20 03:45:37.000000 gotrackit-0.2.2/src/gotrackit/netreverse/NetGen.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.729905 gotrackit-0.2.2/src/gotrackit/netreverse/Parse/
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/Parse/__init__.py
+-rw-rw-rw-   0        0        0    19151 2024-04-10 05:04:41.000000 gotrackit-0.2.2/src/gotrackit/netreverse/Parse/gd_car_path.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.735889 gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/
+-rw-rw-rw-   0        0        0     3697 2024-01-27 14:10:52.000000 gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/GeoProcess.py
+-rw-rw-rw-   0        0        0     1024 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/GraphAna.py
+-rw-rw-rw-   0        0        0     1649 2024-01-28 14:46:20.000000 gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/IndexAna.py
+-rw-rw-rw-   0        0        0      221 2024-01-28 14:46:20.000000 gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/MapProcess.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/__init__.py
+-rw-rw-rw-   0        0        0     4362 2024-03-07 05:54:15.000000 gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/od.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.737892 gotrackit-0.2.2/src/gotrackit/netreverse/Request/
+-rw-rw-rw-   0        0        0        0 2023-12-12 03:03:06.000000 gotrackit-0.2.2/src/gotrackit/netreverse/Request/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.739878 gotrackit-0.2.2/src/gotrackit/netreverse/Request/api/
+-rw-rw-rw-   0        0        0     3812 2024-01-29 14:05:19.000000 gotrackit-0.2.2/src/gotrackit/netreverse/Request/api/WebApi.py
+-rw-rw-rw-   0        0        0      103 2023-12-12 04:05:25.000000 gotrackit-0.2.2/src/gotrackit/netreverse/Request/api/__init__.py
+-rw-rw-rw-   0        0        0     3093 2024-01-29 11:43:10.000000 gotrackit-0.2.2/src/gotrackit/netreverse/Request/request_path.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.743867 gotrackit-0.2.2/src/gotrackit/netreverse/Request/usage/
+-rw-rw-rw-   0        0        0      103 2023-12-12 04:10:22.000000 gotrackit-0.2.2/src/gotrackit/netreverse/Request/usage/__init__.py
+-rw-rw-rw-   0        0        0     7809 2024-01-28 14:46:20.000000 gotrackit-0.2.2/src/gotrackit/netreverse/Request/usage/bd_ts.py
+-rw-rw-rw-   0        0        0    11231 2024-01-31 07:13:59.000000 gotrackit-0.2.2/src/gotrackit/netreverse/Request/usage/gd_car_path.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.750848 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.752843 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/DupProcess/
+-rw-rw-rw-   0        0        0    21741 2024-03-18 03:07:20.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/DupProcess/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.757830 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/
+-rw-rw-rw-   0        0        0      103 2023-12-18 12:14:41.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/__init__.py
+-rw-rw-rw-   0        0        0     6874 2024-01-27 07:40:20.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.763814 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/__init__.py
+-rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py
+-rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py
+-rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py
+-rw-rw-rw-   0        0        0     9459 2024-01-27 07:40:20.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py
+-rw-rw-rw-   0        0        0    12225 2024-03-06 12:24:39.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py
+-rw-rw-rw-   0        0        0    15086 2024-01-27 08:21:05.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.765808 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/
+-rw-rw-rw-   0        0        0      102 2024-03-17 11:27:43.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.770795 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/__init__.py
+-rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py
+-rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py
+-rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py
+-rw-rw-rw-   0        0        0     8948 2024-04-08 05:51:27.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py
+-rw-rw-rw-   0        0        0    21559 2024-04-12 02:47:41.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.774784 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/SaveStreets/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/SaveStreets/__init__.py
+-rw-rw-rw-   0        0        0    21115 2024-03-15 13:54:11.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.776799 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Split/
+-rw-rw-rw-   0        0        0     4266 2024-01-29 13:44:04.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Split/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.777777 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Tools/
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Tools/__init__.py
+-rw-rw-rw-   0        0        0     5745 2024-04-08 08:18:36.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Tools/process.py
+-rw-rw-rw-   0        0        0      133 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/__init__.py
+-rw-rw-rw-   0        0        0     9629 2024-03-27 15:52:33.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/conn.py
+-rw-rw-rw-   0        0        0    18855 2024-03-09 13:07:40.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/increment.py
+-rw-rw-rw-   0        0        0     9043 2024-04-08 07:19:18.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/net_reverse.py
+-rw-rw-rw-   0        0        0     5758 2024-04-20 03:45:37.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/optimize_net.py
+-rw-rw-rw-   0        0        0     1188 2024-03-05 08:17:38.000000 gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/save_file.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.2/src/gotrackit/netreverse/__init__.py
+-rw-rw-rw-   0        0        0     2654 2024-01-29 14:01:55.000000 gotrackit-0.2.2/src/gotrackit/netreverse/book_mark.py
+-rw-rw-rw-   0        0        0     1868 2024-01-27 14:19:15.000000 gotrackit-0.2.2/src/gotrackit/netreverse/format_od.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.779771 gotrackit-0.2.2/src/gotrackit/netxfer/
+-rw-rw-rw-   0        0        0    17197 2024-04-16 10:06:45.000000 gotrackit-0.2.2/src/gotrackit/netxfer/SumoConvert.py
+-rw-rw-rw-   0        0        0      101 2024-03-30 00:52:12.000000 gotrackit-0.2.2/src/gotrackit/netxfer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.781766 gotrackit-0.2.2/src/gotrackit/solver/
+-rw-rw-rw-   0        0        0     9156 2024-04-21 05:56:15.000000 gotrackit-0.2.2/src/gotrackit/solver/Viterbi.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.2/src/gotrackit/solver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.786752 gotrackit-0.2.2/src/gotrackit/tools/
+-rw-rw-rw-   0        0        0      102 2024-01-10 02:23:14.000000 gotrackit-0.2.2/src/gotrackit/tools/__init__.py
+-rw-rw-rw-   0        0        0    10646 2024-03-05 06:26:07.000000 gotrackit-0.2.2/src/gotrackit/tools/coord_trans.py
+-rw-rw-rw-   0        0        0    12119 2024-04-08 08:18:36.000000 gotrackit-0.2.2/src/gotrackit/tools/geo_process.py
+-rw-rw-rw-   0        0        0      812 2024-04-12 02:40:08.000000 gotrackit-0.2.2/src/gotrackit/tools/group.py
+-rw-rw-rw-   0        0        0     1121 2024-01-31 04:02:14.000000 gotrackit-0.2.2/src/gotrackit/tools/save_file.py
+-rw-rw-rw-   0        0        0     9708 2024-04-27 06:20:00.000000 gotrackit-0.2.2/src/gotrackit/visualization.py
+drwxrwxrwx   0        0        0        0 2024-04-27 14:32:17.788747 gotrackit-0.2.2/src/gotrackit.egg-info/
+-rw-rw-rw-   0        0        0     7664 2024-04-27 14:32:17.000000 gotrackit-0.2.2/src/gotrackit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3695 2024-04-27 14:32:17.000000 gotrackit-0.2.2/src/gotrackit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 14:32:17.000000 gotrackit-0.2.2/src/gotrackit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-27 14:32:17.000000 gotrackit-0.2.2/src/gotrackit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-27 14:32:17.000000 gotrackit-0.2.2/src/gotrackit.egg-info/top_level.txt
```

### Comparing `gotrackit-0.2.1/LICENSE` & `gotrackit-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/pyproject.toml` & `gotrackit-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gotrackit"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = ["geopandas>=0.14.1", "shapely", "networkx", "pandas", "numpy", "keplergl", "geopy"]
 requires-python = ">=3.8"
 authors = [
   { name="Kai Tang", email="794568794@qq.com" },
 ]
 description = "A Python Package for Map Matching Algorithm Based on Hidden Markov Model"
 readme = "README.md"
```

### Comparing `gotrackit-0.2.1/src/gotrackit/GlobalVal.py` & `gotrackit-0.2.2/src/gotrackit/GlobalVal.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,17 +14,21 @@
         self.SINGLE_LINK_ID_FIELD = 'single_link_id'
         self.DIRECTION_FIELD = 'dir'
         self.FROM_NODE_FIELD = 'from_node'
         self.TO_NODE_FIELD = 'to_node'
         self.LENGTH_FIELD = 'length'
         self.GEOMETRY_FIELD = 'geometry'
         self.NODE_ID_FIELD = 'node_id'
-        self.NODE_PATH_FIELD = 'node_path'
+        self.S_NODE = 'o_node'
+        self.T_NODE = 'd_node'
+        self.NODE_PATH_FIELD = 'path'
         self.COST_FIELD = 'cost'
         self.LINK_VEC_FIELD = 'dir_vec'
+        self.SEG_COUNT = 'seg_count'
+        self.SEG_ACCU_LENGTH = 'seg_accu_length'
 
 class GpsField(object):
     """gps数据字段"""
     def __init__(self):
         self.POINT_SEQ_FIELD = 'seq'
         self.SUB_SEQ_FIELD = 'sub_seq'
         self.ORIGIN_POINT_SEQ_FIELD = 'origin_seq'
@@ -74,15 +78,15 @@
         self.FROM_STATE_N = 'from_state_node'
         self.TO_STATE_N = 'to_state_node'
         self.ROUTE_LENGTH = 'route_l'
         self.ROUTE_ITEM = 'route_item'
         self.STRAIGHT_LENGTH = 'straight_l'
         self.DIS_GAP = 'dis_gap'
         self.PRJ_L = 'prj_dis'
-        self.PRJ_GEO = 'prj_geo'
+        self.PRJ_GEO = 'prj_p'
         self.DIS_TO_NEXT = 'dis_to_next'
         self.HEADING_GAP = 'heading_gap'
 
 
 class KeplerConfig(object):
     def __init__(self):
         self.__BASE_CONFIG = {
```

### Comparing `gotrackit-0.2.1/src/gotrackit/MapMatch.py` & `gotrackit-0.2.2/src/gotrackit/MapMatch.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 # -- coding: utf-8 --
 # @Time    : 2024/3/25 14:13
 # @Author  : TangKai
 # @Team    : ZheChengData
-
+import os
 
 import numpy as np
 import pandas as pd
+import multiprocessing
 from .map.Net import Net
+from .tools.group import cut_group
 from .gps.LocGps import GpsPointsGdf
 from .model.Markov import HiddenMarkov
 from .GlobalVal import NetField, GpsField
 from .visualization import export_visualization
 
+
 gps_field = GpsField()
 net_field = NetField()
 agent_id_field = gps_field.AGENT_ID_FIELD
 node_id_field = net_field.NODE_ID_FIELD
 
 
 class MapMatch(object):
     def __init__(self, flag_name: str = 'test', net: Net = None, use_sub_net: bool = True, gps_df: pd.DataFrame = None,
                  time_format: str = "%Y-%m-%d %H:%M:%S", time_unit: str = 's',
-                 gps_buffer: float = 100, gps_route_buffer_gap: float = 25.0,
-                 max_increment_times: int = 2, increment_buffer: float = 20.0,
+                 gps_buffer: float = 200.0, gps_route_buffer_gap: float = 15.0,
+                 max_increment_times: int = 2, increment_buffer: float = 15.0,
                  beta: float = 20.0, gps_sigma: float = 20.0, dis_para: float = 0.1,
                  is_lower_f: bool = False, lower_n: int = 2,
                  use_heading_inf: bool = False, heading_para_array: np.ndarray = None,
                  dense_gps: bool = True, dense_interval: float = 80.0,
                  dwell_l_length: float = 10.0, dwell_n: int = 2, del_dwell: bool = True,
                  dup_threshold: float = 10.0,
                  is_rolling_average: bool = False, window: int = 2,
                  export_html: bool = False, use_gps_source: bool = False, html_fldr: str = None,
                  export_geo_res: bool = False,
-                 node_num_threshold: int = 2000, top_k: int = 20, omitted_l: float = 6.0, multi_core: bool = True,
-                 core_num: int = 1, link_width: float = 1.5, node_radius: float = 1.5,
+                 node_num_threshold: int = 2000, top_k: int = 20, omitted_l: float = 6.0,
+                 link_width: float = 1.5, node_radius: float = 1.5,
                  match_link_width: float = 5.0, gps_radius: float = 6.0, export_all_agents: bool = False,
                  visualization_cache_times: int = 50, multi_core_save: bool = False):
         """
         :param flag_name: 标记字符名称, 会用于标记输出的可视化文件, 默认"test"
         :param net: gotrackit路网对象, 必须指定
         :param use_sub_net: 是否在子网络上进行计算, 默认True
         :param gps_df: GPS数据, 必须指定
@@ -61,16 +64,14 @@
         :param window: 滑动窗口大小, 默认2
         :param export_html: 是否输出网页可视化结果html文件, 默认True
         :param use_gps_source: 是否在可视化结果中使用GPS源数据进行展示, 默认False
         :param html_fldr: 保存网页可视化结果的文件目录, 默认当前目录
         :param export_geo_res: 是否输出匹配结果的几何可视化文件, 默认False
         :param node_num_threshold: 默认2000
         :param omitted_l: 当某GPS点与前后GPS点的平均距离小于该距离(m)时, 该GPS点的方向限制作用被取消
-        :param multi_core: 是否启用多核匹配, 默认True
-        :param core_num: 用几个核, 默认1
         :param gps_radius: HTML可视化中GPS点的半径大小，单位米，默认8米
         :param export_all_agents: 是否将所有agent的可视化存储于一个html文件中
         :param visualization_cache_times: 每匹配完几辆车再进行结果的统一存储, 默认50
         :param multi_core_save: 是否启用多进程进行结果存储
         """
         # 坐标系投影
         self.plain_crs = net.planar_crs
@@ -95,60 +96,66 @@
         self.gps_buffer = gps_buffer  # gps的关联范围(m)
         self.use_sub_net = use_sub_net  # 是否启用子网络
         self.max_increment_times = max_increment_times
         self.increment_buffer = increment_buffer
         self.gps_route_buffer_gap = gps_route_buffer_gap
         self.use_heading_inf = use_heading_inf
         self.heading_para_array = heading_para_array
+        if not omitted_l < dense_interval / 2:
+            omitted_l = dense_interval / 2 - 0.1
         self.omitted_l = omitted_l
         self.top_k = top_k
+        if not dup_threshold < (self.gps_buffer + self.gps_route_buffer_gap) / 3:
+            dup_threshold = (self.gps_buffer + self.gps_route_buffer_gap) / 3 - 0.1
         self.dup_threshold = dup_threshold
-        assert dup_threshold < (self.gps_buffer + self.gps_route_buffer_gap) / 3
 
         self.beta = beta  # 状态转移概率参数, 概率与之成正比
         self.gps_sigma = gps_sigma  # 发射概率参数, 概率与之成正比
         self.flag_name = flag_name
         self.dis_para = dis_para
 
         self.export_html = export_html
         self.export_geo_res = export_geo_res
         self.html_fldr = html_fldr
 
         self.may_error_list = dict()
+        self.error_list = list()
 
         self.my_net = net
         self.not_conn_cost = self.my_net.not_conn_cost
         self.use_gps_source = use_gps_source
-        assert omitted_l < dense_interval / 2, 'omitted_l 必须小于 dense_interval / 2'
-        self.multi_core = multi_core
-        self.core_num = core_num
 
         # 网页可视化参数
         self.link_width = link_width
         self.node_radius = node_radius
         self.match_link_width = match_link_width
         self.gps_radius = gps_radius
 
         self.export_all_agents = export_all_agents
         self.visualization_cache_times = visualization_cache_times
         self.multi_core_save = multi_core_save
+        self.sub_net_buffer = self.gps_buffer + self.gps_route_buffer_gap + max_increment_times * increment_buffer
 
-    def execute(self):
+    def execute(self) -> tuple[pd.DataFrame, dict, list]:
         match_res_df = pd.DataFrame()
         hmm_res_list = []  # save hmm_res
         if len(self.my_net.get_node_data()[node_id_field].unique()) <= self.node_num_threshold:
             self.use_sub_net = False
         self.gps_df.dropna(subset=[agent_id_field], inplace=True)
         agent_num = len(self.gps_df[gps_field.AGENT_ID_FIELD].unique())
         if agent_num == 0:
-            raise ValueError('去除agent_id列空值行后, gps数据为空...')
+            print('去除agent_id列空值行后, gps数据为空...')
+            return match_res_df, self.may_error_list, self.error_list
+
         # 对每辆车的轨迹进行匹配
         agent_count = 0
+        add_single_ft = [True]
         for agent_id, _gps_df in self.gps_df.groupby(gps_field.AGENT_ID_FIELD):
-            print(rf'- gotrackit ------> agent: {agent_id} ')
+            agent_count += 1
+            print(rf'- gotrackit ------> No.{agent_count}: agent: {agent_id} ')
             gps_obj = GpsPointsGdf(gps_points_df=_gps_df, time_format=self.time_format,
                                    buffer=self.gps_buffer, time_unit=self.time_unit,
                                    plane_crs=self.plain_crs,
                                    max_increment_times=self.max_increment_times, increment_buffer=self.increment_buffer,
                                    dense_gps=self.dense_gps, dense_interval=self.dense_interval,
                                    dwell_l_length=self.dwell_l_length, dwell_n=self.dwell_n)
             del _gps_df
@@ -169,43 +176,104 @@
                 print(rf'dense gps by interval - {self.dense_interval}m')
                 gps_obj.dense()
 
             # 依据当前的GPS数据(源数据)做一个子网络
             if self.use_sub_net:
                 print(rf'using sub net')
                 used_net = self.my_net.create_computational_net(
-                    gps_array_buffer=gps_obj.get_gps_array_buffer(buffer=self.gps_buffer + self.gps_route_buffer_gap,
-                                                                  dup_threshold=self.dup_threshold))
+                    gps_array_buffer=gps_obj.get_gps_array_buffer(buffer=self.sub_net_buffer,
+                                                                  dup_threshold=self.dup_threshold),
+                    fmm_cache=self.my_net.fmm_cache, weight_field=self.my_net.weight_field,
+                    cache_path=self.my_net.cache_path, cache_id=self.my_net.cache_id,
+                    not_conn_cost=self.my_net.not_conn_cost)
+                if used_net is None:
+                    self.error_list.append(agent_id)
+                    continue
             else:
                 used_net = self.my_net
                 print(rf'using whole net')
 
             # 初始化一个隐马尔可夫模型
             hmm_obj = HiddenMarkov(net=used_net, gps_points=gps_obj, beta=self.beta, gps_sigma=self.gps_sigma,
                                    not_conn_cost=self.not_conn_cost, use_heading_inf=self.use_heading_inf,
                                    heading_para_array=self.heading_para_array, dis_para=self.dis_para,
-                                   top_k=self.top_k, omitted_l=self.omitted_l, multi_core=self.multi_core,
-                                   core_num=self.core_num)
+                                   top_k=self.top_k, omitted_l=self.omitted_l)
 
             # 求解参数
-            hmm_obj.generate_markov_para()
+            is_success = hmm_obj.generate_markov_para(add_single_ft)
+            if not is_success:
+                continue
             hmm_obj.solve()
             _match_res_df = hmm_obj.acquire_res()
             hmm_obj.format_war_info()
             if hmm_obj.is_warn:
                 self.may_error_list[agent_id] = hmm_obj.format_warn_info
             match_res_df = pd.concat([match_res_df, _match_res_df])
-            agent_count += 1
 
             # if export files
             if self.export_html or self.export_geo_res:
                 hmm_res_list.append(hmm_obj)
                 if len(hmm_res_list) >= self.visualization_cache_times or agent_count == agent_num:
                     export_visualization(hmm_obj_list=hmm_res_list, use_gps_source=self.use_gps_source,
                                          export_geo=self.export_geo_res, export_html=self.export_html,
                                          gps_radius=self.gps_radius, export_all_agents=self.export_all_agents,
                                          out_fldr=self.html_fldr, flag_name=self.flag_name,
                                          multi_core_save=self.multi_core_save)
                     del hmm_res_list
                     hmm_res_list = []
 
-        return match_res_df, self.may_error_list
+        return match_res_df, self.may_error_list, self.error_list
+
+    def multi_core_execute(self, core_num: int = 2) -> tuple[pd.DataFrame, dict, list]:
+        agent_id_list = list(self.gps_df[gps_field.AGENT_ID_FIELD].unique())
+        core_num = os.cpu_count() if core_num > os.cpu_count() else core_num
+        agent_group = cut_group(agent_id_list, n=core_num)
+        n = len(agent_group)
+        print(f'using multiprocessing - {n} cores')
+        pool = multiprocessing.Pool(processes=n)
+        result_list = []
+        for i in range(0, n):
+            core_html_fldr = os.path.join(self.html_fldr, rf'core{i}')
+            if os.path.exists(core_html_fldr):
+                pass
+            else:
+                os.makedirs(core_html_fldr)
+
+            agent_id_list = agent_group[i]
+            gps_df = self.gps_df[self.gps_df[gps_field.AGENT_ID_FIELD].isin(agent_id_list)]
+            mmp = MapMatch(gps_df=gps_df, net=self.my_net, use_sub_net=self.use_sub_net, time_format=self.time_format,
+                           time_unit=self.time_unit, gps_buffer=self.gps_buffer,
+                           gps_route_buffer_gap=self.gps_route_buffer_gap,
+                           max_increment_times=self.max_increment_times, increment_buffer=self.increment_buffer,
+                           beta=self.beta,
+                           gps_sigma=self.gps_sigma, dis_para=self.dis_para, is_lower_f=self.is_lower_f,
+                           lower_n=self.lower_n,
+                           use_heading_inf=self.use_heading_inf, heading_para_array=self.heading_para_array,
+                           dense_gps=self.dense_gps,
+                           dense_interval=self.dense_interval, dwell_l_length=self.dwell_l_length, dwell_n=self.dwell_n,
+                           del_dwell=self.del_dwell,
+                           dup_threshold=self.dup_threshold, is_rolling_average=self.is_rolling_average,
+                           window=self.rolling_window,
+                           export_html=self.export_html,
+                           use_gps_source=self.use_gps_source, html_fldr=core_html_fldr,
+                           export_geo_res=self.export_geo_res,
+                           node_num_threshold=self.node_num_threshold,
+                           top_k=self.top_k, omitted_l=self.omitted_l, link_width=self.link_width,
+                           node_radius=self.node_radius,
+                           match_link_width=self.match_link_width, gps_radius=self.gps_radius,
+                           export_all_agents=self.export_all_agents,
+                           visualization_cache_times=self.visualization_cache_times,
+                           multi_core_save=False)
+            result = pool.apply_async(mmp.execute,
+                                      args=())
+            result_list.append(result)
+        pool.close()
+        pool.join()
+
+        match_res, may_error, error = pd.DataFrame(), dict(), list()
+        for res in result_list:
+            _match_res, _may_error, _error = res.get()
+            match_res = pd.concat([match_res, _match_res])
+            may_error.update(_may_error)
+            error.extend(_error)
+        match_res.reset_index(inplace=True, drop=True)
+        return match_res, may_error, error
```

### Comparing `gotrackit-0.2.1/src/gotrackit/WrapsFunc.py` & `gotrackit-0.2.2/src/gotrackit/WrapsFunc.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/generation/GpsGen.py` & `gotrackit-0.2.2/src/gotrackit/generation/GpsGen.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/gps/GpsArray.py` & `gotrackit-0.2.2/src/gotrackit/gps/GpsArray.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/gps/GpsTrip.py` & `gotrackit-0.2.2/src/gotrackit/gps/GpsTrip.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/gps/GpsXfer.py` & `gotrackit-0.2.2/src/gotrackit/gps/GpsXfer.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/gps/LocGps.py` & `gotrackit-0.2.2/src/gotrackit/gps/LocGps.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,22 +96,22 @@
 
         # 存储最原始的GPS信息
         self.__source_gps_points_gdf = self.__gps_points_gdf.copy()
 
         self.done_diff_heading = False
 
     def check(self):
-        assert len(self.__gps_points_gdf) > 1, f'agent: {self.agent_id} GPS样本数据不足两个...'
         assert {gps_field.LNG_FIELD, gps_field.LAT_FIELD,
                 gps_field.AGENT_ID_FIELD, gps_field.TIME_FIELD}.issubset(
             set(self.__gps_points_gdf.columns)), \
             rf'GPS数据字段有误, 请至少包含如下字段: {gps_field.AGENT_ID_FIELD, gps_field.LNG_FIELD, gps_field.LAT_FIELD, gps_field.TIME_FIELD}'
 
-    def dense(self):
-
+    def dense(self) -> None:
+        if len(self.__gps_points_gdf) <= 1:
+            return None
         # 时间差和距离差
         self.calc_adj_dis_gap()
         self.calc_adj_time_gap()
 
         should_be_dense_gdf = self.__gps_points_gdf[self.__gps_points_gdf[dis_gap_field] > self.dense_interval].copy()
         if should_be_dense_gdf.empty:
             return None
@@ -283,20 +283,24 @@
     def gps_gdf(self) -> gpd.GeoDataFrame:
         return self.__gps_points_gdf.copy()
 
     @property
     def crs(self):
         return self.__crs
 
-    def get_gps_array_buffer(self, buffer: float = 200.0, dup_threshold: float = 10.0) -> Polygon:
+    def get_gps_array_buffer(self, buffer: float = 200.0, dup_threshold: float = 10.0) -> Polygon or None:
         """输出gps路径的buffer范围面域"""
-        gps_route_l = gpd.GeoSeries(LineString(self.__gps_points_gdf[gps_field.GEOMETRY_FIELD].to_list()))
-        simplify_gps_route_l = gps_route_l.remove_repeated_points(dup_threshold)
-        gps_array_buffer = simplify_gps_route_l[0].buffer(buffer)
-        return gps_array_buffer
+        if len(self.__gps_points_gdf) <= 1:
+            print(r'经过数据预处理后GPS观测点数据不足2个')
+            return None
+        else:
+            gps_route_l = gpd.GeoSeries(LineString(self.__gps_points_gdf[gps_field.GEOMETRY_FIELD].to_list()))
+            simplify_gps_route_l = gps_route_l.remove_repeated_points(dup_threshold)
+            gps_array_buffer = simplify_gps_route_l[0].buffer(buffer)
+            return gps_array_buffer
 
     def generate_candidate_link(self, net: Net = None) -> tuple[pd.DataFrame, list[int]]:
         """
         计算GPS观测点的候选路段
         :param net:
         :return: GPS候选路段信息, 未匹配到候选路段的gps点id
         """
@@ -330,16 +334,15 @@
             candidate_link.drop(columns=['index_right', 'gps_buffer'], axis=1, inplace=True)
             for col in [net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD,
                         net_field.SINGLE_LINK_ID_FIELD, net_field.DIRECTION_FIELD]:
                 candidate_link[col] = candidate_link[col].astype(int)
             # add link geo
             single_link_gdf.rename(columns={net_field.GEOMETRY_FIELD: 'single_link_geo'}, inplace=True)
             candidate_link = pd.merge(candidate_link,
-                                      single_link_gdf[[net_field.SINGLE_LINK_ID_FIELD, 'single_link_geo',
-                                                       net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD]],
+                                      single_link_gdf[[net_field.SINGLE_LINK_ID_FIELD, 'single_link_geo']],
                                       on=net_field.SINGLE_LINK_ID_FIELD, how='left')
             candidate_link.reset_index(inplace=True, drop=True)
         return candidate_link, remain_gps_list
 
     def to_plane_prj(self) -> None:
         if self.__gps_points_gdf.crs.srs == self.plane_crs:
             self.__crs = self.plane_crs
@@ -402,15 +405,15 @@
         return self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD].to_list()
 
     def del_dwell_points(self) -> None:
         # add field = dis_gap_field
         self.calc_adj_dis_gap()
         self.__gps_points_gdf['dwell_label'] = \
             (self.__gps_points_gdf[dis_gap_field] > self.dwell_l_length).astype(int)
-
+        self.__gps_points_gdf.loc[len(self.__gps_points_gdf) - 1, 'dwell_label'] = 1
         self.__gps_points_gdf = self.del_consecutive_zero(df=self.__gps_points_gdf, col='dwell_label', n=self.dwell_n)
         try:
             self.__gps_points_gdf.drop(columns=[sub_group_field], axis=1, inplace=True)
         except KeyError:
             pass
 
     @staticmethod
```

### Comparing `gotrackit-0.2.1/src/gotrackit/map/Link.py` & `gotrackit-0.2.2/src/gotrackit/map/Link.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,42 +79,26 @@
         :return:
         """
         self.create_single_link(link_gdf=self.link_gdf)
         self.__single_link_gdf.set_index(net_field.SINGLE_LINK_ID_FIELD, inplace=True)
         self.__single_link_gdf[net_field.SINGLE_LINK_ID_FIELD] = list(self.__single_link_gdf.index)
 
     def renew_length(self):
-        _idx = list(self.link_gdf.index)[0]
-        length_a, length_b = \
-            self.link_gdf.at[_idx, net_field.GEOMETRY_FIELD].length, self.link_gdf.at[_idx, net_field.LENGTH_FIELD]
-        if isinstance(length_a, (gpd.GeoSeries, pd.Series)):
-            if 0.8 <= max(length_a / length_b) <= 1.2:
-                return None
-        else:
-            if 0.8 <= length_a / length_b <= 1.2:
-                return None
         self.link_gdf[length_field] = self.link_gdf[geometry_field].length
 
-    def init_link_from_existing_single_link(self, single_link_gdf: gpd.GeoDataFrame = None):
+    def init_link_from_existing_single_link(self, single_link_gdf: gpd.GeoDataFrame = None,
+                                            ft_link_mapping: dict = None,
+                                            double_single_mapping: dict = None, link_ft_mapping: dict = None):
         """通过给定的single_link_gdf初始化link, 用在子net的初始化上"""
         self.__single_link_gdf = single_link_gdf.copy()
-        self.__double_single_mapping = {single_link_id: (link_id, int(direction), f, t) for
-                                        single_link_id, link_id, direction, f, t in
-                                        zip(self.__single_link_gdf[net_field.SINGLE_LINK_ID_FIELD],
-                                            self.__single_link_gdf[net_field.LINK_ID_FIELD],
-                                            self.__single_link_gdf[net_field.DIRECTION_FIELD],
-                                            self.__single_link_gdf[net_field.FROM_NODE_FIELD],
-                                            self.__single_link_gdf[net_field.TO_NODE_FIELD])}
-        self.__ft_link_mapping = {(f, t): single_link for f, t, single_link in
-                                  zip(self.__single_link_gdf[net_field.FROM_NODE_FIELD],
-                                      self.__single_link_gdf[net_field.TO_NODE_FIELD],
-                                      self.__single_link_gdf[net_field.SINGLE_LINK_ID_FIELD])}
 
+        self.__double_single_mapping = double_single_mapping
+        self.__ft_link_mapping = ft_link_mapping
         # single_link: (f, t)
-        self.__link_ft_mapping = {v: k for k, v in self.__ft_link_mapping.items()}
+        self.__link_ft_mapping = link_ft_mapping
 
     def create_single_link(self, link_gdf: gpd.GeoDataFrame):
         """
         基于原来路网创建单向路网, 并且建立映射表
         :return:
         """
         link_gdf[net_field.DIRECTION_FIELD] = link_gdf[net_field.DIRECTION_FIELD].astype(int)
@@ -125,14 +109,16 @@
             neg_link[[net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD]] = neg_link[
                 [net_field.TO_NODE_FIELD, net_field.FROM_NODE_FIELD]]
             neg_link[net_field.GEOMETRY_FIELD] = neg_link[net_field.GEOMETRY_FIELD].apply(
                 lambda line_geo: LineString(list(line_geo.coords)[::-1]))
             self.__single_link_gdf = pd.concat([link_gdf, neg_link])
             self.__single_link_gdf.reset_index(inplace=True, drop=True)
         self.__single_link_gdf[net_field.SINGLE_LINK_ID_FIELD] = [i for i in range(1, len(self.__single_link_gdf) + 1)]
+        self.__single_link_gdf['path'] = self.__single_link_gdf.apply(
+            lambda row: [row[net_field.FROM_NODE_FIELD], row[net_field.TO_NODE_FIELD]], axis=1)
         self.__double_single_mapping = {single_link_id: (link_id, int(direction), f, t) for
                                         single_link_id, link_id, direction, f, t in
                                         zip(self.__single_link_gdf[net_field.SINGLE_LINK_ID_FIELD],
                                             self.__single_link_gdf[net_field.LINK_ID_FIELD],
                                             self.__single_link_gdf[net_field.DIRECTION_FIELD],
                                             self.__single_link_gdf[net_field.FROM_NODE_FIELD],
                                             self.__single_link_gdf[net_field.TO_NODE_FIELD])}
@@ -389,15 +375,15 @@
             return self.link_gdf[self.link_gdf[to_node_field].isin(node_list)][link_id_field].to_list()
 
     def link_series(self, link_id: int = None) -> gpd.GeoSeries:
         return self.link_gdf.loc[link_id, :].copy()
 
     @property
     def link_ft_map(self) -> dict[int, tuple[int, int]]:
-        return self.__link_ft_mapping.copy()
+        return self.__link_ft_mapping
 
     def vertex_degree(self, node: int = None) -> int:
         """无向图的节点度"""
         return self.__ud_graph.degree[node]
 
     def used_node(self) -> set[int]:
         return set(self.link_gdf[from_node_field]) | set(self.link_gdf[to_node_field])
```

### Comparing `gotrackit-0.2.1/src/gotrackit/map/Net.py` & `gotrackit-0.2.2/src/gotrackit/map/Net.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 # @Time    : 2023/12/10 20:02
 # @Author  : TangKai
 # @Team    : ZheChengData
 
 """
 路网信息存储与相关方法
 """
-
+import os
+import pickle
 import numpy as np
 import pandas as pd
+import multiprocessing
 from .Link import Link
 from .Node import Node
 import networkx as nx
 import geopandas as gpd
+from ..tools.group import cut_group
 from shapely.geometry import LineString
 from ..tools.geo_process import prj_inf
 from ..tools.save_file import save_file
 from ..GlobalVal import NetField, PrjConst
 from ..WrapsFunc import function_time_cost
 from shapely.geometry import Polygon, Point
 from ..tools.geo_process import divide_line_by_l
@@ -28,44 +31,80 @@
 link_id_field = net_field.LINK_ID_FIELD
 dir_field = net_field.DIRECTION_FIELD
 from_node_field = net_field.FROM_NODE_FIELD
 to_node_field = net_field.TO_NODE_FIELD
 length_field = net_field.LENGTH_FIELD
 geometry_field = net_field.GEOMETRY_FIELD
 node_id_field = net_field.NODE_ID_FIELD
+path_field = net_field.NODE_PATH_FIELD
+cost_field = net_field.COST_FIELD
+o_node_field, d_node_field = net_field.S_NODE, net_field.T_NODE
 
 
 class Net(object):
 
     @function_time_cost
     def __init__(self, link_path: str = None, node_path: str = None, link_gdf: gpd.GeoDataFrame = None,
                  node_gdf: gpd.GeoDataFrame = None, weight_field: str = 'length', init_from_existing: bool = False,
                  is_check: bool = True, create_single: bool = True, search_method: str = 'dijkstra',
-                 not_conn_cost: float = 999.0, cache_path: bool = True, cache_id: bool = True):
+                 ft_link_mapping: dict = None, double_single_mapping: dict = None, link_ft_mapping: dict = None,
+                 not_conn_cost: float = 999.0, cache_path: bool = True, cache_id: bool = True,
+                 is_sub_net: bool = False, fmm_cache: bool = False, cache_cn: int = 2, cache_slice: int = None,
+                 fmm_cache_fldr: str = None,
+                 cache_name: str = 'cache', recalc_cache: bool = True,
+                 cut_off: float = 1200.0, max_cut_off: float = 5000.0):
         """
         创建Net类
         :param link_path: link层的路网文件路径, 若指定了该参数, 则直接从磁盘IO创建Net线层
         :param node_path: node层的路网文件路径, 若指定了该参数, 则直接从磁盘IO创建Net点层
         :param link_gdf: 若指定了该参数, 则直接从内存中的gdf创建Net线层
         :param node_gdf: 若指定了该参数, 则直接从内存中的gdf创建Net点层
         :param weight_field: 搜路权重字段
         :param create_single: 是否在初始化的时候创建single层
-        :param search_method: 路径搜索方法, 'dijkstra' or 'bellman-ford'
+        :param search_method: 路径搜索方法, 'dijkstra'
         :param init_from_existing: 是否直接从内存中的gdf创建single_link_gdf, 该参数用于类内部创建子net, 用户不用关心该参数, 使用默认值即可
-        :param not_conn_cost: 不连通路径的阻抗(m)
+        :param double_single_mapping:
+        :param link_ft_mapping:
+        :param ft_link_mapping:
+        :param not_conn_cost: 不连通路径的阻抗(m), 默认999.0米
+        :param is_sub_net: 是否是子网络, 默认False
+        :param fmm_cache: 是否启用路径预存储, 默认False
+        :param cache_cn: 使用几个核能进行路径预计算, 默认2
+        :param fmm_cache_fldr: 存储路径预处理结果的文件目录, 默认./
+        :param recalc_cache: 是否重新计算FMM路径缓存, 默认True
+        :param cache_slice: 对于缓存切片转换存储(防止大规模路网导致内存溢出)
+        :param cut_off: 路径搜索截断长度, 米, 默认1000m
+        :param max_cut_off: 最大路径搜索截断长度, 如果在cut_off截断半径下, 没有搜索出任何路径的节点会使用这个长度再次进行搜索, 默认5000米
+        :param cache_name: 路径预存储的标志名称, 默认cache
+
         """
         self.not_conn_cost = not_conn_cost
         self.geo_crs = geo_crs
         self.search_method = search_method
         self.weight_field = weight_field
         self.all_pair_path_df = pd.DataFrame()
-        self.__stp_cache = dict()
-        self.__done_path_cost = dict()
+        self.__stp_cache = dict() or pd.DataFrame
+        self.__done_path_cost = dict() or pd.DataFrame
+        self.__done_stp_cost_df = pd.DataFrame()
+        self.__cache_prj_inf = dict()
         self.cache_path = cache_path
         self.cache_id = cache_id
+        self.__is_sub_net = is_sub_net
+        self.fmm_cache = fmm_cache
+        self.cut_off = cut_off
+        self.max_cut_off = max_cut_off
+        if cache_cn > os.cpu_count():
+            cache_cn = os.cpu_count()
+        self.cache_cn = cache_cn
+        self.cache_name = cache_name
+        self.fmm_cache_fldr = fmm_cache_fldr
+        self.recalc_cache = recalc_cache
+        self.cache_slice = cache_slice
+        if self.cache_slice is None:
+            self.cache_slice = 2 * self.cache_cn
 
         if node_gdf is None:
             self.__node = Node(node_gdf=gpd.read_file(node_path), is_check=is_check, init_available_node=self.cache_id)
         else:
             self.__node = Node(node_gdf=node_gdf, is_check=is_check, init_available_node=self.cache_id)
 
         if link_gdf is None:
@@ -74,50 +113,75 @@
                                not_conn_cost=self.not_conn_cost)
         else:
             self.__link = Link(link_gdf=link_gdf, weight_field=self.weight_field, is_check=is_check,
                                planar_crs=self.__node.planar_crs, init_available_link=self.cache_id,
                                not_conn_cost=self.not_conn_cost)
         self.__planar_crs = self.__node.planar_crs
         self.to_plane_prj()
-        try:
+        if not self.is_sub_net:
             self.__link.renew_length()
-        except:
-            pass
         if not init_from_existing:
             if create_single:
                 self.__link.init_link()
         else:
             if create_single:
-                self.__link.init_link_from_existing_single_link(single_link_gdf=link_gdf)
+                # for sub net
+                self.__link.init_link_from_existing_single_link(single_link_gdf=link_gdf,
+                                                                double_single_mapping=double_single_mapping,
+                                                                ft_link_mapping=ft_link_mapping,
+                                                                link_ft_mapping=link_ft_mapping)
         if not init_from_existing:
             self.__node.init_node()
         else:
             pass
         if is_check:
             self.check()
+
     @property
     def planar_crs(self):
         return self.__planar_crs
 
     @planar_crs.setter
     def planar_crs(self, val):
         self.__planar_crs = val
         self.__link.planar_crs = val
         self.__node.planar_crs = val
 
+    @property
+    def is_sub_net(self) -> bool:
+        return self.__is_sub_net
+
+    def get_path_cache(self) -> pd.DataFrame:
+        return self.__done_stp_cost_df
+
+    def set_path_cache(self, stp_cost_df: pd.DataFrame = None) -> None:
+        self.__done_stp_cost_df = stp_cost_df
+
+    def get_prj_cache(self) -> dict:
+        return self.__cache_prj_inf
+
+    def set_prj_cache(self, cache_prj_inf: dict = None) -> None:
+        self.__cache_prj_inf = cache_prj_inf
+
     def check(self) -> None:
         """检查点层线层的关联一致性"""
         node_set = set(self.__node.get_node_data().index)
         link_node_set = set(self.__link.get_bilateral_link_data()[net_field.FROM_NODE_FIELD]) | \
                         set(self.__link.get_bilateral_link_data()[net_field.TO_NODE_FIELD])
         assert link_node_set.issubset(node_set), 'Link层中部分节点在Node层中没有记录'
 
-    @function_time_cost
-    def init_net(self) -> None:
+    def init_net(self, stp_cost_cache_df: pd.DataFrame = None, cache_prj_inf: dict = None) -> None:
         self.__link.create_graph(weight_field=self.weight_field)
+        if self.fmm_cache:
+            if self.is_sub_net:
+                self.set_path_cache(stp_cost_cache_df)
+                self.set_prj_cache(cache_prj_inf)
+            else:
+                self.fmm_path_cache()
+                self.cache_prj_info()
 
     def search(self, o_node: int = None, d_node: int = None) -> tuple[list, float]:
         """
 
         :param o_node:
         :param d_node:
         :return:
@@ -252,37 +316,48 @@
     def available_link_id(self) -> int:
         return self.__link.available_link_id
 
     def get_ft_node_link_mapping(self):
         return self.__link.get_ft_link_mapping()
 
     @function_time_cost
-    def create_computational_net(self, gps_array_buffer:Polygon = None):
+    def create_computational_net(self, gps_array_buffer: Polygon = None, weight_field: str = 'length',
+                                 cache_path: bool = True, cache_id: bool = True, not_conn_cost: float = 999.0,
+                                 fmm_cache: bool = False):
         """
 
         :param gps_array_buffer:
+        :param weight_field:
+        :param cache_path:
+        :param cache_id:
+        :param not_conn_cost:
+        :param fmm_cache:
         :return:
         """
+        if gps_array_buffer is None:
+            return None
         gps_array_buffer_gdf = gpd.GeoDataFrame({'geometry': [gps_array_buffer]}, geometry='geometry',
                                                 crs=self.planar_crs)
         sub_single_link_gdf = gpd.sjoin(self.get_link_data(), gps_array_buffer_gdf)
         if sub_single_link_gdf.empty:
             raise ValueError(rf'GPS数据在指定的buffer范围内关联不到任何路网数据...')
         sub_single_link_gdf.drop(columns=['index_right'], axis=1, inplace=True)
         sub_single_link_gdf.drop_duplicates(subset=[net_field.SINGLE_LINK_ID_FIELD], inplace=True)
         sub_node_list = list(set(sub_single_link_gdf[net_field.FROM_NODE_FIELD]) | \
                              set(sub_single_link_gdf[net_field.TO_NODE_FIELD]))
         sub_node_gdf = self.__node.get_node_data().loc[sub_node_list, :].copy()
         sub_net = Net(link_gdf=sub_single_link_gdf,
                       node_gdf=sub_node_gdf,
-                      weight_field=self.weight_field,
-                      init_from_existing=True, is_check=False,
-                      search_method=self.search_method, cache_path=self.cache_path, cache_id=self.cache_id,
-                      not_conn_cost=self.not_conn_cost)
-        sub_net.init_net()
+                      weight_field=weight_field,
+                      init_from_existing=True, is_check=False, cache_path=cache_path, cache_id=cache_id,
+                      not_conn_cost=not_conn_cost, is_sub_net=True, fmm_cache=fmm_cache,
+                      ft_link_mapping=self.get_ft_node_link_mapping(),
+                      link_ft_mapping=self.link_ft_map,
+                      double_single_mapping=self.bilateral_unidirectional_mapping, cut_off=self.cut_off)
+        sub_net.init_net(stp_cost_cache_df=self.get_path_cache(), cache_prj_inf=self.get_prj_cache())
         return sub_net
 
     @property
     def graph(self) -> nx.DiGraph:
         return self.__link.get_graph()
 
     @property
@@ -487,8 +562,156 @@
         if is_init_link:
             self.check()
             self.__link.init_link()
             self.__node.init_node()
 
     def get_greater_than_threshold(self, l_threshold: float = None) -> set[int]:
         link_gdf = self.__link.link_gdf
-        return set(link_gdf[link_gdf[length_field] > l_threshold][link_id_field])
+        return set(link_gdf[link_gdf[length_field] > l_threshold][link_id_field])
+
+    @function_time_cost
+    def fmm_path_cache(self):
+        if self.fmm_cache_fldr is None:
+            self.fmm_cache_fldr = r'./'
+        if not self.recalc_cache:
+            try:
+                with open(os.path.join(self.fmm_cache_fldr, rf'{self.cache_name}_path_cache'), 'rb') as f:
+                    done_stp_cache_df = pickle.load(f)
+                self.set_path_cache(done_stp_cache_df)
+                print(rf'using local fmm cache...')
+                return None
+            except Exception as e:
+                print(repr(e))
+
+        link = self.__link.get_bilateral_link_data()
+        g = self.graph
+        node_list = list(set(link[net_field.FROM_NODE_FIELD]) | set(link[net_field.TO_NODE_FIELD]))
+        del link
+        print(rf'calc fmm cache...')
+        if self.cache_cn <= 1:
+            done_stp_cost_df = self.single_source_cache(node_list, g, self.cut_off, self.weight_field, self.cache_slice)
+        else:
+            done_stp_cost_df = pd.DataFrame()
+            node_group = cut_group(obj_list=node_list, n=self.cache_cn)
+            pool = multiprocessing.Pool(processes=len(node_group))
+            result_list = []
+            for i in range(0, len(node_group)):
+                result = pool.apply_async(self.single_source_cache,
+                                          args=(node_group[i], g, self.cut_off, self.weight_field, self.cache_slice))
+                result_list.append(result)
+            pool.close()
+            pool.join()
+            for res in result_list:
+                done_stp_cost_df = pd.concat([done_stp_cost_df, res.get()])
+            done_stp_cost_df.reset_index(inplace=True, drop=False)
+        _ = self.__link.get_link_data()[[net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD,
+                                         self.weight_field]].rename(
+            columns={net_field.FROM_NODE_FIELD: o_node_field, net_field.TO_NODE_FIELD: d_node_field,
+                     self.weight_field: cost_field})
+        _[path_field] = _.apply(lambda row: [int(row[o_node_field]), int(row[d_node_field])], axis=1)
+        done_stp_cost_df = pd.concat([_, done_stp_cost_df])
+        del _
+        done_stp_cost_df.drop_duplicates(subset=[o_node_field, d_node_field], keep='first', inplace=True)
+        done_stp_cost_df.reset_index(inplace=True, drop=True)
+        with open(os.path.join(self.fmm_cache_fldr, rf'{self.cache_name}_path_cache'), 'wb') as f:
+            pickle.dump(done_stp_cost_df, f)
+        self.set_path_cache(done_stp_cost_df)
+
+    @staticmethod
+    def slice_save(done_stp_cache: dict = None, done_cost_cache: dict = None, n: int = 3) -> pd.DataFrame:
+        temp_stp_list = [{} for i in range(n)]
+        temp_cost_list = [{} for i in range(n)]
+        _ = [temp_stp_list[i % n].update({key: done_stp_cache[key]}) for i, key in enumerate(done_stp_cache.keys())]
+        _ = [temp_cost_list[i % n].update({key: done_cost_cache[key]}) for i, key in enumerate(done_cost_cache.keys())]
+
+        stp_cost_res = pd.DataFrame()
+        del done_stp_cache, done_cost_cache
+        for stp_cache, cost_cache in zip(temp_stp_list, temp_cost_list):
+            done_stp_cache_df = pd.DataFrame(stp_cache).stack().reset_index(drop=False).rename(
+                columns={'level_0': d_node_field, 'level_1': o_node_field, 0: path_field})
+            done_stp_cache_df.dropna(subset=[o_node_field, d_node_field], how='any', inplace=True)
+
+            done_cost_cache_df = pd.DataFrame(cost_cache).stack().reset_index(drop=False).rename(
+                columns={'level_0': d_node_field, 'level_1': o_node_field, 0: cost_field})
+            done_cost_cache_df.dropna(subset=[o_node_field, d_node_field], how='any', inplace=True)
+            done_cost_cache_df[cost_field] = np.around(done_cost_cache_df[cost_field], decimals=1)
+
+            stp_cost_cache_df = pd.merge(done_cost_cache_df, done_stp_cache_df, on=[o_node_field, d_node_field])
+            del done_stp_cache_df, done_cost_cache_df
+            stp_cost_res = pd.concat([stp_cost_res, stp_cost_cache_df])
+            del stp_cost_cache_df
+        stp_cost_res.reset_index(inplace=True, drop=True)
+        return stp_cost_res
+
+    def single_source_cache(self, node_list: list = None, g: nx.DiGraph = None,
+                            cut_off: float = 500.0, weight_field: str = 'length', n: int = 2) -> pd.DataFrame:
+        done_cost_cache, done_stp_cache = {}, {}
+        for node in node_list:
+            try:
+                done_cost_cache[node], done_stp_cache[node] = nx.single_source_dijkstra(g, node, weight=weight_field,
+                                                                                        cutoff=cut_off)
+            except nx.exception.NodeNotFound as e:
+                print(repr(e))
+
+        done_stp_cost_df = self.slice_save(done_stp_cache=done_stp_cache,
+                                           done_cost_cache=done_cost_cache,
+                                           n=n)
+        return done_stp_cost_df
+
+    def single_link_ft_cost(self) -> pd.DataFrame:
+        return self.__link.get_link_data()[
+            [net_field.SINGLE_LINK_ID_FIELD, net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD, self.weight_field,
+             'path']].copy()
+
+    def cache_prj_info(self):
+        if self.fmm_cache_fldr is None:
+            self.fmm_cache_fldr = r'./'
+        if not self.recalc_cache:
+            try:
+                with open(os.path.join(self.fmm_cache_fldr, rf'{self.cache_name}_prj'), 'rb') as f:
+                    cache_prj_inf = pickle.load(f)
+                self.set_prj_cache(cache_prj_inf)
+                return None
+            except Exception as e:
+                print(repr(e))
+
+        single_link_gdf = self.__link.get_link_data()
+        single_link_gdf = single_link_gdf[
+            [net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD, net_field.GEOMETRY_FIELD, net_field.LENGTH_FIELD]].copy()
+        cache_prj_gdf = self.split_segment(single_link_gdf)
+        cache_prj_gdf[['f_loc', 't_loc']] = cache_prj_gdf.apply(lambda row: list(row['geometry'].coords), axis=1,
+                                                                result_type='expand')
+        cache_prj_gdf[net_field.LINK_VEC_FIELD] = cache_prj_gdf.apply(
+            lambda row: np.array(row['t_loc']) - np.array(row['f_loc']), axis=1)
+        cache_prj_gdf.drop(columns=['f_loc', 't_loc', net_field.GEOMETRY_FIELD], axis=1, inplace=True)
+        cache_prj_gdf[net_field.SEG_COUNT] = \
+            cache_prj_gdf.groupby([net_field.FROM_NODE_FIELD,
+                                   net_field.TO_NODE_FIELD])[net_field.LINK_VEC_FIELD].transform('count')
+        cache_prj_inf = {1: cache_prj_gdf[cache_prj_gdf[net_field.SEG_COUNT] == 1].copy().reset_index(drop=True),
+                         2: cache_prj_gdf[cache_prj_gdf[net_field.SEG_COUNT] > 1].copy().reset_index(drop=True)}
+        del cache_prj_gdf
+        self.set_prj_cache(cache_prj_inf)
+        with open(os.path.join(self.fmm_cache_fldr, rf'{self.cache_name}_prj'), 'wb') as f:
+            pickle.dump(cache_prj_inf, f)
+
+    @staticmethod
+    def split_segment(path_gdf: gpd.GeoDataFrame = None) -> gpd.GeoDataFrame:
+        """
+        拆解轨迹坐标, 并且粗去重(按照路段的起终点坐标)
+        :param path_gdf: gpd.GeoDataFrame(), 必需参数, 必须字段: [geometry], crs要求EPSG:4326
+        :return: gpd.GeoDataFrame(),
+        """
+        origin_crs = path_gdf.crs.srs
+        path_gdf['point_list'] = path_gdf[net_field.GEOMETRY_FIELD].apply(lambda x: list(x.coords))
+        path_gdf['line_list'] = path_gdf['point_list'].apply(
+            lambda x: [LineString((x[i], x[i + 1])) for i in range(0, len(x) - 1)])
+        path_gdf['topo_seq'] = path_gdf['line_list'].apply(lambda x: [i for i in range(len(x))])
+        path_gdf.drop(columns=[net_field.GEOMETRY_FIELD, 'point_list'], axis=1, inplace=True)
+        path_gdf = pd.DataFrame(path_gdf)
+        path_gdf = path_gdf.explode(column=['line_list', 'topo_seq'], ignore_index=True)
+        path_gdf.rename(columns={'line_list': net_field.GEOMETRY_FIELD}, inplace=True)
+        path_gdf = gpd.GeoDataFrame(path_gdf, crs=origin_crs, geometry=net_field.GEOMETRY_FIELD)
+        path_gdf['__l__'] = path_gdf[net_field.GEOMETRY_FIELD].length
+        path_gdf[net_field.SEG_ACCU_LENGTH] = \
+            path_gdf.groupby([net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD])[['__l__']].cumsum()
+        del path_gdf['__l__']
+        return path_gdf
```

### Comparing `gotrackit-0.2.1/src/gotrackit/map/Node.py` & `gotrackit-0.2.2/src/gotrackit/map/Node.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/model/Markov.py` & `gotrackit-0.2.2/src/gotrackit/model/Markov.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 # -- coding: utf-8 --
 # @Time    : 2023/12/9 8:29
 # @Author  : TangKai
 # @Team    : ZheChengData
 
 """Markov Model Class"""
 
-import time
 import os.path
-import datetime
 import warnings
 import numpy as np
 import pandas as pd
 import networkx as nx
-import multiprocessing
 import geopandas as gpd
 from ..map.Net import Net
-from itertools import chain
 from datetime import timedelta
-from ..tools.group import cut_group
 from ..solver.Viterbi import Viterbi
 from ..gps.LocGps import GpsPointsGdf
 from ..tools.geo_process import prj_inf
 from ..WrapsFunc import function_time_cost
 from shapely.geometry import Point, LineString
 from ..GlobalVal import NetField, GpsField, MarkovField
 from ..tools.geo_process import n_equal_points, hmm_vector_angle
@@ -30,39 +25,43 @@
 gps_field = GpsField()
 net_field = NetField()
 markov_field = MarkovField()
 
 from_link_f, to_link_f = markov_field.FROM_STATE, markov_field.TO_STATE
 from_link_n_f, to_link_n_f = markov_field.FROM_STATE_N, markov_field.TO_STATE_N
 from_gps_f, to_gps_f = gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ
+path_field = net_field.NODE_PATH_FIELD
+cost_field = net_field.COST_FIELD
+o_node_field, d_node_field = net_field.S_NODE, net_field.T_NODE
 MIN_P = 1e-10
 
 
 class HiddenMarkov(object):
     """隐马尔可夫模型类"""
 
     def __init__(self, net: Net, gps_points: GpsPointsGdf, beta: float = 30.1, gps_sigma: float = 20.0,
                  not_conn_cost: float = 999.0, use_heading_inf: bool = True, heading_para_array: np.ndarray = None,
-                 dis_para: float = 0.1, top_k: int = 25, omitted_l: float = 6.0, multi_core: bool = True,
-                 core_num: int = 1):
+                 dis_para: float = 0.1, top_k: int = 25, omitted_l: float = 6.0):
         self.gps_points = gps_points
         self.net = net
         # (gps_seq, single_link_id): (prj_p, prj_dis, route_dis)
         self.__done_prj_dict: dict[tuple[int, int]: tuple[Point, float, float, float, np.ndarray]] = dict()
+        self.__done_prj_df: gpd.GeoDataFrame or pd.DataFrame = None
         self.__adj_seq_path_dict: dict[tuple[int, int], list[int, int]] = dict()
         self.__ft_transition_dict = dict()
         self.__ft_mapping_dict = dict()
+        self.__ft_idx_map = pd.DataFrame()
         self.beta = beta
         self.gps_sigma = gps_sigma
         self.__emission_mat_dict = dict()
         self.__solver = None
         self.index_state_list = None
         self.gps_match_res_gdf = None
         # {(from_seq, to_seq): pd.DataFrame()}
-        self.__s2s_route_l = dict()
+        self.__s2s_route_l = pd.DataFrame()
         self.__plot_mix_gdf, self.__base_link_gdf, self.__base_node_gdf, self.__may_error = None, None, None, None
         self.path_cost_df = pd.DataFrame()
         self.is_warn = False
         self.not_conn_cost = not_conn_cost
         self.use_heading_inf = use_heading_inf
         if heading_para_array is None:
             self.heading_para_array = np.array([1.0, 1.0, 1.0, 0.1, 0.0001, 0.0001, 0.00001, 0.000001, 0.000001])
@@ -70,94 +69,40 @@
             self.heading_para_array = heading_para_array
         self.angle_slice = 180 / len(self.heading_para_array)
         self.dis_para = dis_para
         self.warn_info = {'from_ft': [], 'to_ft': []}
         self.format_warn_info = pd.DataFrame()
         self.top_k = top_k
         self.omitted_l = omitted_l
-        self.multi_core = multi_core
-        self.core_num = int(core_num) if int(core_num) <= os.cpu_count() else os.cpu_count()
         self.gps_candidate_link = None
 
     @function_time_cost
-    def generate_markov_para(self):
-        if self.multi_core and self.core_num >= 1:
-            self.__generate_transition_mat_alpha_multi()
-        else:
-            self.__generate_transition_mat()
-        self.__generate_emission_mat()
-
-    def __generate_transition_mat(self):
-
-        # 计算 初步候选
-        seq_list = self.__generate_candidates()
-
-        self.gps_points.calc_gps_point_dis()
-        # _ = pd.DataFrame()
-        # 计算状态转移概率矩阵
-        for i in range(0, len(seq_list) - 1):
-            from_link = self.gps_candidate_link[self.gps_candidate_link[gps_field.POINT_SEQ_FIELD] == seq_list[i]][
-                net_field.SINGLE_LINK_ID_FIELD].to_list()
-            to_link = self.gps_candidate_link[self.gps_candidate_link[gps_field.POINT_SEQ_FIELD] == seq_list[i + 1]][
-                net_field.SINGLE_LINK_ID_FIELD].to_list()
-
-            transition_df = pd.DataFrame([[int(f), int(t)] for f in from_link for t in to_link],
-                                         columns=[markov_field.FROM_STATE,
-                                                  markov_field.TO_STATE])
-
-            transition_df[markov_field.ROUTE_LENGTH] = \
-                transition_df.apply(
-                    lambda item: self.calc_route_length(from_gps_seq=seq_list[i],
-                                                        to_gps_seq=seq_list[i + 1],
-                                                        from_link_id=item[markov_field.FROM_STATE],
-                                                        to_link_id=item[markov_field.TO_STATE]), axis=1)
-
-            transition_df[markov_field.DIS_GAP] = np.abs(-transition_df[
-                markov_field.ROUTE_LENGTH] + self.gps_points.get_gps_point_dis((seq_list[i], seq_list[i + 1])))
-
-            # _ = pd.concat([_, transition_df])
-            self.__s2s_route_l[(seq_list[i], seq_list[i + 1])] = transition_df[
-                [markov_field.FROM_STATE, markov_field.TO_STATE, markov_field.ROUTE_LENGTH]].copy().set_index(
-                [markov_field.FROM_STATE, markov_field.TO_STATE])
-
-            # 转成matrix
-            transition_mat = transition_df[
-                [markov_field.FROM_STATE, markov_field.TO_STATE, markov_field.DIS_GAP]].set_index(
-                [markov_field.FROM_STATE, markov_field.TO_STATE]).unstack().values
-
-            # 索引映射
-            f_mapping, t_mapping = {i: f for i, f in zip(range(len(from_link)), sorted(from_link))}, \
-                {i: t for i, t in zip(range(len(to_link)), sorted(to_link))}
-            transition_mat = self.transition_probability(self.beta, transition_mat, self.dis_para)
-
-            self.__ft_transition_dict[seq_list[i]] = transition_mat
-            self.__ft_mapping_dict[seq_list[i]] = f_mapping
-            self.__ft_mapping_dict[seq_list[i + 1]] = t_mapping
+    def generate_markov_para(self, add_single_ft: list[bool] = None) -> bool:
 
-        # print(_)
+        is_success = self.__generate_transition_mat_alpha_multi(add_single_ft)
+        if is_success:
+            self.__generate_emission_mat()
+        return is_success
 
     def __generate_emission_mat(self):
 
         # 计算每个观测点的生成概率, 这是在计算状态转移概率之后, 已经将关联不到的GPS点删除了
         # 这里的向量是候选路段的投影点的方向向量
-        emission_p_df = pd.DataFrame(self.__done_prj_dict).T.reset_index(drop=False).rename(
-            columns={'level_0': gps_field.POINT_SEQ_FIELD, 'level_1': net_field.SINGLE_LINK_ID_FIELD,
-                     1: markov_field.PRJ_L, 4: net_field.LINK_VEC_FIELD})[
-            [gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD, markov_field.PRJ_L, net_field.LINK_VEC_FIELD]]
-
+        emission_p_df = self.__done_prj_df.copy()
+        emission_p_df.rename(columns={'p_vec': net_field.LINK_VEC_FIELD}, inplace=True)
         if self.use_heading_inf:
             self.gps_points.calc_diff_heading()
             emission_p_df = pd.merge(emission_p_df, self.gps_points.gps_gdf[[gps_field.POINT_SEQ_FIELD,
                                                                              gps_field.DIFF_VEC]], how='left',
                                      on=gps_field.POINT_SEQ_FIELD)
             emission_p_df[markov_field.HEADING_GAP] = \
-                emission_p_df.apply(
-                    lambda row: hmm_vector_angle(gps_diff_vec=row[gps_field.DIFF_VEC],
-                                                 link_dir_vec=row[net_field.LINK_VEC_FIELD], omitted_l=self.omitted_l),
-                    axis=1)
+                [hmm_vector_angle(gps_diff_vec=diff_vec,
+                                  link_dir_vec=link_vec,
+                                  omitted_l=self.omitted_l) for diff_vec, link_vec in
+                 zip(emission_p_df[gps_field.DIFF_VEC], emission_p_df[net_field.LINK_VEC_FIELD])]
         else:
             emission_p_df[markov_field.HEADING_GAP] = 0
         emission_p_df[markov_field.HEADING_GAP] = emission_p_df[markov_field.HEADING_GAP].astype(object)
         emission_p_df[markov_field.PRJ_L] = emission_p_df[markov_field.PRJ_L].astype(object)
         emission_p_df.sort_values(by=[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD],
                                   ascending=[True, True], inplace=True)
         emission_p_df = emission_p_df.groupby([gps_field.POINT_SEQ_FIELD]).agg(
@@ -173,441 +118,410 @@
 
     def __generate_candidates(self) -> list[int]:
         # 初步依据gps点buffer得到候选路段, 关联不到的GPS点删除掉
         # seq, geometry, single_link_id, from_node, to_node, dir, length
         gps_candidate_link, _gap = self.gps_points.generate_candidate_link(net=self.net)
 
         if gps_candidate_link.empty:
-            raise ValueError(r'GPS数据样本点无法关联到任何路段, 请检查路网完整性或者增加gps_buffer参数...')
+            print(r'GPS数据样本点无法关联到任何路段, 请检查路网完整性或者增加gps_buffer参数')
+            return list()
 
         if _gap:
             warnings.warn(rf'seq为: {_gap}的GPS点没有关联到任何候选路段..., 不会用于路径匹配计算...')
             # 删除关联不到任何路段的gps点
             self.gps_points.delete_target_gps(target_seq_list=list(_gap))
 
         # 一定要排序
         seq_list = sorted(list(gps_candidate_link[gps_field.POINT_SEQ_FIELD].unique()))
         if len(seq_list) <= 1:
-            raise ValueError(
-                r'经过路段关联, 删除掉无法关联到路段的GPS点后, GPS数据样本点不足2个, 请检查路网完整性或者增加gps_buffer参数...')
+            print(r'经过路段关联, 删除掉无法关联到路段的GPS点后, GPS数据样本点不足2个, 请检查路网完整性或者增加gps_buffer参数')
+            return list()
         self.gps_candidate_link = gps_candidate_link
         return seq_list
 
-    @staticmethod
-    def filter_k_candidates(preliminary_candidate_link: gpd.GeoDataFrame or pd.DataFrame = None,
-                            top_k: int = 10) -> tuple[gpd.GeoDataFrame or pd.DataFrame, dict]:
+    def filter_k_candidates(self, preliminary_candidate_link: gpd.GeoDataFrame or pd.DataFrame = None,
+                            top_k: int = 10, using_cache: bool = True,
+                            cache_prj_inf: dict = None) -> gpd.GeoDataFrame or pd.DataFrame:
         """
         对Buffer范围内的初步候选路段进行二次筛选, 需按照投影距离排名前K位, 并且得到计算发射概率需要的数据
         :param preliminary_candidate_link:
         :param top_k
+        :param using_cache
+        :param cache_prj_inf
         :return:
         """
-        preliminary_candidate_link[
-            ['prj_p', 'prj_dis', 'route_dis', 'l_length', 'split_line', 'p_vec']] = preliminary_candidate_link.apply(
-            lambda row: prj_inf(p=row[gps_field.GEOMETRY_FIELD], line=row['single_link_geo']), axis=1,
-            result_type='expand')
-        del preliminary_candidate_link['split_line']
-        preliminary_candidate_link.sort_values(by=[gps_field.POINT_SEQ_FIELD, 'prj_dis'], ascending=[True, True],
+        preliminary_candidate_link.reset_index(inplace=True, drop=True)
+        preliminary_candidate_link['quick_stl'] = preliminary_candidate_link[gps_field.GEOMETRY_FIELD].shortest_line(
+            preliminary_candidate_link['single_link_geo']).length
+        preliminary_candidate_link.sort_values(by=[gps_field.POINT_SEQ_FIELD, 'quick_stl'], ascending=[True, True],
                                                inplace=True)
-        k_candidate_link = preliminary_candidate_link.groupby(gps_field.POINT_SEQ_FIELD).head(top_k)
-        k_candidate_link.reset_index(inplace=True, drop=True)
-        done_prj_dict = {
-            (gps_seq, single_link_id): (prj_p, prj_dis, route_dis, l_length, p_vec) for
-            gps_seq, single_link_id, prj_p, prj_dis, route_dis, l_length, p_vec in
-            zip(k_candidate_link[gps_field.POINT_SEQ_FIELD],
-                k_candidate_link[net_field.SINGLE_LINK_ID_FIELD],
-                k_candidate_link['prj_p'],
-                k_candidate_link['prj_dis'],
-                k_candidate_link['route_dis'],
-                k_candidate_link['l_length'],
-                k_candidate_link['p_vec'])}
-        return k_candidate_link, done_prj_dict
+        preliminary_candidate_link = preliminary_candidate_link.groupby(gps_field.POINT_SEQ_FIELD).head(
+            top_k).reset_index(drop=True)
+        if not using_cache:
+            prj_info_list = [prj_inf(p=geo, line=single_link_geo) for geo, single_link_geo in
+                             zip(preliminary_candidate_link[gps_field.GEOMETRY_FIELD],
+                                 preliminary_candidate_link['single_link_geo'])]
+            prj_df = pd.DataFrame(prj_info_list,
+                                  columns=['prj_p', 'prj_dis', 'route_dis', 'l_length', 'split_line', 'p_vec'])
+            del prj_df['split_line']
+            del preliminary_candidate_link['quick_stl']
+            preliminary_candidate_link = pd.merge(preliminary_candidate_link, prj_df, left_index=True, right_index=True)
+            k_candidate_link = preliminary_candidate_link
+            del prj_df
+            return k_candidate_link
+        else:
+            return self.filter_k_candidates_by_cache(preliminary_candidate_link=preliminary_candidate_link,
+                                                     cache_prj_inf=cache_prj_inf)
+
+    @staticmethod
+    def filter_k_candidates_by_cache(preliminary_candidate_link: gpd.GeoDataFrame or pd.DataFrame = None,
+                                     cache_prj_inf: dict = None) -> pd.DataFrame:
+        del preliminary_candidate_link[net_field.LENGTH_FIELD]
+        preliminary_candidate_link['route_dis'] = preliminary_candidate_link['single_link_geo'].project(
+            preliminary_candidate_link[gps_field.GEOMETRY_FIELD])
+        preliminary_candidate_link['prj_p'] = preliminary_candidate_link['single_link_geo'].interpolate(
+            preliminary_candidate_link['route_dis'])
+        if 1 in cache_prj_inf.keys():
+            cache_prj_gdf_a = cache_prj_inf[1]
+            preliminary_candidate_link = pd.merge(preliminary_candidate_link, cache_prj_gdf_a, how='left',
+                                                  on=[net_field.FROM_NODE_FIELD,
+                                                      net_field.TO_NODE_FIELD])
+            a_info = preliminary_candidate_link[~preliminary_candidate_link[net_field.SEG_ACCU_LENGTH].isna()].copy()
+            preliminary_candidate_link = preliminary_candidate_link[
+                preliminary_candidate_link[net_field.SEG_ACCU_LENGTH].isna()].copy()
+            preliminary_candidate_link.drop(columns=[net_field.SEG_ACCU_LENGTH, 'topo_seq', net_field.LENGTH_FIELD,
+                                                     'dir_vec', net_field.SEG_COUNT], axis=1, inplace=True)
+            del a_info[net_field.SEG_ACCU_LENGTH], a_info[net_field.SEG_COUNT], a_info['topo_seq']
+            if preliminary_candidate_link.empty:
+                a_info.rename(columns={'quick_stl': 'prj_dis', 'dir_vec': 'p_vec'}, inplace=True)
+                return a_info
+        else:
+            a_info = pd.DataFrame()
+
+        if 2 in cache_prj_inf.keys():
+            cache_prj_gdf_b = cache_prj_inf[2]
+            b_info = pd.merge(preliminary_candidate_link, cache_prj_gdf_b, how='inner', on=[net_field.FROM_NODE_FIELD,
+                                                                                            net_field.TO_NODE_FIELD])
+            b_info['ratio'] = b_info['route_dis'] / b_info[net_field.SEG_ACCU_LENGTH]
+
+            c_info = b_info[b_info['ratio'] >= 1].copy()
+            if not c_info.empty:
+                c_info.sort_values(by=[gps_field.POINT_SEQ_FIELD, net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD,
+                                       'topo_seq'], ascending=True)
+                c_info = c_info.groupby(
+                    [gps_field.POINT_SEQ_FIELD, net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD]).tail(n=1)
+                del c_info['topo_seq'], c_info['ratio'], c_info[net_field.SEG_ACCU_LENGTH]
+            d_info = b_info[b_info['ratio'] < 1].copy()
+            if not d_info.empty:
+                d_info['ck'] = \
+                    d_info.groupby([gps_field.POINT_SEQ_FIELD, net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD])[
+                    [net_field.FROM_NODE_FIELD]].transform('count')
+                d_info = d_info[d_info['ck'] == d_info[net_field.SEG_COUNT]].copy()
+
+                d_info = d_info.groupby(
+                    [gps_field.POINT_SEQ_FIELD, net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD]).head(n=1)
+                del d_info['ck'], d_info['topo_seq'], d_info['ratio'], d_info[net_field.SEG_ACCU_LENGTH]
+
+            preliminary_candidate_link = pd.concat([a_info, c_info, d_info])
+            preliminary_candidate_link.reset_index(inplace=True, drop=True)
+            preliminary_candidate_link.rename(columns={'quick_stl': 'prj_dis', 'dir_vec': 'p_vec'}, inplace=True)
+            return preliminary_candidate_link
+        else:
+            return a_info
 
     def solve(self, use_lop_p: bool = True):
         """
-
         :param use_lop_p: 是否使用对数概率, 避免浮点数精度下溢
         :return:
         """
 
         # 使用viterbi模型求解
         self.__solver = Viterbi(observation_list=self.gps_points.used_observation_seq_list,
                                 o_mat_dict=self.__emission_mat_dict,
                                 t_mat_dict=self.__ft_transition_dict, use_log_p=use_lop_p)
         self.__solver.init_model()
         self.index_state_list = self.__solver.iter_model()
-        # print(self.index_state_list)
-
-    def __generate_transition_mat_alpha_multi(self):
-        n = self.core_num
 
+    def __generate_transition_mat_alpha_multi(self, add_single_ft: list[bool] = None) -> bool:
         # 计算 初步候选, 经过这一步, 实际匹配用到的GPS点已经完全确定
         # 得到self.gps_candidate_link
         seq_list = self.__generate_candidates()
+        if not seq_list:
+            return False
 
         # 已经删除了关联不到任何路段的GPS点, 基于新的序列计算相邻GPS点距离
         # gps_field.POINT_SEQ_FIELD, gps_field.NEXT_SEQ, gps_field.ADJ_DIS
         gps_pre_next_dis_df = self.gps_points.calc_pre_next_dis()
         gps_pre_next_dis_df.rename(columns={gps_field.POINT_SEQ_FIELD: gps_field.FROM_GPS_SEQ,
                                             gps_field.NEXT_SEQ: gps_field.TO_GPS_SEQ}, inplace=True)
 
-        single_link_ft_df = self.net.get_link_data()[[net_field.SINGLE_LINK_ID_FIELD, net_field.FROM_NODE_FIELD,
-                                                      net_field.TO_NODE_FIELD]].copy()
+        # 抽取单向信息
+        single_link_ft_df = self.net.single_link_ft_cost()
         single_link_ft_df.reset_index(inplace=True, drop=True)
-
-        ft_list = [[i, i + 1, seq_list[i], seq_list[i + 1]] for i in range(0, len(seq_list) - 1)]
         g = self.net.graph
-        if n > 1:
-            print(f'using multiprocessing - {n} cores')
-            ft_group = cut_group(obj_list=ft_list, n=n)
-            del ft_list
-            pool = multiprocessing.Pool(processes=len(ft_group))
-            result_list = []
-            for i in range(0, len(ft_group)):
-                result = pool.apply_async(self.generate_transition_mat_alpha,
-                                          args=(ft_group[i], single_link_ft_df, self.gps_candidate_link,
-                                                gps_pre_next_dis_df, g,
-                                                self.net.search_method, self.net.weight_field, self.net.cache_path,
-                                                self.net.not_conn_cost))
-                result_list.append(result)
-            pool.close()
-            pool.join()
-            adj_seq_path_dict, ft_transition_dict, ft_mapping_dict, s2s_route_l, prj_done_dict = \
-                dict(), dict(), dict(), dict(), dict()
-            for res in result_list:
-                _adj_seq_path_dict, _ft_transition_dict, _ft_mapping_dict, _s2s_route_l, _prj_done_dict = res.get()
-                adj_seq_path_dict.update(_adj_seq_path_dict)
-                ft_transition_dict.update(_ft_transition_dict)
-                ft_mapping_dict.update(_ft_mapping_dict)
-                s2s_route_l.update(_s2s_route_l)
-                prj_done_dict.update(_prj_done_dict)
+        is_sub_net = self.net.is_sub_net
+        fmm_cache = self.net.fmm_cache
+        cut_off, max_cut_off = self.net.cut_off, self.net.max_cut_off
+        # print(cut_off)
+        if is_sub_net:
+            if fmm_cache:
+                done_stp_cost_df = self.net.get_path_cache()
+                cache_prj_info = self.net.get_prj_cache()
+            else:
+                done_stp_cost_df = pd.DataFrame()
+                cache_prj_info = dict()
         else:
-            adj_seq_path_dict, ft_transition_dict, ft_mapping_dict, s2s_route_l, prj_done_dict = \
-                self.generate_transition_mat_alpha(
-                    ft_list, single_link_ft_df, self.gps_candidate_link, gps_pre_next_dis_df, g,
-                    self.net.search_method, self.net.weight_field, self.net.cache_path,
-                    self.net.not_conn_cost)
+            done_stp_cost_df = self.net.get_path_cache()
+            cache_prj_info = self.net.get_prj_cache()
 
+        adj_seq_path_dict, ft_transition_dict, ft_idx_map, s2s_route_l, prj_done_df, \
+            done_stp_cost_df = \
+            self.generate_transition_mat_beta(single_link_ft_df, self.gps_candidate_link,
+                                              gps_pre_next_dis_df, g, self.net.search_method,
+                                              self.net.weight_field, self.net.cache_path, self.net.not_conn_cost,
+                                              done_stp_cost_df, is_sub_net, fmm_cache,
+                                              cut_off, max_cut_off, cache_prj_info, add_single_ft)
+        # print(len(done_stp_cost_df))
+        ft_idx_map.reset_index(inplace=True, drop=True)
+        s2s_route_l.reset_index(inplace=True, drop=True)
         self.__adj_seq_path_dict = adj_seq_path_dict
-        self.__ft_mapping_dict = ft_mapping_dict
+        self.__ft_idx_map = ft_idx_map
         self.__ft_transition_dict = ft_transition_dict
         self.__s2s_route_l = s2s_route_l
-        self.__done_prj_dict = prj_done_dict
+        self.__done_prj_df = prj_done_df
 
-    def generate_transition_mat_alpha(self, gps_ft_list: list = None, single_link_ft_df: pd.DataFrame = None,
-                                      pre_seq_candidate: pd.DataFrame = None,
-                                      gps_pre_next_dis_df: pd.DataFrame = None,
-                                      g: nx.DiGraph = None,
-                                      method: str = None, weight_field: str = 'length',
-                                      cache_path: bool = True, not_conn_cost: float = 999.0) -> \
-            tuple[dict, dict, dict, dict, dict]:
-        done_stp_cache, done_cost_cache, adj_seq_path_dict, s2s_route_l = dict(), dict(), dict(), dict()
-        ft_transition_dict, ft_mapping_dict = dict(), dict()
-        # seq_candidate这里是初步的
-        gps_ft_df = pd.DataFrame(gps_ft_list, columns=['idx', 'next_idx', 'f_gps_seq', 't_gps_seq'])
-        del gps_ft_df['idx']
-        del gps_ft_df['next_idx']
-        used_gps_seq = list(set(gps_ft_df['f_gps_seq']) | set(gps_ft_df['t_gps_seq']))
-        # p_name = os.getpid()
-        # print(rf'{p_name}:{used_gps_seq}')
-        # print(rf'{p_name}:{len(used_gps_seq)}')
-        pre_seq_candidate = pre_seq_candidate[
-                pre_seq_candidate[gps_field.POINT_SEQ_FIELD].isin(used_gps_seq)].copy()
-        seq_k_candidate, prj_done_dict = \
-            self.filter_k_candidates(preliminary_candidate_link=pre_seq_candidate,
-                                     top_k=self.top_k)
-        # print(rf'{p_name}:{seq_k_candidate}')
+        if not is_sub_net and not fmm_cache:
+            self.net.set_path_cache(stp_cost_df=done_stp_cost_df)
+        return True
+
+    # @function_time_cost
+    def generate_transition_mat_beta(self, single_link_ft_df: pd.DataFrame = None,
+                                     pre_seq_candidate: pd.DataFrame = None,
+                                     gps_pre_next_dis_df: pd.DataFrame = None,
+                                     g: nx.DiGraph = None,
+                                     method: str = None, weight_field: str = 'length',
+                                     cache_path: bool = True, not_conn_cost: float = 999.0,
+                                     done_stp_cost_df: pd.DataFrame = None,
+                                     is_sub_net: bool = True, fmm_cache: bool = False, cut_off: float = 600.0,
+                                     max_cut_off: float = 2000.0, cache_prj_inf: dict = None,
+                                     add_single_ft: list[bool] = None) -> \
+            tuple[dict, dict, pd.DataFrame, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
+        # K候选
+        seq_k_candidate_info = \
+            self.filter_k_candidates(preliminary_candidate_link=pre_seq_candidate, using_cache=fmm_cache,
+                                     top_k=self.top_k, cache_prj_inf=cache_prj_inf)
+        # print(rf'{len(seq_k_candidate_info)}个候选路段...')
+        seq_k_candidate_info['idx'] = seq_k_candidate_info.groupby(gps_field.POINT_SEQ_FIELD)[
+                                          net_field.SINGLE_LINK_ID_FIELD].rank(method='min').astype(int) - 1
+
+        ft_idx_map = seq_k_candidate_info[[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD, 'idx']].copy()
+        ft_idx_map.sort_values(by=[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD], inplace=True)
+        del seq_k_candidate_info['idx']
         del pre_seq_candidate
-        del used_gps_seq
-        seq_k_candidate = seq_k_candidate.groupby(gps_field.POINT_SEQ_FIELD).agg({net_field.SINGLE_LINK_ID_FIELD: list})
-
-        all_ft_state_list = list(chain(*[[[idx, next_idx, f_gps_seq, t_gps_seq, from_link, to_link]
-                                          for from_link in seq_k_candidate.at[f_gps_seq, net_field.SINGLE_LINK_ID_FIELD]
-                                          for to_link in seq_k_candidate.at[t_gps_seq, net_field.SINGLE_LINK_ID_FIELD]]
-                                         for idx, next_idx, f_gps_seq, t_gps_seq in gps_ft_list]))
-        # print(rf'{p_name}: {len(all_ft_state_list)}')
-        transition_df = pd.DataFrame(all_ft_state_list, columns=['idx', 'next_idx',
-                                                                 gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ,
-                                                                 markov_field.FROM_STATE, markov_field.TO_STATE])
-        # print(transition_df)
-        del all_ft_state_list
+        seq_k_candidate = seq_k_candidate_info.groupby(gps_field.POINT_SEQ_FIELD).agg(
+            {net_field.SINGLE_LINK_ID_FIELD: list, gps_field.POINT_SEQ_FIELD: list}).rename(
+            columns={gps_field.POINT_SEQ_FIELD: 'g_s'})
+
+        gps_match_link_route_dis = seq_k_candidate_info[
+            [gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD, 'route_dis']].copy()
+        seq_k_candidate.rename(columns={net_field.SINGLE_LINK_ID_FIELD: markov_field.FROM_STATE,
+                                        'g_s': gps_field.FROM_GPS_SEQ}, inplace=True)
+
+        seq_k_candidate[markov_field.TO_STATE] = seq_k_candidate[markov_field.FROM_STATE].shift(-1)
+        seq_k_candidate[gps_field.TO_GPS_SEQ] = seq_k_candidate[gps_field.FROM_GPS_SEQ].shift(-1)
+
+        seq_k_candidate.dropna(subset=[markov_field.TO_STATE], inplace=True)
+
+        from_state = seq_k_candidate[[markov_field.FROM_STATE, gps_field.FROM_GPS_SEQ]].reset_index(drop=False).rename(
+            columns={gps_field.POINT_SEQ_FIELD: 'g'}).explode(
+            column=[markov_field.FROM_STATE, gps_field.FROM_GPS_SEQ], ignore_index=True)
+
+        to_state = seq_k_candidate[
+            [markov_field.TO_STATE, gps_field.TO_GPS_SEQ]].reset_index(drop=False).rename(
+            columns={gps_field.POINT_SEQ_FIELD: 'g'}).explode(column=[markov_field.TO_STATE, gps_field.TO_GPS_SEQ],
+                                                              ignore_index=True)
+
+        transition_df = pd.merge(from_state, to_state, on='g', how='outer')
+        transition_df.reset_index(inplace=True, drop=True)
+        # print(rf'{len(transition_df)}次状态转移...')
         transition_df = self.diy_merge(left_df=transition_df,
-                                       right_df=single_link_ft_df,
+                                       right_df=single_link_ft_df[
+                                           [net_field.SINGLE_LINK_ID_FIELD, net_field.FROM_NODE_FIELD,
+                                            net_field.TO_NODE_FIELD]],
                                        left_key=markov_field.FROM_STATE, right_key=net_field.SINGLE_LINK_ID_FIELD,
                                        label='from')
         transition_df = self.diy_merge(left_df=transition_df,
-                                       right_df=single_link_ft_df,
+                                       right_df=single_link_ft_df[
+                                           [net_field.SINGLE_LINK_ID_FIELD, net_field.FROM_NODE_FIELD,
+                                            net_field.TO_NODE_FIELD]],
                                        left_key=markov_field.TO_STATE, right_key=net_field.SINGLE_LINK_ID_FIELD,
                                        label='to')
-        del single_link_ft_df
-        transition_df[markov_field.ROUTE_LENGTH] = \
-            transition_df.apply(
-                lambda item: self.calc_route_length_alpha(from_gps_seq=item[gps_field.FROM_GPS_SEQ],
-                                                          to_gps_seq=item[gps_field.TO_GPS_SEQ],
-                                                          from_link_id=item[markov_field.FROM_STATE],
-                                                          to_link_id=item[markov_field.TO_STATE],
-                                                          from_link_ft=(item['from_link_f'], item['from_link_t']),
-                                                          to_link_ft=(item['to_link_f'], item['to_link_t']),
-                                                          di_g=g,
-                                                          weight_field=weight_field,
-                                                          method=method,
-                                                          prj_done_dict=prj_done_dict,
-                                                          done_stp_cache=done_stp_cache,
-                                                          done_cost_cache=done_cost_cache,
-                                                          cache_path=cache_path,
-                                                          not_conn_cost=not_conn_cost,
-                                                          adj_seq_path_dict=adj_seq_path_dict), axis=1)
-        del done_cost_cache, done_stp_cache, g
+        transition_df = self.diy_merge(left_df=transition_df,
+                                       right_df=gps_match_link_route_dis,
+                                       left_key=[gps_field.FROM_GPS_SEQ, markov_field.FROM_STATE],
+                                       right_key=[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD],
+                                       label='from', merge_type='prj')
+        transition_df = self.diy_merge(left_df=transition_df,
+                                       right_df=gps_match_link_route_dis,
+                                       left_key=[gps_field.TO_GPS_SEQ, markov_field.TO_STATE],
+                                       right_key=[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD],
+                                       label='to', merge_type='prj')
+        del gps_match_link_route_dis
+
+        now_source_node = set(transition_df['from_link_f'])
+        if not fmm_cache:
+            # 先计算所有要计算的path
+            if o_node_field in done_stp_cost_df.columns:
+                already_cache_node = set(done_stp_cost_df[o_node_field])
+            else:
+                already_cache_node = set()
+            gap = now_source_node - already_cache_node
+            del single_link_ft_df[net_field.SINGLE_LINK_ID_FIELD]
+            if gap:
+                if not cache_path:
+                    add_single_ft[0] = True
+                done_stp_cost_df = self.add_path_cache(done_stp_cost_df=done_stp_cost_df,
+                                                       source_node_list=gap, cut_off=cut_off,
+                                                       single_link_ft_path_df=single_link_ft_df,
+                                                       weight_field=weight_field, method=method, g=g,
+                                                       add_single_ft=add_single_ft)
+        del single_link_ft_df, g
+
+        transition_df = pd.merge(transition_df, done_stp_cost_df, left_on=['from_link_f', 'to_link_f'],
+                                 right_on=[o_node_field, d_node_field], how='left')
+        del transition_df[o_node_field], transition_df[d_node_field]
+        # sub_net do not share path within different agents
+        if is_sub_net or fmm_cache or not cache_path:
+            del done_stp_cost_df
+            done_stp_cost_df = pd.DataFrame()
+
+        transition_df[cost_field] = transition_df[cost_field].fillna(0)
+        transition_df.reset_index(inplace=True, drop=True)
+        transition_df[markov_field.ROUTE_LENGTH] = not_conn_cost * 1.0
+
+        _ = transition_df[transition_df[cost_field] > 0]
+        adj_seq_path_dict = {(int(f_state), int(t_state)): node_path for f_state, t_state, node_path, c in
+                             zip(_[markov_field.FROM_STATE],
+                                 _[markov_field.TO_STATE],
+                                 _[path_field],
+                                 _[cost_field]) if c > 0}
+        same_link_idx = transition_df[markov_field.FROM_STATE] == transition_df[markov_field.TO_STATE]
+        transition_df.loc[same_link_idx, markov_field.ROUTE_LENGTH] = \
+            np.abs(transition_df.loc[same_link_idx, :]['from_route_dis'] -
+                   transition_df.loc[same_link_idx, :]['to_route_dis'])
+        transition_df['2nd_node'] = -1
+        transition_df['-2nd_node'] = -1
+        normal_path_idx_a = transition_df[cost_field] > 0
+        # normal_path_idx_a可能全是False
+        try:
+            transition_df.loc[normal_path_idx_a, '2nd_node'] = transition_df.loc[normal_path_idx_a, :][
+                path_field].apply(
+                lambda x: x[1])
+            transition_df.loc[normal_path_idx_a, '-2nd_node'] = transition_df.loc[normal_path_idx_a, :][
+                path_field].apply(
+                lambda x: x[-2])
+        except:
+            pass
+        normal_path_idx_b = (normal_path_idx_a & \
+                             (transition_df['2nd_node'] == transition_df['from_link_t']) & \
+                             (transition_df['-2nd_node'] != transition_df['to_link_t'])) | \
+                            ((transition_df['from_link_f'] == transition_df['to_link_t']) &
+                             (transition_df['from_link_t'] == transition_df['to_link_f']))
+
+        transition_df.loc[normal_path_idx_b, markov_field.ROUTE_LENGTH] = \
+            np.abs(transition_df.loc[normal_path_idx_b, :][cost_field] -
+                   transition_df.loc[normal_path_idx_b, :]['from_route_dis'] +
+                   transition_df.loc[normal_path_idx_b, :]['to_route_dis'])
+
         transition_df = pd.merge(transition_df, gps_pre_next_dis_df, on=[gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ],
                                  how='left')
-
         transition_df[markov_field.DIS_GAP] = np.abs(
             -transition_df[markov_field.ROUTE_LENGTH] + transition_df[gps_field.ADJ_DIS])
 
-        for (idx, next_idx, f_gps_seq, t_gps_seq), df in transition_df.groupby(
-                ['idx', 'next_idx', gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ]):
-            s2s_route_l[(f_gps_seq, t_gps_seq)] = df[
-                [markov_field.FROM_STATE, markov_field.TO_STATE, markov_field.ROUTE_LENGTH]].copy().set_index(
-                [markov_field.FROM_STATE, markov_field.TO_STATE])
-
-            # 转成matrix
-            transition_mat = df[
-                [markov_field.FROM_STATE, markov_field.TO_STATE, markov_field.DIS_GAP]].set_index(
-                [markov_field.FROM_STATE, markov_field.TO_STATE]).unstack().values
-            from_link, to_link = list(set(df[markov_field.FROM_STATE])), list(set(df[markov_field.TO_STATE]))
-            # 索引映射
-            f_mapping, t_mapping = {i: f for i, f in zip(range(len(from_link)), sorted(from_link))}, \
-                {i: t for i, t in zip(range(len(to_link)), sorted(to_link))}
-            transition_mat = self.transition_probability(self.beta, transition_mat, self.dis_para)
-
-            ft_transition_dict[f_gps_seq] = transition_mat
-            ft_mapping_dict[f_gps_seq] = f_mapping
-            ft_mapping_dict[t_gps_seq] = t_mapping
-
-        return adj_seq_path_dict, ft_transition_dict, ft_mapping_dict, s2s_route_l, prj_done_dict
+        s2s_route_l = transition_df[[gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ, markov_field.ROUTE_LENGTH,
+                                     markov_field.FROM_STATE, markov_field.TO_STATE]].copy()
+        transition_df['trans_values'] = \
+            self.transition_probability(self.beta, transition_df[markov_field.DIS_GAP].values, self.dis_para)
+        ft_transition_dict = {f_gps_seq: df[
+            [markov_field.FROM_STATE, markov_field.TO_STATE, 'trans_values']].set_index(
+            [markov_field.FROM_STATE, markov_field.TO_STATE]).unstack().values for (f_gps_seq, t_gps_seq), df in
+                              transition_df.groupby([gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ])}
+        return adj_seq_path_dict, ft_transition_dict, ft_idx_map, s2s_route_l, seq_k_candidate_info, done_stp_cost_df
+
+    def add_path_cache(self, done_stp_cost_df: pd.DataFrame = None, source_node_list: list[int] or set[int] = None,
+                       g: nx.DiGraph = None, method: str = 'dijkstra', single_link_ft_path_df: pd.DataFrame = None,
+                       weight_field: str = None, cut_off: float = 600.0, add_single_ft: list[bool] = True) \
+            -> pd.DataFrame:
+        _done_stp_cost_df = self.single_source_path_cache(node_list=source_node_list, method=method, cut_off=cut_off,
+                                                          weight_field=weight_field, g=g)
+        done_stp_cost_df = pd.concat([done_stp_cost_df, _done_stp_cost_df])
+        del _done_stp_cost_df
+        if add_single_ft[0]:
+            single_link_ft_path_df = single_link_ft_path_df[single_link_ft_path_df[self.net.weight_field] > cut_off]
+            if not single_link_ft_path_df.empty:
+                done_stp_cost_df = pd.concat(
+                    [done_stp_cost_df, single_link_ft_path_df.rename(columns={net_field.FROM_NODE_FIELD: o_node_field,
+                                                                              net_field.TO_NODE_FIELD: d_node_field})])
+                done_stp_cost_df.drop_duplicates(subset=[o_node_field, d_node_field], keep='first', inplace=True)
+            print('add single ft')
+            add_single_ft[0] = False
+        done_stp_cost_df.reset_index(inplace=True, drop=True)
+        return done_stp_cost_df
+
+    def single_source_path_cache(self, node_list: list[int] or set[int] = None, g: nx.DiGraph = None,
+                                 method: str = 'dijkstra',
+                                 weight_field: str = None, cut_off: float = 600.0) -> pd.DataFrame:
+        cost, stp = dict(), dict()
+        stp_cost_df = pd.DataFrame()
+        for n in node_list:
+            try:
+                cost[n], stp[n] = \
+                    self._single_source_path_alpha(g, source=n,
+                                                   method=method,
+                                                   weight_field=weight_field,
+                                                   cut_off=cut_off)
+            except nx.NetworkXNoPath:
+                pass
+        if stp:
+            stp_df = pd.DataFrame(stp).stack().reset_index(drop=False).rename(
+                columns={'level_0': d_node_field, 'level_1': o_node_field, 0: path_field})
+            cost_df = pd.DataFrame(cost).stack().reset_index(drop=False).rename(
+                columns={'level_0': d_node_field, 'level_1': o_node_field, 0: cost_field})
+            cost_df[cost_field] = np.around(cost_df[cost_field], decimals=1)
+            stp_cost_df = pd.merge(stp_df, cost_df, on=[o_node_field, d_node_field])
+            del stp_df, cost_df
+            stp_cost_df.reset_index(inplace=True, drop=True)
+        return stp_cost_df
 
     @staticmethod
-    def diy_merge(left_df: pd.DataFrame, right_df: pd.DataFrame or gpd.GeoDataFrame = None, left_key: str = None,
-                  right_key: str = None, label: str = 'from'):
+    def diy_merge(left_df: pd.DataFrame, right_df: pd.DataFrame or gpd.GeoDataFrame = None,
+                  left_key: str or list[str] = None,
+                  right_key: str or list[str] = None, label: str = 'from', merge_type: str = 'ft'):
         df = pd.merge(left_df, right_df, left_on=left_key, right_on=right_key, how='left')
 
-        df.rename(columns={net_field.FROM_NODE_FIELD: label + '_link_f',
-                           net_field.TO_NODE_FIELD: label + '_link_t'}, inplace=True)
-
-        df.drop(columns=[right_key], axis=1, inplace=True)
-        return df
-
-    def calc_route_length(self, from_gps_seq: int = None, to_gps_seq: int = None, from_link_id: int = None,
-                          to_link_id: int = None) -> float:
-        """
-        :param from_gps_seq: 上一观测时刻的gps点序号
-        :param to_gps_seq: 当前观测时刻的gps点序号
-        :param from_link_id: 上一观测时刻候选link_id
-        :param to_link_id: 当前观测时刻候选link_id
-        :return:
-        """
-        # prj_p, prj_dis, route_dis
-        (from_prj_p, from_prj_dis, from_route_dis, from_l_length, from_p_vec) = \
-            self.cache_emission_data(gps_seq=from_gps_seq, single_link_id=from_link_id)
-
-        (to_prj_p, to_prj_dis, to_route_dis, to_l_length, to_p_vec) = \
-            self.cache_emission_data(gps_seq=to_gps_seq, single_link_id=to_link_id)
-
-        # 基于投影信息计算路径长度
-        from_link_ft, to_link_ft = self.net.get_link_from_to(from_link_id, _type='single'), \
-            self.net.get_link_from_to(to_link_id, _type='single')
-
-        # same link
-        if from_link_id == to_link_id:
-            route_l = np.absolute(from_route_dis - to_route_dis)
-            return route_l
-
-        # one same node
-        dup_node_list = list(set(from_link_ft) & set(to_link_ft))
-        if len(dup_node_list) == 1:
-            dup_node = dup_node_list[0]
-            if (dup_node == from_link_ft[1]) and (dup_node == to_link_ft[0]):
-                route_l = from_l_length - from_route_dis + to_route_dis
-                return np.absolute(route_l)
-            else:
-                return self.not_conn_cost
-        # 正好相反的f-t
-        elif len(dup_node_list) == 2:
-            route_l = from_l_length - from_route_dis + to_route_dis
-            return np.absolute(route_l)
-
-        route_item = self.net.search(o_node=from_link_ft[0], d_node=to_link_ft[0])
-        if len(route_item[0]) > 2:
-            self.__adj_seq_path_dict[(from_link_id, to_link_id)] = route_item[0]
-        if route_item[0]:
-            if route_item[0][1] != from_link_ft[1]:
-                # abnormal
-                # route_item_alpha = self.net.search(o_node=from_link_ft[1], d_node=to_link_ft[0],
-                #                                    search_method=self.search_method)
-                # if route_item_alpha[0]:
-                #     route_l1 = route_item[1] + from_route_dis
-                # else:
-                #     return NOT_CONN_COST
-                return self.not_conn_cost
-            else:
-                route_l1 = route_item[1] - from_route_dis
-
-            if route_item[0][-2] == to_link_ft[1]:
-                # abnormal
-                return self.not_conn_cost
-            else:
-                route_l2 = to_route_dis
-
-            route_l = np.absolute(route_l1 + route_l2)
-            return route_l
-        else:
-            return self.not_conn_cost
-
-    def calc_route_length_alpha(self, from_gps_seq: int = None, to_gps_seq: int = None,
-                                from_link_id: int = None, to_link_id: int = None,
-                                from_link_ft=None, to_link_ft=None,
-                                done_stp_cache: dict = None, done_cost_cache: dict = None,
-                                prj_done_dict: dict = None,
-                                adj_seq_path_dict: dict = None,
-                                di_g: nx.DiGraph = None,
-                                method: str = None, weight_field: str = 'length',
-                                cache_path: bool = True, not_conn_cost: float = 999.0) -> float:
-        """"""
-        from_prj_p, from_prj_dis, from_route_dis, from_l_length, from_p_vec = prj_done_dict[
-            (from_gps_seq, from_link_id)]
-        to_prj_p, to_prj_dis, to_route_dis, to_l_length, to_p_vec = prj_done_dict[
-            (to_gps_seq, to_link_id)]
-
-        # same link
-        if from_link_id == to_link_id:
-            route_l = np.absolute(from_route_dis - to_route_dis)
-            return route_l
-
-        # one same node
-        dup_node_list = list(set(from_link_ft) & set(to_link_ft))
-        if len(dup_node_list) == 1:
-            dup_node = dup_node_list[0]
-            if (dup_node == from_link_ft[1]) and (dup_node == to_link_ft[0]):
-                route_l = from_l_length - from_route_dis + to_route_dis
-                return np.absolute(route_l)
-            else:
-                return self.not_conn_cost
-        # 正好相反的f-t
-        elif len(dup_node_list) == 2:
-            route_l = from_l_length - from_route_dis + to_route_dis
-            return np.absolute(route_l)
-        o_node,  d_node = from_link_ft[0], to_link_ft[0]
-        route_item = self.get_od_cost_alpha(g=di_g, o_node=o_node, d_node=d_node,
-                                            done_stp_cache=done_stp_cache, done_cost_cache=done_cost_cache,
-                                            method=method,
-                                            weight_field=weight_field, cache_path=cache_path,
-                                            not_conn_cost=not_conn_cost)
-        if len(route_item[0]) > 2:
-            adj_seq_path_dict[(from_link_id, to_link_id)] = route_item[0]
-        if route_item[0]:
-            if route_item[0][1] != from_link_ft[1]:
-                return not_conn_cost
-            else:
-                route_l1 = route_item[1] - from_route_dis
-
-            if route_item[0][-2] == to_link_ft[1]:
-                # abnormal
-                return not_conn_cost
-            else:
-                route_l2 = to_route_dis
+        if merge_type == 'ft':
+            df.rename(columns={net_field.FROM_NODE_FIELD: label + '_link_f',
+                               net_field.TO_NODE_FIELD: label + '_link_t'}, inplace=True)
 
-            route_l = np.absolute(route_l1 + route_l2)
-            return route_l
+            df.drop(columns=[right_key], axis=1, inplace=True)
         else:
-            return not_conn_cost
-
-    def get_od_cost_alpha(self, g: nx.DiGraph = None, o_node: int = None, d_node: int = None,
-                          cache_path: bool = True, done_stp_cache: dict = None,
-                          done_cost_cache: dict = None, method: str = None,
-                          weight_field: str = 'length', not_conn_cost: float = 999.0) -> tuple[list, float]:
-        """"""
-
-        if o_node in done_stp_cache.keys():
-            try:
-                node_path = done_stp_cache[o_node][d_node]
-                cost = done_cost_cache[o_node][d_node]
-            except KeyError:
-                return [], not_conn_cost
-        else:
-            self.calc_shortest_path_alpha(g=g, source=o_node, method=method, done_cost_cache=done_cost_cache,
-                                          done_stp_cache=done_stp_cache, weight_field=weight_field)
-            try:
-                node_path = done_stp_cache[o_node][d_node]
-                cost = done_cost_cache[o_node][d_node]
-                if not cache_path:
-                    del done_stp_cache[o_node]
-                    del done_cost_cache[o_node]
-            except KeyError:
-                return [], not_conn_cost
-
-        return node_path, cost
-
-    def calc_shortest_path_alpha(self, g: nx.DiGraph = None, source: int = None, done_stp_cache: dict = None,
-                                 done_cost_cache: dict = None, method: str = None,
-                                 weight_field: str = 'length'):
-        """
+            df.rename(columns={'route_dis': label + '_route_dis'}, inplace=True)
+            df.drop(columns=right_key, axis=1, inplace=True)
+        return df
 
-        :param g:
-        :param source:
-        :param done_stp_cache:
-        :param done_cost_cache:
-        :param method:
-        :param weight_field:
-        :return:
-        """
-        try:
-            done_cost_cache[source], done_stp_cache[source] = self._single_source_path_alpha(
-                g, source=source,
-                method=method, weight_field=weight_field)
-        except nx.NetworkXNoPath:
-            pass
 
     @staticmethod
     def _single_source_path_alpha(g: nx.DiGraph = None, source: int = None, method: str = 'dijkstra',
-                                  weight_field: str = None) -> tuple[dict[int, int], dict[int, list]]:
+                                  weight_field: str = None, cut_off: float = 600.0) -> \
+            tuple[dict[int, int], dict[int, list]]:
         if method == 'dijkstra':
-            return nx.single_source_dijkstra(g, source, weight=weight_field)
+            return nx.single_source_dijkstra(g, source, weight=weight_field, cutoff=cut_off)
         else:
             return nx.single_source_bellman_ford(g, source, weight=weight_field)
 
-    def cache_emission_data(self, gps_seq: int = None, single_link_id: int = None) -> \
-            tuple[Point, float, float, float, np.ndarray]:
-        """
-        :param gps_seq:
-        :param single_link_id:
-        :return:
-        """
-        if (gps_seq, single_link_id) in self.__done_prj_dict.keys():
-            # already calculated
-            (prj_p, prj_dis, route_dis, l_length, p_vec) = self.__done_prj_dict[
-                (gps_seq, single_link_id)]
-        else:
-            # new calc and cache
-            # print('# new calc and cache')
-            (prj_p, prj_dis, route_dis, l_length, p_vec) = self.get_gps_prj_info(
-                target_link_id=single_link_id,
-                gps_seq=gps_seq)
-            self.__done_prj_dict.update(
-                {(gps_seq, single_link_id): (prj_p, prj_dis, route_dis, l_length, p_vec)})
-        return prj_p, prj_dis, route_dis, l_length, p_vec
-
-    def get_gps_prj_info(self, gps_seq: int = None, target_link_id: int = None) -> \
-            tuple[Point, float, float, float, np.ndarray]:
-        return self.gps_points.get_prj_inf(line=self.net.get_link_geo(target_link_id, _type='single'), seq=gps_seq)
-
-    def get_gps_prj_info_alpha(self, gps_geo: Point = None, target_link_geo: LineString = None) -> \
-            tuple[Point, float, float, float, np.ndarray]:
-        (prj_p, prj_dis, route_dis, l_length, _, p_vec) = prj_inf(gps_geo, target_link_geo)
-        return prj_p, prj_dis, route_dis, l_length, p_vec
-
     @staticmethod
     def transition_probability(beta: float = 30.2, dis_gap: float or np.ndarray = None, dis_para: float = 0.1):
         """
         dis_gap = straight_l - route_l
         :param beta:
         :param dis_gap:
         :param dis_para
@@ -623,49 +537,48 @@
         heading_gap = self.heading_para_array[(heading_gap / self.angle_slice).astype(int)]
         # print(heading_gap)
         p = heading_gap * np.e ** (-0.5 * (self.dis_para * dis / sigma) ** 2)
         return p
 
     def acquire_res(self) -> gpd.GeoDataFrame():
         # 观测序列 -> (观测序列, single_link)
-        single_link_state_list = [(observe_val, self.__ft_mapping_dict[observe_val][state_index]) for
-                                  observe_val, state_index in
-                                  zip(self.gps_points.used_observation_seq_list,
-                                      self.index_state_list)]
-        # print(single_link_state_list)
-        # 映射回原路网link_id, 以及dir
-        # {[link_id, dir, from_node, to_node], [link_id, dir, from_node, to_node]...}
-        bilateral_unidirectional_mapping = self.net.bilateral_unidirectional_mapping
-        link_state_list = [item + bilateral_unidirectional_mapping[item[1]] for item in single_link_state_list]
+        state_idx_df = pd.DataFrame(
+            {'idx': self.index_state_list, gps_field.POINT_SEQ_FIELD: self.gps_points.used_observation_seq_list})
 
-        gps_link_state_df = pd.DataFrame(link_state_list, columns=[gps_field.POINT_SEQ_FIELD,
-                                                                   net_field.SINGLE_LINK_ID_FIELD,
-                                                                   net_field.LINK_ID_FIELD,
-                                                                   net_field.DIRECTION_FIELD,
-                                                                   net_field.FROM_NODE_FIELD,
-                                                                   net_field.TO_NODE_FIELD])
-        gps_link_state_df[gps_field.SUB_SEQ_FIELD] = 0
+        gps_link_state_df = pd.merge(state_idx_df, self.__ft_idx_map, on=[gps_field.POINT_SEQ_FIELD, 'idx'])
 
-        gps_link_state_df[markov_field.PRJ_GEO] = \
-            gps_link_state_df.apply(lambda item: self.__done_prj_dict[(item[gps_field.POINT_SEQ_FIELD],
-                                                                       item[net_field.SINGLE_LINK_ID_FIELD])][0],
-                                    axis=1)
+        single_link = self.net.get_link_data()[[net_field.SINGLE_LINK_ID_FIELD,
+                                                net_field.LINK_ID_FIELD,
+                                                net_field.DIRECTION_FIELD,
+                                                net_field.FROM_NODE_FIELD,
+                                                net_field.TO_NODE_FIELD]].copy()
+        single_link.reset_index(inplace=True, drop=True)
+        gps_link_state_df = pd.merge(gps_link_state_df, single_link, on=net_field.SINGLE_LINK_ID_FIELD, how='left')
 
+        gps_link_state_df[gps_field.SUB_SEQ_FIELD] = 0
+        gps_link_state_df = pd.merge(gps_link_state_df, self.__done_prj_df[[gps_field.POINT_SEQ_FIELD,
+                                                                            net_field.SINGLE_LINK_ID_FIELD,
+                                                                            markov_field.PRJ_GEO]],
+                                     on=[gps_field.POINT_SEQ_FIELD,
+                                         net_field.SINGLE_LINK_ID_FIELD], how='left')
         gps_link_state_df[['next_single', 'next_seq']] = gps_link_state_df[
             [net_field.SINGLE_LINK_ID_FIELD, gps_field.POINT_SEQ_FIELD]].shift(-1)
         gps_link_state_df.fillna(-99, inplace=True)
         gps_link_state_df[['next_single', 'next_seq']] = gps_link_state_df[['next_single', 'next_seq']].astype(int)
-        gps_link_state_df[markov_field.DIS_TO_NEXT] = \
-            gps_link_state_df.apply(
-                lambda item: self.__s2s_route_l[(item[gps_field.POINT_SEQ_FIELD], item['next_seq'])].at[
-                    (item[net_field.SINGLE_LINK_ID_FIELD],
-                     item['next_single']), markov_field.ROUTE_LENGTH] if item['next_single'] != -99 else np.nan, axis=1)
-
-        del link_state_list
 
+        self.__s2s_route_l.rename(columns={gps_field.FROM_GPS_SEQ: gps_field.POINT_SEQ_FIELD,
+                                           gps_field.TO_GPS_SEQ: 'next_seq',
+                                           markov_field.FROM_STATE: net_field.SINGLE_LINK_ID_FIELD,
+                                           markov_field.TO_STATE: 'next_single',
+                                           markov_field.ROUTE_LENGTH: markov_field.DIS_TO_NEXT}, inplace=True)
+
+        gps_link_state_df = pd.merge(gps_link_state_df, self.__s2s_route_l, how='left', on=[gps_field.POINT_SEQ_FIELD,
+                                                                                            'next_seq',
+                                                                                            net_field.SINGLE_LINK_ID_FIELD,
+                                                                                            'next_single'])
         # agent_id, seq
         gps_match_res_gdf = self.gps_points.gps_gdf
 
         # 获取补全的路径
         # gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD, gps_field.SUB_SEQ_FIELD
         # net_field.LINK_ID_FIELD, net_field.DIRECTION_FIELD, net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD
         # gps_field.TIME_FIELD, net_field.GEOMETRY_FIELD
@@ -709,15 +622,14 @@
             lambda row: (row[markov_field.PRJ_GEO].x, row[markov_field.PRJ_GEO].y), axis=1,
             result_type='expand')
         gps_match_res_gdf = pd.merge(gps_match_res_gdf, prj_gdf, how='left', left_index=True, right_index=True)
         del prj_gdf
         self.gps_match_res_gdf = gps_match_res_gdf
         return self.gps_match_res_gdf
 
-    @function_time_cost
     def acquire_omitted_match_item(self, gps_link_state_df: pd.DataFrame = None) -> pd.DataFrame:
         """
         推算补全不完整的路径之间的path以及GPS点
         :param gps_link_state_df: 初步的匹配结果, 可能存在断掉的路径
         :return:
         """
         bilateral_unidirectional_mapping = self.net.bilateral_unidirectional_mapping
@@ -818,16 +730,14 @@
             # print('初次计算')
             single_link_gdf = self.net.get_link_data()
             single_link_gdf.reset_index(inplace=True, drop=True)
             node_gdf = self.net.get_node_data()
             net_crs = self.net.crs
             plain_crs = self.net.planar_crs
             is_geo_crs = self.net.is_geo_crs()
-            double_link_geo = {l: geo for l, geo in zip(single_link_gdf[net_field.LINK_ID_FIELD],
-                                                        single_link_gdf[net_field.GEOMETRY_FIELD])}
 
             if self.gps_match_res_gdf is None:
                 self.acquire_res()
 
             # 匹配路段
             if use_gps_source:
                 plot_gps_gdf = self.gps_points.source_gps[
@@ -846,17 +756,20 @@
             plot_gps_gdf[net_field.GEOMETRY_FIELD] = plot_gps_gdf[net_field.GEOMETRY_FIELD].buffer(gps_radius)
             plot_gps_gdf[gps_field.TYPE_FIELD] = 'gps'
 
             # 匹配路段GDF
             plot_match_link_gdf = self.gps_match_res_gdf.copy()
             plot_match_link_gdf.drop(columns=[markov_field.PRJ_GEO], axis=1, inplace=True)
             plot_match_link_gdf[gps_field.TYPE_FIELD] = 'link'
-            plot_match_link_gdf[net_field.GEOMETRY_FIELD] = plot_match_link_gdf[net_field.LINK_ID_FIELD].apply(
-                lambda x: double_link_geo[x])
-            plot_match_link_gdf.crs = net_crs
+            del plot_match_link_gdf[net_field.GEOMETRY_FIELD]
+            plot_match_link_gdf = pd.merge(plot_match_link_gdf, single_link_gdf[[net_field.SINGLE_LINK_ID_FIELD,
+                                                                                 net_field.GEOMETRY_FIELD]],
+                                           on=net_field.SINGLE_LINK_ID_FIELD,
+                                           how='inner')
+            plot_match_link_gdf = gpd.GeoDataFrame(plot_match_link_gdf, geometry=net_field.GEOMETRY_FIELD, crs=net_crs)
             plot_match_link_gdf.drop_duplicates(subset=net_field.LINK_ID_FIELD, keep='first', inplace=True)
             plot_match_link_gdf.reset_index(drop=True, inplace=True)
             if is_geo_crs:
                 plot_match_link_gdf = plot_match_link_gdf.to_crs(plain_crs)
             plot_match_link_gdf[net_field.GEOMETRY_FIELD] = \
                 plot_match_link_gdf[net_field.GEOMETRY_FIELD].buffer(match_link_width)
             plot_match_link_gdf.drop(columns=[gps_field.LNG_FIELD, gps_field.LAT_FIELD], axis=1, inplace=True)
@@ -960,14 +873,173 @@
 
     def format_war_info(self):
         if self.warn_info['from_ft']:
             self.format_warn_info = pd.DataFrame(self.warn_info)
         del self.warn_info
 
 
+    # @function_time_cost
+    # def generate_transition_mat_beta1(self, gps_ft_list: list = None, single_link_ft_df: pd.DataFrame = None,
+    #                                   pre_seq_candidate: pd.DataFrame = None,
+    #                                   gps_pre_next_dis_df: pd.DataFrame = None,
+    #                                   g: nx.DiGraph = None,
+    #                                   method: str = None, weight_field: str = 'length',
+    #                                   cache_path: bool = True, not_conn_cost: float = 999.0,
+    #                                   done_stp_cost_df: pd.DataFrame = None,
+    #                                   is_sub_net: bool = True, fmm_cache: bool = False, cut_off: float = 600.0,
+    #                                   max_cut_off: float = 2000.0, cache_prj_inf: dict = None) -> \
+    #         tuple[dict, dict, pd.DataFrame, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
+    #     gps_ft_df = pd.DataFrame(gps_ft_list, columns=['f_gps_seq', 't_gps_seq'])
+    #     used_gps_seq = list(set(gps_ft_df['f_gps_seq']) | set(gps_ft_df['t_gps_seq']))
+    #
+    #     # 确定最终的top_k候选
+    #     pre_seq_candidate = pre_seq_candidate[
+    #         pre_seq_candidate[gps_field.POINT_SEQ_FIELD].isin(used_gps_seq)].copy()
+    #     seq_k_candidate_info = self.filter_k_candidates(preliminary_candidate_link=pre_seq_candidate,
+    #                                                     top_k=self.top_k, cache_prj_inf=cache_prj_inf)
+    #
+    #     # 存储状态的索引和状态序列的映射
+    #     seq_k_candidate_info['idx'] = seq_k_candidate_info.groupby(gps_field.POINT_SEQ_FIELD)[
+    #                                       net_field.SINGLE_LINK_ID_FIELD].rank(method='min').astype(int) - 1
+    #     ft_idx_map = seq_k_candidate_info[[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD, 'idx']].copy()
+    #     ft_idx_map.sort_values(by=[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD], inplace=True)
+    #     del seq_k_candidate_info['idx']
+    #
+    #     del pre_seq_candidate
+    #     del used_gps_seq
+    #
+    #     s = time.time()
+    #     # 构造状态转移表
+    #     seq_k_candidate = seq_k_candidate_info.groupby(gps_field.POINT_SEQ_FIELD).agg(
+    #         {net_field.SINGLE_LINK_ID_FIELD: list, gps_field.POINT_SEQ_FIELD: list,
+    #          net_field.FROM_NODE_FIELD: list, net_field.TO_NODE_FIELD: list, 'route_dis': list}).rename(
+    #         columns={gps_field.POINT_SEQ_FIELD: gps_field.FROM_GPS_SEQ,
+    #                  net_field.SINGLE_LINK_ID_FIELD: markov_field.FROM_STATE,
+    #                  net_field.FROM_NODE_FIELD: 'from_link_f', net_field.TO_NODE_FIELD: 'from_link_t',
+    #                  'route_dis': 'from_route_dis'})
+    #
+    #     seq_k_candidate[[gps_field.TO_GPS_SEQ, markov_field.TO_STATE, 'to_link_f', 'to_link_t', 'to_route_dis']] = \
+    #         seq_k_candidate[[gps_field.FROM_GPS_SEQ, markov_field.FROM_STATE, 'from_link_f', 'from_link_t',
+    #                          'from_route_dis']].shift(-1)
+    #     seq_k_candidate.dropna(subset=[markov_field.TO_STATE], inplace=True)
+    #
+    #     from_state = seq_k_candidate[
+    #         [markov_field.FROM_STATE, gps_field.FROM_GPS_SEQ,
+    #          'from_link_f', 'from_link_t', 'from_route_dis']].reset_index(drop=False).explode(
+    #         column=[markov_field.FROM_STATE, gps_field.FROM_GPS_SEQ, 'from_link_f', 'from_link_t',
+    #                 'from_route_dis'], ignore_index=True)
+    #
+    #     to_state = seq_k_candidate[
+    #         [markov_field.TO_STATE, gps_field.TO_GPS_SEQ, 'to_link_f', 'to_link_t', 'to_route_dis']].reset_index(
+    #         drop=False).explode(
+    #         column=[markov_field.TO_STATE, gps_field.TO_GPS_SEQ, 'to_link_f', 'to_link_t', 'to_route_dis'],
+    #         ignore_index=True)
+    #     del seq_k_candidate
+    #     transition_df = pd.merge(from_state, to_state, on=gps_field.POINT_SEQ_FIELD, how='outer')
+    #     del transition_df[gps_field.POINT_SEQ_FIELD]
+    #     del from_state, to_state
+    #     transition_df.reset_index(inplace=True, drop=True)
+    #     print(rf'构造: {time.time() - s}')
+    #     t = time.time()
+    #     del single_link_ft_df
+    #
+    #     now_source_node = set(transition_df['from_link_f'])
+    #     if not fmm_cache:
+    #         # 先计算所有要计算的path
+    #         already_cache_node = set(done_stp_cost_df['o_node'])
+    #         gap = now_source_node - already_cache_node
+    #         if not gap:
+    #             done_stp_cost_df = self.add_path_cache(done_stp_cost_df=done_stp_cost_df,
+    #                                                    source_node_list=gap, cut_off=cut_off,
+    #                                                    weight_field=weight_field, method=method, g=g)
+    #             now_source_node = set(done_stp_cost_df['o_node'])
+    #
+    #     # 如果某些点除开自身-自身没有其他点, 则加一个5km搜索
+    #     done_stp_cost_df.drop(index=done_stp_cost_df[done_stp_cost_df['o_node'] == done_stp_cost_df['d_node']].index,
+    #                           inplace=True)
+    #     no_path_node = now_source_node - set(done_stp_cost_df['o_node'])
+    #     if no_path_node:
+    #         done_stp_cost_df = self.add_path_cache(done_stp_cost_df=done_stp_cost_df,
+    #                                                source_node_list=no_path_node, cut_off=max_cut_off,
+    #                                                weight_field=weight_field, method=method, g=g)
+    #     del g
+    #
+    #     # transition_df['from_route_dis'] = transition_df['from_route_dis'].astype(float)
+    #     # transition_df['to_route_dis'] = transition_df['to_route_dis'].astype(float)
+    #
+    #     transition_df = pd.merge(transition_df, done_stp_cost_df, left_on=['from_link_f', 'to_link_f'],
+    #                              right_on=['o_node', 'd_node'], how='left')
+    #     del transition_df['o_node'], transition_df['d_node']
+    #     # sub_net do not share path within different agents
+    #     if is_sub_net or fmm_cache or not cache_path:
+    #         del done_stp_cost_df
+    #         done_stp_cost_df = pd.DataFrame()
+    #
+    #     transition_df['cost'] = transition_df['cost'].fillna(0)
+    #     transition_df.reset_index(inplace=True, drop=True)
+    #     transition_df[markov_field.ROUTE_LENGTH] = not_conn_cost * 1.0
+    #
+    #     _ = transition_df[transition_df['cost'] > 0]
+    #     adj_seq_path_dict = {(int(f_state), int(t_state)): node_path for f_state, t_state, node_path, c in
+    #                          zip(_[markov_field.FROM_STATE],
+    #                              _[markov_field.TO_STATE],
+    #                              _['path'],
+    #                              _['cost']) if c > 0}
+    #     z = time.time()
+    #     same_link_idx = transition_df[markov_field.FROM_STATE] == transition_df[markov_field.TO_STATE]
+    #     transition_df.loc[same_link_idx, markov_field.ROUTE_LENGTH] = \
+    #         np.abs(transition_df.loc[same_link_idx, :]['from_route_dis'].values.astype(float) -
+    #                transition_df.loc[same_link_idx, :]['to_route_dis'].values.astype(float))
+    #     transition_df['2nd_node'] = -1
+    #     transition_df['-2nd_node'] = -1
+    #     normal_path_idx_a = transition_df['cost'] > 0
+    #     t2 = time.time()
+    #     transition_df.loc[normal_path_idx_a, '2nd_node'] = transition_df.loc[normal_path_idx_a, :]['path'].apply(
+    #         lambda x: x[1])
+    #     transition_df.loc[normal_path_idx_a, '-2nd_node'] = transition_df.loc[normal_path_idx_a, :]['path'].apply(
+    #         lambda x: x[-2])
+    #     t3 = time.time()
+    #     normal_path_idx_b = (normal_path_idx_a & \
+    #                          (transition_df['2nd_node'] == transition_df['from_link_t']) & \
+    #                          (transition_df['-2nd_node'] != transition_df['to_link_t'])) | \
+    #                         ((transition_df['from_link_f'] == transition_df['to_link_t']) &
+    #                          (transition_df['from_link_t'] == transition_df['to_link_f']))
+    #
+    #     transition_df.loc[normal_path_idx_b, markov_field.ROUTE_LENGTH] = \
+    #         np.abs(transition_df.loc[normal_path_idx_b, :]['cost'].values -
+    #                transition_df.loc[normal_path_idx_b, :]['from_route_dis'].values.astype(float) +
+    #                transition_df.loc[normal_path_idx_b, :]['to_route_dis'].values.astype(float))
+    #     print(rf'cache_len: {len(done_stp_cost_df)}')
+    #
+    #     transition_df = pd.merge(transition_df, gps_pre_next_dis_df, on=[gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ],
+    #                              how='left')
+    #
+    #     transition_df[markov_field.DIS_GAP] = np.abs(
+    #         -transition_df[markov_field.ROUTE_LENGTH] + transition_df[gps_field.ADJ_DIS])
+    #     t4 = time.time()
+    #     # print(transition_df[markov_field.DIS_GAP])
+    #     print(rf'向量化总时间: {t4 - z}')
+    #     print(rf'apply: {t3 - t2}')
+    #     print(rf'总计算: {t4 - t}')
+    #
+    #     s2s_route_l = transition_df[[gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ, markov_field.ROUTE_LENGTH,
+    #                                  markov_field.FROM_STATE, markov_field.TO_STATE]].copy()
+    #
+    #     transition_df['trans_values'] = \
+    #         self.transition_probability(self.beta, transition_df[markov_field.DIS_GAP].values, self.dis_para)
+    #
+    #     ft_transition_dict = {f_gps_seq: df[
+    #         [markov_field.FROM_STATE, markov_field.TO_STATE, 'trans_values']].set_index(
+    #         [markov_field.FROM_STATE, markov_field.TO_STATE]).unstack().values for (f_gps_seq, t_gps_seq), df in
+    #                           transition_df.groupby([gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ])}
+    #     print(rf'归并mat: {time.time() - t4}')
+    #
+    #     return adj_seq_path_dict, ft_transition_dict, ft_idx_map, s2s_route_l, seq_k_candidate_info, done_stp_cost_df
+
+
 if __name__ == '__main__':
     pass
     # a = LineString([(0, 0), (0, 1)])
     # z = a.segmentize(1/3 + 0.1 * 1/ 3)
     # print(z)
 
     # x = pd.DataFrame({'a': [1,2,3], 'b': [4,5,6]})
```

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/GlobalVal.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/GlobalVal.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/NetGen.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/NetGen.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,16 @@
                                     save_streets_after_modify_minimum=save_streets_after_modify_minimum,
                                     save_streets_before_modify_minimum=save_streets_before_modify_minimum)
         return link_gdf, node_gdf, node_group_status_gdf
 
     def topology_optimization(self, link_gdf: gpd.GeoDataFrame = None, node_gdf: gpd.GeoDataFrame = None,
                               out_fldr: str = None) -> \
             tuple[gpd.GeoDataFrame, gpd.GeoDataFrame, dict]:
-        assert self.limit_col_name in link_gdf.columns, rf'limit_col_name: {self.limit_col_name}, 该字段不在线层表中...'
+        if self.limit_col_name not in link_gdf.columns:
+            self.limit_col_name = None
         link_gdf, node_gdf, dup_info_dict = optimize(link_gdf=link_gdf, node_gdf=node_gdf,
                                                      ignore_dir=self.ignore_dir,
                                                      allow_ring=self.allow_ring,
                                                      limit_col_name=self.limit_col_name,
                                                      plain_prj=self.plain_prj,
                                                      accu_l_threshold=self.accu_l_threshold,
                                                      angle_threshold=self.angle_threshold,
```

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/Parse/gd_car_path.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/Parse/gd_car_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/GeoProcess.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/GeoProcess.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/GraphAna.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/GraphAna.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/IndexAna.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/IndexAna.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/od.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/PublicTools/od.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/Request/api/WebApi.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/Request/api/WebApi.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/Request/request_path.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/Request/request_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/Request/usage/bd_ts.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/Request/usage/bd_ts.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/Request/usage/gd_car_path.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/Request/usage/gd_car_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Tools/process.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/Tools/process.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/conn.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/conn.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/increment.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/increment.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/net_reverse.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/net_reverse.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/optimize_net.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/optimize_net.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from ..book_mark import generate_book_mark
 from .DupProcess.DupLinks import process_dup_link
 from .Merge.merge_links import merge_two_degrees_node
 from .MultiCoreMerge.merge_links_multi import merge_links_multi
 
 
 def optimize(link_gdf: gpd.GeoDataFrame = None, node_gdf: gpd.GeoDataFrame = None, ignore_dir: bool = False,
-             allow_ring: bool = False, limit_col_name: str = 'road_name', plain_prj: str = 'EPSG:32650',
+             allow_ring: bool = False, limit_col_name: str = None, plain_prj: str = 'EPSG:32650',
              accu_l_threshold: float = 500.0, angle_threshold: float = 15.0, restrict_length: bool = True,
              restrict_angle: bool = True, save_preliminary: bool = True, out_fldr: str = None,
              is_process_dup_link: bool = True, process_dup_link_buffer: float = 0.75, min_length: float = 50.0,
              dup_link_buffer_ratio: float = 60.0, modify_minimum_buffer: float = 0.8, multi_core: bool = False,
              core_num: int = 3) -> \
         tuple[gpd.GeoDataFrame, gpd.GeoDataFrame, dict]:
     """crs input: EPSG:4326
```

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/save_file.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/RoadNet/save_file.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/book_mark.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/book_mark.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netreverse/format_od.py` & `gotrackit-0.2.2/src/gotrackit/netreverse/format_od.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/netxfer/SumoConvert.py` & `gotrackit-0.2.2/src/gotrackit/netxfer/SumoConvert.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/solver/Viterbi.py` & `gotrackit-0.2.2/src/gotrackit/solver/Viterbi.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,14 @@
         if self.use_log_p:
             self.zeta_array_dict[self.o_seq_list[0]] = np.log((1 / init_n) * init_b.astype(float))
         else:
             self.zeta_array_dict[self.o_seq_list[0]] = (1 / init_n) * init_b
 
         # print(rf'初始化后:{self.zeta_array_dict[0]}')
 
-    @function_time_cost
     def iter_model(self) -> list[int]:
         """动态规划迭代求解"""
 
         # 1.迭代状态转移(i状态向 i + 1状态 转移)
         for i, o in enumerate(self.o_seq_list[:-1]):
 
             # 第i个观测点的各状态的概率 * (i -> i + 1)状态转移概率 * 当前状态的概率
```

### Comparing `gotrackit-0.2.1/src/gotrackit/tools/coord_trans.py` & `gotrackit-0.2.2/src/gotrackit/tools/coord_trans.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/tools/geo_process.py` & `gotrackit-0.2.2/src/gotrackit/tools/geo_process.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/tools/group.py` & `gotrackit-0.2.2/src/gotrackit/tools/group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/tools/save_file.py` & `gotrackit-0.2.2/src/gotrackit/tools/save_file.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit/visualization.py` & `gotrackit-0.2.2/src/gotrackit/visualization.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.1/src/gotrackit.egg-info/SOURCES.txt` & `gotrackit-0.2.2/src/gotrackit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

