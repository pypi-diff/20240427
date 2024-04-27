# Comparing `tmp/tradedangerous-11.0.4.tar.gz` & `tmp/tradedangerous-11.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradedangerous-11.0.4.tar", last modified: Fri Apr 26 11:34:29 2024, max compression
+gzip compressed data, was "tradedangerous-11.0.5.tar", last modified: Sat Apr 27 10:28:05 2024, max compression
```

## Comparing `tradedangerous-11.0.4.tar` & `tradedangerous-11.0.5.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.571901 tradedangerous-11.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-26 11:34:29.571901 tradedangerous-11.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-26 11:34:29.571901 tradedangerous-11.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.555901 tradedangerous-11.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_bootstrap_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_bootstrap_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_peek.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_trade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_trade_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.559901 tradedangerous-11.0.4/tradedangerous/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36071 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.563901 tradedangerous-11.0.4/tradedangerous/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/TEMPLATE.py
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/buildcache_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/buy_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/commandenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/export_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/import_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/local_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/market_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/nav_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/olddata_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/rares_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    47650 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/sell_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/shipvendor_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    16219 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/station_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/trade_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/update_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/update_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/csvexport.py
--rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/edscupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/edsmupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)    43676 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/jsonprices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.563901 tradedangerous-11.0.4/tradedangerous/mfd/
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/mfd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.563901 tradedangerous-11.0.4/tradedangerous/mfd/saitek/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/mfd/saitek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/mfd/saitek/directoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/mfd/saitek/x52pro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.567901 tradedangerous-11.0.4/tradedangerous/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/checkpricebounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/clipboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/coord64.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/derp-sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/diff-system-csvs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/eddb.py
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/eddn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/edsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/edsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/importeddbstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/prices-json-exp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.567901 tradedangerous-11.0.4/tradedangerous/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42262 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/plugins/edapi_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/plugins/edcd_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    21606 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/plugins/eddblink_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/plugins/edmc_batch_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/plugins/journal_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/plugins/netlog_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    26762 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/plugins/spansh_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/prices.py
--rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/submit-distances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.567901 tradedangerous-11.0.4/tradedangerous/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/templates/Added.csv
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/templates/Category.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/templates/RareItem.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/templates/TradeDangerous.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/trade.py
--rw-r--r--   0 runner    (1001) docker     (127)    42075 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/tradecalc.py
--rw-r--r--   0 runner    (1001) docker     (127)    72220 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/tradedb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/tradeenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/tradeexcept.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/tradegui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/transfers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-26 11:33:41.000000 tradedangerous-11.0.4/tradedangerous/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.571901 tradedangerous-11.0.4/tradedangerous.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-26 11:34:29.000000 tradedangerous-11.0.4/tradedangerous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-26 11:34:29.000000 tradedangerous-11.0.4/tradedangerous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:34:29.000000 tradedangerous-11.0.4/tradedangerous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-26 11:34:29.000000 tradedangerous-11.0.4/tradedangerous.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:34:29.000000 tradedangerous-11.0.4/tradedangerous.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-26 11:34:29.000000 tradedangerous-11.0.4/tradedangerous.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 11:34:29.000000 tradedangerous-11.0.4/tradedangerous.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.030022 tradedangerous-11.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-27 10:28:05.030022 tradedangerous-11.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-27 10:28:05.030022 tradedangerous-11.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.014022 tradedangerous-11.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_bootstrap_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_bootstrap_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_peek.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_trade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_trade_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/trade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.018022 tradedangerous-11.0.5/tradedangerous/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36071 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.022022 tradedangerous-11.0.5/tradedangerous/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/TEMPLATE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/buildcache_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/buy_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/commandenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/export_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/import_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/local_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/market_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/nav_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/olddata_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/rares_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47650 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/sell_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/shipvendor_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16219 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/station_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/trade_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/update_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/commands/update_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/csvexport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/edscupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/edsmupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43676 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/jsonprices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.022022 tradedangerous-11.0.5/tradedangerous/mfd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/mfd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.022022 tradedangerous-11.0.5/tradedangerous/mfd/saitek/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/mfd/saitek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/mfd/saitek/directoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/mfd/saitek/x52pro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.026022 tradedangerous-11.0.5/tradedangerous/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/checkpricebounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/clipboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/coord64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/derp-sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/diff-system-csvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/eddb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/eddn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/edsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/edsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/importeddbstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/prices-json-exp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/misc/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.026022 tradedangerous-11.0.5/tradedangerous/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42262 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/plugins/edapi_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/plugins/edcd_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21606 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/plugins/eddblink_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/plugins/edmc_batch_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/plugins/journal_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/plugins/netlog_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26801 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/plugins/spansh_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/submit-distances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.030022 tradedangerous-11.0.5/tradedangerous/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/templates/Added.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/templates/Category.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/templates/RareItem.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/templates/TradeDangerous.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42075 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/tradecalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72220 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/tradedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/tradeenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/tradeexcept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradedangerous/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-27 10:27:17.000000 tradedangerous-11.0.5/tradedangerous/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:28:05.030022 tradedangerous-11.0.5/tradedangerous.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-27 10:28:04.000000 tradedangerous-11.0.5/tradedangerous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-27 10:28:05.000000 tradedangerous-11.0.5/tradedangerous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 10:28:04.000000 tradedangerous-11.0.5/tradedangerous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-27 10:28:04.000000 tradedangerous-11.0.5/tradedangerous.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 10:28:04.000000 tradedangerous-11.0.5/tradedangerous.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-27 10:28:04.000000 tradedangerous-11.0.5/tradedangerous.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-27 10:28:04.000000 tradedangerous-11.0.5/tradedangerous.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-27 10:26:56.000000 tradedangerous-11.0.5/tradegui.py
```

### Comparing `tradedangerous-11.0.4/LICENSE` & `tradedangerous-11.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/PKG-INFO` & `tradedangerous-11.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 11.0.4
+Version: 11.0.5
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-11.0.4/README.md` & `tradedangerous-11.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/setup.py` & `tradedangerous-11.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 exec(open("tradedangerous/version.py").read())  # pylint: disable=W0122
 
 setup(name = package,
         version = __version__,  # pylint: disable=E0602
         install_requires = ["requests", "appJar", "ijson", "rich"],
         setup_requires = ["pytest-runner"],
         tests_require = ["pytest"],
-        packages = ['tradedangerous', 'tradedangerous.commands', 'tradedangerous.mfd', 'tradedangerous.mfd.saitek', 'tradedangerous.misc', 'tradedangerous.plugins'],
+        packages = ['.', 'tradedangerous', 'tradedangerous.commands', 'tradedangerous.mfd', 'tradedangerous.mfd.saitek', 'tradedangerous.misc', 'tradedangerous.plugins'],
         url = "https://github.com/eyeonus/Trade-Dangerous",
         project_urls = {
             "Bug Tracker": "https://github.com/eyeonus/Trade-Dangerous/issues",
             "Documentation": "https://github.com/eyeonus/Trade-Dangerous/wiki",
             "Source Code": "https://github.com/eyeonus/Trade-Dangerous",
         },
         author = "eyeonus",
@@ -53,13 +53,13 @@
             "Operating System :: OS Independent",
         ],
         license = "MPL",
         test_suite = "tests",
         package_data = {"tradedangerous": ["templates/TradeDangerous.sql", "templates/Added.csv", "templates/Category.csv", "templates/RareItem.csv"]},
         entry_points = {
             "console_scripts": [
-                "trade=tradedangerous.trade:main",
-                "tradegui=tradedangerous.tradegui:main"
+                "trade=trade:main",
+                "tradegui=tradegui:main"
             ]
         },
         zip_safe = False
 )
