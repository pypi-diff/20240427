# Comparing `tmp/mns-scheduler-1.0.3.3.tar.gz` & `tmp/mns-scheduler-1.0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.3.3.tar", last modified: Wed Apr 24 09:38:12 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.3.5.tar", last modified: Sat Apr 27 03:58:43 2024, max compression
```

## Comparing `mns-scheduler-1.0.3.3.tar` & `mns-scheduler-1.0.3.5.tar`

### file list

```diff
@@ -1,100 +1,102 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.721346 mns-scheduler-1.0.3.3/
--rw-rw-rw-   0        0        0       62 2024-04-24 09:38:12.720348 mns-scheduler-1.0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.689432 mns-scheduler-1.0.3.3/mns_scheduler/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.691426 mns-scheduler-1.0.3.3/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2023-12-22 04:57:03.000000 mns-scheduler-1.0.3.3/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.693421 mns-scheduler-1.0.3.3/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    15238 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    20332 2024-04-18 14:12:36.000000 mns-scheduler-1.0.3.3/mns_scheduler/company_info/company_info_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.693421 mns-scheduler-1.0.3.3/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.694418 mns-scheduler-1.0.3.3/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     2440 2024-03-22 08:13:08.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.696412 mns-scheduler-1.0.3.3/mns_scheduler/concept/em/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/em/__init__.py
--rw-rw-rw-   0        0        0     4993 2023-12-22 05:01:59.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2023-12-22 05:01:59.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2335 2023-12-22 05:01:59.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.697409 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.697409 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/app/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.699404 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0    10238 2024-04-13 05:32:34.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     1662 2024-04-15 02:52:26.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.700401 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/symbol/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/symbol/__init__.py
--rw-rw-rw-   0        0        0     1928 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8757 2024-04-16 06:53:57.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.702396 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/web/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/web/__init__.py
--rw-rw-rw-   0        0        0     5001 2024-04-13 05:23:41.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3605 2024-03-21 16:54:56.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.703394 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/wen_cai/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.704391 mns-scheduler-1.0.3.3/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-02-28 08:33:00.000000 mns-scheduler-1.0.3.3/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.705388 mns-scheduler-1.0.3.3/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.706386 mns-scheduler-1.0.3.3/mns_scheduler/ipo/
--rw-rw-rw-   0        0        0      163 2024-01-08 10:50:26.000000 mns-scheduler-1.0.3.3/mns_scheduler/ipo/__init__.py
--rw-rw-rw-   0        0        0      387 2024-01-08 10:59:33.000000 mns-scheduler-1.0.3.3/mns_scheduler/ipo/auto_ipo_buy_api.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.706386 mns-scheduler-1.0.3.3/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.708381 mns-scheduler-1.0.3.3/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    21833 2024-01-09 10:50:36.000000 mns-scheduler-1.0.3.3/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     7988 2024-04-18 13:32:07.000000 mns-scheduler-1.0.3.3/mns_scheduler/k_line/clean/k_line_info_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.708381 mns-scheduler-1.0.3.3/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5654 2024-03-29 10:48:40.000000 mns-scheduler-1.0.3.3/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.709378 mns-scheduler-1.0.3.3/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.709378 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.711372 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     4765 2024-04-24 09:37:02.000000 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
--rw-rw-rw-   0        0        0     8016 2024-04-02 13:03:08.000000 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.711372 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.712370 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0    10461 2024-04-20 14:08:05.000000 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.714365 mns-scheduler-1.0.3.3/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     8850 2024-04-01 01:27:55.000000 mns-scheduler-1.0.3.3/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.715362 mns-scheduler-1.0.3.3/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2023-12-17 03:50:52.000000 mns-scheduler-1.0.3.3/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.718354 mns-scheduler-1.0.3.3/mns_scheduler/zt/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2023-12-17 13:29:39.000000 mns-scheduler-1.0.3.3/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17269 2024-03-09 09:58:27.000000 mns-scheduler-1.0.3.3/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-01-04 12:05:04.000000 mns-scheduler-1.0.3.3/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7534 2024-04-16 13:51:28.000000 mns-scheduler-1.0.3.3/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.719351 mns-scheduler-1.0.3.3/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    14500 2024-04-24 08:54:42.000000 mns-scheduler-1.0.3.3/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-03-23 03:12:05.000000 mns-scheduler-1.0.3.3/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.720348 mns-scheduler-1.0.3.3/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-04-24 09:38:12.000000 mns-scheduler-1.0.3.3/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3078 2024-04-24 09:38:12.000000 mns-scheduler-1.0.3.3/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 09:38:12.000000 mns-scheduler-1.0.3.3/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-24 09:38:12.000000 mns-scheduler-1.0.3.3/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 09:38:12.721346 mns-scheduler-1.0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-04-24 09:38:10.000000 mns-scheduler-1.0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.031075 mns-scheduler-1.0.3.5/
+-rw-rw-rw-   0        0        0       62 2024-04-27 03:58:43.030564 mns-scheduler-1.0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.000412 mns-scheduler-1.0.3.5/mns_scheduler/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.002495 mns-scheduler-1.0.3.5/mns_scheduler/backup/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/mns_scheduler/backup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.003515 mns-scheduler-1.0.3.5/mns_scheduler/backup/app/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/mns_scheduler/backup/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/mns_scheduler/backup/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.005547 mns-scheduler-1.0.3.5/mns_scheduler/backup/em/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/mns_scheduler/backup/em/__init__.py
+-rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/mns_scheduler/backup/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/mns_scheduler/backup/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.006064 mns-scheduler-1.0.3.5/mns_scheduler/backup/wen_cai/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/mns_scheduler/backup/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.007084 mns-scheduler-1.0.3.5/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.008612 mns-scheduler-1.0.3.5/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    15238 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    20332 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/company_info/company_info_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.009121 mns-scheduler-1.0.3.5/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.009636 mns-scheduler-1.0.3.5/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     2459 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/mns_scheduler/concept/clean/ths_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.010148 mns-scheduler-1.0.3.5/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.011683 mns-scheduler-1.0.3.5/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0     6542 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     4305 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.012701 mns-scheduler-1.0.3.5/mns_scheduler/concept/ths/sync_new_index/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/mns_scheduler/concept/ths/sync_new_index/__init__.py
+-rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.014222 mns-scheduler-1.0.3.5/mns_scheduler/concept/ths/update_concept_info/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/mns_scheduler/concept/ths/update_concept_info/__init__.py
+-rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.015750 mns-scheduler-1.0.3.5/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.016265 mns-scheduler-1.0.3.5/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.017282 mns-scheduler-1.0.3.5/mns_scheduler/ipo/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/ipo/__init__.py
+-rw-rw-rw-   0        0        0      387 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/ipo/auto_ipo_buy_api.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.017793 mns-scheduler-1.0.3.5/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.018811 mns-scheduler-1.0.3.5/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    21833 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     7988 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.019836 mns-scheduler-1.0.3.5/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5654 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.020345 mns-scheduler-1.0.3.5/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.020345 mns-scheduler-1.0.3.5/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.021875 mns-scheduler-1.0.3.5/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     4503 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
+-rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.022385 mns-scheduler-1.0.3.5/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.023403 mns-scheduler-1.0.3.5/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.024935 mns-scheduler-1.0.3.5/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     8850 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.025447 mns-scheduler-1.0.3.5/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.028514 mns-scheduler-1.0.3.5/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17269 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7534 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.029537 mns-scheduler-1.0.3.5/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    14916 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.3.5/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-04-27 03:58:43.030053 mns-scheduler-1.0.3.5/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-04-27 03:58:42.000000 mns-scheduler-1.0.3.5/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3157 2024-04-27 03:58:42.000000 mns-scheduler-1.0.3.5/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 03:58:42.000000 mns-scheduler-1.0.3.5/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-27 03:58:42.000000 mns-scheduler-1.0.3.5/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 03:58:43.031075 mns-scheduler-1.0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-04-27 03:55:36.000000 mns-scheduler-1.0.3.5/setup.py
```

### Comparing `mns-scheduler-1.0.3.3/README.md` & `mns-scheduler-1.0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.3.5/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.3.5/mns_scheduler/company_info/company_constant_data.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.3.5/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py` & `mns-scheduler-1.0.3.5/mns_scheduler/concept/clean/ths_concept_clean_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         concept_count = (mongodb_util
                          .count(query, 'ths_stock_concept_detail'))
         ths_concept_list_one_df = ths_concept_list.loc[ths_concept_list['symbol'] == ths_concept_one.symbol]
         ths_concept_list_one_df['concept_count'] = concept_count
         mongodb_util.save_mongo(ths_concept_list_one_df, 'ths_concept_list')
 
 
