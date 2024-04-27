# Comparing `tmp/libolecf-python-20240212.tar.gz` & `tmp/libolecf-python-20240427.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libolecf-python-20240212.tar", last modified: Mon Feb 12 05:00:56 2024, max compression
+gzip compressed data, was "libolecf-python-20240427.tar", last modified: Sat Apr 27 09:02:46 2024, max compression
```

## Comparing `libolecf-python-20240212.tar` & `libolecf-python-20240427.tar`

### file list

```diff
@@ -1,878 +1,882 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3540 2024-02-12 04:38:42.000000 libolecf-20240212/libolecf.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:54.000000 libolecf-20240212/libfole/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-02-12 04:47:11.000000 libolecf-20240212/libfole/libfole_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-12 04:47:11.000000 libolecf-20240212/libfole/libfole_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      665 2024-02-12 04:47:11.000000 libolecf-20240212/libfole/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1555 2024-02-12 04:47:11.000000 libolecf-20240212/libfole/libfole_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-12 04:47:11.000000 libolecf-20240212/libfole/libfole_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-02-12 04:47:11.000000 libolecf-20240212/libfole/libfole_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1407 2024-02-12 04:47:11.000000 libolecf-20240212/libfole/libfole_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-02-12 04:47:11.000000 libolecf-20240212/libfole/libfole_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3793 2024-02-12 04:47:11.000000 libolecf-20240212/libfole/libfole_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-12 04:47:11.000000 libolecf-20240212/libfole/libfole_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-12 04:47:11.000000 libolecf-20240212/libfole/libfole_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29307 2024-02-12 04:47:25.000000 libolecf-20240212/libfole/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-12 04:47:11.000000 libolecf-20240212/libfole/libfole_extern.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/libolecf/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2593 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/olecf_property_set.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23541 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_property_section.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2751 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_directory_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3367 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_property_section.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2612 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_directory_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3877 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2038 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4933 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_ole.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1924 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    46491 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16011 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_file_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18982 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_property_set.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/olecf_directory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4557 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2718 2023-12-03 09:12:34.000000 libolecf-20240212/libolecf/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2926 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_property_set_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1276 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_libfole.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2100 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42634 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9462 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2024-02-12 04:47:34.000000 libolecf-20240212/libolecf/libolecf.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33123 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    59693 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_property_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1517 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_libfwps.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26754 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_directory_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8242 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_allocation_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1404 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_directory_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2655 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5790 2024-02-12 04:47:34.000000 libolecf-20240212/libolecf/libolecf_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5792 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3395 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_directory_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1364 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_property_set_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3640 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/olecf_file_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/olecf_compound_object.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7088 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_property_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8893 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26095 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_compound_object_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1826 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1858 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2025 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_allocation_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2761 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_file_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37110 2024-02-12 04:47:25.000000 libolecf-20240212/libolecf/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1356 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_compound_object_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5369 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14768 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_directory_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2950 2024-02-12 04:38:43.000000 libolecf-20240212/libolecf/libolecf_property_set.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-02-12 04:38:42.000000 libolecf-20240212/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-02-12 04:47:25.000000 libolecf-20240212/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 04:38:42.000000 libolecf-20240212/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-02-12 04:47:25.000000 libolecf-20240212/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:54.000000 libolecf-20240212/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-12 04:47:10.000000 libolecf-20240212/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-02-12 04:47:10.000000 libolecf-20240212/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-02-12 04:47:10.000000 libolecf-20240212/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-12 04:47:10.000000 libolecf-20240212/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      681 2024-02-12 04:47:10.000000 libolecf-20240212/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-12 04:47:10.000000 libolecf-20240212/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-12 04:47:10.000000 libolecf-20240212/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-02-12 04:47:10.000000 libolecf-20240212/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-02-12 04:47:10.000000 libolecf-20240212/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-02-12 04:47:10.000000 libolecf-20240212/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-02-12 04:47:10.000000 libolecf-20240212/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29384 2024-02-12 04:47:25.000000 libolecf-20240212/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-12 04:47:10.000000 libolecf-20240212/libfguid/libfguid_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:53.000000 libolecf-20240212/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:12:36.000000 libolecf-20240212/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2023-12-03 09:12:36.000000 libolecf-20240212/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:12:35.000000 libolecf-20240212/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:12:36.000000 libolecf-20240212/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:12:35.000000 libolecf-20240212/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:12:35.000000 libolecf-20240212/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:12:35.000000 libolecf-20240212/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:12:35.000000 libolecf-20240212/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:12:35.000000 libolecf-20240212/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3956 2023-12-03 09:12:36.000000 libolecf-20240212/m4/libfole.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:12:36.000000 libolecf-20240212/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:12:35.000000 libolecf-20240212/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:12:35.000000 libolecf-20240212/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:12:36.000000 libolecf-20240212/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:12:36.000000 libolecf-20240212/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-02-12 04:47:20.000000 libolecf-20240212/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-02-12 04:47:20.000000 libolecf-20240212/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:12:36.000000 libolecf-20240212/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8519 2023-12-03 09:12:35.000000 libolecf-20240212/m4/libfwps.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5232 2023-12-03 09:12:36.000000 libolecf-20240212/m4/libfuse.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-02-12 04:47:20.000000 libolecf-20240212/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:12:35.000000 libolecf-20240212/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:12:35.000000 libolecf-20240212/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:12:36.000000 libolecf-20240212/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2023-12-03 09:12:36.000000 libolecf-20240212/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:12:35.000000 libolecf-20240212/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:12:35.000000 libolecf-20240212/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-02-12 04:47:20.000000 libolecf-20240212/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:12:35.000000 libolecf-20240212/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:12:35.000000 libolecf-20240212/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-02-12 04:47:20.000000 libolecf-20240212/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:12:35.000000 libolecf-20240212/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:12:36.000000 libolecf-20240212/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19791 2023-12-03 09:12:35.000000 libolecf-20240212/m4/libfvalue.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:12:36.000000 libolecf-20240212/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:12:36.000000 libolecf-20240212/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:53.000000 libolecf-20240212/include/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:53.000000 libolecf-20240212/include/libolecf/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4916 2024-02-12 04:38:43.000000 libolecf-20240212/include/libolecf/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4914 2024-02-12 04:47:34.000000 libolecf-20240212/include/libolecf/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5108 2024-02-12 04:38:43.000000 libolecf-20240212/include/libolecf/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4977 2024-02-12 04:47:34.000000 libolecf-20240212/include/libolecf/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-12 04:38:43.000000 libolecf-20240212/include/libolecf/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-02-12 04:38:43.000000 libolecf-20240212/include/libolecf/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-12 04:38:43.000000 libolecf-20240212/include/libolecf/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2024-02-12 04:47:34.000000 libolecf-20240212/include/libolecf/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4600 2024-02-12 04:38:43.000000 libolecf-20240212/include/libolecf/ole.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-02-12 04:38:43.000000 libolecf-20240212/include/libolecf/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28257 2024-02-12 04:47:34.000000 libolecf-20240212/include/libolecf.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      492 2024-02-12 04:38:42.000000 libolecf-20240212/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28257 2024-02-12 04:38:43.000000 libolecf-20240212/include/libolecf.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27948 2024-02-12 04:47:25.000000 libolecf-20240212/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:54.000000 libolecf-20240212/libfwps/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2490 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_set.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2104 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_store.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3827 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3731 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_format_class_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9704 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_store.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2244 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_property_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_format_class_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7534 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_property_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5115 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    60049 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16442 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_set.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31371 2024-02-12 04:47:25.000000 libolecf-20240212/libfwps/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-12 04:47:13.000000 libolecf-20240212/libfwps/libfwps_unused.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:53.000000 libolecf-20240212/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-02-12 04:38:43.000000 libolecf-20240212/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-02-12 04:38:43.000000 libolecf-20240212/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-02-12 04:38:43.000000 libolecf-20240212/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-02-12 04:38:43.000000 libolecf-20240212/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-12 04:38:43.000000 libolecf-20240212/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-02-12 04:38:43.000000 libolecf-20240212/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-02-12 04:38:43.000000 libolecf-20240212/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-02-12 04:38:42.000000 libolecf-20240212/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-02-12 04:38:43.000000 libolecf-20240212/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-02-12 04:47:34.000000 libolecf-20240212/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16614 2024-02-12 04:47:24.000000 libolecf-20240212/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17599 2024-02-12 04:47:34.000000 libolecf-20240212/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-02-12 04:38:43.000000 libolecf-20240212/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-02-12 04:38:43.000000 libolecf-20240212/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-02-12 04:38:43.000000 libolecf-20240212/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24937 2024-02-12 04:47:25.000000 libolecf-20240212/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:54.000000 libolecf-20240212/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-02-12 04:47:03.000000 libolecf-20240212/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-02-12 04:47:03.000000 libolecf-20240212/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-02-12 04:47:03.000000 libolecf-20240212/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-02-12 04:47:03.000000 libolecf-20240212/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-12 04:47:03.000000 libolecf-20240212/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-12 04:47:03.000000 libolecf-20240212/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-02-12 04:47:03.000000 libolecf-20240212/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-02-12 04:47:03.000000 libolecf-20240212/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-02-12 04:47:03.000000 libolecf-20240212/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-02-12 04:47:03.000000 libolecf-20240212/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29940 2024-02-12 04:47:25.000000 libolecf-20240212/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-12 04:47:03.000000 libolecf-20240212/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-02-12 04:47:03.000000 libolecf-20240212/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-02-12 04:47:03.000000 libolecf-20240212/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/pyolecf/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23134 2024-02-12 04:39:37.000000 libolecf-20240212/pyolecf/pyolecf_property_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2904 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_property_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3224 2024-02-12 04:39:37.000000 libolecf-20240212/pyolecf/pyolecf_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32941 2024-02-12 04:39:37.000000 libolecf-20240212/pyolecf/pyolecf_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_libolecf.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18824 2024-02-12 04:39:37.000000 libolecf-20240212/pyolecf/pyolecf.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9021 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_items.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3290 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9639 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_property_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_property_set_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1790 2023-12-03 09:12:36.000000 libolecf-20240212/pyolecf/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1175 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_guid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4624 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_property_set_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_value_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9763 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_property_sections.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13870 2024-02-12 04:39:37.000000 libolecf-20240212/pyolecf/pyolecf_property_section.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1860 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2592 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_property_sections.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33880 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3255 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6804 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_item_types.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16609 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_datetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14739 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19072 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_value_types.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1358 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2862 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_guid.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28148 2024-02-12 04:39:37.000000 libolecf-20240212/pyolecf/pyolecf_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2558 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_property_set.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1826 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_datetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13330 2024-02-12 04:39:37.000000 libolecf-20240212/pyolecf/pyolecf_property_set.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    61463 2024-02-12 04:47:25.000000 libolecf-20240212/pyolecf/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2550 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_property_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1620 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_item_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2705 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_property_section.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2340 2024-02-12 04:38:43.000000 libolecf-20240212/pyolecf/pyolecf_items.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2352 2023-12-03 09:12:27.000000 libolecf-20240212/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:54.000000 libolecf-20240212/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-02-12 04:47:25.000000 libolecf-20240212/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-02-12 04:46:58.000000 libolecf-20240212/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:12:28.000000 libolecf-20240212/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-02-12 04:47:25.000000 libolecf-20240212/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:53.000000 libolecf-20240212/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-02-12 04:38:44.000000 libolecf-20240212/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:53.000000 libolecf-20240212/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-02-12 04:38:42.000000 libolecf-20240212/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-02-12 04:38:42.000000 libolecf-20240212/dpkg/libolecf-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2227 2024-02-12 04:38:42.000000 libolecf-20240212/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      769 2024-02-12 04:38:42.000000 libolecf-20240212/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-02-12 04:38:42.000000 libolecf-20240212/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-02-12 04:38:42.000000 libolecf-20240212/dpkg/libolecf-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-02-12 04:47:34.000000 libolecf-20240212/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-02-12 04:38:42.000000 libolecf-20240212/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-02-12 04:38:42.000000 libolecf-20240212/dpkg/libolecf.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-02-12 04:38:42.000000 libolecf-20240212/dpkg/libolecf-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      482 2024-02-12 04:47:34.000000 libolecf-20240212/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-02-12 04:38:42.000000 libolecf-20240212/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1892069 2024-02-12 04:47:23.000000 libolecf-20240212/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-02-12 04:47:25.000000 libolecf-20240212/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-02-12 04:47:25.000000 libolecf-20240212/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32442 2024-02-12 04:39:22.000000 libolecf-20240212/msvscpp/libolecf.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/olecf_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5890 2024-02-12 04:39:22.000000 libolecf-20240212/msvscpp/olecf_test_notify/olecf_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/libfole/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4605 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/libfole/libfole.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/olecf_test_property_set/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5908 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/olecf_test_property_set/olecf_test_property_set.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/libolecf/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10241 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/libolecf/libolecf.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/olecf_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5835 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/olecf_test_tools_output/olecf_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/olecfinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6801 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/olecfinfo/olecfinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/olecfmount/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7444 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/olecfmount/olecfmount.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/libfwps/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6294 2024-02-12 04:39:22.000000 libolecf-20240212/msvscpp/libfwps/libfwps.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/pyolecf/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8567 2024-02-12 04:39:22.000000 libolecf-20240212/msvscpp/pyolecf/pyolecf.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1559 2024-02-12 04:39:22.000000 libolecf-20240212/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/olecf_test_item/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5884 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/olecf_test_item/olecf_test_item.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/olecfexport/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7058 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/olecfexport/olecfexport.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/olecf_test_file_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6155 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/olecf_test_file_header/olecf_test_file_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/olecf_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5899 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/olecf_test_io_handle/olecf_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/olecf_test_file/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6547 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/olecf_test_file/olecf_test_file.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/olecf_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5641 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/olecf_test_error/olecf_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/olecf_test_property_value/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5914 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/olecf_test_property_value/olecf_test_property_value.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/olecf_test_allocation_table/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5920 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/olecf_test_allocation_table/olecf_test_allocation_table.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/olecf_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5835 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/olecf_test_tools_signal/olecf_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/olecf_test_property_section/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5920 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/olecf_test_property_section/olecf_test_property_section.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/olecf_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6000 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/olecf_test_tools_info_handle/olecf_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/olecf_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6556 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/olecf_test_support/olecf_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23464 2024-02-12 04:47:25.000000 libolecf-20240212/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8010 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/libfvalue/libfvalue.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/olecf_test_directory_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6000 2024-02-12 04:39:22.000000 libolecf-20240212/msvscpp/olecf_test_directory_entry/olecf_test_directory_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-02-12 04:39:04.000000 libolecf-20240212/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/olecftools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37205 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/mount_dokan.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2989 2024-02-12 04:39:37.000000 libolecf-20240212/olecftools/mount_file_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecftools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26459 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/mount_fuse.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3536 2024-02-12 04:39:37.000000 libolecf-20240212/olecftools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1409 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecftools_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5417 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/mount_dokan.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecftools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30251 2024-02-12 04:39:37.000000 libolecf-20240212/olecftools/mount_file_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4648 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecftools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecftools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1418 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecftools_libfole.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecftools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3212 2023-12-03 09:12:37.000000 libolecf-20240212/olecftools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1443 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecftools_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecftools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1467 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecftools_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecftools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21404 2024-02-12 04:39:37.000000 libolecf-20240212/olecftools/mount_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52038 2024-02-12 04:39:37.000000 libolecf-20240212/olecftools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34790 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/export_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3615 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/mount_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecftools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7995 2024-02-12 04:39:37.000000 libolecf-20240212/olecftools/olecfinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9777 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecfexport.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5938 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/log_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15862 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecfmount.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2279 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/mount_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecftools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecftools_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1446 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecftools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3567 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/export_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12382 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/mount_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecftools_libolecf.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecftools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecftools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36034 2024-02-12 04:47:25.000000 libolecf-20240212/olecftools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1674 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/log_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/olecftools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2765 2024-02-12 04:38:43.000000 libolecf-20240212/olecftools/mount_fuse.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-02-12 04:38:42.000000 libolecf-20240212/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:54.000000 libolecf-20240212/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30704 2024-02-12 04:47:25.000000 libolecf-20240212/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-02-12 04:47:02.000000 libolecf-20240212/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      470 2024-02-12 04:39:22.000000 libolecf-20240212/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-02-12 04:47:25.000000 libolecf-20240212/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:54.000000 libolecf-20240212/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32388 2024-02-12 04:47:25.000000 libolecf-20240212/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-12 04:46:59.000000 libolecf-20240212/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-02-12 04:38:42.000000 libolecf-20240212/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      483 2024-02-12 04:38:42.000000 libolecf-20240212/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-02-12 04:47:25.000000 libolecf-20240212/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-02-12 04:38:42.000000 libolecf-20240212/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1785 2024-02-12 04:38:42.000000 libolecf-20240212/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:12:28.000000 libolecf-20240212/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:54.000000 libolecf-20240212/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32794 2024-02-12 04:47:25.000000 libolecf-20240212/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-02-12 04:47:07.000000 libolecf-20240212/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-02-12 04:47:25.000000 libolecf-20240212/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:54.000000 libolecf-20240212/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-02-12 04:47:05.000000 libolecf-20240212/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-12 04:47:05.000000 libolecf-20240212/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-02-12 04:47:05.000000 libolecf-20240212/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-02-12 04:47:05.000000 libolecf-20240212/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-12 04:47:05.000000 libolecf-20240212/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-12 04:47:05.000000 libolecf-20240212/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-12 04:47:05.000000 libolecf-20240212/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-02-12 04:47:05.000000 libolecf-20240212/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-02-12 04:47:05.000000 libolecf-20240212/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-12 04:47:05.000000 libolecf-20240212/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-12 04:47:05.000000 libolecf-20240212/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-12 04:47:05.000000 libolecf-20240212/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29982 2024-02-12 04:47:25.000000 libolecf-20240212/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-12 04:47:05.000000 libolecf-20240212/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-12 04:47:05.000000 libolecf-20240212/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-02-12 04:47:05.000000 libolecf-20240212/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-02-12 04:47:05.000000 libolecf-20240212/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11230 2023-12-03 09:12:27.000000 libolecf-20240212/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2100 2024-02-12 04:38:44.000000 libolecf-20240212/manuals/olecfinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      192 2023-12-03 09:12:33.000000 libolecf-20240212/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11257 2024-02-12 04:38:44.000000 libolecf-20240212/manuals/libolecf.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26941 2024-02-12 04:47:25.000000 libolecf-20240212/manuals/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2537 2024-02-12 04:38:44.000000 libolecf-20240212/manuals/olecfexport.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      766 2024-02-12 04:38:42.000000 libolecf-20240212/libolecf.pc.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21973 2024-02-12 04:39:22.000000 libolecf-20240212/tests/olecf_test_file_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1812 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35624 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8355 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_io_handle.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4068 2024-02-12 04:39:37.000000 libolecf-20240212/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5634 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_tools_info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6694 2024-02-12 04:39:22.000000 libolecf-20240212/tests/olecf_test_allocation_table.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4771 2024-02-12 04:38:44.000000 libolecf-20240212/tests/test_olecfexport.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6728 2024-02-12 04:39:22.000000 libolecf-20240212/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13259 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_libolecf.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_memory.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-02-12 04:38:44.000000 libolecf-20240212/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4077 2024-02-12 04:40:00.000000 libolecf-20240212/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9376 2024-02-12 04:39:22.000000 libolecf-20240212/tests/olecf_test_directory_entry.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3320 2024-02-12 04:38:44.000000 libolecf-20240212/tests/test_olecfinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3524 2024-02-12 04:39:22.000000 libolecf-20240212/tests/olecf_test_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15225 2024-02-12 04:39:22.000000 libolecf-20240212/tests/olecf_test_property_set.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50191 2024-02-12 04:39:22.000000 libolecf-20240212/tests/olecf_test_property_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-02-12 04:38:44.000000 libolecf-20240212/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14367 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17122 2024-02-12 04:39:22.000000 libolecf-20240212/tests/olecf_test_property_section.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6660 2024-02-12 04:39:37.000000 libolecf-20240212/tests/pyolecf_test_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    63061 2024-02-12 04:47:25.000000 libolecf-20240212/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3440 2024-02-12 04:39:37.000000 libolecf-20240212/tests/pyolecf_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2024-02-12 04:38:44.000000 libolecf-20240212/tests/olecf_test_tools_signal.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4170 2024-02-12 04:39:37.000000 libolecf-20240212/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-02-12 04:38:43.000000 libolecf-20240212/ossfuzz/ossfuzz_libolecf.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-12-03 09:12:30.000000 libolecf-20240212/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-12 04:38:43.000000 libolecf-20240212/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2916 2024-02-12 04:38:43.000000 libolecf-20240212/ossfuzz/item_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2214 2024-02-12 04:38:43.000000 libolecf-20240212/ossfuzz/file_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33955 2024-02-12 04:47:25.000000 libolecf-20240212/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-02-12 04:47:20.000000 libolecf-20240212/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:54.000000 libolecf-20240212/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-02-12 04:47:06.000000 libolecf-20240212/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-02-12 04:47:06.000000 libolecf-20240212/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-02-12 04:47:06.000000 libolecf-20240212/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-02-12 04:47:06.000000 libolecf-20240212/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-12 04:47:06.000000 libolecf-20240212/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-02-12 04:47:06.000000 libolecf-20240212/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-12 04:47:06.000000 libolecf-20240212/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-02-12 04:47:06.000000 libolecf-20240212/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-12 04:47:06.000000 libolecf-20240212/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-02-12 04:47:06.000000 libolecf-20240212/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-12 04:47:06.000000 libolecf-20240212/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-02-12 04:47:06.000000 libolecf-20240212/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-12 04:47:06.000000 libolecf-20240212/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-12 04:47:06.000000 libolecf-20240212/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-12 04:47:06.000000 libolecf-20240212/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-02-12 04:47:06.000000 libolecf-20240212/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30762 2024-02-12 04:47:25.000000 libolecf-20240212/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-02-12 04:47:06.000000 libolecf-20240212/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-02-12 04:47:06.000000 libolecf-20240212/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:55.000000 libolecf-20240212/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:12:35.000000 libolecf-20240212/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:12:35.000000 libolecf-20240212/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:12:35.000000 libolecf-20240212/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:12:35.000000 libolecf-20240212/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:12:35.000000 libolecf-20240212/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:12:35.000000 libolecf-20240212/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:12:35.000000 libolecf-20240212/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:12:35.000000 libolecf-20240212/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:12:35.000000 libolecf-20240212/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-02-12 04:47:34.000000 libolecf-20240212/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:12:35.000000 libolecf-20240212/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:12:35.000000 libolecf-20240212/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:54.000000 libolecf-20240212/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53506 2024-02-12 04:47:25.000000 libolecf-20240212/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-02-12 04:47:16.000000 libolecf-20240212/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41061 2024-02-12 04:47:25.000000 libolecf-20240212/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:54.000000 libolecf-20240212/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_split_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_split_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1684 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_split_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_binary_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_value_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_split_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_floating_point.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_binary_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_value_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35219 2024-02-12 04:47:25.000000 libolecf-20240212/libfvalue/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_floating_point.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-12 04:47:12.000000 libolecf-20240212/libfvalue/libfvalue_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:54.000000 libolecf-20240212/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-12 04:47:04.000000 libolecf-20240212/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-12 04:47:04.000000 libolecf-20240212/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-02-12 04:47:04.000000 libolecf-20240212/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-02-12 04:47:04.000000 libolecf-20240212/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-02-12 04:47:04.000000 libolecf-20240212/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-12 04:47:04.000000 libolecf-20240212/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-02-12 04:47:04.000000 libolecf-20240212/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-02-12 04:47:04.000000 libolecf-20240212/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-02-12 04:47:04.000000 libolecf-20240212/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-02-12 04:47:04.000000 libolecf-20240212/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-02-12 04:47:04.000000 libolecf-20240212/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29816 2024-02-12 04:47:25.000000 libolecf-20240212/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-12 04:47:04.000000 libolecf-20240212/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-02-12 04:47:04.000000 libolecf-20240212/libcnotify/libcnotify_print.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2539 2024-02-12 04:47:34.000000 libolecf-20240212/libolecf.spec
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:54.000000 libolecf-20240212/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-02-12 04:47:00.000000 libolecf-20240212/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-02-12 04:47:00.000000 libolecf-20240212/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-12 04:47:00.000000 libolecf-20240212/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-02-12 04:47:00.000000 libolecf-20240212/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-12 04:47:00.000000 libolecf-20240212/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-12 04:47:00.000000 libolecf-20240212/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-02-12 04:47:00.000000 libolecf-20240212/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-02-12 04:47:00.000000 libolecf-20240212/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-02-12 04:47:00.000000 libolecf-20240212/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-12 04:47:00.000000 libolecf-20240212/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-12 04:47:00.000000 libolecf-20240212/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29329 2024-02-12 04:47:25.000000 libolecf-20240212/libcerror/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-12 05:00:54.000000 libolecf-20240212/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1148 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32555 2024-02-12 04:47:25.000000 libolecf-20240212/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-02-12 04:47:09.000000 libolecf-20240212/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56853 2024-02-12 04:47:22.000000 libolecf-20240212/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7959 2024-02-12 04:38:42.000000 libolecf-20240212/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      414 2024-02-12 05:00:56.214719 libolecf-20240212/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3540 2024-04-27 03:38:36.000000 libolecf-20240427/libolecf.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:43.000000 libolecf-20240427/libfole/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-27 05:20:04.000000 libolecf-20240427/libfole/libfole_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-27 05:20:04.000000 libolecf-20240427/libfole/libfole_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      661 2024-04-27 05:20:04.000000 libolecf-20240427/libfole/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1555 2024-04-27 05:20:04.000000 libolecf-20240427/libfole/libfole_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-27 05:20:04.000000 libolecf-20240427/libfole/libfole_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-27 05:20:04.000000 libolecf-20240427/libfole/libfole_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1407 2024-04-27 05:20:04.000000 libolecf-20240427/libfole/libfole_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-27 05:20:04.000000 libolecf-20240427/libfole/libfole_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3793 2024-04-27 05:20:04.000000 libolecf-20240427/libfole/libfole_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-27 05:20:04.000000 libolecf-20240427/libfole/libfole_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-27 05:20:04.000000 libolecf-20240427/libfole/libfole_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29510 2024-04-27 05:20:22.000000 libolecf-20240427/libfole/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-27 05:20:04.000000 libolecf-20240427/libfole/libfole_extern.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:44.000000 libolecf-20240427/libolecf/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2593 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/olecf_property_set.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23541 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_property_section.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2751 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_directory_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3367 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_property_section.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2612 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_directory_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3877 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2038 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4933 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_ole.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1924 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    46491 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16011 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_file_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18982 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_property_set.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/olecf_directory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4557 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2704 2024-04-27 03:46:03.000000 libolecf-20240427/libolecf/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2926 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_property_set_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1276 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_libfole.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2100 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42634 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9462 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2024-04-27 05:20:34.000000 libolecf-20240427/libolecf/libolecf.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33123 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    59693 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_property_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1517 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_libfwps.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26754 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_directory_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8242 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_allocation_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1404 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_directory_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2655 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5790 2024-04-27 05:20:34.000000 libolecf-20240427/libolecf/libolecf_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5792 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3395 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_directory_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1364 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_property_set_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3640 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/olecf_file_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/olecf_compound_object.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7088 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_property_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8893 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26095 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_compound_object_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1826 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1858 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2025 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_allocation_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2761 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_file_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38026 2024-04-27 05:20:22.000000 libolecf-20240427/libolecf/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1356 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_compound_object_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5369 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14768 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_directory_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2950 2024-04-27 03:38:40.000000 libolecf-20240427/libolecf/libolecf_property_set.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-27 03:38:36.000000 libolecf-20240427/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-27 05:20:21.000000 libolecf-20240427/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 03:38:36.000000 libolecf-20240427/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-27 05:20:22.000000 libolecf-20240427/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:43.000000 libolecf-20240427/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-27 05:20:03.000000 libolecf-20240427/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-04-27 05:20:03.000000 libolecf-20240427/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-04-27 05:20:03.000000 libolecf-20240427/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-27 05:20:03.000000 libolecf-20240427/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-04-27 05:20:03.000000 libolecf-20240427/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-27 05:20:03.000000 libolecf-20240427/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-27 05:20:03.000000 libolecf-20240427/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-04-27 05:20:03.000000 libolecf-20240427/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-04-27 05:20:03.000000 libolecf-20240427/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-04-27 05:20:03.000000 libolecf-20240427/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-04-27 05:20:03.000000 libolecf-20240427/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29590 2024-04-27 05:20:22.000000 libolecf-20240427/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-27 05:20:03.000000 libolecf-20240427/libfguid/libfguid_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:41.000000 libolecf-20240427/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-04-27 03:38:43.000000 libolecf-20240427/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-04-27 03:38:43.000000 libolecf-20240427/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:12:35.000000 libolecf-20240427/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-04-27 03:38:43.000000 libolecf-20240427/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:12:35.000000 libolecf-20240427/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:12:35.000000 libolecf-20240427/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-04-27 03:38:43.000000 libolecf-20240427/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:12:35.000000 libolecf-20240427/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:12:35.000000 libolecf-20240427/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4187 2024-04-27 03:38:43.000000 libolecf-20240427/m4/libfole.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-04-27 03:38:43.000000 libolecf-20240427/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-04-27 03:38:43.000000 libolecf-20240427/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-04-27 03:38:43.000000 libolecf-20240427/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-27 03:38:43.000000 libolecf-20240427/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-27 03:38:43.000000 libolecf-20240427/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-27 05:20:15.000000 libolecf-20240427/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-27 05:20:15.000000 libolecf-20240427/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:12:36.000000 libolecf-20240427/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10266 2024-04-27 03:38:43.000000 libolecf-20240427/m4/libfwps.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7058 2024-04-27 03:38:43.000000 libolecf-20240427/m4/libfuse.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-27 05:20:15.000000 libolecf-20240427/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:12:35.000000 libolecf-20240427/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-27 03:38:43.000000 libolecf-20240427/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-27 03:38:43.000000 libolecf-20240427/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-04-27 03:38:43.000000 libolecf-20240427/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-04-27 03:38:43.000000 libolecf-20240427/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:12:35.000000 libolecf-20240427/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-27 05:20:15.000000 libolecf-20240427/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:12:35.000000 libolecf-20240427/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:12:35.000000 libolecf-20240427/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-27 05:20:15.000000 libolecf-20240427/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:12:35.000000 libolecf-20240427/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-04-27 03:38:43.000000 libolecf-20240427/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20032 2024-04-27 03:38:43.000000 libolecf-20240427/m4/libfvalue.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:12:36.000000 libolecf-20240427/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-27 03:38:43.000000 libolecf-20240427/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:41.000000 libolecf-20240427/include/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:41.000000 libolecf-20240427/include/libolecf/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4916 2024-04-27 03:38:39.000000 libolecf-20240427/include/libolecf/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4914 2024-04-27 05:20:34.000000 libolecf-20240427/include/libolecf/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5108 2024-04-27 03:38:39.000000 libolecf-20240427/include/libolecf/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4977 2024-04-27 05:20:34.000000 libolecf-20240427/include/libolecf/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-27 03:38:39.000000 libolecf-20240427/include/libolecf/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-04-27 03:38:39.000000 libolecf-20240427/include/libolecf/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-27 03:38:39.000000 libolecf-20240427/include/libolecf/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2024-04-27 05:20:34.000000 libolecf-20240427/include/libolecf/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4600 2024-04-27 03:38:39.000000 libolecf-20240427/include/libolecf/ole.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-04-27 03:38:39.000000 libolecf-20240427/include/libolecf/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28257 2024-04-27 05:20:34.000000 libolecf-20240427/include/libolecf.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      443 2024-04-27 03:44:26.000000 libolecf-20240427/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28257 2024-04-27 03:38:39.000000 libolecf-20240427/include/libolecf.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27984 2024-04-27 05:20:21.000000 libolecf-20240427/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:43.000000 libolecf-20240427/libfwps/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2490 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_set.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2104 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_store.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1202 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3827 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3731 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_format_class_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9704 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_store.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3967 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2244 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_property_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_format_class_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7534 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_property_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7144 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    83917 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16442 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_set.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32454 2024-04-27 05:20:22.000000 libolecf-20240427/libfwps/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-27 05:20:07.000000 libolecf-20240427/libfwps/libfwps_unused.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:41.000000 libolecf-20240427/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-27 03:38:38.000000 libolecf-20240427/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-27 03:38:38.000000 libolecf-20240427/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-27 03:38:38.000000 libolecf-20240427/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-27 03:38:38.000000 libolecf-20240427/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-27 03:38:38.000000 libolecf-20240427/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-27 03:38:38.000000 libolecf-20240427/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-27 03:38:39.000000 libolecf-20240427/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-27 03:44:26.000000 libolecf-20240427/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-27 03:38:39.000000 libolecf-20240427/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-04-27 05:20:34.000000 libolecf-20240427/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16697 2024-04-27 05:20:21.000000 libolecf-20240427/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17688 2024-04-27 05:20:34.000000 libolecf-20240427/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-27 03:38:39.000000 libolecf-20240427/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-27 03:38:39.000000 libolecf-20240427/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-27 03:38:38.000000 libolecf-20240427/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25000 2024-04-27 05:20:21.000000 libolecf-20240427/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:42.000000 libolecf-20240427/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-04-27 05:19:56.000000 libolecf-20240427/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-27 05:19:56.000000 libolecf-20240427/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-04-27 05:19:56.000000 libolecf-20240427/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-04-27 05:19:56.000000 libolecf-20240427/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-27 05:19:56.000000 libolecf-20240427/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-27 05:19:56.000000 libolecf-20240427/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-04-27 05:19:56.000000 libolecf-20240427/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-04-27 05:19:56.000000 libolecf-20240427/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-04-27 05:19:56.000000 libolecf-20240427/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-04-27 05:19:56.000000 libolecf-20240427/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30198 2024-04-27 05:20:21.000000 libolecf-20240427/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-27 05:19:56.000000 libolecf-20240427/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-04-27 05:19:56.000000 libolecf-20240427/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-04-27 05:19:56.000000 libolecf-20240427/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:44.000000 libolecf-20240427/pyolecf/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23125 2024-04-27 03:39:50.000000 libolecf-20240427/pyolecf/pyolecf_property_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2904 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_property_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3224 2024-04-27 03:39:50.000000 libolecf-20240427/pyolecf/pyolecf_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32941 2024-04-27 03:39:50.000000 libolecf-20240427/pyolecf/pyolecf_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_libolecf.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18824 2024-04-27 03:39:50.000000 libolecf-20240427/pyolecf/pyolecf.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9021 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_items.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3290 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9639 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_property_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_property_set_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1786 2024-04-27 03:45:47.000000 libolecf-20240427/pyolecf/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1175 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_guid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4624 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_property_set_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_value_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9763 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_property_sections.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13870 2024-04-27 03:39:50.000000 libolecf-20240427/pyolecf/pyolecf_property_section.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1860 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2592 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_property_sections.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33880 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3255 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6804 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_item_types.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16609 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_datetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14739 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19072 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_value_types.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1358 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2862 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_guid.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28148 2024-04-27 03:39:50.000000 libolecf-20240427/pyolecf/pyolecf_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2558 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_property_set.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1826 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_datetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13330 2024-04-27 03:39:50.000000 libolecf-20240427/pyolecf/pyolecf_property_set.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    62566 2024-04-27 05:20:22.000000 libolecf-20240427/pyolecf/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2550 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_property_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1620 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_item_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2705 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_property_section.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2340 2024-04-27 03:38:41.000000 libolecf-20240427/pyolecf/pyolecf_items.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2160 2024-04-27 03:46:42.000000 libolecf-20240427/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:43.000000 libolecf-20240427/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34050 2024-04-27 05:20:21.000000 libolecf-20240427/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-04-27 05:19:50.000000 libolecf-20240427/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:12:28.000000 libolecf-20240427/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-27 05:20:21.000000 libolecf-20240427/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:41.000000 libolecf-20240427/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-04-27 03:38:43.000000 libolecf-20240427/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:41.000000 libolecf-20240427/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-27 03:38:36.000000 libolecf-20240427/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-27 03:38:36.000000 libolecf-20240427/dpkg/libolecf-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2227 2024-04-27 03:38:36.000000 libolecf-20240427/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      769 2024-04-27 03:38:36.000000 libolecf-20240427/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-04-27 03:38:36.000000 libolecf-20240427/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-27 03:38:36.000000 libolecf-20240427/dpkg/libolecf-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-04-27 05:20:34.000000 libolecf-20240427/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-27 03:38:36.000000 libolecf-20240427/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-27 03:38:36.000000 libolecf-20240427/dpkg/libolecf.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-04-27 03:38:36.000000 libolecf-20240427/dpkg/libolecf-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      482 2024-04-27 05:20:34.000000 libolecf-20240427/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-27 03:38:36.000000 libolecf-20240427/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1913199 2024-04-27 05:20:20.000000 libolecf-20240427/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-27 05:20:21.000000 libolecf-20240427/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-27 05:20:21.000000 libolecf-20240427/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32442 2024-04-27 03:39:23.000000 libolecf-20240427/msvscpp/libolecf.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/olecf_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5890 2024-04-27 03:39:23.000000 libolecf-20240427/msvscpp/olecf_test_notify/olecf_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/libfole/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4605 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/libfole/libfole.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/olecf_test_property_set/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5908 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/olecf_test_property_set/olecf_test_property_set.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/libolecf/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10241 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/libolecf/libolecf.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/olecf_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5835 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/olecf_test_tools_output/olecf_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/olecfinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6801 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/olecfinfo/olecfinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/olecfmount/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7444 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/olecfmount/olecfmount.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/libfwps/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6294 2024-04-27 03:39:23.000000 libolecf-20240427/msvscpp/libfwps/libfwps.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/pyolecf/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8567 2024-04-27 03:39:23.000000 libolecf-20240427/msvscpp/pyolecf/pyolecf.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1530 2024-04-27 03:45:35.000000 libolecf-20240427/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/olecf_test_item/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5884 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/olecf_test_item/olecf_test_item.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/olecfexport/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7058 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/olecfexport/olecfexport.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/olecf_test_file_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6155 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/olecf_test_file_header/olecf_test_file_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/olecf_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5899 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/olecf_test_io_handle/olecf_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/olecf_test_file/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6547 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/olecf_test_file/olecf_test_file.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/olecf_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5641 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/olecf_test_error/olecf_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/olecf_test_property_value/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5914 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/olecf_test_property_value/olecf_test_property_value.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/olecf_test_allocation_table/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5920 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/olecf_test_allocation_table/olecf_test_allocation_table.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/olecf_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5835 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/olecf_test_tools_signal/olecf_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/olecf_test_property_section/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5920 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/olecf_test_property_section/olecf_test_property_section.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/olecf_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6000 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/olecf_test_tools_info_handle/olecf_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/olecf_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6556 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/olecf_test_support/olecf_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23520 2024-04-27 05:20:22.000000 libolecf-20240427/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8010 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/libfvalue/libfvalue.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/olecf_test_directory_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6000 2024-04-27 03:39:23.000000 libolecf-20240427/msvscpp/olecf_test_directory_entry/olecf_test_directory_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-04-27 03:39:05.000000 libolecf-20240427/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:44.000000 libolecf-20240427/olecftools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37205 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/mount_dokan.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2989 2024-04-27 03:39:50.000000 libolecf-20240427/olecftools/mount_file_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecftools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26459 2024-04-27 03:39:50.000000 libolecf-20240427/olecftools/mount_fuse.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3536 2024-04-27 03:39:50.000000 libolecf-20240427/olecftools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1409 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecftools_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5417 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/mount_dokan.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecftools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30251 2024-04-27 03:39:50.000000 libolecf-20240427/olecftools/mount_file_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4648 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecftools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecftools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1418 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecftools_libfole.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecftools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3208 2024-04-27 03:45:24.000000 libolecf-20240427/olecftools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1443 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecftools_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecftools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1467 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecftools_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecftools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21404 2024-04-27 03:39:50.000000 libolecf-20240427/olecftools/mount_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52038 2024-04-27 03:39:50.000000 libolecf-20240427/olecftools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34790 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/export_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3615 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/mount_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecftools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7995 2024-04-27 03:39:50.000000 libolecf-20240427/olecftools/olecfinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9777 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecfexport.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5938 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/log_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15862 2024-04-27 03:39:50.000000 libolecf-20240427/olecftools/olecfmount.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2279 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/mount_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecftools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecftools_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1446 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecftools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3567 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/export_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12382 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/mount_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecftools_libolecf.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecftools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecftools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36633 2024-04-27 05:20:22.000000 libolecf-20240427/olecftools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1674 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/log_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-04-27 03:38:42.000000 libolecf-20240427/olecftools/olecftools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2765 2024-04-27 03:39:50.000000 libolecf-20240427/olecftools/mount_fuse.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-04-27 03:38:38.000000 libolecf-20240427/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:43.000000 libolecf-20240427/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31031 2024-04-27 05:20:21.000000 libolecf-20240427/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-04-27 05:19:54.000000 libolecf-20240427/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      470 2024-04-27 03:39:50.000000 libolecf-20240427/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-27 05:20:21.000000 libolecf-20240427/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:42.000000 libolecf-20240427/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32944 2024-04-27 05:20:21.000000 libolecf-20240427/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-27 05:19:52.000000 libolecf-20240427/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-27 03:38:36.000000 libolecf-20240427/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      483 2024-04-27 03:38:36.000000 libolecf-20240427/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-27 05:20:21.000000 libolecf-20240427/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-27 03:38:36.000000 libolecf-20240427/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1785 2024-04-27 03:38:36.000000 libolecf-20240427/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:12:28.000000 libolecf-20240427/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:42.000000 libolecf-20240427/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33383 2024-04-27 05:20:22.000000 libolecf-20240427/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-27 05:20:00.000000 libolecf-20240427/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-27 05:20:22.000000 libolecf-20240427/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:43.000000 libolecf-20240427/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-04-27 05:19:58.000000 libolecf-20240427/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-27 05:19:58.000000 libolecf-20240427/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-04-27 05:19:58.000000 libolecf-20240427/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-04-27 05:19:58.000000 libolecf-20240427/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-27 05:19:58.000000 libolecf-20240427/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-27 05:19:58.000000 libolecf-20240427/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-27 05:19:58.000000 libolecf-20240427/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-04-27 05:19:58.000000 libolecf-20240427/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-27 05:19:58.000000 libolecf-20240427/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-27 05:19:58.000000 libolecf-20240427/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-27 05:19:58.000000 libolecf-20240427/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-27 05:19:58.000000 libolecf-20240427/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30229 2024-04-27 05:20:21.000000 libolecf-20240427/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-27 05:19:58.000000 libolecf-20240427/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-27 05:19:58.000000 libolecf-20240427/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-04-27 05:19:58.000000 libolecf-20240427/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-04-27 05:19:58.000000 libolecf-20240427/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11230 2023-12-03 09:12:27.000000 libolecf-20240427/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2100 2024-04-27 03:38:43.000000 libolecf-20240427/manuals/olecfinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      163 2024-04-27 03:45:08.000000 libolecf-20240427/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11257 2024-04-27 03:38:43.000000 libolecf-20240427/manuals/libolecf.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26997 2024-04-27 05:20:22.000000 libolecf-20240427/manuals/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2537 2024-04-27 03:38:43.000000 libolecf-20240427/manuals/olecfexport.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      766 2024-04-27 03:38:36.000000 libolecf-20240427/libolecf.pc.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21973 2024-04-27 03:39:23.000000 libolecf-20240427/tests/olecf_test_file_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2024-04-27 03:38:43.000000 libolecf-20240427/tests/olecf_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1812 2024-04-27 03:38:42.000000 libolecf-20240427/tests/olecf_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-04-27 03:38:43.000000 libolecf-20240427/tests/olecf_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35624 2024-04-27 03:38:42.000000 libolecf-20240427/tests/olecf_test_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-04-27 03:38:43.000000 libolecf-20240427/tests/olecf_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-04-27 03:38:42.000000 libolecf-20240427/tests/olecf_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8355 2024-04-27 03:38:42.000000 libolecf-20240427/tests/olecf_test_io_handle.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4037 2024-04-27 03:41:52.000000 libolecf-20240427/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-04-27 03:38:42.000000 libolecf-20240427/tests/olecf_test_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5634 2024-04-27 03:38:43.000000 libolecf-20240427/tests/olecf_test_tools_info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-04-27 03:38:43.000000 libolecf-20240427/tests/olecf_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6694 2024-04-27 03:39:23.000000 libolecf-20240427/tests/olecf_test_allocation_table.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4740 2024-04-27 03:42:34.000000 libolecf-20240427/tests/test_olecfexport.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6745 2024-04-27 03:47:02.000000 libolecf-20240427/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-04-27 03:38:42.000000 libolecf-20240427/tests/olecf_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13259 2024-04-27 03:38:42.000000 libolecf-20240427/tests/olecf_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-04-27 03:38:43.000000 libolecf-20240427/tests/olecf_test_libolecf.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-04-27 03:38:43.000000 libolecf-20240427/tests/olecf_test_memory.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-27 03:38:42.000000 libolecf-20240427/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4406 2024-04-27 03:41:30.000000 libolecf-20240427/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-27 03:38:43.000000 libolecf-20240427/tests/olecf_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-04-27 03:38:42.000000 libolecf-20240427/tests/olecf_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9376 2024-04-27 03:39:23.000000 libolecf-20240427/tests/olecf_test_directory_entry.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3289 2024-04-27 03:38:42.000000 libolecf-20240427/tests/test_olecfinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-04-27 03:38:43.000000 libolecf-20240427/tests/olecf_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3524 2024-04-27 03:39:23.000000 libolecf-20240427/tests/olecf_test_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15225 2024-04-27 03:39:23.000000 libolecf-20240427/tests/olecf_test_property_set.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50191 2024-04-27 03:39:23.000000 libolecf-20240427/tests/olecf_test_property_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-27 03:38:42.000000 libolecf-20240427/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-04-27 03:38:42.000000 libolecf-20240427/tests/olecf_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-04-27 03:38:43.000000 libolecf-20240427/tests/olecf_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-04-27 03:38:42.000000 libolecf-20240427/tests/olecf_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14367 2024-04-27 03:38:43.000000 libolecf-20240427/tests/olecf_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17122 2024-04-27 03:39:23.000000 libolecf-20240427/tests/olecf_test_property_section.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6660 2024-04-27 03:39:50.000000 libolecf-20240427/tests/pyolecf_test_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64128 2024-04-27 05:20:22.000000 libolecf-20240427/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-04-27 03:38:43.000000 libolecf-20240427/tests/olecf_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3440 2024-04-27 03:39:50.000000 libolecf-20240427/tests/pyolecf_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2024-04-27 03:38:43.000000 libolecf-20240427/tests/olecf_test_tools_signal.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4139 2024-04-27 03:40:56.000000 libolecf-20240427/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-04-27 03:38:40.000000 libolecf-20240427/ossfuzz/ossfuzz_libolecf.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1388 2024-04-27 03:44:44.000000 libolecf-20240427/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-27 03:38:40.000000 libolecf-20240427/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2916 2024-04-27 03:38:40.000000 libolecf-20240427/ossfuzz/item_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2214 2024-04-27 03:38:40.000000 libolecf-20240427/ossfuzz/file_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34107 2024-04-27 05:20:22.000000 libolecf-20240427/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-27 05:20:15.000000 libolecf-20240427/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:42.000000 libolecf-20240427/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-04-27 05:19:59.000000 libolecf-20240427/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-04-27 05:19:59.000000 libolecf-20240427/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-04-27 05:19:59.000000 libolecf-20240427/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-04-27 05:19:59.000000 libolecf-20240427/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-27 05:19:59.000000 libolecf-20240427/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-04-27 05:19:59.000000 libolecf-20240427/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-27 05:19:59.000000 libolecf-20240427/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-04-27 05:19:59.000000 libolecf-20240427/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-27 05:19:59.000000 libolecf-20240427/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-04-27 05:19:59.000000 libolecf-20240427/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-27 05:19:59.000000 libolecf-20240427/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-04-27 05:19:59.000000 libolecf-20240427/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-27 05:19:59.000000 libolecf-20240427/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-27 05:19:59.000000 libolecf-20240427/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-27 05:19:59.000000 libolecf-20240427/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-04-27 05:19:59.000000 libolecf-20240427/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31126 2024-04-27 05:20:22.000000 libolecf-20240427/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-04-27 05:19:59.000000 libolecf-20240427/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-04-27 05:19:59.000000 libolecf-20240427/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:45.000000 libolecf-20240427/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:12:35.000000 libolecf-20240427/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:12:35.000000 libolecf-20240427/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:12:35.000000 libolecf-20240427/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:12:35.000000 libolecf-20240427/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:12:35.000000 libolecf-20240427/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:12:35.000000 libolecf-20240427/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:12:35.000000 libolecf-20240427/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:12:35.000000 libolecf-20240427/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:12:35.000000 libolecf-20240427/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-04-27 05:20:34.000000 libolecf-20240427/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:12:35.000000 libolecf-20240427/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:12:35.000000 libolecf-20240427/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:43.000000 libolecf-20240427/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56710 2024-04-27 05:20:22.000000 libolecf-20240427/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-04-27 05:20:10.000000 libolecf-20240427/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40999 2024-04-27 05:20:21.000000 libolecf-20240427/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:43.000000 libolecf-20240427/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_split_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_split_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_split_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_binary_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_value_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_split_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_floating_point.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_binary_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_value_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36019 2024-04-27 05:20:22.000000 libolecf-20240427/libfvalue/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_floating_point.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-27 05:20:06.000000 libolecf-20240427/libfvalue/libfvalue_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:42.000000 libolecf-20240427/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-27 05:19:57.000000 libolecf-20240427/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-27 05:19:57.000000 libolecf-20240427/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-27 05:19:57.000000 libolecf-20240427/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-27 05:19:57.000000 libolecf-20240427/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-27 05:19:57.000000 libolecf-20240427/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-27 05:19:57.000000 libolecf-20240427/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-27 05:19:57.000000 libolecf-20240427/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-27 05:19:57.000000 libolecf-20240427/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-27 05:19:57.000000 libolecf-20240427/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-27 05:19:57.000000 libolecf-20240427/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-27 05:19:57.000000 libolecf-20240427/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30067 2024-04-27 05:20:21.000000 libolecf-20240427/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-27 05:19:57.000000 libolecf-20240427/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-27 05:19:57.000000 libolecf-20240427/libcnotify/libcnotify_print.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2541 2024-04-27 05:20:34.000000 libolecf-20240427/libolecf.spec
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:41.000000 libolecf-20240427/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-27 05:19:53.000000 libolecf-20240427/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-27 05:19:53.000000 libolecf-20240427/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-27 05:19:53.000000 libolecf-20240427/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-27 05:19:53.000000 libolecf-20240427/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-27 05:19:53.000000 libolecf-20240427/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-27 05:19:53.000000 libolecf-20240427/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-27 05:19:53.000000 libolecf-20240427/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-27 05:19:53.000000 libolecf-20240427/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-27 05:19:53.000000 libolecf-20240427/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-27 05:19:53.000000 libolecf-20240427/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-27 05:19:53.000000 libolecf-20240427/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29534 2024-04-27 05:20:21.000000 libolecf-20240427/libcerror/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-27 09:02:43.000000 libolecf-20240427/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33118 2024-04-27 05:20:22.000000 libolecf-20240427/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-04-27 05:20:02.000000 libolecf-20240427/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56853 2024-04-27 05:20:18.000000 libolecf-20240427/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7959 2024-04-27 03:38:36.000000 libolecf-20240427/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      414 2024-04-27 09:02:46.112960 libolecf-20240427/PKG-INFO
```

### Comparing `libolecf-20240212/libolecf.spec.in` & `libolecf-20240427/libolecf.spec.in`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfole/libfole_value_type.h` & `libolecf-20240427/libfole/libfole_value_type.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfole/libfole_error.c` & `libolecf-20240427/libfole/libfole_error.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfole/Makefile.am` & `libolecf-20240427/libfole/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFOLE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfole.la
 
 libfole_la_SOURCES = \
 	libfole_definitions.h \
 	libfole_extern.h \
@@ -13,19 +13,17 @@
 	libfole_libcerror.h \
 	libfole_support.c libfole_support.h \
 	libfole_types.h \
 	libfole_unused.h \
 	libfole_value_type.c libfole_value_type.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfole ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfole_la_SOURCES)
```

