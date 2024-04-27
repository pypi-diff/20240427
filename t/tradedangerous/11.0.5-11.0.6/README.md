# Comparing `tmp/tradedangerous-11.0.5.tar.gz` & `tmp/tradedangerous-11.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradedangerous-11.0.5.tar", last modified: Sat Apr 27 10:28:05 2024, max compression
+gzip compressed data, was "tradedangerous-11.0.6.tar", last modified: Sat Apr 27 17:56:36 2024, max compression
```

## Comparing `tradedangerous-11.0.5.tar` & `tradedangerous-11.0.6.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.030022 tradedangerous-11.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-27 10:28:05.030022 tradedangerous-11.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-27 10:28:05.030022 tradedangerous-11.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.014022 tradedangerous-11.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_bootstrap_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_bootstrap_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_peek.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_trade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_trade_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/trade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.018022 tradedangerous-11.0.5/tradedangerous/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36071 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.022022 tradedangerous-11.0.5/tradedangerous/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/TEMPLATE.py
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/buildcache_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/buy_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/commandenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/export_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/import_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/local_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/market_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/nav_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/olddata_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/rares_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    47650 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/sell_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/shipvendor_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    16219 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/station_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/trade_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/update_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/update_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/csvexport.py
--rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/edscupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/edsmupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)    43676 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/jsonprices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.022022 tradedangerous-11.0.5/tradedangerous/mfd/
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/mfd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.022022 tradedangerous-11.0.5/tradedangerous/mfd/saitek/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/mfd/saitek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/mfd/saitek/directoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/mfd/saitek/x52pro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.026022 tradedangerous-11.0.5/tradedangerous/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/checkpricebounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/clipboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/coord64.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/derp-sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/diff-system-csvs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/eddb.py
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/eddn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/edsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/edsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/importeddbstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/prices-json-exp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.026022 tradedangerous-11.0.5/tradedangerous/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42262 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/plugins/edapi_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/plugins/edcd_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    21606 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/plugins/eddblink_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/plugins/edmc_batch_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/plugins/journal_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/plugins/netlog_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    26801 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/plugins/spansh_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/prices.py
--rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/submit-distances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.030022 tradedangerous-11.0.5/tradedangerous/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/templates/Added.csv
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/templates/Category.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/templates/RareItem.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/templates/TradeDangerous.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    42075 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/tradecalc.py
--rw-r--r--   0 runner    (1001) docker     (127)    72220 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/tradedb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/tradeenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/tradeexcept.py
--rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/transfers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-27 10:27:17.000000 tradedangerous-11.0.5/tradedangerous/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.030022 tradedangerous-11.0.5/tradedangerous.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-27 10:28:04.000000 tradedangerous-11.0.5/tradedangerous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-27 10:28:05.000000 tradedangerous-11.0.5/tradedangerous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 10:28:04.000000 tradedangerous-11.0.5/tradedangerous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-27 10:28:04.000000 tradedangerous-11.0.5/tradedangerous.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 10:28:04.000000 tradedangerous-11.0.5/tradedangerous.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-27 10:28:04.000000 tradedangerous-11.0.5/tradedangerous.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-27 10:28:04.000000 tradedangerous-11.0.5/tradedangerous.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradegui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:36.754642 tradedangerous-11.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-27 17:56:36.754642 tradedangerous-11.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-27 17:56:36.754642 tradedangerous-11.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:36.742642 tradedangerous-11.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tests/test_bootstrap_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tests/test_bootstrap_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tests/test_peek.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tests/test_trade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tests/test_trade_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/trade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:36.746642 tradedangerous-11.0.6/tradedangerous/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36071 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:36.750642 tradedangerous-11.0.6/tradedangerous/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/TEMPLATE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/buildcache_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/buy_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/commandenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/export_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/import_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/local_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/market_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/nav_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/olddata_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/rares_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47650 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/sell_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/shipvendor_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16219 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/station_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/trade_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/update_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/commands/update_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/csvexport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/edscupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/edsmupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43676 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/jsonprices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:36.750642 tradedangerous-11.0.6/tradedangerous/mfd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/mfd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:36.750642 tradedangerous-11.0.6/tradedangerous/mfd/saitek/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/mfd/saitek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/mfd/saitek/directoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/mfd/saitek/x52pro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:36.754642 tradedangerous-11.0.6/tradedangerous/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/misc/checkpricebounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/misc/clipboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/misc/coord64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/misc/derp-sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/misc/diff-system-csvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/misc/eddb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/misc/eddn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/misc/edsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/misc/edsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/misc/importeddbstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/misc/prices-json-exp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/misc/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:36.754642 tradedangerous-11.0.6/tradedangerous/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42262 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/plugins/edapi_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/plugins/edcd_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21525 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/plugins/eddblink_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/plugins/edmc_batch_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/plugins/journal_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/plugins/netlog_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27048 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/plugins/spansh_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/submit-distances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:36.754642 tradedangerous-11.0.6/tradedangerous/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/templates/Added.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/templates/Category.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/templates/RareItem.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/templates/TradeDangerous.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42075 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/tradecalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72220 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/tradedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/tradeenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/tradeexcept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradedangerous/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-27 17:55:48.000000 tradedangerous-11.0.6/tradedangerous/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:56:36.754642 tradedangerous-11.0.6/tradedangerous.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-27 17:56:36.000000 tradedangerous-11.0.6/tradedangerous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-27 17:56:36.000000 tradedangerous-11.0.6/tradedangerous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:56:36.000000 tradedangerous-11.0.6/tradedangerous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-27 17:56:36.000000 tradedangerous-11.0.6/tradedangerous.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:56:36.000000 tradedangerous-11.0.6/tradedangerous.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-27 17:56:36.000000 tradedangerous-11.0.6/tradedangerous.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-27 17:56:36.000000 tradedangerous-11.0.6/tradedangerous.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-27 17:55:28.000000 tradedangerous-11.0.6/tradegui.py
```

### Comparing `tradedangerous-11.0.5/LICENSE` & `tradedangerous-11.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/PKG-INFO` & `tradedangerous-11.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 11.0.5
+Version: 11.0.6
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-11.0.5/README.md` & `tradedangerous-11.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/setup.py` & `tradedangerous-11.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tests/test_bootstrap_commands.py` & `tradedangerous-11.0.6/tests/test_bootstrap_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tests/test_bootstrap_plugins.py` & `tradedangerous-11.0.6/tests/test_bootstrap_plugins.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tests/test_cache.py` & `tradedangerous-11.0.6/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tests/test_commands.py` & `tradedangerous-11.0.6/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tests/test_fs.py` & `tradedangerous-11.0.6/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tests/test_peek.py` & `tradedangerous-11.0.6/tests/test_peek.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tests/test_trade.py` & `tradedangerous-11.0.6/tests/test_trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tests/test_trade_run.py` & `tradedangerous-11.0.6/tests/test_trade_run.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tests/test_utils.py` & `tradedangerous-11.0.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/trade.py` & `tradedangerous-11.0.6/trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/__init__.py` & `tradedangerous-11.0.6/tradedangerous/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/cache.py` & `tradedangerous-11.0.6/tradedangerous/cache.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/cli.py` & `tradedangerous-11.0.6/tradedangerous/cli.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/TEMPLATE.py` & `tradedangerous-11.0.6/tradedangerous/commands/TEMPLATE.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/__init__.py` & `tradedangerous-11.0.6/tradedangerous/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/buildcache_cmd.py` & `tradedangerous-11.0.6/tradedangerous/commands/buildcache_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 
 
 def run(results, cmdenv, tdb: TradeDB):
     # Check that the file doesn't already exist.
     if not cmdenv.force:
         if tdb.dbPath.exists():
             raise CommandLineError(
-                "SQLite3 database '{tdb.dbFilename}' already exists.\n"
+                f"SQLite3 database '{tdb.dbFilename}' already exists.\n"
                 "Either remove the file first or use the '-f' option.")
     
     if not tdb.sqlPath.exists():