+# 更新空名字
 def update_null_name():
     query = {"_id": {'$gte': 886025}}
     ths_concept_list = mongodb_util.find_query_data('ths_concept_list', query)
     ths_concept_list = ths_concept_list.sort_values(by=['_id'], ascending=False)
 
     for concept_one in ths_concept_list.itertuples():
         concept_code = concept_one.symbol
```

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/concept/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.3.5/mns_scheduler/backup/em/em_new_concept_his_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 sys.path.append(project_path)
 
 import akshare as ak
 from loguru import logger
 from datetime import datetime
 import mns_common.utils.date_handle_util as date_handle_util
 import mns_common.db.MongodbUtil as MongodbUtil
-import mns_scheduler.concept.em.em_new_concept_sync_common_api as em_new_concept_sync_common_api
+import mns_scheduler.backup.em.em_new_concept_sync_common_api as em_new_concept_sync_common_api
 import mns_common.api.em.em_concept_index_api as em_concept_index_api
 
 mongodb_util = MongodbUtil('27017')
 
 
 # 同步概念k线
 def sync_concept_k_line(symbol, period, start_date, end_date, adjust):
```

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/concept/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.3.5/mns_scheduler/backup/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/concept/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.3.5/mns_scheduler/backup/em/em_new_concept_sync_web.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 end = file_path.index('mns') + 17
 project_path = file_path[0:end]
 sys.path.append(project_path)
 
 import datetime
 import time
 from loguru import logger
-import mns_scheduler.concept.em.em_new_concept_sync_common_api as em_new_concept_sync_common_api
+import mns_scheduler.backup.em.em_new_concept_sync_common_api as em_new_concept_sync_common_api
 
 
 # 同步东财新概念
 def sync_new_concept_data():
     concept_code = em_new_concept_sync_common_api.get_max_concept_code()
     # 装换为数字
     concept_code = int(concept_code)