### Comparing `libolecf-20240212/libfole/libfole_definitions.h` & `libolecf-20240427/libfole/libfole_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfole/definitions.h> are copied here
  * for local use of libfole
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFOLE_VERSION					20240119
+#define LIBFOLE_VERSION					20240416
 
 /* The version string
  */
-#define LIBFOLE_VERSION_STRING				"20240119"
+#define LIBFOLE_VERSION_STRING				"20240416"
 
 /* The byte order definitions
  */
 #define LIBFOLE_ENDIAN_BIG				_BYTE_STREAM_ENDIAN_BIG
 #define LIBFOLE_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 #endif /* !defined( HAVE_LOCAL_LIBFOLE ) */
```

### Comparing `libolecf-20240212/libfole/libfole_error.h` & `libolecf-20240427/libfole/libfole_error.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfole/libfole_support.h` & `libolecf-20240427/libfole/libfole_support.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfole/libfole_types.h` & `libolecf-20240427/libfole/libfole_types.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfole/libfole_support.c` & `libolecf-20240427/libfole/libfole_support.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfole/libfole_value_type.c` & `libolecf-20240427/libfole/libfole_value_type.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfole/libfole_unused.h` & `libolecf-20240427/libfole/libfole_unused.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfole/libfole_libcerror.h` & `libolecf-20240427/libfole/libfole_libcerror.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfole/Makefile.in` & `libolecf-20240427/libfole/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -453,14 +453,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -519,30 +521,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFOLE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFOLE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFOLE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFOLE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFOLE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFOLE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFOLE_TRUE@noinst_LTLIBRARIES = libfole.la
 @HAVE_LOCAL_LIBFOLE_TRUE@libfole_la_SOURCES = \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_definitions.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_extern.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_error.c libfole_error.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_libcerror.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_support.c libfole_support.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_types.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_unused.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_value_type.c libfole_value_type.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -744,24 +747,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfole_error.Plo
+	-rm -f ./$(DEPDIR)/libfole_support.Plo
+	-rm -f ./$(DEPDIR)/libfole_value_type.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -847,17 +855,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfole ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfole_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libolecf-20240212/libfole/libfole_extern.h` & `libolecf-20240427/libfole/libfole_extern.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/olecf_property_set.h` & `libolecf-20240427/libolecf/olecf_property_set.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_notify.h` & `libolecf-20240427/libolecf/libolecf_notify.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_libcerror.h` & `libolecf-20240427/libolecf/libolecf_libcerror.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_property_section.c` & `libolecf-20240427/libolecf/libolecf_property_section.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_directory_entry.h` & `libolecf-20240427/libolecf/libolecf_directory_entry.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_property_section.h` & `libolecf-20240427/libolecf/libolecf_property_section.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_directory_tree.h` & `libolecf-20240427/libolecf/libolecf_directory_tree.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_io_handle.h` & `libolecf-20240427/libolecf/libolecf_io_handle.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_notify.c` & `libolecf-20240427/libolecf/libolecf_notify.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_support.h` & `libolecf-20240427/libolecf/libolecf_support.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_libbfio.h` & `libolecf-20240427/libolecf/libolecf_libbfio.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_ole.h` & `libolecf-20240427/libolecf/libolecf_ole.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_types.h` & `libolecf-20240427/libolecf/libolecf_types.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_file.c` & `libolecf-20240427/libolecf/libolecf_file.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_file_header.c` & `libolecf-20240427/libolecf/libolecf_file_header.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_property_set.c` & `libolecf-20240427/libolecf/libolecf_property_set.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/olecf_directory.h` & `libolecf-20240427/libolecf/olecf_directory.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_item.h` & `libolecf-20240427/libolecf/libolecf_item.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_libuna.h` & `libolecf-20240427/libolecf/libolecf_libuna.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/Makefile.am` & `libolecf-20240427/libolecf/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -84,21 +84,19 @@
 libolecf_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libolecf_definitions.h.in \
 	libolecf.rc \
 	libolecf.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libolecf_definitions.h \
+	libolecf.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libolecf_definitions.h
-	-rm -f libolecf.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libolecf ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libolecf_la_SOURCES)
```

### Comparing `libolecf-20240212/libolecf/libolecf_property_set_stream.c` & `libolecf-20240427/libolecf/libolecf_property_set_stream.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_libfole.h` & `libolecf-20240427/libolecf/libolecf_libfole.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_debug.h` & `libolecf-20240427/libolecf/libolecf_debug.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_io_handle.c` & `libolecf-20240427/libolecf/libolecf_io_handle.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_support.c` & `libolecf-20240427/libolecf/libolecf_support.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf.rc` & `libolecf-20240427/libolecf/libolecf.rc.in`

 * *Files 11% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Object Linking and Embedding (OLE) Compound File (CF) format\0"
-      VALUE "FileVersion",		"20240212" "\0"
+      VALUE "FileVersion",		"@VERSION@" "\0"
       VALUE "InternalName",		"libolecf.dll\0"
       VALUE "LegalCopyright",		"(C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libolecf.dll\0"
       VALUE "ProductName",		"libolecf\0"
-      VALUE "ProductVersion",		"20240212" "\0"
+      VALUE "ProductVersion",		"@VERSION@" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libolecf/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libolecf-20240212/libolecf/libolecf_item.c` & `libolecf-20240427/libolecf/libolecf_item.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_libfvalue.h` & `libolecf-20240427/libolecf/libolecf_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_property_value.c` & `libolecf-20240427/libolecf/libolecf_property_value.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_libcnotify.h` & `libolecf-20240427/libolecf/libolecf_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_libfwps.h` & `libolecf-20240427/libolecf/libolecf_libfwps.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_directory_tree.c` & `libolecf-20240427/libolecf/libolecf_directory_tree.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_allocation_table.c` & `libolecf-20240427/libolecf/libolecf_allocation_table.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_directory_list.h` & `libolecf-20240427/libolecf/libolecf_directory_list.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_codepage.h` & `libolecf-20240427/libolecf/libolecf_codepage.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_libfdatetime.h` & `libolecf-20240427/libolecf/libolecf_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_definitions.h` & `libolecf-20240427/libolecf/libolecf_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #if !defined( HAVE_LOCAL_LIBOLECF )
 #include <libolecf/definitions.h>
 
 /* The definitions in <libolecf/definitions.h> are copied here
  * for local use of libolecf
  */
 #else
-#define LIBOLECF_VERSION						20240212
+#define LIBOLECF_VERSION						20240427
 
 /* The version string
  */
-#define LIBOLECF_VERSION_STRING						"20240212"
+#define LIBOLECF_VERSION_STRING						"20240427"
 
 /* The file access flags
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 #define LIBOLECF_ACCESS_FLAG_READ					0x01
```

### Comparing `libolecf-20240212/libolecf/libolecf_definitions.h.in` & `libolecf-20240427/libolecf/libolecf_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_directory_list.c` & `libolecf-20240427/libolecf/libolecf_directory_list.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf.rc.in` & `libolecf-20240427/libolecf/libolecf.rc`

 * *Files 23% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Object Linking and Embedding (OLE) Compound File (CF) format\0"
-      VALUE "FileVersion",		"@VERSION@" "\0"
+      VALUE "FileVersion",		"20240427" "\0"
       VALUE "InternalName",		"libolecf.dll\0"
       VALUE "LegalCopyright",		"(C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libolecf.dll\0"
       VALUE "ProductName",		"libolecf\0"
-      VALUE "ProductVersion",		"@VERSION@" "\0"
+      VALUE "ProductVersion",		"20240427" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libolecf/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libolecf-20240212/libolecf/libolecf_property_set_stream.h` & `libolecf-20240427/libolecf/libolecf_property_set_stream.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/olecf_file_header.h` & `libolecf-20240427/libolecf/olecf_file_header.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/olecf_compound_object.h` & `libolecf-20240427/libolecf/olecf_compound_object.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_error.h` & `libolecf-20240427/libolecf/libolecf_error.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_property_value.h` & `libolecf-20240427/libolecf/libolecf_property_value.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_stream.c` & `libolecf-20240427/libolecf/libolecf_stream.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_compound_object_stream.c` & `libolecf-20240427/libolecf/libolecf_compound_object_stream.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_stream.h` & `libolecf-20240427/libolecf/libolecf_stream.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf.c` & `libolecf-20240427/libolecf/libolecf.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_unused.h` & `libolecf-20240427/libolecf/libolecf_unused.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_libclocale.h` & `libolecf-20240427/libolecf/libolecf_libclocale.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_extern.h` & `libolecf-20240427/libolecf/libolecf_extern.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_allocation_table.h` & `libolecf-20240427/libolecf/libolecf_allocation_table.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_file_header.h` & `libolecf-20240427/libolecf/libolecf_file_header.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/Makefile.in` & `libolecf-20240427/libolecf/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -500,14 +500,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -566,16 +568,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -653,15 +655,18 @@
 
 libolecf_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libolecf_definitions.h.in \
 	libolecf.rc \
 	libolecf.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libolecf_definitions.h \
+	libolecf.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -910,24 +915,45 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libolecf.Plo
+	-rm -f ./$(DEPDIR)/libolecf_allocation_table.Plo
+	-rm -f ./$(DEPDIR)/libolecf_compound_object_stream.Plo
+	-rm -f ./$(DEPDIR)/libolecf_debug.Plo
+	-rm -f ./$(DEPDIR)/libolecf_directory_entry.Plo
+	-rm -f ./$(DEPDIR)/libolecf_directory_list.Plo
+	-rm -f ./$(DEPDIR)/libolecf_directory_tree.Plo
+	-rm -f ./$(DEPDIR)/libolecf_error.Plo
+	-rm -f ./$(DEPDIR)/libolecf_file.Plo
+	-rm -f ./$(DEPDIR)/libolecf_file_header.Plo
+	-rm -f ./$(DEPDIR)/libolecf_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libolecf_item.Plo
+	-rm -f ./$(DEPDIR)/libolecf_notify.Plo
+	-rm -f ./$(DEPDIR)/libolecf_property_section.Plo
+	-rm -f ./$(DEPDIR)/libolecf_property_set.Plo
+	-rm -f ./$(DEPDIR)/libolecf_property_set_stream.Plo
+	-rm -f ./$(DEPDIR)/libolecf_property_value.Plo
+	-rm -f ./$(DEPDIR)/libolecf_stream.Plo
+	-rm -f ./$(DEPDIR)/libolecf_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1029,19 +1055,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libolecf_definitions.h
-	-rm -f libolecf.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libolecf ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libolecf_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libolecf-20240212/libolecf/libolecf_libfguid.h` & `libolecf-20240427/libolecf/libolecf_libfguid.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_libcdata.h` & `libolecf-20240427/libolecf/libolecf_libcdata.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_compound_object_stream.h` & `libolecf-20240427/libolecf/libolecf_compound_object_stream.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_debug.c` & `libolecf-20240427/libolecf/libolecf_debug.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_file.h` & `libolecf-20240427/libolecf/libolecf_file.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_directory_entry.c` & `libolecf-20240427/libolecf/libolecf_directory_entry.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_error.c` & `libolecf-20240427/libolecf/libolecf_error.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf/libolecf_property_set.h` & `libolecf-20240427/libolecf/libolecf_property_set.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/COPYING` & `libolecf-20240427/COPYING`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/install-sh` & `libolecf-20240427/install-sh`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/depcomp` & `libolecf-20240427/depcomp`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfguid/libfguid_error.c` & `libolecf-20240427/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfguid/libfguid_support.h` & `libolecf-20240427/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfguid/libfguid_identifier.h` & `libolecf-20240427/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfguid/libfguid_libcerror.h` & `libolecf-20240427/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfguid/Makefile.am` & `libolecf-20240427/libfguid/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFGUID
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfguid.la
 
 libfguid_la_SOURCES = \
 	libfguid_definitions.h \
 	libfguid_extern.h \
@@ -13,19 +13,17 @@
 	libfguid_libcerror.h \
 	libfguid_identifier.c libfguid_identifier.h \
 	libfguid_support.c libfguid_support.h \
 	libfguid_types.h \
 	libfguid_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
```

### Comparing `libolecf-20240212/libfguid/libfguid_unused.h` & `libolecf-20240427/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfguid/libfguid_extern.h` & `libolecf-20240427/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfguid/libfguid_types.h` & `libolecf-20240427/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfguid/libfguid_identifier.c` & `libolecf-20240427/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfguid/libfguid_support.c` & `libolecf-20240427/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfguid/libfguid_definitions.h` & `libolecf-20240427/libfguid/libfguid_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfguid/definitions.h> are copied here
  * for local use of libfguid
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFGUID_VERSION					20240116
+#define LIBFGUID_VERSION					20240415
 
 /* The version string
  */
-#define LIBFGUID_VERSION_STRING					"20240116"
+#define LIBFGUID_VERSION_STRING					"20240415"
 
 /* The byte order definitions
  */
 #define LIBFGUID_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFGUID_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The GUID identifier version definitions
```

### Comparing `libolecf-20240212/libfguid/Makefile.in` & `libolecf-20240427/libfguid/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -454,14 +454,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -520,30 +522,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFGUID_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFGUID_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFGUID_TRUE@noinst_LTLIBRARIES = libfguid.la
 @HAVE_LOCAL_LIBFGUID_TRUE@libfguid_la_SOURCES = \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_definitions.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_extern.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_error.c libfguid_error.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_libcerror.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_identifier.c libfguid_identifier.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_support.c libfguid_support.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_types.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -745,24 +748,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfguid_error.Plo
+	-rm -f ./$(DEPDIR)/libfguid_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfguid_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -848,17 +856,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libolecf-20240212/libfguid/libfguid_error.h` & `libolecf-20240427/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/m4/libcfile.m4` & `libolecf-20240427/m4/libcfile.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcfile required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcfile is available
 dnl ac_libcfile_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCFILE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno],
     [ac_cv_libcfile=no],
     [ac_cv_libcfile=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcfile which returns "yes" and --with-libcfile= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect],