```

### Comparing `tradedangerous-11.0.4/tests/test_bootstrap_commands.py` & `tradedangerous-11.0.5/tests/test_bootstrap_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tests/test_bootstrap_plugins.py` & `tradedangerous-11.0.5/tests/test_bootstrap_plugins.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tests/test_cache.py` & `tradedangerous-11.0.5/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tests/test_commands.py` & `tradedangerous-11.0.5/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tests/test_fs.py` & `tradedangerous-11.0.5/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tests/test_peek.py` & `tradedangerous-11.0.5/tests/test_peek.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tests/test_trade.py` & `tradedangerous-11.0.5/tests/test_trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tests/test_trade_run.py` & `tradedangerous-11.0.5/tests/test_trade_run.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tests/test_utils.py` & `tradedangerous-11.0.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/__init__.py` & `tradedangerous-11.0.5/tradedangerous/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/cache.py` & `tradedangerous-11.0.5/tradedangerous/cache.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/cli.py` & `tradedangerous-11.0.5/tradedangerous/cli.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/TEMPLATE.py` & `tradedangerous-11.0.5/tradedangerous/commands/TEMPLATE.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/__init__.py` & `tradedangerous-11.0.5/tradedangerous/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/buildcache_cmd.py` & `tradedangerous-11.0.5/tradedangerous/commands/buildcache_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/buy_cmd.py` & `tradedangerous-11.0.5/tradedangerous/commands/buy_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/commandenv.py` & `tradedangerous-11.0.5/tradedangerous/commands/commandenv.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/exceptions.py` & `tradedangerous-11.0.5/tradedangerous/commands/exceptions.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/export_cmd.py` & `tradedangerous-11.0.5/tradedangerous/commands/export_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/import_cmd.py` & `tradedangerous-11.0.5/tradedangerous/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/local_cmd.py` & `tradedangerous-11.0.5/tradedangerous/commands/local_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/market_cmd.py` & `tradedangerous-11.0.5/tradedangerous/commands/market_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/nav_cmd.py` & `tradedangerous-11.0.5/tradedangerous/commands/nav_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/olddata_cmd.py` & `tradedangerous-11.0.5/tradedangerous/commands/olddata_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/parsing.py` & `tradedangerous-11.0.5/tradedangerous/commands/parsing.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/rares_cmd.py` & `tradedangerous-11.0.5/tradedangerous/commands/rares_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/run_cmd.py` & `tradedangerous-11.0.5/tradedangerous/commands/run_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/sell_cmd.py` & `tradedangerous-11.0.5/tradedangerous/commands/sell_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/shipvendor_cmd.py` & `tradedangerous-11.0.5/tradedangerous/commands/shipvendor_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/station_cmd.py` & `tradedangerous-11.0.5/tradedangerous/commands/station_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/trade_cmd.py` & `tradedangerous-11.0.5/tradedangerous/commands/trade_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/update_cmd.py` & `tradedangerous-11.0.5/tradedangerous/commands/update_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/commands/update_gui.py` & `tradedangerous-11.0.5/tradedangerous/commands/update_gui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/corrections.py` & `tradedangerous-11.0.5/tradedangerous/corrections.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/csvexport.py` & `tradedangerous-11.0.5/tradedangerous/csvexport.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/edscupdate.py` & `tradedangerous-11.0.5/tradedangerous/edscupdate.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/edsmupdate.py` & `tradedangerous-11.0.5/tradedangerous/edsmupdate.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/formatting.py` & `tradedangerous-11.0.5/tradedangerous/formatting.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/fs.py` & `tradedangerous-11.0.5/tradedangerous/fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/gui.py` & `tradedangerous-11.0.5/tradedangerous/gui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/jsonprices.py` & `tradedangerous-11.0.5/tradedangerous/jsonprices.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/mapping.py` & `tradedangerous-11.0.5/tradedangerous/mapping.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/mfd/__init__.py` & `tradedangerous-11.0.5/tradedangerous/mfd/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/mfd/saitek/directoutput.py` & `tradedangerous-11.0.5/tradedangerous/mfd/saitek/directoutput.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/mfd/saitek/x52pro.py` & `tradedangerous-11.0.5/tradedangerous/mfd/saitek/x52pro.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/misc/checkpricebounds.py` & `tradedangerous-11.0.5/tradedangerous/misc/checkpricebounds.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/misc/clipboard.py` & `tradedangerous-11.0.5/tradedangerous/misc/clipboard.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/misc/coord64.py` & `tradedangerous-11.0.5/tradedangerous/misc/coord64.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/misc/derp-sentinel.py` & `tradedangerous-11.0.5/tradedangerous/misc/derp-sentinel.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/misc/diff-system-csvs.py` & `tradedangerous-11.0.5/tradedangerous/misc/diff-system-csvs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/misc/eddb.py` & `tradedangerous-11.0.5/tradedangerous/misc/eddb.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/misc/eddn.py` & `tradedangerous-11.0.5/tradedangerous/misc/eddn.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/misc/edsc.py` & `tradedangerous-11.0.5/tradedangerous/misc/edsc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/misc/edsm.py` & `tradedangerous-11.0.5/tradedangerous/misc/edsm.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/misc/importeddbstats.py` & `tradedangerous-11.0.5/tradedangerous/misc/importeddbstats.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/misc/prices-json-exp.py` & `tradedangerous-11.0.5/tradedangerous/misc/prices-json-exp.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/misc/progress.py` & `tradedangerous-11.0.5/tradedangerous/misc/progress.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/plugins/__init__.py` & `tradedangerous-11.0.5/tradedangerous/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/plugins/edapi_plug.py` & `tradedangerous-11.0.5/tradedangerous/plugins/edapi_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/plugins/edcd_plug.py` & `tradedangerous-11.0.5/tradedangerous/plugins/edcd_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/plugins/eddblink_plug.py` & `tradedangerous-11.0.5/tradedangerous/plugins/eddblink_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/plugins/edmc_batch_plug.py` & `tradedangerous-11.0.5/tradedangerous/plugins/edmc_batch_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/plugins/journal_plug.py` & `tradedangerous-11.0.5/tradedangerous/plugins/journal_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/plugins/netlog_plug.py` & `tradedangerous-11.0.5/tradedangerous/plugins/netlog_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/plugins/spansh_plug.py` & `tradedangerous-11.0.5/tradedangerous/plugins/spansh_plug.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,41 +290,43 @@
                         self.ensure_system(system, upper_sys)
                     
                     station_count = 0
                     commodity_count = 0
                     
                     for station, commodities in stations:
                         fq_station_name = f'@{upper_sys}/{station.name}'
