# Comparing `tmp/pixeltable-0.2.4.tar.gz` & `tmp/pixeltable-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixeltable-0.2.4.tar", max compression
+gzip compressed data, was "pixeltable-0.2.5.tar", max compression
```

## Comparing `pixeltable-0.2.4.tar` & `pixeltable-0.2.5.tar`

### file list

```diff
@@ -1,132 +1,139 @@
--rw-r--r--   0        0        0      746 2024-03-22 03:20:30.854989 pixeltable-0.2.4/LICENSE
--rw-r--r--   0        0        0     4680 2024-04-17 01:12:13.386362 pixeltable-0.2.4/README.md
--rw-r--r--   0        0        0      959 2024-04-04 00:11:47.491970 pixeltable-0.2.4/pixeltable/__init__.py
--rw-r--r--   0        0        0      453 2024-03-22 03:20:30.929081 pixeltable-0.2.4/pixeltable/catalog/__init__.py
--rw-r--r--   0        0        0     7908 2024-04-04 00:11:47.492457 pixeltable-0.2.4/pixeltable/catalog/catalog.py
--rw-r--r--   0        0        0     8663 2024-04-17 01:12:13.387513 pixeltable-0.2.4/pixeltable/catalog/column.py
--rw-r--r--   0        0        0      919 2024-03-22 03:20:30.929659 pixeltable-0.2.4/pixeltable/catalog/dir.py
--rw-r--r--   0        0        0      943 2024-03-22 03:20:30.929786 pixeltable-0.2.4/pixeltable/catalog/globals.py
--rw-r--r--   0        0        0     8280 2024-04-04 00:11:47.492972 pixeltable-0.2.4/pixeltable/catalog/insertable_table.py
--rw-r--r--   0        0        0     1147 2024-03-22 03:20:30.930368 pixeltable-0.2.4/pixeltable/catalog/named_function.py
--rw-r--r--   0        0        0     1677 2024-04-04 00:11:47.493163 pixeltable-0.2.4/pixeltable/catalog/path.py
--rw-r--r--   0        0        0     5941 2024-04-04 00:11:47.493341 pixeltable-0.2.4/pixeltable/catalog/path_dict.py
--rw-r--r--   0        0        0     1059 2024-03-22 03:20:30.931044 pixeltable-0.2.4/pixeltable/catalog/schema_object.py
--rw-r--r--   0        0        0    25499 2024-04-04 00:11:47.493604 pixeltable-0.2.4/pixeltable/catalog/table.py
--rw-r--r--   0        0        0    35680 2024-04-04 00:11:47.493943 pixeltable-0.2.4/pixeltable/catalog/table_version.py
--rw-r--r--   0        0        0     5461 2024-04-04 00:11:47.494156 pixeltable-0.2.4/pixeltable/catalog/table_version_path.py
--rw-r--r--   0        0        0     9734 2024-04-04 00:11:47.494389 pixeltable-0.2.4/pixeltable/catalog/view.py
--rw-r--r--   0        0        0    23616 2024-04-17 01:12:13.388062 pixeltable-0.2.4/pixeltable/client.py
--rw-r--r--   0        0        0    28339 2024-04-06 17:38:28.087008 pixeltable-0.2.4/pixeltable/dataframe.py
--rw-r--r--   0        0        0    15744 2024-04-17 01:12:13.388412 pixeltable-0.2.4/pixeltable/env.py
--rw-r--r--   0        0        0      376 2024-03-22 03:20:30.937922 pixeltable-0.2.4/pixeltable/exceptions.py
--rw-r--r--   0        0        0      412 2024-03-22 03:20:30.938153 pixeltable-0.2.4/pixeltable/exec/__init__.py
--rw-r--r--   0        0        0     3321 2024-04-04 00:11:47.495476 pixeltable-0.2.4/pixeltable/exec/aggregation_node.py
--rw-r--r--   0        0        0     5212 2024-04-08 22:50:04.684752 pixeltable-0.2.4/pixeltable/exec/cache_prefetch_node.py
--rw-r--r--   0        0        0     4069 2024-03-22 03:20:30.939348 pixeltable-0.2.4/pixeltable/exec/component_iteration_node.py
--rw-r--r--   0        0        0     3505 2024-03-22 03:20:30.939513 pixeltable-0.2.4/pixeltable/exec/data_row_batch.py
--rw-r--r--   0        0        0      924 2024-03-22 03:20:30.939633 pixeltable-0.2.4/pixeltable/exec/exec_context.py
--rw-r--r--   0        0        0     2170 2024-03-22 03:20:30.939748 pixeltable-0.2.4/pixeltable/exec/exec_node.py
--rw-r--r--   0        0        0    10810 2024-04-04 00:11:47.495696 pixeltable-0.2.4/pixeltable/exec/expr_eval_node.py
--rw-r--r--   0        0        0     2949 2024-03-22 03:20:30.941553 pixeltable-0.2.4/pixeltable/exec/in_memory_data_node.py
--rw-r--r--   0        0        0     1514 2024-03-22 03:20:30.945244 pixeltable-0.2.4/pixeltable/exec/media_validation_node.py
--rw-r--r--   0        0        0    10318 2024-03-22 03:20:30.945695 pixeltable-0.2.4/pixeltable/exec/sql_scan_node.py
--rw-r--r--   0        0        0      935 2024-04-04 00:11:47.495925 pixeltable-0.2.4/pixeltable/exprs/__init__.py
--rw-r--r--   0        0        0     4386 2024-03-22 03:20:30.948503 pixeltable-0.2.4/pixeltable/exprs/arithmetic_expr.py
--rw-r--r--   0        0        0     2131 2024-03-22 03:20:30.948806 pixeltable-0.2.4/pixeltable/exprs/array_slice.py
--rw-r--r--   0        0        0     2706 2024-03-22 03:20:30.949036 pixeltable-0.2.4/pixeltable/exprs/column_property_ref.py
--rw-r--r--   0        0        0     4794 2024-03-22 03:20:30.949236 pixeltable-0.2.4/pixeltable/exprs/column_ref.py
--rw-r--r--   0        0        0     3000 2024-03-22 03:20:30.949375 pixeltable-0.2.4/pixeltable/exprs/comparison.py
--rw-r--r--   0        0        0     3830 2024-03-22 03:20:30.949509 pixeltable-0.2.4/pixeltable/exprs/compound_predicate.py
--rw-r--r--   0        0        0     8046 2024-04-08 22:50:04.685112 pixeltable-0.2.4/pixeltable/exprs/data_row.py
--rw-r--r--   0        0        0    23748 2024-04-04 00:11:47.496409 pixeltable-0.2.4/pixeltable/exprs/expr.py
--rw-r--r--   0        0        0     1222 2024-03-22 03:20:30.954653 pixeltable-0.2.4/pixeltable/exprs/expr_set.py
--rw-r--r--   0        0        0    16961 2024-04-04 00:11:47.496718 pixeltable-0.2.4/pixeltable/exprs/function_call.py
--rw-r--r--   0        0        0     1537 2024-03-22 03:20:30.958471 pixeltable-0.2.4/pixeltable/exprs/globals.py
--rw-r--r--   0        0        0     4663 2024-03-22 03:20:30.958665 pixeltable-0.2.4/pixeltable/exprs/image_member_access.py
--rw-r--r--   0        0        0     1906 2024-03-22 03:20:30.958803 pixeltable-0.2.4/pixeltable/exprs/image_similarity_predicate.py
--rw-r--r--   0        0        0     4312 2024-03-22 03:20:30.958978 pixeltable-0.2.4/pixeltable/exprs/inline_array.py
--rw-r--r--   0        0        0     3695 2024-03-22 03:20:30.959427 pixeltable-0.2.4/pixeltable/exprs/inline_dict.py
--rw-r--r--   0        0        0     1041 2024-03-22 03:20:30.959589 pixeltable-0.2.4/pixeltable/exprs/is_null.py
--rw-r--r--   0        0        0     4559 2024-03-22 03:20:30.959717 pixeltable-0.2.4/pixeltable/exprs/json_mapper.py
--rw-r--r--   0        0        0     6526 2024-03-22 03:20:30.959875 pixeltable-0.2.4/pixeltable/exprs/json_path.py
--rw-r--r--   0        0        0     1885 2024-03-22 03:20:30.960091 pixeltable-0.2.4/pixeltable/exprs/literal.py
--rw-r--r--   0        0        0     1250 2024-03-22 03:20:30.960205 pixeltable-0.2.4/pixeltable/exprs/object_ref.py
--rw-r--r--   0        0        0     1859 2024-03-22 03:20:30.960322 pixeltable-0.2.4/pixeltable/exprs/predicate.py
--rw-r--r--   0        0        0    16992 2024-04-04 00:11:47.497017 pixeltable-0.2.4/pixeltable/exprs/row_builder.py
--rw-r--r--   0        0        0     4268 2024-03-22 03:20:30.962221 pixeltable-0.2.4/pixeltable/exprs/rowid_ref.py
--rw-r--r--   0        0        0     1793 2024-03-22 03:20:30.962353 pixeltable-0.2.4/pixeltable/exprs/type_cast.py
--rw-r--r--   0        0        0     1361 2024-04-04 00:11:47.497543 pixeltable-0.2.4/pixeltable/exprs/variable.py
--rw-r--r--   0        0        0      457 2024-04-04 00:11:47.497746 pixeltable-0.2.4/pixeltable/func/__init__.py
--rw-r--r--   0        0        0     9177 2024-04-04 00:11:47.497895 pixeltable-0.2.4/pixeltable/func/aggregate_function.py
--rw-r--r--   0        0        0     2350 2024-04-04 00:11:47.498062 pixeltable-0.2.4/pixeltable/func/batched_function.py
--rw-r--r--   0        0        0     2357 2024-04-04 00:11:47.498480 pixeltable-0.2.4/pixeltable/func/callable_function.py
--rw-r--r--   0        0        0     3392 2024-04-04 00:11:47.498601 pixeltable-0.2.4/pixeltable/func/expr_template_function.py
--rw-r--r--   0        0        0     4023 2024-04-04 00:11:47.498783 pixeltable-0.2.4/pixeltable/func/function.py
--rw-r--r--   0        0        0    11456 2024-04-04 00:11:47.498985 pixeltable-0.2.4/pixeltable/func/function_registry.py
--rw-r--r--   0        0        0     1220 2024-04-04 00:11:47.499364 pixeltable-0.2.4/pixeltable/func/globals.py
--rw-r--r--   0        0        0     9650 2024-04-04 00:11:47.499601 pixeltable-0.2.4/pixeltable/func/nos_function.py
--rw-r--r--   0        0        0     7107 2024-04-04 00:11:47.499798 pixeltable-0.2.4/pixeltable/func/signature.py
--rw-r--r--   0        0        0     6457 2024-04-04 00:11:47.499973 pixeltable-0.2.4/pixeltable/func/udf.py
--rw-r--r--   0        0        0     3390 2024-04-17 01:12:13.388971 pixeltable-0.2.4/pixeltable/functions/__init__.py
--rw-r--r--   0        0        0     8453 2024-04-04 00:11:47.500621 pixeltable-0.2.4/pixeltable/functions/eval.py
--rw-r--r--   0        0        0      908 2024-04-17 01:12:13.389269 pixeltable-0.2.4/pixeltable/functions/fireworks.py
--rw-r--r--   0        0        0     4804 2024-04-04 00:11:47.500918 pixeltable-0.2.4/pixeltable/functions/huggingface.py
--rw-r--r--   0        0        0      431 2024-04-04 00:11:47.501186 pixeltable-0.2.4/pixeltable/functions/image.py
--rw-r--r--   0        0        0     6861 2024-04-17 01:12:13.389598 pixeltable-0.2.4/pixeltable/functions/openai.py
--rw-r--r--   0        0        0     6217 2024-04-04 00:11:47.501525 pixeltable-0.2.4/pixeltable/functions/pil/image.py
--rw-r--r--   0        0        0      516 2024-04-04 00:11:47.501661 pixeltable-0.2.4/pixeltable/functions/string.py
--rw-r--r--   0        0        0     3423 2024-04-17 01:12:13.390515 pixeltable-0.2.4/pixeltable/functions/together.py
--rw-r--r--   0        0        0     1596 2024-04-04 00:11:47.502099 pixeltable-0.2.4/pixeltable/functions/util.py
--rw-r--r--   0        0        0     2403 2024-04-04 00:11:47.502279 pixeltable-0.2.4/pixeltable/functions/video.py
--rw-r--r--   0        0        0       70 2024-03-22 03:20:30.970568 pixeltable-0.2.4/pixeltable/iterators/__init__.py
--rw-r--r--   0        0        0     1545 2024-03-22 03:20:30.970760 pixeltable-0.2.4/pixeltable/iterators/base.py
--rw-r--r--   0        0        0    13105 2024-04-08 22:50:04.685460 pixeltable-0.2.4/pixeltable/iterators/document.py
--rw-r--r--   0        0        0     3444 2024-03-22 03:20:30.991846 pixeltable-0.2.4/pixeltable/iterators/video.py
--rw-r--r--   0        0        0     2083 2024-04-04 00:11:47.502483 pixeltable-0.2.4/pixeltable/metadata/__init__.py
--rw-r--r--   0        0        0      733 2024-03-22 03:20:30.992614 pixeltable-0.2.4/pixeltable/metadata/converters/convert_10.py
--rw-r--r--   0        0        0     7761 2024-04-04 00:11:47.502834 pixeltable-0.2.4/pixeltable/metadata/schema.py
--rw-r--r--   0        0        0    34710 2024-04-04 00:11:47.503153 pixeltable-0.2.4/pixeltable/plan.py
--rw-r--r--   0        0        0    19511 2024-04-08 22:50:04.685849 pixeltable-0.2.4/pixeltable/store.py
--rw-r--r--   0        0        0     6684 2024-04-17 01:12:13.409679 pixeltable-0.2.4/pixeltable/tests/conftest.py
--rw-r--r--   0        0        0     1666 2024-04-17 01:12:13.428542 pixeltable-0.2.4/pixeltable/tests/functions/test_fireworks.py
--rw-r--r--   0        0        0     2884 2024-04-17 01:12:13.428969 pixeltable-0.2.4/pixeltable/tests/functions/test_functions.py
--rw-r--r--   0        0        0     7739 2024-04-17 01:12:13.429213 pixeltable-0.2.4/pixeltable/tests/functions/test_huggingface.py
--rw-r--r--   0        0        0     8172 2024-04-17 01:12:13.429479 pixeltable-0.2.4/pixeltable/tests/functions/test_openai.py
--rw-r--r--   0        0        0     4788 2024-04-17 01:12:13.429686 pixeltable-0.2.4/pixeltable/tests/functions/test_together.py
--rw-r--r--   0        0        0     3186 2024-04-04 00:11:47.504570 pixeltable-0.2.4/pixeltable/tests/test_audio.py
--rw-r--r--   0        0        0     1189 2024-03-22 03:20:31.514506 pixeltable-0.2.4/pixeltable/tests/test_catalog.py
--rw-r--r--   0        0        0      531 2024-04-04 00:11:47.504789 pixeltable-0.2.4/pixeltable/tests/test_client.py
--rw-r--r--   0        0        0    17732 2024-04-06 17:38:28.114456 pixeltable-0.2.4/pixeltable/tests/test_component_view.py
--rw-r--r--   0        0        0    17975 2024-04-17 01:12:13.430071 pixeltable-0.2.4/pixeltable/tests/test_dataframe.py
--rw-r--r--   0        0        0     3611 2024-04-04 00:11:47.505572 pixeltable-0.2.4/pixeltable/tests/test_dirs.py
--rw-r--r--   0        0        0     5810 2024-04-06 17:38:32.384273 pixeltable-0.2.4/pixeltable/tests/test_document.py
--rw-r--r--   0        0        0    32743 2024-04-08 22:50:04.687225 pixeltable-0.2.4/pixeltable/tests/test_exprs.py
--rw-r--r--   0        0        0    12817 2024-04-04 00:11:47.506385 pixeltable-0.2.4/pixeltable/tests/test_function.py
--rw-r--r--   0        0        0     1535 2024-04-04 00:11:47.506868 pixeltable-0.2.4/pixeltable/tests/test_migration.py
--rw-r--r--   0        0        0     2649 2024-04-04 00:11:47.507072 pixeltable-0.2.4/pixeltable/tests/test_nos.py
--rw-r--r--   0        0        0     9297 2024-04-04 00:11:47.507288 pixeltable-0.2.4/pixeltable/tests/test_snapshot.py
--rw-r--r--   0        0        0    53303 2024-04-17 01:12:13.430814 pixeltable-0.2.4/pixeltable/tests/test_table.py
--rw-r--r--   0        0        0     1308 2024-04-04 00:11:47.507879 pixeltable-0.2.4/pixeltable/tests/test_transactional_directory.py
--rw-r--r--   0        0        0      970 2024-04-04 00:11:47.508085 pixeltable-0.2.4/pixeltable/tests/test_types.py
--rw-r--r--   0        0        0     7782 2024-04-06 17:38:32.385556 pixeltable-0.2.4/pixeltable/tests/test_video.py
--rw-r--r--   0        0        0    21859 2024-04-04 00:11:47.508548 pixeltable-0.2.4/pixeltable/tests/test_view.py
--rw-r--r--   0        0        0    14359 2024-04-17 01:12:13.431171 pixeltable-0.2.4/pixeltable/tests/utils.py
--rw-r--r--   0        0        0     5148 2024-04-04 00:11:47.508980 pixeltable-0.2.4/pixeltable/tool/create_test_db_dump.py
--rw-r--r--   0        0        0     2899 2024-04-06 17:38:28.116159 pixeltable-0.2.4/pixeltable/tool/create_test_video.py
--rw-r--r--   0        0        0    30374 2024-04-17 01:12:13.431574 pixeltable-0.2.4/pixeltable/type_system.py
--rw-r--r--   0        0        0      439 2024-03-22 03:20:31.517814 pixeltable-0.2.4/pixeltable/utils/__init__.py
--rw-r--r--   0        0        0     3692 2024-04-17 01:12:13.431812 pixeltable-0.2.4/pixeltable/utils/arrow.py
--rw-r--r--   0        0        0      720 2024-03-22 03:20:31.517938 pixeltable-0.2.4/pixeltable/utils/clip.py
--rw-r--r--   0        0        0     5604 2024-03-22 03:20:31.518069 pixeltable-0.2.4/pixeltable/utils/coco.py
--rw-r--r--   0        0        0     1094 2024-03-22 03:20:31.518173 pixeltable-0.2.4/pixeltable/utils/documents.py
--rw-r--r--   0        0        0     7839 2024-03-22 03:20:31.518306 pixeltable-0.2.4/pixeltable/utils/filecache.py
--rw-r--r--   0        0        0      252 2024-03-22 03:20:31.518421 pixeltable-0.2.4/pixeltable/utils/help.py
--rw-r--r--   0        0        0     7005 2024-04-17 01:12:13.432021 pixeltable-0.2.4/pixeltable/utils/hf_datasets.py
--rw-r--r--   0        0        0     3116 2024-03-22 03:20:31.518536 pixeltable-0.2.4/pixeltable/utils/media_store.py
--rw-r--r--   0        0        0     7120 2024-04-17 01:12:13.432624 pixeltable-0.2.4/pixeltable/utils/parquet.py
--rw-r--r--   0        0        0     3483 2024-04-17 01:12:13.433243 pixeltable-0.2.4/pixeltable/utils/pytorch.py
--rw-r--r--   0        0        0      432 2024-03-22 03:20:31.518890 pixeltable-0.2.4/pixeltable/utils/s3.py
--rw-r--r--   0        0        0      765 2024-03-22 03:20:31.519000 pixeltable-0.2.4/pixeltable/utils/sql.py
--rw-r--r--   0        0        0     1349 2024-04-04 00:11:47.509715 pixeltable-0.2.4/pixeltable/utils/transactional_directory.py
--rw-r--r--   0        0        0     3332 2024-04-17 01:12:13.436364 pixeltable-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     5983 1970-01-01 00:00:00.000000 pixeltable-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      746 2024-03-22 03:20:30.000000 pixeltable-0.2.5/LICENSE
+-rw-r--r--   0        0        0     4778 2024-04-26 23:52:15.843337 pixeltable-0.2.5/README.md
+-rw-r--r--   0        0        0      959 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/__init__.py
+-rw-r--r--   0        0        0      453 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/catalog/__init__.py
+-rw-r--r--   0        0        0     7908 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/catalog/catalog.py
+-rw-r--r--   0        0        0     7887 2024-04-26 23:52:15.860281 pixeltable-0.2.5/pixeltable/catalog/column.py
+-rw-r--r--   0        0        0      919 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/catalog/dir.py
+-rw-r--r--   0        0        0      943 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/catalog/globals.py
+-rw-r--r--   0        0        0     8303 2024-04-26 23:52:15.860489 pixeltable-0.2.5/pixeltable/catalog/insertable_table.py
+-rw-r--r--   0        0        0     1147 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/catalog/named_function.py
+-rw-r--r--   0        0        0     1677 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/catalog/path.py
+-rw-r--r--   0        0        0     5941 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/catalog/path_dict.py
+-rw-r--r--   0        0        0     1059 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/catalog/schema_object.py
+-rw-r--r--   0        0        0    30675 2024-04-26 23:52:15.860760 pixeltable-0.2.5/pixeltable/catalog/table.py
+-rw-r--r--   0        0        0    48818 2024-04-26 23:52:15.861070 pixeltable-0.2.5/pixeltable/catalog/table_version.py
+-rw-r--r--   0        0        0     5482 2024-04-26 23:52:15.861379 pixeltable-0.2.5/pixeltable/catalog/table_version_path.py
+-rw-r--r--   0        0        0     9734 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/catalog/view.py
+-rw-r--r--   0        0        0    23442 2024-04-26 23:52:15.861740 pixeltable-0.2.5/pixeltable/client.py
+-rw-r--r--   0        0        0    30014 2024-04-26 23:52:15.862042 pixeltable-0.2.5/pixeltable/dataframe.py
+-rw-r--r--   0        0        0    16303 2024-04-26 23:52:15.862207 pixeltable-0.2.5/pixeltable/env.py
+-rw-r--r--   0        0        0      376 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exceptions.py
+-rw-r--r--   0        0        0      412 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exec/__init__.py
+-rw-r--r--   0        0        0     3321 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/exec/aggregation_node.py
+-rw-r--r--   0        0        0     5241 2024-04-26 23:52:15.862576 pixeltable-0.2.5/pixeltable/exec/cache_prefetch_node.py
+-rw-r--r--   0        0        0     4069 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exec/component_iteration_node.py
+-rw-r--r--   0        0        0     3505 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exec/data_row_batch.py
+-rw-r--r--   0        0        0      924 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exec/exec_context.py
+-rw-r--r--   0        0        0     2170 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exec/exec_node.py
+-rw-r--r--   0        0        0    10810 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/exec/expr_eval_node.py
+-rw-r--r--   0        0        0     3171 2024-04-26 23:52:15.862984 pixeltable-0.2.5/pixeltable/exec/in_memory_data_node.py
+-rw-r--r--   0        0        0     1514 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exec/media_validation_node.py
+-rw-r--r--   0        0        0    10318 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exec/sql_scan_node.py
+-rw-r--r--   0        0        0      935 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/exprs/__init__.py
+-rw-r--r--   0        0        0     4386 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/arithmetic_expr.py
+-rw-r--r--   0        0        0     2131 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/array_slice.py
+-rw-r--r--   0        0        0     2706 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/column_property_ref.py
+-rw-r--r--   0        0        0     4794 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/column_ref.py
+-rw-r--r--   0        0        0     2964 2024-04-26 23:52:15.863463 pixeltable-0.2.5/pixeltable/exprs/comparison.py
+-rw-r--r--   0        0        0     3830 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/compound_predicate.py
+-rw-r--r--   0        0        0     8278 2024-04-26 23:52:15.863796 pixeltable-0.2.5/pixeltable/exprs/data_row.py
+-rw-r--r--   0        0        0    23748 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/exprs/expr.py
+-rw-r--r--   0        0        0     1222 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/expr_set.py
+-rw-r--r--   0        0        0    16961 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/exprs/function_call.py
+-rw-r--r--   0        0        0     1537 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/globals.py
+-rw-r--r--   0        0        0     4663 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/image_member_access.py
+-rw-r--r--   0        0        0     1906 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/image_similarity_predicate.py
+-rw-r--r--   0        0        0     4312 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/inline_array.py
+-rw-r--r--   0        0        0     3695 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/inline_dict.py
+-rw-r--r--   0        0        0     1041 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/is_null.py
+-rw-r--r--   0        0        0     4559 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/json_mapper.py
+-rw-r--r--   0        0        0     6526 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/json_path.py
+-rw-r--r--   0        0        0     2396 2024-04-26 23:52:15.864641 pixeltable-0.2.5/pixeltable/exprs/literal.py
+-rw-r--r--   0        0        0     1250 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/object_ref.py
+-rw-r--r--   0        0        0     1859 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/predicate.py
+-rw-r--r--   0        0        0    15321 2024-04-26 23:52:15.864817 pixeltable-0.2.5/pixeltable/exprs/row_builder.py
+-rw-r--r--   0        0        0     4268 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/rowid_ref.py
+-rw-r--r--   0        0        0     1793 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/type_cast.py
+-rw-r--r--   0        0        0     1361 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/exprs/variable.py
+-rw-r--r--   0        0        0      269 2024-04-26 23:52:15.864917 pixeltable-0.2.5/pixeltable/ext/__init__.py
+-rw-r--r--   0        0        0     3131 2024-04-26 23:52:15.865002 pixeltable-0.2.5/pixeltable/ext/functions/yolox.py
+-rw-r--r--   0        0        0      457 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/func/__init__.py
+-rw-r--r--   0        0        0     9267 2024-04-26 23:52:15.865380 pixeltable-0.2.5/pixeltable/func/aggregate_function.py
+-rw-r--r--   0        0        0     2350 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/func/batched_function.py
+-rw-r--r--   0        0        0     2357 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/func/callable_function.py
+-rw-r--r--   0        0        0     3807 2024-04-26 23:52:15.865719 pixeltable-0.2.5/pixeltable/func/expr_template_function.py
+-rw-r--r--   0        0        0     4023 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/func/function.py
+-rw-r--r--   0        0        0    11456 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/func/function_registry.py
+-rw-r--r--   0        0        0     1483 2024-04-26 23:52:15.866057 pixeltable-0.2.5/pixeltable/func/globals.py
+-rw-r--r--   0        0        0     9650 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/func/nos_function.py
+-rw-r--r--   0        0        0     7343 2024-04-26 23:52:15.866428 pixeltable-0.2.5/pixeltable/func/signature.py
+-rw-r--r--   0        0        0     6711 2024-04-26 23:52:15.866878 pixeltable-0.2.5/pixeltable/func/udf.py
+-rw-r--r--   0        0        0     3297 2024-04-26 23:52:15.866971 pixeltable-0.2.5/pixeltable/functions/__init__.py
+-rw-r--r--   0        0        0     8404 2024-04-26 23:52:15.867168 pixeltable-0.2.5/pixeltable/functions/eval.py
+-rw-r--r--   0        0        0      908 2024-04-17 01:12:13.000000 pixeltable-0.2.5/pixeltable/functions/fireworks.py
+-rw-r--r--   0        0        0     5693 2024-04-26 23:52:15.867554 pixeltable-0.2.5/pixeltable/functions/huggingface.py
+-rw-r--r--   0        0        0      431 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/functions/image.py
+-rw-r--r--   0        0        0     6870 2024-04-26 23:52:15.867781 pixeltable-0.2.5/pixeltable/functions/openai.py
+-rw-r--r--   0        0        0     6217 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/functions/pil/image.py
+-rw-r--r--   0        0        0      516 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/functions/string.py
+-rw-r--r--   0        0        0     3423 2024-04-17 01:12:13.000000 pixeltable-0.2.5/pixeltable/functions/together.py
+-rw-r--r--   0        0        0     1860 2024-04-26 23:52:15.868147 pixeltable-0.2.5/pixeltable/functions/util.py
+-rw-r--r--   0        0        0     2403 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/functions/video.py
+-rw-r--r--   0        0        0       72 2024-04-26 23:52:15.868217 pixeltable-0.2.5/pixeltable/index/__init__.py
+-rw-r--r--   0        0        0     1362 2024-04-26 23:52:15.868269 pixeltable-0.2.5/pixeltable/index/base.py
+-rw-r--r--   0        0        0     4372 2024-04-26 23:52:15.868362 pixeltable-0.2.5/pixeltable/index/embedding_index.py
+-rw-r--r--   0        0        0       70 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/iterators/__init__.py
+-rw-r--r--   0        0        0     1545 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/iterators/base.py
+-rw-r--r--   0        0        0    13105 2024-04-08 22:50:04.000000 pixeltable-0.2.5/pixeltable/iterators/document.py
+-rw-r--r--   0        0        0     3444 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/iterators/video.py
+-rw-r--r--   0        0        0     2083 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/metadata/__init__.py
+-rw-r--r--   0        0        0      733 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/metadata/converters/convert_10.py
+-rw-r--r--   0        0        0     8335 2024-04-26 23:52:15.868900 pixeltable-0.2.5/pixeltable/metadata/schema.py
+-rw-r--r--   0        0        0    33549 2024-04-26 23:52:15.869190 pixeltable-0.2.5/pixeltable/plan.py
+-rw-r--r--   0        0        0    19426 2024-04-26 23:52:15.869492 pixeltable-0.2.5/pixeltable/store.py
+-rw-r--r--   0        0        0     6339 2024-04-26 23:52:15.879933 pixeltable-0.2.5/pixeltable/tests/conftest.py
+-rw-r--r--   0        0        0     1085 2024-04-26 23:52:15.883996 pixeltable-0.2.5/pixeltable/tests/ext/test_yolox.py
+-rw-r--r--   0        0        0     1690 2024-04-26 23:52:15.884519 pixeltable-0.2.5/pixeltable/tests/functions/test_fireworks.py
+-rw-r--r--   0        0        0     2884 2024-04-17 01:12:13.000000 pixeltable-0.2.5/pixeltable/tests/functions/test_functions.py
+-rw-r--r--   0        0        0     7657 2024-04-26 23:52:15.884812 pixeltable-0.2.5/pixeltable/tests/functions/test_huggingface.py
+-rw-r--r--   0        0        0     8659 2024-04-26 23:52:15.885170 pixeltable-0.2.5/pixeltable/tests/functions/test_openai.py
+-rw-r--r--   0        0        0     4812 2024-04-26 23:52:15.885535 pixeltable-0.2.5/pixeltable/tests/functions/test_together.py
+-rw-r--r--   0        0        0     3186 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/tests/test_audio.py
+-rw-r--r--   0        0        0     1189 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/tests/test_catalog.py
+-rw-r--r--   0        0        0      531 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/tests/test_client.py
+-rw-r--r--   0        0        0    18221 2024-04-26 23:52:15.885726 pixeltable-0.2.5/pixeltable/tests/test_component_view.py
+-rw-r--r--   0        0        0    17906 2024-04-26 23:52:15.885857 pixeltable-0.2.5/pixeltable/tests/test_dataframe.py
+-rw-r--r--   0        0        0     3611 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/tests/test_dirs.py
+-rw-r--r--   0        0        0     5810 2024-04-06 17:38:32.000000 pixeltable-0.2.5/pixeltable/tests/test_document.py
+-rw-r--r--   0        0        0    32181 2024-04-26 23:52:15.886175 pixeltable-0.2.5/pixeltable/tests/test_exprs.py
+-rw-r--r--   0        0        0    12987 2024-04-26 23:52:15.886344 pixeltable-0.2.5/pixeltable/tests/test_function.py
+-rw-r--r--   0        0        0     5410 2024-04-26 23:52:15.886438 pixeltable-0.2.5/pixeltable/tests/test_index.py
+-rw-r--r--   0        0        0     1599 2024-04-26 23:52:15.886763 pixeltable-0.2.5/pixeltable/tests/test_migration.py
+-rw-r--r--   0        0        0     2649 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/tests/test_nos.py
+-rw-r--r--   0        0        0    10331 2024-04-26 23:52:15.887131 pixeltable-0.2.5/pixeltable/tests/test_snapshot.py
+-rw-r--r--   0        0        0    56557 2024-04-26 23:52:15.887436 pixeltable-0.2.5/pixeltable/tests/test_table.py
+-rw-r--r--   0        0        0     1308 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/tests/test_transactional_directory.py
+-rw-r--r--   0        0        0     2045 2024-04-26 23:52:15.887779 pixeltable-0.2.5/pixeltable/tests/test_types.py
+-rw-r--r--   0        0        0     7740 2024-04-26 23:52:15.887909 pixeltable-0.2.5/pixeltable/tests/test_video.py
+-rw-r--r--   0        0        0    22108 2024-04-26 23:52:15.888166 pixeltable-0.2.5/pixeltable/tests/test_view.py
+-rw-r--r--   0        0        0    15106 2024-04-26 23:52:15.888400 pixeltable-0.2.5/pixeltable/tests/utils.py
+-rw-r--r--   0        0        0     5842 2024-04-26 23:52:15.888794 pixeltable-0.2.5/pixeltable/tool/create_test_db_dump.py
+-rw-r--r--   0        0        0     2899 2024-04-06 17:38:28.000000 pixeltable-0.2.5/pixeltable/tool/create_test_video.py
+-rw-r--r--   0        0        0    29929 2024-04-26 23:52:15.888989 pixeltable-0.2.5/pixeltable/type_system.py
+-rw-r--r--   0        0        0      439 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/utils/__init__.py
+-rw-r--r--   0        0        0     3692 2024-04-17 01:12:13.000000 pixeltable-0.2.5/pixeltable/utils/arrow.py
+-rw-r--r--   0        0        0      720 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/utils/clip.py
+-rw-r--r--   0        0        0     5604 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/utils/coco.py
+-rw-r--r--   0        0        0     1094 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/utils/documents.py
+-rw-r--r--   0        0        0     7839 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/utils/filecache.py
+-rw-r--r--   0        0        0      252 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/utils/help.py
+-rw-r--r--   0        0        0     7005 2024-04-17 01:12:13.000000 pixeltable-0.2.5/pixeltable/utils/hf_datasets.py
+-rw-r--r--   0        0        0     3116 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/utils/media_store.py
+-rw-r--r--   0        0        0     7120 2024-04-17 01:12:13.000000 pixeltable-0.2.5/pixeltable/utils/parquet.py
+-rw-r--r--   0        0        0     3483 2024-04-17 01:12:13.000000 pixeltable-0.2.5/pixeltable/utils/pytorch.py
+-rw-r--r--   0        0        0      432 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/utils/s3.py
+-rw-r--r--   0        0        0      765 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/utils/sql.py
+-rw-r--r--   0        0        0     1349 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/utils/transactional_directory.py
+-rw-r--r--   0        0        0     3481 2024-04-26 23:52:15.890789 pixeltable-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     6081 1970-01-01 00:00:00.000000 pixeltable-0.2.5/PKG-INFO
```

### Comparing `pixeltable-0.2.4/LICENSE` & `pixeltable-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/README.md` & `pixeltable-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,20 @@
 
 ## ⚡Quick Start
 Learn the basics of Pixeltable through interactive examples. View the notebooks on Google Colab or Kaggle, for free.
 
 ### Pixeltable Basics
 In this tutorial, we'll survey how to create tables, populate them with data, and enhance them with built-in and user-defined transformations and AI operations.
 