+      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcfile"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcfile],
           [1])
@@ -199,16 +201,17 @@
             libcfile_file_remove_wide,
             [ac_cv_libcfile_dummy=yes],
             [ac_cv_libcfile=no])
           ])
 
         ac_cv_libcfile_LIBADD="-lcfile"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes],
+      [test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcfile in directory: $ac_cv_with_libcfile],
         [1])
       ])
     ])
 
   AS_IF(
@@ -354,15 +357,15 @@
   AS_IF(
     [test "x$ac_cv_func_unlink" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: unlink],
       [1])
     ])
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
   ])
 
 dnl Function to detect how to enable libcfile
 AC_DEFUN([AX_LIBCFILE_CHECK_ENABLE],
```

### Comparing `libolecf-20240212/m4/libfdatetime.m4` & `libolecf-20240427/m4/libfdatetime.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfdatetime required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfdatetime is available
 dnl ac_libfdatetime_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno],
     [ac_cv_libfdatetime=no],
     [ac_cv_libfdatetime=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdatetime which returns "yes" and --with-libfdatetime= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect],
+      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdatetime"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdatetime],
           [1])
@@ -455,16 +457,17 @@
           fdatetime,
           libfdatetime_systemetime_copy_to_utf32_string_with_index,
           [ac_cv_libfdatetime_dummy=yes],
           [ac_cv_libfdatetime=no])
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes],
+      [test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime],
         [1])
       ])
     ])
 
   AS_IF(
@@ -486,15 +489,15 @@
     ])
   ])
 
 dnl Function to detect if libfdatetime dependencies are available
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
   ])
 
 dnl Function to detect how to enable libfdatetime
 AC_DEFUN([AX_LIBFDATETIME_CHECK_ENABLE],
```

### Comparing `libolecf-20240212/m4/tests.m4` & `libolecf-20240427/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/m4/libcpath.m4` & `libolecf-20240427/m4/libcpath.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcpath required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcpath is available
 dnl ac_libcpath_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCPATH_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno],
     [ac_cv_libcpath=no],
     [ac_cv_libcpath=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcpath which returns "yes" and --with-libcpath= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect],
+      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcpath"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcpath],
           [1])
@@ -148,16 +150,17 @@
             libcpath_path_make_directory_wide,
             [ac_cv_libcpath_dummy=yes],
             [ac_cv_libcpath=no])
           ])
 
         ac_cv_libcpath_LIBADD="-lcpath"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes],
+      [test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcpath in directory: $ac_cv_with_libcpath],
         [1])
       ])
     ])
 
   AS_IF(
@@ -269,15 +272,15 @@
     [AC_MSG_FAILURE(
       [Missing functions: getcwd],
       [1])
     ])
 
   AX_LIBCPATH_CHECK_FUNC_MKDIR
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
   ])
 
 dnl Function to detect how to enable libcpath
 AC_DEFUN([AX_LIBCPATH_CHECK_ENABLE],
```

### Comparing `libolecf-20240212/m4/lib-prefix.m4` & `libolecf-20240427/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/m4/progtest.m4` & `libolecf-20240427/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/m4/libuna.m4` & `libolecf-20240427/m4/libuna.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20230702
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -23,16 +23,18 @@
 dnl ac_libuna_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBUNA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno],
     [ac_cv_libuna=no],
     [ac_cv_libuna=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libuna which returns "yes" and --with-libuna= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect],
+      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libuna"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libuna],
           [1])
@@ -938,16 +940,17 @@
           [ac_cv_libuna_defines_compare_greater])
         AS_IF(
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -969,15 +972,15 @@
     ])
   ])
 
 dnl Function to detect if libuna dependencies are available
 AC_DEFUN([AX_LIBUNA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
   ])
 
 dnl Function to detect how to enable libuna
 AC_DEFUN([AX_LIBUNA_CHECK_ENABLE],
```

### Comparing `libolecf-20240212/m4/gettext.m4` & `libolecf-20240427/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/m4/lib-ld.m4` & `libolecf-20240427/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/m4/libfole.m4` & `libolecf-20240427/m4/libfole.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfole required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfole is available
 dnl ac_libfole_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFOLE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfole" = xno],
     [ac_cv_libfole=no],
     [ac_cv_libfole=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfole which returns "yes" and --with-libfole= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect],
+      [test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect && test "x$ac_cv_with_libfole" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfole"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfole}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfole}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfole],
           [1])
@@ -53,16 +55,17 @@
           [ac_cv_libfole_dummy=yes],
           [ac_cv_libfole=no])
 
         dnl TODO add functions
 
         ac_cv_libfole_LIBADD="-lfole"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect && test "x$ac_cv_libfole" != xyes],
+      [test "x$ac_cv_libfole" != xyes && test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect && test "x$ac_cv_with_libfole" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfole in directory: $ac_cv_with_libfole],
         [1])
       ])
     ])
 
   AS_IF(
@@ -84,15 +87,15 @@
     ])
   ])
 
 dnl Function to detect if libfole dependencies are available
 AC_DEFUN([AX_LIBFOLE_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfole_CPPFLAGS="-I../libfole";
+  ac_cv_libfole_CPPFLAGS="-I../libfole -I\$(top_srcdir)/libfole";
   ac_cv_libfole_LIBADD="../libfole/libfole.la";
 
   ac_cv_libfole=local
   ])
 
 dnl Function to detect how to enable libfole
 AC_DEFUN([AX_LIBFOLE_CHECK_ENABLE],
```

### Comparing `libolecf-20240212/m4/libclocale.m4` & `libolecf-20240427/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
     [ac_cv_libclocale=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libclocale which returns "yes" and --with-libclocale= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect],
+      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libclocale"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libclocale],
           [1])
@@ -122,16 +124,17 @@
           clocale,
           libclocale_initialize,
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -216,15 +219,15 @@
     [AC_MSG_FAILURE(
       [Missing function: setlocale],
       [1])
     ])
 
   AX_LIBCLOCALE_CHECK_FUNC_LANGINFO_CODESET
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
   ])
 
 dnl Function to detect how to enable libclocale
 AC_DEFUN([AX_LIBCLOCALE_CHECK_ENABLE],
```

### Comparing `libolecf-20240212/m4/libcdata.m4` & `libolecf-20240427/m4/libcdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20230108
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
     [ac_cv_libcdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcdata which returns "yes" and --with-libcdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect],
+      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcdata],
           [1])
@@ -493,16 +495,17 @@
           cdata,
           libcdata_tree_node_get_leaf_node_list,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -524,15 +527,15 @@
     ])
   ])
 
 dnl Function to detect if libcdata dependencies are available
 AC_DEFUN([AX_LIBCDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
   ])
 
 dnl Function to detect how to enable libcdata
 AC_DEFUN([AX_LIBCDATA_CHECK_ENABLE],
```

### Comparing `libolecf-20240212/m4/libcsplit.m4` & `libolecf-20240427/m4/libcsplit.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcsplit required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcsplit is available
 dnl ac_libcsplit_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno],
     [ac_cv_libcsplit=no],
     [ac_cv_libcsplit=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcsplit which returns "yes" and --with-libcsplit= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect],
+      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcsplit"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcsplit],
           [1])
@@ -143,16 +145,17 @@
             libcsplit_wide_split_string_set_segment_by_index,
             [ac_cv_libcsplit_dummy=yes],
             [ac_cv_libcsplit=no])
           ])
 
         ac_cv_libcsplit_LIBADD="-lcsplit"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes],
+      [test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcsplit in directory: $ac_cv_with_libcsplit],
         [1])
       ])
     ])
 
   AS_IF(
@@ -174,15 +177,15 @@
     ])
   ])
 
 dnl Function to detect if libcsplit dependencies are available
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
   ])
 
 dnl Function to detect how to enable libcsplit
 AC_DEFUN([AX_LIBCSPLIT_CHECK_ENABLE],
```

### Comparing `libolecf-20240212/m4/common.m4` & `libolecf-20240427/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libolecf-20240212/m4/libcthreads.m4` & `libolecf-20240427/m4/libcthreads.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
     [ac_cv_libcthreads=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcthreads which returns "yes" and --with-libcthreads= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect],
+      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcthreads"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcthreads],
           [1])
@@ -244,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -286,15 +288,15 @@
     [dnl Check for enabling pthread support
     AX_PTHREAD_CHECK_ENABLE
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread],
     [ac_cv_libcthreads_multi_threading="winapi"])
 
   AS_IF(
     [test "x$ac_cv_libcthreads_multi_threading" != xno],
-    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local],
     [ac_cv_libcthreads=no])
   ])
 
 dnl Function to detect how to enable libcthreads
```

### Comparing `libolecf-20240212/m4/ltversion.m4` & `libolecf-20240427/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/m4/ltsugar.m4` & `libolecf-20240427/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/m4/host-cpu-c-abi.m4` & `libolecf-20240427/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/m4/libfwps.m4` & `libolecf-20240427/m4/libfwps.m4`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 dnl Checks for libfwps required headers and functions
 dnl
-dnl Version: 20230711
+dnl Version: 20240413
 
 dnl Function to detect if libfwps is available
 dnl ac_libfwps_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFWPS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfwps" = xno],
     [ac_cv_libfwps=no],
     [ac_cv_libfwps=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfwps which returns "yes" and --with-libfwps= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfwps" != x && test "x$ac_cv_with_libfwps" != xauto-detect],
+      [test "x$ac_cv_with_libfwps" != x && test "x$ac_cv_with_libfwps" != xauto-detect && test "x$ac_cv_with_libfwps" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfwps"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfwps}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfwps}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfwps],
           [1])
         ])
       ],
       [dnl Check for a pkg-config file
       AS_IF(
         [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
         [PKG_CHECK_MODULES(
           [libfwps],
-          [libfwps >= 20230711],
+          [libfwps >= 20240224],
           [ac_cv_libfwps=yes],
           [ac_cv_libfwps=check])
         ])
       AS_IF(
         [test "x$ac_cv_libfwps" = xyes],
         [ac_cv_libfwps_CPPFLAGS="$pkg_cv_libfwps_CFLAGS"
         ac_cv_libfwps_LIBADD="$pkg_cv_libfwps_LIBS"])
@@ -103,25 +105,75 @@
           fwps,
           libfwps_record_free,
           [ac_cv_libfwps_dummy=yes],
           [ac_cv_libfwps=no])
 
         AC_CHECK_LIB(
           fwps,
+          libfwps_record_get_utf8_entry_name_size,
+          [ac_cv_libfwps_dummy=yes],
+          [ac_cv_libfwps=no])
+        AC_CHECK_LIB(
+          fwps,
+          libfwps_record_get_utf8_entry_name,
+          [ac_cv_libfwps_dummy=yes],
+          [ac_cv_libfwps=no])
+        AC_CHECK_LIB(
+          fwps,
+          libfwps_record_get_utf16_entry_name_size,
+          [ac_cv_libfwps_dummy=yes],
+          [ac_cv_libfwps=no])
+        AC_CHECK_LIB(
+          fwps,
+          libfwps_record_get_utf16_entry_name,
+          [ac_cv_libfwps_dummy=yes],
+          [ac_cv_libfwps=no])
+        AC_CHECK_LIB(
+          fwps,
           libfwps_record_get_entry_type,
           [ac_cv_libfwps_dummy=yes],
           [ac_cv_libfwps=no])
         AC_CHECK_LIB(
           fwps,
+          libfwps_record_get_utf8_value_name_size,
+          [ac_cv_libfwps_dummy=yes],
+          [ac_cv_libfwps=no])
+        AC_CHECK_LIB(
+          fwps,
+          libfwps_record_get_utf8_value_name,
+          [ac_cv_libfwps_dummy=yes],
+          [ac_cv_libfwps=no])
+        AC_CHECK_LIB(
+          fwps,
+          libfwps_record_get_utf16_value_name_size,
+          [ac_cv_libfwps_dummy=yes],
+          [ac_cv_libfwps=no])
+        AC_CHECK_LIB(
+          fwps,
+          libfwps_record_get_utf16_value_name,
+          [ac_cv_libfwps_dummy=yes],
+          [ac_cv_libfwps=no])
+        AC_CHECK_LIB(
+          fwps,
           libfwps_record_get_value_type,
           [ac_cv_libfwps_dummy=yes],
           [ac_cv_libfwps=no])
 
         AC_CHECK_LIB(
           fwps,
+          libfwps_record_get_data,
+          [ac_cv_libfwps_dummy=yes],
+          [ac_cv_libfwps=no])
+        AC_CHECK_LIB(
+          fwps,
+          libfwps_record_get_data_size,
+          [ac_cv_libfwps_dummy=yes],
+          [ac_cv_libfwps=no])
+        AC_CHECK_LIB(
+          fwps,
           libfwps_record_get_data_as_boolean,
           [ac_cv_libfwps_dummy=yes],
           [ac_cv_libfwps=no])
         AC_CHECK_LIB(
           fwps,
           libfwps_record_get_data_as_8bit_integer,
           [ac_cv_libfwps_dummy=yes],
@@ -196,15 +248,15 @@
           libfwps_record_get_data_as_guid,
           [ac_cv_libfwps_dummy=yes],
           [ac_cv_libfwps=no])
 
         ac_cv_libfwps_LIBADD="-lfwps"])
       ])
     AS_IF(
-      [test "x$ac_cv_with_libfwps" != x && test "x$ac_cv_with_libfwps" != xauto-detect && test "x$ac_cv_libfwps" != xyes],
+      [test "x$ac_cv_libfwps" != xyes && test "x$ac_cv_with_libfwps" != x && test "x$ac_cv_with_libfwps" != xauto-detect && test "x$ac_cv_with_libfwps" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfwps in directory: $ac_cv_with_libfwps],
         [1])
       ])
     ])
 
   dnl Check for debug functions
@@ -242,15 +294,15 @@
     ])
   ])
 
 dnl Function to detect if libfwps dependencies are available
 AC_DEFUN([AX_LIBFWPS_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfwps_CPPFLAGS="-I../libfwps";
+  ac_cv_libfwps_CPPFLAGS="-I../libfwps -I\$(top_srcdir)/libfwps";
   ac_cv_libfwps_LIBADD="../libfwps/libfwps.la";
 
   ac_cv_libfwps=local
   ])
 
 dnl Function to detect how to enable libfwps
 AC_DEFUN([AX_LIBFWPS_CHECK_ENABLE],
```

### Comparing `libolecf-20240212/m4/libfuse.m4` & `libolecf-20240427/m4/libfuse.m4`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,90 @@
 dnl Checks for libfuse required headers and functions
 dnl
-dnl Version: 20220118
+dnl Version: 20240413
 
 dnl Function to detect if libfuse is available
 dnl ac_libfuse_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFUSE_CHECK_LIB],
-  [dnl Check if parameters were provided
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect],
-    [AS_IF(
-      [test -d "$ac_cv_with_libfuse"],
-      [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
-      [AC_MSG_WARN([no such directory: $ac_cv_with_libfuse])
-      ])
-    ])
-
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" = xno],
+  [AS_IF(
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno],
     [ac_cv_libfuse=no],
-    [dnl Check for a pkg-config file
+    [dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfuse which returns "yes" and --with-libfuse= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
-      [PKG_CHECK_MODULES(
-        [fuse],
-        [fuse >= 2.6],
-        [ac_cv_libfuse=libfuse],
-        [ac_cv_libfuse=no])
+      [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_libfuse"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
+        [AC_MSG_FAILURE(
+          [no such directory: $ac_cv_with_libfuse],
+          [1])
+        ])],
+      [dnl Check for a pkg-config file
+      AS_IF(
+        [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
+        [PKG_CHECK_MODULES(
+          [fuse3],
+          [fuse3 >= 3.0],
+          [ac_cv_libfuse=libfuse3],
+          [ac_cv_libfuse=no])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xno],
+          [PKG_CHECK_MODULES(
+            [fuse],
+            [fuse >= 2.6],
+            [ac_cv_libfuse=libfuse],
+            [ac_cv_libfuse=no])
+          ])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"])
+        ])
       ])
 
+    backup_CPPFLAGS="$CPPFLAGS"
+
+    dnl Check for libfuse and libfuse3
     AS_IF(
-      [test "x$ac_cv_libfuse" = xlibfuse],
-      [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"],
+      [test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3],
       [dnl Check for headers
-      AC_CHECK_HEADERS(
-        [fuse.h],
-        [ac_cv_header_fuse_h=yes],
-        [ac_cv_header_fuse_h=no])
 
-      dnl libfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      dnl macFuse requires -DFUSE_USE_VERSION=26 to be set
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      AC_CHECK_HEADERS([fuse.h])
+
       AS_IF(
-        [test "x$ac_cv_header_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+        [test "x$ac_cv_header_fuse_h" = xyes],
+        [ac_cv_libfuse=libfuse3],
+        [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         AC_CHECK_HEADERS([fuse.h])
-      ])
+
+        AS_IF(
+          [test "x$ac_cv_header_fuse_h" = xyes],
+          [ac_cv_libfuse=libfuse])
+        ])
 
       AS_IF(
         [test "x$ac_cv_header_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
-        ac_cv_libfuse=libfuse
+        AC_CHECK_LIB(
+          fuse,
+          fuse_invalidate,
+          [ac_cv_libfuse=libfuse],
+          [ac_cv_libfuse=libfuse3])
 
         AC_CHECK_LIB(
           fuse,
           fuse_daemonize,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
@@ -71,32 +99,30 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           fuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+        dnl libfuse and libfuse3 require -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_LIBADD="-lfuse3"],
+          [ac_cv_libfuse_LIBADD="-lfuse"])
         ])
       ])
 
     dnl Check for libosxfuse
     AS_IF(
       [test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno],
-      [CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
+      [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
       AC_CHECK_HEADERS([osxfuse/fuse.h])
 
-      dnl libosxfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      AS_IF(
-        [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_osxfuse_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        AC_CHECK_HEADERS([osxfuse/fuse.h])
-      ])
-
       AS_IF(
         [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
         ac_cv_libfuse=libosxfuse
 
         AC_CHECK_LIB(
@@ -116,27 +142,46 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           osxfuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
+        dnl libosxfuse requires -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
         ])
       ])
+
+    AS_IF(
+      [test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported libfuse in directory: $ac_cv_with_libfuse],
+        [1])
+      ])
+
+    CPPFLAGS="$backup_CPPFLAGS"
     ])
 
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_DEFINE(
       [HAVE_LIBFUSE],
       [1],
       [Define to 1 if you have the 'fuse' library (-lfuse).])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_DEFINE(
+      [HAVE_LIBFUSE3],
+      [1],
+      [Define to 1 if you have the 'fuse3' library (-lfuse3).])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_DEFINE(
       [HAVE_LIBOSXFUSE],
       [1],
       [Define to 1 if you have the 'osxfuse' library (-losxfuse).])
     ])
 
@@ -179,14 +224,20 @@
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-lfuse])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_pc_libs_private],
+      [-lfuse3])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-losxfuse])
     ])
 
   AS_IF(
@@ -194,9 +245,18 @@
     [AC_SUBST(
       [ax_libfuse_spec_requires],
       [fuse-libs])
     AC_SUBST(
       [ax_libfuse_spec_build_requires],
       [fuse-devel])
     ])
+  AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_spec_requires],
+      [fuse3-libs])
+    AC_SUBST(
+      [ax_libfuse_spec_build_requires],
+      [fuse3-devel])
+    ])
   ])
```

### Comparing `libolecf-20240212/m4/libtool.m4` & `libolecf-20240427/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/m4/po.m4` & `libolecf-20240427/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/m4/libcerror.m4` & `libolecf-20240427/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libolecf-20240212/m4/libcnotify.m4` & `libolecf-20240427/m4/libcnotify.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
     [ac_cv_libcnotify=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcnotify which returns "yes" and --with-libcnotify= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect],
+      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcnotify"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcnotify],
           [1])
@@ -92,16 +94,17 @@
           cnotify,
           libcnotify_verbose_set,
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
       [Missing headers: stdarg.h and varargs.h],
       [1])
     ])
 
   dnl Headers included in libcnotify/libcnotify_stream.c
   AC_CHECK_HEADERS([errno.h])
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
   ])
 
 dnl Function to detect how to enable libcnotify
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_ENABLE],
```

### Comparing `libolecf-20240212/m4/libfguid.m4` & `libolecf-20240427/m4/libfguid.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfguid required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfguid is available
 dnl ac_libfguid_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFGUID_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno],
     [ac_cv_libfguid=no],
     [ac_cv_libfguid=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfguid which returns "yes" and --with-libfguid= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect],
+      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfguid"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfguid],
           [1])
@@ -103,16 +105,17 @@
           fguid,
           libfguid_identifier_copy_to_utf32_string_with_index,
           [ac_cv_libfguid_dummy=yes],
           [ac_cv_libfguid=no])
 
         ac_cv_libfguid_LIBADD="-lfguid"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes],
+      [test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfguid in directory: $ac_cv_with_libfguid],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
     ])
   ])
 
 dnl Function to detect if libfguid dependencies are available
 AC_DEFUN([AX_LIBFGUID_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
   ])
 
 
 dnl Function to detect how to enable libfguid
```

### Comparing `libolecf-20240212/m4/libbfio.m4` & `libolecf-20240427/m4/libbfio.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libbfio required headers and functions
 dnl
-dnl Version: 20201125
+dnl Version: 20240413
 
 dnl Function to detect if libbfio is available
 dnl ac_libbfio_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBBFIO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno],
     [ac_cv_libbfio=no],
     [ac_cv_libbfio=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libbfio which returns "yes" and --with-libbfio= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect],
+      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libbfio"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libbfio],
           [1])
@@ -316,16 +318,17 @@
             libbfio_file_pool_open_wide,
             [ac_cv_libbfio_dummy=yes],
             [ac_cv_libbfio=no])
           ])
 
         ac_cv_libbfio_LIBADD="-lbfio"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes],
+      [test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libbfio in directory: $ac_cv_with_libbfio],
         [1])
       ])
     ])
 
   AS_IF(
@@ -347,15 +350,15 @@
     ])
   ])
 
 dnl Function to detect if libbfio dependencies are available
 AC_DEFUN([AX_LIBBFIO_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
   ])
 
 dnl Function to detect how to enable libbfio
 AC_DEFUN([AX_LIBBFIO_CHECK_ENABLE],
```

### Comparing `libolecf-20240212/m4/intlmacosx.m4` & `libolecf-20240427/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/m4/lt~obsolete.m4` & `libolecf-20240427/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/m4/lib-link.m4` & `libolecf-20240427/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/m4/iconv.m4` & `libolecf-20240427/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/m4/ltoptions.m4` & `libolecf-20240427/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/m4/nls.m4` & `libolecf-20240427/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/m4/python.m4` & `libolecf-20240427/m4/python.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20231119
+dnl Version: 20240418
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -72,18 +72,20 @@
     PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
-    dnl For CygWin add the -no-undefined linker flag
+    dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
-      [$host_os],
-      [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [$build],
+      [*-*-cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-msys*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
       [*],[])
 
     dnl Check for the existence of Python.h
     BACKUP_CPPFLAGS="${CPPFLAGS}"
     CPPFLAGS="${CPPFLAGS} ${PYTHON_INCLUDES}"
 
     AC_CHECK_HEADERS(
```

### Comparing `libolecf-20240212/m4/libfvalue.m4` & `libolecf-20240427/m4/libfvalue.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfvalue required headers and functions
 dnl
-dnl Version: 20200711
+dnl Version: 20240413
 
 dnl Function to detect if libfvalue is available
 dnl ac_libfvalue_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFVALUE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfvalue" = xno],
     [ac_cv_libfvalue=no],
     [ac_cv_libfvalue=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfvalue which returns "yes" and --with-libfvalue= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect],
+      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfvalue"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfvalue}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfvalue}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfvalue],
           [1])
@@ -585,16 +587,17 @@
           fvalue,
           libfvalue_value_type_set_data_strings_array,
           [ac_cv_libfvalue_dummy=yes],
           [ac_cv_libfvalue=no])
 
         ac_cv_libfvalue_LIBADD="-lfvalue"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_libfvalue" != xyes],
+      [test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfvalue in directory: $ac_cv_with_libfvalue],
         [1])
       ])
     ])
 
   AS_IF(
@@ -616,15 +619,15 @@
     ])
   ])
 
 dnl Function to detect if libfvalue dependencies are available
 AC_DEFUN([AX_LIBFVALUE_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
   ])
 
 dnl Function to detect how to enable libfvalue
 AC_DEFUN([AX_LIBFVALUE_CHECK_ENABLE],
```

### Comparing `libolecf-20240212/m4/types.m4` & `libolecf-20240427/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/m4/pthread.m4` & `libolecf-20240427/m4/pthread.m4`

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,196 @@
 dnl Functions for pthread
 dnl
-dnl Version: 20130509
+dnl Version: 20240308
 
 dnl Function to detect if pthread is available
 AC_DEFUN([AX_PTHREAD_CHECK_LIB],
- [dnl Check if parameters were provided
- AS_IF(
-  [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect],
   [AS_IF(
-   [test -d "$ac_cv_with_pthread"],
-   [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
-   [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
-   ])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_with_pthread" = xno],
-  [ac_cv_pthread=no],
-  [dnl Check for headers
-  AC_CHECK_HEADERS([pthread.h])
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno],
+    [ac_cv_pthread=no],
+    [ac_cv_pthread=check
+    dnl Check if parameters were provided
+    dnl For both --with-pthread which returns "yes" and --with-pthread= which returns ""
+    dnl treat them as auto-detection.
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_pthread"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
+        [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
+        ])
+      ])
+    ])
+
+    AS_IF(
+      [test "x$ac_cv_pthread" = xcheck],
+      [dnl Check for headers
+      AC_CHECK_HEADERS([pthread.h])
+
+      AS_IF(
+        [test "x$ac_cv_header_pthread_h" = xno],
+        [ac_cv_pthread=no],
+        [dnl Check for the individual functions
+        ac_cv_pthread=pthread
+
+        dnl Thread functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_create,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_exit,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_join,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Condition functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_broadcast,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_signal,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_wait,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Mutex functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_lock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_trylock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Read/Write lock functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_rdlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_wrlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        ac_cv_pthread_LIBADD="-lpthread";
+      ])
+
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported pthread in directory: $ac_cv_with_pthread],
+        [1])
+      ])
+    ])
 
   AS_IF(
-   [test "x$ac_cv_header_pthread_h" = xno],
-   [ac_cv_pthread=no],
-   [dnl Check for the individual functions
-   ac_cv_pthread=pthread
-
-   dnl Thread functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_create,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_exit,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_join,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Condition functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_broadcast,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_signal,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_wait,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Mutex functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_lock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_trylock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Read/Write lock functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_rdlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_wrlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   ac_cv_pthread_LIBADD="-lpthread";
-   ])
-  ])
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_DEFINE(
+      [HAVE_PTHREAD],
+      [1],
+      [Define to 1 if you have the 'pthread' library (-lpthread).])
+    ])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_DEFINE(
-   [HAVE_PTHREAD],
-   [1],
-   [Define to 1 if you have the 'pthread' library (-lpthread).])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_pthread" != xno],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [1]) ],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [0])
+  AS_IF(
+    [test "x$ac_cv_pthread" != xno],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [1]) ],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [0])
+    ])
   ])
- ])
 
 dnl Function to detect how to enable pthread
 AC_DEFUN([AX_PTHREAD_CHECK_ENABLE],
- [AX_COMMON_ARG_WITH(
-  [pthread],
-  [pthread],
-  [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
-  [auto-detect],
-  [DIR])
-
- dnl Check for a shared library version
- AX_PTHREAD_CHECK_LIB
-
- AS_IF(
-  [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
-  [AC_SUBST(
-   [PTHREAD_CPPFLAGS],
-   [$ac_cv_pthread_CPPFLAGS])
-  ])
- AS_IF(
-  [test "x$ac_cv_pthread_LIBADD" != "x"],
-  [AC_SUBST(
-   [PTHREAD_LIBADD],
-   [$ac_cv_pthread_LIBADD])
-  ])
+  [AX_COMMON_ARG_WITH(
+    [pthread],
+    [pthread],
+    [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
+    [auto-detect],
+    [DIR])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_SUBST(
-   [ax_pthread_pc_libs_private],
-   [-lpthread])
+  dnl Check for a shared library version
+  AX_PTHREAD_CHECK_LIB
+
+  AS_IF(
+    [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
+    [AC_SUBST(
+      [PTHREAD_CPPFLAGS],
+      [$ac_cv_pthread_CPPFLAGS])
+    ])
+  AS_IF(
+    [test "x$ac_cv_pthread_LIBADD" != "x"],
+    [AC_SUBST(
+      [PTHREAD_LIBADD],
+      [$ac_cv_pthread_LIBADD])
+    ])
+
+  AS_IF(
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_SUBST(
+      [ax_pthread_pc_libs_private],
+      [-lpthread])
+    ])
   ])
- ])
```

### Comparing `libolecf-20240212/include/libolecf/definitions.h.in` & `libolecf-20240427/include/libolecf/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/include/libolecf/definitions.h` & `libolecf-20240427/include/libolecf/definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBOLECF_DEFINITIONS_H )
 #define _LIBOLECF_DEFINITIONS_H
 
 #include <libolecf/types.h>
 
-#define LIBOLECF_VERSION						20240212
+#define LIBOLECF_VERSION						20240427
 
 /* The version string
  */
-#define LIBOLECF_VERSION_STRING						"20240212"
+#define LIBOLECF_VERSION_STRING						"20240427"
 
 /* The file access flags
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 #define LIBOLECF_ACCESS_FLAG_READ					0x01
```

### Comparing `libolecf-20240212/include/libolecf/types.h.in` & `libolecf-20240427/include/libolecf/types.h.in`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/include/libolecf/types.h` & `libolecf-20240427/include/libolecf/types.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/include/libolecf/features.h.in` & `libolecf-20240427/include/libolecf/features.h.in`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/include/libolecf/error.h` & `libolecf-20240427/include/libolecf/error.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/include/libolecf/extern.h` & `libolecf-20240427/include/libolecf/extern.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/include/libolecf/features.h` & `libolecf-20240427/include/libolecf/features.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/include/libolecf/ole.h` & `libolecf-20240427/include/libolecf/ole.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/include/libolecf/codepage.h` & `libolecf-20240427/include/libolecf/codepage.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/include/libolecf.h` & `libolecf-20240427/include/libolecf.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/include/libolecf.h.in` & `libolecf-20240427/include/libolecf.h.in`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/include/Makefile.in` & `libolecf-20240427/include/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -444,14 +444,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -527,15 +529,20 @@
 
 EXTRA_DIST = \
 	libolecf.h.in \
 	libolecf/definitions.h.in \
 	libolecf/features.h.in \
 	libolecf/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libolecf.h \
+	libolecf/definitions.h \
+	libolecf/features.h \
+	libolecf/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -732,23 +739,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -830,17 +839,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libolecf.h
-	-rm -f libolecf/definitions.h
-	-rm -f libolecf/features.h
-	-rm -f libolecf/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libolecf-20240212/libfwps/libfwps_set.h` & `libolecf-20240427/libfwps/libfwps_set.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfwps/libfwps_types.h` & `libolecf-20240427/libfwps/libfwps_types.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfwps/libfwps_libfguid.h` & `libolecf-20240427/libfwps/libfwps_libfguid.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfwps/libfwps_libcerror.h` & `libolecf-20240427/libfwps/libfwps_libcerror.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfwps/libfwps_libcnotify.h` & `libolecf-20240427/tests/olecf_test_libcnotify.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * The internal libcnotify header
+ * The libcnotify header wrapper
  *
- * Copyright (C) 2013-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFWPS_LIBCNOTIFY_H )
-#define _LIBFWPS_LIBCNOTIFY_H
+#if !defined( _OLECF_TEST_LIBCNOTIFY_H )
+#define _OLECF_TEST_LIBCNOTIFY_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCNOTIFY for local use of libcnotify
  */
 #if defined( HAVE_LOCAL_LIBCNOTIFY )
 
@@ -40,11 +40,11 @@
  */
 #if defined( _WIN32 ) && defined( DLL_IMPORT )
 #define LIBCNOTIFY_DLL_IMPORT
 #endif
 
 #include <libcnotify.h>
 
-#endif
+#endif /* defined( HAVE_LOCAL_LIBCNOTIFY ) */
 
-#endif
+#endif /* !defined( _OLECF_TEST_LIBCNOTIFY_H ) */
```

### Comparing `libolecf-20240212/libfwps/libfwps_store.h` & `libolecf-20240427/libfwps/libfwps_store.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfwps/libfwps_libcdata.h` & `libolecf-20240427/libfwps/libfwps_libcdata.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfwps/libfwps_error.c` & `libolecf-20240427/libfwps/libfwps_error.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfwps/Makefile.am` & `libolecf-20240427/libfwps/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 if HAVE_LOCAL_LIBFWPS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfwps.la
 
 libfwps_la_SOURCES = \
 	libfwps_codepage.h \
+	libfwps_debug.c libfwps_debug.h \
 	libfwps_definitions.h \
 	libfwps_extern.h \
 	libfwps_error.c libfwps_error.h \
 	libfwps_format_class_identifier.c libfwps_format_class_identifier.h \
 	libfwps_libcdata.h \
 	libfwps_libcerror.h \
 	libfwps_libcnotify.h \
 	libfwps_libfguid.h \
 	libfwps_libuna.h \
+	libfwps_notify.c libfwps_notify.h \
 	libfwps_property_identifier.c libfwps_property_identifier.h \
 	libfwps_record.c libfwps_record.h \
 	libfwps_set.c libfwps_set.h \
 	libfwps_store.c libfwps_store.h \
 	libfwps_support.c libfwps_support.h \
 	libfwps_types.h \
 	libfwps_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwps ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwps_la_SOURCES)
