# Comparing `tmp/xbrl_filings_api-1.0.0.dev1.tar.gz` & `tmp/xbrl_filings_api-1.0a1.tar.gz`

## Comparing `xbrl_filings_api-1.0.0.dev1.tar` & `xbrl_filings_api-1.0a1.tar`

### file list

```diff
@@ -1,39 +1,89 @@
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/examples.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/tests/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/__about__.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/__init__.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/__main__.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/api_request.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/constants.py
--rw-r--r--   0        0        0     8997 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/database_processor.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/debug.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/download_item.py
--rw-r--r--   0        0        0     8252 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/download_processor.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/enums.py
--rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/exceptions.py
--rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/filings_api.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/lang_code_transform.py
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/options.py
--rw-r--r--   0        0        0    10118 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/request_processor.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/save_paths.py
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/sqlite_views.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/time_formats.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/api_object/__init__.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/api_object/api_error.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/api_object/api_object.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/api_object/api_page.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/api_object/api_resource.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/api_object/entity.py
--rw-r--r--   0        0        0    21795 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/api_object/filing.py
--rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/api_object/filings_page.py
--rw-r--r--   0        0        0     9616 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/api_object/json_tree.py
--rw-r--r--   0        0        0     9447 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/api_object/validation_message.py
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/data_export/data_utils.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/filing_set/__init__.py
--rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/filing_set/filing_set.py
--rw-r--r--   0        0        0     4363 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/filing_set/resource_collection.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/.gitignore
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/LICENSE.txt
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/README.md
--rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/ruff.toml
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/__init__.py
+-rw-r--r--   0        0        0    19804 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/conftest.py
+-rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/conftest_source.py
+-rw-r--r--   0        0        0    38020 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/mock_upgrade.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/urlmock.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/integration/__init__.py
+-rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/integration/test_pandas_data.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/__init__.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_api_error.py
+-rw-r--r--   0        0        0     8340 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_api_page.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_api_resource.py
+-rw-r--r--   0        0        0     8362 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_debug.py
+-rw-r--r--   0        0        0    22670 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_default_views_sql.py
+-rw-r--r--   0        0        0    42478 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_downloading.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_entity.py
+-rw-r--r--   0        0        0    24579 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_filing.py
+-rw-r--r--   0        0        0    29838 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_filing_set.py
+-rw-r--r--   0        0        0    52691 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_filing_set_mutableset.py
+-rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_filings_page.py
+-rw-r--r--   0        0        0     5540 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_general.py
+-rw-r--r--   0        0        0    16741 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_json_tree.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_main.py
+-rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_options_views.py
+-rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_pandas_data_unit.py
+-rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_query.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_query_add_api_params.py
+-rw-r--r--   0        0        0    11289 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_query_filters_multifilters.py
+-rw-r--r--   0        0        0    10865 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_query_filters_short_dates.py
+-rw-r--r--   0        0        0    21513 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_query_filters_single.py
+-rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_query_filters_unsupported.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_query_flags.py
+-rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_query_paging_single.py
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_query_sort.py
+-rw-r--r--   0        0        0     7758 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_resource_collection.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_source_data_bugs.py
+-rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_stats.py
+-rw-r--r--   0        0        0    15788 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/test_validation_message.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/downloader/__init__.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/downloader/conftest.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/downloader/test_download.py
+-rw-r--r--   0        0        0    10607 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/downloader/test_download_async.py
+-rw-r--r--   0        0        0    11101 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/downloader/test_download_parallel.py
+-rw-r--r--   0        0        0    14647 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/downloader/test_download_parallel_aiter.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/downloader/test_downloader_stats.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/tests/unit/downloader/test_validate_stem_pattern.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/__about__.py
+-rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/__init__.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/__main__.py
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/api_error.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/api_object.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/api_page.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/api_request.py
+-rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/api_resource.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/constants.py
+-rw-r--r--   0        0        0     9313 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/database_processor.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/debug.py
+-rw-r--r--   0        0        0     9833 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/default_views.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/download_info.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/download_item.py
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/download_specs_construct.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/entity.py
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/exceptions.py
+-rw-r--r--   0        0        0    31925 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/filing.py
+-rw-r--r--   0        0        0    46052 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/filing_set.py
+-rw-r--r--   0        0        0     8203 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/filings_page.py
+-rw-r--r--   0        0        0    11422 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/json_tree.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/lang_code_transform.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/options.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/order_columns.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/parse_type.py
+-rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/query.py
+-rw-r--r--   0        0        0    21073 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/request_processor.py
+-rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/resource_collection.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/scope_flag.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/sqlite_view.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/stats.py
+-rw-r--r--   0        0        0    11328 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/validation_message.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/downloader/__init__.py
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/downloader/download_processor.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/downloader/download_result.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/downloader/download_specs.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/downloader/exceptions.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/xbrl_filings_api/downloader/stats.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/.gitignore
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/LICENSE.txt
+-rw-r--r--   0        0        0     8536 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/README.md
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/pyproject.toml
+-rw-r--r--   0        0        0    10239 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0a1/PKG-INFO
```

### Comparing `xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/database_processor.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/database_processor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,288 +1,298 @@
-"""
-Module for processing SQLite3 databases.
+"""Module for processing SQLite3 databases."""
 
-"""
-
-# SPDX-FileCopyrightText: 2023-present Lauri Salmela <lauri.m.salmela@gmail.com>
+# SPDX-FileCopyrightText: 2023 Lauri Salmela <lauri.m.salmela@gmail.com>
 #
 # SPDX-License-Identifier: MIT
 
+# Double quotes are used in all SQL strings by default.
+# ruff: noqa: Q000
+
+from __future__ import annotations
+
+import errno
+import logging
+import os
+import sqlite3
+from collections.abc import Collection, Sequence
 from datetime import datetime
 from pathlib import Path
-from collections.abc import Generator, Iterable
-import sqlite3
+from typing import Optional
+
+from xbrl_filings_api import options, order_columns
+from xbrl_filings_api.api_resource import APIResource
+from xbrl_filings_api.constants import DataAttributeType
+from xbrl_filings_api.entity import Entity
+from xbrl_filings_api.exceptions import DatabaseSchemaUnmatchError
+from xbrl_filings_api.filing import Filing
+from xbrl_filings_api.scope_flag import ScopeFlag
+from xbrl_filings_api.validation_message import ValidationMessage
+
+__all__ = ['sets_to_sqlite']
 
-from .api_object.api_resource import APIResource
-from .api_object.entity import Entity
-from .api_object.filing import Filing
-from .api_object.filings_page import FilingsPage
-from .api_object.validation_message import ValidationMessage
-from .enums import (
-    ScopeFlag, GET_ONLY_FILINGS, GET_ENTITY, GET_VALIDATION_MESSAGES)
-from .exceptions import (
-    DatabaseFileExistsError, DatabasePathIsReservedError,
-    DatabaseSchemaUnmatch
-    )
-from .time_formats import time_formats
-import xbrl_filings_api.data_export.data_utils as data_utils
-import xbrl_filings_api.options as options
+logger = logging.getLogger(__name__)
 
-CurrentSchemaType = dict[str, list[str]]
+_CurrentSchemaType = dict[str, list[str]]
 """`{'TableName': ['col1', 'col2', ...]}`"""
 
 
 def sets_to_sqlite(
         flags: ScopeFlag,
-        ppath: Path,
-        update: bool,
-        data_objs: dict[str, Iterable[APIResource]],
+        db_path: Path,
+        data_objs: dict[str, Collection[APIResource]],
+        *,
+        update: bool
         ) -> None:
     """
     Save sets to SQLite3 database.
 
     Raises
     ------
-    DatabaseFileExistsError
-    DatabasePathIsReservedError
-    DatabaseSchemaUnmatch
+    FileExistsError
+    DatabaseSchemaUnmatchError
     sqlite3.DatabaseError
     """
-    _validate_path(update, ppath)
-    filing_data_attrs = data_utils.get_data_attributes(
-        Filing, flags, data_objs['Filing'])
+    _validate_path(db_path, update=update)
+    _validate_views()
+    filing_data_attrs = Filing.get_data_attributes(
+        flags, data_objs['Filing'])
     con, table_schema = _create_database_or_extend_schema(
-        flags, ppath, update, filing_data_attrs)
+        flags, db_path, filing_data_attrs, update=update)
     _insert_data(table_schema, data_objs, con)
     con.close()
 
 
-def pages_to_sqlite(
-        flags: ScopeFlag,
-        ppath: Path,
-        update: bool,
-        page_gen: Generator[FilingsPage, None, None],
-        ) -> None:
+def _validate_path(db_path: Path, *, update: bool) -> None:
     """
-    Save API pages to SQLite3 database.
+    Validate path by raising expections.
 
     Raises
     ------
-    DatabaseFileExistsError
-    DatabasePathIsReservedError
-    DatabaseSchemaUnmatch
-    sqlite3.DatabaseError
+    FileExistsError
+        When file exists in path and `update` is :pt:`False`.
     """
-    _validate_path(update, ppath)
-    filing_data_attrs = data_utils.get_data_attributes(Filing, flags)
-    con, table_schema = _create_database_or_extend_schema(
-        flags, ppath, update, filing_data_attrs)
+    if db_path.is_file():
+        if not update:
+            raise FileExistsError(
+                errno.EEXIST,
+                os.strerror(errno.EEXIST),
+                str(db_path)
+                )
 
-    for page in page_gen:
-        entities = []
-        messages = []
-        for filing in page.filing_list:
-            if filing.entity:
-                entities.append(filing.entity)
-            if filing.validation_messages:
-                messages.extend(filing.validation_messages)
-        data_objs = {
-            'Filing': page.filing_list,
-            'Entity': entities,
-            'ValidationMessage': messages
-            }
-        _insert_data(table_schema, data_objs, con)
-    con.close()
 
+def _validate_views():
+    used = set()
+    if options.views:
+        for view in options.views:
+            if view.name in used:
+                msg = (
+                    f'Multiple views in options.views with name "{view.name}"')
+                raise ValueError(msg)
+            used.add(view.name)
 
-def _validate_path(update: bool, ppath: Path) -> None:
-    """
-    When file exists in path, raise if ``update=False`` and raise if
-    path is reserved.
 
-    Raises
-    ------
-    DatabaseFileExistsError
-    DatabasePathIsReservedError
+def _create_database_or_extend_schema(
+        flags: ScopeFlag,
+        db_path: Path,
+        filing_data_attrs: list[str],
+        *,
+        update: bool
+        ) -> tuple[sqlite3.Connection, _CurrentSchemaType]:
     """
-    if ppath.is_file():
-        if not update:
-            raise DatabaseFileExistsError(str(ppath))
-    elif ppath.exists():
-        raise DatabasePathIsReservedError(str(ppath))
+    Create a new SQLite3 database or extend the database schema.
 
+    When ``update`` is :pt:`True`, any of the tables in existing
+    database must match required tables and all of these matching tables
+    must have a column ``api_id``.
 
-def _create_database_or_extend_schema(
-        flags: ScopeFlag, db_path: Path, update: bool,
-        filing_data_attrs: list[str]
-        ) -> tuple[sqlite3.Connection, CurrentSchemaType]:
-    """
-    Creates an SQLite3 database or extends the tables and columns of
-    an existing database.
-    
     Returns
     -------
-    tuple of sqlite3.Connection, CurrentSchemaType
-        ``(con, table_schema)``.
+    sqlite3.Connection
+    CurrentSchemaType
 
     Raises
     ------
-    DatabaseSchemaUnmatch
+    DatabaseSchemaUnmatchError
     sqlite3.DatabaseError
     """
     resource_types: list[type[APIResource]] = [Filing]
     data_attrs = {'Filing': filing_data_attrs}
-    if GET_ONLY_FILINGS not in flags:
-        if GET_ENTITY in flags:
+    if ScopeFlag.GET_ONLY_FILINGS not in flags:
+        if ScopeFlag.GET_ENTITY in flags:
             resource_types.append(Entity)
-            data_attrs['Entity'] = data_utils.get_data_attributes(Entity)
-        if GET_VALIDATION_MESSAGES in flags:
+            data_attrs['Entity'] = Entity.get_data_attributes()
+        if ScopeFlag.GET_VALIDATION_MESSAGES in flags:
             resource_types.append(ValidationMessage)
             data_attrs['ValidationMessage'] = (
-                data_utils.get_data_attributes(ValidationMessage))
-    
+                ValidationMessage.get_data_attributes())
+
     db_path.parent.mkdir(parents=True, exist_ok=True)
 
     connection = sqlite3.connect(db_path)
     cur = connection.cursor()
-    table_names = {cls.__name__ for cls in resource_types}
-    existing_tables: set[str] = {}
-    existing_views: set[str] = {}
+    required_table_names = {cls.__name__ for cls in resource_types}
+    existing_tables: set[str] = set()
+    existing_views: set[str] = set()
 
     if update:
-        schema_match = False
         _exec(
             cur,
             "SELECT type, name FROM sqlite_schema "
             "WHERE name NOT LIKE 'sqlite_%'"
             )
         db_objs = cur.fetchall()
         existing_tables = {row[1] for row in db_objs if row[0] == 'table'}
         existing_views = {row[1] for row in db_objs if row[0] == 'view'}
-        for table_name in existing_tables:
-            if table_name in table_names:
+        schema_match = False
+        for existing_table in existing_tables:
+            if existing_table in required_table_names:
                 schema_match = True
                 break
         if not schema_match:
             path = str(db_path)
-            raise DatabaseSchemaUnmatch(path)
+            raise DatabaseSchemaUnmatchError(path)
 
-    table_schema: CurrentSchemaType = dict()
+    table_schema: _CurrentSchemaType = {}
     for type_obj in resource_types:
         table_name = type_obj.__name__
-        cols = data_attrs[table_name]
-        
-        col_defs = _get_col_defs(cols)
+        required_columns = data_attrs[table_name]
+
+        col_defs = _get_col_defs(required_columns)
         table_schema[table_name] = [cd[0] for cd in col_defs]
 
         if table_name in existing_tables:
-            schema_match = False
-            _exec(
-                cur,
-                f"SELECT name FROM pragma_table_info('{table_name}')"
-                )
-            existing_cols = [row[0] for row in cur.fetchall()]
-            add_cols = []
-            for col in cols:
-                try:
-                    existing_cols.index(col)
-                except ValueError:
-                    add_cols.append(col)
-                else:
-                    schema_match = True
-            if not schema_match or 'api_id' not in cols:
+            existing_cols = _get_existing_column_names(table_name, cur)
+            if 'api_id' not in existing_cols:
                 path = str(db_path)
-                raise DatabaseSchemaUnmatch(path)
-            for col, tc in _get_col_defs(add_cols):
-                _exec(
-                    cur,
-                    f"ALTER TABLE {table_name} ADD COLUMN {col} {tc}"
-                    )
-                table_schema[table_name].append(col)
-            connection.commit()
-            continue
+                raise DatabaseSchemaUnmatchError(path)
+            _add_missing_required_columns(
+                table_name, cur, required_columns, existing_cols)
+        else:
+            _create_new_table(table_name, cur, col_defs)
+        connection.commit()
 
+    if options.views:
+        _add_compatible_views(cur, existing_views, table_schema)
+        connection.commit()
+    return connection, table_schema
+
+
+def _add_missing_required_columns(
+        table_name: str, cur: sqlite3.Cursor, required_columns: list[str],
+        existing_cols: set[str]):
+    add_cols = []
+    for col in required_columns:
+        if col not in existing_cols:
+            add_cols.append(col)
+    add_cols = order_columns.order_columns(add_cols)
+    for cname, ctype in _get_col_defs(add_cols):
         _exec(
             cur,
-            f"CREATE TABLE {table_name} (\n  "
-            + ",\n  ".join((' '.join(cd) for cd in col_defs))
-            + "\n) WITHOUT ROWID"
+            f"ALTER TABLE {table_name} ADD COLUMN {cname} {ctype}"
             )
-        connection.commit()
-    
-    if options.views:
-        for view_name, (required_tables, view_sql) in options.views.items():
-            if view_name in existing_views:
-                continue
-            for table_name in required_tables:
-                if table_name not in table_schema:
-                    continue
-            _exec(
-                cur,
-                f"CREATE VIEW {view_name}\n"
-                "AS" + view_sql.rstrip()
-                )
-            connection.commit()
-    return connection, table_schema
 
 
-def _get_col_defs(cols: list[str]) -> list[tuple[int, str, str]]:
-    """Get list of (order, col_name, type_const)."""
-    cols = data_utils.order_columns(cols)
+def _create_new_table(
+        table_name: str, cur: sqlite3.Cursor, col_defs: list[tuple[str, str]]):
+    _exec(
+        cur,
+        f"CREATE TABLE {table_name} (\n  "
+        + ",\n  ".join(f'{cname} {ctype}' for cname, ctype in col_defs)
+        + "\n) WITHOUT ROWID"
+        )
+
+
+def _add_compatible_views(
+        cur: sqlite3.Cursor, existing_views: set[str],
+        table_schema: _CurrentSchemaType):
+    if options.views is None:
+        return
+    for view in options.views:
+        if view.name in existing_views:
+            continue
+        if not set(view.required_tables).issubset(set(table_schema)):
+            continue
+        _exec(
+            cur,
+            f"CREATE VIEW {view.name}\n"
+            "AS" + view.sql.rstrip()
+            )
+
+
+def _get_existing_column_names(
+        table_name: str, cur: sqlite3.Cursor) -> set[str]:
+    _exec(
+        cur,
+        "SELECT name FROM pragma_table_info(?)",
+        (table_name,))
+    return set(*zip(*cur.fetchall()))
+
+
+def _get_col_defs(cols: list[str]) -> list[tuple[str, str]]:
+    """Get list of (col_name, type_const)."""
+    cols = order_columns.order_columns(cols)
     col_defs = []
     for col in cols:
         type_const = 'TEXT'
         if col.endswith('_count'):
             type_const = 'INTEGER'
         elif col.endswith('_sum') or col.startswith('duplicate_'):
             type_const = 'REAL'
         if col == 'api_id':
             type_const += ' PRIMARY KEY NOT NULL'
         col_defs.append((col, type_const))
     return col_defs
 
 
 def _insert_data(
-        table_schema: CurrentSchemaType,
-        data_objs: dict[Iterable[APIResource]],
+        table_schema: _CurrentSchemaType,
+        data_objs: dict[str, Collection[APIResource]],
         con: sqlite3.Connection):
     cur = con.cursor()
     for table_name in table_schema:
         cols = table_schema[table_name]