-[![Open in Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/code/brunep/pixeltable-basics) <a target="_blank" href="https://colab.research.google.com/github/pixeltable/pixeltable/blob/master/docs/tutorials/pixeltable-basics.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>
+[![Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://kaggle.com/kernels/welcome?src=https://github.com/pixeltable/pixeltable/blob/master/docs/tutorials/pixeltable-basics.ipynb)&nbsp;&nbsp;
+<a target="_blank" href="https://colab.research.google.com/github/pixeltable/pixeltable/blob/master/docs/tutorials/pixeltable-basics.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>
 
 
 ## 💾 Installation
-Pixeltable works with Python 3.9, 3.10, or 3.11 running on Linux or MacOS.
+Pixeltable works with Python 3.9, 3.10, 3.11, or 3.12 running on Linux, MacOS, or Windows.
 
 ```
 pip install pixeltable
 ```
 
 To verify that it's working:
```

### Comparing `pixeltable-0.2.4/pixeltable/__init__.py` & `pixeltable-0.2.5/pixeltable/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/catalog/catalog.py` & `pixeltable-0.2.5/pixeltable/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/catalog/column.py` & `pixeltable-0.2.5/pixeltable/catalog/column.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,59 @@
 from __future__ import annotations
 
 import logging
 from typing import Optional, Union, Callable, Set
 
 import sqlalchemy as sql
-from pgvector.sqlalchemy import Vector
 
 from pixeltable import exceptions as excs
-from pixeltable.metadata import schema
 from pixeltable.type_system import ColumnType, StringType
 from .globals import is_valid_identifier
 
 _logger = logging.getLogger('pixeltable')
 
 class Column:
     """Representation of a column in the schema of a Table/DataFrame.
 
     A Column contains all the metadata necessary for executing queries and updates against a particular version of a
     table/view.
     """
     def __init__(
-            self, name: str, col_type: Optional[ColumnType] = None,
+            self, name: Optional[str], col_type: Optional[ColumnType] = None,
             computed_with: Optional[Union['Expr', Callable]] = None,
-            primary_key: bool = False, stored: Optional[bool] = None,
-            indexed: bool = False,
-            # these parameters aren't set by users
-            col_id: Optional[int] = None):
+            is_pk: bool = False, stored: Optional[bool] = None,
+            col_id: Optional[int] = None, schema_version_add: Optional[int] = None,
+            schema_version_drop: Optional[int] = None, sa_col_type: Optional[sql.sqltypes.TypeEngine] = None
+    ):
         """Column constructor.
 
         Args:
-            name: column name
+            name: column name; None for system columns (eg, index columns)
             col_type: column type; can be None if the type can be derived from ``computed_with``
             computed_with: a callable or an Expr object that computes the column value
-            primary_key: if True, this column is part of the primary key
+            is_pk: if True, this column is part of the primary key
             stored: determines whether a computed column is present in the stored table or recomputed on demand
-            indexed: if True, this column has a nearest neighbor index (only valid for image columns)
             col_id: column ID (only used internally)
 
         Computed columns: those have a non-None ``computed_with`` argument
-
         - when constructed by the user: ``computed_with`` was constructed explicitly and is passed in;
           col_type is None
         - when loaded from md store: ``computed_with`` is set and col_type is set
 
         ``computed_with`` is a Callable:
-
         - the callable's parameter names must correspond to existing columns in the table for which this Column
           is being used
         - ``col_type`` needs to be set to the callable's return type
 
         ``stored`` (only valid for computed image columns):
-
         - if True: the column is present in the stored table
         - if False: the column is not present in the stored table and recomputed during a query
         - if None: the system chooses for you (at present, this is always False, but this may change in the future)
-
-        indexed: only valid for image columns; if true, maintains an NN index for this column
         """
-        if not is_valid_identifier(name):
+        if name is not None and not is_valid_identifier(name):
             raise excs.Error(f"Invalid column name: '{name}'")
         self.name = name
         if col_type is None and computed_with is None:
             raise excs.Error(f'Column `{name}`: col_type is required if computed_with is not specified')
 
         self.value_expr: Optional['Expr'] = None
         self.compute_func: Optional[Callable] = None
@@ -86,43 +78,28 @@
         if col_type is not None:
             self.col_type = col_type
         assert self.col_type is not None
 
         self.stored = stored
         self.dependent_cols: Set[Column] = set()  # cols with value_exprs that reference us; set by TableVersion
         self.id = col_id
-        self.primary_key = primary_key
+        self.is_pk = is_pk
+        self.schema_version_add = schema_version_add
+        self.schema_version_drop = schema_version_drop
 
         # column in the stored table for the values of this Column
         self.sa_col: Optional[sql.schema.Column] = None
+        self.sa_col_type = sa_col_type
 
         # computed cols also have storage columns for the exception string and type
         self.sa_errormsg_col: Optional[sql.schema.Column] = None
         self.sa_errortype_col: Optional[sql.schema.Column] = None
-        # indexed columns also have a column for the embeddings
-        self.sa_idx_col: Optional[sql.schema.Column] = None
         from .table_version import TableVersion
         self.tbl: Optional[TableVersion] = None  # set by owning TableVersion
 
-        if indexed and not self.col_type.is_image_type():
-            raise excs.Error(f'Column {name}: indexed=True requires ImageType')
-        self.is_indexed = indexed
-
-    @classmethod
-    def from_md(cls, col_id: int, md: schema.SchemaColumn, tbl: 'TableVersion') -> Column:
-        """Construct a Column from metadata.
-
-        Leaves out value_expr, because that requires TableVersion.cols to be complete.
-        """
-        col = cls(
-            md.name, col_type=ColumnType.from_dict(md.col_type), primary_key=md.is_pk,
-            stored=md.stored, indexed=md.is_indexed, col_id=col_id)
-        col.tbl = tbl
-        return col
-
     def __hash__(self) -> int:
         assert self.tbl is not None
         return hash((self.tbl.id, self.id))
 
     def check_value_expr(self) -> None:
         assert self.value_expr is not None
         if self.stored == False and self.is_computed and self.has_window_fn_call():
@@ -163,34 +140,34 @@
 
     def create_sa_cols(self) -> None:
         """
         These need to be recreated for every new table schema version.
         """
         assert self.is_stored
         # all storage columns are nullable (we deal with null errors in Pixeltable directly)
-        self.sa_col = sql.Column(self.storage_name(), self.col_type.to_sa_type(), nullable=True)
+        self.sa_col = sql.Column(
+            self.store_name(), self.col_type.to_sa_type() if self.sa_col_type is None else self.sa_col_type,
+            nullable=True)
         if self.is_computed or self.col_type.is_media_type():
-            self.sa_errormsg_col = sql.Column(self.errormsg_storage_name(), StringType().to_sa_type(), nullable=True)
-            self.sa_errortype_col = sql.Column(self.errortype_storage_name(), StringType().to_sa_type(), nullable=True)
-        if self.is_indexed:
-            self.sa_idx_col = sql.Column(self.index_storage_name(), Vector(512), nullable=True)
+            self.sa_errormsg_col = sql.Column(self.errormsg_store_name(), StringType().to_sa_type(), nullable=True)
+            self.sa_errortype_col = sql.Column(self.errortype_store_name(), StringType().to_sa_type(), nullable=True)
 
-    def storage_name(self) -> str:
+    def get_sa_col_type(self) -> sql.sqltypes.TypeEngine:
+        return self.col_type.to_sa_type() if self.sa_col_type is None else self.sa_col_type
+
+    def store_name(self) -> str:
         assert self.id is not None
         assert self.is_stored
         return f'col_{self.id}'
 
-    def errormsg_storage_name(self) -> str:
-        return f'{self.storage_name()}_errormsg'
-
-    def errortype_storage_name(self) -> str:
-        return f'{self.storage_name()}_errortype'
+    def errormsg_store_name(self) -> str:
+        return f'{self.store_name()}_errormsg'
 
-    def index_storage_name(self) -> str:
-        return f'{self.storage_name()}_idx_0'
+    def errortype_store_name(self) -> str:
+        return f'{self.store_name()}_errortype'
 
     def __str__(self) -> str:
         return f'{self.name}: {self.col_type}'
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Column):
             return False
```

### Comparing `pixeltable-0.2.4/pixeltable/catalog/dir.py` & `pixeltable-0.2.5/pixeltable/catalog/dir.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/catalog/globals.py` & `pixeltable-0.2.5/pixeltable/catalog/globals.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/catalog/insertable_table.py` & `pixeltable-0.2.5/pixeltable/catalog/insertable_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,25 @@
 import sqlalchemy.orm as orm
 
 import pixeltable
 import pixeltable.type_system as ts
 from pixeltable import exceptions as excs
 from pixeltable.env import Env
 from .catalog import Catalog
+from .globals import UpdateStatus
 from .table import Table
 from .table_version import TableVersion
 from .table_version_path import TableVersionPath
 
 _logger = logging.getLogger('pixeltable')
 
+
 class InsertableTable(Table):
     """A `Table` that allows inserting and deleting rows."""
+
     def __init__(self, dir_id: UUID, tbl_version: TableVersion):
         tbl_version_path = TableVersionPath(tbl_version)
         super().__init__(tbl_version.id, dir_id, tbl_version.name, tbl_version_path)
 
     @classmethod
     def display_name(cls) -> str:
         return 'table'
@@ -38,15 +41,15 @@
         column_names = [col.name for col in columns]
         for pk_col in primary_key:
             if pk_col not in column_names:
                 raise excs.Error(f'Primary key column {pk_col} not found in table schema')
             col = columns[column_names.index(pk_col)]
             if col.col_type.nullable:
                 raise excs.Error(f'Primary key column {pk_col} cannot be nullable')
-            col.primary_key = True
+            col.is_pk = True
 
         with orm.Session(Env.get().engine, future=True) as session:
             _, tbl_version = TableVersion.create(session, dir_id, name, columns, num_retained_versions, comment)
             tbl = cls(dir_id, tbl_version)
             session.commit()
             cat = Catalog.get()
             cat.tbl_dependents[tbl._id] = []
@@ -58,15 +61,15 @@
 
     @overload
     def insert(self, rows: Iterable[Dict[str, Any]], /, print_stats: bool = False, fail_on_exception: bool = True): ...
 
     @overload
     def insert(self, print_stats: bool = False, fail_on_exception: bool = True, **kwargs: Any): ...
 
-    def insert(self, *args, **kwargs) -> Table.UpdateStatus:
+    def insert(self, *args, **kwargs) -> UpdateStatus:
         """Insert rows into table.
 
         To insert multiple rows at a time:
 
         ``insert(rows: List[Dict[str, Any]], print_stats: bool = False, fail_on_exception: bool = True)``
 
         To insert just a single row, you can use the more convenient syntax:
@@ -157,15 +160,15 @@
                     # basic sanity checks here
                     checked_val = col.col_type.create_literal(val)
                     row[col_name] = checked_val
                 except TypeError as e:
                     msg = str(e)
                     raise excs.Error(f'Error in column {col.name}: {msg[0].lower() + msg[1:]}\nRow: {row}')
 
-    def delete(self, where: Optional['pixeltable.exprs.Predicate'] = None) -> Table.UpdateStatus:
+    def delete(self, where: Optional['pixeltable.exprs.Predicate'] = None) -> UpdateStatus:
         """Delete rows in this table.
 
         Args:
             where: a Predicate to filter rows to delete.
 
         Examples:
             Delete all rows in a table:
@@ -177,15 +180,15 @@
             >>> tbl.delete(tbl.a > 5)
         """
         from pixeltable.exprs import Predicate
         from pixeltable.plan import Planner
         if where is not None:
             if not isinstance(where, Predicate):
                 raise excs.Error(f"'where' argument must be a Predicate, got {type(where)}")
-            analysis_info = Planner.analyze(self.tbl_version, where)
+            analysis_info = Planner.analyze(self.tbl_version_path, where)
             if analysis_info.similarity_clause is not None:
                 raise excs.Error('nearest() cannot be used with delete()')
             # for now we require that the updated rows can be identified via SQL, rather than via a Python filter
             if analysis_info.filter is not None:
                 raise excs.Error(f'Filter {analysis_info.filter} not expressible in SQL')
 
         return self.tbl_version.delete(where)
```

### Comparing `pixeltable-0.2.4/pixeltable/catalog/named_function.py` & `pixeltable-0.2.5/pixeltable/catalog/named_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/catalog/path.py` & `pixeltable-0.2.5/pixeltable/catalog/path.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/catalog/path_dict.py` & `pixeltable-0.2.5/pixeltable/catalog/path_dict.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/catalog/schema_object.py` & `pixeltable-0.2.5/pixeltable/catalog/schema_object.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/catalog/table.py` & `pixeltable-0.2.5/pixeltable/catalog/table.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,37 @@
 from __future__ import annotations
 
-import dataclasses
 import json
 import logging
 from pathlib import Path
-from typing import Union, Any, List, Dict, Optional, Callable, Set, Tuple
+from typing import Union, Any, List, Dict, Optional, Callable, Set, Tuple, Iterable
 from uuid import UUID
 
 import pandas as pd
 import sqlalchemy as sql
 
 import pixeltable
 import pixeltable.catalog as catalog
 import pixeltable.env as env
 import pixeltable.exceptions as excs
 import pixeltable.exprs as exprs
 import pixeltable.metadata.schema as schema
 import pixeltable.type_system as ts
 from .column import Column
-from .globals import is_valid_identifier, is_system_column_name
+from .globals import is_valid_identifier, is_system_column_name, UpdateStatus
 from .schema_object import SchemaObject
 from .table_version import TableVersion
 from .table_version_path import TableVersionPath
 
 _logger = logging.getLogger('pixeltable')
 
 class Table(SchemaObject):
     """Base class for all tabular SchemaObjects."""
 
-    @dataclasses.dataclass
-    class UpdateStatus:
-        num_rows: int = 0
-        # TODO: change to num_computed_columns (the number of computed slots isn't really meaningful to the user)
-        num_computed_values: int = 0
-        num_excs: int = 0
-        updated_cols: List[str] = dataclasses.field(default_factory=list)
-        cols_with_excs: List[str] = dataclasses.field(default_factory=list)
+    ROWID_COLUMN_NAME = '_rowid'
 
     def __init__(self, id: UUID, dir_id: UUID, name: str, tbl_version_path: TableVersionPath):
         super().__init__(id, name, dir_id)
         self.is_dropped = False
         self.tbl_version_path = tbl_version_path
 
     def move(self, new_name: str, new_dir_id: UUID) -> None:
@@ -221,15 +213,15 @@
     def __setitem__(self, column_name: str, value: Union[ts.ColumnType, exprs.Expr, Callable, dict]) -> None:
         """Adds a column to the table
         Args:
             column_name: the name of the new column
             value: column type or value expression or column specification dictionary:
                 column type: a Pixeltable column type (if the table already contains rows, it must be nullable)
                 value expression: a Pixeltable expression that computes the column values
-                column specification: a dictionary with possible keys 'type', 'value', 'stored', 'indexed'
+                column specification: a dictionary with possible keys 'type', 'value', 'stored'
         Examples:
             Add an int column with ``None`` values:
 
             >>> tbl['new_col'] = IntType(nullable=True)
 
             For a table with int column ``int_col``, add a column that is the factorial of ``int_col``. The names of
             the parameters of the Callable must correspond to existing column names (the column values are then passed
@@ -243,41 +235,35 @@
             (by default, computed image columns are not stored but recomputed on demand):
 
             >>> tbl['rotated'] = tbl.frame.rotate(90)
 
             Do the same, but now the column is stored:
 
             >>> tbl['rotated'] = {'value': tbl.frame.rotate(90), 'stored': True}
-
-            Add a resized version of the ``frame`` column and index it. The column does not need to be stored in order
-            to be indexed:
-
-            >>> tbl['small_frame'] = {'value': tbl.frame.resize([224, 224]), 'indexed': True}
         """
         if not isinstance(column_name, str):
             raise excs.Error(f'Column name must be a string, got {type(column_name)}')
         if not is_valid_identifier(column_name):
             raise excs.Error(f'Invalid column name: {column_name!r}')
 
         new_col = self._create_columns({column_name: value})[0]
         self._verify_column(new_col, self.column_names())
         return self.tbl_version_path.tbl_version.add_column(new_col)
 
     def add_column(
             self, *,
-            type: Optional[ts.ColumnType] = None, stored: Optional[bool] = None, indexed: Optional[bool] = None,
-            print_stats: bool = False, **kwargs: Any
+            type: Optional[ts.ColumnType] = None, stored: Optional[bool] = None, print_stats: bool = False,
+            **kwargs: Any
     ) -> UpdateStatus:
         """Adds a column to the table.
 
         Args:
             kwargs: Exactly one keyword argument of the form ``column-name=type|value-expression``.
             type: The type of the column. Only valid and required if ``value-expression`` is a Callable.
             stored: Whether the column is materialized and stored or computed on demand. Only valid for image columns.
-            indexed: Whether the column is indexed.
             print_stats: If ``True``, print execution metrics.
 
         Returns:
             execution status
 
         Raises:
             Error: If the column name is invalid or already exists.
@@ -314,23 +300,14 @@
             Do the same, but now the column is stored:
 
             >>> tbl.add_column(rotated=tbl.frame.rotate(90), stored=True)
 
             Alternatively, this can also be expressed as:
 
             >>> tbl['rotated'] = {'value': tbl.frame.rotate(90), 'stored': True}
-
-            Add a resized version of the ``frame`` column and index it. The column does not need to be stored in order
-            to be indexed:
-
-            >>> tbl.add_column(small_frame=tbl.frame.resize([224, 224]), indexed=True)
-
-            Alternatively, this can also be expressed as:
-
-            >>> tbl['small_frame'] = {'value': tbl.frame.resize([224, 224]), 'indexed': True}
         """
         self._check_is_dropped()
         # verify kwargs and construct column schema dict
         if len(kwargs) != 1:
             raise excs.Error((
                 f'add_column() requires exactly one keyword argument of the form "column-name=type|value-expression", '
                 f'got {len(kwargs)} instead ({", ".join(list(kwargs.keys()))})'
@@ -345,30 +322,28 @@
             if isinstance(spec, exprs.Expr) and type is not None:
                 raise excs.Error(f'add_column(): keyword argument "type" is redundant')
             col_schema['value'] = spec
         if type is not None:
             col_schema['type'] = type
         if stored is not None:
             col_schema['stored'] = stored
-        if indexed is not None:
-            col_schema['indexed'] = indexed
 
         new_col = self._create_columns({col_name: col_schema})[0]
         self._verify_column(new_col, self.column_names())
         return self.tbl_version_path.tbl_version.add_column(new_col, print_stats=print_stats)
 
     @classmethod
     def _validate_column_spec(cls, name: str, spec: Dict[str, Any]) -> None:
         """Check integrity of user-supplied Column spec
 
         We unfortunately can't use something like jsonschema for validation, because this isn't strictly a JSON schema
         (on account of containing Python Callables or Exprs).
         """
         assert isinstance(spec, dict)
-        valid_keys = {'type', 'value', 'stored', 'indexed'}
+        valid_keys = {'type', 'value', 'stored'}
         has_type = False
         for k in spec.keys():
             if k not in valid_keys:
                 raise excs.Error(f'Column {name}: invalid key {k!r}')
 
         if 'type' in spec:
             has_type = True
@@ -389,28 +364,25 @@
             else:
                 has_type = True
                 if 'type' in spec:
                     raise excs.Error(f'Column {name}: "type" is redundant if value is a Pixeltable expression')
 
         if 'stored' in spec and not isinstance(spec['stored'], bool):
             raise excs.Error(f'Column {name}: "stored" must be a bool, got {spec["stored"]}')
-        if 'indexed' in spec and not isinstance(spec['indexed'], bool):
-            raise excs.Error(f'Column {name}: "indexed" must be a bool, got {spec["indexed"]}')
         if not has_type:
             raise excs.Error(f'Column {name}: "type" is required')
 
     @classmethod
     def _create_columns(cls, schema: Dict[str, Any]) -> List[Column]:
         """Construct list of Columns, given schema"""
         columns: List[Column] = []
         for name, spec in schema.items():
             col_type: Optional[ts.ColumnType] = None
             value_expr: Optional[exprs.Expr] = None
             stored: Optional[bool] = None
-            indexed: Optional[bool] = None
             primary_key: Optional[bool] = None
 
             if isinstance(spec, ts.ColumnType):
                 # TODO: create copy
                 col_type = spec
             elif isinstance(spec, exprs.Expr):
                 # create copy so we can modify it
@@ -424,20 +396,18 @@
                 cls._validate_column_spec(name, spec)
                 col_type = spec.get('type')
                 value_expr = spec.get('value')
                 if value_expr is not None and isinstance(value_expr, exprs.Expr):
                     # create copy so we can modify it
                     value_expr = value_expr.copy()
                 stored = spec.get('stored')
-                indexed = spec.get('indexed')
                 primary_key = spec.get('primary_key')
 
             column = Column(
-                name, col_type=col_type, computed_with=value_expr, stored=stored, indexed=indexed,
-                primary_key=primary_key)
+                name, col_type=col_type, computed_with=value_expr, stored=stored, is_pk=primary_key)
             columns.append(column)
         return columns
 
     @classmethod
     def _verify_column(cls, col: Column, existing_column_names: Set[str]) -> None:
         """Check integrity of user-supplied Column and supply defaults"""
         if is_system_column_name(col.name):
@@ -494,88 +464,224 @@
             Rename column ``factorial`` to ``fac``:
 
             >>> tbl.rename_column('factorial', 'fac')
         """
         self._check_is_dropped()
         self.tbl_version_path.tbl_version.rename_column(old_name, new_name)
 
+    def add_embedding_index(
+            self, col_name: str, *, idx_name: Optional[str] = None,
+            text_embed: Optional[pixeltable.Function] = None, img_embed: Optional[pixeltable.Function] = None
+    ) -> None:
+        """Add an index to the table.
+        Args:
+            col_name: name of column to index
+            idx_name: name of index, which needs to be unique for the table; if not provided, a name will be generated
+            idx_type: type of index (one of 'embedding')
+
+        Raises:
+            Error: If an index with that name already exists for the table or if the column does not exist.
+
+        Examples:
+            Add an index to the ``img`` column:
+
+            >>> tbl.add_embedding_index('img', text_embed=...)
+
+            Add another index to the ``img`` column, with a specific name:
+
+            >>> tbl.add_embedding_index('img', idx_name='clip_idx', text_embed=...)
+        """
+        if self.tbl_version_path.is_snapshot():
+            raise excs.Error('Cannot add an index to a snapshot')
+        self._check_is_dropped()
+        col = self.tbl_version_path.get_column(col_name, include_bases=True)
+        if col is None:
+            raise excs.Error(f'Column {col_name} unknown')
+        if idx_name is not None and idx_name in self.tbl_version_path.tbl_version.idxs_by_name:
+            raise excs.Error(f'Duplicate index name: {idx_name}')
+        from pixeltable.index import EmbeddingIndex
+        # create the EmbeddingIndex instance to verify args
+        idx = EmbeddingIndex(col, text_embed=text_embed, img_embed=img_embed)
+        status = self.tbl_version_path.tbl_version.add_index(col, idx_name=idx_name, idx=idx)
+        # TODO: how to deal with exceptions here? drop the index and raise?
+
+    def drop_index(self, *, column_name: Optional[str] = None, idx_name: Optional[str] = None) -> None:
+        """Drop an index from the table.
+
+        Args:
+            column_name: The name of the column whose index to drop. Invalid if the column has multiple indices.
+            idx_name: The name of the index to drop.
+
+        Raises:
+            Error: If the index does not exist.
+
+        Examples:
+            Drop index on the ``img`` column:
+
+            >>> tbl.drop_index(column_name='img')
+        """
+        if self.tbl_version_path.is_snapshot():
+            raise excs.Error('Cannot drop an index from a snapshot')
+        self._check_is_dropped()
+        if (column_name is None) == (idx_name is None):
+            raise excs.Error('Exactly one of column_name or idx_name must be provided')
+        tbl_version = self.tbl_version_path.tbl_version
+
+        if idx_name is not None:
+            if idx_name not in tbl_version.idxs_by_name:
+                raise excs.Error(f'Index {idx_name} does not exist')
+            idx_id = tbl_version.idxs_by_name[idx_name].id
+        else:
+            col = self.tbl_version_path.get_column(column_name, include_bases=True)
+            if col is None:
+                raise excs.Error(f'Column {column_name} unknown')
+            if col.tbl.id != tbl_version.id:
+                raise excs.Error(
+                    f'Column {column_name}: cannot drop index from column that belongs to base ({col.tbl.name})')
+            idx_ids = [info.id for info in tbl_version.idxs_by_name.values() if info.col.id == col.id]
+            if len(idx_ids) == 0:
+                raise excs.Error(f'Column {column_name} does not have an index')
+            if len(idx_ids) > 1:
+                raise excs.Error(f'Column {column_name} has multiple indices; specify idx_name instead')
+            idx_id = idx_ids[0]
+        self.tbl_version_path.tbl_version.drop_index(idx_id)
+
     def update(
-            self, value_spec: Dict[str, Union['pixeltable.exprs.Expr', Any]],
-            where: Optional['pixeltable.exprs.Predicate'] = None, cascade: bool = True
+            self, value_spec: dict[str, Any], where: Optional['pixeltable.exprs.Predicate'] = None, cascade: bool = True
     ) -> UpdateStatus:
         """Update rows in this table.
 
         Args:
             value_spec: a dictionary mapping column names to literal values or Pixeltable expressions.
             where: a Predicate to filter rows to update.
             cascade: if True, also update all computed columns that transitively depend on the updated columns.
 
         Examples:
-            Set newly-added column `int_col` to 1 for all rows:
+            Set column `int_col` to 1 for all rows:
 
             >>> tbl.update({'int_col': 1})
 
-            Set newly-added column `int_col` to 1 for all rows where `int_col` is 0:
+            Set column `int_col` to 1 for all rows where `int_col` is 0:
 
             >>> tbl.update({'int_col': 1}, where=tbl.int_col == 0)
 
             Set `int_col` to the value of `other_int_col` + 1:
 
             >>> tbl.update({'int_col': tbl.other_int_col + 1})
 
             Increment `int_col` by 1 for all rows where `int_col` is 0:
 
             >>> tbl.update({'int_col': tbl.int_col + 1}, where=tbl.int_col == 0)
         """
+        if self.tbl_version_path.is_snapshot():
+            raise excs.Error('Cannot update a snapshot')
+        self._check_is_dropped()
+
+        update_spec = self._validate_update_spec(value_spec, allow_pk=False, allow_exprs=True)
+        from pixeltable.plan import Planner
+        if where is not None:
+            if not isinstance(where, exprs.Predicate):
+                raise excs.Error(f"'where' argument must be a Predicate, got {type(where)}")
+            analysis_info = Planner.analyze(self.tbl_version_path, where)
+            if analysis_info.similarity_clause is not None:
+                raise excs.Error('nearest() cannot be used with update()')
+            # for now we require that the updated rows can be identified via SQL, rather than via a Python filter
+            if analysis_info.filter is not None:
+                raise excs.Error(f'Filter {analysis_info.filter} not expressible in SQL')
+
+        return self.tbl_version_path.tbl_version.update(update_spec, where, cascade)
+
+    def batch_update(self, rows: Iterable[dict[str, Any]], cascade: bool = True) -> UpdateStatus:
+        """Update rows in this table.
+
+        Args:
+            rows: an Iterable of dictionaries containing values for the updated columns plus values for the primary key
+                  columns.
+            cascade: if True, also update all computed columns that transitively depend on the updated columns.
+
+        Examples:
+            Update the 'name' and 'age' columns for the rows with ids 1 and 2 (assuming 'id' is the primary key):
+
+            >>> tbl.update([{'id': 1, 'name': 'Alice', 'age': 30}, {'id': 2, 'name': 'Bob', 'age': 40}])
+        """
+        if self.tbl_version_path.is_snapshot():
+            raise excs.Error('Cannot update a snapshot')
+        self._check_is_dropped()
+
+        row_updates: List[Dict[Column, exprs.Expr]] = []
+        pk_col_names = set(c.name for c in self.tbl_version_path.tbl_version.primary_key_columns())
+
+        # pseudo-column _rowid: contains the rowid of the row to update and can be used instead of the primary key
+        has_rowid = self.ROWID_COLUMN_NAME in rows[0]
+        rowids: list[Tuple[int, ...]] = []
+        if len(pk_col_names) == 0 and not has_rowid:
+            raise excs.Error('Table must have primary key for batch update')
+
+        for row_spec in rows:
+            col_vals = self._validate_update_spec(row_spec, allow_pk=not has_rowid, allow_exprs=False)
+            if has_rowid:
+                # we expect the _rowid column to be present for each row
+                assert self.ROWID_COLUMN_NAME in row_spec
+                rowids.append(row_spec[self.ROWID_COLUMN_NAME])
+            else:
+                col_names = set(col.name for col in col_vals.keys())
+                if any(pk_col_name not in col_names for pk_col_name in pk_col_names):
+                    missing_cols = pk_col_names - set(col.name for col in col_vals.keys())
+                    raise excs.Error(f'Primary key columns ({", ".join(missing_cols)}) missing in {row_spec}')
+            row_updates.append(col_vals)
+        return self.tbl_version_path.tbl_version.batch_update(row_updates, rowids, cascade)
+
+    def _validate_update_spec(
+            self, value_spec: dict[str, Any], allow_pk: bool, allow_exprs: bool
+    ) -> dict[Column, 'pixeltable.exprs.Expr']:
         from pixeltable import exprs
-        update_targets: List[Tuple[Column, exprs.Expr]] = []
+        update_targets: dict[Column, exprs.Expr] = {}
         for col_name, val in value_spec.items():
             if not isinstance(col_name, str):
                 raise excs.Error(f'Update specification: dict key must be column name, got {col_name!r}')
+            if col_name == self.ROWID_COLUMN_NAME:
+                # ignore pseudo-column _rowid
+                continue
             col = self.tbl_version_path.get_column(col_name, include_bases=False)
             if col is None:
                 # TODO: return more informative error if this is trying to update a base column
                 raise excs.Error(f'Column {col_name} unknown')
             if col.is_computed:
                 raise excs.Error(f'Column {col_name} is computed and cannot be updated')
-            if col.primary_key:
+            if col.is_pk and not allow_pk:
                 raise excs.Error(f'Column {col_name} is a primary key column and cannot be updated')
             if col.col_type.is_media_type():
                 raise excs.Error(f'Column {col_name} has type image/video/audio/document and cannot be updated')
 
             # make sure that the value is compatible with the column type
-            # check if this is a literal
             try:
+                # check if this is a literal
                 value_expr = exprs.Literal(val, col_type=col.col_type)
             except TypeError:
+                if not allow_exprs:
+                    raise excs.Error(
+                        f'Column {col_name}: value {val!r} is not a valid literal for this column '
+                        f'(expected {col.col_type})')
                 # it's not a literal, let's try to create an expr from it
                 value_expr = exprs.Expr.from_object(val)
                 if value_expr is None:
                     raise excs.Error(f'Column {col_name}: value {val!r} is not a recognized literal or expression')
                 if not col.col_type.matches(value_expr.col_type):
                     raise excs.Error((
                         f'Type of value {val!r} ({value_expr.col_type}) is not compatible with the type of column '
                         f'{col_name} ({col.col_type})'
                     ))
-            update_targets.append((col, value_expr))
+            update_targets[col] = value_expr
 
-        from pixeltable.plan import Planner
-        if where is not None:
-            if not isinstance(where, exprs.Predicate):
-                raise excs.Error(f"'where' argument must be a Predicate, got {type(where)}")
-            analysis_info = Planner.analyze(self.tbl_version_path, where)
-            if analysis_info.similarity_clause is not None:
-                raise excs.Error('nearest() cannot be used with update()')
-            # for now we require that the updated rows can be identified via SQL, rather than via a Python filter
-            if analysis_info.filter is not None:
-                raise excs.Error(f'Filter {analysis_info.filter} not expressible in SQL')
+        return update_targets
 
-        return self.tbl_version_path.tbl_version.update(update_targets, where, cascade)
 
     def revert(self) -> None:
         """Reverts the table to the previous version.
 
         .. warning::
             This operation is irreversible.
         """
+        if self.tbl_version_path.is_snapshot():
+            raise excs.Error('Cannot revert a snapshot')
         self._check_is_dropped()
         self.tbl_version_path.tbl_version.revert()
```

### Comparing `pixeltable-0.2.4/pixeltable/catalog/table_version.py` & `pixeltable-0.2.5/pixeltable/catalog/table_version.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,38 +9,49 @@
 from uuid import UUID
 
 import sqlalchemy as sql
 import sqlalchemy.orm as orm
 
 import pixeltable
 import pixeltable.func as func
-from pixeltable import exceptions as excs
+import pixeltable.type_system as ts
+import pixeltable.exceptions as excs
+import pixeltable.index as index
 from pixeltable.env import Env
 from pixeltable.iterators import ComponentIterator
 from pixeltable.metadata import schema
 from pixeltable.utils.filecache import FileCache
 from pixeltable.utils.media_store import MediaStore
 from .column import Column
 from .globals import UpdateStatus, POS_COLUMN_NAME, is_valid_identifier
 
 _logger = logging.getLogger('pixeltable')
 
 class TableVersion:
     """
-    TableVersion represents a particular version of a table/view along with its store table:
+    TableVersion represents a particular version of a table/view along with its physical representation:
+    - the physical representation is a store table with indices
     - the version can be mutable or a snapshot
     - tables and their recursive views form a tree, and a mutable TableVersion also records its own
       mutable views in order to propagate updates
     - each view TableVersion records its base:
       * the base is correct only for mutable views (snapshot versions form a DAG, not a tree)
       * the base is useful for getting access to the StoreTable and the base id
       * TODO: create a separate hierarchy of objects that records the version-independent tree of tables/views, and
         have TableVersions reference those
     - mutable TableVersions record their TableVersionPath, which is needed for expr evaluation in updates
     """
+    @dataclasses.dataclass
+    class IndexInfo:
+        id: int
+        idx: index.IndexBase
+        col: Column
+        val_col: Column
+        undo_col: Column
+
 
     def __init__(
             self, id: UUID, tbl_md: schema.TableMd, version: int, schema_version_md: schema.TableSchemaVersionMd,
             base: Optional[TableVersion] = None, base_path: Optional['pixeltable.catalog.TableVersionPath'] = None,
             is_snapshot: Optional[bool] = None
     ):
         # only one of base and base_path can be non-None
@@ -63,20 +74,21 @@
             self.path = None
         else:
             self.path = TableVersionPath(self, base=base_path) if base_path is not None else TableVersionPath(self)
 
         self.base = base_path.tbl_version if base_path is not None else base
         if self.is_snapshot:
             self.next_col_id = -1
+            self.next_idx_id = -1  # TODO: can snapshots have separate indices?
             self.next_rowid = -1
         else:
             assert tbl_md.current_version == self.version
             self.next_col_id = tbl_md.next_col_id
+            self.next_idx_id = tbl_md.next_idx_id
             self.next_rowid = tbl_md.next_row_id
-        self.column_history = tbl_md.column_history
 
         # view-specific initialization
         from pixeltable import exprs
         predicate_dict = None if not is_view or tbl_md.view_md.predicate is None else tbl_md.view_md.predicate
         self.predicate = exprs.Expr.from_dict(predicate_dict) if predicate_dict is not None else None
         self.mutable_views: List[TableVersion] = []  # targets for update propagation
         if self.base is not None and not self.base.is_snapshot and not self.is_snapshot:
@@ -97,75 +109,73 @@
             assert tbl_md.view_md.iterator_args is not None
 
         # register this table version now so that it's available when we're re-creating value exprs
         import pixeltable.catalog as catalog
         cat = catalog.Catalog.get()
         cat.tbl_versions[(self.id, self.effective_version)] = self
 
-        # do this after we determined whether we're a component view, and before we create the store table
-        self._init_schema(schema_version_md)
+        # init schema after we determined whether we're a component view, and before we create the store table
+        self.cols: List[Column] = []  # contains complete history of columns, incl dropped ones
+        self.cols_by_name: dict[str, Column] = {}  # contains only user-facing (named) columns visible in this version
+        self.cols_by_id: dict[int, Column] = {}  # contains only columns visible in this version
+        self.idx_md = tbl_md.index_md  # needed for _create_tbl_md()
+        self.idxs_by_name: dict[str, TableVersion.IndexInfo] = {}  # contains only actively maintained indices
+        self._init_schema(tbl_md, schema_version_md)
 
     def __hash__(self) -> int:
         return hash(self.id)
 
     def create_snapshot_copy(self) -> TableVersion:
         """Create a snapshot copy of this TableVersion"""
         assert not self.is_snapshot
         return TableVersion(
-            self.id, self._create_md(), self.version,
+            self.id, self._create_tbl_md(), self.version,
             self._create_schema_version_md(preceding_schema_version=0),  # preceding_schema_version: dummy value
             is_snapshot=True, base=self.base)
 
     @classmethod
     def create(
-            cls, session: orm.Session, dir_id: UUID, name: str, cols: List[Column], num_retained_versions: int, comment: str,
-            base_path: Optional['pixeltable.catalog.TableVersionPath'] = None, view_md: Optional[schema.ViewMd] = None
+            cls, session: orm.Session, dir_id: UUID, name: str, cols: List[Column], num_retained_versions: int,
+            comment: str, base_path: Optional['pixeltable.catalog.TableVersionPath'] = None,
+            view_md: Optional[schema.ViewMd] = None
     ) -> Tuple[UUID, Optional[TableVersion]]:
         # assign ids
         cols_by_name: Dict[str, Column] = {}
         for pos, col in enumerate(cols):
             col.id = pos
+            col.schema_version_add = 0
             cols_by_name[col.name] = col
             if col.value_expr is None and col.compute_func is not None:
                 cls._create_value_expr(col, base_path)
             if col.is_computed:
                 col.check_value_expr()
 
         ts = time.time()
         # create schema.Table
-        column_history = {
-            col.id: schema.ColumnHistory(col_id=col.id, schema_version_add=0, schema_version_drop=None)
-            for col in cols
-        }
+        # Column.dependent_cols for existing cols is wrong at this point, but init() will set it correctly
+        column_md = cls._create_column_md(cols)
         table_md = schema.TableMd(
             name=name, current_version=0, current_schema_version=0,
-            next_col_id=len(cols), next_row_id=0, column_history=column_history,
-            view_md=view_md)
+            next_col_id=len(cols), next_idx_id=0, next_row_id=0, column_md=column_md, index_md={}, view_md=view_md)
         tbl_record = schema.Table(dir_id=dir_id, md=dataclasses.asdict(table_md))
         session.add(tbl_record)
         session.flush()  # sets tbl_record.id
         assert tbl_record.id is not None
 
         # create schema.TableVersion
         table_version_md = schema.TableVersionMd(created_at=ts, version=0, schema_version=0)
         tbl_version_record = schema.TableVersion(
             tbl_id=tbl_record.id, version=0, md=dataclasses.asdict(table_version_md))
         session.add(tbl_version_record)
 
         # create schema.TableSchemaVersion
-        column_md: Dict[int, schema.SchemaColumn] = {}
-        for pos, col in enumerate(cols):
-            # Column.dependent_cols for existing cols is wrong at this point, but init() will set it correctly
-            value_expr_dict = col.value_expr.as_dict() if col.value_expr is not None else None
-            column_md[col.id] = schema.SchemaColumn(
-                pos=pos, name=col.name, col_type=col.col_type.as_dict(),
-                is_pk=col.primary_key, value_expr=value_expr_dict, stored=col.stored, is_indexed=col.is_indexed)
+        schema_col_md = {col.id: schema.SchemaColumn(pos=pos, name=col.name) for pos, col in enumerate(cols)}
 
         schema_version_md = schema.TableSchemaVersionMd(
-            schema_version=0, preceding_schema_version=None, columns=column_md,
+            schema_version=0, preceding_schema_version=None, columns=schema_col_md,
             num_retained_versions=num_retained_versions, comment=comment)
         schema_version_record = schema.TableSchemaVersion(
             tbl_id=tbl_record.id, schema_version=0, md=dataclasses.asdict(schema_version_md))
         session.add(schema_version_record)
 
         # if this is purely a snapshot (it doesn't require any additional storage for columns and it # doesn't have a
         # predicate to apply at runtime), we don't create a physical table and simply use the base's table version path
@@ -198,62 +208,185 @@
 
         # de-register table version from catalog
         from .catalog import Catalog
         cat = Catalog.get()
         del cat.tbl_versions[(self.id, self.effective_version)]
         # TODO: remove from tbl_dependents
 
-    def _init_schema(self, schema_version_md: schema.TableSchemaVersionMd) -> None:
-        """Initialize self.cols as well as self.store_tbl"""
-        self.cols = [Column.from_md(col_id, col_md, self) for col_id, col_md in schema_version_md.columns.items()]
-        self.cols_by_name = {col.name: col for col in self.cols}
-        self.cols_by_id = {col.id: col for col in self.cols}
-
-        # make sure to traverse columns ordered by position = order in which cols were created;
-        # this guarantees that references always point backwards
-        from pixeltable import exprs
-        for col, col_md in zip(self.cols, schema_version_md.columns.values()):
+    def _init_schema(self, tbl_md: schema.TableMd, schema_version_md: schema.TableSchemaVersionMd) -> None:
+        # create columns first, so the indices can reference them
+        self._init_cols(tbl_md, schema_version_md)
+        self._init_idxs(tbl_md)
+        # create the sa schema only after creating the columns and indices
+        self._init_sa_schema()
+
+    def _init_cols(self, tbl_md: schema.TableMd, schema_version_md: schema.TableSchemaVersionMd) -> None:
+        """Initialize self.cols with the columns visible in our effective version"""
+        import pixeltable.exprs as exprs
+        self.cols = []
+        self.cols_by_name = {}
+        self.cols_by_id = {}
+        for col_md in tbl_md.column_md.values():
+            col_name = schema_version_md.columns[col_md.id].name if col_md.id in schema_version_md.columns else None
+            col = Column(
+                col_id=col_md.id, name=col_name, col_type=ts.ColumnType.from_dict(col_md.col_type),
+                is_pk=col_md.is_pk, stored=col_md.stored,
+                schema_version_add=col_md.schema_version_add, schema_version_drop=col_md.schema_version_drop)
             col.tbl = self
+            self.cols.append(col)
+
+            # populate the lookup structures before Expr.from_dict()
+            if col_md.schema_version_add > self.schema_version:
+                # column was added after this version
+                continue
+            if col_md.schema_version_drop is not None and col_md.schema_version_drop <= self.schema_version:
+                # column was dropped
+                continue
+            if col.name is not None:
+                self.cols_by_name[col.name] = col
+            self.cols_by_id[col.id] = col
+
+            # make sure to traverse columns ordered by position = order in which cols were created;
+            # this guarantees that references always point backwards
             if col_md.value_expr is not None:
                 col.value_expr = exprs.Expr.from_dict(col_md.value_expr)
                 self._record_value_expr(col)
 
+    def _init_idxs(self, tbl_md: schema.TableMd) -> None:
+        self.idx_md = tbl_md.index_md
+        self.idxs_by_name = {}
+        import pixeltable.index as index_module
+        for md in tbl_md.index_md.values():
+            if md.schema_version_add > self.schema_version \
+                    or md.schema_version_drop is not None and md.schema_version_drop <= self.schema_version:
+                # column not visible in this schema version
+                continue
+
+            # instantiate index object
+            cls_name = md.class_fqn.rsplit('.', 1)[-1]
+            cls = getattr(index_module, cls_name)
+            idx_col = self.cols_by_id[md.indexed_col_id]
+            idx = cls.from_dict(idx_col, md.init_args)
+
+            # fix up the sa column type of the index value and undo columns
+            val_col = self.cols_by_id[md.index_val_col_id]
+            val_col.sa_col_type = idx.index_sa_type()
+            undo_col = self.cols_by_id[md.index_val_undo_col_id]
+            undo_col.sa_col_type = idx.index_sa_type()
+            idx_info = self.IndexInfo(id=md.id, idx=idx, col=idx_col, val_col=val_col, undo_col=undo_col)
+            self.idxs_by_name[md.name] = idx_info
+
+    def _init_sa_schema(self) -> None:
         # create the sqlalchemy schema; do this after instantiating columns, in order to determine whether they
         # need to record errors
         from pixeltable.store import StoreBase, StoreTable, StoreView, StoreComponentView
         if self.is_component_view():
             self.store_tbl: StoreBase = StoreComponentView(self)
         elif self.is_view():
             self.store_tbl: StoreBase = StoreView(self)
         else:
             self.store_tbl: StoreBase = StoreTable(self)
 
-    def _update_md(
-            self, ts: float, preceding_schema_version: Optional[int], conn: sql.engine.Connection) -> None:
+    def _update_md(self, ts: float, preceding_schema_version: Optional[int], conn: sql.engine.Connection) -> None:
         """Update all recorded metadata in response to a data or schema change.
         Args:
             ts: timestamp of the change
             preceding_schema_version: last schema version if schema change, else None
         """
         conn.execute(
             sql.update(schema.Table.__table__)
-                .values({schema.Table.md: dataclasses.asdict(self._create_md())})
+                .values({schema.Table.md: dataclasses.asdict(self._create_tbl_md())})
                 .where(schema.Table.id == self.id))
+
         version_md = self._create_version_md(ts)
         conn.execute(
             sql.insert(schema.TableVersion.__table__)
                 .values(tbl_id=self.id, version=self.version, md=dataclasses.asdict(version_md)))
         if preceding_schema_version is not None:
             schema_version_md = self._create_schema_version_md(preceding_schema_version)
             conn.execute(
                 sql.insert(schema.TableSchemaVersion.__table__)
                 .values(
                     tbl_id=self.id, schema_version=self.schema_version,
                     md=dataclasses.asdict(schema_version_md)))
 
+    def _store_idx_name(self, idx_id: int) -> str:
+        """Return name of index in the store, which needs to be globally unique"""
+        return f'idx_{self.id.hex}_{idx_id}'
+
+    def add_index(self, col: Column, idx_name: Optional[str], idx: index.IndexBase) -> UpdateStatus:
+        assert not self.is_snapshot
+        idx_id = self.next_idx_id
+        self.next_idx_id += 1
+        if idx_name is None:
+            idx_name = f'idx{idx_id}'
+        else:
+            assert is_valid_identifier(idx_name)
+            assert idx_name not in [i.name for i in self.idx_md.values()]
+
+        # we're creating a new schema version
+        self.version += 1
+        preceding_schema_version = self.schema_version
+        self.schema_version = self.version
+        with Env.get().engine.begin() as conn:
+            # add the index value and undo columns (which need to be nullable);
+            # we don't create a new schema version, because indices aren't part of the logical schema
+            val_col = Column(
+                col_id=self.next_col_id, name=None, computed_with=idx.index_value_expr(),
+                sa_col_type=idx.index_sa_type(), stored=True,
+                schema_version_add=self.schema_version, schema_version_drop=None)
+            val_col.tbl = self
+            val_col.col_type.nullable = True
+            self.next_col_id += 1
+
+            undo_col = Column(
+                col_id=self.next_col_id, name=None, col_type=val_col.col_type,
+                sa_col_type=val_col.sa_col_type, stored=True,
+                schema_version_add=self.schema_version, schema_version_drop=None)
+            undo_col.tbl = self
+            undo_col.col_type.nullable = True
+            self.next_col_id += 1
+
+            # create and register the index metadata
+            idx_cls = type(idx)
+            idx_md = schema.IndexMd(
+                id=idx_id, name=idx_name,
+                indexed_col_id=col.id, index_val_col_id=val_col.id, index_val_undo_col_id=undo_col.id,
+                schema_version_add=self.schema_version, schema_version_drop=None,
+                class_fqn=idx_cls.__module__ + '.' + idx_cls.__name__, init_args=idx.as_dict())
+            idx_info = self.IndexInfo(id=idx_id, idx=idx, col=col, val_col=val_col, undo_col=undo_col)
+            self.idx_md[idx_id] = idx_md
+            self.idxs_by_name[idx_name] = idx_info
+
+            # add the columns and update the metadata
+            status = self._add_columns([val_col, undo_col], conn, preceding_schema_version=preceding_schema_version)
+            # now create the index structure
+            idx.create_index(self._store_idx_name(idx_id), val_col, conn)
+
+        _logger.info(f'Added index {idx_name} on column {col.name} to table {self.name}')
+        return status
+
+    def drop_index(self, idx_id: int) -> None:
+        assert not self.is_snapshot
+        assert idx_id in self.idx_md
+
+        # we're creating a new schema version
+        self.version += 1
+        preceding_schema_version = self.schema_version
+        self.schema_version = self.version
+        idx_md = self.idx_md[idx_id]
+        idx_md.schema_version_drop = self.schema_version
+        assert idx_md.name in self.idxs_by_name
+        idx_info = self.idxs_by_name[idx_md.name]
+        del self.idxs_by_name[idx_md.name]
+
+        with Env.get().engine.begin() as conn:
+            self._drop_columns([idx_info.val_col, idx_info.undo_col], conn, preceding_schema_version)
+            _logger.info(f'Dropped index {idx_md.name} on table {self.name}')
+
     def add_column(self, col: Column, print_stats: bool = False) -> UpdateStatus:
         """Adds a column to the table.
         """
         assert not self.is_snapshot
         assert is_valid_identifier(col.name)
         assert col.stored is not None
         assert col.name not in self.cols_by_name
@@ -264,105 +397,154 @@
         if col.compute_func is not None:
             # create value_expr from compute_func
             self._create_value_expr(col, self.path)
         if col.value_expr is not None:
             col.check_value_expr()
             self._record_value_expr(col)
 
-        row_count = self.store_tbl.count()
-        if row_count > 0 and not col.col_type.nullable and not col.is_computed:
-            raise excs.Error(f'Cannot add non-nullable column "{col.name}" to table {self.name} with existing rows')
-
         # we're creating a new schema version
-        ts = time.time()
         self.version += 1
         preceding_schema_version = self.schema_version
         self.schema_version = self.version
+        with Env.get().engine.begin() as conn:
+            status = self._add_columns([col], conn, preceding_schema_version, print_stats=print_stats)
+        _logger.info(f'Added column {col.name} to table {self.name}, new version: {self.version}')
+
+        msg = (
+            f'Added {status.num_rows} column value{"" if status.num_rows == 1 else "s"} '
+            f'with {status.num_excs} error{"" if status.num_excs == 1 else "s"}.'
+        )
+        print(msg)
+        _logger.info(f'Column {col.name}: {msg}')
+        return status
 
-        self.cols.append(col)
-        self.cols_by_name[col.name] = col
-        self.cols_by_id[col.id] = col
-        self.column_history[col.id] = schema.ColumnHistory(col.id, self.schema_version, None)
+    def _add_columns(
+            self, cols: List[Column], conn: sql.engine.Connection, preceding_schema_version: Optional[int] = None,
+            print_stats: bool = False
+    ) -> UpdateStatus:
+        """Add and populate columns within the current transaction"""
+        ts = time.time()
+
+        row_count = self.store_tbl.count(conn=conn)
+        for col in cols:
+            if not col.col_type.nullable and not col.is_computed:
+                if row_count > 0:
+                    raise excs.Error(
+                        f'Cannot add non-nullable column "{col.name}" to table {self.name} with existing rows')
+
+        num_excs = 0
+        cols_with_excs: List[Column] = []
+        for col in cols:
+            col.schema_version_add = self.schema_version
+            # add the column to the lookup structures now, rather than after the store changes executed successfully,
+            # because it might be referenced by the next column's value_expr
+            self.cols.append(col)
+            if col.name is not None:
+                self.cols_by_name[col.name] = col
+            self.cols_by_id[col.id] = col
 
-        with Env.get().engine.begin() as conn:
-            self._update_md(ts, preceding_schema_version, conn)
-            _logger.info(f'Added column {col.name} to table {self.name}, new version: {self.version}')
             if col.is_stored:
                 self.store_tbl.add_column(col, conn)
 
-        print(f'Added column `{col.name}` to table `{self.name}`.')
-        if row_count == 0:
-            return UpdateStatus()
-        if (not col.is_computed or not col.is_stored) and not col.is_indexed:
-            return UpdateStatus(num_rows=row_count)
-        # compute values for the existing rows and compute embeddings, if this column is indexed;
-        # for some reason, it's not possible to run the following updates in the same transaction as the one
-        # that we just used to create the metadata (sqlalchemy hangs when exec() tries to run the query)
-        from pixeltable.plan import Planner
-        plan, value_expr_slot_idx, embedding_slot_idx = Planner.create_add_column_plan(self.path, col)
-        plan.ctx.num_rows = row_count
-        # TODO: create pgvector index, if col is indexed
-
-        try:
-            # TODO: do this in the same transaction as the metadata update
-            with Env.get().engine.begin() as conn:
+            if not col.is_computed or not col.is_stored or row_count == 0:
+                continue
+
+            # populate the column
+            from pixeltable.plan import Planner
+            plan, value_expr_slot_idx = Planner.create_add_column_plan(self.path, col)
+            plan.ctx.num_rows = row_count
+
+            try:
                 plan.ctx.conn = conn
                 plan.open()
-                num_excs = self.store_tbl.load_column(col, plan, value_expr_slot_idx, embedding_slot_idx, conn)
-        except sql.exc.DBAPIError as e:
-            self.drop_column(col.name)
-            raise excs.Error(f'Error during SQL execution:\n{e}')
-        finally:
-            plan.close()
+                num_excs = self.store_tbl.load_column(col, plan, value_expr_slot_idx, conn)
+                if num_excs > 0:
+                    cols_with_excs.append(col)
+            except sql.exc.DBAPIError as e:
+                self.cols.pop()
+                for col in cols:
+                    # remove columns that we already added
+                    if col.id not in self.cols_by_id:
+                        continue
+                    if col.name is not None:
+                        del self.cols_by_name[col.name]
+                    del self.cols_by_id[col.id]
+                # we need to re-initialize the sqlalchemy schema
+                self.store_tbl.create_sa_tbl()
+                raise excs.Error(f'Error during SQL execution:\n{e}')
+            finally:
+                plan.close()
 
-        msg = f'Added {row_count} column value{"" if row_count == 1 else "s"} with {num_excs} error{"" if num_excs == 1 else "s"}.'
-        print(msg)
-        _logger.info(f'Column {col.name}: {msg}')
+        self._update_md(ts, preceding_schema_version, conn)
         if print_stats:
             plan.ctx.profile.print(num_rows=row_count)
+        # TODO(mkornacker): what to do about system columns with exceptions?
         return UpdateStatus(
             num_rows=row_count, num_computed_values=row_count, num_excs=num_excs,
-            cols_with_excs=[f'{self.name}.{col.name}'] if num_excs > 0 else [])
+            cols_with_excs=[f'{col.tbl.name}.{col.name}'for col in cols_with_excs if col.name is not None])
 
     def drop_column(self, name: str) -> None:
         """Drop a column from the table.
         """
         assert not self.is_snapshot
         if name not in self.cols_by_name:
             raise excs.Error(f'Unknown column: {name}')
         col = self.cols_by_name[name]
