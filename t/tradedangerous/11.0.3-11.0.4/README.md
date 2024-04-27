# Comparing `tmp/tradedangerous-11.0.3.tar.gz` & `tmp/tradedangerous-11.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradedangerous-11.0.3.tar", last modified: Fri Apr 26 09:43:30 2024, max compression
+gzip compressed data, was "tradedangerous-11.0.4.tar", last modified: Fri Apr 26 11:34:29 2024, max compression
```

## Comparing `tradedangerous-11.0.3.tar` & `tradedangerous-11.0.4.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:43:30.643313 tradedangerous-11.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-26 09:43:30.643313 tradedangerous-11.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-26 09:43:30.643313 tradedangerous-11.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:43:30.623313 tradedangerous-11.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tests/test_bootstrap_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tests/test_bootstrap_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tests/test_peek.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tests/test_trade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tests/test_trade_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:43:30.631313 tradedangerous-11.0.3/tradedangerous/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36028 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:43:30.635313 tradedangerous-11.0.3/tradedangerous/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/TEMPLATE.py
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/buildcache_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/buy_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/commandenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/export_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/import_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/local_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/market_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/nav_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/olddata_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/rares_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    47650 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/sell_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/shipvendor_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    16219 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/station_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/trade_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/update_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/commands/update_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/csvexport.py
--rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/edscupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/edsmupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)    43676 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/jsonprices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:43:30.635313 tradedangerous-11.0.3/tradedangerous/mfd/
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/mfd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:43:30.635313 tradedangerous-11.0.3/tradedangerous/mfd/saitek/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/mfd/saitek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/mfd/saitek/directoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/mfd/saitek/x52pro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:43:30.639313 tradedangerous-11.0.3/tradedangerous/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/misc/checkpricebounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/misc/clipboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/misc/coord64.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/misc/derp-sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/misc/diff-system-csvs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/misc/eddb.py
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/misc/eddn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/misc/edsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/misc/edsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/misc/importeddbstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/misc/prices-json-exp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/misc/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:43:30.639313 tradedangerous-11.0.3/tradedangerous/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42262 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/plugins/edapi_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/plugins/edcd_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    21961 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/plugins/eddblink_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/plugins/edmc_batch_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/plugins/journal_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/plugins/netlog_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    26730 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/plugins/spansh_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/prices.py
--rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/submit-distances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:43:30.639313 tradedangerous-11.0.3/tradedangerous/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/templates/Added.csv
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/templates/Category.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/templates/RareItem.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/templates/TradeDangerous.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/trade.py
--rw-r--r--   0 runner    (1001) docker     (127)    42075 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/tradecalc.py
--rw-r--r--   0 runner    (1001) docker     (127)    72220 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/tradedb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/tradeenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/tradeexcept.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/tradegui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/transfers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-26 09:42:21.000000 tradedangerous-11.0.3/tradedangerous/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-26 09:42:43.000000 tradedangerous-11.0.3/tradedangerous/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:43:30.643313 tradedangerous-11.0.3/tradedangerous.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-26 09:43:30.000000 tradedangerous-11.0.3/tradedangerous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-26 09:43:30.000000 tradedangerous-11.0.3/tradedangerous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:43:30.000000 tradedangerous-11.0.3/tradedangerous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-26 09:43:30.000000 tradedangerous-11.0.3/tradedangerous.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:43:30.000000 tradedangerous-11.0.3/tradedangerous.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-26 09:43:30.000000 tradedangerous-11.0.3/tradedangerous.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 09:43:30.000000 tradedangerous-11.0.3/tradedangerous.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.571901 tradedangerous-11.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-26 11:34:29.571901 tradedangerous-11.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-26 11:34:29.571901 tradedangerous-11.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.555901 tradedangerous-11.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_bootstrap_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_bootstrap_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_peek.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_trade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_trade_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.559901 tradedangerous-11.0.4/tradedangerous/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36071 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.563901 tradedangerous-11.0.4/tradedangerous/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/TEMPLATE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/buildcache_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/buy_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/commandenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/export_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/import_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/local_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/market_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/nav_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/olddata_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/rares_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47650 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/sell_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/shipvendor_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16219 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/station_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/trade_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/update_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/commands/update_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/csvexport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/edscupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/edsmupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43676 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/jsonprices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.563901 tradedangerous-11.0.4/tradedangerous/mfd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/mfd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.563901 tradedangerous-11.0.4/tradedangerous/mfd/saitek/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/mfd/saitek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/mfd/saitek/directoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/mfd/saitek/x52pro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.567901 tradedangerous-11.0.4/tradedangerous/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/checkpricebounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/clipboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/coord64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/derp-sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/diff-system-csvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/eddb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/eddn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/edsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/edsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/importeddbstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/prices-json-exp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/misc/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.567901 tradedangerous-11.0.4/tradedangerous/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42262 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/plugins/edapi_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/plugins/edcd_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21606 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/plugins/eddblink_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/plugins/edmc_batch_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/plugins/journal_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/plugins/netlog_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26762 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/plugins/spansh_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/submit-distances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.567901 tradedangerous-11.0.4/tradedangerous/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/templates/Added.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/templates/Category.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/templates/RareItem.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/templates/TradeDangerous.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/trade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42075 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/tradecalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72220 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/tradedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/tradeenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/tradeexcept.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/tradegui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-26 11:33:22.000000 tradedangerous-11.0.4/tradedangerous/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-26 11:33:41.000000 tradedangerous-11.0.4/tradedangerous/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:34:29.571901 tradedangerous-11.0.4/tradedangerous.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-26 11:34:29.000000 tradedangerous-11.0.4/tradedangerous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-26 11:34:29.000000 tradedangerous-11.0.4/tradedangerous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:34:29.000000 tradedangerous-11.0.4/tradedangerous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-26 11:34:29.000000 tradedangerous-11.0.4/tradedangerous.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:34:29.000000 tradedangerous-11.0.4/tradedangerous.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-26 11:34:29.000000 tradedangerous-11.0.4/tradedangerous.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 11:34:29.000000 tradedangerous-11.0.4/tradedangerous.egg-info/top_level.txt
```

### Comparing `tradedangerous-11.0.3/LICENSE` & `tradedangerous-11.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/PKG-INFO` & `tradedangerous-11.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 11.0.3
+Version: 11.0.4
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-11.0.3/README.md` & `tradedangerous-11.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/setup.py` & `tradedangerous-11.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tests/test_bootstrap_commands.py` & `tradedangerous-11.0.4/tests/test_bootstrap_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tests/test_bootstrap_plugins.py` & `tradedangerous-11.0.4/tests/test_bootstrap_plugins.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tests/test_cache.py` & `tradedangerous-11.0.4/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tests/test_commands.py` & `tradedangerous-11.0.4/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tests/test_fs.py` & `tradedangerous-11.0.4/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tests/test_peek.py` & `tradedangerous-11.0.4/tests/test_peek.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tests/test_trade.py` & `tradedangerous-11.0.4/tests/test_trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tests/test_trade_run.py` & `tradedangerous-11.0.4/tests/test_trade_run.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tests/test_utils.py` & `tradedangerous-11.0.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/__init__.py` & `tradedangerous-11.0.4/tradedangerous/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/cache.py` & `tradedangerous-11.0.4/tradedangerous/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
 class MultipleItemEntriesError(DuplicateKeyError):
     """ Raised when one item appears multiple times in the same station. """
     
     def __init__(self, fromFile: Path, lineNo: int, item: str, prevLineNo: int) -> None:
         super().__init__(fromFile, lineNo, 'item', item, prevLineNo)
 
 