-        raise CommandLineError("SQL File does not exist: {tdb.sqlFilename}")
+        raise CommandLineError(f"SQL File does not exist: {tdb.sqlFilename}")
     
     buildCache(tdb, cmdenv)
     
     return None
```

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/buy_cmd.py` & `tradedangerous-11.0.6/tradedangerous/commands/buy_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/commandenv.py` & `tradedangerous-11.0.6/tradedangerous/commands/commandenv.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/exceptions.py` & `tradedangerous-11.0.6/tradedangerous/commands/exceptions.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/export_cmd.py` & `tradedangerous-11.0.6/tradedangerous/commands/export_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/import_cmd.py` & `tradedangerous-11.0.6/tradedangerous/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/local_cmd.py` & `tradedangerous-11.0.6/tradedangerous/commands/local_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/market_cmd.py` & `tradedangerous-11.0.6/tradedangerous/commands/market_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/nav_cmd.py` & `tradedangerous-11.0.6/tradedangerous/commands/nav_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/olddata_cmd.py` & `tradedangerous-11.0.6/tradedangerous/commands/olddata_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/parsing.py` & `tradedangerous-11.0.6/tradedangerous/commands/parsing.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/rares_cmd.py` & `tradedangerous-11.0.6/tradedangerous/commands/rares_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/run_cmd.py` & `tradedangerous-11.0.6/tradedangerous/commands/run_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/sell_cmd.py` & `tradedangerous-11.0.6/tradedangerous/commands/sell_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/shipvendor_cmd.py` & `tradedangerous-11.0.6/tradedangerous/commands/shipvendor_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/station_cmd.py` & `tradedangerous-11.0.6/tradedangerous/commands/station_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/trade_cmd.py` & `tradedangerous-11.0.6/tradedangerous/commands/trade_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/update_cmd.py` & `tradedangerous-11.0.6/tradedangerous/commands/update_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/commands/update_gui.py` & `tradedangerous-11.0.6/tradedangerous/commands/update_gui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/corrections.py` & `tradedangerous-11.0.6/tradedangerous/corrections.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/csvexport.py` & `tradedangerous-11.0.6/tradedangerous/csvexport.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/edscupdate.py` & `tradedangerous-11.0.6/tradedangerous/edscupdate.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/edsmupdate.py` & `tradedangerous-11.0.6/tradedangerous/edsmupdate.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/formatting.py` & `tradedangerous-11.0.6/tradedangerous/formatting.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/fs.py` & `tradedangerous-11.0.6/tradedangerous/fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/gui.py` & `tradedangerous-11.0.6/tradedangerous/gui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/jsonprices.py` & `tradedangerous-11.0.6/tradedangerous/jsonprices.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,26 @@
-#!/usr/bin/env python3.6
+from tradedangerous import tradedb
+from tradedangerous.tradeexcept import TradeException
 
-import tradedb
-from tradeexcept import TradeException
 import json
+import sys
+
+
+sys.stderr.write("*** WARNING: jsonprices.py is deprecated; if you rely on it, please post a github issue\n")
+
 
 class UnknownSystemError(TradeException):
     def __str__(self):
         return "Unknown System: " + ' '.join(self.args)
 
 class UnknownStationError(TradeException):
     def __str__(self):
         return "Unknown Station: " + ' '.join(self.args)
 
+
 def lookup_system(tdb, tdenv, name, x, y, z):
     try:
         system = tdb.systemByName[name.upper()]
     except KeyError:
         system = None
     if not system:
         try:
@@ -108,14 +113,21 @@
     
     try:
         blackMarket = stnData['bm'].upper()
         if blackMarket not in [ 'Y', 'N' ]:
             blackMarket = '?'
     except KeyError:
         blackMarket = '?'
+
+    try:
+        maxPadSize = stnData['mps'].upper()
+        if maxPadSize not in ['S', 'M', 'L']:
+            maxPadSize = '?'
+    except KeyError:
+        maxPadSize = '?'
     
     system = lookup_system(
             tdb, tdenv,
             sysName,
             pos[0], pos[1], pos[2],
             )
     if not system:
@@ -135,14 +147,15 @@
     
     station = lookup_station(
             tdb, tdenv,
             system,
             stnName,
             lsFromStar,
             blackMarket,
+            maxPadSize,
             )
     if not station:
         if tdenv.ignoreUnknown:
             raise UnknownStationError(stnName)
         if not tdenv.quiet:
             print("NOTE: Ignoring unknown station: {}/{}".format(
                     sysName.upper(), stnName
```