-        records = [
-            [getattr(item, col) for col in cols]
-            for item in data_objs[table_name]
-            ]
+        records: list[tuple[DataAttributeType, ...]] = []
+        logger.debug(f'Got {len(data_objs[table_name])} of {table_name}')
+        for item in data_objs[table_name]:
+            col_data = []
+            for col in cols:
+                if col.endswith('_time') and col != 'query_time':
+                    col_data.append(getattr(item, f'{col}_str'))
+                else:
+                    col_data.append(getattr(item, col))
+            records.append(tuple(col_data))
         colsql = '\n  ' + ',\n  '.join(cols) + '\n  '
         phs = ', '.join(['?'] * len(cols))
         _exec(
             cur,
             f"REPLACE INTO {table_name} ({colsql})\nVALUES ({phs})",
-            records
+            many=records
             )
         con.commit()
 
 
-def _exec(cur: sqlite3.Cursor, sql: str, data: list[list[str]] = None) -> None:
-    data_len = f' <count: {len(data)}>' if data else ''
-    print(sql + ';' + data_len)
+def _exec(
+        cur: sqlite3.Cursor,
+        sql: str,
+        params: Sequence[str] = (),
+        *,
+        many: Optional[Collection[Sequence[DataAttributeType]]] = None
+        ) -> None:
+    data_len = f' <count: {len(many)}>' if many else ''
+    logger.debug(sql + ';' + data_len)
 
-    if data:
-        cur.executemany(sql, data)
+    if many is not None:
+        cur.executemany(sql, many)
     else:
-        cur.execute(sql)
+        cur.execute(sql, params)
 
 
-def adapt_datetime(dt: datetime):
-    try:
-        fstr = time_formats[options.time_accuracy]
-    except KeyError:
-        fstr = time_formats['min']
-    return dt.strftime(fstr)
+def _adapt_datetime(dt: datetime):
+    return dt.strftime('%Y-%m-%d %H:%M:%S.%f')
 
 
-def adapt_list(list_in: list):
+def _adapt_list(list_in: list):
     return '\n'.join(list_in)
 
 
-sqlite3.register_adapter(datetime, adapt_datetime)
-sqlite3.register_adapter(list, adapt_list)
+sqlite3.register_adapter(datetime, _adapt_datetime)
+sqlite3.register_adapter(list, _adapt_list)
```

### Comparing `xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/download_processor.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/downloader/download_processor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,268 +1,326 @@
-"""
-Define download functions.
+"""Define sequential and parallel download functions."""
 
-"""
-
-# SPDX-FileCopyrightText: 2023-present Lauri Salmela <lauri.m.salmela@gmail.com>
+# SPDX-FileCopyrightText: 2023 Lauri Salmela <lauri.m.salmela@gmail.com>
 #
 # SPDX-License-Identifier: MIT
 
-from collections.abc import Awaitable, AsyncIterator, Coroutine
-from pathlib import PurePath, Path
-from typing import Any, Optional, Never
 import asyncio
 import hashlib
 import urllib.parse
+from collections.abc import AsyncIterator
+from pathlib import Path, PurePath
+from typing import Optional, Union
 
 import requests
 
-from .download_item import FullDownloadItem
-from .exceptions import CorruptDownloadError
-
-
-item_counter = 0
-byte_counter = 0
+from xbrl_filings_api.downloader import stats
+from xbrl_filings_api.downloader.download_result import DownloadResult
+from xbrl_filings_api.downloader.download_specs import DownloadSpecs
+from xbrl_filings_api.downloader.exceptions import CorruptDownloadError
+
+__all__ = [
+    'download',
+    'download_async',
+    'download_parallel',
+    'download_parallel_aiter',
+    'validate_stem_pattern',
+    ]
 
 
 def download(
         url: str,
-        to_dir: str | PurePath,
+        to_dir: Union[str, PurePath],
+        *,
         stem_pattern: Optional[str] = None,
         filename: Optional[str] = None,
-        sha256: Optional[str] = None
+        sha256: Optional[str] = None,
+        timeout: float = 30.0
         ) -> str:
     """
-    Download a file and optionally check if it is corrupt.
+    Download a file synchronously.
 
     See documentation of `download_async`.
     """
     return asyncio.run(download_async(
-        url, to_dir, stem_pattern, filename, sha256))
+        url, to_dir,
+        stem_pattern=stem_pattern, filename=filename, sha256=sha256,
+        timeout=timeout
+        ))
 
 
 async def download_async(
         url: str,
-        to_dir: str | PurePath,
+        to_dir: Union[str, PurePath],
+        *,
         stem_pattern: Optional[str] = None,
         filename: Optional[str] = None,
-        sha256: Optional[str] = None
+        sha256: Optional[str] = None,
+        timeout: float = 30.0
         ) -> str:
     """
-    Download a file and optionally check if it is corrupt.
+    Download a file asynchronously.
 
-    The directories in `to_dir` will be created if they do not exist. If
-    no `filename` is given, name is derived from `url`. If file already
-    exists, it will be overwritten.
-
-    If the `sha256` does not match with the hash of the downloaded file,
-    `CorruptDownloadError` will be raised and the name of the downloaded
-    file will be appended with ``.corrupt``.
+    The directories in parameter ``to_dir`` will be created if they do
+    not exist. If no ``filename`` is given, name is derived from
+    parameter ``url``. If file already exists, it will be overwritten.
+
+    If the ``sha256`` does not match with the checksum of the downloaded
+    file,
+    :exc:`xbrl_filings_api.downloader.exceptions.CorruptDownloadError`
+    will be raised and the name of the downloaded file will be appended
+    with ``".corrupt"``.
 
     If download is interrupted, the file will be left with a suffix
-    ``.unfinished``.
-    
-    If no name could be derived from `url`, the file will be named
+    ``".unfinished"``.
+
+    If no name could be derived from ``url``, the file will be named
     ``file0001``, ``file0002``, etc. In this case a new file is always
     created.
-    
+
     Parameters
     ----------
     url : str
         URL to download.
-    to_dir : str or pathlike
+    to_dir : path-like
         Directory to save the file.
     stem_pattern : str, optional
-        Pattern to add to the filename stems. Placeholder ``/name/``
+        Pattern to add to the filename stems. Placeholder ``"/name/"``
         is always required.
     filename : str, optional
         Name to be used for the saved file.
     sha256 : str, optional
-        Expected SHA-256 hash as a hex string. Case-insensitive. No
-        hash is calculated if this parameter is not given.
-    
+        Expected SHA-256 checksum as a hex string. Case-insensitive. No
+        checksum is calculated if this parameter is not given.
+    timeout : float, default 30.0
+        Maximum timeout for getting an initial response from the server
+        in seconds.
+
     Returns
     -------
-    coroutine of str
+    str
         Local path where the downloaded file was saved.
 
     Raises
     ------
-    CorruptDownloadError
-        Parameter `sha256` does not match the calculated hash.
+    xbrl_filings_api.downloader.exceptions.CorruptDownloadError
+        Attribute `Filing.package_sha256` does not match the calculated
+        hash of package file.
     requests.HTTPError
         HTTP status error occurs.
     requests.ConnectionError
         Connection fails.
     """
-    global item_counter, byte_counter
-
     validate_stem_pattern(stem_pattern)
     if not isinstance(to_dir, Path):
         to_dir = Path(to_dir)
     to_dir.mkdir(parents=True, exist_ok=True)
 
     if not filename:
         uqurl = urllib.parse.unquote(url)
         filename = urllib.parse.urlparse(uqurl).path.split('/')[-1]
         if filename.strip() == '':
             num = 1
             while (to_dir / f'file{num:04}').is_file():
                 num += 1
             filename = f'file{num:04}'
 
-    res = requests.get(url, stream=True)
-    item_counter += 1
+    res = requests.get(url, stream=True, timeout=timeout)
     res.raise_for_status()
 
-    hash = None
+    hash_ = None
     if sha256:
-        hash = hashlib.sha256()
-    
+        hash_ = hashlib.sha256()
+
     if stem_pattern:
         fnpath = Path(filename)
         filename = stem_pattern.replace('/name/', fnpath.stem) + fnpath.suffix
-    
+
     save_path = Path.cwd() / to_dir / filename
     temp_path = save_path.with_suffix(f'{save_path.suffix}.unfinished')
     with open(temp_path, 'wb') as fd:
         for chunk in res.iter_content(chunk_size=None):
             fd.write(chunk)
-            if hash:
-                hash.update(chunk)
-            byte_counter += len(chunk)
+            if sha256 and hash_:
+                hash_.update(chunk)
+            stats.byte_counter += len(chunk)
             await asyncio.sleep(0.0)
-    
-    if hash:
-        sha256: str
-        if hash.digest() != bytes.fromhex(sha256):
+    stats.item_counter += 1
+
+    if sha256 and hash_:
+        if hash_.digest() != bytes.fromhex(sha256):
             corrupt_path = save_path.with_suffix(f'{save_path.suffix}.corrupt')
             corrupt_path.unlink(missing_ok=True)
             path = str(temp_path.rename(corrupt_path))
-            
-            calculated = hash.hexdigest().lower()
+
+            calculated = hash_.hexdigest().lower()
             expected = sha256.lower()
             raise CorruptDownloadError(path, url, calculated, expected)
-    
+
     save_path.unlink(missing_ok=True)
     temp_path.rename(save_path)
     return str(save_path)
 
 
 def download_parallel(
-        items: list[FullDownloadItem], max_concurrent: int
-        ) -> list[tuple[Any, str | Exception]]:
+        items: list[DownloadSpecs],
+        *,
+        max_concurrent: Union[int, None] = None,
+        timeout: float = 30.0
+        ) -> list[DownloadResult]:
     """
     Download multiple files in parallel.
-    
-    See documentation of `download_parallel_async_iter`.
 
-    Parameters
-    ----------
-    items : list of FullDownloadItem
-    max_concurrent : int
+    The order in parameter ``items`` is not guaranteed on the returned
+    list.
 
-    Returns
-    -------
-    list of tuple of (any, {str, Exception})
-        List of `download_parallel_async_iter` yield values.
-    """
-    return asyncio.run(download_parallel_async(items, max_concurrent))
-
-
-async def download_parallel_async(
-        items: list[FullDownloadItem], max_concurrent: int
-        ) -> list[tuple[Any, str | Exception]]:
-    """
-    Download multiple files in parallel.
-    
-    See documentation of `download_parallel_async_iter`.
+    See documentation of `download_parallel_aiter`.
 
     Parameters
     ----------
-    items : list of FullDownloadItem
-    max_concurrent : int
+    items : list of DownloadSpecs
+    max_concurrent : int or None, default None
+    timeout : float, default 30.0
 
     Returns
     -------
-    coroutine of list of tuple of (any, {str, Exception})
-        List of `download_parallel_async_iter` yield values.
+    list of DownloadResult
+        Contains information on the finished download.
     """
-    results = []
-    async for item in download_parallel_async_iter(
-            items, max_concurrent):
-        results.append(item)
-    return results
+    async def _download_parallel_async(
+            items: list[DownloadSpecs],
+            max_concurrent: Union[int, None],
+            timeout: float
+            ) -> list[DownloadResult]:
+        results = []
+        dliter = download_parallel_aiter(
+            items,
+            max_concurrent=max_concurrent,
+            timeout=timeout
+            )
+        async for item in dliter:
+            results.append(item)
+        return results
+    return asyncio.run(
+        _download_parallel_async(items, max_concurrent, timeout))
 
 
-async def download_parallel_async_iter(
-        items: list[FullDownloadItem], max_concurrent: int
-        ) -> AsyncIterator[tuple[Any, str | Exception]]:
+async def download_parallel_aiter(
+        items: list[DownloadSpecs],
+        *,
+        max_concurrent: Union[int, None] = None,
+        timeout: float = 30.0
+        ) -> AsyncIterator[DownloadResult]:
     """
-    Download multiple files in parallel and return an asynchronous
-    iterator.
+    Download multiple files in parallel, return asynchronous iterator.
+
+    The ordering in parameter ``items`` defines the order in which the
+    requests will be started. As the downloads take arbitrary periods of
+    time to finish, it does not guarantee the same order in the yielded
+    results. For this purpose, an additional any-typed attribute
+    ``info`` of both `DownloadSpecs` and `DownloadResult` is provided to
+    keep track of individual downloads.
+
+    Yielded `DownloadResult` objects will not have the
+    :attr:`~DownloadResult.path` attribute value when the ``sha256``
+    check fails even though the file is in fact saved with filename
+    suffix ``".corrupt"``.
+
+    Calls function `download_async` via parameter ``items``.
 
-    Calls method `download_async` via parameter `items`, see
-    documentation.
-    
     Parameters
     ----------
-    items : list of FullDownloadItem
-        Instances of `FullDownloadItem` accept the same parameters as
-        method `download_async` with additional parameters `obj` and
-        `attr_base`.
-    max_concurrent : int
-        Maximum number of simultaneous downloads allowed.
-    
+    items : list of DownloadSpecs
+        Instances of `DownloadSpecs` accept the same parameters as
+        function `download_async` with an additional no-op attribute
+        :attr:`~DownloadSpecs.info`.
+    max_concurrent : int or None, default None
+        Maximum number of simultaneous downloads allowed at any moment.
+        If :pt:`None`, all downloads will be started immediately. If
+        ``1``, downloading will be sequential.
+    timeout : float, default 30.0
+        Maximum timeout for getting the initial response for a single
+        download from the server in seconds.
+
     Yields
     ------
-    tuple of (any, str, {str, exception})
-        First part is `obj` attribute from `items` item, the second is
-        file format and the last is a save path or exception.
+    DownloadResult
+        Contains information on the finished download.
     """
-    dlque: asyncio.Queue[FullDownloadItem] = asyncio.Queue()
+    itemlen = len(items)
+    if max_concurrent is None:
+        max_concurrent = itemlen
+    else:
+        max_concurrent = min(max_concurrent, itemlen)
+
+    dlque: asyncio.Queue[Union[DownloadSpecs, None]] = asyncio.Queue()
     for item in items:
         dlque.put_nowait(item)
-    
-    resultque: asyncio.Queue[tuple[Any, str, Exception | str]] = (
-        asyncio.Queue())
-    tasks: list[asyncio.Task] = []
-    for worker_num in range(1, min(max_concurrent, len(items)) + 1):
+    # Termination markers for each worker
+    for _ in range(max_concurrent):
+        dlque.put_nowait(None)
+
+    resultque: asyncio.Queue[DownloadResult] = asyncio.Queue()
+
+    tasks: set[asyncio.Task] = set()
+    for worker_num in range(1, max_concurrent + 1):
         task = asyncio.create_task(
-            _download_parallel_worker(dlque, resultque),
+            _download_parallel_worker(dlque, resultque, timeout),
             name=f'worker-{worker_num}'
             )
-        tasks.append(task)
-    
-    for _ in range(len(items)):
+        tasks.add(task)
+
+    for _ in range(itemlen):
         result = await resultque.get()
         yield result
-    
-    for task in tasks:
-        task.cancel()
-    await asyncio.gather(*tasks, return_exceptions=True)
 
 
 async def _download_parallel_worker(
-        dlque: asyncio.Queue, resultque: asyncio.Queue) -> Never:
-    """Coroutine worker for `download_parallel_async_iter`."""
+        dlque: asyncio.Queue[Union[DownloadSpecs, None]],
+        resultque: asyncio.Queue[DownloadResult],
+        timeout: float
+        ) -> None:
+    """Coroutine worker for `download_parallel_aiter`."""
     while True:
-        item: FullDownloadItem = await dlque.get()
+        item: Union[DownloadSpecs, None] = await dlque.get()
+        if item is None:
+            break
+        result = None
         try:
             path = await download_async(
-                item.url, item.to_dir, item.stem_pattern, item.filename,
-                item.sha256
+                item.url,
+                item.to_dir,
+                stem_pattern=item.stem_pattern,
+                filename=item.filename,
+                sha256=item.sha256,
+                timeout=timeout
                 )
         except Exception as err:
-            resultque.put_nowait((item.obj, item.attr_base, err))
+            result = DownloadResult(
+                url=item.url, err=err, info=item.info)
         else:
-            resultque.put_nowait((item.obj, item.attr_base, path))
+            result = DownloadResult(
+                url=item.url, path=path, info=item.info)
+        resultque.put_nowait(result)
         dlque.task_done()
 
 
-def validate_stem_pattern(stem_pattern: str | None):
+def validate_stem_pattern(stem_pattern: Union[str, None]):
+    """
+    Validate parameter ``stem_pattern`` of module functions.
+
+    Parameters
+    ----------
+    stem_pattern : str or None
+        Stem pattern parameter.
+
+    Raises
+    ------
+    ValueError
+        When stem pattern is invalid.
+    """
     if stem_pattern and '/name/' not in stem_pattern:
         msg = (
-            "Placeholder '/name/' missing in 'stem_pattern' value "
+            'Placeholder "/name/" missing in \'stem_pattern\' value '
             + repr(stem_pattern)
             )
         raise ValueError(msg)
```

### Comparing `xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/exceptions.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,158 +1,134 @@
 """
 The exceptions for the library.
 
-Exception `APIError` is defined separately in module
-`api_object.api_error`.
+All the exceptions are accessible through the package root namespace.
 
-All of the exceptions are subclasses of `FilingsAPIError,
-`FilingsAPIErrorGroup` or `FilingsAPIWarning`. This includes `APIError`.
+All of the exceptions are subclasses of :class:`FilingsAPIError` or
+:class:`FilingsAPIWarning`. This includes :class:`APIError`.
+
+Exception :class:`APIError` is defined separately in module
+:mod:`api_error` due to also being a subclass of :class:`APIObject`.
 
 """
 
-# SPDX-FileCopyrightText: 2023-present Lauri Salmela <lauri.m.salmela@gmail.com>
+# SPDX-FileCopyrightText: 2023 Lauri Salmela <lauri.m.salmela@gmail.com>
 #
 # SPDX-License-Identifier: MIT
 
