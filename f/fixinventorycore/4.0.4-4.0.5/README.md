# Comparing `tmp/fixinventorycore-4.0.4.tar.gz` & `tmp/fixinventorycore-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventorycore-4.0.4.tar", last modified: Wed Apr 24 19:32:33 2024, max compression
+gzip compressed data, was "fixinventorycore-4.0.5.tar", last modified: Fri Apr 26 23:42:38 2024, max compression
```

## Comparing `fixinventorycore-4.0.4.tar` & `fixinventorycore-4.0.5.tar`

### file list

```diff
@@ -1,754 +1,754 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.439643 fixinventorycore-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-24 19:32:33.439643 fixinventorycore-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.295643 fixinventorycore-4.0.4/fixcore/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.299643 fixinventorycore-4.0.4/fixcore/action_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/action_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/action_handlers/merge_outer_edge_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.299643 fixinventorycore-4.0.4/fixcore/analytics/
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/analytics/posthog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/analytics/recurrent_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/async_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.299643 fixinventorycore-4.0.4/fixcore/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31738 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   276866 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (127)    29181 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/cli/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/cli/tip_of_the_day.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.299643 fixinventorycore-4.0.4/fixcore/config/
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13420 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/config/config_handler_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/config/config_override_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    12670 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/config/core_config_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/console_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    35525 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/core_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.303643 fixinventorycore-4.0.4/fixcore/db/
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46365 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/arango_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/arangodb_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/arangodb_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21571 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/async_arangodb.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/configdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    31907 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/db_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/deferredouteredgedb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/entitydb.py
--rw-r--r--   0 runner    (1001) docker     (127)    87214 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/graphdb.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/jobdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/modeldb.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/packagedb.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/reportdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/runningtaskdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/system_data_db.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/templatedb.py
--rw-r--r--   0 runner    (1001) docker     (127)    13753 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/timeseriesdb.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/db/usagedb.py
--rw-r--r--   0 runner    (1001) docker     (127)    19730 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.303643 fixinventorycore-4.0.4/fixcore/graph_manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/graph_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/graph_manager/graph_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/ids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.303643 fixinventorycore-4.0.4/fixcore/infra_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/infra_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/infra_apps/local_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/infra_apps/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13696 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/infra_apps/package_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/infra_apps/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.307643 fixinventorycore-4.0.4/fixcore/jupyterlite/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.283643 fixinventorycore-4.0.4/fixcore/jupyterlite/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.307643 fixinventorycore-4.0.4/fixcore/jupyterlite/api/contents/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-24 19:32:31.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/api/contents/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.307643 fixinventorycore-4.0.4/fixcore/jupyterlite/api/translations/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 19:32:30.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/api/translations/all.json
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-24 19:32:30.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/api/translations/en.json
--rw-r--r--   0 runner    (1001) docker     (127)     3223 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/bootstrap.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.379643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/
--rw-r--r--   0 runner    (1001) docker     (127)    40339 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1053.7a56130.js
--rw-r--r--   0 runner    (1001) docker     (127)     4145 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1088.33c6076.js
--rw-r--r--   0 runner    (1001) docker     (127)     9193 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1091.1cf35e6.js
--rw-r--r--   0 runner    (1001) docker     (127)     5021 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1122.d86c258.js
--rw-r--r--   0 runner    (1001) docker     (127)     1079 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/114.1c04540.js
--rw-r--r--   0 runner    (1001) docker     (127)     4133 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1169.4cf2d13.js
--rw-r--r--   0 runner    (1001) docker     (127)     2128 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/125.4c6ac03.js
--rw-r--r--   0 runner    (1001) docker     (127)    45561 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1261.3da9a56.js
--rw-r--r--   0 runner    (1001) docker     (127)    17387 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/131.5b6a7ab.js
--rw-r--r--   0 runner    (1001) docker     (127)     2033 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1385.707019c.js
--rw-r--r--   0 runner    (1001) docker     (127)     9183 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1388.0f22ef8.js
--rw-r--r--   0 runner    (1001) docker     (127)     2081 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1418.d9431d8.js
--rw-r--r--   0 runner    (1001) docker     (127)   412668 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/142.6e89fb8.js
--rw-r--r--   0 runner    (1001) docker     (127)   457855 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1495.671bdd4.js
--rw-r--r--   0 runner    (1001) docker     (127)      493 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1495.671bdd4.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   133253 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1542.22098a5.js
--rw-r--r--   0 runner    (1001) docker     (127)      483 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1542.22098a5.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2053 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1558.548303d.js
--rw-r--r--   0 runner    (1001) docker     (127)    35637 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1584.d919fce.js
--rw-r--r--   0 runner    (1001) docker     (127)     4181 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1618.983fc32.js
--rw-r--r--   0 runner    (1001) docker     (127)    18800 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1715.ebbb93b.js
--rw-r--r--   0 runner    (1001) docker     (127)     6293 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1769.10c2b5d.js
--rw-r--r--   0 runner    (1001) docker     (127)     7983 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1815.2af66e5.js
--rw-r--r--   0 runner    (1001) docker     (127)     5509 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1837.622ebbe.js
--rw-r--r--   0 runner    (1001) docker     (127)     4941 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1846.ed084ce.js
--rw-r--r--   0 runner    (1001) docker     (127)      612 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1869.86f5778.js
--rw-r--r--   0 runner    (1001) docker     (127)    74760 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1871.7fed383.js
--rw-r--r--   0 runner    (1001) docker     (127)      945 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/1941.79180b2.js
--rw-r--r--   0 runner    (1001) docker     (127)   119985 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2065.410c3bc.js
--rw-r--r--   0 runner    (1001) docker     (127)    20937 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/214.300dbf1.js
--rw-r--r--   0 runner    (1001) docker     (127)     3072 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2188.9676797.js
--rw-r--r--   0 runner    (1001) docker     (127)     2185 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/221.59c0059.js
--rw-r--r--   0 runner    (1001) docker     (127)    16250 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2213.b58cab4.js
--rw-r--r--   0 runner    (1001) docker     (127)    82064 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2241.91c6cce.js
--rw-r--r--   0 runner    (1001) docker     (127)    47604 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2323.7e4d795.js
--rw-r--r--   0 runner    (1001) docker     (127)  1481212 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2324.aff3939.js
--rw-r--r--   0 runner    (1001) docker     (127)     4331 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2343.3cf0fe8.js
--rw-r--r--   0 runner    (1001) docker     (127)     4128 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2349.9acb0b1.js
--rw-r--r--   0 runner    (1001) docker     (127)     2129 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2363.6aa6a7f.js
--rw-r--r--   0 runner    (1001) docker     (127)     2405 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2386.5f8e2da.js
--rw-r--r--   0 runner    (1001) docker     (127)    29147 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2520.5c65366.js
--rw-r--r--   0 runner    (1001) docker     (127)    54845 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2552.6c5224e.js
--rw-r--r--   0 runner    (1001) docker     (127)    37964 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/261.431b309.js
--rw-r--r--   0 runner    (1001) docker     (127)     2784 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2622.3d61d64.js
--rw-r--r--   0 runner    (1001) docker     (127)    12742 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2666.6cce729.js
--rw-r--r--   0 runner    (1001) docker     (127)     1216 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2682.0c612a1.js
--rw-r--r--   0 runner    (1001) docker     (127)    30032 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2692.f2b8d53.js
--rw-r--r--   0 runner    (1001) docker     (127)     7589 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/270.9675bfe.js
--rw-r--r--   0 runner    (1001) docker     (127)      745 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2702.0e1a6ff.js
--rw-r--r--   0 runner    (1001) docker     (127)    55572 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/28.9f8dd00.js
--rw-r--r--   0 runner    (1001) docker     (127)     6706 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2871.e1a64a6.js
--rw-r--r--   0 runner    (1001) docker     (127)   128665 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2913.25c5e72.js
--rw-r--r--   0 runner    (1001) docker     (127)      559 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2913.25c5e72.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   256757 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2930.896decd.js
--rw-r--r--   0 runner    (1001) docker     (127)   169282 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/2955.c8d0773.js
--rw-r--r--   0 runner    (1001) docker     (127)    74307 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/306.b568c30.js
--rw-r--r--   0 runner    (1001) docker     (127)    35812 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3079.18e3c32.js
--rw-r--r--   0 runner    (1001) docker     (127)     3294 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/311.76f79fc.js
--rw-r--r--   0 runner    (1001) docker     (127)     4341 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3111.8de2d0a.js
--rw-r--r--   0 runner    (1001) docker     (127)     4545 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3154.5d8f80d.js
--rw-r--r--   0 runner    (1001) docker     (127)     4274 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3211.aa42b4a.js
--rw-r--r--   0 runner    (1001) docker     (127)     5817 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3218.758a794.js
--rw-r--r--   0 runner    (1001) docker     (127)       99 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3218.758a794.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6827 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3230.2c849ff.js
--rw-r--r--   0 runner    (1001) docker     (127)     1368 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3245.c48f805.js
--rw-r--r--   0 runner    (1001) docker     (127)     9703 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3322.428e385.js
--rw-r--r--   0 runner    (1001) docker     (127)     2505 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3336.3d4780f.js
--rw-r--r--   0 runner    (1001) docker     (127)     2502 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3370.b5d78cd.js
--rw-r--r--   0 runner    (1001) docker     (127)     5287 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3420.418f467.js
--rw-r--r--   0 runner    (1001) docker     (127)     4032 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3449.4a13bea.js
--rw-r--r--   0 runner    (1001) docker     (127)    39449 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3488.9d14a3e.js
--rw-r--r--   0 runner    (1001) docker     (127)    22236 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/35.26a4324.js
--rw-r--r--   0 runner    (1001) docker     (127)     3879 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3501.a0b897f.js
--rw-r--r--   0 runner    (1001) docker     (127)     4774 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3562.77d1e3d.js
--rw-r--r--   0 runner    (1001) docker     (127)    20774 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3604.9c8b7b0.js
--rw-r--r--   0 runner    (1001) docker     (127)     7383 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3694.3437882.js
--rw-r--r--   0 runner    (1001) docker     (127)     1837 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3700.ab2c843.js
--rw-r--r--   0 runner    (1001) docker     (127)      170 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3752.8735345.js
--rw-r--r--   0 runner    (1001) docker     (127)     6789 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3797.2bb532c.js
--rw-r--r--   0 runner    (1001) docker     (127)    15060 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/383.0385e5e.js
--rw-r--r--   0 runner    (1001) docker     (127)    31562 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3864.acf045c.js
--rw-r--r--   0 runner    (1001) docker     (127)     1466 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/3992.5a17c7b.js
--rw-r--r--   0 runner    (1001) docker     (127)    10989 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4002.d2530f2.js
--rw-r--r--   0 runner    (1001) docker     (127)     4576 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/403.ea946dc.js
--rw-r--r--   0 runner    (1001) docker     (127)     6923 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4030.8963386.js
--rw-r--r--   0 runner    (1001) docker     (127)    22224 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4035.88e3670.js
--rw-r--r--   0 runner    (1001) docker     (127)     2326 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4038.bb0e593.js
--rw-r--r--   0 runner    (1001) docker     (127)     7912 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4039.2635132.js
--rw-r--r--   0 runner    (1001) docker     (127)    12480 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4105.05362d2.js
--rw-r--r--   0 runner    (1001) docker     (127)     2689 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4148.0cb7e6d.js
--rw-r--r--   0 runner    (1001) docker     (127)     2841 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/431.f294aa7.js
--rw-r--r--   0 runner    (1001) docker     (127)    62818 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4324.992bd2c.js
--rw-r--r--   0 runner    (1001) docker     (127)   205182 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4333.fdaab90.js
--rw-r--r--   0 runner    (1001) docker     (127)     3743 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4387.f2b950d.js
--rw-r--r--   0 runner    (1001) docker     (127)     2215 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4434.547c185.js
--rw-r--r--   0 runner    (1001) docker     (127)    65652 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4478.8778446.js
--rw-r--r--   0 runner    (1001) docker     (127)     4446 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4498.fced3e4.js
--rw-r--r--   0 runner    (1001) docker     (127)    73801 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4499.7b7aa96.js
--rw-r--r--   0 runner    (1001) docker     (127)     2226 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4521.c2278f6.js
--rw-r--r--   0 runner    (1001) docker     (127)    12658 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4588.66d005c.js
--rw-r--r--   0 runner    (1001) docker     (127)   232363 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4630.32049fe.js
--rw-r--r--   0 runner    (1001) docker     (127)      366 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4630.32049fe.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2653 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4670.72adecb.js
--rw-r--r--   0 runner    (1001) docker     (127)    58986 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4780.f7ebd53.js
--rw-r--r--   0 runner    (1001) docker     (127)     2671 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4810.fdb4bef.js
--rw-r--r--   0 runner    (1001) docker     (127)     9509 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4825.0f290ff.js
--rw-r--r--   0 runner    (1001) docker     (127)     3737 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4843.96ed13d.js
--rw-r--r--   0 runner    (1001) docker     (127)   189502 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4926.3619db2.js
--rw-r--r--   0 runner    (1001) docker     (127)      160 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4926.3619db2.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4128 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4954.ac85606.js
--rw-r--r--   0 runner    (1001) docker     (127)     1574 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4965.9c0bd12.js
--rw-r--r--   0 runner    (1001) docker     (127)     3244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/4971.ba52a81.js
--rw-r--r--   0 runner    (1001) docker     (127)     1827 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/500.b866efa.js
--rw-r--r--   0 runner    (1001) docker     (127)     1303 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5008.7707efe.js
--rw-r--r--   0 runner    (1001) docker     (127)    13539 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5013.5ff10dd.js
--rw-r--r--   0 runner    (1001) docker     (127)    27124 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5019.fe7898c.js
--rw-r--r--   0 runner    (1001) docker     (127)      488 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5051.baecc00.js
--rw-r--r--   0 runner    (1001) docker     (127)     5283 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5061.d662bbf.js
--rw-r--r--   0 runner    (1001) docker     (127)    55045 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5115.c11e8fa.js
--rw-r--r--   0 runner    (1001) docker     (127)     6292 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/514.1c1b052.js
--rw-r--r--   0 runner    (1001) docker     (127)      864 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5233.96f1668.js
--rw-r--r--   0 runner    (1001) docker     (127)     3708 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5249.847f856.js
--rw-r--r--   0 runner    (1001) docker     (127)    22174 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5261.2a76287.js
--rw-r--r--   0 runner    (1001) docker     (127)    17171 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5276.069ed0f.js
--rw-r--r--   0 runner    (1001) docker     (127)     5308 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5299.4fe47ed.js
--rw-r--r--   0 runner    (1001) docker     (127)    25735 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5343.c65eb48.js
--rw-r--r--   0 runner    (1001) docker     (127)     3346 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5425.ff5465e.js
--rw-r--r--   0 runner    (1001) docker     (127)    17359 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5464.7c73ae4.js
--rw-r--r--   0 runner    (1001) docker     (127)       55 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5464.7c73ae4.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3526 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5494.db2521b.js
--rw-r--r--   0 runner    (1001) docker     (127)     1368 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5597.2470f52.js
--rw-r--r--   0 runner    (1001) docker     (127)     2456 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/563.7fd8ced.js
--rw-r--r--   0 runner    (1001) docker     (127)     2378 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5691.16de5f4.js
--rw-r--r--   0 runner    (1001) docker     (127)     1927 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5698.7febbe1.js
--rw-r--r--   0 runner    (1001) docker     (127)    16498 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5765.72d36d2.js
--rw-r--r--   0 runner    (1001) docker     (127)    16498 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5777.c1c07e5.js
--rw-r--r--   0 runner    (1001) docker     (127)     8379 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5822.7e14b54.js
--rw-r--r--   0 runner    (1001) docker     (127)    25560 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5828.e1ab6ce.js
--rw-r--r--   0 runner    (1001) docker     (127)     4057 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5834.ba430d2.js
--rw-r--r--   0 runner    (1001) docker     (127)    77942 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5850.9fd6e53.js
--rw-r--r--   0 runner    (1001) docker     (127)      857 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5945.4a06217.js
--rw-r--r--   0 runner    (1001) docker     (127)     4724 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5972.aa32cae.js
--rw-r--r--   0 runner    (1001) docker     (127)     5952 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/5996.8503bba.js
--rw-r--r--   0 runner    (1001) docker     (127)     2227 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/6139.0c4aaeb.js
--rw-r--r--   0 runner    (1001) docker     (127)   122842 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/6236.5f93bea.js
--rw-r--r--   0 runner    (1001) docker     (127)       95 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/6236.5f93bea.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    40991 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/6271.c4952fd.js
--rw-r--r--   0 runner    (1001) docker     (127)    11869 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/6281.f763d40.js
--rw-r--r--   0 runner    (1001) docker     (127)     3030 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/632.200fdf3.js
--rw-r--r--   0 runner    (1001) docker     (127)    10676 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/6417.bebf125.js
--rw-r--r--   0 runner    (1001) docker     (127)    11489 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/6433.a6cfc6e.js
--rw-r--r--   0 runner    (1001) docker     (127)    77133 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/644.0a629ee.js
--rw-r--r--   0 runner    (1001) docker     (127)      212 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/644.0a629ee.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1960 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/647.8cecbd3.js
--rw-r--r--   0 runner    (1001) docker     (127)     1303 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/6473.a97af61.js
--rw-r--r--   0 runner    (1001) docker     (127)     5819 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/653.7dd3d36.js
--rw-r--r--   0 runner    (1001) docker     (127)     9121 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/6553.a73f98d.js
--rw-r--r--   0 runner    (1001) docker     (127)   243122 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/6607.4ee069b.js
--rw-r--r--   0 runner    (1001) docker     (127)    16747 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/661.477cacc.js
--rw-r--r--   0 runner    (1001) docker     (127)    10601 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/6640.bf24711.js
--rw-r--r--   0 runner    (1001) docker     (127)    13477 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/6667.60cb1d2.js
--rw-r--r--   0 runner    (1001) docker     (127)     7469 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/67.3672096.js
--rw-r--r--   0 runner    (1001) docker     (127)    25966 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/6739.d19f4c2.js
--rw-r--r--   0 runner    (1001) docker     (127)     3497 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/677.493cb60.js
--rw-r--r--   0 runner    (1001) docker     (127)     2967 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/6788.4fb5bb9.js
--rw-r--r--   0 runner    (1001) docker     (127)     1318 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/69.fc53c91.js
--rw-r--r--   0 runner    (1001) docker     (127)     8125 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/6941.7241556.js
--rw-r--r--   0 runner    (1001) docker     (127)     4275 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/6942.bcc3a2f.js
--rw-r--r--   0 runner    (1001) docker     (127)    71168 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/6972.930242c.js
--rw-r--r--   0 runner    (1001) docker     (127)     2706 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7005.de1d9f9.js
--rw-r--r--   0 runner    (1001) docker     (127)    37281 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7010.979a827.js
--rw-r--r--   0 runner    (1001) docker     (127)     5011 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7022.6d0ffc3.js
--rw-r--r--   0 runner    (1001) docker     (127)      488 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7036.d0dae7d.js
--rw-r--r--   0 runner    (1001) docker     (127)     2980 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7054.de34848.js
--rw-r--r--   0 runner    (1001) docker     (127)     1828 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7061.30f7cf6.js
--rw-r--r--   0 runner    (1001) docker     (127)    24171 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7097.d4214d0.js
--rw-r--r--   0 runner    (1001) docker     (127)     2649 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7125.4a0562f.js
--rw-r--r--   0 runner    (1001) docker     (127)    10601 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7153.135087f.js
--rw-r--r--   0 runner    (1001) docker     (127)    79078 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7154.804d332.js
--rw-r--r--   0 runner    (1001) docker     (127)     2725 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7170.7bba13a.js
--rw-r--r--   0 runner    (1001) docker     (127)     9092 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7179.af46233.js
--rw-r--r--   0 runner    (1001) docker     (127)    50998 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7259.6d595ca.js
--rw-r--r--   0 runner    (1001) docker     (127)     1971 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7264.0ec5936.js
--rw-r--r--   0 runner    (1001) docker     (127)     4269 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7360.7b1e065.js
--rw-r--r--   0 runner    (1001) docker     (127)   210697 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7369.a12e276.js
--rw-r--r--   0 runner    (1001) docker     (127)     6663 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7378.b4f5497.js
--rw-r--r--   0 runner    (1001) docker     (127)      237 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7378.b4f5497.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    68002 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7427.368a8bc.js
--rw-r--r--   0 runner    (1001) docker     (127)     1807 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/745.83ff9e4.js
--rw-r--r--   0 runner    (1001) docker     (127)    26652 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7450.d5ee0a9.js
--rw-r--r--   0 runner    (1001) docker     (127)    38991 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7471.30d9d48.js
--rw-r--r--   0 runner    (1001) docker     (127)    28319 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7495.3c478a0.js
--rw-r--r--   0 runner    (1001) docker     (127)     4149 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7534.a755d75.js
--rw-r--r--   0 runner    (1001) docker     (127)    13033 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/755.6424780.js
--rw-r--r--   0 runner    (1001) docker     (127)    18136 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7557.bd5cd49.js
--rw-r--r--   0 runner    (1001) docker     (127)    15293 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7582.7350cc5.js
--rw-r--r--   0 runner    (1001) docker     (127)      232 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7634.7befbe5.js
--rw-r--r--   0 runner    (1001) docker     (127)   101829 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7674.93d7410.js
--rw-r--r--   0 runner    (1001) docker     (127)      849 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7803.45d27da.js
--rw-r--r--   0 runner    (1001) docker     (127)    11315 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7811.bd10193.js
--rw-r--r--   0 runner    (1001) docker     (127)      249 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7811.bd10193.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2730 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7817.6a39acf.js
--rw-r--r--   0 runner    (1001) docker     (127)    28662 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7866.e7f89f6.js
--rw-r--r--   0 runner    (1001) docker     (127)     2033 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7892.c46785d.js
--rw-r--r--   0 runner    (1001) docker     (127)     1188 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7918.506a625.js
--rw-r--r--   0 runner    (1001) docker     (127)    14437 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/792.f22b43b.js
--rw-r--r--   0 runner    (1001) docker     (127)    60194 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7969.f8f9146.js
--rw-r--r--   0 runner    (1001) docker     (127)    62260 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7995.e40b57d.js
--rw-r--r--   0 runner    (1001) docker     (127)      240 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7995.e40b57d.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26076 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/7997.46ee9b7.js
--rw-r--r--   0 runner    (1001) docker     (127)    95179 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8010.dbb2b65.js
--rw-r--r--   0 runner    (1001) docker     (127)    12379 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8103.25c6881.js
--rw-r--r--   0 runner    (1001) docker     (127)    14035 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8178.6647b58.js
--rw-r--r--   0 runner    (1001) docker     (127)    15318 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8285.46eba3a.js
--rw-r--r--   0 runner    (1001) docker     (127)     7917 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8378.d951634.js
--rw-r--r--   0 runner    (1001) docker     (127)     2679 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8381.4b39fc5.js
--rw-r--r--   0 runner    (1001) docker     (127)     1466 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8387.c2a5ccb.js
--rw-r--r--   0 runner    (1001) docker     (127)     7983 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8427.379d337.js
--rw-r--r--   0 runner    (1001) docker     (127)     1150 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8433.c26711e.js
--rw-r--r--   0 runner    (1001) docker     (127)    31538 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8443.32841be.js
--rw-r--r--   0 runner    (1001) docker     (127)     2520 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8446.d952b7d.js
--rw-r--r--   0 runner    (1001) docker     (127)    37231 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8479.7ad07d9.js
--rw-r--r--   0 runner    (1001) docker     (127)     1001 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/85.eb26499.js
--rw-r--r--   0 runner    (1001) docker     (127)    31624 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/850.16f7c82.js
--rw-r--r--   0 runner    (1001) docker     (127)     7383 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8579.7c15dcd.js
--rw-r--r--   0 runner    (1001) docker     (127)      232 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8701.9ba3e4c.js
--rw-r--r--   0 runner    (1001) docker     (127)    37514 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8734.0965980.js
--rw-r--r--   0 runner    (1001) docker     (127)     8576 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8768.cd685a6.js
--rw-r--r--   0 runner    (1001) docker     (127)      857 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8800.5b7449b.js
--rw-r--r--   0 runner    (1001) docker     (127)    17638 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8801.7946caf.js
--rw-r--r--   0 runner    (1001) docker     (127)     8107 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/883.7552b75.js
--rw-r--r--   0 runner    (1001) docker     (127)   197120 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8845.3412b3f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1144 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8845.3412b3f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12870 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8927.b773418.js
--rw-r--r--   0 runner    (1001) docker     (127)   122785 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8929.0b66a95.js
--rw-r--r--   0 runner    (1001) docker     (127)     6103 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8937.6c8605f.js
--rw-r--r--   0 runner    (1001) docker     (127)     6360 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8979.2760112.js
--rw-r--r--   0 runner    (1001) docker     (127)      949 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/8983.5db65ea.js
--rw-r--r--   0 runner    (1001) docker     (127)     6530 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/899.dd8da16.js
--rw-r--r--   0 runner    (1001) docker     (127)     2941 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9022.85c8176.js
--rw-r--r--   0 runner    (1001) docker     (127)     4058 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9037.6397c79.js
--rw-r--r--   0 runner    (1001) docker     (127)    10341 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/906.f6a46ca.js
--rw-r--r--   0 runner    (1001) docker     (127)     1032 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9060.9fe49c6.js
--rw-r--r--   0 runner    (1001) docker     (127)     8533 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9073.fadf4d8.js
--rw-r--r--   0 runner    (1001) docker     (127)      492 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9116.656701b.js
--rw-r--r--   0 runner    (1001) docker     (127)     1188 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9166.d072a52.js
--rw-r--r--   0 runner    (1001) docker     (127)     3037 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9208.10ca99e.js
--rw-r--r--   0 runner    (1001) docker     (127)     1731 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9233.b14ca62.js
--rw-r--r--   0 runner    (1001) docker     (127)     2184 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9234.488a70b.js
--rw-r--r--   0 runner    (1001) docker     (127)    22474 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9239.13871ef.js
--rw-r--r--   0 runner    (1001) docker     (127)     8960 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9244.a95e8aa.js
--rw-r--r--   0 runner    (1001) docker     (127)    11877 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9250.43c7d24.js
--rw-r--r--   0 runner    (1001) docker     (127)    29186 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/927.399dde7.js
--rw-r--r--   0 runner    (1001) docker     (127)      163 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/927.399dde7.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3037 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9282.eb25fa6.js
--rw-r--r--   0 runner    (1001) docker     (127)     4219 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9331.415f707.js
--rw-r--r--   0 runner    (1001) docker     (127)    24754 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9334.9101b2f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1342 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9372.65a2507.js
--rw-r--r--   0 runner    (1001) docker     (127)    22275 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9425.d103ed5.js
--rw-r--r--   0 runner    (1001) docker     (127)      232 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9531.5517c40.js
--rw-r--r--   0 runner    (1001) docker     (127)     2795 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9558.09c3851.js
--rw-r--r--   0 runner    (1001) docker     (127)    13560 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9565.66944bd.js
--rw-r--r--   0 runner    (1001) docker     (127)    12802 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9597.9d6c989.js
--rw-r--r--   0 runner    (1001) docker     (127)     2123 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9604.c2c5590.js
--rw-r--r--   0 runner    (1001) docker     (127)    82415 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9643.4b4e30e.js
--rw-r--r--   0 runner    (1001) docker     (127)     1562 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9676.f7b737a.js
--rw-r--r--   0 runner    (1001) docker     (127)    41456 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9799.ecf3e29.js
--rw-r--r--   0 runner    (1001) docker     (127)     8960 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9847.20223dd.js
--rw-r--r--   0 runner    (1001) docker     (127)    35515 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9866.ea3fe7f.js
--rw-r--r--   0 runner    (1001) docker     (127)    36793 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9879.951cc05.js
--rw-r--r--   0 runner    (1001) docker     (127)   246342 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/9903.633a36a.js
--rw-r--r--   0 runner    (1001) docker     (127)    40808 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_AMS-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     9908 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Calligraphic-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)     9600 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Calligraphic-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    22340 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Fraktur-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    21480 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Fraktur-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    34464 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Main-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    20832 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Main-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    34160 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Main-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19776 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Math-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19360 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Math-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    15944 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_SansSerif-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    14628 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_SansSerif-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12660 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_SansSerif-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    11852 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Script-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     5792 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Size1-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     5464 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Size2-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     3244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Size3-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     5148 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Size4-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    17604 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Typewriter-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     1116 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Vector-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)     1136 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Vector-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     1368 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Zero.woff
--rw-r--r--   0 runner    (1001) docker     (127)   134294 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   747927 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)   133988 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    89988 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    76736 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    34034 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   144714 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)    33736 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16276 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13224 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   203030 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (127)   918991 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (127)   202744 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   101648 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (127)    78268 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (127)  2437261 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/jlab_core.b96c356.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.379643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/lab/
--rw-r--r--   0 runner    (1001) docker     (127)    63254 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/lab/bundle.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.383643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.283643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.383643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1805 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/menus.json
--rw-r--r--   0 runner    (1001) docker     (127)      473 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/pages.json
--rw-r--r--   0 runner    (1001) docker     (127)      864 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/shell.json
--rw-r--r--   0 runner    (1001) docker     (127)      223 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/title.json
--rw-r--r--   0 runner    (1001) docker     (127)      832 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/top.json
--rw-r--r--   0 runner    (1001) docker     (127)      386 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/zen.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.383643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/help-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      472 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/help-extension/open.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.383643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      256 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/checkpoints.json
--rw-r--r--   0 runner    (1001) docker     (127)      560 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/edit-notebook-metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)      237 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/kernel-logo.json
--rw-r--r--   0 runner    (1001) docker     (127)      517 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/scroll-output.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.383643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      557 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/file-actions.json
--rw-r--r--   0 runner    (1001) docker     (127)     2244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/widget.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.287643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.383643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     8478 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json
--rw-r--r--   0 runner    (1001) docker     (127)     3219 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json
--rw-r--r--   0 runner    (1001) docker     (127)      543 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/property-inspector.json
--rw-r--r--   0 runner    (1001) docker     (127)     3036 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json
--rw-r--r--   0 runner    (1001) docker     (127)     2151 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/top-bar.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.387643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1379 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/notification.json
--rw-r--r--   0 runner    (1001) docker     (127)      936 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json
--rw-r--r--   0 runner    (1001) docker     (127)      563 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json
--rw-r--r--   0 runner    (1001) docker     (127)      677 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/sanitizer.json
--rw-r--r--   0 runner    (1001) docker     (127)     4575 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json
--rw-r--r--   0 runner    (1001) docker     (127)      694 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/utilityCommands.json
--rw-r--r--   0 runner    (1001) docker     (127)      457 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/workspaces.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.387643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     2518 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.387643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/celltags-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      751 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/celltags-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.387643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      444 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.387643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1849 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/inline-completer.json
--rw-r--r--   0 runner    (1001) docker     (127)     1445 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/manager.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.387643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      343 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/completer.json
--rw-r--r--   0 runner    (1001) docker     (127)      365 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/foreign.json
--rw-r--r--   0 runner    (1001) docker     (127)     3674 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.387643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     2244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json
--rw-r--r--   0 runner    (1001) docker     (127)     2244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.387643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      465 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/download.json
--rw-r--r--   0 runner    (1001) docker     (127)     3935 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.387643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     2233 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.387643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     6714 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json
--rw-r--r--   0 runner    (1001) docker     (127)      513 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json
--rw-r--r--   0 runner    (1001) docker     (127)      385 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
--rw-r--r--   0 runner    (1001) docker     (127)      477 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-with.json
--rw-r--r--   0 runner    (1001) docker     (127)     3147 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.391643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      336 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/completer.json
--rw-r--r--   0 runner    (1001) docker     (127)     6617 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.391643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/help-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      422 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/help-extension/about.json
--rw-r--r--   0 runner    (1001) docker     (127)      456 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/help-extension/jupyter-forum.json
--rw-r--r--   0 runner    (1001) docker     (127)      364 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/help-extension/launch-classic.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.391643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     2465 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.391643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.391643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      332 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (127)      782 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json
--rw-r--r--   0 runner    (1001) docker     (127)      319 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.391643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      662 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.391643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.391643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/lsp-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     2293 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/lsp-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.391643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/
--rw-r--r--   0 runner    (1001) docker     (127)    10058 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.391643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     2325 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.391643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/mathjax-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      756 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/mathjax-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.391643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/metadataform-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     2387 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/metadataform-extension/metadataforms.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.391643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      348 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/completer.json
--rw-r--r--   0 runner    (1001) docker     (127)      672 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json
--rw-r--r--   0 runner    (1001) docker     (127)     3267 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json
--rw-r--r--   0 runner    (1001) docker     (127)     3605 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tools.json
--rw-r--r--   0 runner    (1001) docker     (127)    24926 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.391643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/running-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1487 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/running-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.395643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      389 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/form-ui.json
--rw-r--r--   0 runner    (1001) docker     (127)      440 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.395643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.395643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      848 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.395643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/toc-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     2050 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/toc-extension/registry.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.395643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      551 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (127)      402 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/files.json
--rw-r--r--   0 runner    (1001) docker     (127)      572 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.395643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/translation-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1394 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.287643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlite/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.395643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlite/application-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      359 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlite/application-extension/share-file.json
--rw-r--r--   0 runner    (1001) docker     (127)   105099 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/all.json
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-24 19:32:31.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/all_federated.json
--rw-r--r--   0 runner    (1001) docker     (127)     1626 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/service-worker.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.287643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.287643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/themes/@jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.395643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/
--rw-r--r--   0 runner    (1001) docker     (127)    17882 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.395643 fixinventorycore-4.0.4/fixcore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/
--rw-r--r--   0 runner    (1001) docker     (127)    16550 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.js
--rw-r--r--   0 runner    (1001) docker     (127)   415751 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/build/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (127)     7193 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/config-utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.287643 fixinventorycore-4.0.4/fixcore/jupyterlite/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.395643 fixinventorycore-4.0.4/fixcore/jupyterlite/doc/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      303 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/doc/tree/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.395643 fixinventorycore-4.0.4/fixcore/jupyterlite/doc/workspaces/
--rw-r--r--   0 runner    (1001) docker     (127)      295 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/doc/workspaces/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.291643 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.287643 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.395643 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/
--rw-rw-rw-   0 runner    (1001) docker     (127)      219 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/install.json
--rw-rw-rw-   0 runner    (1001) docker     (127)     2343 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.399643 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/
--rw-rw-rw-   0 runner    (1001) docker     (127)     6950 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/312.749011b8237164f040ce.js
--rw-rw-rw-   0 runner    (1001) docker     (127)       88 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/312.749011b8237164f040ce.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (127)    14992 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/584.7e49152bd31ca0f8291b.js
--rw-rw-rw-   0 runner    (1001) docker     (127)       88 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/584.7e49152bd31ca0f8291b.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (127)    16598 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/5e8d6f34d83488f083fd.png
--rw-rw-rw-   0 runner    (1001) docker     (127)     6950 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/692.c1aeb4d97f766d3b4515.js
--rw-rw-rw-   0 runner    (1001) docker     (127)       88 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/692.c1aeb4d97f766d3b4515.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (127)      598 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/804.fb6a8eda889cf61eea27.js
--rw-rw-rw-   0 runner    (1001) docker     (127)     4254 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/b1c098fa349a030dacbe.png
--rw-rw-rw-   0 runner    (1001) docker     (127)     7359 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.6014628263d9ee9ca44a.js
--rw-rw-rw-   0 runner    (1001) docker     (127)      118 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (127)    13107 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.399643 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/
--rw-rw-rw-   0 runner    (1001) docker     (127)     2732 2024-04-24 19:32:18.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.407643 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/
--rw-rw-rw-   0 runner    (1001) docker     (127)     2643 2024-04-24 19:32:18.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/133.7957020c5e8bc5703dbc.js
--rw-rw-rw-   0 runner    (1001) docker     (127)     8311 2024-04-24 19:32:18.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/423.d0d3e2912c33c7566484.js
--rw-rw-rw-   0 runner    (1001) docker     (127)  3598363 2024-04-24 19:32:18.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/478.b48f45da3d88616ad3f9.js
--rw-rw-rw-   0 runner    (1001) docker     (127)     1110 2024-04-24 19:32:18.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/478.b48f45da3d88616ad3f9.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (127)    70520 2024-04-24 19:32:18.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
--rw-rw-rw-   0 runner    (1001) docker     (127)      336 2024-04-24 19:32:18.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (127)     2360 2024-04-24 19:32:18.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/657.15db1deb504caf7dbc6d.js
--rw-rw-rw-   0 runner    (1001) docker     (127)    14766 2024-04-24 19:32:18.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/855.323c80e7298812d692e7.js
--rw-rw-rw-   0 runner    (1001) docker     (127)     7706 2024-04-24 19:32:18.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.70a4f7e7a0383740860d.js
--rw-rw-rw-   0 runner    (1001) docker     (127)      118 2024-04-24 19:32:18.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (127)     5802 2024-04-24 19:32:18.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.407643 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab_pygments/
--rw-rw-rw-   0 runner    (1001) docker     (127)      199 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab_pygments/install.json
--rw-rw-rw-   0 runner    (1001) docker     (127)     5919 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab_pygments/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.407643 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/
--rw-rw-rw-   0 runner    (1001) docker     (127)      224 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
--rw-rw-rw-   0 runner    (1001) docker     (127)     8351 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/747.67662283a5707eeb4d4c.js
--rw-rw-rw-   0 runner    (1001) docker     (127)     3925 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.5cbb9d2323598fbda535.js
--rw-rw-rw-   0 runner    (1001) docker     (127)      162 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (127)     2452 2024-04-24 19:32:23.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.407643 fixinventorycore-4.0.4/fixcore/jupyterlite/files/
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/files/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4609 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (127)    20954 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/icon-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     2516 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1489 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/jupyter-lite.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-04-24 19:32:31.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/jupyter-lite.json
--rw-r--r--   0 runner    (1001) docker     (127)    11526 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/jupyterlite.schema.v0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.411643 fixinventorycore-4.0.4/fixcore/jupyterlite/lab/
--rw-r--r--   0 runner    (1001) docker     (127)   324251 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/lab/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1030 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/lab/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1489 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/lab/jupyter-lite.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      166 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/lab/jupyter-lite.json
--rw-r--r--   0 runner    (1001) docker     (127)    12425 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/lab/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.411643 fixinventorycore-4.0.4/fixcore/jupyterlite/lab/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      290 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/lab/tree/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.411643 fixinventorycore-4.0.4/fixcore/jupyterlite/lab/workspaces/
--rw-r--r--   0 runner    (1001) docker     (127)      288 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/lab/workspaces/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      690 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/manifest.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)     1088 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     1626 1985-10-26 08:15:00.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/service-worker.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.291643 fixinventorycore-4.0.4/fixcore/jupyterlite/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.411643 fixinventorycore-4.0.4/fixcore/jupyterlite/static/favicons/
--rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-24 19:32:26.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/static/favicons/favicon-busy-1.ico
--rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-24 19:32:26.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/static/favicons/favicon-busy-2.ico
--rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-24 19:32:26.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/static/favicons/favicon-busy-3.ico
--rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-24 19:32:26.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/static/favicons/favicon-file.ico
--rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-24 19:32:26.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/static/favicons/favicon-notebook.ico
--rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-24 19:32:26.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/static/favicons/favicon-terminal.ico
--rw-rw-rw-   0 runner    (1001) docker     (127)    32038 2024-04-24 19:32:26.000000 fixinventorycore-4.0.4/fixcore/jupyterlite/static/favicons/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    11967 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/message_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.415643 fixinventorycore-4.0.4/fixcore/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/model/adjust_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/model/db_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/model/exportable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    30006 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/model/graph_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/model/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    69697 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/model/model_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/model/resolve_in_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/model/transform_kind_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/model/typed_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.415643 fixinventorycore-4.0.4/fixcore/query/
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51739 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/query/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15449 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/query/query_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/query/template_expander.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/query/template_expander_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.415643 fixinventorycore-4.0.4/fixcore/report/
--rw-r--r--   0 runner    (1001) docker     (127)    19667 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/report/benchmark_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    26776 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/report/inspector_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/report/report_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.415643 fixinventorycore-4.0.4/fixcore/static/
--rw-r--r--   0 runner    (1001) docker     (127)   141248 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/static/api-doc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/static/ck-unicode-truecolor.ans
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/static/fix.css
--rw-r--r--   0 runner    (1001) docker     (127)    14617 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/static/fixinventory_logo_and_text.svg
--rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/system_start.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.419643 fixinventorycore-4.0.4/fixcore/task/
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/task/job_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/task/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/task/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/task/start_workflow_on_first_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/task/subscribers.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/task/task_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    33482 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/task/task_description.py
--rw-r--r--   0 runner    (1001) docker     (127)    30250 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/task/task_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.419643 fixinventorycore-4.0.4/fixcore/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/templates/create_first_user.html
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/templates/home.html
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.419643 fixinventorycore-4.0.4/fixcore/user/
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/user/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/user/user_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    15809 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.419643 fixinventorycore-4.0.4/fixcore/web/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/web/accesslog.py
--rw-r--r--   0 runner    (1001) docker     (127)    80914 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/web/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/web/certificate_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8726 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/web/content_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/web/directives.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/web/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/web/tsdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/fixcore/worker_task_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.435643 fixinventorycore-4.0.4/fixinventorycore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-24 19:32:33.000000 fixinventorycore-4.0.4/fixinventorycore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    30702 2024-04-24 19:32:33.000000 fixinventorycore-4.0.4/fixinventorycore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:32:33.000000 fixinventorycore-4.0.4/fixinventorycore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 19:32:33.000000 fixinventorycore-4.0.4/fixinventorycore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:32:33.000000 fixinventorycore-4.0.4/fixinventorycore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-24 19:32:33.000000 fixinventorycore-4.0.4/fixinventorycore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 19:32:33.000000 fixinventorycore-4.0.4/fixinventorycore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-24 19:32:33.439643 fixinventorycore-4.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.423643 fixinventorycore-4.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.423643 fixinventorycore-4.0.4/tests/fixcore/
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.423643 fixinventorycore-4.0.4/tests/fixcore/analytics/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/analytics/posthog_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/analytics/recurrent_events_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.427643 fixinventorycore-4.0.4/tests/fixcore/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/cli/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    65515 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/cli/command_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/cli/model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.427643 fixinventorycore-4.0.4/tests/fixcore/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/config/config_handler_service_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/config/config_override_service_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/config/core_config_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    31093 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/console_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/core_config_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.427643 fixinventorycore-4.0.4/tests/fixcore/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19729 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/db/arango_query_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/db/arangodb_functions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/db/async_arangodb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/db/configdb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/db/db_access_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/db/deferredouteredgedb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/db/entitydb.py
--rw-r--r--   0 runner    (1001) docker     (127)    41807 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/db/graphdb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/db/jobdb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/db/model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/db/modeldb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/db/reportdb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/db/runningtaskdb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/db/system_data_db_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/db/templatedb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/db/timeseriesdb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/dependencies_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.431643 fixinventorycore-4.0.4/tests/fixcore/graph_manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/graph_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/graph_manager/graph_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/hypothesis_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.431643 fixinventorycore-4.0.4/tests/fixcore/infra_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/infra_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/infra_apps/local_runtime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/infra_apps/package_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/message_bus_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.431643 fixinventorycore-4.0.4/tests/fixcore/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/model/adjust_node_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/model/db_updater_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/model/exportable_model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16753 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/model/graph_access_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/model/json_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/model/model_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28507 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/model/model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/model/resolve_in_graph_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/model/typed_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.431643 fixinventorycore-4.0.4/tests/fixcore/query/
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/query/model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18737 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/query/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/query/template_expander_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.431643 fixinventorycore-4.0.4/tests/fixcore/report/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/report/benchmark_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/report/inspector_service_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.435643 fixinventorycore-4.0.4/tests/fixcore/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/task/job_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/task/start_workflow_on_first_subscriber_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/task/subscribers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11073 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/task/task_description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/task/task_handler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.435643 fixinventorycore-4.0.4/tests/fixcore/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/user/user_management_service_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/util_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/validator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:32:33.435643 fixinventorycore-4.0.4/tests/fixcore/web/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15974 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/web/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    24351 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/web/api_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/web/auth_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/web/certificate_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/web/content_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/web/permission_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-24 19:28:53.000000 fixinventorycore-4.0.4/tests/fixcore/worker_task_queue_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.826850 fixinventorycore-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-26 23:42:38.826850 fixinventorycore-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.702849 fixinventorycore-4.0.5/fixcore/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.702849 fixinventorycore-4.0.5/fixcore/action_handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/action_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/action_handlers/merge_outer_edge_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.706849 fixinventorycore-4.0.5/fixcore/analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/analytics/posthog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/analytics/recurrent_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/async_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.706849 fixinventorycore-4.0.5/fixcore/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31738 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   276866 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29181 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/cli/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/cli/tip_of_the_day.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.706849 fixinventorycore-4.0.5/fixcore/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13420 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/config/config_handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/config/config_override_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12670 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/config/core_config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/console_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35525 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/core_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.710849 fixinventorycore-4.0.5/fixcore/db/
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46365 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/arango_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/arangodb_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/arangodb_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21571 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/async_arangodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/configdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31907 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/db_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/deferredouteredgedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/entitydb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87214 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/graphdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/jobdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/modeldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/packagedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/reportdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/runningtaskdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/system_data_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/templatedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13753 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/timeseriesdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/db/usagedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19730 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.710849 fixinventorycore-4.0.5/fixcore/graph_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/graph_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/graph_manager/graph_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/ids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.710849 fixinventorycore-4.0.5/fixcore/infra_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/infra_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/infra_apps/local_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/infra_apps/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13696 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/infra_apps/package_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/infra_apps/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.710849 fixinventorycore-4.0.5/fixcore/jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.690849 fixinventorycore-4.0.5/fixcore/jupyterlite/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.714849 fixinventorycore-4.0.5/fixcore/jupyterlite/api/contents/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-26 23:42:36.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/api/contents/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.714849 fixinventorycore-4.0.5/fixcore/jupyterlite/api/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-26 23:42:36.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/api/translations/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-26 23:42:36.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/api/translations/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/bootstrap.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.782850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/
+-rw-r--r--   0 runner    (1001) docker     (127)    40339 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1053.7a56130.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1088.33c6076.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9193 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1091.1cf35e6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1122.d86c258.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/114.1c04540.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1169.4cf2d13.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/125.4c6ac03.js
+-rw-r--r--   0 runner    (1001) docker     (127)    45561 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1261.3da9a56.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17387 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/131.5b6a7ab.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1385.707019c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1388.0f22ef8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1418.d9431d8.js
+-rw-r--r--   0 runner    (1001) docker     (127)   412668 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/142.6e89fb8.js
+-rw-r--r--   0 runner    (1001) docker     (127)   457855 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1495.671bdd4.js
+-rw-r--r--   0 runner    (1001) docker     (127)      493 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1495.671bdd4.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   133253 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1542.22098a5.js
+-rw-r--r--   0 runner    (1001) docker     (127)      483 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1542.22098a5.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1558.548303d.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35637 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1584.d919fce.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1618.983fc32.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18800 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1715.ebbb93b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1769.10c2b5d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1815.2af66e5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1837.622ebbe.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1846.ed084ce.js
+-rw-r--r--   0 runner    (1001) docker     (127)      612 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1869.86f5778.js
+-rw-r--r--   0 runner    (1001) docker     (127)    74760 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1871.7fed383.js
+-rw-r--r--   0 runner    (1001) docker     (127)      945 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/1941.79180b2.js
+-rw-r--r--   0 runner    (1001) docker     (127)   119985 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2065.410c3bc.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20937 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/214.300dbf1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2188.9676797.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/221.59c0059.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16250 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2213.b58cab4.js
+-rw-r--r--   0 runner    (1001) docker     (127)    82064 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2241.91c6cce.js
+-rw-r--r--   0 runner    (1001) docker     (127)    47604 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2323.7e4d795.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1481212 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2324.aff3939.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2343.3cf0fe8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2349.9acb0b1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2363.6aa6a7f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2386.5f8e2da.js
+-rw-r--r--   0 runner    (1001) docker     (127)    29147 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2520.5c65366.js
+-rw-r--r--   0 runner    (1001) docker     (127)    54845 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2552.6c5224e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    37964 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/261.431b309.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2622.3d61d64.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12742 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2666.6cce729.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2682.0c612a1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    30032 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2692.f2b8d53.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/270.9675bfe.js
+-rw-r--r--   0 runner    (1001) docker     (127)      745 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2702.0e1a6ff.js
+-rw-r--r--   0 runner    (1001) docker     (127)    55572 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/28.9f8dd00.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2871.e1a64a6.js
+-rw-r--r--   0 runner    (1001) docker     (127)   128665 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2913.25c5e72.js
+-rw-r--r--   0 runner    (1001) docker     (127)      559 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2913.25c5e72.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   256757 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2930.896decd.js
+-rw-r--r--   0 runner    (1001) docker     (127)   169282 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/2955.c8d0773.js
+-rw-r--r--   0 runner    (1001) docker     (127)    74307 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/306.b568c30.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35812 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3079.18e3c32.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/311.76f79fc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3111.8de2d0a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3154.5d8f80d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3211.aa42b4a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3218.758a794.js
+-rw-r--r--   0 runner    (1001) docker     (127)       99 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3218.758a794.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3230.2c849ff.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3245.c48f805.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9703 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3322.428e385.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3336.3d4780f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3370.b5d78cd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3420.418f467.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3449.4a13bea.js
+-rw-r--r--   0 runner    (1001) docker     (127)    39449 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3488.9d14a3e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22236 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/35.26a4324.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3501.a0b897f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3562.77d1e3d.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20774 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3604.9c8b7b0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3694.3437882.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3700.ab2c843.js
+-rw-r--r--   0 runner    (1001) docker     (127)      170 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3752.8735345.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3797.2bb532c.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15060 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/383.0385e5e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    31562 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3864.acf045c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/3992.5a17c7b.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10989 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4002.d2530f2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/403.ea946dc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4030.8963386.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22224 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4035.88e3670.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4038.bb0e593.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4039.2635132.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12480 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4105.05362d2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4148.0cb7e6d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/431.f294aa7.js
+-rw-r--r--   0 runner    (1001) docker     (127)    62818 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4324.992bd2c.js
+-rw-r--r--   0 runner    (1001) docker     (127)   205182 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4333.fdaab90.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4387.f2b950d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4434.547c185.js
+-rw-r--r--   0 runner    (1001) docker     (127)    65652 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4478.8778446.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4498.fced3e4.js
+-rw-r--r--   0 runner    (1001) docker     (127)    73801 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4499.7b7aa96.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4521.c2278f6.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12658 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4588.66d005c.js
+-rw-r--r--   0 runner    (1001) docker     (127)   232363 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4630.32049fe.js
+-rw-r--r--   0 runner    (1001) docker     (127)      366 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4630.32049fe.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4670.72adecb.js
+-rw-r--r--   0 runner    (1001) docker     (127)    58986 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4780.f7ebd53.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4810.fdb4bef.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9509 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4825.0f290ff.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4843.96ed13d.js
+-rw-r--r--   0 runner    (1001) docker     (127)   189502 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4926.3619db2.js
+-rw-r--r--   0 runner    (1001) docker     (127)      160 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4926.3619db2.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4954.ac85606.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4965.9c0bd12.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/4971.ba52a81.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/500.b866efa.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5008.7707efe.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13539 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5013.5ff10dd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    27124 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5019.fe7898c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      488 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5051.baecc00.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5061.d662bbf.js
+-rw-r--r--   0 runner    (1001) docker     (127)    55045 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5115.c11e8fa.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6292 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/514.1c1b052.js
+-rw-r--r--   0 runner    (1001) docker     (127)      864 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5233.96f1668.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5249.847f856.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22174 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5261.2a76287.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17171 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5276.069ed0f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5299.4fe47ed.js
+-rw-r--r--   0 runner    (1001) docker     (127)    25735 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5343.c65eb48.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5425.ff5465e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17359 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5464.7c73ae4.js
+-rw-r--r--   0 runner    (1001) docker     (127)       55 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5464.7c73ae4.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5494.db2521b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5597.2470f52.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/563.7fd8ced.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5691.16de5f4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5698.7febbe1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16498 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5765.72d36d2.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16498 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5777.c1c07e5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5822.7e14b54.js
+-rw-r--r--   0 runner    (1001) docker     (127)    25560 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5828.e1ab6ce.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5834.ba430d2.js
+-rw-r--r--   0 runner    (1001) docker     (127)    77942 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5850.9fd6e53.js
+-rw-r--r--   0 runner    (1001) docker     (127)      857 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5945.4a06217.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5972.aa32cae.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/5996.8503bba.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/6139.0c4aaeb.js
+-rw-r--r--   0 runner    (1001) docker     (127)   122842 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/6236.5f93bea.js
+-rw-r--r--   0 runner    (1001) docker     (127)       95 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/6236.5f93bea.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    40991 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/6271.c4952fd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11869 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/6281.f763d40.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/632.200fdf3.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/6417.bebf125.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11489 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/6433.a6cfc6e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    77133 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/644.0a629ee.js
+-rw-r--r--   0 runner    (1001) docker     (127)      212 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/644.0a629ee.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/647.8cecbd3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/6473.a97af61.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/653.7dd3d36.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/6553.a73f98d.js
+-rw-r--r--   0 runner    (1001) docker     (127)   243122 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/6607.4ee069b.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16747 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/661.477cacc.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10601 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/6640.bf24711.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13477 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/6667.60cb1d2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/67.3672096.js
+-rw-r--r--   0 runner    (1001) docker     (127)    25966 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/6739.d19f4c2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/677.493cb60.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/6788.4fb5bb9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/69.fc53c91.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/6941.7241556.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/6942.bcc3a2f.js
+-rw-r--r--   0 runner    (1001) docker     (127)    71168 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/6972.930242c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7005.de1d9f9.js
+-rw-r--r--   0 runner    (1001) docker     (127)    37281 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7010.979a827.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7022.6d0ffc3.js
+-rw-r--r--   0 runner    (1001) docker     (127)      488 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7036.d0dae7d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7054.de34848.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7061.30f7cf6.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24171 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7097.d4214d0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7125.4a0562f.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10601 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7153.135087f.js
+-rw-r--r--   0 runner    (1001) docker     (127)    79078 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7154.804d332.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7170.7bba13a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9092 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7179.af46233.js
+-rw-r--r--   0 runner    (1001) docker     (127)    50998 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7259.6d595ca.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7264.0ec5936.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7360.7b1e065.js
+-rw-r--r--   0 runner    (1001) docker     (127)   210697 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7369.a12e276.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7378.b4f5497.js
+-rw-r--r--   0 runner    (1001) docker     (127)      237 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7378.b4f5497.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    68002 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7427.368a8bc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/745.83ff9e4.js
+-rw-r--r--   0 runner    (1001) docker     (127)    26652 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7450.d5ee0a9.js
+-rw-r--r--   0 runner    (1001) docker     (127)    38991 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7471.30d9d48.js
+-rw-r--r--   0 runner    (1001) docker     (127)    28319 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7495.3c478a0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7534.a755d75.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13033 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/755.6424780.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18136 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7557.bd5cd49.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15293 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7582.7350cc5.js
+-rw-r--r--   0 runner    (1001) docker     (127)      232 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7634.7befbe5.js
+-rw-r--r--   0 runner    (1001) docker     (127)   101829 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7674.93d7410.js
+-rw-r--r--   0 runner    (1001) docker     (127)      849 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7803.45d27da.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11315 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7811.bd10193.js
+-rw-r--r--   0 runner    (1001) docker     (127)      249 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7811.bd10193.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7817.6a39acf.js
+-rw-r--r--   0 runner    (1001) docker     (127)    28662 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7866.e7f89f6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7892.c46785d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7918.506a625.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14437 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/792.f22b43b.js
+-rw-r--r--   0 runner    (1001) docker     (127)    60194 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7969.f8f9146.js
+-rw-r--r--   0 runner    (1001) docker     (127)    62260 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7995.e40b57d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      240 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7995.e40b57d.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26076 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/7997.46ee9b7.js
+-rw-r--r--   0 runner    (1001) docker     (127)    95179 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8010.dbb2b65.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12379 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8103.25c6881.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14035 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8178.6647b58.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15318 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8285.46eba3a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7917 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8378.d951634.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8381.4b39fc5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8387.c2a5ccb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8427.379d337.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8433.c26711e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    31538 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8443.32841be.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8446.d952b7d.js
+-rw-r--r--   0 runner    (1001) docker     (127)    37231 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8479.7ad07d9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/85.eb26499.js
+-rw-r--r--   0 runner    (1001) docker     (127)    31624 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/850.16f7c82.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8579.7c15dcd.js
+-rw-r--r--   0 runner    (1001) docker     (127)      232 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8701.9ba3e4c.js
+-rw-r--r--   0 runner    (1001) docker     (127)    37514 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8734.0965980.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8576 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8768.cd685a6.js
+-rw-r--r--   0 runner    (1001) docker     (127)      857 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8800.5b7449b.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17638 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8801.7946caf.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8107 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/883.7552b75.js
+-rw-r--r--   0 runner    (1001) docker     (127)   197120 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8845.3412b3f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8845.3412b3f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12870 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8927.b773418.js
+-rw-r--r--   0 runner    (1001) docker     (127)   122785 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8929.0b66a95.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8937.6c8605f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8979.2760112.js
+-rw-r--r--   0 runner    (1001) docker     (127)      949 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/8983.5db65ea.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/899.dd8da16.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9022.85c8176.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9037.6397c79.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10341 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/906.f6a46ca.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9060.9fe49c6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9073.fadf4d8.js
+-rw-r--r--   0 runner    (1001) docker     (127)      492 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9116.656701b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9166.d072a52.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9208.10ca99e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9233.b14ca62.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9234.488a70b.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22474 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9239.13871ef.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9244.a95e8aa.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11877 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9250.43c7d24.js
+-rw-r--r--   0 runner    (1001) docker     (127)    29186 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/927.399dde7.js
+-rw-r--r--   0 runner    (1001) docker     (127)      163 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/927.399dde7.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9282.eb25fa6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9331.415f707.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24754 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9334.9101b2f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9372.65a2507.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22275 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9425.d103ed5.js
+-rw-r--r--   0 runner    (1001) docker     (127)      232 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9531.5517c40.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9558.09c3851.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13560 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9565.66944bd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12802 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9597.9d6c989.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9604.c2c5590.js
+-rw-r--r--   0 runner    (1001) docker     (127)    82415 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9643.4b4e30e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9676.f7b737a.js
+-rw-r--r--   0 runner    (1001) docker     (127)    41456 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9799.ecf3e29.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9847.20223dd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35515 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9866.ea3fe7f.js
+-rw-r--r--   0 runner    (1001) docker     (127)    36793 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9879.951cc05.js
+-rw-r--r--   0 runner    (1001) docker     (127)   246342 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/9903.633a36a.js
+-rw-r--r--   0 runner    (1001) docker     (127)    40808 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_AMS-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Calligraphic-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     9600 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Calligraphic-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    22340 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Fraktur-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    21480 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Fraktur-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    34464 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Main-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    20832 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Main-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    34160 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Main-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19776 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Math-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19360 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Math-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    15944 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_SansSerif-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    14628 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_SansSerif-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_SansSerif-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    11852 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Script-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Size1-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Size2-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Size3-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Size4-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    17604 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Typewriter-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Vector-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Vector-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Zero.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   134294 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   747927 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   133988 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    89988 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    76736 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    34034 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   144714 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    33736 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16276 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13224 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   203030 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   918991 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   202744 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   101648 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    78268 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)  2437261 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/jlab_core.b96c356.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.782850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/lab/
+-rw-r--r--   0 runner    (1001) docker     (127)    63254 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/lab/bundle.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.782850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.690849 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.782850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/menus.json
+-rw-r--r--   0 runner    (1001) docker     (127)      473 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/pages.json
+-rw-r--r--   0 runner    (1001) docker     (127)      864 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/shell.json
+-rw-r--r--   0 runner    (1001) docker     (127)      223 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/title.json
+-rw-r--r--   0 runner    (1001) docker     (127)      832 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/top.json
+-rw-r--r--   0 runner    (1001) docker     (127)      386 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/zen.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.782850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/help-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/help-extension/open.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.786850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/checkpoints.json
+-rw-r--r--   0 runner    (1001) docker     (127)      560 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/edit-notebook-metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      237 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/kernel-logo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      517 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/scroll-output.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.786850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/file-actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/widget.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.694849 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.786850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      543 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/property-inspector.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/top-bar.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.786850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/notification.json
+-rw-r--r--   0 runner    (1001) docker     (127)      936 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json
+-rw-r--r--   0 runner    (1001) docker     (127)      563 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json
+-rw-r--r--   0 runner    (1001) docker     (127)      677 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/sanitizer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      694 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/utilityCommands.json
+-rw-r--r--   0 runner    (1001) docker     (127)      457 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/workspaces.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.786850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.786850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/celltags-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/celltags-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.786850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.786850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/inline-completer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/manager.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.786850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/completer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      365 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/foreign.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.786850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.786850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/download.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.786850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.790850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json
+-rw-r--r--   0 runner    (1001) docker     (127)      513 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json
+-rw-r--r--   0 runner    (1001) docker     (127)      385 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
+-rw-r--r--   0 runner    (1001) docker     (127)      477 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-with.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.790850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/completer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.790850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/help-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/help-extension/about.json
+-rw-r--r--   0 runner    (1001) docker     (127)      456 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/help-extension/jupyter-forum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      364 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/help-extension/launch-classic.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.790850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.790850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.790850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (127)      782 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json
+-rw-r--r--   0 runner    (1001) docker     (127)      319 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.790850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.790850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.790850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/lsp-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/lsp-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.790850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)    10058 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.790850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.790850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/mathjax-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/mathjax-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.790850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/metadataform-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/metadataform-extension/metadataforms.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.790850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/completer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      672 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tools.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24926 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.790850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/running-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/running-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.790850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/form-ui.json
+-rw-r--r--   0 runner    (1001) docker     (127)      440 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.790850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.794850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.794850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/toc-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/toc-extension/registry.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.794850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (127)      402 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/files.json
+-rw-r--r--   0 runner    (1001) docker     (127)      572 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.794850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/translation-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.694849 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.794850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlite/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlite/application-extension/share-file.json
+-rw-r--r--   0 runner    (1001) docker     (127)   105099 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-26 23:42:36.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/all_federated.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.694849 fixinventorycore-4.0.5/fixcore/jupyterlite/build/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.694849 fixinventorycore-4.0.5/fixcore/jupyterlite/build/themes/@jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.794850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)    17882 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.794850 fixinventorycore-4.0.5/fixcore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)    16550 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   415751 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/build/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/config-utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.694849 fixinventorycore-4.0.5/fixcore/jupyterlite/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.794850 fixinventorycore-4.0.5/fixcore/jupyterlite/doc/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/doc/tree/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.794850 fixinventorycore-4.0.5/fixcore/jupyterlite/doc/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/doc/workspaces/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.698849 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.698849 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.794850 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/
+-rw-rw-rw-   0 runner    (1001) docker     (127)      219 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/install.json
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2343 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.794850 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/
+-rw-rw-rw-   0 runner    (1001) docker     (127)     6950 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/312.749011b8237164f040ce.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)       88 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/312.749011b8237164f040ce.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (127)    14992 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/584.7e49152bd31ca0f8291b.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)       88 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/584.7e49152bd31ca0f8291b.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (127)    16598 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/5e8d6f34d83488f083fd.png
+-rw-rw-rw-   0 runner    (1001) docker     (127)     6950 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/692.c1aeb4d97f766d3b4515.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)       88 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/692.c1aeb4d97f766d3b4515.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (127)      598 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/804.fb6a8eda889cf61eea27.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)     4254 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/b1c098fa349a030dacbe.png
+-rw-rw-rw-   0 runner    (1001) docker     (127)     7359 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.6014628263d9ee9ca44a.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)      118 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)    13107 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.794850 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2732 2024-04-26 23:42:23.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.802850 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2643 2024-04-26 23:42:23.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/133.7957020c5e8bc5703dbc.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)     8311 2024-04-26 23:42:23.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/423.d0d3e2912c33c7566484.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)  3598363 2024-04-26 23:42:23.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/478.b48f45da3d88616ad3f9.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1110 2024-04-26 23:42:23.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/478.b48f45da3d88616ad3f9.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (127)    70520 2024-04-26 23:42:23.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)      336 2024-04-26 23:42:23.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2360 2024-04-26 23:42:23.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/657.15db1deb504caf7dbc6d.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)    14766 2024-04-26 23:42:23.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/855.323c80e7298812d692e7.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)     7706 2024-04-26 23:42:23.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.70a4f7e7a0383740860d.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)      118 2024-04-26 23:42:23.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)     5802 2024-04-26 23:42:23.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.802850 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab_pygments/
+-rw-rw-rw-   0 runner    (1001) docker     (127)      199 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab_pygments/install.json
+-rw-rw-rw-   0 runner    (1001) docker     (127)     5919 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab_pygments/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.802850 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/
+-rw-rw-rw-   0 runner    (1001) docker     (127)      224 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)     8351 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/747.67662283a5707eeb4d4c.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)     3925 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.5cbb9d2323598fbda535.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)      162 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2452 2024-04-26 23:42:28.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.802850 fixinventorycore-4.0.5/fixcore/jupyterlite/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/files/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20954 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/icon-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/jupyter-lite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-04-26 23:42:36.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/jupyter-lite.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11526 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/jupyterlite.schema.v0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.802850 fixinventorycore-4.0.5/fixcore/jupyterlite/lab/
+-rw-r--r--   0 runner    (1001) docker     (127)   324251 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/lab/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/lab/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/lab/jupyter-lite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      166 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/lab/jupyter-lite.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12425 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/lab/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.802850 fixinventorycore-4.0.5/fixcore/jupyterlite/lab/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/lab/tree/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.806850 fixinventorycore-4.0.5/fixcore/jupyterlite/lab/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/lab/workspaces/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      690 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/manifest.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 1985-10-26 08:15:00.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.698849 fixinventorycore-4.0.5/fixcore/jupyterlite/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.806850 fixinventorycore-4.0.5/fixcore/jupyterlite/static/favicons/
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-26 23:42:31.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/static/favicons/favicon-busy-1.ico
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-26 23:42:31.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/static/favicons/favicon-busy-2.ico
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-26 23:42:31.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/static/favicons/favicon-busy-3.ico
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-26 23:42:31.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/static/favicons/favicon-file.ico
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-26 23:42:31.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/static/favicons/favicon-notebook.ico
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-26 23:42:31.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/static/favicons/favicon-terminal.ico
+-rw-rw-rw-   0 runner    (1001) docker     (127)    32038 2024-04-26 23:42:31.000000 fixinventorycore-4.0.5/fixcore/jupyterlite/static/favicons/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    11967 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.806850 fixinventorycore-4.0.5/fixcore/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/model/adjust_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/model/db_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/model/exportable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30006 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/model/graph_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/model/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69697 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/model/model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/model/resolve_in_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/model/transform_kind_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/model/typed_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.806850 fixinventorycore-4.0.5/fixcore/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51739 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/query/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15449 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/query/query_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/query/template_expander.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/query/template_expander_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.806850 fixinventorycore-4.0.5/fixcore/report/
+-rw-r--r--   0 runner    (1001) docker     (127)    19667 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/report/benchmark_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26776 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/report/inspector_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/report/report_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.810850 fixinventorycore-4.0.5/fixcore/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   141248 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/static/api-doc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/static/ck-unicode-truecolor.ans
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/static/fix.css
+-rw-r--r--   0 runner    (1001) docker     (127)    14617 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/static/fixinventory_logo_and_text.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/system_start.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.810850 fixinventorycore-4.0.5/fixcore/task/
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/task/job_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/task/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/task/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/task/start_workflow_on_first_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/task/subscribers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/task/task_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33482 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/task/task_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30250 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/task/task_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.810850 fixinventorycore-4.0.5/fixcore/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/templates/create_first_user.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/templates/home.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.810850 fixinventorycore-4.0.5/fixcore/user/
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/user/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/user/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15809 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.814850 fixinventorycore-4.0.5/fixcore/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/web/accesslog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80914 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/web/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/web/certificate_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8726 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/web/content_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/web/directives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/web/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/web/tsdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/fixcore/worker_task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.826850 fixinventorycore-4.0.5/fixinventorycore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-26 23:42:38.000000 fixinventorycore-4.0.5/fixinventorycore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30702 2024-04-26 23:42:38.000000 fixinventorycore-4.0.5/fixinventorycore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 23:42:38.000000 fixinventorycore-4.0.5/fixinventorycore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-26 23:42:38.000000 fixinventorycore-4.0.5/fixinventorycore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 23:42:38.000000 fixinventorycore-4.0.5/fixinventorycore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-26 23:42:38.000000 fixinventorycore-4.0.5/fixinventorycore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 23:42:38.000000 fixinventorycore-4.0.5/fixinventorycore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-26 23:42:38.826850 fixinventorycore-4.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.814850 fixinventorycore-4.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.814850 fixinventorycore-4.0.5/tests/fixcore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.814850 fixinventorycore-4.0.5/tests/fixcore/analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/analytics/posthog_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/analytics/recurrent_events_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.818850 fixinventorycore-4.0.5/tests/fixcore/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/cli/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65515 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/cli/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/cli/model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.818850 fixinventorycore-4.0.5/tests/fixcore/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/config/config_handler_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/config/config_override_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/config/core_config_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31093 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/console_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/core_config_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.818850 fixinventorycore-4.0.5/tests/fixcore/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19729 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/db/arango_query_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/db/arangodb_functions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/db/async_arangodb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/db/configdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/db/db_access_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/db/deferredouteredgedb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/db/entitydb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41807 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/db/graphdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/db/jobdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/db/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/db/modeldb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/db/reportdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/db/runningtaskdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/db/system_data_db_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/db/templatedb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/db/timeseriesdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/dependencies_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.818850 fixinventorycore-4.0.5/tests/fixcore/graph_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/graph_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/graph_manager/graph_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/hypothesis_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.822850 fixinventorycore-4.0.5/tests/fixcore/infra_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/infra_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/infra_apps/local_runtime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/infra_apps/package_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/message_bus_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.822850 fixinventorycore-4.0.5/tests/fixcore/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/model/adjust_node_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/model/db_updater_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/model/exportable_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16753 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/model/graph_access_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/model/json_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/model/model_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28507 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/model/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/model/resolve_in_graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/model/typed_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.822850 fixinventorycore-4.0.5/tests/fixcore/query/
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/query/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18737 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/query/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/query/template_expander_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.822850 fixinventorycore-4.0.5/tests/fixcore/report/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/report/benchmark_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/report/inspector_service_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.822850 fixinventorycore-4.0.5/tests/fixcore/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/task/job_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/task/start_workflow_on_first_subscriber_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/task/subscribers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11073 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/task/task_description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/task/task_handler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.822850 fixinventorycore-4.0.5/tests/fixcore/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/user/user_management_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/util_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/validator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 23:42:38.826850 fixinventorycore-4.0.5/tests/fixcore/web/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15974 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/web/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24351 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/web/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/web/auth_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/web/certificate_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/web/content_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/web/permission_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-26 23:39:00.000000 fixinventorycore-4.0.5/tests/fixcore/worker_task_queue_test.py
```

### Comparing `fixinventorycore-4.0.4/PKG-INFO` & `fixinventorycore-4.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventorycore
-Version: 4.0.4
+Version: 4.0.5
 Summary: Keeps all the things.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Homepage, https://inventory.fix.security
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `fixinventorycore-4.0.4/README.md` & `fixinventorycore-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/__main__.py` & `fixinventorycore-4.0.5/fixcore/__main__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/action_handlers/merge_outer_edge_handler.py` & `fixinventorycore-4.0.5/fixcore/action_handlers/merge_outer_edge_handler.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/analytics/__init__.py` & `fixinventorycore-4.0.5/fixcore/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/analytics/posthog.py` & `fixinventorycore-4.0.5/fixcore/analytics/posthog.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/analytics/recurrent_events.py` & `fixinventorycore-4.0.5/fixcore/analytics/recurrent_events.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/async_extensions.py` & `fixinventorycore-4.0.5/fixcore/async_extensions.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/cli/__init__.py` & `fixinventorycore-4.0.5/fixcore/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/cli/cli.py` & `fixinventorycore-4.0.5/fixcore/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/cli/command.py` & `fixinventorycore-4.0.5/fixcore/cli/command.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/cli/model.py` & `fixinventorycore-4.0.5/fixcore/cli/model.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/cli/tip_of_the_day.py` & `fixinventorycore-4.0.5/fixcore/cli/tip_of_the_day.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/config/__init__.py` & `fixinventorycore-4.0.5/fixcore/config/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/config/config_handler_service.py` & `fixinventorycore-4.0.5/fixcore/config/config_handler_service.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/config/config_override_service.py` & `fixinventorycore-4.0.5/fixcore/config/config_override_service.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/config/core_config_handler.py` & `fixinventorycore-4.0.5/fixcore/config/core_config_handler.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/console_renderer.py` & `fixinventorycore-4.0.5/fixcore/console_renderer.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/constants.py` & `fixinventorycore-4.0.5/fixcore/constants.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/core_config.py` & `fixinventorycore-4.0.5/fixcore/core_config.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/db/__init__.py` & `fixinventorycore-4.0.5/fixcore/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/db/arango_query.py` & `fixinventorycore-4.0.5/fixcore/db/arango_query.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/db/arangodb_extensions.py` & `fixinventorycore-4.0.5/fixcore/db/arangodb_extensions.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/db/arangodb_functions.py` & `fixinventorycore-4.0.5/fixcore/db/arangodb_functions.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/db/async_arangodb.py` & `fixinventorycore-4.0.5/fixcore/db/async_arangodb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/db/configdb.py` & `fixinventorycore-4.0.5/fixcore/db/configdb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/db/db_access.py` & `fixinventorycore-4.0.5/fixcore/db/db_access.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/db/deferredouteredgedb.py` & `fixinventorycore-4.0.5/fixcore/db/deferredouteredgedb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/db/entitydb.py` & `fixinventorycore-4.0.5/fixcore/db/entitydb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/db/graphdb.py` & `fixinventorycore-4.0.5/fixcore/db/graphdb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/db/model.py` & `fixinventorycore-4.0.5/fixcore/db/model.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/db/packagedb.py` & `fixinventorycore-4.0.5/fixcore/db/packagedb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/db/reportdb.py` & `fixinventorycore-4.0.5/fixcore/db/reportdb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/db/runningtaskdb.py` & `fixinventorycore-4.0.5/fixcore/db/runningtaskdb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/db/system_data_db.py` & `fixinventorycore-4.0.5/fixcore/db/system_data_db.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/db/timeseriesdb.py` & `fixinventorycore-4.0.5/fixcore/db/timeseriesdb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/db/usagedb.py` & `fixinventorycore-4.0.5/fixcore/db/usagedb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/dependencies.py` & `fixinventorycore-4.0.5/fixcore/dependencies.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/error.py` & `fixinventorycore-4.0.5/fixcore/error.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/graph_manager/graph_manager.py` & `fixinventorycore-4.0.5/fixcore/graph_manager/graph_manager.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/ids.py` & `fixinventorycore-4.0.5/fixcore/ids.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/infra_apps/local_runtime.py` & `fixinventorycore-4.0.5/fixcore/infra_apps/local_runtime.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/infra_apps/manifest.py` & `fixinventorycore-4.0.5/fixcore/infra_apps/manifest.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/infra_apps/package_manager.py` & `fixinventorycore-4.0.5/fixcore/infra_apps/package_manager.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/infra_apps/runtime.py` & `fixinventorycore-4.0.5/fixcore/infra_apps/runtime.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/bootstrap.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/bootstrap.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1053.7a56130.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1053.7a56130.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1088.33c6076.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1088.33c6076.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1091.1cf35e6.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1091.1cf35e6.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1122.d86c258.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1122.d86c258.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/114.1c04540.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/114.1c04540.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1169.4cf2d13.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1169.4cf2d13.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/125.4c6ac03.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/125.4c6ac03.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1261.3da9a56.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1261.3da9a56.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/131.5b6a7ab.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/131.5b6a7ab.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1385.707019c.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1385.707019c.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1388.0f22ef8.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1388.0f22ef8.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1418.d9431d8.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1418.d9431d8.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/142.6e89fb8.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/142.6e89fb8.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1495.671bdd4.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1495.671bdd4.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1542.22098a5.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1542.22098a5.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1558.548303d.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1558.548303d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1584.d919fce.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1584.d919fce.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1618.983fc32.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1618.983fc32.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1715.ebbb93b.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1715.ebbb93b.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1769.10c2b5d.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1769.10c2b5d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1815.2af66e5.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1815.2af66e5.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1837.622ebbe.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1837.622ebbe.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1846.ed084ce.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1846.ed084ce.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1869.86f5778.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1869.86f5778.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1871.7fed383.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1871.7fed383.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/1941.79180b2.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/1941.79180b2.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2065.410c3bc.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2065.410c3bc.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/214.300dbf1.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/214.300dbf1.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2188.9676797.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2188.9676797.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/221.59c0059.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/221.59c0059.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2213.b58cab4.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2213.b58cab4.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2241.91c6cce.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2241.91c6cce.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2323.7e4d795.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2323.7e4d795.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2324.aff3939.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2324.aff3939.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2343.3cf0fe8.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2343.3cf0fe8.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2349.9acb0b1.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2349.9acb0b1.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2363.6aa6a7f.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2363.6aa6a7f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2386.5f8e2da.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2386.5f8e2da.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2520.5c65366.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2520.5c65366.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2552.6c5224e.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2552.6c5224e.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/261.431b309.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/261.431b309.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2622.3d61d64.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2622.3d61d64.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2666.6cce729.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2666.6cce729.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2682.0c612a1.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2682.0c612a1.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2692.f2b8d53.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2692.f2b8d53.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/270.9675bfe.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/270.9675bfe.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2702.0e1a6ff.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2702.0e1a6ff.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/28.9f8dd00.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/28.9f8dd00.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2871.e1a64a6.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2871.e1a64a6.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2913.25c5e72.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2913.25c5e72.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2913.25c5e72.js.LICENSE.txt` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2913.25c5e72.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2930.896decd.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2930.896decd.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/2955.c8d0773.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/2955.c8d0773.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/306.b568c30.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/306.b568c30.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3079.18e3c32.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3079.18e3c32.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/311.76f79fc.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/311.76f79fc.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3111.8de2d0a.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3111.8de2d0a.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3154.5d8f80d.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3154.5d8f80d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3211.aa42b4a.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3211.aa42b4a.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3218.758a794.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3218.758a794.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3230.2c849ff.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3230.2c849ff.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3245.c48f805.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3245.c48f805.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3322.428e385.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3322.428e385.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3336.3d4780f.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3336.3d4780f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3370.b5d78cd.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3370.b5d78cd.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3420.418f467.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3420.418f467.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3449.4a13bea.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3449.4a13bea.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3488.9d14a3e.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3488.9d14a3e.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/35.26a4324.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/35.26a4324.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3501.a0b897f.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3501.a0b897f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3562.77d1e3d.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3562.77d1e3d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3604.9c8b7b0.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3604.9c8b7b0.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3694.3437882.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3694.3437882.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3700.ab2c843.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3700.ab2c843.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3797.2bb532c.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3797.2bb532c.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/383.0385e5e.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/383.0385e5e.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3864.acf045c.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3864.acf045c.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/3992.5a17c7b.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/3992.5a17c7b.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4002.d2530f2.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4002.d2530f2.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/403.ea946dc.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/403.ea946dc.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4030.8963386.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4030.8963386.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4035.88e3670.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4035.88e3670.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4038.bb0e593.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4038.bb0e593.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4039.2635132.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4039.2635132.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4105.05362d2.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4105.05362d2.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4148.0cb7e6d.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4148.0cb7e6d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/431.f294aa7.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/431.f294aa7.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4324.992bd2c.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4324.992bd2c.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4333.fdaab90.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4333.fdaab90.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4387.f2b950d.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4387.f2b950d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4434.547c185.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4434.547c185.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4478.8778446.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4478.8778446.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4498.fced3e4.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4498.fced3e4.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4499.7b7aa96.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4499.7b7aa96.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4521.c2278f6.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4521.c2278f6.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4588.66d005c.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4588.66d005c.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4630.32049fe.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4630.32049fe.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4670.72adecb.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4670.72adecb.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4780.f7ebd53.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4780.f7ebd53.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4810.fdb4bef.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4810.fdb4bef.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4825.0f290ff.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4825.0f290ff.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4843.96ed13d.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4843.96ed13d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4926.3619db2.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4926.3619db2.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4954.ac85606.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4954.ac85606.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4965.9c0bd12.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4965.9c0bd12.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/4971.ba52a81.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/4971.ba52a81.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/500.b866efa.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/500.b866efa.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5008.7707efe.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5008.7707efe.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5013.5ff10dd.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5013.5ff10dd.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5019.fe7898c.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5019.fe7898c.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5061.d662bbf.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5061.d662bbf.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5115.c11e8fa.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5115.c11e8fa.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/514.1c1b052.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/514.1c1b052.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5233.96f1668.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5233.96f1668.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5249.847f856.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5249.847f856.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5261.2a76287.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5261.2a76287.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5276.069ed0f.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5276.069ed0f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5299.4fe47ed.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5299.4fe47ed.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5343.c65eb48.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5343.c65eb48.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5425.ff5465e.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5425.ff5465e.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5464.7c73ae4.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5464.7c73ae4.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5494.db2521b.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5494.db2521b.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5597.2470f52.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5597.2470f52.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/563.7fd8ced.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/563.7fd8ced.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5691.16de5f4.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5691.16de5f4.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5698.7febbe1.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5698.7febbe1.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5765.72d36d2.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5765.72d36d2.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5777.c1c07e5.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5777.c1c07e5.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5822.7e14b54.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5822.7e14b54.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5828.e1ab6ce.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5828.e1ab6ce.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5834.ba430d2.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5834.ba430d2.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5850.9fd6e53.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5850.9fd6e53.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5945.4a06217.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5945.4a06217.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5972.aa32cae.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5972.aa32cae.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/5996.8503bba.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/5996.8503bba.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/6139.0c4aaeb.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/6139.0c4aaeb.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/6236.5f93bea.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/6236.5f93bea.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/6271.c4952fd.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/6271.c4952fd.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/6281.f763d40.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/6281.f763d40.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/632.200fdf3.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/632.200fdf3.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/6417.bebf125.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/6417.bebf125.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/6433.a6cfc6e.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/6433.a6cfc6e.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/644.0a629ee.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/644.0a629ee.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/647.8cecbd3.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/647.8cecbd3.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/6473.a97af61.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/6473.a97af61.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/653.7dd3d36.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/653.7dd3d36.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/6553.a73f98d.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/6553.a73f98d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/6607.4ee069b.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/6607.4ee069b.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/661.477cacc.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/661.477cacc.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/6640.bf24711.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/6640.bf24711.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/6667.60cb1d2.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/6667.60cb1d2.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/67.3672096.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/67.3672096.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/6739.d19f4c2.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/6739.d19f4c2.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/677.493cb60.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/677.493cb60.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/6788.4fb5bb9.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/6788.4fb5bb9.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/69.fc53c91.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/69.fc53c91.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/6941.7241556.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/6941.7241556.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/6942.bcc3a2f.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/6942.bcc3a2f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/6972.930242c.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/6972.930242c.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7005.de1d9f9.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7005.de1d9f9.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7010.979a827.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7010.979a827.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7022.6d0ffc3.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7022.6d0ffc3.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7054.de34848.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7054.de34848.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7061.30f7cf6.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7061.30f7cf6.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7097.d4214d0.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7097.d4214d0.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7125.4a0562f.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7125.4a0562f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7153.135087f.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7153.135087f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7154.804d332.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7154.804d332.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7170.7bba13a.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7170.7bba13a.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7179.af46233.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7179.af46233.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7259.6d595ca.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7259.6d595ca.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7264.0ec5936.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7264.0ec5936.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7360.7b1e065.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7360.7b1e065.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7369.a12e276.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7369.a12e276.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7378.b4f5497.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7378.b4f5497.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7427.368a8bc.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7427.368a8bc.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/745.83ff9e4.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/745.83ff9e4.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7450.d5ee0a9.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7450.d5ee0a9.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7471.30d9d48.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7471.30d9d48.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7495.3c478a0.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7495.3c478a0.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7534.a755d75.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7534.a755d75.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/755.6424780.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/755.6424780.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7557.bd5cd49.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7557.bd5cd49.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7582.7350cc5.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7582.7350cc5.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7674.93d7410.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7674.93d7410.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7803.45d27da.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7803.45d27da.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7811.bd10193.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7811.bd10193.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7817.6a39acf.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7817.6a39acf.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7866.e7f89f6.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7866.e7f89f6.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7892.c46785d.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7892.c46785d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7918.506a625.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7918.506a625.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/792.f22b43b.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/792.f22b43b.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7969.f8f9146.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7969.f8f9146.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7995.e40b57d.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7995.e40b57d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/7997.46ee9b7.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/7997.46ee9b7.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8010.dbb2b65.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8010.dbb2b65.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8103.25c6881.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8103.25c6881.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8178.6647b58.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8178.6647b58.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8285.46eba3a.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8285.46eba3a.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8378.d951634.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8378.d951634.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8381.4b39fc5.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8381.4b39fc5.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8387.c2a5ccb.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8387.c2a5ccb.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8427.379d337.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8427.379d337.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8433.c26711e.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8433.c26711e.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8443.32841be.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8443.32841be.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8446.d952b7d.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8446.d952b7d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8479.7ad07d9.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8479.7ad07d9.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/85.eb26499.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/85.eb26499.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/850.16f7c82.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/850.16f7c82.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8579.7c15dcd.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8579.7c15dcd.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8734.0965980.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8734.0965980.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8768.cd685a6.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8768.cd685a6.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8800.5b7449b.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8800.5b7449b.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8801.7946caf.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8801.7946caf.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/883.7552b75.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/883.7552b75.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8845.3412b3f.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8845.3412b3f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8845.3412b3f.js.LICENSE.txt` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8845.3412b3f.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8927.b773418.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8927.b773418.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8929.0b66a95.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8929.0b66a95.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8937.6c8605f.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8937.6c8605f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8979.2760112.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8979.2760112.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/8983.5db65ea.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/8983.5db65ea.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/899.dd8da16.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/899.dd8da16.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9022.85c8176.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9022.85c8176.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9037.6397c79.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9037.6397c79.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/906.f6a46ca.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/906.f6a46ca.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9060.9fe49c6.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9060.9fe49c6.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9073.fadf4d8.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9073.fadf4d8.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9166.d072a52.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9166.d072a52.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9208.10ca99e.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9208.10ca99e.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9233.b14ca62.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9233.b14ca62.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9234.488a70b.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9234.488a70b.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9239.13871ef.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9239.13871ef.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9244.a95e8aa.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9244.a95e8aa.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9250.43c7d24.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9250.43c7d24.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/927.399dde7.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/927.399dde7.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9282.eb25fa6.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9282.eb25fa6.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9331.415f707.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9331.415f707.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9334.9101b2f.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9334.9101b2f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9372.65a2507.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9372.65a2507.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9425.d103ed5.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9425.d103ed5.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9558.09c3851.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9558.09c3851.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9565.66944bd.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9565.66944bd.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9597.9d6c989.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9597.9d6c989.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9604.c2c5590.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9604.c2c5590.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9643.4b4e30e.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9643.4b4e30e.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9676.f7b737a.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9676.f7b737a.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9799.ecf3e29.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9799.ecf3e29.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9847.20223dd.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9847.20223dd.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9866.ea3fe7f.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9866.ea3fe7f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9879.951cc05.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9879.951cc05.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/9903.633a36a.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/9903.633a36a.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_AMS-Regular.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_AMS-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Calligraphic-Bold.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Calligraphic-Bold.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Calligraphic-Regular.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Calligraphic-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Fraktur-Bold.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Fraktur-Bold.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Fraktur-Regular.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Fraktur-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Main-Bold.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Main-Bold.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Main-Italic.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Main-Italic.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Main-Regular.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Main-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Math-BoldItalic.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Math-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Math-Italic.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Math-Italic.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_SansSerif-Bold.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_SansSerif-Bold.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_SansSerif-Italic.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_SansSerif-Italic.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_SansSerif-Regular.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_SansSerif-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Script-Regular.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Script-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Size1-Regular.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Size1-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Size2-Regular.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Size2-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Size3-Regular.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Size3-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Size4-Regular.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Size4-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Typewriter-Regular.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Typewriter-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Vector-Bold.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Vector-Bold.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Vector-Regular.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Vector-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/MathJax_Zero.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/MathJax_Zero.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-brands-400.eot` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-brands-400.svg` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-brands-400.ttf` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-brands-400.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-brands-400.woff2` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-regular-400.eot` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-regular-400.svg` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-regular-400.ttf` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-regular-400.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-regular-400.woff2` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-solid-900.eot` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-solid-900.svg` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-solid-900.ttf` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-solid-900.woff` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/fa-solid-900.woff2` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/jlab_core.b96c356.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/jlab_core.b96c356.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/lab/bundle.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/lab/bundle.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/menus.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/menus.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/shell.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/shell.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/top.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/top.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/edit-notebook-metadata.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/edit-notebook-metadata.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/scroll-output.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/scroll-output.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/file-actions.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/file-actions.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/widget.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/widget.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/property-inspector.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/property-inspector.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/top-bar.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/top-bar.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/notification.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/notification.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/sanitizer.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/sanitizer.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/utilityCommands.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/utilityCommands.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/celltags-extension/plugin.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/celltags-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/inline-completer.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/inline-completer.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/manager.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/manager.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/lsp-extension/plugin.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/lsp-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/mathjax-extension/plugin.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/mathjax-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/metadataform-extension/metadataforms.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/metadataform-extension/metadataforms.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tools.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tools.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/running-extension/plugin.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/running-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/toc-extension/registry.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/toc-extension/registry.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/schemas/all.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/schemas/all.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/service-worker.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/build/third-party-licenses.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/build/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/config-utils.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/config-utils.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/312.749011b8237164f040ce.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/312.749011b8237164f040ce.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/584.7e49152bd31ca0f8291b.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/584.7e49152bd31ca0f8291b.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/5e8d6f34d83488f083fd.png` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/5e8d6f34d83488f083fd.png`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/692.c1aeb4d97f766d3b4515.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/692.c1aeb4d97f766d3b4515.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/804.fb6a8eda889cf61eea27.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/804.fb6a8eda889cf61eea27.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/b1c098fa349a030dacbe.png` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/b1c098fa349a030dacbe.png`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.6014628263d9ee9ca44a.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.6014628263d9ee9ca44a.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/package.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/package.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/133.7957020c5e8bc5703dbc.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/133.7957020c5e8bc5703dbc.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/423.d0d3e2912c33c7566484.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/423.d0d3e2912c33c7566484.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/478.b48f45da3d88616ad3f9.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/478.b48f45da3d88616ad3f9.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/478.b48f45da3d88616ad3f9.js.LICENSE.txt` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/478.b48f45da3d88616ad3f9.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/657.15db1deb504caf7dbc6d.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/657.15db1deb504caf7dbc6d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/855.323c80e7298812d692e7.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/855.323c80e7298812d692e7.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.70a4f7e7a0383740860d.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.70a4f7e7a0383740860d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab_pygments/package.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab_pygments/package.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/747.67662283a5707eeb4d4c.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/747.67662283a5707eeb4d4c.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.5cbb9d2323598fbda535.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.5cbb9d2323598fbda535.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/files/example.ipynb` & `fixinventorycore-4.0.5/fixcore/jupyterlite/files/example.ipynb`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/icon-120x120.png` & `fixinventorycore-4.0.5/fixcore/jupyterlite/icon-120x120.png`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/icon-512x512.png` & `fixinventorycore-4.0.5/fixcore/jupyterlite/icon-512x512.png`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/index.html` & `fixinventorycore-4.0.5/fixcore/jupyterlite/index.html`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/jupyter-lite.ipynb` & `fixinventorycore-4.0.5/fixcore/jupyterlite/jupyter-lite.ipynb`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/jupyter-lite.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/jupyter-lite.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/jupyterlite.schema.v0.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/jupyterlite.schema.v0.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/lab/favicon.ico` & `fixinventorycore-4.0.5/fixcore/jupyterlite/lab/favicon.ico`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/lab/index.html` & `fixinventorycore-4.0.5/fixcore/jupyterlite/lab/index.html`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/lab/jupyter-lite.ipynb` & `fixinventorycore-4.0.5/fixcore/jupyterlite/lab/jupyter-lite.ipynb`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/lab/package.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/lab/package.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/manifest.webmanifest` & `fixinventorycore-4.0.5/fixcore/jupyterlite/manifest.webmanifest`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/package.json` & `fixinventorycore-4.0.5/fixcore/jupyterlite/package.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/service-worker.js` & `fixinventorycore-4.0.5/fixcore/jupyterlite/service-worker.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/static/favicons/favicon-busy-1.ico` & `fixinventorycore-4.0.5/fixcore/jupyterlite/static/favicons/favicon-busy-1.ico`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/static/favicons/favicon-busy-2.ico` & `fixinventorycore-4.0.5/fixcore/jupyterlite/static/favicons/favicon-busy-2.ico`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/static/favicons/favicon-busy-3.ico` & `fixinventorycore-4.0.5/fixcore/jupyterlite/static/favicons/favicon-busy-3.ico`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/static/favicons/favicon-file.ico` & `fixinventorycore-4.0.5/fixcore/jupyterlite/static/favicons/favicon-file.ico`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/static/favicons/favicon-notebook.ico` & `fixinventorycore-4.0.5/fixcore/jupyterlite/static/favicons/favicon-notebook.ico`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/static/favicons/favicon-terminal.ico` & `fixinventorycore-4.0.5/fixcore/jupyterlite/static/favicons/favicon-terminal.ico`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/jupyterlite/static/favicons/favicon.ico` & `fixinventorycore-4.0.5/fixcore/jupyterlite/static/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/message_bus.py` & `fixinventorycore-4.0.5/fixcore/message_bus.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/metrics.py` & `fixinventorycore-4.0.5/fixcore/metrics.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/model/adjust_node.py` & `fixinventorycore-4.0.5/fixcore/model/adjust_node.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/model/db_updater.py` & `fixinventorycore-4.0.5/fixcore/model/db_updater.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/model/exportable_model.py` & `fixinventorycore-4.0.5/fixcore/model/exportable_model.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/model/graph_access.py` & `fixinventorycore-4.0.5/fixcore/model/graph_access.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/model/json_schema.py` & `fixinventorycore-4.0.5/fixcore/model/json_schema.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/model/model.py` & `fixinventorycore-4.0.5/fixcore/model/model.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/model/model_handler.py` & `fixinventorycore-4.0.5/fixcore/model/model_handler.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/model/resolve_in_graph.py` & `fixinventorycore-4.0.5/fixcore/model/resolve_in_graph.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/model/transform_kind_convert.py` & `fixinventorycore-4.0.5/fixcore/model/transform_kind_convert.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/model/typed_model.py` & `fixinventorycore-4.0.5/fixcore/model/typed_model.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/query/__init__.py` & `fixinventorycore-4.0.5/fixcore/query/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/query/model.py` & `fixinventorycore-4.0.5/fixcore/query/model.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/query/query_parser.py` & `fixinventorycore-4.0.5/fixcore/query/query_parser.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/query/template_expander.py` & `fixinventorycore-4.0.5/fixcore/query/template_expander.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/query/template_expander_service.py` & `fixinventorycore-4.0.5/fixcore/query/template_expander_service.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/report/__init__.py` & `fixinventorycore-4.0.5/fixcore/report/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/report/benchmark_renderer.py` & `fixinventorycore-4.0.5/fixcore/report/benchmark_renderer.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/report/inspector_service.py` & `fixinventorycore-4.0.5/fixcore/report/inspector_service.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/report/report_config.py` & `fixinventorycore-4.0.5/fixcore/report/report_config.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/static/api-doc.yaml` & `fixinventorycore-4.0.5/fixcore/static/api-doc.yaml`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/static/ck-unicode-truecolor.ans` & `fixinventorycore-4.0.5/fixcore/static/ck-unicode-truecolor.ans`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/static/fixinventory_logo_and_text.svg` & `fixinventorycore-4.0.5/fixcore/static/fixinventory_logo_and_text.svg`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/system_start.py` & `fixinventorycore-4.0.5/fixcore/system_start.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/task/__init__.py` & `fixinventorycore-4.0.5/fixcore/task/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/task/model.py` & `fixinventorycore-4.0.5/fixcore/task/model.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/task/scheduler.py` & `fixinventorycore-4.0.5/fixcore/task/scheduler.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/task/start_workflow_on_first_subscriber.py` & `fixinventorycore-4.0.5/fixcore/task/start_workflow_on_first_subscriber.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/task/subscribers.py` & `fixinventorycore-4.0.5/fixcore/task/subscribers.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/task/task_description.py` & `fixinventorycore-4.0.5/fixcore/task/task_description.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/task/task_handler.py` & `fixinventorycore-4.0.5/fixcore/task/task_handler.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/templates/base.html` & `fixinventorycore-4.0.5/fixcore/templates/base.html`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/templates/create_first_user.html` & `fixinventorycore-4.0.5/fixcore/templates/create_first_user.html`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/templates/home.html` & `fixinventorycore-4.0.5/fixcore/templates/home.html`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/templates/login.html` & `fixinventorycore-4.0.5/fixcore/templates/login.html`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/types.py` & `fixinventorycore-4.0.5/fixcore/types.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/user/__init__.py` & `fixinventorycore-4.0.5/fixcore/user/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/user/model.py` & `fixinventorycore-4.0.5/fixcore/user/model.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/user/user_management.py` & `fixinventorycore-4.0.5/fixcore/user/user_management.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/util.py` & `fixinventorycore-4.0.5/fixcore/util.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/validator.py` & `fixinventorycore-4.0.5/fixcore/validator.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/web/accesslog.py` & `fixinventorycore-4.0.5/fixcore/web/accesslog.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/web/api.py` & `fixinventorycore-4.0.5/fixcore/web/api.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/web/auth.py` & `fixinventorycore-4.0.5/fixcore/web/auth.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/web/certificate_handler.py` & `fixinventorycore-4.0.5/fixcore/web/certificate_handler.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/web/content_renderer.py` & `fixinventorycore-4.0.5/fixcore/web/content_renderer.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/web/directives.py` & `fixinventorycore-4.0.5/fixcore/web/directives.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/web/permission.py` & `fixinventorycore-4.0.5/fixcore/web/permission.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/web/tsdb.py` & `fixinventorycore-4.0.5/fixcore/web/tsdb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixcore/worker_task_queue.py` & `fixinventorycore-4.0.5/fixcore/worker_task_queue.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/fixinventorycore.egg-info/PKG-INFO` & `fixinventorycore-4.0.5/fixinventorycore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventorycore
-Version: 4.0.4
+Version: 4.0.5
 Summary: Keeps all the things.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Homepage, https://inventory.fix.security
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `fixinventorycore-4.0.4/fixinventorycore.egg-info/SOURCES.txt` & `fixinventorycore-4.0.5/fixinventorycore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/pyproject.toml` & `fixinventorycore-4.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fixinventorycore"
-version = "4.0.4"
+version = "4.0.5"
 authors = [{name="Some Engineering Inc."}]
 description = "Keeps all the things."
 license = { text="AGPLv3" }
 urls = {"Homepage" = "https://inventory.fix.security"}
 requires-python = ">=3.11"
 classifiers = [
     # Current project status
```

### Comparing `fixinventorycore-4.0.4/tests/fixcore/__init__.py` & `fixinventorycore-4.0.5/tests/fixcore/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/analytics/posthog_test.py` & `fixinventorycore-4.0.5/tests/fixcore/analytics/posthog_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/analytics/recurrent_events_test.py` & `fixinventorycore-4.0.5/tests/fixcore/analytics/recurrent_events_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/cli/cli_test.py` & `fixinventorycore-4.0.5/tests/fixcore/cli/cli_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/cli/command_test.py` & `fixinventorycore-4.0.5/tests/fixcore/cli/command_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/cli/model_test.py` & `fixinventorycore-4.0.5/tests/fixcore/cli/model_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/config/config_handler_service_test.py` & `fixinventorycore-4.0.5/tests/fixcore/config/config_handler_service_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/config/config_override_service_test.py` & `fixinventorycore-4.0.5/tests/fixcore/config/config_override_service_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/config/core_config_handler_test.py` & `fixinventorycore-4.0.5/tests/fixcore/config/core_config_handler_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/conftest.py` & `fixinventorycore-4.0.5/tests/fixcore/conftest.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/console_renderer_test.py` & `fixinventorycore-4.0.5/tests/fixcore/console_renderer_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/core_config_test.py` & `fixinventorycore-4.0.5/tests/fixcore/core_config_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/db/arango_query_test.py` & `fixinventorycore-4.0.5/tests/fixcore/db/arango_query_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/db/arangodb_functions_test.py` & `fixinventorycore-4.0.5/tests/fixcore/db/arangodb_functions_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/db/async_arangodb_test.py` & `fixinventorycore-4.0.5/tests/fixcore/db/async_arangodb_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/db/configdb_test.py` & `fixinventorycore-4.0.5/tests/fixcore/db/configdb_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/db/db_access_test.py` & `fixinventorycore-4.0.5/tests/fixcore/db/db_access_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/db/deferredouteredgedb_test.py` & `fixinventorycore-4.0.5/tests/fixcore/db/deferredouteredgedb_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/db/entitydb.py` & `fixinventorycore-4.0.5/tests/fixcore/db/entitydb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/db/graphdb_test.py` & `fixinventorycore-4.0.5/tests/fixcore/db/graphdb_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/db/jobdb_test.py` & `fixinventorycore-4.0.5/tests/fixcore/db/jobdb_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/db/model_test.py` & `fixinventorycore-4.0.5/tests/fixcore/db/model_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/db/modeldb_test.py` & `fixinventorycore-4.0.5/tests/fixcore/db/modeldb_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/db/reportdb_test.py` & `fixinventorycore-4.0.5/tests/fixcore/db/reportdb_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/db/runningtaskdb_test.py` & `fixinventorycore-4.0.5/tests/fixcore/db/runningtaskdb_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/db/system_data_db_test.py` & `fixinventorycore-4.0.5/tests/fixcore/db/system_data_db_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/db/templatedb_test.py` & `fixinventorycore-4.0.5/tests/fixcore/db/templatedb_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/db/timeseriesdb_test.py` & `fixinventorycore-4.0.5/tests/fixcore/db/timeseriesdb_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/dependencies_test.py` & `fixinventorycore-4.0.5/tests/fixcore/dependencies_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/graph_manager/graph_manager_test.py` & `fixinventorycore-4.0.5/tests/fixcore/graph_manager/graph_manager_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/hypothesis_extension.py` & `fixinventorycore-4.0.5/tests/fixcore/hypothesis_extension.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/infra_apps/local_runtime_test.py` & `fixinventorycore-4.0.5/tests/fixcore/infra_apps/local_runtime_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/infra_apps/package_manager_test.py` & `fixinventorycore-4.0.5/tests/fixcore/infra_apps/package_manager_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/message_bus_test.py` & `fixinventorycore-4.0.5/tests/fixcore/message_bus_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/model/__init__.py` & `fixinventorycore-4.0.5/tests/fixcore/model/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/model/adjust_node_test.py` & `fixinventorycore-4.0.5/tests/fixcore/model/adjust_node_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/model/db_updater_test.py` & `fixinventorycore-4.0.5/tests/fixcore/model/db_updater_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/model/exportable_model_test.py` & `fixinventorycore-4.0.5/tests/fixcore/model/exportable_model_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/model/graph_access_test.py` & `fixinventorycore-4.0.5/tests/fixcore/model/graph_access_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/model/json_schema_test.py` & `fixinventorycore-4.0.5/tests/fixcore/model/json_schema_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/model/model_handler_test.py` & `fixinventorycore-4.0.5/tests/fixcore/model/model_handler_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/model/model_test.py` & `fixinventorycore-4.0.5/tests/fixcore/model/model_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/model/typed_model_test.py` & `fixinventorycore-4.0.5/tests/fixcore/model/typed_model_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/query/__init__.py` & `fixinventorycore-4.0.5/tests/fixcore/query/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/query/model_test.py` & `fixinventorycore-4.0.5/tests/fixcore/query/model_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/query/query_parser_test.py` & `fixinventorycore-4.0.5/tests/fixcore/query/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/query/template_expander_test.py` & `fixinventorycore-4.0.5/tests/fixcore/query/template_expander_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/report/benchmark_renderer_test.py` & `fixinventorycore-4.0.5/tests/fixcore/report/benchmark_renderer_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/report/inspector_service_test.py` & `fixinventorycore-4.0.5/tests/fixcore/report/inspector_service_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/task/job_handler_test.py` & `fixinventorycore-4.0.5/tests/fixcore/task/job_handler_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/task/start_workflow_on_first_subscriber_test.py` & `fixinventorycore-4.0.5/tests/fixcore/task/start_workflow_on_first_subscriber_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/task/subscribers_test.py` & `fixinventorycore-4.0.5/tests/fixcore/task/subscribers_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/task/task_description_test.py` & `fixinventorycore-4.0.5/tests/fixcore/task/task_description_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/task/task_handler_test.py` & `fixinventorycore-4.0.5/tests/fixcore/task/task_handler_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/user/user_management_service_test.py` & `fixinventorycore-4.0.5/tests/fixcore/user/user_management_service_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/util_test.py` & `fixinventorycore-4.0.5/tests/fixcore/util_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/utils.py` & `fixinventorycore-4.0.5/tests/fixcore/utils.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/validator_test.py` & `fixinventorycore-4.0.5/tests/fixcore/validator_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/web/api_client.py` & `fixinventorycore-4.0.5/tests/fixcore/web/api_client.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/web/api_test.py` & `fixinventorycore-4.0.5/tests/fixcore/web/api_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/web/auth_test.py` & `fixinventorycore-4.0.5/tests/fixcore/web/auth_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/web/certificate_handler_test.py` & `fixinventorycore-4.0.5/tests/fixcore/web/certificate_handler_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/web/content_renderer_test.py` & `fixinventorycore-4.0.5/tests/fixcore/web/content_renderer_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/web/permission_test.py` & `fixinventorycore-4.0.5/tests/fixcore/web/permission_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.4/tests/fixcore/worker_task_queue_test.py` & `fixinventorycore-4.0.5/tests/fixcore/worker_task_queue_test.py`

 * *Files identical despite different names*