```

### Comparing `libolecf-20240212/libfwps/libfwps_definitions.h` & `libolecf-20240427/libfwps/libfwps_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfwps/definitions.h> are copied here
  * for local use of libfwps
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFWPS_VERSION					20240120
+#define LIBFWPS_VERSION					20240417
 
 /* The version string
  */
-#define LIBFWPS_VERSION_STRING				"20240120"
+#define LIBFWPS_VERSION_STRING				"20240417"
 
 /* The byte order definitions
  */
 #define LIBFWPS_ENDIAN_BIG				_BYTE_STREAM_ENDIAN_BIG
 #define LIBFWPS_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The value types
```

### Comparing `libolecf-20240212/libfwps/libfwps_error.h` & `libolecf-20240427/libfwps/libfwps_error.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfwps/libfwps_libuna.h` & `libolecf-20240427/libfwps/libfwps_libuna.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfwps/libfwps_support.h` & `libolecf-20240427/libfwps/libfwps_support.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfwps/libfwps_format_class_identifier.c` & `libolecf-20240427/libfwps/libfwps_format_class_identifier.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfwps/libfwps_codepage.h` & `libolecf-20240427/libfwps/libfwps_codepage.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfwps/libfwps_support.c` & `libolecf-20240427/libfwps/libfwps_support.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfwps/libfwps_extern.h` & `libolecf-20240427/libfwps/libfwps_extern.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfwps/libfwps_store.c` & `libolecf-20240427/libfwps/libfwps_store.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfwps/libfwps_property_identifier.h` & `libolecf-20240427/libfwps/libfwps_property_identifier.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfwps/libfwps_format_class_identifier.h` & `libolecf-20240427/libfwps/libfwps_format_class_identifier.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfwps/libfwps_property_identifier.c` & `libolecf-20240427/libfwps/libfwps_property_identifier.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfwps/libfwps_record.h` & `libolecf-20240427/libfwps/libfwps_record.h`

 * *Files 23% similar despite different names*

```diff
@@ -41,18 +41,34 @@
 	 */
 	uint8_t type;
 
 	/* The size
 	 */
 	uint32_t size;
 
+	/* The entry name
+	 */
+	uint8_t *entry_name;
+
+	/* The entry name size
+	 */
+	uint32_t entry_name_size;
+
 	/* The entry type
 	 */
 	uint32_t entry_type;
 
+	/* The value name
+	 */
+	uint8_t *value_name;
+
+	/* The value name size
+	 */
+	uint32_t value_name_size;
+
 	/* The value type
 	 */
 	uint32_t value_type;
 
 	/* The value data
 	 */
 	uint8_t *value_data;
@@ -84,26 +100,91 @@
      libfwps_record_t *record,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      int ascii_codepage,
      libcerror_error_t **error );
 
 LIBFWPS_EXTERN \