-        if len(col.dependent_cols) > 0:
+        dependent_user_cols = [c for c in col.dependent_cols if c.name is not None]
+        if len(dependent_user_cols) > 0:
             raise excs.Error(
                 f'Cannot drop column {name} because the following columns depend on it:\n',
-                f'{", ".join([c.name for c in col.dependent_cols])}')
-
-        if col.value_expr is not None:
-            # update Column.dependent_cols
-            for c in self.cols:
-                if c == col:
-                    break
-                c.dependent_cols.discard(col)
+                f'{", ".join([c.name for c in dependent_user_cols])}')
 
         # we're creating a new schema version
-        ts = time.time()
         self.version += 1
         preceding_schema_version = self.schema_version
         self.schema_version = self.version
 
-        self.cols.remove(col)
-        del self.cols_by_name[name]
-        del self.cols_by_id[col.id]
-        self.column_history[col.id].schema_version_drop = self.schema_version
-
         with Env.get().engine.begin() as conn:
-            self._update_md(ts, preceding_schema_version, conn)
-        if col.is_stored:
-            self.store_tbl.drop_column()
+            # drop this column and all dependent index columns and indices
+            dropped_cols = [col]
+            dropped_idx_names: List[str] = []
+            for idx_info in self.idxs_by_name.values():
+                if idx_info.col != col:
+                    continue
+                dropped_cols.extend([idx_info.val_col, idx_info.undo_col])
+                idx_md = self.idx_md[idx_info.id]
+                idx_md.schema_version_drop = self.schema_version
+                assert idx_md.name in self.idxs_by_name
+                dropped_idx_names.append(idx_md.name)
+            # update idxs_by_name
+            for idx_name in dropped_idx_names:
+                del self.idxs_by_name[idx_name]
+            self._drop_columns(dropped_cols, conn, preceding_schema_version)
         _logger.info(f'Dropped column {name} from table {self.name}, new version: {self.version}')
 
+    def _drop_columns(self, cols: list[Column], conn: sql.engine.Connection, preceding_schema_version: int) -> None:
+        """Mark columns as dropped"""
+        assert not self.is_snapshot
+
+        ts = time.time()
+        for col in cols:
+            if col.value_expr is not None:
+                # update Column.dependent_cols
+                for c in self.cols:
+                    if c == col:
+                        break
+                    c.dependent_cols.discard(col)
+
+            col.schema_version_drop = self.schema_version
+            if col.name is not None:
+                assert col.name in self.cols_by_name
+                del self.cols_by_name[col.name]
+            assert col.id in self.cols_by_id
+            del self.cols_by_id[col.id]
+
+        self._update_md(ts, preceding_schema_version, conn)
+        self.store_tbl.create_sa_tbl()
+
     def rename_column(self, old_name: str, new_name: str) -> None:
         """Rename a column.
         """
         assert not self.is_snapshot
         if old_name not in self.cols_by_name:
             raise excs.Error(f'Unknown column: {old_name}')
         if not is_valid_identifier(new_name):
@@ -383,22 +565,22 @@
         with Env.get().engine.begin() as conn:
             self._update_md(ts, preceding_schema_version, conn)
         _logger.info(f'Renamed column {old_name} to {new_name} in table {self.name}, new version: {self.version}')
 
     def set_comment(self, new_comment: Optional[str]):
         _logger.info(f'[{self.name}] Updating comment: {new_comment}')
         self.comment = new_comment
-        self._commit_new_schema_version()
+        self._create_schema_version()
 
     def set_num_retained_versions(self, new_num_retained_versions: int):
         _logger.info(f'[{self.name}] Updating num_retained_versions: {new_num_retained_versions} (was {self.num_retained_versions})')
         self.num_retained_versions = new_num_retained_versions
-        self._commit_new_schema_version()
+        self._create_schema_version()
 
-    def _commit_new_schema_version(self):
+    def _create_schema_version(self):
         # we're creating a new schema version
         ts = time.time()
         self.version += 1
         preceding_schema_version = self.schema_version
         self.schema_version = self.version
         with Env.get().engine.begin() as conn:
             self._update_md(ts, preceding_schema_version, conn)
@@ -444,39 +626,96 @@
         result.cols_with_excs = list(dict.fromkeys(result.cols_with_excs).keys())  # remove duplicates
         if print_stats:
             plan.ctx.profile.print(num_rows=num_rows)
         _logger.info(f'TableVersion {self.name}: new version {self.version}')
         return result
 
     def update(
-            self, update_targets: Optional[List[Tuple[Column, 'pixeltable.exprs.Expr']]] = None,
+            self, update_targets: dict[Column, 'pixeltable.exprs.Expr'],
+            where_clause: Optional['pixeltable.exprs.Predicate'] = None, cascade: bool = True
+    ) -> UpdateStatus:
+        with Env.get().engine.begin() as conn:
+            return self._update(conn, update_targets, where_clause, cascade)
+
+    def batch_update(
+            self, batch: list[dict[Column, 'pixeltable.exprs.Expr']], rowids: list[Tuple[int, ...]],
+            cascade: bool = True
+    ) -> UpdateStatus:
+        """Update rows in batch.
+        Args:
+            batch: one dict per row, each mapping Columns to LiteralExprs representing the new values
+            rowids: if not empty, one tuple per row, each containing the rowid values for the corresponding row in batch
+        """
+        # if we do lookups of rowids, we must have one for each row in the batch
+        assert len(rowids) == 0 or len(rowids) == len(batch)
+        import pixeltable.exprs as exprs
+        result_status = UpdateStatus()
+        cols_with_excs: set[str] = set()
+        updated_cols: set[str] = set()
+        pk_cols = self.primary_key_columns()
+        use_rowids = len(rowids) > 0
+
+        with Env.get().engine.begin() as conn:
+            for i, row in enumerate(batch):
+                where_clause: Optional[exprs.Expr] = None
+                if use_rowids:
+                    # construct Where clause to match rowid
+                    num_rowid_cols = len(self.store_tbl.rowid_columns())
+                    for col_idx in range(num_rowid_cols):
+                        assert len(rowids[i]) == num_rowid_cols
+                        clause = exprs.RowidRef(self, col_idx) == rowids[i][col_idx]
+                        if where_clause is None:
+                            where_clause = clause
+                        else:
+                            where_clause = where_clause & clause
+                else:
+                    # construct Where clause for primary key columns
+                    for col in pk_cols:
+                        assert col in row
+                        clause = exprs.ColumnRef(col) == row[col]
+                        if where_clause is None:
+                            where_clause = clause
+                        else:
+                            where_clause = where_clause & clause
+
+                update_targets = {col: row[col] for col in row if col not in pk_cols}
+                status = self._update(conn, update_targets, where_clause, cascade)
+                result_status.num_rows += status.num_rows
+                result_status.num_excs += status.num_excs
+                result_status.num_computed_values += status.num_computed_values
+                cols_with_excs.update(status.cols_with_excs)
+                updated_cols.update(status.updated_cols)
+
+            result_status.cols_with_excs = list(cols_with_excs)
+            result_status.updated_cols = list(updated_cols)
+            return result_status
+
+    def _update(
+            self, conn: sql.engine.Connection, update_targets: dict[Column, 'pixeltable.exprs.Expr'],
             where_clause: Optional['pixeltable.exprs.Predicate'] = None, cascade: bool = True
     ) -> UpdateStatus:
         """Update rows in this table.
         Args:
             update_targets: a list of (column, value) pairs specifying the columns to update and their new values.
             where_clause: a Predicate to filter rows to update.
             cascade: if True, also update all computed columns that transitively depend on the updated columns,
                 including within views.
         """
-        if update_targets is None:
-            update_targets = []
         assert not self.is_snapshot
         from pixeltable.plan import Planner
         plan, updated_cols, recomputed_cols = \
             Planner.create_update_plan(self.path, update_targets, [], where_clause, cascade)
-        with Env.get().engine.begin() as conn:
-            ts = time.time()
-            result = self._update(
-                plan, where_clause.sql_expr() if where_clause is not None else None, recomputed_cols,
-                base_versions=[], conn=conn, ts=ts, cascade=cascade)
-            result.updated_cols = updated_cols
-            return result
+        ts = time.time()
+        result = self._propagate_update(
+            plan, where_clause.sql_expr() if where_clause is not None else None, recomputed_cols,
+            base_versions=[], conn=conn, ts=ts, cascade=cascade)
+        result.updated_cols = updated_cols
+        return result
 
-    def _update(
+    def _propagate_update(
             self, plan: Optional[exec.ExecNode], where_clause: Optional[sql.ClauseElement],
             recomputed_view_cols: List[Column], base_versions: List[Optional[int]], conn: sql.engine.Connection,
             ts: float, cascade: bool
     ) -> UpdateStatus:
         result = UpdateStatus()
         if plan is not None:
             # we're creating a new version
@@ -493,15 +732,15 @@
             # propagate to views
             for view in self.mutable_views:
                 recomputed_cols = [col for col in recomputed_view_cols if col.tbl is view]
                 plan: Optional[exec.ExecNode] = None
                 if len(recomputed_cols) > 0:
                     from pixeltable.plan import Planner
                     plan = Planner.create_view_update_plan(view.path, recompute_targets=recomputed_cols)
-                status = view._update(
+                status = view._propagate_update(
                     plan, None, recomputed_view_cols, base_versions=base_versions, conn=conn, ts=ts, cascade=True)
                 result.num_rows += status.num_rows
                 result.num_excs += status.num_excs
                 result.cols_with_excs += status.cols_with_excs
 
         result.cols_with_excs = list(dict.fromkeys(result.cols_with_excs).keys())  # remove duplicates
         return result
@@ -550,14 +789,23 @@
         assert not self.is_snapshot
         if self.version == 0:
             raise excs.Error('Cannot revert version 0')
         with orm.Session(Env.get().engine, future=True) as session:
             self._revert(session)
             session.commit()
 
+    def _delete_column(self, col: Column, conn: sql.engine.Connection) -> None:
+        """Physically remove the column from the schema and the store table"""
+        if col.is_stored:
+            self.store_tbl.drop_column(col, conn)
+        self.cols.remove(col)
+        if col.name is not None:
+            del self.cols_by_name[col.name]
+        del self.cols_by_id[col.id]
+
     def _revert(self, session: orm.Session) -> None:
         """Reverts this table version and propagates to views"""
         conn = session.connection()
         # make sure we don't have a snapshot referencing this version
         # (unclear how to express this with sqlalchemy)
         query = (
             f"select ts.dir_id, ts.md->'name' "
@@ -573,54 +821,70 @@
                 f'({", ".join(names)})'
             ))
 
         conn = session.connection()
         # delete newly-added data
         MediaStore.delete(self.id, version=self.version)
         conn.execute(sql.delete(self.store_tbl.sa_tbl).where(self.store_tbl.sa_tbl.c.v_min == self.version))
+
         # revert new deletions
-        conn.execute(
-            sql.update(self.store_tbl.sa_tbl) \
-                .values({self.store_tbl.sa_tbl.c.v_max: schema.Table.MAX_VERSION})
-                .where(self.store_tbl.sa_tbl.c.v_max == self.version))
+        set_clause = {self.store_tbl.sa_tbl.c.v_max: schema.Table.MAX_VERSION}
+        for index_info in self.idxs_by_name.values():
+            # copy the index value back from the undo column and reset the undo column to NULL
+            set_clause[index_info.val_col.sa_col] = index_info.undo_col.sa_col
+            set_clause[index_info.undo_col.sa_col] = None
+        stmt = sql.update(self.store_tbl.sa_tbl) \
+            .values(set_clause) \
+            .where(self.store_tbl.sa_tbl.c.v_max == self.version)
+        conn.execute(stmt)
 
+        # revert schema changes
         if self.version == self.schema_version:
-            # the current version involved a schema change:
-            # if the schema change was to add a column, we now need to drop it
-            added_col_ids = [
-                col_history.col_id for col_history in self.column_history.values()
-                if col_history.schema_version_add == self.schema_version
-            ]
-            assert len(added_col_ids) <= 1
-            added_col: Optional[Column] = None
-            if len(added_col_ids) == 1:
-                added_col_id = added_col_ids[0]
-                # drop this newly-added column and its ColumnHistory record
-                c = self.cols_by_id[added_col_id]
-                if c.is_stored:
-                    added_col = c
-                del self.column_history[c.id]
+            # delete newly-added columns
+            added_cols = [col for col in self.cols if col.schema_version_add == self.schema_version]
+            if len(added_cols) > 0:
+                next_col_id = min(col.id for col in added_cols)
+                for col in added_cols:
+                    self._delete_column(col, conn)
+                self.next_col_id = next_col_id
+
+            # remove newly-added indices from the lookup structures
+            # (the value and undo columns got removed in the preceding step)
+            added_idx_md = [md for md in self.idx_md.values() if md.schema_version_add == self.schema_version]
+            if len(added_idx_md) > 0:
+                next_idx_id = min(md.id for md in added_idx_md)
+                for md in added_idx_md:
+                    del self.idx_md[md.id]
+                    del self.idxs_by_name[md.name]
+                self.next_idx_id = next_idx_id
+
+            # make newly-dropped columns visible again
+            dropped_cols = [col for col in self.cols if col.schema_version_drop == self.schema_version]
+            for col in dropped_cols:
+                col.schema_version_drop = None
+
+            # make newly-dropped indices visible again
+            dropped_idx_md = [md for md in self.idx_md.values() if md.schema_version_drop == self.schema_version]
+            for md in dropped_idx_md:
+                md.schema_version_drop = None
 
             # we need to determine the preceding schema version and reload the schema
             schema_version_md_dict = session.query(schema.TableSchemaVersion.md) \
                 .where(schema.TableSchemaVersion.tbl_id == self.id) \
                 .where(schema.TableSchemaVersion.schema_version == self.schema_version) \
                 .scalar()
             preceding_schema_version = schema_version_md_dict['preceding_schema_version']
             preceding_schema_version_md_dict = session.query(schema.TableSchemaVersion.md) \
                 .where(schema.TableSchemaVersion.tbl_id == self.id) \
                 .where(schema.TableSchemaVersion.schema_version == preceding_schema_version) \
                 .scalar()
             preceding_schema_version_md = schema.md_from_dict(
                 schema.TableSchemaVersionMd, preceding_schema_version_md_dict)
-            self._init_schema(preceding_schema_version_md)
-
-            # physically drop the column, but only after we have re-created the schema
-            if added_col is not None:
-                self.store_tbl.drop_column(added_col, conn)
+            tbl_md = self._create_tbl_md()
+            self._init_schema(tbl_md, preceding_schema_version_md)
 
             conn.execute(
                 sql.delete(schema.TableSchemaVersion.__table__)
                     .where(schema.TableSchemaVersion.tbl_id == self.id)
                     .where(schema.TableSchemaVersion.schema_version == self.schema_version))
             self.schema_version = preceding_schema_version
             self.comment = preceding_schema_version_md.comment
@@ -630,15 +894,15 @@
             sql.delete(schema.TableVersion.__table__)
                 .where(schema.TableVersion.tbl_id == self.id)
                 .where(schema.TableVersion.version == self.version)
         )
         self.version -= 1
         conn.execute(
             sql.update(schema.Table.__table__)
-                .values({schema.Table.md: dataclasses.asdict(self._create_md())})
+                .values({schema.Table.md: dataclasses.asdict(self._create_tbl_md())})
                 .where(schema.Table.id == self.id))
 
         # propagate to views
         for view in self.mutable_views:
             view._revert(session)
         _logger.info(f'TableVersion {self.name}: reverted to version {self.version}')
 