### Comparing `tradedangerous-11.0.5/tradedangerous/mapping.py` & `tradedangerous-11.0.6/tradedangerous/mapping.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/mfd/__init__.py` & `tradedangerous-11.0.6/tradedangerous/mfd/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/mfd/saitek/directoutput.py` & `tradedangerous-11.0.6/tradedangerous/mfd/saitek/directoutput.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/mfd/saitek/x52pro.py` & `tradedangerous-11.0.6/tradedangerous/mfd/saitek/x52pro.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/misc/checkpricebounds.py` & `tradedangerous-11.0.6/tradedangerous/misc/checkpricebounds.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/misc/clipboard.py` & `tradedangerous-11.0.6/tradedangerous/misc/clipboard.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/misc/coord64.py` & `tradedangerous-11.0.6/tradedangerous/misc/coord64.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/misc/derp-sentinel.py` & `tradedangerous-11.0.6/tradedangerous/misc/derp-sentinel.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/misc/diff-system-csvs.py` & `tradedangerous-11.0.6/tradedangerous/misc/diff-system-csvs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/misc/eddb.py` & `tradedangerous-11.0.6/tradedangerous/misc/eddb.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/misc/eddn.py` & `tradedangerous-11.0.6/tradedangerous/misc/eddn.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/misc/edsc.py` & `tradedangerous-11.0.6/tradedangerous/misc/edsc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/misc/edsm.py` & `tradedangerous-11.0.6/tradedangerous/misc/edsm.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/misc/importeddbstats.py` & `tradedangerous-11.0.6/tradedangerous/misc/importeddbstats.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/misc/prices-json-exp.py` & `tradedangerous-11.0.6/tradedangerous/misc/prices-json-exp.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/misc/progress.py` & `tradedangerous-11.0.6/tradedangerous/misc/progress.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/plugins/__init__.py` & `tradedangerous-11.0.6/tradedangerous/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/plugins/edapi_plug.py` & `tradedangerous-11.0.6/tradedangerous/plugins/edapi_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/plugins/edcd_plug.py` & `tradedangerous-11.0.6/tradedangerous/plugins/edcd_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/plugins/eddblink_plug.py` & `tradedangerous-11.0.6/tradedangerous/plugins/eddblink_plug.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,14 @@
         'all':          "Update everything with latest dumpfiles. (Regenerates all tables)",
         'clean':        "Erase entire database and rebuild from empty. (Regenerates all tables.)",
         'skipvend':     "Don't regenerate ShipVendors or UpgradeVendors. (Supercedes '-O all', '-O clean'.)",
         'force':        "Force regeneration of selected items even if source file not updated since previous run. "
                         "(Useful for updating Vendor tables if they were skipped during a '-O clean' run.)",
         'purge':        "Remove any empty systems that previously had fleet carriers.",
         'solo':         "Don't download crowd-sourced market data. (Implies '-O skipvend', supercedes '-O all', '-O clean', '-O listings'.)",