+int libfwps_record_get_utf8_entry_name_size(
+     libfwps_record_t *record,
+     size_t *utf8_string_size,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
+int libfwps_record_get_utf8_entry_name(
+     libfwps_record_t *record,
+     uint8_t *utf8_string,
+     size_t utf8_string_size,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
+int libfwps_record_get_utf16_entry_name_size(
+     libfwps_record_t *record,
+     size_t *utf16_string_size,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
+int libfwps_record_get_utf16_entry_name(
+     libfwps_record_t *record,
+     uint16_t *utf16_string,
+     size_t utf16_string_size,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
 int libfwps_record_get_entry_type(
      libfwps_record_t *record,
      uint32_t *entry_type,
      libcerror_error_t **error );
 
 LIBFWPS_EXTERN \
+int libfwps_record_get_utf8_value_name_size(
+     libfwps_record_t *record,
+     size_t *utf8_string_size,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
+int libfwps_record_get_utf8_value_name(
+     libfwps_record_t *record,
+     uint8_t *utf8_string,
+     size_t utf8_string_size,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
+int libfwps_record_get_utf16_value_name_size(
+     libfwps_record_t *record,
+     size_t *utf16_string_size,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
+int libfwps_record_get_utf16_value_name(
+     libfwps_record_t *record,
+     uint16_t *utf16_string,
+     size_t utf16_string_size,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
 int libfwps_record_get_value_type(
      libfwps_record_t *record,
      uint32_t *value_type,
      libcerror_error_t **error );
 
 LIBFWPS_EXTERN \
+int libfwps_record_get_data_size(
+     libfwps_record_t *record,
+     size_t *data_size,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
+int libfwps_record_get_data(
+     libfwps_record_t *record,
+     uint8_t *data,
+     size_t data_size,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_boolean(
      libfwps_record_t *record,
      uint8_t *value_boolean,
      libcerror_error_t **error );
 
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_8bit_integer(
@@ -126,14 +207,20 @@
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_64bit_integer(
      libfwps_record_t *record,
      uint64_t *value_64bit,
      libcerror_error_t **error );
 
 LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_floatingtime(
+     libfwps_record_t *record,
+     uint64_t *floatingtime,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_filetime(
      libfwps_record_t *record,
      uint64_t *filetime,
      libcerror_error_t **error );
 
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_floating_point(
```

### Comparing `libolecf-20240212/libfwps/libfwps_record.c` & `libolecf-20240427/libfwps/libfwps_record.c`

 * *Files 18% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 #include <byte_stream.h>
 #include <memory.h>
 #include <narrow_string.h>
 #include <system_string.h>
 #include <types.h>
 #include <wide_string.h>
 
+#include "libfwps_debug.h"
 #include "libfwps_definitions.h"
 #include "libfwps_libcerror.h"
 #include "libfwps_libcnotify.h"
 #include "libfwps_libuna.h"
 #include "libfwps_record.h"
 #include "libfwps_types.h"
 
@@ -168,14 +169,24 @@
 		 "%s: invalid internal record.",
 		 function );
 
 		return( -1 );
 	}
 	if( *internal_record != NULL )
 	{
+		if( ( *internal_record )->entry_name != NULL )
+		{
+			memory_free(
+			 ( *internal_record )->entry_name );
+		}
+		if( ( *internal_record )->value_name != NULL )
+		{
+			memory_free(
+			 ( *internal_record )->value_name );
+		}
 		if( ( *internal_record )->value_data != NULL )
 		{
 			memory_free(
 			 ( *internal_record )->value_data );
 		}
 		memory_free(
 		 *internal_record );
@@ -195,19 +206,22 @@
      int ascii_codepage,
      libcerror_error_t **error )
 {
 	libfwps_internal_record_t *internal_record = NULL;
 	static char *function                      = "libfwps_record_copy_from_byte_stream";
 	size_t byte_stream_offset                  = 0;
 	uint32_t name_size                         = 0;
+	uint32_t number_of_values                  = 0;
+	uint32_t value_index                       = 0;
+	uint32_t vector_value_data_size            = 0;
+	uint16_t value_16bit                       = 0;
+	int has_variable_data_size                 = 0;
 
 #if defined( HAVE_DEBUG_OUTPUT )
 	system_character_t *value_string           = NULL;
-	size_t value_string_size                   = 0;
-	int result                                 = 0;
 #endif
 
 	if( record == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
@@ -215,14 +229,36 @@
 		 "%s: invalid record.",
 		 function );
 
 		return( -1 );
 	}
 	internal_record = (libfwps_internal_record_t *) record;
 
+	if( internal_record->entry_name != NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_ALREADY_SET,
+		 "%s: invalid record - entry name already set.",
+		 function );
+
+		return( -1 );
+	}
+	if( internal_record->value_name != NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_ALREADY_SET,
+		 "%s: invalid record - value name already set.",
+		 function );
+
+		return( -1 );
+	}
 	if( internal_record->value_data != NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_VALUE_ALREADY_SET,
 		 "%s: invalid record - value data already set.",
@@ -334,105 +370,64 @@
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
 			 "%s: invalid name size value out of bounds.",
 			 function );
 
 			goto on_error;
 		}
-#if defined( HAVE_DEBUG_OUTPUT )
-		if( libcnotify_verbose != 0 )
-		{
-#if defined( HAVE_WIDE_SYSTEM_CHARACTER )
-			result = libuna_utf16_string_size_from_utf16_stream(
-				  &( byte_stream[ byte_stream_offset ] ),
-				  name_size,
-				  LIBUNA_ENDIAN_LITTLE,
-				  &value_string_size,
-				  error );
-#else
-			result = libuna_utf8_string_size_from_utf16_stream(
-				  &( byte_stream[ byte_stream_offset ] ),
-				  name_size,
-				  LIBUNA_ENDIAN_LITTLE,
-				  &value_string_size,
-				  error );
-#endif
-			if( result != 1 )
-			{
-				libcerror_error_set(
-				 error,
-				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-				 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-				 "%s: unable to determine size of URI string.",
-				 function );
+		internal_record->entry_name = (uint8_t *) memory_allocate(
+		                                           sizeof( uint8_t ) * name_size );
 
-				goto on_error;
-			}
-			if( value_string_size > (size_t) ( SSIZE_MAX / sizeof( system_character_t ) ) )
-			{
-				libcerror_error_set(
-				 error,
-				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-				 LIBCERROR_RUNTIME_ERROR_VALUE_EXCEEDS_MAXIMUM,
-				 "%s: invalid URI string size value exceeds maximum.",
-				 function );
+		if( internal_record->entry_name == NULL )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_MEMORY,
+			 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
+			 "%s: unable to create entry name.",
+			 function );
 
-				goto on_error;
-			}
-			value_string = system_string_allocate(
-					value_string_size );
+			goto on_error;
+		}
+		if( memory_copy(
+		     internal_record->entry_name,
+		     &( byte_stream[ byte_stream_offset ] ),
+		     name_size ) == NULL )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_MEMORY,
+			 LIBCERROR_MEMORY_ERROR_COPY_FAILED,
+			 "%s: unable to copy entry name data.",
+			 function );
 
-			if( value_string == NULL )
-			{
-				libcerror_error_set(
-				 error,
-				 LIBCERROR_ERROR_DOMAIN_MEMORY,
-				 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
-				 "%s: unable to create URI string.",
-				 function );
+			goto on_error;
+		}
+		internal_record->entry_name_size = name_size;
 
-				goto on_error;
-			}
-#if defined( HAVE_WIDE_SYSTEM_CHARACTER )
-			result = libuna_utf16_string_copy_from_utf16_stream(
-				  (libuna_utf16_character_t *) value_string,
-				  value_string_size,
-				  &( byte_stream[ byte_stream_offset ] ),
-				  name_size,
-				  LIBUNA_ENDIAN_LITTLE,
-				  error );
-#else
-			result = libuna_utf8_string_copy_from_utf16_stream(
-				  (libuna_utf8_character_t *) value_string,
-				  value_string_size,
-				  &( byte_stream[ byte_stream_offset ] ),
-				  name_size,
-				  LIBUNA_ENDIAN_LITTLE,
-				  error );
-#endif
-			if( result != 1 )
+#if defined( HAVE_DEBUG_OUTPUT )
+		if( libcnotify_verbose != 0 )
+		{
+			if( libfwps_debug_print_utf16_string_value(
+			     function,
+			     "entry name\t\t\t",
+			     internal_record->entry_name,
+			     internal_record->entry_name_size,
+			     LIBUNA_ENDIAN_LITTLE,
+			     error ) != 1 )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-				 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
-				 "%s: unable to set URI string.",
+				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+				 "%s: unable to print UTF-16 string value.",
 				 function );
 
 				goto on_error;
 			}
-			libcnotify_printf(
-			 "%s: name\t\t\t\t: %" PRIs_SYSTEM "\n",
-			 function,
-			 value_string );
-
-			memory_free(
-			 value_string );
-
-			value_string = NULL;
 		}
 #endif /* defined( HAVE_DEBUG_OUTPUT ) */
 
 		byte_stream_offset += name_size;
 	}
 	if( byte_stream_offset > ( byte_stream_size - 4 ) )
 	{
@@ -451,166 +446,488 @@
 
 	byte_stream_offset += 4;
 
 #if defined( HAVE_DEBUG_OUTPUT )
 	if( libcnotify_verbose != 0 )
 	{
 		libcnotify_printf(
-		 "%s: value type\t\t\t: %" PRIu32 "\n",
+		 "%s: value type\t\t\t: 0x%04" PRIx32 "\n",
 		 function,
 		 internal_record->value_type );
 	}
 #endif
-	switch( internal_record->value_type )
+	/* TODO add support for VT_ARRAY and VT_BYREF
+	 */
+	switch( internal_record->value_type & 0xffffefffUL )
 	{
+		case LIBFWPS_VALUE_TYPE_NULL:
+			internal_record->value_data_size = 0;
+			break;
+
 		case LIBFWPS_VALUE_TYPE_BOOLEAN:
 		case LIBFWPS_VALUE_TYPE_INTEGER_8BIT_SIGNED:
 		case LIBFWPS_VALUE_TYPE_INTEGER_8BIT_UNSIGNED:
 			internal_record->value_data_size = 1;
 			break;
 
 		case LIBFWPS_VALUE_TYPE_INTEGER_16BIT_SIGNED:
 		case LIBFWPS_VALUE_TYPE_INTEGER_16BIT_UNSIGNED:
 			internal_record->value_data_size = 2;
 			break;
 
+		case LIBFWPS_VALUE_TYPE_ERROR:
 		case LIBFWPS_VALUE_TYPE_FLOAT_32BIT:
 		case LIBFWPS_VALUE_TYPE_INTEGER_32BIT_SIGNED:
 		case LIBFWPS_VALUE_TYPE_INTEGER_32BIT_UNSIGNED:
+		case LIBFWPS_VALUE_TYPE_INTEGER_SIGNED:
+		case LIBFWPS_VALUE_TYPE_INTEGER_UNSIGNED:
 			internal_record->value_data_size = 4;
 			break;
 
+		case LIBFWPS_VALUE_TYPE_APPLICATION_TIME:
 		case LIBFWPS_VALUE_TYPE_CURRENCY:
 		case LIBFWPS_VALUE_TYPE_DOUBLE_64BIT:
 		case LIBFWPS_VALUE_TYPE_FILETIME:
 		case LIBFWPS_VALUE_TYPE_INTEGER_64BIT_SIGNED:
 		case LIBFWPS_VALUE_TYPE_INTEGER_64BIT_UNSIGNED:
 			internal_record->value_data_size = 8;
 			break;
 
 		case LIBFWPS_VALUE_TYPE_FIXED_POINT_128BIT:
 		case LIBFWPS_VALUE_TYPE_GUID:
 			internal_record->value_data_size = 16;
 			break;
 
+		case LIBFWPS_VALUE_TYPE_BINARY_DATA:
 		case LIBFWPS_VALUE_TYPE_BINARY_STRING:
+		case LIBFWPS_VALUE_TYPE_STREAM:
 		case LIBFWPS_VALUE_TYPE_STRING_ASCII:
 		case LIBFWPS_VALUE_TYPE_STRING_UNICODE:
-			internal_record->value_data_size = 0;
+			has_variable_data_size = 1;
 			break;
 
 		default:
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-			 "%s: invalid record entry - unsupported value type.",
-			 function );
+			 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
+			 function,
+			 internal_record->value_type );
 
 			goto on_error;
 	}
-	if( internal_record->value_data_size == 0 )
+	if( internal_record->value_type == LIBFWPS_VALUE_TYPE_STREAM )
 	{
 		if( byte_stream_offset > ( byte_stream_size - 4 ) )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 			 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
 			 "%s: invalid byte stream size value too small.",
 			 function );
 
 			goto on_error;
 		}
 		byte_stream_copy_to_uint32_little_endian(
 		 &( byte_stream[ byte_stream_offset ] ),
-		 internal_record->value_data_size );
+		 name_size );
 
 		byte_stream_offset += 4;
 
-		if( internal_record->value_type == LIBFWPS_VALUE_TYPE_STRING_UNICODE )
-		{
-			internal_record->value_data_size *= 2;
-		}
-	}
-#if defined( HAVE_DEBUG_OUTPUT )
-	if( libcnotify_verbose != 0 )
-	{
-		libcnotify_printf(
-		 "%s: value data size\t\t\t: %" PRIu32 "\n",
-		 function,
-		 internal_record->value_data_size );
-	}
-#endif
-	if( internal_record->value_data_size > 0 )
-	{
-		if( ( internal_record->value_data_size > byte_stream_size )
-		 || ( byte_stream_offset > ( byte_stream_size - internal_record->value_data_size ) ) )
+		if( ( name_size > byte_stream_size )
+		 || ( byte_stream_offset > ( byte_stream_size - name_size ) ) )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
-			 "%s: invalid valud data size value out of bounds.",
+			 "%s: invalid name size value out of bounds.",
 			 function );
 
 			goto on_error;
 		}
-#if defined( HAVE_DEBUG_OUTPUT )
-		if( libcnotify_verbose != 0 )
+		internal_record->value_name = (uint8_t *) memory_allocate(
+		                                           sizeof( uint8_t ) * name_size );
+
+		if( internal_record->value_name == NULL )
 		{
-			libcnotify_printf(
-			 "%s: value data:\n",
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_MEMORY,
+			 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
+			 "%s: unable to create value name.",
 			 function );
-			libcnotify_print_data(
-			 &( byte_stream[ byte_stream_offset ] ),
-			 internal_record->value_data_size,
-			 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
+
+			goto on_error;
 		}
-#endif
-		if( internal_record->value_data_size > MEMORY_MAXIMUM_ALLOCATION_SIZE )
+		if( memory_copy(
+		     internal_record->value_name,
+		     &( byte_stream[ byte_stream_offset ] ),
+		     name_size ) == NULL )
 		{
 			libcerror_error_set(
 			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_VALUE_EXCEEDS_MAXIMUM,
-			 "%s: invalid value data size value exceeds maximum.",
+			 LIBCERROR_ERROR_DOMAIN_MEMORY,
+			 LIBCERROR_MEMORY_ERROR_COPY_FAILED,
+			 "%s: unable to copy value name data.",
 			 function );
 
 			goto on_error;
 		}
-		internal_record->value_data = (uint8_t *) memory_allocate(
-		                                           sizeof( uint8_t ) * internal_record->value_data_size );
+		internal_record->value_name_size = name_size;
+
+#if defined( HAVE_DEBUG_OUTPUT )
+		if( libcnotify_verbose != 0 )
+		{
+			if( libfwps_debug_print_utf16_string_value(
+			     function,
+			     "value name\t\t\t",
+			     internal_record->value_name,
+			     internal_record->value_name_size,
+			     LIBUNA_ENDIAN_LITTLE,
+			     error ) != 1 )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+				 "%s: unable to print UTF-16 string value.",
+				 function );
+
+				goto on_error;
+			}
+		}
+#endif /* defined( HAVE_DEBUG_OUTPUT ) */
+
+		byte_stream_offset += name_size;
 
-		if( internal_record->value_data == NULL )
+		if( byte_stream_offset > ( byte_stream_size - 2 ) )
 		{
 			libcerror_error_set(
 			 error,
-			 LIBCERROR_ERROR_DOMAIN_MEMORY,
-			 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
-			 "%s: unable to create value data.",
+			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+			 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+			 "%s: invalid byte stream size value too small.",
 			 function );
 
 			goto on_error;
 		}
-		if( memory_copy(
-		     internal_record->value_data,
-		     &( byte_stream[ byte_stream_offset ] ),
-		     internal_record->value_data_size ) == NULL )
+#if defined( HAVE_DEBUG_OUTPUT )
+		if( libcnotify_verbose != 0 )
+		{
+			byte_stream_copy_to_uint16_little_endian(
+			 &( byte_stream[ byte_stream_offset ] ),
+			 value_16bit );
+			libcnotify_printf(
+			 "%s: unknown1\t\t\t\t: 0x%04" PRIx16 "\n",
+			 function,
+			 value_16bit );
+		}
+#endif
+		byte_stream_offset += 2;
+	}
+	if( ( internal_record->value_type & 0x0000f000UL ) == 0x00001000UL )
+	{
+		if( byte_stream_offset > ( byte_stream_size - 4 ) )
 		{
 			libcerror_error_set(
 			 error,
-			 LIBCERROR_ERROR_DOMAIN_MEMORY,
-			 LIBCERROR_MEMORY_ERROR_COPY_FAILED,
-			 "%s: unable to copy value data.",
+			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+			 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+			 "%s: invalid byte stream size value too small.",
 			 function );
 
 			goto on_error;
 		}
-		byte_stream_offset += internal_record->value_data_size;
+		byte_stream_copy_to_uint32_little_endian(
+		 &( byte_stream[ byte_stream_offset ] ),
+		 number_of_values );
+
+#if defined( HAVE_DEBUG_OUTPUT )
+		if( libcnotify_verbose != 0 )
+		{
+			if( has_variable_data_size == 0 )
+			{
+				libcnotify_printf(
+				 "%s: value data size\t\t\t: %" PRIu32 "\n",
+				 function,
+				 internal_record->value_data_size );
+			}
+			libcnotify_printf(
+			 "%s: number of values\t\t\t: %" PRIu32 "\n",
+			 function,
+			 number_of_values );
+		}
+#endif
+		byte_stream_offset += 4;
+
+		if( has_variable_data_size == 0 )
+		{
+			if( ( internal_record->value_data_size > 0 )
+			 && ( number_of_values > ( (size_t) SSIZE_MAX / internal_record->value_data_size ) ) )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+				 "%s: invalid number of values value out of bounds.",
+				 function );
+
+				goto on_error;
+			}
+#if defined( HAVE_DEBUG_OUTPUT )
+			if( libcnotify_verbose != 0 )
+			{
+				libcnotify_printf(
+				 "%s: vector values data:\n",
+				 function,
+				 value_index );
+				libcnotify_print_data(
+				 &( byte_stream[ byte_stream_offset ] ),
+				 internal_record->value_data_size,
+				 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
+			}
+#endif
+			internal_record->value_data_size *= number_of_values;
+
+			byte_stream_offset += internal_record->value_data_size;
+		}
+		else
+		{
+			if( ( number_of_values > ( ( byte_stream_size - byte_stream_offset ) / 4 ) )
+			 || ( number_of_values == 0xffffffffUL ) )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+				 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+				 "%s: invalid number of values value out of bounds.",
+				 function );
+
+				goto on_error;
+			}
+			for( value_index = 0;
+			     value_index < number_of_values;
+			     value_index++ )
+			{
+				if( byte_stream_offset > ( byte_stream_size - 4 ) )
+				{
+					libcerror_error_set(
+					 error,
+					 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+					 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+					 "%s: invalid byte stream size value too small.",
+					 function );
+
+					goto on_error;
+				}
+				byte_stream_copy_to_uint32_little_endian(
+				 &( byte_stream[ byte_stream_offset ] ),
+				 vector_value_data_size );
+
+#if defined( HAVE_DEBUG_OUTPUT )
+				if( libcnotify_verbose != 0 )
+				{
+					libcnotify_printf(
+					 "%s: vector value: %" PRIu32 " data size\t\t: %" PRIu32 "\n",
+					 function,
+					 value_index,
+					 vector_value_data_size );
+				}
+#endif
+				byte_stream_offset += 4;
+
+				if( ( internal_record->value_type & 0x00000fffUL ) == LIBFWPS_VALUE_TYPE_STRING_UNICODE )
+				{
+					if( vector_value_data_size > ( (uint32_t) UINT32_MAX / 2 ) )
+					{
+						libcerror_error_set(
+						 error,
+						 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+						 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+						 "%s: invalid vector value: %" PRIu32 " data size value out of bounds.",
+						 function,
+						 value_index );
+
+						goto on_error;
+					}
+					vector_value_data_size *= 2;
+				}
+				if( vector_value_data_size > ( (size_t) SSIZE_MAX - internal_record->value_data_size ) )
+				{
+					libcerror_error_set(
+					 error,
+					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+					 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+					 "%s: invalid vector value: %" PRIu32 " data size value out of bounds.",
+					 function,
+					 value_index );
+
+					goto on_error;
+				}
+#if defined( HAVE_DEBUG_OUTPUT )
+				if( libcnotify_verbose != 0 )
+				{
+					libcnotify_printf(
+					 "%s: vector value: %" PRIu32 " data:\n",
+					 function,
+					 value_index );
+					libcnotify_print_data(
+					 &( byte_stream[ byte_stream_offset ] ),
+					 vector_value_data_size,
+					 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
+				}
+#endif
+				byte_stream_offset += vector_value_data_size;
+
+				internal_record->value_data_size += 4 + vector_value_data_size;
+
+				if( byte_stream_offset <= ( byte_stream_size - 2 ) )
+				{
+					byte_stream_copy_to_uint16_little_endian(
+					 &( byte_stream[ byte_stream_offset ] ),
+					 value_16bit );
+
+					if( value_16bit == 0 )
+					{
+#if defined( HAVE_DEBUG_OUTPUT )
+						if( libcnotify_verbose != 0 )
+						{
+							libcnotify_printf(
+							 "%s: alignment padding data:\n",
+							 function );
+							libcnotify_print_data(
+							 &( byte_stream[ byte_stream_offset ] ),
+							 2,
+							 0 );
+						}
+#endif
+						byte_stream_offset += 2;
+
+						internal_record->value_data_size += 2;
+					}
+				}
+			}
+		}
+	}
+	else
+	{
+		if( has_variable_data_size != 0 )
+		{
+			if( byte_stream_offset > ( byte_stream_size - 4 ) )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+				 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+				 "%s: invalid byte stream size value too small.",
+				 function );
+
+				goto on_error;
+			}
+			byte_stream_copy_to_uint32_little_endian(
+			 &( byte_stream[ byte_stream_offset ] ),
+			 internal_record->value_data_size );
+
+			byte_stream_offset += 4;
+
+			if( internal_record->value_type == LIBFWPS_VALUE_TYPE_STRING_UNICODE )
+			{
+				if( internal_record->value_data_size > ( (size_t) SSIZE_MAX / 2 ) )
+				{
+					libcerror_error_set(
+					 error,
+					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+					 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+					 "%s: invalid value data size value out of bounds.",
+					 function );
+
+					goto on_error;
+				}
+				internal_record->value_data_size *= 2;
+			}
+		}
+#if defined( HAVE_DEBUG_OUTPUT )
+		if( libcnotify_verbose != 0 )
+		{
+			libcnotify_printf(
+			 "%s: value data size\t\t\t: %" PRIu32 "\n",
+			 function,
+			 internal_record->value_data_size );
+		}
+#endif
+		if( internal_record->value_data_size > 0 )
+		{
+			if( ( internal_record->value_data_size > byte_stream_size )
+			 || ( byte_stream_offset > ( byte_stream_size - internal_record->value_data_size ) ) )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+				 "%s: invalid value data size value out of bounds.",
+				 function );
+
+				goto on_error;
+			}
+#if defined( HAVE_DEBUG_OUTPUT )
+			if( libcnotify_verbose != 0 )
+			{
+				libcnotify_printf(
+				 "%s: value data:\n",
+				 function );
+				libcnotify_print_data(
+				 &( byte_stream[ byte_stream_offset ] ),
+				 internal_record->value_data_size,
+				 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
+			}
+#endif
+			if( internal_record->value_data_size > MEMORY_MAXIMUM_ALLOCATION_SIZE )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_VALUE_EXCEEDS_MAXIMUM,
+				 "%s: invalid value data size value exceeds maximum.",
+				 function );
+
+				goto on_error;
+			}
+			internal_record->value_data = (uint8_t *) memory_allocate(
+			                                           sizeof( uint8_t ) * internal_record->value_data_size );
+
+			if( internal_record->value_data == NULL )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_MEMORY,
+				 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
+				 "%s: unable to create value data.",
+				 function );
+
+				goto on_error;
+			}
+			if( memory_copy(
+			     internal_record->value_data,
+			     &( byte_stream[ byte_stream_offset ] ),
+			     internal_record->value_data_size ) == NULL )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_MEMORY,
+				 LIBCERROR_MEMORY_ERROR_COPY_FAILED,
+				 "%s: unable to copy value data.",
+				 function );
+
+				goto on_error;
+			}
+			byte_stream_offset += internal_record->value_data_size;
+		}
 	}
 #if defined( HAVE_DEBUG_OUTPUT )
 	if( libcnotify_verbose != 0 )
 	{
 		if( byte_stream_offset < internal_record->size )
 		{
 			libcnotify_printf(
@@ -618,15 +935,16 @@
 			 function );
 			libcnotify_print_data(
 			 &( byte_stream[ byte_stream_offset ] ),
 			 internal_record->size - byte_stream_offset,
 			 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
 		}
 	}
-#endif
+#endif /* defined( HAVE_DEBUG_OUTPUT ) */
+
 	internal_record->ascii_codepage = ascii_codepage;
 
 	return( 1 );
 
 on_error:
 #if defined( HAVE_DEBUG_OUTPUT )
 	if( value_string != NULL )
@@ -640,17 +958,231 @@
 		memory_free(
 		 internal_record->value_data );
 
 		internal_record->value_data = NULL;
 	}
 	internal_record->value_data_size = 0;
 
+	if( internal_record->value_name != NULL )
+	{
+		memory_free(
+		 internal_record->value_name );
+
+		internal_record->value_name = NULL;
+	}
+	internal_record->value_name_size = 0;
+
+	if( internal_record->entry_name != NULL )
+	{
+		memory_free(
+		 internal_record->entry_name );
+
+		internal_record->entry_name = NULL;
+	}
+	internal_record->entry_name_size = 0;
+
 	return( -1 );
 }
 
+/* Retrieves the size of the UTF-8 encoded entry name
+ * The returned size includes the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_utf8_entry_name_size(
+     libfwps_record_t *record,
+     size_t *utf8_string_size,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_utf8_entry_name_size";
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( internal_record->type != LIBFWPS_RECORD_TYPE_NAMED )
+	{
+		return( 0 );
+	}
+	if( libuna_utf8_string_size_from_utf16_stream(
+	     internal_record->entry_name,
+	     internal_record->entry_name_size,
+	     LIBUNA_ENDIAN_LITTLE,
+	     utf8_string_size,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to retrieve size of entry name as UTF-8 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the UTF-8 encoded entry name
+ * The size should include the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_utf8_entry_name(
+     libfwps_record_t *record,
+     uint8_t *utf8_string,
+     size_t utf8_string_size,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_utf8_entry_name";
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( internal_record->type != LIBFWPS_RECORD_TYPE_NAMED )
+	{
+		return( 0 );
+	}
+	if( libuna_utf8_string_copy_from_utf16_stream(
+	     utf8_string,
+	     utf8_string_size,
+	     internal_record->entry_name,
+	     internal_record->entry_name_size,
+	     LIBUNA_ENDIAN_LITTLE,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to retrieve entry name as UTF-8 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the size of the UTF-16 encoded entry name
+ * The returned size includes the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_utf16_entry_name_size(
+     libfwps_record_t *record,
+     size_t *utf16_string_size,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_utf16_entry_name_size";
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( internal_record->type != LIBFWPS_RECORD_TYPE_NAMED )
+	{
+		return( 0 );
+	}
+	if( libuna_utf16_string_size_from_utf16_stream(
+	     internal_record->entry_name,
+	     internal_record->entry_name_size,
+	     LIBUNA_ENDIAN_LITTLE,
+	     utf16_string_size,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to retrieve size of entry name as UTF-16 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the UTF-16 encoded entry name
+ * The size should include the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_utf16_entry_name(
+     libfwps_record_t *record,
+     uint16_t *utf16_string,
+     size_t utf16_string_size,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_utf16_entry_name";
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( internal_record->type != LIBFWPS_RECORD_TYPE_NAMED )
+	{
+		return( 0 );
+	}
+	if( libuna_utf16_string_copy_from_utf16_stream(
+	     utf16_string,
+	     utf16_string_size,
+	     internal_record->entry_name,
+	     internal_record->entry_name_size,
+	     LIBUNA_ENDIAN_LITTLE,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to retrieve entry name as UTF-16 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
 /* Retrieves the entry type
  * Returns 1 if successful, 0 if not available or -1 on error
  */
 int libfwps_record_get_entry_type(
      libfwps_record_t *record,
      uint32_t *entry_type,
      libcerror_error_t **error )
@@ -678,23 +1210,223 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid entry type.",
 		 function );
 
 		return( -1 );
 	}
-	if( internal_record->type == LIBFWPS_RECORD_TYPE_NAMED )
+	if( internal_record->type != LIBFWPS_RECORD_TYPE_NUMERIC )
 	{
 		return( 0 );
 	}
 	*entry_type = internal_record->entry_type;
 
 	return( 1 );
 }
 
+/* Retrieves the size of the UTF-8 encoded value name
+ * The returned size includes the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_utf8_value_name_size(
+     libfwps_record_t *record,
+     size_t *utf8_string_size,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_utf8_value_name_size";
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( ( internal_record->value_name_size == 0 )
+	 || ( internal_record->value_name == NULL ) )
+	{
+		return( 0 );
+	}
+	if( libuna_utf8_string_size_from_utf16_stream(
+	     internal_record->value_name,
+	     internal_record->value_name_size,
+	     LIBUNA_ENDIAN_LITTLE,
+	     utf8_string_size,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to retrieve size of value name as UTF-8 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the UTF-8 encoded value name
+ * The size should include the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_utf8_value_name(
+     libfwps_record_t *record,
+     uint8_t *utf8_string,
+     size_t utf8_string_size,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_utf8_value_name";
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( ( internal_record->value_name_size == 0 )
+	 || ( internal_record->value_name == NULL ) )
+	{
+		return( 0 );
+	}
+	if( libuna_utf8_string_copy_from_utf16_stream(
+	     utf8_string,
+	     utf8_string_size,
+	     internal_record->value_name,
+	     internal_record->value_name_size,
+	     LIBUNA_ENDIAN_LITTLE,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to retrieve value name as UTF-8 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the size of the UTF-16 encoded value name
+ * The returned size includes the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_utf16_value_name_size(
+     libfwps_record_t *record,
+     size_t *utf16_string_size,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_utf16_value_name_size";
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( ( internal_record->value_name_size == 0 )
+	 || ( internal_record->value_name == NULL ) )
+	{
+		return( 0 );
+	}
+	if( libuna_utf16_string_size_from_utf16_stream(
+	     internal_record->value_name,
+	     internal_record->value_name_size,
+	     LIBUNA_ENDIAN_LITTLE,
+	     utf16_string_size,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to retrieve size of value name as UTF-16 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the UTF-16 encoded value name
+ * The size should include the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_utf16_value_name(
+     libfwps_record_t *record,
+     uint16_t *utf16_string,
+     size_t utf16_string_size,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_utf16_value_name";
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( ( internal_record->value_name_size == 0 )
+	 || ( internal_record->value_name == NULL ) )
+	{
+		return( 0 );
+	}
+	if( libuna_utf16_string_copy_from_utf16_stream(
+	     utf16_string,
+	     utf16_string_size,
+	     internal_record->value_name,
+	     internal_record->value_name_size,
+	     LIBUNA_ENDIAN_LITTLE,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to retrieve value name as UTF-16 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
 /* Retrieves the value type
  * Returns 1 if successful or -1 on error
  */
 int libfwps_record_get_value_type(
      libfwps_record_t *record,
      uint32_t *value_type,
      libcerror_error_t **error )
@@ -727,14 +1459,130 @@
 		return( -1 );
 	}
 	*value_type = internal_record->value_type;
 
 	return( 1 );
 }
 
+/* Retrieves the data size
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_data_size(
+     libfwps_record_t *record,
+     size_t *data_size,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_data_size";
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( data_size == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid data size.",
+		 function );
+
+		return( -1 );
+	}
+	*data_size = internal_record->value_data_size;
+
+	return( 1 );
+}
+
+/* Retrieves the data
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_data(
+     libfwps_record_t *record,
+     uint8_t *data,
+     size_t data_size,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_data";
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( internal_record->value_data == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
+		 "%s: invalid record entry - missing value data.",
+		 function );
+
+		return( -1 );
+	}
+	if( data == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid data.",
+		 function );
+
+		return( -1 );
+	}
+	if( ( data_size < internal_record->value_data_size )
+	 || ( data_size > (size_t) SSIZE_MAX ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_OUT_OF_BOUNDS,
+		 "%s: invalid data size value out of bounds.",
+		 function );
+
+		return( -1 );
+	}
+	if( memory_copy(
+	     data,
+	     internal_record->value_data,
+	     internal_record->value_data_size ) == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_MEMORY,
+		 LIBCERROR_MEMORY_ERROR_COPY_FAILED,
+		 "%s: unable to copy data.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
 /* Retrieves the data as a boolean value
  * Returns 1 if successful or -1 on error
  */
 int libfwps_record_get_data_as_boolean(
      libfwps_record_t *record,
      uint8_t *value_boolean,
      libcerror_error_t **error )
@@ -757,16 +1605,17 @@
 
 	if( internal_record->value_type != LIBFWPS_VALUE_TYPE_BOOLEAN )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: invalid record entry - unsupported value type.",
-		 function );
+		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
+		 function,
+		 internal_record->value_type );
 
 		return( -1 );
 	}
 	if( internal_record->value_data == NULL )
 	{
 		libcerror_error_set(
 		 error,
@@ -831,16 +1680,17 @@
 	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_8BIT_SIGNED )
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_8BIT_UNSIGNED ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: invalid record entry - unsupported value type.",
-		 function );
+		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
+		 function,
+		 internal_record->value_type );
 
 		return( -1 );
 	}
 	if( internal_record->value_data == NULL )
 	{
 		libcerror_error_set(
 		 error,
@@ -905,16 +1755,17 @@
 	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_16BIT_SIGNED )
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_16BIT_UNSIGNED ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: invalid record entry - unsupported value type.",
-		 function );
+		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
+		 function,
+		 internal_record->value_type );
 
 		return( -1 );
 	}
 	if( internal_record->value_data == NULL )
 	{
 		libcerror_error_set(
 		 error,
@@ -974,24 +1825,27 @@
 		 "%s: invalid record entry.",
 		 function );
 
 		return( -1 );
 	}
 	internal_record = (libfwps_internal_record_t *) record;
 
-	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_32BIT_SIGNED )
+	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_ERROR )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_32BIT_SIGNED )
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_32BIT_UNSIGNED )
-	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_ERROR ) )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_SIGNED )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_UNSIGNED ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: invalid record entry - unsupported value type.",
-		 function );
+		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
+		 function,
+		 internal_record->value_type );
 
 		return( -1 );
 	}
 	if( internal_record->value_data == NULL )
 	{
 		libcerror_error_set(
 		 error,
@@ -1051,24 +1905,27 @@
 		 "%s: invalid record entry.",
 		 function );
 
 		return( -1 );
 	}
 	internal_record = (libfwps_internal_record_t *) record;
 
-	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_64BIT_SIGNED )
-	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_64BIT_UNSIGNED )
-	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_CURRENCY ) )
+	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_APPLICATION_TIME )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_CURRENCY )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_FILETIME )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_64BIT_SIGNED )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_INTEGER_64BIT_UNSIGNED ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: invalid record entry - unsupported value type.",
-		 function );
+		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
+		 function,
+		 internal_record->value_type );
 
 		return( -1 );
 	}
 	if( internal_record->value_data == NULL )
 	{
 		libcerror_error_set(
 		 error,
@@ -1104,14 +1961,90 @@
 	byte_stream_copy_to_uint64_little_endian(
 	 internal_record->value_data,
 	 *value_64bit );
 
 	return( 1 );
 }
 
+/* Retrieves the data as a 64-bit floatingtime value
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_data_as_floatingtime(
+     libfwps_record_t *record,
+     uint64_t *floatingtime,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_data_as_floatingtime";
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record entry.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( internal_record->value_type != LIBFWPS_VALUE_TYPE_APPLICATION_TIME )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
+		 function,
+		 internal_record->value_type );
+
+		return( -1 );
+	}
+	if( internal_record->value_data == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
+		 "%s: invalid record entry - missing value data.",
+		 function );
+
+		return( -1 );
+	}
+	if( internal_record->value_data_size != 8 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported value data size.",
+		 function );
+
+		return( -1 );
+	}
+	if( floatingtime == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid floatingtime.",
+		 function );
+
+		return( -1 );
+	}
+	byte_stream_copy_to_uint64_little_endian(
+	 internal_record->value_data,
+	 *floatingtime );
+
+	return( 1 );
+}
+
 /* Retrieves the data as a 64-bit FILETIME value
  * Returns 1 if successful or -1 on error
  */
 int libfwps_record_get_data_as_filetime(
      libfwps_record_t *record,
      uint64_t *filetime,
      libcerror_error_t **error )
@@ -1134,16 +2067,17 @@
 
 	if( internal_record->value_type != LIBFWPS_VALUE_TYPE_FILETIME )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: invalid record entry - unsupported value type.",
-		 function );
+		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
+		 function,
+		 internal_record->value_type );
 
 		return( -1 );
 	}
 	if( internal_record->value_data == NULL )
 	{
 		libcerror_error_set(
 		 error,
@@ -1206,23 +2140,25 @@
 		 "%s: invalid record entry.",
 		 function );
 
 		return( -1 );
 	}
 	internal_record = (libfwps_internal_record_t *) record;
 
-	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_FLOAT_32BIT )
+	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_APPLICATION_TIME )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_FLOAT_32BIT )
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_DOUBLE_64BIT ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: invalid record entry - unsupported value type.",
-		 function );
+		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
+		 function,
+		 internal_record->value_type );
 
 		return( -1 );
 	}
 	if( internal_record->value_data == NULL )
 	{
 		libcerror_error_set(
 		 error,
@@ -1309,16 +2245,17 @@
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: invalid record entry - unsupported value type.",
-		 function );
+		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
+		 function,
+		 internal_record->value_type );
 
 		return( -1 );
 	}
 	if( utf8_string_size == NULL )
 	{
 		libcerror_error_set(
 		 error,
@@ -1427,16 +2364,17 @@
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: invalid record entry - unsupported value type.",
-		 function );
+		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
+		 function,
+		 internal_record->value_type );
 
 		return( -1 );
 	}
 	if( utf8_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
@@ -1560,16 +2498,17 @@
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: invalid record entry - unsupported value type.",
-		 function );
+		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
+		 function,
+		 internal_record->value_type );
 
 		return( -1 );
 	}
 	if( utf16_string_size == NULL )
 	{
 		libcerror_error_set(
 		 error,
@@ -1678,16 +2617,17 @@
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: invalid record entry - unsupported value type.",
-		 function );
+		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
+		 function,
+		 internal_record->value_type );
 
 		return( -1 );
 	}
 	if( utf16_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
@@ -1812,16 +2752,17 @@
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: invalid record entry - unsupported value type.",
-		 function );
+		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
+		 function,
+		 internal_record->value_type );
 
 		return( -1 );
 	}
 	if( utf8_string_size == NULL )
 	{
 		libcerror_error_set(
 		 error,
@@ -1931,16 +2872,17 @@
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: invalid record entry - unsupported value type.",
-		 function );
+		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
+		 function,
+		 internal_record->value_type );
 
 		return( -1 );
 	}
 	if( utf8_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
@@ -2065,16 +3007,17 @@
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: invalid record entry - unsupported value type.",
-		 function );
+		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
+		 function,
+		 internal_record->value_type );
 
 		return( -1 );
 	}
 	if( utf16_string_size == NULL )
 	{
 		libcerror_error_set(
 		 error,
@@ -2184,16 +3127,17 @@
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: invalid record entry - unsupported value type.",
-		 function );
+		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
+		 function,
+		 internal_record->value_type );
 
 		return( -1 );
 	}
 	if( utf16_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
@@ -2312,16 +3256,17 @@
 
 	if( internal_record->value_type != LIBFWPS_VALUE_TYPE_GUID )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: invalid record entry - unsupported value type.",
-		 function );
+		 "%s: invalid record entry - unsupported value type: 0x%04" PRIx32 ".",
+		 function,
+		 internal_record->value_type );
 
 		return( -1 );
 	}
 	if( internal_record->value_data == NULL )
 	{
 		libcerror_error_set(
 		 error,
```

### Comparing `libolecf-20240212/libfwps/libfwps_set.c` & `libolecf-20240427/libfwps/libfwps_set.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfwps/Makefile.in` & `libolecf-20240427/libfwps/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -115,26 +115,29 @@
 DIST_COMMON = $(srcdir)/Makefile.am $(am__DIST_COMMON)
 mkinstalldirs = $(install_sh) -d
 CONFIG_HEADER = $(top_builddir)/common/config.h
 CONFIG_CLEAN_FILES =
 CONFIG_CLEAN_VPATH_FILES =
 LTLIBRARIES = $(noinst_LTLIBRARIES)
 libfwps_la_LIBADD =
-am__libfwps_la_SOURCES_DIST = libfwps_codepage.h libfwps_definitions.h \
-	libfwps_extern.h libfwps_error.c libfwps_error.h \
+am__libfwps_la_SOURCES_DIST = libfwps_codepage.h libfwps_debug.c \
+	libfwps_debug.h libfwps_definitions.h libfwps_extern.h \
+	libfwps_error.c libfwps_error.h \
 	libfwps_format_class_identifier.c \
 	libfwps_format_class_identifier.h libfwps_libcdata.h \
 	libfwps_libcerror.h libfwps_libcnotify.h libfwps_libfguid.h \
-	libfwps_libuna.h libfwps_property_identifier.c \
-	libfwps_property_identifier.h libfwps_record.c \
-	libfwps_record.h libfwps_set.c libfwps_set.h libfwps_store.c \
-	libfwps_store.h libfwps_support.c libfwps_support.h \
-	libfwps_types.h libfwps_unused.h
-@HAVE_LOCAL_LIBFWPS_TRUE@am_libfwps_la_OBJECTS = libfwps_error.lo \
+	libfwps_libuna.h libfwps_notify.c libfwps_notify.h \
+	libfwps_property_identifier.c libfwps_property_identifier.h \
+	libfwps_record.c libfwps_record.h libfwps_set.c libfwps_set.h \
+	libfwps_store.c libfwps_store.h libfwps_support.c \
+	libfwps_support.h libfwps_types.h libfwps_unused.h
+@HAVE_LOCAL_LIBFWPS_TRUE@am_libfwps_la_OBJECTS = libfwps_debug.lo \
+@HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_error.lo \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_format_class_identifier.lo \
+@HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_notify.lo \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_property_identifier.lo \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_record.lo libfwps_set.lo \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_store.lo libfwps_support.lo
 libfwps_la_OBJECTS = $(am_libfwps_la_OBJECTS)
 AM_V_lt = $(am__v_lt_@AM_V@)
 am__v_lt_ = $(am__v_lt_@AM_DEFAULT_V@)
 am__v_lt_0 = --silent
@@ -151,16 +154,18 @@
 AM_V_at = $(am__v_at_@AM_V@)
 am__v_at_ = $(am__v_at_@AM_DEFAULT_V@)
 am__v_at_0 = @
 am__v_at_1 = 
 DEFAULT_INCLUDES = -I.@am__isrc@ -I$(top_builddir)/common
 depcomp = $(SHELL) $(top_srcdir)/depcomp
 am__maybe_remake_depfiles = depfiles
-am__depfiles_remade = ./$(DEPDIR)/libfwps_error.Plo \
+am__depfiles_remade = ./$(DEPDIR)/libfwps_debug.Plo \
+	./$(DEPDIR)/libfwps_error.Plo \
 	./$(DEPDIR)/libfwps_format_class_identifier.Plo \
+	./$(DEPDIR)/libfwps_notify.Plo \
 	./$(DEPDIR)/libfwps_property_identifier.Plo \
 	./$(DEPDIR)/libfwps_record.Plo ./$(DEPDIR)/libfwps_set.Plo \
 	./$(DEPDIR)/libfwps_store.Plo ./$(DEPDIR)/libfwps_support.Plo
 am__mv = mv -f
 COMPILE = $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) \
 	$(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS)
 LTCOMPILE = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
@@ -463,14 +468,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -529,46 +536,49 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFWPS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFWPS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFWPS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFWPS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFWPS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFWPS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWPS_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWPS_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWPS_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWPS_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWPS_TRUE@	@LIBFDATETIME_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWPS_TRUE@	@LIBFGUID_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWPS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFWPS_TRUE@noinst_LTLIBRARIES = libfwps.la
 @HAVE_LOCAL_LIBFWPS_TRUE@libfwps_la_SOURCES = \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_codepage.h \
+@HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_debug.c libfwps_debug.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_definitions.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_extern.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_error.c libfwps_error.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_format_class_identifier.c libfwps_format_class_identifier.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_libcdata.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_libcerror.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_libcnotify.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_libfguid.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_libuna.h \
+@HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_notify.c libfwps_notify.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_property_identifier.c libfwps_property_identifier.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_record.c libfwps_record.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_set.c libfwps_set.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_store.c libfwps_store.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_support.c libfwps_support.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_types.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -617,16 +627,18 @@
 
 mostlyclean-compile:
 	-rm -f *.$(OBJEXT)
 
 distclean-compile:
 	-rm -f *.tab.c
 
+@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwps_debug.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwps_error.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwps_format_class_identifier.Plo@am__quote@ # am--include-marker
+@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwps_notify.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwps_property_identifier.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwps_record.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwps_set.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwps_store.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwps_support.Plo@am__quote@ # am--include-marker
 
 $(am__depfiles_remade):
@@ -774,24 +786,35 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfwps_debug.Plo
+	-rm -f ./$(DEPDIR)/libfwps_error.Plo
+	-rm -f ./$(DEPDIR)/libfwps_format_class_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwps_notify.Plo
+	-rm -f ./$(DEPDIR)/libfwps_property_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwps_record.Plo
+	-rm -f ./$(DEPDIR)/libfwps_set.Plo
+	-rm -f ./$(DEPDIR)/libfwps_store.Plo
+	-rm -f ./$(DEPDIR)/libfwps_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -828,16 +851,18 @@
 install-ps: install-ps-am
 
 install-ps-am:
 
 installcheck-am:
 
 maintainer-clean: maintainer-clean-am
-		-rm -f ./$(DEPDIR)/libfwps_error.Plo
+		-rm -f ./$(DEPDIR)/libfwps_debug.Plo
+	-rm -f ./$(DEPDIR)/libfwps_error.Plo
 	-rm -f ./$(DEPDIR)/libfwps_format_class_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwps_notify.Plo
 	-rm -f ./$(DEPDIR)/libfwps_property_identifier.Plo
 	-rm -f ./$(DEPDIR)/libfwps_record.Plo
 	-rm -f ./$(DEPDIR)/libfwps_set.Plo
 	-rm -f ./$(DEPDIR)/libfwps_store.Plo
 	-rm -f ./$(DEPDIR)/libfwps_support.Plo
 	-rm -f Makefile
 maintainer-clean-am: distclean-am maintainer-clean-generic
@@ -881,17 +906,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwps ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwps_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libolecf-20240212/libfwps/libfwps_unused.h` & `libolecf-20240427/libfwps/libfwps_unused.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/common/config_borlandc.h` & `libolecf-20240427/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/common/file_stream.h` & `libolecf-20240427/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/common/memory.h` & `libolecf-20240427/common/memory.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/common/byte_stream.h` & `libolecf-20240427/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/common/common.h` & `libolecf-20240427/common/common.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/common/config_winapi.h` & `libolecf-20240427/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/common/system_string.h` & `libolecf-20240427/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/common/types.h.in` & `libolecf-20240427/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/common/types.h` & `libolecf-20240427/common/types.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/common/config.h.in` & `libolecf-20240427/common/config.h.in`

 * *Files 0% similar despite different names*

```diff
@@ -206,14 +206,17 @@
 
 /* Define to 1 if you have the <libfole.h> header file. */
 #undef HAVE_LIBFOLE_H
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
 #undef HAVE_LIBFUSE
 
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#undef HAVE_LIBFUSE3
+
 /* Define to 1 if you have the `fvalue' library (-lfvalue). */
 #undef HAVE_LIBFVALUE
 
 /* Define to 1 if you have the <libfvalue.h> header file. */
 #undef HAVE_LIBFVALUE_H
 
 /* Define to 1 if you have the `fwps' library (-lfwps). */
```

### Comparing `libolecf-20240212/common/config.h` & `libolecf-20240427/common/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,18 @@
 /* Define to 1 if you have the `fole' library (-lfole). */
 /* #undef HAVE_LIBFOLE */
 
 /* Define to 1 if you have the <libfole.h> header file. */
 /* #undef HAVE_LIBFOLE_H */
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
-#define HAVE_LIBFUSE 1
+/* #undef HAVE_LIBFUSE */
+
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#define HAVE_LIBFUSE3 1
 
 /* Define to 1 if you have the `fvalue' library (-lfvalue). */
 /* #undef HAVE_LIBFVALUE */
 
 /* Define to 1 if you have the <libfvalue.h> header file. */
 /* #undef HAVE_LIBFVALUE_H */
 
@@ -550,24 +553,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libolecf"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libolecf 20240212"
+#define PACKAGE_STRING "libolecf 20240427"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libolecf"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240212"
+#define PACKAGE_VERSION "20240427"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -585,15 +588,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20240212"
+#define VERSION "20240427"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libolecf-20240212/common/wide_string.h` & `libolecf-20240427/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/common/narrow_string.h` & `libolecf-20240427/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/common/config_msc.h` & `libolecf-20240427/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/common/Makefile.in` & `libolecf-20240427/common/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -414,14 +414,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -479,15 +481,17 @@
 sharedstatedir = @sharedstatedir@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -495,15 +499,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -671,23 +678,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -767,15 +776,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libolecf-20240212/libclocale/libclocale_wide_string.c` & `libolecf-20240427/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libclocale/libclocale_support.h` & `libolecf-20240427/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libclocale/Makefile.am` & `libolecf-20240427/libclocale/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 if HAVE_LOCAL_LIBCLOCALE
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libclocale.la
 
 libclocale_la_SOURCES = \
 	libclocale_codepage.c libclocale_codepage.h \
 	libclocale_definitions.h \
@@ -14,19 +14,17 @@
 	libclocale_libcerror.h \
 	libclocale_locale.c libclocale_locale.h \
 	libclocale_support.c libclocale_support.h \
 	libclocale_unused.h \
 	libclocale_wide_string.c libclocale_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
```

### Comparing `libolecf-20240212/libclocale/libclocale_definitions.h` & `libolecf-20240427/libclocale/libclocale_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #include <libclocale/definitions.h>
 
 /* The definitions in <libclocale/definitions.h> are copied here
  * for local use of libclocale
  */
 #else
 
-#define LIBCLOCALE_VERSION					20240107
+#define LIBCLOCALE_VERSION					20240414
 
 /* The libclocale version string
  */
-#define LIBCLOCALE_VERSION_STRING				"20240107"
+#define LIBCLOCALE_VERSION_STRING				"20240414"
 
 /* The codepage feature flag definitions
  */
 enum LIBCLOCALE_CODEPAGES_FEATURE_FLAGS
 {
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_ISO_8859		= 0x00000001UL,
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_KOI8		= 0x00000002UL,
```

### Comparing `libolecf-20240212/libclocale/libclocale_unused.h` & `libolecf-20240427/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libclocale/libclocale_libcerror.h` & `libolecf-20240427/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libclocale/libclocale_locale.h` & `libolecf-20240427/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libclocale/libclocale_support.c` & `libolecf-20240427/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libclocale/libclocale_codepage.c` & `libolecf-20240427/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libclocale/libclocale_locale.c` & `libolecf-20240427/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libclocale/Makefile.in` & `libolecf-20240427/libclocale/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -458,14 +458,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -525,30 +527,31 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCLOCALE_TRUE@AM_CPPFLAGS = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	-DLOCALEDIR=\"$(datadir)/locale\" \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCLOCALE_TRUE@noinst_LTLIBRARIES = libclocale.la
 @HAVE_LOCAL_LIBCLOCALE_TRUE@libclocale_la_SOURCES = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_codepage.c libclocale_codepage.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_definitions.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_extern.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_libcerror.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_locale.c libclocale_locale.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_support.c libclocale_support.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_unused.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_wide_string.c libclocale_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -751,24 +754,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libclocale_codepage.Plo
+	-rm -f ./$(DEPDIR)/libclocale_locale.Plo
+	-rm -f ./$(DEPDIR)/libclocale_support.Plo
+	-rm -f ./$(DEPDIR)/libclocale_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -855,17 +864,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libolecf-20240212/libclocale/libclocale_extern.h` & `libolecf-20240427/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libclocale/libclocale_wide_string.h` & `libolecf-20240427/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libclocale/libclocale_codepage.h` & `libolecf-20240427/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_property_value.c` & `libolecf-20240427/pyolecf/pyolecf_property_value.c`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 	  "get_type() -> Integer or None\n"
 	  "\n"
 	  "Retrieves the value type." },
 
 	{ "get_data",
 	  (PyCFunction) pyolecf_property_value_get_data,
 	  METH_NOARGS,
-	  "get_data() -> Binary string or None\n"
+	  "get_data()-> Bytes or None\n"
 	  "\n"
 	  "Retrieves the data." },
 
 	{ "get_data_as_boolean",
 	  (PyCFunction) pyolecf_property_value_get_data_as_boolean,
 	  METH_NOARGS,
 	  "get_data_as_boolean() -> Integer or None\n"
```

### Comparing `libolecf-20240212/pyolecf/pyolecf_property_value.h` & `libolecf-20240427/pyolecf/pyolecf_property_value.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_item.h` & `libolecf-20240427/pyolecf/pyolecf_item.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_libclocale.h` & `libolecf-20240427/pyolecf/pyolecf_libclocale.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_file.c` & `libolecf-20240427/pyolecf/pyolecf_file.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_libolecf.h` & `libolecf-20240427/pyolecf/pyolecf_libolecf.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_codepage.h` & `libolecf-20240427/pyolecf/pyolecf_codepage.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf.c` & `libolecf-20240427/pyolecf/pyolecf.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_items.c` & `libolecf-20240427/pyolecf/pyolecf_items.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_codepage.c` & `libolecf-20240427/pyolecf/pyolecf_codepage.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_python.h` & `libolecf-20240427/pyolecf/pyolecf_python.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_file_object_io_handle.h` & `libolecf-20240427/pyolecf/pyolecf_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_property_values.c` & `libolecf-20240427/pyolecf/pyolecf_property_values.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_property_set_stream.h` & `libolecf-20240427/pyolecf/pyolecf_property_set_stream.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_libcerror.h` & `libolecf-20240427/pyolecf/pyolecf_libcerror.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/Makefile.am` & `libolecf-20240427/pyolecf/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -56,13 +56,11 @@
 	@LIBFGUID_LIBADD@
 
 pyolecf_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyolecf_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libolecf-20240212/pyolecf/pyolecf_integer.h` & `libolecf-20240427/pyolecf/pyolecf_integer.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_guid.h` & `libolecf-20240427/pyolecf/pyolecf_guid.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_property_set_stream.c` & `libolecf-20240427/pyolecf/pyolecf_property_set_stream.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_value_types.h` & `libolecf-20240427/pyolecf/pyolecf_value_types.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_property_sections.c` & `libolecf-20240427/pyolecf/pyolecf_property_sections.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_error.c` & `libolecf-20240427/pyolecf/pyolecf_error.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_property_section.c` & `libolecf-20240427/pyolecf/pyolecf_property_section.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf.h` & `libolecf-20240427/pyolecf/pyolecf.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_property_sections.h` & `libolecf-20240427/pyolecf/pyolecf_property_sections.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_error.h` & `libolecf-20240427/pyolecf/pyolecf_error.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_file_object_io_handle.c` & `libolecf-20240427/pyolecf/pyolecf_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_unused.h` & `libolecf-20240427/pyolecf/pyolecf_unused.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_file.h` & `libolecf-20240427/pyolecf/pyolecf_file.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_item_types.c` & `libolecf-20240427/pyolecf/pyolecf_item_types.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_stream.h` & `libolecf-20240427/pyolecf/pyolecf_stream.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_datetime.c` & `libolecf-20240427/pyolecf/pyolecf_datetime.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_stream.c` & `libolecf-20240427/pyolecf/pyolecf_stream.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_value_types.c` & `libolecf-20240427/pyolecf/pyolecf_value_types.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_libfguid.h` & `libolecf-20240427/pyolecf/pyolecf_libfguid.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_guid.c` & `libolecf-20240427/pyolecf/pyolecf_guid.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_libbfio.h` & `libolecf-20240427/pyolecf/pyolecf_libbfio.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_item.c` & `libolecf-20240427/pyolecf/pyolecf_item.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_integer.c` & `libolecf-20240427/pyolecf/pyolecf_integer.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_property_set.h` & `libolecf-20240427/pyolecf/pyolecf_property_set.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_datetime.h` & `libolecf-20240427/pyolecf/pyolecf_datetime.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_property_set.c` & `libolecf-20240427/pyolecf/pyolecf_property_set.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/Makefile.in` & `libolecf-20240427/pyolecf/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -530,14 +530,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -596,16 +598,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -652,15 +654,16 @@
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBFGUID_LIBADD@
 
 @HAVE_PYTHON_TRUE@pyolecf_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyolecf_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1038,24 +1041,45 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pyolecf_la-pyolecf.Plo
+	-rm -f ./$(DEPDIR)/pyolecf_la-pyolecf_codepage.Plo
+	-rm -f ./$(DEPDIR)/pyolecf_la-pyolecf_datetime.Plo
+	-rm -f ./$(DEPDIR)/pyolecf_la-pyolecf_error.Plo
+	-rm -f ./$(DEPDIR)/pyolecf_la-pyolecf_file.Plo
+	-rm -f ./$(DEPDIR)/pyolecf_la-pyolecf_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pyolecf_la-pyolecf_guid.Plo
+	-rm -f ./$(DEPDIR)/pyolecf_la-pyolecf_integer.Plo
+	-rm -f ./$(DEPDIR)/pyolecf_la-pyolecf_item.Plo
+	-rm -f ./$(DEPDIR)/pyolecf_la-pyolecf_item_types.Plo
+	-rm -f ./$(DEPDIR)/pyolecf_la-pyolecf_items.Plo
+	-rm -f ./$(DEPDIR)/pyolecf_la-pyolecf_property_section.Plo
+	-rm -f ./$(DEPDIR)/pyolecf_la-pyolecf_property_sections.Plo
+	-rm -f ./$(DEPDIR)/pyolecf_la-pyolecf_property_set.Plo
+	-rm -f ./$(DEPDIR)/pyolecf_la-pyolecf_property_set_stream.Plo
+	-rm -f ./$(DEPDIR)/pyolecf_la-pyolecf_property_value.Plo
+	-rm -f ./$(DEPDIR)/pyolecf_la-pyolecf_property_values.Plo
+	-rm -f ./$(DEPDIR)/pyolecf_la-pyolecf_stream.Plo
+	-rm -f ./$(DEPDIR)/pyolecf_la-pyolecf_value_types.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1158,13 +1182,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libolecf-20240212/pyolecf/pyolecf_property_values.h` & `libolecf-20240427/pyolecf/pyolecf_property_values.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_item_types.h` & `libolecf-20240427/pyolecf/pyolecf_item_types.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_property_section.h` & `libolecf-20240427/pyolecf/pyolecf_property_section.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/pyolecf/pyolecf_items.h` & `libolecf-20240427/pyolecf/pyolecf_items.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/Makefile.am` & `libolecf-20240427/Makefile.am`

 * *Files 20% similar despite different names*

```diff
@@ -60,16 +60,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libolecf.pc \
+	libolecf.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libolecf.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -93,19 +100,7 @@
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfole && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwps && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libolecf && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libolecf.pc
-	-rm -f libolecf.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libolecf-20240212/libbfio/libbfio_file_range.h` & `libolecf-20240427/libbfio/libbfio_file_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_file_range_io_handle.c` & `libolecf-20240427/libbfio/libbfio_file_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_support.c` & `libolecf-20240427/libbfio/libbfio_support.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_libcpath.h` & `libolecf-20240427/libbfio/libbfio_libcpath.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcpath header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_error.h` & `libolecf-20240427/libbfio/libbfio_error.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_libclocale.h` & `libolecf-20240427/libbfio/libbfio_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_error.c` & `libolecf-20240427/libbfio/libbfio_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_libuna.h` & `libolecf-20240427/libbfio/libbfio_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_file_io_handle.h` & `libolecf-20240427/libbfio/libbfio_file_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_file_pool.h` & `libolecf-20240427/libbfio/libbfio_file_pool.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_file_range.c` & `libolecf-20240427/libbfio/libbfio_file_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_types.h` & `libolecf-20240427/libbfio/libbfio_types.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_unused.h` & `libolecf-20240427/libbfio/libbfio_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_libcdata.h` & `libolecf-20240427/libbfio/libbfio_libcdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_file.h` & `libolecf-20240427/libbfio/libbfio_file.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/Makefile.am` & `libolecf-20240427/libbfio/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBBFIO
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -38,17 +38,17 @@
 	libbfio_pool.c libbfio_pool.h \
 	libbfio_support.c libbfio_support.h \
 	libbfio_system_string.c libbfio_system_string.h \
 	libbfio_types.h \
 	libbfio_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
```

### Comparing `libolecf-20240212/libbfio/libbfio_libcfile.h` & `libolecf-20240427/libbfio/libbfio_libcfile.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcfile header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_definitions.h` & `libolecf-20240427/libbfio/libbfio_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBBFIO )
 #include <libbfio/definitions.h>
 
 /* The definitions in <libbfio/definitions.h> are copied here
  * for local use of libbfio
  */
 #else
-#define LIBBFIO_VERSION					20221025
+#define LIBBFIO_VERSION					20240414
 
 /* The libbfio version string
  */
-#define LIBBFIO_VERSION_STRING				"20221025"
+#define LIBBFIO_VERSION_STRING				"20240414"
 
 /* The library flags definitions
  */
 enum LIBBFIO_FLAGS
 {
 	/* The IO handle is not managed by the library
 	 */
```

### Comparing `libolecf-20240212/libbfio/libbfio_codepage.h` & `libolecf-20240427/libbfio/libbfio_codepage.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_file_io_handle.c` & `libolecf-20240427/libbfio/libbfio_file_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_support.h` & `libolecf-20240427/libbfio/libbfio_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_memory_range.h` & `libolecf-20240427/libbfio/libbfio_memory_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_file_pool.c` & `libolecf-20240427/libbfio/libbfio_file_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_file_range_io_handle.h` & `libolecf-20240427/libbfio/libbfio_file_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_libcthreads.h` & `libolecf-20240427/libbfio/libbfio_libcthreads.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcthreads header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_system_string.h` & `libolecf-20240427/libbfio/libbfio_system_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_memory_range_io_handle.c` & `libolecf-20240427/libbfio/libbfio_memory_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_handle.c` & `libolecf-20240427/libbfio/libbfio_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_file.c` & `libolecf-20240427/libbfio/libbfio_file.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_handle.h` & `libolecf-20240427/libbfio/libbfio_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_memory_range.c` & `libolecf-20240427/libbfio/libbfio_memory_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_pool.c` & `libolecf-20240427/libbfio/libbfio_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_libcerror.h` & `libolecf-20240427/libbfio/libbfio_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/Makefile.in` & `libolecf-20240427/libbfio/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -479,14 +479,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -545,16 +547,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBBFIO_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCFILE_CPPFLAGS@ \
@@ -585,15 +587,16 @@
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_memory_range_io_handle.c libbfio_memory_range_io_handle.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_pool.c libbfio_pool.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_support.c libbfio_support.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_system_string.c libbfio_system_string.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_types.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -804,24 +807,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libbfio_error.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_support.Plo
+	-rm -f ./$(DEPDIR)/libbfio_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -890,14 +907,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -908,23 +927,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libolecf-20240212/libbfio/libbfio_system_string.c` & `libolecf-20240427/libbfio/libbfio_system_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_memory_range_io_handle.h` & `libolecf-20240427/libbfio/libbfio_memory_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_extern.h` & `libolecf-20240427/libbfio/libbfio_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/libbfio/libbfio_pool.h` & `libolecf-20240427/libbfio/libbfio_pool.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libolecf-20240212/config.guess` & `libolecf-20240427/config.guess`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/dpkg/copyright` & `libolecf-20240427/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/dpkg/control` & `libolecf-20240427/dpkg/control`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/dpkg/rules` & `libolecf-20240427/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/COPYING.LESSER` & `libolecf-20240427/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/configure` & `libolecf-20240427/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libolecf 20240212.
+# Generated by GNU Autoconf 2.71 for libolecf 20240427.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libolecf'
 PACKAGE_TARNAME='libolecf'
-PACKAGE_VERSION='20240212'
-PACKAGE_STRING='libolecf 20240212'
+PACKAGE_VERSION='20240427'
+PACKAGE_STRING='libolecf 20240427'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libolecf.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -678,14 +678,16 @@
 ax_libfuse_spec_requires
 ax_libfuse_pc_libs_private
 LIBFUSE_LIBADD
 LIBFUSE_CPPFLAGS
 HAVE_LIBFUSE
 fuse_LIBS
 fuse_CFLAGS
+fuse3_LIBS
+fuse3_CFLAGS
 HAVE_PYTHON_TESTS_FALSE
 HAVE_PYTHON_TESTS_TRUE
 HAVE_PYTHON_FALSE
 HAVE_PYTHON_TRUE
 PYTHON_PACKAGE_DIR
 PYTHON_LIBRARY_DIR
 pyexecdir
@@ -1115,14 +1117,16 @@
 libfguid_LIBS
 libfole_CFLAGS
 libfole_LIBS
 libfvalue_CFLAGS
 libfvalue_LIBS
 libfwps_CFLAGS
 libfwps_LIBS
+fuse3_CFLAGS
+fuse3_LIBS
 fuse_CFLAGS
 fuse_LIBS'
 
 
 # Initialize some variables set by options.
 ac_init_help=
 ac_init_version=false
@@ -1665,15 +1669,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libolecf 20240212 to adapt to many kinds of systems.
+\`configure' configures libolecf 20240427 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1736,15 +1740,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libolecf 20240212:";;
+     short | recursive ) echo "Configuration of libolecf 20240427:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1923,14 +1927,17 @@
               C compiler flags for libfvalue, overriding pkg-config
   libfvalue_LIBS
               linker flags for libfvalue, overriding pkg-config
   libfwps_CFLAGS
               C compiler flags for libfwps, overriding pkg-config
   libfwps_LIBS
               linker flags for libfwps, overriding pkg-config
+  fuse3_CFLAGS
+              C compiler flags for fuse3, overriding pkg-config
+  fuse3_LIBS  linker flags for fuse3, overriding pkg-config
   fuse_CFLAGS C compiler flags for fuse, overriding pkg-config
   fuse_LIBS   linker flags for fuse, overriding pkg-config
 
 Use these variables to override the choices made by `configure' or to help
 it to find libraries and programs with nonstandard names/locations.
 
 Report bugs to <joachim.metz@gmail.com>.
@@ -1993,15 +2000,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libolecf configure 20240212
+libolecf configure 20240427
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2714,15 +2721,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libolecf $as_me 20240212, which was
+It was created by libolecf $as_me 20240427, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4203,15 +4210,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libolecf'
- VERSION='20240212'
+ VERSION='20240427'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23798,15 +23805,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -24297,15 +24304,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24447,15 +24455,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24549,15 +24557,15 @@
     ac_cv_libcthreads_multi_threading="no"
 else $as_nop
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno
 then :
   ac_cv_libcthreads=no
 else $as_nop
   ac_cv_libcthreads=check
-        if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect
+                if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   if test -d "$ac_cv_with_libcthreads"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -26189,15 +26197,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -26251,47 +26259,52 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_pthread=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_pthread" >&5
 printf "%s\n" "$ac_cv_with_pthread" >&6; }
 
-   if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno
+then :
+  ac_cv_pthread=no
+else $as_nop
+  ac_cv_pthread=check
+                if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
 then :
   if test -d "$ac_cv_with_pthread"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
 else $as_nop
   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_pthread" >&5
 printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_pthread" >&2;}
 
 fi
 
 fi
 
- if test "x$ac_cv_with_pthread" = xno
+fi
+
+    if test "x$ac_cv_pthread" = xcheck
 then :
-  ac_cv_pthread=no
-else $as_nop
-    ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
+        ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
 if test "x$ac_cv_header_pthread_h" = xyes
 then :
   printf "%s\n" "#define HAVE_PTHREAD_H 1" >>confdefs.h
 
 fi
 
 
-  if test "x$ac_cv_header_pthread_h" = xno
+      if test "x$ac_cv_header_pthread_h" = xno
 then :
   ac_cv_pthread=no
 else $as_nop
-     ac_cv_pthread=pthread
+          ac_cv_pthread=pthread
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
 printf %s "checking for pthread_create in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_create+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26325,15 +26338,15 @@
 if test "x$ac_cv_lib_pthread_pthread_create" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
 printf %s "checking for pthread_exit in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_exit+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26367,15 +26380,15 @@
 if test "x$ac_cv_lib_pthread_pthread_exit" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
 printf %s "checking for pthread_join in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_join+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26410,15 +26423,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
 printf %s "checking for pthread_cond_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26452,15 +26465,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
 printf %s "checking for pthread_cond_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26494,15 +26507,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
 printf %s "checking for pthread_cond_broadcast in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_broadcast+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26536,15 +26549,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_broadcast" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
 printf %s "checking for pthread_cond_signal in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_signal+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26578,15 +26591,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_signal" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
 printf %s "checking for pthread_cond_wait in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_wait+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26621,15 +26634,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
 printf %s "checking for pthread_mutex_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26663,15 +26676,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
 printf %s "checking for pthread_mutex_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26705,15 +26718,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
 printf %s "checking for pthread_mutex_lock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_lock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26747,15 +26760,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_lock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
 printf %s "checking for pthread_mutex_trylock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_trylock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26789,15 +26802,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_trylock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
 printf %s "checking for pthread_mutex_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26832,15 +26845,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
 printf %s "checking for pthread_rwlock_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26874,15 +26887,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
 printf %s "checking for pthread_rwlock_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26916,15 +26929,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_rdlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_rdlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26958,15 +26971,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_rdlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_wrlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_wrlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27000,15 +27013,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_wrlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27043,67 +27056,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
+
+fi
+
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
 
 printf "%s\n" "#define HAVE_PTHREAD 1" >>confdefs.h
 
 
 fi
 
- if test "x$ac_cv_pthread" != xno
+  if test "x$ac_cv_pthread" != xno
 then :
   HAVE_PTHREAD=1
 
 else $as_nop
   HAVE_PTHREAD=0
 
 
 fi
 
 
- if test "x$ac_cv_pthread_CPPFLAGS" != "x"
+  if test "x$ac_cv_pthread_CPPFLAGS" != "x"
 then :
   PTHREAD_CPPFLAGS=$ac_cv_pthread_CPPFLAGS
 
 
 fi
- if test "x$ac_cv_pthread_LIBADD" != "x"
+  if test "x$ac_cv_pthread_LIBADD" != "x"
 then :
   PTHREAD_LIBADD=$ac_cv_pthread_LIBADD
 
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
   ax_pthread_pc_libs_private=-lpthread
 
 
 fi
 
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread
 else $as_nop
   ac_cv_libcthreads_multi_threading="winapi"
 fi
 
   if test "x$ac_cv_libcthreads_multi_threading" != xno
 then :
-  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local
 else $as_nop
   ac_cv_libcthreads=no
 fi
 
@@ -27191,15 +27213,15 @@
 printf "%s\n" "$ac_cv_with_libcdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno
 then :
   ac_cv_libcdata=no
 else $as_nop
   ac_cv_libcdata=check
-        if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect
+                if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   if test -d "$ac_cv_with_libcdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -30970,15 +30992,16 @@
 fi
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes
+
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31003,15 +31026,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31081,15 +31104,15 @@
 printf "%s\n" "$ac_cv_with_libclocale" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno
 then :
   ac_cv_libclocale=no
 else $as_nop
   ac_cv_libclocale=check
-        if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect
+                if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   if test -d "$ac_cv_with_libclocale"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31636,15 +31659,16 @@
 fi
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes
+
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31800,15 +31824,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31878,15 +31902,15 @@
 printf "%s\n" "$ac_cv_with_libcnotify" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno
 then :
   ac_cv_libcnotify=no
 else $as_nop
   ac_cv_libcnotify=check
-        if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect
+                if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   if test -d "$ac_cv_with_libcnotify"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -32336,15 +32360,16 @@
 fi
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes
+
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -32399,15 +32424,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32477,15 +32502,15 @@
 printf "%s\n" "$ac_cv_with_libcsplit" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno
 then :
   ac_cv_libcsplit=no
 else $as_nop
   ac_cv_libcsplit=check
-        if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect
+                if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   if test -d "$ac_cv_with_libcsplit"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -33200,15 +33225,16 @@
 
 fi
 
         ac_cv_libcsplit_LIBADD="-lcsplit"
 fi
 
 fi
-    if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes
+
+    if test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcsplit in directory: $ac_cv_with_libcsplit
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -33233,15 +33259,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33311,15 +33337,15 @@
 printf "%s\n" "$ac_cv_with_libuna" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno
 then :
   ac_cv_libuna=no
 else $as_nop
   ac_cv_libuna=check
-        if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect
+                if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   if test -d "$ac_cv_with_libuna"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -40521,15 +40547,16 @@
   ac_cv_libuna=no
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes
+
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -40554,15 +40581,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40632,15 +40659,15 @@
 printf "%s\n" "$ac_cv_with_libcfile" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno
 then :
   ac_cv_libcfile=no
 else $as_nop
   ac_cv_libcfile=check
-        if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect
+                if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   if test -d "$ac_cv_with_libcfile"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -41821,15 +41848,16 @@
 
 fi
 
         ac_cv_libcfile_LIBADD="-lcfile"
 fi
 
 fi
-    if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes
+
+    if test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcfile in directory: $ac_cv_with_libcfile
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -42143,15 +42171,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: unlink
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCFILE 1" >>confdefs.h
@@ -42221,15 +42249,15 @@
 printf "%s\n" "$ac_cv_with_libcpath" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno
 then :
   ac_cv_libcpath=no
 else $as_nop
   ac_cv_libcpath=check
-        if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect
+                if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   if test -d "$ac_cv_with_libcpath"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -43026,15 +43054,16 @@
 
 fi
 
         ac_cv_libcpath_LIBADD="-lcpath"
 fi
 
 fi
-    if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes
+
+    if test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcpath in directory: $ac_cv_with_libcpath
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43224,15 +43253,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43302,15 +43331,15 @@
 printf "%s\n" "$ac_cv_with_libbfio" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno
 then :
   ac_cv_libbfio=no
 else $as_nop
   ac_cv_libbfio=check
-        if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect
+                if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   if test -d "$ac_cv_with_libbfio"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -45420,15 +45449,16 @@
 
 fi
 
         ac_cv_libbfio_LIBADD="-lbfio"
 fi
 
 fi
-    if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes
+
+    if test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libbfio in directory: $ac_cv_with_libbfio
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -45453,15 +45483,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45531,15 +45561,15 @@
 printf "%s\n" "$ac_cv_with_libfdatetime" >&6; }
 
   if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno
 then :
   ac_cv_libfdatetime=no
 else $as_nop
   ac_cv_libfdatetime=check
-        if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect
+                if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   if test -d "$ac_cv_with_libfdatetime"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -48975,15 +49005,16 @@
 fi
 
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes
+
+    if test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -49008,15 +49039,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdatetime" != xyes
 then :
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATETIME 1" >>confdefs.h
@@ -49086,15 +49117,15 @@
 printf "%s\n" "$ac_cv_with_libfguid" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno
 then :
   ac_cv_libfguid=no
 else $as_nop
   ac_cv_libfguid=check
-        if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect
+                if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   if test -d "$ac_cv_with_libfguid"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -49668,15 +49699,16 @@
 fi
 
 
         ac_cv_libfguid_LIBADD="-lfguid"
 fi
 
 fi
-    if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes
+
+    if test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfguid in directory: $ac_cv_with_libfguid
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -49701,15 +49733,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfguid" != xyes
 then :
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFGUID 1" >>confdefs.h
@@ -49779,15 +49811,15 @@
 printf "%s\n" "$ac_cv_with_libfole" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfole" = xno
 then :
   ac_cv_libfole=no
 else $as_nop
   ac_cv_libfole=check
-        if test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect
+                if test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect && test "x$ac_cv_with_libfole" != xyes
 then :
   if test -d "$ac_cv_with_libfole"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfole}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfole}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -49941,15 +49973,16 @@
 
 
 
         ac_cv_libfole_LIBADD="-lfole"
 fi
 
 fi
-    if test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect && test "x$ac_cv_libfole" != xyes
+
+    if test "x$ac_cv_libfole" != xyes && test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect && test "x$ac_cv_with_libfole" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfole in directory: $ac_cv_with_libfole
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -49974,15 +50007,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfole" != xyes
 then :
 
-  ac_cv_libfole_CPPFLAGS="-I../libfole";
+  ac_cv_libfole_CPPFLAGS="-I../libfole -I\$(top_srcdir)/libfole";
   ac_cv_libfole_LIBADD="../libfole/libfole.la";
 
   ac_cv_libfole=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFOLE 1" >>confdefs.h
@@ -50052,15 +50085,15 @@
 printf "%s\n" "$ac_cv_with_libfvalue" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfvalue" = xno
 then :
   ac_cv_libfvalue=no
 else $as_nop
   ac_cv_libfvalue=check
-        if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect
+                if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
 then :
   if test -d "$ac_cv_with_libfvalue"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfvalue}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfvalue}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -54366,15 +54399,16 @@
 fi
 
 
         ac_cv_libfvalue_LIBADD="-lfvalue"
 fi
 
 fi
-    if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_libfvalue" != xyes
+
+    if test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfvalue in directory: $ac_cv_with_libfvalue
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -54399,15 +54433,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfvalue" != xyes
 then :
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFVALUE 1" >>confdefs.h
@@ -54477,15 +54511,15 @@
 printf "%s\n" "$ac_cv_with_libfwps" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfwps" = xno
 then :
   ac_cv_libfwps=no
 else $as_nop
   ac_cv_libfwps=check
-        if test "x$ac_cv_with_libfwps" != x && test "x$ac_cv_with_libfwps" != xauto-detect
+                if test "x$ac_cv_with_libfwps" != x && test "x$ac_cv_with_libfwps" != xauto-detect && test "x$ac_cv_with_libfwps" != xyes
 then :
   if test -d "$ac_cv_with_libfwps"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfwps}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfwps}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -54496,44 +54530,44 @@
 fi
 
 else $as_nop
         if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
 then :
 
 pkg_failed=no
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps >= 20230711" >&5
-printf %s "checking for libfwps >= 20230711... " >&6; }
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps >= 20240224" >&5
+printf %s "checking for libfwps >= 20240224... " >&6; }
 
 if test -n "$libfwps_CFLAGS"; then
     pkg_cv_libfwps_CFLAGS="$libfwps_CFLAGS"
  elif test -n "$PKG_CONFIG"; then
     if test -n "$PKG_CONFIG" && \
-    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libfwps >= 20230711\""; } >&5
-  ($PKG_CONFIG --exists --print-errors "libfwps >= 20230711") 2>&5
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libfwps >= 20240224\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "libfwps >= 20240224") 2>&5
   ac_status=$?
   printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
   test $ac_status = 0; }; then
