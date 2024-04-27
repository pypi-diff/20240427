# Comparing `tmp/adafruit-circuitpython-requests-3.2.4.tar.gz` & `tmp/adafruit_circuitpython_requests-3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-requests-3.2.4.tar", last modified: Wed Apr 10 23:58:42 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_requests-3.2.5.tar", last modified: Mon Apr 15 15:55:43 2024, max compression
```

## Comparing `adafruit-circuitpython-requests-3.2.4.tar` & `adafruit_circuitpython_requests-3.2.5.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.180429 adafruit-circuitpython-requests-3.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.164429 adafruit-circuitpython-requests-3.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.168429 adafruit-circuitpython-requests-3.2.4/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.168429 adafruit-circuitpython-requests-3.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/.github/workflows/release_pypi.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1724 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     6147 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1098 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.168429 adafruit-circuitpython-requests-3.2.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-10 23:58:42.180429 adafruit-circuitpython-requests-3.2.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2642 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.180429 adafruit-circuitpython-requests-3.2.4/adafruit_circuitpython_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-10 23:58:42.000000 adafruit-circuitpython-requests-3.2.4/adafruit_circuitpython_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-10 23:58:42.000000 adafruit-circuitpython-requests-3.2.4/adafruit_circuitpython_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:58:42.000000 adafruit-circuitpython-requests-3.2.4/adafruit_circuitpython_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 23:58:42.000000 adafruit-circuitpython-requests-3.2.4/adafruit_circuitpython_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 23:58:42.000000 adafruit-circuitpython-requests-3.2.4/adafruit_circuitpython_requests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21346 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/adafruit_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.172429 adafruit-circuitpython-requests-3.2.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.172429 adafruit-circuitpython-requests-3.2.4/docs/_static/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4414 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/_static/favicon.ico.license
--rwxr-xr-x   0 runner    (1001) docker     (127)      267 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/api.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (127)     5400 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      803 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/examples.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (127)      973 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.164429 adafruit-circuitpython-requests-3.2.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.172429 adafruit-circuitpython-requests-3.2.4/examples/cpython/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/cpython/requests_cpython_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/cpython/requests_cpython_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.172429 adafruit-circuitpython-requests-3.2.4/examples/esp32spi/
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/esp32spi/requests_esp32spi_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/esp32spi/requests_esp32spi_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.172429 adafruit-circuitpython-requests-3.2.4/examples/fona/
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/fona/requests_fona_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/fona/requests_fona_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.172429 adafruit-circuitpython-requests-3.2.4/examples/wifi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.176429 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_discord.py
--rw-r--r--   0 runner    (1001) docker     (127)    15732 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_fitbit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_mastodon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py
--rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_premiereleague.py
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_steam.py
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_twitch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_youtube.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_multiple_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/requests_wifi_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/requests_wifi_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.176429 adafruit-circuitpython-requests-3.2.4/examples/wiznet5k/
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wiznet5k/requests_wiznet5k_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wiznet5k/requests_wiznet5k_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 23:58:42.180429 adafruit-circuitpython-requests-3.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.180429 adafruit-circuitpython-requests-3.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/chunk_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/chunked_redirect_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/header_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/method_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/mocket.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/parse_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/protocol_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/reuse_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:43.320688 adafruit_circuitpython_requests-3.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:43.304688 adafruit_circuitpython_requests-3.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:43.308688 adafruit_circuitpython_requests-3.2.5/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:43.312688 adafruit_circuitpython_requests-3.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/.github/workflows/release_pypi.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1724 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6147 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1098 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:43.312688 adafruit_circuitpython_requests-3.2.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-15 15:55:43.320688 adafruit_circuitpython_requests-3.2.5/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2642 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:43.320688 adafruit_circuitpython_requests-3.2.5/adafruit_circuitpython_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-15 15:55:43.000000 adafruit_circuitpython_requests-3.2.5/adafruit_circuitpython_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-15 15:55:43.000000 adafruit_circuitpython_requests-3.2.5/adafruit_circuitpython_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:55:43.000000 adafruit_circuitpython_requests-3.2.5/adafruit_circuitpython_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 15:55:43.000000 adafruit_circuitpython_requests-3.2.5/adafruit_circuitpython_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 15:55:43.000000 adafruit_circuitpython_requests-3.2.5/adafruit_circuitpython_requests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21346 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/adafruit_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:43.312688 adafruit_circuitpython_requests-3.2.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:43.312688 adafruit_circuitpython_requests-3.2.5/docs/_static/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4414 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/docs/_static/favicon.ico.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)      267 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/docs/api.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5400 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      803 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/docs/examples.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)      973 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:43.308688 adafruit_circuitpython_requests-3.2.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:43.312688 adafruit_circuitpython_requests-3.2.5/examples/cpython/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/cpython/requests_cpython_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/cpython/requests_cpython_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:43.316688 adafruit_circuitpython_requests-3.2.5/examples/esp32spi/
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/esp32spi/requests_esp32spi_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/esp32spi/requests_esp32spi_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:43.316688 adafruit_circuitpython_requests-3.2.5/examples/fona/
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/fona/requests_fona_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/fona/requests_fona_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:43.316688 adafruit_circuitpython_requests-3.2.5/examples/wifi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:43.316688 adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_discord.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15732 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_fitbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_mastodon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_premiereleague.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_steam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_twitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_youtube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_multiple_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/wifi/requests_wifi_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/wifi/requests_wifi_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:43.316688 adafruit_circuitpython_requests-3.2.5/examples/wiznet5k/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/wiznet5k/requests_wiznet5k_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/examples/wiznet5k/requests_wiznet5k_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:55:43.320688 adafruit_circuitpython_requests-3.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:55:43.320688 adafruit_circuitpython_requests-3.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/tests/chunk_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/tests/chunked_redirect_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/tests/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/tests/header_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/tests/method_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/tests/mocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/tests/parse_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/tests/protocol_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-04-15 15:55:40.000000 adafruit_circuitpython_requests-3.2.5/tests/reuse_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-15 15:55:30.000000 adafruit_circuitpython_requests-3.2.5/tox.ini
```

### Comparing `adafruit-circuitpython-requests-3.2.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_requests-3.2.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/.gitignore` & `adafruit_circuitpython_requests-3.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/.pre-commit-config.yaml` & `adafruit_circuitpython_requests-3.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/.pylintrc` & `adafruit_circuitpython_requests-3.2.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_requests-3.2.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/LICENSE` & `adafruit_circuitpython_requests-3.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_requests-3.2.5/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/LICENSES/MIT.txt` & `adafruit_circuitpython_requests-3.2.5/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/LICENSES/Unlicense.txt` & `adafruit_circuitpython_requests-3.2.5/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/PKG-INFO` & `adafruit_circuitpython_requests-3.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-requests
-Version: 3.2.4
+Version: 3.2.5
 Summary: A requests-like library for web interfacing
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Requests
 Keywords: adafruit,blinka,circuitpython,micropython,requests,requests,,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-requests-3.2.4/README.rst` & `adafruit_circuitpython_requests-3.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/adafruit_circuitpython_requests.egg-info/PKG-INFO` & `adafruit_circuitpython_requests-3.2.5/adafruit_circuitpython_requests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-requests
