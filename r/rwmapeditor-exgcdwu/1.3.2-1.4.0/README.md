# Comparing `tmp/rwmapeditor_exgcdwu-1.3.2.tar.gz` & `tmp/rwmapeditor_exgcdwu-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwmapeditor_exgcdwu-1.3.2.tar", last modified: Sun Apr 21 15:36:14 2024, max compression
+gzip compressed data, was "rwmapeditor_exgcdwu-1.4.0.tar", last modified: Sat Apr 27 09:38:35 2024, max compression
```

## Comparing `rwmapeditor_exgcdwu-1.3.2.tar` & `rwmapeditor_exgcdwu-1.4.0.tar`

### file list

```diff
@@ -1,312 +1,320 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:14.327436 rwmapeditor_exgcdwu-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    41868 2024-04-21 15:36:14.327436 rwmapeditor_exgcdwu-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:14.275436 rwmapeditor_exgcdwu-1.3.2/rwmap/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:14.275436 rwmapeditor_exgcdwu-1.3.2/rwmap/_case/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_case/_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_case/_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_case/_objectgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_case/_tileset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:14.275436 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:14.275436 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/otgroup_grid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/otgroup_grid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:14.275436 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tile_group_grid/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tile_group_grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tile_group_grid/_tile_group_addlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tile_group_grid/_tile_group_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tile_group_grid/_tile_group_one.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:14.279436 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject/_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject/_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject/_mapText.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject/_mapinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject/_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject/_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject/_tobject_one.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject/_unitAdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject/_unitDetect.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject/_unitRemove.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:14.279436 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject_group/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject_group/_city.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject_group/_refresh_building.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:14.279436 rwmapeditor_exgcdwu-1.3.2/rwmap/_frame/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_frame/_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_frame/_element_ori.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_frame/_element_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:14.279436 rwmapeditor_exgcdwu-1.3.2/rwmap/_object/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_object/_object_global.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_object/_object_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_object/_object_one_and_acti.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_object/_object_pos.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_object/_object_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_object/_object_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:14.279436 rwmapeditor_exgcdwu-1.3.2/rwmap/_otgroup/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_otgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_otgroup/_object_tile_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:14.279436 rwmapeditor_exgcdwu-1.3.2/rwmap/_tile/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_tile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_tile/_tile_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:14.283436 rwmapeditor_exgcdwu-1.3.2/rwmap/_util/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_util/_add_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_util/_class_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_util/_dict_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_util/_etElement_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_util/_list_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_util/_png_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/_util/_str_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:14.283436 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:14.283436 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:14.315436 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/
--rw-r--r--   0 runner    (1001) docker     (127)    66356 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/bridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/decoration.png
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/deepwater.png
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt.png
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt_details.png
--rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dust.png
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/fauna.png
--rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/fauna_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/fauna_highland.png
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice.png
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/lava.png
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/lava2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/lava2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass.png
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16002 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16661 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    17103 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    17019 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/misc.png
--rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain.png
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9946 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    14341 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/nothing2road_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand.png
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2.png
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2_old.png
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    19617 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10227 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2sand_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    23903 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/shallowwater.png
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/shortgrass.png
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow.png
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2snow_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone.png
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2lava.png
--rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2snow.png
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)   111877 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/units.png
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/water.png
--rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/decoration.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/misc.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:14.323436 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Dirt Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Dirt ShalowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Ice Ice - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Ice ShallowWater - Broken.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Ice ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/LongGrass Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/LongGrass Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/LongGrass LongGrass - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/LongGrass ShortGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Mountain Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Mountain Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Mountain LongGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Mountain Mountain - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Mountain Mountain - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Mountain Nothing - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Mountain Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Mountain ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Mountain Snow - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Mountain Stone - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Nothing Dust - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Nothing Road - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Nothing Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Sand Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Sand Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Sand LandGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Sand Nothing - Flat - 2.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Sand Nothing - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Sand Sand - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Sand ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Sand ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/ShallowWater Water - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Snow Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Snow Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Snow Ice - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Snow Snow - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Snow Snow - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Stone Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Stone ShallowWater - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Stone Snow - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Water DeepWater - Flat.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:14.327436 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/terrain/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/terrain/Deep Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/terrain/Dirt.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/terrain/Dirt_Details.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/terrain/Dust.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/terrain/Ice.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/terrain/Lava.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/terrain/Long Grass.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/terrain/Mountain.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/terrain/Sand.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/terrain/Shallow Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/terrain/Short Grass.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/terrain/Snow.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/terrain/Stone.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/terrain/Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/units.tsx
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:36:14.327436 rwmapeditor_exgcdwu-1.3.2/rwmapeditor_exgcdwu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41868 2024-04-21 15:36:14.000000 rwmapeditor_exgcdwu-1.3.2/rwmapeditor_exgcdwu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13710 2024-04-21 15:36:14.000000 rwmapeditor_exgcdwu-1.3.2/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 15:36:14.000000 rwmapeditor_exgcdwu-1.3.2/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 15:36:14.000000 rwmapeditor_exgcdwu-1.3.2/rwmapeditor_exgcdwu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 15:36:14.000000 rwmapeditor_exgcdwu-1.3.2/rwmapeditor_exgcdwu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 15:36:14.327436 rwmapeditor_exgcdwu-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-21 15:36:06.000000 rwmapeditor_exgcdwu-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.366977 rwmapeditor_exgcdwu-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    42034 2024-04-27 09:38:35.366977 rwmapeditor_exgcdwu-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.318976 rwmapeditor_exgcdwu-1.4.0/rwmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.318976 rwmapeditor_exgcdwu-1.4.0/rwmap/_case/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_case/_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_case/_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_case/_objectgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_case/_tileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10669 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.318976 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.318976 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/otgroup_grid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/otgroup_grid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.318976 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tile_group_grid/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tile_group_grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tile_group_grid/_tile_group_addlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tile_group_grid/_tile_group_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tile_group_grid/_tile_group_one.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.322977 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_mapText.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_mapinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_unitAdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_unitDetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_unitRemove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.322977 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.322977 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13710 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/_city.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/_city_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/_city_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/_city_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/_normal_unit_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14857 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/_refresh_building.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.322977 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_troop/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_troop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_troop/_troop_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.322977 rwmapeditor_exgcdwu-1.4.0/rwmap/_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_frame/_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_frame/_element_ori.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_frame/_element_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.326977 rwmapeditor_exgcdwu-1.4.0/rwmap/_object/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_one_and_acti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.326977 rwmapeditor_exgcdwu-1.4.0/rwmap/_otgroup/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_otgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_otgroup/_object_tile_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.326977 rwmapeditor_exgcdwu-1.4.0/rwmap/_tile/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_tile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_tile/_tile_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.326977 rwmapeditor_exgcdwu-1.4.0/rwmap/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_add_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_class_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_etElement_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_list_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_png_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_str_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.326977 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.326977 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.354977 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)    66356 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/bridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/decoration.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/deepwater.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt_details.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dust.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/fauna.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/fauna_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/fauna_highland.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16002 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16661 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17103 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17019 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/misc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9946 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14341 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/nothing2road_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2_old.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19617 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10227 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2sand_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23903 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shortgrass.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2snow_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2lava.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2snow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)   111877 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/units.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/water.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/decoration.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/misc.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.362977 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Dirt Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Dirt ShalowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Ice Ice - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Ice ShallowWater - Broken.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Ice ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/LongGrass Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/LongGrass Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/LongGrass LongGrass - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/LongGrass ShortGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain LongGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Mountain - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Mountain - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Nothing - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Snow - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Stone - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Nothing Dust - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Nothing Road - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Nothing Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand LandGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand Nothing - Flat - 2.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand Nothing - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand Sand - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/ShallowWater Water - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Snow Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Snow Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Snow Ice - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Snow Snow - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Snow Snow - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Stone Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Stone ShallowWater - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Stone Snow - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Water DeepWater - Flat.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.366977 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Deep Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Dirt.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Dirt_Details.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Dust.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Ice.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Lava.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Long Grass.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Mountain.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Sand.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Shallow Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Short Grass.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Snow.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Stone.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/units.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.366977 rwmapeditor_exgcdwu-1.4.0/rwmapeditor_exgcdwu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42034 2024-04-27 09:38:35.000000 rwmapeditor_exgcdwu-1.4.0/rwmapeditor_exgcdwu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14016 2024-04-27 09:38:35.000000 rwmapeditor_exgcdwu-1.4.0/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 09:38:35.000000 rwmapeditor_exgcdwu-1.4.0/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-27 09:38:35.000000 rwmapeditor_exgcdwu-1.4.0/rwmapeditor_exgcdwu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-27 09:38:35.000000 rwmapeditor_exgcdwu-1.4.0/rwmapeditor_exgcdwu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-27 09:38:35.366977 rwmapeditor_exgcdwu-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/setup.py
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/LICENSE` & `rwmapeditor_exgcdwu-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/PKG-INFO` & `rwmapeditor_exgcdwu-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.3.2
+Version: 1.4.0
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -688,14 +688,16 @@
 
 ___一个铁锈战争 (Rusted Warfare) 地图编辑 python 库___
 
 ![released version](https://img.shields.io/pypi/v/rwmapeditor-exgcdwu.svg)
 
 [简易使用教程](https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-/blob/main/Tutorial.md)
 
+[简单城夺地图代码例子](https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-/blob/main/examples/example1/example1.py)
+
 ## 目标
 
 python实现铁锈地图文件地块编辑和宾语编辑。
 
 暂时不打算接触地块集。
 
 重点减轻城市争夺地图的宾语编辑工作量
@@ -712,15 +714,15 @@
 pip install rwmapeditor-exgcdwu
 ```
 
 ## 使用之前
 
 ### 1.使用地图编辑器(Tiled,notTiled)创建新地图
 
-地图格式：zlib、gzip
+地图格式：zlib、gzip、纯base64
 
 渲染顺序：右下(right-down)
 
 方向：orthogonal
 
 #### 2.手动载入地块集
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_case/_layer.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_case/_layer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,67 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 import xml.etree.ElementTree as et
 import numpy as np
+from copy import deepcopy
+from typing import Union
 
 import rwmap._util as utility
 import rwmap._frame as frame
 from rwmap._frame._element_ori import ElementOri
 from rwmap._frame._element_property import ElementProperties
 
+
 class Layer(ElementOri):
-    def __init__(self, properties:ElementProperties, tilematrix:np.ndarray, encoding:str, compression:str)->None:
+    def __init__(self, properties:ElementProperties, tilematrix:np.ndarray, encoding:str, compression:Union[str, None])->None:
         super().__init__(properties)
-        self._tilematrix = tilematrix
-        self._encoding = encoding
-        self._compression = compression
+        self._tilematrix = deepcopy(tilematrix)
+        self._encoding = deepcopy(encoding)
+        self._compression = deepcopy(compression)
     @classmethod
     def init_etElement(cls, root:et.Element)->None:
         properties = ElementProperties.init_etElement(root)
-        data = utility.get_etElement_callable_from_tag(root, "data")
+        data = utility.get_etElement_callable_from_tag_s(root, "data")
         _tilematrix = utility.get_etElement_ndarray_from_text_packed(data, frame.Coordinate(root.attrib['width'], root.attrib['height']))
-        return cls(properties, _tilematrix, data.attrib["encoding"], data.attrib["compression"])
+        return cls(properties, _tilematrix, data.attrib["encoding"], data.attrib.get("compression"))
 
     def output_str(self, output_rectangle:frame.Rectangle = frame.Rectangle(frame.Coordinate(), frame.Coordinate(-1, -1)))->str:
         str_ans = ""
         str_ans = str_ans + self._properties.output_str() + "\n"
         str_ans = str_ans + "".join([" ".join([str(self._tilematrix[i][j]) for j in range(max(output_rectangle.i().y(), 0), min(output_rectangle.e().y(), self._tilematrix.shape[1]))]) + "\n"
                                  for i in range(max(output_rectangle.i().x(), 0), min(output_rectangle.e().x(), self._tilematrix.shape[0]))]) + "\n"
         str_ans = utility.indentstr_Tab(str_ans)
         return str_ans
 
     def output_etElement(self)->et.Element:
         root = et.Element("layer")
-        self._properties.output_etElement(root)
+        root = self._properties.output_etElement(root)
         root.append(utility.get_etElement_from_text_packed(self._tilematrix, self._encoding, self._compression))
         return root
     
+    def name(self)->str:
+        return self._properties.returnDefaultProperty("name")
+    
+    def size(self)->frame.Coordinate:
+        return frame.Coordinate(int(self._properties.returnDefaultProperty("width")), 
+                                int(self._properties.returnDefaultProperty("height")))
+
     def __repr__(self)->str:
         return self.output_str()
 
     def id(self)->int:
         return int(self._properties.default_properties["id"])
     
     def tileid(self, place_grid:frame.Coordinate)->int:
         return int(self._tilematrix[place_grid.x()][place_grid.y()])
     
     def assigntileid(self, place_grid:frame.Coordinate, tileid:int):
         self._tilematrix[place_grid.y()][place_grid.x()] = tileid
+
+    def assigntileid_square(self, square_grid:frame.Rectangle, tileid:int):
+        self._tilematrix[square_grid.i().y():square_grid.e().y()][square_grid.i().x():square_grid.e().x()] = tileid
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_case/_object.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_case/_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import xml.etree.ElementTree as et
+from copy import deepcopy
+from typing import Union
 
 import rwmap._frame as frame
 import rwmap._util as utility
 from rwmap._frame._element_property import ElementProperties
 
 class TObject(ElementProperties):
-    def __init__(self, tag:str, default_properties:dict[str, str] = {}, optional_properties:dict[str, str] = {}, other_properties:list[et.Element] = [])->None:
+    def __init__(self, tag:str, default_properties:dict[str, str] = {}, optional_properties:dict[str, Union[str, dict[str, str]]] = {}, other_properties:list[et.Element] = [])->None:
         super().__init__(tag, default_properties, optional_properties)
-        self._other_properties = other_properties
+        self._other_properties = deepcopy(other_properties)
         
     @classmethod
     def init_etElement(cls, root:et.Element):
         if root == None:
             return None
-        optional_properties = utility.get_etElement_properties(utility.get_etElement_callable_from_tag(root, "properties"))
+        optional_properties = utility.get_etElement_properties(utility.get_etElement_callable_from_tag_s(root, "properties"))
         other_properties = []
         for etEle in root:
             if etEle.tag != "properties":
-                other_properties.append(etEle)
+                other_properties.append(deepcopy(etEle))
         return cls(root.tag, root.attrib, optional_properties, other_properties)
     
-    def output_etElement(self, root:et.Element)->None:
-        super().output_etElement(root)
+    def output_etElement(self, root:et.Element)->et.Element:
+        etElement_ans = super().output_etElement(root)
         for etEle in self._other_properties:
-            root.append(etEle)
+            etElement_ans.append(deepcopy(etEle))
+        return etElement_ans
         
     def output_str(self)->str:
         str_ans = super().output_str()
         str_add = "other_properties:" + str(self._other_properties) + "\n"
         str_add = utility.indentstr_Tab(str_ans)
         str_ans = str_ans + str_add
         return str_ans
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_case/_objectgroup.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_case/_objectgroup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 
 import xml.etree.ElementTree as et
+from copy import deepcopy
+from typing import Union
 
 import rwmap._util as utility
 import rwmap._frame as frame
 from rwmap._case._object import TObject
 from rwmap._frame._element_ori import ElementOri
 from rwmap._frame._element_property import ElementProperties
 
 class ObjectGroup(ElementOri):
     def __init__(self, properties:ElementProperties, object_list:list[TObject])->None:
         super().__init__(properties)
-        self._object_list = object_list
+        self._object_list = deepcopy(object_list)
 
     def __iter__(self):
         return self._object_list
 
     @classmethod
     def init_etElement(cls, root:et.Element)->None:
         properties = ElementProperties.init_etElement(root)
         object_list = [TObject.init_etElement(tobject) for tobject in root if tobject.tag == "object"]
         return cls(properties, object_list)
     
     def output_str(self, objectnum:int = -1)->str:
         str_ans = ""
         str_ans = str_ans + self._properties.output_str() + "\n"
-        str_ans = str_ans + "".join([self._object_list[i].output_str() + "\n" for i in range(0, -1)]) + "\n"
+        str_ans = str_ans + "".join([self._object_list[i].output_str() + "\n" for i in range(0, min(len(self._object_list), objectnum))]) + "\n"
         str_ans = utility.indentstr_Tab(str_ans)
         return str_ans
     
+    def name(self)->str:
+        return self._properties.returnDefaultProperty("name")
+
     def __repr__(self)->str:
         return self.output_str()
 
     def output_etElement(self)->et.Element:
         root = et.Element("objectgroup")
-        self._properties.output_etElement(root)
+        root = self._properties.output_etElement(root)
         for tobject in self._object_list:
             tobject_element = et.Element("object")
-            tobject.output_etElement(tobject_element)
+            tobject_element = tobject.output_etElement(tobject_element)
             root.append(tobject_element)
         return root
     
-    def addObject(self, default_properties:dict[str, str] = {}, optional_properties:dict[str, str] = {}, other_properties:list[et.Element] = [])->None:
+    def addObject(self, default_properties:dict[str, str] = {}, optional_properties:dict[str, Union[str, dict[str, str]]] = {}, other_properties:list[et.Element] = [])->None:
         self._object_list.append(TObject("object", default_properties, optional_properties, other_properties))
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_case/_tileset.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_case/_tileset.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,63 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 import xml.etree.ElementTree as et
+from copy import deepcopy
 
 import rwmap._util as utility
 import rwmap._frame as frame
 import rwmap._exceptions as exception
 from rwmap._frame._element_ori import ElementOri
 from rwmap._frame._element_property import ElementProperties
 
 class TileSet(ElementOri):
     def __init__(self, properties:ElementProperties, size:frame.Coordinate, image_properties:ElementProperties = None,
                   png_text:str = None, tilelist_properties:list[ElementProperties] = None)->None:
         super().__init__(properties)
-        self._size = size
-        self._image_properties = image_properties
-        self._png_text = png_text
-        self._tilelist_properties = tilelist_properties
+        self._size = deepcopy(size)
+        self._image_properties = deepcopy(image_properties)
+        self._png_text = deepcopy(png_text)
+        self._tilelist_properties = deepcopy(tilelist_properties)
     @classmethod
     def init_etElement(cls, root:et.Element, rwmaps_dir:str)->None:
-        png_text_pro = utility.get_etElement_callable_from_tag(root, "properties")
-        png_text = utility.get_etElement_name_to_text_rm(png_text_pro, "embedded_png")
+        png_text_pro = utility.get_etElement_callable_from_tag_s(root, "properties")
+        png_text = utility.get_etElement_name_to_text_s(png_text_pro, "embedded_png")
         properties = ElementProperties.init_etElement(root)
-        image_properties = ElementProperties.init_etElement(utility.get_etElement_callable_from_tag(root, "image"))
+        if png_text != None:
+            properties.deleteOptionalProperty("embedded_png")
+        image_properties = ElementProperties.init_etElement(utility.get_etElement_callable_from_tag_s(root, "image"))
         tilelist_properties = [ElementProperties.init_etElement(tile) for tile in root if tile.tag == "tile"]
         tilelist_properties = None if tilelist_properties == [] else tilelist_properties
         
         if properties.returnDefaultProperty("columns") == None:
-            source_file = properties.returnDefaultProperty("source")
 
+            source_file = properties.returnDefaultProperty("source")
+            source_list = source_file.split("/")
+            source_list = source_list[utility.search_list_to_index(source_list, "maps") + 1:]
+            source_list = source_list[utility.search_list_to_index(source_list, "tilesets") + 1:]
+            source_file = "/".join(source_list)
             source = rwmaps_dir + source_file
+
             root = et.ElementTree(file = source).getroot()
-            #if root.attrib.get("columns") == None:
             tilewidth = int(root.attrib["tilewidth"])
             tileheight = int(root.attrib["tileheight"])
-            image_element = utility.get_etElement_callable_from_tag(root, "image")
-            if image_element.attrib.get("width") == None:
+
+            if root.attrib.get("columns") == None:
+                image_element = utility.get_etElement_callable_from_tag_s(root, "image")
                 image_file = rwmaps_dir + "bitmaps/" + image_element.attrib["source"].split("/")[-1]
                 width = utility.image_width(image_file)
                 height = utility.image_height(image_file)
+
+                column = int(width / tilewidth)
+                row = int(height / tileheight)
             else:
-                width = int(image_element.attrib["width"])
-                height = int(image_element.attrib["height"])
-            column = int(width / tilewidth)
-            row = int(height / tileheight)
-            #else:
-                #column = int(root.attrib["columns"])
-                #row = int(int(root.attrib["tilecount"]) / column)
+                column = int(root.attrib["columns"])
+                row = int(int(root.attrib["tilecount"]) / column)
 
         else:
             column = int(properties.returnDefaultProperty("columns"))
             row = int(int(properties.returnDefaultProperty("tilecount")) / column)
         size = frame.Coordinate(row, column)
         return cls(properties, size, image_properties, png_text, tilelist_properties)
     
@@ -69,45 +75,75 @@
         return str_ans
     
     def __repr__(self)->str:
         return self.output_str()
 
     def output_etElement(self)->et.Element:
         root = et.Element("tileset")
-        self._properties.output_etElement(root)
+        root = self._properties.output_etElement(root)
         if self._image_properties != None:
             image_element = et.Element("image")
-            self._image_properties.output_etElement(image_element)
+            image_element = self._image_properties.output_etElement(image_element)
             root.append(image_element)
         if self._png_text != None:
             png_element = et.Element("property", {"name": "embedded_png"})
             png_element.text = self._png_text
-            properties = utility.get_etElement_callable_from_tag(root, "properties")
+            properties = utility.get_etElement_callable_from_tag_s(root, "properties")
             properties.insert(0, png_element)
         if self._tilelist_properties != None:
             for tile in self._tilelist_properties:
                 tile_element = et.Element("tile")
-                tile.output_etElement(tile_element)
+                tile_element = tile.output_etElement(tile_element)
                 root.append(tile_element)
         return root
     
-    def output_name(self)->str:
+    def name(self)->str:
         tileset_name = self._properties.returnDefaultProperty("name")
         if tileset_name == None:
             tileset_name = self._properties.returnDefaultProperty("source")
         tileset_name = utility.str_slash_to_dot(tileset_name)
         return tileset_name
     
-    def tileid(self, tile_grid:frame.Coordinate)->int:
+    def totalgid(self)->int:
+        return self._size.x() * self._size.y()
+
+    def firstgid(self)->int:
+        return int(self._properties.returnDefaultProperty("firstgid"))
+    
+    def endgid(self)->int:
+        return self.firstgid() + self.totalgid()
+
+    def gid_to_tileid(self, gid:int)->tuple[str, int]:
+        tileid = gid - self.firstgid()
+        if tileid < 0:
+            raise IndexError("The gid cannot be loaded into the current tileset.")
+        return (self.name(), gid - self.firstgid())
+    
+    def tileid_to_gid(self, tileid:int)->int:
+        return self.firstgid() + tileid
+    
+    def tileid_to_coo(self, tileid:int)->frame.TagCoordinate:
+        if tileid < self.totalgid:
+            tagcoo = frame.TagCoordinate.init_id(self.name(), tileid, self._size.y())
+        else:
+            raise exception.CoordinateIndexError(f"Beyond the boundary of this tileset{self.name()}")
+        return tagcoo
+
+    def coo_to_tileid(self, tile_grid:frame.Coordinate)->int:
         if tile_grid < self._size:
-            id_now = tile_grid.id(self._size.y())
-            id_ans = int(self._properties.returnDefaultProperty("firstgid")) + id_now
+            id_ans = tile_grid.id(self._size.y())
         else:
-            raise exception.CoordinateIndexError(f"Beyond the boundary of this tileset{self.output_name()}")
+            raise exception.CoordinateIndexError(f"Beyond the boundary of this tileset{self.name()}")
         return id_ans
     
+    def coo_to_gid(self, tile_grid:frame.Coordinate)->int:
+        return self.coo_to_tileid(tile_grid) + self.firstgid()
+    
+    def gid_to_coo(self, gid:int)->frame.TagCoordinate:
+        return self.tileid_to_coo(self.gid_to_tileid(gid))
+
     def isexist(self)->bool:
         return self._properties.returnDefaultProperty("firstgid") != "0"
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_core.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,87 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 import xml.etree.ElementTree as et
 import re
 import os
-from typing import Generator
+from copy import deepcopy
+from typing import Generator, Union
+from numbers import Integral
 
 import rwmap._exceptions as rwexceptions
 import rwmap._util as utility
 import rwmap._case as case
 import rwmap._frame as frame
 from rwmap._frame._element_ori import ElementOri
 from rwmap._frame._element_property import ElementProperties
 import rwmap._tile as tile
 import rwmap._object as object
 import rwmap._otgroup as otgroup
+import rwmap._data.const as const
 
 
 RWMAP_DIR = os.path.dirname(__file__)
 RWMAP_MAPS = RWMAP_DIR + "/other_data/maps/"
 
 class RWmap(ElementOri):
     def __init__(self, properties:ElementProperties, tileset_list:list[case.TileSet],
                   layer_list:list[case.Layer], objectGroup_list:list[case.ObjectGroup])->None:
         super().__init__(properties)
-        self._tileset_list = tileset_list
-        self._layer_list = layer_list
-        self._objectGroup_list = objectGroup_list
+        self._tileset_list = deepcopy(tileset_list)
+        self._layer_list = deepcopy(layer_list)
+        self._objectGroup_list = deepcopy(objectGroup_list)
     @classmethod
-    def init_mapfile(cls, map_file:str, rwmaps_dir = RWMAP_MAPS)->None:
+    def init_mapfile(cls, map_file:str, rwmaps_dir = RWMAP_MAPS):
         xmlTree:et.ElementTree = et.ElementTree(file=map_file)
         root:et.Element = xmlTree.getroot()
         properties = ElementProperties.init_etElement(root)
 
         tileset_list = [case.TileSet(ElementProperties("tileset", {"firstgid": "0", "name": "empty"}), frame.Coordinate(1, 1))]
         tileset_list = tileset_list + [case.TileSet.init_etElement(tileset, rwmaps_dir) for tileset in root if tileset.tag == "tileset"]
         layer_list = [case.Layer.init_etElement(layer) for layer in root if layer.tag == "layer"]
         objectGroup_list = [case.ObjectGroup.init_etElement(objectGroup) for objectGroup in root if objectGroup.tag == "objectgroup"]  
         
-        tileset_list = None if tileset_list == [] else tileset_list
-        layer_list = None if layer_list == [] else layer_list
-        objectGroup_list = None if objectGroup_list == [] else objectGroup_list
-        
         return cls(properties, tileset_list, layer_list, objectGroup_list)
 
     def size(self)->frame.Coordinate:
         return frame.Coordinate(int(self._properties.returnDefaultProperty("width")), 
                                 int(self._properties.returnDefaultProperty("height")))
     
     def tile_size(self)->frame.Coordinate:
         return frame.Coordinate(int(self._properties.returnDefaultProperty("tilewidth")), 
                                 int(self._properties.returnDefaultProperty("tileheight")))
+    
+    def tileset_name_list(self)->list[str]:
+        return [tileset.name() for tileset in self._tileset_list]
+    
+    def layer_name_list(self)->list[str]:
+        return [layer.name() for layer in self._layer_list]
+    
+    def objectgroup_name_list(self)->list[str]:
+        return [objectgroup.name() for objectgroup in self._objectGroup_list]
+    
+    def get_layer_s(self, name:str)->case.Layer:
+        layer = utility.get_ElementOri_from_list_by_name_s(self._layer_list, name)
+        if layer == None:
+            raise KeyError("layer name:" + name + " not found")
+        return layer
+        
+    def get_tileset_s(self, name:str)->case.TileSet:
+        tileset = utility.get_ElementOri_from_list_by_name_s(self._tileset_list, name)
+        if tileset == None:
+            raise KeyError("tileset name:" + name + " not found")
+        return tileset
+        
+    def get_objectgroup_s(self, name:str)->case.ObjectGroup:
+        objectgroup = utility.get_ElementOri_from_list_by_name_s(self._objectGroup_list, name)
+        if objectgroup == None:
+            raise KeyError("objectgroup name:" + name + " not found")
+        return objectgroup
 
     def output_str(self, pngtextnum:int = -1, tilenum:int = -1, output_rectangle:frame.Rectangle = frame.Rectangle(frame.Coordinate(), frame.Coordinate(-1, -1)), objectnum:int = -1)->str:
         str_ans = ""
         str_ans = str_ans + self._properties.output_str() + "\n"
         str_ans = str_ans + "\n".join([tileset.output_str(pngtextnum, tilenum) for tileset in self._tileset_list if tileset.isexist()]) + "\n"
         str_ans = str_ans + "\n".join([layer.output_str(output_rectangle) for layer in self._layer_list]) + "\n"
         str_ans = str_ans + "\n".join([tobject.output_str(objectnum) for tobject in self._objectGroup_list]) + "\n"
@@ -63,15 +89,15 @@
         return str_ans
 
     def __repr__(self)->str:
         return self.output_str()
 
     def output_etElement(self)->et.Element:
         root = et.Element("map")
-        self._properties.output_etElement(root)
+        root = self._properties.output_etElement(root)
         if self._tileset_list != None:
             for tileset in self._tileset_list:
                 if tileset.isexist():
                     root.append(tileset.output_etElement())
         if self._layer_list != None:
             for layer in self._layer_list:
                 root.append(layer.output_etElement())
@@ -79,34 +105,45 @@
             for objectGroup in self._objectGroup_list:
                 root.append(objectGroup.output_etElement())
         return root
     
     def write_file(self, map_file:str)->None:
         utility.output_file_from_etElement(self.output_etElement(), map_file)
 
-    def addObject(self, objectGroup_name:str, default_properties:dict[str, str] = {}, optional_properties :dict[str, str] = {}, other_properties:list[et.Element] = [])->None:
-        objectGroup_now:case.ObjectGroup = utility.get_ElementOri_from_list_by_name(self._objectGroup_list, objectGroup_name)
+    def addObject_dict(self, objectGroup_name:str, default_properties:dict[str, str] = {}, optional_properties :dict[str, Union[str, dict[str, str]]] = {}, other_properties:list[et.Element] = [])->None:
+        objectGroup_now:case.ObjectGroup = utility.get_ElementOri_from_list_by_name_s(self._objectGroup_list, objectGroup_name)
         if objectGroup_now == None:
             raise KeyError("objectGroup name:" + objectGroup_name + " not found")
-        objectGroup_now.addObject(default_properties, optional_properties, other_properties)
-        if default_properties.get("id") == None:
-            default_properties["id"] = self._properties.returnDefaultProperty("nextobjectid")
-        str_nextobjectid = str(max(int(self._properties.returnDefaultProperty("nextobjectid")), int(default_properties["id"]) + 1))
+        default_properties_n = deepcopy(default_properties)
+        if default_properties_n.get("id") == None:
+            default_properties_n["id"] = self._properties.returnDefaultProperty("nextobjectid")
+        objectGroup_now.addObject(default_properties_n, optional_properties, other_properties)
+        str_nextobjectid = str(max(int(self._properties.returnDefaultProperty("nextobjectid")), int(default_properties_n["id"]) + 1))
         self._properties.assignDefaultProperty("nextobjectid", str_nextobjectid)
     
-    def addObject_one(self, tobject:object.TObject_One, offset:frame.Coordinate = frame.Coordinate()):
-        ntobject = tobject.offset(offset)
-        self.addObject("Triggers", ntobject.default_properties(), ntobject.optional_properties(), ntobject.other_properties())
+    def addObject_one(self, tobject_one:object.TObject_One, offset:frame.Coordinate = frame.Coordinate()):
+        ntobject = tobject_one.offset(offset)
+        self.addObject_dict("Triggers", ntobject.default_properties(), ntobject.optional_properties(), ntobject.other_properties())
 
     def addObject_group(self, tobject_group:object.TObject_Group, offset:frame.Coordinate = frame.Coordinate()):
         for tobject in tobject_group._TObject_One_list:
             self.addObject_one(tobject, offset)
+        for tobject_group in tobject_group._TObject_Group_list:
+            self.addObject_group(tobject_group, offset)
+
+    def addObject(self, tobject:Union[object.TObject_One, object.TObject_Group], offset:frame.Coordinate = frame.Coordinate()):
+        if isinstance(tobject, object.TObject_One):
+            self.addObject_one(tobject, offset)
+        elif isinstance(tobject, object.TObject_Group):
+            self.addObject_group(tobject, offset)
+        else:
+            raise TypeError("The type of RWmap.addObject(tobject, ...) is wrong.")
 
-    def iterator_object(self, objectGroup_name:str, default_re:dict[str, str] = {}, optional_re:dict[str, str] = {})->Generator[case.TObject, None, None]:
-        objectGroup_now:case.ObjectGroup = utility.get_ElementOri_from_list_by_name(self._objectGroup_list, objectGroup_name)
+    def iterator_object_s(self, objectGroup_name:str, default_re:dict[str, str] = {}, optional_re:dict[str, str] = {})->Generator[case.TObject, None, None]:
+        objectGroup_now:case.ObjectGroup = utility.get_ElementOri_from_list_by_name_s(self._objectGroup_list, objectGroup_name)
         if objectGroup_now == None:
             raise KeyError("objectGroup name:" + objectGroup_name + " not found")
         for tobject in objectGroup_now._object_list:
             tobject_sas:bool = True
             for dname, dvalue in default_re.items():
                 if dvalue != "":
                     if tobject.returnDefaultProperty(dname) == None or re.match(dvalue, tobject.returnDefaultProperty(dname)) == None:
@@ -118,49 +155,55 @@
                 if dvalue != "":
                     if tobject.returnOptionalProperty(dname) == None or re.match(dvalue, tobject.returnOptionalProperty(dname)) == None:
                         tobject_sas = False
                         break
             if tobject_sas == False:
                 continue
             yield tobject
+    
+    def _tileplace_to_gid(self, tileplace:Union[int, tuple[str, int], frame.TagCoordinate])->int:
+        if isinstance(tileplace, int):
+            tileplace_now = tileplace
+        elif isinstance(tileplace, tuple) and isinstance(tileplace[0], str) and isinstance(tileplace[1], int):
+            tileplace_now = self.get_tileset_s(tileplace[0]).tileid_to_gid(tileplace[1])
+        elif isinstance(tileplace, frame.TagCoordinate):
+            tileplace_now = self.get_tileset_s(tileplace.tag()).coo_to_gid(tileplace.place())
+        else:
+            raise TypeError("The type of RWmap.addTile(..., tileplace) is wrong.")
+        return tileplace_now
+
+    def addTile_gid(self, layerplace:frame.TagCoordinate, gid:int):
+        if gid >= 0 and isinstance(gid, Integral):
+            layer:case.Layer = self.get_layer_s(layerplace.tag())
+        else:
+            raise TypeError("gid is less than 0 or not integer.")
+        layer.assigntileid(layerplace.place(), gid)
+
+    def addTile(self, layerplace:frame.TagCoordinate, tileplace:Union[int, tuple[str, int], frame.TagCoordinate]):
+        tileplace_now = self._tileplace_to_gid(tileplace)
+        self.addTile_gid(layerplace, tileplace_now)
+
+    def addTile_square(self, layerRectangle:frame.TagRectangle, tileplace:Union[int, tuple[str, int], frame.TagCoordinate])->None:
+        tileplace_now = self._tileplace_to_gid(tileplace)
+        layer:case.Layer = self.get_layer_s(layerRectangle.tag())
+        layer.assigntileid_square(layerRectangle.rectangle(), tileplace_now)
 
-    def addTile_place(self, layerplace:frame.TagCoordinate, tileplace:frame.TagCoordinate):
-        layer:case.Layer = utility.get_ElementOri_from_list_by_name(self._layer_list, layerplace.tag())
-        if layer == None:
-            raise KeyError("layer name:" + layerplace.tag() + " not found")
-        for tileset_now in self._tileset_list:
-            if tileset_now.output_name() == tileplace.tag():
-                tileset = tileset_now
-        try:
-            layer.assigntileid(layerplace.place(), tileset.tileid(tileplace.place()))
-        except UnboundLocalError:
-            raise KeyError("tileset name:" + tileplace.tag() + " not found")
-
-    def addTile(self, layer_name:str, place_grid:frame.Coordinate, tileset_name:str, tile_grid:frame.Coordinate)->None:        
-        layer_name = layer_name.strip()
-        tileset_name = tileset_name.strip()
-        self.addTile_place(frame.TagCoordinate(layer_name, place_grid), \
-                           frame.TagCoordinate(tileset_name, tile_grid))
-
-    def addTile_group(self, original_grid:frame.Coordinate, tilegroup:tile.TileGroup_One):
+    def addTile_group(self, tilegroup:tile.TileGroup_One, original_grid:frame.Coordinate):
         for place_grid in tilegroup.size():
             layerplace = frame.TagCoordinate(tilegroup.layername(), original_grid + place_grid)
             tileplace = tilegroup[place_grid]
-            self.addTile_place(layerplace, tileplace)
+            if tileplace.tag() != "empty":
+                self.addTile(layerplace, tileplace)
 
-    def addTile_group_list(self, original_grid:frame.Coordinate, tilegroup_list:tile.TileGroup_List):
+    def addTile_group_list(self, tilegroup_list:tile.TileGroup_List, original_grid:frame.Coordinate):
         for tilegroup in tilegroup_list:
-            self.addTile_group(original_grid, tilegroup)
-
-    def addTile_square(self, layer_name:str, place_rectangle:frame.Rectangle, tileset_name:str, tile_grid:frame.Coordinate)->None:
-        for place_grid in place_rectangle:
-            self.addTile(layer_name, place_grid, tileset_name, tile_grid)
+            self.addTile_group(tilegroup, original_grid)
 
-    def add_OTGroup(self, otgroup:otgroup.OTGroup, offset_grid:frame.Coordinate = frame.Coordinate(), ):
-        self.addTile_group_list(offset_grid, otgroup._tilegroup_list)
+    def addOTGroup(self, otgroup:otgroup.OTGroup, offset_grid:frame.Coordinate = frame.Coordinate()):
+        self.addTile_group_list(otgroup._tilegroup_list, offset_grid)
         self.addObject_group(otgroup._tobject_group, offset_grid * self.tile_size())
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_data/const.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/const.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import rwmap._frame as frame
-
+from typing import Union
 
 class KEY:
     empty_tile = "0"
 
 class NAME:
     Ground = "Ground"
     Triggers = "Triggers"
@@ -27,10 +27,13 @@
     allBuildings = "allBuildings"
     commandCenter = "commandCenter"
     requiredObjectives = "requiredObjectives"
 
 class COO:
     SIZE_STANDARD = frame.Coordinate(20, 20)
 
+class TYPE:
+    tileid = Union[int, tuple[str, int], frame.TagCoordinate]
+
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject/_mapText.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_mapText.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import rwmap._object as object
 import rwmap._frame as frame
 import rwmap._data.const as const
 
 class MapText(object.TObject_One):
     def __init__(self, pos:frame.Coordinate, text:str, size:frame.Coordinate = const.COO.SIZE_STANDARD, 
                  textColor:str = None, textSize:int = -1, name:str = None,
-                 actiBy:list[object.TObject_One] = [], deactiBy:list[object.TObject_One] = [], 
+                 actiBy_s:list[object.TObject_One] = [], deactiBy_s:list[object.TObject_One] = [], 
                  isalltoacti:bool = False):
         upos = frame.Rectangle(pos - size / 2, size)
         object.TObject_One.__init__(self, object.TObject_Type.init_mapText(text, textColor = textColor, textSize = textSize), 
                                     object.TObject_Pos.init_rectangle(upos), name, 
-                                    object.TObject_Acti.init_acti(actiBy = actiBy, deactiBy = deactiBy, isalltoacti = isalltoacti))
+                                    object.TObject_Acti.init_acti(actiBy_s = actiBy_s, deactiBy_s = deactiBy_s, isalltoacti = isalltoacti))
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject/_mapinfo.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_mapinfo.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject/_message.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_message.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import rwmap._frame as frame
 import rwmap._data.const as const
 
 class Message(object.TObject_One):
     def __init__(self, pos:frame.Coordinate, message:str, size:frame.Coordinate = const.COO.SIZE_STANDARD, 
                  delayPerChar:int = -1, textColor:str = None, 
                  name:str = None, warmup:int = -1, reset:int = -1, 
-                 actiBy:list[object.TObject_One] = [], deactiBy:list[object.TObject_One] = [], 
+                 actiBy_s:list[object.TObject_One] = [], deactiBy_s:list[object.TObject_One] = [], 
                  isalltoacti:bool = False):
         upos = frame.Rectangle(pos - size / 2, size)
         object.TObject_One.__init__(self, object.TObject_Type.init_mapText(None), 
                                     object.TObject_Pos.init_rectangle(upos), 
-                                    name, object.TObject_Acti.init_acti(actiBy = actiBy, deactiBy = deactiBy, isalltoacti = isalltoacti), 
+                                    name, object.TObject_Acti.init_acti(actiBy_s = actiBy_s, deactiBy_s = deactiBy_s, isalltoacti = isalltoacti), 
                                     object.TObject_Time.init_time(warmup = warmup, reset = reset), 
                                     object.TObject_Global.init_global(message = message, 
                                                                       delayPerChar = delayPerChar, textColor = textColor))
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject/_node.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import rwmap._object as object
 import rwmap._frame as frame
 import rwmap._data.const as const
 
 class Node(object.TObject_One):
     def __init__(self, pos:frame.Coordinate, size:frame.Coordinate = const.COO.SIZE_STANDARD, 
                  name:str = None, warmup:int = -1, reset:int = -1, 
-                 id:str = None, alsoacti:list[object.TObject_One] = [], 
-                 actiBy:list[object.TObject_One] = [], deactiBy:list[object.TObject_One] = [], 
+                 id:str = None, alsoacti_s:list[object.TObject_One] = [], 
+                 actiBy_s:list[object.TObject_One] = [], deactiBy_s:list[object.TObject_One] = [], 
                  isalltoacti:bool = False):
         upos = frame.Rectangle(pos - size / 2, size)
         object.TObject_One.__init__(self, object.TObject_Type.init_node(), 
                                     object.TObject_Pos.init_rectangle(upos), 
-                                    name, object.TObject_Acti.init_acti(id = id, alsoacti = alsoacti, 
-                                                                        actiBy = actiBy, deactiBy = deactiBy, 
+                                    name, object.TObject_Acti.init_acti(id = id, alsoacti_s = alsoacti_s, 
+                                                                        actiBy_s = actiBy_s, deactiBy_s = deactiBy_s, 
                                                                         isalltoacti = isalltoacti), 
                                     object.TObject_Time.init_time(warmup = warmup, reset = reset))
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject/_unitAdd.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_unitAdd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import rwmap._object as object
 import rwmap._frame as frame
 import rwmap._data.const as const
 
 class UnitAdd(object.TObject_One):
     def __init__(self, pos: frame.Coordinate, team:int, spawnUnits:str, size:frame.Coordinate = const.COO.SIZE_STANDARD, 
                  name:str = None, techLevel:int = -1, warmup:int = -1, reset:int = -1, 
-                 actiBy:list[object.TObject_One] = [], deactiBy:list[object.TObject_One] = [], 
+                 actiBy_s:list[object.TObject_One] = [], deactiBy_s:list[object.TObject_One] = [], 
                  isalltoacti:bool = False):
         upos = frame.Rectangle(pos - size / 2, size)
         object.TObject_One.__init__(self, object.TObject_Type.init_unitAdd(team, spawnUnits, techLevel), 
                                     object.TObject_Pos.init_rectangle(upos), name, 
-                                    object.TObject_Acti.init_acti(actiBy = actiBy, deactiBy = deactiBy, isalltoacti = isalltoacti), 
+                                    object.TObject_Acti.init_acti(actiBy_s = actiBy_s, deactiBy_s = deactiBy_s, isalltoacti = isalltoacti), 
                                     object.TObject_Time.init_time(warmup = warmup, reset = reset))
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject/_unitDetect.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_unitDetect.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 import rwmap._frame as frame
 import rwmap._data.const as const
 
 class UnitDetect(object.TObject_One):
     def __init__(self, pos:frame.Coordinate, size:frame.Coordinate, name:str = None,
                  team:int = None, minUnits:int = None, maxUnits:int = None, 
                  unitType:str = None, onlyList:list[str] = [], warmup:int = -1, reset:int = -1, 
-                 id:str = None, alsoacti:list[object.TObject_One] = []):
+                 id:str = None, alsoacti_s:list[object.TObject_One] = []):
         upos = frame.Rectangle(pos - size / 2, size)
         object.TObject_One.__init__(self, object.TObject_Type.init_unitDetect(team = team, minUnits = minUnits, maxUnits = maxUnits, 
                                                                               unitType = unitType, onlyList = onlyList), 
                                     object.TObject_Pos.init_rectangle(upos), 
-                                    name, object.TObject_Acti.init_acti(id = id, alsoacti = alsoacti), 
+                                    name, object.TObject_Acti.init_acti(id = id, alsoacti_s = alsoacti_s), 
                                     object.TObject_Time.init_time(warmup = warmup, reset = reset))
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_data/tobject/_unitRemove.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_unitRemove.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import rwmap._object as object
 import rwmap._frame as frame
 
 class UnitRemove(object.TObject_One):
     def __init__(self, pos:frame.Coordinate, size:frame.Coordinate, name:str = None, team:int = None, 
-               warmup:int = -1, reset:int = -1, actiBy:list[object.TObject_One] = [], 
-               deactiBy:list[object.TObject_One] = [], isalltoacti:bool = False):
+               warmup:int = -1, reset:int = -1, actiBy_s:list[object.TObject_One] = [], 
+               deactiBy_s:list[object.TObject_One] = [], isalltoacti:bool = False):
         upos = frame.Rectangle(pos - size / 2, size)
         object.TObject_One.__init__(self, object.TObject_Type.init_unitRemove(team), 
                                     object.TObject_Pos.init_rectangle(upos), 
-                                    name, object.TObject_Acti.init_acti(actiBy = actiBy, deactiBy = deactiBy, isalltoacti = isalltoacti), 
+                                    name, object.TObject_Acti.init_acti(actiBy_s = actiBy_s, deactiBy_s = deactiBy_s, isalltoacti = isalltoacti), 
                                     object.TObject_Time.init_time(warmup = warmup, reset = reset))
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_frame/_element_property.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_frame/_element_property.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 import xml.etree.ElementTree as et
+from copy import deepcopy
+from typing import Union
+
 import rwmap._util as utility
 
 class ElementProperties:
-    def __init__(self, tag:str, default_properties:dict[str, str] = {}, optional_properties:dict[str, str] = {})->None:
-        self.tag = tag
-        self._default_properties = default_properties
-        self._optional_properties = optional_properties
+    def __init__(self, tag:str, default_properties:dict[str, str] = {}, optional_properties:dict[str, Union[str, dict[str, str]]] = {})->None:
+        self._tag = tag
+        self._default_properties = deepcopy(default_properties)
+        self._optional_properties = deepcopy(optional_properties)
         
     @classmethod
     def init_etElement(cls, root:et.Element):
         if root == None:
             return None
-        optional_properties = utility.get_etElement_properties(utility.get_etElement_callable_from_tag(root, "properties"))
+        optional_properties = utility.get_etElement_properties(utility.get_etElement_callable_from_tag_s(root, "properties"))
         return cls(root.tag, root.attrib, optional_properties)
         
     def output_etElement(self, root:et.Element)->et.Element:
-        root.tag = self.tag
+        etElement_ans = deepcopy(root)
+        etElement_ans.tag = self._tag
         if self._default_properties != {}:
-            root.attrib = self._default_properties
+            etElement_ans.attrib = self._default_properties
         if self._optional_properties != {}:
-            root.append(utility.output_etElement_properties(self._optional_properties))
+            etElement_ans.append(utility.output_etElement_properties(self._optional_properties))
+        return etElement_ans
         
     def output_str(self)->str:
         str_ans = ""
-        str_ans = str_ans + self.tag + ":\n"
+        str_ans = str_ans + self._tag + ":\n"
         str_ans = str_ans + "default_properties:" + str(self._default_properties) + "\n"
         str_ans = str_ans + "optional_properties:" + str(self._optional_properties) + "\n"
         str_ans = utility.indentstr_Tab(str_ans)
         return str_ans
     
-    def assignDefaultProperty(self, name:str, value:str):
+    def assignDefaultProperty(self, name:str, value:Union[str, dict[str, str]]):
         self._default_properties[name] = value
     
-    def assignOptionalProperty(self, name:str, value:str):
+    def assignOptionalProperty(self, name:str, value:Union[str, dict[str, str]]):
         self._optional_properties[name] = value
 
-    def returnDefaultProperty(self, name:str):
+    def returnDefaultProperty(self, name:str)->Union[str, dict[str, str]]:
         return self._default_properties.get(name)
     
-    def returnOptionalProperty(self, name:str):
+    def returnOptionalProperty(self, name:str)->Union[str, dict[str, str]]:
         return self._optional_properties.get(name)
     
-    def deleteDefaultProperty(self, name:str):
-        del self._default_properties[name]
+    def deleteDefaultProperty(self, name:str)->None:
+        self._default_properties.pop(name)
     
-    def deleteOptionalProperty(self, name:str):
-        del self._optional_properties[name]
+    def deleteOptionalProperty(self, name:str)->None:
+        self._optional_properties.pop(name)
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_object/_object_global.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_global.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import rwmap._util as utility
+from copy import deepcopy
 
 class TObject_Global:
     def __init__(self, optional_properties:dict[str, str] = {}):
-        self._optional_properties = optional_properties
+        self._optional_properties = deepcopy(optional_properties)
 
     def output_optional_properties(self):
-        return self._optional_properties
+        return deepcopy(self._optional_properties)
     
     @classmethod
     def init_global(cls, message:str, delayPerChar:int = -1, textColor:str = None, issecond:bool = True):
         op_dict = {}
         op_dict.update({"globalMessage", message})
         op_dict.update(utility.add_time_pro("globalMessage_delayPerChar", delayPerChar, issecond))
         op_dict.update(utility.add_str_pro("globalMessage_textColor", textColor))
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_object/_object_group.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_group.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from rwmap._object._object_one_and_acti import TObject_One
 
 class TObject_Group:
     pass
 
 class TObject_Group:
     def __init__(self, TObject_One_list:list[TObject_One], TObject_Group_list:list[TObject_Group] = []):
-        self._TObject_One_list = TObject_One_list
-        for tobject_group in TObject_Group_list:
-            self._TObject_One_list = self._TObject_One_list + tobject_group._TObject_One_list
+        self._TObject_One_list = [deepcopy(TObject) for TObject in TObject_One_list]
+        self._TObject_Group_list = [deepcopy(TObject_Groupn) for TObject_Groupn in TObject_Group_list]
 
     def offset(self, offset:frame.Coordinate)->TObject_Group:
         ntob = deepcopy(self)
         for tob in ntob._TObject_One_list:
             tob._pos = tob.offset(offset)
+        for tobg in ntob._TObject_Group_list:
+            tobg.offset(offset)
         return ntob
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_object/_object_one_and_acti.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_one_and_acti.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,111 @@
 import xml.etree.ElementTree as et
 from typing import Union
+from copy import deepcopy
 
 import rwmap._frame as frame
 import rwmap._util as utility
 
 from rwmap._object._object_pos import TObject_Pos
 from rwmap._object._object_type import TObject_Type
 from rwmap._object._object_time import TObject_Time
 from rwmap._object._object_global import TObject_Global
 
-from copy import deepcopy
-
 class TObject_One:
     pass
 
 class TObject_Acti:
-    def __init__(self, idTObject_One:TObject_One = None, alsoacti:list[TObject_One] = [], 
-                 actiBy:list[TObject_One] = [], deactiBy:list[TObject_One] = [], 
+    def __init__(self, idTObject_One_s:TObject_One = None, alsoacti_s:list[TObject_One] = [], 
+                 actiBy_s:list[TObject_One] = [], deactiBy_s:list[TObject_One] = [], 
                  isalltoacti:bool = False):
-        self._idTObject_One = idTObject_One
-        self._alsoacti = alsoacti
-        self._actiBy = actiBy
-        self._deactiBy = deactiBy
+        self._idTObject_One_s = idTObject_One_s
+        self._alsoacti_s = alsoacti_s
+        self._actiBy_s = actiBy_s
+        self._deactiBy_s = deactiBy_s
         self._isalltoacti = isalltoacti
 
     @classmethod
-    def init_acti(cls, id:str = None, alsoacti:list[TObject_One] = [], 
-                 actiBy:list[TObject_One] = [], deactiBy:list[TObject_One] = [], 
+    def init_acti(cls, id:str = None, alsoacti_s:list[TObject_One] = [], 
+                 actiBy_s:list[TObject_One] = [], deactiBy_s:list[TObject_One] = [], 
                  isalltoacti:bool = False):
-        return cls(TObject_One(TObject_Type({}), name = id) if id != None else None, alsoacti, actiBy, deactiBy, isalltoacti)
+        return cls(TObject_One(TObject_Type({}), name = id) if id != None else None, alsoacti_s, actiBy_s, deactiBy_s, isalltoacti)
 
-    def add_alsoacti(self, add_TObject_One:list[TObject_One] = []):
-        self._alsoacti = self._alsoacti + add_TObject_One
+    def add_alsoacti_s(self, add_TObject_One_s:Union[list[TObject_One], TObject_One] = []):
+        add_TObject_One_s_list = utility.list_variable_s(add_TObject_One_s)
+        self._alsoacti_s = self._alsoacti_s + add_TObject_One_s_list
+
+    def add_actiBy_s(self, add_TObject_One_s:Union[list[TObject_One], TObject_One] = []):
+        add_TObject_One_s_list = utility.list_variable_s(add_TObject_One_s)
+        self._actiBy_s = self._actiBy_s + add_TObject_One_s_list
+
+    def add_deactiBy_s(self, add_TObject_One_s:Union[list[TObject_One], TObject_One] = []):
+        add_TObject_One_s_list = utility.list_variable_s(add_TObject_One_s)
+        self._deactiBy_s = self._deactiBy_s + add_TObject_One_s_list
+
+    def add_twoactiBy_s(self, add_TObject_One_two_s:tuple[list[TObject_One], 
+                                                          list[TObject_One]] = ([], [])):
+        self.add_actiBy_s(add_TObject_One_two_s[0])
+        self.add_deactiBy_s(add_TObject_One_two_s[1])
 
-    def add_actiBy(self, add_TObject_One:list[TObject_One] = []):
-        self._actiBy = self._actiBy + add_TObject_One
-
-    def add_deactiBy(self, add_TObject_One:list[TObject_One] = []):
-        self._deactiBy = self._deactiBy + add_TObject_One
-
-    def return_idTObject(self)->Union[TObject_One, None]:
-        return self._idTObject_One
+    def idTObject_s(self)->Union[TObject_One, None]:
+        return self._idTObject_One_s
 
     def output_optional_properties(self)->dict[str, str]:
         op_dict = {}
-        if self._idTObject_One != None:
-            op_dict.update({"id": self._idTObject_One._name}) 
+        if self._idTObject_One_s != None:
+            op_dict.update({"id": self._idTObject_One_s._name}) 
         if self._isalltoacti:
             op_dict.update({"allToActivate": "1"}) 
-        op_dict.update(utility.add_acti_pro("alsoActivate", self._alsoacti))
-        op_dict.update(utility.add_acti_pro("activatedBy", self._actiBy))
-        op_dict.update(utility.add_acti_pro("deactivatedBy", self._deactiBy))
+        op_dict.update(utility.add_acti_pro("alsoactivate", self._alsoacti_s))
+        op_dict.update(utility.add_acti_pro("activatedBy", self._actiBy_s))
+        op_dict.update(utility.add_acti_pro("deactivatedBy", self._deactiBy_s))
         return op_dict
 
 class TObject_One:
     def __init__(self, otype:TObject_Type, pos:TObject_Pos = TObject_Pos({}), name:str = None, 
                  acti:TObject_Acti = TObject_Acti(), time:TObject_Time = TObject_Time(),
                  nglobal:TObject_Global = TObject_Global()):
-        self._name = name
-        self._pos = pos
-        self._otype = otype
-        self._acti = acti
-        self._time = time
-        self._global = nglobal
+        self._name = deepcopy(name)
+        self._pos = deepcopy(pos)
+        self._otype = deepcopy(otype)
+        self._acti = deepcopy(acti)
+        self._time = deepcopy(time)
+        self._global = deepcopy(nglobal)
 
     def default_properties(self)->dict[str, str]:
         dict_ans = {}
         if self._name != None:
             dict_ans = dict_ans.update({"name": self._name})
         dict_ans = {**self._pos.output_default_properties(), **self._otype.output_default_properties()}
         return dict_ans
     
     def offset(self, offset:frame.Coordinate)->TObject_One:
         ntob = deepcopy(self)
         ntob._pos = ntob._pos.offset(offset)
         return ntob
 
-    def optional_properties(self)->dict[str, str]:
+    def optional_properties(self)->dict[str, Union[str, dict[str, str]]]:
         return {**self._otype.output_optional_properties(), 
                 **self._acti.output_optional_properties(),
                 **self._time.output_optional_properties(), 
                 **self._global.output_optional_properties()}
     
     def other_properties(self)->list[et.Element]:
         return self._pos.output_other_properties()
     
-    def return_idTObject(self)->Union[TObject_One, None]:
-        return self._acti.return_idTObject()
+    def idTObject_s(self)->Union[TObject_One, None]:
+        return self._acti.idTObject_s()
     
-    def add_alsoacti(self, add_TObject_One:list[TObject_One] = []):
-        self._acti.add_alsoacti(add_TObject_One)
+    def add_alsoacti_s(self, add_TObject_One_s:list[TObject_One] = []):
+        self._acti.add_alsoacti_s(add_TObject_One_s)
+
+    def add_actiBy_s(self, add_TObject_One_s:list[TObject_One] = []):
+        self._acti.add_actiBy_s(add_TObject_One_s)
 
-    def add_actiBy(self, add_TObject_One:list[TObject_One] = []):
-        self._acti.add_actiBy(add_TObject_One)
+    def add_deactiBy_s(self, add_TObject_One_s:list[TObject_One] = []):
+        self._acti.add_deactiBy_s(add_TObject_One_s)
 
-    def add_deactiBy(self, add_TObject_One:list[TObject_One] = []):
-        self._acti.add_deactiBy(add_TObject_One)
+    def add_twoactiBy_s(self, add_TObject_One_two_s:tuple[list[TObject_One], 
+                                                          list[TObject_One]] = ([], [])):
+        self._acti.add_twoactiBy_s(add_TObject_One_two_s)
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_object/_object_time.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_time.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from copy import deepcopy
+
 import rwmap._util as utility
 
 class TObject_Time:
     def __init__(self, optional_properties:dict[str, str] = {}):
-        self._optional_properties = optional_properties
+        self._optional_properties = deepcopy(optional_properties)
 
     def output_optional_properties(self):
-        return self._optional_properties
+        return deepcopy(self._optional_properties)
     
     @classmethod
     def init_time(cls, warmup:int = -1, delay:int = -1, reset:int = -1, repeat:int = -1, issecond:bool = True):
         op_dict = {}
         op_dict.update(utility.add_time_pro("warmup", warmup))
         op_dict.update(utility.add_time_pro("delay", delay))
         op_dict.update(utility.add_time_pro("resetActivationAfter", reset))
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_object/_object_type.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import xml.etree.ElementTree as et
-import re
+from copy import deepcopy
+from typing import Union
 
 import rwmap._frame as frame
 import rwmap._util as utility
 
 class TObject_Type:
-    def __init__(self, default_properties:dict[str, str], optional_properties:dict[str, str] = {}):
-        self._default_properties = default_properties
-        self._optional_properties = optional_properties
+    def __init__(self, default_properties:dict[str, str], optional_properties:dict[str, Union[str, dict[str, str]]] = {}):
+        self._default_properties = deepcopy(default_properties)
+        self._optional_properties = deepcopy(optional_properties)
 
     def output_default_properties(self):
-        return self._default_properties
+        return deepcopy(self._default_properties)
     
     def output_optional_properties(self):
-        return self._optional_properties
+        return deepcopy(self._optional_properties)
     
     def _add_optional(self, name:str, value:str):
         self._optional_properties.update(utility.add_str_pro(name, value))
 
     @classmethod
     def init_node(cls):
         return cls({"type": "unitAdd"}, {})
@@ -34,15 +35,16 @@
         otype._add_optional("team", team)
         otype._add_optional("unitType", unitType)
         otype._add_optional("minUnits", minUnits)
         otype._add_optional("maxUnits", maxUnits)
         for only in onlyList:
             if only[0:13] == "onlyTechLevel":
                 otype._add_optional(only[0:13], only[13])
-            otype._add_optional(only, "1")
+            else:
+                otype._optional_properties.update({only:{"type": "bool", "value": "true"}})
         return otype
 
     @classmethod
     def init_unitRemove(cls, team:int = None):
         otype = cls({"type": "unitRemove"}, {})
         otype._add_optional("team", team)
         return otype
@@ -52,18 +54,19 @@
         otype = cls({"type": "mapText"}, {})
         otype._add_optional("text", text)
         otype._add_optional("textColor", textColor)
         otype._optional_properties.update(utility.add_time_pro("textSize", textSize, False))
         return otype
 
     @classmethod
-    def init_changeCredits(cls, setCredits:int = None, addCredits:int = None):
+    def init_changeCredits(cls, team:int, setCredits:int = None, addCredits:int = None):
         otype = cls({"type": "changeCredits"}, {})
-        otype._add_optional("set", str(setCredits))
-        otype._add_optional("add", str(addCredits))
+        otype._add_optional("set", setCredits)
+        otype._add_optional("add", addCredits)
+        otype._add_optional("team", team)
         return otype
 
     @classmethod
     def init_mapinfo(cls, mapType:str, mapFog:str, winCondition:str, text:str = None):
         otype = cls({"name": "map_info"}, {})
         otype._add_optional("type", mapType)
         otype._add_optional("fog", mapFog)
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_tile/_tile_group.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_tile/_tile_group.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import numpy as np
+from copy import deepcopy
+from typing import Union
 
 import rwmap._frame as frame
 import rwmap._util as utility
 from rwmap._exceptions import KeyConflictError
+from rwmap._data.const import TYPE
 
 tilestate_type = "S20"
 
 class TileGroup_Matrix:
     def __init__(self, tilename_matrix):
-        self._tilematrix = np.array(tilename_matrix, tilestate_type)
+        self._tilematrix = deepcopy(np.array(tilename_matrix, tilestate_type))
         self._size = frame.Coordinate(self._tilematrix.shape[0], self._tilematrix.shape[1])
 
     def tilematrix(self):
         return self._tilematrix
 
     def size(self)->frame.Coordinate:
         return self._size
     
     def __getitem__(self, place:frame.Coordinate)->str:
-        return self._tilematrix[place.x()][place.y()]
+        return deepcopy(self._tilematrix[place.x()][place.y()])
     
 class TileGroup_AddLayer(TileGroup_Matrix):
     def __init__(self, layername:str, tilename_matrix):
         TileGroup_Matrix.__init__(self, tilename_matrix)
         TileGroup_AddLayer._add_layername(self, layername)
 
     def _add_layername(self, layername:str)->None:
@@ -34,86 +37,89 @@
     
     @classmethod
     def init_tilegroup(cls, tilegroup):
         return cls(tilegroup.layername(), tilegroup.tilematrix())
 
     def layername(self)->str:
         return self._layername
-    
+
+
+
 class TileGroup_AddFile(TileGroup_Matrix):
-    def __init__(self, tilename_to_tileset:dict[str, frame.TagCoordinate], tilename_matrix):
+    def __init__(self, tilename_to_tileset:dict[str, TYPE.tileid], tilename_matrix):
         TileGroup_Matrix.__init__(self, tilename_matrix)
         TileGroup_AddFile._add_tilename(self, tilename_to_tileset)
 
-    def _add_tilename(self, tilename_to_tileset:dict[str, frame.TagCoordinate])->None:
+    def _add_tilename(self, tilename_to_tileset:dict[str, TYPE.tileid])->None:
+        tilename_to_tileset_n = deepcopy(tilename_to_tileset)
         zeroadd = {"0": frame.TagCoordinate.init_xy("empty", 0, 0)}
         if utility.dict_isconflict(tilename_to_tileset, zeroadd):
             raise KeyConflictError("Key-value of the tile group conflicts at instantiation. \
                                    0 is the default empty tile.")
-        tilename_to_tileset.update(zeroadd)
-        self._tilename_to_tileset = tilename_to_tileset
+        tilename_to_tileset_n.update(zeroadd)
+        self._tilename_to_tileset = tilename_to_tileset_n
 
     @classmethod
     def init_tilegroup_matrix(cls, tilename_to_tileset:str, tilegroup_matrix:TileGroup_Matrix):
         return cls(tilename_to_tileset, tilegroup_matrix._tilematrix)
 
-    def __getitem__(self, place: frame.Coordinate) -> frame.TagCoordinate:
+    def __getitem__(self, place: frame.Coordinate) -> TYPE.tileid:
         stritems = bytes(TileGroup_Matrix.__getitem__(self, place)).decode("utf-8")
-        return self._tilename_to_tileset[stritems]
+        return deepcopy(self._tilename_to_tileset[stritems])
     
-    def tilename_to_tileset(self)->dict[str, frame.TagCoordinate]:
-        return self._tilename_to_tileset
+    def tilename_to_tileset(self)->dict[str, TYPE.tileid]:
+        return deepcopy(self._tilename_to_tileset)
     
 class TileGroup_One(TileGroup_AddFile, TileGroup_AddLayer):
-    def __init__(self, layername:str, tilename_to_tileset:dict[str, frame.TagCoordinate], tilename_matrix)->None:
+    def __init__(self, layername:str, tilename_to_tileset:dict[str, TYPE.tileid], tilename_matrix)->None:
         TileGroup_Matrix.__init__(self, tilename_matrix)
         self._add_layername(layername)
         self._add_tilename(tilename_to_tileset)
     
     @classmethod
-    def init_tilegroup_matrix(cls, layername:str, tilename_to_tileset:dict[str, frame.TagCoordinate], tilegroup_matrix:TileGroup_Matrix):
+    def init_tilegroup_matrix(cls, layername:str, tilename_to_tileset:dict[str, TYPE.tileid], tilegroup_matrix:TileGroup_Matrix):
         return cls(layername, tilename_to_tileset, tilegroup_matrix._tilematrix)
     
     @classmethod
     def init_tilegroup_addfile(cls, layername:str, tilegroup_addfile:TileGroup_AddFile):
         return cls(layername, tilegroup_addfile._tilename_to_tileset, tilegroup_addfile._tilematrix)
 
     @classmethod
-    def init_tilegroup_addlayer(cls, tilename_to_tileset:dict[str, frame.TagCoordinate], tilegroup_addlayer:TileGroup_AddLayer):
+    def init_tilegroup_addlayer(cls, tilename_to_tileset:dict[str, TYPE.tileid], tilegroup_addlayer:TileGroup_AddLayer):
         return cls(tilegroup_addlayer._layername, tilename_to_tileset, tilegroup_addlayer._tilematrix)
 
 class TileGroup_List_SubTileName:
     def __init__(self, tilegrouplist_addlayer:list[TileGroup_AddLayer]):
-        self._tilegrouplist_addlayer = tilegrouplist_addlayer
+        self._tilegrouplist_addlayer = deepcopy(tilegrouplist_addlayer)
 
     def tilegrouplist(self):
-        return self._tilegrouplist_addlayer
+        return deepcopy(self._tilegrouplist_addlayer)
 
 class TileGroup_List(TileGroup_List_SubTileName):
-    def __init__(self, tilename_to_tileset:dict[str, frame.TagCoordinate], tilegrouplist_addlayer:list[TileGroup_AddLayer]):
+    def __init__(self, tilename_to_tileset:dict[str, TYPE.tileid], tilegrouplist_addlayer:list[TileGroup_AddLayer]):
         super().__init__(self, tilegrouplist_addlayer)
         self._add_tilename(tilename_to_tileset)
 
-    def _add_tilename(self, tilename_to_tileset:dict[str, frame.TagCoordinate])->None:
-        self._tilename_to_tileset = tilename_to_tileset
+    def _add_tilename(self, tilename_to_tileset:dict[str, TYPE.tileid])->None:
+        self._tilename_to_tileset = deepcopy(tilename_to_tileset)
 
     @classmethod
-    def init_tilegroup_list_subtilename(cls, tilename_to_tileset:dict[str, frame.TagCoordinate], tilegrouplist_subtilename:TileGroup_List_SubTileName):
+    def init_tilegroup_list_subtilename(cls, tilename_to_tileset:dict[str, TYPE.tileid], tilegrouplist_subtilename:TileGroup_List_SubTileName):
         return cls(tilename_to_tileset, tilegrouplist_subtilename.tilegrouplist())
 
     @classmethod
     def init_tilegroup_list(cls, tilegrouplist:list[TileGroup_One]):
         tilegrouplist_addlayer = []
         tilename_to_tileset = {}
         for tilegroup in tilegrouplist:
             if utility.dict_isconflict(tilename_to_tileset, tilegroup.tilename_to_tileset()):
                 raise KeyConflictError("Key-value of the tile group conflicts at instantiation.")
             tilename_to_tileset.update(tilegroup.tilename_to_tileset())
             tilegrouplist_addlayer.append(TileGroup_AddLayer.init_tilegroup(tilegroup))
         return cls(tilename_to_tileset, tilegrouplist_addlayer)
 
-    def __next__(self):
+    def _iterator(self):
         for tilegroup in self._tilegrouplist_addlayer:
             yield TileGroup_One.init_tilegroup_addlayer(self._tilename_to_tileset, tilegroup)
 
     def __iter__(self):
-        return self
+        return self._iterator()
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_util/__init__.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_util/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding=utf8 -*-
 from rwmap._util._etElement_process import get_etElement_properties
-from rwmap._util._etElement_process import get_etElement_name_to_text_rm
-from rwmap._util._etElement_process import get_etElement_callable_from_tag
+from rwmap._util._etElement_process import get_etElement_name_to_text_s
+from rwmap._util._etElement_process import get_etElement_callable_from_tag_s
 from rwmap._util._etElement_process import get_etElement_ndarray_from_text_packed
 from rwmap._util._etElement_process import get_etElement_from_text_packed
 from rwmap._util._etElement_process import output_file_from_etElement
 from rwmap._util._etElement_process import output_etElement_properties
 
 from rwmap._util._str_util import indentstr_Tab
 from rwmap._util._str_util import str_slash_to_dot
 
-from rwmap._util._dict_util import dict_isconflict
+from rwmap._util._dict_util import dict_isconflict, udictstr_to_dict
 
-from rwmap._util._class_rel import get_ElementOri_from_list_by_name
+from rwmap._util._class_rel import get_ElementOri_from_list_by_name_s
 
 from rwmap._util._png_rel import image_width, image_height
 
-from rwmap._util._list_util import fill_list_of_list
+from rwmap._util._list_util import fill_list_of_list, list_variable_s, list_get_s, team_list_inv, search_list_to_index
 
 from rwmap._util._add_dict import add_str_pro, add_time_pro, add_acti_pro
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_util/_add_dict.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_add_dict.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,13 +18,14 @@
     
 def add_acti_pro(name:str, tob_list:list[TObject_One])->dict[str, str]:
     value_list = []
     if tob_list != []:
         for tobject in tob_list:
             value_list.append(tobject._name)
             if tobject._name == None:
-                raise rwexception.ObjectNameError
+                raise rwexception.ObjectNameError\
             ("The object does not have a name but participates in activation or deactivation.")
+        value_list = list(set(value_list))
         value = ",".join(value_list)
         return {name: value}
     else:
         return {}
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_util/_etElement_process.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_etElement_process.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,83 @@
 import xml.etree.ElementTree as et
 import numpy as np
+from typing import Union
+from copy import deepcopy
 
 from xml.dom import minidom
 
+
 import rwmap._frame as frame
 import rwmap._util._str_util as str_utility
+import rwmap._util._dict_util as dict_utility
 
-def get_etElement_properties(root:et.Element)->dict[str,str]:
-    if root == None:
+def get_etElement_properties(root:et.Element)->dict[str,Union[str, dict[str, str]]]:
+    rootn = deepcopy(root)
+    if rootn == None:
         return None
     dict_properties = {}
-    for nproperty in root:
+    for nproperty in rootn:
         if nproperty.attrib.get('value') == None:
             nproperty.attrib['value'] = ""
-        dict_properties[nproperty.attrib['name']] = nproperty.attrib['value']
+        if len(nproperty.attrib) == 2:
+            dict_properties[nproperty.attrib['name']] = nproperty.attrib['value']
+        else:
+            nproperty.attrib.pop('name')
+            dict_properties[nproperty.attrib['name']] = nproperty.attrib
     return dict_properties
 
-def output_etElement_properties(dict_properties:dict[str, str])->et.Element:
+def output_etElement_properties(dict_properties:dict[str, Union[dict[str, str], str]])->et.Element:
     root = et.Element("properties")
     if dict_properties != None:
         for name, value in dict_properties.items():
-            root.append(et.Element("property", attrib = {"name":name, "value":value}))
+            dict_n = {"name":name}
+            dict_n.update(dict_utility.udictstr_to_dict(value))
+            nproperty = et.Element("property", dict_n)
+            root.append(nproperty)
     return root
 
-def get_etElement_name_to_text_rm(root:et.Element, name:str)->str:
+def get_etElement_name_to_text_s(root:et.Element, name:str)->Union[str, None]:
     if root == None:
         return None
     for nproperty in root:
         if nproperty.attrib['name'] == name:
             text = nproperty.text
-            root.remove(nproperty)
             return text
 
 def get_etElement_ndarray_from_text_packed(root:et.Element, reshape_Coordinate:frame.Coordinate)->np.ndarray:
     if root == None:
         return None
     nmatrix = str_utility.ndarray_from_text_packed(root.text, root.attrib["encoding"], root.attrib["compression"])
     nmatrix = np.reshape(nmatrix, [reshape_Coordinate.y(), reshape_Coordinate.x()])
     return nmatrix
 
 def get_etElement_from_text_packed(tilematrix:np.ndarray, encoding:str, compression:str)->et.Element:
     root = et.Element("data", {"encoding": encoding, "compression": compression})
     root.text = str_utility.text_packed_from_ndarray(tilematrix, encoding, compression)
     return root
 
-def get_etElement_callable_from_tagone(root:et.Element, tag:str)->et.Element:
+def get_etElement_callable_from_tagone_s(root:et.Element, tag:str)->et.Element:
     if root == None:
         return None
     for etchild in root:
         if etchild.tag == tag:
             return etchild
         
-def get_etElement_callable_from_taglist(root:et.Element, tag_list:list[str])->et.Element:
+def get_etElement_callable_from_taglist_s(root:et.Element, tag_list:list[str])->et.Element:
     if root == None:
         return None
     for tagnow in tag_list:
-        root = get_etElement_callable_from_tagone(root, tagnow)
+        root = get_etElement_callable_from_tagone_s(root, tagnow)
     return root
 
-def get_etElement_callable_from_tag(root:et.Element, tag:str)->et.Element:
+def get_etElement_callable_from_tag_s(root:et.Element, tag:str)->et.Element:
     if root == None:
         return None
     tag_list = tag.split(",")
-    return get_etElement_callable_from_taglist(root, tag_list)
+    return get_etElement_callable_from_taglist_s(root, tag_list)
 
 def output_file_from_etElement(root:et.Element, file:str)->None:
     dom = minidom.parseString(et.tostring(root, encoding='utf-8'))
     pretty_xml = dom.toprettyxml(indent='  ')
     with open(file, 'w', encoding='utf-8') as file_now:
         file_now.write(pretty_xml)
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/_util/_str_util.py` & `rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_str_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,30 @@
         nmatrix = base64.b64decode(text)
     else:
         raise NotImplementedError(f": encoding type {encoding} not supported")
     if compression == "zlib":
         nmatrix = zlib.decompress(nmatrix)
     elif compression == "gzip":
         nmatrix = gzip.decompress(nmatrix)
+    elif compression == None:
+        pass
     else:
         raise NotImplementedError(f": Compression type {compression} not supported")
     nmatrix = np.frombuffer(nmatrix, dtype=np.uint32)
     nmatrix = np.copy(nmatrix)
     return nmatrix
 
 def text_packed_from_ndarray(ndarray_now:np.ndarray, encoding:str, compression:str):
     text_packed = ndarray_now.flatten().tobytes()
     if compression == "zlib":
         text_packed = zlib.compress(text_packed)
     elif compression == "gzip":
         text_packed = gzip.compress(text_packed)
+    elif compression == None:
+        pass
     else:
         raise NotImplementedError(f": Compression type {compression} not supported")
     if encoding == "base64":
         text_packed = base64.b64encode(text_packed).decode(encoding="utf-8")
     else:
         raise NotImplementedError(f": encoding type {encoding} not supported")
     return text_packed
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/bridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/bridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/decoration.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/decoration.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/deepwater.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/deepwater.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dirt_details.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt_details.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/dust.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dust.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/fauna.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/fauna.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/fauna_dark.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/fauna_dark.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/fauna_highland.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/fauna_highland.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2ice_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/lava.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/lava2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/lava2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/misc.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/misc.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/nothing2road_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/nothing2road_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2_old.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2_old.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2ice_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2lava_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2sand_hill.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2sand_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2stone_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sand_dark.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand_dark.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/shallowwater.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/shortgrass.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shortgrass.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2snow_hill.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2snow_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2lava.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2lava.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2snow.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2snow.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/units.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/units.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/water.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/water.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/misc.tsx` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/misc.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/terrain/Lava.tsx` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Lava.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmap/other_data/maps/units.tsx` & `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/units.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmapeditor_exgcdwu.egg-info/PKG-INFO` & `rwmapeditor_exgcdwu-1.4.0/rwmapeditor_exgcdwu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.3.2
+Version: 1.4.0
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -688,14 +688,16 @@
 
 ___一个铁锈战争 (Rusted Warfare) 地图编辑 python 库___
 
 ![released version](https://img.shields.io/pypi/v/rwmapeditor-exgcdwu.svg)
 
 [简易使用教程](https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-/blob/main/Tutorial.md)
 
+[简单城夺地图代码例子](https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-/blob/main/examples/example1/example1.py)
+
 ## 目标
 
 python实现铁锈地图文件地块编辑和宾语编辑。
 
 暂时不打算接触地块集。
 
 重点减轻城市争夺地图的宾语编辑工作量
@@ -712,15 +714,15 @@
 pip install rwmapeditor-exgcdwu
 ```
 
 ## 使用之前
 
 ### 1.使用地图编辑器(Tiled,notTiled)创建新地图
 
-地图格式：zlib、gzip
+地图格式：zlib、gzip、纯base64
 
 渲染顺序：右下(right-down)
 
 方向：orthogonal
 
 #### 2.手动载入地块集
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/rwmapeditor_exgcdwu.egg-info/SOURCES.txt` & `rwmapeditor_exgcdwu-1.4.0/rwmapeditor_exgcdwu.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,21 +20,27 @@
 rwmap/_data/tobject/__init__.py
 rwmap/_data/tobject/_camera.py
 rwmap/_data/tobject/_credit.py
 rwmap/_data/tobject/_mapText.py
 rwmap/_data/tobject/_mapinfo.py
 rwmap/_data/tobject/_message.py
 rwmap/_data/tobject/_node.py
-rwmap/_data/tobject/_tobject_one.py
 rwmap/_data/tobject/_unitAdd.py
 rwmap/_data/tobject/_unitDetect.py
 rwmap/_data/tobject/_unitRemove.py
 rwmap/_data/tobject_group/__init__.py
-rwmap/_data/tobject_group/_city.py
-rwmap/_data/tobject_group/_refresh_building.py
+rwmap/_data/tobject_group/_city/__init__.py
+rwmap/_data/tobject_group/_city/_city.py
+rwmap/_data/tobject_group/_city/_city_detect.py
+rwmap/_data/tobject_group/_city/_city_remove.py
+rwmap/_data/tobject_group/_city/_city_text.py
+rwmap/_data/tobject_group/_city/_normal_unit_add.py
+rwmap/_data/tobject_group/_city/_refresh_building.py
+rwmap/_data/tobject_group/_troop/__init__.py
+rwmap/_data/tobject_group/_troop/_troop_add.py
 rwmap/_frame/__init__.py
 rwmap/_frame/_coordinate.py
 rwmap/_frame/_element_ori.py
 rwmap/_frame/_element_property.py
 rwmap/_object/__init__.py
 rwmap/_object/_object_global.py
 rwmap/_object/_object_group.py
```

### Comparing `rwmapeditor_exgcdwu-1.3.2/setup.py` & `rwmapeditor_exgcdwu-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 
 import os
 from setuptools import setup, find_packages
 
-__version__ = '1.3.2'
+__version__ = '1.4.0'
 
 def read_file(file:str):
     with open(file) as file:
         return file.read()
 
 def readline_file(file:str):
     with open(file) as file:
@@ -20,13 +20,13 @@
     version = __version__,
     author = 'exgcdwu',
     author_email = '1006605318@qq.com',
     license = read_file('LICENSE'),
     url = "https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-",
     long_description = read_file('README.md'),
     long_description_content_type = "text/markdown",
-    packages = find_packages(exclude=["tests"]),
+    packages = find_packages(exclude=["tests", "examples"]),
     package_data={'rwmap': ['other_data/*.txt', DATA_PREFIX_MAPS + '*.tsx', DATA_PREFIX_MAPS + 'bitmaps/*.png',
                              DATA_PREFIX_MAPS + 'ridges/*.tsx', DATA_PREFIX_MAPS + 'terrain/*.tsx']},
     python_requires = '>=3.6.0',
     install_requires = readline_file("./rwmap/other_data/requirements.txt")
 )
```