@@ -663,14 +927,18 @@
             return True
         return False
 
     def user_columns(self) -> List[Column]:
         """Return all non-system columns"""
         return [c for c in self.cols if not self.is_system_column(c)]
 
+    def primary_key_columns(self) -> List[Column]:
+        """Return all non-system columns"""
+        return [c for c in self.cols if c.is_pk]
+
     def get_required_col_names(self) -> List[str]:
         """Return the names of all columns for which values must be specified in insert()"""
         assert not self.is_view()
         names = [c.name for c in self.cols if not c.is_computed and not c.col_type.nullable]
         return names
 
     def get_computed_col_names(self) -> List[str]:
@@ -723,27 +991,35 @@
 
     def num_rowid_columns(self) -> int:
         """Return the number of columns of the rowids, without accessing store_tbl"""
         if self.is_component_view():
             return 1 + self.base.num_rowid_columns()
         return 1
 
-    def _create_md(self) -> schema.TableMd:
+    @classmethod
+    def _create_column_md(cls, cols: List[Column]) -> dict[int, schema.ColumnMd]:
+        column_md: Dict[int, schema.ColumnMd] = {}
+        for col in cols:
+            value_expr_dict = col.value_expr.as_dict() if col.value_expr is not None else None
+            column_md[col.id] = schema.ColumnMd(
+                id=col.id, col_type=col.col_type.as_dict(), is_pk=col.is_pk,
+                schema_version_add=col.schema_version_add, schema_version_drop=col.schema_version_drop,
+                value_expr=value_expr_dict, stored=col.stored)
+        return column_md
+
+    def _create_tbl_md(self) -> schema.TableMd:
         return schema.TableMd(
             name=self.name, current_version=self.version, current_schema_version=self.schema_version,
-            next_col_id=self.next_col_id, next_row_id=self.next_rowid, column_history=self.column_history,
-            view_md=self.view_md)
+            next_col_id=self.next_col_id, next_idx_id=self.next_idx_id, next_row_id=self.next_rowid,
+            column_md=self._create_column_md(self.cols), index_md=self.idx_md, view_md=self.view_md)
 
     def _create_version_md(self, ts: float) -> schema.TableVersionMd:
         return schema.TableVersionMd(created_at=ts, version=self.version, schema_version=self.schema_version)
 
     def _create_schema_version_md(self, preceding_schema_version: int) -> schema.TableSchemaVersionMd:
         column_md: Dict[int, schema.SchemaColumn] = {}
-        for pos, col in enumerate(self.cols):
-            value_expr_dict = col.value_expr.as_dict() if col.value_expr is not None else None
-            column_md[col.id] = schema.SchemaColumn(
-                pos=pos, name=col.name, col_type=col.col_type.as_dict(),
-                is_pk=col.primary_key, value_expr=value_expr_dict, stored=col.stored, is_indexed=col.is_indexed)
+        for pos, col in enumerate(self.cols_by_name.values()):
+            column_md[col.id] = schema.SchemaColumn(pos=pos, name=col.name)
         # preceding_schema_version to be set by the caller
         return schema.TableSchemaVersionMd(
             schema_version=self.schema_version, preceding_schema_version=preceding_schema_version,
             columns=column_md, num_retained_versions=self.num_retained_versions, comment=self.comment)
```

### Comparing `pixeltable-0.2.4/pixeltable/catalog/table_version_path.py` & `pixeltable-0.2.5/pixeltable/catalog/table_version_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,16 @@
         if isinstance(index, str):
             # basically <tbl>.<colname>
             return self.__getattr__(index)
         from pixeltable.dataframe import DataFrame
         return DataFrame(self).__getitem__(index)
 
     def columns(self) -> List[Column]:
-        """Return all columns visible in this tbl version path, including columns from bases"""
-        result = self.tbl_version.cols.copy()
+        """Return all user columns visible in this tbl version path, including columns from bases"""
+        result = list(self.tbl_version.cols_by_name.values())
         if self.base is not None:
             base_cols = self.base.columns()
             # we only include base columns that don't conflict with one of our column names
             result.extend([c for c in base_cols if c.name not in self.tbl_version.cols_by_name])
         return result
 
     def get_column(self, name: str, include_bases: bool = True) -> Optional[Column]:
```

### Comparing `pixeltable-0.2.4/pixeltable/catalog/view.py` & `pixeltable-0.2.5/pixeltable/catalog/view.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/client.py` & `pixeltable-0.2.5/pixeltable/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,18 +128,14 @@
         Raises:
             Error: if the path already exists or is invalid.
 
         Examples:
             Create a table with an int and a string column:
 
             >>> table = cl.create_table('my_table', schema={'col1': IntType(), 'col2': StringType()})
-
-            Create a table with a single indexed image column:
-
-            >>> table = cl.create_table('my_table', schema={'col1': {'type': ImageType(), 'indexed': True}})
         """
         path = catalog.Path(path_str)
         self.catalog.paths.check_is_valid(path, expected=None)
         dir = self.catalog.paths[path.parent]
 
         if len(schema) == 0:
             raise excs.Error(f'Table schema is empty: `{path_str}`')
```

### Comparing `pixeltable-0.2.4/pixeltable/dataframe.py` & `pixeltable-0.2.5/pixeltable/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import json
 import logging
 import mimetypes
 import traceback
 from pathlib import Path
 from typing import List, Optional, Any, Dict, Generator, Tuple, Set
 
+import PIL.Image
+import cv2
 import pandas as pd
 import pandas.io.formats.style
 import sqlalchemy as sql
 from PIL import Image
 
 import pixeltable.catalog as catalog
 import pixeltable.exceptions as excs
@@ -27,48 +29,35 @@
 
 __all__ = [
     'DataFrame'
 ]
 
 _logger = logging.getLogger('pixeltable')
 
-def _format_img(img: object) -> str:
-    """
-    Create <img> tag for Image object.
-    """
-    assert isinstance(img, Image.Image), f'Wrong type: {type(img)}'
-    with io.BytesIO() as buffer:
-        img.save(buffer, 'jpeg')
-        img_base64 = base64.b64encode(buffer.getvalue()).decode()
-        return f'<div style="width:200px;"><img src="data:image/jpeg;base64,{img_base64}" width="200" /></div>'
 
 def _create_source_tag(file_path: str) -> str:
     abs_path = Path(file_path)
     assert abs_path.is_absolute()
     src_url = f'{Env.get().http_address}/{abs_path}'
     mime = mimetypes.guess_type(src_url)[0]
     # if mime is None, the attribute string would not be valid html.
     mime_attr = f'type="{mime}"' if mime is not None else ''
     return f'<source src="{src_url}" {mime_attr} />'
 
-def _format_video(file_path: str) -> str:
-    return f'<video controls>{_create_source_tag(file_path)}</video>'
-
-def _format_audio(file_path: str) -> str:
-    return f'<audio controls>{_create_source_tag(file_path)}</audio>'
 
 class DataFrameResultSet:
+
     def __init__(self, rows: List[List[Any]], col_names: List[str], col_types: List[ColumnType]):
         self._rows = rows
         self._col_names = col_names
         self._col_types = col_types
         self._formatters = {
-            ts.ImageType: _format_img,
-            ts.VideoType: _format_video,
-            ts.AudioType: _format_audio,
+            ts.ImageType: self._format_img,
+            ts.VideoType: self._format_video,
+            ts.AudioType: self._format_audio,
         }
 
     def __len__(self) -> int:
         return len(self._rows)
 
     def column_names(self) -> List[str]:
         return self._col_names
@@ -81,31 +70,87 @@
 
     def _repr_html_(self) -> str:
         formatters = {
             col_name: self._formatters[col_type.__class__]
             for col_name, col_type in zip(self._col_names, self._col_types)
             if col_type.__class__ in self._formatters
         }
-
-        # TODO: why does mypy complain about formatters having an incorrect type?
-        return self.to_pandas().to_html(formatters=formatters, escape=False, index=False)  # type: ignore[arg-type]
+        return self.to_pandas().to_html(formatters=formatters, escape=False, index=False)
 
     def __str__(self) -> str:
         return self.to_pandas().to_string()
 
     def _reverse(self) -> None:
         """Reverse order of rows"""
         self._rows.reverse()
 
     def to_pandas(self) -> pd.DataFrame:
         return pd.DataFrame.from_records(self._rows, columns=self._col_names)
 
     def _row_to_dict(self, row_idx: int) -> Dict[str, Any]:
         return {self._col_names[i]: self._rows[row_idx][i] for i in range(len(self._col_names))}
 
+    # Formatters
+
+    def _format_img(self, img: Image.Image) -> str:
+        """
+        Create <img> tag for Image object.
+        """
+        assert isinstance(img, Image.Image), f'Wrong type: {type(img)}'
+        # Try to make it look decent in a variety of display scenarios
+        if len(self._rows) > 1:
+            width = 240  # Multiple rows: display small images
+        elif len(self._col_names) > 1:
+            width = 480  # Multiple columns: display medium images
+        else:
+            width = 640  # A single image: larger display
+        with io.BytesIO() as buffer:
+            img.save(buffer, 'jpeg')
+            img_base64 = base64.b64encode(buffer.getvalue()).decode()
+            return f'''
+            <div style="width:{width}px;">
+                <img src="data:image/jpeg;base64,{img_base64}" width="{width}" />
+            </div>
+            '''
+
+    def _format_video(self, file_path: str) -> str:
+        thumb_tag = ""
+        # Attempt to extract the first frame of the video to use as a thumbnail,
+        # so that the notebook can be exported as HTML and viewed in contexts where
+        # the video itself is not accessible.
+        # TODO(aaron-siegel): If the video is backed by a concrete external URL,
+        # should we link to that instead?
+        video_reader = cv2.VideoCapture(str(file_path))
+        if video_reader.isOpened():
+            status, img_array = video_reader.read()
+            if status:
+                img_array = cv2.cvtColor(img_array, cv2.COLOR_BGR2RGB)
+                thumb = PIL.Image.fromarray(img_array)
+                with io.BytesIO() as buffer:
+                    thumb.save(buffer, 'jpeg')
+                    thumb_base64 = base64.b64encode(buffer.getvalue()).decode()
+                    thumb_tag = f'poster="data:image/jpeg;base64,{thumb_base64}"'
+            video_reader.release()
+        if len(self._rows) > 1:
+            width = 320
+        elif len(self._col_names) > 1:
+            width = 480
+        else:
+            width = 800
+        return f'''
+        <div style="width:{width}px;">
+            <video controls width="{width}" {thumb_tag}>
+                {_create_source_tag(file_path)}
+            </video>
+        </div>
+        '''
+
+    def _format_audio(self, file_path: str) -> str:
+        return f'<audio controls>{_create_source_tag(file_path)}</audio>'
+
     def __getitem__(self, index: Any) -> Any:
         if isinstance(index, str):
             if index not in self._col_names:
                 raise excs.Error(f'Invalid column name: {index}')
             col_idx = self._col_names.index(index)
             return [row[col_idx] for row in self._rows]
         if isinstance(index, int):
@@ -169,15 +214,14 @@
         """
         exprs.Expr.release_list(self.sql_scan_output_exprs)
         exprs.Expr.release_list(self.agg_output_exprs)
         if self.filter is not None:
             self.filter.release()
 
 
-
 class DataFrame:
     def __init__(
             self, tbl: catalog.TableVersionPath,
             select_list: Optional[List[Tuple[exprs.Expr, Optional[str]]]] = None,
             where_clause: Optional[exprs.Predicate] = None,
             group_by_clause: Optional[List[exprs.Expr]] = None,
             grouping_tbl: Optional[catalog.TableVersion] = None,
```

### Comparing `pixeltable-0.2.4/pixeltable/env.py` & `pixeltable-0.2.5/pixeltable/env.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 import importlib
 import importlib.util
 import logging
 import os
 import socketserver
 import sys
 import threading
-import typing
 import uuid
+import warnings
 from pathlib import Path
 from typing import Callable, Optional, Dict, Any, List
 
 import pgserver
 import sqlalchemy as sql
 import yaml
 from sqlalchemy_utils.functions import database_exists, create_database, drop_database
+from tqdm import TqdmWarning
 
 import pixeltable.exceptions as excs
 from pixeltable import metadata
 
 
 class Env:
     """
@@ -184,19 +185,29 @@
             self._tmp_dir.mkdir()
 
         # configure _logger to log to a file
         self._logfilename = datetime.datetime.now().strftime('%Y%m%d_%H%M%S') + '.log'
         fh = logging.FileHandler(self._log_dir / self._logfilename, mode='w')
         fh.setFormatter(logging.Formatter(self._log_fmt_str))
         self._logger.addHandler(fh)
+
+        # configure sqlalchemy logging
         sql_logger = logging.getLogger('sqlalchemy.engine')
         sql_logger.setLevel(logging.INFO)
         sql_logger.addHandler(fh)
         sql_logger.propagate = False
 
+        # configure pyav logging
+        av_logfilename = self._logfilename.replace('.log', '_av.log')
+        av_fh = logging.FileHandler(self._log_dir / av_logfilename, mode='w')
+        av_fh.setFormatter(logging.Formatter(self._log_fmt_str))
+        av_logger = logging.getLogger('libav')
+        av_logger.addHandler(av_fh)
+        av_logger.propagate = False
+
         # empty tmp dir
         for path in glob.glob(f'{self._tmp_dir}/*'):
             os.remove(path)
 
         self._db_name = os.environ.get('PIXELTABLE_DB', 'pixeltable')
         self._pgdata_dir = Path(os.environ.get('PIXELTABLE_PGDATA', str(self._home / 'pgdata')))
 
@@ -225,14 +236,17 @@
 
         print(f'Connected to Pixeltable database at: {self.db_url}')
 
         # we now have a home directory and db; start other services
         self._set_up_runtime()
         self.log_to_stdout(False)
 
+        # Disable spurious warnings
+        warnings.simplefilter("ignore", category=TqdmWarning)
+
     def upgrade_metadata(self) -> None:
         metadata.upgrade_md(self._sa_engine)
 
     def _create_nos_client(self) -> None:
         import nos
         self._logger.info('connecting to NOS')
         nos.init(logging_level=logging.DEBUG)
@@ -316,14 +330,15 @@
                 self._installed_packages[package] = None
 
         check('datasets')
         check('torch')
         check('torchvision')
         check('transformers')
         check('sentence_transformers')
+        check('yolox')
         check('boto3')
         check('pyarrow')
         check('spacy')  # TODO: deal with en-core-web-sm
         if self.is_installed_package('spacy'):
             import spacy
             self._spacy_nlp = spacy.load('en_core_web_sm')
         check('tiktoken')
```

### Comparing `pixeltable-0.2.4/pixeltable/exec/aggregation_node.py` & `pixeltable-0.2.5/pixeltable/exec/aggregation_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exec/cache_prefetch_node.py` & `pixeltable-0.2.5/pixeltable/exec/cache_prefetch_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         parsed = urllib.parse.urlparse(url)
         # Use len(parsed.scheme) > 1 here to ensure we're not being passed
         # a Windows filename
         assert len(parsed.scheme) > 1 and parsed.scheme != 'file'
         # preserve the file extension, if there is one
         extension = ''
         if parsed.path != '':
-            p = Path(urllib.parse.unquote(parsed.path))
+            p = Path(urllib.parse.unquote(urllib.request.url2pathname(parsed.path)))
             extension = p.suffix
         tmp_path = env.Env.get().create_tmp_path(extension=extension)
         try:
             if parsed.scheme == 's3':
                 from pixeltable.utils.s3 import get_client
                 with self.boto_client_lock:
                     if self.boto_client is None:
```

### Comparing `pixeltable-0.2.4/pixeltable/exec/component_iteration_node.py` & `pixeltable-0.2.5/pixeltable/exec/component_iteration_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exec/data_row_batch.py` & `pixeltable-0.2.5/pixeltable/exec/data_row_batch.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exec/exec_context.py` & `pixeltable-0.2.5/pixeltable/exec/exec_context.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exec/exec_node.py` & `pixeltable-0.2.5/pixeltable/exec/exec_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exec/expr_eval_node.py` & `pixeltable-0.2.5/pixeltable/exec/expr_eval_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exec/in_memory_data_node.py` & `pixeltable-0.2.5/pixeltable/exec/in_memory_data_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,39 +25,43 @@
         self.input_rows = rows
         self.start_row_id = start_row_id
         self.has_returned_data = False
         self.output_rows: Optional[DataRowBatch] = None
 
     def _open(self) -> None:
         """Create row batch and populate with self.input_rows"""
-        column_info = {info.col.name: info for info in self.row_builder.output_slot_idxs()}
+        column_info = {info.col.id: info for info in self.row_builder.output_slot_idxs()}
+        # exclude system columns
+        user_column_info = {info.col.name: info for _, info in column_info.items() if info.col.name is not None}
         # stored columns that are not computed
-        inserted_column_names = set([
-            info.col.name for info in self.row_builder.output_slot_idxs()
+        inserted_col_ids = set([
+            info.col.id for info in self.row_builder.output_slot_idxs()
             if info.col.is_stored and not info.col.is_computed
         ])
 
         self.output_rows = DataRowBatch(self.tbl, self.row_builder, len(self.input_rows))
         for row_idx, input_row in enumerate(self.input_rows):
             # populate the output row with the values provided in the input row
+            input_col_ids: List[int] = []
             for col_name, val in input_row.items():
-                col_info = column_info.get(col_name)
+                col_info = user_column_info.get(col_name)
                 assert col_info is not None
 
                 if col_info.col.col_type.is_image_type() and isinstance(val, bytes):
                     # this is a literal image, ie, a sequence of bytes; we save this as a media file and store the path
                     path = str(MediaStore.prepare_media_path(self.tbl.id, col_info.col.id, self.tbl.version))
                     open(path, 'wb').write(val)
                     val = path
                 self.output_rows[row_idx][col_info.slot_idx] = val
+                input_col_ids.append(col_info.col.id)
 
             # set the remaining stored non-computed columns to null
-            null_col_names = inserted_column_names - set(input_row.keys())
-            for col_name in null_col_names:
-                col_info = column_info.get(col_name)
+            null_col_ids = inserted_col_ids - set(input_col_ids)
+            for col_id in null_col_ids:
+                col_info = column_info.get(col_id)
                 assert col_info is not None
                 self.output_rows[row_idx][col_info.slot_idx] = None
 
         self.output_rows.set_row_ids([self.start_row_id + i for i in range(len(self.output_rows))])
         self.ctx.num_rows = len(self.output_rows)
 
     def __next__(self) -> DataRowBatch:
```

### Comparing `pixeltable-0.2.4/pixeltable/exec/media_validation_node.py` & `pixeltable-0.2.5/pixeltable/exec/media_validation_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exec/sql_scan_node.py` & `pixeltable-0.2.5/pixeltable/exec/sql_scan_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/__init__.py` & `pixeltable-0.2.5/pixeltable/exprs/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/arithmetic_expr.py` & `pixeltable-0.2.5/pixeltable/exprs/arithmetic_expr.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/array_slice.py` & `pixeltable-0.2.5/pixeltable/exprs/array_slice.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/column_property_ref.py` & `pixeltable-0.2.5/pixeltable/exprs/column_property_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/column_ref.py` & `pixeltable-0.2.5/pixeltable/exprs/column_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/comparison.py` & `pixeltable-0.2.5/pixeltable/exprs/comparison.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
+
 from typing import Optional, List, Any, Dict, Tuple
 
 import sqlalchemy as sql
 
-from .globals import ComparisonOperator
+from .data_row import DataRow
 from .expr import Expr
+from .globals import ComparisonOperator
 from .predicate import Predicate
-from .data_row import DataRow
 from .row_builder import RowBuilder
-import pixeltable.catalog as catalog
 
 
 class Comparison(Predicate):
     def __init__(self, operator: ComparisonOperator, op1: Expr, op2: Expr):
         super().__init__()
         self.operator = operator
         self.components = [op1, op2]
```

### Comparing `pixeltable-0.2.4/pixeltable/exprs/compound_predicate.py` & `pixeltable-0.2.5/pixeltable/exprs/compound_predicate.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/data_row.py` & `pixeltable-0.2.5/pixeltable/exprs/data_row.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import io
 import urllib.parse
 import urllib.request
 from typing import Optional, List, Any, Tuple
 
+import sqlalchemy as sql
+import pgvector.sqlalchemy
 import PIL
 import numpy as np
 
 
 class DataRow:
     """
     Encapsulates all data and execution state needed by RowBuilder and DataRowBatch:
@@ -106,29 +108,31 @@
             assert self.file_paths[index] is not None
             if self.vals[index] is None:
                 self.vals[index] = PIL.Image.open(self.file_paths[index])
                 self.vals[index].load()
 
         return self.vals[index]
 
-    def get_stored_val(self, index: object) -> Any:
+    def get_stored_val(self, index: object, sa_col_type: Optional[sql.types.TypeEngine] = None) -> Any:
         """Return the value that gets stored in the db"""
         assert self.excs[index] is None
         if not self.has_val[index]:
             # for debugging purposes
             pass
         assert self.has_val[index]
 
         if self.file_urls[index] is not None and (index in self.img_slot_idxs or index in self.media_slot_idxs):
             # if this is an image or other media type we want to store, we should have a url
             return self.file_urls[index]
 
         if self.vals[index] is not None and index in self.array_slot_idxs:
             assert isinstance(self.vals[index], np.ndarray)
             np_array = self.vals[index]
+            if sa_col_type is not None and isinstance(sa_col_type, pgvector.sqlalchemy.Vector):
+                return np_array
             buffer = io.BytesIO()
             np.save(buffer, np_array)
             return buffer.getvalue()
 
         return self.vals[index]
 
     def __setitem__(self, idx: object, val: Any) -> None:
```

### Comparing `pixeltable-0.2.4/pixeltable/exprs/expr.py` & `pixeltable-0.2.5/pixeltable/exprs/expr.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/expr_set.py` & `pixeltable-0.2.5/pixeltable/exprs/expr_set.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/function_call.py` & `pixeltable-0.2.5/pixeltable/exprs/function_call.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/globals.py` & `pixeltable-0.2.5/pixeltable/exprs/globals.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/image_member_access.py` & `pixeltable-0.2.5/pixeltable/exprs/image_member_access.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/image_similarity_predicate.py` & `pixeltable-0.2.5/pixeltable/exprs/image_similarity_predicate.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/inline_array.py` & `pixeltable-0.2.5/pixeltable/exprs/inline_array.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/inline_dict.py` & `pixeltable-0.2.5/pixeltable/exprs/inline_dict.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/is_null.py` & `pixeltable-0.2.5/pixeltable/exprs/is_null.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/json_mapper.py` & `pixeltable-0.2.5/pixeltable/exprs/json_mapper.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/json_path.py` & `pixeltable-0.2.5/pixeltable/exprs/json_path.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/literal.py` & `pixeltable-0.2.5/pixeltable/exprs/literal.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
+
+import datetime
 from typing import Optional, List, Any, Dict, Tuple
 
 import sqlalchemy as sql
 
-from .expr import Expr
+import pixeltable.exceptions as excs
+import pixeltable.type_system as ts
 from .data_row import DataRow
+from .expr import Expr
 from .row_builder import RowBuilder
-import pixeltable.catalog as catalog
-import pixeltable.type_system as ts
+
 
 class Literal(Expr):
     def __init__(self, val: Any, col_type: Optional[ts.ColumnType] = None):
         if col_type is not None:
             val = col_type.create_literal(val)
         else:
             # try to determine a type for val
@@ -42,13 +45,22 @@
         return sql.sql.expression.literal(self.val)
 
     def eval(self, data_row: DataRow, row_builder: RowBuilder) -> None:
         # this will be called, even though sql_expr() does not return None
         data_row[self.slot_idx] = self.val
 
     def _as_dict(self) -> Dict:
-        return {'val': self.val, **super()._as_dict()}
+        # For some types, we need to explictly record their type, because JSON does not know
+        # how to interpret them unambiguously
+        if self.col_type.is_timestamp_type():
+            return {'val': self.val.isoformat(), 'val_t': self.col_type._type.name, **super()._as_dict()}
+        else:
+            return {'val': self.val, **super()._as_dict()}
 
     @classmethod
     def _from_dict(cls, d: Dict, components: List[Expr]) -> Expr:
         assert 'val' in d
+        if 'val_t' in d:
+            val_t = d['val_t']
+            assert val_t == ts.ColumnType.Type.TIMESTAMP.name
+            return cls(datetime.datetime.fromisoformat(d['val']))
         return cls(d['val'])
```

### Comparing `pixeltable-0.2.4/pixeltable/exprs/object_ref.py` & `pixeltable-0.2.5/pixeltable/exprs/object_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/predicate.py` & `pixeltable-0.2.5/pixeltable/exprs/predicate.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/row_builder.py` & `pixeltable-0.2.5/pixeltable/exprs/row_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,34 +50,31 @@
         """Context for evaluating a set of target exprs"""
         slot_idxs: List[int]  # slot idxs of exprs needed to evaluate target exprs; does not contain duplicates
         exprs: List[Expr]  # exprs corresponding to slot_idxs
         target_slot_idxs: List[int]  # slot idxs of target exprs; might contain duplicates
         target_exprs: List[Expr]  # exprs corresponding to target_slot_idxs
 
     def __init__(
-            self, output_exprs: List[Expr], columns: List[catalog.Column],
-            indices: List[Tuple[catalog.Column, func.Function]], input_exprs: List[Expr]
+            self, output_exprs: List[Expr], columns: List[catalog.Column], input_exprs: List[Expr]
     ):
         """
         Args:
             output_exprs: list of Exprs to be evaluated
             columns: list of columns to be materialized
-            indices: list of embeddings to be materialized (Tuple[indexed column, embedding function])
         """
         self.unique_exprs = ExprSet()  # dependencies precede their dependents
         self.next_slot_idx = 0
 
         # record input and output exprs; make copies to avoid reusing execution state
         unique_input_exprs = [self._record_unique_expr(e.copy(), recursive=False) for e in input_exprs]
         self.input_expr_slot_idxs = {e.slot_idx for e in unique_input_exprs}
 
         # output exprs: all exprs the caller wants to materialize
         # - explicitly requested output_exprs
         # - values for computed columns
-        # - embedding values for indices
         resolve_cols = set(columns)
         self.output_exprs = [
             self._record_unique_expr(e.copy().resolve_computed_cols(resolve_cols=resolve_cols), recursive=True)
             for e in output_exprs
         ]
 
         # record columns for create_table_row()
@@ -93,29 +90,14 @@
                 self.output_exprs.append(expr)
             else:
                 # record a ColumnRef so that references to this column resolve to the same slot idx
                 ref = ColumnRef(col)
                 ref = self._record_unique_expr(ref, recursive=False)
                 self.add_table_column(col, ref.slot_idx)
 
-        # record indices; indexed by slot_idx
-        self.index_columns: List[catalog.Column] = []
-        for col, embedding_fn in indices:
-            # we assume that the parameter of the embedding function is a ref to an image column
-            assert col.col_type.is_image_type()
-            # construct expr to compute embedding; explicitly resize images to the required size
-            target_img_type = next(iter(embedding_fn.signature.parameters.values())).col_type
-            expr = embedding_fn(ColumnRef(col).resize(target_img_type.size))
-            expr = self._record_unique_expr(expr, recursive=True)
-            self.output_exprs.append(expr)
-            if len(self.index_columns) <= expr.slot_idx:
-                # pad to slot_idx
-                self.index_columns.extend([None] * (expr.slot_idx - len(self.index_columns) + 1))
-            self.index_columns[expr.slot_idx] = col
-
         # default eval ctx: all output exprs
         self.default_eval_ctx = self.create_eval_ctx(self.output_exprs, exclude=unique_input_exprs)
 
         # references to unstored iterator columns:
         # - those ColumnRefs need to instantiate iterators
         # - we create and record the iterator args here and pass them to their respective ColumnRefs
         # - we do this instead of simply recording the iterator args as a component of those ColumnRefs,
@@ -166,21 +148,14 @@
         """Record a column that is part of the table row"""
         self.table_columns.append(ColumnSlotIdx(col, slot_idx))
 
     def output_slot_idxs(self) -> List[ColumnSlotIdx]:
         """Return ColumnSlotIdx for output columns"""
         return self.table_columns
 
-    def index_slot_idxs(self) -> List[ColumnSlotIdx]:
-        """Return ColumnSlotIdx for index columns"""
-        return [
-            ColumnSlotIdx(self.output_columns[i], i) for i in range(len(self.index_columns))
-            if self.output_columns[i] is not None
-        ]
-
     @property
     def num_materialized(self) -> int:
         return self.next_slot_idx
 
     def get_output_exprs(self) -> List[Expr]:
         """Returns exprs that were requested in the c'tor and require evaluation"""
         return self.output_exprs
@@ -330,26 +305,19 @@
         for info in self.table_columns:
             col, slot_idx = info.col, info.slot_idx
             if data_row.has_exc(slot_idx):
                 # exceptions get stored in the errortype/-msg columns
                 exc = data_row.get_exc(slot_idx)
                 num_excs += 1
                 exc_col_ids.add(col.id)
-                table_row[col.storage_name()] = None
-                table_row[col.errortype_storage_name()] = type(exc).__name__
-                table_row[col.errormsg_storage_name()] = str(exc)
+                table_row[col.store_name()] = None
+                table_row[col.errortype_store_name()] = type(exc).__name__
+                table_row[col.errormsg_store_name()] = str(exc)
             else:
-                val = data_row.get_stored_val(slot_idx)
-                table_row[col.storage_name()] = val
+                val = data_row.get_stored_val(slot_idx, col.sa_col.type)
+                table_row[col.store_name()] = val
                 # we unfortunately need to set these, even if there are no errors
-                table_row[col.errortype_storage_name()] = None
-                table_row[col.errormsg_storage_name()] = None
-
-        for slot_idx, col in enumerate(self.index_columns):
-            if col is None:
-                continue
-            # don't use get_stored_val() here, we need to pass in the ndarray
-            val = data_row[slot_idx]
-            table_row[col.index_storage_name()] = val
+                table_row[col.errortype_store_name()] = None
+                table_row[col.errormsg_store_name()] = None
 
         return table_row, num_excs
```

### Comparing `pixeltable-0.2.4/pixeltable/exprs/rowid_ref.py` & `pixeltable-0.2.5/pixeltable/exprs/rowid_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/type_cast.py` & `pixeltable-0.2.5/pixeltable/exprs/type_cast.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/exprs/variable.py` & `pixeltable-0.2.5/pixeltable/exprs/variable.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/func/aggregate_function.py` & `pixeltable-0.2.5/pixeltable/func/aggregate_function.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 import abc
 import importlib
 import inspect
-from typing import Optional, Any, Type, List, Dict
+from typing import Optional, Any, Type, List, Dict, Callable
 import itertools
 
 import pixeltable.exceptions as excs
 import pixeltable.type_system as ts
 from .function import Function
 from .signature import Signature, Parameter
+from .globals import validate_symbol_path
 
 
 class Aggregator(abc.ABC):
     def update(self, *args: Any, **kwargs: Any) -> None:
         pass
     def value(self) -> Any:
         pass
@@ -132,16 +133,15 @@
 
 def uda(
         *,
         value_type: ts.ColumnType,
         update_types: List[ts.ColumnType],
         init_types: Optional[List[ts.ColumnType]] = None,
         requires_order_by: bool = False, allows_std_agg: bool = True, allows_window: bool = False,
-        name: Optional[str] = None
-) -> Type[Aggregator]:
+) -> Callable:
     """Decorator for user-defined aggregate functions.
 
     The decorated class must inherit from Aggregator and implement the following methods:
     - __init__(self, ...) to initialize the aggregator
     - update(self, ...) to update the aggregator with a new value
     - value(self) to return the final result
 
@@ -151,22 +151,19 @@
     Parameters:
     - init_types: list of types for the __init__() parameters; must match the number of parameters
     - update_types: list of types for the update() parameters; must match the number of parameters
     - value_type: return type of the aggregator
     - requires_order_by: if True, the first parameter to the function is the order-by expression
     - allows_std_agg: if True, the function can be used as a standard aggregate function w/o a window
     - allows_window: if True, the function can be used with a window
-    - name: name of the AggregateFunction instance; if None, the class name is used
     """
-    if name is not None and not name.isidentifier():
-        raise excs.Error(f'Invalid name: {name}')
     if init_types is None:
         init_types = []
 
-    def decorator(cls: Type[Aggregator]) -> Type[Aggregator]:
+    def decorator(cls: Type[Aggregator]) -> Type[Function]:
         # validate type parameters
         num_init_params = len(inspect.signature(cls.__init__).parameters) - 1
         if num_init_params > 0:
             if len(init_types) != num_init_params:
                 raise excs.Error(
                     f'init_types must be a list of {num_init_params} types, one for each parameter of __init__()')
         num_update_params = len(inspect.signature(cls.update).parameters) - 1
@@ -174,21 +171,24 @@
             raise excs.Error('update() must have at least one parameter')
         if len(update_types) != num_update_params:
             raise excs.Error(
                 f'update_types must be a list of {num_update_params} types, one for each parameter of update()')
         assert value_type is not None
 
         # the AggregateFunction instance resides in the same module as cls
-        module_path = cls.__module__
-        nonlocal name
-        name = name or cls.__name__
-        instance_path = f'{module_path}.{name}'
+        class_path = f'{cls.__module__}.{cls.__qualname__}'
+        # nonlocal name
+        # name = name or cls.__name__
+        # instance_path_elements = class_path.split('.')[:-1] + [name]
+        # instance_path = '.'.join(instance_path_elements)
 
         # create the corresponding AggregateFunction instance
         instance = AggregateFunction(
-            cls, instance_path, init_types, update_types, value_type, requires_order_by, allows_std_agg, allows_window)
-        module = importlib.import_module(module_path)
-        setattr(module, name, instance)
+            cls, class_path, init_types, update_types, value_type, requires_order_by, allows_std_agg, allows_window)
+        # do the path validation at the very end, in order to be able to write tests for the other failure cases
+        validate_symbol_path(class_path)
+        #module = importlib.import_module(cls.__module__)
+        #setattr(module, name, instance)
 
-        return cls
+        return instance
 
     return decorator
```

### Comparing `pixeltable-0.2.4/pixeltable/func/batched_function.py` & `pixeltable-0.2.5/pixeltable/func/batched_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/func/callable_function.py` & `pixeltable-0.2.5/pixeltable/func/callable_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/func/expr_template_function.py` & `pixeltable-0.2.5/pixeltable/func/expr_template_function.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,17 +46,25 @@
 
     def instantiate(self, *args: object, **kwargs: object) -> 'pixeltable.exprs.Expr':
         bound_args = self.py_signature.bind(*args, **kwargs).arguments
         # apply defaults, otherwise we might have Parameters left over
         bound_args.update(
             {param_name: default for param_name, default in self.defaults.items() if param_name not in bound_args})
         result = self.expr.copy()