```

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.3.5/mns_scheduler/backup/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.3.5/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,241 +1,181 @@
-import sys
 import os
-
+import sys
 import pandas as pd
-import time
 import mns_common.api.ths.ths_stock_api as ths_stock_api
-import datetime
+import mns_common.api.em.east_money_stock_api as east_money_stock_api
+import mns_common.component.common_service_fun_api as common_service_fun_api
 from mns_common.db.MongodbUtil import MongodbUtil
-import mns_common.component.company.company_common_service_api as company_common_service_api
+from loguru import logger
+import mns_common.utils.data_frame_util as data_frame_util
+from datetime import datetime
+from mns_common.utils.async_fun import async_fun
+import mns_scheduler.concept.ths.common.ths_concept_sync_common_api as ths_concept_sync_common_api
+import threading
+import mns_scheduler.concept.ths.common.ths_concept_update_common_api as ths_concept_update_common_api
+import mns_common.utils.date_handle_util as date_handle_util
 
 file_path = os.path.abspath(__file__)
 end = file_path.index('mns') + 17
 project_path = file_path[0:end]
 sys.path.append(project_path)
 mongodb_util = MongodbUtil('27017')
-import mns_common.api.msg.push_msg_api as push_msg_api
-import mns_scheduler.company_info.company_info_sync_api as company_info_sync_api
-import mns_common.utils.data_frame_util as data_frame_util
-max_concept_code = 886110
+# 分页大小
+MAX_PAGE_NUMBER = 2500
+# 获取单只股票新增概念
 
-order_fields = [
-    "index",
-    "symbol",
-    "name",
-    "now_price",
-    "chg",
-    "change",
-    "exchange",
-    "amount",
-    "concept_code",
-]
-
-
-def push_msg_to_we_chat_web(concept_code, concept_name, url):
-    msg = "概念代码:" + str(concept_code) + "," + "概念名称:" + concept_name + "," + "url:   " + url
-    title = "新增同花顺概念:" + str(concept_code) + "-" + concept_name
-    push_msg_api.push_msg_to_wechat(title, msg)
-
-
-# 保存新概念信息到数据库
-def save_ths_concept_list(concept_code, concept_name, str_day, str_now_time):
-    url = 'http://q.10jqka.com.cn/thshy/detail/code/' + str(concept_code)
-    ths_concept_list = pd.DataFrame([
-        [concept_code, concept_code, concept_name, str_day, url, str_now_time, True, True],
-    ], columns=['_id', 'symbol', 'name', 'str_day', 'url', 'str_now_time', 'success', 'valid'])
-    mongodb_util.save_mongo(ths_concept_list, 'ths_concept_list')
-
-
-# 获取最大概念代码
-def get_max_concept_code():
-    query = {"symbol": {'$ne': 'null'}, "success": True}
-    ths_concept_max = mongodb_util.descend_query(query, 'ths_concept_list', 'symbol', 1)
-    if ths_concept_max.shape[0] == 0:
-        concept_code = 885284
-    else:
-        concept_code = list(ths_concept_max['symbol'])[0]
+db_name = 'ths_stock_concept_detail_app'
 
-    return concept_code
 
+def create_index():
+    mongodb_util.create_index(db_name, [("symbol", 1)])
+    mongodb_util.create_index(db_name, [("str_day", 1)])
+    mongodb_util.create_index(db_name, [("title", 1)])
+    mongodb_util.create_index(db_name, [("str_now_date", 1)])
 
-# 保存新概念详细信息到数据库
-def save_ths_concept_detail(new_concept_symbol_df,
-                            concept_name, str_day,
-                            str_now_time, concept_code):
-    concept_code = int(concept_code)
-    new_concept_symbol_df['symbol'] = new_concept_symbol_df['symbol'].astype(str)
-    new_concept_symbol_df['_id'] = str(concept_code) + '_' + new_concept_symbol_df['symbol']
-    new_concept_symbol_df['concept_code'] = concept_code
-    new_concept_symbol_df['concept_name'] = concept_name
-
-    new_concept_symbol_df['concept_name'] = new_concept_symbol_df['concept_name'].replace(" ", "")
-
-    query_ths_concept = {'symbol': concept_code}
-    ths_concept_list = mongodb_util.find_query_data('ths_concept_list', query_ths_concept)
-    if ths_concept_list.shape[0] == 0:
-        concept_create_day = str_day
-    else:
-        concept_create_day = list(ths_concept_list['str_day'])[0]
 
-    new_concept_symbol_df['str_day'] = str_day
-    new_concept_symbol_df['str_now_time'] = str_now_time
-    new_concept_symbol_df['concept_create_day'] = concept_create_day
-
-    new_concept_symbol_list = list(new_concept_symbol_df['symbol'])
-
-    query_company_info = {'symbol': {'$in': new_concept_symbol_list}}
-    query_field = {"first_industry": 1, "first_industry": 1, "industry": 1,
-                   "company_type": 1, "flow_mv_sp": 1,
-                   "total_mv_sp": 1}
-    company_info = mongodb_util.find_query_data_choose_field('company_info',
-                                                             query_company_info, query_field)
-
-    company_info = company_info.set_index(['_id'], drop=True)
-    new_concept_symbol_df = new_concept_symbol_df.set_index(['symbol'], drop=False)
-
-    new_concept_symbol_df = pd.merge(new_concept_symbol_df, company_info, how='outer',
-                                     left_index=True, right_index=True)
-    new_concept_symbol_df['concept_name'] = new_concept_symbol_df['concept_name'].replace(" ", "")
-    query = {'concept_code': concept_code}
-
-    if bool(1 - ('way' in new_concept_symbol_df.columns)):
-        new_concept_symbol_df['way'] = 'symbol_sync'
-
-    new_concept_symbol_df = new_concept_symbol_df[[
-        "_id",
-        "index",
-        "symbol",
-        "name",
-        "now_price",
-        "chg",
-        "change",
-        "exchange",
-        "amount",
-        "concept_code",
-        "concept_name",
-        "str_day",
-        "str_now_time",
-        "industry",
-        "flow_mv_sp",
-        "total_mv_sp",
-        "company_type",
-        "concept_create_day",
-        "way"
-    ]]
-
-    exist_concept_detail = mongodb_util.find_query_data('ths_stock_concept_detail', query)
-    if exist_concept_detail is None or exist_concept_detail.shape[0] == 0:
-        mongodb_util.save_mongo(new_concept_symbol_df, 'ths_stock_concept_detail')
-    else:
-        exist_concept_detail_symbol_list = list(exist_concept_detail['symbol'])
-        new_concept_symbol_df = new_concept_symbol_df.loc[~(
-            new_concept_symbol_df['symbol'].isin(exist_concept_detail_symbol_list))]
-        if new_concept_symbol_df.shape[0] > 0:
-            mongodb_util.save_mongo(new_concept_symbol_df, 'ths_stock_concept_detail')
-            # 保存到当日新增概念列表
-            new_concept_symbol_df['concept_type'] = 'ths'
-            mongodb_util.save_mongo(new_concept_symbol_df, 'today_new_concept_list')
-    update_company_info(new_concept_symbol_df)
-    # 公司缓存信息清除
-    company_common_service_api.company_info_industry_cache_clear()
-
-
-# 更新公司表信息 todo 清空cache 公司表中  common_service_fun_api.py  get_company_info_industry
-def update_company_info(new_concept_symbol_df):
-    if new_concept_symbol_df.shape[0] > 0:
-        symbol_list = list(new_concept_symbol_df['symbol'])
-        company_info_sync_api.sync_company_base_info(symbol_list)
-        company_info_sync_api.fix_company_industry(None)
-        # 公司缓存信息清除
-        company_common_service_api.company_info_industry_cache_clear()
-
-
-def update_null_name():
-    query = {"_id": {'$gte': 886025}}
-    ths_concept_list = mongodb_util.find_query_data('ths_concept_list', query)
-    ths_concept_list = ths_concept_list.sort_values(by=['_id'], ascending=False)
-
-    for concept_one in ths_concept_list.itertuples():
-        concept_code = concept_one.symbol
-        name = concept_one.name
-        exist_url = concept_one.url
-
-        if name == '':
-            concept_name = ths_stock_api.get_concept_name(concept_code)
-            query_concept = {"symbol": concept_code}
-            new_values = {'$set': {"name": concept_name}}
-            mongodb_util.update_one_query(query_concept, new_values, 'ths_concept_list')
-
-            new_values_detail = {'$set': {"concept_name": concept_name}}
-
-            query_concept_detail = {"concept_code": concept_code}
-
-            mongodb_util.update_many(query_concept_detail, new_values_detail, 'ths_stock_concept_detail')
-            time.sleep(10)
-
-        if exist_url == '' or pd.isna(exist_url):
-            url = 'http://q.10jqka.com.cn/thshy/detail/code/' + str(concept_code)
-            str_now_time = concept_one.str_day + " " + "00:00:00"
-            query_concept = {"symbol": concept_code}
-            new_values = {'$set': {"url": url, "str_now_time": str_now_time}}
-            mongodb_util.update_one_query(query_concept, new_values, 'ths_concept_list')
-
-
-# 更新概念数量
-def update_concept_number():
-    query = {}
-    ths_concept_list = mongodb_util.find_query_data('ths_concept_list', query)
-    ths_concept_list = ths_concept_list.sort_values(by=['_id'], ascending=False)
-    for concept_one in ths_concept_list.itertuples():
+# 同步新概念到详情表中
+# @async_fun
+def sync_new_concept_to_ths_detail(symbol_add_new_concept_df, str_day, str_now_time):
+    for new_concept_one in symbol_add_new_concept_df.itertuples():
         try:
-            query_detail = {'concept_code': concept_one.symbol}
-            concept_number = mongodb_util.count(query_detail, 'ths_stock_concept_detail')
-            query_update = {"symbol": concept_one.symbol}
-            new_values = {'$set': {"concept_number": concept_number}}
-            mongodb_util.update_one_query(query_update, new_values, 'ths_concept_list')
-        except BaseException as e:
-            print(e)
-
+            concept_code = new_concept_one.concept_code
+            query = {'web_concept_code': int(concept_code)}
+            ths_concept_list = mongodb_util.find_query_data('ths_concept_list', query)
+            if data_frame_util.is_empty(ths_concept_list):
+                logger.error("无此同花顺概念:{}", new_concept_one.title)
+            else:
+                concept_code = list(ths_concept_list['symbol'])[0]
+                concept_name = list(ths_concept_list['name'])[0]
+                ths_concept_sync_common_api.save_ths_concept_detail(symbol_add_new_concept_df,
+                                                                    concept_name, str_day,
+                                                                    str_now_time, concept_code)
 
-def get_concept_detail_info_web(concept_code):
-    new_concept_symbol_list = ths_stock_api.ths_stock_concept(concept_code)
-    if new_concept_symbol_list is None or new_concept_symbol_list.shape[0] == 0:
-        return None
-    new_concept_symbol_list['_id'] = str(concept_code) + '-' + new_concept_symbol_list['symbol']
-    return new_concept_symbol_list
-
-
-def update_nan_data():
-    query = {"concept_code": float('NaN')}
-    ths_stock_concept_detail = mongodb_util.find_query_data('ths_stock_concept_detail', query)
-
-    ths_stock_concept_detail['concept_code'] = ths_stock_concept_detail['_id']
-    for stock_one in ths_stock_concept_detail.itertuples():
-        query = {"symbol": stock_one.symbol}
-        company_info = mongodb_util.find_query_data('company_info', query)
-
-        concept_code = stock_one.concept_code
-        concept_code = int(concept_code[0:6])
-
-        new_values = {'$set': {"concept_code": concept_code,
-                               "flow_mv_sp": list(company_info['flow_mv_sp'])[0],
-                               "total_mv_sp": list(company_info['total_mv_sp'])[0],
-                               "company_type": list(company_info['company_type'])[0]
+        except BaseException as e:
+            logger.error("转换同花顺概念异常:{},{}", new_concept_one, e)
 
-                               }}
-        query_update = {"_id": stock_one.concept_code}
-        mongodb_util.update_many(query_update, new_values, 'ths_stock_concept_detail')
 
+# 保存数据到对比
+@async_fun
+def save_data_to_db(ths_concept_df):
+    if data_frame_util.is_empty(ths_concept_df):
+        return
+    json_data = ths_concept_df.to_dict(orient='records')
+    mongodb_util.save_mongo_json(json_data, db_name)
+
+
+# 对比数据库和接口概念详情的差值
+def choose_new_concept_from_compare_db(ths_concept_df, symbol_ths_new_concept_exist_db):
+    if data_frame_util.is_empty(symbol_ths_new_concept_exist_db):
+        return ths_concept_df
+    else:
+        symbol_add_new_concept = ths_concept_df.loc[~(
+            ths_concept_df['_id'].isin(list(symbol_ths_new_concept_exist_db['_id'])))]
+        return symbol_add_new_concept
+
+
+# 选择接口返回为新概念标识的数据
+def choose_type_new_concept(ths_concept_df):
+    filtered_df = ths_concept_df[
+        ths_concept_df['label'].apply(lambda x: any(item['type'] == 'new' for item in x))]
+    if data_frame_util.is_empty(filtered_df):
+        return
+    return ths_concept_df
+
+
+# 同步新概念 多线程实现
+def update_symbol_new_concept(symbol_df, page_number):
+    for stock_one in symbol_df.itertuples():
+        try:
+            ths_concept_json = ths_stock_api.get_symbol_add_new_concept(stock_one.symbol)
+            logger.info("同步symbol概念信息:{}", stock_one.symbol)
+            symbol_ths_concept_all_df = pd.DataFrame(ths_concept_json)
+            if data_frame_util.is_empty(symbol_ths_concept_all_df):
+                continue
+
+            now_date = datetime.now()
+            # 开盘交易前不同步 资源开销过大
+            if date_handle_util.is_close_time(now_date):
+                ths_concept_update_common_api.update_ths_concept_choose_reason(symbol_ths_concept_all_df, stock_one.symbol)
+
+            str_day = now_date.strftime('%Y-%m-%d')
+            str_now_date = now_date.strftime('%Y-%m-%d %H:%M:%S')
+            symbol_ths_concept_all_df.loc[:, 'str_day'] = str_day
+            symbol_ths_concept_all_df.loc[:, 'str_now_date'] = str_now_date
+            symbol_ths_concept_all_df.loc[:, 'symbol'] = stock_one.symbol
+            symbol_ths_concept_all_df.loc[:, 'name'] = stock_one.name
+            symbol_ths_concept_all_df.loc[:, 'index'] = 1
+            symbol_ths_concept_all_df.loc[:, 'now_price'] = stock_one.now_price
+            symbol_ths_concept_all_df.loc[:, 'chg'] = stock_one.chg
+            symbol_ths_concept_all_df.loc[:, 'change'] = stock_one.now_price - stock_one.open
+            symbol_ths_concept_all_df.loc[:, 'exchange'] = stock_one.exchange
+            symbol_ths_concept_all_df.loc[:, 'amount'] = stock_one.amount
+            symbol_ths_concept_all_df.loc[:, 'concept_create_day'] = str_day
+
+            symbol_ths_concept_all_df['concept_code'] = symbol_ths_concept_all_df['cid'].apply(str)
+            symbol_ths_concept_all_df['name'] = symbol_ths_concept_all_df['name'].replace(" ", "")
+
+            symbol_ths_concept_all_df.loc[:, '_id'] = symbol_ths_concept_all_df['symbol'] + '_' + \
+                                                      symbol_ths_concept_all_df['concept_code']
+
+            query = {'symbol': stock_one.symbol}
+            query_field = {"_id": 1}
+            # 已经存在的数据
+            symbol_ths_new_concept_exist_db = mongodb_util.find_query_data_choose_field('ths_stock_concept_detail_app',
+                                                                                        query, query_field)
+            # 与存在的概念对比 找出新增概念
+            symbol_add_new_concept_db_df = choose_new_concept_from_compare_db(symbol_ths_concept_all_df,
+                                                                              symbol_ths_new_concept_exist_db)
+            # 接口中带new 标记的数据
+            symbol_add_new_concept_api_df = choose_type_new_concept(symbol_ths_concept_all_df)
+
+            symbol_add_new_concept_df = data_frame_util.merge_choose_data_no_drop(symbol_add_new_concept_api_df,
+                                                                                  symbol_add_new_concept_db_df)
+            if data_frame_util.is_empty(symbol_add_new_concept_df):
+                continue
+
+            symbol_add_new_concept_df.drop_duplicates('_id', keep='last', inplace=True)
+
+            if data_frame_util.is_empty(symbol_ths_new_concept_exist_db):
+                symbol_add_new_concept_df = symbol_add_new_concept_df
+            else:
+                symbol_add_new_concept_df = symbol_add_new_concept_df.loc[~(
+                    symbol_add_new_concept_df['_id'].isin(list(symbol_ths_new_concept_exist_db['_id'])))]
+            if data_frame_util.is_empty(symbol_add_new_concept_df):
+                continue
+            # 保存到概念详情集合中
+            save_data_to_db(symbol_add_new_concept_df)
+            sync_new_concept_to_ths_detail(symbol_add_new_concept_df, str_day, str_now_date)
+            logger.info("symbol新增概念信息:{},{}", stock_one.symbol, stock_one.name)
+        except BaseException as e:
+            logger.error("发生异常:{},{}", e, stock_one.symbol)
 
-def update_concept_create_day():
-    query = {"symbol": {'$exists': True}}
-    new_concept_list = mongodb_util.descend_query(query, "ths_concept_list", "_id", 500)
 
-    if new_concept_list.shape[0] > 0:
-        for one_concept in new_concept_list.itertuples():
-            concept_create_day = one_concept.str_day
-            query_update = {"concept_code": one_concept.symbol}
+def sync_symbol_all_concept(symbol):
+    create_index()
+    real_time_quotes_now = east_money_stock_api.get_real_time_quotes_all_stocks()
+    real_time_quotes_now = common_service_fun_api.classify_symbol(real_time_quotes_now)
+    if symbol is not None:
+        real_time_quotes_now = real_time_quotes_now.loc[real_time_quotes_now['symbol'] == symbol]
+    count = real_time_quotes_now.shape[0]
+    page_number = round(count / MAX_PAGE_NUMBER, 0) + 1
+    page_number = int(page_number)
+    threads = []
+    # 创建多个线程来获取数据
+    for page in range(page_number):  # 0到100页
+        end_count = (page + 1) * MAX_PAGE_NUMBER
+        begin_count = page * MAX_PAGE_NUMBER
+        if symbol is None:
+            page_df = real_time_quotes_now.loc[begin_count:end_count]
+        else:
+            page_df = real_time_quotes_now
+        thread = threading.Thread(target=update_symbol_new_concept, args=(page_df, page_number))
+        threads.append(thread)
+        thread.start()
+
+    # 等待所有线程完成
+    for thread in threads:
+        thread.join()
 
-            new_values = {'$set': {"concept_create_day": concept_create_day}}
 
-            mongodb_util.update_many(query_update, new_values, 'ths_stock_concept_detail')
+if __name__ == '__main__':
+    sync_symbol_all_concept(None)
```

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py` & `mns-scheduler-1.0.3.5/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.3.5/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.3.5/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.3.5/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.3.5/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.3.5/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.3.5/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.3.5/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.3.5/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.3.5/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py` & `mns-scheduler-1.0.3.5/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,27 +47,22 @@
     kpl_best_choose_index_number = all_kpl_best_choose_index_df.shape[0]
     page_max_number = kpl_best_choose_index_number / kpl_common_api.HIS_PAGE_MAX_COUNT
     page_number = 0
     number = 1
     for end_time in KPL_MINUTE_LIST:
         while page_number <= page_max_number:
             index = page_number * kpl_common_api.HIS_PAGE_MAX_COUNT
