# Comparing `tmp/pyrasp-0.6.1rc2.tar.gz` & `tmp/pyrasp-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrasp-0.6.1rc2.tar", last modified: Wed Apr 17 06:44:32 2024, max compression
+gzip compressed data, was "pyrasp-0.6.2.tar", last modified: Sat Apr 27 12:55:33 2024, max compression
```

## Comparing `pyrasp-0.6.1rc2.tar` & `pyrasp-0.6.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 06:44:32.217777 pyrasp-0.6.1rc2/
--rw-rw-rw-   0        0        0    35823 2024-04-17 06:44:24.000000 pyrasp-0.6.1rc2/LICENSE
--rw-rw-rw-   0        0        0    43607 2024-04-17 06:44:32.215633 pyrasp-0.6.1rc2/PKG-INFO
--rw-rw-rw-   0        0        0     1666 2024-04-17 06:44:24.000000 pyrasp-0.6.1rc2/README.md
--rw-rw-rw-   0        0        0      780 2024-04-17 06:44:24.000000 pyrasp-0.6.1rc2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-17 06:44:32.195483 pyrasp-0.6.1rc2/pyrasp/
--rw-rw-rw-   0        0        0        0 2024-04-17 06:44:24.000000 pyrasp-0.6.1rc2/pyrasp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:44:32.209278 pyrasp-0.6.1rc2/pyrasp/data/
--rw-rw-rw-   0        0        0   486969 2024-04-17 06:44:24.000000 pyrasp-0.6.1rc2/pyrasp/data/sqli_model-1.1.0
--rw-rw-rw-   0        0        0  1111448 2024-04-17 06:44:24.000000 pyrasp-0.6.1rc2/pyrasp/data/xss_model-1.2.0
--rw-rw-rw-   0        0        0    87941 2024-04-17 06:44:24.000000 pyrasp-0.6.1rc2/pyrasp/pyrasp.py
--rw-rw-rw-   0        0        0     6372 2024-04-17 06:44:24.000000 pyrasp-0.6.1rc2/pyrasp/pyrasp_data.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:44:32.213535 pyrasp-0.6.1rc2/pyrasp.egg-info/
--rw-rw-rw-   0        0        0    43607 2024-04-17 06:44:32.000000 pyrasp-0.6.1rc2/pyrasp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2024-04-17 06:44:32.000000 pyrasp-0.6.1rc2/pyrasp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 06:44:32.000000 pyrasp-0.6.1rc2/pyrasp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-17 06:44:32.000000 pyrasp-0.6.1rc2/pyrasp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-17 06:44:32.000000 pyrasp-0.6.1rc2/pyrasp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 06:44:32.217777 pyrasp-0.6.1rc2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-27 12:55:33.347148 pyrasp-0.6.2/
+-rw-rw-rw-   0        0        0    35823 2024-04-27 12:55:27.000000 pyrasp-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0    43555 2024-04-27 12:55:33.345703 pyrasp-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1617 2024-04-27 12:55:27.000000 pyrasp-0.6.2/README.md
+-rw-rw-rw-   0        0        0      777 2024-04-27 12:55:27.000000 pyrasp-0.6.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-27 12:55:33.328569 pyrasp-0.6.2/pyrasp/
+-rw-rw-rw-   0        0        0        0 2024-04-27 12:55:27.000000 pyrasp-0.6.2/pyrasp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 12:55:33.340597 pyrasp-0.6.2/pyrasp/data/
+-rw-rw-rw-   0        0        0   483629 2024-04-27 12:55:27.000000 pyrasp-0.6.2/pyrasp/data/sqli_model-1.1.0
+-rw-rw-rw-   0        0        0  1116155 2024-04-27 12:55:27.000000 pyrasp-0.6.2/pyrasp/data/xss_model-1.2.0
+-rw-rw-rw-   0        0        0    96789 2024-04-27 12:55:27.000000 pyrasp-0.6.2/pyrasp/pyrasp.py
+-rw-rw-rw-   0        0        0     6631 2024-04-27 12:55:27.000000 pyrasp-0.6.2/pyrasp/pyrasp_data.py
+drwxrwxrwx   0        0        0        0 2024-04-27 12:55:33.343144 pyrasp-0.6.2/pyrasp.egg-info/
+-rw-rw-rw-   0        0        0    43555 2024-04-27 12:55:33.000000 pyrasp-0.6.2/pyrasp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2024-04-27 12:55:33.000000 pyrasp-0.6.2/pyrasp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 12:55:33.000000 pyrasp-0.6.2/pyrasp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-27 12:55:33.000000 pyrasp-0.6.2/pyrasp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-27 12:55:33.000000 pyrasp-0.6.2/pyrasp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 12:55:33.347148 pyrasp-0.6.2/setup.cfg
```

### Comparing `pyrasp-0.6.1rc2/LICENSE` & `pyrasp-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrasp-0.6.1rc2/PKG-INFO` & `pyrasp-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrasp
-Version: 0.6.1rc2
+Version: 0.6.2
 Summary: Python RASP
 Author-email: Renaud Bidou <renaud@paracyberbellum.io>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,18 +690,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sqlparse
 Requires-Dist: scikit-learn==1.3.0
 Requires-Dist: requests
 Requires-Dist: psutil
 
-<span style="font-size:2em;font-weight:bold">Python RASP</span>
+![](pyrasp.png)
 
 <p>
-    <img src="https://img.shields.io/badge/Version-0.6.1-green?style=for-the-badge" alt="version 0.6.1"/>
+    <img src="https://img.shields.io/badge/Version-0.6.2-green?style=for-the-badge" alt="version 0.6.2"/>
     <a href="https://www.paracyberbellum.io">
         <img src="https://img.shields.io/badge/A%20project%20by-ParaCyberBellum-blue?style=for-the-badge" alt="A project by ParaCyberBellum"/>
     </a>
     <a href="https://twitter.com/ParaCyberBellum">
         <img src="https://img.shields.io/badge/Twitter-@ParaCyberBellum-yellow?style=for-the-badge&color=666666" alt="@ParaCyberBellum on Twitter"/>
     </a>
 </p>