+__all__ = [
+    'FilingsAPIError',
+    'FilingsAPIWarning',
+    'CorruptDownloadError',
+    'DatabaseSchemaUnmatchError',
+    'HTTPStatusError',
+    'JSONAPIFormatError',
+    'FilterNotSupportedWarning',
+    ]
+
 
 class FilingsAPIError(Exception):
-    """
+    r"""
     Base class for exceptions in this library.
-    
+
     Not to be confused with `APIError` which is a subclass of this class
     representing an error returned by JSON:API.
     """
 
-
-class FilingsAPIErrorGroup(ExceptionGroup):
-    """Base class for exception groups in this library."""
+    def __str__(self) -> str:
+        """
+        Return "[<``msg``>] [list of <attr>=<value>]".
+
+        Placeholder ``attr`` refers to any own attribute of the
+        exception instance except ``msg`` or ``body``. Placeholder
+        ``value`` is always in :func:`repr` format. The attribute
+        ``body``, has a different display form: ``len(body)=<len>``.
+        """
+        parts = []
+        msg = getattr(self, 'msg', None)
+        if msg:
+            parts.append(msg)
+        attrlist = []
+        for attr_name in dir(self):
+            if not (attr_name == 'msg'
+                    or attr_name.startswith('_')
+                    or getattr(Exception, attr_name, False)):
+                val = getattr(self, attr_name)
+                if attr_name != 'body':
+                    attrlist.append(f'{attr_name}={val!r}')
+                else:
+                    attrlist.append(f'len(body)={len(val)}')
+        attrstr = ', '.join(attrlist)
+        if attrstr:
+            parts.append(attrstr)
+        return ' '.join(parts)
 
 
-class FilingsAPIWarning(Warning):
+class FilingsAPIWarning(UserWarning):
     """Base class for warnings in this library."""
 
 
-class HTTPStatusError(FilingsAPIError):
-    """
-    The API returns no errors and the HTTP status is other than 200.
-
-    Attributes
-    ----------
-    status_code : int
-    status_text : str
-    body : str
-    """
-
-    def __init__(self, status_code: int, status_text: str, body: str) -> None:
-        """Initialize `HTTPStatusError`."""
-        self.status_code = status_code
-        """HTTP status code."""
-        self.status_text = status_text
-        """Description of the HTTP status."""
-        self.body = body
-        """Body text of the response."""
-        super().__init__()
-
-
-class DownloadErrorGroup(FilingsAPIErrorGroup):
-    """Exceptions raised during download of files."""
-
-
 class CorruptDownloadError(FilingsAPIError):
     """
-    SHA-256 hash of the downloaded file does not match value from API.
+    SHA-256 checksum does not match expected value from API.
 
-    Attributes
-    ----------
-    path : str
-    url : str
-    calculated_hash : str
-    expected_hash : str
+    See Also
+    --------
+    downloader.CorruptDownloadError : Not FilingsAPIError subclassed.
     """
 
     def __init__(
             self, path: str, url: str, calculated_hash: str,
             expected_hash: str) -> None:
-        """Initialize `CorruptDownloadError`."""
-        self.path = path
+        self.path: str = path
         """Path where the file was saved."""
-        self.url = url
+        self.url: str = url
         """URL where the file was downloaded from."""
-        self.calculated_hash = calculated_hash
-        """Actual SHA-256 hash of the file in lowercase hex."""
-        self.expected_hash = expected_hash
-        """Expected SHA-256 hash of the file from API in lowercase hex."""
-        super().__init__()
-
-
-class FileNotAvailableWarning(FilingsAPIWarning):
-    """File requested for download was not available."""
+        self.calculated_hash: str = calculated_hash
+        """Actual SHA-256 checksum of the file in lowercase hex."""
+        self.expected_hash: str = expected_hash
+        """
+        Expected SHA-256 checksum of the file in lowercase hex.
 
-
-class DatabaseFileExistsError(FilingsAPIError):
-    """
-    The intended save path for the database is an existing file.
-    
-    Set parameter `update` to `True` to update an existing database.
-
-    Attributes
-    ----------
-    path : str
-    """
-
-    def __init__(self, path: str):
-        self.path = path
-        """Intended save path for the file."""
-        super().__init__()
-
-
-class DatabasePathIsReservedError(FilingsAPIError):
-    """
-    The intended save path for the database is already reserved by a
-    non-file database object.
-
-    Attributes
-    ----------
-    path : str
-    """
-
-    def __init__(self, path: str):
-        self.path = path
-        """Intended save path for the file."""
+        Originates from `Filing` attribute `package_sha256`.
+        """
         super().__init__()
 
 
-class DatabaseSchemaUnmatch(FilingsAPIError):
+class DatabaseSchemaUnmatchError(FilingsAPIError):
     """
-    The file contains a database whose schema does not match the
-    expected format.
+    The file contains a database whose schema is non-conformant.
 
     Either none of the expected tables are present or none of the
     expected columns for a matching table.
-
-    Attributes
-    ----------
-    path : str
     """
 
     def __init__(self, path: str):
-        self.path = path
+        self.path: str = path
         """Path for the database file."""
         super().__init__()
 
 
-class ApiReferenceWarning(FilingsAPIWarning):
-    """Resource referencing between filings, entities and validation
-    messages fails.
-    """
+class HTTPStatusError(FilingsAPIError):
+    """No APIError but the HTTP status is not 200."""
 
+    def __init__(self, status_code: int, status_text: str, body: str) -> None:
+        self.status_code: int = status_code
+        """HTTP status code."""
+        self.status_text: str = status_text
+        """Description of the HTTP status."""
+        self.body: str = body
+        """Body text of the response."""
+        super().__init__()
 
-class ApiIdCoherenceWarning(FilingsAPIWarning):
-    """Multiple query pages return resources with the same ``id``."""
 
+class JSONAPIFormatError(FilingsAPIError):
+    r"""The API returns a JSON:API document in bad format."""
 
-class APIStringParseWarning(FilingsAPIWarning):
-    """Parsing of API JSON string based on type `ParseType` failed."""
+    def __init__(self, msg: str) -> None:
+        self.msg: str = msg
+        """Error message."""
+        super().__init__()
 
 
-class DerivedValueError(FilingsAPIWarning):
-    """Could not generate a derived value."""
+class FilterNotSupportedWarning(FilingsAPIWarning):
+    """Used filter is not supported but can be used."""
```

### Comparing `xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/filings_api.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/query.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,316 +1,342 @@
 """
-Python API for filings.xbrl.org JSON:API by XBRL International.
+Define query functions for the API.
 
-The API provides an access to a repository of XBRL filings at
-``filings.xbrl.org``. There are three types of API resources:
-filings, entities and validation messages.
+All the functions are accessible through the package root namespace.
 
-The parameter `filters` in methods accepts a mapping such as a
-dictionary. Key is the attribute being searched for and the value is
+The parameter ``filters`` in functions/methods accepts a mapping such as
+a dictionary. Key is the attribute being searched for and the value is
 the searched item or an iterable of searched items. Both attribute
 styles are supported: the ones used by this library and the actual
 attribute names in the API. Search is case-sensitive. The API only
 supports equivalence filtering of one value, but by giving the
 mapping a value which is an iterable of strings, you may execute
-multiple equivalence filtering queries in one method call.
+multiple equivalence filtering queries in one function/method call.
 
-You will find the list of valid filtering attributes in list
-`data_attrs`. Please note
-that derived attributes such as `reporting_date` or `language` may
-not be used for filtering.
-
-Note however that as of July 2023, attributes ending with ``_count``
-and ``_url`` could not be used. To filter only the filings reported
-in Finland, you may use the following parameter::
+You will find the list of valid filtering attributes in the keys of dict
+`api_attribute_map`. Bear in mind that derived attributes such as
+`reporting_date` or `language` may not be used for filtering.
+
+To filter only the filings reported in Finland, you may use the
+following parameter::
 
     filters={'country': 'FI'}
 
 To filter reports of Finnish companies Apetit and Boreo, the most
 reliable way is to filter them using their LEI codes which are
-defined in the entity `identifier` attribute::
+defined in the `Entity.identifier` attribute::
 
     filters={'entity.identifier': [
                 '743700RSFZUIQYABYT14',
                 '743700OD4QRWKZ4ODC98']}
 
-For validation messages, plural prefix `validation_messages.` is
-required:
-    
-    filters={'validation_messages.code': 'message:tech_duplicated_facts1'}
-
-Date fields have a special functioning in `filters`. If you filter
-by a date that only has a year, a minimum of 12 requests are made
-for the end dates of each month. The months will start by default
-from August of the specified year and continue until July of the
-year following the specified year. Option `year_filter_months` can
-be used to change this behaviour. If you filter by a year and a
-month, the filter will assign the end date of that month to the
-filter automatically. So the following filter::
+For validation messages, plural prefix ``"validation_messages."`` is
+required::
+
+    filters={
+        'validation_messages.code': 'message:tech_duplicated_facts1'
+        }
+
+Date fields have a special functioning in ``filters``. If you filter
+by a date that only has a year, 12 requests are made by default for the
+end dates of each month. The months will start by default from January
+of the specified year and continue until December of the same year.
+Option :data:`~options.year_filter_months` can be used to change this
+behaviour. So the following filter::
 
-    filters={'last_end_date': '2022'}
+    filters={'last_end_date': 2022}
 
-Will yield the following requests::
+Will yield requests with the following parameter values::
 
-    last_end_date=2022-08-31
-    last_end_date=2022-09-30
+    last_end_date='2022-01-31'
+    last_end_date='2022-02-28'
     ...
-    last_end_date=2023-06-30
-    last_end_date=2023-07-31
+    last_end_date='2022-11-30'
+    last_end_date='2022-12-31'
 
-The parameter `sort` in methods accepts a single attribute string or
-a sequence (e.g. list) of attribute strings. Normal sort order is
-ascending, but descending order can be obtained by prefixing the
+If you filter by a year and a month, the filter will assign the end date
+of that month to the filter automatically, so
+:pt:`filters={'last_end_date': '2022-12'}` becomes
+:pt:`filters={'last_end_date': '2022-12-31'}`.
+
+The parameter ``sort`` in functions/methods accepts a single attribute
+string or a sequence (e.g. list) of attribute strings. Normal sort order
+is ascending, but descending order can be obtained by prefixing the
 attribute with a minus sign (-). As with filtering, attributes
-ending with ``_count`` and ``_url`` did not work in July 2023. The
-same keys of `api_attributes` dict are valid values for sort. To get
+ending with ``_count`` and ``_url`` did not work in July 2023.
+
+The keys of `api_attribute_map` dict are valid values for sort. To get
 the most recently added filings, specify the following parameter::
 
     sort='-added_time'
 
-Attributes
-----------
-download_count : int
-api_request_count : int
-total_request_count : int
-download_bytes : int
-download_size_str : str
+.. note::
+    Apart from `filing_page_iter`, the query functions return custom set
+    objects. Parameter ``sort`` can be used to filter either ends of the
+    value spectrum but it does not mean that the returned sets would
+    have any kind of order.
 
 """
 
-# SPDX-FileCopyrightText: 2023-present Lauri Salmela <lauri.m.salmela@gmail.com>
+# SPDX-FileCopyrightText: 2023 Lauri Salmela <lauri.m.salmela@gmail.com>
 #
 # SPDX-License-Identifier: MIT
 
-from collections.abc import Mapping, Sequence, Iterable, Generator
+from collections.abc import Iterable, Iterator, Mapping, Sequence
 from pathlib import Path
-from typing import Optional
+from typing import Any, Optional, Union
+
+from xbrl_filings_api import request_processor
+from xbrl_filings_api.constants import NO_LIMIT
+from xbrl_filings_api.filing_set import FilingSet
+from xbrl_filings_api.filings_page import FilingsPage
+from xbrl_filings_api.resource_collection import ResourceCollection
+from xbrl_filings_api.scope_flag import ScopeFlag
+
+__all__ = [
+    'get_filings',
+    'to_sqlite',
+    'filing_page_iter',
+    ]
 
-from .api_object.filing import Filing
-from .api_object.filings_page import FilingsPage
-from .enums import ScopeFlag, GET_ONLY_FILINGS
-from .filing_set.filing_set import FilingSet
-from .filing_set.resource_collection import ResourceCollection
-import xbrl_filings_api.database_processor as database_processor
-import xbrl_filings_api.request_processor as request_processor
 
-    
 def get_filings(
-        filters: Optional[Mapping[str, str | Iterable[str]]] = None,
-        sort: Optional[str | Sequence[str]] = None,
-        max_size: Optional[int] = 100,
-        flags: Optional[ScopeFlag] = GET_ONLY_FILINGS,
-        add_api_params: Optional[Mapping[str, str]] = None
-        ) -> FilingSet[Filing]:
+        filters: Optional[Mapping[str, Union[Any, Iterable[Any]]]] = None,
+        *,
+        sort: Optional[Union[str, Sequence[str]]] = None,
+        limit: int = NO_LIMIT,
+        flags: ScopeFlag = ScopeFlag.GET_ONLY_FILINGS,
+        add_api_params: Optional[Mapping] = None
+        ) -> FilingSet:
     """
-    Retrieve filings from the API.
+    Return a `FilingSet` of all the filings matching the query.
+
+    See :mod:`xbrl_filings_api.query` module documentation for specifics
+    of parameter usage.
 
     Parameters
     ----------
-    filters : mapping of str: {str, iterable of str}, optional
-        Mapping of filters. See `FilingAPI` class documentation.
+    filters : mapping of {str: any or iterable of any}, optional
+        Mapping of filters. Iterable values may be used to make a logic
+        OR-style query with multiple API requests.
     sort : str or sequence of str, optional
-        Sort result set by specified attribute(s). Use values of
-        `data_attrs`. Descending order field begins with minus sign (-).
-    max_size : int or NO_LIMIT, default 100
-        Maximum number of filings to retrieve. With `NO_LIMIT`,
-        you'll reach for the sky. Filings will be retrieved in
-        batches (pages) of option `max_page_size`.
+        Used together with ``limit`` to return filings from either end
+        of sorted attribute values. Order is lost in `FilingSet` object.
+        Default order is ascending; prefix attribute name with minus (-)
+        to get descending order.
+    limit : int, default NO_LIMIT
+        Maximum number of filings to retrieve. Filings will be retrieved
+        on pages (HTTP requests) of size `options.max_page_size`.
     flags : ScopeFlag, default GET_ONLY_FILINGS
         Scope of retrieval. Flag `GET_ENTITY` will retrieve and
-        create the object for `filing.entity` and
+        create the object for `Filing.entity` and
         `GET_VALIDATION_MESSAGES` a set of objects for
-        `filing.validation_messages`.
+        `Filing.validation_messages`.
     add_api_params: mapping, optional
-        Add additional JSON:API parameters to the query. All parts
-        will be URL-encoded automatically.
-    
+        Add additional, overriding request parameters to the query. All
+        parts will be URL-encoded automatically. Cannot be used to
+        override filters.
+
     Returns
     -------
     FilingSet of Filing
         Set of retrieved filings.
-    
-    Raises
-    ------
 
-    Warns
+    Notes
     -----
-    ApiIdCoherenceWarning
-        Filings with the same API id are returned more than once.
-    ApiReferenceWarning
-        Resource referencing between filings, entities and
-        validation messages fails.
+    Parameter ``add_api_params`` is handled by :class:`requests.Request`
+    parameter ``params``.
     """
-    if isinstance(sort, str):
-        sort = [sort]
-    filings = FilingSet({})
+    filings = FilingSet()
     res_colls: dict[str, ResourceCollection] = {
         'Entity': filings.entities,
         'ValidationMessage': filings.validation_messages
         }
+
     page_gen = request_processor.generate_pages(
-        filters, sort, max_size, flags, add_api_params, res_colls)
+        filters, limit, flags, res_colls, sort, add_api_params)
     for page in page_gen:
-        filings.update(page.filing_list)
+        # Do not deep copy or test filing_list by using FilingSet.update
+        filings._filings.update(page.filing_list)
     return filings
 
 
 def to_sqlite(
-        path: str | Path,
+        path: Union[str, Path],
+        *,
         update: bool = False,
-        filters: Optional[Mapping[str, str | Iterable[str]]] = None,
-        sort: Optional[str | Sequence[str]] = None,
-        max_size: Optional[int] = 100,
-        flags: Optional[ScopeFlag] = GET_ONLY_FILINGS,
-        add_api_params: Optional[Mapping[str, str]] = None
+        filters: Optional[Mapping[str, Union[Any, Iterable[Any]]]] = None,
+        sort: Optional[Union[str, Sequence[str]]] = None,
+        limit: int = NO_LIMIT,
+        flags: ScopeFlag = ScopeFlag.GET_ONLY_FILINGS,
+        add_api_params: Optional[Mapping] = None
         ) -> None:
     """
-    Read data from filings.xbrl.org database to an SQLite3 database.
+    Insert all filings from the query to an SQLite database.
+
+    See :mod:`xbrl_filings_api.query` module documentation for specifics
+    of parameter usage.
 
-    Tables ``Filing``, ``Entity`` and ``ValidationMessage`` will be
-    created according to settings in `flags`. Dependencies for SQL
-    joins:
-        * ``Filing.entity_api_id = Entity.api_id``
-        * ``Filing.api_id = ValidationMessage.filing_api_id``
-
-    If a file exists in `path` parameter path and `update` is
-    `False` (default), a `DatabaseFileExistsError` exception will be
-    raised. If `update` is `True`, retrieved records will update the
-    existing ones based on `api_id` and the new ones will be added.
-    A database to be updated may have additional tables and
-    additional columns. Missing tables and columns will be created.
+    Tables ``Filing``, ``Entity``, and ``ValidationMessage`` will be
+    created according to settings in parameter ``flags``. Dependencies
+    for SQL joins:
 
-    If the intermediary folders in `path` do not exist, they will be
-    created.
+    * ``Filing.entity_api_id = Entity.api_id``
+    * ``Filing.api_id = ValidationMessage.filing_api_id``
 
