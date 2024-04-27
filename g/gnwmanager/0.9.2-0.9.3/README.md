# Comparing `tmp/gnwmanager-0.9.2.tar.gz` & `tmp/gnwmanager-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnwmanager-0.9.2.tar", max compression
+gzip compressed data, was "gnwmanager-0.9.3.tar", max compression
```

## Comparing `gnwmanager-0.9.2.tar` & `gnwmanager-0.9.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11357 2024-03-17 21:53:28.310287 gnwmanager-0.9.2/LICENSE
--rw-r--r--   0        0        0     7858 2024-03-17 21:53:28.310287 gnwmanager-0.9.2/README.md
--rw-r--r--   0        0        0      134 2024-03-17 21:54:58.418572 gnwmanager-0.9.2/gnwmanager/__init__.py
--rw-r--r--   0        0        0       41 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/__main__.py
--rw-r--r--   0        0        0      639 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/cli/__init__.py
--rw-r--r--   0        0        0     2651 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/cli/_debug.py
--rw-r--r--   0        0        0     2074 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/cli/_dump.py
--rw-r--r--   0        0        0      981 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/cli/_erase.py
--rw-r--r--   0        0        0     8092 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/cli/_filesystem.py
--rw-r--r--   0        0        0     1667 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/cli/_flash.py
--rw-r--r--   0        0        0     1738 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/cli/_gdb.py
--rw-r--r--   0        0        0     3618 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/cli/_install.py
--rw-r--r--   0        0        0     2351 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/cli/_lock.py
--rw-r--r--   0        0        0     2173 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/cli/_monitor.py
--rw-r--r--   0        0        0     1769 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/cli/_parsers.py
--rw-r--r--   0        0        0     2297 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/cli/_pull.py
--rw-r--r--   0        0        0     3651 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/cli/_push.py
--rw-r--r--   0        0        0     2545 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/cli/_screenshot.py
--rw-r--r--   0        0        0     1179 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/cli/_start.py
--rw-r--r--   0        0        0     5531 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/cli/_unlock.py
--rw-r--r--   0        0        0     5045 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/cli/devices.py
--rw-r--r--   0        0        0     8038 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/cli/main.py
--rw-r--r--   0        0        0     1488 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/elf.py
--rw-r--r--   0        0        0      262 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/exceptions.py
--rw-r--r--   0        0        0     3744 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/filesystem.py
--rwxr-xr-x   0        0        0    35176 2024-03-17 21:54:57.946570 gnwmanager-0.9.2/gnwmanager/firmware.bin
--rw-r--r--   0        0        0    19845 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/gnw.py
--rw-r--r--   0        0        0      129 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/ocdbackend/__init__.py
--rw-r--r--   0        0        0     2380 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/ocdbackend/base.py
--rw-r--r--   0        0        0    10615 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/ocdbackend/openocd_backend.py
--rw-r--r--   0        0        0     3511 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/ocdbackend/pyocd_backend.py
--rw-r--r--   0        0        0        0 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/py.typed
--rw-r--r--   0        0        0      351 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/status.py
--rw-r--r--   0        0        0        1 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/target.py
--rw-r--r--   0        0        0      149 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/time.py
--rw-r--r--   0        0        0     1288 2024-03-17 21:54:57.050567 gnwmanager-0.9.2/gnwmanager/unlock.bin
--rw-r--r--   0        0        0     2643 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/utils.py
--rw-r--r--   0        0        0      675 2024-03-17 21:53:28.318287 gnwmanager-0.9.2/gnwmanager/validation.py
--rw-r--r--   0        0        0     3484 2024-03-17 21:54:58.414572 gnwmanager-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     8949 1970-01-01 00:00:00.000000 gnwmanager-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-17 22:05:49.124149 gnwmanager-0.9.3/LICENSE
+-rw-r--r--   0        0        0     7858 2024-03-17 22:05:49.124149 gnwmanager-0.9.3/README.md
+-rw-r--r--   0        0        0      134 2024-03-17 22:07:18.872622 gnwmanager-0.9.3/gnwmanager/__init__.py
+-rw-r--r--   0        0        0       41 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/__main__.py
+-rw-r--r--   0        0        0      639 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/cli/__init__.py
+-rw-r--r--   0        0        0     2651 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/cli/_debug.py
+-rw-r--r--   0        0        0     2074 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/cli/_dump.py
+-rw-r--r--   0        0        0      981 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/cli/_erase.py
+-rw-r--r--   0        0        0     8092 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/cli/_filesystem.py
+-rw-r--r--   0        0        0     1667 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/cli/_flash.py
+-rw-r--r--   0        0        0     1738 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/cli/_gdb.py
+-rw-r--r--   0        0        0     3739 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/cli/_install.py
+-rw-r--r--   0        0        0     2351 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/cli/_lock.py
+-rw-r--r--   0        0        0     2173 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/cli/_monitor.py
+-rw-r--r--   0        0        0     1769 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/cli/_parsers.py
+-rw-r--r--   0        0        0     2297 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/cli/_pull.py
+-rw-r--r--   0        0        0     3651 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/cli/_push.py
+-rw-r--r--   0        0        0     2545 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/cli/_screenshot.py
+-rw-r--r--   0        0        0     1179 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/cli/_start.py
+-rw-r--r--   0        0        0     5531 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/cli/_unlock.py
+-rw-r--r--   0        0        0     5045 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/cli/devices.py
+-rw-r--r--   0        0        0     8038 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/cli/main.py
+-rw-r--r--   0        0        0     1488 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/elf.py
+-rw-r--r--   0        0        0      262 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/exceptions.py
+-rw-r--r--   0        0        0     3744 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/filesystem.py
+-rwxr-xr-x   0        0        0    35176 2024-03-17 22:07:18.400619 gnwmanager-0.9.3/gnwmanager/firmware.bin
+-rw-r--r--   0        0        0    19845 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/gnw.py
+-rw-r--r--   0        0        0      129 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/ocdbackend/__init__.py
+-rw-r--r--   0        0        0     2380 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/ocdbackend/base.py
+-rw-r--r--   0        0        0    10615 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/ocdbackend/openocd_backend.py
+-rw-r--r--   0        0        0     3511 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/ocdbackend/pyocd_backend.py
+-rw-r--r--   0        0        0        0 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/py.typed
+-rw-r--r--   0        0        0      351 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/status.py
+-rw-r--r--   0        0        0        1 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/target.py
+-rw-r--r--   0        0        0      149 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/time.py
+-rw-r--r--   0        0        0     1288 2024-03-17 22:07:17.536615 gnwmanager-0.9.3/gnwmanager/unlock.bin
+-rw-r--r--   0        0        0     2643 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/utils.py
+-rw-r--r--   0        0        0      675 2024-03-17 22:05:49.136149 gnwmanager-0.9.3/gnwmanager/validation.py
+-rw-r--r--   0        0        0     3484 2024-03-17 22:07:18.872622 gnwmanager-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     8949 1970-01-01 00:00:00.000000 gnwmanager-0.9.3/PKG-INFO
```

### Comparing `gnwmanager-0.9.2/LICENSE` & `gnwmanager-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/README.md` & `gnwmanager-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/cli/__init__.py` & `gnwmanager-0.9.3/gnwmanager/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/cli/_debug.py` & `gnwmanager-0.9.3/gnwmanager/cli/_debug.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/cli/_dump.py` & `gnwmanager-0.9.3/gnwmanager/cli/_dump.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/cli/_erase.py` & `gnwmanager-0.9.3/gnwmanager/cli/_erase.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/cli/_filesystem.py` & `gnwmanager-0.9.3/gnwmanager/cli/_filesystem.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/cli/_flash.py` & `gnwmanager-0.9.3/gnwmanager/cli/_flash.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/cli/_gdb.py` & `gnwmanager-0.9.3/gnwmanager/cli/_gdb.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/cli/_install.py` & `gnwmanager-0.9.3/gnwmanager/cli/_install.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,48 +31,49 @@
     sys.exit(1)
 
 
 @installable_programs
 def openocd(platform: str):
     install_cmds = {
         "linux": {
-            "apt-get": [["sudo", "apt-get", "update"], ["sudo", "apt-get", "install", "openocd"]],
-            "pacman": [["sudo", "pacman", "-Sy", "openocd"]],
-            "yum": [["sudo", "yum", "install", "openocd"]],
-            "dnf": [["sudo", "dnf", "install", "openocd"]],
-            "zypper": [["sudo", "zypper", "install", "openocd"]],
+            "apt-get": [["sudo", "apt-get", "update"], ["sudo", "apt-get", "-y", "install", "openocd"]],
+            "pacman": [["sudo", "pacman", "-Sy", "--noconfirm", "openocd"]],
+            "yum": [["sudo", "yum", "-y", "install", "openocd"]],
+            "dnf": [["sudo", "dnf", "-y", "install", "openocd"]],
+            "zypper": [["sudo", "zypper", "--non-interactive", "install", "openocd"]],
         },
         "darwin": {
             "brew": [["brew", "install", "openocd"]],
         },
         "win32": {
-            "choco": [["choco", "install", "openocd"]],
+            "choco": [["choco", "install", "openocd", "-y"]],
         },
     }
 
     _install_from_available_package_manager(install_cmds[platform])
 
 
 @installable_programs
 def arm_toolchain(platform: str):
     install_cmds = {
         "linux": {
-            "apt-get": [["sudo", "apt-get", "update"], ["sudo", "apt-get", "install", "gcc-arm-none-eabi"]],
-            "pacman": [["sudo", "pacman", "-Sy", "arm-none-eabi-gcc"]],
-            "yum": [["sudo", "yum", "install", "arm-none-eabi-newlib", "arm-none-eabi-gcc-cs"]],
-            "dnf": [["sudo", "dnf", "install", "arm-none-eabi-newlib", "arm-none-eabi-gcc-cs"]],
-            "zypper": [["sudo", "zypper", "install", "cross-arm-none-gcc-cs"]],
+            "apt-get": [["sudo", "apt-get", "update"], ["sudo", "apt-get", "-y", "install", "gcc-arm-none-eabi"]],
+            "pacman": [["sudo", "pacman", "-Sy", "--noconfirm", "arm-none-eabi-gcc"]],
+            "yum": [["sudo", "yum", "-y", "install", "arm-none-eabi-newlib", "arm-none-eabi-gcc-cs"]],
+            "dnf": [["sudo", "dnf", "-y", "install", "arm-none-eabi-newlib", "arm-none-eabi-gcc-cs"]],
+            "zypper": [["sudo", "zypper", "--non-interactive", "install", "cross-arm-none-gcc-cs"]],
         },
         "darwin": {
             "brew": [["brew", "install", "arm-gcc-bin"]],
         },
         "win32": {
-            "choco": [["choco", "install", "gcc-arm-embedded"]],
+            "choco": [["choco", "install", "gcc-arm-embedded", "-y"]],
         },
     }
