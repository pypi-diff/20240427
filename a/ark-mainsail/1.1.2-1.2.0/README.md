# Comparing `tmp/ark-mainsail-1.1.2.tar.gz` & `tmp/ark-mainsail-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ark-mainsail-1.1.2.tar", last modified: Wed Apr 24 18:09:41 2024, max compression
+gzip compressed data, was "ark-mainsail-1.2.0.tar", last modified: Sat Apr 27 07:08:31 2024, max compression
```

## Comparing `ark-mainsail-1.1.2.tar` & `ark-mainsail-1.2.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 18:09:41.944076 ark-mainsail-1.1.2/
--rw-rw-rw-   0        0        0     1063 2024-03-31 14:12:30.000000 ark-mainsail-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     4281 2024-04-24 18:09:41.942081 ark-mainsail-1.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 18:09:41.940087 ark-mainsail-1.1.2/ark_mainsail.egg-info/
--rw-rw-rw-   0        0        0     4281 2024-04-24 18:09:41.000000 ark-mainsail-1.1.2/ark_mainsail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      936 2024-04-24 18:09:41.000000 ark-mainsail-1.1.2/ark_mainsail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 18:09:41.000000 ark-mainsail-1.1.2/ark_mainsail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-24 18:09:41.000000 ark-mainsail-1.1.2/ark_mainsail.egg-info/requires.txt
--rw-rw-rw-   0        0        0       40 2024-04-24 18:09:41.000000 ark-mainsail-1.1.2/ark_mainsail.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-24 18:09:41.907174 ark-mainsail-1.1.2/mainsail/
--rw-rw-rw-   0        0        0     1924 2024-04-13 21:52:02.000000 ark-mainsail-1.1.2/mainsail/__init__.py
--rw-rw-rw-   0        0        0      961 2024-04-07 19:01:11.000000 ark-mainsail-1.1.2/mainsail/config.py
--rw-rw-rw-   0        0        0     1585 2024-03-31 14:12:31.000000 ark-mainsail-1.1.2/mainsail/deserializer.py
--rw-rw-rw-   0        0        0     9663 2024-04-07 05:49:52.000000 ark-mainsail-1.1.2/mainsail/identity.py
--rw-rw-rw-   0        0        0     5204 2024-04-21 15:46:24.000000 ark-mainsail-1.1.2/mainsail/rest.py
--rw-rw-rw-   0        0        0     1884 2024-03-31 14:12:31.000000 ark-mainsail-1.1.2/mainsail/serializer.py
--rw-rw-rw-   0        0        0     9397 2024-04-21 10:35:01.000000 ark-mainsail-1.1.2/mainsail/transaction.py
-drwxrwxrwx   0        0        0        0 2024-04-24 18:09:41.911163 ark-mainsail-1.1.2/mainsail/tx/
--rw-rw-rw-   0        0        0     1424 2024-04-07 15:25:42.000000 ark-mainsail-1.1.2/mainsail/tx/__init__.py
--rw-rw-rw-   0        0        0     7080 2024-04-13 15:44:25.000000 ark-mainsail-1.1.2/mainsail/tx/v1.py
--rw-rw-rw-   0        0        0     5013 2024-04-21 15:08:34.000000 ark-mainsail-1.1.2/mainsail/webhook.py
-drwxrwxrwx   0        0        0        0 2024-04-24 18:09:41.929120 ark-mainsail-1.1.2/pool/
--rw-rw-rw-   0        0        0     4840 2024-04-24 08:02:47.000000 ark-mainsail-1.1.2/pool/__init__.py
--rw-rw-rw-   0        0        0     5358 2024-04-23 19:26:57.000000 ark-mainsail-1.1.2/pool/__main__.py
--rw-rw-rw-   0        0        0     1251 2024-04-24 08:02:26.000000 ark-mainsail-1.1.2/pool/api.py
--rw-rw-rw-   0        0        0    11508 2024-04-24 18:05:21.000000 ark-mainsail-1.1.2/pool/biom.py
--rw-rw-rw-   0        0        0     9519 2024-04-24 05:58:10.000000 ark-mainsail-1.1.2/pool/tbw.py
--rw-rw-rw-   0        0        0       42 2024-04-24 18:09:41.944076 ark-mainsail-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1599 2024-04-24 09:12:19.000000 ark-mainsail-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 18:09:41.937094 ark-mainsail-1.1.2/test/
--rw-rw-rw-   0        0        0       25 2024-04-01 18:54:30.000000 ark-mainsail-1.1.2/test/__init__.py
--rw-rw-rw-   0        0        0     1765 2024-04-06 14:10:01.000000 ark-mainsail-1.1.2/test/test_identity.py
--rw-rw-rw-   0        0        0     3635 2024-04-20 11:21:27.000000 ark-mainsail-1.1.2/test/test_v1_builders.py
+drwxrwxrwx   0        0        0        0 2024-04-27 07:08:31.627492 ark-mainsail-1.2.0/
+-rw-rw-rw-   0        0        0     1063 2024-03-31 14:12:30.000000 ark-mainsail-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4681 2024-04-27 07:08:31.625497 ark-mainsail-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3409 2024-04-27 06:46:21.000000 ark-mainsail-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 07:08:31.623507 ark-mainsail-1.2.0/ark_mainsail.egg-info/
+-rw-rw-rw-   0        0        0     4681 2024-04-27 07:08:30.000000 ark-mainsail-1.2.0/ark_mainsail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2024-04-27 07:08:30.000000 ark-mainsail-1.2.0/ark_mainsail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 07:08:30.000000 ark-mainsail-1.2.0/ark_mainsail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-27 07:08:30.000000 ark-mainsail-1.2.0/ark_mainsail.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2024-04-27 07:08:30.000000 ark-mainsail-1.2.0/ark_mainsail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-27 07:08:30.000000 ark-mainsail-1.2.0/ark_mainsail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 07:08:31.314906 ark-mainsail-1.2.0/mainsail/
+-rw-rw-rw-   0        0        0     1924 2024-04-13 21:52:02.000000 ark-mainsail-1.2.0/mainsail/__init__.py
+-rw-rw-rw-   0        0        0      961 2024-04-07 19:01:11.000000 ark-mainsail-1.2.0/mainsail/config.py
+-rw-rw-rw-   0        0        0     1585 2024-03-31 14:12:31.000000 ark-mainsail-1.2.0/mainsail/deserializer.py
+-rw-rw-rw-   0        0        0     9841 2024-04-24 20:18:46.000000 ark-mainsail-1.2.0/mainsail/identity.py
+-rw-rw-rw-   0        0        0     5208 2024-04-27 05:59:41.000000 ark-mainsail-1.2.0/mainsail/rest.py
+-rw-rw-rw-   0        0        0     1884 2024-03-31 14:12:31.000000 ark-mainsail-1.2.0/mainsail/serializer.py
+-rw-rw-rw-   0        0        0     9397 2024-04-21 10:35:01.000000 ark-mainsail-1.2.0/mainsail/transaction.py
+drwxrwxrwx   0        0        0        0 2024-04-27 07:08:31.363258 ark-mainsail-1.2.0/mainsail/tx/
+-rw-rw-rw-   0        0        0     1424 2024-04-07 15:25:42.000000 ark-mainsail-1.2.0/mainsail/tx/__init__.py
+-rw-rw-rw-   0        0        0     7119 2024-04-25 06:54:53.000000 ark-mainsail-1.2.0/mainsail/tx/v1.py
+-rw-rw-rw-   0        0        0     5052 2024-04-24 20:10:37.000000 ark-mainsail-1.2.0/mainsail/webhook.py
+drwxrwxrwx   0        0        0        0 2024-04-27 07:08:31.521772 ark-mainsail-1.2.0/mnsl_pool/
+-rw-rw-rw-   0        0        0     5235 2024-04-26 07:11:22.000000 ark-mainsail-1.2.0/mnsl_pool/__init__.py
+-rw-rw-rw-   0        0        0     5363 2024-04-26 07:11:10.000000 ark-mainsail-1.2.0/mnsl_pool/__main__.py
+-rw-rw-rw-   0        0        0     1237 2024-04-26 07:11:15.000000 ark-mainsail-1.2.0/mnsl_pool/api.py
+-rw-rw-rw-   0        0        0    12503 2024-04-27 05:24:23.000000 ark-mainsail-1.2.0/mnsl_pool/biom.py
+-rw-rw-rw-   0        0        0     9468 2024-04-25 19:54:38.000000 ark-mainsail-1.2.0/mnsl_pool/tbw.py
+-rw-rw-rw-   0        0        0       42 2024-04-27 07:08:31.627492 ark-mainsail-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1993 2024-04-26 17:46:53.000000 ark-mainsail-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 07:08:31.578691 ark-mainsail-1.2.0/test/
+-rw-rw-rw-   0        0        0       25 2024-04-01 18:54:30.000000 ark-mainsail-1.2.0/test/__init__.py
+-rw-rw-rw-   0        0        0     1765 2024-04-06 14:10:01.000000 ark-mainsail-1.2.0/test/test_identity.py
+-rw-rw-rw-   0        0        0     3635 2024-04-20 11:21:27.000000 ark-mainsail-1.2.0/test/test_v1_builders.py
```

### Comparing `ark-mainsail-1.1.2/LICENSE` & `ark-mainsail-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.2/PKG-INFO` & `ark-mainsail-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ark-mainsail
-Version: 1.1.2
-Summary: Interact with ARK blockchain and forks
+Version: 1.2.0
+Summary: Interact with ARK blockchain trough mainsail framework
 Home-page: https://github.com/Moustikitos/python-mainsail
 Author: Toons
 Author-email: moustikitos@gmail.com
 Maintainer: Toons
 Maintainer-email: moustikitos@gmail.com
 License: Copyright 2024, MIT licence
 Project-URL: Bug Reports, https://github.com/Moustikitos/python-mainsail/issues