-  pkg_cv_libfwps_CFLAGS=`$PKG_CONFIG --cflags "libfwps >= 20230711" 2>/dev/null`
+  pkg_cv_libfwps_CFLAGS=`$PKG_CONFIG --cflags "libfwps >= 20240224" 2>/dev/null`
 		      test "x$?" != "x0" && pkg_failed=yes
 else
   pkg_failed=yes
 fi
  else
     pkg_failed=untried
 fi
 if test -n "$libfwps_LIBS"; then
     pkg_cv_libfwps_LIBS="$libfwps_LIBS"
  elif test -n "$PKG_CONFIG"; then
     if test -n "$PKG_CONFIG" && \
-    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libfwps >= 20230711\""; } >&5
-  ($PKG_CONFIG --exists --print-errors "libfwps >= 20230711") 2>&5
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libfwps >= 20240224\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "libfwps >= 20240224") 2>&5
   ac_status=$?
   printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
   test $ac_status = 0; }; then
-  pkg_cv_libfwps_LIBS=`$PKG_CONFIG --libs "libfwps >= 20230711" 2>/dev/null`
+  pkg_cv_libfwps_LIBS=`$PKG_CONFIG --libs "libfwps >= 20240224" 2>/dev/null`
 		      test "x$?" != "x0" && pkg_failed=yes
 else
   pkg_failed=yes
 fi
  else
     pkg_failed=untried
 fi
@@ -54546,17 +54580,17 @@
 
 if $PKG_CONFIG --atleast-pkgconfig-version 0.20; then
         _pkg_short_errors_supported=yes
 else
         _pkg_short_errors_supported=no
 fi
         if test $_pkg_short_errors_supported = yes; then
-                libfwps_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "libfwps >= 20230711" 2>&1`
+                libfwps_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "libfwps >= 20240224" 2>&1`
         else
-                libfwps_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "libfwps >= 20230711" 2>&1`
+                libfwps_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "libfwps >= 20240224" 2>&1`
         fi
         # Put the nasty error message in config.log where it belongs
         echo "$libfwps_PKG_ERRORS" >&5
 
         ac_cv_libfwps=check
 elif test $pkg_failed = untried; then
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
@@ -55016,14 +55050,182 @@
 then :
   ac_cv_libfwps_dummy=yes
 else $as_nop
   ac_cv_libfwps=no
 fi
 
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps_record_get_utf8_entry_name_size in -lfwps" >&5
+printf %s "checking for libfwps_record_get_utf8_entry_name_size in -lfwps... " >&6; }
+if test ${ac_cv_lib_fwps_libfwps_record_get_utf8_entry_name_size+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfwps  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libfwps_record_get_utf8_entry_name_size ();
+int
+main (void)
+{
+return libfwps_record_get_utf8_entry_name_size ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fwps_libfwps_record_get_utf8_entry_name_size=yes
+else $as_nop
+  ac_cv_lib_fwps_libfwps_record_get_utf8_entry_name_size=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fwps_libfwps_record_get_utf8_entry_name_size" >&5
+printf "%s\n" "$ac_cv_lib_fwps_libfwps_record_get_utf8_entry_name_size" >&6; }
+if test "x$ac_cv_lib_fwps_libfwps_record_get_utf8_entry_name_size" = xyes
+then :
+  ac_cv_libfwps_dummy=yes
+else $as_nop
+  ac_cv_libfwps=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps_record_get_utf8_entry_name in -lfwps" >&5
+printf %s "checking for libfwps_record_get_utf8_entry_name in -lfwps... " >&6; }
+if test ${ac_cv_lib_fwps_libfwps_record_get_utf8_entry_name+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfwps  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libfwps_record_get_utf8_entry_name ();
+int
+main (void)
+{
+return libfwps_record_get_utf8_entry_name ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fwps_libfwps_record_get_utf8_entry_name=yes
+else $as_nop
+  ac_cv_lib_fwps_libfwps_record_get_utf8_entry_name=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fwps_libfwps_record_get_utf8_entry_name" >&5
+printf "%s\n" "$ac_cv_lib_fwps_libfwps_record_get_utf8_entry_name" >&6; }
+if test "x$ac_cv_lib_fwps_libfwps_record_get_utf8_entry_name" = xyes
+then :
+  ac_cv_libfwps_dummy=yes
+else $as_nop
+  ac_cv_libfwps=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps_record_get_utf16_entry_name_size in -lfwps" >&5
+printf %s "checking for libfwps_record_get_utf16_entry_name_size in -lfwps... " >&6; }
+if test ${ac_cv_lib_fwps_libfwps_record_get_utf16_entry_name_size+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfwps  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libfwps_record_get_utf16_entry_name_size ();
+int
+main (void)
+{
+return libfwps_record_get_utf16_entry_name_size ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fwps_libfwps_record_get_utf16_entry_name_size=yes
+else $as_nop
+  ac_cv_lib_fwps_libfwps_record_get_utf16_entry_name_size=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fwps_libfwps_record_get_utf16_entry_name_size" >&5
+printf "%s\n" "$ac_cv_lib_fwps_libfwps_record_get_utf16_entry_name_size" >&6; }
+if test "x$ac_cv_lib_fwps_libfwps_record_get_utf16_entry_name_size" = xyes
+then :
+  ac_cv_libfwps_dummy=yes
+else $as_nop
+  ac_cv_libfwps=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps_record_get_utf16_entry_name in -lfwps" >&5
+printf %s "checking for libfwps_record_get_utf16_entry_name in -lfwps... " >&6; }
+if test ${ac_cv_lib_fwps_libfwps_record_get_utf16_entry_name+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfwps  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libfwps_record_get_utf16_entry_name ();
+int
+main (void)
+{
+return libfwps_record_get_utf16_entry_name ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fwps_libfwps_record_get_utf16_entry_name=yes
+else $as_nop
+  ac_cv_lib_fwps_libfwps_record_get_utf16_entry_name=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fwps_libfwps_record_get_utf16_entry_name" >&5
+printf "%s\n" "$ac_cv_lib_fwps_libfwps_record_get_utf16_entry_name" >&6; }
+if test "x$ac_cv_lib_fwps_libfwps_record_get_utf16_entry_name" = xyes
+then :
+  ac_cv_libfwps_dummy=yes
+else $as_nop
+  ac_cv_libfwps=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps_record_get_entry_type in -lfwps" >&5
 printf %s "checking for libfwps_record_get_entry_type in -lfwps... " >&6; }
 if test ${ac_cv_lib_fwps_libfwps_record_get_entry_type+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -55058,14 +55260,182 @@
 if test "x$ac_cv_lib_fwps_libfwps_record_get_entry_type" = xyes
 then :
   ac_cv_libfwps_dummy=yes
 else $as_nop
   ac_cv_libfwps=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps_record_get_utf8_value_name_size in -lfwps" >&5
+printf %s "checking for libfwps_record_get_utf8_value_name_size in -lfwps... " >&6; }
+if test ${ac_cv_lib_fwps_libfwps_record_get_utf8_value_name_size+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfwps  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libfwps_record_get_utf8_value_name_size ();
+int
+main (void)
+{
+return libfwps_record_get_utf8_value_name_size ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fwps_libfwps_record_get_utf8_value_name_size=yes
+else $as_nop
+  ac_cv_lib_fwps_libfwps_record_get_utf8_value_name_size=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fwps_libfwps_record_get_utf8_value_name_size" >&5
+printf "%s\n" "$ac_cv_lib_fwps_libfwps_record_get_utf8_value_name_size" >&6; }
+if test "x$ac_cv_lib_fwps_libfwps_record_get_utf8_value_name_size" = xyes
+then :
+  ac_cv_libfwps_dummy=yes
+else $as_nop
+  ac_cv_libfwps=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps_record_get_utf8_value_name in -lfwps" >&5
+printf %s "checking for libfwps_record_get_utf8_value_name in -lfwps... " >&6; }
+if test ${ac_cv_lib_fwps_libfwps_record_get_utf8_value_name+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfwps  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libfwps_record_get_utf8_value_name ();
+int
+main (void)
+{
+return libfwps_record_get_utf8_value_name ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fwps_libfwps_record_get_utf8_value_name=yes
+else $as_nop
+  ac_cv_lib_fwps_libfwps_record_get_utf8_value_name=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fwps_libfwps_record_get_utf8_value_name" >&5
+printf "%s\n" "$ac_cv_lib_fwps_libfwps_record_get_utf8_value_name" >&6; }
+if test "x$ac_cv_lib_fwps_libfwps_record_get_utf8_value_name" = xyes
+then :
+  ac_cv_libfwps_dummy=yes
+else $as_nop
+  ac_cv_libfwps=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps_record_get_utf16_value_name_size in -lfwps" >&5
+printf %s "checking for libfwps_record_get_utf16_value_name_size in -lfwps... " >&6; }
+if test ${ac_cv_lib_fwps_libfwps_record_get_utf16_value_name_size+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfwps  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libfwps_record_get_utf16_value_name_size ();
+int
+main (void)
+{
+return libfwps_record_get_utf16_value_name_size ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fwps_libfwps_record_get_utf16_value_name_size=yes
+else $as_nop
+  ac_cv_lib_fwps_libfwps_record_get_utf16_value_name_size=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fwps_libfwps_record_get_utf16_value_name_size" >&5
+printf "%s\n" "$ac_cv_lib_fwps_libfwps_record_get_utf16_value_name_size" >&6; }
+if test "x$ac_cv_lib_fwps_libfwps_record_get_utf16_value_name_size" = xyes
+then :
+  ac_cv_libfwps_dummy=yes
+else $as_nop
+  ac_cv_libfwps=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps_record_get_utf16_value_name in -lfwps" >&5
+printf %s "checking for libfwps_record_get_utf16_value_name in -lfwps... " >&6; }
+if test ${ac_cv_lib_fwps_libfwps_record_get_utf16_value_name+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfwps  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libfwps_record_get_utf16_value_name ();
+int
+main (void)
+{
+return libfwps_record_get_utf16_value_name ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fwps_libfwps_record_get_utf16_value_name=yes
+else $as_nop
+  ac_cv_lib_fwps_libfwps_record_get_utf16_value_name=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fwps_libfwps_record_get_utf16_value_name" >&5
+printf "%s\n" "$ac_cv_lib_fwps_libfwps_record_get_utf16_value_name" >&6; }
+if test "x$ac_cv_lib_fwps_libfwps_record_get_utf16_value_name" = xyes
+then :
+  ac_cv_libfwps_dummy=yes
+else $as_nop
+  ac_cv_libfwps=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps_record_get_value_type in -lfwps" >&5
 printf %s "checking for libfwps_record_get_value_type in -lfwps... " >&6; }
 if test ${ac_cv_lib_fwps_libfwps_record_get_value_type+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -55101,14 +55471,98 @@
 then :
   ac_cv_libfwps_dummy=yes
 else $as_nop
   ac_cv_libfwps=no
 fi
 
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps_record_get_data in -lfwps" >&5
+printf %s "checking for libfwps_record_get_data in -lfwps... " >&6; }
+if test ${ac_cv_lib_fwps_libfwps_record_get_data+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfwps  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libfwps_record_get_data ();
+int
+main (void)
+{
+return libfwps_record_get_data ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fwps_libfwps_record_get_data=yes
+else $as_nop
+  ac_cv_lib_fwps_libfwps_record_get_data=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fwps_libfwps_record_get_data" >&5
+printf "%s\n" "$ac_cv_lib_fwps_libfwps_record_get_data" >&6; }
+if test "x$ac_cv_lib_fwps_libfwps_record_get_data" = xyes
+then :
+  ac_cv_libfwps_dummy=yes
+else $as_nop
+  ac_cv_libfwps=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps_record_get_data_size in -lfwps" >&5
+printf %s "checking for libfwps_record_get_data_size in -lfwps... " >&6; }
+if test ${ac_cv_lib_fwps_libfwps_record_get_data_size+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfwps  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libfwps_record_get_data_size ();
+int
+main (void)
+{
+return libfwps_record_get_data_size ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fwps_libfwps_record_get_data_size=yes
+else $as_nop
+  ac_cv_lib_fwps_libfwps_record_get_data_size=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fwps_libfwps_record_get_data_size" >&5
+printf "%s\n" "$ac_cv_lib_fwps_libfwps_record_get_data_size" >&6; }
+if test "x$ac_cv_lib_fwps_libfwps_record_get_data_size" = xyes
+then :
+  ac_cv_libfwps_dummy=yes
+else $as_nop
+  ac_cv_libfwps=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps_record_get_data_as_boolean in -lfwps" >&5
 printf %s "checking for libfwps_record_get_data_as_boolean in -lfwps... " >&6; }
 if test ${ac_cv_lib_fwps_libfwps_record_get_data_as_boolean+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -55778,15 +56232,15 @@
 fi
 
 
         ac_cv_libfwps_LIBADD="-lfwps"
 fi
 
 fi
-    if test "x$ac_cv_with_libfwps" != x && test "x$ac_cv_with_libfwps" != xauto-detect && test "x$ac_cv_libfwps" != xyes
+    if test "x$ac_cv_libfwps" != xyes && test "x$ac_cv_with_libfwps" != x && test "x$ac_cv_with_libfwps" != xauto-detect && test "x$ac_cv_with_libfwps" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfwps in directory: $ac_cv_with_libfwps
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -55901,15 +56355,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfwps" != xyes
 then :
 
-  ac_cv_libfwps_CPPFLAGS="-I../libfwps";
+  ac_cv_libfwps_CPPFLAGS="-I../libfwps -I\$(top_srcdir)/libfwps";
   ac_cv_libfwps_LIBADD="../libfwps/libfwps.la";
 
   ac_cv_libfwps=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFWPS 1" >>confdefs.h
@@ -56220,16 +56674,20 @@
         PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for Python libraries" >&5
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
-        case $host_os in #(
-  cygwin*) :
+        case $build in #(
+  *-*-cygwin*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-msys*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
@@ -56387,33 +56845,107 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_libfuse=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_libfuse" >&5
 printf "%s\n" "$ac_cv_with_libfuse" >&6; }
 
-      if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno
+then :
+  ac_cv_libfuse=no
+else $as_nop
+              if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
 then :
   if test -d "$ac_cv_with_libfuse"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
 else $as_nop
-  { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_libfuse" >&5
-printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_libfuse" >&2;}
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "no such directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
+else $as_nop
+        if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+then :
+
+pkg_failed=no
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse3 >= 3.0" >&5
+printf %s "checking for fuse3 >= 3.0... " >&6; }
+
+if test -n "$fuse3_CFLAGS"; then
+    pkg_cv_fuse3_CFLAGS="$fuse3_CFLAGS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_CFLAGS=`$PKG_CONFIG --cflags "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
+fi
+if test -n "$fuse3_LIBS"; then
+    pkg_cv_fuse3_LIBS="$fuse3_LIBS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_LIBS=`$PKG_CONFIG --libs "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
+fi
+
+
+
+if test $pkg_failed = yes; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
 
+if $PKG_CONFIG --atleast-pkgconfig-version 0.20; then
+        _pkg_short_errors_supported=yes
+else
+        _pkg_short_errors_supported=no
 fi
+        if test $_pkg_short_errors_supported = yes; then
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        else
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        fi
+        # Put the nasty error message in config.log where it belongs
+        echo "$fuse3_PKG_ERRORS" >&5
 
+        ac_cv_libfuse=no
+elif test $pkg_failed = untried; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
+        ac_cv_libfuse=no
+else
+        fuse3_CFLAGS=$pkg_cv_fuse3_CFLAGS
+        fuse3_LIBS=$pkg_cv_fuse3_LIBS
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
+printf "%s\n" "yes" >&6; }
+        ac_cv_libfuse=libfuse3
 fi
 
