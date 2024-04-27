# Comparing `tmp/prometheus_pve_exporter-3.2.5.tar.gz` & `tmp/prometheus_pve_exporter-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_pve_exporter-3.2.5.tar", last modified: Wed Apr 17 05:14:14 2024, max compression
+gzip compressed data, was "prometheus_pve_exporter-3.3.0.tar", last modified: Sat Apr 27 10:08:03 2024, max compression
```

## Comparing `prometheus_pve_exporter-3.2.5.tar` & `prometheus_pve_exporter-3.3.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:14:14.197552 prometheus_pve_exporter-3.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:14:14.193552 prometheus_pve_exporter-3.2.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:14:14.193552 prometheus_pve_exporter-3.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/.github/workflows/container-image.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/.github/workflows/container-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    10448 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-04-17 05:14:14.197552 prometheus_pve_exporter-3.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12840 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/pve.yml
--rw-r--r--   0 runner    (1001) docker     (127)    21005 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/pylintrc.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)    30041 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:14:14.197552 prometheus_pve_exporter-3.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:14:14.189552 prometheus_pve_exporter-3.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:14:14.193552 prometheus_pve_exporter-3.2.5/src/prometheus_pve_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-04-17 05:14:14.000000 prometheus_pve_exporter-3.2.5/src/prometheus_pve_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-17 05:14:14.000000 prometheus_pve_exporter-3.2.5/src/prometheus_pve_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 05:14:14.000000 prometheus_pve_exporter-3.2.5/src/prometheus_pve_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 05:14:14.000000 prometheus_pve_exporter-3.2.5/src/prometheus_pve_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-17 05:14:14.000000 prometheus_pve_exporter-3.2.5/src/prometheus_pve_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 05:14:14.000000 prometheus_pve_exporter-3.2.5/src/prometheus_pve_exporter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:14:14.193552 prometheus_pve_exporter-3.2.5/src/pve_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/src/pve_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/src/pve_exporter/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3845 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/src/pve_exporter/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:14:14.193552 prometheus_pve_exporter-3.2.5/src/pve_exporter/collector/
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/src/pve_exporter/collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/src/pve_exporter/collector/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/src/pve_exporter/collector/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/src/pve_exporter/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-17 05:14:06.000000 prometheus_pve_exporter-3.2.5/src/pve_exporter/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:08:03.936236 prometheus_pve_exporter-3.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:08:03.936236 prometheus_pve_exporter-3.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:08:03.936236 prometheus_pve_exporter-3.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/.github/workflows/container-image.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/.github/workflows/container-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10638 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15275 2024-04-27 10:08:03.936236 prometheus_pve_exporter-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/pve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    21005 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/pylintrc.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)    30041 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 10:08:03.936236 prometheus_pve_exporter-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:08:03.932236 prometheus_pve_exporter-3.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:08:03.936236 prometheus_pve_exporter-3.3.0/src/prometheus_pve_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15275 2024-04-27 10:08:03.000000 prometheus_pve_exporter-3.3.0/src/prometheus_pve_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-27 10:08:03.000000 prometheus_pve_exporter-3.3.0/src/prometheus_pve_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 10:08:03.000000 prometheus_pve_exporter-3.3.0/src/prometheus_pve_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-27 10:08:03.000000 prometheus_pve_exporter-3.3.0/src/prometheus_pve_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-27 10:08:03.000000 prometheus_pve_exporter-3.3.0/src/prometheus_pve_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-27 10:08:03.000000 prometheus_pve_exporter-3.3.0/src/prometheus_pve_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:08:03.936236 prometheus_pve_exporter-3.3.0/src/pve_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/src/pve_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/src/pve_exporter/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4115 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/src/pve_exporter/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:08:03.936236 prometheus_pve_exporter-3.3.0/src/pve_exporter/collector/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/src/pve_exporter/collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/src/pve_exporter/collector/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/src/pve_exporter/collector/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/src/pve_exporter/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-27 10:08:00.000000 prometheus_pve_exporter-3.3.0/src/pve_exporter/http.py
```

### Comparing `prometheus_pve_exporter-3.2.5/.github/workflows/ci.yml` & `prometheus_pve_exporter-3.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.2.5/.github/workflows/container-image.yml` & `prometheus_pve_exporter-3.3.0/.github/workflows/container-image.yml`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.2.5/.github/workflows/container-test.yml` & `prometheus_pve_exporter-3.3.0/.github/workflows/container-test.yml`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.2.5/.github/workflows/pypi.yml` & `prometheus_pve_exporter-3.3.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.2.5/CHANGELOG.rst` & `prometheus_pve_exporter-3.3.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 The format is based on `Keep a Changelog`_ and this project adheres to
 `Semantic Versioning`_.
 
 `Unreleased`_
 -------------
 
 