-        "prices":       "Backup listings to the TradeDangerous.prices cache file",
     }
     
     def __init__(self, tdb, tdenv):
         super().__init__(tdb, tdenv)
         
         self.dataPath = Path(os.environ.get('TD_EDDB')) if os.environ.get('TD_EDDB') else self.tdb.dataPath / Path("eddb")
         self.categoriesPath = Path("Category.csv")
@@ -495,15 +494,15 @@
         
         if self.getOption("listings"):
             if self.downloadFile(self.listingsPath) or self.getOption("force"):
                 self.importListings(self.listingsPath)
             if self.downloadFile(self.liveListingsPath) or self.getOption("force"):
                 self.importListings(self.liveListingsPath)
         
-        if self.getOption("prices"):
+        if self.getOption("listings"):
             self.tdenv.NOTE("Regenerating .prices file.")
             cache.regeneratePricesFile(self.tdb, self.tdenv)
         
         self.tdenv.NOTE("Import completed.")
         
         # TD doesn't need to do anything, tell it to just quit.
         return False
```

### Comparing `tradedangerous-11.0.5/tradedangerous/plugins/edmc_batch_plug.py` & `tradedangerous-11.0.6/tradedangerous/plugins/edmc_batch_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/plugins/journal_plug.py` & `tradedangerous-11.0.6/tradedangerous/plugins/journal_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/plugins/netlog_plug.py` & `tradedangerous-11.0.6/tradedangerous/plugins/netlog_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/plugins/spansh_plug.py` & `tradedangerous-11.0.6/tradedangerous/plugins/spansh_plug.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,14 +370,19 @@
                 csvexport.exportTableToFile(self.tdb, self.tdenv, table)
             
             self.print(
                 f'{timedelta(seconds=int(timing.elapsed))!s}  Done  '
                 f'{total_station_count} st  {total_commodity_count} co'
             )
         