-                        if age_cutoff and (now - station.modified) > age_cutoff:
-                            if self.tdenv.detail:
-                                self.print(f'        |  {fq_station_name:50s}  |  Skipping station due to age: {now - station.modified}, ts: {station.modified}')
-                            progress.bump(sys_task)
-                            continue
                         
                         station_info = self.known_stations.get(station.id)
-                        if not station_info:
+                        if not station_info or station.modified > station_info[2]:
                             self.ensure_station(station)
                         elif station_info[1] != station.system_id:
                             self.print(f'        |  {station.name:50s}  |  Megaship station moved, updating system')
                             self.execute("UPDATE Station SET system_id = ? WHERE station_id = ?", station.system_id, station.id, commitable=True)
-                            self.known_stations[station.id] = (station.name, station.system_id)
+                            self.known_stations[station.id] = (station.name, station.system_id, station.modified)
                         
                         items = []
                         db_times = dict(self.execute("SELECT item_id, modified FROM StationItem WHERE station_id = ?", station.id))
                         
                         for commodity in commodities:
                             if commodity.id not in self.known_commodities:
                                 commodity = self.ensure_commodity(commodity)
                             
+                            # We're concerned with the market age, not the station age,
+                            # as they each have their own 'modified' times.
+                            if age_cutoff and (now - commodity.modified) > age_cutoff:
+                                if self.tdenv.detail:
+                                    self.print(f'        |  {fq_station_name:50s}  |  Skipping station due to age: {now - station.modified}, ts: {station.modified}')
+                                break
+                            
                             db_modified = db_times.get(commodity.id)
                             modified = parse_ts(db_modified) if db_modified else None
                             if modified and commodity.modified <= modified:
                                 # All commodities in a station will have the same modified time,
                                 # so no need to check the rest if the fist is older.