@@ -711,15 +711,15 @@
 
 It can operate using a local configuration file or get it from a remote/cloud server. Logs and telemetry (optional) can be sent to remote servers as well, and threats information can be shared across agents.
 
 One specificity of `pyrasp` relies on the fact that it does not use signatures. Instead it will leverage decoys, thresholds, system and application internals, machine learning and grammatical analysis.
 
 # Documentation
 [Full documentation](https://paracyberbellum.gitbook.io/pyrasp)
-<br>[Release Notes](https://github.com/rbidou/pyrasp/blob/main/RELEASE-NOTES.txt)
+<br>[Release Notes](https://github.com/rbidou/pyrasp/blob/main/RELEASE-NOTES.md)
 
 # Contacts
 Renaud Bidou - renaud@paracyberbellum.io
```

### Comparing `pyrasp-0.6.1rc2/README.md` & `pyrasp-0.6.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-<span style="font-size:2em;font-weight:bold">Python RASP</span>
+![](pyrasp.png)
 
 <p>
-    <img src="https://img.shields.io/badge/Version-0.6.1-green?style=for-the-badge" alt="version 0.6.1"/>
+    <img src="https://img.shields.io/badge/Version-0.6.2-green?style=for-the-badge" alt="version 0.6.2"/>
     <a href="https://www.paracyberbellum.io">
         <img src="https://img.shields.io/badge/A%20project%20by-ParaCyberBellum-blue?style=for-the-badge" alt="A project by ParaCyberBellum"/>
     </a>
     <a href="https://twitter.com/ParaCyberBellum">
         <img src="https://img.shields.io/badge/Twitter-@ParaCyberBellum-yellow?style=for-the-badge&color=666666" alt="@ParaCyberBellum on Twitter"/>
     </a>
 </p>
@@ -15,15 +15,15 @@
 
 It can operate using a local configuration file or get it from a remote/cloud server. Logs and telemetry (optional) can be sent to remote servers as well, and threats information can be shared across agents.
 
 One specificity of `pyrasp` relies on the fact that it does not use signatures. Instead it will leverage decoys, thresholds, system and application internals, machine learning and grammatical analysis.
 
 # Documentation
 [Full documentation](https://paracyberbellum.gitbook.io/pyrasp)
-<br>[Release Notes](https://github.com/rbidou/pyrasp/blob/main/RELEASE-NOTES.txt)
+<br>[Release Notes](https://github.com/rbidou/pyrasp/blob/main/RELEASE-NOTES.md)
 
 # Contacts
 Renaud Bidou - renaud@paracyberbellum.io
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Python RASP
-[version 0.6.1]_[_A_ _p_r_o_j_e_c_t_ _b_y_ _P_a_r_a_C_y_b_e_r_B_e_l_l_u_m_]_[_@_P_a_r_a_C_y_b_e_r_B_e_l_l_u_m_ _o_n_ _T_w_i_t_t_e_r_]
+![](pyrasp.png)
+[version 0.6.2]_[_A_ _p_r_o_j_e_c_t_ _b_y_ _P_a_r_a_C_y_b_e_r_B_e_l_l_u_m_]_[_@_P_a_r_a_C_y_b_e_r_B_e_l_l_u_m_ _o_n_ _T_w_i_t_t_e_r_]
 # What is PyRASP ? `pyrasp` is a **Runtime Application Self Protection**
 package for Python-based Web Servers (Flask, FastAPI and Django) and Serverless
 Functions (AWS Lambda, Google Cloud Functions). It protects against the main
 attacks web applications are exposed to, from within the application. It is
 also capable of providing basic telemetry such as cpu and memory usage, as well
 as requests count. It can operate using a local configuration file or get it
 from a remote/cloud server. Logs and telemetry (optional) can be sent to remote
 servers as well, and threats information can be shared across agents. One
 specificity of `pyrasp` relies on the fact that it does not use signatures.
 Instead it will leverage decoys, thresholds, system and application internals,
 machine learning and grammatical analysis. # Documentation [Full documentation]
 (https://paracyberbellum.gitbook.io/pyrasp)
-[Release Notes](https://github.com/rbidou/pyrasp/blob/main/RELEASE-NOTES.txt) #
+[Release Notes](https://github.com/rbidou/pyrasp/blob/main/RELEASE-NOTES.md) #
 Contacts Renaud Bidou - renaud@paracyberbellum.io
```

### Comparing `pyrasp-0.6.1rc2/pyproject.toml` & `pyrasp-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyrasp"
-version = "0.6.1rc2"
+version = "0.6.2"
 authors = [
     { name = "Renaud Bidou", email = "renaud@paracyberbellum.io" }
 ]
 description = "Python RASP"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `pyrasp-0.6.1rc2/pyrasp/pyrasp.py` & `pyrasp-0.6.2/pyrasp/pyrasp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = '0.6.1'
+VERSION = '0.6.2'
 
 from pprint import pprint
 import time
 import re
 import sqlparse
 import sqlite3
 import pickle
@@ -43,39 +43,48 @@
     from django.conf import settings as django_settings
     from django.http import HttpResponse
     from django.urls import resolve
 
 except:
     pass
 
+# Azure
+try:
+    import azure.functions as func
+
+except:
+    pass
+
 # MULTIPROCESSING - NOT FOR AWS & GCP ENVIRONMENTS
 if all([ 
     os.environ.get("AWS_EXECUTION_ENV") is None,
     os.environ.get("K_SERVICE") is None,
 ]):
     from threading import Thread
     from queue import Queue
 
 # DATA GLOBALS
 try:
     from pyrasp.pyrasp_data import DATA_VERSION, XSS_MODEL_VERSION, SQLI_MODEL_VERSION
-    from pyrasp.pyrasp_data import DEFAULT_CONFIG
-    from pyrasp.pyrasp_data import ATTACKS, ATTACKS_CHECKS, ATTACKS_CODES
-    from pyrasp.pyrasp_data import SQL_INJECTIONS_POINTS, SQL_INJECTIONS_VECTORS, SQL_INJECTIONS_FP
-    from pyrasp.pyrasp_data import XSS_VECTORS
+    from pyrasp.pyrasp_data import CLOUD_FUNCTIONS
+    from pyrasp.pyrasp_data import DEFAULT_CONFIG, DEFAULT_SECURITY_CHECKS
+    from pyrasp.pyrasp_data import ATTACKS, ATTACKS_CHECKS, ATTACKS_CODES, BRUTE_FORCE_ATTACKS
+    from pyrasp.pyrasp_data import SQL_INJECTIONS_POINTS, SQL_INJECTIONS_VECTORS, SQL_INJECTIONS_FP, SQL_QUOTES
+    from pyrasp.pyrasp_data import XSS_VECTORS, XSS_NON_ALPHA_PATTERN, NON_ALPHA_PATTERN
     from pyrasp.pyrasp_data import COMMAND_INJECTIONS_VECTORS
     from pyrasp.pyrasp_data import DLP_PATTERNS
     from pyrasp.pyrasp_data import PATTERN_CHECK_FUNCTIONS
-    from pyrasp.pyrasp_data import ATTACK_BLACKLIST, ATTACK_CMD, ATTACK_DECOY, ATTACK_FLOOD, ATTACK_FORMAT, ATTACK_HEADER, ATTACK_HPP, ATTACK_PATH, ATTACK_SPOOF, ATTACK_SQLI, ATTACK_XSS, ATTACK_DLP
+    from pyrasp.pyrasp_data import ATTACK_BLACKLIST, ATTACK_CMD, ATTACK_DECOY, ATTACK_FLOOD, ATTACK_FORMAT, ATTACK_HEADER, ATTACK_HPP, ATTACK_PATH, ATTACK_SPOOF, ATTACK_SQLI, ATTACK_XSS, ATTACK_DLP, ATTACK_BRUTE
 except:
     from pyrasp_data import DATA_VERSION, XSS_MODEL_VERSION, SQLI_MODEL_VERSION
-    from pyrasp_data import DEFAULT_CONFIG
-    from pyrasp_data import ATTACKS, ATTACKS_CHECKS, ATTACKS_CODES
-    from pyrasp_data import SQL_INJECTIONS_POINTS, SQL_INJECTIONS_VECTORS, SQL_INJECTIONS_FP
-    from pyrasp_data import XSS_VECTORS
+    from pyrasp_data import CLOUD_FUNCTIONS
+    from pyrasp_data import DEFAULT_CONFIG, DEFAULT_SECURITY_CHECKS
+    from pyrasp_data import ATTACKS, ATTACKS_CHECKS, ATTACKS_CODES, BRUTE_FORCE_ATTACKS
+    from pyrasp_data import SQL_INJECTIONS_POINTS, SQL_INJECTIONS_VECTORS, SQL_INJECTIONS_FP, SQL_QUOTES
+    from pyrasp_data import XSS_VECTORS, XSS_NON_ALPHA_PATTERN, NON_ALPHA_PATTERN
     from pyrasp_data import COMMAND_INJECTIONS_VECTORS
     from pyrasp_data import DLP_PATTERNS
     from pyrasp_data import PATTERN_CHECK_FUNCTIONS
     from pyrasp_data import ATTACK_BLACKLIST, ATTACK_CMD, ATTACK_DECOY, ATTACK_FLOOD, ATTACK_FORMAT, ATTACK_HEADER, ATTACK_HPP, ATTACK_PATH, ATTACK_SPOOF, ATTACK_SQLI, ATTACK_XSS, ATTACK_DLP, ATTACK_BRUTE
 
 # IP
 IP_COUNTRY = {}
@@ -450,16 +459,16 @@
 
             if not sqli_model_loaded:
                 self.print_screen('[!] SQLI model not loaded', init=False, new_line_up = False)
             else:
                 self.print_screen('[+] SQLI model loaded', init=True, new_line_up = False)
 
 
-        # AWS & GCP
-        if self.PLATFORM in [ 'AWS Lambda', 'Google Cloud Function']:
+        # AWS, GCP & Azure
+        if self.PLATFORM in CLOUD_FUNCTIONS:
             pass
 
         # Other environments
         else:   
             from threading import Thread
             from queue import Queue
 
@@ -472,15 +481,15 @@
                 self.start_beacon()
 
         self.print_screen('[+] PyRASP succesfully started', init=True)
         self.print_screen('############################', init=True, new_line_down=True)
 
     def __del__(self):
 
-        if not self.PLATFORM in [ 'AWS Lambda', 'Google Cloud Function']:
+        if not self.PLATFORM in CLOUD_FUNCTIONS:
 
             if self.BEACON:
                 global STOP_BEACON_THREAD
                 STOP_BEACON_THREAD = True
 
             if self.LOG_ENABLED:
                 self.LOG_QUEUE.put('--STOP--')
@@ -605,15 +614,15 @@
         if not error and server_data.get('config'):
             self.print_screen('[PyRASP] Loading new configuration')
             new_config = { 'config': server_data['config'] }
             config_changes = self.check_config_change(server_data['config'])
             self.load_config(new_config)
 
         # Restart services
-        if not error and not self.PLATFORM == 'AWS Lambda':
+        if not error and not self.PLATFORM in CLOUD_FUNCTIONS:
             if config_changes['logs']:
                 self.start_logging(restart = True) 
             if config_changes['beacon']:
                 pass
 
     def check_config_change(self, new_config):
 
@@ -754,14 +763,19 @@
     def load_config(self, config):
 
         # Load parameters
         config_params = config.get('config') or config
 
         for key in config_params:
             setattr(self, key, config_params[key])
+
+        # Setting defautl security checks
+        for security_check in DEFAULT_SECURITY_CHECKS:
+            if config_params['SECURITY_CHECKS'].get(security_check) == None:
+                config_params['SECURITY_CHECKS'][security_check] = DEFAULT_SECURITY_CHECKS[security_check]
         
         for key in config_params:
             self.print_screen(f'[+] {key} => {config_params[key]}', 100, init=False)    
 
         # Load blacklist
         config_blacklist = config.get('blacklist')
 
@@ -791,14 +805,15 @@
         attack_details['action'] = action
         if ATTACKS_CODES.get(attack_id):
             attack_details['codes'] = ATTACKS_CODES[attack_id]
 
         if not self.BLACKLIST_OVERRIDE and action == 2:
             self.blacklist_ip(source_ip, timestamp, attack_check)
 
+
         try:
             self.print_screen(f'[!] {ATTACKS[attack_id]}: {attack["details"]["location"]} -> {attack["details"]["payload"]}')
         except:
             self.print_screen(f'[!] Attack - No details')
     
         if self.LOG_ENABLED:
             self.log_security_event(attack_check, source_ip, None, attack_details)
@@ -893,27 +908,41 @@
                 if attack == None:
                     if self.SECURITY_CHECKS.get('sqli'):
                         attack = self.check_sqli(inject_vectors)
 
         return attack
 
     # Outbound attacks
-    def check_outbound_attacks(self, response_content, request_path, source_ip, timestamp, error):
+    def check_outbound_attacks(self, response_content, request_path, source_ip, timestamp, status_code, attack_type):
 
         attack = None
+        error = False
+        check_brute = False
+        check_dlp = False
 
-        # Check flood errors
+        if status_code >= 400:
+            error = True
+
+        # Check errors floods and brute force
         if error:
+            check_brute = True
+        elif attack_type in BRUTE_FORCE_ATTACKS:
+            check_brute = True
+
+
+        if check_brute:
 
-            if not attack is None and attack.get('type') == ATTACK_BLACKLIST:
-                if self.SECURITY_CHECKS.get('flood'):
-                    attack = self.flood_and_brute_check(request_path, source_ip, timestamp, error=True)
+            if self.SECURITY_CHECKS.get('brute'):
+                attack = self.flood_and_brute_check(request_path, source_ip, timestamp, error=True)
 
         # Check DLP
-        if not error and attack == None:
+        if not error and attack is None:
+            check_dlp = True
+
+        if check_dlp:
 
             if self.SECURITY_CHECKS.get('dlp') and not response_content == None:
                 attack = self.check_dlp(response_content)
 
         return attack
     
     # Alter response
@@ -1079,62 +1108,74 @@
                     if re.search(fp_pattern, injection):
                         fp = True
                         break
                 if fp:
                     continue
 
                 # Select proper injected request format
-                quotes = ''
+                sql_quotes = ['']
                 injections_point = SQL_INJECTIONS_POINTS
                               
+                '''
                 for c in injection:
                     if c == '"':
                         quotes = '"'
                         break
                     if c == "'":
                         quotes = "'"
                         break
+                '''
+
+                for c in injection:
+                    if c in SQL_QUOTES and not c in sql_quotes:
+                        sql_quotes.append(c)
                 
                 # Test valid SQL for injection point
                 for injection_point in injections_point:
 
-                    # Add input at injection point with quotes if necessary
-                    sql = injection_point.replace('{{vector}}', quotes+injection+quotes)
+                    for quotes in sql_quotes:
 
-                    # Add spaces
-                    sql = re.sub('\(', ' ( ', sql)
-                    sql = re.sub('\)', ' ) ', sql)
-                    sql = re.sub('"', ' " ', sql)
-                    sql = re.sub("'", " ' ", sql)
-
-                    # Remove comments
-                    sql = re.sub('/\*[^*]?\*/', '', sql)
-                    sql = re.sub('/\*.*', '', sql)
-                    sql = re.sub('--.*', '', sql)
-                    sql = re.sub('#.*', '', sql)
+                        # Add input at injection point with quotes if necessary
+                        sql = injection_point.replace('{{vector}}', quotes+injection+quotes)
 
-                    # Parses request to split stacked requests
-                    parsed = sqlparse.split(sql)
-                    
-                    for statement in parsed:
+                        # Add spaces
+                        sql = re.sub('\(', ' ( ', sql)
+                        sql = re.sub('\)', ' ) ', sql)
+                        sql = re.sub('"', ' " ', sql)
+                        sql = re.sub("'", " ' ", sql)
+
+                        # Remove comments
+                        sql = re.sub('/\*[^*]?\*/', '', sql)
+                        sql = re.sub('/\*.*', '', sql)
+                        sql = re.sub('--.*', '', sql)
+                        sql = re.sub('#.*', '', sql)
 
-                        if len(statement):
+                        # Parses request to split stacked requests
+                        parsed = sqlparse.split(sql)
+                        
+                        for statement in parsed:
 
-                            try:
-                                temp_db.execute(statement)
-                            except Exception as e:
-                                if 'no such table' in str(e):
-                                    sql_injection = True
-                                    
+                            if len(statement):
 
+                                try:
+                                    temp_db.execute(statement)
+                                except Exception as e:
+                                    if 'no such table' in str(e):
+                                        sql_injection = True
+                                        
+
+                            if sql_injection:
+                                break
+                                
                         if sql_injection:
-                            break
                             
+                            break
+
                     if sql_injection:
-                        
+
                         break
 
                 if len(injection) < self.MIN_SQLI_LEN:
                     continue
 
                 # Machine Learning check
                 if not sql_injection:
@@ -1171,15 +1212,15 @@
 
             # Get request values
             for injection in vectors[vector_type]:
 
                 # Requires minimum_length
                 if len(injection) > self.MIN_XSS_LEN:
 
-                    if injection.count('[') > 8 and injection.count(']') > 8:
+                    if re.match(NON_ALPHA_PATTERN, injection) or len(re.findall(XSS_NON_ALPHA_PATTERN, injection)) > 8:
                         xss = True
                         break
 
                     xss_probability = self.xss_model.predict_proba([injection.lower()])[0]
                     if xss_probability[1] > self.XSS_PROBA:
                         xss = True
                         break
@@ -1722,55 +1763,48 @@
 
             (host, request_method, request_path, source_ip, timestamp) = self.get_params(request)
             
             attack = self.check_inbound_attacks(host, request_method, request_path, source_ip, timestamp, request)
 
             # Send attack status in status code for handling by @after_request
             if not attack == None:
-                #attack_type = attack['type']
-                #self.handle_attack(attack, host, request_path, source_ip, timestamp)
                 attack_id = '::'.join([host, request_method, request_path, source_ip])
                 self.CURRENT_ATTACKS[attack_id] = attack
-                security_check = self.SECURITY_CHECKS.get(ATTACKS_CHECKS[attack['type']])
 
-                # Block attck
-                if security_check == 1 or security_check == 2:
-                    return self.GTFO_MSG, self.DENY_STATUS_CODE
-        
     # Outgoing responses
     def set_after_security_checks(self, app):
         @app.after_request
         def after_request_callback(response):
 
             (host, request_method, request_path, source_ip, timestamp) = self.get_params(request)
 
-            error = False
+            status_code = 200
             response_attack = None
             request_attack = None
             log_only = False
             security_check = None
+            inbound_attack_type = None
 
             # Get attack from @before_request checks
             attack_id = '::'.join([host, request_method, request_path, source_ip])
             current_attack = self.CURRENT_ATTACKS.get(attack_id)
             if current_attack:
                 request_attack = current_attack
                 del self.CURRENT_ATTACKS[attack_id]
 
-            # Check if response is error
-            if request_attack or response.status_code >= 400:
-                error = True
+            status_code = response.status_code
+            inbound_attack_type = current_attack['type'] if current_attack else None
 
             # Check brute force and flood
             try:
                 response_content =  response.get_data(True)
             except:
                 pass
             else:
-                response_attack = self.check_outbound_attacks(response_content, request_path, source_ip, timestamp, error)
+                response_attack = self.check_outbound_attacks(response_content, request_path, source_ip, timestamp, status_code, inbound_attack_type)
                 
             # Set response   
             if response_attack:
                 security_check = ATTACKS_CHECKS[response_attack['type']]
             elif request_attack:
                 security_check = ATTACKS_CHECKS[request_attack['type']]
             
@@ -1922,15 +1956,15 @@
     def register_security_checks(self, app):
 
         @app.middleware('http')
         async def security_checks_setup(request: Request, call_next):
     
             inbound_attack = None
             outbound_attack = None
-            error = False
+            status_code = 200
             log_only = False
             security_check = None
 
             # Get Main params
             (host, request_method, request_path, source_ip, timestamp) = self.get_params(request)
 
             # Get vectors - need to do it here as async
@@ -1943,26 +1977,29 @@
             if inbound_attack:
                 security_check = ATTACKS_CHECKS[inbound_attack['type']]
 
             if not inbound_attack or self.SECURITY_CHECKS.get(security_check) == 3:
                 response = await call_next(request)
             else:
                 response = FastApiResponse()
+
+            status_code = response.status_code
+            inbound_attack_type = inbound_attack['type'] if inbound_attack else None
             
             # Check outbound attacks
-            if inbound_attack or response.status_code >= 400:
-                error = True
+            if inbound_attack or status_code >= 400:
                 response_content = None
+            
             else:
                 
                 response_body = [chunk async for chunk in response.body_iterator]
                 response.body_iterator = iterate_in_threadpool(iter(response_body))
                 response_content = response_body[0].decode()
                 
-            outbound_attack = self.check_outbound_attacks(response_content, request_path, source_ip, timestamp, error)
+            outbound_attack = self.check_outbound_attacks(response_content, request_path, source_ip, timestamp, status_code, inbound_attack_type)
 
             # Set response   
             if outbound_attack:
                 security_check = ATTACKS_CHECKS[outbound_attack['type']]
 
             if outbound_attack:
                 self.handle_attack(outbound_attack, host, request_path, source_ip, timestamp)
@@ -2183,14 +2220,15 @@
         super().__init__(None, None, [], conf, key, cloud_url, 10, False)
 
     def __call__(self, request):
 
         inbound_attack = None
         outbound_attack = None
         error = False
+        status_code = 200
         log_only = False
         security_check = None
 
         # Get Main params
         (host, request_method, request_path, source_ip, timestamp) = self.get_params(request)
 
         # Check inboud attacks
@@ -2200,21 +2238,25 @@
             security_check = ATTACKS_CHECKS[inbound_attack['type']]
 
         if not inbound_attack or self.SECURITY_CHECKS.get(security_check) == 3:
             response = self.get_response(request)
         else:
             response = HttpResponse()
 
-        if inbound_attack or response.status_code >= 400:
-            error = True
+        status_code = response.status_code
+        inbound_attack_type = inbound_attack['type'] if inbound_attack else None
+
+        # Check outbound attacks
+        if inbound_attack or status_code >= 400:
             response_content = None
+
         else:
             response_content = response.content.decode()
 
-        outbound_attack = self.check_outbound_attacks(response_content, request_path, source_ip, timestamp, error)
+        outbound_attack = self.check_outbound_attacks(response_content, request_path, source_ip, timestamp, status_code, inbound_attack_type)
 
         if outbound_attack:
             security_check = ATTACKS_CHECKS[outbound_attack['type']]
 
         if outbound_attack:
             self.handle_attack(outbound_attack, host, request_path, source_ip, timestamp)
         elif inbound_attack:
@@ -2362,39 +2404,36 @@
                 self.LAST_BEACON = time_now
 
             (host, request_method, request_path, source_ip, timestamp) = self.get_params(request)
 
             # Analyze request
             inbound_attack = None
             outbound_attack = None
-            error = False
+            status_code = 200
             log_only = False
             security_check = None
             response = {}
 
             inbound_attack = self.check_inbound_attacks(host, request_method, request_path, source_ip, timestamp, request)
 
             if inbound_attack:
                 security_check = ATTACKS_CHECKS[inbound_attack['type']]
 
             if not inbound_attack or self.SECURITY_CHECKS.get(security_check) == 3:
                 response = f(request, context)
 
-                
-
             # Set response params
             response_content_structure = response.get('body') or {}
             response_content = json.dumps(response_content_structure)
-            error = True
+
             status_code = response.get('statusCode')
-            if inbound_attack or (status_code and int(status_code) < 400):
-                error = False
+            inbound_attack_type = inbound_attack['type'] if inbound_attack else None
 
             # Analyze response
-            outbound_attack = self.check_outbound_attacks(response_content, request_path, source_ip, timestamp, error)
+            outbound_attack = self.check_outbound_attacks(response_content, request_path, source_ip, timestamp, status_code, inbound_attack_type)
 
             if outbound_attack:
                 security_check = ATTACKS_CHECKS[outbound_attack['type']]
 
             if outbound_attack:
                 self.handle_attack(outbound_attack, host, request_path, source_ip, timestamp)
             elif inbound_attack:
@@ -2501,15 +2540,15 @@
                 request_method = http.get('method')
                 source_ip = http.get('sourceIp')
 
             else:
                 request_path = request.get('path')
                 request_method = request.get('httpMethod')
                 if context and context.get('identity'):
-                        source_ip = context['identity'].get('sourceIp')
+                    source_ip = context['identity'].get('sourceIp')
 
         return (host, request_method, request_path, source_ip, timestamp)
     
     def get_query_string(self, request):
 
         query_string = request.get('multiValueQueryStringParameters')
 
@@ -2592,15 +2631,15 @@
             self.send_beacon()
 
 
     ####################################################
     # CHECKS CONTROL
     ####################################################
 
-    # AWS handler wrapper
+    # GCP handler wrapper
     def register(self, f):
     
         @wraps(f)
         def decorator(request):
 
             # Sending beacons to get configuration and blacklist updates
             time_now = time.time()
@@ -2609,35 +2648,32 @@
                 self.LAST_BEACON = time_now
 
             (host, request_method, request_path, source_ip, timestamp) = self.get_params(request)
 
             # Analyze request
             inbound_attack = None
             outbound_attack = None
-            error = False
             log_only = False
             security_check = None
-            response = {}
+            status_code = 200
+            response = None
 
             inbound_attack = self.check_inbound_attacks(host, request_method, request_path, source_ip, timestamp, request)
 
             if inbound_attack:
                 security_check = ATTACKS_CHECKS[inbound_attack['type']]
 
             if not inbound_attack or self.SECURITY_CHECKS.get(security_check) == 3:
                 response = f(request)
 
-            (response_content, status_code) = self.get_response_data(response)
+            (response_content, status_code) = self.get_response_data(response) or None
+            inbound_attack_type = inbound_attack['type'] if inbound_attack else None
 
-            # Check if response is error
-            if inbound_attack or status_code >= 400:
-                error = True
-            
             # Analyze response
-            outbound_attack = self.check_outbound_attacks(response_content, request_path, source_ip, timestamp, error)
+            outbound_attack = self.check_outbound_attacks(response_content, request_path, source_ip, timestamp, status_code, inbound_attack_type)
 
             if outbound_attack:
                 security_check = ATTACKS_CHECKS[outbound_attack['type']]
 
             if outbound_attack:
                 self.handle_attack(outbound_attack, host, request_path, source_ip, timestamp)
             elif inbound_attack:
@@ -2739,11 +2775,228 @@
                 sock.settimeout(1)
                 sock.send(log_data)
                 sock.close()
 
         except:
             pass
 
+class AzureRASP(PyRASP):
+
+    LAST_BEACON = time.time()
+
+    def __init__(self, app=None, app_name=None, hosts=[], conf=None, key=None, cloud_url=None, verbose_level=10, dev=False):
+        self.PLATFORM = 'Azure Function'
+        super().__init__(app, app_name, hosts, conf, key, cloud_url, verbose_level, dev)
 
+    ####################################################
+    # CHECKS CONTROL
+    ####################################################
+
+    # Azure Function handler wrapper
+    def register(self, f):
     
+        @wraps(f)
+        def decorator(req):
+
+            request = req
+
+            # Sending beacons to get configuration and blacklist updates
+            time_now = time.time()
+            if self.BEACON and time_now > self.LAST_BEACON + self.BEACON_DELAY:
+                self.send_beacon()
+                self.LAST_BEACON = time_now
+
+            (host, request_method, request_path, source_ip, timestamp) = self.get_params(request)
+
+            # Analyze request
+            inbound_attack = None
+            outbound_attack = None
+            log_only = False
+            security_check = None
+            status_code = 200
+            response = func.HttpResponse()
+
+            inbound_attack = self.check_inbound_attacks(host, request_method, request_path, source_ip, timestamp, request)
+
+            if inbound_attack:
+                security_check = ATTACKS_CHECKS[inbound_attack['type']]
+
+            if not inbound_attack or self.SECURITY_CHECKS.get(security_check) == 3:
+                response = f(req)
+
+            response_content = response.get_body().decode() or ''
+            status_code = response.status_code
+            inbound_attack_type = inbound_attack['type'] if inbound_attack else None
+
+            # Analyze response
+            outbound_attack = self.check_outbound_attacks(response_content, request_path, source_ip, timestamp, status_code, inbound_attack_type)
+
+            if outbound_attack:
+                security_check = ATTACKS_CHECKS[outbound_attack['type']]
+
+            if outbound_attack:
+                self.handle_attack(outbound_attack, host, request_path, source_ip, timestamp)
+            elif inbound_attack:
+                self.handle_attack(inbound_attack, host, request_path, source_ip, timestamp)
+
+            # Check log only
+            if security_check and self.SECURITY_CHECKS.get(security_check) == 3:
+                log_only = True
+
+            response = self.process_response(response, inbound_attack or outbound_attack, log_only = log_only)
+                
+            return response
+            
+        return decorator
+    
+    ####################################################
+    # RESPONSE PROCESSING
+    ####################################################
+
+    # Alter response
+    def process_response(self, response, attack = None, log_only = True):
+
+        status_code = response.status_code
+
+        if attack:
+            if not log_only:
+                response = self.make_attack_response()
+            self.REQUESTS['attacks'] += 1
+
+        elif status_code == 200:
+            self.REQUESTS['success'] += 1
+
+        else:
+            self.REQUESTS['errors'] += 1
+
+        return response
+    
+    def make_attack_response(self):
+
+        response = func.HttpResponse(self.GTFO_MSG, status_code=self.DENY_STATUS_CODE)
+
+        return response
+
+    ####################################################
+    # PARAMS & VECTORS
+    ####################################################
+
+    def get_params(self, request):
+
+        (host, request_method, request_path, source_ip, timestamp) = ('', '', '', '', time.time())
+
+
+        headers = dict(request.headers)
+
+        host = headers.get('host') if headers.get('host') else '127.0.0.1'
+        request_method = str(request.method)
+        request_path = headers.get('x-original-url') if headers.get('x-original-url') else '/'
+
+        source_ip_port = headers.get('x-forwarded-for')
+        source_ip = source_ip_port.split(':')[0] if source_ip_port else '127.0.0.1'
+
+        return (host, request_method, request_path, source_ip, timestamp)
+    
+    def get_query_string(self, request):
+
+        query_string_list = dict(request.params)
+
+        query_string = {}
+        for qs_variable in query_string_list:
+            qs_value = query_string_list[qs_variable]
+            if not qs_variable in query_string:
+                query_string[qs_variable] = []
+            query_string[qs_variable].append(qs_value)
+
+        return query_string
+    
+    def get_posted_data(self, request):
+
+        posted_data = {}
+
+        posted_data_full = request.get_body().decode() or ''
+
+        posted_data_parts = posted_data_full.split('&')
+
+        for posted_data_part in posted_data_parts:
+            posted_data_tuple = posted_data_part.split('=')
+            if len(posted_data_tuple) == 2:
+                post_variable = posted_data_tuple[0]
+                post_value = posted_data_tuple[1]
+
+                if not post_variable in posted_data:
+                    posted_data[post_variable] = []
+
+                posted_data[post_variable].append(post_value)
+
+        return posted_data
+    
+    def get_request_path(self, request):
+        
+        headers = dict(request.headers)
+
+        request_path = headers.get('x-original-url') if headers.get('x-original-url') else '/'
+
+        return request_path
+    
+    def get_json_data(self, request):
+
+        json_keys = []
+        json_values = []
+
+        try:
+            json_data = request.get_json()
+            (json_keys, json_values) = self.analyze_json(json_data)
+        except:
+            pass
+
+        return (json_keys, json_values)
+    
+    def get_request_headers(self, request):
+
+        headers = dict(request.headers)
+
+        return headers
+
+    ####################################################
+    # LOGGING
+    ####################################################
+
+    def log_security_event(self, event_type, source_ip, user = None, details = {}):
+
+        log_data = make_security_log(self.APP_NAME, event_type, source_ip, self.LOG_FORMAT, user, details, False)
         
+        webhook = False
+        syslog_udp = False
+        syslog_tcp = False
+
+        if self.LOG_FORMAT.lower() in ['json', 'pcb']:
+            path = self.LOG_PATH
+            if not path.startswith('/'):
+                path = '/'+path
+            server_url = f'{self.LOG_PROTOCOL.lower()}://{self.LOG_SERVER}:{self.LOG_PORT}{path}'
+            webhook = True
+
+        elif self.LOG_FORMAT.lower() == 'syslog':
+            if self.LOG_PROTOCOL.lower() == 'udp':
+                syslog_udp = True
+                sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+            elif self.LOG_PROTOCOL.lower() == 'tcp':
+                syslog_tcp = True
+                sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+
+        try:
+            if webhook:
+                requests.post(server_url, json=log_data, timeout=1) 
+            elif syslog_udp:
+                sock.sendto(log_data.encode(), (self.LOG_SERVER, self.LOG_PORT))
+            elif syslog_tcp:
+                sock.connect((self.LOG_SERVER, self.LOG_PORT))
+                sock.settimeout(1)
+                sock.send(log_data)
+                sock.close()
+
+        except:
+            pass
+
+
```

### Comparing `pyrasp-0.6.1rc2/pyrasp/pyrasp_data.py` & `pyrasp-0.6.2/pyrasp/pyrasp_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 # VERSION
 #
 
 DATA_VERSION = '1.1.0'
 XSS_MODEL_VERSION = '1.2.0'
 SQLI_MODEL_VERSION = '1.1.0'
 
+#
+# PLATFORMS
+#
+
+CLOUD_FUNCTIONS = ['AWS Lambda', 'Google Cloud Function', 'Azure Function' ]
+
 # 
 # UTILS
 #
 
 PATTERN_CHECK_FUNCTIONS = [ 'regex', 'starts', 'contains', 'match' ]
 
 #
@@ -24,18 +30,20 @@
     'Decoyed',              # 4
     'Format Mismatch',      # 5
     'SQL Injection',        # 6
     'XSS',                  # 7
     'Parameter Pollution',  # 8
     'Command Injection',    # 9
     'Forbidden Header',     # 10
-    'Data Leak Prevention'  # 11
+    'Data Leak Prevention', # 11
     'Brute Force'           # 12
 ]
 
+BRUTE_FORCE_ATTACKS = [ 1, 3, 5, 10 ]
+
 # Attacks IDs
 ATTACK_BLACKLIST = 0
 ATTACK_PATH = 1
 ATTACK_FLOOD = 2
 ATTACK_SPOOF = 3
 ATTACK_DECOY = 4
 ATTACK_FORMAT = 5
@@ -110,14 +118,17 @@
     'select * from test group by {{vector}}',
     'update test set var={{vector}}',
     'update test set var=value where column_name={{vector}}',
     'insert into test values(null,{{vector}})',
 ]
 
 SQL_INJECTIONS_VECTORS = [ 'path', 'cookies', 'qs_values', 'post_values', 'json_values' ]
+
+SQL_QUOTES = [ '"', "'", '' ]
+
 XSS_VECTORS = [ 'path', 'cookies', 'qs_values', 'post_values', 'json_values', 'headers_values', 'referer' ]
 COMMAND_INJECTIONS_VECTORS = [ 'qs_values', 'post_values', 'json_values' ]
 
 DLP_PATTERNS = {
     'phone': [ r'(011|00|\+)((?:9[679]|8[035789]|6[789]|5[90]|42|3[578]|2[1-689])|9[0-58]|8[1246]|6[0-6]|5[1-8]|4[013-9]|3[0-469]|2[70]|7|1)(?:\W*\d){0,13}\d' ],
     'cc': [ r'(?:4[0-9]{12}(?:[0-9]{3})?|(?:5[1-5][0-9]{2}|222[1-9]|22[3-9][0-9]|2[3-6][0-9]{2}|27[01][0-9]|2720)[0-9]{12}|3[47][0-9]{13})' ],
     'key': [ r'-----BEGIN ([A-Z]+ )?PRIVATE KEY( BLOCK)?-----' ],
@@ -133,43 +144,47 @@
     'linux': [
         r'\$(1|2(a|y)?|5|6)\$[a-z0-9\/.]{0,96}\$[a-z0-9\/.]{22,128}?' , # MD5 / Blowfish / SHA-256 / SHA-512
         r'\$(y|7)\$[.\/A-Za-z0-9]+\$[.\/A-Za-z0-9]{,86}\$[.\/A-Za-z0-9]{43}', # Yescrypt
     ]
 
 }
 
-
+XSS_NON_ALPHA_PATTERN = '\[[^A-Za-z0-9\]]*\]'
+NON_ALPHA_PATTERN = '^[^A-Za-z0-9]+$'
 
 #
 # DEFAULT CONFIGURATION
 #
 
+DEFAULT_SECURITY_CHECKS = {
+    "path": 1,
+    "headers": 0,
+    "flood": 2,
+    "spoofing": 0,
+    "decoy": 2,
+    "format": 2,
+    "sqli": 2,
+    "xss": 2,
+    "hpp": 2,
+    "command": 2,
+    "method": 0,
+    "dlp": 0,
+    "brute": 2
+}
+
 DEFAULT_CONFIG = {
     "HOSTS" : [],
     "APP_NAME" : "Web Server",
     "GTFO_MSG" : 'Blocked',
     "DENY_STATUS_CODE": 403,
 
     "VERBOSE" : 0,
     "DECODE_B64" : True,
 
-    "SECURITY_CHECKS" : {
-        "path": 1,
-        "headers": 0,
-        "flood": 2,
-        "spoofing": 0,
-        "decoy": 2,
-        "format": 2,
-        "sqli": 2,
-        "xss": 2,
-        "hpp": 2,
-        "command": 2,
-        "method": 0,
-        "dlp": 0
-    },    
+    "SECURITY_CHECKS" : { },    
 
     "WHITELIST": [],
     "IGNORE_PATHS" : ["^/favicon.ico$","^/robots.txt$","^/sitemap\.(txt|xml)$"],
 
     "FORBIDDEN_HEADERS": [ ],
 
     "BRUTE_AND_FLOOD_PATHS" : ["^/"],
```

### Comparing `pyrasp-0.6.1rc2/pyrasp.egg-info/PKG-INFO` & `pyrasp-0.6.2/pyrasp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrasp
-Version: 0.6.1rc2
+Version: 0.6.2
 Summary: Python RASP
 Author-email: Renaud Bidou <renaud@paracyberbellum.io>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,18 +690,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sqlparse
 Requires-Dist: scikit-learn==1.3.0
 Requires-Dist: requests
 Requires-Dist: psutil
 
-<span style="font-size:2em;font-weight:bold">Python RASP</span>
+![](pyrasp.png)
 
 <p>
-    <img src="https://img.shields.io/badge/Version-0.6.1-green?style=for-the-badge" alt="version 0.6.1"/>
+    <img src="https://img.shields.io/badge/Version-0.6.2-green?style=for-the-badge" alt="version 0.6.2"/>
     <a href="https://www.paracyberbellum.io">
         <img src="https://img.shields.io/badge/A%20project%20by-ParaCyberBellum-blue?style=for-the-badge" alt="A project by ParaCyberBellum"/>
     </a>
     <a href="https://twitter.com/ParaCyberBellum">
         <img src="https://img.shields.io/badge/Twitter-@ParaCyberBellum-yellow?style=for-the-badge&color=666666" alt="@ParaCyberBellum on Twitter"/>
     </a>
 </p>
@@ -711,15 +711,15 @@
 
 It can operate using a local configuration file or get it from a remote/cloud server. Logs and telemetry (optional) can be sent to remote servers as well, and threats information can be shared across agents.
 
 One specificity of `pyrasp` relies on the fact that it does not use signatures. Instead it will leverage decoys, thresholds, system and application internals, machine learning and grammatical analysis.
 
 # Documentation
 [Full documentation](https://paracyberbellum.gitbook.io/pyrasp)
-<br>[Release Notes](https://github.com/rbidou/pyrasp/blob/main/RELEASE-NOTES.txt)
+<br>[Release Notes](https://github.com/rbidou/pyrasp/blob/main/RELEASE-NOTES.md)
 
 # Contacts
 Renaud Bidou - renaud@paracyberbellum.io
```