-    If `update` is `True` and the database does not have any
+    If parameter ``path`` value is a file and ``update`` is :pt:`False`
+    (default), a `FileExistsError` exception will be raised. If
+    ``update`` is :pt:`True`, retrieved records will update the existing
+    ones based on primary key ``api_id`` in tables and the new objects
+    will be added. A database to be updated may have additional tables
+    and additional columns. Missing tables and columns will be created.
+
+    If the intermediary folders in parameter ``path`` do not exist, they
+    will be created.
+
+    If ``update`` is :pt:`True` and the database does not have any
     expected tables defined or any of the expected tables contain no
-    expected columns, a `DatabaseSchemaUnmatch` exception will be
+    expected columns, a `DatabaseSchemaUnmatchError` exception will be
     raised.
 
-    The parameter `add_api_params` can be used to override
-    automatically generated JSON:API parameters ``page[size]``,
-    ``include`` and ``filter[<field>]`` and to add more of them to
-    the query.
+    Datetime values will be exported to the database as the same string
+    that was received from the API. The format is, as of April 2024,
+    :meth:`~datetime.datetime.strftime` format string
+    ``%Y-%m-%d %H:%M:%S.%f`` or ``%Y-%m-%d %H:%M:%S``.
 
     Parameters
     ----------
-    path or Path
+    path : str or Path
         Path to the SQLite database.
     update : bool, default False
         If the database already exists, update it with retrieved
         records. Old records are updated and new ones are added.
-    filters : mapping of str: {str, iterable of str}, optional
-        Mapping of filters. See `FilingAPI` class documentation.
+    filters : mapping of {str: any or iterable of any}, optional
+        Mapping of filters. Iterable values may be used to make a logic
+        OR-style query with multiple API requests.
     sort : str or sequence of str, optional
-        Sort result set by specified attribute(s). Use values of
-        `data_attrs`. Descending order field begins with minus sign (-).
-    max_size : int or NO_LIMIT, default 100
-        Maximum number of filings to retrieve. With `NO_LIMIT`,
-        you'll reach for the sky. Filings will be retrieved in
-        batches (pages) of option `max_page_size`.
+        Used together with parameter ``limit`` to return filings from
+        either end of sorted attribute values. Order is lost in
+        `FilingSet` object. Default order is ascending; prefix attribute
+        name with minus (-) to get descending order.
+    limit : int, default NO_LIMIT
+        Maximum number of filings to retrieve. Filings will be retrieved
+        on pages (HTTP requests) of size `options.max_page_size`.
     flags : ScopeFlag, default GET_ONLY_FILINGS
         Scope of retrieval. Flag `GET_ENTITY` will retrieve entity
         records of filings and `GET_VALIDATION_MESSAGES` the
         validation messages.
     add_api_params: mapping, optional
-        Add additional JSON:API parameters to the query. All parts
-        will be URL-encoded automatically.
-    
+        Add additional, overriding request parameters to the query. All
+        parts will be URL-encoded automatically. Cannot be used to
+        override filters.
+
     Raises
     ------
-    APIErrorGroup of APIError
-        If filings API returns errors.
+    APIError
+        First error returned by the filings API.
     HTTPStatusError
         If filings API does not return errors but HTTP status is not
         200.
-    DatabaseFileExistsError
-        When ``update=False``, if the intended save path for the
-        database is an existing file.
-    DatabasePathIsReservedError
-        The intended save path for the database is already reserved
-        by a non-file database object.
-    DatabaseSchemaUnmatch
-        When ``update=True``, if the file contains a database whose
-        schema does not match the expected format.
+    FileExistsError
+        When ``update`` is :pt:`False` and the intended save path for
+        the database is an existing file.
+    DatabaseSchemaUnmatchError
+        When ``update`` is :pt:`True` and the file contains a database
+        whose schema does not match the expected format.
     requests.ConnectionError
         If connection fails.
     sqlite3.DatabaseError
-        When ``update=True``, if the file is not a database
-        (``err.sqlite_errorname='SQLITE_NOTADB'``) etc.
+        For example when ``update`` is :pt:`True` and the file is not a
+        database etc.
+
+    See Also
+    --------
+    FilingSet.to_sqlite : Save a ready set to SQLite.
 
-    Warns
+    Notes
     -----
-    ApiIdCoherenceWarning
-        Filings with the same API id are returned more than once.
-    ApiReferenceWarning
-        Resource referencing between filings, entities and
-        validation messages fails.
+    Parameter ``add_api_params`` is handled by :class:`requests.Request`
+    parameter ``params``.
     """
-    ppath = path if isinstance(path, Path) else Path(path)
-    if isinstance(sort, str):
-        sort = [sort]
-    
+    filings = FilingSet()
+    res_colls: dict[str, ResourceCollection] = {
+        'Entity': filings.entities,
+        'ValidationMessage': filings.validation_messages
+        }
+
     page_gen = request_processor.generate_pages(
-        filters, sort, max_size, flags, add_api_params)
-    database_processor.pages_to_sqlite(
-        flags, ppath, update, page_gen)
+        filters, limit, flags, res_colls, sort, add_api_params)
+    for page in page_gen:
+        page_filings = FilingSet(page.filing_list)
+        page_filings.to_sqlite(
+            path=path,
+            update=update,
+            flags=flags
+            )
+        # ResourceCollection reads subresource references in FilingSet
+        filings.update(page_filings)
+        # After database creation, next pages are always added to
+        # existing db
+        update = True
 
 
 def filing_page_iter(
-        filters: Optional[Mapping[str, str | Iterable[str]]] = None,
-        sort: Optional[str | Sequence[str]] = None,
-        max_size: Optional[int] = 100,
-        flags: Optional[ScopeFlag] = GET_ONLY_FILINGS,
-        add_api_params: Optional[Mapping[str, str]] = None
-        ) -> Generator[FilingsPage, None, None]:
+        filters: Optional[Mapping[str, Union[Any, Iterable[Any]]]] = None,
+        sort: Optional[Union[str, Sequence[str]]] = None,
+        limit: int = NO_LIMIT,
+        flags: ScopeFlag = ScopeFlag.GET_ONLY_FILINGS,
+        add_api_params: Optional[Mapping] = None
+        ) -> Iterator[FilingsPage]:
     """
-    Iterate API query results page by page.
+    Lazily iterate query results page by page.
+
+    See :mod:`xbrl_filings_api.query` module documentation for specifics
+    of parameter usage.
+
+    The iterator is lazy and a new HTTP request is made only when the
+    next value is requested from it.
+
+    Subresources, namely `Entity`, are only created once. This means
+    that subsequent pages containing filings of the same entity as on an
+    earlier page, will refer to the same object.
 
     Parameters
     ----------
-    filters : mapping of str: {str, iterable of str}, optional
-        Mapping of filters. See `FilingAPI` class documentation.
+    filters : mapping of {str: any or iterable of any}, optional
+        Mapping of filters. Iterable values may be used to make a logic
+        OR-style query with multiple API requests.
     sort : str or sequence of str, optional
-        Sort result set by specified attribute(s). Use values of
-        `data_attrs`. Descending order field begins with minus sign (-).
-    max_size : int or NO_LIMIT, default 100
-        Maximum number of filings to retrieve. With `NO_LIMIT`,
-        you'll reach for the sky. Filings will be retrieved in
-        batches (pages) of option `max_page_size`.
+        Sort filings on pages. Default order is ascending; prefix
+        attribute name with minus (-) to get descending order.
+    limit : int, default NO_LIMIT
+        Maximum number of filings to retrieve. Filings will be retrieved
+        on pages (HTTP requests) of size `options.max_page_size`.
     flags : ScopeFlag, default GET_ONLY_FILINGS
         Scope of retrieval. Flag `GET_ENTITY` will retrieve and
-        create the object for `filing.entity` and
+        create the object for `Filing.entity` and
         `GET_VALIDATION_MESSAGES` a set of objects for
-        `filing.validation_messages`.
+        `Filing.validation_messages`.
     add_api_params: mapping, optional
-        Add additional JSON:API parameters to the query. All parts
-        will be URL-encoded automatically.
-    
+        Add additional, overriding request parameters to the query. All
+        parts will be URL-encoded automatically. Cannot be used to
+        override filters.
+
     Yields
     ------
     FilingsPage
         Filings page containing a batch of downloaded filings
-    
-    Raises
-    ------
 
-    Warns
+    Notes
     -----
-    ApiIdCoherenceWarning
-        Filings with the same API id are returned more than once.
-    ApiReferenceWarning
-        Resource referencing between filings, entities and
-        validation messages fails.
+    Parameter ``add_api_params`` is handled by :class:`requests.Request`
+    parameter ``params``.
     """
-    if isinstance(sort, str):
-        sort = [sort]
-    filings = FilingSet({})
+    filings = FilingSet()
     res_colls: dict[str, ResourceCollection] = {
         'Entity': filings.entities,
         'ValidationMessage': filings.validation_messages
         }
+
     page_gen = request_processor.generate_pages(
-        filters, sort, max_size, flags, add_api_params, res_colls)
-    for page in page_gen:
-        filings.update(page.filing_list)
-    return filings
+        filters, limit, flags, res_colls, sort, add_api_params)
+    yield from page_gen
```

### Comparing `xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/lang_code_transform.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/lang_code_transform.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """
-Dictionary for tranformation of offial European Union languages from
-ISO 639-2 (alpha-3 codes) to ISO 639-1 (alpha-2 codes).
+Define alpha-3 to alpha-2 language code transformations.
+
+Defines :class:`dict` ``LANG_CODE_TRANSFORM`` for tranformation of
+offial European Union languages from ISO 639-2 (alpha-3 codes) to ISO
+639-1 (alpha-2 codes).
 
 The transformations are needed for year 2020 ESEF reports when
-requirements to report the language in the file name was obscure.
+requirements to report the language in the file name were obscure. They
+affect the resolution of derived attribute `Filing.language`.
 
 """
 
-# SPDX-FileCopyrightText: 2023-present Lauri Salmela <lauri.m.salmela@gmail.com>
+# SPDX-FileCopyrightText: 2023 Lauri Salmela <lauri.m.salmela@gmail.com>
 #
 # SPDX-License-Identifier: MIT
 
+__all__ = ['LANG_CODE_TRANSFORM']
+
 
 LANG_CODE_TRANSFORM = {
     'bul': 'bg', # Bulgarian
     'ces': 'cs', # Czech
     'dan': 'da', # Danish
     'deu': 'de', # German
     'ell': 'el', # Greek
@@ -32,9 +38,9 @@
     'nld': 'nl', # Dutch
     'pol': 'pl', # Polish
     'por': 'pt', # Portuguese
     'ron': 'ro', # Romanian
     'slk': 'sk', # Slovak
     'slv': 'sl', # Slovenian
     'spa': 'es', # Spanish
-    'swe': 'sv' # Swedish
+    'swe': 'sv', # Swedish
 }
```

### Comparing `xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/api_object/entity.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/entity.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,87 @@
-"""
-Define `Entity` class.
+"""Define `Entity` class."""
 
-"""
-
-# SPDX-FileCopyrightText: 2023-present Lauri Salmela <lauri.m.salmela@gmail.com>
+# SPDX-FileCopyrightText: 2023 Lauri Salmela <lauri.m.salmela@gmail.com>
 #
 # SPDX-License-Identifier: MIT
 
-from types import EllipsisType
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Optional, Union
+
+from xbrl_filings_api.api_request import APIRequest
+from xbrl_filings_api.api_resource import APIResource
+from xbrl_filings_api.constants import Prototype
+from xbrl_filings_api.parse_type import ParseType
+from xbrl_filings_api.scope_flag import ScopeFlag
+
+if TYPE_CHECKING:
+    from xbrl_filings_api.filing import Filing
 
-from ..enums import ParseType, GET_ENTITY
-from ..api_request import APIRequest
-from .api_resource import APIResource
+__all__ = ['Entity']
 
 
 class Entity(APIResource):
     """
-    Entity of ``filings.xbrl.org`` API.
-    
-    Attributes
-    ----------
-    api_id : str or None
-    identifier: str | None
-    name: str | None
-    filings: set of Filing
-    api_entity_filings_url: str | None
-    request_time : datetime
-    request_url : str
+    Entity in the database which has filed filings.
+
+    In most cases, the entity is the parent company of the group.
     """
-    
+
     TYPE = 'entity'
     NAME = 'attributes.name'
     IDENTIFIER = 'attributes.identifier'
     API_ENTITY_FILINGS_URL = 'relationships.filings.links.related'
 
-    _FILING_FLAG = GET_ENTITY
+    _FILING_FLAG = ScopeFlag.GET_ENTITY
 
     def __init__(
             self,
-            json_frag: dict | EllipsisType,
-            api_request: APIRequest | None = None
+            json_frag: Union[dict, Prototype],
+            api_request: Optional[APIRequest] = None
             ) -> None:
+        # Signatures::
+        #     Entity(json_frag: dict, api_request: APIRequest)
+        #     Entity(json_frag: Prototype)
         super().__init__(json_frag, api_request)
 
-        self.identifier: str | None = self._json.get(self.IDENTIFIER)
+        self.identifier: Union[str, None] = self._json.get(self.IDENTIFIER)
         """
         The identifier for entity.
-        
-        For ESEF filers, this is the LEI code.
+
+        For ESEF filers, this should be the LEI code.
         """
 
-        self.name: str | None = self._json.get(self.NAME)
+        self.name: Union[str, None] = self._json.get(self.NAME)
         """Name of the entity."""
 
-        # Set of Filing objects
-        self.filings: set[object] = set()
-        """Set of `Filing` objects from the query reported by this
-        entity.
-        """
+        self.filings: set[Filing] = set()
+        """Set of filings reported by this entity."""
 
-        self.api_entity_filings_url: str | None = self._json.get(
+        self.api_entity_filings_url: Union[str, None] = self._json.get(
             self.API_ENTITY_FILINGS_URL, ParseType.URL)
-        """A link to the JSON:API page with full list of filings by this
-        entity.
-        """
-        
+        r"""URL to the page with full list of filings by this entity."""
+
         self._json.close()
 
     def __repr__(self) -> str:
-        return f'{self.__class__.__name__}(name={self.name!r})'
+        """Return repr with `api_id` and `name`."""
+        return (
+            f'{type(self).__name__}('
+            f'api_id={self.api_id!r}, name={self.name!r})'
+            )
+
+    def __str__(self) -> str:
+        """
+        Return "<`name`> (<`identifier`>)", or either alone.
+
+        If both are defined, full string is returned but if only one is
+        defined, it is returned. If neither is defined, return empty
+        string.
+        """
+        if self.name and self.identifier:
+            return f'{self.name} ({self.identifier})'
+        if self.name:
+            return self.name
+        if self.identifier:
+            return self.identifier
+        return ''
```

### Comparing `xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/api_object/filings_page.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/filings_page.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,199 +1,208 @@
-"""
-Define `FilingsPage` class.
+"""Define `FilingsPage` class."""
 
-"""
-
-# SPDX-FileCopyrightText: 2023-present Lauri Salmela <lauri.m.salmela@gmail.com>
+# SPDX-FileCopyrightText: 2023 Lauri Salmela <lauri.m.salmela@gmail.com>
 #
 # SPDX-License-Identifier: MIT
 
+import logging
+from collections.abc import Iterable
 from itertools import chain
-import warnings
+from typing import Any, Union
+
+from xbrl_filings_api.api_page import APIPage
+from xbrl_filings_api.api_request import APIRequest
+from xbrl_filings_api.api_resource import APIResource
+from xbrl_filings_api.entity import Entity
+from xbrl_filings_api.filing import Filing
+from xbrl_filings_api.resource_collection import ResourceCollection
+from xbrl_filings_api.scope_flag import ScopeFlag
+from xbrl_filings_api.validation_message import ValidationMessage
+
+__all__ = ['FilingsPage']
 
-from ..api_request import APIRequest
-from ..enums import (
-    ScopeFlag, GET_ONLY_FILINGS, GET_ENTITY, GET_VALIDATION_MESSAGES)
-from ..exceptions import ApiIdCoherenceWarning
-from ..exceptions import ApiReferenceWarning
-from ..filing_set.resource_collection import ResourceCollection
-from .api_page import APIPage
-from .api_resource import APIResource
-from .entity import Entity
-from .filing import Filing
-from .validation_message import ValidationMessage
+logger = logging.getLogger(__name__)
 
 
 class FilingsPage(APIPage):
-    """
-    JSON:API response page containing filing resources.
-    
-    Attributes
-    ----------
-    request_time : datetime
-    query_filing_count : int or None
-    filing_list: list of Filing
-    entity_list : list of Entity or None
-    validation_message_list : list of ValidationMessage or None
-    jsonapi_version : str or None
-    api_self_url : str or None
-    api_prev_page_url : str or None
-    api_next_page_url : str or None
-    api_first_page_url : str or None
-    api_last_page_url : str or None
-    request_url : str
-    """
+    """Response page containing filings as primary resource."""
+
     def __init__(
             self, json_frag: dict, api_request: APIRequest,
             flags: ScopeFlag, received_api_ids: dict[str, set],
             res_colls: dict[str, ResourceCollection]
             ) -> None:
-        """Initiate a JSON:API response page.
-
-        Warns
-        -----
-        ApiReferenceWarning
-            Resource referencing between filings, entities and
-            validation messages fails.
-        """
         super().__init__(json_frag, api_request)
 
         self.query_filing_count = self._data_count
         """Total count of filings of the query including the ones not on
         this page.
         """
 
         self.filing_list: list[Filing]
         """List of `Filing` objects on this page."""
 
-        self.entity_list: list[Entity] | None = (
-            self._get_inc_resource(
-                api_request=api_request,
-                received_api_ids=received_api_ids,
-                type_obj=Entity,
-                flag_member=GET_ENTITY,
-                flags=flags
-                ))
-        """
-        Set of `Entity` objects on this page.
-        
-        Is `None` if `flags` parameter did not include `GET_ENTITY`.
-        """
-        
-        self.validation_message_list: list[ValidationMessage] | None = (
-            self._get_inc_resource(
-                api_request=api_request,
-                received_api_ids=received_api_ids,
-                type_obj=ValidationMessage,
-                flag_member=GET_VALIDATION_MESSAGES,
-                flags=flags
-                ))
+        ents = self._get_inc_resource(
+            type_obj=Entity,
+            api_request=api_request,
+            received_api_ids=received_api_ids,
+            flag_member=ScopeFlag.GET_ENTITY,
+            flags=flags
+            )
+        # type_obj=Entity always returns list[Entity] | None
+        self.entity_list: Union[list[Entity], None] = (
+            ents) # type: ignore[assignment]
+        """
+        List of `Entity` objects on this page.
+
+        Is :pt:`None` if ``flags`` parameter did not include
+        `GET_ENTITY`.
+        """
+
+        vmsgs = self._get_inc_resource(
+            type_obj=ValidationMessage,
+            api_request=api_request,
+            received_api_ids=received_api_ids,
+            flag_member=ScopeFlag.GET_VALIDATION_MESSAGES,
+            flags=flags
+            )
+        # type_obj=ValidationMessage always returns
+        # list[ValidationMessage] | None
+        self.validation_message_list: Union[list[ValidationMessage], None] = (
+            vmsgs) # type: ignore[assignment]
         """
