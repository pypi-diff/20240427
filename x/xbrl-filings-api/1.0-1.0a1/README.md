# Comparing `tmp/xbrl_filings_api-1.0.tar.gz` & `tmp/xbrl_filings_api-1.0a1.tar.gz`

## Comparing `xbrl_filings_api-1.0.tar` & `xbrl_filings_api-1.0a1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/ruff.toml
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/__init__.py
--rw-r--r--   0        0        0    19804 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/conftest.py
--rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/conftest_source.py
--rw-r--r--   0        0        0    38020 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/mock_upgrade.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/urlmock.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/integration/__init__.py
--rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/integration/test_pandas_data.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/__init__.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_api_error.py
--rw-r--r--   0        0        0     8340 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_api_page.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_api_resource.py
--rw-r--r--   0        0        0     8362 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_debug.py
--rw-r--r--   0        0        0    22670 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_default_views_sql.py
--rw-r--r--   0        0        0    42478 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_downloading.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_entity.py
--rw-r--r--   0        0        0    24579 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_filing.py
--rw-r--r--   0        0        0    29838 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_filing_set.py
--rw-r--r--   0        0        0    52691 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_filing_set_mutableset.py
--rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_filings_page.py
--rw-r--r--   0        0        0     5540 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_general.py
--rw-r--r--   0        0        0    16741 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_json_tree.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_main.py
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_options_views.py
--rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_pandas_data_unit.py
--rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_query.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_query_add_api_params.py
--rw-r--r--   0        0        0    11289 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_query_filters_multifilters.py
--rw-r--r--   0        0        0    10865 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_query_filters_short_dates.py
--rw-r--r--   0        0        0    21513 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_query_filters_single.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_query_filters_unsupported.py
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_query_flags.py
--rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_query_paging_single.py
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_query_sort.py
--rw-r--r--   0        0        0     7758 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_resource_collection.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_source_data_bugs.py
--rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_stats.py
--rw-r--r--   0        0        0    15788 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/test_validation_message.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/downloader/__init__.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/downloader/conftest.py
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/downloader/test_download.py
--rw-r--r--   0        0        0    10607 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/downloader/test_download_async.py
--rw-r--r--   0        0        0    11101 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/downloader/test_download_parallel.py
--rw-r--r--   0        0        0    14647 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/downloader/test_download_parallel_aiter.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/downloader/test_downloader_stats.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/tests/unit/downloader/test_validate_stem_pattern.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/__about__.py
--rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/__init__.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/__main__.py
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/api_error.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/api_object.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/api_page.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/api_request.py
--rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/api_resource.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/constants.py
--rw-r--r--   0        0        0     9313 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/database_processor.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/debug.py
--rw-r--r--   0        0        0     9833 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/default_views.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/download_info.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/download_item.py
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/download_specs_construct.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/entity.py
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/exceptions.py
--rw-r--r--   0        0        0    31925 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/filing.py
--rw-r--r--   0        0        0    46052 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/filing_set.py
--rw-r--r--   0        0        0     8203 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/filings_page.py
--rw-r--r--   0        0        0    11422 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/json_tree.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/lang_code_transform.py
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/options.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/order_columns.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/parse_type.py
--rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/query.py
--rw-r--r--   0        0        0    21073 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/request_processor.py
--rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/resource_collection.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/scope_flag.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/sqlite_view.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/stats.py
--rw-r--r--   0        0        0    11328 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/validation_message.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/downloader/__init__.py
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/downloader/download_processor.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/downloader/download_result.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/downloader/download_specs.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/downloader/exceptions.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/xbrl_filings_api/downloader/stats.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/.gitignore
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/LICENSE.txt
--rw-r--r--   0        0        0     8536 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/README.md
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/pyproject.toml
--rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 xbrl_filings_api-1.0/PKG-INFO
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