+`3.3.0`_ - 2024-04-27
+---------------------
+
+Added
+~~~~~
+
+- Add ZFS replication metrics (#243)
+
+
 `3.2.5`_ - 2024-04-17
 ---------------------
 
 Changed
 ~~~~~~~
 
 - Bump gunicorn from 21.2.0 to 22.0.0 (#241)
@@ -385,24 +394,25 @@
 ~~~~~
 
 -  IPv6 support
 
 
 .. _Keep a Changelog: http://keepachangelog.com/en/1.0.0/
 .. _Semantic Versioning: http://semver.org/spec/v2.0.0.html
-.. _Unreleased: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.5...HEAD
-.. _3.2.5: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.5...v3.2.4
-.. _3.2.4: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.4...v3.2.3
-.. _3.2.3: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.3...v3.2.2
-.. _3.2.2: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.2...v3.2.1
-.. _3.2.1: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.1...v3.2.0
-.. _3.2.0: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.0...v3.1.0
-.. _3.1.0: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.1.0...v3.0.2
-.. _3.0.2: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.0.2...v3.0.1
-.. _3.0.1: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.0.1...v3.0.0
+.. _Unreleased: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.3.0...HEAD
+.. _3.3.0: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.5...v3.3.0
+.. _3.2.5: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.4...v3.2.5
+.. _3.2.4: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.3...v3.2.4
+.. _3.2.3: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.2...v3.2.3
+.. _3.2.2: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.1...v3.2.2
+.. _3.2.1: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.0...v3.2.1
+.. _3.2.0: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.1.0...v3.2.0
+.. _3.1.0: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.0.2...v3.1.0
+.. _3.0.2: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.0.1...v3.0.2
+.. _3.0.1: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.0.0...v3.0.1
 .. _3.0.0: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.0.0b1...v3.0.0
 .. _3.0.0b1: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v2.3.1...v3.0.0b1
 .. _2.3.1: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v2.3.0...v2.3.1
 .. _2.3.0: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v2.2.4...v2.3.0
 .. _2.2.3: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v2.2.3...v2.2.4
 .. _2.2.3: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v2.2.2...v2.2.3
 .. _2.2.2: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v2.2.1...v2.2.2
```

### Comparing `prometheus_pve_exporter-3.2.5/Dockerfile` & `prometheus_pve_exporter-3.3.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.2.5/LICENSE` & `prometheus_pve_exporter-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.2.5/PKG-INFO` & `prometheus_pve_exporter-3.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-pve-exporter
-Version: 3.2.5
+Version: 3.3.0
 Summary: Proxmox VE exporter for the Prometheus monitoring system.
 Author-email: Lorenz Schori <lo@znerol.ch>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/prometheus-pve/prometheus-pve-exporter
 Keywords: prometheus,exporter,network,monitoring,proxmox
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
@@ -76,14 +76,15 @@
 
     usage: pve_exporter [-h] [--collector.status | --no-collector.status]
                         [--collector.version | --no-collector.version]
                         [--collector.node | --no-collector.node]
                         [--collector.cluster | --no-collector.cluster]
                         [--collector.resources | --no-collector.resources]
                         [--collector.config | --no-collector.config]
+                        [--collector.replication | --no-collector.replication]
                         [--config.file CONFIG_FILE]
                         [--web.listen-address WEB_LISTEN_ADDRESS]
                         [--server.keyfile SERVER_KEYFILE]
                         [--server.certfile SERVER_CERTFILE]
 
     options:
       -h, --help            show this help message and exit
@@ -114,14 +115,16 @@
 
     node collectors:
       node collectors are run if the url parameter node=1 is set and skipped if
       the url parameter node=0 is set on a scrape url.
 
       --collector.config, --no-collector.config
                             Exposes PVE onboot status
+      --collector.replication, --no-collector.replication
+                            Exposes PVE replication info
 
 
 Use `[::]` in the `--web.listen-address` flag in order to bind to both IPv6 and
 IPv4 sockets on dual stacked machines.
 
 Visit http://localhost:9221/pve?target=1.2.3.4&cluster=1&node=1 where 1.2.3.4
 is the IP of the Proxmox VE node to get metrics from. Specify the ``module``
@@ -215,14 +218,32 @@
     pve_node_info{id="node/proxmox",level="",name="proxmox",nodeid="0"} 1.0
     # HELP pve_onboot_status Proxmox vm config onboot value
     # TYPE pve_onboot_status gauge
     pve_onboot_status{id="qemu/201",node="proxmox",type="qemu"} 1.0
     # HELP pve_version_info Proxmox VE version info
     # TYPE pve_version_info gauge
     pve_version_info{release="7.1",repoid="6fe299a0",version="7.1-5"} 1.0
+    # HELP pve_replication_duration_seconds Proxmox vm replication duration
+    # TYPE pve_replication_duration_seconds gauge
+    pve_replication_duration_seconds{id="1-0"} 7.73584
+    # HELP pve_replication_last_sync_timestamp_seconds Proxmox vm replication last_sync
+    # TYPE pve_replication_last_sync_timestamp_seconds gauge
+    pve_replication_last_sync_timestamp_seconds{id="1-0"} 1.713382503e+09
+    # HELP pve_replication_last_try_timestamp_seconds Proxmox vm replication last_try
+    # TYPE pve_replication_last_try_timestamp_seconds gauge
+    pve_replication_last_try_timestamp_seconds{id="1-0"} 1.713382503e+09
+    # HELP pve_replication_next_sync_timestamp_seconds Proxmox vm replication next_sync
+    # TYPE pve_replication_next_sync_timestamp_seconds gauge
+    pve_replication_next_sync_timestamp_seconds{id="1-0"} 1.7134689e+09
+    # HELP pve_replication_failed_syncs Proxmox vm replication fail_count
+    # TYPE pve_replication_failed_syncs gauge
+    pve_replication_failed_syncs{id="1-0"} 0.0
+    # HELP pve_replication_info Proxmox vm replication info
+    # TYPE pve_replication_info gauge
+    pve_replication_info{guest="qemu/1",id="1-0",source="node/proxmox1",target="node/proxmox2",type="local"} 1.0
 
 Authentication
 --------------
 
 **Using pve.yml config file**
 
 Example ``pve.yml`` for password authentication:
```

### Comparing `prometheus_pve_exporter-3.2.5/README.rst` & `prometheus_pve_exporter-3.3.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
     usage: pve_exporter [-h] [--collector.status | --no-collector.status]
                         [--collector.version | --no-collector.version]
                         [--collector.node | --no-collector.node]
                         [--collector.cluster | --no-collector.cluster]
                         [--collector.resources | --no-collector.resources]
                         [--collector.config | --no-collector.config]
+                        [--collector.replication | --no-collector.replication]
                         [--config.file CONFIG_FILE]
                         [--web.listen-address WEB_LISTEN_ADDRESS]
                         [--server.keyfile SERVER_KEYFILE]
                         [--server.certfile SERVER_CERTFILE]
 
     options:
       -h, --help            show this help message and exit
@@ -86,14 +87,16 @@
 
     node collectors:
       node collectors are run if the url parameter node=1 is set and skipped if
       the url parameter node=0 is set on a scrape url.
 
       --collector.config, --no-collector.config
                             Exposes PVE onboot status
+      --collector.replication, --no-collector.replication
+                            Exposes PVE replication info
 
 
 Use `[::]` in the `--web.listen-address` flag in order to bind to both IPv6 and
 IPv4 sockets on dual stacked machines.
 
 Visit http://localhost:9221/pve?target=1.2.3.4&cluster=1&node=1 where 1.2.3.4
 is the IP of the Proxmox VE node to get metrics from. Specify the ``module``
@@ -187,14 +190,32 @@
     pve_node_info{id="node/proxmox",level="",name="proxmox",nodeid="0"} 1.0
     # HELP pve_onboot_status Proxmox vm config onboot value
     # TYPE pve_onboot_status gauge
     pve_onboot_status{id="qemu/201",node="proxmox",type="qemu"} 1.0
     # HELP pve_version_info Proxmox VE version info
     # TYPE pve_version_info gauge
     pve_version_info{release="7.1",repoid="6fe299a0",version="7.1-5"} 1.0
+    # HELP pve_replication_duration_seconds Proxmox vm replication duration
+    # TYPE pve_replication_duration_seconds gauge
+    pve_replication_duration_seconds{id="1-0"} 7.73584
+    # HELP pve_replication_last_sync_timestamp_seconds Proxmox vm replication last_sync
+    # TYPE pve_replication_last_sync_timestamp_seconds gauge
+    pve_replication_last_sync_timestamp_seconds{id="1-0"} 1.713382503e+09
+    # HELP pve_replication_last_try_timestamp_seconds Proxmox vm replication last_try
+    # TYPE pve_replication_last_try_timestamp_seconds gauge
+    pve_replication_last_try_timestamp_seconds{id="1-0"} 1.713382503e+09
+    # HELP pve_replication_next_sync_timestamp_seconds Proxmox vm replication next_sync
+    # TYPE pve_replication_next_sync_timestamp_seconds gauge
+    pve_replication_next_sync_timestamp_seconds{id="1-0"} 1.7134689e+09
+    # HELP pve_replication_failed_syncs Proxmox vm replication fail_count
+    # TYPE pve_replication_failed_syncs gauge
+    pve_replication_failed_syncs{id="1-0"} 0.0
+    # HELP pve_replication_info Proxmox vm replication info
+    # TYPE pve_replication_info gauge
+    pve_replication_info{guest="qemu/1",id="1-0",source="node/proxmox1",target="node/proxmox2",type="local"} 1.0
 
 Authentication
 --------------
 
 **Using pve.yml config file**
 
 Example ``pve.yml`` for password authentication:
```

### Comparing `prometheus_pve_exporter-3.2.5/pylintrc.toml` & `prometheus_pve_exporter-3.3.0/pylintrc.toml`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.2.5/pyproject.toml` & `prometheus_pve_exporter-3.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prometheus-pve-exporter"
-version = "3.2.5"
+version = "3.3.0"
 authors = [{ name = "Lorenz Schori", email = "lo@znerol.ch" }]
 description = "Proxmox VE exporter for the Prometheus monitoring system."
 requires-python = ">=3.9"
 keywords = ["prometheus", "exporter", "network", "monitoring", "proxmox"]
 license = { text = "Apache-2.0" }
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `prometheus_pve_exporter-3.2.5/requirements.txt` & `prometheus_pve_exporter-3.3.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.2.5/src/prometheus_pve_exporter.egg-info/PKG-INFO` & `prometheus_pve_exporter-3.3.0/src/prometheus_pve_exporter.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-pve-exporter
-Version: 3.2.5
+Version: 3.3.0
 Summary: Proxmox VE exporter for the Prometheus monitoring system.
 Author-email: Lorenz Schori <lo@znerol.ch>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/prometheus-pve/prometheus-pve-exporter
 Keywords: prometheus,exporter,network,monitoring,proxmox
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
@@ -76,14 +76,15 @@
 
     usage: pve_exporter [-h] [--collector.status | --no-collector.status]
                         [--collector.version | --no-collector.version]
                         [--collector.node | --no-collector.node]
                         [--collector.cluster | --no-collector.cluster]
                         [--collector.resources | --no-collector.resources]
                         [--collector.config | --no-collector.config]
+                        [--collector.replication | --no-collector.replication]
                         [--config.file CONFIG_FILE]
                         [--web.listen-address WEB_LISTEN_ADDRESS]
                         [--server.keyfile SERVER_KEYFILE]
                         [--server.certfile SERVER_CERTFILE]
 
     options:
       -h, --help            show this help message and exit
@@ -114,14 +115,16 @@
 
     node collectors:
       node collectors are run if the url parameter node=1 is set and skipped if
       the url parameter node=0 is set on a scrape url.
 
       --collector.config, --no-collector.config
                             Exposes PVE onboot status
+      --collector.replication, --no-collector.replication
+                            Exposes PVE replication info
 
 
 Use `[::]` in the `--web.listen-address` flag in order to bind to both IPv6 and
 IPv4 sockets on dual stacked machines.
 
 Visit http://localhost:9221/pve?target=1.2.3.4&cluster=1&node=1 where 1.2.3.4
 is the IP of the Proxmox VE node to get metrics from. Specify the ``module``
@@ -215,14 +218,32 @@
     pve_node_info{id="node/proxmox",level="",name="proxmox",nodeid="0"} 1.0
     # HELP pve_onboot_status Proxmox vm config onboot value
     # TYPE pve_onboot_status gauge
     pve_onboot_status{id="qemu/201",node="proxmox",type="qemu"} 1.0
     # HELP pve_version_info Proxmox VE version info
     # TYPE pve_version_info gauge
     pve_version_info{release="7.1",repoid="6fe299a0",version="7.1-5"} 1.0
+    # HELP pve_replication_duration_seconds Proxmox vm replication duration
+    # TYPE pve_replication_duration_seconds gauge
+    pve_replication_duration_seconds{id="1-0"} 7.73584
+    # HELP pve_replication_last_sync_timestamp_seconds Proxmox vm replication last_sync
+    # TYPE pve_replication_last_sync_timestamp_seconds gauge
+    pve_replication_last_sync_timestamp_seconds{id="1-0"} 1.713382503e+09
+    # HELP pve_replication_last_try_timestamp_seconds Proxmox vm replication last_try
+    # TYPE pve_replication_last_try_timestamp_seconds gauge
+    pve_replication_last_try_timestamp_seconds{id="1-0"} 1.713382503e+09
+    # HELP pve_replication_next_sync_timestamp_seconds Proxmox vm replication next_sync
+    # TYPE pve_replication_next_sync_timestamp_seconds gauge
+    pve_replication_next_sync_timestamp_seconds{id="1-0"} 1.7134689e+09
+    # HELP pve_replication_failed_syncs Proxmox vm replication fail_count
+    # TYPE pve_replication_failed_syncs gauge
+    pve_replication_failed_syncs{id="1-0"} 0.0
+    # HELP pve_replication_info Proxmox vm replication info
+    # TYPE pve_replication_info gauge
+    pve_replication_info{guest="qemu/1",id="1-0",source="node/proxmox1",target="node/proxmox2",type="local"} 1.0
 
 Authentication
 --------------
 
 **Using pve.yml config file**
 
 Example ``pve.yml`` for password authentication:
```

### Comparing `prometheus_pve_exporter-3.2.5/src/prometheus_pve_exporter.egg-info/SOURCES.txt` & `prometheus_pve_exporter-3.3.0/src/prometheus_pve_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.2.5/src/pve_exporter/cli.py` & `prometheus_pve_exporter-3.3.0/src/pve_exporter/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,18 @@
         'node collectors are run if the url parameter node=1 is set and '
         'skipped if the url parameter node=0 is set on a scrape url.'
     ))
     nodeflags.add_argument('--collector.config', dest='collector_config',
                            action=BooleanOptionalAction, default=True,
                            help='Exposes PVE onboot status')
 