-class SyntaxError(BuildCacheBaseException):
+class InvalidLineError(BuildCacheBaseException):
     """
     Raised when an invalid line is read.
     Attributes:
         problem     The problem that occurred
         text        Offending text
     """
     
@@ -254,15 +254,15 @@
     #   level <- Unknown / Low / Medium / High;
     #   Unknown <- '?';
     #   Low <- 'L';
     #   Medium <- 'M';
     #   High <- 'H';
     if reading == '?':
         return -1, -1
-    elif reading == '-':
+    if reading == '-':
         return 0, 0
     
     # extract the left most digits into unit and the last character into the level reading.
     units, level = reading[0:-1], reading[-1]
     
     # Extract the right most character as the "level" and look up its numeric value.
     levelNo = SUPPLY_LEVEL_VALUES.get(level)
@@ -600,62 +600,62 @@
             continue
         
         ########################################
         # ## "@ STAR/Station" lines.
         if text.startswith('@'):
             matches = systemStationRe.match(text)
             if not matches:
-                raise SyntaxError(priceFile, lineNo, "Unrecognized '@' line", text)
+                raise InvalidLineError(priceFile, lineNo, "Unrecognized '@' line", text)
             changeStation(matches)
             continue
         
         if not stationID:
             # Need a station to process any other type of line.
-            raise SyntaxError(priceFile, lineNo, "Expecting '@ SYSTEM / Station' line", text)
+            raise InvalidLineError(priceFile, lineNo, "Expecting '@ SYSTEM / Station' line", text)
         if stationID == DELETED:
             # Ignore all values from a deleted station/system.
             continue
         
         ########################################
         # ## "+ Category" lines
         if text.startswith('+'):
             # we now ignore these.
             continue
         
         ########################################
         # ## "Item sell buy ..." lines.
         matches = newItemPriceRe.match(text)
         if not matches:
-            raise SyntaxError(priceFile, lineNo, "Unrecognized line/syntax", text)
+            raise InvalidLineError(priceFile, lineNo, "Unrecognized line/syntax", text)
         
         processItemLine(matches)
     
     numSys = len(processedSystems)
     
     if localAdd > 0:
         tdenv.NOTE(
             "Placeholder stations are added to the local DB only "
             "(not the .CSV).\n"
             "Use 'trade.py export --table Station' "
             "if you /need/ to persist them."
         )
     
-    stations = tuple((ID,) for ID in processedStations.keys())
+    stations = tuple((ID,) for ID in processedStations)
     return stations, items, zeros, newItems, updtItems, ignItems, numSys
 
 
 ######################################################################
 
 
 def processPricesFile(tdenv: TradeEnv, db: sqlite3.Connection, pricesPath: Path, pricesFh: Optional[TextIO] = None, defaultZero: bool = False) -> None:
     tdenv.DEBUG0("Processing Prices file '{}'", pricesPath)
     
-    with pricesFh or pricesPath.open('r', encoding='utf-8') as pricesFh:
+    with (pricesFh or pricesPath.open('r', encoding='utf-8')) as fh:
         stations, items, zeros, newItems, updtItems, ignItems, numSys = processPrices(
-            tdenv, pricesFh, db, defaultZero
+            tdenv, fh, db, defaultZero
         )
     
     if not tdenv.mergeImport:
         db.executemany("""
             DELETE FROM StationItem
              WHERE station_id = ?
         """, stations)
@@ -903,15 +903,15 @@
                             prevLineNo
                         )
                     uniqueIndex[key] = lineNo
                 
                 try:
                     db.execute(sql_stmt, linein)
                     importCount += 1