### Comparing `xbrl_filings_api-1.0/ruff.toml` & `xbrl_filings_api-1.0a1/ruff.toml`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/conftest.py` & `xbrl_filings_api-1.0a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/conftest_source.py` & `xbrl_filings_api-1.0a1/tests/conftest_source.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/mock_upgrade.py` & `xbrl_filings_api-1.0a1/tests/mock_upgrade.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/urlmock.py` & `xbrl_filings_api-1.0a1/tests/urlmock.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/integration/test_pandas_data.py` & `xbrl_filings_api-1.0a1/tests/integration/test_pandas_data.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_api_error.py` & `xbrl_filings_api-1.0a1/tests/unit/test_api_error.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_api_page.py` & `xbrl_filings_api-1.0a1/tests/unit/test_api_page.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_api_resource.py` & `xbrl_filings_api-1.0a1/tests/unit/test_api_resource.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_debug.py` & `xbrl_filings_api-1.0a1/tests/unit/test_debug.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_default_views_sql.py` & `xbrl_filings_api-1.0a1/tests/unit/test_default_views_sql.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_downloading.py` & `xbrl_filings_api-1.0a1/tests/unit/test_downloading.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_entity.py` & `xbrl_filings_api-1.0a1/tests/unit/test_entity.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_filing.py` & `xbrl_filings_api-1.0a1/tests/unit/test_filing.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_filing_set.py` & `xbrl_filings_api-1.0a1/tests/unit/test_filing_set.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_filing_set_mutableset.py` & `xbrl_filings_api-1.0a1/tests/unit/test_filing_set_mutableset.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_filings_page.py` & `xbrl_filings_api-1.0a1/tests/unit/test_filings_page.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_general.py` & `xbrl_filings_api-1.0a1/tests/unit/test_general.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_json_tree.py` & `xbrl_filings_api-1.0a1/tests/unit/test_json_tree.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_options_views.py` & `xbrl_filings_api-1.0a1/tests/unit/test_options_views.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_pandas_data_unit.py` & `xbrl_filings_api-1.0a1/tests/unit/test_pandas_data_unit.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_query.py` & `xbrl_filings_api-1.0a1/tests/unit/test_query.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_query_add_api_params.py` & `xbrl_filings_api-1.0a1/tests/unit/test_query_add_api_params.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_query_filters_multifilters.py` & `xbrl_filings_api-1.0a1/tests/unit/test_query_filters_multifilters.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_query_filters_short_dates.py` & `xbrl_filings_api-1.0a1/tests/unit/test_query_filters_short_dates.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_query_filters_single.py` & `xbrl_filings_api-1.0a1/tests/unit/test_query_filters_single.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_query_filters_unsupported.py` & `xbrl_filings_api-1.0a1/tests/unit/test_query_filters_unsupported.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_query_flags.py` & `xbrl_filings_api-1.0a1/tests/unit/test_query_flags.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_query_paging_single.py` & `xbrl_filings_api-1.0a1/tests/unit/test_query_paging_single.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_query_sort.py` & `xbrl_filings_api-1.0a1/tests/unit/test_query_sort.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_resource_collection.py` & `xbrl_filings_api-1.0a1/tests/unit/test_resource_collection.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_source_data_bugs.py` & `xbrl_filings_api-1.0a1/tests/unit/test_source_data_bugs.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_stats.py` & `xbrl_filings_api-1.0a1/tests/unit/test_stats.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/test_validation_message.py` & `xbrl_filings_api-1.0a1/tests/unit/test_validation_message.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/downloader/conftest.py` & `xbrl_filings_api-1.0a1/tests/unit/downloader/conftest.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/downloader/test_download.py` & `xbrl_filings_api-1.0a1/tests/unit/downloader/test_download.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/downloader/test_download_async.py` & `xbrl_filings_api-1.0a1/tests/unit/downloader/test_download_async.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/downloader/test_download_parallel.py` & `xbrl_filings_api-1.0a1/tests/unit/downloader/test_download_parallel.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/downloader/test_download_parallel_aiter.py` & `xbrl_filings_api-1.0a1/tests/unit/downloader/test_download_parallel_aiter.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/downloader/test_downloader_stats.py` & `xbrl_filings_api-1.0a1/tests/unit/downloader/test_downloader_stats.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/tests/unit/downloader/test_validate_stem_pattern.py` & `xbrl_filings_api-1.0a1/tests/unit/downloader/test_validate_stem_pattern.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/__init__.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/__init__.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/api_error.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/api_error.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/api_object.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/api_object.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/api_page.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/api_page.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/api_resource.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/api_resource.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/constants.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/constants.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/database_processor.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/database_processor.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/debug.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/debug.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/default_views.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/default_views.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/download_info.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/download_info.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/download_item.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/download_item.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/download_specs_construct.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/download_specs_construct.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/entity.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/entity.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/exceptions.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/filing.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/filing.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/filing_set.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/filing_set.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/filings_page.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/filings_page.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/json_tree.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/json_tree.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/lang_code_transform.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/lang_code_transform.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/options.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/options.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/order_columns.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/order_columns.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/parse_type.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/parse_type.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/query.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/query.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/request_processor.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/request_processor.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/resource_collection.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/resource_collection.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/scope_flag.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/scope_flag.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/sqlite_view.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/sqlite_view.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/stats.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/stats.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/validation_message.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/validation_message.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/downloader/__init__.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/downloader/download_processor.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/downloader/download_processor.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/downloader/download_result.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/downloader/download_result.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/downloader/download_specs.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/downloader/download_specs.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/xbrl_filings_api/downloader/exceptions.py` & `xbrl_filings_api-1.0a1/xbrl_filings_api/downloader/exceptions.py`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/LICENSE.txt` & `xbrl_filings_api-1.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/README.md` & `xbrl_filings_api-1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `xbrl_filings_api-1.0/pyproject.toml` & `xbrl_filings_api-1.0a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -51,236 +51,235 @@
 00000320: 206e 616d 6520 3d20 224c 6175 7269 2053   name = "Lauri S
 00000330: 616c 6d65 6c61 222c 2065 6d61 696c 203d  almela", email =
 00000340: 2022 6c61 7572 692e 6d2e 7361 6c6d 656c   "lauri.m.salmel
 00000350: 6140 676d 6169 6c2e 636f 6d22 207d 2c0d  a@gmail.com" },.
 00000360: 0a5d 0d0a 636c 6173 7369 6669 6572 7320  .]..classifiers 
 00000370: 3d20 5b0d 0a20 2020 2022 4465 7665 6c6f  = [..    "Develo
 00000380: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
-00000390: 3520 2d20 5072 6f64 7563 7469 6f6e 2f53  5 - Production/S
-000003a0: 7461 626c 6522 2c0d 0a20 2020 2022 5072  table",..    "Pr
-000003b0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000003c0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000003d0: 332e 3922 2c0d 0a20 2020 2022 5072 6f67  3.9",..    "Prog
-000003e0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000003f0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000400: 3130 222c 0d0a 2020 2020 2250 726f 6772  10",..    "Progr
-00000410: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000420: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-00000430: 3122 2c0d 0a20 2020 2022 5072 6f67 7261  1",..    "Progra
-00000440: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000450: 3a20 5079 7468 6f6e 203a 3a20 332e 3132  : Python :: 3.12
-00000460: 222c 0d0a 2020 2020 2250 726f 6772 616d  ",..    "Program
-00000470: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000480: 2050 7974 686f 6e20 3a3a 2049 6d70 6c65   Python :: Imple
-00000490: 6d65 6e74 6174 696f 6e20 3a3a 2043 5079  mentation :: CPy
-000004a0: 7468 6f6e 222c 0d0a 2020 2020 2250 726f  thon",..    "Pro
-000004b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000004c0: 6520 3a3a 2050 7974 686f 6e22 2c0d 0a20  e :: Python",.. 
-000004d0: 2020 2022 5072 6f67 7261 6d6d 696e 6720     "Programming 
-000004e0: 4c61 6e67 7561 6765 203a 3a20 5351 4c22  Language :: SQL"
-000004f0: 2c0d 0a20 2020 2022 4f70 6572 6174 696e  ,..    "Operatin
-00000500: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-00000510: 6e64 6570 656e 6465 6e74 222c 0d0a 2020  ndependent",..  
-00000520: 2020 2249 6e74 656e 6465 6420 4175 6469    "Intended Audi
-00000530: 656e 6365 203a 3a20 4669 6e61 6e63 6961  ence :: Financia
-00000540: 6c20 616e 6420 496e 7375 7261 6e63 6520  l and Insurance 
-00000550: 496e 6475 7374 7279 222c 0d0a 2020 2020  Industry",..    
-00000560: 2249 6e74 656e 6465 6420 4175 6469 656e  "Intended Audien
-00000570: 6365 203a 3a20 496e 666f 726d 6174 696f  ce :: Informatio
-00000580: 6e20 5465 6368 6e6f 6c6f 6779 222c 0d0a  n Technology",..
-00000590: 2020 2020 2249 6e74 656e 6465 6420 4175      "Intended Au
-000005a0: 6469 656e 6365 203a 3a20 5363 6965 6e63  dience :: Scienc
-000005b0: 652f 5265 7365 6172 6368 222c 0d0a 2020  e/Research",..  
-000005c0: 2020 224c 6963 656e 7365 203a 3a20 4f53    "License :: OS
-000005d0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-000005e0: 5420 4c69 6365 6e73 6522 2c0d 0a20 2020  T License",..   
-000005f0: 2022 546f 7069 6320 3a3a 2046 696c 6520   "Topic :: File 
-00000600: 466f 726d 6174 7320 3a3a 204a 534f 4e22  Formats :: JSON"
-00000610: 2c0d 0a20 2020 2022 546f 7069 6320 3a3a  ,..    "Topic ::
-00000620: 2049 6e74 6572 6e65 7420 3a3a 2057 5757   Internet :: WWW
-00000630: 2f48 5454 5020 3a3a 2049 6e64 6578 696e  /HTTP :: Indexin
-00000640: 672f 5365 6172 6368 222c 0d0a 2020 2020  g/Search",..    
-00000650: 2254 6f70 6963 203a 3a20 4f66 6669 6365  "Topic :: Office
-00000660: 2f42 7573 696e 6573 7320 3a3a 2046 696e  /Business :: Fin
-00000670: 616e 6369 616c 222c 0d0a 2020 2020 2254  ancial",..    "T
-00000680: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
-00000690: 2044 6576 656c 6f70 6d65 6e74 203a 3a20   Development :: 
-000006a0: 4c69 6272 6172 6965 7322 2c0d 0a5d 0d0a  Libraries",..]..
-000006b0: 6465 7065 6e64 656e 6369 6573 203d 205b  dependencies = [
-000006c0: 0d0a 2020 2020 2272 6571 7565 7374 7322  ..    "requests"
-000006d0: 2c0d 0a5d 0d0a 0d0a 5b70 726f 6a65 6374  ,..]....[project
-000006e0: 2e75 726c 735d 0d0a 486f 6d65 7061 6765  .urls]..Homepage
-000006f0: 203d 2022 6874 7470 733a 2f2f 6769 7468   = "https://gith
-00000700: 7562 2e63 6f6d 2f6c 7361 6c6d 656c 612f  ub.com/lsalmela/
-00000710: 7862 726c 2d66 696c 696e 6773 2d61 7069  xbrl-filings-api
-00000720: 220d 0a44 6f63 756d 656e 7461 7469 6f6e  "..Documentation
-00000730: 203d 2022 6874 7470 733a 2f2f 6c73 616c   = "https://lsal
-00000740: 6d65 6c61 2e67 6974 6875 622e 696f 2f78  mela.github.io/x
-00000750: 6272 6c2d 6669 6c69 6e67 732d 6170 6922  brl-filings-api"
-00000760: 0d0a 536f 7572 6365 203d 2022 6874 7470  ..Source = "http
-00000770: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
-00000780: 7361 6c6d 656c 612f 7862 726c 2d66 696c  salmela/xbrl-fil
-00000790: 696e 6773 2d61 7069 220d 0a49 7373 7565  ings-api"..Issue
-000007a0: 7320 3d20 2268 7474 7073 3a2f 2f67 6974  s = "https://git
-000007b0: 6875 622e 636f 6d2f 6c73 616c 6d65 6c61  hub.com/lsalmela
-000007c0: 2f78 6272 6c2d 6669 6c69 6e67 732d 6170  /xbrl-filings-ap
-000007d0: 692f 6973 7375 6573 220d 0a0d 0a5b 746f  i/issues"....[to
-000007e0: 6f6c 2e68 6174 6368 2e76 6572 7369 6f6e  ol.hatch.version
-000007f0: 5d0d 0a70 6174 6820 3d20 2278 6272 6c5f  ]..path = "xbrl_
-00000800: 6669 6c69 6e67 735f 6170 692f 5f5f 6162  filings_api/__ab
-00000810: 6f75 745f 5f2e 7079 220d 0a0d 0a5b 746f  out__.py"....[to
-00000820: 6f6c 2e68 6174 6368 2e62 7569 6c64 2e74  ol.hatch.build.t
-00000830: 6172 6765 7473 2e73 6469 7374 5d0d 0a65  argets.sdist]..e
-00000840: 7863 6c75 6465 203d 205b 0d0a 2020 2020  xclude = [..    
-00000850: 222f 2e67 6974 6875 6222 2c0d 0a20 2020  "/.github",..   
-00000860: 2022 2f74 6573 7473 2f6d 6f63 6b5f 7265   "/tests/mock_re
-00000870: 7370 6f6e 7365 732f 2a22 2c0d 0a20 2020  sponses/*",..   
-00000880: 2022 2f64 6f63 7322 2c0d 0a5d 0d0a 0d0a   "/docs",..]....
-00000890: 5b74 6f6f 6c2e 6861 7463 682e 6275 696c  [tool.hatch.buil
-000008a0: 642e 7461 7267 6574 732e 7768 6565 6c5d  d.targets.wheel]
-000008b0: 0d0a 7061 636b 6167 6573 203d 205b 2278  ..packages = ["x
-000008c0: 6272 6c5f 6669 6c69 6e67 735f 6170 6922  brl_filings_api"
-000008d0: 5d0d 0a0d 0a5b 746f 6f6c 2e68 6174 6368  ]....[tool.hatch
-000008e0: 2e65 6e76 732e 6465 6661 756c 745d 0d0a  .envs.default]..
-000008f0: 6465 7065 6e64 656e 6369 6573 203d 205b  dependencies = [
-00000900: 0d0a 2020 2020 2263 6f76 6572 6167 655b  ..    "coverage[
-00000910: 746f 6d6c 5d3e 3d37 2e34 222c 0d0a 2020  toml]>=7.4",..  
-00000920: 2020 2270 7974 6573 743e 3d37 2e34 222c    "pytest>=7.4",
-00000930: 0d0a 2020 2020 2320 4173 206f 6620 7079  ..    # As of py
-00000940: 7465 7374 5f61 7379 6e63 696f 2030 2e32  test_asyncio 0.2
-00000950: 332e 352c 2069 7420 7365 656d 7320 6e6f  3.5, it seems no
-00000960: 7420 746f 2062 6520 706f 7373 6962 6c65  t to be possible
-00000970: 2074 6f20 6765 7420 7269 6420 6f66 0d0a   to get rid of..
-00000980: 2020 2020 2320 6c6f 6767 6564 2077 6172      # logged war
-00000990: 6e69 6e67 2022 4465 7072 6563 6174 696f  ning "Deprecatio
-000009a0: 6e57 6172 6e69 6e67 3a20 5468 6572 6520  nWarning: There 
-000009b0: 6973 206e 6f20 6375 7272 656e 7420 6576  is no current ev
-000009c0: 656e 7420 6c6f 6f70 220d 0a20 2020 2022  ent loop"..    "
-000009d0: 7079 7465 7374 2d61 7379 6e63 696f 3e3d  pytest-asyncio>=
-000009e0: 302e 3233 2e35 222c 0d0a 2020 2020 2272  0.23.5",..    "r
-000009f0: 6573 706f 6e73 6573 7e3d 302e 3233 2e33  esponses~=0.23.3
-00000a00: 222c 2023 2055 7369 6e67 2062 6574 6120  ", # Using beta 
-00000a10: 6665 6174 7572 6573 2028 7265 636f 7264  features (record
-00000a20: 6572 290d 0a20 2020 2022 7061 6e64 6173  er)..    "pandas
-00000a30: 3e3d 322e 312e 3422 2c0d 0a5d 0d0a 0d0a  >=2.1.4",..]....
-00000a40: 5b74 6f6f 6c2e 6861 7463 682e 656e 7673  [tool.hatch.envs
-00000a50: 2e64 6566 6175 6c74 2e73 6372 6970 7473  .default.scripts
-00000a60: 5d0d 0a74 6573 7420 3d20 2270 7974 6573  ]..test = "pytes
-00000a70: 7420 7b61 7267 733a 7465 7374 737d 220d  t {args:tests}".
-00000a80: 0a74 6573 742d 636f 7620 3d20 2263 6f76  .test-cov = "cov
-00000a90: 6572 6167 6520 7275 6e20 2d6d 2070 7974  erage run -m pyt
-00000aa0: 6573 7420 7b61 7267 733a 7465 7374 737d  est {args:tests}
-00000ab0: 220d 0a63 6f76 2d72 6570 6f72 7420 3d20  "..cov-report = 
-00000ac0: 5b0d 0a20 2020 2022 2d20 636f 7665 7261  [..    "- covera
-00000ad0: 6765 2063 6f6d 6269 6e65 222c 0d0a 2020  ge combine",..  
-00000ae0: 2020 2263 6f76 6572 6167 6520 7265 706f    "coverage repo
-00000af0: 7274 222c 0d0a 5d0d 0a63 6f76 203d 205b  rt",..]..cov = [
-00000b00: 0d0a 2020 2020 2274 6573 742d 636f 7622  ..    "test-cov"
-00000b10: 2c0d 0a20 2020 2022 636f 762d 7265 706f  ,..    "cov-repo
-00000b20: 7274 222c 0d0a 5d0d 0a0d 0a5b 5b74 6f6f  rt",..]....[[too
-00000b30: 6c2e 6861 7463 682e 656e 7673 2e61 6c6c  l.hatch.envs.all
-00000b40: 2e6d 6174 7269 785d 5d0d 0a70 7974 686f  .matrix]]..pytho
-00000b50: 6e20 3d20 5b22 332e 3922 2c20 2233 2e31  n = ["3.9", "3.1
-00000b60: 3022 2c20 2233 2e31 3122 2c20 2233 2e31  0", "3.11", "3.1
-00000b70: 3222 5d0d 0a0d 0a5b 746f 6f6c 2e68 6174  2"]....[tool.hat
-00000b80: 6368 2e65 6e76 732e 6c69 6e74 5d0d 0a64  ch.envs.lint]..d
-00000b90: 6574 6163 6865 6420 3d20 7472 7565 0d0a  etached = true..
-00000ba0: 6465 7065 6e64 656e 6369 6573 203d 205b  dependencies = [
-00000bb0: 0d0a 2020 2020 226d 7970 793e 3d31 2e35  ..    "mypy>=1.5
-00000bc0: 2e31 222c 0d0a 5d0d 0a0d 0a5b 746f 6f6c  .1",..]....[tool
-00000bd0: 2e68 6174 6368 2e65 6e76 732e 6c69 6e74  .hatch.envs.lint
-00000be0: 2e73 6372 6970 7473 5d0d 0a74 7970 696e  .scripts]..typin
-00000bf0: 6720 3d20 226d 7970 7920 2d2d 696e 7374  g = "mypy --inst
-00000c00: 616c 6c2d 7479 7065 7320 2d2d 6e6f 6e2d  all-types --non-
-00000c10: 696e 7465 7261 6374 6976 6520 7b61 7267  interactive {arg
-00000c20: 733a 7862 726c 5f66 696c 696e 6773 5f61  s:xbrl_filings_a
-00000c30: 7069 7d22 0d0a 616c 6c20 3d20 5b0d 0a20  pi}"..all = [.. 
-00000c40: 2020 2022 6861 7463 6820 666d 7420 2d6c     "hatch fmt -l
-00000c50: 222c 0d0a 2020 2020 2274 7970 696e 6722  ",..    "typing"
-00000c60: 2c0d 0a5d 0d0a 0d0a 5b74 6f6f 6c2e 6861  ,..]....[tool.ha
-00000c70: 7463 682e 656e 7673 2e64 6f63 5d0d 0a64  tch.envs.doc]..d
-00000c80: 6570 656e 6465 6e63 6965 7320 3d20 5b0d  ependencies = [.
-00000c90: 0a20 2020 2022 7370 6869 6e78 3e3d 372e  .    "sphinx>=7.
-00000ca0: 322e 3622 2c0d 0a20 2020 2022 6675 726f  2.6",..    "furo
-00000cb0: 3e3d 3230 3234 2e31 2e32 3922 2c0d 0a20  >=2024.1.29",.. 
-00000cc0: 2020 2022 7370 6869 6e78 6578 742d 6f70     "sphinxext-op
-00000cd0: 656e 6772 6170 683e 3d30 2e39 2e31 222c  engraph>=0.9.1",
-00000ce0: 0d0a 2020 2020 2273 7068 696e 782d 636f  ..    "sphinx-co
-00000cf0: 7079 6275 7474 6f6e 3e3d 302e 352e 3222  pybutton>=0.5.2"
-00000d00: 2c0d 0a5d 0d0a 0d0a 5b74 6f6f 6c2e 6861  ,..]....[tool.ha
-00000d10: 7463 682e 656e 7673 2e64 6f63 2e73 6372  tch.envs.doc.scr
-00000d20: 6970 7473 5d0d 0a62 7569 6c64 203d 2022  ipts]..build = "
-00000d30: 7370 6869 6e78 2d62 7569 6c64 207b 6172  sphinx-build {ar
-00000d40: 6773 7d20 646f 6373 2f73 6f75 7263 6520  gs} docs/source 
-00000d50: 646f 6373 2f62 7569 6c64 220d 0a23 2057  docs/build"..# W
-00000d60: 696e 646f 7773 2d73 7065 6369 6669 630d  indows-specific.
-00000d70: 0a64 656c 6765 6e20 3d20 2772 6d64 6972  .delgen = 'rmdir
-00000d80: 202f 7320 2f71 2022 646f 6373 5c73 6f75   /s /q "docs\sou
-00000d90: 7263 655c 6170 6922 2022 646f 6373 5c73  rce\api" "docs\s
-00000da0: 6f75 7263 655c 6465 765c 7265 6622 2022  ource\dev\ref" "
-00000db0: 646f 6373 5c62 7569 6c64 2227 0d0a 6662  docs\build"'..fb
-00000dc0: 7569 6c64 203d 205b 0d0a 2020 2020 2264  uild = [..    "d
-00000dd0: 656c 6765 6e22 2c0d 0a20 2020 2022 6275  elgen",..    "bu
-00000de0: 696c 6422 2c0d 0a20 2020 205d 0d0a 6c69  ild",..    ]..li
-00000df0: 6e6b 6368 6563 6b20 3d20 5b0d 0a20 2020  nkcheck = [..   
-00000e00: 2022 7370 6869 6e78 2d62 7569 6c64 202d   "sphinx-build -
-00000e10: 6220 6c69 6e6b 6368 6563 6b20 7b61 7267  b linkcheck {arg
-00000e20: 737d 2064 6f63 732f 736f 7572 6365 2064  s} docs/source d
-00000e30: 6f63 732f 6275 696c 642f 6c69 6e6b 6368  ocs/build/linkch
-00000e40: 6563 6b22 2c0d 0a20 2020 2022 646f 6373  eck",..    "docs
-00000e50: 2f62 7569 6c64 2f6c 696e 6b63 6865 636b  /build/linkcheck
-00000e60: 2f6f 7574 7075 742e 7478 7422 2c0d 0a20  /output.txt",.. 
-00000e70: 2020 205d 0d0a 0d0a 5b74 6f6f 6c2e 636f     ]....[tool.co
-00000e80: 7665 7261 6765 2e72 756e 5d0d 0a73 6f75  verage.run]..sou
-00000e90: 7263 655f 706b 6773 203d 205b 2278 6272  rce_pkgs = ["xbr
-00000ea0: 6c5f 6669 6c69 6e67 735f 6170 6922 2c20  l_filings_api", 
-00000eb0: 2274 6573 7473 225d 0d0a 6272 616e 6368  "tests"]..branch
-00000ec0: 203d 2074 7275 650d 0a70 6172 616c 6c65   = true..paralle
-00000ed0: 6c20 3d20 7472 7565 0d0a 6f6d 6974 203d  l = true..omit =
-00000ee0: 205b 0d0a 2020 2020 2278 6272 6c5f 6669   [..    "xbrl_fi
-00000ef0: 6c69 6e67 735f 6170 692f 5f5f 6162 6f75  lings_api/__abou
-00000f00: 745f 5f2e 7079 222c 0d0a 2020 2020 2274  t__.py",..    "t
-00000f10: 6573 7473 2f63 6f6e 6674 6573 745f 736f  ests/conftest_so
-00000f20: 7572 6365 2e70 7922 2c0d 0a20 2020 2022  urce.py",..    "
-00000f30: 7465 7374 732f 6d6f 636b 5f75 7067 7261  tests/mock_upgra
-00000f40: 6465 2e70 7922 2c0d 0a20 2020 2022 7465  de.py",..    "te
-00000f50: 7374 732f 7572 6c6d 6f63 6b2e 7079 222c  sts/urlmock.py",
-00000f60: 0d0a 5d0d 0a0d 0a5b 746f 6f6c 2e63 6f76  ..]....[tool.cov
-00000f70: 6572 6167 652e 7061 7468 735d 0d0a 7862  erage.paths]..xb
-00000f80: 726c 5f66 696c 696e 6773 5f61 7069 203d  rl_filings_api =
-00000f90: 205b 2278 6272 6c5f 6669 6c69 6e67 735f   ["xbrl_filings_
-00000fa0: 6170 6922 2c20 222a 2f78 6272 6c2d 6669  api", "*/xbrl-fi
-00000fb0: 6c69 6e67 732d 6170 692f 7862 726c 5f66  lings-api/xbrl_f
-00000fc0: 696c 696e 6773 5f61 7069 225d 0d0a 7465  ilings_api"]..te
-00000fd0: 7374 7320 3d20 5b22 7465 7374 7322 2c20  sts = ["tests", 
-00000fe0: 222a 2f78 6272 6c2d 6669 6c69 6e67 732d  "*/xbrl-filings-
-00000ff0: 6170 692f 7465 7374 7322 5d0d 0a0d 0a5b  api/tests"]....[
-00001000: 746f 6f6c 2e63 6f76 6572 6167 652e 7265  tool.coverage.re
-00001010: 706f 7274 5d0d 0a65 7863 6c75 6465 5f6c  port]..exclude_l
-00001020: 696e 6573 203d 205b 0d0a 2020 2020 226e  ines = [..    "n
-00001030: 6f20 636f 7622 2c0d 0a20 2020 2022 6966  o cov",..    "if
-00001040: 205f 5f6e 616d 655f 5f20 3d3d 202e 5f5f   __name__ == .__
-00001050: 6d61 696e 5f5f 2e3a 222c 0d0a 2020 2020  main__.:",..    
-00001060: 2269 6620 5459 5045 5f43 4845 434b 494e  "if TYPE_CHECKIN
-00001070: 473a 222c 0d0a 5d0d 0a0d 0a5b 746f 6f6c  G:",..]....[tool
-00001080: 2e70 7974 6573 742e 696e 695f 6f70 7469  .pytest.ini_opti
-00001090: 6f6e 735d 0d0a 6d61 726b 6572 7320 3d20  ons]..markers = 
-000010a0: 5b0d 0a20 2020 2022 7371 6c69 7465 3a20  [..    "sqlite: 
-000010b0: 7465 7374 2068 6173 2073 716c 6974 6533  test has sqlite3
-000010c0: 206f 7065 7261 7469 6f6e 7322 2c0d 0a20   operations",.. 
-000010d0: 2020 2022 7061 6769 6e67 3a20 7061 6769     "paging: pagi
-000010e0: 6e67 2061 2073 696e 676c 6520 7175 6572  ng a single quer
-000010f0: 7922 2c0d 0a20 2020 2022 6d75 6c74 6966  y",..    "multif
-00001100: 696c 7465 723a 206d 756c 7469 706c 6520  ilter: multiple 
-00001110: 7175 6572 6965 7320 696e 2074 6865 2073  queries in the s
-00001120: 616d 6520 6361 6c6c 222c 0d0a 2020 2020  ame call",..    
-00001130: 2264 6174 653a 2070 726f 6365 7373 696e  "date: processin
-00001140: 6720 6461 7465 206f 626a 6563 7473 222c  g date objects",
-00001150: 0d0a 2020 2020 2264 6174 6574 696d 653a  ..    "datetime:
-00001160: 2070 726f 6365 7373 696e 6720 6461 7465   processing date
-00001170: 7469 6d65 206f 626a 6563 7473 222c 0d0a  time objects",..
-00001180: 5d0d 0a0d 0a5b 746f 6f6c 2e69 736f 7274  ]....[tool.isort
-00001190: 5d0d 0a70 795f 7665 7273 696f 6e3d 3339  ]..py_version=39
-000011a0: 0d0a 2320 5665 7274 6963 616c 2048 616e  ..# Vertical Han
-000011b0: 6769 6e67 2049 6e64 656e 7420 4272 6163  ging Indent Brac
-000011c0: 6b65 740d 0a6d 756c 7469 5f6c 696e 655f  ket..multi_line_
-000011d0: 6f75 7470 7574 203d 2038 0d0a            output = 8..
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

### Comparing `xbrl_filings_api-1.0/PKG-INFO` & `xbrl_filings_api-1.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: xbrl-filings-api
-Version: 1.0
+Version: 1.0a1
 Summary: Python API for filings.xbrl.org XBRL report repository.
 Project-URL: Homepage, https://github.com/lsalmela/xbrl-filings-api
 Project-URL: Documentation, https://lsalmela.github.io/xbrl-filings-api
 Project-URL: Source, https://github.com/lsalmela/xbrl-filings-api
 Project-URL: Issues, https://github.com/lsalmela/xbrl-filings-api/issues
 Author-email: Lauri Salmela <lauri.m.salmela@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: AFR,ESEF,ESMA,EU,European Single Electronic Format,European Union,Extensible Business Reporting Language,IFRS,Inline XBRL,JSON,JSON-API,XBRL,accounting,accounting quality,annual financial report,consolidated,consolidation,financial analysis,financial statement,financial statement analysis,iXBRL,listed company,regulated markets,stock exchange,structured data,transparency
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
```