+
     _install_from_available_package_manager(install_cmds[platform])
 
 
 @app.command
 def install(
     *programs: Path,
     show: Annotated[bool, Parameter(negative=[], show_default=False)] = False,
```

### Comparing `gnwmanager-0.9.2/gnwmanager/cli/_lock.py` & `gnwmanager-0.9.3/gnwmanager/cli/_lock.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/cli/_monitor.py` & `gnwmanager-0.9.3/gnwmanager/cli/_monitor.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/cli/_parsers.py` & `gnwmanager-0.9.3/gnwmanager/cli/_parsers.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/cli/_pull.py` & `gnwmanager-0.9.3/gnwmanager/cli/_pull.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/cli/_push.py` & `gnwmanager-0.9.3/gnwmanager/cli/_push.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/cli/_screenshot.py` & `gnwmanager-0.9.3/gnwmanager/cli/_screenshot.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/cli/_start.py` & `gnwmanager-0.9.3/gnwmanager/cli/_start.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/cli/_unlock.py` & `gnwmanager-0.9.3/gnwmanager/cli/_unlock.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/cli/devices.py` & `gnwmanager-0.9.3/gnwmanager/cli/devices.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/cli/main.py` & `gnwmanager-0.9.3/gnwmanager/cli/main.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/elf.py` & `gnwmanager-0.9.3/gnwmanager/elf.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/filesystem.py` & `gnwmanager-0.9.3/gnwmanager/filesystem.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/firmware.bin` & `gnwmanager-0.9.3/gnwmanager/firmware.bin`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/gnw.py` & `gnwmanager-0.9.3/gnwmanager/gnw.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/ocdbackend/base.py` & `gnwmanager-0.9.3/gnwmanager/ocdbackend/base.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/ocdbackend/openocd_backend.py` & `gnwmanager-0.9.3/gnwmanager/ocdbackend/openocd_backend.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/ocdbackend/pyocd_backend.py` & `gnwmanager-0.9.3/gnwmanager/ocdbackend/pyocd_backend.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/unlock.bin` & `gnwmanager-0.9.3/gnwmanager/unlock.bin`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/utils.py` & `gnwmanager-0.9.3/gnwmanager/utils.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/gnwmanager/validation.py` & `gnwmanager-0.9.3/gnwmanager/validation.py`

 * *Files identical despite different names*

### Comparing `gnwmanager-0.9.2/pyproject.toml` & `gnwmanager-0.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poetry]
 name = "gnwmanager"
-version = "0.9.2"  # Do not change, let poetry-dynamic-versioning handle it.
+version = "0.9.3"  # Do not change, let poetry-dynamic-versioning handle it.
 homepage = "https://github.com/BrianPugh/gnwmanager"
 repository = "https://github.com/BrianPugh/gnwmanager"
 license = "Apache-2.0"
 description = ""
 authors = ["Brian Pugh"]
 readme = "README.md"
 packages = [{include = "gnwmanager"}]
```

### Comparing `gnwmanager-0.9.2/PKG-INFO` & `gnwmanager-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnwmanager
-Version: 0.9.2
+Version: 0.9.3
 Summary: 
 Home-page: https://github.com/BrianPugh/gnwmanager
 License: Apache-2.0
 Author: Brian Pugh
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