-        Set of `ValidationMessage` objects on this page.
+        List of `ValidationMessage` objects on this page.
 
-        Is `None` if `flags` parameter did not include
+        Is :pt:`None` if ``flags`` parameter did not include
         `GET_VALIDATION_MESSAGES`.
         """
-        
+
         self._json.close()
 
         self.filing_list = self._get_filings(
             received_api_ids, res_colls, flags)
         self._check_validation_messages_references()
         self._determine_unexpected_inc_resources()
-    
+
+    def __repr__(self) -> str:
+        """
+        Return repr with request_url, query_time, and len(filing_list).
+
+        Attribute :attr:`~APIObject.request_url` is shown as repr,
+        `query_time` as unprefixed datetime() constructor, and
+        len(`filing_list`) as integer.
+        """
+        time_str = self.query_time.strftime('%Y, %m, %d, %H, %M, %S')
+        query_time = f'datetime({time_str})'
+        subreslist = ''
+        if self.entity_list is not None:
+            subreslist += f', len(entity_list)={len(self.entity_list)}'
+        if self.validation_message_list is not None:
+            subreslist += (
+                ', len(validation_message_list)='
+                + str(len(self.validation_message_list))
+                )
+        return (
+            f'{type(self).__name__}('
+            f'request_url={self.request_url!r}, '
+            f'query_time={query_time}, '
+            f'len(filing_list)={len(self.filing_list)}{subreslist})'
+            )
+
+    def _check_validation_messages_references(self) -> None:
+        if self.validation_message_list is not None:
+            for vmsg in self.validation_message_list:
+                if vmsg.filing is None:
+                    msg = f'No filing defined for {vmsg!r}'
+                    logger.warning(msg, stacklevel=2)
+
+    def _determine_unexpected_inc_resources(self) -> None:
+        self._json.unexpected_resource_types.update(
+            [(res.type_, 'included') for res in self._included_resources])
+
     def _get_filings(
             self, received_api_ids: dict[str, set],
             res_colls: dict[str, ResourceCollection], flags: ScopeFlag
             ) -> list[Filing]:
-        """Get filings from from `data` key.
-
-        Warns
-        -----
-        ApiReferenceWarning
-        """
+        """Get filings from from document ``data`` key."""
         filing_list = []
         if not received_api_ids.get('Filing'):
             received_api_ids['Filing'] = set()
         received_set = received_api_ids['Filing']
 
         if self._data:
             for res_frag in self._data:
                 res_type = str(res_frag.get('type')).lower()
 
                 if res_type == Filing.TYPE:
-                    res_id = str(res_frag.get('id'))
-                    if res_id in received_set:
-                        msg = (
-                            f'Same filing returned again, api_id={res_id!r}.'
-                            )
-                        warnings.warn(msg, ApiIdCoherenceWarning)
-                    else:
-                        received_set.add(res_id)
-                        entity_iter = None
-                        message_iter = None
-                        if GET_ONLY_FILINGS not in flags:
-                            if GET_ENTITY in flags:
-                                entity_iter = chain(
-                                    self.entity_list,
-                                    res_colls['Entity']
-                                    )
-                            if GET_VALIDATION_MESSAGES in flags:
-                                message_iter = chain(
-                                    self.validation_message_list,
-                                    res_colls['ValidationMessage']
-                                    )
-                        filing = Filing(
-                            res_frag,
-                            APIRequest(self.request_url, self.request_time),
-                            entity_iter,
-                            message_iter
-                            )
+                    filing = self._parse_filing_fragment(
+                        res_frag, received_set, res_colls, flags)
+                    if filing:
                         filing_list.append(filing)
                 else:
                     self._json.unexpected_resource_types.add(
                         (res_type, 'data'))
         return filing_list
 
     def _get_inc_resource(
             self,
+            type_obj: type[APIResource],
             api_request: APIRequest,
             received_api_ids: dict[str, set],
-            type_obj: type[APIResource],
             flag_member: ScopeFlag,
             flags: ScopeFlag
-            ) -> list[Entity | ValidationMessage] | None:
-        if (GET_ONLY_FILINGS in flags or flag_member not in flags):
+            ) -> Union[list[APIResource], None]:
+        if (ScopeFlag.GET_ONLY_FILINGS in flags or flag_member not in flags):
             return None
-        
+
         resource_list = []
-        type_name = type_obj.__class__.__name__
+        type_name = type_obj.__name__
         if not received_api_ids.get(type_name):
             received_api_ids[type_name] = set()
         received_set = received_api_ids[type_name]
 
         found_ix = []
         for res_i, res in enumerate(self._included_resources):
-            if res.type == type_obj.TYPE:
-                if res.id not in received_set:
-                    received_set.add(res.id)
+            if res.type_ == type_obj.TYPE:
+                if res.id_ not in received_set:
+                    received_set.add(res.id_)
                     # Construct Entity() or ValidationMessage()
                     res_instance = type_obj(res.frag, api_request)
                     resource_list.append(res_instance)
                     found_ix.append(res_i)
         found_ix.reverse()
         for res_i in found_ix:
             del self._included_resources[res_i]
         return resource_list
-    
-    def _determine_unexpected_inc_resources(self) -> None:
-        self._json.unexpected_resource_types.update(
-            [(res.type, 'included') for res in self._included_resources])
-    
-    def _check_validation_messages_references(self) -> None:
-        if self.validation_message_list is not None:
-            for vmsg in self.validation_message_list:
-                if vmsg.filing is None:
-                    msg = (
-                        f'No filing defined for {vmsg!r}, api_id={vmsg.api_id}'
+
+    def _parse_filing_fragment(
+            self, res_frag: dict[str, Any], received_set: set[str],
+            res_colls: dict[str, ResourceCollection], flags: ScopeFlag
+            ) -> Union[Filing, None]:
+        """Get filings from from a single ``data`` key fragment."""
+        res_id = str(res_frag.get('id'))
+        if res_id in received_set:
+            msg = f'Same filing returned again, api_id={res_id!r}.'
+            logger.warning(msg, stacklevel=3)
+            return None
+        else:
+            received_set.add(res_id)
+            entity_iter: Union[Iterable[Entity], None] = None
+            message_iter: Union[Iterable[ValidationMessage], None] = None
+            if ScopeFlag.GET_ONLY_FILINGS not in flags:
+                if ScopeFlag.GET_ENTITY in flags:
+                    ents = self.entity_list if self.entity_list else ()
+                    entity_iter = chain(
+                        ents,
+                        res_colls['Entity'] # type: ignore[arg-type]
+                        )
+                if ScopeFlag.GET_VALIDATION_MESSAGES in flags:
+                    vmsgs = (
+                        self.validation_message_list
+                        if self.validation_message_list else ()
+                        )
+                    message_iter = chain(
+                        vmsgs,
+                        res_colls['ValidationMessage'] # type: ignore[arg-type]
                         )
-                    warnings.warn(msg, ApiReferenceWarning, stacklevel=2)
+            api_request = APIRequest(self.request_url, self.query_time)
+            return Filing(res_frag, api_request, entity_iter, message_iter)
```

### Comparing `xbrl_filings_api-1.0.0.dev1/xbrl_filings_api/api_object/validation_message.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/validation_message.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,257 +1,309 @@
-"""
-Define `ValidationMessage` class.
+"""Define `ValidationMessage` class."""
 
-"""
-
-# SPDX-FileCopyrightText: 2023-present Lauri Salmela <lauri.m.salmela@gmail.com>
+# SPDX-FileCopyrightText: 2023 Lauri Salmela <lauri.m.salmela@gmail.com>
 #
 # SPDX-License-Identifier: MIT
 
-from pathlib import PurePath
-from types import EllipsisType
+from __future__ import annotations
+
+import logging
 import re
 import urllib.parse
-import warnings
+from pathlib import PurePosixPath
+from typing import TYPE_CHECKING, Optional, Union
+
+from xbrl_filings_api.api_request import APIRequest
+from xbrl_filings_api.api_resource import APIResource
+from xbrl_filings_api.constants import Prototype
+from xbrl_filings_api.scope_flag import ScopeFlag
 
-from ..api_request import APIRequest
-from ..enums import GET_VALIDATION_MESSAGES
-from ..exceptions import DerivedValueError
-from .api_resource import APIResource
+if TYPE_CHECKING:
+    from xbrl_filings_api.filing import Filing
+
+__all__ = ['ValidationMessage']
+
+logger = logging.getLogger(__name__)
 
 
 class ValidationMessage(APIResource):
     """
-    A single validation message of any severity.
+    Message for a filing in the database from a validator software.
 
-    The source of validation has not been published by filings.xbrl.org
-    but it seems likely that they originate from Arelle software.
-    
     Validation messages are issues in XBRL standard conformance, and the
     formula rules defined in the XBRL taxonomy.
 
     Country-specific filing rules defined by financial regulatory
     authorities and other agencies are not in the scope of validation.
     The rules defined in ESEF Reporting Manual are not checked if they
     are not codified in the taxonomy formula rules.
 
     Calculation inconsistency is the term used for issues in accounting
     coherence.
-    
-    Attributes
-    ----------
-    api_id : str or None
-    severity : str or None
-    text : str or None
-    code : str or None
-    filing_api_id : str or None
-    filing : Filing or None
-    calc_computed_sum : float or None
-    calc_reported_sum : float or None
-    calc_context_id : str or None
-    calc_line_item : str or None
-    calc_short_role : str or None
-    calc_unreported_items : str or None
-    duplicate_greater : float or None
-    duplicate_lesser : float or None
-    request_time : datetime
-    request_url : str
+
+    Derived attributes beginning ``calc_`` are only available when
+    `code` is ``'xbrl.5.2.5.2:calcInconsistency'``. The ones beginning
+    ``duplicate_`` are available for `code`
+    ``'message:tech_duplicated_facts1'`` if the values are numeric. They
+    are parsed out from the `text` of the message.
+
+    Notes
+    -----
+    The source of validation has not been published by the API provider.
+    However, it seems likely that they originate from Arelle software as
+    they seem similar and JSON and iXBRL viewer files are also generated
+    with it.
     """
 
     TYPE = 'validation_message'
     SEVERITY = 'attributes.severity'
     TEXT = 'attributes.message'
     CODE = 'attributes.code'
 
-    _FILING_FLAG = GET_VALIDATION_MESSAGES
-    
+    _FILING_FLAG = ScopeFlag.GET_VALIDATION_MESSAGES
+
     _LINE_ITEM_RE = re.compile(r'\bfrom (\S+)')
     _SHORT_ROLE_RE = re.compile(r'\blink role (\S+)')
     _REPORTED_SUM_RE = re.compile(r'\breported sum (\S+)')
     _COMPUTED_SUM_RE = re.compile(r'\bcomputed sum (\S+)')
     _CONTEXT_ID_RE = re.compile(r'\bcontext (\S+)')
     _UNREPORTED_ITEMS_RE = re.compile(r'\bunreportedContributingItems (.+)')
     _COMMA_RE = re.compile(r'\s*,\s*')
     _DUPLICATE_1_RE = re.compile(r'\bvalue:\s*(\S+)')
     _DUPLICATE_2_RE = re.compile(r'!=\s+(\S+)')
 
     def __init__(
             self,
-            json_frag: dict | EllipsisType,
-            api_request: APIRequest | None = None
+            json_frag: Union[dict, Prototype],
+            api_request: Optional[APIRequest] = None
             ) -> None:
+        # Signatures::
+        #     ValidationMessage(
+        #         json_frag: dict,
+        #         api_request: APIRequest
+        #         )
+        #     ValidationMessage(json_frag: Prototype)
         super().__init__(json_frag, api_request)
 
-        self.severity: str | None = self._json.get(self.SEVERITY)
+        self.code: Union[str, None] = self._json.get(self.CODE)
+        """
+        The code describing the source of the broken rule.
+
+        For example, code ``'xbrl.5.2.5.2:calcInconsistency'`` refers to
+        XBRL 2.1 base specification heading 5.2.5.2 with title "The
+        <calculationArc> element".
+        """
+
+        self.severity: Union[str, None] = self._json.get(self.SEVERITY)
         """
         Severity of the validation message.
-        
+
         Can be ``ERROR``, ``WARNING`` or ``INCONSISTENCY``.
         Might include ``ERROR-SEMANTIC`` and ``WARNING-SEMANTIC`` but
         most likely not.
 
         Arelle has also more message levels, but these are very
         certainly not included anywhere (``(DYNAMIC)``, ``CRITICAL``,
         ``DEBUG``, ``EXCEPTION``, ``INFO``, ``INFO-RESULT``).
         """
 
-        self.text: str | None = self._json.get(self.TEXT)
+        self.text: Union[str, None] = self._json.get(self.TEXT)
         """Validation message text."""
         if isinstance(self.text, str):
             self.text = self.text.strip()
 
-        self.code: str | None = self._json.get(self.CODE)
-        """
-        The code describing the source of the broken rule.
-        
-        For example, code ``xbrl.5.2.5.2:calcInconsistency`` refers to
-        XBRL 2.1 base specification heading 5.2.5.2 with title "The
-        <calculationArc> element".
-        """
-
-        self.filing_api_id: str | None = None
-        """`api_id` of Filing object."""
-
-        # Filing object
-        self.filing: object | None = None
-        """`Filing` object of this validation message."""
-        
-        self._json.close()
-
-        self.calc_computed_sum: float | None = None
+        self.calc_computed_sum: Union[float, None] = None
         """
         Derived computed sum of the calculation inconsistency.
-        
+
         Based on attribute `text` for validation messages whose `code`
-        is ``xbrl.5.2.5.2:calcInconsistency``.
+        is ``'xbrl.5.2.5.2:calcInconsistency'``.
         """
 
-        self.calc_reported_sum: float | None = None
+        self.calc_reported_sum: Union[float, None] = None
         """
         Derived reported sum of the calculation inconsistency.
-        
+
         Based on attribute `text` for validation messages whose `code`
-        is ``xbrl.5.2.5.2:calcInconsistency``.
+        is ``'xbrl.5.2.5.2:calcInconsistency'``.
         """
 
-        self.calc_context_id: str | None = None
+        self.calc_context_id: Union[str, None] = None
         """
         Derived XBRL context ID of the calculation inconsistency.
-        
+
         Based on attribute `text` for validation messages whose `code`
-        is ``xbrl.5.2.5.2:calcInconsistency``.
+        is ``'xbrl.5.2.5.2:calcInconsistency'``.
         """
 
-        self.calc_line_item: str | None = None
+        self.calc_line_item: Union[str, None] = None
         """
         Derived line item name of the calculation inconsistency.
 
         This field contains the qualified name of the line item (XBRL
         concept) with the taxonomy prefix and the local name parts. It
-        could be for example "ifrs-full:Assets".
-        
+        could be for example ``ifrs-full:Assets``.
+
         Based on attribute `text` for validation messages whose `code`
-        is ``xbrl.5.2.5.2:calcInconsistency``.
+        is ``'xbrl.5.2.5.2:calcInconsistency'``.
         """
 
-        self.calc_short_role: str | None = None
+        self.calc_short_role: Union[str, None] = None
         """
         Derived last part of the link role of the calculation
         inconsistency.
 
         For example a link role URI
         "http://www.example.com/esef/taxonomy/2022-12-31/FinancialPositionConsolidated"
         is truncated to "FinancialPositionConsolidated".
-        
+
         Based on attribute `text` for validation messages whose `code`
-        is ``xbrl.5.2.5.2:calcInconsistency``.
+        is ``'xbrl.5.2.5.2:calcInconsistency'``.
         """
 
-        self.calc_unreported_items: list[str] | None = None
+        self.calc_unreported_items: Union[list[str], None] = None
         """
         Derived unreported contributing line items of the calculation
         inconsistency.
 
         This refers to the line item names of items which are defined as
         the addends for `calc_line_item` in any of the link roles in the
         XBRL taxonomies of this report and which were not reported in
         the same XBRL context with this fact.
 
         When the data is output to a database, this field is a string
-        with parts joined by a newline character ('\\n').
-        
+        with parts joined by a newline character.
+
         Based on attribute `text` for validation messages whose `code`
-        is ``xbrl.5.2.5.2:calcInconsistency``.
+        is ``'xbrl.5.2.5.2:calcInconsistency'``.
         """
 
-        self.duplicate_greater: float | None = None
+        self.duplicate_greater: Union[float, None] = None
         """
         Derived greater item of the duplicate pair.
-        
+
         Based on attribute `text` for validation messages whose `code`
-        is ``message:tech_duplicated_facts1``.
+        is ``'message:tech_duplicated_facts1'``.
+
+        Does not include code ``'formula:assertionUnsatisfied'`` with
+        ``tech_duplicated_facts1`` in the beginning of the message (more
+        than 2 duplicated facts).
         """
 
-        self.duplicate_lesser: float | None = None
+        self.duplicate_lesser: Union[float, None] = None
         """
         Derived lesser item of the duplicate pair.
-        
+
         Based on attribute `text` for validation messages whose `code`