-                except Exception as e:
+                except Exception as e:  # pylint: disable=broad-exception-caught
                     tdenv.WARN(
                         "*** INTERNAL ERROR: {err}\n"
                         "CSV File: {file}:{line}\n"
                         "SQL Query: {query}\n"
                         "Params: {params}\n"
                         .format(
                             err = str(e),
```

### Comparing `tradedangerous-11.0.3/tradedangerous/cli.py` & `tradedangerous-11.0.4/tradedangerous/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,42 +28,43 @@
 # please consult the file "README.md".
 #
 # DEVELOPERS: If you are a programmer who wants TD to do something
 # cool, please see the TradeDB and TradeCalc modules. TD is designed
 # to empower other programmers to do cool stuff.
 
 import os
+import sys
 import traceback
 
 from . import commands
+from . import tradeexcept
 from .commands import exceptions
 from .plugins import PluginException
 
-
 from . import tradedb
 
+if "CPROF" in os.environ:
+    import cProfile
+
 
 def main(argv = None):
-    import sys
     if not argv:
         argv = sys.argv
-    if sys.hexversion < 0x03040200:
+    if sys.hexversion < 0x03070000:
         raise SystemExit(
-            "Sorry: TradeDangerous requires Python 3.4.2 or higher.\n"
+            "Sorry: TradeDangerous requires Python 3.7 or higher.\n"
             "For assistance, see:\n"
             "\tBug Tracker: https://github.com/eyeonus/Trade-Dangerous/issues\n"
             "\tDocumentation: https://github.com/eyeonus/Trade-Dangerous/wiki\n"
             "\tEDForum Thread: https://forums.frontier.co.uk/showthread.php/441509\n"
         )
-    from . import tradeexcept
     
     try:
         try:
             if "CPROF" in os.environ:
-                import cProfile
                 cProfile.run("trade(argv)")
             else:
                 trade(argv)
         except PluginException as e:
             print("PLUGIN ERROR: {}".format(e))
             if 'EXCEPTIONS' in os.environ:
                 raise e
@@ -75,15 +76,15 @@
             sys.exit(1)
     except (UnicodeEncodeError, UnicodeDecodeError):
         print("-----------------------------------------------------------")
         print("ERROR: Unexpected unicode error in the wild!")
         print()
         print(traceback.format_exc())
         print(
-            "Please report this bug (http://kfs.org/td/issues). You may be "
+            "Please report this bug (http://github.com/eyeonus/Trade-Dangerous/issues). You may be "
             "able to work around it by using the '-q' parameter. Windows "
             "users may be able to use 'chcp.com 65001' to tell the console "
             "you want to support UTF-8 characters."
         )
 
 def trade(argv):
     """
```

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/TEMPLATE.py` & `tradedangerous-11.0.4/tradedangerous/commands/TEMPLATE.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/__init__.py` & `tradedangerous-11.0.4/tradedangerous/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/buildcache_cmd.py` & `tradedangerous-11.0.4/tradedangerous/commands/buildcache_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/buy_cmd.py` & `tradedangerous-11.0.4/tradedangerous/commands/buy_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/commandenv.py` & `tradedangerous-11.0.4/tradedangerous/commands/commandenv.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/exceptions.py` & `tradedangerous-11.0.4/tradedangerous/commands/exceptions.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/export_cmd.py` & `tradedangerous-11.0.4/tradedangerous/commands/export_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/import_cmd.py` & `tradedangerous-11.0.4/tradedangerous/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/local_cmd.py` & `tradedangerous-11.0.4/tradedangerous/commands/local_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/market_cmd.py` & `tradedangerous-11.0.4/tradedangerous/commands/market_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/nav_cmd.py` & `tradedangerous-11.0.4/tradedangerous/commands/nav_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/olddata_cmd.py` & `tradedangerous-11.0.4/tradedangerous/commands/olddata_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/parsing.py` & `tradedangerous-11.0.4/tradedangerous/commands/parsing.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/rares_cmd.py` & `tradedangerous-11.0.4/tradedangerous/commands/rares_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/run_cmd.py` & `tradedangerous-11.0.4/tradedangerous/commands/run_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/sell_cmd.py` & `tradedangerous-11.0.4/tradedangerous/commands/sell_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/shipvendor_cmd.py` & `tradedangerous-11.0.4/tradedangerous/commands/shipvendor_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/station_cmd.py` & `tradedangerous-11.0.4/tradedangerous/commands/station_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/trade_cmd.py` & `tradedangerous-11.0.4/tradedangerous/commands/trade_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/update_cmd.py` & `tradedangerous-11.0.4/tradedangerous/commands/update_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/commands/update_gui.py` & `tradedangerous-11.0.4/tradedangerous/commands/update_gui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/corrections.py` & `tradedangerous-11.0.4/tradedangerous/corrections.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/csvexport.py` & `tradedangerous-11.0.4/tradedangerous/csvexport.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 # Helpers
 ######################################################################
 
 def search_keyList(items, val):
     for row in items:
         if row['from'] == row['to'] == val:
             return row
+    return None
 
 def getUniqueIndex(conn, tableName):
     """ return all unique columns """
     idxCursor = conn.cursor()
     unqIndex = []
     for idxRow in idxCursor.execute("PRAGMA index_list('%s')" % tableName):
         if idxRow['unique']:
```

### Comparing `tradedangerous-11.0.3/tradedangerous/edscupdate.py` & `tradedangerous-11.0.4/tradedangerous/edscupdate.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/edsmupdate.py` & `tradedangerous-11.0.4/tradedangerous/edsmupdate.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/formatting.py` & `tradedangerous-11.0.4/tradedangerous/formatting.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 """
 from __future__ import annotations
 
 import itertools
 import typing
 
 if typing.TYPE_CHECKING:
-    from typing import Any, Callable, Optional
+    from typing import Any, Optional
+    from collections.abc import Callable
+
 
 class ColumnFormat:
     """
         Describes formatting of a column to be populated with data.
         
         Member Functions:
             
@@ -193,12 +195,11 @@
         print('-' * len(rowTitle))
         for row in rows:
             print(rowFmt.format(row))
     
     print("Simple usage:")
     present()
     
-    print()
-    print("Adding age ColumnFormat:")
-    
-    rowFmt.append(after='Name', col=ColumnFormat("Age", '>', 3, pre='|', post='|', key=lambda row: row['age']))
-    present()
+    #print()
+    #print("Adding age ColumnFormat:")
+    #rowFmt.append(after='Name', col=ColumnFormat("Age", '>', 3, pre='|', post='|', key=lambda row: row['age']))
+    #present()
```

### Comparing `tradedangerous-11.0.3/tradedangerous/fs.py` & `tradedangerous-11.0.4/tradedangerous/fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/gui.py` & `tradedangerous-11.0.4/tradedangerous/gui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/jsonprices.py` & `tradedangerous-11.0.4/tradedangerous/jsonprices.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/mapping.py` & `tradedangerous-11.0.4/tradedangerous/mapping.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/mfd/__init__.py` & `tradedangerous-11.0.4/tradedangerous/mfd/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/mfd/saitek/directoutput.py` & `tradedangerous-11.0.4/tradedangerous/mfd/saitek/directoutput.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/mfd/saitek/x52pro.py` & `tradedangerous-11.0.4/tradedangerous/mfd/saitek/x52pro.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/misc/checkpricebounds.py` & `tradedangerous-11.0.4/tradedangerous/misc/checkpricebounds.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/misc/clipboard.py` & `tradedangerous-11.0.4/tradedangerous/misc/clipboard.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/misc/coord64.py` & `tradedangerous-11.0.4/tradedangerous/misc/coord64.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/misc/derp-sentinel.py` & `tradedangerous-11.0.4/tradedangerous/misc/derp-sentinel.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/misc/diff-system-csvs.py` & `tradedangerous-11.0.4/tradedangerous/misc/diff-system-csvs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/misc/eddb.py` & `tradedangerous-11.0.4/tradedangerous/misc/eddb.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/misc/eddn.py` & `tradedangerous-11.0.4/tradedangerous/misc/eddn.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/misc/edsc.py` & `tradedangerous-11.0.4/tradedangerous/misc/edsc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/misc/edsm.py` & `tradedangerous-11.0.4/tradedangerous/misc/edsm.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/misc/importeddbstats.py` & `tradedangerous-11.0.4/tradedangerous/misc/importeddbstats.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/misc/prices-json-exp.py` & `tradedangerous-11.0.4/tradedangerous/misc/prices-json-exp.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/misc/progress.py` & `tradedangerous-11.0.4/tradedangerous/misc/progress.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/plugins/__init__.py` & `tradedangerous-11.0.4/tradedangerous/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/plugins/edapi_plug.py` & `tradedangerous-11.0.4/tradedangerous/plugins/edapi_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/plugins/edcd_plug.py` & `tradedangerous-11.0.4/tradedangerous/plugins/edcd_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/plugins/eddblink_plug.py` & `tradedangerous-11.0.4/tradedangerous/plugins/eddblink_plug.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,116 @@
-# ----------------------------------------------------------------
-# Import plugin that uses data files from EDDB.io and (optionally)
-# a EDDBlink_listener server to update the Database.
-# ----------------------------------------------------------------
+"""
+Import plugin that uses data files from 
+https://elite.tromador.com/ to update the Database.
+"""
+from __future__ import annotations
 import certifi
 import csv
 import datetime
 import json
 import os
 import sqlite3
 import ssl
 import time
+import typing
 
 from urllib import request
-from calendar import timegm
 from pathlib import Path
 
 from .. import plugins, cache, transfers
 from ..misc import progress as pbar
 from ..plugins import PluginException
 
+
+if typing.TYPE_CHECKING:
+    from typing import Optional
+    from .. tradeenv import TradeEnv
+
+
 # Constants
 BASE_URL = os.environ.get('TD_SERVER') or "https://elite.tromador.com/files/"
 CONTEXT=ssl.create_default_context(cafile=certifi.where())
 
 
-def request_url(url, headers=None):
+def _request_url(url, headers=None):
     data = None
     if headers:
         data = bytes(json.dumps(headers), encoding="utf-8")
     
-    return request.urlopen(request.Request(url, data=data), context=CONTEXT)
+    return request.urlopen(request.Request(url, data=data), context=CONTEXT, timeout=90)
 
 
 class DecodingError(PluginException):
     pass
 
 
-def file_line_count(from_file: Path, bufsize: int = 128 * 1024) -> int:
+def _file_line_count(from_file: Path, bufsize: int = 128 * 1024) -> int:
     """ counts the number of newline characters in a given file. """
-    # Pre-allocate a buffer so we're not putting pressure on the garbage collector,
-    # capture it's counting method so we don't have to keep looking that up on
-    # large files.
+    # Pre-allocate a buffer so we aren't putting pressure on the garbage collector.
     buf = bytearray(bufsize)
+    
+    # Capture it's counting method, so we don't have to keep looking that up on
+    # large files.
     counter = buf.count
-
+    
     total = 0
-
     with from_file.open("rb") as fh:
         # Capture the 'readinto' method to avoid lookups.
         reader = fh.readinto
 
         # read into the buffer and capture the number of bytes fetched,
         # which will be 'size' until the last read from the file.
         read = reader(buf)
         while read == bufsize:  # nominal case for large files
             total += counter(b'\n')
             read = reader(buf)
 
         # when 0 <= read < bufsize we're on the last page of the
         # file, so we need to take a slice of the buffer, which creates
         # a new object and thus we also have to lookup count. it's trivial
-        # but if you have to do it 10,000x it's definitly not a rounding error.
+        # but if you have to do it 10,000x it's definitely not a rounding error.
         return total + buf[:read].count(b'\n')
 
 
+def _count_listing_entries(tdenv: TradeEnv, listings: Path) -> int:
+    """ Calculates the number of entries in a listing file by counting the lines. """
+    if not listings.exists():
+        tdenv.NOTE("File not found, aborting: {}", listings)
+        return 0
+    
+    tdenv.DEBUG0(f"Getting total number of entries in {listings}...")
+    count = _file_line_count(listings)
+    if count <= 1:
+        if count == 1:
+            tdenv.DEBUG0("Listing count of 1 suggests nothing but a header")
+        else:
+            tdenv.DEBUG0("Listings file is empty, nothing to do.")
+        return 0
+
+    return count + 1  # kfsone: Doesn't the header already make this + 1?
+
+
+def _make_item_id_lookup(tdenv: TradeEnv, db: sqlite3.Cursor) -> frozenset[int]:
+    """ helper: retrieve the list of commodities in database. """
+    tdenv.DEBUG0("Getting list of commodities...")
+    return frozenset(cols[0] for cols in db.execute("SELECT item_id FROM Item"))
+
+
+def _make_station_id_lookup(tdenv: TradeEnv, db: sqlite3.Cursor) -> frozenset[int]:
+    """ helper: retrieve the list of station IDs in database. """
+    tdenv.DEBUG0("Getting list of stations...")
+    return frozenset(cols[0] for cols in db.execute("SELECT station_id FROM Station"))
+
+
+def _collect_station_modified_times(tdenv: TradeEnv, db: sqlite3.Cursor) -> dict[int, int]:
+    """ helper: build a list of the last modified time for all stations by id. """
+    tdenv.DEBUG0("Getting last-update times for stations...")
+    return dict(db.execute("SELECT station_id, strftime('%s', MIN(modified)) FROM StationItem GROUP BY station_id"))
+
+
 class ImportPlugin(plugins.ImportPluginBase):
     """
     Plugin that downloads data from eddb.
     """
     
     pluginOptions = {
         'item':         "Update Items using latest file from server. (Implies '-O system,station')",
@@ -109,69 +152,33 @@
         self.listingsPath = Path("listings.csv")
         self.liveListingsPath = Path("listings-live.csv")
         self.pricesPath = Path("listings.prices")
     
     def now(self):
         return datetime.datetime.now()
     
-    def execute(self, sql_cmd, args = None):
-        cur = self.tdb.getDB().cursor()
-        
-        self.tdenv.DEBUG2(f"SQL-Statement:\n'{sql_cmd},{args}'")
-        success = False
-        result = None
-        while not success:
-            try:
-                if args:
-                    result = cur.execute(sql_cmd, args)
-                else:
-                    result = cur.execute(sql_cmd)
-                success = True
-            except sqlite3.OperationalError as e:
-                if "locked" not in str(e):
-                    success = True
-                    raise sqlite3.OperationalError(e)
-                else:
-                    print("(execute) Database is locked, waiting for access.", end = "\r")
-                    time.sleep(1)
-        return result
-    
-    @staticmethod
-    def fetchIter(cursor, arraysize = 1000):
-        """
-        An iterator that uses fetchmany to keep memory usage down
-        and speed up the time to retrieve the results dramatically.
-        """
-        while True:
-            results = cursor.fetchmany(arraysize)
-            if not results:
-                break
-            for result in results:
-                yield result
-    
-
     def downloadFile(self, path):
         """
         Fetch the latest dumpfile from the website if newer than local copy.
         """
         
         def openURL(url):
-            return request_url(url, headers = {'User-Agent': 'Trade-Dangerous'})
+            return _request_url(url, headers = {'User-Agent': 'Trade-Dangerous'})
         
-        if path != self.liveListingsPath and path != self.listingsPath:
-            localPath = self.tdb.dataPath / path
+        if path not in (self.liveListingsPath, self.listingsPath):
+            localPath = Path(self.tdb.dataPath, path)
         else:
-            localPath = self.dataPath / path
+            localPath = Path(self.dataPath, path)
         
         url  = BASE_URL + str(path)
         
         self.tdenv.NOTE("Checking for update to '{}'.", path)
         try:
             response = openURL(url)
-        except Exception as e:
+        except Exception as e:  # pylint: disable=broad-exception-caught
             self.tdenv.WARN("Problem with download:\n    URL: {}\n    Error: {}", BASE_URL + str(path), str(e))
             return False
         
         url_time = response.getheader("Last-Modified")
         dumpModded = datetime.datetime.strptime(url_time, "%a, %d %b %Y %H:%M:%S %Z").timestamp()
         
         if Path.exists(localPath):
@@ -186,156 +193,145 @@
         return True
     
     def purgeSystems(self):
         """
         Purges systems from the System table that do not have any stations claiming to be in them.
         Keeps table from becoming too large because of fleet carriers moving to unpopulated systems.
         """
-        
+        db = self.tdb.getDB()
         self.tdenv.NOTE("Purging Systems with no stations: Start time = {}", self.now())
-        
-        self.execute("PRAGMA foreign_keys = OFF")
-        
-        print("Saving systems with stations.... " + str(self.now()) + "\t\t\t\t", end="\r")
-        self.execute("DROP TABLE IF EXISTS System_copy")
-        self.execute("""CREATE TABLE System_copy AS SELECT * FROM System
+
+        db.execute("PRAGMA foreign_keys = OFF")
+
+        self.tdenv.DEBUG0("Saving systems with stations.... " + str(self.now()) + "\t\t\t\t", end="\r")
+        db.execute("DROP TABLE IF EXISTS System_copy")
+        db.execute("""CREATE TABLE System_copy AS SELECT * FROM System
                             WHERE system_id IN (SELECT system_id FROM Station)
                     """)
-        
-        print("Erasing table and reinserting kept systems.... " + str(self.now()) + "\t\t\t\t", end="\r")
-        self.execute("DELETE FROM System")
-        self.execute("INSERT INTO System SELECT * FROM System_copy")
-        
-        print("Removing copy.... " + str(self.now()) + "\t\t\t\t", end="\r")
-        self.execute("PRAGMA foreign_keys = ON")
-        self.execute("DROP TABLE IF EXISTS System_copy")
-        
+
+        self.tdenv.DEBUG0("Erasing table and reinserting kept systems.... " + str(self.now()) + "\t\t\t\t", end="\r")
+        db.execute("DELETE FROM System")
+        db.execute("INSERT INTO System SELECT * FROM System_copy")
+
+        self.tdenv.DEBUG0("Removing copy.... " + str(self.now()) + "\t\t\t\t", end="\r")
+        db.execute("PRAGMA foreign_keys = ON")
+        db.execute("DROP TABLE IF EXISTS System_copy")
+
+        db.commit()
+
         self.tdenv.NOTE("Finished purging Systems. End time = {}", self.now())
     
-    def commit(self):
-        success = False
-        while not success:
-            try:
-                self.tdb.getDB().commit()
-                success = True
-            except sqlite3.OperationalError:
-                print("(commit) Database is locked, waiting for access.", end = "\r")
-                time.sleep(1)
-    
     def importListings(self, listings_file):
         """
-        Updates the market data (AKA the StationItem table) using listings.csv
+        Updates the market data (AKA the StationItem table) using listings_file
         Writes directly to database.
         """
+        listings_path = Path(self.dataPath, listings_file).absolute()
+        from_live = listings_path != Path(self.dataPath, self.listingsPath).absolute()
+        self.tdenv.NOTE("Processing market data from {}: Start time = {}. Live = {}", listings_file, self.now(), from_live)
         
-        self.tdenv.NOTE("Processing market data from {}: Start time = {}", listings_file, self.now())
-        if not (self.dataPath / listings_file).exists():
-            self.tdenv.NOTE("File not found, aborting: {}", (self.dataPath / listings_file))
+        total = _count_listing_entries(self.tdenv, listings_path)
+        if not total:
             return
+
+        stmt_unliven_station = """UPDATE StationItem SET from_live = 0 WHERE station_id = ?"""
+        stmt_flush_station   = """DELETE from StationItem WHERE station_id = ?"""
+        stmt_add_listing     = """
+            INSERT OR IGNORE INTO StationItem (
+                station_id, item_id, modified, from_live,
+                demand_price, demand_units, demand_level,
+                supply_price, supply_units, supply_level
+            )
+            VALUES (
+                ?, ?, datetime(?, 'unixepoch'), ?,
+                ?, ?, ?,
+                ?, ?, ?
+            )
+        """
         
-        total = 1
-        
-        from_live = 0 if listings_file == self.listingsPath else 1
-        
-        self.tdenv.DEBUG0(f"Getting total number of entries in {listings_file}...")
-        listings_path = Path(self.dataPath, listings_file)
-        total += file_line_count(listings_path)
-        
-        liveStmt = """UPDATE StationItem
-                    SET from_live = 0
-                    WHERE station_id = ?"""
-        
-        delStmt = "DELETE from StationItem WHERE station_id = ?"
-        
-        listingStmt = """INSERT OR IGNORE INTO StationItem
-                        (station_id, item_id, modified,
-                         demand_price, demand_units, demand_level,
-                         supply_price, supply_units, supply_level, from_live)
-                        VALUES ( ?, ?, ?, ?, ?, ?, ?, ?, ?, ? )"""
-        
-        self.tdenv.DEBUG0("Getting list of commodities...")
-        items = [cols[0] for cols in self.execute("SELECT item_id FROM Item ORDER BY item_id")]
-        
-        self.tdenv.DEBUG0("Getting list of stations...")
-        stationList = {
-            stationID
-            for (stationID,) in self.execute("SELECT station_id FROM Station")
-        }
-        
-        stationItems = dict(self.execute('SELECT station_id, UNIXEPOCH(modified) FROM StationItem').fetchall())
+        # Fetch all the items IDS
+        db = self.tdb.getDB()
+        item_lookup = _make_item_id_lookup(self.tdenv, db.cursor())
+        station_lookup = _make_station_id_lookup(self.tdenv, db.cursor())
+        last_station_update_times = _collect_station_modified_times(self.tdenv, db.cursor())
         
+        cur_station = None
         self.tdenv.DEBUG0("Processing entries...")
         with listings_path.open("r", encoding="utf-8", errors="ignore") as fh:
             prog = pbar.Progress(total, 50)
-            listings = csv.DictReader(fh)
-            
-            cur_station = -1
+
+            cursor: Optional[sqlite3.Cursor] = db.cursor()
             
-            for listing in listings:
-                if prog.increment(1, postfix = lambda value, total: f" {(value / total * 100):.0f}% {value} / {total}"):
-                    # Do a commit and close the DB every 2%.
-                    # This ensures the listings are put in the DB and the WAL is cleared.
-                    self.commit()
-                    self.tdb.close()
+            for listing in csv.DictReader(fh):
+                prog.increment(1, postfix = lambda value, total: f" {(value / total * 100):.0f}% {value} / {total}")
                 
                 station_id = int(listing['station_id'])
-                if station_id not in stationList:
+                if station_id not in station_lookup:
                     continue
                 
+                listing_time = int(listing['collected_at'])
+                
                 if station_id != cur_station:
-                    cur_station = station_id
-                    skipStation = False
+                    # commit anything from the previous station, get a new cursor
+                    db.commit()
+                    cur_station, skip_station, cursor = station_id, False, db.cursor()
                     
                     # Check if listing already exists in DB and needs updated.
-                    if stationItems.get(station_id):
+                    last_modified: int = int(last_station_update_times.get(station_id, 0))
+                    if last_modified:
                         # When the listings.csv data matches the database, update to make from_live == 0.
-                        if int(listing['collected_at']) == stationItems.get(station_id) and not from_live:
-                            self.tdenv.DEBUG1(f"Marking {cur_station} as no longer 'live'.")
-                            self.execute(liveStmt, (cur_station,))
+                        if listing_time == last_modified and not from_live:
+                            self.tdenv.DEBUG1(f"Marking {cur_station} as no longer 'live' (old={last_modified}, listing={listing_time}).")
+                            cursor.execute(stmt_unliven_station, (cur_station,))
+                            skip_station = True
+                            continue
+
                         # Unless the import file data is newer, nothing else needs to be done for this station,
                         # so the rest of the listings for this station can be skipped.
-                        if int(listing['collected_at']) <= stationItems.get(station_id):
-                            skipStation = True
+                        if listing_time <= last_modified:
+                            skip_station = True
                             continue
                         
                         # The data from the import file is newer, so we need to delete the old data for this station.
-                        self.tdenv.DEBUG1(f"Deleting old listing data for {cur_station}.")
-                        self.execute(delStmt, (cur_station,))
-                        # We've deleted all the items from this station, so remove it.
-                        del stationItems[station_id]
-
+                        self.tdenv.DEBUG1(f"Deleting old listing data for {cur_station} (old={last_modified}, listing={listing_time}).")
+                        cursor.execute(stmt_flush_station, (cur_station,))
+                        last_station_update_times[station_id] = listing_time
                 
-                if skipStation:
+                # station skip lasts until we change station id.
+                if skip_station:
                     continue
                 
                 # Since this station is not being skipped, get the data and prepare for insertion into the DB.
                 item_id = int(listing['commodity_id'])
                 # listings.csv includes rare items, which we are ignoring.
-                if item_id not in items:
+                if item_id not in item_lookup:
                     continue
-                modified = datetime.datetime.utcfromtimestamp(int(listing['collected_at'])).strftime('%Y-%m-%d %H:%M:%S')
+
                 demand_price = int(listing['sell_price'])
                 demand_units = int(listing['demand'])
-                demand_level = int(listing['demand_bracket']) if listing['demand_bracket'] != '' else -1
+                demand_level = int(listing.get('demand_bracket') or '-1')
                 supply_price = int(listing['buy_price'])
                 supply_units = int(listing['supply'])
-                supply_level = int(listing['supply_bracket']) if listing['supply_bracket'] != '' else -1
+                supply_level = int(listing.get('supply_bracket') or '-1')
                 
                 self.tdenv.DEBUG1(f"Inserting new listing data for {station_id}.")
-                self.execute(listingStmt, (station_id, item_id, modified,
-                                    demand_price, demand_units, demand_level,
-                                    supply_price, supply_units, supply_level, from_live))
+                cursor.execute(stmt_add_listing, (
+                        station_id, item_id, listing_time, from_live,
+                        demand_price, demand_units, demand_level,
+                        supply_price, supply_units, supply_level,
+                ))
             
-            # Do a final commit to be sure
-            self.commit()
-            self.tdb.close()
-            
-            while prog.value < prog.maxValue:
-                prog.increment(1, postfix = lambda value, total: " " + str(round(value / total * 100)) + "%")
-            prog.clear()
+        prog.clear()
+        
+        # Do a final commit to be sure
+        db.commit()
+        
+        self.tdenv.NOTE("Optimizing database...")
+        db.execute("VACUUM")
+        self.tdb.close()
         
         self.tdenv.NOTE("Finished processing market data. End time = {}", self.now())
     
     def run(self):
         # Create the /eddb folder for downloading the source files if it doesn't exist.
         try:
             Path(str(self.dataPath)).mkdir()
@@ -343,22 +339,21 @@
             pass
         
         # Run 'listings' by default:
         # If no options, or if only 'force', and/or 'skipvend',
         # have been passed, enable 'listings'.
         default = True
         for option in self.options:
-            # if not option in ('force', 'fallback', 'skipvend', 'progbar'):
-            if option not in ('force', 'skipvend'):
+            if option not in ('force', 'skipvend', 'purge'):
                 default = False
         if default:
             self.options["listings"] = True
         
-        # We can probably safely assume that the plugin has never been run if
-        # the prices file doesn't exist, since the plugin always generates it.
+        # We can probably safely assume that the plugin
+        # has never been run if the db file doesn't exist.
         if not (self.tdb.dataPath / Path("TradeDangerous.db")).exists():
             self.options["clean"] = True
         
         if self.getOption("clean"):
             # Rebuild the tables from scratch. Must be done on first run of plugin.
             # Can be done at anytime with the "clean" option.
             for name in [
@@ -493,15 +488,14 @@
             self.tdb.close()
             self.tdb.reloadCache()
         
         self.tdenv.ignoreUnknown = True
         
         if self.getOption("purge"):
             self.purgeSystems()
-            # self.commit()
         
         if self.getOption("listings"):
             if self.downloadFile(self.listingsPath) or self.getOption("force"):
                 self.importListings(self.listingsPath)
             if self.downloadFile(self.liveListingsPath) or self.getOption("force"):
                 self.importListings(self.liveListingsPath)
```

### Comparing `tradedangerous-11.0.3/tradedangerous/plugins/edmc_batch_plug.py` & `tradedangerous-11.0.4/tradedangerous/plugins/edmc_batch_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/plugins/journal_plug.py` & `tradedangerous-11.0.4/tradedangerous/plugins/journal_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/plugins/netlog_plug.py` & `tradedangerous-11.0.4/tradedangerous/plugins/netlog_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/plugins/spansh_plug.py` & `tradedangerous-11.0.4/tradedangerous/plugins/spansh_plug.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,33 @@
+""" Plugin for importing data from spansh """
 from __future__ import annotations
 
+from collections import namedtuple
 from contextlib import contextmanager
 from datetime import datetime, timedelta
 from pathlib import Path
+from rich.progress import Progress
 
+from .. import plugins, cache, transfers, csvexport, corrections
+
+import sqlite3
 import sys
 import time
 import typing
-from collections import namedtuple
+
+import ijson
+
 if sys.version_info.major == 3 and sys.version_info.minor >= 10:
     from dataclasses import dataclass
 else:
     dataclass = False  # pylint: disable=invalid-name
 
-from rich.progress import Progress
-import ijson
-import sqlite3
-
-from .. import plugins, cache, transfers, csvexport, corrections
-
 if typing.TYPE_CHECKING:
-    from typing import Any, Iterable, Optional
+    from typing import Any, Optional
+    from collections.abc import Iterable
     from .. tradeenv import TradeEnv
 
 SOURCE_URL = 'https://downloads.spansh.co.uk/galaxy_stations.json'
 
 STATION_TYPE_MAP = {
     'None': [0, False],
     'Outpost': [1, False],
@@ -233,19 +236,19 @@
     def print(self, *args, **kwargs) -> None:
         """ Shortcut to the TradeEnv uprint method. """
         self.tdenv.uprint(*args, **kwargs)
     
     def commit(self, *, force: bool = False) -> None:
         """ Perform a commit if required, but try not to do a crazy amount of committing. """
         if not force and not self.need_commit:
-            return self.cursor
+            return
         
         if not force and self.commit_limit > 0:
             self.commit_limit -= 1
-            return self.cursor
+            return
         
         db = self.tdb.getDB()
         db.commit()
         self.cursor = db.cursor()
         
         self.commit_limit = self.commit_rate
         self.need_commit = False
@@ -388,46 +391,46 @@
     
     def categorise_commodities(self, commodities):
         categories = {}
         for commodity in commodities:
             categories.setdefault(commodity.category, []).append(commodity)
         return categories
     
-    def execute(self, query: str, *params, commitable: bool = False) -> Optional[sqlite3.Cursor]:
+    def execute(self, query: str, *params, commitable: bool = False) -> sqlite3.Cursor:
         """ helper method that performs retriable queries and marks the transaction as needing to commit
             if the query is commitable."""
         if commitable:
             self.need_commit = True
         attempts = 5
         while True:
             try:
                 return self.cursor.execute(query, params)
             except sqlite3.OperationalError as ex:
                 if "no transaction is active" in str(ex):
                     self.print(f"no transaction for {query}")
-                    return
+                    raise
                 if not attempts:
                     raise
                 attempts -= 1
                 self.print(f'Retrying query \'{query}\': {ex!s}')
                 time.sleep(1)
     
-    def executemany(self, query: str, data: Iterable[Any], *, commitable: bool = False) -> Optional[sqlite3.Cursor]:
+    def executemany(self, query: str, data: Iterable[Any], *, commitable: bool = False) -> sqlite3.Cursor:
         """ helper method that performs retriable queries and marks the transaction as needing to commit
             if the query is commitable."""
         if commitable:
             self.need_commit = True
         attempts = 5
         while True:
             try:
                 return self.cursor.executemany(query, data)
             except sqlite3.OperationalError as ex:
                 if "no transaction is active" in str(ex):
                     self.print(f"no transaction for {query}")
-                    return
+                    raise
                 if not attempts:
                     raise
                 attempts -= 1
                 self.print(f'Retrying query \'{query}\': {ex!s}')
                 time.sleep(1)
     
     def load_known_systems(self) -> dict[int, str]:
```

### Comparing `tradedangerous-11.0.3/tradedangerous/prices.py` & `tradedangerous-11.0.4/tradedangerous/prices.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/submit-distances.py` & `tradedangerous-11.0.4/tradedangerous/submit-distances.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/templates/Added.csv` & `tradedangerous-11.0.4/tradedangerous/templates/Added.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/templates/RareItem.csv` & `tradedangerous-11.0.4/tradedangerous/templates/RareItem.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/templates/TradeDangerous.sql` & `tradedangerous-11.0.4/tradedangerous/templates/TradeDangerous.sql`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/tools.py` & `tradedangerous-11.0.4/tradedangerous/tools.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/trade.py` & `tradedangerous-11.0.4/tradedangerous/trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/tradecalc.py` & `tradedangerous-11.0.4/tradedangerous/tradecalc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/tradedb.py` & `tradedangerous-11.0.4/tradedangerous/tradedb.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/tradeenv.py` & `tradedangerous-11.0.4/tradedangerous/tradeenv.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/tradegui.py` & `tradedangerous-11.0.4/tradedangerous/tradegui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/transfers.py` & `tradedangerous-11.0.4/tradedangerous/transfers.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/utils.py` & `tradedangerous-11.0.4/tradedangerous/utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.3/tradedangerous/version.py` & `tradedangerous-11.0.4/tradedangerous/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 # this software so long as you include this copyright notice.
 # I guarantee there is at least one bug neither of us knew about.
 # --------------------------------------------------------------------
 
 """just keeper of current version"""
 
 # TODO: remember to update tests when version changes
-__version__ = '11.0.3'
+__version__ = '11.0.4'
```

### Comparing `tradedangerous-11.0.3/tradedangerous.egg-info/PKG-INFO` & `tradedangerous-11.0.4/tradedangerous.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 11.0.3
+Version: 11.0.4
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-11.0.3/tradedangerous.egg-info/SOURCES.txt` & `tradedangerous-11.0.4/tradedangerous.egg-info/SOURCES.txt`

 * *Files identical despite different names*