-                                if self.tdenv.detail:
+                                if self.tdenv.detail > 2:
                                     self.print(f'        |  {fq_station_name:50s}  |  Skipping older commodity data')
                                 break
                             items.append((station.id, commodity.id, commodity.modified,
                                 commodity.sell, commodity.demand, -1,
                                 commodity.buy, commodity.supply, -1, 0))
                         if items:
                             self.executemany("""INSERT OR REPLACE INTO StationItem (
@@ -333,16 +335,16 @@
                                 supply_price, supply_units, supply_level, from_live
                             ) VALUES (
                                 ?, ?, IFNULL(?, CURRENT_TIMESTAMP),
                                 ?, ?, ?,
                                 ?, ?, ?, ?
                             )""", items, commitable=True)
                             commodity_count += len(items)
-                            # Good time to save data and try to keep the transaction small
-                            self.commit()
+                        # Good time to save data and try to keep the transaction small
+                        self.commit()
                         
                         if commodity_count:
                             station_count += 1
                         progress.bump(sys_task)
                     
                     if station_count:
                         system_count += 1
@@ -356,20 +358,14 @@
                     self.commit()
                     
                     if system_count % 25 == 1:
                         avg_stations = total_station_count / (system_count or 1)
                         progress.update(f"{sys_desc}{DIM} ({total_station_count}:station:, {avg_stations:.1f}per:glowing_star:){CLOSE}")
             
             self.commit()