-        is ``message:tech_duplicated_facts1``.
+        is ``'message:tech_duplicated_facts1'``.
+
+        Does not include code ``'formula:assertionUnsatisfied'`` with
+        ``tech_duplicated_facts1`` in the beginning of the message (more
+        than 2 duplicated facts).
         """
 
+        self.filing_api_id: Union[str, None] = None
+        """`api_id` of `filing` object."""
+
+        self.filing: Union[Filing, None] = None
+        """Filing of this validation message."""
+
+        self._json.close()
+
         if self.code == 'xbrl.5.2.5.2:calcInconsistency':
-            self.calc_computed_sum = self._derive_calc_float(
-                self._COMPUTED_SUM_RE, 'calc_computed_sum')
-            self.calc_reported_sum = self._derive_calc_float(
-                self._REPORTED_SUM_RE, 'calc_reported_sum')
-            self.calc_context_id = self._derive_calc(
-                self._CONTEXT_ID_RE)
-            self.calc_line_item = self._derive_calc(
-                self._LINE_ITEM_RE)
-            self.calc_short_role = self._derive_calc(
-                self._SHORT_ROLE_RE)
-            unreported_items = self._derive_calc(
-                self._UNREPORTED_ITEMS_RE)
-            
-            uri_path = urllib.parse.urlparse(self.calc_short_role).path
-            if uri_path.strip():
-                last_part = PurePath(uri_path).name
-                if last_part.strip():
-                    self.calc_short_role = last_part
-            
-            if unreported_items and unreported_items.lower() != 'none':
-                self.calc_unreported_items = (
-                    self._COMMA_RE.split(unreported_items))
-        
-        if self.code == 'message:tech_duplicated_facts1':
-            duplicate_1 = self._derive_calc_float(
-                self._DUPLICATE_1_RE, 'duplicate_*')
-            duplicate_2 = self._derive_calc_float(
-                self._DUPLICATE_2_RE, 'duplicate_*')
-            if (isinstance(duplicate_1, float)
-                    and isinstance(duplicate_2, float)):
-                self.duplicate_greater = max(duplicate_1, duplicate_2)
-                self.duplicate_lesser = min(duplicate_1, duplicate_2)
+            self._derive_calc_prefixed_attrs()
+        elif self.code == 'message:tech_duplicated_facts1':
+            self._derive_duplicate_prefixed_attrs()
 
     def __repr__(self) -> str:
-        return f'{self.__class__.__name__}(code={self.code!r})'
-    
-    def _derive_calc(self, re_obj: re.Pattern) -> str | None:
+        """Return repr with `api_id`, `code` and `severity`."""
+        return (
+            f'{type(self).__name__}('
+            f'api_id={self.api_id!r}, code={self.code!r}, '
+            f'severity={self.severity!r})'
+            )
+
+    def __str__(self) -> str:
+        r"""
+        Return "[`severity`\ [:3] `code`] `text`".
+
+        Attribute ``severity`` shows only the first three characters.
+        Square brackets are used to encompass ``severity`` and ``code``.
+        """
+        text = '' if self.text is None else f' {self.text}'
+        plist = []
+        if self.severity:
+            plist.append(self.severity[:3])
+        if self.code:
+            plist.append(self.code)
+        prefix = ' '.join(plist)
+        return f'[{prefix}]{text}'
+
+    def _derive_calc(self, re_obj: re.Pattern) -> Union[str, None]:
         mt = re_obj.search(self.text)
         if mt:
             return mt[1]
         return None
-    
-    def _derive_calc_float(self, re_obj: re.Pattern, attr_name: str) -> float | None:
+
+    def _derive_calc_float(
+            self, re_obj: re.Pattern, attr_name: str) -> Union[float, None]:
         calc_str = self._derive_calc(re_obj)
         calc_float = None
         if calc_str is not None:
             try:
                 calc_float = float(calc_str.replace(',', ''))
             except ValueError:
                 msg = (
                     f'String {calc_str!r} of attribute {attr_name!r} could '
                     'not be parsed into float.'
                     )
-                warnings.warn(msg, DerivedValueError)
+                logger.warning(msg, stacklevel=2)
         return calc_float
+
+    def _derive_calc_prefixed_attrs(self):
+        self.calc_computed_sum = self._derive_calc_float(
+            self._COMPUTED_SUM_RE, 'calc_computed_sum')
+        self.calc_reported_sum = self._derive_calc_float(
+            self._REPORTED_SUM_RE, 'calc_reported_sum')
+        self.calc_context_id = self._derive_calc(self._CONTEXT_ID_RE)
+        self.calc_line_item = self._derive_calc(self._LINE_ITEM_RE)
+        unreported_items = self._derive_calc(self._UNREPORTED_ITEMS_RE)
+        self.calc_short_role = self._derive_calc_short_role()
+
+        if unreported_items and unreported_items.lower() != 'none':
+            self.calc_unreported_items = (
+                self._COMMA_RE.split(unreported_items))
+
+    def _derive_calc_short_role(self) -> Union[str, None]:
+        matched_uri = self._derive_calc(self._SHORT_ROLE_RE)
+        if not matched_uri:
+            return None
+
+        uri_path = ''
+        try:
+            parse_res = urllib.parse.urlparse(matched_uri)
+        except ValueError:
+            pass
+        else:
+            uri_path = parse_res.path
+        if not uri_path.strip():
+            return None
+        uri_path = urllib.parse.unquote(uri_path)
+
+        short_role = None
+        try:
+            plib_path = PurePosixPath(uri_path)
+        except ValueError:
+            pass
+        else:
+            short_role = plib_path.name
+        return short_role
+
+    def _derive_duplicate_prefixed_attrs(self):
+        duplicate_1 = self._derive_calc_float(
+            self._DUPLICATE_1_RE, 'duplicate_*')
+        duplicate_2 = self._derive_calc_float(
+            self._DUPLICATE_2_RE, 'duplicate_*')
+        if (isinstance(duplicate_1, float)
+                and isinstance(duplicate_2, float)):
+            self.duplicate_greater = max(duplicate_1, duplicate_2)
+            self.duplicate_lesser = min(duplicate_1, duplicate_2)
```

### Comparing `xbrl_filings_api-1.0.0.dev1/LICENSE.txt` & `xbrl_filings_api-1.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0.0.dev1/pyproject.toml` & `xbrl_filings_api-1.0a1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -43,242 +43,243 @@
 000002a0: 2073 7461 7465 6d65 6e74 2061 6e61 6c79   statement analy
 000002b0: 7369 7322 2c20 2245 7874 656e 7369 626c  sis", "Extensibl
 000002c0: 6520 4275 7369 6e65 7373 2052 6570 6f72  e Business Repor
 000002d0: 7469 6e67 204c 616e 6775 6167 6522 2c0d  ting Language",.
 000002e0: 0a20 2020 2022 4575 726f 7065 616e 2053  .    "European S
 000002f0: 696e 676c 6520 456c 6563 7472 6f6e 6963  ingle Electronic
 00000300: 2046 6f72 6d61 7422 2c0d 0a5d 0d0a 6175   Format",..]..au
-00000310: 7468 6f72 7320 3d20 5b0d 0a20 207b 206e  thors = [..  { n
-00000320: 616d 6520 3d20 224c 6175 7269 2053 616c  ame = "Lauri Sal
-00000330: 6d65 6c61 222c 2065 6d61 696c 203d 2022  mela", email = "
-00000340: 6c61 7572 692e 6d2e 7361 6c6d 656c 6140  lauri.m.salmela@
-00000350: 676d 6169 6c2e 636f 6d22 207d 2c0d 0a5d  gmail.com" },..]
-00000360: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
-00000370: 5b0d 0a20 2020 2022 4465 7665 6c6f 706d  [..    "Developm
-00000380: 656e 7420 5374 6174 7573 203a 3a20 3120  ent Status :: 1 
-00000390: 2d20 506c 616e 6e69 6e67 222c 0d0a 2020  - Planning",..  
-000003a0: 2020 2250 726f 6772 616d 6d69 6e67 204c    "Programming L
-000003b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000003c0: 6e20 3a3a 2033 2e31 3022 2c0d 0a20 2020  n :: 3.10",..   
-000003d0: 2022 5072 6f67 7261 6d6d 696e 6720 4c61   "Programming La
-000003e0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000003f0: 203a 3a20 332e 3131 222c 0d0a 2020 2020   :: 3.11",..    
-00000400: 2250 726f 6772 616d 6d69 6e67 204c 616e  "Programming Lan
-00000410: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000420: 3a3a 2033 2e39 222c 0d0a 2020 2020 2250  :: 3.9",..    "P
-00000430: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000440: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000450: 2049 6d70 6c65 6d65 6e74 6174 696f 6e20   Implementation 
-00000460: 3a3a 2043 5079 7468 6f6e 222c 0d0a 2020  :: CPython",..  
-00000470: 2020 2250 726f 6772 616d 6d69 6e67 204c    "Programming L
-00000480: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000490: 6e22 2c0d 0a20 2020 2022 5072 6f67 7261  n",..    "Progra
-000004a0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000004b0: 3a20 5351 4c22 2c0d 0a20 2020 2022 4f70  : SQL",..    "Op
-000004c0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-000004d0: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-000004e0: 222c 0d0a 2020 2020 2246 7261 6d65 776f  ",..    "Framewo
-000004f0: 726b 203a 3a20 4173 796e 6349 4f22 2c0d  rk :: AsyncIO",.
-00000500: 0a20 2020 2022 4672 616d 6577 6f72 6b20  .    "Framework 
-00000510: 3a3a 2048 6174 6368 222c 0d0a 2020 2020  :: Hatch",..    
-00000520: 2246 7261 6d65 776f 726b 203a 3a20 5079  "Framework :: Py
-00000530: 7465 7374 222c 0d0a 2020 2020 2249 6e74  test",..    "Int
-00000540: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
-00000550: 3a20 4669 6e61 6e63 6961 6c20 616e 6420  : Financial and 
-00000560: 496e 7375 7261 6e63 6520 496e 6475 7374  Insurance Indust
-00000570: 7279 222c 0d0a 2020 2020 2249 6e74 656e  ry",..    "Inten
-00000580: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-00000590: 496e 666f 726d 6174 696f 6e20 5465 6368  Information Tech
-000005a0: 6e6f 6c6f 6779 222c 0d0a 2020 2020 2249  nology",..    "I
-000005b0: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
-000005c0: 203a 3a20 5363 6965 6e63 652f 5265 7365   :: Science/Rese
-000005d0: 6172 6368 222c 0d0a 2020 2020 224c 6963  arch",..    "Lic
-000005e0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-000005f0: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
-00000600: 6e73 6522 2c0d 0a20 2020 2022 546f 7069  nse",..    "Topi
-00000610: 6320 3a3a 2046 696c 6520 466f 726d 6174  c :: File Format
-00000620: 7320 3a3a 204a 534f 4e22 2c0d 0a20 2020  s :: JSON",..   
-00000630: 2022 546f 7069 6320 3a3a 2049 6e74 6572   "Topic :: Inter
-00000640: 6e65 7420 3a3a 2057 5757 2f48 5454 5020  net :: WWW/HTTP 
-00000650: 3a3a 2049 6e64 6578 696e 672f 5365 6172  :: Indexing/Sear
-00000660: 6368 222c 0d0a 2020 2020 2254 6f70 6963  ch",..    "Topic
-00000670: 203a 3a20 4f66 6669 6365 2f42 7573 696e   :: Office/Busin
-00000680: 6573 7320 3a3a 2046 696e 616e 6369 616c  ess :: Financial
-00000690: 222c 0d0a 2020 2020 2254 6f70 6963 203a  ",..    "Topic :
-000006a0: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
-000006b0: 6f70 6d65 6e74 203a 3a20 4c69 6272 6172  opment :: Librar
-000006c0: 6965 7322 2c0d 0a5d 0d0a 6465 7065 6e64  ies",..]..depend
-000006d0: 656e 6369 6573 203d 205b 0d0a 2020 2020  encies = [..    
-000006e0: 2272 6571 7565 7374 7322 2c0d 0a5d 0d0a  "requests",..]..
-000006f0: 0d0a 5b70 726f 6a65 6374 2e75 726c 735d  ..[project.urls]
-00000700: 0d0a 486f 6d65 7061 6765 203d 2022 6874  ..Homepage = "ht
-00000710: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000720: 2f6c 7361 6c6d 656c 612f 7862 726c 2d66  /lsalmela/xbrl-f
-00000730: 696c 696e 6773 2d61 7069 220d 0a44 6f63  ilings-api"..Doc
-00000740: 756d 656e 7461 7469 6f6e 203d 2022 6874  umentation = "ht
-00000750: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000760: 2f6c 7361 6c6d 656c 612f 7862 726c 2d66  /lsalmela/xbrl-f
-00000770: 696c 696e 6773 2d61 7069 2372 6561 646d  ilings-api#readm
-00000780: 6522 0d0a 536f 7572 6365 203d 2022 6874  e"..Source = "ht
-00000790: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000007a0: 2f6c 7361 6c6d 656c 612f 7862 726c 2d66  /lsalmela/xbrl-f
-000007b0: 696c 696e 6773 2d61 7069 220d 0a49 7373  ilings-api"..Iss
-000007c0: 7565 7320 3d20 2268 7474 7073 3a2f 2f67  ues = "https://g
-000007d0: 6974 6875 622e 636f 6d2f 6c73 616c 6d65  ithub.com/lsalme
-000007e0: 6c61 2f78 6272 6c2d 6669 6c69 6e67 732d  la/xbrl-filings-
-000007f0: 6170 692f 6973 7375 6573 220d 0a0d 0a5b  api/issues"....[
-00000800: 746f 6f6c 2e68 6174 6368 2e76 6572 7369  tool.hatch.versi
-00000810: 6f6e 5d0d 0a70 6174 6820 3d20 2278 6272  on]..path = "xbr
-00000820: 6c5f 6669 6c69 6e67 735f 6170 692f 5f5f  l_filings_api/__
-00000830: 6162 6f75 745f 5f2e 7079 220d 0a0d 0a5b  about__.py"....[
-00000840: 746f 6f6c 2e68 6174 6368 2e62 7569 6c64  tool.hatch.build
-00000850: 2e74 6172 6765 7473 2e73 6469 7374 5d0d  .targets.sdist].
-00000860: 0a65 7863 6c75 6465 203d 205b 0d0a 2020  .exclude = [..  
-00000870: 222f 2e67 6974 6875 6222 2c0d 0a20 2022  "/.github",..  "
-00000880: 2f64 6f63 7322 2c0d 0a5d 0d0a 0d0a 5b74  /docs",..]....[t
-00000890: 6f6f 6c2e 6861 7463 682e 6275 696c 642e  ool.hatch.build.
-000008a0: 7461 7267 6574 732e 7768 6565 6c5d 0d0a  targets.wheel]..
-000008b0: 7061 636b 6167 6573 203d 205b 2278 6272  packages = ["xbr
-000008c0: 6c5f 6669 6c69 6e67 735f 6170 6922 5d0d  l_filings_api"].
-000008d0: 0a0d 0a5b 746f 6f6c 2e68 6174 6368 2e65  ...[tool.hatch.e
-000008e0: 6e76 732e 6465 6661 756c 745d 0d0a 6465  nvs.default]..de
-000008f0: 7065 6e64 656e 6369 6573 203d 205b 0d0a  pendencies = [..
-00000900: 2020 2263 6f76 6572 6167 655b 746f 6d6c    "coverage[toml
-00000910: 5d3e 3d36 2e35 222c 0d0a 2020 2270 7974  ]>=6.5",..  "pyt
-00000920: 6573 7422 2c0d 0a20 2022 7265 7370 6f6e  est",..  "respon
-00000930: 7365 7322 2c0d 0a5d 0d0a 5b74 6f6f 6c2e  ses",..]..[tool.
-00000940: 6861 7463 682e 656e 7673 2e64 6566 6175  hatch.envs.defau
-00000950: 6c74 2e73 6372 6970 7473 5d0d 0a74 6573  lt.scripts]..tes
-00000960: 7420 3d20 2270 7974 6573 7420 7b61 7267  t = "pytest {arg
-00000970: 733a 7465 7374 737d 220d 0a74 6573 742d  s:tests}"..test-
-00000980: 636f 7620 3d20 2263 6f76 6572 6167 6520  cov = "coverage 
-00000990: 7275 6e20 2d6d 2070 7974 6573 7420 7b61  run -m pytest {a
-000009a0: 7267 733a 7465 7374 737d 220d 0a63 6f76  rgs:tests}"..cov
-000009b0: 2d72 6570 6f72 7420 3d20 5b0d 0a20 2022  -report = [..  "
-000009c0: 2d20 636f 7665 7261 6765 2063 6f6d 6269  - coverage combi
-000009d0: 6e65 222c 0d0a 2020 2263 6f76 6572 6167  ne",..  "coverag
-000009e0: 6520 7265 706f 7274 222c 0d0a 5d0d 0a63  e report",..]..c
-000009f0: 6f76 203d 205b 0d0a 2020 2274 6573 742d  ov = [..  "test-
-00000a00: 636f 7622 2c0d 0a20 2022 636f 762d 7265  cov",..  "cov-re
-00000a10: 706f 7274 222c 0d0a 5d0d 0a0d 0a5b 5b74  port",..]....[[t
-00000a20: 6f6f 6c2e 6861 7463 682e 656e 7673 2e61  ool.hatch.envs.a
-00000a30: 6c6c 2e6d 6174 7269 785d 5d0d 0a70 7974  ll.matrix]]..pyt
-00000a40: 686f 6e20 3d20 5b22 332e 3922 2c20 2233  hon = ["3.9", "3
-00000a50: 2e31 3022 2c20 2233 2e31 3122 5d0d 0a0d  .10", "3.11"]...
-00000a60: 0a5b 746f 6f6c 2e68 6174 6368 2e65 6e76  .[tool.hatch.env
-00000a70: 732e 6c69 6e74 5d0d 0a64 6574 6163 6865  s.lint]..detache
-00000a80: 6420 3d20 7472 7565 0d0a 6465 7065 6e64  d = true..depend
-00000a90: 656e 6369 6573 203d 205b 0d0a 2020 2262  encies = [..  "b
-00000aa0: 6c61 636b 3e3d 3233 2e37 2e30 222c 0d0a  lack>=23.7.0",..
-00000ab0: 2020 226d 7970 793e 3d31 2e35 2e31 222c    "mypy>=1.5.1",
-00000ac0: 0d0a 2020 2272 7566 663e 3d30 2e30 2e32  ..  "ruff>=0.0.2
-00000ad0: 3835 222c 0d0a 5d0d 0a5b 746f 6f6c 2e68  85",..]..[tool.h
-00000ae0: 6174 6368 2e65 6e76 732e 6c69 6e74 2e73  atch.envs.lint.s
-00000af0: 6372 6970 7473 5d0d 0a74 7970 696e 6720  cripts]..typing 
-00000b00: 3d20 226d 7970 7920 2d2d 696e 7374 616c  = "mypy --instal
-00000b10: 6c2d 7479 7065 7320 2d2d 6e6f 6e2d 696e  l-types --non-in
-00000b20: 7465 7261 6374 6976 6520 7b61 7267 733a  teractive {args:
-00000b30: 7862 726c 5f66 696c 696e 6773 5f61 7069  xbrl_filings_api
-00000b40: 2074 6573 7473 7d22 0d0a 7374 796c 6520   tests}"..style 
-00000b50: 3d20 5b0d 0a20 2022 7275 6666 207b 6172  = [..  "ruff {ar
-00000b60: 6773 3a2e 7d22 2c0d 0a20 2022 626c 6163  gs:.}",..  "blac
-00000b70: 6b20 2d2d 6368 6563 6b20 2d2d 6469 6666  k --check --diff
-00000b80: 207b 6172 6773 3a2e 7d22 2c0d 0a5d 0d0a   {args:.}",..]..
-00000b90: 666d 7420 3d20 5b0d 0a20 2022 626c 6163  fmt = [..  "blac
-00000ba0: 6b20 7b61 7267 733a 2e7d 222c 0d0a 2020  k {args:.}",..  
-00000bb0: 2272 7566 6620 2d2d 6669 7820 7b61 7267  "ruff --fix {arg
-00000bc0: 733a 2e7d 222c 0d0a 2020 2273 7479 6c65  s:.}",..  "style
-00000bd0: 222c 0d0a 5d0d 0a61 6c6c 203d 205b 0d0a  ",..]..all = [..
-00000be0: 2020 2273 7479 6c65 222c 0d0a 2020 2274    "style",..  "t
-00000bf0: 7970 696e 6722 2c0d 0a5d 0d0a 0d0a 5b74  yping",..]....[t
-00000c00: 6f6f 6c2e 626c 6163 6b5d 0d0a 7461 7267  ool.black]..targ
-00000c10: 6574 2d76 6572 7369 6f6e 203d 205b 2270  et-version = ["p
-00000c20: 7933 3922 5d0d 0a6c 696e 652d 6c65 6e67  y39"]..line-leng
-00000c30: 7468 203d 2037 390d 0a73 6b69 702d 7374  th = 79..skip-st
-00000c40: 7269 6e67 2d6e 6f72 6d61 6c69 7a61 7469  ring-normalizati
-00000c50: 6f6e 203d 2074 7275 650d 0a0d 0a5b 746f  on = true....[to
-00000c60: 6f6c 2e72 7566 665d 0d0a 7461 7267 6574  ol.ruff]..target
-00000c70: 2d76 6572 7369 6f6e 203d 2022 7079 3339  -version = "py39
-00000c80: 220d 0a6c 696e 652d 6c65 6e67 7468 203d  "..line-length =
-00000c90: 2037 390d 0a73 656c 6563 7420 3d20 5b0d   79..select = [.
-00000ca0: 0a20 2022 4122 2c0d 0a20 2022 4152 4722  .  "A",..  "ARG"
-00000cb0: 2c0d 0a20 2022 4222 2c0d 0a20 2022 4322  ,..  "B",..  "C"
-00000cc0: 2c0d 0a20 2022 4454 5a22 2c0d 0a20 2022  ,..  "DTZ",..  "
-00000cd0: 4522 2c0d 0a20 2022 454d 222c 0d0a 2020  E",..  "EM",..  
-00000ce0: 2246 222c 0d0a 2020 2246 4254 222c 0d0a  "F",..  "FBT",..
-00000cf0: 2020 2249 222c 0d0a 2020 2249 434e 222c    "I",..  "ICN",
-00000d00: 0d0a 2020 2249 5343 222c 0d0a 2020 224e  ..  "ISC",..  "N
-00000d10: 222c 0d0a 2020 2250 4c43 222c 0d0a 2020  ",..  "PLC",..  
-00000d20: 2250 4c45 222c 0d0a 2020 2250 4c52 222c  "PLE",..  "PLR",
-00000d30: 0d0a 2020 2250 4c57 222c 0d0a 2020 2251  ..  "PLW",..  "Q
-00000d40: 222c 0d0a 2020 2252 5546 222c 0d0a 2020  ",..  "RUF",..  
-00000d50: 2253 222c 0d0a 2020 2254 222c 0d0a 2020  "S",..  "T",..  
-00000d60: 2254 4944 222c 0d0a 2020 2255 5022 2c0d  "TID",..  "UP",.
-00000d70: 0a20 2022 5722 2c0d 0a20 2022 5954 5422  .  "W",..  "YTT"
-00000d80: 2c0d 0a5d 0d0a 6967 6e6f 7265 203d 205b  ,..]..ignore = [
-00000d90: 0d0a 2020 2320 416c 6c6f 7720 6e6f 6e2d  ..  # Allow non-
-00000da0: 6162 7374 7261 6374 2065 6d70 7479 206d  abstract empty m
-00000db0: 6574 686f 6473 2069 6e20 6162 7374 7261  ethods in abstra
-00000dc0: 6374 2062 6173 6520 636c 6173 7365 730d  ct base classes.
-00000dd0: 0a20 2022 4230 3237 222c 0d0a 2020 2320  .  "B027",..  # 
-00000de0: 416c 6c6f 7720 626f 6f6c 6561 6e20 706f  Allow boolean po
-00000df0: 7369 7469 6f6e 616c 2076 616c 7565 7320  sitional values 
-00000e00: 696e 2066 756e 6374 696f 6e20 6361 6c6c  in function call
-00000e10: 732c 206c 696b 6520 6064 6963 742e 6765  s, like `dict.ge
-00000e20: 7428 2e2e 2e20 5472 7565 2960 0d0a 2020  t(... True)`..  
-00000e30: 2246 4254 3030 3322 2c0d 0a20 2023 2049  "FBT003",..  # I
-00000e40: 676e 6f72 6520 6368 6563 6b73 2066 6f72  gnore checks for
-00000e50: 2070 6f73 7369 626c 6520 7061 7373 776f   possible passwo
-00000e60: 7264 730d 0a20 2022 5331 3035 222c 2022  rds..  "S105", "
-00000e70: 5331 3036 222c 2022 5331 3037 222c 0d0a  S106", "S107",..
-00000e80: 2020 2320 4967 6e6f 7265 2063 6f6d 706c    # Ignore compl
-00000e90: 6578 6974 790d 0a20 2022 4339 3031 222c  exity..  "C901",
-00000ea0: 2022 504c 5230 3931 3122 2c20 2250 4c52   "PLR0911", "PLR
-00000eb0: 3039 3132 222c 2022 504c 5230 3931 3322  0912", "PLR0913"
-00000ec0: 2c20 2250 4c52 3039 3135 222c 0d0a 5d0d  , "PLR0915",..].
-00000ed0: 0a75 6e66 6978 6162 6c65 203d 205b 0d0a  .unfixable = [..
-00000ee0: 2020 2320 446f 6e27 7420 746f 7563 6820    # Don't touch 
-00000ef0: 756e 7573 6564 2069 6d70 6f72 7473 0d0a  unused imports..
-00000f00: 2020 2246 3430 3122 2c0d 0a5d 0d0a 0d0a    "F401",..]....
-00000f10: 5b74 6f6f 6c2e 7275 6666 2e69 736f 7274  [tool.ruff.isort
-00000f20: 5d0d 0a6b 6e6f 776e 2d66 6972 7374 2d70  ]..known-first-p
-00000f30: 6172 7479 203d 205b 2278 6272 6c5f 6669  arty = ["xbrl_fi
-00000f40: 6c69 6e67 735f 6170 6922 5d0d 0a0d 0a5b  lings_api"]....[
-00000f50: 746f 6f6c 2e72 7566 662e 666c 616b 6538  tool.ruff.flake8
-00000f60: 2d74 6964 792d 696d 706f 7274 735d 0d0a  -tidy-imports]..
-00000f70: 6261 6e2d 7265 6c61 7469 7665 2d69 6d70  ban-relative-imp
-00000f80: 6f72 7473 203d 2022 616c 6c22 0d0a 0d0a  orts = "all"....
-00000f90: 5b74 6f6f 6c2e 7275 6666 2e70 6572 2d66  [tool.ruff.per-f
-00000fa0: 696c 652d 6967 6e6f 7265 735d 0d0a 2320  ile-ignores]..# 
-00000fb0: 5465 7374 7320 6361 6e20 7573 6520 6d61  Tests can use ma
-00000fc0: 6769 6320 7661 6c75 6573 2c20 6173 7365  gic values, asse
-00000fd0: 7274 696f 6e73 2c20 616e 6420 7265 6c61  rtions, and rela
-00000fe0: 7469 7665 2069 6d70 6f72 7473 0d0a 2274  tive imports.."t
-00000ff0: 6573 7473 2f2a 2a2f 2a22 203d 205b 2250  ests/**/*" = ["P
-00001000: 4c52 3230 3034 222c 2022 5331 3031 222c  LR2004", "S101",
-00001010: 2022 5449 4432 3532 225d 0d0a 0d0a 5b74   "TID252"]....[t
-00001020: 6f6f 6c2e 636f 7665 7261 6765 2e72 756e  ool.coverage.run
-00001030: 5d0d 0a73 6f75 7263 655f 706b 6773 203d  ]..source_pkgs =
-00001040: 205b 2278 6272 6c5f 6669 6c69 6e67 735f   ["xbrl_filings_
-00001050: 6170 6922 2c20 2274 6573 7473 225d 0d0a  api", "tests"]..
-00001060: 6272 616e 6368 203d 2074 7275 650d 0a70  branch = true..p
-00001070: 6172 616c 6c65 6c20 3d20 7472 7565 0d0a  arallel = true..
-00001080: 6f6d 6974 203d 205b 0d0a 2020 2278 6272  omit = [..  "xbr
-00001090: 6c5f 6669 6c69 6e67 735f 6170 692f 5f5f  l_filings_api/__
-000010a0: 6162 6f75 745f 5f2e 7079 222c 0d0a 5d0d  about__.py",..].
-000010b0: 0a0d 0a5b 746f 6f6c 2e63 6f76 6572 6167  ...[tool.coverag
-000010c0: 652e 7061 7468 735d 0d0a 7862 726c 5f66  e.paths]..xbrl_f
-000010d0: 696c 696e 6773 5f61 7069 203d 205b 2278  ilings_api = ["x
-000010e0: 6272 6c5f 6669 6c69 6e67 735f 6170 6922  brl_filings_api"
-000010f0: 2c20 222a 2f78 6272 6c2d 6669 6c69 6e67  , "*/xbrl-filing
-00001100: 732d 6170 692f 7862 726c 5f66 696c 696e  s-api/xbrl_filin
-00001110: 6773 5f61 7069 225d 0d0a 7465 7374 7320  gs_api"]..tests 
-00001120: 3d20 5b22 7465 7374 7322 2c20 222a 2f78  = ["tests", "*/x
-00001130: 6272 6c2d 6669 6c69 6e67 732d 6170 692f  brl-filings-api/
-00001140: 7465 7374 7322 5d0d 0a0d 0a5b 746f 6f6c  tests"]....[tool
-00001150: 2e63 6f76 6572 6167 652e 7265 706f 7274  .coverage.report
-00001160: 5d0d 0a65 7863 6c75 6465 5f6c 696e 6573  ]..exclude_lines
-00001170: 203d 205b 0d0a 2020 226e 6f20 636f 7622   = [..  "no cov"
-00001180: 2c0d 0a20 2022 6966 205f 5f6e 616d 655f  ,..  "if __name_
-00001190: 5f20 3d3d 202e 5f5f 6d61 696e 5f5f 2e3a  _ == .__main__.:
-000011a0: 222c 0d0a 2020 2269 6620 5459 5045 5f43  ",..  "if TYPE_C
-000011b0: 4845 434b 494e 473a 222c 0d0a 5d0d 0a    HECKING:",..]..
+00000310: 7468 6f72 7320 3d20 5b0d 0a20 2020 207b  thors = [..    {
+00000320: 206e 616d 6520 3d20 224c 6175 7269 2053   name = "Lauri S
+00000330: 616c 6d65 6c61 222c 2065 6d61 696c 203d  almela", email =
+00000340: 2022 6c61 7572 692e 6d2e 7361 6c6d 656c   "lauri.m.salmel
+00000350: 6140 676d 6169 6c2e 636f 6d22 207d 2c0d  a@gmail.com" },.
+00000360: 0a5d 0d0a 636c 6173 7369 6669 6572 7320  .]..classifiers 
+00000370: 3d20 5b0d 0a20 2020 2022 4465 7665 6c6f  = [..    "Develo
+00000380: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
+00000390: 3320 2d20 416c 7068 6122 2c0d 0a20 2020  3 - Alpha",..   
+000003a0: 2022 5072 6f67 7261 6d6d 696e 6720 4c61   "Programming La
+000003b0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000003c0: 203a 3a20 332e 3922 2c0d 0a20 2020 2022   :: 3.9",..    "
+000003d0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000003e0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000003f0: 3a20 332e 3130 222c 0d0a 2020 2020 2250  : 3.10",..    "P
+00000400: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000410: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000420: 2033 2e31 3122 2c0d 0a20 2020 2022 5072   3.11",..    "Pr
+00000430: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000440: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000450: 332e 3132 222c 0d0a 2020 2020 2250 726f  3.12",..    "Pro
+00000460: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000470: 6520 3a3a 2050 7974 686f 6e20 3a3a 2049  e :: Python :: I
+00000480: 6d70 6c65 6d65 6e74 6174 696f 6e20 3a3a  mplementation ::
+00000490: 2043 5079 7468 6f6e 222c 0d0a 2020 2020   CPython",..    
+000004a0: 2250 726f 6772 616d 6d69 6e67 204c 616e  "Programming Lan
+000004b0: 6775 6167 6520 3a3a 2050 7974 686f 6e22  guage :: Python"
+000004c0: 2c0d 0a20 2020 2022 5072 6f67 7261 6d6d  ,..    "Programm
+000004d0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000004e0: 5351 4c22 2c0d 0a20 2020 2022 4f70 6572  SQL",..    "Oper
+000004f0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+00000500: 4f53 2049 6e64 6570 656e 6465 6e74 222c  OS Independent",
+00000510: 0d0a 2020 2020 2249 6e74 656e 6465 6420  ..    "Intended 
+00000520: 4175 6469 656e 6365 203a 3a20 4669 6e61  Audience :: Fina
+00000530: 6e63 6961 6c20 616e 6420 496e 7375 7261  ncial and Insura
+00000540: 6e63 6520 496e 6475 7374 7279 222c 0d0a  nce Industry",..
+00000550: 2020 2020 2249 6e74 656e 6465 6420 4175      "Intended Au
+00000560: 6469 656e 6365 203a 3a20 496e 666f 726d  dience :: Inform
+00000570: 6174 696f 6e20 5465 6368 6e6f 6c6f 6779  ation Technology
+00000580: 222c 0d0a 2020 2020 2249 6e74 656e 6465  ",..    "Intende
+00000590: 6420 4175 6469 656e 6365 203a 3a20 5363  d Audience :: Sc
+000005a0: 6965 6e63 652f 5265 7365 6172 6368 222c  ience/Research",
+000005b0: 0d0a 2020 2020 224c 6963 656e 7365 203a  ..    "License :
+000005c0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+000005d0: 3a20 4d49 5420 4c69 6365 6e73 6522 2c0d  : MIT License",.
+000005e0: 0a20 2020 2022 546f 7069 6320 3a3a 2046  .    "Topic :: F
+000005f0: 696c 6520 466f 726d 6174 7320 3a3a 204a  ile Formats :: J
+00000600: 534f 4e22 2c0d 0a20 2020 2022 546f 7069  SON",..    "Topi
+00000610: 6320 3a3a 2049 6e74 6572 6e65 7420 3a3a  c :: Internet ::
+00000620: 2057 5757 2f48 5454 5020 3a3a 2049 6e64   WWW/HTTP :: Ind
+00000630: 6578 696e 672f 5365 6172 6368 222c 0d0a  exing/Search",..
+00000640: 2020 2020 2254 6f70 6963 203a 3a20 4f66      "Topic :: Of
+00000650: 6669 6365 2f42 7573 696e 6573 7320 3a3a  fice/Business ::
+00000660: 2046 696e 616e 6369 616c 222c 0d0a 2020   Financial",..  
+00000670: 2020 2254 6f70 6963 203a 3a20 536f 6674    "Topic :: Soft
+00000680: 7761 7265 2044 6576 656c 6f70 6d65 6e74  ware Development
+00000690: 203a 3a20 4c69 6272 6172 6965 7322 2c0d   :: Libraries",.
+000006a0: 0a5d 0d0a 6465 7065 6e64 656e 6369 6573  .]..dependencies
+000006b0: 203d 205b 0d0a 2020 2020 2272 6571 7565   = [..    "reque
+000006c0: 7374 7322 2c0d 0a5d 0d0a 0d0a 5b70 726f  sts",..]....[pro
+000006d0: 6a65 6374 2e75 726c 735d 0d0a 486f 6d65  ject.urls]..Home
+000006e0: 7061 6765 203d 2022 6874 7470 733a 2f2f  page = "https://
+000006f0: 6769 7468 7562 2e63 6f6d 2f6c 7361 6c6d  github.com/lsalm
+00000700: 656c 612f 7862 726c 2d66 696c 696e 6773  ela/xbrl-filings
+00000710: 2d61 7069 220d 0a44 6f63 756d 656e 7461  -api"..Documenta
+00000720: 7469 6f6e 203d 2022 6874 7470 733a 2f2f  tion = "https://
+00000730: 6c73 616c 6d65 6c61 2e67 6974 6875 622e  lsalmela.github.
+00000740: 696f 2f78 6272 6c2d 6669 6c69 6e67 732d  io/xbrl-filings-
+00000750: 6170 6922 0d0a 536f 7572 6365 203d 2022  api"..Source = "
+00000760: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000770: 6f6d 2f6c 7361 6c6d 656c 612f 7862 726c  om/lsalmela/xbrl
+00000780: 2d66 696c 696e 6773 2d61 7069 220d 0a49  -filings-api"..I
+00000790: 7373 7565 7320 3d20 2268 7474 7073 3a2f  ssues = "https:/
+000007a0: 2f67 6974 6875 622e 636f 6d2f 6c73 616c  /github.com/lsal
+000007b0: 6d65 6c61 2f78 6272 6c2d 6669 6c69 6e67  mela/xbrl-filing
+000007c0: 732d 6170 692f 6973 7375 6573 220d 0a0d  s-api/issues"...
+000007d0: 0a5b 746f 6f6c 2e68 6174 6368 2e76 6572  .[tool.hatch.ver
+000007e0: 7369 6f6e 5d0d 0a70 6174 6820 3d20 2278  sion]..path = "x
+000007f0: 6272 6c5f 6669 6c69 6e67 735f 6170 692f  brl_filings_api/
+00000800: 5f5f 6162 6f75 745f 5f2e 7079 220d 0a0d  __about__.py"...
+00000810: 0a5b 746f 6f6c 2e68 6174 6368 2e62 7569  .[tool.hatch.bui
+00000820: 6c64 2e74 6172 6765 7473 2e73 6469 7374  ld.targets.sdist
+00000830: 5d0d 0a65 7863 6c75 6465 203d 205b 0d0a  ]..exclude = [..
+00000840: 2020 2020 222f 2e67 6974 6875 6222 2c0d      "/.github",.
+00000850: 0a20 2020 2022 2f74 6573 7473 2f6d 6f63  .    "/tests/moc
+00000860: 6b5f 7265 7370 6f6e 7365 732f 2a22 2c0d  k_responses/*",.
+00000870: 0a20 2020 2022 2f64 6f63 7322 2c0d 0a5d  .    "/docs",..]
+00000880: 0d0a 0d0a 5b74 6f6f 6c2e 6861 7463 682e  ....[tool.hatch.
+00000890: 6275 696c 642e 7461 7267 6574 732e 7768  build.targets.wh
+000008a0: 6565 6c5d 0d0a 7061 636b 6167 6573 203d  eel]..packages =
+000008b0: 205b 2278 6272 6c5f 6669 6c69 6e67 735f   ["xbrl_filings_
+000008c0: 6170 6922 5d0d 0a0d 0a5b 746f 6f6c 2e68  api"]....[tool.h
+000008d0: 6174 6368 2e65 6e76 732e 6465 6661 756c  atch.envs.defaul
+000008e0: 745d 0d0a 6465 7065 6e64 656e 6369 6573  t]..dependencies
+000008f0: 203d 205b 0d0a 2020 2020 2263 6f76 6572   = [..    "cover
+00000900: 6167 655b 746f 6d6c 5d3e 3d37 2e34 222c  age[toml]>=7.4",
+00000910: 0d0a 2020 2020 2270 7974 6573 743e 3d37  ..    "pytest>=7
+00000920: 2e34 222c 0d0a 2020 2020 2320 4173 206f  .4",..    # As o
+00000930: 6620 7079 7465 7374 5f61 7379 6e63 696f  f pytest_asyncio
+00000940: 2030 2e32 332e 352c 2069 7420 7365 656d   0.23.5, it seem
+00000950: 7320 6e6f 7420 746f 2062 6520 706f 7373  s not to be poss
+00000960: 6962 6c65 2074 6f20 6765 7420 7269 6420  ible to get rid 
+00000970: 6f66 0d0a 2020 2020 2320 6c6f 6767 6564  of..    # logged
+00000980: 2077 6172 6e69 6e67 2022 4465 7072 6563   warning "Deprec
+00000990: 6174 696f 6e57 6172 6e69 6e67 3a20 5468  ationWarning: Th
+000009a0: 6572 6520 6973 206e 6f20 6375 7272 656e  ere is no curren
+000009b0: 7420 6576 656e 7420 6c6f 6f70 220d 0a20  t event loop".. 
+000009c0: 2020 2022 7079 7465 7374 2d61 7379 6e63     "pytest-async
+000009d0: 696f 3e3d 302e 3233 2e35 222c 0d0a 2020  io>=0.23.5",..  
+000009e0: 2020 2272 6573 706f 6e73 6573 7e3d 302e    "responses~=0.
+000009f0: 3233 2e33 222c 2023 2055 7369 6e67 2062  23.3", # Using b
+00000a00: 6574 6120 6665 6174 7572 6573 2028 7265  eta features (re
+00000a10: 636f 7264 6572 290d 0a20 2020 2022 7061  corder)..    "pa
+00000a20: 6e64 6173 3e3d 322e 312e 3422 2c0d 0a5d  ndas>=2.1.4",..]
+00000a30: 0d0a 0d0a 5b74 6f6f 6c2e 6861 7463 682e  ....[tool.hatch.
+00000a40: 656e 7673 2e64 6566 6175 6c74 2e73 6372  envs.default.scr
+00000a50: 6970 7473 5d0d 0a74 6573 7420 3d20 2270  ipts]..test = "p
+00000a60: 7974 6573 7420 7b61 7267 733a 7465 7374  ytest {args:test
+00000a70: 737d 220d 0a74 6573 742d 636f 7620 3d20  s}"..test-cov = 
+00000a80: 2263 6f76 6572 6167 6520 7275 6e20 2d6d  "coverage run -m
+00000a90: 2070 7974 6573 7420 7b61 7267 733a 7465   pytest {args:te
+00000aa0: 7374 737d 220d 0a63 6f76 2d72 6570 6f72  sts}"..cov-repor
+00000ab0: 7420 3d20 5b0d 0a20 2020 2022 2d20 636f  t = [..    "- co
+00000ac0: 7665 7261 6765 2063 6f6d 6269 6e65 222c  verage combine",
+00000ad0: 0d0a 2020 2020 2263 6f76 6572 6167 6520  ..    "coverage 
+00000ae0: 7265 706f 7274 222c 0d0a 5d0d 0a63 6f76  report",..]..cov
+00000af0: 203d 205b 0d0a 2020 2020 2274 6573 742d   = [..    "test-
+00000b00: 636f 7622 2c0d 0a20 2020 2022 636f 762d  cov",..    "cov-
+00000b10: 7265 706f 7274 222c 0d0a 5d0d 0a0d 0a5b  report",..]....[
+00000b20: 5b74 6f6f 6c2e 6861 7463 682e 656e 7673  [tool.hatch.envs
+00000b30: 2e61 6c6c 2e6d 6174 7269 785d 5d0d 0a70  .all.matrix]]..p
+00000b40: 7974 686f 6e20 3d20 5b22 332e 3922 2c20  ython = ["3.9", 
+00000b50: 2233 2e31 3022 2c20 2233 2e31 3122 2c20  "3.10", "3.11", 
+00000b60: 2233 2e31 3222 5d0d 0a0d 0a5b 746f 6f6c  "3.12"]....[tool
+00000b70: 2e68 6174 6368 2e65 6e76 732e 6c69 6e74  .hatch.envs.lint
+00000b80: 5d0d 0a64 6574 6163 6865 6420 3d20 7472  ]..detached = tr
+00000b90: 7565 0d0a 6465 7065 6e64 656e 6369 6573  ue..dependencies
+00000ba0: 203d 205b 0d0a 2020 2020 226d 7970 793e   = [..    "mypy>
+00000bb0: 3d31 2e35 2e31 222c 0d0a 5d0d 0a0d 0a5b  =1.5.1",..]....[
+00000bc0: 746f 6f6c 2e68 6174 6368 2e65 6e76 732e  tool.hatch.envs.
+00000bd0: 6c69 6e74 2e73 6372 6970 7473 5d0d 0a74  lint.scripts]..t
+00000be0: 7970 696e 6720 3d20 226d 7970 7920 2d2d  yping = "mypy --
+00000bf0: 696e 7374 616c 6c2d 7479 7065 7320 2d2d  install-types --
+00000c00: 6e6f 6e2d 696e 7465 7261 6374 6976 6520  non-interactive 
+00000c10: 7b61 7267 733a 7862 726c 5f66 696c 696e  {args:xbrl_filin
+00000c20: 6773 5f61 7069 7d22 0d0a 616c 6c20 3d20  gs_api}"..all = 
+00000c30: 5b0d 0a20 2020 2022 6861 7463 6820 666d  [..    "hatch fm
+00000c40: 7420 2d6c 222c 0d0a 2020 2020 2274 7970  t -l",..    "typ
+00000c50: 696e 6722 2c0d 0a5d 0d0a 0d0a 5b74 6f6f  ing",..]....[too
+00000c60: 6c2e 6861 7463 682e 656e 7673 2e64 6f63  l.hatch.envs.doc
+00000c70: 5d0d 0a64 6570 656e 6465 6e63 6965 7320  ]..dependencies 
+00000c80: 3d20 5b0d 0a20 2020 2022 7370 6869 6e78  = [..    "sphinx
+00000c90: 3e3d 372e 322e 3622 2c0d 0a20 2020 2022  >=7.2.6",..    "
+00000ca0: 6675 726f 3e3d 3230 3234 2e31 2e32 3922  furo>=2024.1.29"
+00000cb0: 2c0d 0a20 2020 2022 7370 6869 6e78 6578  ,..    "sphinxex
+00000cc0: 742d 6f70 656e 6772 6170 683e 3d30 2e39  t-opengraph>=0.9
+00000cd0: 2e31 222c 0d0a 2020 2020 2273 7068 696e  .1",..    "sphin
+00000ce0: 782d 636f 7079 6275 7474 6f6e 3e3d 302e  x-copybutton>=0.
+00000cf0: 352e 3222 2c0d 0a5d 0d0a 0d0a 5b74 6f6f  5.2",..]....[too
+00000d00: 6c2e 6861 7463 682e 656e 7673 2e64 6f63  l.hatch.envs.doc
+00000d10: 2e73 6372 6970 7473 5d0d 0a62 7569 6c64  .scripts]..build
+00000d20: 203d 2022 7370 6869 6e78 2d62 7569 6c64   = "sphinx-build
+00000d30: 207b 6172 6773 7d20 646f 6373 2f73 6f75   {args} docs/sou
+00000d40: 7263 6520 646f 6373 2f62 7569 6c64 220d  rce docs/build".
+00000d50: 0a23 2057 696e 646f 7773 2d73 7065 6369  .# Windows-speci
+00000d60: 6669 630d 0a64 656c 6765 6e20 3d20 2772  fic..delgen = 'r
+00000d70: 6d64 6972 202f 7320 2f71 2022 646f 6373  mdir /s /q "docs
+00000d80: 5c73 6f75 7263 655c 6170 6922 2022 646f  \source\api" "do
+00000d90: 6373 5c73 6f75 7263 655c 6465 765c 7265  cs\source\dev\re
+00000da0: 6622 2022 646f 6373 5c62 7569 6c64 2227  f" "docs\build"'
+00000db0: 0d0a 6662 7569 6c64 203d 205b 0d0a 2020  ..fbuild = [..  
+00000dc0: 2020 2264 656c 6765 6e22 2c0d 0a20 2020    "delgen",..   
+00000dd0: 2022 6275 696c 6422 2c0d 0a20 2020 205d   "build",..    ]
+00000de0: 0d0a 6c69 6e6b 6368 6563 6b20 3d20 5b0d  ..linkcheck = [.
+00000df0: 0a20 2020 2022 7370 6869 6e78 2d62 7569  .    "sphinx-bui
+00000e00: 6c64 202d 6220 6c69 6e6b 6368 6563 6b20  ld -b linkcheck 
+00000e10: 7b61 7267 737d 2064 6f63 732f 736f 7572  {args} docs/sour
+00000e20: 6365 2064 6f63 732f 6275 696c 642f 6c69  ce docs/build/li
+00000e30: 6e6b 6368 6563 6b22 2c0d 0a20 2020 2022  nkcheck",..    "
+00000e40: 646f 6373 2f62 7569 6c64 2f6c 696e 6b63  docs/build/linkc
+00000e50: 6865 636b 2f6f 7574 7075 742e 7478 7422  heck/output.txt"
+00000e60: 2c0d 0a20 2020 205d 0d0a 0d0a 5b74 6f6f  ,..    ]....[too
+00000e70: 6c2e 636f 7665 7261 6765 2e72 756e 5d0d  l.coverage.run].
+00000e80: 0a73 6f75 7263 655f 706b 6773 203d 205b  .source_pkgs = [
+00000e90: 2278 6272 6c5f 6669 6c69 6e67 735f 6170  "xbrl_filings_ap
+00000ea0: 6922 2c20 2274 6573 7473 225d 0d0a 6272  i", "tests"]..br
+00000eb0: 616e 6368 203d 2074 7275 650d 0a70 6172  anch = true..par
+00000ec0: 616c 6c65 6c20 3d20 7472 7565 0d0a 6f6d  allel = true..om
+00000ed0: 6974 203d 205b 0d0a 2020 2020 2278 6272  it = [..    "xbr
+00000ee0: 6c5f 6669 6c69 6e67 735f 6170 692f 5f5f  l_filings_api/__
+00000ef0: 6162 6f75 745f 5f2e 7079 222c 0d0a 2020  about__.py",..  
+00000f00: 2020 2274 6573 7473 2f63 6f6e 6674 6573    "tests/conftes
+00000f10: 745f 736f 7572 6365 2e70 7922 2c0d 0a20  t_source.py",.. 
+00000f20: 2020 2022 7465 7374 732f 6d6f 636b 5f75     "tests/mock_u
+00000f30: 7067 7261 6465 2e70 7922 2c0d 0a20 2020  pgrade.py",..   
+00000f40: 2022 7465 7374 732f 7572 6c6d 6f63 6b2e   "tests/urlmock.
+00000f50: 7079 222c 0d0a 5d0d 0a0d 0a5b 746f 6f6c  py",..]....[tool
+00000f60: 2e63 6f76 6572 6167 652e 7061 7468 735d  .coverage.paths]
+00000f70: 0d0a 7862 726c 5f66 696c 696e 6773 5f61  ..xbrl_filings_a
+00000f80: 7069 203d 205b 2278 6272 6c5f 6669 6c69  pi = ["xbrl_fili
+00000f90: 6e67 735f 6170 6922 2c20 222a 2f78 6272  ngs_api", "*/xbr
+00000fa0: 6c2d 6669 6c69 6e67 732d 6170 692f 7862  l-filings-api/xb
+00000fb0: 726c 5f66 696c 696e 6773 5f61 7069 225d  rl_filings_api"]
+00000fc0: 0d0a 7465 7374 7320 3d20 5b22 7465 7374  ..tests = ["test
+00000fd0: 7322 2c20 222a 2f78 6272 6c2d 6669 6c69  s", "*/xbrl-fili
+00000fe0: 6e67 732d 6170 692f 7465 7374 7322 5d0d  ngs-api/tests"].
+00000ff0: 0a0d 0a5b 746f 6f6c 2e63 6f76 6572 6167  ...[tool.coverag
+00001000: 652e 7265 706f 7274 5d0d 0a65 7863 6c75  e.report]..exclu
+00001010: 6465 5f6c 696e 6573 203d 205b 0d0a 2020  de_lines = [..  
+00001020: 2020 226e 6f20 636f 7622 2c0d 0a20 2020    "no cov",..   
+00001030: 2022 6966 205f 5f6e 616d 655f 5f20 3d3d   "if __name__ ==
+00001040: 202e 5f5f 6d61 696e 5f5f 2e3a 222c 0d0a   .__main__.:",..
+00001050: 2020 2020 2269 6620 5459 5045 5f43 4845      "if TYPE_CHE
+00001060: 434b 494e 473a 222c 0d0a 5d0d 0a0d 0a5b  CKING:",..]....[
+00001070: 746f 6f6c 2e70 7974 6573 742e 696e 695f  tool.pytest.ini_
+00001080: 6f70 7469 6f6e 735d 0d0a 6d61 726b 6572  options]..marker
+00001090: 7320 3d20 5b0d 0a20 2020 2022 7371 6c69  s = [..    "sqli
+000010a0: 7465 3a20 7465 7374 2068 6173 2073 716c  te: test has sql
+000010b0: 6974 6533 206f 7065 7261 7469 6f6e 7322  ite3 operations"
+000010c0: 2c0d 0a20 2020 2022 7061 6769 6e67 3a20  ,..    "paging: 
+000010d0: 7061 6769 6e67 2061 2073 696e 676c 6520  paging a single 
+000010e0: 7175 6572 7922 2c0d 0a20 2020 2022 6d75  query",..    "mu
+000010f0: 6c74 6966 696c 7465 723a 206d 756c 7469  ltifilter: multi
+00001100: 706c 6520 7175 6572 6965 7320 696e 2074  ple queries in t
+00001110: 6865 2073 616d 6520 6361 6c6c 222c 0d0a  he same call",..
+00001120: 2020 2020 2264 6174 653a 2070 726f 6365      "date: proce
+00001130: 7373 696e 6720 6461 7465 206f 626a 6563  ssing date objec
+00001140: 7473 222c 0d0a 2020 2020 2264 6174 6574  ts",..    "datet
+00001150: 696d 653a 2070 726f 6365 7373 696e 6720  ime: processing 
+00001160: 6461 7465 7469 6d65 206f 626a 6563 7473  datetime objects
+00001170: 222c 0d0a 5d0d 0a0d 0a5b 746f 6f6c 2e69  ",..]....[tool.i
+00001180: 736f 7274 5d0d 0a70 795f 7665 7273 696f  sort]..py_versio
+00001190: 6e3d 3339 0d0a 2320 5665 7274 6963 616c  n=39..# Vertical
+000011a0: 2048 616e 6769 6e67 2049 6e64 656e 7420   Hanging Indent 
+000011b0: 4272 6163 6b65 740d 0a6d 756c 7469 5f6c  Bracket..multi_l
+000011c0: 696e 655f 6f75 7470 7574 203d 2038 0d0a  ine_output = 8..
```

