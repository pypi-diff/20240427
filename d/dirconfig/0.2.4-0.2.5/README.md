# Comparing `tmp/dirconfig-0.2.4.tar.gz` & `tmp/dirconfig-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirconfig-0.2.4.tar", last modified: Sat Apr 27 05:18:42 2024, max compression
+gzip compressed data, was "dirconfig-0.2.5.tar", last modified: Sat Apr 27 18:34:18 2024, max compression
```

## Comparing `dirconfig-0.2.4.tar` & `dirconfig-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:18:42.634647 dirconfig-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-27 05:18:20.000000 dirconfig-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-04-27 05:18:42.634647 dirconfig-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-04-27 05:18:20.000000 dirconfig-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:18:42.634647 dirconfig-0.2.4/dirconfig/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 05:18:20.000000 dirconfig-0.2.4/dirconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9525 2024-04-27 05:18:20.000000 dirconfig-0.2.4/dirconfig/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:18:42.634647 dirconfig-0.2.4/dirconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-04-27 05:18:42.000000 dirconfig-0.2.4/dirconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-27 05:18:42.000000 dirconfig-0.2.4/dirconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 05:18:42.000000 dirconfig-0.2.4/dirconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-27 05:18:42.000000 dirconfig-0.2.4/dirconfig.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-27 05:18:42.000000 dirconfig-0.2.4/dirconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-27 05:18:42.000000 dirconfig-0.2.4/dirconfig.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 05:18:42.634647 dirconfig-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-27 05:18:40.000000 dirconfig-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 05:18:42.634647 dirconfig-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 05:18:20.000000 dirconfig-0.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-27 05:18:20.000000 dirconfig-0.2.4/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:34:18.967827 dirconfig-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-27 18:34:03.000000 dirconfig-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-27 18:34:18.967827 dirconfig-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-27 18:34:03.000000 dirconfig-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:34:18.967827 dirconfig-0.2.5/dirconfig/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 18:34:03.000000 dirconfig-0.2.5/dirconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-04-27 18:34:03.000000 dirconfig-0.2.5/dirconfig/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:34:18.967827 dirconfig-0.2.5/dirconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-27 18:34:18.000000 dirconfig-0.2.5/dirconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-27 18:34:18.000000 dirconfig-0.2.5/dirconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 18:34:18.000000 dirconfig-0.2.5/dirconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-27 18:34:18.000000 dirconfig-0.2.5/dirconfig.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-27 18:34:18.000000 dirconfig-0.2.5/dirconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-27 18:34:18.000000 dirconfig-0.2.5/dirconfig.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 18:34:18.967827 dirconfig-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-27 18:34:17.000000 dirconfig-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:34:18.967827 dirconfig-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 18:34:03.000000 dirconfig-0.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-27 18:34:03.000000 dirconfig-0.2.5/tests/test_main.py
```

### Comparing `dirconfig-0.2.4/LICENSE` & `dirconfig-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dirconfig-0.2.4/PKG-INFO` & `dirconfig-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: dirconfig
-Version: 0.2.4
+Version: 0.2.5
 Summary: A simple directory configuration tool
 Home-page: https://github.com/judahpaul16/dirconfig
 Author: Judah Paul
 Author-email: me@judahpaul.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyYAML==6.0.1