-            
-            # Need to make sure cached tables are updated, if changes were made
-            # if self.update_cache:
-            #     for table in [ "Item", "Station", "System" ]:
-            #         _, path = csvexport.exportTableToFile( self.tdb, self.tdenv, table )
-            
             self.tdb.close()
             
             # Need to make sure cached tables are updated
             for table in ("Item", "Station", "System", "StationItem"):
                 # _, path =
                 csvexport.exportTableToFile(self.tdb, self.tdenv, table)
             
@@ -441,15 +437,15 @@
             self.print("[purple]:thinking_face:Assuming no system data yet")
             self.tdenv.DEBUG0(f"load_known_systems query raised {e}")
             return {}
     
     def load_known_stations(self) -> dict[int, tuple[str, int]]:
         """ Returns a dictionary of {station_id -> (station_name, system_id)} for all current stations in the database. """
         try:
-            return {cols[0]: (cols[1], cols[2]) for cols in self.cursor.execute('SELECT station_id, name, system_id FROM Station')}
+            return {cols[0]: (cols[1], cols[2], parse_ts(cols[3])) for cols in self.cursor.execute('SELECT station_id, name, system_id, modified FROM Station')}
         except Exception as e:  # pylint: disable=broad-except
             self.print("[purple]:thinking_face:Assuming no station data yet")
             self.tdenv.DEBUG0(f"load_known_stations query raised {e}")
             return {}
     
     def load_known_commodities(self):
         """ Returns a dictionary of {fdev_id -> name} for all current commodities in the database. """