-  if test "x$ac_cv_with_libfuse" = xno
-then :
-  ac_cv_libfuse=no
-else $as_nop
-      if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+        if test "x$ac_cv_libfuse" = xno
 then :
 
 pkg_failed=no
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse >= 2.6" >&5
 printf %s "checking for fuse >= 2.6... " >&6; }
 
 if test -n "$fuse_CFLAGS"; then
@@ -56481,51 +57013,110 @@
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
 printf "%s\n" "yes" >&6; }
         ac_cv_libfuse=libfuse
 fi
 
 fi
 
-    if test "x$ac_cv_libfuse" = xlibfuse
+        if test "x$ac_cv_libfuse" = xlibfuse3
 then :
-  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
-else $as_nop
-               for ac_header in fuse.h
-do :
-  ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"
+fi
+
+        if test "x$ac_cv_libfuse" = xlibfuse
+then :
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
+fi
+
+fi
+
+fi
+
+    backup_CPPFLAGS="$CPPFLAGS"
+
+        if test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3
+then :
+
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
- ac_cv_header_fuse_h=yes
-else $as_nop
-  ac_cv_header_fuse_h=no
+
 fi
 
-done
 
-                  if test "x$ac_cv_header_fuse_h" = xno
+      if test "x$ac_cv_header_fuse_h" = xyes
 then :
-  { ac_cv_header_fuse_h=; unset ac_cv_header_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+  ac_cv_libfuse=libfuse3
+else $as_nop
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
+        if test "x$ac_cv_header_fuse_h" = xyes
+then :
+  ac_cv_libfuse=libfuse
+fi
+
 fi
 
       if test "x$ac_cv_header_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
-          ac_cv_libfuse=libfuse
+          { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_invalidate in -lfuse" >&5
+printf %s "checking for fuse_invalidate in -lfuse... " >&6; }
+if test ${ac_cv_lib_fuse_fuse_invalidate+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfuse  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char fuse_invalidate ();
+int
+main (void)
+{
+return fuse_invalidate ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fuse_fuse_invalidate=yes
+else $as_nop
+  ac_cv_lib_fuse_fuse_invalidate=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fuse_fuse_invalidate" >&5
+printf "%s\n" "$ac_cv_lib_fuse_fuse_invalidate" >&6; }
+if test "x$ac_cv_lib_fuse_fuse_invalidate" = xyes
+then :
+  ac_cv_libfuse=libfuse
+else $as_nop
+  ac_cv_libfuse=libfuse3
+fi
+
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -lfuse" >&5
 printf %s "checking for fuse_daemonize in -lfuse... " >&6; }
 if test ${ac_cv_lib_fuse_fuse_daemonize+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
@@ -56688,45 +57279,38 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
 
+        if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ac_cv_libfuse_LIBADD="-lfuse3"
+else $as_nop
+  ac_cv_libfuse_LIBADD="-lfuse"
 fi
 
 fi
 
-        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
-then :
-  CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
-      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
-if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
-then :
-  printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
-
 fi
 
-
-            if test "x$ac_cv_header_osxfuse_fuse_h" = xno
+        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
 then :
-  { ac_cv_header_osxfuse_fuse_h=; unset ac_cv_header_osxfuse_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
+      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
-fi
-
       if test "x$ac_cv_header_osxfuse_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
           ac_cv_libfuse=libosxfuse
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -losxfuse" >&5
@@ -56894,29 +57478,49 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
 
 fi
 
 fi
 
+    if test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported libfuse in directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
+
+    CPPFLAGS="$backup_CPPFLAGS"
+
 fi
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBFUSE 1" >>confdefs.h
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+
+printf "%s\n" "#define HAVE_LIBFUSE3 1" >>confdefs.h
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBOSXFUSE 1" >>confdefs.h
 
 
 fi
@@ -56947,14 +57551,20 @@
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
   ax_libfuse_pc_libs_private=-lfuse
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_pc_libs_private=-lfuse3
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
   ax_libfuse_pc_libs_private=-losxfuse
 
 
 fi
 
@@ -56962,14 +57572,22 @@
 then :
   ax_libfuse_spec_requires=fuse-libs
 
     ax_libfuse_spec_build_requires=fuse-devel
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_spec_requires=fuse3-libs
+
+    ax_libfuse_spec_build_requires=fuse3-devel
+
+
+fi
 
 
 ac_fn_c_check_header_compile "$LINENO" "signal.h" "ac_cv_header_signal_h" "$ac_includes_default"
 if test "x$ac_cv_header_signal_h" = xyes
 then :
   printf "%s\n" "#define HAVE_SIGNAL_H 1" >>confdefs.h
 
@@ -57918,15 +58536,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libolecf $as_me 20240212, which was
+This file was extended by libolecf $as_me 20240427, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -57986,15 +58604,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libolecf config.status 20240212
+libolecf config.status 20240427
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libolecf-20240212/compile` & `libolecf-20240427/compile`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/missing` & `libolecf-20240427/missing`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/libolecf.sln` & `libolecf-20240427/msvscpp/libolecf.sln`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/olecf_test_notify/olecf_test_notify.vcproj` & `libolecf-20240427/msvscpp/olecf_test_notify/olecf_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/libfole/libfole.vcproj` & `libolecf-20240427/msvscpp/libfole/libfole.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/olecf_test_property_set/olecf_test_property_set.vcproj` & `libolecf-20240427/msvscpp/olecf_test_property_set/olecf_test_property_set.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/libolecf/libolecf.vcproj` & `libolecf-20240427/msvscpp/libolecf/libolecf.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/olecf_test_tools_output/olecf_test_tools_output.vcproj` & `libolecf-20240427/msvscpp/olecf_test_tools_output/olecf_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/olecfinfo/olecfinfo.vcproj` & `libolecf-20240427/msvscpp/olecfinfo/olecfinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/olecfmount/olecfmount.vcproj` & `libolecf-20240427/msvscpp/olecfmount/olecfmount.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/libfguid/libfguid.vcproj` & `libolecf-20240427/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/libfwps/libfwps.vcproj` & `libolecf-20240427/msvscpp/libfwps/libfwps.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/libclocale/libclocale.vcproj` & `libolecf-20240427/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/pyolecf/pyolecf.vcproj` & `libolecf-20240427/msvscpp/pyolecf/pyolecf.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/Makefile.am` & `libolecf-20240427/msvscpp/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -35,13 +35,11 @@
 	olecfmount/olecfmount.vcproj \
 	pyolecf/pyolecf.vcproj \
 	libolecf.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libolecf-20240212/msvscpp/libbfio/libbfio.vcproj` & `libolecf-20240427/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/olecf_test_item/olecf_test_item.vcproj` & `libolecf-20240427/msvscpp/olecf_test_item/olecf_test_item.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/olecfexport/olecfexport.vcproj` & `libolecf-20240427/msvscpp/olecfexport/olecfexport.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/olecf_test_file_header/olecf_test_file_header.vcproj` & `libolecf-20240427/msvscpp/olecf_test_file_header/olecf_test_file_header.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/olecf_test_io_handle/olecf_test_io_handle.vcproj` & `libolecf-20240427/msvscpp/olecf_test_io_handle/olecf_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/olecf_test_file/olecf_test_file.vcproj` & `libolecf-20240427/msvscpp/olecf_test_file/olecf_test_file.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/olecf_test_error/olecf_test_error.vcproj` & `libolecf-20240427/msvscpp/olecf_test_error/olecf_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/libcfile/libcfile.vcproj` & `libolecf-20240427/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/olecf_test_property_value/olecf_test_property_value.vcproj` & `libolecf-20240427/msvscpp/olecf_test_property_value/olecf_test_property_value.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/olecf_test_allocation_table/olecf_test_allocation_table.vcproj` & `libolecf-20240427/msvscpp/olecf_test_allocation_table/olecf_test_allocation_table.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/libcdata/libcdata.vcproj` & `libolecf-20240427/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/olecf_test_tools_signal/olecf_test_tools_signal.vcproj` & `libolecf-20240427/msvscpp/olecf_test_tools_signal/olecf_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/olecf_test_property_section/olecf_test_property_section.vcproj` & `libolecf-20240427/msvscpp/olecf_test_property_section/olecf_test_property_section.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/olecf_test_tools_info_handle/olecf_test_tools_info_handle.vcproj` & `libolecf-20240427/msvscpp/olecf_test_tools_info_handle/olecf_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/libcthreads/libcthreads.vcproj` & `libolecf-20240427/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/libcpath/libcpath.vcproj` & `libolecf-20240427/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/olecf_test_support/olecf_test_support.vcproj` & `libolecf-20240427/msvscpp/olecf_test_support/olecf_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/libcsplit/libcsplit.vcproj` & `libolecf-20240427/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/libuna/libuna.vcproj` & `libolecf-20240427/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/Makefile.in` & `libolecf-20240427/msvscpp/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -396,14 +396,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -502,15 +504,16 @@
 	olecfmount/olecfmount.vcproj \
 	pyolecf/pyolecf.vcproj \
 	libolecf.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -614,23 +617,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -709,13 +714,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libolecf-20240212/msvscpp/libfvalue/libfvalue.vcproj` & `libolecf-20240427/msvscpp/libfvalue/libfvalue.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/olecf_test_directory_entry/olecf_test_directory_entry.vcproj` & `libolecf-20240427/msvscpp/olecf_test_directory_entry/olecf_test_directory_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/libcnotify/libcnotify.vcproj` & `libolecf-20240427/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/libcerror/libcerror.vcproj` & `libolecf-20240427/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/msvscpp/libfdatetime/libfdatetime.vcproj` & `libolecf-20240427/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/mount_dokan.c` & `libolecf-20240427/olecftools/mount_dokan.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/mount_file_system.h` & `libolecf-20240427/olecftools/mount_file_system.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecftools_libclocale.h` & `libolecf-20240427/olecftools/olecftools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/mount_fuse.c` & `libolecf-20240427/olecftools/mount_fuse.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/info_handle.h` & `libolecf-20240427/olecftools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecftools_libcpath.h` & `libolecf-20240427/olecftools/olecftools_libcpath.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/mount_dokan.h` & `libolecf-20240427/olecftools/mount_dokan.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecftools_signal.c` & `libolecf-20240427/olecftools/olecftools_signal.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/mount_file_system.c` & `libolecf-20240427/olecftools/mount_file_system.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecftools_output.c` & `libolecf-20240427/olecftools/olecftools_output.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecftools_unused.h` & `libolecf-20240427/olecftools/olecftools_unused.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecftools_libfole.h` & `libolecf-20240427/olecftools/olecftools_libfole.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecftools_getopt.h` & `libolecf-20240427/olecftools/olecftools_getopt.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/Makefile.am` & `libolecf-20240427/olecftools/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -110,20 +110,18 @@
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libolecf/libolecf.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on olecfexport ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(olecfexport_SOURCES)
 	@echo "Running splint on olecfinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(olecfinfo_SOURCES)
 	@echo "Running splint on olecfmount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(olecfmount_SOURCES)
```

### Comparing `libolecf-20240212/olecftools/olecftools_libfguid.h` & `libolecf-20240427/olecftools/olecftools_libfguid.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecftools_signal.h` & `libolecf-20240427/olecftools/olecftools_signal.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecftools_libcfile.h` & `libolecf-20240427/olecftools/olecftools_libcfile.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecftools_getopt.c` & `libolecf-20240427/olecftools/olecftools_getopt.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/mount_file_entry.c` & `libolecf-20240427/olecftools/mount_file_entry.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/info_handle.c` & `libolecf-20240427/olecftools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/export_handle.c` & `libolecf-20240427/olecftools/export_handle.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/mount_file_entry.h` & `libolecf-20240427/olecftools/mount_file_entry.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecftools_i18n.h` & `libolecf-20240427/olecftools/olecftools_i18n.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecfinfo.c` & `libolecf-20240427/olecftools/olecfinfo.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecfexport.c` & `libolecf-20240427/olecftools/olecfexport.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/log_handle.c` & `libolecf-20240427/olecftools/log_handle.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecfmount.c` & `libolecf-20240427/olecftools/olecfmount.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/mount_handle.h` & `libolecf-20240427/olecftools/mount_handle.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecftools_libcnotify.h` & `libolecf-20240427/olecftools/olecftools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecftools_libfdatetime.h` & `libolecf-20240427/olecftools/olecftools_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecftools_output.h` & `libolecf-20240427/olecftools/olecftools_output.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/export_handle.h` & `libolecf-20240427/olecftools/export_handle.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/mount_handle.c` & `libolecf-20240427/olecftools/mount_handle.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecftools_libolecf.h` & `libolecf-20240427/olecftools/olecftools_libolecf.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecftools_libbfio.h` & `libolecf-20240427/olecftools/olecftools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecftools_libcerror.h` & `libolecf-20240427/olecftools/olecftools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/Makefile.in` & `libolecf-20240427/olecftools/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -471,14 +471,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -537,16 +539,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -646,15 +648,16 @@
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libolecf/libolecf.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -917,23 +920,39 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/export_handle.Po
+	-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/log_handle.Po
+	-rm -f ./$(DEPDIR)/mount_dokan.Po
+	-rm -f ./$(DEPDIR)/mount_file_entry.Po
+	-rm -f ./$(DEPDIR)/mount_file_system.Po
+	-rm -f ./$(DEPDIR)/mount_fuse.Po
+	-rm -f ./$(DEPDIR)/mount_handle.Po
+	-rm -f ./$(DEPDIR)/olecfexport.Po
+	-rm -f ./$(DEPDIR)/olecfinfo.Po
+	-rm -f ./$(DEPDIR)/olecfmount.Po
+	-rm -f ./$(DEPDIR)/olecftools_getopt.Po
+	-rm -f ./$(DEPDIR)/olecftools_output.Po
+	-rm -f ./$(DEPDIR)/olecftools_signal.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1030,17 +1049,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on olecfexport ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(olecfexport_SOURCES)
 	@echo "Running splint on olecfinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(olecfinfo_SOURCES)
 	@echo "Running splint on olecfmount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(olecfmount_SOURCES)
```

### Comparing `libolecf-20240212/olecftools/log_handle.h` & `libolecf-20240427/olecftools/log_handle.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/olecftools_libuna.h` & `libolecf-20240427/olecftools/olecftools_libuna.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/olecftools/mount_fuse.h` & `libolecf-20240427/olecftools/mount_fuse.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/libcfile_extern.h` & `libolecf-20240427/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/libcfile_support.h` & `libolecf-20240427/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/libcfile_unused.h` & `libolecf-20240427/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/libcfile_notify.h` & `libolecf-20240427/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/libcfile_support.c` & `libolecf-20240427/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/libcfile_types.h` & `libolecf-20240427/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/Makefile.am` & `libolecf-20240427/libcfile/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCFILE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcfile.la
 
@@ -22,19 +22,17 @@
 	libcfile_support.c libcfile_support.h \
 	libcfile_system_string.c libcfile_system_string.h \
 	libcfile_types.h \
 	libcfile_unused.h \
 	libcfile_winapi.c libcfile_winapi.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
```

### Comparing `libolecf-20240212/libcfile/libcfile_notify.c` & `libolecf-20240427/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/libcfile_system_string.h` & `libolecf-20240427/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/libcfile_file.h` & `libolecf-20240427/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/libcfile_libcnotify.h` & `libolecf-20240427/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/libcfile_system_string.c` & `libolecf-20240427/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/libcfile_error.h` & `libolecf-20240427/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/libcfile_libcerror.h` & `libolecf-20240427/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/libcfile_file.c` & `libolecf-20240427/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/libcfile_libclocale.h` & `libolecf-20240427/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/libcfile_winapi.h` & `libolecf-20240427/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/Makefile.in` & `libolecf-20240427/libcfile/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -461,14 +461,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -527,16 +529,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCFILE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCFILE_TRUE@noinst_LTLIBRARIES = libcfile.la
 @HAVE_LOCAL_LIBCFILE_TRUE@libcfile_la_SOURCES = \
@@ -551,15 +553,16 @@
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_notify.c libcfile_notify.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_support.c libcfile_support.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_system_string.c libcfile_system_string.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_types.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_unused.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_winapi.c libcfile_winapi.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -764,24 +767,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcfile_error.Plo
+	-rm -f ./$(DEPDIR)/libcfile_file.Plo
+	-rm -f ./$(DEPDIR)/libcfile_notify.Plo
+	-rm -f ./$(DEPDIR)/libcfile_support.Plo
+	-rm -f ./$(DEPDIR)/libcfile_system_string.Plo
+	-rm -f ./$(DEPDIR)/libcfile_winapi.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -870,17 +881,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libolecf-20240212/libcfile/libcfile_error.c` & `libolecf-20240427/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/libcfile_libuna.h` & `libolecf-20240427/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/libcfile_winapi.c` & `libolecf-20240427/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcfile/libcfile_definitions.h` & `libolecf-20240427/libcfile/libcfile_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcfile/definitions.h>
 
 /* The definitions in <libcfile/definitions.h> are copied here
  * for local use of libcfile
  */
 #else
 
-#define LIBCFILE_VERSION				20240106
+#define LIBCFILE_VERSION				20240414
 
 /* The libcfile version string
  */
-#define LIBCFILE_VERSION_STRING				"20240106"
+#define LIBCFILE_VERSION_STRING				"20240414"
 
 /* The file access flags
  * bit 1	set to 1 for read access
  * bit 2	set to 1 for write access
  * bit 3	set to 1 to truncate an existing file on write
  * bit 4-8	not used
  */
```

### Comparing `libolecf-20240212/INSTALL` & `libolecf-20240427/INSTALL`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_list_element.h` & `libolecf-20240427/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_array.h` & `libolecf-20240427/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_definitions.h` & `libolecf-20240427/libcdata/libcdata_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdata/definitions.h>
 
 /* The definitions in <libcdata/definitions.h> are copied here
  * for local use of libcdata
  */
 #else
 
-#define LIBCDATA_VERSION				20240103
+#define LIBCDATA_VERSION				20240414
 
 /* The libcdata version string
  */
-#define LIBCDATA_VERSION_STRING				"20240103"
+#define LIBCDATA_VERSION_STRING				"20240414"
 
 /* The comparison function definitions
  */
 enum LIBCDATA_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libolecf-20240212/libcdata/libcdata_libcerror.h` & `libolecf-20240427/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_unused.h` & `libolecf-20240427/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_btree.h` & `libolecf-20240427/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_btree.c` & `libolecf-20240427/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_support.c` & `libolecf-20240427/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_list.c` & `libolecf-20240427/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_extern.h` & `libolecf-20240427/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_list.h` & `libolecf-20240427/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_btree_values_list.h` & `libolecf-20240427/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/Makefile.am` & `libolecf-20240427/libcdata/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdata.la
 
 libcdata_la_SOURCES = \
@@ -24,19 +24,17 @@
 	libcdata_range_list_value.c libcdata_range_list_value.h \
 	libcdata_support.c libcdata_support.h \
 	libcdata_tree_node.c libcdata_tree_node.h \
 	libcdata_types.h \
 	libcdata_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
```

### Comparing `libolecf-20240212/libcdata/libcdata_btree_node.h` & `libolecf-20240427/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_range_list_value.h` & `libolecf-20240427/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_range_list.h` & `libolecf-20240427/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_range_list.c` & `libolecf-20240427/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_array.c` & `libolecf-20240427/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_list_element.c` & `libolecf-20240427/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_libcthreads.h` & `libolecf-20240427/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_tree_node.h` & `libolecf-20240427/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_error.h` & `libolecf-20240427/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_types.h` & `libolecf-20240427/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_btree_node.c` & `libolecf-20240427/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_tree_node.c` & `libolecf-20240427/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_support.h` & `libolecf-20240427/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/Makefile.in` & `libolecf-20240427/libcdata/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -475,14 +475,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -541,16 +543,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDATA_TRUE@noinst_LTLIBRARIES = libcdata.la
 @HAVE_LOCAL_LIBCDATA_TRUE@libcdata_la_SOURCES = \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_array.c libcdata_array.h \
@@ -567,15 +569,16 @@
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list.c libcdata_range_list.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list_value.c libcdata_range_list_value.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_support.c libcdata_support.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_tree_node.c libcdata_tree_node.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_types.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -785,24 +788,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdata_array.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_node.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_values_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_error.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list_value.Plo
+	-rm -f ./$(DEPDIR)/libcdata_support.Plo
+	-rm -f ./$(DEPDIR)/libcdata_tree_node.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -896,17 +912,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libolecf-20240212/libcdata/libcdata_range_list_value.c` & `libolecf-20240427/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_btree_values_list.c` & `libolecf-20240427/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcdata/libcdata_error.c` & `libolecf-20240427/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/config.sub` & `libolecf-20240427/config.sub`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/setup.py` & `libolecf-20240427/setup.py`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/acinclude.m4` & `libolecf-20240427/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/config.rpath` & `libolecf-20240427/config.rpath`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_thread.h` & `libolecf-20240427/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_read_write_lock.h` & `libolecf-20240427/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_thread.c` & `libolecf-20240427/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_thread_pool.h` & `libolecf-20240427/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_support.h` & `libolecf-20240427/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_lock.h` & `libolecf-20240427/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_unused.h` & `libolecf-20240427/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_lock.c` & `libolecf-20240427/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_condition.h` & `libolecf-20240427/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_repeating_thread.h` & `libolecf-20240427/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/Makefile.am` & `libolecf-20240427/libcthreads/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCTHREADS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcthreads.la
 
 libcthreads_la_SOURCES = \
 	libcthreads_condition.c libcthreads_condition.h \
@@ -22,19 +22,17 @@
 	libcthreads_thread.c libcthreads_thread.h \
 	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 	libcthreads_types.h \
 	libcthreads_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
```

### Comparing `libolecf-20240212/libcthreads/libcthreads_support.c` & `libolecf-20240427/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_mutex.c` & `libolecf-20240427/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_queue.c` & `libolecf-20240427/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_mutex.h` & `libolecf-20240427/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_types.h` & `libolecf-20240427/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_thread_attributes.h` & `libolecf-20240427/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_condition.c` & `libolecf-20240427/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_error.c` & `libolecf-20240427/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_read_write_lock.c` & `libolecf-20240427/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_libcerror.h` & `libolecf-20240427/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_definitions.h` & `libolecf-20240427/libcthreads/libcthreads_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcthreads/definitions.h>
 
 /* The definitions in <libcthreads/definitions.h> are copied here
  * for local use of libcthreads
  */
 #else
 
-#define LIBCTHREADS_VERSION				20240102
+#define LIBCTHREADS_VERSION				20240413
 
 /* The libcthreads version string
  */
-#define LIBCTHREADS_VERSION_STRING			"20240102"
+#define LIBCTHREADS_VERSION_STRING			"20240413"
 
 /* The comparison function definitions
  */
 enum LIBCTHREADS_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libolecf-20240212/libcthreads/libcthreads_thread_pool.c` & `libolecf-20240427/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_error.h` & `libolecf-20240427/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_thread_attributes.c` & `libolecf-20240427/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_extern.h` & `libolecf-20240427/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/libcthreads_repeating_thread.c` & `libolecf-20240427/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcthreads/Makefile.in` & `libolecf-20240427/libcthreads/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -479,14 +479,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -545,16 +547,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCTHREADS_TRUE@noinst_LTLIBRARIES = libcthreads.la
 @HAVE_LOCAL_LIBCTHREADS_TRUE@libcthreads_la_SOURCES = \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_condition.c libcthreads_condition.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_definitions.h \
@@ -569,15 +571,16 @@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_support.c libcthreads_support.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread.c libcthreads_thread.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_types.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -787,24 +790,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcthreads_condition.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_error.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_mutex.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_queue.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_read_write_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_repeating_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_support.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_attributes.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_pool.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -898,17 +914,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libolecf-20240212/libcthreads/libcthreads_queue.h` & `libolecf-20240427/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/test-driver` & `libolecf-20240427/test-driver`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcpath/libcpath_support.c` & `libolecf-20240427/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcpath/libcpath_libcerror.h` & `libolecf-20240427/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcpath/libcpath_definitions.h` & `libolecf-20240427/libcpath/libcpath_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcpath/definitions.h>
 
 /* The definitions in <libcpath/definitions.h> are copied here
  * for local use of libcpath
  */
 #else
 
-#define LIBCPATH_VERSION			20240109
+#define LIBCPATH_VERSION			20240414
 
 /* The libcpath version string
  */
-#define LIBCPATH_VERSION_STRING			"20240109"
+#define LIBCPATH_VERSION_STRING			"20240414"
 
 #if defined( WINAPI )
 #define LIBCPATH_SEPARATOR			'\\'
 
 #else
 #define LIBCPATH_SEPARATOR			'/'
```

### Comparing `libolecf-20240212/libcpath/Makefile.am` & `libolecf-20240427/libcpath/Makefile.am`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCPATH
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcpath.la
 
@@ -19,19 +19,17 @@
 	libcpath_libcsplit.h \
 	libcpath_libuna.h \
 	libcpath_support.c libcpath_support.h \
 	libcpath_system_string.c libcpath_system_string.h \
 	libcpath_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
```

### Comparing `libolecf-20240212/libcpath/libcpath_error.c` & `libolecf-20240427/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcpath/libcpath_extern.h` & `libolecf-20240427/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcpath/libcpath_system_string.h` & `libolecf-20240427/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcpath/libcpath_support.h` & `libolecf-20240427/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcpath/libcpath_libcsplit.h` & `libolecf-20240427/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcpath/libcpath_system_string.c` & `libolecf-20240427/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcpath/libcpath_libclocale.h` & `libolecf-20240427/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcpath/libcpath_error.h` & `libolecf-20240427/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcpath/Makefile.in` & `libolecf-20240427/libcpath/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -455,14 +455,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -521,16 +523,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCPATH_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCPATH_TRUE@noinst_LTLIBRARIES = libcpath.la
 @HAVE_LOCAL_LIBCPATH_TRUE@libcpath_la_SOURCES = \
@@ -542,15 +544,16 @@
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libclocale.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libcsplit.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libuna.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_support.c libcpath_support.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_system_string.c libcpath_system_string.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -753,24 +756,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcpath_error.Plo
+	-rm -f ./$(DEPDIR)/libcpath_path.Plo
+	-rm -f ./$(DEPDIR)/libcpath_support.Plo
+	-rm -f ./$(DEPDIR)/libcpath_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -857,17 +866,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libolecf-20240212/libcpath/libcpath_libuna.h` & `libolecf-20240427/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcpath/libcpath_unused.h` & `libolecf-20240427/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcpath/libcpath_path.c` & `libolecf-20240427/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcpath/libcpath_path.h` & `libolecf-20240427/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/ChangeLog` & `libolecf-20240427/ChangeLog`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/manuals/olecfinfo.1` & `libolecf-20240427/manuals/olecfinfo.1`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/manuals/libolecf.3` & `libolecf-20240427/manuals/libolecf.3`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/manuals/Makefile.in` & `libolecf-20240427/manuals/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -428,14 +428,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -503,15 +505,16 @@
 	libolecf.3
 
 EXTRA_DIST = \
 	olecfexport.1 \
 	olecfinfo.1 \
 	libolecf.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -704,23 +707,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -802,13 +807,10 @@
 	mostlyclean-libtool pdf pdf-am ps ps-am sources-am \
 	sources-local splint-am splint-local tags-am uninstall \
 	uninstall-am uninstall-man uninstall-man1 uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libolecf-20240212/manuals/olecfexport.1` & `libolecf-20240427/manuals/olecfexport.1`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf.pc.in` & `libolecf-20240427/libolecf.pc.in`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_file_header.c` & `libolecf-20240427/tests/olecf_test_file_header.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_tools_output.c` & `libolecf-20240427/tests/olecf_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_functions.h` & `libolecf-20240427/tests/olecf_test_functions.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_memory.h` & `libolecf-20240427/tests/olecf_test_memory.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_file.c` & `libolecf-20240427/tests/olecf_test_file.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_macros.h` & `libolecf-20240427/tests/olecf_test_macros.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_getopt.c` & `libolecf-20240427/tests/olecf_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_io_handle.c` & `libolecf-20240427/tests/olecf_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/test_tools.sh` & `libolecf-20240427/tests/test_library.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env bash
-# Tests tools functions and types.
+# Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
-TOOLS_TESTS="info_handle output signal";
-TOOLS_TESTS_WITH_INPUT="";
+LIBRARY_TESTS="allocation_table directory_entry error file_header io_handle item notify property_section property_set property_value";
+LIBRARY_TESTS_WITH_INPUT="file support";
 OPTION_SETS=();
 
 INPUT_GLOB="*";
 
 run_test()
 {
 	local TEST_NAME=$1;
 
 	local TEST_DESCRIPTION="Testing: ${TEST_NAME}";
-	local TEST_EXECUTABLE="./olecf_test_tools_${TEST_NAME}";
+	local TEST_EXECUTABLE="./olecf_test_${TEST_NAME}";
 
 	if ! test -x "${TEST_EXECUTABLE}";
 	then
 		TEST_EXECUTABLE="${TEST_EXECUTABLE}.exe";
 	fi
 
 	# TODO: add support for TEST_PROFILE and OPTION_SETS?
@@ -33,15 +33,15 @@
 }
 
 run_test_with_input()
 {
 	local TEST_NAME=$1;
 
 	local TEST_DESCRIPTION="Testing: ${TEST_NAME}";
-	local TEST_EXECUTABLE="./olecf_test_tools_${TEST_NAME}";
+	local TEST_EXECUTABLE="./olecf_test_${TEST_NAME}";
 
 	if ! test -x "${TEST_EXECUTABLE}";
 	then
 		TEST_EXECUTABLE="${TEST_EXECUTABLE}.exe";
 	fi
 
 	if ! test -d "input";
@@ -55,15 +55,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "olecftools");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "libolecf");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -132,38 +132,35 @@
 			break;
 		fi
 	done
 
 	return ${RESULT};
 }
 
-if test -n "${SKIP_TOOLS_TESTS}";
+if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
 RESULT=${EXIT_IGNORE};
 
-for TEST_NAME in ${TOOLS_TESTS};
+for TEST_NAME in ${LIBRARY_TESTS};
 do
 	run_test "${TEST_NAME}";
 	RESULT=$?;
 
 	if test ${RESULT} -ne ${EXIT_SUCCESS};
 	then
 		break;
@@ -171,15 +168,15 @@
 done
 
 if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 then
 	exit ${RESULT};
 fi
 
-for TEST_NAME in ${TOOLS_TESTS_WITH_INPUT};
+for TEST_NAME in ${LIBRARY_TESTS_WITH_INPUT};
 do
 	if test -d "input";
 	then
 		run_test_with_input "${TEST_NAME}";
 		RESULT=$?;
 	else
 		run_test "${TEST_NAME}";
```

### Comparing `libolecf-20240212/tests/olecf_test_libcdata.h` & `libolecf-20240427/tests/olecf_test_libcdata.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_tools_info_handle.c` & `libolecf-20240427/tests/olecf_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_notify.c` & `libolecf-20240427/tests/olecf_test_notify.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_allocation_table.c` & `libolecf-20240427/tests/olecf_test_allocation_table.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/test_olecfexport.sh` & `libolecf-20240427/tests/test_olecfexport.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Export tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("olecfexport");
 OPTIONS_PER_PROFILE=("");
@@ -71,20 +71,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libolecf-20240212/tests/Makefile.am` & `libolecf-20240427/tests/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTOMAKE_OPTIONS = subdir-objects
 
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -281,13 +281,12 @@
 	olecf_test_tools_signal.c \
 	olecf_test_unused.h
 
 olecf_test_tools_signal_LDADD = \
 	../libolecf/libolecf.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
-
-distclean: clean
-	-rm -f Makefile
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
```

### Comparing `libolecf-20240212/tests/olecf_test_libbfio.h` & `libolecf-20240427/tests/olecf_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_functions.c` & `libolecf-20240427/tests/olecf_test_functions.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_libolecf.h` & `libolecf-20240427/tests/olecf_test_libolecf.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_memory.c` & `libolecf-20240427/tests/olecf_test_memory.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/test_python_module.sh` & `libolecf-20240427/tests/test_python_module.sh`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20240120
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="";
 TEST_FUNCTIONS_WITH_INPUT="file support";
 OPTION_SETS=();
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libolecf";
+PYTHON_MODULE="pyolecf";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyolecf_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyolecf_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -46,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pyolecf");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -121,30 +124,35 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
+PLATFORM=`uname -s | sed 's/-.*$//'`;
+
+if test "${PLATFORM}" = "MINGW64_NT" || test "${PLATFORM}" = "MSYS_NT";
+then
+	cp ../${LIBRARY_NAME}/.libs/*.dll ../${PYTHON_MODULE}/.libs/;
+	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
+fi
+
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
```

### Comparing `libolecf-20240212/tests/olecf_test_unused.h` & `libolecf-20240427/tests/olecf_test_unused.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_getopt.h` & `libolecf-20240427/tests/olecf_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_directory_entry.c` & `libolecf-20240427/tests/olecf_test_directory_entry.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/test_olecfinfo.sh` & `libolecf-20240427/tests/test_olecfinfo.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Info tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("olecfinfo");
 OPTIONS_PER_PROFILE=("");
@@ -28,20 +28,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libolecf-20240212/tests/olecf_test_libclocale.h` & `libolecf-20240427/tests/olecf_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_item.c` & `libolecf-20240427/tests/olecf_test_item.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_property_set.c` & `libolecf-20240427/tests/olecf_test_property_set.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_property_value.c` & `libolecf-20240427/tests/olecf_test_property_value.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/test_runner.sh` & `libolecf-20240427/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_error.c` & `libolecf-20240427/tests/olecf_test_error.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_libuna.h` & `libolecf-20240427/tests/olecf_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_libcerror.h` & `libolecf-20240427/tests/olecf_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_support.c` & `libolecf-20240427/tests/olecf_test_support.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_property_section.c` & `libolecf-20240427/tests/olecf_test_property_section.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/pyolecf_test_file.py` & `libolecf-20240427/tests/pyolecf_test_file.py`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/Makefile.in` & `libolecf-20240427/tests/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -775,14 +775,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -842,16 +844,16 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AUTOMAKE_OPTIONS = subdir-objects
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -1107,16 +1109,18 @@
 	olecf_test_tools_signal.c \
 	olecf_test_unused.h
 
 olecf_test_tools_signal_LDADD = \
 	../libolecf/libolecf.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -1606,24 +1610,47 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../olecftools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../olecftools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../olecftools/$(DEPDIR)/info_handle.Po
+	-rm -f ../olecftools/$(DEPDIR)/olecftools_output.Po
+	-rm -f ../olecftools/$(DEPDIR)/olecftools_signal.Po
+	-rm -f ./$(DEPDIR)/olecf_test_allocation_table.Po
+	-rm -f ./$(DEPDIR)/olecf_test_directory_entry.Po
+	-rm -f ./$(DEPDIR)/olecf_test_error.Po
+	-rm -f ./$(DEPDIR)/olecf_test_file.Po
+	-rm -f ./$(DEPDIR)/olecf_test_file_header.Po
+	-rm -f ./$(DEPDIR)/olecf_test_functions.Po
+	-rm -f ./$(DEPDIR)/olecf_test_getopt.Po
+	-rm -f ./$(DEPDIR)/olecf_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/olecf_test_item.Po
+	-rm -f ./$(DEPDIR)/olecf_test_memory.Po
+	-rm -f ./$(DEPDIR)/olecf_test_notify.Po
+	-rm -f ./$(DEPDIR)/olecf_test_property_section.Po
+	-rm -f ./$(DEPDIR)/olecf_test_property_set.Po
+	-rm -f ./$(DEPDIR)/olecf_test_property_value.Po
+	-rm -f ./$(DEPDIR)/olecf_test_support.Po
+	-rm -f ./$(DEPDIR)/olecf_test_tools_info_handle.Po
+	-rm -f ./$(DEPDIR)/olecf_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/olecf_test_tools_signal.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1727,13 +1754,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libolecf-20240212/tests/olecf_test_libcnotify.h` & `libolecf-20240427/libfvalue/libfvalue_libcnotify.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * The libcnotify header wrapper
+ * The internal libcnotify header
  *
- * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _OLECF_TEST_LIBCNOTIFY_H )
-#define _OLECF_TEST_LIBCNOTIFY_H
+#if !defined( _LIBFVALUE_LIBCNOTIFY_H )
+#define _LIBFVALUE_LIBCNOTIFY_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCNOTIFY for local use of libcnotify
  */
 #if defined( HAVE_LOCAL_LIBCNOTIFY )
 
@@ -40,11 +40,11 @@
  */
 #if defined( _WIN32 ) && defined( DLL_IMPORT )
 #define LIBCNOTIFY_DLL_IMPORT
 #endif
 
 #include <libcnotify.h>
 
-#endif /* defined( HAVE_LOCAL_LIBCNOTIFY ) */
+#endif
 
-#endif /* !defined( _OLECF_TEST_LIBCNOTIFY_H ) */
+#endif
```

### Comparing `libolecf-20240212/tests/pyolecf_test_support.py` & `libolecf-20240427/tests/pyolecf_test_support.py`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/olecf_test_tools_signal.c` & `libolecf-20240427/tests/olecf_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/tests/test_library.sh` & `libolecf-20240427/tests/test_tools.sh`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env bash
-# Tests library functions and types.
+# Tests tools functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
-LIBRARY_TESTS="allocation_table directory_entry error file_header io_handle item notify property_section property_set property_value";
-LIBRARY_TESTS_WITH_INPUT="file support";
+TOOLS_TESTS="info_handle output signal";
+TOOLS_TESTS_WITH_INPUT="";
 OPTION_SETS=();
 
 INPUT_GLOB="*";
 
 run_test()
 {
 	local TEST_NAME=$1;
 
 	local TEST_DESCRIPTION="Testing: ${TEST_NAME}";
-	local TEST_EXECUTABLE="./olecf_test_${TEST_NAME}";
+	local TEST_EXECUTABLE="./olecf_test_tools_${TEST_NAME}";
 
 	if ! test -x "${TEST_EXECUTABLE}";
 	then
 		TEST_EXECUTABLE="${TEST_EXECUTABLE}.exe";
 	fi
 
 	# TODO: add support for TEST_PROFILE and OPTION_SETS?
@@ -33,15 +33,15 @@
 }
 
 run_test_with_input()
 {
 	local TEST_NAME=$1;
 
 	local TEST_DESCRIPTION="Testing: ${TEST_NAME}";
-	local TEST_EXECUTABLE="./olecf_test_${TEST_NAME}";
+	local TEST_EXECUTABLE="./olecf_test_tools_${TEST_NAME}";
 
 	if ! test -x "${TEST_EXECUTABLE}";
 	then
 		TEST_EXECUTABLE="${TEST_EXECUTABLE}.exe";
 	fi
 
 	if ! test -d "input";
@@ -55,15 +55,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "libolecf");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "olecftools");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -132,38 +132,35 @@
 			break;
 		fi
 	done
 
 	return ${RESULT};
 }
 
-if test -n "${SKIP_LIBRARY_TESTS}";
+if test -n "${SKIP_TOOLS_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
 RESULT=${EXIT_IGNORE};
 
-for TEST_NAME in ${LIBRARY_TESTS};
+for TEST_NAME in ${TOOLS_TESTS};
 do
 	run_test "${TEST_NAME}";
 	RESULT=$?;
 
 	if test ${RESULT} -ne ${EXIT_SUCCESS};
 	then
 		break;
@@ -171,15 +168,15 @@
 done
 
 if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 then
 	exit ${RESULT};
 fi
 
-for TEST_NAME in ${LIBRARY_TESTS_WITH_INPUT};
+for TEST_NAME in ${TOOLS_TESTS_WITH_INPUT};
 do
 	if test -d "input";
 	then
 		run_test_with_input "${TEST_NAME}";
 		RESULT=$?;
 	else
 		run_test "${TEST_NAME}";
```

### Comparing `libolecf-20240212/ossfuzz/ossfuzz_libolecf.h` & `libolecf-20240427/ossfuzz/ossfuzz_libolecf.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/ossfuzz/Makefile.am` & `libolecf-20240427/ossfuzz/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -48,19 +48,17 @@
 	../libolecf/libolecf.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on file_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_fuzzer_SOURCES)
 	@echo "Running splint on item_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(item_fuzzer_SOURCES)