-Version: 3.2.4
+Version: 3.2.5
 Summary: A requests-like library for web interfacing
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Requests
 Keywords: adafruit,blinka,circuitpython,micropython,requests,requests,,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-requests-3.2.4/adafruit_circuitpython_requests.egg-info/SOURCES.txt` & `adafruit_circuitpython_requests-3.2.5/adafruit_circuitpython_requests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/adafruit_requests.py` & `adafruit_circuitpython_requests-3.2.5/adafruit_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
   https://github.com/adafruit/circuitpython/releases
 
 * Adafruit's Connection Manager library:
   https://github.com/adafruit/Adafruit_CircuitPython_ConnectionManager
 
 """
 
-__version__ = "3.2.4"
+__version__ = "3.2.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Requests.git"
 
 import errno
 import json as json_module
 import sys
 
 from adafruit_connection_manager import get_connection_manager
```

### Comparing `adafruit-circuitpython-requests-3.2.4/docs/_static/favicon.ico` & `adafruit_circuitpython_requests-3.2.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/docs/conf.py` & `adafruit_circuitpython_requests-3.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/docs/examples.rst` & `adafruit_circuitpython_requests-3.2.5/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/docs/index.rst` & `adafruit_circuitpython_requests-3.2.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/cpython/requests_cpython_advanced.py` & `adafruit_circuitpython_requests-3.2.5/examples/cpython/requests_cpython_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/cpython/requests_cpython_simpletest.py` & `adafruit_circuitpython_requests-3.2.5/examples/cpython/requests_cpython_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/esp32spi/requests_esp32spi_advanced.py` & `adafruit_circuitpython_requests-3.2.5/examples/esp32spi/requests_esp32spi_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/esp32spi/requests_esp32spi_simpletest.py` & `adafruit_circuitpython_requests-3.2.5/examples/esp32spi/requests_esp32spi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/fona/requests_fona_advanced.py` & `adafruit_circuitpython_requests-3.2.5/examples/fona/requests_fona_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/fona/requests_fona_simpletest.py` & `adafruit_circuitpython_requests-3.2.5/examples/fona/requests_fona_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py` & `adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_discord.py` & `adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_discord.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_fitbit.py` & `adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_fitbit.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_github.py` & `adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_github.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_mastodon.py` & `adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_mastodon.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py` & `adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # SPDX-FileCopyrightText: 2024 DJDevon3
 # SPDX-License-Identifier: MIT
-# Coded for Circuit Python 8.2.x
+# Coded for Circuit Python 9.x
 """OpenSky-Network.org Single Flight Private API Example"""
 
 import binascii
 import os
 import time
 
 import adafruit_connection_manager
```

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py` & `adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py` & `adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # SPDX-FileCopyrightText: 2024 DJDevon3
 # SPDX-License-Identifier: MIT
-# Coded for Circuit Python 8.2.x
-"""OpenSky-Network.org Public API Example"""
-# pylint: disable=import-error
+# Coded for Circuit Python 9.x
+"""OpenSky-Network.org Single Flight Public API Example"""
 
 import os
 import time
 
 import adafruit_connection_manager
 import wifi
 
 import adafruit_requests
 
 # No login necessary for Public API. Drastically reduced daily limit vs Private
 # OpenSky-Networks.org REST API: https://openskynetwork.github.io/opensky-api/rest.html
 # All active flights JSON: https://opensky-network.org/api/states/all PICK ONE!
 # JSON order: transponder, callsign, country
 # ACTIVE transpondes only, for multiple "c822af&icao24=cb3993&icao24=c63923"
-TRANSPONDER = "3c5ef8"
+TRANSPONDER = "88044d"
 
 # Get WiFi details, ensure these are setup in settings.toml
 ssid = os.getenv("CIRCUITPY_WIFI_SSID")
 password = os.getenv("CIRCUITPY_WIFI_PASSWORD")
-osnusername = os.getenv("OSN_USERNAME")  # Website Credentials
-osnpassword = os.getenv("OSN_PASSWORD")  # Website Credentials
 
 # API Polling Rate
 # 900 = 15 mins, 1800 = 30 mins, 3600 = 1 hour
 # OpenSky-Networks IP bans for too many requests, check rate limit.
 # https://openskynetwork.github.io/opensky-api/rest.html#limitations
 SLEEP_TIME = 1800
 
@@ -76,23 +73,24 @@
             wifi.radio.connect(ssid, password)
         except ConnectionError as e:
             print("❌ Connection Error:", e)
             print("Retrying in 10 seconds")
     print("✅ Wifi!")
 
     try:
-        print(" | Attempting to GET OpenSky-Network Single Flight JSON!")
+        print(" | Attempting to GET OpenSky-Network Single Public Flight JSON!")
+        print(" | Website Credentials NOT Required! Less daily calls than Private.")
         try:
             opensky_response = requests.get(url=OPENSKY_SOURCE)
             opensky_json = opensky_response.json()
         except ConnectionError as e:
             print("Connection Error:", e)
             print("Retrying in 10 seconds")
 
-        print(" | ✅ OpenSky-Network JSON!")
+        print(" | ✅ OpenSky-Network Public JSON!")
 
         if DEBUG:
             print("Full API GET URL: ", OPENSKY_SOURCE)
             print(opensky_json)
 
         # ERROR MESSAGE RESPONSES
         if "timestamp" in opensky_json:
```

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_premiereleague.py` & `adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_premiereleague.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py` & `adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_steam.py` & `adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_steam.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_twitch.py` & `adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_twitch.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_youtube.py` & `adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_api_youtube.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_multiple_cookies.py` & `adafruit_circuitpython_requests-3.2.5/examples/wifi/expanded/requests_wifi_multiple_cookies.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/wifi/requests_wifi_advanced.py` & `adafruit_circuitpython_requests-3.2.5/examples/wifi/requests_wifi_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/wifi/requests_wifi_simpletest.py` & `adafruit_circuitpython_requests-3.2.5/examples/wifi/requests_wifi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/wiznet5k/requests_wiznet5k_advanced.py` & `adafruit_circuitpython_requests-3.2.5/examples/wiznet5k/requests_wiznet5k_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/examples/wiznet5k/requests_wiznet5k_simpletest.py` & `adafruit_circuitpython_requests-3.2.5/examples/wiznet5k/requests_wiznet5k_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/pyproject.toml` & `adafruit_circuitpython_requests-3.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-requests"
 description = "A requests-like library for web interfacing"
-version = "3.2.4"
+version = "3.2.5"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Requests"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-requests-3.2.4/tests/chunk_test.py` & `adafruit_circuitpython_requests-3.2.5/tests/chunk_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/tests/chunked_redirect_test.py` & `adafruit_circuitpython_requests-3.2.5/tests/chunked_redirect_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/tests/concurrent_test.py` & `adafruit_circuitpython_requests-3.2.5/tests/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/tests/conftest.py` & `adafruit_circuitpython_requests-3.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/tests/header_test.py` & `adafruit_circuitpython_requests-3.2.5/tests/header_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/tests/method_test.py` & `adafruit_circuitpython_requests-3.2.5/tests/method_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/tests/mocket.py` & `adafruit_circuitpython_requests-3.2.5/tests/mocket.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/tests/parse_test.py` & `adafruit_circuitpython_requests-3.2.5/tests/parse_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/tests/protocol_test.py` & `adafruit_circuitpython_requests-3.2.5/tests/protocol_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/tests/reuse_test.py` & `adafruit_circuitpython_requests-3.2.5/tests/reuse_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.4/tox.ini` & `adafruit_circuitpython_requests-3.2.5/tox.ini`

 * *Files identical despite different names*