-            kpl_plate_best_index_df = kpl_common_api.get_plate_index_his(index, int(kpl_common_api.BEST_CHOOSE),
+            kpl_plate_best_index_df = kpl_common_api.get_plate_index_his(index, kpl_common_api.BEST_CHOOSE,
                                                                          str_day, KPL_MINUTE_BEGIN,
                                                                          end_time)
 
             if data_frame_util.is_empty(kpl_plate_best_index_df):
                 continue
             kpl_plate_best_index_df['number'] = number
             kpl_plate_best_index_df['str_day'] = str_day
-            hour = end_time[0:2]
-            minute = end_time[2:4]
-            kpl_plate_best_index_df['str_day'] = str_day
-
-            kpl_plate_best_index_df['str_now_date'] = str_day + " " + hour + ":" + minute + ":00"
             kpl_plate_best_index_df = kpl_plate_best_index_df[[
                 "plate_code",
                 "plate_name",
                 "heat_score",
                 "chg",
                 "speed",
                 "amount",
@@ -79,37 +74,37 @@
                 "super_order_net",
                 "total_mv",
                 "last_reason_organ_add",
                 "ava_pe_now",
                 "ava_pe_next",
                 "number",
                 "str_day",
-                "str_now_date"
+
             ]]
             save_kpl_his_index(kpl_plate_best_index_df, str_day, end_time)
             if end_time == KPL_MINUTE_END:
                 save_kpl_his_daily(kpl_plate_best_index_df, str_day, end_time)
             page_number = page_number + 1
         # 执行下一个时间段
         page_number = 0
         number = number + 1
 
 
 def save_kpl_his_index(kpl_plate_best_index_df, str_day, end_time):
     kpl_plate_best_index_df['_id'] = str_day + '-' + end_time + '-' + kpl_plate_best_index_df['plate_code']
-    mongodb_util.save_mongo(kpl_plate_best_index_df, db_name_constant.KPL_BEST_CHOOSE_HIS)
+    mongodb_util.insert_mongo(kpl_plate_best_index_df, db_name_constant.KPL_BEST_CHOOSE_HIS)
 
 
 def save_kpl_his_daily(kpl_plate_best_index_df, str_day, end_time):
     kpl_plate_best_index_df['_id'] = str_day + '-' + end_time + '-' + kpl_plate_best_index_df['plate_code']
     mongodb_util.save_mongo(kpl_plate_best_index_df, db_name_constant.KPL_BEST_CHOOSE_DAILY)
 
 
 def sync_all_days():
-    query = {"_id": {"$gte": '2022-07-19'}, 'trade_date': {"$lte": "2024-04-23"}}
+    query = {"_id": {"$gte": '2022-07-22'}, 'trade_date': {"$lte": "2024-04-21"}}
     trade_date_list = mongodb_util.find_query_data('trade_date_list', query)
     trade_date_list = trade_date_list.sort_values(by=['trade_date'], ascending=False)
     for trade_one in trade_date_list.itertuples():
         sync_best_choose_his_index(trade_one.trade_date)
 
 
 if __name__ == '__main__':
```

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.3.5/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.3.5/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.3.5/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.3.5/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.3.5/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.3.5/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.3.5/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.3.5/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.3.5/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.3.5/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.3.5/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.3.5/mns_scheduler/zz_task/data_sync_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,25 +20,27 @@
 import mns_scheduler.big_deal.ths_big_deal_sync as ths_big_deal_sync_api
 import mns_scheduler.zt.realtime_quotes_now_zt_kc_sync as realtime_quotes_now_zt_kc_sync_api
 import mns_scheduler.zt.export_open_data_to_excel as export_open_data_to_excel_api
 import mns_scheduler.zt.zt_five_boards_sync_api as zt_five_boards_sync_api
 import mns_scheduler.zt.zt_pool_sync_api as zt_pool_sync_api
 import mns_scheduler.zt.today_high_chg_pool_sync_api as today_high_chg_pool_sync_api
 import mns_scheduler.k_line.clean.k_line_info_clean_service as k_line_info_clean_service
-import mns_scheduler.concept.clean.ths_effective_concept_clean_api as ths_effective_concept_choose_api
+import mns_scheduler.concept.clean.ths_concept_clean_api as ths_concept_choose_api
 import mns_common.api.em.east_money_stock_gdfx_free_top_10_api as east_money_stock_gdfx_free_top_10_api
-import mns_scheduler.concept.ths.symbol.sync_concept_all_symbols_api as sync_concept_all_symbols_api
-import mns_scheduler.concept.ths.symbol.sync_symbol_all_concepts_api as sync_symbol_all_concepts_api
-import mns_scheduler.concept.ths.web.sync_ths_new_concept_by_web_api as sync_ths_new_concept_by_web_api
-import mns_scheduler.concept.ths.web.sync_ths_concept_by_ak_api as sync_ths_concept_by_ak_api
-import mns_scheduler.concept.clean.ths_effective_concept_clean_api as ths_effective_concept_clean_api
+import \
+    mns_scheduler.concept.ths.update_concept_info.sync_one_concept_all_symbols_api as sync_one_concept_all_symbols_api
+import \
+    mns_scheduler.concept.ths.update_concept_info.sync_one_symbol_all_concepts_api as sync_one_symbol_all_concepts_api
+import mns_scheduler.concept.ths.sync_new_index.sync_ths_new_concept_by_web_api as sync_ths_new_concept_by_web_api
+import mns_scheduler.concept.ths.sync_new_index.sync_ths_concept_by_ak_api as sync_ths_concept_by_ak_api
 import mns_scheduler.kpl.selection.total.sync_kpl_best_total_sync_api as sync_kpl_best_total_sync_api
 import mns_scheduler.company_info.company_info_sync_api as company_info_sync_api
 import mns_scheduler.ipo.auto_ipo_buy_api as auto_ipo_buy_api
 import mns_scheduler.kpl.selection.index.sync_best_choose_his_index as sync_best_choose_his_index
+import mns_scheduler.concept.ths.common.ths_concept_update_common_api as ths_concept_update_common_api
 
 
 # 同步交易日期任务完成
 def sync_trade_date():
     trade_date_common_service_api.sync_trade_date()
     logger.info('同步交易日期任务完成')
 
@@ -196,37 +198,42 @@
     now_date = datetime.now()
     str_day = now_date.strftime('%Y-%m-%d')
     if trade_date_common_service_api.is_trade_day(str_day):
         k_line_info_clean_service.sync_k_line_info_task(str_day)
         logger.info('计算当日k线信息完成:{}', str_day)
 
 
-#  更新空概念名称
-def update_null_name():
-    ths_effective_concept_choose_api.update_null_name()
-
-
 # 同步所有股票前十大流通股本
 def sync_stock_gdfx_free_top_10_one_day():
     logger.info('同步所有股票前十大流通股本')
     now_date = datetime.now()
     str_day = now_date.strftime('%Y-%m-%d')
     east_money_stock_gdfx_free_top_10_api.sync_stock_gdfx_free_top_10_one_day(str_day)
 
 
+# 更新同花顺概念信息
+def ths_concept_info_clean():
+    #  更新空概念名称
+    ths_concept_choose_api.update_null_name()
+    #  更新概念包含个数
+    ths_concept_choose_api.update_concept_num()
+
+
 # 同步概念下所有股票组成 by 概念指数
-def update_concept_all_symbol_detail():
+def update_one_concept_all_symbol_detail():
     logger.info('同步概念下所有股票组成')
-    sync_concept_all_symbols_api.update_concept_all_symbol_detail()
+    sync_one_concept_all_symbols_api.update_concept_all_symbol_detail()
+    update_ths_concept_choose_null_reason()
 
 
 # 同步单只股票下所有概念 by 股票代码
-def sync_symbol_all_concept():
-    sync_symbol_all_concepts_api.sync_symbol_all_concept(None)
+def update_one_symbol_all_concepts():
     logger.info('同步单只股票所有概念组成')
+    sync_one_symbol_all_concepts_api.sync_symbol_all_concept(None)
+    update_ths_concept_choose_null_reason()
 
 
 # 同步同花顺新增概念指数通过web端接口爬取 8开头
 def sync_new_concept_data_by_web():
     sync_ths_new_concept_by_web_api.sync_new_concept_data_by_web()
 
 
@@ -251,15 +258,22 @@
 
 # 同步新概念通过web端
 def sync_new_concept_data_web():
     # 同步同花顺新增概念指数通过web端接口爬取
     sync_new_concept_data_by_web()
     # 同步同花顺新增概念指数通过ak_share接口爬取
     sync_new_ths_concept_by_ak_api()
-    logger.info("同步新概念web端数据任务完成", )
+    update_ths_concept_choose_null_reason()
+    logger.info("同步新概念web端数据任务完成")
+
+
+# 更新空的入选概念
+def update_ths_concept_choose_null_reason():
+    logger.info("更新空的入选概念")
+    ths_concept_update_common_api.update_ths_concept_choose_null_reason()
 
 
 # 清洗公司基本信息
 def update_company_base_info():
     company_info_sync_api.sync_company_base_info(None)
     company_info_sync_api.fix_company_industry(None)
     logger.info('同步公司基本信息任务完成')
@@ -275,17 +289,15 @@
 
 # 同步开盘啦当日精选指数行情数据
 
 def sync_kpl_best_his_quotes():
     now_date = datetime.now()
     str_day = now_date.strftime('%Y-%m-%d')
     if trade_date_common_service_api.is_trade_day(str_day):
-        last_trade_day = trade_date_common_service_api.get_last_trade_day(str_day)
-        # 当天不能获取历史数据
-        sync_best_choose_his_index.sync_best_choose_his_index(last_trade_day)
+        sync_best_choose_his_index.sync_best_choose_his_index(str_day)
         logger.info('同步开盘啦当日精选指数行情数据任务完成')
 
 
 # # 定义BlockingScheduler
 blockingScheduler = BlockingScheduler()
 # sync_trade_date 同步交易日期
 blockingScheduler.add_job(sync_trade_date, 'cron', hour='20', minute='43')
@@ -303,35 +315,37 @@
 blockingScheduler.add_job(stock_sync_qfq_monthly, 'cron', hour='15,18', minute='35')
 
 # 数据备份
 blockingScheduler.add_job(col_data_move, 'cron', hour='15', minute='33')
 
 # 数据库健康检查
 blockingScheduler.add_job(db_status_check, 'interval', seconds=30, max_instances=4)
-# 更新空概念名称
-blockingScheduler.add_job(update_null_name, 'cron', hour='9,18', minute='01')
+
 # 同步大单数据
 blockingScheduler.add_job(sync_ths_big_deal, 'cron', hour='09', minute='30', max_instances=4)
 
 # todo 需要前后顺序执行
 # todo 当日k线信息
 # 同步一天k线 涨停 数据
 blockingScheduler.add_job(sync_daily_data_info, 'cron', hour='15,20', minute='21')
 
 # 开盘前同步当天交易需要的k线数据
 blockingScheduler.add_job(sync_today_trade_k_line_info, 'cron', hour='08', minute='30')
 
 # 同步十大流通股东信息
 blockingScheduler.add_job(sync_stock_gdfx_free_top_10_one_day, 'cron', hour='08,22', minute='23')
 
+# 更新同花顺概念信息
+blockingScheduler.add_job(ths_concept_info_clean, 'cron', hour='9,18', minute='01')
+
 # 更新概念指数下所有股票组成 by 概念代码
-blockingScheduler.add_job(update_concept_all_symbol_detail, 'cron', hour='08,18,12', minute='30')
+blockingScheduler.add_job(update_one_concept_all_symbol_detail, 'cron', hour='08,18,12', minute='30')
 
 # 同步单只股票下所有概念 by 股票代码
-blockingScheduler.add_job(sync_symbol_all_concept, 'cron', hour='09,18,12', minute='15')
+blockingScheduler.add_job(update_one_symbol_all_concepts, 'cron', hour='09,18,12', minute='15')
 
 # 开盘前同步同花顺新概念指数
 blockingScheduler.add_job(sync_new_concept_data_web, 'cron', hour='09', minute='05,10,15,20,25')
 
 # 同步同花顺新增概念指数(定时轮训,暂时10分钟)
 blockingScheduler.add_job(sync_new_concept_data_web, 'interval', minutes=10, max_instances=4)
 
@@ -346,14 +360,14 @@
 # 自动打新 打新中签高时间段 10:30-11:30
 blockingScheduler.add_job(auto_ipo_buy, 'cron', hour='10', minute='40,50')
 
 # 更新开盘啦指数关系
 blockingScheduler.add_job(update_best_choose_plate_relation, 'cron', hour='09,18', minute='25')
 
 # 更新开盘啦指数关系
-blockingScheduler.add_job(sync_kpl_best_his_quotes, 'cron', hour='16,22', minute='48')
+blockingScheduler.add_job(sync_kpl_best_his_quotes, 'cron', hour='18,22', minute='25')
 
 print('定时任务启动成功')
 blockingScheduler.start()
 
 # if __name__ == '__main__':
 #     sync_daily_data_info()
```

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.3.5/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.3/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.3.5/mns_scheduler.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 README.md
 setup.py
 mns_scheduler/__init__.py
 mns_scheduler.egg-info/PKG-INFO
 mns_scheduler.egg-info/SOURCES.txt
 mns_scheduler.egg-info/dependency_links.txt
 mns_scheduler.egg-info/top_level.txt
+mns_scheduler/backup/__init__.py
+mns_scheduler/backup/app/__init__.py
+mns_scheduler/backup/app/ths_new_concept_sync_app.py
+mns_scheduler/backup/em/__init__.py
+mns_scheduler/backup/em/em_new_concept_his_sync.py
+mns_scheduler/backup/em/em_new_concept_sync_common_api.py
+mns_scheduler/backup/em/em_new_concept_sync_web.py
+mns_scheduler/backup/wen_cai/__init__.py
+mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
 mns_scheduler/big_deal/__init__.py
 mns_scheduler/big_deal/ths_big_deal_sync.py
 mns_scheduler/company_info/__init__.py
 mns_scheduler/company_info/company_constant_data.py
 mns_scheduler/company_info/company_info_sync_api.py
 mns_scheduler/concept/__init__.py
 mns_scheduler/concept/clean/__init__.py
-mns_scheduler/concept/clean/ths_effective_concept_clean_api.py
-mns_scheduler/concept/em/__init__.py
-mns_scheduler/concept/em/em_new_concept_his_sync.py
-mns_scheduler/concept/em/em_new_concept_sync_common_api.py
-mns_scheduler/concept/em/em_new_concept_sync_web.py
+mns_scheduler/concept/clean/ths_concept_clean_api.py
 mns_scheduler/concept/ths/__init__.py
-mns_scheduler/concept/ths/app/__init__.py
-mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py
 mns_scheduler/concept/ths/common/__init__.py
 mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
 mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
-mns_scheduler/concept/ths/symbol/__init__.py
-mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py
-mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py
-mns_scheduler/concept/ths/web/__init__.py
-mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py
-mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py
-mns_scheduler/concept/ths/wen_cai/__init__.py
-mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py
+mns_scheduler/concept/ths/sync_new_index/__init__.py
+mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
+mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
+mns_scheduler/concept/ths/update_concept_info/__init__.py
+mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
+mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
 mns_scheduler/db/__init__.py
 mns_scheduler/db/col_move_service.py
 mns_scheduler/db/db_status.py
 mns_scheduler/dt/__init__.py
 mns_scheduler/dt/stock_dt_pool_sync.py
 mns_scheduler/ipo/__init__.py
 mns_scheduler/ipo/auto_ipo_buy_api.py
```