+        import pixeltable.exprs as exprs
         for param_name, arg in bound_args.items():
             param_expr = self.param_exprs_by_name[param_name]
-            result = result.substitute(param_expr, arg)
+            if not isinstance(arg, exprs.Expr):
+                # TODO: use the available param_expr.col_type
+                arg_expr = exprs.Expr.from_object(arg)
+                if arg_expr is None:
+                    raise excs.Error(f'{self.self_name}(): cannot convert argument {arg} to a Pixeltable expression')
+            else:
+                arg_expr = arg
+            result = result.substitute(param_expr, arg_expr)
         import pixeltable.exprs as exprs
         assert not result.contains(exprs.Variable)
         return result
 
     @property
     def display_name(self) -> str:
         return self.self_name
```

### Comparing `pixeltable-0.2.4/pixeltable/func/function.py` & `pixeltable-0.2.5/pixeltable/func/function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/func/function_registry.py` & `pixeltable-0.2.5/pixeltable/func/function_registry.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/func/globals.py` & `pixeltable-0.2.5/pixeltable/func/globals.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,43 @@
-from typing import Optional
-from types import ModuleType
 import importlib
 import inspect
+from types import ModuleType
+from typing import Optional
 
+import pixeltable.exceptions as excs
 
-def resolve_symbol(symbol_path: str) -> object:
+
+def resolve_symbol(symbol_path: str) -> Optional[object]:
     path_elems = symbol_path.split('.')
     module: Optional[ModuleType] = None
-    if path_elems[0:2] == ['pixeltable', 'functions'] and len(path_elems) > 2:
-        # if this is a pixeltable.functions submodule, it cannot be resolved via pixeltable.functions;
-        # try to import the submodule directly
-        submodule_path = '.'.join(path_elems[0:3])
+    i = len(path_elems) - 1
+    while i > 0 and module is None:
         try:
-            module = importlib.import_module(submodule_path)
-            path_elems = path_elems[3:]
+            module = importlib.import_module('.'.join(path_elems[:i]))
         except ModuleNotFoundError:
-            pass
-    if module is None:
-        module = importlib.import_module(path_elems[0])
-        path_elems = path_elems[1:]
+            i -= 1
+    if i == 0:
+        return None  # Not resolvable
     obj = module
-    for el in path_elems:
+    for el in path_elems[i:]:
         obj = getattr(obj, el)
     return obj
 
+
+def validate_symbol_path(fn_path: str) -> None:
+    path_elems = fn_path.split('.')
+    fn_name = path_elems[-1]
+    if any(el == '<locals>' for el in path_elems):
+        raise excs.Error(
+            f'{fn_name}(): nested functions are not supported. Move the function to the module level or into a class.')
+    if any(not el.isidentifier() for el in path_elems):
+        raise excs.Error(
+            f'{fn_name}(): cannot resolve symbol path {fn_path}. Move the function to the module level or into a class.')
+
+
 def get_caller_module_path() -> str:
     """Return the module path of our caller's caller"""
     stack = inspect.stack()
     try:
         caller_frame = stack[2].frame
         module_path = caller_frame.f_globals['__name__']
     finally:
```

### Comparing `pixeltable-0.2.4/pixeltable/func/nos_function.py` & `pixeltable-0.2.5/pixeltable/func/nos_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/func/signature.py` & `pixeltable-0.2.5/pixeltable/func/signature.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,35 +110,28 @@
                 py_type = typing.get_args(type_args[0])[0]
         if py_type is None:
             py_type = annotation
         col_type = ts.ColumnType.from_python_type(py_type)
         return (col_type, is_batched)
 
     @classmethod
-    def create(
-            cls, c: Callable,
-            param_types: Optional[List[ts.ColumnType]] = None,
-            return_type: Optional[Union[ts.ColumnType, Callable]] = None
-    ) -> Signature:
-        """Create a signature for the given Callable.
-        Infer the parameter and return types, if none are specified.
-        Raises an exception if the types cannot be inferred.
-        """
+    def create_parameters(
+            cls, c: Callable, param_types: Optional[List[ts.ColumnType]] = None) -> List[Parameter]:
         sig = inspect.signature(c)
         py_parameters = list(sig.parameters.values())
-
-        # check non-var parameters for name collisions and default value compatibility
         parameters: List[Parameter] = []
+
         for idx, param in enumerate(py_parameters):
             if param.name in cls.SPECIAL_PARAM_NAMES:
                 raise excs.Error(f"'{param.name}' is a reserved parameter name")
             if param.kind == inspect.Parameter.VAR_POSITIONAL or param.kind == inspect.Parameter.VAR_KEYWORD:
                 parameters.append(Parameter(param.name, None, param.kind, False))
                 continue
 
+            # check non-var parameters for name collisions and default value compatibility
             if param_types is not None:
                 if idx >= len(param_types):
                     raise excs.Error(f'Missing type for parameter {param.name}')
                 param_type = param_types[idx]
                 is_batched = False
             else:
                 param_type, is_batched = cls._infer_type(param.annotation)
@@ -151,15 +144,28 @@
                 try:
                     _ = param_type.create_literal(default_val)
                 except TypeError as e:
                     raise excs.Error(f'Default value for parameter {param.name}: {str(e)}')
 
             parameters.append(Parameter(param.name, param_type, param.kind, is_batched))
 
-        return_is_batched = False
+        return parameters
+
+    @classmethod
+    def create(
+            cls, c: Callable,
+            param_types: Optional[List[ts.ColumnType]] = None,
+            return_type: Optional[Union[ts.ColumnType, Callable]] = None
+    ) -> Signature:
+        """Create a signature for the given Callable.
+        Infer the parameter and return types, if none are specified.
+        Raises an exception if the types cannot be inferred.
+        """
+        parameters = cls.create_parameters(c, param_types)
+        sig = inspect.signature(c)
         if return_type is None:
             return_type, return_is_batched = cls._infer_type(sig.return_annotation)
             if return_type is None:
                 raise excs.Error('Cannot infer pixeltable return type')
         else:
             _, return_is_batched = cls._infer_type(sig.return_annotation)
```

### Comparing `pixeltable-0.2.4/pixeltable/func/udf.py` & `pixeltable-0.2.5/pixeltable/func/udf.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import pixeltable.exceptions as excs
 import pixeltable.type_system as ts
 from .batched_function import ExplicitBatchedFunction
 from .callable_function import CallableFunction
 from .expr_template_function import ExprTemplateFunction
 from .function import Function
 from .function_registry import FunctionRegistry
+from .globals import validate_symbol_path
 from .signature import Signature
 
 
 # Decorator invoked without parentheses: @pxt.udf
 @overload
 def udf(decorated_fn: Callable) -> Function: ...
 
@@ -120,14 +121,16 @@
         result = CallableFunction(signature=sig, py_fn=py_fn, self_path=function_path, self_name=function_name)
     else:
         result = ExplicitBatchedFunction(
             signature=sig, batch_size=batch_size, invoker_fn=py_fn, self_path=function_path)
 
     # If this function is part of a module, register it
     if function_path is not None:
+        # do the validation at the very end, so it's easier to write tests for other failure scenarios
+        validate_symbol_path(function_path)
         FunctionRegistry.get().register_function(function_path, result)
 
     return result
 
 @overload
 def expr_udf(py_fn: Callable) -> ExprTemplateFunction: ...
 
@@ -138,25 +141,27 @@
     def decorator(py_fn: Callable, param_types: Optional[List[ts.ColumnType]]) -> ExprTemplateFunction:
         if py_fn.__module__ != '__main__' and py_fn.__name__.isidentifier():
             # this is a named function in a module
             function_path = f'{py_fn.__module__}.{py_fn.__qualname__}'
         else:
             function_path = None
 
-        sig = Signature.create(py_fn, param_types=param_types, return_type=None)
         # TODO: verify that the inferred return type matches that of the template
         # TODO: verify that the signature doesn't contain batched parameters
 
         # construct Parameters from the function signature
+        params = Signature.create_parameters(py_fn, param_types=param_types)
         import pixeltable.exprs as exprs
-        var_exprs = [exprs.Variable(param.name, param.col_type) for param in sig.parameters.values()]
+        var_exprs = [exprs.Variable(param.name, param.col_type) for param in params]
         # call the function with the parameter expressions to construct an Expr with parameters
         template = py_fn(*var_exprs)
         assert isinstance(template, exprs.Expr)
         py_sig = inspect.signature(py_fn)
+        if function_path is not None:
+            validate_symbol_path(function_path)
         return ExprTemplateFunction(template, py_signature=py_sig, self_path=function_path, name=py_fn.__name__)
 
     if len(args) == 1:
         assert len(kwargs) == 0 and callable(args[0])
         return decorator(args[0], None)
     else:
         assert len(args) == 0 and len(kwargs) == 1 and 'param_types' in kwargs
```

### Comparing `pixeltable-0.2.4/pixeltable/functions/__init__.py` & `pixeltable-0.2.5/pixeltable/functions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,57 +19,57 @@
 
 # TODO: remove and replace calls with astype()
 def cast(expr: exprs.Expr, target_type: ColumnType) -> exprs.Expr:
     expr.col_type = target_type
     return expr
 
 @func.uda(
-    update_types=[IntType()], value_type=IntType(), name='sum', allows_window=True, requires_order_by=False)
-class SumAggregator(func.Aggregator):
+    update_types=[IntType()], value_type=IntType(), allows_window=True, requires_order_by=False)
+class sum(func.Aggregator):
     def __init__(self):
         self.sum: Union[int, float] = 0
     def update(self, val: Union[int, float]) -> None:
         if val is not None:
             self.sum += val
     def value(self) -> Union[int, float]:
         return self.sum
 
 
 @func.uda(
-    update_types=[IntType()], value_type=IntType(), name='count', allows_window = True, requires_order_by = False)
-class CountAggregator(func.Aggregator):
+    update_types=[IntType()], value_type=IntType(), allows_window = True, requires_order_by = False)
+class count(func.Aggregator):
     def __init__(self):
         self.count = 0
     def update(self, val: int) -> None:
         if val is not None:
             self.count += 1
     def value(self) -> int:
         return self.count
 
 
 @func.uda(
-    update_types=[IntType()], value_type=FloatType(), name='mean', allows_window=False, requires_order_by=False)
-class MeanAggregator(func.Aggregator):
+    update_types=[IntType()], value_type=FloatType(), allows_window=False, requires_order_by=False)
+class mean(func.Aggregator):
     def __init__(self):
         self.sum = 0
         self.count = 0
     def update(self, val: int) -> None:
         if val is not None:
             self.sum += val
             self.count += 1
     def value(self) -> float:
         if self.count == 0:
             return None
         return self.sum / self.count
 
 
 @func.uda(
-    init_types=[IntType()], update_types=[ImageType()], value_type=VideoType(), name='make_video',
+    init_types=[IntType()], update_types=[ImageType()], value_type=VideoType(),
     requires_order_by=True, allows_window=False)
-class VideoAggregator(func.Aggregator):
+class make_video(func.Aggregator):
     def __init__(self, fps: int = 25):
         """follows https://pyav.org/docs/develop/cookbook/numpy.html#generating-video"""
         self.container: Optional[av.container.OutputContainer] = None
         self.stream: Optional[av.stream.Stream] = None
         self.fps = fps
 
     def update(self, frame: PIL.Image.Image) -> None:
```

### Comparing `pixeltable-0.2.4/pixeltable/functions/eval.py` & `pixeltable-0.2.5/pixeltable/functions/eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import annotations
 from typing import List, Tuple, Dict
 from collections import defaultdict
 import sys
 
 import numpy as np
 
 import pixeltable.type_system as ts
@@ -153,40 +152,40 @@
         ts.JsonType(nullable=False),
         ts.JsonType(nullable=False),
         ts.JsonType(nullable=False),
         ts.JsonType(nullable=False),
         ts.JsonType(nullable=False)
     ])
 def eval_detections(
-        pred_bboxes: List[List[int]], pred_classes: List[int], pred_scores: List[float],
-        gt_bboxes: List[List[int]], gt_classes: List[int]
+        pred_bboxes: List[List[int]], pred_labels: List[int], pred_scores: List[float],
+        gt_bboxes: List[List[int]], gt_labels: List[int]
 ) -> Dict:
-    class_idxs = list(set(pred_classes + gt_classes))
+    class_idxs = list(set(pred_labels + gt_labels))
     result: List[Dict] = []
     pred_bboxes_arr = np.asarray(pred_bboxes)
-    pred_classes_arr = np.asarray(pred_classes)
+    pred_classes_arr = np.asarray(pred_labels)
     pred_scores_arr = np.asarray(pred_scores)
     gt_bboxes_arr = np.asarray(gt_bboxes)
-    gt_classes_arr = np.asarray(gt_classes)
+    gt_classes_arr = np.asarray(gt_labels)
     for class_idx in class_idxs:
         pred_filter = pred_classes_arr == class_idx
         gt_filter = gt_classes_arr == class_idx
         class_pred_scores = pred_scores_arr[pred_filter]
         tp, fp = calculate_image_tpfp(
             pred_bboxes_arr[pred_filter], class_pred_scores, gt_bboxes_arr[gt_filter], [0.5])
         ordered_class_pred_scores = -np.sort(-class_pred_scores)
         result.append({
             'min_iou': 0.5, 'class': class_idx, 'tp': tp.tolist(), 'fp': fp.tolist(),
             'scores': ordered_class_pred_scores.tolist(), 'num_gts': gt_filter.sum().item(),
         })
     return result
 
 @func.uda(
-    update_types=[ts.JsonType()], value_type=ts.JsonType(), name='mean_ap', allows_std_agg=True, allows_window=False)
-class MeanAPAggregator:
+    update_types=[ts.JsonType()], value_type=ts.JsonType(), allows_std_agg=True, allows_window=False)
+class mean_ap(func.Aggregator):
     def __init__(self):
         self.class_tpfp: Dict[int, List[Dict]] = defaultdict(list)
 
     def update(self, eval_dicts: List[Dict]) -> None:
         for eval_dict in eval_dicts:
             class_idx = eval_dict['class']
             self.class_tpfp[class_idx].append(eval_dict)
```

### Comparing `pixeltable-0.2.4/pixeltable/functions/fireworks.py` & `pixeltable-0.2.5/pixeltable/functions/fireworks.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/functions/huggingface.py` & `pixeltable-0.2.5/pixeltable/functions/huggingface.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-from typing import Any, Callable
+from typing import Callable, TypeVar, Optional
 
 import PIL.Image
 import numpy as np
 
 import pixeltable as pxt
 import pixeltable.env as env
 import pixeltable.type_system as ts
 from pixeltable.func import Batch
+from pixeltable.functions.util import resolve_torch_device
 
 
 @pxt.udf(batch_size=32, return_type=ts.ArrayType((None,), dtype=ts.FloatType()))
-def sentence_transformer(sentences: Batch[str], *, model_id: str, normalize_embeddings: bool = False) -> Batch[np.ndarray]:
+def sentence_transformer(
+        sentences: Batch[str], *, model_id: str, normalize_embeddings: bool = False
+) -> Batch[np.ndarray]:
     env.Env.get().require_package('sentence_transformers')
     from sentence_transformers import SentenceTransformer
 
     model = _lookup_model(model_id, SentenceTransformer)
 
     array = model.encode(sentences, normalize_embeddings=normalize_embeddings)
     return [array[i] for i in range(array.shape[0])]
@@ -49,71 +52,96 @@
 
     model = _lookup_model(model_id, CrossEncoder)
 
     array = model.predict([[sentence1, s2] for s2 in sentences2], convert_to_numpy=True)
     return array.tolist()
 
 
-@pxt.udf(batch_size=32, return_type=ts.ArrayType((None,), dtype=ts.FloatType(), nullable=False))
+@pxt.udf(batch_size=32, return_type=ts.ArrayType((512,), dtype=ts.FloatType(), nullable=False))
 def clip_text(text: Batch[str], *, model_id: str) -> Batch[np.ndarray]:
     env.Env.get().require_package('transformers')
+    device = resolve_torch_device('auto')
+    import torch
     from transformers import CLIPModel, CLIPProcessor
 
-    model = _lookup_model(model_id, CLIPModel.from_pretrained)
+    model = _lookup_model(model_id, CLIPModel.from_pretrained, device=device)
+    assert model.config.projection_dim == 512
     processor = _lookup_processor(model_id, CLIPProcessor.from_pretrained)
 
-    inputs = processor(text=text, return_tensors='pt', padding=True, truncation=True)
-    embeddings = model.get_text_features(**inputs).detach().numpy()
+    with torch.no_grad():
+        inputs = processor(text=text, return_tensors='pt', padding=True, truncation=True)
+        embeddings = model.get_text_features(**inputs.to(device)).detach().to('cpu').numpy()
+
     return [embeddings[i] for i in range(embeddings.shape[0])]
 
 
-@pxt.udf(batch_size=32, return_type=ts.ArrayType((None,), dtype=ts.FloatType(), nullable=False))
+@pxt.udf(batch_size=32, return_type=ts.ArrayType((512,), dtype=ts.FloatType(), nullable=False))
 def clip_image(image: Batch[PIL.Image.Image], *, model_id: str) -> Batch[np.ndarray]:
     env.Env.get().require_package('transformers')
+    device = resolve_torch_device('auto')
+    import torch
     from transformers import CLIPModel, CLIPProcessor
 
-    model = _lookup_model(model_id, CLIPModel.from_pretrained)
+    model = _lookup_model(model_id, CLIPModel.from_pretrained, device=device)
+    assert model.config.projection_dim == 512
     processor = _lookup_processor(model_id, CLIPProcessor.from_pretrained)
 
-    inputs = processor(images=image, return_tensors='pt', padding=True)
-    embeddings = model.get_image_features(**inputs).detach().numpy()
+    with torch.no_grad():
+        inputs = processor(images=image, return_tensors='pt', padding=True)
+        embeddings = model.get_image_features(**inputs.to(device)).detach().to('cpu').numpy()
+
     return [embeddings[i] for i in range(embeddings.shape[0])]
 
 
-@pxt.udf(batch_size=32)
+@pxt.udf(batch_size=4)
 def detr_for_object_detection(image: Batch[PIL.Image.Image], *, model_id: str, threshold: float = 0.5) -> Batch[dict]:
     env.Env.get().require_package('transformers')
+    device = resolve_torch_device('auto')
+    import torch
     from transformers import DetrImageProcessor, DetrForObjectDetection
 
-    model = _lookup_model(model_id, lambda x: DetrForObjectDetection.from_pretrained(x, revision='no_timm'))
+    model = _lookup_model(
+        model_id, lambda x: DetrForObjectDetection.from_pretrained(x, revision='no_timm'), device=device)
     processor = _lookup_processor(model_id, lambda x: DetrImageProcessor.from_pretrained(x, revision='no_timm'))
 
-    inputs = processor(images=image, return_tensors='pt')
-    outputs = model(**inputs)
+    with torch.no_grad():
+        inputs = processor(images=image, return_tensors='pt')
+        outputs = model(**inputs.to(device))
+        results = processor.post_process_object_detection(
+            outputs, threshold=threshold, target_sizes=[(img.height, img.width) for img in image]
+        )
 
-    results = processor.post_process_object_detection(outputs, threshold=threshold)
     return [
         {
             'scores': [score.item() for score in result['scores']],
             'labels': [label.item() for label in result['labels']],
             'label_text': [model.config.id2label[label.item()] for label in result['labels']],
             'boxes': [box.tolist() for box in result['boxes']]
         }
         for result in results
     ]
 
 
-def _lookup_model(model_id: str, create: Callable) -> Any:
-    key = (model_id, create)  # For safety, include the `create` callable in the cache key
+T = TypeVar('T')
+
+
+def _lookup_model(model_id: str, create: Callable[[str], T], device: Optional[str] = None) -> T:
+    from torch import nn
+    key = (model_id, create, device)  # For safety, include the `create` callable in the cache key
     if key not in _model_cache:
-        _model_cache[key] = create(model_id)
+        model = create(model_id)
+        if device is not None:
+            model.to(device)
+        if isinstance(model, nn.Module):
+            model.eval()
+        _model_cache[key] = model
     return _model_cache[key]
 
 
-def _lookup_processor(model_id: str, create: Callable) -> Any:
+def _lookup_processor(model_id: str, create: Callable[[str], T]) -> T:
     key = (model_id, create)  # For safety, include the `create` callable in the cache key
     if key not in _processor_cache:
         _processor_cache[key] = create(model_id)
     return _processor_cache[key]
 
 
 _model_cache = {}
```

### Comparing `pixeltable-0.2.4/pixeltable/functions/openai.py` & `pixeltable-0.2.5/pixeltable/functions/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 # Exponential backoff decorator using tenacity.
 # TODO(aaron-siegel): Right now this hardwires random exponential backoff with defaults suggested
 # by OpenAI. Should we investigate making this more customizable in the future?
 def _retry(fn: Callable) -> Callable:
     return tenacity.retry(
         retry=tenacity.retry_if_exception_type(openai.RateLimitError),
-        wait=tenacity.wait_random_exponential(min=1, max=60),
-        stop=tenacity.stop_after_attempt(6)
+        wait=tenacity.wait_random_exponential(multiplier=3, max=180),
+        stop=tenacity.stop_after_attempt(20)
     )(fn)
 
 
 #####################################
 # Audio Endpoints
 
 @pxt.udf(return_type=ts.AudioType())
```

### Comparing `pixeltable-0.2.4/pixeltable/functions/pil/image.py` & `pixeltable-0.2.5/pixeltable/functions/pil/image.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/functions/string.py` & `pixeltable-0.2.5/pixeltable/functions/string.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/functions/together.py` & `pixeltable-0.2.5/pixeltable/functions/together.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/functions/util.py` & `pixeltable-0.2.5/pixeltable/functions/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -35,7 +35,18 @@
 
         # add a Function for this model to the module
         model_id = info.name.replace("/", "_").replace("-", "_")
         pt_func = func.NOSFunction(info, f'{submodule_name}.{model_id}')
         setattr(sub_module, model_id, pt_func)
 
     return new_modules
+
+
+def resolve_torch_device(device: str) -> str:
+    import torch
+    if device == 'auto':
+        if torch.cuda.is_available():
+            return 'cuda'
+        if torch.backends.mps.is_available():
+            return 'mps'
+        return 'cpu'
+    return device
```

### Comparing `pixeltable-0.2.4/pixeltable/functions/video.py` & `pixeltable-0.2.5/pixeltable/functions/video.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/iterators/base.py` & `pixeltable-0.2.5/pixeltable/iterators/base.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/iterators/document.py` & `pixeltable-0.2.5/pixeltable/iterators/document.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/iterators/video.py` & `pixeltable-0.2.5/pixeltable/iterators/video.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/metadata/__init__.py` & `pixeltable-0.2.5/pixeltable/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/metadata/converters/convert_10.py` & `pixeltable-0.2.5/pixeltable/metadata/converters/convert_10.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/metadata/schema.py` & `pixeltable-0.2.5/pixeltable/metadata/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, List, Dict, get_type_hints, Type, Any, TypeVar, Tuple, Union
+from typing import Optional, List, get_type_hints, Type, Any, TypeVar, Tuple, Union
 import platform
 import uuid
 import dataclasses
 
 import sqlalchemy as sql
 from sqlalchemy import Integer, String, Boolean, BigInteger, LargeBinary
 from sqlalchemy.dialects.postgresql import UUID, JSONB
@@ -67,61 +67,88 @@
 
     id = sql.Column(UUID(as_uuid=True), primary_key=True, default=uuid.uuid4, nullable=False)
     parent_id = sql.Column(UUID(as_uuid=True), ForeignKey('dirs.id'), nullable=True)
     md = sql.Column(JSONB, nullable=False)
 
 
 @dataclasses.dataclass
-class ColumnHistory:
+class ColumnMd:
     """
-    Records when a column was added/dropped, which is needed to GC unreachable storage columns
-    (a column that was added after table snapshot n and dropped before table snapshot n+1 can be removed
-    from the stored table).
-    One record per column (across all schema versions).
+    Records the non-versioned metadata of a column.
+    - immutable attributes: type, primary key, etc.
+    - when a column was added/dropped, which is needed to GC unreachable storage columns
+      (a column that was added after table snapshot n and dropped before table snapshot n+1 can be removed
+      from the stored table).
      """
-    col_id: int
+    id: int
     schema_version_add: int
     schema_version_drop: Optional[int]
+    col_type: dict
+
+    # if True, is part of the primary key
+    is_pk: bool
+
+    # if set, this is a computed column
+    value_expr: Optional[dict]
+
+    # if True, the column is present in the stored table
+    stored: Optional[bool]
+
+
+@dataclasses.dataclass
+class IndexMd:
+    """
+    Metadata needed to instantiate an EmbeddingIndex
+    """
+    id: int
+    name: str
+    indexed_col_id: int  # column being indexed
+    index_val_col_id: int  # column holding the values to be indexed
+    index_val_undo_col_id: int  # column holding index values for deleted rows
+    schema_version_add: int
+    schema_version_drop: Optional[int]
+    class_fqn: str
+    init_args: dict[str, Any]
 
 
 @dataclasses.dataclass
 class ViewMd:
     is_snapshot: bool
 
     # (table id, version); for mutable views, all versions are None
     base_versions: List[Tuple[str, Optional[int]]]
 
     # filter predicate applied to the base table; view-only
-    predicate: Optional[Dict[str, Any]]
+    predicate: Optional[dict[str, Any]]
 
     # ComponentIterator subclass; only for component views
     iterator_class_fqn: Optional[str]
 
     # args to pass to the iterator class constructor; only for component views
-    iterator_args: Optional[Dict[str, Any]]
+    iterator_args: Optional[dict[str, Any]]
 
 
 @dataclasses.dataclass
 class TableMd:
     name: str
 
     # monotonically increasing w/in Table for both data and schema changes, starting at 0
     current_version: int
     # each version has a corresponding schema version (current_version >= current_schema_version)
     current_schema_version: int
 
-    # used to assign Column.id
-    next_col_id: int
+    next_col_id: int  # used to assign Column.id
+    next_idx_id: int  # used to assign IndexMd.id
 
     # - used to assign the rowid column in the storage table
     # - every row is assigned a unique and immutable rowid on insertion
     next_row_id: int
 
-    column_history: Dict[int, ColumnHistory]  # col_id -> ColumnHistory
-
+    column_md: dict[int, ColumnMd]  # col_id -> ColumnMd
+    index_md: dict[int, IndexMd]  # index_id -> IndexMd
     view_md: Optional[ViewMd]
 
 
 class Table(Base):
     """
     Table represents both tables and views.
 
@@ -151,32 +178,28 @@
     version = sql.Column(BigInteger, primary_key=True, nullable=False)
     md = sql.Column(JSONB, nullable=False)  # TableVersionMd
 
 
 @dataclasses.dataclass
 class SchemaColumn:
     """
-    Records the logical (user-visible) schema of a table.
-    Contains the full set of columns for each new schema version: one record per (column x schema version).
+    Records the versioned metadata of a column.
     """
     pos: int
     name: str
-    col_type: dict
-    is_pk: bool
-    value_expr: Optional[dict]
-    stored: Optional[bool]
-    # if True, creates vector index for this column
-    is_indexed: bool
 
 
 @dataclasses.dataclass
 class TableSchemaVersionMd:
+    """
+    Records all versioned table metadata.
+    """
     schema_version: int
     preceding_schema_version: Optional[int]
-    columns: Dict[int, SchemaColumn]  # col_id -> SchemaColumn
+    columns: dict[int, SchemaColumn]  # col_id -> SchemaColumn
     num_retained_versions: int
     comment: str
 
 
 # versioning: each table schema change results in a new record
 class TableSchemaVersion(Base):
     __tablename__ = 'tableschemaversions'
```

### Comparing `pixeltable-0.2.4/pixeltable/plan.py` & `pixeltable-0.2.5/pixeltable/plan.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,16 @@
                 if len(similarity_clauses) == 1:
                     if len(self.order_by_clause) > 0:
                         raise excs.Error((
                             f'nearest() returns results in order of proximity and cannot be used in conjunction with '
                             f'order_by()'))
                     self.similarity_clause = similarity_clauses[0]
                     img_col = self.similarity_clause.img_col_ref.col
-                    if not img_col.is_indexed:
+                    indexed_col_ids = {info.col.id for info in tbl.tbl_version.idxs_by_name.values()}
+                    if img_col.id not in indexed_col_ids:
                         raise excs.Error(f'nearest() not available for unindexed column {img_col.name}')
 
         # all exprs that are evaluated in Python; not executable
         self.all_exprs = self.select_list.copy()
         self.all_exprs.extend(self.group_by_clause)
         self.all_exprs.extend([e for e, _ in self.order_by_clause])
         if self.filter is not None:
@@ -216,26 +217,19 @@
 
     @classmethod
     def create_insert_plan(
             cls, tbl: catalog.TableVersion, rows: List[Dict[str, Any]], ignore_errors: bool
     ) -> exec.ExecNode:
         """Creates a plan for TableVersion.insert()"""
         assert not tbl.is_view()
-        # things we need to materialize:
-        # 1. stored_cols: all cols we need to store, incl computed cols (and indices)
+        # stored_cols: all cols we need to store, incl computed cols (and indices)
         stored_cols = [c for c in tbl.cols if c.is_stored]
         assert len(stored_cols) > 0
-        # 2. values to insert into indices
-        indexed_cols = [c for c in tbl.cols if c.is_indexed]
-        index_info: List[Tuple[catalog.Column, func.Function]] = []
-        if len(indexed_cols) > 0:
-            from pixeltable.functions.nos.image_embedding import openai_clip
-            index_info = [(c, openai_clip) for c in tbl.cols if c.is_indexed]
 
-        row_builder = exprs.RowBuilder([], stored_cols, index_info, [])
+        row_builder = exprs.RowBuilder([], stored_cols, [])
 
         # create InMemoryDataNode for 'rows'
         stored_col_info = row_builder.output_slot_idxs()
         stored_img_col_info = [info for info in stored_col_info if info.col.col_type.is_image_type()]
         input_col_info = [info for info in stored_col_info if not info.col.is_computed]
         plan = exec.InMemoryDataNode(tbl, rows, row_builder, tbl.next_rowid)
 
@@ -256,15 +250,15 @@
                 row_builder, batch_size=0, show_pbar=True, num_computed_exprs=len(computed_exprs),
                 ignore_errors=ignore_errors))
         return plan
 
     @classmethod
     def create_update_plan(
             cls, tbl: catalog.TableVersionPath,
-            update_targets: List[Tuple[catalog.Column, exprs.Expr]],
+            update_targets: dict[catalog.Column, exprs.Expr],
             recompute_targets: List[catalog.Column],
             where_clause: Optional[exprs.Predicate], cascade: bool
     ) -> Tuple[exec.ExecNode, List[str], List[catalog.Column]]:
         """Creates a plan to materialize updated rows.
         The plan:
         - retrieves rows that are visible at the current version of the table
         - materializes all stored columns and the update targets
@@ -275,32 +269,32 @@
             - root node of the plan
             - list of qualified column names that are getting updated
             - list of columns that are being recomputed
         """
         # retrieve all stored cols and all target exprs
         assert isinstance(tbl, catalog.TableVersionPath)
         target = tbl.tbl_version  # the one we need to update
-        updated_cols = [col for col, _ in update_targets]
+        updated_cols = list(update_targets.keys())
         if len(recompute_targets) > 0:
             recomputed_cols = recompute_targets.copy()
         else:
             recomputed_cols = target.get_dependent_columns(updated_cols) if cascade else {}
             # we only need to recompute stored columns (unstored ones are substituted away)
             recomputed_cols = {c for c in recomputed_cols if c.is_stored}
         recomputed_base_cols = {col for col in recomputed_cols if col.tbl == target}
         copied_cols = [
             col for col in target.cols if col.is_stored and not col in updated_cols and not col in recomputed_base_cols
         ]
         select_list = [exprs.ColumnRef(col) for col in copied_cols]
-        select_list.extend([expr for _, expr in update_targets])
+        select_list.extend(update_targets.values())
 
         recomputed_exprs = \
             [c.value_expr.copy().resolve_computed_cols(resolve_cols=recomputed_base_cols) for c in recomputed_base_cols]
         # recomputed cols reference the new values of the updated cols
-        for col, e in update_targets:
+        for col, e in update_targets.items():
             exprs.Expr.list_substitute(recomputed_exprs, exprs.ColumnRef(col), e)
         select_list.extend(recomputed_exprs)
 
         # we need to retrieve the PK columns of the existing rows
         plan = cls.create_query_plan(tbl, select_list, where_clause=where_clause, with_pk=True, ignore_errors=True)
         all_base_cols = copied_cols + updated_cols + list(recomputed_base_cols)  # same order as select_list
         # update row builder with column information
@@ -371,24 +365,18 @@
         # things we need to materialize as DataRows:
         # 1. stored computed cols
         # - iterator columns are effectively computed, just not with a value_expr
         # - we can ignore stored non-computed columns because they have a default value that is supplied directly by
         #   the store
         target = view.tbl_version  # the one we need to populate
         stored_cols = [c for c in target.cols if c.is_stored and (c.is_computed or target.is_iterator_column(c))]
-        # 2. index values
-        indexed_cols = [c for c in target.cols if c.is_indexed]
-        index_info: List[Tuple[catalog.Column, func.Function]] = []
-        if len(indexed_cols) > 0:
-            from pixeltable.functions.nos.image_embedding import openai_clip
-            index_info = [(c, openai_clip) for c in target.cols if c.is_indexed]
-        # 3. for component views: iterator args
+        # 2. for component views: iterator args
         iterator_args = [target.iterator_args] if target.iterator_args is not None else []
 
-        row_builder = exprs.RowBuilder(iterator_args, stored_cols, index_info, [])
+        row_builder = exprs.RowBuilder(iterator_args, stored_cols, [])
 
         # execution plan:
         # 1. materialize exprs computed from the base that are needed for stored view columns
         # 2. if it's an iterator view, expand the base rows into component rows
         # 3. materialize stored view columns that haven't been produced by step 1
         base_output_exprs = [e for e in row_builder.default_eval_ctx.exprs if e.is_bound_by(view.base)]
         view_output_exprs = [
@@ -544,15 +532,15 @@
         if order_by_clause is None:
             order_by_clause = []
         if exact_version_only is None:
             exact_version_only = []
         analyzer = Analyzer(
             tbl, select_list, where_clause=where_clause, group_by_clause=group_by_clause,
             order_by_clause=order_by_clause)
-        row_builder = exprs.RowBuilder(analyzer.all_exprs, [], [], analyzer.sql_exprs)
+        row_builder = exprs.RowBuilder(analyzer.all_exprs, [], analyzer.sql_exprs)
 
         analyzer.finalize(row_builder)
         # select_list: we need to materialize everything that's been collected
         # with_pk: for now, we always retrieve the PK, because we need it for the file cache
         plan = cls._create_query_plan(
             tbl, row_builder, analyzer=analyzer, limit=limit, with_pk=True, exact_version_only=exact_version_only)
         plan.ctx.ignore_errors = ignore_errors
@@ -623,34 +611,27 @@
     @classmethod
     def analyze(cls, tbl: catalog.TableVersionPath, where_clause: exprs.Predicate) -> Analyzer:
         return Analyzer(tbl, [], where_clause=where_clause)
 
     @classmethod
     def create_add_column_plan(
             cls, tbl: catalog.TableVersionPath, col: catalog.Column
-    ) -> Tuple[exec.ExecNode, Optional[int], Optional[int]]:
+    ) -> Tuple[exec.ExecNode, Optional[int]]:
         """Creates a plan for InsertableTable.add_column()
         Returns:
             plan: the plan to execute