+    nodeflags.add_argument('--collector.replication', dest='collector_replication',
+                           action=BooleanOptionalAction, default=True,
+                           help='Exposes PVE replication info')
+
     parser.add_argument('--config.file', type=pathlib.Path,
                         dest="config_file", default='/etc/prometheus/pve.yml',
                         help='Path to config file (/etc/prometheus/pve.yml)')
 
     parser.add_argument('--web.listen-address',
                         dest="web_listen_address", default='[::]:9221',
                         help=(
@@ -65,15 +69,16 @@
 
     collectors = CollectorsOptions(
         status=params.collector_status,
         version=params.collector_version,
         node=params.collector_node,
         cluster=params.collector_cluster,
         resources=params.collector_resources,
-        config=params.collector_config
+        config=params.collector_config,
+        replication=params.collector_replication
     )
 
     # Load configuration.
     if 'PVE_USER' in os.environ:
         config = config_from_env(os.environ)
     else:
         with open(params.config_file, encoding='utf-8') as handle:
```

### Comparing `prometheus_pve_exporter-3.2.5/src/pve_exporter/collector/__init__.py` & `prometheus_pve_exporter-3.3.0/src/pve_exporter/collector/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,27 @@
 from pve_exporter.collector.cluster import (
     StatusCollector,
     ClusterResourcesCollector,
     ClusterNodeCollector,
     VersionCollector,
     ClusterInfoCollector
 )
-from pve_exporter.collector.node import NodeConfigCollector
+from pve_exporter.collector.node import (
+    NodeConfigCollector,
+    NodeReplicationCollector
+)
 
 CollectorsOptions = collections.namedtuple('CollectorsOptions', [
     'status',
     'version',
     'node',
     'cluster',
     'resources',
     'config',
+    'replication'
 ])
 
 
 def collect_pve(config, host, cluster, node, options: CollectorsOptions):
     """Scrape a host and return prometheus text format for it"""
 
     pve = ProxmoxAPI(host, **config)
@@ -40,9 +44,11 @@
         registry.register(ClusterNodeCollector(pve))
     if cluster and options.cluster:
         registry.register(ClusterInfoCollector(pve))
     if cluster and options.version:
         registry.register(VersionCollector(pve))
     if node and options.config:
         registry.register(NodeConfigCollector(pve))
+    if node and options.replication:
+        registry.register(NodeReplicationCollector(pve))
 
     return generate_latest(registry)
```

### Comparing `prometheus_pve_exporter-3.2.5/src/pve_exporter/collector/cluster.py` & `prometheus_pve_exporter-3.3.0/src/pve_exporter/collector/cluster.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.2.5/src/pve_exporter/config.py` & `prometheus_pve_exporter-3.3.0/src/pve_exporter/config.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.2.5/src/pve_exporter/http.py` & `prometheus_pve_exporter-3.3.0/src/pve_exporter/http.py`

 * *Files identical despite different names*