@@ -19,24 +19,24 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: base58
-Requires-Dist: pyaes
-Requires-Dist: blspy
-Requires-Dist: cSecp256k1
+Requires-Dist: requests==2.31.0
+Requires-Dist: base58==2.1.1
+Requires-Dist: pyaes==1.6.1
+Requires-Dist: blspy==2.0.3
+Requires-Dist: cSecp256k1==1.1.2
 
 # python-mainsail
 
-This package aims to provide a simple implementation to bake offline `Ark`
-transaction and interact with the blockchain API.
+This package provides a simple implementation to interact with `Ark` blockchain
+API and managment tools for validators aiming to run a pool.
 
 ```python
 >>> from mainsail.tx.v1 import Transfer
 >>> from mainsail import rest
 >>> # http://xxx.xxx.xxx.xxx:4006/api/wallets/toons
 >>> wallet = rest.GET.api.wallets.toons()
 >>> wallet["address"]
@@ -51,51 +51,25 @@
 >>> t = Transfer(1, 'D5Ha4o3UTuTd59vjDw1F26mYhaRdXh7YPv', 'message \U0001f919')
 >>> t.sign()
 Type or paste your passphrase >
 >>> t.send()
 {'data': {'accept': [0], 'broadcast': [0], 'excess': [], 'invalid': []}}
 ```
 
-## Validator pool managment tool
+## Linux distributions
 