-            ctx: the context to use for the plan
             value_expr slot idx for the plan output (for computed cols)
-            embedding slot idx for the plan output (for indexed image cols)
         """
         assert isinstance(tbl, catalog.TableVersionPath)
         index_info: List[Tuple[catalog.Column, func.Function]] = []
-        if col.is_indexed:
-            from pixeltable.functions.nos.image_embedding import openai_clip
-            index_info = [(col, openai_clip)]
-        row_builder = exprs.RowBuilder(
-            output_exprs=[], columns=[col], indices=index_info, input_exprs=[])
+        row_builder = exprs.RowBuilder(output_exprs=[], columns=[col], input_exprs=[])
         analyzer = Analyzer(tbl, row_builder.default_eval_ctx.target_exprs)
         plan = cls._create_query_plan(tbl, row_builder=row_builder, analyzer=analyzer, with_pk=True)
         plan.ctx.batch_size = 16
         plan.ctx.show_pbar = True
         plan.ctx.ignore_errors = True
 
         # we want to flush images
         if col.is_computed and col.is_stored and col.col_type.is_image_type():
             plan.set_stored_img_cols(row_builder.output_slot_idxs())
-        value_expr_slot_idx: Optional[int] = row_builder.output_slot_idxs()[0].slot_idx if col.is_computed else None
-        embedding_slot_idx: Optional[int] = row_builder.index_slot_idxs()[0].slot_idx if col.is_indexed else None
-        return plan, value_expr_slot_idx, embedding_slot_idx
+        value_expr_slot_idx = row_builder.output_slot_idxs()[0].slot_idx if col.is_computed else None
+        return plan, value_expr_slot_idx
```

### Comparing `pixeltable-0.2.4/pixeltable/store.py` & `pixeltable-0.2.5/pixeltable/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     - v_max: version at which the row was deleted (or MAX_VERSION if it's still live)
     """
 
     def __init__(self, tbl_version: catalog.TableVersion):
         self.tbl_version = tbl_version
         self.sa_md = sql.MetaData()
         self.sa_tbl: Optional[sql.Table] = None
-        self._create_sa_tbl()
+        self.create_sa_tbl()
 
     def pk_columns(self) -> List[sql.Column]:
         return self._pk_columns
 
     def rowid_columns(self) -> List[sql.Column]:
         return self._pk_columns[:-1]
 
@@ -58,31 +58,28 @@
         self.v_min_col = sql.Column('v_min', sql.BigInteger, nullable=False)
         self.v_max_col = \
             sql.Column('v_max', sql.BigInteger, nullable=False, server_default=str(schema.Table.MAX_VERSION))
         self._pk_columns = [*rowid_cols, self.v_min_col]
         return [*rowid_cols, self.v_min_col, self.v_max_col]
 
 
-    def _create_sa_tbl(self) -> None:
+    def create_sa_tbl(self) -> None:
         """Create self.sa_tbl from self.tbl_version."""
         system_cols = self._create_system_columns()
         all_cols = system_cols.copy()
         idxs: List[sql.Index] = []
         for col in [c for c in self.tbl_version.cols if c.is_stored]:
             # re-create sql.Column for each column, regardless of whether it already has sa_col set: it was bound
             # to the last sql.Table version we created and cannot be reused
             col.create_sa_cols()
             all_cols.append(col.sa_col)
             if col.records_errors:
                 all_cols.append(col.sa_errormsg_col)
                 all_cols.append(col.sa_errortype_col)
 
-            if col.is_indexed:
-                all_cols.append(col.sa_idx_col)
-
             # we create an index for:
             # - scalar columns (except for strings, because long strings can't be used for B-tree indices)
             # - non-computed video and image columns (they will contain external paths/urls that users might want to
             #   filter on)
             if (col.col_type.is_scalar_type() and not col.col_type.is_string_type()) \
                     or (col.col_type.is_media_type() and not col.is_computed):
                 # index names need to be unique within the Postgres instance
@@ -141,16 +138,16 @@
 
     def _move_tmp_media_files(
             self, table_rows: List[Dict[str, Any]], media_cols: List[catalog.Column], v_min: int
     ) -> None:
         """Move tmp media files that we generated to a permanent location"""
         for c in media_cols:
             for table_row in table_rows:
-                file_url = table_row[c.storage_name()]
-                table_row[c.storage_name()] = self._move_tmp_media_file(file_url, c, v_min)
+                file_url = table_row[c.store_name()]
+                table_row[c.store_name()] = self._move_tmp_media_file(file_url, c, v_min)
 
     def _create_table_row(
             self, input_row: exprs.DataRow, row_builder: exprs.RowBuilder, media_cols: List[catalog.Column],
             exc_col_ids: Set[int], v_min: int
     ) -> Tuple[Dict[str, Any], int]:
         """Return Tuple[complete table row, # of exceptions] for insert()
         Creates a row that includes the PK columns, with the values from input_row.pk.
@@ -164,24 +161,27 @@
             if pk_col == self.v_min_col:
                 table_row[pk_col.name] = v_min
             else:
                 table_row[pk_col.name] = pk_val
 
         return table_row, num_excs
 
-    def count(self) -> None:
+    def count(self, conn: Optional[sql.engine.Connection] = None) -> int:
         """Return the number of rows visible in self.tbl_version"""
         stmt = sql.select(sql.func.count('*'))\
             .select_from(self.sa_tbl)\
             .where(self.v_min_col <= self.tbl_version.version)\
             .where(self.v_max_col > self.tbl_version.version)
-        with env.Env.get().engine.begin() as conn:
+        if conn is None:
+            with env.Env.get().engine.connect() as conn:
+                result = conn.execute(stmt).scalar_one()
+        else:
             result = conn.execute(stmt).scalar_one()
-            assert isinstance(result, int)
-            return result
+        assert isinstance(result, int)
+        return result
 
     def create(self, conn: sql.engine.Connection) -> None:
         self.sa_md.create_all(bind=conn)
 
     def drop(self, conn: sql.engine.Connection) -> None:
         """Drop store table"""
         self.sa_md.drop_all(bind=conn)
@@ -189,46 +189,43 @@
     def add_column(self, col: catalog.Column, conn: sql.engine.Connection) -> None:
         """Add column(s) to the store-resident table based on a catalog column
 
         Note that a computed catalog column will require two extra columns (for the computed value and for the error
         message).
         """
         assert col.is_stored
-        stmt = sql.text(f'ALTER TABLE {self._storage_name()} ADD COLUMN {col.storage_name()} {col.col_type.to_sql()}')
+        col_type_str = col.get_sa_col_type().compile(dialect=conn.dialect)
+        stmt = sql.text(f'ALTER TABLE {self._storage_name()} ADD COLUMN {col.store_name()} {col_type_str} NULL')
         log_stmt(_logger, stmt)
         conn.execute(stmt)
-        added_storage_cols = [col.storage_name()]
+        added_storage_cols = [col.store_name()]
         if col.records_errors:
             # we also need to create the errormsg and errortype storage cols
             stmt = (f'ALTER TABLE {self._storage_name()} '
-                    f'ADD COLUMN {col.errormsg_storage_name()} {StringType().to_sql()} DEFAULT NULL')
+                    f'ADD COLUMN {col.errormsg_store_name()} {StringType().to_sql()} DEFAULT NULL')
             conn.execute(sql.text(stmt))
             stmt = (f'ALTER TABLE {self._storage_name()} '
-                    f'ADD COLUMN {col.errortype_storage_name()} {StringType().to_sql()} DEFAULT NULL')
+                    f'ADD COLUMN {col.errortype_store_name()} {StringType().to_sql()} DEFAULT NULL')
             conn.execute(sql.text(stmt))
-        added_storage_cols.extend([col.errormsg_storage_name(), col.errortype_storage_name()])
-        self._create_sa_tbl()
+            added_storage_cols.extend([col.errormsg_store_name(), col.errortype_store_name()])
+        self.create_sa_tbl()
         _logger.info(f'Added columns {added_storage_cols} to storage table {self._storage_name()}')
 
-    def drop_column(self, col: Optional[catalog.Column] = None, conn: Optional[sql.engine.Connection] = None) -> None:
-        """Re-create self.sa_tbl and drop column, if one is given"""
-        if col is not None:
-            assert conn is not None
-            stmt = f'ALTER TABLE {self._storage_name()} DROP COLUMN {col.storage_name()}'
+    def drop_column(self, col: catalog.Column, conn: sql.engine.Connection) -> None:
+        """Execute Alter Table Drop Column statement"""
+        stmt = f'ALTER TABLE {self._storage_name()} DROP COLUMN {col.store_name()}'
+        conn.execute(sql.text(stmt))
+        if col.records_errors:
+            stmt = f'ALTER TABLE {self._storage_name()} DROP COLUMN {col.errormsg_store_name()}'
+            conn.execute(sql.text(stmt))
+            stmt = f'ALTER TABLE {self._storage_name()} DROP COLUMN {col.errortype_store_name()}'
             conn.execute(sql.text(stmt))
-            if col.records_errors:
-                stmt = f'ALTER TABLE {self._storage_name()} DROP COLUMN {col.errormsg_storage_name()}'
-                conn.execute(sql.text(stmt))
-                stmt = f'ALTER TABLE {self._storage_name()} DROP COLUMN {col.errortype_storage_name()}'
-                conn.execute(sql.text(stmt))
-        self._create_sa_tbl()
 
     def load_column(
-            self, col: catalog.Column, exec_plan: ExecNode, value_expr_slot_idx: int, embedding_slot_idx: int,
-            conn: sql.engine.Connection
+            self, col: catalog.Column, exec_plan: ExecNode, value_expr_slot_idx: int, conn: sql.engine.Connection
     ) -> int:
         """Update store column of a computed column with values produced by an execution plan
 
         Returns:
             number of rows with exceptions
         Raises:
             sql.exc.DBAPIError if there was an error during SQL execution
@@ -249,26 +246,19 @@
                         error_msg = str(value_exc)
                         values_dict = {
                             col.sa_col: None,
                             col.sa_errortype_col: error_type,
                             col.sa_errormsg_col: error_msg
                         }
                     else:
-                        val = result_row.get_stored_val(value_expr_slot_idx)
+                        val = result_row.get_stored_val(value_expr_slot_idx, col.sa_col.type)
                         if col.col_type.is_media_type():
                             val = self._move_tmp_media_file(val, col, result_row.pk[-1])
                         values_dict = {col.sa_col: val}
 
-                if col.is_indexed:
-                    # TODO: deal with exceptions
-                    assert not result_row.has_exc(embedding_slot_idx)
-                    # don't use get_stored_val() here, we need to pass the ndarray
-                    embedding = result_row[embedding_slot_idx]
-                    values_dict[col.sa_index_col] = embedding
-
                 update_stmt = sql.update(self.sa_tbl).values(values_dict)
                 for pk_col, pk_val in zip(self.pk_columns(), result_row.pk):
                     update_stmt = update_stmt.where(pk_col == pk_val)
                 log_stmt(_logger, update_stmt)
                 conn.execute(update_stmt)
 
         return num_excs