```

### Comparing `libolecf-20240212/ossfuzz/ossfuzz_libbfio.h` & `libolecf-20240427/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/ossfuzz/item_fuzzer.cc` & `libolecf-20240427/ossfuzz/item_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/ossfuzz/file_fuzzer.cc` & `libolecf-20240427/ossfuzz/file_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/ossfuzz/Makefile.in` & `libolecf-20240427/ossfuzz/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -478,14 +478,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -544,16 +546,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -591,15 +593,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libolecf/libolecf.la \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -846,23 +849,27 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/file_fuzzer.Po
+	-rm -f ./$(DEPDIR)/item_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -947,17 +954,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on file_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_fuzzer_SOURCES)
 	@echo "Running splint on item_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(item_fuzzer_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libolecf-20240212/ltmain.sh` & `libolecf-20240427/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcsplit/libcsplit_narrow_string.c` & `libolecf-20240427/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcsplit/libcsplit_definitions.h` & `libolecf-20240427/libcsplit/libcsplit_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 #include <libcsplit/definitions.h>
 
 /* The definitions in <libcsplit/definitions.h> are copied here
  * for local use of libcsplit
  */
 #else
 
-#define LIBCSPLIT_VERSION			20240110
+#define LIBCSPLIT_VERSION			20240414
 
 /* The libcsplit version string
  */
-#define LIBCSPLIT_VERSION_STRING		"20240110"
+#define LIBCSPLIT_VERSION_STRING		"20240414"
 
 #endif /* !defined( HAVE_LOCAL_LIBCSPLIT ) */
 
 #endif
```

### Comparing `libolecf-20240212/libcsplit/libcsplit_types.h` & `libolecf-20240427/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcsplit/libcsplit_wide_split_string.c` & `libolecf-20240427/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcsplit/libcsplit_support.h` & `libolecf-20240427/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcsplit/Makefile.am` & `libolecf-20240427/libcsplit/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCSPLIT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcsplit.la
 
 libcsplit_la_SOURCES = \
 	libcsplit_definitions.h \
 	libcsplit_error.c libcsplit_error.h \
@@ -16,19 +16,17 @@
 	libcsplit_support.c libcsplit_support.h \
 	libcsplit_types.h \
 	libcsplit_unused.h \
 	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 	libcsplit_wide_string.c libcsplit_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
```

### Comparing `libolecf-20240212/libcsplit/libcsplit_libcerror.h` & `libolecf-20240427/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcsplit/libcsplit_wide_string.c` & `libolecf-20240427/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcsplit/libcsplit_unused.h` & `libolecf-20240427/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcsplit/libcsplit_wide_split_string.h` & `libolecf-20240427/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcsplit/libcsplit_error.c` & `libolecf-20240427/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcsplit/libcsplit_narrow_split_string.c` & `libolecf-20240427/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcsplit/libcsplit_extern.h` & `libolecf-20240427/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcsplit/libcsplit_error.h` & `libolecf-20240427/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcsplit/libcsplit_support.c` & `libolecf-20240427/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcsplit/libcsplit_wide_string.h` & `libolecf-20240427/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcsplit/Makefile.in` & `libolecf-20240427/libcsplit/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -465,14 +465,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -531,16 +533,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCSPLIT_TRUE@noinst_LTLIBRARIES = libcsplit.la
 @HAVE_LOCAL_LIBCSPLIT_TRUE@libcsplit_la_SOURCES = \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_definitions.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_error.c libcsplit_error.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_extern.h \
@@ -549,15 +551,16 @@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_libcerror.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_support.c libcsplit_support.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_types.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_unused.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_string.c libcsplit_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -762,24 +765,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcsplit_error.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_support.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -868,17 +879,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libolecf-20240212/libcsplit/libcsplit_narrow_split_string.h` & `libolecf-20240427/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcsplit/libcsplit_narrow_string.h` & `libolecf-20240427/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/po/remove-potcdate.sin` & `libolecf-20240427/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/po/Makefile.in.in` & `libolecf-20240427/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/po/en@quot.header` & `libolecf-20240427/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/po/en@boldquot.header` & `libolecf-20240427/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/po/insert-header.sin` & `libolecf-20240427/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/po/Makevars` & `libolecf-20240427/po/Makevars`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/po/Makevars.in` & `libolecf-20240427/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/po/Rules-quot` & `libolecf-20240427/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_1251.c` & `libolecf-20240427/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_utf16_string.c` & `libolecf-20240427/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_base16_stream.c` & `libolecf-20240427/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_utf8_stream.h` & `libolecf-20240427/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_2.h` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_932.c` & `libolecf-20240427/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_dingbats.h` & `libolecf-20240427/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_utf8_string.c` & `libolecf-20240427/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_base64_stream.c` & `libolecf-20240427/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_error.h` & `libolecf-20240427/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_turkish.h` & `libolecf-20240427/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_unicode_character.c` & `libolecf-20240427/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_gaelic.c` & `libolecf-20240427/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_arabic.h` & `libolecf-20240427/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_thai.c` & `libolecf-20240427/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_874.h` & `libolecf-20240427/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_15.h` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_utf8_string.h` & `libolecf-20240427/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_16.c` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_1255.c` & `libolecf-20240427/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_utf7_stream.c` & `libolecf-20240427/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_byte_stream.h` & `libolecf-20240427/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_koi8_u.c` & `libolecf-20240427/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_unused.h` & `libolecf-20240427/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_6.c` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_14.c` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_base64_stream.h` & `libolecf-20240427/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_error.c` & `libolecf-20240427/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_centraleurroman.h` & `libolecf-20240427/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_romanian.c` & `libolecf-20240427/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_6.h` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_9.c` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_russian.h` & `libolecf-20240427/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_dingbats.c` & `libolecf-20240427/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_15.c` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_936.c` & `libolecf-20240427/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_croatian.h` & `libolecf-20240427/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_scsu.h` & `libolecf-20240427/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/Makefile.am` & `libolecf-20240427/libuna/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBUNA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libuna.la
 
 libuna_la_SOURCES = \
 	libuna_base16_stream.c libuna_base16_stream.h \
 	libuna_base32_stream.c libuna_base32_stream.h \
@@ -73,19 +73,17 @@
 	libuna_utf32_stream.c libuna_utf32_stream.h \
 	libuna_utf32_string.c libuna_utf32_string.h \
 	libuna_utf7_stream.c libuna_utf7_stream.h \
 	libuna_utf8_stream.c libuna_utf8_stream.h \
 	libuna_utf8_string.c libuna_utf8_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libolecf-20240212/libuna/libuna_utf32_stream.c` & `libolecf-20240427/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_936.h` & `libolecf-20240427/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_10.c` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_roman.c` & `libolecf-20240427/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_utf7_stream.h` & `libolecf-20240427/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_3.h` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_thai.h` & `libolecf-20240427/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_farsi.h` & `libolecf-20240427/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_ukrainian.c` & `libolecf-20240427/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_inuit.c` & `libolecf-20240427/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_932.h` & `libolecf-20240427/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_874.c` & `libolecf-20240427/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_5.c` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_10.h` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_definitions.h` & `libolecf-20240427/libuna/libuna_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20240130
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20240130"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libolecf-20240212/libuna/libuna_url_stream.h` & `libolecf-20240427/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_icelandic.h` & `libolecf-20240427/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_koi8_u.h` & `libolecf-20240427/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_utf16_stream.c` & `libolecf-20240427/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_1253.c` & `libolecf-20240427/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_4.h` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_greek.c` & `libolecf-20240427/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_libcerror.h` & `libolecf-20240427/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_centraleurroman.c` & `libolecf-20240427/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_1254.c` & `libolecf-20240427/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_13.h` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_7.h` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_1255.h` & `libolecf-20240427/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_unicode_character.h` & `libolecf-20240427/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_8.h` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_13.c` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_949.h` & `libolecf-20240427/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_cyrillic.c` & `libolecf-20240427/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_celtic.c` & `libolecf-20240427/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_support.h` & `libolecf-20240427/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_4.c` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_949.c` & `libolecf-20240427/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_utf16_stream.h` & `libolecf-20240427/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_symbol.c` & `libolecf-20240427/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_roman.h` & `libolecf-20240427/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_1257.c` & `libolecf-20240427/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_1254.h` & `libolecf-20240427/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_950.c` & `libolecf-20240427/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_extern.h` & `libolecf-20240427/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_1256.c` & `libolecf-20240427/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_types.h` & `libolecf-20240427/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_base32_stream.h` & `libolecf-20240427/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_1253.h` & `libolecf-20240427/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_16.h` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_utf8_stream.c` & `libolecf-20240427/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_1250.h` & `libolecf-20240427/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_2.c` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_support.c` & `libolecf-20240427/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_koi8_r.c` & `libolecf-20240427/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_5.h` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_utf16_string.h` & `libolecf-20240427/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_utf32_string.c` & `libolecf-20240427/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_icelandic.c` & `libolecf-20240427/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_1256.h` & `libolecf-20240427/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_utf32_string.h` & `libolecf-20240427/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_romanian.h` & `libolecf-20240427/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_8.c` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_koi8_r.h` & `libolecf-20240427/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_cyrillic.h` & `libolecf-20240427/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_arabic.c` & `libolecf-20240427/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_croatian.c` & `libolecf-20240427/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_9.h` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_greek.h` & `libolecf-20240427/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_1258.h` & `libolecf-20240427/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_7.c` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/Makefile.in` & `libolecf-20240427/libuna/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -633,14 +633,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -699,16 +701,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBUNA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBUNA_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBUNA_TRUE@noinst_LTLIBRARIES = libuna.la
 @HAVE_LOCAL_LIBUNA_TRUE@libuna_la_SOURCES = \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base16_stream.c libuna_base16_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base32_stream.c libuna_base32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base64_stream.c libuna_base64_stream.h \
@@ -774,15 +776,16 @@
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf16_string.c libuna_utf16_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_stream.c libuna_utf32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_string.c libuna_utf32_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf7_stream.c libuna_utf7_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_stream.c libuna_utf8_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_string.c libuna_utf8_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1044,24 +1047,89 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libuna_base16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base64_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_byte_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_10.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_13.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_14.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_15.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_16.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_2.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_3.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_4.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_5.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_6.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_7.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_8.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_9.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_r.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_u.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_arabic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_celtic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_centraleurroman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_croatian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_cyrillic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_dingbats.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_farsi.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_gaelic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_greek.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_icelandic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_inuit.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_roman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_romanian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_russian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_symbol.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_thai.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_turkish.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_ukrainian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1250.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1251.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1252.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1253.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1254.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1255.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1256.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1257.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1258.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_874.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_932.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_936.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_949.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_950.Plo
+	-rm -f ./$(DEPDIR)/libuna_error.Plo
+	-rm -f ./$(DEPDIR)/libuna_scsu.Plo
+	-rm -f ./$(DEPDIR)/libuna_support.Plo
+	-rm -f ./$(DEPDIR)/libuna_unicode_character.Plo
+	-rm -f ./$(DEPDIR)/libuna_url_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf7_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1207,17 +1275,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_3.c` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_1250.c` & `libolecf-20240427/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_scsu.c` & `libolecf-20240427/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_1252.c` & `libolecf-20240427/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_turkish.c` & `libolecf-20240427/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_ukrainian.h` & `libolecf-20240427/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_russian.c` & `libolecf-20240427/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_1258.c` & `libolecf-20240427/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_celtic.h` & `libolecf-20240427/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_byte_stream.c` & `libolecf-20240427/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_gaelic.h` & `libolecf-20240427/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_utf32_stream.h` & `libolecf-20240427/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_symbol.h` & `libolecf-20240427/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_1257.h` & `libolecf-20240427/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_inuit.h` & `libolecf-20240427/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_mac_farsi.c` & `libolecf-20240427/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_950.h` & `libolecf-20240427/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_url_stream.c` & `libolecf-20240427/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_1251.h` & `libolecf-20240427/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_windows_1252.h` & `libolecf-20240427/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_codepage_iso_8859_14.h` & `libolecf-20240427/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_base16_stream.h` & `libolecf-20240427/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libuna/libuna_base32_stream.c` & `libolecf-20240427/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/Makefile.in` & `libolecf-20240427/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -515,14 +515,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -645,16 +647,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libolecf.pc \
+	libolecf.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libolecf.pc
 
 all: all-recursive
 
@@ -1071,23 +1080,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1199,22 +1211,10 @@
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfole && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwps && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libolecf && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libolecf.pc
-	-rm -f libolecf.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libolecf-20240212/libfvalue/libfvalue_filetime.c` & `libolecf-20240427/libfvalue/libfvalue_filetime.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_utf16_string.c` & `libolecf-20240427/libfvalue/libfvalue_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_libfwnt.h` & `libolecf-20240427/libfvalue/libfvalue_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_value.c` & `libolecf-20240427/libfvalue/libfvalue_value.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_value.h` & `libolecf-20240427/libfvalue/libfvalue_value.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_definitions.h` & `libolecf-20240427/libfvalue/libfvalue_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfvalue/definitions.h> are copied here
  * for local use of libfvalue
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFVALUE_VERSION						20240124
+#define LIBFVALUE_VERSION						20240415
 
 /* The libfvalue version string
  */
-#define LIBFVALUE_VERSION_STRING					"20240124"
+#define LIBFVALUE_VERSION_STRING					"20240415"
 
 /* The endian definitions
  */
 #define LIBFVALUE_ENDIAN_BIG						_BYTE_STREAM_ENDIAN_BIG
 #define LIBFVALUE_ENDIAN_LITTLE						_BYTE_STREAM_ENDIAN_LITTLE
 #define LIBFVALUE_ENDIAN_NATIVE						(uint8_t) 'n'
```

### Comparing `libolecf-20240212/libfvalue/libfvalue_codepage.h` & `libolecf-20240427/libfvalue/libfvalue_codepage.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_split_utf16_string.c` & `libolecf-20240427/libfvalue/libfvalue_split_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_error.c` & `libolecf-20240427/libfvalue/libfvalue_error.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_utf8_string.c` & `libolecf-20240427/libfvalue/libfvalue_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_unused.h` & `libolecf-20240427/libfvalue/libfvalue_unused.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_split_utf16_string.h` & `libolecf-20240427/libfvalue/libfvalue_split_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_filetime.h` & `libolecf-20240427/libfvalue/libfvalue_filetime.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_support.c` & `libolecf-20240427/libfvalue/libfvalue_support.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_extern.h` & `libolecf-20240427/libfvalue/libfvalue_extern.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/Makefile.am` & `libolecf-20240427/libfvalue/Makefile.am`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFVALUE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
@@ -40,19 +40,17 @@
 	libfvalue_value_type.c libfvalue_value_type.h \
 	libfvalue_support.c libfvalue_support.h \
 	libfvalue_unused.h \
 	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 	libfvalue_utf16_string.c libfvalue_utf16_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
```

### Comparing `libolecf-20240212/libfvalue/libfvalue_value_type.h` & `libolecf-20240427/libfvalue/libfvalue_value_type.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_libcerror.h` & `libolecf-20240427/libfvalue/libfvalue_libcerror.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_split_utf8_string.c` & `libolecf-20240427/libfvalue/libfvalue_split_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_data_handle.h` & `libolecf-20240427/libfvalue/libfvalue_data_handle.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_libcnotify.h` & `libolecf-20240427/libfwps/libfwps_libcnotify.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * The internal libcnotify header
+ * The libcnotify header wrapper
  *
- * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2013-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFVALUE_LIBCNOTIFY_H )
-#define _LIBFVALUE_LIBCNOTIFY_H
+#if !defined( _LIBFWPS_LIBCNOTIFY_H )
+#define _LIBFWPS_LIBCNOTIFY_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCNOTIFY for local use of libcnotify
  */
 #if defined( HAVE_LOCAL_LIBCNOTIFY )
 
@@ -40,11 +40,11 @@
  */
 #if defined( _WIN32 ) && defined( DLL_IMPORT )
 #define LIBCNOTIFY_DLL_IMPORT
 #endif
 
 #include <libcnotify.h>
 
-#endif
+#endif /* defined( HAVE_LOCAL_LIBCNOTIFY ) */
 
-#endif
+#endif /* !defined( _LIBFWPS_LIBCNOTIFY_H ) */
```

### Comparing `libolecf-20240212/libfvalue/libfvalue_data_handle.c` & `libolecf-20240427/libfvalue/libfvalue_data_handle.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_integer.c` & `libolecf-20240427/libfvalue/libfvalue_integer.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_value_type.c` & `libolecf-20240427/libfvalue/libfvalue_value_type.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_integer.h` & `libolecf-20240427/libfvalue/libfvalue_integer.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_binary_data.h` & `libolecf-20240427/libfvalue/libfvalue_binary_data.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_value_entry.h` & `libolecf-20240427/libfvalue/libfvalue_value_entry.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_utf16_string.h` & `libolecf-20240427/libfvalue/libfvalue_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_error.h` & `libolecf-20240427/libfvalue/libfvalue_error.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_table.h` & `libolecf-20240427/libfvalue/libfvalue_table.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_libfguid.h` & `libolecf-20240427/libfvalue/libfvalue_libfguid.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_split_utf8_string.h` & `libolecf-20240427/libfvalue/libfvalue_split_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_floating_point.h` & `libolecf-20240427/libfvalue/libfvalue_floating_point.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_libfdatetime.h` & `libolecf-20240427/libfvalue/libfvalue_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_string.h` & `libolecf-20240427/libfvalue/libfvalue_string.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_binary_data.c` & `libolecf-20240427/libfvalue/libfvalue_binary_data.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_value_entry.c` & `libolecf-20240427/libfvalue/libfvalue_value_entry.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_libcdata.h` & `libolecf-20240427/libfvalue/libfvalue_libcdata.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_support.h` & `libolecf-20240427/libfvalue/libfvalue_support.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_table.c` & `libolecf-20240427/libfvalue/libfvalue_table.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/Makefile.in` & `libolecf-20240427/libfvalue/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -496,14 +496,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -562,16 +564,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFVALUE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBFDATETIME_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBFGUID_CPPFLAGS@ \
@@ -604,15 +606,16 @@
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_entry.c libfvalue_value_entry.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_type.c libfvalue_value_type.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_support.c libfvalue_support.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_unused.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf16_string.c libfvalue_utf16_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -827,24 +830,42 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfvalue_binary_data.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_error.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_floating_point.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_integer.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_support.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_table.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_entry.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_type.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -943,17 +964,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libolecf-20240212/libfvalue/libfvalue_utf8_string.h` & `libolecf-20240427/libfvalue/libfvalue_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_floating_point.c` & `libolecf-20240427/libfvalue/libfvalue_floating_point.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_types.h` & `libolecf-20240427/libfvalue/libfvalue_types.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_string.c` & `libolecf-20240427/libfvalue/libfvalue_string.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfvalue/libfvalue_libuna.h` & `libolecf-20240427/libfvalue/libfvalue_libuna.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcnotify/libcnotify_definitions.h` & `libolecf-20240427/libcnotify/libcnotify_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcnotify/definitions.h>
 
 /* The definitions in <libcnotify/definitions.h> are copied here
  * for local use of libcnotify
  */
 #else
 
-#define LIBCNOTIFY_VERSION				20240108
+#define LIBCNOTIFY_VERSION				20240414
 
 /* The libcnotify version string
  */
-#define LIBCNOTIFY_VERSION_STRING			"20240108"
+#define LIBCNOTIFY_VERSION_STRING			"20240414"
 
 /* The print data flags
  */
 enum LIBCNOTIFY_NOTIFY_PRINT_DATA_FLAGS
 {
 	LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA		= 0x01,
 };
```

### Comparing `libolecf-20240212/libcnotify/libcnotify_extern.h` & `libolecf-20240427/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcnotify/libcnotify_support.c` & `libolecf-20240427/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcnotify/libcnotify_stream.h` & `libolecf-20240427/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcnotify/Makefile.am` & `libolecf-20240427/libcnotify/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCNOTIFY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcnotify.la
 
 libcnotify_la_SOURCES = \
 	libcnotify_definitions.h \
 	libcnotify_extern.h \
@@ -13,19 +13,17 @@
 	libcnotify_print.c libcnotify_print.h \
 	libcnotify_stream.c libcnotify_stream.h \
 	libcnotify_support.c libcnotify_support.h \
 	libcnotify_unused.h \
 	libcnotify_verbose.c libcnotify_verbose.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
```

### Comparing `libolecf-20240212/libcnotify/libcnotify_unused.h` & `libolecf-20240427/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcnotify/libcnotify_verbose.h` & `libolecf-20240427/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcnotify/libcnotify_print.h` & `libolecf-20240427/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcnotify/libcnotify_stream.c` & `libolecf-20240427/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcnotify/libcnotify_support.h` & `libolecf-20240427/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcnotify/libcnotify_verbose.c` & `libolecf-20240427/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcnotify/Makefile.in` & `libolecf-20240427/libcnotify/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -457,14 +457,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -523,30 +525,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@noinst_LTLIBRARIES = libcnotify.la
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@libcnotify_la_SOURCES = \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_definitions.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_extern.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_libcerror.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_print.c libcnotify_print.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_stream.c libcnotify_stream.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_support.c libcnotify_support.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_unused.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_verbose.c libcnotify_verbose.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -749,24 +752,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcnotify_print.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_stream.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_support.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_verbose.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -853,17 +862,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libolecf-20240212/libcnotify/libcnotify_libcerror.h` & `libolecf-20240427/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcnotify/libcnotify_print.c` & `libolecf-20240427/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libolecf.spec` & `libolecf-20240427/libolecf.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libolecf
-Version: 20240212
+Version: 20240427
 Release: 1
 Summary: Library to access the Object Linking and Embedding (OLE) Compound File (CF) format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libolecf
                
@@ -36,16 +36,16 @@
 
 %description -n libolecf-python3
 Python 3 bindings for libolecf
 
 %package -n libolecf-tools
 Summary: Several tools for reading Object Linking and Embedding (OLE) Compound Files (CF)
 Group: Applications/System
-Requires: libolecf = %{version}-%{release} fuse-libs
-BuildRequires: fuse-devel
+Requires: libolecf = %{version}-%{release} fuse3-libs
+BuildRequires: fuse3-devel
 
 %description -n libolecf-tools
 Several tools for reading Object Linking and Embedding (OLE) Compound Files (CF)
 
 %prep
 %setup -q
 
@@ -91,10 +91,10 @@
 %files -n libolecf-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Mon Feb 12 2024 Joachim Metz <joachim.metz@gmail.com> 20240212-1
+* Sat Apr 27 2024 Joachim Metz <joachim.metz@gmail.com> 20240427-1
 - Auto-generated
```

### Comparing `libolecf-20240212/libcerror/libcerror_system.c` & `libolecf-20240427/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcerror/libcerror_error.c` & `libolecf-20240427/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcerror/libcerror_extern.h` & `libolecf-20240427/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcerror/Makefile.am` & `libolecf-20240427/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libolecf-20240212/libcerror/libcerror_types.h` & `libolecf-20240427/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcerror/libcerror_support.h` & `libolecf-20240427/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcerror/libcerror_error.h` & `libolecf-20240427/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcerror/libcerror_system.h` & `libolecf-20240427/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcerror/libcerror_definitions.h` & `libolecf-20240427/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libolecf-20240212/libcerror/libcerror_support.c` & `libolecf-20240427/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcerror/libcerror_unused.h` & `libolecf-20240427/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libcerror/Makefile.in` & `libolecf-20240427/libcerror/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -454,14 +454,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -520,28 +522,29 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -743,24 +746,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -846,17 +854,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_floatingtime.h` & `libolecf-20240427/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_nsf_timedate.c` & `libolecf-20240427/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_error.h` & `libolecf-20240427/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_floatingtime.c` & `libolecf-20240427/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_support.h` & `libolecf-20240427/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_hfs_time.h` & `libolecf-20240427/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_definitions.h` & `libolecf-20240427/libfdatetime/libfdatetime_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfdatetime/definitions.h> are copied here
  * for local use of libfdatetime
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFDATETIME_VERSION					20240115
+#define LIBFDATETIME_VERSION					20240415
 
 /* The version string
  */
-#define LIBFDATETIME_VERSION_STRING				"20240115"
+#define LIBFDATETIME_VERSION_STRING				"20240415"
 
 /* The byte order definitions
  */
 #define LIBFDATETIME_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFDATETIME_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The string format definition flags
```

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_hfs_time.c` & `libolecf-20240427/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/Makefile.am` & `libolecf-20240427/libfdatetime/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATETIME
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfdatetime.la
 
 libfdatetime_la_SOURCES = \
 	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 	libfdatetime_definitions.h \
@@ -20,19 +20,17 @@
 	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 	libfdatetime_support.c libfdatetime_support.h \
 	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 	libfdatetime_types.h \
 	libfdatetime_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
```

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_filetime.c` & `libolecf-20240427/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_systemtime.h` & `libolecf-20240427/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_extern.h` & `libolecf-20240427/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_posix_time.c` & `libolecf-20240427/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_unused.h` & `libolecf-20240427/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_fat_date_time.h` & `libolecf-20240427/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_systemtime.c` & `libolecf-20240427/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_nsf_timedate.h` & `libolecf-20240427/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_libcerror.h` & `libolecf-20240427/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_support.c` & `libolecf-20240427/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_error.c` & `libolecf-20240427/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_posix_time.h` & `libolecf-20240427/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_date_time_values.h` & `libolecf-20240427/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_filetime.h` & `libolecf-20240427/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_date_time_values.c` & `libolecf-20240427/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_types.h` & `libolecf-20240427/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/libfdatetime/Makefile.in` & `libolecf-20240427/libfdatetime/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -476,14 +476,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -542,16 +544,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFDATETIME_TRUE@noinst_LTLIBRARIES = libfdatetime.la
 @HAVE_LOCAL_LIBFDATETIME_TRUE@libfdatetime_la_SOURCES = \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_definitions.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_extern.h \
@@ -564,15 +566,16 @@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_nsf_timedate.c libfdatetime_nsf_timedate.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_support.c libfdatetime_support.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_types.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -781,24 +784,36 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdatetime_date_time_values.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_error.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_fat_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_floatingtime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_hfs_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_nsf_timedate.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_posix_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_support.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_systemtime.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -891,17 +906,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libolecf-20240212/libfdatetime/libfdatetime_fat_date_time.c` & `libolecf-20240427/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/aclocal.m4` & `libolecf-20240427/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libolecf-20240212/configure.ac` & `libolecf-20240427/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libolecf],
- [20240212],
+ [20240427],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libolecf.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