+Requires-Dist: watchdog==4.0.0
 
 # dirconfig 📂
 
 [![PyPI](https://img.shields.io/pypi/v/dirconfig)](https://pypi.org/project/dirconfig/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dirconfig)
 [![PyPI - License](https://img.shields.io/pypi/l/dirconfig)](LICENSE)
 [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/judahpaul16/dirconfig/workflow.yaml)](https://github.com/judahpaul16/dirconfig/actions)
@@ -77,22 +79,31 @@
 
 To initiate **dirconfig** and begin the monitoring process, use the following command:
 
 ```sh
 dirconfig start
 ```
 
-This command starts **dirconfig**, which then operates in the background. It will watch the source directories specified in your `config.yml` for any changes, organizing files according to your predefined rules.
+This command starts **dirconfig**, which operates in the background. It will watch the source directories specified in your `config.yml` for any changes, organizing files according to your predefined rules.
 
-To run **dirconfig** as a separate process, use the following command:
+Alternatively, to run **dirconfig** as a separate process, use the following command:
 
 ```sh
 dirconfig start &
 ```
 
+### Stopping dirconfig
+
+To stop the **dirconfig** daemon, execute:
+
+```sh
+dirconfig stop
+```
+This command stops the background process of **dirconfig**, halting the monitoring and file organization tasks.
+
 ### Command Line Options
 ```sh
 usage: dirconfig [-h] [--config CONFIG] [--log LOG] [--pid PID] {start,stop,generate}
 
 dirconfig Daemon
 
 positional arguments:
@@ -102,38 +113,31 @@
 options:
   -h, --help            show this help message and exit
   --config CONFIG       Path to the configuration file
   --log LOG             Path to the log file
   --pid PID             Path to the PID file
 ```
 
-### Stopping dirconfig
-
-To stop the **dirconfig** daemon, execute:
-
-```sh
-dirconfig stop
-```
-
-This command stops the background process of **dirconfig**, halting the monitoring and file organization tasks.
-
 ### Advanced Management
 
 For long-term operation or deployment, integrating **dirconfig** with system services or process managers can offer more graceful management, including automatic restarts, logging, and simplified start/stop operations.
 
 ## Extending dirconfig
 
 **dirconfig** welcomes enhancements and customization. If you're interested in adding new features or improving the tool, consider contributing to the source code. Your input and contributions are highly appreciated.
 
 ## Urbackup Documentation
 For more information on the Urbackup API, please refer to these resources:
 * *[Urbackup Python API Wrapper](https://github.com/uroni/urbackup-server-python-web-api-wrapper)*
 * *[Urbackup Backend ClientCTL](https://github.com/uroni/urbackup_backend/tree/dev/clientctl)*
 
+*Important Note: For Windows the command-line tool is `urbackupclient_cmd`. Mac and Linux use `urbackupclientctl`.
+
 Command Line Options for `urbackupclientctl` are as follows:
+
 ```sh
 USAGE:
 
         urbackupclientctl [--help] [--version] <command> [<args>]
 
 Get specific command help with urbackupclientctl <command> --help
```

### Comparing `dirconfig-0.2.4/README.md` & `dirconfig-0.2.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -63,22 +63,31 @@
 
 To initiate **dirconfig** and begin the monitoring process, use the following command:
 
 ```sh
 dirconfig start
 ```
 
-This command starts **dirconfig**, which then operates in the background. It will watch the source directories specified in your `config.yml` for any changes, organizing files according to your predefined rules.
+This command starts **dirconfig**, which operates in the background. It will watch the source directories specified in your `config.yml` for any changes, organizing files according to your predefined rules.
 
-To run **dirconfig** as a separate process, use the following command:
+Alternatively, to run **dirconfig** as a separate process, use the following command:
 
 ```sh
 dirconfig start &
 ```
 
+### Stopping dirconfig
+
+To stop the **dirconfig** daemon, execute:
+
+```sh
+dirconfig stop
+```
+This command stops the background process of **dirconfig**, halting the monitoring and file organization tasks.
+
 ### Command Line Options
 ```sh
 usage: dirconfig [-h] [--config CONFIG] [--log LOG] [--pid PID] {start,stop,generate}
 
 dirconfig Daemon
 
 positional arguments:
@@ -88,38 +97,31 @@
 options:
   -h, --help            show this help message and exit
   --config CONFIG       Path to the configuration file
   --log LOG             Path to the log file
   --pid PID             Path to the PID file
 ```
 
-### Stopping dirconfig
-
-To stop the **dirconfig** daemon, execute:
-
-```sh
-dirconfig stop
-```
-
-This command stops the background process of **dirconfig**, halting the monitoring and file organization tasks.
-
 ### Advanced Management
 
 For long-term operation or deployment, integrating **dirconfig** with system services or process managers can offer more graceful management, including automatic restarts, logging, and simplified start/stop operations.
 
 ## Extending dirconfig
 
 **dirconfig** welcomes enhancements and customization. If you're interested in adding new features or improving the tool, consider contributing to the source code. Your input and contributions are highly appreciated.
 
 ## Urbackup Documentation
 For more information on the Urbackup API, please refer to these resources:
 * *[Urbackup Python API Wrapper](https://github.com/uroni/urbackup-server-python-web-api-wrapper)*
 * *[Urbackup Backend ClientCTL](https://github.com/uroni/urbackup_backend/tree/dev/clientctl)*
 
+*Important Note: For Windows the command-line tool is `urbackupclient_cmd`. Mac and Linux use `urbackupclientctl`.
+
 Command Line Options for `urbackupclientctl` are as follows:
+
 ```sh
 USAGE:
 
         urbackupclientctl [--help] [--version] <command> [<args>]
 
 Get specific command help with urbackupclientctl <command> --help
```

### Comparing `dirconfig-0.2.4/dirconfig/main.py` & `dirconfig-0.2.5/dirconfig/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import os
 
 # Global variables
 observer = None
 backup_thread = None # Thread for backup scheduling
 shutdown_event = Event()  # Event to signal shutdown to backup thread
 PID_FILE = 'dirconfig.pid' # Default PID file path
+MODULE_DIR = os.path.dirname(os.path.abspath(__file__)) # Directory of the module
 
 class ChangeHandler(FileSystemEventHandler):
     def __init__(self, tasks):
         self.tasks = tasks
 
     def on_any_event(self, event):
         for task in self.tasks:
@@ -69,34 +70,43 @@
     logging.info("Received interrupt signal. Stopping dirconfig...")
     if observer is not None:
         observer.stop()
         observer.join()  # Ensure all threads are joined
         if os.path.exists(PID_FILE):
             os.remove(PID_FILE)
         sys.exit(0)
+        
+def get_urbackup_command():
+    if os.name == 'nt':  # Windows
+        return 'urbackupclient_cmd'
+    else:  # Linux or macOS
+        return 'urbackupclientctl'
 
 def check_and_install_urbackup_client(backup_config):
-    stdout, stderr, returncode = subprocess.run(["urbackupclientctl", "status"], capture_output=True, text=True)
+    stdout, stderr, returncode = subprocess.run([get_urbackup_command(), "status"], capture_output=True, text=True)
     if returncode != 0:
         print("UrBackup client not running. Attempting installation...")
         logging.info("UrBackup client not running. Attempting installation...")
         # Determine OS type for choosing the correct installer
         os_type = installer_os.Linux if os.name != 'nt' else installer_os.Windows
         installer_filename = "urbackup_client_installer" + (".exe" if os_type == installer_os.Windows else "")
         backup_server = urbackup_server(
             server_url=backup_config['connection']['server'],
             server_username=backup_config['connection']['username'],
             server_password=backup_config['connection']['password']
         )
         if backup_server.login():
             client_name = f"{backup_config['name']}-dirconfig"
             if backup_server.download_installer(installer_filename, client_name, os_type):
-                if os.name != 'nt':
+                if os_type != 'Windows':
                     subprocess.run(["chmod", "+x", installer_filename])  # Make executable on Unix/Linux
-                subprocess.run([f"./{installer_filename}"])  # Execute installer
+                subprocess.run([os.path.join(MODULE_DIR, '{installer_filename}')])  # Execute installer
+                # Add urbackupclientctl to PATH if Windows
+                if os_type == 'Windows':
+                    subprocess.run([os.path.join(MODULE_DIR, 'add_to_path.exe')], check=True)
                 print("Installation successful.")
                 logging.info("Installation successful.")
             else:
                 print("Failed to download installer.")
                 logging.error("Failed to download installer.")
         else:
             print("Failed to log in to the backup server.")
@@ -104,15 +114,15 @@
     else:
         print("UrBackup client is running.")
         logging.info("UrBackup client is running.")
 
 def setup_backup_dirs(backup_config):
     """Add directories specified in config to UrBackup."""
     for directory in backup_config['directories']:
-        cmd = ["urbackupclientctl", "add-backupdir", "--path", directory]
+        cmd = [get_urbackup_command(), "add-backupdir", "--path", directory]
         result = subprocess.run(cmd, capture_output=True, text=True)
         if result.returncode == 0:
             print(f"Successfully added backup directory: {directory}")
             logging.info(f"Successfully added backup directory: {directory}")
         else:
             print(f"Failed to add backup directory: {directory}. Error: {result.stderr}")
             logging.error(f"Failed to add backup directory: {directory}. Error: {result.stderr}")
@@ -121,15 +131,15 @@
     """Initiate the backup process using the urbackupclientctl command with detailed options."""
     if 'incremental' in backup_type:
         backup_option = '-i'
     else:
         backup_option = '-f'
 
     cmd = [
-        "urbackupclientctl", "start", backup_option,
+        get_urbackup_command(), "start", backup_option,
         "--non-blocking", "--client", client_name
     ]
     result = subprocess.run(cmd, capture_output=True, text=True)
     if result.returncode == 0:
         print(f"Successfully started {backup_type} backup for {client_name}.")
         logging.info(f"Successfully started {backup_type} backup for {client_name}.")
     else:
```

### Comparing `dirconfig-0.2.4/dirconfig.egg-info/PKG-INFO` & `dirconfig-0.2.5/dirconfig.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: dirconfig
-Version: 0.2.4
+Version: 0.2.5
 Summary: A simple directory configuration tool
 Home-page: https://github.com/judahpaul16/dirconfig
 Author: Judah Paul
 Author-email: me@judahpaul.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyYAML==6.0.1
+Requires-Dist: watchdog==4.0.0
 
 # dirconfig 📂
 
 [![PyPI](https://img.shields.io/pypi/v/dirconfig)](https://pypi.org/project/dirconfig/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dirconfig)
 [![PyPI - License](https://img.shields.io/pypi/l/dirconfig)](LICENSE)
 [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/judahpaul16/dirconfig/workflow.yaml)](https://github.com/judahpaul16/dirconfig/actions)
@@ -77,22 +79,31 @@
 
 To initiate **dirconfig** and begin the monitoring process, use the following command:
 
 ```sh
 dirconfig start
 ```
 
-This command starts **dirconfig**, which then operates in the background. It will watch the source directories specified in your `config.yml` for any changes, organizing files according to your predefined rules.
+This command starts **dirconfig**, which operates in the background. It will watch the source directories specified in your `config.yml` for any changes, organizing files according to your predefined rules.
 
-To run **dirconfig** as a separate process, use the following command:
+Alternatively, to run **dirconfig** as a separate process, use the following command:
 
 ```sh
 dirconfig start &
 ```
 
+### Stopping dirconfig
+
+To stop the **dirconfig** daemon, execute:
+
+```sh
+dirconfig stop
+```
+This command stops the background process of **dirconfig**, halting the monitoring and file organization tasks.
+
 ### Command Line Options
 ```sh
 usage: dirconfig [-h] [--config CONFIG] [--log LOG] [--pid PID] {start,stop,generate}
 
 dirconfig Daemon
 
 positional arguments:
@@ -102,38 +113,31 @@
 options:
   -h, --help            show this help message and exit
   --config CONFIG       Path to the configuration file
   --log LOG             Path to the log file
   --pid PID             Path to the PID file
 ```
 
-### Stopping dirconfig
-
-To stop the **dirconfig** daemon, execute:
-
-```sh
-dirconfig stop
-```
-
-This command stops the background process of **dirconfig**, halting the monitoring and file organization tasks.
-
 ### Advanced Management
 
 For long-term operation or deployment, integrating **dirconfig** with system services or process managers can offer more graceful management, including automatic restarts, logging, and simplified start/stop operations.
 
 ## Extending dirconfig
 
 **dirconfig** welcomes enhancements and customization. If you're interested in adding new features or improving the tool, consider contributing to the source code. Your input and contributions are highly appreciated.
 
 ## Urbackup Documentation
 For more information on the Urbackup API, please refer to these resources:
 * *[Urbackup Python API Wrapper](https://github.com/uroni/urbackup-server-python-web-api-wrapper)*
 * *[Urbackup Backend ClientCTL](https://github.com/uroni/urbackup_backend/tree/dev/clientctl)*
 
+*Important Note: For Windows the command-line tool is `urbackupclient_cmd`. Mac and Linux use `urbackupclientctl`.
+
 Command Line Options for `urbackupclientctl` are as follows:
+
 ```sh
 USAGE:
 
         urbackupclientctl [--help] [--version] <command> [<args>]
 
 Get specific command help with urbackupclientctl <command> --help
```

### Comparing `dirconfig-0.2.4/setup.py` & `dirconfig-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dirconfig",
-    version="0.2.4",
+    version="0.2.5",
     author="Judah Paul",
     author_email="me@judahpaul.com",
     description="A simple directory configuration tool",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/judahpaul16/dirconfig",
     packages=find_packages(),
```

### Comparing `dirconfig-0.2.4/tests/test_main.py` & `dirconfig-0.2.5/tests/test_main.py`

 * *Files identical despite different names*