@@ -333,14 +323,15 @@
             return clause
         return sql.and_(clause, self.base._versions_clause(versions[1:], match_on_vmin))
 
     def delete_rows(
             self, current_version: int, base_versions: List[Optional[int]], match_on_vmin: bool,
             where_clause: Optional[sql.ClauseElement], conn: sql.engine.Connection) -> int:
         """Mark rows as deleted that are live and were created prior to current_version.
+        Also: populate the undo columns
         Args:
             base_versions: if non-None, join only to base rows that were created at that version,
                 otherwise join to rows that are live in the base's current version (which is distinct from the
                 current_version parameter)
             match_on_vmin: if True, match exact versions on v_min; if False, match on v_max
             where_clause: if not None, also apply where_clause
         Returns:
@@ -350,16 +341,22 @@
         where_clause = sql.and_(
             self.v_min_col < current_version,
             self.v_max_col == schema.Table.MAX_VERSION,
             where_clause)
         rowid_join_clause = self._rowid_join_predicate()
         base_versions_clause = sql.true() if len(base_versions) == 0 \
             else self.base._versions_clause(base_versions, match_on_vmin)
+        set_clause = {self.v_max_col: current_version}
+        for index_info in self.tbl_version.idxs_by_name.values():
+            # copy value column to undo column
+            set_clause[index_info.undo_col.sa_col] = index_info.val_col.sa_col
+            # set value column to NULL
+            set_clause[index_info.val_col.sa_col] = None
         stmt = sql.update(self.sa_tbl) \
-            .values({self.v_max_col: current_version}) \
+            .values(set_clause) \
             .where(where_clause) \
             .where(rowid_join_clause) \
             .where(base_versions_clause)
         log_explain(_logger, stmt, conn)
         status = conn.execute(stmt)
         return status.rowcount
 
@@ -412,16 +409,16 @@
         self.rowid_cols = [sql.Column(c.name, c.type) for c in self.base.rowid_columns()]
         # name of pos column: avoid collisions with bases' pos columns
         self.pos_col = sql.Column(f'pos_{len(self.rowid_cols) - 1}', sql.BigInteger, nullable=False)
         self.pos_col_idx = len(self.rowid_cols)
         self.rowid_cols.append(self.pos_col)
         return self.rowid_cols
 
-    def _create_sa_tbl(self) -> None:
-        super()._create_sa_tbl()
+    def create_sa_tbl(self) -> None:
+        super().create_sa_tbl()
         # we need to fix up the 'pos' column in TableVersion
         self.tbl_version.cols_by_name['pos'].sa_col = self.pos_col
 
     def _rowid_join_predicate(self) -> sql.ClauseElement:
         return sql.and_(
             self.base._rowid_join_predicate(),
             *[c1 == c2 for c1, c2 in zip(self.rowid_columns()[:-1], self.base.rowid_columns())])
```

### Comparing `pixeltable-0.2.4/pixeltable/tests/conftest.py` & `pixeltable-0.2.5/pixeltable/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import logging
 import os
 import pathlib
 from typing import List
 
 import numpy as np
 import pytest
+import PIL.Image
 
 import pixeltable as pxt
 import pixeltable.catalog as catalog
 from pixeltable import exprs
-from pixeltable import functions as ptf
+import pixeltable.functions as pxtf
 from pixeltable.exprs import RELATIVE_PATH_ROOT as R
 from pixeltable.metadata import SystemInfo, create_system_info
 from pixeltable.metadata.schema import TableSchemaVersion, TableVersion, Table, Function, Dir
 from pixeltable.tests.utils import read_data_file, create_test_tbl, create_all_datatypes_tbl, skip_test_if_not_installed
 from pixeltable.type_system import StringType, ImageType, FloatType
 
 
@@ -116,16 +117,15 @@
         t.c3.apply(str),
         t.c4.apply(str),
         t.c5.apply(str),
         t.c6.apply(str),
         t.c1.apply(json.loads),
         t.c8.errortype,
         t.c8.errormsg,
-        ptf.sum(t.c2, group_by=t.c4, order_by=t.c3),
-        #test_stored_fn(t.c2),
+        pxtf.sum(t.c2, group_by=t.c4, order_by=t.c3),
     ]
 
 @pytest.fixture(scope='function')
 def all_datatypes_tbl(test_client: pxt.Client) -> catalog.Table:
     return create_all_datatypes_tbl(test_client)
 
 @pytest.fixture(scope='function')
@@ -149,25 +149,19 @@
         img_t.img.rotate(90),
         # we're using a list here, not a tuple; the latter turns into a list during the back/forth conversion
         img_t.img.rotate(90).resize([224, 224]),
         img_t.img.fileurl,
         img_t.img.localpath,
     ]
 
-# TODO: why does this not work with a session scope? (some user tables don't get created with create_all())
-#@pytest.fixture(scope='session')
-#def indexed_img_tbl(init_env: None) -> catalog.Table:
-#    cl = pxt.Client()
-#    db = cl.create_db('test_indexed')
 @pytest.fixture(scope='function')
-def indexed_img_tbl(test_client: pxt.Client) -> catalog.Table:
-    skip_test_if_not_installed('nos')
+def small_img_tbl(test_client: pxt.Client) -> catalog.Table:
     cl = test_client
     schema = {
-        'img': { 'type': ImageType(nullable=False), 'indexed': True },
+        'img': ImageType(nullable=False),
         'category': StringType(nullable=False),
         'split': StringType(nullable=False),
     }
     tbl = cl.create_table('test_indexed_img_tbl', schema)
     rows = read_data_file('imagenette2-160', 'manifest.csv', ['img'])
     # select output_rows randomly in the hope of getting a good sample of the available categories
     rng = np.random.default_rng(17)
```

### Comparing `pixeltable-0.2.4/pixeltable/tests/functions/test_fireworks.py` & `pixeltable-0.2.5/pixeltable/tests/functions/test_fireworks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pytest
 
 import pixeltable as pxt
 import pixeltable.exceptions as excs
 from pixeltable.tests.utils import skip_test_if_not_installed, validate_update_status
 
 
+@pytest.mark.remote_api
 class TestFireworks:
 
     def test_fireworks(self, test_client: pxt.Client) -> None:
         skip_test_if_not_installed('fireworks')
         TestFireworks.skip_test_if_no_fireworks_client()
         cl = test_client
         t = cl.create_table('test_tbl', {'input': pxt.StringType()})
```

### Comparing `pixeltable-0.2.4/pixeltable/tests/functions/test_functions.py` & `pixeltable-0.2.5/pixeltable/tests/functions/test_functions.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/tests/functions/test_huggingface.py` & `pixeltable-0.2.5/pixeltable/tests/functions/test_huggingface.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,18 +119,18 @@
 
         # run multiple models one at a time in order to exercise batching
         from pixeltable.functions.huggingface import clip_text, clip_image
         model_ids = ['openai/clip-vit-base-patch32', 'laion/CLIP-ViT-B-32-laion2B-s34B-b79K']
         for idx, model_id in enumerate(model_ids):
             col_name = f'embed_text{idx}'
             t[col_name] = clip_text(t.text, model_id=model_id)
-            assert t.column_types()[col_name] == ArrayType((None,), dtype=FloatType(), nullable=False)
+            assert t.column_types()[col_name].is_array_type()
             col_name = f'embed_img{idx}'
             t[col_name] = clip_image(t.img, model_id=model_id)
-            assert t.column_types()[col_name] == ArrayType((None,), dtype=FloatType(), nullable=False)
+            assert t.column_types()[col_name].is_array_type()
 
         def verify_row(row: Dict[str, Any]) -> None:
             for idx, _ in enumerate(model_ids):
                 assert row[f'embed_text{idx}'].shape == (512,)
                 assert row[f'embed_img{idx}'].shape == (512,)
 
         verify_row(t.tail(1)[0])
```

### Comparing `pixeltable-0.2.4/pixeltable/tests/functions/test_openai.py` & `pixeltable-0.2.5/pixeltable/tests/functions/test_openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import pixeltable as pxt
 import pixeltable.exceptions as excs
 from pixeltable.tests.utils import SAMPLE_IMAGE_URL, skip_test_if_not_installed, validate_update_status
 from pixeltable.type_system import StringType, ImageType
 
 
+@pytest.mark.remote_api
 class TestOpenai:
 
     def test_audio(self, test_client: pxt.Client) -> None:
         skip_test_if_not_installed('openai')
         TestOpenai.skip_test_if_no_openai_client()
         cl = test_client
         t = cl.create_table('test_tbl', {'input': StringType()})
@@ -18,27 +19,27 @@
         t.add_column(speech_2=speech(t.input, model='tts-1', voice='onyx', response_format='flac', speed=1.05))
         t.add_column(transcription=transcriptions(t.speech, model='whisper-1'))
         t.add_column(transcription_2=transcriptions(
             t.speech, model='whisper-1', language='en', prompt='Transcribe the contents of this recording.'
         ))
         t.add_column(translation=translations(t.speech, model='whisper-1'))
         t.add_column(translation_2=translations(
-            t.speech, model='whisper-1', prompt='Translate the recording from Spanish into English.', temperature=0.7
+            t.speech, model='whisper-1', prompt='Translate the recording from Spanish into English.', temperature=0.05
         ))
         validate_update_status(t.insert([
             {'input': 'I am a banana.'},
             {'input': 'Es fácil traducir del español al inglés.'}
         ]), expected_rows=2)
         # The audio generation -> transcription loop on these examples should be simple and clear enough
         # that the unit test can reliably expect the output closely enough to pass these checks.
         results = t.collect()
         assert results[0]['transcription']['text'] in ['I am a banana.', "I'm a banana."]
         assert results[0]['transcription_2']['text'] in ['I am a banana.', "I'm a banana."]
-        assert 'easy to translate from Spanish' in results[1]['translation']['text']
-        assert 'easy to translate from Spanish' in results[1]['translation_2']['text']
+        assert 'easy to translate' in results[1]['translation']['text']
+        assert 'easy to translate' in results[1]['translation_2']['text']
 
     def test_chat_completions(self, test_client: pxt.Client) -> None:
         skip_test_if_not_installed('openai')
         TestOpenai.skip_test_if_no_openai_client()
         cl = test_client
         t = cl.create_table('test_tbl', {'input': StringType()})
         from pixeltable.functions.openai import chat_completions
@@ -128,21 +129,30 @@
         t = cl.create_table('test_tbl', {'input': StringType()})
         from pixeltable.functions.openai import image_generations
         t.add_column(img=image_generations(t.input))
         # Test dall-e-2 options
         t.add_column(img_2=image_generations(
             t.input, model='dall-e-2', size='512x512', user='pixeltable'
         ))
+        validate_update_status(t.insert(input='A friendly dinosaur playing tennis in a cornfield'), 1)
+        assert t.collect()['img'][0].size == (1024, 1024)
+        assert t.collect()['img_2'][0].size == (512, 512)
+
+    @pytest.mark.skip('Test is expensive and slow')
+    def test_image_generations_dall_e_3(self, test_client: pxt.Client) -> None:
+        skip_test_if_not_installed('openai')
+        TestOpenai.skip_test_if_no_openai_client()
+        cl = test_client
+        t = cl.create_table('test_tbl', {'input': StringType()})
+        from pixeltable.functions.openai import image_generations
         # Test dall-e-3 options
         t.add_column(img_3=image_generations(
             t.input, model='dall-e-3', quality='hd', size='1792x1024', style='natural', user='pixeltable'
         ))
         validate_update_status(t.insert(input='A friendly dinosaur playing tennis in a cornfield'), 1)
-        assert t.collect()['img'][0].size == (1024, 1024)
-        assert t.collect()['img_2'][0].size == (512, 512)
         assert t.collect()['img_3'][0].size == (1792, 1024)
 
     # This ensures that the test will be skipped, rather than returning an error, when no API key is
     # available (for example, when a PR runs in CI).
     @staticmethod
     def skip_test_if_no_openai_client() -> None:
         try:
```

### Comparing `pixeltable-0.2.4/pixeltable/tests/functions/test_together.py` & `pixeltable-0.2.5/pixeltable/tests/functions/test_together.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pytest
 
 import pixeltable as pxt
 import pixeltable.exceptions as excs
 from pixeltable.tests.utils import skip_test_if_not_installed, validate_update_status
 
 
+@pytest.mark.remote_api
 class TestTogether:
 
     def test_completions(self, test_client: pxt.Client) -> None:
         skip_test_if_not_installed('together')
         TestTogether.skip_test_if_no_together_client()
         cl = test_client
         t = cl.create_table('test_tbl', {'input': pxt.StringType()})
```

### Comparing `pixeltable-0.2.4/pixeltable/tests/test_audio.py` & `pixeltable-0.2.5/pixeltable/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/tests/test_catalog.py` & `pixeltable-0.2.5/pixeltable/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/tests/test_client.py` & `pixeltable-0.2.5/pixeltable/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/tests/test_component_view.py` & `pixeltable-0.2.5/pixeltable/tests/test_component_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pandas as pd
 import pytest
 
 import pixeltable as pxt
 from pixeltable import exceptions as excs
 from pixeltable.iterators import ComponentIterator
 from pixeltable.iterators.video import FrameIterator
-from pixeltable.tests.utils import assert_resultset_eq, get_test_video_files
+from pixeltable.tests.utils import assert_resultset_eq, get_test_video_files, validate_update_status
 from pixeltable.type_system import IntType, VideoType, JsonType
 
 class ConstantImgIterator(ComponentIterator):
     """Component iterator that generates a fixed number of all-black 1280x720 images."""
     def __init__(self, video: str, num_frames: int = 10):
         self.img = PIL.Image.new('RGB', (1280, 720))
         self.next_frame_idx = 0
@@ -153,18 +153,27 @@
 
         video_filepaths = get_test_video_files()
         rows = [{'video': p} for p in video_filepaths]
         status = video_t.insert(rows)
         assert status.num_excs == 0
         import urllib
         video_url = urllib.parse.urljoin('file:', urllib.request.pathname2url(video_filepaths[0]))
-        status = view_t.update({'annotation': {'a': 1}}, where=view_t.video == video_url)
-        c1 = view_t.where(view_t.annotation != None).count()
-        c2 = view_t.where(view_t.video == video_url).count()
-        assert c1 == c2
+        validate_update_status(
+            view_t.update({'annotation': {'a': 1}}, where=view_t.video == video_url),
+            expected_rows=view_t.where(view_t.video == video_url).count())
+        assert view_t.where(view_t.annotation != None).count() == view_t.where(view_t.video == video_url).count()
+
+        # batch update with _rowid works
+        validate_update_status(
+            view_t.batch_update(
+                [{'annotation': {'a': 1}, '_rowid': (1, 0)}, {'annotation': {'a': 1}, '_rowid': (1, 1)}]),
+            expected_rows=2)
+        with pytest.raises(AssertionError):
+            # malformed _rowid
+            view_t.batch_update([{'annotation': {'a': 1}, '_rowid': (1,)}])
 
         with pytest.raises(excs.Error) as excinfo:
             _ = cl.create_view(
                 'bad_view', video_t, schema={'annotation': JsonType(nullable=False)},
                 iterator_class=FrameIterator, iterator_args=args)
         assert 'must be nullable' in str(excinfo.value)
```

### Comparing `pixeltable-0.2.4/pixeltable/tests/test_dataframe.py` & `pixeltable-0.2.5/pixeltable/tests/test_dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,30 @@
 from pixeltable import catalog
 from pixeltable import exceptions as excs
 from pixeltable.iterators import FrameIterator
 from pixeltable.tests.utils import get_video_files, get_audio_files, skip_test_if_not_installed
 
 
 class TestDataFrame:
+
+    @pxt.udf(return_type=pxt.JsonType(nullable=False), param_types=[pxt.JsonType(nullable=False)])
+    def yolo_to_coco(detections):
+        bboxes, labels = detections['bboxes'], detections['labels']
+        num_annotations = len(detections['bboxes'])
+        assert num_annotations == len(detections['labels'])
+        result = []
+        for i in range(num_annotations):
+            bbox = bboxes[i]
+            ann = {
+                'bbox': [round(bbox[0]), round(bbox[1]), round(bbox[2] - bbox[0]), round(bbox[3] - bbox[1])],
+                'category': labels[i],
+            }
+            result.append(ann)
+        return result
+
     def test_select_where(self, test_tbl: catalog.Table) -> None:
         t = test_tbl
         res1 = t[t.c1, t.c2, t.c3].show(0)
         res2 = t.select(t.c1, t.c2, t.c3).show(0)
         assert res1 == res2
 
         res1 = t[t.c2 < 10][t.c1, t.c2, t.c3].show(0)
@@ -152,25 +168,25 @@
         df = t.select(t.c1).where(t.c2 < 10).limit(10)
         df.describe()
 
         # TODO: how to you check the output of these?
         _ = df.__repr__()
         _ = df._repr_html_()
 
-    def test_count(self, test_tbl: catalog.Table, indexed_img_tbl: catalog.Table) -> None:
+    def test_count(self, test_tbl: catalog.Table, small_img_tbl) -> None:
         skip_test_if_not_installed('nos')
         t = test_tbl
         cnt = t.count()
         assert cnt == 100
 
         cnt = t.where(t.c2 < 10).count()
         assert cnt == 10
 
         # count() doesn't work with similarity search
-        t = indexed_img_tbl
+        t = small_img_tbl
         probe = t.select(t.img).show(1)
         img = probe[0, 0]
         with pytest.raises(excs.Error):
             _ = t.where(t.img.nearest(img)).count()
         with pytest.raises(excs.Error):
             _ = t.where(t.img.nearest('car')).count()
 
@@ -393,30 +409,15 @@
         base_t = cl.create_table('videos', {'video': pxt.VideoType()})
         args = {'video': base_t.video, 'fps': 1}
         view_t = cl.create_view('frames', base_t, iterator_class=FrameIterator, iterator_args=args)
         from pixeltable.functions.nos.object_detection_2d import yolox_medium
         view_t.add_column(detections=yolox_medium(view_t.frame))
         base_t.insert(video=get_video_files()[0])
 
-        @pxt.udf(return_type=pxt.JsonType(nullable=False), param_types=[pxt.JsonType(nullable=False)])
-        def yolo_to_coco(detections):
-            bboxes, labels = detections['bboxes'], detections['labels']
-            num_annotations = len(detections['bboxes'])
-            assert num_annotations == len(detections['labels'])
-            result = []
-            for i in range(num_annotations):
-                bbox = bboxes[i]
-                ann = {
-                    'bbox': [round(bbox[0]), round(bbox[1]), round(bbox[2] - bbox[0]), round(bbox[3] - bbox[1])],
-                    'category': labels[i],
-                }
-                result.append(ann)
-            return result
-
-        query = view_t.select({'image': view_t.frame, 'annotations': yolo_to_coco(view_t.detections)})
+        query = view_t.select({'image': view_t.frame, 'annotations': self.yolo_to_coco(view_t.detections)})
         path = query.to_coco_dataset()
         # we get a valid COCO dataset
         coco_ds = COCO(path)
         assert len(coco_ds.imgs) == view_t.count()
 
         # we call to_coco_dataset() again and get the cached dataset
         new_path = query.to_coco_dataset()
```

### Comparing `pixeltable-0.2.4/pixeltable/tests/test_dirs.py` & `pixeltable-0.2.5/pixeltable/tests/test_dirs.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/tests/test_document.py` & `pixeltable-0.2.5/pixeltable/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/tests/test_exprs.py` & `pixeltable-0.2.5/pixeltable/tests/test_exprs.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,56 @@
 from pixeltable.iterators import FrameIterator
 from pixeltable.tests.utils import get_image_files, skip_test_if_not_installed
 from pixeltable.type_system import StringType, BoolType, IntType, ArrayType, ColumnType, FloatType, \
     VideoType
 
 
 class TestExprs:
+    @pxt.udf(return_type=FloatType(), param_types=[IntType(), IntType()])
+    def div_0_error(a: int, b: int) -> float:
+        return a / b
+
+    # function that does allow nulls
+    @pxt.udf(return_type=FloatType(nullable=True),
+            param_types=[FloatType(nullable=False), FloatType(nullable=True)])
+    def null_args_fn(a: int, b: int) -> int:
+        if b is None:
+            return a
+        return a + b
+
+    # error in agg.init()
+    @pxt.uda(update_types=[IntType()], value_type=IntType())
+    class init_exc(pxt.Aggregator):
+        def __init__(self):
+            self.sum = 1 / 0
+        def update(self, val):
+            pass
+        def value(self):
+            return 1
+
+    # error in agg.update()
+    @pxt.uda(update_types=[IntType()], value_type=IntType())
+    class update_exc(pxt.Aggregator):
+        def __init__(self):
+            self.sum = 0
+        def update(self, val):
+            self.sum += 1 / val
+        def value(self):
+            return 1
+
+    # error in agg.value()
+    @pxt.uda(update_types=[IntType()], value_type=IntType())
+    class value_exc(pxt.Aggregator):
+        def __init__(self):
+            self.sum = 0
+        def update(self, val):
+            self.sum += val
+        def value(self):
+            return 1 / self.sum
+
     def test_basic(self, test_tbl: catalog.Table) -> None:
         t = test_tbl
         assert t['c1'].equals(t.c1)
         assert t['c7']['*'].f5.equals(t.c7['*'].f5)
 
         assert isinstance(t.c1 == None, Expr)
         assert isinstance(t.c1 < 'a', Expr)
@@ -58,21 +100,21 @@
         e = (~(t.c1 == 'test string')).sql_expr()
         assert isinstance(e, sql.sql.expression.BinaryExpression)
 
         with pytest.raises(TypeError) as exc_info:
             _ = t.where((t.c1 == 'test string') or (t.c6.f1 > 50)).collect()
         assert 'cannot be used in conjunction with python boolean operators' in str(exc_info.value).lower()
 
-        # compound predicates with Python functions
-        @pxt.udf(return_type=BoolType(), param_types=[StringType()])
-        def udf(_: str) -> bool:
-            return True
-        @pxt.udf(return_type=BoolType(), param_types=[IntType()])
-        def udf2(_: int) -> bool:
-            return True
+        # # compound predicates with Python functions
+        # @pt.udf(return_type=BoolType(), param_types=[StringType()])
+        # def udf(_: str) -> bool:
+        #     return True
+        # @pt.udf(return_type=BoolType(), param_types=[IntType()])
+        # def udf2(_: int) -> bool:
+        #     return True
 
         # TODO: find a way to test this
         # # & can be split
         # p = (t.c1 == 'test string') & udf(t.c1)
         # assert p.sql_expr() is None
         # sql_pred, other_pred = p.extract_sql_predicate()
         # assert isinstance(sql_pred, sql.sql.expression.BinaryExpression)
@@ -116,55 +158,29 @@
             _ = t[(t.c2 + 1) / t.c2].show()
 
         # error in expr that's handled in Python
         with pytest.raises(excs.Error):
             _ = t[(t.c6.f2 + 1) / (t.c2 - 10)].show()
 
         # the same, but with an inline function
-        @pxt.udf(return_type=FloatType(), param_types=[IntType(), IntType()])
-        def f(a: int, b: int) -> float:
-            return a / b
         with pytest.raises(excs.Error):
-            _ = t[f(t.c2 + 1, t.c2)].show()
+            _ = t[self.div_0_error(t.c2 + 1, t.c2)].show()
 
         # error in agg.init()
-        @pxt.uda(update_types=[IntType()], value_type=IntType(), name='agg')
-        class Aggregator(pxt.Aggregator):
-            def __init__(self):
-                self.sum = 1 / 0
-            def update(self, val):
-                pass
-            def value(self):
-                return 1
-        with pytest.raises(excs.Error):
-            _ = t[agg(t.c2)].show()
+        with pytest.raises(excs.Error) as exc_info:
+            _ = t[self.init_exc(t.c2)].show()
+        assert 'division by zero' in str(exc_info.value)
 
         # error in agg.update()
-        @pxt.uda(update_types=[IntType()], value_type=IntType(), name='agg')
-        class Aggregator(pxt.Aggregator):
-            def __init__(self):
-                self.sum = 0
-            def update(self, val):
-                self.sum += 1 / val
-            def value(self):
-                return 1
         with pytest.raises(excs.Error):
-            _ = t[agg(t.c2 - 10)].show()
+            _ = t[self.update_exc(t.c2 - 10)].show()
 
         # error in agg.value()
-        @pxt.uda(update_types=[IntType()], value_type=IntType(), name='agg')
-        class Aggregator(pxt.Aggregator):
-            def __init__(self):
-                self.sum = 0
-            def update(self, val):
-                self.sum += val
-            def value(self):
-                return 1 / self.sum
         with pytest.raises(excs.Error):
-            _ = t[t.c2 <= 2][agg(t.c2 - 1)].show()
+            _ = t[t.c2 <= 2][self.value_exc(t.c2 - 1)].show()
 
     def test_props(self, test_tbl: catalog.Table, img_tbl: catalog.Table) -> None:
         t = test_tbl
         # errortype/-msg for computed column
         res = t.select(error=t.c8.errortype).collect()
         assert res.to_pandas()['error'].isna().all()
         res = t.select(error=t.c8.errormsg).collect()
@@ -217,22 +233,15 @@
     def test_null_args(self, test_client: pxt.Client) -> None:
         # create table with two int columns
         schema = {'c1': FloatType(nullable=True), 'c2': FloatType(nullable=True)}
         t = test_client.create_table('test', schema)
 
         # computed column that doesn't allow nulls
         t.add_column(c3=lambda c1, c2: c1 + c2, type=FloatType(nullable=False))
-        # function that does allow nulls
-        @pxt.udf(return_type=FloatType(nullable=True),
-                 param_types=[FloatType(nullable=False), FloatType(nullable=True)])
-        def f(a: int, b: int) -> int:
-            if b is None:
-                return a
-            return a + b
-        t.add_column(c4=f(t.c1, t.c2))
+        t.add_column(c4=self.null_args_fn(t.c1, t.c2))
 
         # data that tests all combinations of nulls
         data = [{'c1': 1.0, 'c2': 1.0}, {'c1': 1.0, 'c2': None}, {'c1': None, 'c2': 1.0}, {'c1': None, 'c2': None}]
         status = t.insert(data, fail_on_exception=False)
         assert status.num_rows == len(data)
         assert status.num_excs == len(data) - 1
         result = t.select(t.c3, t.c4).collect()
@@ -509,17 +518,18 @@
         result = t[(t.split == 'val') & (t.img.entropy() > 1) & (t.category == 'n03445777')].show()
         print(result)
         result = t[
             (t.split == 'train') & (t.img.entropy() > 1) & (t.split == 'val') & (t.img.entropy() < 0)
         ][t.img, t.split].show()
         print(result)
 
-    def test_similarity(self, indexed_img_tbl: catalog.Table) -> None:
+    @pytest.mark.skip(reason='temporarily disabled')
+    def test_similarity(self, small_img_tbl) -> None:
         skip_test_if_not_installed('nos')
-        t = indexed_img_tbl
+        t = small_img_tbl
         _ = t.show(30)
         probe = t.select(t.img, t.category).show(1)
         img = probe[0, 0]
         result = t.where(t.img.nearest(img)).show(10)
         assert len(result) == 10
         # nearest() with one SQL predicate and one Python predicate
         result = t[t.img.nearest(img) & (t.category == probe[0, 1]) & (t.img.width > 1)].show(10)
@@ -652,76 +662,75 @@
         with pytest.raises(excs.Error):
             # mixing aggregates and non-aggregates
             _ = t[sum(t.c2) + t.c2].group_by(t.c2 % 2).show()
         with pytest.raises(excs.Error):
             # nested aggregates
             _ = t[sum(count(t.c2))].group_by(t.c2 % 2).show()
 
+    @pxt.uda(
+        init_types=[IntType()], update_types=[IntType()], value_type=IntType(),
+        allows_window=True, requires_order_by=False)
+    class window_agg:
+        def __init__(self, val: int = 0):
+            self.val = val
+        def update(self, ignore: int) -> None:
+            pass
+        def value(self) -> int:
+            return self.val
+
+    @pxt.uda(
+        init_types=[IntType()], update_types=[IntType()], value_type=IntType(),
+        requires_order_by=True, allows_window=True)
+    class ordered_agg:
+        def __init__(self, val: int = 0):
+            self.val = val
+        def update(self, i: int) -> None:
+            pass
+        def value(self) -> int:
+            return self.val
+
+    @pxt.uda(
+        init_types=[IntType()], update_types=[IntType()], value_type=IntType(),
+        requires_order_by=False, allows_window=False)
+    class std_agg:
+        def __init__(self, val: int = 0):
+            self.val = val
+        def update(self, i: int) -> None:
+            pass
+        def value(self) -> int:
+            return self.val
+
     def test_udas(self, test_tbl: catalog.Table) -> None:
         t = test_tbl
-
-        @pxt.uda(
-            name='window_agg', init_types=[IntType()], update_types=[IntType()], value_type=IntType(),
-            allows_window=True, requires_order_by=False)
-        class WindowAgg:
-            def __init__(self, val: int = 0):
-                self.val = val
-            def update(self, ignore: int) -> None:
-                pass
-            def value(self) -> int:
-                return self.val
-
-        @pxt.uda(
-            name='ordered_agg', init_types=[IntType()], update_types=[IntType()], value_type=IntType(),
-            requires_order_by=True, allows_window=True)
-        class WindowAgg:
-            def __init__(self, val: int = 0):
-                self.val = val
-            def update(self, i: int) -> None:
-                pass
-            def value(self) -> int:
-                return self.val
-
-        @pxt.uda(
-            name='std_agg', init_types=[IntType()], update_types=[IntType()], value_type=IntType(),
-            requires_order_by=False, allows_window=False)
-        class StdAgg:
-            def __init__(self, val: int = 0):
-                self.val = val
-            def update(self, i: int) -> None:
-                pass
-            def value(self) -> int:
-                return self.val
-
         # init arg is passed along
-        assert t.select(out=window_agg(t.c2, order_by=t.c2)).collect()[0]['out'] == 0
-        assert t.select(out=window_agg(t.c2, val=1, order_by=t.c2)).collect()[0]['out'] == 1
+        assert t.select(out=self.window_agg(t.c2, order_by=t.c2)).collect()[0]['out'] == 0
+        assert t.select(out=self.window_agg(t.c2, val=1, order_by=t.c2)).collect()[0]['out'] == 1
 
         with pytest.raises(excs.Error) as exc_info:
-            _ = t.select(window_agg(t.c2, val=t.c2, order_by=t.c2)).collect()
+            _ = t.select(self.window_agg(t.c2, val=t.c2, order_by=t.c2)).collect()
         assert 'needs to be a constant' in str(exc_info.value)
 
         with pytest.raises(excs.Error) as exc_info:
             # ordering expression not a pixeltable expr
-            _ = t.select(ordered_agg(1, t.c2)).collect()
+            _ = t.select(self.ordered_agg(1, t.c2)).collect()
         assert 'but instead is a' in str(exc_info.value).lower()
 
         with pytest.raises(excs.Error) as exc_info:
             # explicit order_by
-            _ = t.select(ordered_agg(t.c2, order_by=t.c2)).collect()
+            _ = t.select(self.ordered_agg(t.c2, order_by=t.c2)).collect()
         assert 'order_by invalid' in str(exc_info.value).lower()
 
         with pytest.raises(excs.Error) as exc_info:
             # order_by for non-window function
-            _ = t.select(std_agg(t.c2, order_by=t.c2)).collect()
+            _ = t.select(self.std_agg(t.c2, order_by=t.c2)).collect()
         assert 'does not allow windows' in str(exc_info.value).lower()
 
         with pytest.raises(excs.Error) as exc_info:
             # group_by for non-window function
-            _ = t.select(std_agg(t.c2, group_by=t.c4)).collect()
+            _ = t.select(self.std_agg(t.c2, group_by=t.c4)).collect()
         assert 'group_by invalid' in str(exc_info.value).lower()
 
         with pytest.raises(excs.Error) as exc_info:
             # missing init type
             @pxt.uda(update_types=[IntType()], value_type=IntType())
             class WindowAgg:
                 def __init__(self, val: int = 0):
@@ -765,26 +774,14 @@
                 def update(self, val: int) -> None:
                     pass
                 def value(self) -> int:
                     return self.val
         assert 'cannot have parameters with the same name: val' in str(exc_info.value)
 
         with pytest.raises(excs.Error) as exc_info:
-            # invalid name
-            @pxt.uda(name='not an identifier', init_types=[IntType()], update_types=[IntType()], value_type=IntType())
-            class WindowAgg:
-                def __init__(self, val: int = 0):
-                    self.val = val
-                def update(self, i1: int, i2: int) -> None:
-                    pass
-                def value(self) -> int:
-                    return self.val
-        assert 'invalid name' in str(exc_info.value).lower()
-
-        with pytest.raises(excs.Error) as exc_info:
             # reserved parameter name
             @pxt.uda(init_types=[IntType()], update_types=[IntType()], value_type=IntType())
             class WindowAgg:
                 def __init__(self, val: int = 0):
                     self.val = val
                 def update(self, order_by: int) -> None:
                     pass
```

### Comparing `pixeltable-0.2.4/pixeltable/tests/test_function.py` & `pixeltable-0.2.5/pixeltable/tests/test_function.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     return i
 
 class TestFunction:
     @pxt.udf(return_type=IntType(), param_types=[IntType()])
     def func(x: int) -> int:
         return x + 1
 
-    @pxt.uda(name='agg', value_type=IntType(), update_types=[IntType()])
-    class Aggregator:
+    @pxt.uda(value_type=IntType(), update_types=[IntType()])
+    class agg:
         def __init__(self):
             self.sum = 0
         def update(self, val: int) -> None:
             if val is not None:
                 self.sum += val
         def value(self) -> int:
             return self.sum
@@ -156,69 +156,70 @@
         func.FunctionRegistry.get().clear_cache()
         cl = pxt.Client(reload=True)
         t = cl.get_table('test')
         status = t.insert(rows)
         assert status.num_rows == len(rows)
         assert status.num_excs == 0
 
+    @pxt.udf(return_type=IntType(), param_types=[IntType(), FloatType(), FloatType(), FloatType()])
+    def f1(a: int, b: float, c: float = 0.0, d: float = 1.0) -> float:
+        return a + b + c + d
+
+    @pxt.udf(
+        return_type=IntType(),
+        param_types=[IntType(nullable=True), FloatType(nullable=False), FloatType(nullable=True)])
+    def f2(a: int, b: float = 0.0, c: float = 1.0) -> float:
+        return (0.0 if a is None else a) + b + (0.0 if c is None else c)
+
     def test_call(self, test_tbl: catalog.Table) -> None:
         t = test_tbl
 
-        @pxt.udf(return_type=IntType(), param_types=[IntType(), FloatType(), FloatType(), FloatType()])
-        def f1(a: int, b: float, c: float = 0.0, d: float = 1.0) -> float:
-            return a + b + c + d
-
         r0 = t[t.c2, t.c3].show(0).to_pandas()
         # positional params with default args
-        r1 = t[f1(t.c2, t.c3)].show(0).to_pandas()['col_0']
+        r1 = t[self.f1(t.c2, t.c3)].show(0).to_pandas()['col_0']
         assert np.all(r1 == r0.c2 + r0.c3 + 1.0)
         # kw args only
-        r2 = t[f1(c=0.0, b=t.c3, a=t.c2)].show(0).to_pandas()['col_0']
+        r2 = t[self.f1(c=0.0, b=t.c3, a=t.c2)].show(0).to_pandas()['col_0']
         assert np.all(r1 == r2)
         # overriding default args
-        r3 = t[f1(d=0.0, c=1.0, b=t.c3, a=t.c2)].show(0).to_pandas()['col_0']
+        r3 = t[self.f1(d=0.0, c=1.0, b=t.c3, a=t.c2)].show(0).to_pandas()['col_0']
         assert np.all(r2 == r3)
         # overriding default with positional arg
-        r4 = t[f1(t.c2, t.c3, 0.0)].show(0).to_pandas()['col_0']
+        r4 = t[self.f1(t.c2, t.c3, 0.0)].show(0).to_pandas()['col_0']
         assert np.all(r3 == r4)
         # overriding default with positional arg and kw arg
-        r5 = t[f1(t.c2, t.c3, 1.0, d=0.0)].show(0).to_pandas()['col_0']
+        r5 = t[self.f1(t.c2, t.c3, 1.0, d=0.0)].show(0).to_pandas()['col_0']
         assert np.all(r4 == r5)
         # d is kwarg
-        r6 = t[f1(t.c2, d=1.0, b=t.c3)].show(0).to_pandas()['col_0']
+        r6 = t[self.f1(t.c2, d=1.0, b=t.c3)].show(0).to_pandas()['col_0']
         assert np.all(r5 == r6)
         # d is Expr kwarg
-        r6 = t[f1(1, d=t.c3, b=t.c3)].show(0).to_pandas()['col_0']
+        r6 = t[self.f1(1, d=t.c3, b=t.c3)].show(0).to_pandas()['col_0']
         assert np.all(r5 == r6)
 
         # test handling of Nones
-        @pxt.udf(
-            return_type=IntType(),
-            param_types=[IntType(nullable=True), FloatType(nullable=False), FloatType(nullable=True)])
-        def f2(a: int, b: float = 0.0, c: float = 1.0) -> float:
-            return (0.0 if a is None else a) + b + (0.0 if c is None else c)
-        r0 = t[f2(1, t.c3)].show(0).to_pandas()['col_0']
-        r1 = t[f2(None, t.c3, 2.0)].show(0).to_pandas()['col_0']
+        r0 = t[self.f2(1, t.c3)].show(0).to_pandas()['col_0']
+        r1 = t[self.f2(None, t.c3, 2.0)].show(0).to_pandas()['col_0']
         assert np.all(r0 == r1)
-        r2 = t[f2(2, t.c3, None)].show(0).to_pandas()['col_0']
+        r2 = t[self.f2(2, t.c3, None)].show(0).to_pandas()['col_0']
         assert np.all(r1 == r2)
         # kwarg with None
-        r3 = t[f2(c=None, a=t.c2)].show(0).to_pandas()['col_0']
+        r3 = t[self.f2(c=None, a=t.c2)].show(0).to_pandas()['col_0']
         # kwarg with Expr
-        r4 = t[f2(c=t.c3, a=None)].show(0).to_pandas()['col_0']
+        r4 = t[self.f2(c=t.c3, a=None)].show(0).to_pandas()['col_0']
         assert np.all(r3 == r4)
 
         with pytest.raises(TypeError) as exc_info:
-            _ = t[f1(t.c2, c=0.0)].show(0)
+            _ = t[self.f1(t.c2, c=0.0)].show(0)
         assert "'b'" in str(exc_info.value)
         with pytest.raises(TypeError) as exc_info:
-            _ = t[f1(t.c2)].show(0)
+            _ = t[self.f1(t.c2)].show(0)
         assert "'b'" in str(exc_info.value)
         with pytest.raises(TypeError) as exc_info:
-            _ = t[f1(c=1.0, a=t.c2)].show(0)
+            _ = t[self.f1(c=1.0, a=t.c2)].show(0)
         assert "'b'" in str(exc_info.value)
 
         # bad default value
         with pytest.raises(excs.Error) as exc_info:
             @pxt.udf(return_type=IntType(), param_types=[IntType(), FloatType(), FloatType()])
             def f1(a: int, b: float, c: str = '') -> float:
                 return a + b + c
@@ -238,60 +239,67 @@
         # bad parameter name
         with pytest.raises(excs.Error) as exc_info:
             @pxt.udf(return_type=IntType(), param_types=[IntType()])
             def f1(order_by: int) -> int:
                 return order_by
         assert 'reserved' in str(exc_info.value)
 
+    @pxt.expr_udf
+    def add1(x: int) -> int:
+        return x + 1
+
+    @pxt.expr_udf
+    def add2(x: int, y: int):
+        return x + y
+
+    @pxt.expr_udf
+    def add2_with_default(x: int, y: int = 1) -> int:
+        return x + y
+
     def test_expr_udf(self, test_tbl: catalog.Table) -> None:
         t = test_tbl
-        @pxt.expr_udf
-        def times2(x: int) -> int:
-            return x + x
-        res1 = t.select(out=times2(t.c2)).order_by(t.c2).collect()
+
+        res1 = t.select(out=self.add1(t.c2)).order_by(t.c2).collect()
+        res2 = t.select(t.c2 + 1).order_by(t.c2).collect()
+        assert_resultset_eq(res1, res2)
+
+        # return type inferred from expression
+        res1 = t.select(out=self.add2(t.c2, t.c2)).order_by(t.c2).collect()
         res2 = t.select(t.c2 * 2).order_by(t.c2).collect()
         assert_resultset_eq(res1, res2)
 
         with pytest.raises(TypeError) as exc_info:
-            _ = t.select(times2(y=t.c2)).collect()
+            _ = t.select(self.add1(y=t.c2)).collect()
         assert 'missing a required argument' in str(exc_info.value).lower()
 
         with pytest.raises(excs.Error) as exc_info:
             # parameter types cannot be inferred
             @pxt.expr_udf
             def add1(x, y) -> int:
                 return x + y
         assert 'cannot infer pixeltable type' in str(exc_info.value).lower()
 
         with pytest.raises(excs.Error) as exc_info:
-            # return type cannot be inferred
-            @pxt.expr_udf
-            def add1(x: int, y: int):
-                return x + y
-        assert 'cannot infer pixeltable return type' in str(exc_info.value).lower()
-
-        with pytest.raises(excs.Error) as exc_info:
             # missing param types
             @pxt.expr_udf(param_types=[IntType()])
             def add1(x, y) -> int:
                 return x + y
         assert 'missing type for parameter y' in str(exc_info.value).lower()
 
         with pytest.raises(TypeError) as exc_info:
             # signature has correct parameter kind
             @pxt.expr_udf
             def add1(*, x: int) -> int:
-                return x + 1
+                return x + y
             _ = t.select(add1(t.c2)).collect()
         assert 'takes 0 positional arguments' in str(exc_info.value).lower()
 
-        @pxt.expr_udf
-        def add2(x: int, y: int = 1) -> int:
-            return x + y
-        res1 = t.select(out=add2(t.c2)).order_by(t.c2).collect()
+        res1 = t.select(out=self.add2_with_default(t.c2)).order_by(t.c2).collect()
+        res2 = t.select(out=self.add2(t.c2, 1)).order_by(t.c2).collect()
+        assert_resultset_eq(res1, res2)
 
     # Test that various invalid udf definitions generate
     # correct error messages.
     def test_invalid_udfs(self):
         with pytest.raises(excs.Error) as exc_info:
             @pxt.udf
             def udf1(name: Batch[str]) -> str:
```

### Comparing `pixeltable-0.2.4/pixeltable/tests/test_migration.py` & `pixeltable-0.2.5/pixeltable/tests/test_migration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import glob
 import logging
 import os
+import platform
 import subprocess
 
 import pgserver
 import pytest
 
 import pixeltable as pxt
 from pixeltable.env import Env
 from pixeltable.tests.conftest import clean_db
 
 _logger = logging.getLogger('pixeltable')
 
 
 class TestMigration:
 
-    @pytest.mark.skip(reason='Suspended')
+    @pytest.mark.skipif(platform.system() == 'Windows', reason='Does not run on Windows')
     def test_db_migration(self, init_env) -> None:
         env = Env.get()
         pg_package_dir = os.path.dirname(pgserver.__file__)
         pg_restore_binary = f'{pg_package_dir}/pginstall/bin/pg_restore'
         _logger.info(f'Using pg_restore binary at: {pg_restore_binary}')
         dump_files = glob.glob('pixeltable/tests/data/dbdumps/*.dump.gz')
         dump_files.sort()
```

### Comparing `pixeltable-0.2.4/pixeltable/tests/test_nos.py` & `pixeltable-0.2.5/pixeltable/tests/test_nos.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/tests/test_snapshot.py` & `pixeltable-0.2.5/pixeltable/tests/test_snapshot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict
 
 import numpy as np
 import pytest
 
 import pixeltable as pxt
 import pixeltable.exceptions as excs
-from pixeltable.tests.utils import create_test_tbl, assert_resultset_eq
+from pixeltable.tests.utils import create_test_tbl, assert_resultset_eq, create_img_tbl, img_embed
 from pixeltable.type_system import IntType
 
 
 class TestSnapshot:
     def run_basic_test(
             self, cl: pxt.Client, tbl: pxt.Table, snap: pxt.Table, extra_items: Dict[str, Any], filter: Any,
             reload_md: bool
@@ -85,14 +85,37 @@
                         'v2': {'value': lambda c3: c3 * 2.0, 'type': pxt.FloatType()}
                     } if has_cols else {}
                     extra_items = {'v1': tbl.c3 * 2.0, 'v2': tbl.c3 * 2.0} if has_cols else {}
                     filter = tbl.c2 < 10 if has_filter else None
                     snap = cl.create_view(snap_path, tbl, schema=schema, filter=filter, is_snapshot=True)
                     self.run_basic_test(cl, tbl, snap, extra_items=extra_items, filter=filter, reload_md=reload_md)
 
+    def test_errors(self, test_client: pxt.Client) -> None:
+        cl = test_client
+        tbl = create_test_tbl(client=cl)
+        snap = cl.create_view('snap', tbl, is_snapshot=True)
+
+        with pytest.raises(pxt.Error) as excinfo:
+            _ = snap.update({'c3': snap.c3 + 1.0})
+        assert 'cannot update a snapshot' in str(excinfo.value).lower()
+
+        with pytest.raises(pxt.Error) as excinfo:
+            _ = snap.batch_update([{'c3': 1.0, 'c2': 1}])
+        assert 'cannot update a snapshot' in str(excinfo.value).lower()
+
+        with pytest.raises(pxt.Error) as excinfo:
+            _ = snap.revert()
+        assert 'cannot revert a snapshot' in str(excinfo.value).lower()
+
+        with pytest.raises(pxt.Error) as excinfo:
+            img_tbl = create_img_tbl(cl)
+            snap = cl.create_view('img_snap', img_tbl, is_snapshot=True)
+            snap.add_embedding_index('img', img_embed=img_embed)
+        assert 'cannot add an index to a snapshot' in str(excinfo.value).lower()
+
     def test_views_of_snapshots(self, test_client: pxt.Client) -> None:
         cl = test_client
         t = cl.create_table('tbl', {'a': IntType()})
         rows = [{'a': 1}, {'a': 2}, {'a': 3}]
         status = t.insert(rows)
         assert status.num_rows == len(rows)
         assert status.num_excs == 0
```

### Comparing `pixeltable-0.2.4/pixeltable/tests/test_table.py` & `pixeltable-0.2.5/pixeltable/tests/test_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import pixeltable as pxt
 import pixeltable.functions as ptf
 from pixeltable import catalog
 from pixeltable import exceptions as excs
 from pixeltable.iterators import FrameIterator
 from pixeltable.tests.utils import \
     make_tbl, create_table_data, read_data_file, get_video_files, get_audio_files, get_image_files, get_documents, \
-    assert_resultset_eq, assert_hf_dataset_equal, make_test_arrow_table
+    assert_resultset_eq, assert_hf_dataset_equal, make_test_arrow_table, validate_update_status
 from pixeltable.tests.utils import skip_test_if_not_installed
 from pixeltable.type_system import \
     StringType, IntType, FloatType, TimestampType, ImageType, VideoType, JsonType, BoolType, ArrayType, AudioType, \
     DocumentType
 from pixeltable.utils.filecache import FileCache
 from pixeltable.utils.media_store import MediaStore
 
@@ -37,14 +37,29 @@
     def f2(a: float) -> float:
         return a + 1
 
     @pxt.expr_udf(param_types=[IntType(nullable=False)])
     def add1(a: int) -> int:
         return a + 1
 
+    @pxt.uda(
+        update_types=[IntType()], value_type=IntType(), requires_order_by=True,
+        allows_window=True)
+    class window_fn:
+        def __init__(self):
+            pass
+        def update(self, i: int) -> None:
+            pass
+        def value(self) -> int:
+            return 1
+
+    @pxt.expr_udf(param_types=[IntType(nullable=False)])
+    def add1(a: int) -> int:
+        return a + 1
+
     def test_create(self, test_client: pxt.Client) -> None:
         cl = test_client
         cl.create_dir('dir1')
         schema = {
             'c1': StringType(nullable=False),
             'c2': IntType(nullable=False),
             'c3': FloatType(nullable=False),
@@ -52,15 +67,15 @@
         }
         tbl = cl.create_table('test', schema)
         _ = cl.create_table('dir1.test', schema)
 
         with pytest.raises(excs.Error):
             _ = cl.create_table('1test', schema)
         with pytest.raises(excs.Error):
-            _ = catalog.Column('1c', StringType())
+            _ = cl.create_table('bad name', schema={'c1': StringType()})
         with pytest.raises(excs.Error):
             _ = cl.create_table('test', schema)
         with pytest.raises(excs.Error):
             _ = cl.create_table('dir2.test2', schema)
 
         _ = cl.list_tables()
         _ = cl.list_tables('dir1')
@@ -296,18 +311,14 @@
         assert '"type" is required' in str(exc_info.value)
 
         with pytest.raises(excs.Error) as exc_info:
             cl.create_table('test', {'c1': {'type': StringType(), 'stored': 'true'}})
         assert '"stored" must be a bool' in str(exc_info.value)
 
         with pytest.raises(excs.Error) as exc_info:
-            cl.create_table('test', {'c1': {'type': StringType(), 'indexed': 'true'}})
-        assert '"indexed" must be a bool' in str(exc_info.value)
-
-        with pytest.raises(excs.Error) as exc_info:
             cl.create_table('test', {'c1': StringType()}, primary_key='c2')
         assert 'primary key column c2 not found' in str(exc_info.value).lower()
 
         with pytest.raises(excs.Error) as exc_info:
             cl.create_table('test', {'c1': StringType()}, primary_key=['c1', 'c2'])
         assert 'primary key column c2 not found' in str(exc_info.value).lower()
 
@@ -497,26 +508,16 @@
         view = cl.create_view('test_view', tbl, iterator_class=FrameIterator, iterator_args=args)
         view.add_column(c1=view.frame.rotate(30), stored=True)
         view.add_column(c2=view.c1.rotate(40), stored=False)
         view.add_column(c3=view.c2.rotate(50), stored=True)
         # a non-materialized column that refers to another non-materialized column
         view.add_column(c4=view.c2.rotate(60), stored=False)
 
-        @pxt.uda(
-            name='window_fn', update_types=[IntType()], value_type=IntType(), requires_order_by = True,
-            allows_window = True)
-        class WindowFnAggregator:
-            def __init__(self):
-                pass
-            def update(self, i: int) -> None:
-                pass
-            def value(self) -> int:
-                return 1
         # cols computed with window functions are stored by default
-        view.add_column(c5=window_fn(view.frame_idx, 1, group_by=view.video))
+        view.add_column(c5=self.window_fn(view.frame_idx, 1, group_by=view.video))
 
         # reload to make sure that metadata gets restored correctly
         cl = pxt.Client(reload=True)
         tbl = cl.get_table('test_tbl')
         view = cl.get_table('test_view')
         # we're inserting only a single row and the video column is not in position 0
         url = 's3://multimedia-commons/data/videos/mp4/ffe/ff3/ffeff3c6bf57504e7a6cecaff6aefbc9.mp4'
@@ -549,14 +550,31 @@
         with pytest.raises(excs.Error) as exc_info:
             cl.drop_table('test_tbl')
         assert 'has dependents: test_view' in str(exc_info.value)
         cl.drop_table('test_view')
         cl.drop_table('test_tbl')
         assert MediaStore.count(view.get_id()) == 0
 
+    def test_insert_nulls(self, test_client: pxt.Client) -> None:
+        cl = test_client
+        schema = {
+            'c1': StringType(nullable=True),
+            'c2': IntType(nullable=True),
+            'c3': FloatType(nullable=True),
+            'c4': BoolType(nullable=True),
+            'c5': ArrayType((2, 3), dtype=IntType(), nullable=True),
+            'c6': JsonType(nullable=True),
+            'c7': ImageType(nullable=True),
+            'c8': VideoType(nullable=True),
+        }
+        t = cl.create_table('test1', schema)
+        status = t.insert(c1='abc')
+        assert status.num_rows == 1
+        assert status.num_excs == 0
+
     def test_insert(self, test_client: pxt.Client) -> None:
         cl = test_client
         schema = {
             'c1': StringType(nullable=False),
             'c2': IntType(nullable=False),
             'c3': FloatType(nullable=False),
             'c4': BoolType(nullable=False),
@@ -646,15 +664,71 @@
         _ = t.show(n=0)
 
         # test querying existing table
         cl = pxt.Client(reload=True)
         t2 = cl.get_table('test')
         _  = t2.show(n=0)
 
-    def test_update(self, test_tbl: pxt.Table, indexed_img_tbl: pxt.Table) -> None:
+    def test_batch_update(self, test_tbl: pxt.Table) -> None:
+        t = test_tbl
+        validate_update_status(
+            t.batch_update([{'c1': '1', 'c2': 1}, {'c1': '2', 'c2': 2}]),
+            expected_rows=2)
+        assert t.where(t.c2 == 1).collect()[0]['c1'] == '1'
+        assert t.where(t.c2 == 2).collect()[0]['c1'] == '2'
+        validate_update_status(
+            t.batch_update([{'c1': 'one', '_rowid': (1,)}, {'c1': 'two', '_rowid': (2,)}]),
+            expected_rows=2)
+        assert t.where(t.c2 == 1).collect()[0]['c1'] == 'one'
+        assert t.where(t.c2 == 2).collect()[0]['c1'] == 'two'
+
+        cl = pxt.Client()
+        # test composite primary key
+        schema = {'c1': StringType(), 'c2': IntType(), 'c3': FloatType()}
+        t = cl.create_table('composite', schema=schema, primary_key=['c1', 'c2'])
+        rows = [{'c1': str(i), 'c2': i, 'c3': float(i)} for i in range(10)]
+        validate_update_status(t.insert(rows), expected_rows=10)
+
+        validate_update_status(
+            t.batch_update([{'c1': '1', 'c2': 1, 'c3': 2.0}, {'c1': '2', 'c2': 2, 'c3': 3.0}]),
+            expected_rows=2)
+
+        with pytest.raises(excs.Error) as exc_info:
+            # can't mix _rowid with primary key
+            _ = t.batch_update([{'c1': '1', 'c2': 1, 'c3': 2.0, '_rowid': (1,)}])
+        assert 'c1 is a primary key column' in str(exc_info.value).lower()
+
+        with pytest.raises(excs.Error) as exc_info:
+            # bad literal
+            _ = t.batch_update([{'c2': 1, 'c3': 'a'}])
+        assert "'a' is not a valid literal" in str(exc_info.value).lower()
+
+        with pytest.raises(excs.Error) as exc_info:
+            # missing primary key column
+            t.batch_update([{'c1': '1', 'c3': 2.0}])
+        assert 'primary key columns (c2) missing' in str(exc_info.value).lower()
+
+        # table without primary key
+        t2 = cl.create_table('no_pk', schema=schema)
+        validate_update_status(t2.insert(rows), expected_rows=10)
+        with pytest.raises(excs.Error) as exc_info:
+            _ = t2.batch_update([{'c1': '1', 'c2': 1, 'c3': 2.0}])
+        assert 'must have primary key for batch update' in str(exc_info.value).lower()
+
+        # updating with _rowid still works
+        validate_update_status(
+            t2.batch_update([{'c1': 'one', '_rowid': (1,)}, {'c1': 'two', '_rowid': (2,)}]),
+            expected_rows=2)
+        assert t2.where(t2.c2 == 1).collect()[0]['c1'] == 'one'
+        assert t2.where(t2.c2 == 2).collect()[0]['c1'] == 'two'
+        with pytest.raises(AssertionError):
+            # some rows are missing rowids
+            _ = t2.batch_update([{'c1': 'one', '_rowid': (1,)}, {'c1': 'two'}])
+
+    def test_update(self, test_tbl: pxt.Table, small_img_tbl) -> None:
         t = test_tbl
         # update every type with a literal
         test_cases = [
             ('c1', 'new string'),
             # TODO: ('c1n', None),
             ('c3', -1.0),
             ('c4', True),
@@ -751,15 +825,15 @@
         assert 'not a recognized' in str(excinfo.value)
 
         # non-Predicate filter
         with pytest.raises(excs.Error) as excinfo:
             t.update({'c3': 1.0}, where=lambda c2: c2 == 10)
         assert 'Predicate' in str(excinfo.value)
 
-        img_t = indexed_img_tbl
+        img_t = small_img_tbl
 
         # can't update image col
         with pytest.raises(excs.Error) as excinfo:
             img_t.update({'img': 17}, where=img_t.img.nearest('car'))
         assert 'has type image' in str(excinfo.value)
 
         # similarity search is not supported
@@ -781,15 +855,15 @@
         # computed column that depends on two columns: exercise duplicate elimination during query construction
         t.add_column(d2=t.c3 - t.c10)
         r1 = t.where(t.c2 < 5).select(t.c3 + 1.0, t.c10 - 1.0, t.c3, 2.0).order_by(t.c2).show(0)
         t.update({'c4': True, 'c3': t.c3 + 1.0, 'c10': t.c10 - 1.0}, where=t.c2 < 5, cascade=True)
         r2 = t.where(t.c2 < 5).select(t.c3, t.c10, t.d1, t.d2).order_by(t.c2).show(0)
         assert_resultset_eq(r1, r2)
 
-    def test_delete(self, test_tbl: pxt.Table, indexed_img_tbl: pxt.Table) -> None:
+    def test_delete(self, test_tbl: pxt.Table, small_img_tbl) -> None:
         t = test_tbl
 
         cnt = t.where(t.c3 < 10.0).count()
         assert cnt == 10
         cnt = t.where(t.c3 == 10.0).count()
         assert cnt == 1
         status = t.delete(where=t.c3 < 10.0)
@@ -809,15 +883,15 @@
         assert cnt == 1
 
         # non-Predicate filter
         with pytest.raises(excs.Error) as excinfo:
             t.delete(where=lambda c2: c2 == 10)
         assert 'Predicate' in str(excinfo.value)
 
-        img_t = indexed_img_tbl
+        img_t = small_img_tbl
         # similarity search is not supported
         with pytest.raises(excs.Error) as excinfo:
             img_t.delete(where=img_t.img.nearest('car'))
         assert 'nearest()' in str(excinfo.value)
 
         # filter not expressible in SQL
         with pytest.raises(excs.Error) as excinfo:
@@ -975,14 +1049,18 @@
         res = t2.show(0)
         tbl_df = t2.show(0).to_pandas()
 
         # revert also removes computed images
         t2.revert()
         assert MediaStore.count(t2.get_id()) == t2.count() * stores_img_col
 
+    @pxt.udf(return_type=ImageType(), param_types=[ImageType()])
+    def img_fn_with_exc(img: PIL.Image.Image) -> PIL.Image.Image:
+        raise RuntimeError
+
     def test_computed_img_cols(self, test_client: pxt.Client) -> None:
         cl = test_client
         schema = {'img': ImageType(nullable=False)}
         t = cl.create_table('test', schema)
         t.add_column(c2=t.img.width)
         # c3 is not stored by default
         t.add_column(c3=t.img.rotate(90))
@@ -992,18 +1070,15 @@
         # c3 is now stored
         t.add_column(c3=t.img.rotate(90), stored=True)
         self._test_computed_img_cols(t, stores_img_col=True)
         _ = t[t.c3.errortype].show(0)
 
         # computed img col with exceptions
         t = cl.create_table('test3', schema)
-        @pxt.udf(return_type=ImageType(), param_types=[ImageType()])
-        def f(img: PIL.Image.Image) -> PIL.Image.Image:
-            raise RuntimeError
-        t.add_column(c3=f(t.img), stored=True)
+        t.add_column(c3=self.img_fn_with_exc(t.img), stored=True)
         rows = read_data_file('imagenette2-160', 'manifest.csv', ['img'])
         rows = [{'img': r['img']} for r in rows[:20]]
         t.insert(rows, fail_on_exception=False)
         _ = t[t.c3.errortype].show(0)
 
     def test_computed_window_fn(self, test_client: pxt.Client, test_tbl: catalog.Table) -> None:
         cl = test_client
@@ -1207,14 +1282,15 @@
 
         # make sure this is still true after reloading the metadata
         cl = pxt.Client(reload=True)
         t = cl.get_table(t.get_name())
         check_rename(t, 'c1_renamed', 'c1')
 
         # revert() works
+        _ = t.select(t.c1_renamed).collect()
         t.revert()
         _ = t.select(t.c1).collect()
         #check_rename(t, 'c1', 'c1_renamed')
 
         # make sure this is still true after reloading the metadata once more
         cl = pxt.Client(reload=True)
         t = cl.get_table(t.get_name())
```

### Comparing `pixeltable-0.2.4/pixeltable/tests/test_transactional_directory.py` & `pixeltable-0.2.5/pixeltable/tests/test_transactional_directory.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/tests/test_types.py` & `pixeltable-0.2.5/pixeltable/tests/test_types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+import datetime
+from copy import copy
+from typing import List, Dict, Optional
+
 from pixeltable.type_system import \
     ColumnType, StringType, IntType, BoolType, ImageType, InvalidType, FloatType, TimestampType, JsonType, ArrayType
 
 
 class TestTypes:
     def test_serialize(self, init_env) -> None:
         type_vals = [
@@ -16,7 +20,33 @@
             ArrayType((224, 224, 3), dtype=IntType()),
         ]
 
         for t in type_vals:
             t_serialized = t.serialize()
             t_deserialized = ColumnType.deserialize(t_serialized)
             assert t == t_deserialized
+
+    def test_from_python_type(self) -> None:
+        test_cases = {
+            str: StringType(),
+            int: IntType(),
+            float: FloatType(),
+            bool: BoolType(),
+            datetime.date: TimestampType(),
+            datetime.datetime: TimestampType(),
+            list: JsonType(),
+            dict: JsonType(),
+            list[int]: JsonType(),
+            list[dict[str, int]]: JsonType(),
+            dict[int, str]: JsonType(),
+            dict[dict[str, int], list[int]]: JsonType(),
+            List: JsonType(),
+            Dict: JsonType(),
+            List[int]: JsonType(),
+            List[Dict[str, int]]: JsonType(),
+            Dict[int, str]: JsonType()
+        }
+        for py_type, pxt_type in test_cases.items():
+            assert ColumnType.from_python_type(py_type) == pxt_type
+            opt_pxt_type = copy(pxt_type)
+            opt_pxt_type.nullable = True
+            assert ColumnType.from_python_type(Optional[py_type]) == opt_pxt_type
```

### Comparing `pixeltable-0.2.4/pixeltable/tests/test_video.py` & `pixeltable-0.2.5/pixeltable/tests/test_video.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,26 @@
         view_t.add_column(c3=view_t.c2.rotate(20))
         view_t.add_column(c4=view_t.c1.rotate(30))
         for name in ['c1', 'c2', 'c3', 'c4']:
             assert not view_t.tbl_version_path.tbl_version.cols_by_name[name].is_stored
         base_t.insert({'video': p} for p in video_filepaths)
         _ = view_t[view_t.c1, view_t.c2, view_t.c3, view_t.c4].show(0)
 
+    # window function that simply passes through the frame
+    @pxt.uda(
+        update_types=[ImageType()], value_type=ImageType(),
+        requires_order_by=True, allows_std_agg=False, allows_window=True)
+    class agg_fn:
+        def __init__(self):
+            self.img = None
+        def update(self, frame: PIL.Image.Image) -> None:
+            self.img = frame
+        def value(self) -> PIL.Image.Image:
+            return self.img
+
     def test_make_video(self, test_client: pxt.Client) -> None:
         video_filepaths = get_video_files()
         cl = test_client
         base_t, view_t = self.create_tbls(cl)
         base_t.insert({'video': p} for p in video_filepaths)
         # reference to the frame col requires ordering by base, pos
         from pixeltable.functions import make_video
@@ -127,33 +139,21 @@
             _ = view_t.select(make_video(view_t.frame, order_by=view_t.pos)).show()
         with pytest.raises(excs.Error):
             # incompatible ordering requirements
             _ = view_t.select(
                 make_video(view_t.pos, view_t.frame),
                 make_video(view_t.pos - 1, view_t.transformed)).group_by(base_t).show()
 
-        # window function that simply passes through the frame
-        @pxt.uda(
-            update_types=[ImageType()], value_type=ImageType(), name='agg_fn',
-            requires_order_by=True, allows_std_agg=False, allows_window=True)
-        class WindowAgg:
-            def __init__(self):
-                self.img = None
-            def update(self, frame: PIL.Image.Image) -> None:
-                self.img = frame
-            def value(self) -> PIL.Image.Image:
-                return self.img
-
         # make sure it works
-        _ = view_t.select(agg_fn(view_t.pos, view_t.frame, group_by=base_t)).show()
-        status = view_t.add_column(agg=agg_fn(view_t.pos, view_t.frame, group_by=base_t))
+        _ = view_t.select(self.agg_fn(view_t.pos, view_t.frame, group_by=base_t)).show()
+        status = view_t.add_column(agg=self.agg_fn(view_t.pos, view_t.frame, group_by=base_t))
         assert status.num_excs == 0
         _ = view_t.select(make_video(view_t.pos, view_t.agg)).group_by(base_t).show()
 
         # image cols computed with a window function currently need to be stored
         with pytest.raises(excs.Error):
-            view_t.add_column(agg2=agg_fn(view_t.pos, view_t.frame, group_by=base_t), stored=False)
+            view_t.add_column(agg2=self.agg_fn(view_t.pos, view_t.frame, group_by=base_t), stored=False)
 
         # reload from store
         cl = pxt.Client(reload=True)
         base_t, view_t = cl.get_table(base_t.get_name()), cl.get_table(view_t.get_name())
-        _ = view_t.select(agg_fn(view_t.pos, view_t.frame, group_by=base_t)).show()
+        _ = view_t.select(self.agg_fn(view_t.pos, view_t.frame, group_by=base_t)).show()
```

### Comparing `pixeltable-0.2.4/pixeltable/tests/test_view.py` & `pixeltable-0.2.5/pixeltable/tests/test_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import logging
 
 import PIL
 import pytest
 
 import pixeltable as pxt
 from pixeltable import catalog
@@ -410,14 +411,18 @@
         # base table delete is reflected in view
         t.delete(where=t.c2 < 5)
         assert t.count() == 110
         assert_resultset_eq(
             v.order_by(v.c2).show(0),
             t.where(t.c2 < 10).order_by(t.c2).show(0))
 
+        # create views with filters containing date and datetime
+        _ = cl.create_view('test_view_2', t, filter=t.c5 >= datetime.date.today())
+        _ = cl.create_view('test_view_3', t, filter=t.c5 < datetime.datetime.now())
+
     def test_view_of_snapshot(self, test_client: pxt.Client) -> None:
         """Test view over a snapshot"""
         cl = test_client
         t = self.create_tbl(cl)
         snap = cl.create_view('test_snap', t, is_snapshot=True)
 
         # create view with filter and computed columns
```

### Comparing `pixeltable-0.2.4/pixeltable/tests/utils.py` & `pixeltable-0.2.5/pixeltable/tests/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 import glob
 import json
 import os
 from collections import namedtuple
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Set
 
+import PIL.Image
 import numpy as np
 import pandas as pd
 import pytest
 
 import pixeltable as pxt
 import pixeltable.type_system as ts
 from pixeltable import catalog
 from pixeltable.catalog.globals import UpdateStatus
 from pixeltable.dataframe import DataFrameResultSet
 from pixeltable.env import Env
+from pixeltable.functions.huggingface import clip_image, clip_text
 from pixeltable.type_system import (
     ArrayType,
     BoolType,
     ColumnType,
     FloatType,
     ImageType,
     IntType,
@@ -39,23 +41,26 @@
         return FloatType()
     if t == ColumnType.Type.BOOL:
         return BoolType()
     if t == ColumnType.Type.TIMESTAMP:
         return TimestampType()
     assert False
 
+
 def make_tbl(cl: pxt.Client, name: str = 'test', col_names: Optional[List[str]] = None) -> catalog.InsertableTable:
     if col_names is None:
         col_names = ['c1']
     schema: Dict[str, ts.ColumnType] = {}
     for i, col_name in enumerate(col_names):
         schema[f'{col_name}'] = make_default_type(ColumnType.Type(i % 5))
     return cl.create_table(name, schema)
 
-def create_table_data(t: catalog.Table, col_names: Optional[List[str]] = None, num_rows: int = 10) -> List[Dict[str, Any]]:
+
+def create_table_data(t: catalog.Table, col_names: Optional[List[str]] = None, num_rows: int = 10) -> List[
+    Dict[str, Any]]:
     if col_names is None:
         col_names = []
     data: Dict[str, Any] = {}
 
     sample_dict = {
         'detections': [{
             'id': '637e8e073b28441a453564cf',
@@ -120,14 +125,15 @@
         if col_type.is_video_type():
             video_path = get_video_files()[0]
             col_data = [video_path for i in range(num_rows)]
         data[col_name] = col_data
     rows = [{col_name: data[col_name][i] for col_name in col_names} for i in range(num_rows)]
     return rows
 
+
 def create_test_tbl(client: pxt.Client, name: str = 'test_tbl') -> catalog.Table:
     schema = {
         'c1': StringType(nullable=False),
         'c1n': StringType(nullable=True),
         'c2': IntType(nullable=False),
         'c3': FloatType(nullable=False),
         'c4': BoolType(nullable=False),
@@ -185,93 +191,113 @@
             'c7': c7_data[i],
         }
         for i in range(num_rows)
     ]
     t.insert(rows)
     return t
 
+
+def create_img_tbl(cl: pxt.Client, name: str = 'test_img_tbl') -> catalog.Table:
+    schema = {
+        'img': ImageType(nullable=False),
+        'category': StringType(nullable=False),
+        'split': StringType(nullable=False),
+    }
+    tbl = cl.create_table(name, schema)
+    rows = read_data_file('imagenette2-160', 'manifest.csv', ['img'])
+    tbl.insert(rows)
+    return tbl
+
+
 def create_all_datatypes_tbl(test_client: pxt.Client) -> catalog.Table:
     """ Creates a table with all supported datatypes.
     """
     schema = {
-        'row_id': IntType(nullable=False), # used for row selection
-        'c_array': ArrayType(shape=(10,),  dtype=FloatType(), nullable=True),
+        'row_id': IntType(nullable=False),  # used for row selection
+        'c_array': ArrayType(shape=(10,), dtype=FloatType(), nullable=True),
         'c_bool': BoolType(nullable=True),
         'c_float': FloatType(nullable=True),
         'c_image': ImageType(nullable=True),
         'c_int': IntType(nullable=True),
         'c_json': JsonType(nullable=True),
         'c_string': StringType(nullable=True),
         'c_timestamp': TimestampType(nullable=True),
         'c_video': VideoType(nullable=True),
     }
     tbl = test_client.create_table('all_datatype_tbl', schema)
     example_rows = create_table_data(tbl, num_rows=11)
 
-    for i,r in enumerate(example_rows):
-        r['row_id'] = i # row_id
+    for i, r in enumerate(example_rows):
+        r['row_id'] = i  # row_id
 
     tbl.insert(example_rows)
     return tbl
 
+
 def read_data_file(dir_name: str, file_name: str, path_col_names: Optional[List[str]] = None) -> List[Dict[str, Any]]:
     """
     Locate dir_name, create df out of file_name.
     path_col_names: col names in csv file that contain file names; those will be converted to absolute paths
     by adding the path to 'file_name' as a prefix.
     Returns:
         tuple of (list of rows, list of column names)
     """
     if path_col_names is None:
         path_col_names = []
-    tests_dir = os.path.dirname(__file__) # search with respect to tests/ dir
+    tests_dir = os.path.dirname(__file__)  # search with respect to tests/ dir
     glob_result = glob.glob(f'{tests_dir}/**/{dir_name}', recursive=True)
     assert len(glob_result) == 1, f'Could not find {dir_name}'
     abs_path = Path(glob_result[0])
     data_file_path = abs_path / file_name
     assert data_file_path.is_file(), f'Not a file: {str(data_file_path)}'
     df = pd.read_csv(str(data_file_path))
     for col_name in path_col_names:
         assert col_name in df.columns
         df[col_name] = df.apply(lambda r: str(abs_path / r[col_name]), axis=1)
     return df.to_dict(orient='records')
 
+
 def get_video_files(include_bad_video: bool = False) -> List[str]:
-    tests_dir = os.path.dirname(__file__) # search with respect to tests/ dir
+    tests_dir = os.path.dirname(__file__)  # search with respect to tests/ dir
     glob_result = glob.glob(f'{tests_dir}/**/videos/*', recursive=True)
     if not include_bad_video:
         glob_result = [f for f in glob_result if 'bad_video' not in f]
 
     half_res = [f for f in glob_result if 'half_res' in f or 'bad_video' in f]
     return half_res
 
+
 def get_test_video_files() -> List[str]:
-    tests_dir = os.path.dirname(__file__) # search with respect to tests/ dir
+    tests_dir = os.path.dirname(__file__)  # search with respect to tests/ dir
     glob_result = glob.glob(f'{tests_dir}/**/test_videos/*', recursive=True)
     return glob_result
 
+
 def get_image_files(include_bad_image: bool = False) -> List[str]:
-    tests_dir = os.path.dirname(__file__) # search with respect to tests/ dir
+    tests_dir = os.path.dirname(__file__)  # search with respect to tests/ dir
     glob_result = glob.glob(f'{tests_dir}/**/imagenette2-160/*', recursive=True)
     if not include_bad_image:
         glob_result = [f for f in glob_result if 'bad_image' not in f]
     return glob_result
 
+
 def get_audio_files(include_bad_audio: bool = False) -> List[str]:
     tests_dir = os.path.dirname(__file__)
     glob_result = glob.glob(f'{tests_dir}/**/audio/*', recursive=True)
     if not include_bad_audio:
         glob_result = [f for f in glob_result if 'bad_audio' not in f]
     return glob_result
 
+
 def get_documents() -> List[str]:
     tests_dir = os.path.dirname(__file__)
     # for now, we can only handle .html and .md
     return [p for p in glob.glob(f'{tests_dir}/**/documents/*', recursive=True) if not p.endswith('.pdf')]
 
+
 def get_sentences(n: int = 100) -> List[str]:
     tests_dir = os.path.dirname(__file__)
     path = glob.glob(f'{tests_dir}/**/jeopardy.json', recursive=True)[0]
     with open(path, 'r', encoding='utf8') as f:
         questions_list = json.load(f)
     # this dataset contains \' around the questions
     return [q['question'].replace("'", '') for q in questions_list[:n]]
@@ -399,10 +425,18 @@
                 value = tuple([float(x) for x in value])
 
             encoded_tup[column_name] = value
 
         check_tup = DatasetTuple(**encoded_tup)
         assert check_tup in acc_dataset
 
+@pxt.expr_udf
+def img_embed(img: PIL.Image.Image) -> np.ndarray:
+    return clip_image(img, model_id='openai/clip-vit-base-patch32')
+
+@pxt.expr_udf
+def text_embed(txt: str) -> np.ndarray:
+    return clip_text(txt, model_id='openai/clip-vit-base-patch32')
 
 SAMPLE_IMAGE_URL = \
     'https://raw.githubusercontent.com/pixeltable/pixeltable/master/docs/source/data/images/000000000009.jpg'
+
```

### Comparing `pixeltable-0.2.4/pixeltable/tool/create_test_db_dump.py` & `pixeltable-0.2.5/pixeltable/tool/create_test_db_dump.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,14 +132,30 @@
                 'c5': c5_data[i],
                 'c6': c6_data[i],
                 'c7': c7_data[i],
             }
             for i in range(num_rows)
         ]
         t.insert(rows)
+        self.cl.create_dir('views')
+        v = self.cl.create_view('views.sample_view', t, filter=(t.c2 < 50))
+        _ = self.cl.create_view('views.sample_snapshot', t, filter=(t.c2 >= 75), is_snapshot=True)
+        # Computed column using a library function
+        v['str_format'] = pxt.functions.string.str_format('{0} {key}', t.c1, key=t.c1)
+        # Computed column using a bespoke udf
+        v['test_udf'] = test_udf(t.c2)
+        # astype
+        v['astype'] = t.c1.astype(pxt.FloatType())
+        # computed column using a stored function
+        v['stored'] = t.c1.apply(lambda x: f'Hello, {x}', col_type=pxt.StringType())
+
+
+@pxt.udf
+def test_udf(n: int) -> int:
+    return n + 1
 
 
 def main() -> None:
     _logger.info("Creating pixeltable test artifact.")
     dumper = Dumper()
     dumper.create_tables()
     dumper.dump_db()
```

### Comparing `pixeltable-0.2.4/pixeltable/tool/create_test_video.py` & `pixeltable-0.2.5/pixeltable/tool/create_test_video.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/type_system.py` & `pixeltable-0.2.5/pixeltable/type_system.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import abc
 import datetime
 import enum
 import json
 import typing
 import urllib.parse
+import urllib.request
+from copy import copy
 from pathlib import Path
 from typing import Any, Optional, Tuple, Dict, Callable, List, Union, Sequence, Mapping
 
 import PIL.Image
 import av
 import numpy as np
 import sqlalchemy as sql
@@ -289,15 +291,15 @@
 
     def _validate_file_path(self, val: Any) -> None:
         """Raises TypeError if not a valid local file path or not a path/byte sequence"""
         if isinstance(val, str):
             parsed = urllib.parse.urlparse(val)
             if parsed.scheme != '' and parsed.scheme != 'file':
                 return
-            path = Path(urllib.parse.unquote(parsed.path))
+            path = Path(urllib.parse.unquote(urllib.request.url2pathname(parsed.path)))
             if not path.is_file():
                 raise TypeError(f'File not found: {str(path)}')
         else:
             if not isinstance(val, bytes):
                 raise TypeError(f'expected file path or bytes, got {type(val)}')
 
     @abc.abstractmethod
@@ -372,38 +374,19 @@
     def to_sql(self) -> str:
         """
         Return corresponding Postgres type.
         """
         pass
 
     @abc.abstractmethod
-    def to_sa_type(self) -> Any:
+    def to_sa_type(self) -> sql.types.TypeEngine:
         """
         Return corresponding SQLAlchemy type.