@@ -473,15 +469,15 @@
             self.print(f'        |  {upper_name:50s}  |  Added missing system :glowing_star:')
         self.known_systems[system.id] = system.name
     
     def ensure_station(self, station: Station) -> None:
         """ Adds a record for a station, and registers the station in the known_stations dict. """
         self.execute(
             '''
-            INSERT INTO Station (
+            INSERT OR REPLACE INTO Station (
                 system_id, station_id, name,
                 ls_from_star, max_pad_size,
                 market, blackmarket, shipyard, outfitting,
                 rearm, refuel, repair,
                 planetary,
                 modified,
                 type_id
@@ -509,17 +505,18 @@
             self.bool_yn(station.refuel),
             self.bool_yn(station.repair),
             self.bool_yn(station.planetary),
             station.modified,
             station.type,
             commitable=True,
         )
+        note = "Updated" if self.known_stations.get(station.id) else "Added"
         if self.tdenv.detail > 1:
-            self.print(f'        |  {station.name:50s}  |  Added missing station')
-        self.known_stations[station.id] = (station.name, station.system_id)
+            self.print(f'        |  {station.name:50s}  |  {note} station')
+        self.known_stations[station.id] = (station.name, station.system_id, station.modified)
     
     def ensure_commodity(self, commodity: Commodity):
         """ Adds a record for a commodity and registers the commodity in the known_commodities dict. """
         self.execute(
             '''
             INSERT INTO Item (item_id, category_id, name, fdev_id)
             VALUES (?, (SELECT category_id FROM Category WHERE upper(name) = ?), ?, ?)
```

### Comparing `tradedangerous-11.0.4/tradedangerous/prices.py` & `tradedangerous-11.0.5/tradedangerous/prices.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/submit-distances.py` & `tradedangerous-11.0.5/tradedangerous/submit-distances.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/templates/Added.csv` & `tradedangerous-11.0.5/tradedangerous/templates/Added.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/templates/RareItem.csv` & `tradedangerous-11.0.5/tradedangerous/templates/RareItem.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/templates/TradeDangerous.sql` & `tradedangerous-11.0.5/tradedangerous/templates/TradeDangerous.sql`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/tools.py` & `tradedangerous-11.0.5/tradedangerous/tools.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/trade.py` & `tradedangerous-11.0.5/trade.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,23 +29,16 @@
 # 
 # END USERS: If you are a user looking to find out how to use TD,
 # please consult the file "README.md".
 # 
 # DEVELOPERS: If you are a programmer who wants TD to do something
 # cool, please see the TradeDB and TradeCalc modules. TD is designed
 # to empower other programmers to do cool stuff.
-from __future__ import annotations
-
 from tradedangerous import cli
 
-import sys
-    
-
-def main(argv: list[tuple] = None) -> None:
-    """ Entry point for the TradeDangerous command-line app. """
-    if argv is None:
-        argv = sys.argv
-    cli.main(argv)
-
+def main(argv = None):
+  import sys
+  cli.main(sys.argv)
 
 if __name__ == "__main__":
-    cli.main(sys.argv)
+  import sys
+  cli.main(sys.argv)
```

### Comparing `tradedangerous-11.0.4/tradedangerous/tradecalc.py` & `tradedangerous-11.0.5/tradedangerous/tradecalc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/tradedb.py` & `tradedangerous-11.0.5/tradedangerous/tradedb.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/tradeenv.py` & `tradedangerous-11.0.5/tradedangerous/tradeenv.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/tradegui.py` & `tradedangerous-11.0.5/tradegui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/transfers.py` & `tradedangerous-11.0.5/tradedangerous/transfers.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/utils.py` & `tradedangerous-11.0.5/tradedangerous/utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.4/tradedangerous/version.py` & `tradedangerous-11.0.5/tradedangerous/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 # this software so long as you include this copyright notice.
 # I guarantee there is at least one bug neither of us knew about.
 # --------------------------------------------------------------------
 
 """just keeper of current version"""
 
 # TODO: remember to update tests when version changes
-__version__ = '11.0.4'
+__version__ = '11.0.5'
```

### Comparing `tradedangerous-11.0.4/tradedangerous.egg-info/PKG-INFO` & `tradedangerous-11.0.5/tradedangerous.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 11.0.4
+Version: 11.0.5
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-11.0.4/tradedangerous.egg-info/SOURCES.txt` & `tradedangerous-11.0.5/tradedangerous.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+trade.py
+tradegui.py
 tests/test_bootstrap_commands.py
 tests/test_bootstrap_plugins.py
 tests/test_cache.py
 tests/test_commands.py
 tests/test_fs.py
 tests/test_peek.py
 tests/test_tools.py
@@ -24,20 +26,18 @@
 tradedangerous/fs.py
 tradedangerous/gui.py
 tradedangerous/jsonprices.py
 tradedangerous/mapping.py
 tradedangerous/prices.py
 tradedangerous/submit-distances.py
 tradedangerous/tools.py
-tradedangerous/trade.py
 tradedangerous/tradecalc.py
 tradedangerous/tradedb.py
 tradedangerous/tradeenv.py
 tradedangerous/tradeexcept.py
-tradedangerous/tradegui.py
 tradedangerous/transfers.py
 tradedangerous/utils.py
 tradedangerous/version.py
 tradedangerous.egg-info/PKG-INFO
 tradedangerous.egg-info/SOURCES.txt
 tradedangerous.egg-info/dependency_links.txt
 tradedangerous.egg-info/entry_points.txt
```