+        with Timing() as timing:
+            self.print('Exporting to cache...')
+            cache.regeneratePricesFile(self.tdb, self.tdenv)
+            self.print(f'Cache export completed in {timedelta(seconds=int(timing.elapsed))!s}')
+        
         return False
     
     def data_stream(self):
         if self.file == '-':
             self.print('Reading prices from stdin')
             stream = sys.stdin
         elif self.file:
```

### Comparing `tradedangerous-11.0.5/tradedangerous/prices.py` & `tradedangerous-11.0.6/tradedangerous/prices.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/submit-distances.py` & `tradedangerous-11.0.6/tradedangerous/submit-distances.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,26 +17,30 @@
 import random
 import re
 import requests
 import sys
 import tradedb
 import tradeenv
 
-from misc.edsc import StarSubmission, StarSubmissionResult, SubmissionError
-from misc.clipboard import SystemNameClip
+from tradedangerous.misc.edsc import StarSubmission, StarSubmissionResult, SubmissionError
+from tradedangerous.misc.clipboard import SystemNameClip
 
 
 standardStars = [
     "SOL",
     "NEW YEMBO",
     "VESUVIT",
     "HIP 79884",
     "ASELLUS AUSTRALIS",
 ]
 
+
+sys.stderr.write("*** WARNING: submit-distances.py is deprecated; if you rely on it, please post a github issue\n")
+
+
 ############################################################################
 
 
 class UsageError(Exception):
     def __init__(self, argv, error):
         self.argv, self.error = argv, error
```

### Comparing `tradedangerous-11.0.5/tradedangerous/templates/Added.csv` & `tradedangerous-11.0.6/tradedangerous/templates/Added.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/templates/RareItem.csv` & `tradedangerous-11.0.6/tradedangerous/templates/RareItem.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/templates/TradeDangerous.sql` & `tradedangerous-11.0.6/tradedangerous/templates/TradeDangerous.sql`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/tools.py` & `tradedangerous-11.0.6/tradedangerous/tools.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/tradecalc.py` & `tradedangerous-11.0.6/tradedangerous/tradecalc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/tradedb.py` & `tradedangerous-11.0.6/tradedangerous/tradedb.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/tradeenv.py` & `tradedangerous-11.0.6/tradedangerous/tradeenv.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/transfers.py` & `tradedangerous-11.0.6/tradedangerous/transfers.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/utils.py` & `tradedangerous-11.0.6/tradedangerous/utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradedangerous/version.py` & `tradedangerous-11.0.6/tradedangerous/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 # this software so long as you include this copyright notice.
 # I guarantee there is at least one bug neither of us knew about.
 # --------------------------------------------------------------------
 
 """just keeper of current version"""
 
 # TODO: remember to update tests when version changes
-__version__ = '11.0.5'
+__version__ = '11.0.6'
```

### Comparing `tradedangerous-11.0.5/tradedangerous.egg-info/PKG-INFO` & `tradedangerous-11.0.6/tradedangerous.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 11.0.5
+Version: 11.0.6
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-11.0.5/tradedangerous.egg-info/SOURCES.txt` & `tradedangerous-11.0.6/tradedangerous.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.5/tradegui.py` & `tradedangerous-11.0.6/tradegui.py`

 * *Files identical despite different names*