-        return type Any: there doesn't appear to be a superclass for the sqlalchemy types
         """
-        assert self._type != self.Type.INVALID
-        if self._type == self.Type.STRING:
-            return sql.String
-        if self._type == self.Type.INT:
-            return sql.Integer
-        if self._type == self.Type.FLOAT:
-            return sql.Float
-        if self._type == self.Type.BOOL:
-            return sql.Boolean
-        if self._type == self.Type.TIMESTAMP:
-            return sql.TIMESTAMP
-        if self._type == self.Type.IMAGE:
-            # the URL
-            return sql.String
-        if self._type == self.Type.JSON:
-            return sql.dialects.postgresql.JSONB
-        if self._type == self.Type.ARRAY:
-            return sql.VARBINARY
-        assert False
+        pass
 
     @staticmethod
     def no_conversion(v: Any) -> Any:
         """
         Special return value of conversion_fn() that indicates that no conversion is necessary.
         Should not be called
         """
@@ -420,23 +403,24 @@
 class InvalidType(ColumnType):
     def __init__(self, nullable: bool = False):
         super().__init__(self.Type.INVALID, nullable=nullable)
 
     def to_sql(self) -> str:
         assert False
 
-    def to_sa_type(self) -> Any:
+    def to_sa_type(self) -> sql.types.TypeEngine:
         assert False
 
     def print_value(self, val: Any) -> str:
         assert False
 
     def _validate_literal(self, val: Any) -> None:
         assert False
 
+
 class StringType(ColumnType):
     def __init__(self, nullable: bool = False):
         super().__init__(self.Type.STRING, nullable=nullable)
 
     def conversion_fn(self, target: ColumnType) -> Optional[Callable[[Any], Any]]:
         if not target.is_timestamp_type():
             return None
@@ -447,16 +431,16 @@
             except ValueError:
                 return None
         return convert
 
     def to_sql(self) -> str:
         return 'VARCHAR'
 
-    def to_sa_type(self) -> str:
-        return sql.String
+    def to_sa_type(self) -> sql.types.TypeEngine:
+        return sql.String()
 
     def print_value(self, val: Any) -> str:
         return f"'{val}'"
 
     def _validate_literal(self, val: Any) -> None:
         if not isinstance(val, str):
             raise TypeError(f'Expected string, got {val.__class__.__name__}')
@@ -465,86 +449,90 @@
         # Replace null byte within python string with space to avoid issues with Postgres.
         # Use a space to avoid merging words.
         # TODO(orm): this will also be an issue with JSON inputs, would space still be a good replacement?
         if isinstance(val, str) and '\x00' in val:
             return val.replace('\x00', ' ')
         return val
 
+
 class IntType(ColumnType):
     def __init__(self, nullable: bool = False):
         super().__init__(self.Type.INT, nullable=nullable)
 
     def to_sql(self) -> str:
         return 'BIGINT'
 
-    def to_sa_type(self) -> str:
-        return sql.BigInteger
+    def to_sa_type(self) -> sql.types.TypeEngine:
+        return sql.BigInteger()
 
     def _validate_literal(self, val: Any) -> None:
         if not isinstance(val, int):
             raise TypeError(f'Expected int, got {val.__class__.__name__}')
 
 
 class FloatType(ColumnType):
     def __init__(self, nullable: bool = False):
         super().__init__(self.Type.FLOAT, nullable=nullable)
 
     def to_sql(self) -> str:
         return 'FLOAT'
 
-    def to_sa_type(self) -> str:
-        return sql.Float
+    def to_sa_type(self) -> sql.types.TypeEngine:
+        return sql.Float()
 
     def _validate_literal(self, val: Any) -> None:
         if not isinstance(val, float):
             raise TypeError(f'Expected float, got {val.__class__.__name__}')
 
     def _create_literal(self, val: Any) -> Any:
         if isinstance(val, int):
             return float(val)
         return val
 
+
 class BoolType(ColumnType):
     def __init__(self, nullable: bool = False):
         super().__init__(self.Type.BOOL, nullable=nullable)
 
     def to_sql(self) -> str:
         return 'BOOLEAN'
 
-    def to_sa_type(self) -> str:
-        return sql.Boolean
+    def to_sa_type(self) -> sql.types.TypeEngine:
+        return sql.Boolean()
 
     def _validate_literal(self, val: Any) -> None:
         if not isinstance(val, bool):
             raise TypeError(f'Expected bool, got {val.__class__.__name__}')
 
     def _create_literal(self, val: Any) -> Any:
         if isinstance(val, int):
             return bool(val)
         return val
 
+
 class TimestampType(ColumnType):
     def __init__(self, nullable: bool = False):
         super().__init__(self.Type.TIMESTAMP, nullable=nullable)
 
     def to_sql(self) -> str:
         return 'INTEGER'
 
-    def to_sa_type(self) -> str:
-        return sql.TIMESTAMP
+    def to_sa_type(self) -> sql.types.TypeEngine:
+        return sql.TIMESTAMP()
 
     def _validate_literal(self, val: Any) -> None:
         if not isinstance(val, datetime.datetime) and not isinstance(val, datetime.date):
             raise TypeError(f'Expected datetime.datetime or datetime.date, got {val.__class__.__name__}')
 
     def _create_literal(self, val: Any) -> Any:
         if isinstance(val, str):
             return datetime.datetime.fromisoformat(val)
         return val
 
+
 class JsonType(ColumnType):
     # TODO: type_spec also needs to be able to express lists
     def __init__(self, type_spec: Optional[Dict[str, ColumnType]] = None, nullable: bool = False):
         super().__init__(self.Type.JSON, nullable=nullable)
         self.type_spec = type_spec
 
     def _as_dict(self) -> Dict:
@@ -562,16 +550,16 @@
                 field_name: cls.deserialize(field_type_dict) for field_name, field_type_dict in d['type_spec'].items()
             }
         return cls(type_spec, nullable=d['nullable'])
 
     def to_sql(self) -> str:
         return 'JSONB'
 
-    def to_sa_type(self) -> str:
-        return sql.dialects.postgresql.JSONB
+    def to_sa_type(self) -> sql.types.TypeEngine:
+        return sql.dialects.postgresql.JSONB()
 
     def print_value(self, val: Any) -> str:
         val_type = self.infer_literal_type(val)
         if val_type == self:
             return str(val)
         return val_type.print_value(val)
 
@@ -584,14 +572,15 @@
             raise TypeError(f'Expected JSON-serializable object, got {val}')
 
     def _create_literal(self, val: Any) -> Any:
         if isinstance(val, tuple):
             val = list(val)
         return val
 
+
 class ArrayType(ColumnType):
     def __init__(
             self, shape: Tuple[Union[int, None], ...], dtype: ColumnType, nullable: bool = False):
         super().__init__(self.Type.ARRAY, nullable=nullable)
         self.shape = shape
         assert dtype.is_int_type() or dtype.is_float_type() or dtype.is_bool_type() or dtype.is_string_type()
         self.dtype = dtype._type
@@ -667,16 +656,16 @@
             # declared for this type, rather than assume float64
             return np.array(val, dtype=self.numpy_dtype())
         return val
 
     def to_sql(self) -> str:
         return 'BYTEA'
 
-    def to_sa_type(self) -> str:
-        return sql.LargeBinary
+    def to_sa_type(self) -> sql.types.TypeEngine:
+        return sql.LargeBinary()
 
     def numpy_dtype(self) -> np.dtype:
         if self.dtype == self.Type.INT:
             return np.dtype(np.int64)
         if self.dtype == self.Type.FLOAT:
             return np.dtype(np.float32)
         if self.dtype == self.Type.BOOL:
@@ -772,39 +761,40 @@
                 img = img.convert(target.mode.to_pil())
             return img
         return convert
 
     def to_sql(self) -> str:
         return 'VARCHAR'
 
-    def to_sa_type(self) -> str:
-        return sql.String
+    def to_sa_type(self) -> sql.types.TypeEngine:
+        return sql.String()
 
     def _validate_literal(self, val: Any) -> None:
         if isinstance(val, PIL.Image.Image):
             return
         self._validate_file_path(val)
 
     def validate_media(self, val: Any) -> None:
         assert isinstance(val, str)
         try:
             _ = PIL.Image.open(val)
         except PIL.UnidentifiedImageError:
             raise excs.Error(f'Not a valid image: {val}') from None
 
+
 class VideoType(ColumnType):
     def __init__(self, nullable: bool = False):
         super().__init__(self.Type.VIDEO, nullable=nullable)
 
     def to_sql(self) -> str:
         # stored as a file path
         return 'VARCHAR'
 
-    def to_sa_type(self) -> str:
-        return sql.String
+    def to_sa_type(self) -> sql.types.TypeEngine:
+        return sql.String()
 
     def _validate_literal(self, val: Any) -> None:
         self._validate_file_path(val)
 
     def validate_media(self, val: Any) -> None:
         assert isinstance(val, str)
         try:
@@ -821,24 +811,25 @@
                         break
                 if num_decoded < 2:
                     # this is most likely an image file
                     raise excs.Error(f'Not a valid video: {val}')
         except av.AVError:
             raise excs.Error(f'Not a valid video: {val}') from None
 
+
 class AudioType(ColumnType):
     def __init__(self, nullable: bool = False):
         super().__init__(self.Type.AUDIO, nullable=nullable)
 
     def to_sql(self) -> str:
         # stored as a file path
         return 'VARCHAR'
 
-    def to_sa_type(self) -> str:
-        return sql.String
+    def to_sa_type(self) -> sql.types.TypeEngine:
+        return sql.String()
 
     def _validate_literal(self, val: Any) -> None:
         self._validate_file_path(val)
 
     def validate_media(self, val: Any) -> None:
         try:
             with av.open(val) as container:
@@ -850,14 +841,15 @@
                 # TODO: is there some way to verify it's a playable audio file other than decoding all of it?
                 for packet in container.demux(audio_stream):
                     for _ in packet.decode():
                         pass
         except av.AVError as e:
             raise excs.Error(f'Not a valid audio file: {val}\n{e}') from None
 
+
 class DocumentType(ColumnType):
     @enum.unique
     class DocumentFormat(enum.Enum):
         HTML = 0
         MD = 1
         PDF = 2
 
@@ -872,16 +864,16 @@
         else:
             self._doc_formats = [t for t in self.DocumentFormat]
 
     def to_sql(self) -> str:
         # stored as a file path
         return 'VARCHAR'
 
-    def to_sa_type(self) -> str:
-        return sql.String
+    def to_sa_type(self) -> sql.types.TypeEngine:
+        return sql.String()
 
     def _validate_literal(self, val: Any) -> None:
         self._validate_file_path(val)
 
     def validate_media(self, val: Any) -> None:
         assert isinstance(val, str)
         from pixeltable.utils.documents import get_document_handle
```

### Comparing `pixeltable-0.2.4/pixeltable/utils/arrow.py` & `pixeltable-0.2.5/pixeltable/utils/arrow.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/utils/clip.py` & `pixeltable-0.2.5/pixeltable/utils/clip.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/utils/coco.py` & `pixeltable-0.2.5/pixeltable/utils/coco.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/utils/documents.py` & `pixeltable-0.2.5/pixeltable/utils/documents.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/utils/filecache.py` & `pixeltable-0.2.5/pixeltable/utils/filecache.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/utils/hf_datasets.py` & `pixeltable-0.2.5/pixeltable/utils/hf_datasets.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/utils/media_store.py` & `pixeltable-0.2.5/pixeltable/utils/media_store.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/utils/parquet.py` & `pixeltable-0.2.5/pixeltable/utils/parquet.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/utils/pytorch.py` & `pixeltable-0.2.5/pixeltable/utils/pytorch.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/utils/sql.py` & `pixeltable-0.2.5/pixeltable/utils/sql.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pixeltable/utils/transactional_directory.py` & `pixeltable-0.2.5/pixeltable/utils/transactional_directory.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.4/pyproject.toml` & `pixeltable-0.2.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pixeltable"
-version = "0.2.4"
+version = "0.2.5"
 description = "Pixeltable: The Multimodal AI Data Plane"
 authors = ["Marcel Kornacker <marcelk@gmail.com>"]
 readme = "README.md"
 exclude = [
     ".pytype",
     ".pytest_cache",
     "pixeltable/.pytest_cache",
@@ -32,15 +32,15 @@
 pgvector = "^0.2.1"
 av = ">=10.0.0"
 beautifulsoup4 = "^4.0.0"
 requests = "^2.31.0"
 pyyaml = "^6.0.1"
 jinja2 = "^3.1.3"
 tenacity = "^8.2"
-pgserver = "0.1.0"
+pgserver = "0.1.2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 # pytest-related
 pytest = "^7.2.1"
@@ -105,14 +105,20 @@
 # R0801: Similar lines in 2 files
 # R0902: Too many instance attributes
 # R0913: Too many arguments
 # R0914: Too many local variables
 # W0511: TODO
 disable = ["C0114","C0116","C0415","E1121","R0401","R0801","R0902","R0913","R0914","W0511"]
 
+[tool.pytest.ini_options]
+addopts = "-v -m \"not remote_api\""
+markers = [
+    "remote_api: marks tests as calling a remote API (such as OpenAI)"
+]
+
 [tool.ruff]
 line-length = 120
 
 [tool.ruff.lint]
 select = ["F", "E", "W", "C", "I", "N", "B", "A", "ICN", "PYI", "SIM", "TD002", "PL", "RUF"]
 ignore = ["PLC0415", "PLR0904", "PLR0912", "PLR0913", "PLR0914", "PLR0915", "PLR2004"]
 preview = true
```

### Comparing `pixeltable-0.2.4/PKG-INFO` & `pixeltable-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixeltable
-Version: 0.2.4
+Version: 0.2.5
 Summary: Pixeltable: The Multimodal AI Data Plane
 Author: Marcel Kornacker
 Author-email: marcelk@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,15 +14,15 @@
 Requires-Dist: beautifulsoup4 (>=4.0.0,<5.0.0)
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
 Requires-Dist: numpy (>=1.26)
 Requires-Dist: opencv-python-headless (>=4.7.0.68,<5.0.0.0)
 Requires-Dist: pandas (>=2.0,<3.0)
-Requires-Dist: pgserver (==0.1.0)
+Requires-Dist: pgserver (==0.1.2)
 Requires-Dist: pgvector (>=0.2.1,<0.3.0)
 Requires-Dist: pillow (>=10.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: regex (>=2022.10.31,<2023.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
@@ -56,19 +56,20 @@
 
 ## ⚡Quick Start
 Learn the basics of Pixeltable through interactive examples. View the notebooks on Google Colab or Kaggle, for free.
 
 ### Pixeltable Basics
 In this tutorial, we'll survey how to create tables, populate them with data, and enhance them with built-in and user-defined transformations and AI operations.
 
-[![Open in Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/code/brunep/pixeltable-basics) <a target="_blank" href="https://colab.research.google.com/github/pixeltable/pixeltable/blob/master/docs/tutorials/pixeltable-basics.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>
+[![Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://kaggle.com/kernels/welcome?src=https://github.com/pixeltable/pixeltable/blob/master/docs/tutorials/pixeltable-basics.ipynb)&nbsp;&nbsp;
+<a target="_blank" href="https://colab.research.google.com/github/pixeltable/pixeltable/blob/master/docs/tutorials/pixeltable-basics.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>
 
 
 ## 💾 Installation
-Pixeltable works with Python 3.9, 3.10, or 3.11 running on Linux or MacOS.
+Pixeltable works with Python 3.9, 3.10, 3.11, or 3.12 running on Linux, MacOS, or Windows.
 
 ```
 pip install pixeltable
 ```
 
 To verify that it's working:
```