-Install and deploy server:
-
-```bash
-~$ wget https://raw.githubusercontent.com/Moustikitos/python-mainsail/master/mnsl-pool.sh
-~$ bash mnsl-pool.sh
-~$ mnsl_pool_deploy
-```
-
-Add delegate:
-
-```bash
-~$ add_validator 02968e862011738ac185e87f47dec61b32c842fd8e24fab625c02a15ad7e2d0f65
-Type or paste your passphrase>
-enter pin code to secure secret>
-provide a valid network peer> http://127.0.0.1:4003
-provide a valid webhook peer> http://127.0.0.1:4004
-provide a valid target endpoint> http://127.0.0.1:5000/block/forged
-```
-
-Check the logs:
-
-```bash
-~$ log_mnsl_pool
-~$ log_mnsl_bg
-```
-
-## [RIPEMD160 issue with OpenSSL v>=3](https://github.com/openssl/openssl/issues/16994) on ubuntu
-
-Get the installation folder:
+Due to [RIPEMD160 issue with OpenSSL v>=3](https://github.com/openssl/openssl/issues/16994)
+`hashlib.ripemd160` is disabled within `python3`. To enable it back, get the
+installation folder...
 
 ```bash
 openssl version -d
 ```
 
-Make sure that the openssl config file contains following lines:
+... and make sure that the openssl config file contains following lines:
 
 ```conf
 openssl_conf = openssl_init
 
 [openssl_init]
 providers = provider_sect
 
@@ -106,30 +80,74 @@
 [default_sect]
 activate = 1
 
 [legacy_sect]
 activate = 1
 ```
 
+## Validator pool managment tools
+
+### Ubuntu installation
+
+First read [installation script](https://bit.ly/3U6BI8v), then:
+
+```bash
+~$ bash <(wget -qO- https://bit.ly/3U6BI8v)
+```
+
+### Deploy pool server
+
+```bash
+~$ mnsl_deploy # use ip address 0.0.0.0 with  port #5000
+```
+
+If you plan to deploy pool server behind a proxy, it is possible to customize
+`ip` and `port`:
+
+```bash
+~$ mnsl_deploy host=127.0.0.1 port=7542 # use localhost address with port #7542
+```
+
+Setup a pool using validator public key:
+
+```bash
+~$ add_pool puk=02968e862011738ac185e87f47dec61b32c842fd8e24fab625c02a15ad7e2d0f65
+```
+
+Configure pool options:
+
+```bash
+~$ set_pool ?key=value?
+```
+
+Check the logs:
+
+```bash
+~$ log_mnsl_pool
+~$ log_mnsl_bg
+```
+
 ## Available transactions
 
 * [x] Transfer
 * [x] ValidatorRegistration
 * [x] Vote
 * [x] MultiSignature
 * [x] MultiPayment
 * [x] ValidatorResignation
 * [x] UsernameRegistration
 * [x] UsernameResignation
 
 ## Features
 
-* [x] pool server with remote managment tool
 * [x] secured private keys storage
 * [x] secured webhook subscriptions storage
 * [x] offline network configuration available
+* [x] pool server with remote managment tool
+* [x] `cmd` command line `set_validator` for windows platform
+* [x] pool installation and update using pip
 
 ## Support this project
 
 <!-- [![Liberapay receiving](https://img.shields.io/liberapay/goal/Toons?logo=liberapay)](https://liberapay.com/Toons/donate) -->
 [![Paypal me](https://img.shields.io/badge/PayPal-toons-00457C?logo=paypal&logoColor=white)](https://paypal.me/toons)
 [![Bitcoin](https://img.shields.io/badge/Donate-bc1q6aqr0hfq6shwlaux8a7ydvncw53lk2zynp277x-ff9900?logo=bitcoin)](https://github.com/Moustikitos/python-mainsail/blob/master/docs/img/bc1q6aqr0hfq6shwlaux8a7ydvncw53lk2zynp277x.png)
```

### Comparing `ark-mainsail-1.1.2/ark_mainsail.egg-info/PKG-INFO` & `ark-mainsail-1.2.0/ark_mainsail.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ark-mainsail
-Version: 1.1.2
-Summary: Interact with ARK blockchain and forks
+Version: 1.2.0
+Summary: Interact with ARK blockchain trough mainsail framework
 Home-page: https://github.com/Moustikitos/python-mainsail
 Author: Toons
 Author-email: moustikitos@gmail.com
 Maintainer: Toons
 Maintainer-email: moustikitos@gmail.com
 License: Copyright 2024, MIT licence
 Project-URL: Bug Reports, https://github.com/Moustikitos/python-mainsail/issues
@@ -19,24 +19,24 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: base58
-Requires-Dist: pyaes
-Requires-Dist: blspy
-Requires-Dist: cSecp256k1
+Requires-Dist: requests==2.31.0
+Requires-Dist: base58==2.1.1
+Requires-Dist: pyaes==1.6.1
+Requires-Dist: blspy==2.0.3
+Requires-Dist: cSecp256k1==1.1.2
 
 # python-mainsail
 
-This package aims to provide a simple implementation to bake offline `Ark`
-transaction and interact with the blockchain API.
+This package provides a simple implementation to interact with `Ark` blockchain
+API and managment tools for validators aiming to run a pool.
 
 ```python
 >>> from mainsail.tx.v1 import Transfer
 >>> from mainsail import rest
 >>> # http://xxx.xxx.xxx.xxx:4006/api/wallets/toons
 >>> wallet = rest.GET.api.wallets.toons()
 >>> wallet["address"]
@@ -51,51 +51,25 @@
 >>> t = Transfer(1, 'D5Ha4o3UTuTd59vjDw1F26mYhaRdXh7YPv', 'message \U0001f919')
 >>> t.sign()
 Type or paste your passphrase >
 >>> t.send()
 {'data': {'accept': [0], 'broadcast': [0], 'excess': [], 'invalid': []}}
 ```
 
-## Validator pool managment tool
+## Linux distributions
 
-Install and deploy server:
-
-```bash
-~$ wget https://raw.githubusercontent.com/Moustikitos/python-mainsail/master/mnsl-pool.sh
-~$ bash mnsl-pool.sh
-~$ mnsl_pool_deploy
-```
-
-Add delegate:
-
-```bash
-~$ add_validator 02968e862011738ac185e87f47dec61b32c842fd8e24fab625c02a15ad7e2d0f65
-Type or paste your passphrase>
-enter pin code to secure secret>
-provide a valid network peer> http://127.0.0.1:4003
-provide a valid webhook peer> http://127.0.0.1:4004
-provide a valid target endpoint> http://127.0.0.1:5000/block/forged
-```
-
-Check the logs:
-
-```bash
-~$ log_mnsl_pool
-~$ log_mnsl_bg
-```
-
-## [RIPEMD160 issue with OpenSSL v>=3](https://github.com/openssl/openssl/issues/16994) on ubuntu
-
-Get the installation folder:
+Due to [RIPEMD160 issue with OpenSSL v>=3](https://github.com/openssl/openssl/issues/16994)
+`hashlib.ripemd160` is disabled within `python3`. To enable it back, get the
+installation folder...
 
 ```bash
 openssl version -d
 ```
 
-Make sure that the openssl config file contains following lines:
+... and make sure that the openssl config file contains following lines:
 
 ```conf
 openssl_conf = openssl_init
 
 [openssl_init]
 providers = provider_sect
 
@@ -106,30 +80,74 @@
 [default_sect]
 activate = 1
 
 [legacy_sect]
 activate = 1
 ```
 
+## Validator pool managment tools
+
+### Ubuntu installation
+
+First read [installation script](https://bit.ly/3U6BI8v), then:
+
+```bash
+~$ bash <(wget -qO- https://bit.ly/3U6BI8v)
+```
+
+### Deploy pool server
+
+```bash
+~$ mnsl_deploy # use ip address 0.0.0.0 with  port #5000
+```
+
+If you plan to deploy pool server behind a proxy, it is possible to customize
+`ip` and `port`:
+
+```bash
+~$ mnsl_deploy host=127.0.0.1 port=7542 # use localhost address with port #7542
+```
+
+Setup a pool using validator public key:
+
+```bash
+~$ add_pool puk=02968e862011738ac185e87f47dec61b32c842fd8e24fab625c02a15ad7e2d0f65
+```
+
+Configure pool options:
+
+```bash
+~$ set_pool ?key=value?
+```
+
+Check the logs:
+
+```bash
+~$ log_mnsl_pool
+~$ log_mnsl_bg
+```
+
 ## Available transactions
 
 * [x] Transfer
 * [x] ValidatorRegistration
 * [x] Vote
 * [x] MultiSignature
 * [x] MultiPayment
 * [x] ValidatorResignation
 * [x] UsernameRegistration
 * [x] UsernameResignation
 
 ## Features
 
-* [x] pool server with remote managment tool
 * [x] secured private keys storage
 * [x] secured webhook subscriptions storage
 * [x] offline network configuration available
+* [x] pool server with remote managment tool
+* [x] `cmd` command line `set_validator` for windows platform
+* [x] pool installation and update using pip
 
 ## Support this project
 
 <!-- [![Liberapay receiving](https://img.shields.io/liberapay/goal/Toons?logo=liberapay)](https://liberapay.com/Toons/donate) -->
 [![Paypal me](https://img.shields.io/badge/PayPal-toons-00457C?logo=paypal&logoColor=white)](https://paypal.me/toons)
 [![Bitcoin](https://img.shields.io/badge/Donate-bc1q6aqr0hfq6shwlaux8a7ydvncw53lk2zynp277x-ff9900?logo=bitcoin)](https://github.com/Moustikitos/python-mainsail/blob/master/docs/img/bc1q6aqr0hfq6shwlaux8a7ydvncw53lk2zynp277x.png)
```

### Comparing `ark-mainsail-1.1.2/mainsail/__init__.py` & `ark-mainsail-1.2.0/mainsail/__init__.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.2/mainsail/config.py` & `ark-mainsail-1.2.0/mainsail/config.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.2/mainsail/deserializer.py` & `ark-mainsail-1.2.0/mainsail/deserializer.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.2/mainsail/identity.py` & `ark-mainsail-1.2.0/mainsail/identity.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,19 @@
     >>> signer.verify(puk, "simple message", sig)
     True
     >>> type(signer)  # bcrypto 4.10 specification used
     <class 'mainsail.identity.Bcrpt410'>
     ```
     """
 
+    @staticmethod
+    def path(pin: Union[bytes, List[int]]) -> str:
+        code = binascii.hexlify(bytes(pin))
+        return _encryption_file_path(code.decode("utf-8"))
+
     def dump(self, pin: Union[bytes, List[int]]) -> None:
         """
         Securely dump `KeyRing` into filesystem using pin code. Override
         existing file if any.
 
         Args:
             pin (bytes|List[int]): pin code used to _encrypt KeyRing. Pin code
```

### Comparing `ark-mainsail-1.1.2/mainsail/rest.py` & `ark-mainsail-1.2.0/mainsail/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from mainsail import config
 from urllib.parse import urlencode, urlparse, urlunparse
 from collections import namedtuple
 
 # namedtuple to match the internal signature of urlunparse
 Urltuple = namedtuple(
     typename='Urltuple', field_names=[
-        'scheme', 'netloc', 'url', 'path', 'query', 'fragment'
+        'scheme', 'netloc', 'path', 'params', 'query', 'fragment'
     ]
 )
 
 
 class ApiError(Exception):
     pass
 
@@ -77,15 +77,15 @@
             # default -> http://127.0.0.1:5000
             base_url = Urltuple(
                 'http',
                 f"{peer.get('ip', '127.0.0.1')}:" +
                 f"{peer.get('ports', {}).get(ports[0], 5000)}",
                 None, None, None, None
             )
-        base_url = base_url._replace(url='/'.join((self.path,) + path))
+        base_url = base_url._replace(path='/'.join((self.path,) + path))
         if self.func in (requests.post, requests.delete):
             resp = self.func(urlunparse(base_url), headers=headers, json=data)
         else:
             base_url = base_url._replace(query=urlencode(data))
             resp = self.func(urlunparse(base_url), headers=headers)
 
         try:
```

### Comparing `ark-mainsail-1.1.2/mainsail/serializer.py` & `ark-mainsail-1.2.0/mainsail/serializer.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.2/mainsail/transaction.py` & `ark-mainsail-1.2.0/mainsail/transaction.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.2/mainsail/tx/__init__.py` & `ark-mainsail-1.2.0/mainsail/tx/__init__.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.2/mainsail/tx/v1.py` & `ark-mainsail-1.2.0/mainsail/tx/v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     "Transfer", "ValidatorRegistration", "ValidatorResignation",
     "UsernameRegistration", "UsernameResignation", "Vote", "MultiPayment",
     "MultiSignature"
 ]
 
 
 class Transfer(Transaction):
+    """
+    TODO: write doc
+    """
 
     def __init__(
         self, amount: float, recipientId: str,
         vendorField: Union[str, bytes] = None
     ) -> None:
         try:
             base58.b58decode_check(recipientId)
```

### Comparing `ark-mainsail-1.1.2/mainsail/webhook.py` & `ark-mainsail-1.2.0/mainsail/webhook.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,15 +127,18 @@
     else:
         token = authorization + data["verification"]
         return \
             hashlib.sha256(token.encode("utf-8")).hexdigest() == data["hash"]
 
 
 def list() -> list:
-    return [name for name in next(os.walk(DATA))[-1] if name.endswith(".json")]
+    return [
+        name.split(".")[0] for name in next(os.walk(DATA))[-1]
+        if name.endswith(".json")
+    ]
 
 
 def open(whk_id: str) -> dict:
     return loadJson(os.path.join(DATA, whk_id + ".json"))
 
 
 def unsubscribe(whk_id: str) -> dict:
```

### Comparing `ark-mainsail-1.1.2/pool/__init__.py` & `ark-mainsail-1.2.0/mnsl_pool/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,35 +10,34 @@
 ```bash
 wget https://bit.ly/3U6BI8v
 bash mnsl-pool.sh
 ```
 
 Setup script creates 7 commands into `~/.bash_aliases` file:
 
-* [x] `mnsl_pool_deploy` takes broadcast ip address and port to create
+* [x] `mnsl_deploy` takes broadcast ip address and port to create
   services managed by `systemd`.
-* [x] `add_validator` takes a validator public key to configure listening
+* [x] `add_pool` takes a validator public key to configure listening
   subscription on blockchain.
-* [x] `set_validator` modifies validator TBW service parameters.
-* [x] `mnsl_venv_activate` activates the virtual environment used to run
+* [x] `set_pool` modifies validator TBW pool service parameters.
+* [x] `mnsl_venv` activates the virtual environment used to run
   mainsail pool.
-* [x] `restart_mnsl_pool` restarts the server.
-* [x] `restart_mnsl_bg` restarts background tasks.
+* [x] `mnsl_restart` restarts pool tasks.
 * [x] `log_mnsl_pool` shows server logs.
 * [x] `log_mnsl_bg` shows background tasks logs.
 """
 
 import os
 import json
 import queue
 import flask
 import logging
 
 from mainsail import webhook, loadJson, dumpJson
-from pool import tbw, biom
+from mnsl_pool import tbw, biom
 
 # set basic logging
 logging.basicConfig()
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.DEBUG)
 
 CONF_PARAMETERS = [
@@ -82,33 +81,45 @@
             )
             dumpJson(conf, path, ensure_ascii=False)
             return flask.jsonify({"status": 204}), 200
     else:
         return flask.jsonify({"status": 403}), 200
 
 
-@app.route("/configure/delegate", methods=["POST"])
-def configure_delegate() -> flask.Response:
+@app.route("/pool/configure", methods=["POST"])
+def pool_configure() -> flask.Response:
+    """
+    Flask endpoint to configure validator pool parameters. Requests are secured
+    using validator signature on UTC-time-based nonce. Available parameters are
+    set in `pool.biom:DELEGATE_PARAMETERS` dict.
+
+    This end point is used by `set_pool` command.
+    """
+
     if biom.check_headers(flask.request.headers):
         puk = flask.request.headers["puk"]
         path = os.path.join(tbw.DATA, f"{puk}.json")
         data = json.loads(flask.request.data)
+        # BUGFIX: when used directly on server where pool is runing, the
+        # headers seem to be copied into request data...
+        data.pop("headers", False)
+        ##########################
         info = dict(
             loadJson(path), **dict(
                 [k, v] for k, v in data.items()
                 if k in biom.DELEGATE_PARAMETERS.keys()
             )
         )
         if flask.request.method == "POST":
             LOGGER.debug(f"---- received> {data}")
             LOGGER.info(f"updating {puk} info> {info}")
             dumpJson(info, path, ensure_ascii=False)
-            return flask.jsonify({"status": 204, "updated": data}), 200
+            return flask.jsonify({"status": 204, "updated": data})
     else:
-        return flask.jsonify({"status": 403}), 200
+        return flask.jsonify({"status": 403})
 
 
 @app.route("/block/forged", methods=["POST", "GET"])
 def block_forged() -> flask.Response:
     check = False
     if flask.request.method == "POST":
         check = webhook.verify(
@@ -118,15 +129,15 @@
         if check is True and flask.request.data != b'':
             data = json.loads(flask.request.data)
             block = data.get("data", {}).get("block", {}).get("data", {})
             LOGGER.debug("block received> %s", block)
             JOB.put(block)
         else:
             check = False
-    return flask.jsonify({"acknowledge": check}), 200
+    return flask.jsonify({"acknowledge": check})
 
 
 def main():
     """
     Server main loop ran as a `threading.Thread` target. It gets block
     passed by `block_forged` (`/block/forged` endpoint) and update forgery
     of validator issuing the block.
```

### Comparing `ark-mainsail-1.1.2/pool/__main__.py` & `ark-mainsail-1.2.0/mnsl_pool/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import time
 import queue
 import binascii
 import threading
 
 from mainsail import rest, identity
-from pool import tbw, biom, loadJson, dumpJson, LOGGER
+from mnsl_pool import tbw, biom, loadJson, dumpJson, LOGGER
 
 TASK = queue.Queue()
 SLEEP = threading.Event()
 
 
 def payroll():
     while True:
```

### Comparing `ark-mainsail-1.1.2/pool/api.py` & `ark-mainsail-1.2.0/mnsl_pool/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # -*- coding: utf-8 -*-
 
 import os
 import threading
 
-from pool import tbw, flask, loadJson, main, app, JOB
+from mnsl_pool import tbw, flask, loadJson, main, app, JOB
 
 
 @app.route("/<string:puk>", methods=["GET"])
-def delegate(puk: str) -> flask.Response:
+def validator(puk: str) -> flask.Response:
     info = loadJson(os.path.join(tbw.DATA, f"{puk}.json"))
     if len(info):
         info.pop("prk", False)
-        return flask.jsonify(info), 200
-    return flask.jsonify({"status": 404}), 200
+        return flask.jsonify(info)
+    return flask.jsonify({"status": 404})
 
 
 @app.route("/<string:puk>/forgery", methods=["GET"])
 def forgery(puk: str) -> flask.Response:
     path = os.path.join(tbw.DATA, puk, "forgery.json")
     if os.path.exists(path):
         forgery = loadJson(path)
         forgery.pop("reward", False)
         for k in forgery:
             if k not in ["blocks", "contributions"]:
                 forgery[k] /= tbw.XTOSHI
         for k in forgery.get("contributions", {}):
             forgery["contributions"][k] /= tbw.XTOSHI
-        return flask.jsonify(forgery), 200
-    return flask.jsonify({"status": 404}), 200
+        return flask.jsonify(forgery)
+    return flask.jsonify({"status": 404})
 
 
 def run(debug: bool = True) -> flask.Flask:
     global app, MAIN
 
     MAIN = threading.Thread(target=main)
     MAIN.daemon = True
```

### Comparing `ark-mainsail-1.1.2/pool/biom.py` & `ark-mainsail-1.2.0/mnsl_pool/biom.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import getpass
 import logging
 import datetime
 import requests
 
 from datetime import timezone
 from urllib import parse
-from pool import tbw
+from mnsl_pool import tbw
 from mainsail import identity, rest, webhook, dumpJson, loadJson
 from typing import Union, List
 
 # set basic logging
 logging.basicConfig()
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.DEBUG)
@@ -81,14 +81,63 @@
         LOGGER.info("global lock released")
 
 
 class IdentityError(Exception):
     pass
 
 
+def _merge_options(**options):
+    # update from command line
+    for arg in [a for a in sys.argv if "=" in a]:
+        key, value = arg.split("=")
+        key = key.replace("--", "").replace("-", "_")
+        options[key] = value
+    # manage parameters
+    params = {}
+    for key, value in options.items():
+        if key == "port":
+            try:
+                params[key] = int(value)
+            except Exception:
+                LOGGER.info(
+                    f"conversion into {type(0)} impossible for {value}"
+                )
+        elif key == "wallet":
+            try:
+                base58.b58decode_check(value)
+            except Exception:
+                LOGGER.info(f"{value} is not a valid wallet address")
+            else:
+                params[key] = value
+        elif key == "excludes":
+            addresses = []
+            for address in [
+                addr.strip() for addr in value.split(",") if addr != ""
+            ]:
+                try:
+                    base58.b58decode_check(address)
+                except Exception:
+                    LOGGER.info(f"{address} is not a valid wallet address")
+                else:
+                    addresses.append(address)
+            params[key] = addresses
+        elif key in DELEGATE_PARAMETERS.keys():
+            try:
+                params[key] = DELEGATE_PARAMETERS[key](value)
+            except Exception:
+                LOGGER.info(
+                    f"conversion into {DELEGATE_PARAMETERS[key]} "
+                    f"impossible for {value}"
+                )
+        else:
+            params[key] = value
+    LOGGER.info(f"grabed options: {params}")
+    return params
+
+
 def get_nonces():
     base_time = math.ceil(time.time()/5) * 5
     datetimes = [
         datetime.datetime.fromtimestamp(base_time + n)
         .astimezone(timezone.utc).strftime("%Y-%m-%H%m%S").encode("utf-8")
         for n in [-5, 0]
     ]
@@ -113,21 +162,21 @@
         puk=prk.puk().encode()
     )
     return headers
 
 
 def check_headers(headers: dict) -> bool:
     try:
-        path = os.path.join(tbw.DATA, f"{headers['puk']}.json")
+        path = os.path.join(tbw.DATA, f"{headers['puk']}")
         valid_nonces = get_nonces()
         LOGGER.debug(
             f"---- received nonce {headers['nonce']} - "
             f"valid nonces: {'|'.join(valid_nonces)}"
         )
-        if os.path.exists(path) and headers["nonce"] in valid_nonces:
+        if os.path.isdir(path) and headers["nonce"] in valid_nonces:
             return identity.get_signer().verify(
                 headers["puk"], headers["nonce"], headers["sig"]
             )
     except KeyError:
         pass
     return False
 
@@ -141,27 +190,31 @@
     if data is None:
         return endpoint(peer=peer)
     else:
         return endpoint(data=data, peer=peer)
 
 
 def deploy(host: str = "127.0.0.1", port: int = 5000):
+    options = _merge_options()
+    host = options.get("host", host)
+    port = options.get("port", host)
+
     normpath = os.path.normpath
     executable = normpath(sys.executable)
 
-    with io.open("./mnsl-pool.service", "w") as unit:
+    with io.open("./mnsl-srv.service", "w") as unit:
         unit.write(f"""[Unit]
 Description=Mainsail TBW server
 After=network.target
 
 [Service]
 User={os.environ.get('USER', 'unknown')}
 WorkingDirectory={normpath(sys.prefix)}
-Environment=PYTHONPATH={normpath(os.path.dirname(os.path.dirname(__file__)))}
-ExecStart={os.path.dirname(executable)}/gunicorn 'pool.api:run(debug=False)' \
+ExecStart={os.path.dirname(executable)}/gunicorn \
+'mnsl_pool.api:run(debug=False)' \
 --bind={host}:{port} --workers=2 --timeout 10 --access-logfile -
 Restart=always
 
 [Install]
 WantedBy=multi-user.target
 """)
 
@@ -170,86 +223,42 @@
 Description=Mainsail pool backround tasks
 After=network.target
 
 [Service]
 User={os.environ.get("USER", "unknown")}
 WorkingDirectory={normpath(sys.prefix)}
 Environment=PYTHONPATH={normpath(os.path.dirname(os.path.dirname(__file__)))}
-ExecStart={normpath(sys.executable)} -m pool --workers=1 --access-logfile -
+ExecStart={normpath(sys.executable)} -m mnsl_pool \
+--workers=1 --access-logfile -
 Restart=always
 
 [Install]
 WantedBy=multi-user.target
 """)
 
     if os.system(f"{executable} -m pip show gunicorn") != "0":
         os.system(f"{executable} -m pip install gunicorn")
 
-    os.system("chmod +x ./mnsl-pool.service")
+    os.system("chmod +x ./mnsl-srv.service")
     os.system("chmod +x ./mnsl-bg.service")
-    os.system("sudo mv --force ./mnsl-pool.service /etc/systemd/system")
+    os.system("sudo mv --force ./mnsl-srv.service /etc/systemd/system")
     os.system("sudo mv --force ./mnsl-bg.service /etc/systemd/system")
 
     os.system("sudo systemctl daemon-reload")
-    if not os.system("sudo systemctl restart mnsl-pool"):
-        os.system("sudo systemctl start mnsl-pool")
+    if not os.system("sudo systemctl restart mnsl-srv"):
+        os.system("sudo systemctl start mnsl-srv")
     if not os.system("sudo systemctl restart mnsl-bg"):
         os.system("sudo systemctl start mnsl-bg")
 
 
-def _merge_options(**options):
-    # update from command line
-    for arg in [a for a in sys.argv if "=" in a]:
-        key, value = arg.split("=")
-        key = key.replace("--", "").replace("-", "_")
-        options[key] = value
-    # manage parameters
-    params = {}
-    for key, value in options.items():
-        if key == "port":
-            try:
-                params[key] = int(value)
-            except Exception:
-                LOGGER.info(
-                    f"conversion into {type(0)} impossible for {value}"
-                )
-        elif key == "wallet":
-            try:
-                base58.b58decode_check(value)
-            except Exception:
-                LOGGER.info(f"{value} is not a valid wallet address")
-            else:
-                params[key] = value
-        elif key == "excludes":
-            addresses = []
-            for address in [
-                addr.strip() for addr in value.split(",") if addr != ""
-            ]:
-                try:
-                    base58.b58decode_check(address)
-                except Exception:
-                    LOGGER.info(f"{address} is not a valid wallet address")
-                else:
-                    addresses.append(address)
-            params[key] = addresses
-        elif key in DELEGATE_PARAMETERS.keys():
-            try:
-                params[key] = DELEGATE_PARAMETERS[key](value)
-            except Exception:
-                LOGGER.info(
-                    f"conversion into {DELEGATE_PARAMETERS[key]} "
-                    f"impossible for {value}"
-                )
-        else:
-            params[key] = value
-    LOGGER.info(f"grabed options: {params}")
-    return params
-
-
-def add_delegate(puk: str, **kwargs) -> None:
+def add_pool(**kwargs) -> None:
+    options = _merge_options()
+    puk = options.get("puk", None)
+    if puk is None:
+        raise IdentityError("no pulic key provided")
     # check identity
     prk = identity.KeyRing.create(kwargs.pop("prk", None))
     if prk.puk().encode() != puk:
         raise IdentityError(f"private key does not match public key {puk}")
     # secure private key using a pincode
     # it will give the possibility to mnsl-bg service to sign transactions
     answer = ""
@@ -268,14 +277,15 @@
             )
         except KeyboardInterrupt:
             print("\n")
             break
         except Exception as error:
             LOGGER.info("%r", error)
             pass
+    options["username"] = rest.GET.api.wallets(puk).get("username", None)
     # reach a valid subscription node
     webhook_peer = None
     while webhook_peer is None:
         webhook_peer = input(
             "provide your webhook peer [default=localhost:4004]> "
         ) or "http://127.0.0.1:4004"
         try:
@@ -313,20 +323,38 @@
             target_endpoint, webhook.condition(
                 f"block.data.generatorPublicKey=={puk}"
             )
         )
     )
     # dump delegate options
     path = os.path.join(tbw.DATA, f"{puk}.json")
-    dumpJson(dict(options, **loadJson(path)), path, ensure_ascii=False)
+    dumpJson(dict(loadJson(path), **options), path, ensure_ascii=False)
     os.makedirs(os.path.join(tbw.DATA, puk), exist_ok=True)
     LOGGER.info(f"delegate {puk} set")
 
 
-def set_delegate(**kwargs) -> requests.Response:
+def set_pool(**kwargs) -> requests.Response:
+    """
+    ```bash
+    $ set_pool ?key=value?
+    ```
+
+    *Pool parameters:*
+
+    - [x] `share` - share rate in float number (0. <= share = 1.0).
+    - [x] `min_vote` - minimum vote to be considered by the pool.
+    - [x] `max_vote` - maximum vote weight caped in the pool.
+    - [x] `min_share` - minimum reward to reach for a vote wallet to be
+          included in payroll.
+    - [x] `excludes` - comma-separated list of wallet to exclude.
+    - [x] `block_delay` - number of forged block between two payrolls.
+    - [x] `message` - vendorFied message to be set on each payroll transacion.
+    - [x] `chunck_size` - maximum number of recipient for a multipayment.
+    - [x] `wallet` - custom wallet to receive validator share.
+    """
     # `peer` is just to be used inside this function so we pop it from kwargs
     # if # found there
     peer = kwargs.pop("peer", {})
     # merge kwargs with command line
     options = _merge_options(**kwargs)
     # because `ip` and `port` of remote pool can be set using command line args
     # we pop them from here
@@ -337,11 +365,11 @@
     answer = options.pop("pincode", "")
     if "pincode" not in options:
         while re.match(r"^[0-9]+$", answer) is None:
             answer = getpass.getpass("enter validator security pincode> ")
     pincode = [int(e) for e in answer]
     # only valid delegate parameters available in `options` from there
     # secure POST headers and send parameters
-    return rest.POST.configure.delegate(
+    return rest.POST.pool.configure(
         peer=peer, **options,
         headers=secure_headers(rest.POST.headers, pincode)
     )
```

### Comparing `ark-mainsail-1.1.2/pool/tbw.py` & `ark-mainsail-1.2.0/mnsl_pool/tbw.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,24 +30,23 @@
         raise UnknownValidator(f"{publicKey} has no subcription here")
     excludes = info.get("excludes", [])
     # Minimum vote and maximum vote have to be converted to Xtoshi.
     min_vote = info.get("min_vote", 1) * XTOSHI
     max_vote = info.get("max_vote", int(1e6)) * XTOSHI
     share = info.get("share", 1.0)
     peer = info.get("peer", PEER)
-    # Load network.
-    rest.load_network(info["nethash"])
-    # address = identity.get_wallet(publicKey)
 
     # 2. GET FEES AND REWARDS SINCE LAST FORGED BLOCK
     last_block = loadJson(os.path.join(DATA, publicKey, "last.block"))
     # If no block found save the first one and exit.
     if last_block == {}:
         dumpJson(block, os.path.join(DATA, publicKey, "last.block"))
         return False
+    # Load network.
+    rest.load_network(info["nethash"])
     blocks = 1
     reward = int(block["reward"])
     fee = int(block["totalFee"])
     # get all unparsed blocks till the last forged
     unparsed_blocks, page, last_height = [], 1, last_block["height"]
     while page > 0:  # infinite loop
         resp = rest.GET.api.delegates(
@@ -91,15 +90,15 @@
             if v["address"] not in excludes
         )
         if resp.get("meta", {}).get("next", None) is None:
             break  # -> exit infinite loop
         page += 1  # -> go to next API page
     # filter all voters using minimum and maximum votes
     voters = dict(
-        [a, b] for a, b in voters.items() if b >= min_vote and b <= max_vote
+        [a, min(max_vote, b)] for a, b in voters.items() if b >= min_vote
     )
     LOGGER.debug(f"---- found {len(voters)} valid voters")
     # compute vote weight amongs fltered voters
     vote_weight = float(sum(voters.values()))
     voters_weight = dict([a, b / vote_weight] for a, b in voters.items())
 
     # 4. UPDATE FORGERY ACCORDING TO REWARDS AND VOTER WEIGHT
```

### Comparing `ark-mainsail-1.1.2/setup.py` & `ark-mainsail-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 
 with open("README.md") as f2:
     LONG_DESCRIPTION = f2.read()
 
 kw = {
-    "version": "1.1.2",
+    "version": "1.2.0",
     "name": "ark-mainsail",
     "keywords": ["api", "ark", "blockchain"],
     "author": "Toons",
     "author_email": "moustikitos@gmail.com",
     "maintainer": "Toons",
     "maintainer_email": "moustikitos@gmail.com",
     "url": "https://github.com/Moustikitos/python-mainsail",
@@ -19,27 +19,45 @@
         "Bug Reports": "https://github.com/Moustikitos/python-mainsail/issues",
         "Funding":
             "https://github.com/Moustikitos/python-mainsail?tab=readme-ov-file"
             "#support-this-project",
         "Source": "https://github.com/Moustikitos/python-mainsail/",
     },
     "include_package_data": False,
-    "description": "Interact with ARK blockchain and forks",
+    "description": "Interact with ARK blockchain trough mainsail framework",
     "long_description": LONG_DESCRIPTION,
     "long_description_content_type": "text/markdown",
-    "install_requires": ["requests", "base58", "pyaes", "blspy", "cSecp256k1"],
+    "install_requires": [
+        "requests==2.31.0",
+        "base58==2.1.1",
+        "pyaes==1.6.1",
+        "blspy==2.0.3",
+        "cSecp256k1==1.1.2"
+    ],
     "license": "Copyright 2024, MIT licence",
     "classifiers": [
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "Intended Audience :: End Users/Desktop",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
-    "package_dir": {"": "."}
+    "packages": [
+        "mainsail", "mainsail.tx", "mnsl_pool"
+    ],
+    "package_dir": {
+        "mainsail": "./mainsail",
+        "mnsl_pool": "./mnsl_pool"
+    },
+    "entry_points": {
+        'console_scripts': [
+            'set_pool = mnsl_pool.biom:set_pool'
+        ]
+    },
+    "zip-safe": True
 }
 
 setup(**kw)
```

### Comparing `ark-mainsail-1.1.2/test/test_identity.py` & `ark-mainsail-1.2.0/test/test_identity.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.2/test/test_v1_builders.py` & `ark-mainsail-1.2.0/test/test_v1_builders.py`

 * *Files identical despite different names*

