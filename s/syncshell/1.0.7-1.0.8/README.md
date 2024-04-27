# Comparing `tmp/syncshell-1.0.7.tar.gz` & `tmp/syncshell-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncshell-1.0.7.tar", max compression
+gzip compressed data, was "syncshell-1.0.8.tar", max compression
```

## Comparing `syncshell-1.0.7.tar` & `syncshell-1.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2022-06-16 10:22:30.000000 syncshell-1.0.7/LICENSE.txt
--rw-r--r--   0        0        0     3702 2023-04-22 13:57:36.633541 syncshell-1.0.7/README.md
--rw-r--r--   0        0        0     1406 2023-07-05 20:42:23.497807 syncshell-1.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-03 23:49:18.310340 syncshell-1.0.7/syncshell/__init__.py
--rw-r--r--   0        0        0     6652 2023-07-05 20:42:23.498652 syncshell-1.0.7/syncshell/cli.py
--rw-r--r--   0        0        0        0 2022-06-23 08:51:02.381314 syncshell-1.0.7/syncshell/utils/__init__.py
--rw-r--r--   0        0        0     4097 2023-07-05 20:42:23.499263 syncshell-1.0.7/syncshell/utils/config.py
--rw-r--r--   0        0        0      967 2023-07-05 20:42:23.500231 syncshell-1.0.7/syncshell/utils/constants.py
--rw-r--r--   0        0        0      567 2022-06-23 08:51:02.382500 syncshell-1.0.7/syncshell/utils/spinner.py
--rw-r--r--   0        0        0     4752 1970-01-01 00:00:00.000000 syncshell-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-06-16 10:22:30.000000 syncshell-1.0.8/LICENSE.txt
+-rw-r--r--   0        0        0     3858 2024-02-03 18:43:36.969331 syncshell-1.0.8/README.md
+-rw-r--r--   0        0        0     1326 2024-04-04 14:41:26.264598 syncshell-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-03 23:49:18.310340 syncshell-1.0.8/syncshell/__init__.py
+-rw-r--r--   0        0        0     6676 2024-04-27 19:10:14.398635 syncshell-1.0.8/syncshell/cli.py
+-rw-r--r--   0        0        0        0 2022-06-23 08:51:02.381314 syncshell-1.0.8/syncshell/utils/__init__.py
+-rw-r--r--   0        0        0     4065 2024-04-27 19:10:14.399397 syncshell-1.0.8/syncshell/utils/config.py
+-rw-r--r--   0        0        0      967 2024-04-27 18:38:41.984933 syncshell-1.0.8/syncshell/utils/constants.py
+-rw-r--r--   0        0        0      569 2024-04-27 19:10:14.400071 syncshell-1.0.8/syncshell/utils/spinner.py
+-rw-r--r--   0        0        0     4958 1970-01-01 00:00:00.000000 syncshell-1.0.8/PKG-INFO
```

### Comparing `syncshell-1.0.7/LICENSE.txt` & `syncshell-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `syncshell-1.0.7/README.md` & `syncshell-1.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -59,35 +59,43 @@
 
 ```bash
 $ syncshell
 Type:        Application
 String form: <syncshell.cli.Application object at 0x101b1ff10>
 Docstring:   SyncShell CLI Application
 
-Usage:       syncshell 
+Usage:       syncshell
              syncshell auth
              syncshell download
              syncshell upload
 ```
 
 ## How it Works
 
 SyncShell is a tool that synchronizes shell history across all devices by securely storing the history file on Github Gist. Github Gist provides two types of Gists, `public` and `secret`. When the `syncshell upload` command is executed, the shell history file is uploaded and stored securely on Github Gist as a secret Gist. To download the uploaded shell history on other devices, the `syncshell download` command is used. This command retrieves the previously uploaded Gist, allowing the user to access their shell history on any device.
 
 **Security:** A Gist will be secret until it's not shared and will be secret and safe until you only have the Github Token and Gist ID.
 
 **Privacy:** In case of having password or secret in a history file, Its suggested to first have a alignment with privacy policies for any usecase.
 
 ## Contributing
-Appreciate the contribution to this repository.
 
-To contribute, you need to follow the below steps for suggesting a change or a new feature:
+I would love to have your help in making SyncShell idea better and expand it capabilities.
+
+### Branching
+
+- `main` is being used for the latest development version.
+- `release` is being used for the latest stable version.
+
+
+### Pull Requests
+To contribute follow the below steps:
 
 1. Install [poetry](https://python-poetry.org/docs/#installation) as a dependency manager
-2. Install dependencies by running ```poetry install```
+2. Install dependencies by running ```poetry shell && poetry install```
 3. Make your changes
 4. Run and debug your changes by running ```poetry run python syncshell```
 5. Run tests by running ```poetry run pytest -c pytest.ini -s```
 6. Submit a pull request
 
 ## License
 The code is licensed under the MIT License. See the data's [LICENSE](https://github.com/msudgh/syncshell/blob/main/LICENSE) file for more information.
```

#### html2text {}

```diff
@@ -24,16 +24,18 @@
 history file is uploaded and stored securely on Github Gist as a secret Gist.
 To download the uploaded shell history on other devices, the `syncshell
 download` command is used. This command retrieves the previously uploaded Gist,
 allowing the user to access their shell history on any device. **Security:** A
 Gist will be secret until it's not shared and will be secret and safe until you
 only have the Github Token and Gist ID. **Privacy:** In case of having password
 or secret in a history file, Its suggested to first have a alignment with
-privacy policies for any usecase. ## Contributing Appreciate the contribution
-to this repository. To contribute, you need to follow the below steps for
-suggesting a change or a new feature: 1. Install [poetry](https://python-
-poetry.org/docs/#installation) as a dependency manager 2. Install dependencies
-by running ```poetry install``` 3. Make your changes 4. Run and debug your
-changes by running ```poetry run python syncshell``` 5. Run tests by running
-```poetry run pytest -c pytest.ini -s``` 6. Submit a pull request ## License
-The code is licensed under the MIT License. See the data's [LICENSE](https://
-github.com/msudgh/syncshell/blob/main/LICENSE) file for more information.
+privacy policies for any usecase. ## Contributing I would love to have your
+help in making SyncShell idea better and expand it capabilities. ### Branching
+- `main` is being used for the latest development version. - `release` is being
+used for the latest stable version. ### Pull Requests To contribute follow the
+below steps: 1. Install [poetry](https://python-poetry.org/docs/#installation)
+as a dependency manager 2. Install dependencies by running ```poetry shell &&
+poetry install``` 3. Make your changes 4. Run and debug your changes by running
+```poetry run python syncshell``` 5. Run tests by running ```poetry run pytest
+-c pytest.ini -s``` 6. Submit a pull request ## License The code is licensed
+under the MIT License. See the data's [LICENSE](https://github.com/msudgh/
+syncshell/blob/main/LICENSE) file for more information.
```

### Comparing `syncshell-1.0.7/pyproject.toml` & `syncshell-1.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "syncshell"
-version = "v1.0.7"
+version = "v1.0.8"
 description = "Keep your machine's shell history synchronized"
 license = "MIT"
 authors = ["Masoud Ghorbani <masoudghorbani@pm.me>"]
 readme = "README.md"
 repository = "https://github.com/msudgh/syncshell"
 homepage = "https://github.com/msudgh/syncshell"
 keywords = ["sync", "shell", "history", "bash", "zsh"]
 include = [
     { path = ".syncshell.ini", format = "wheel" },
     { path = "README.md", format = "wheel" },
-    { path = "pyproject.toml", format = "wheel" }
+    { path = "pyproject.toml", format = "wheel" },
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -24,31 +24,21 @@
     "Natural Language :: English",
     "Topic :: Utilities",
     "Topic :: System :: Shells",
     "Topic :: Software Development",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8.16"
-fire = "0.5.0"
+python = "^3.8.18"
+fire = "0.6.0"
 halo = "0.0.31"
-PyGithub = "1.59.0"
+PyGithub = "2.3.0"
 
 [tool.poetry.group.dev.dependencies]
-flake8 = "^6.0.0"
-black = "23.3.0"
-pytest = "7.4.0"
+pytest = "8.1.1"
 pytest-testdox = "^3.0.1"
-
-[tool.black]
-py36 = true
-include = '\.pyi?$'
-exclude = '''
-/(
-    \.git
-    | dist
-)/
-'''
+ruff = ">=0.1.5,<0.4.0"
+pre-commit = "^3.5.0"
 
 # Ref: https://python-poetry.org/docs/pyproject/#scripts
 [tool.poetry.scripts]
 syncshell = "syncshell.cli:main"
```

### Comparing `syncshell-1.0.7/syncshell/cli.py` & `syncshell-1.0.8/syncshell/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,73 +28,73 @@
 
         files[history_file["path"]] = InputFileContent(history_file["content"])
         files[config_file["path"]] = InputFileContent(config_file["content"])
 
         return files
 
     def auth(self):
-        """Retrieve & authenticate user token"""
+        """Retrieve & authenticate user's token"""
         try:
             # Help message
             getting_started = textwrap.fill(constants.HELP_MESSAGE, width=80)
             print(getting_started)
 
-            # Promte token key
+            # Prompt token key
             prompt_token = input("Enter your Github token key: ")
             config.parser["Auth"]["token"] = str(prompt_token)
 
             # Set new token key
-            config.gist = Github(config.parser["Auth"]["token"])
+            config.github = Github(config.parser["Auth"]["token"])
 
             spinner = Spinner.NewTask("Check authentication...")
 
-            # Write config file if Github user alreaded authorized
+            # Write config file if Github user already authorized
             if config.is_logged_in():
                 spinner.succeed("Your Github token key is authenticated.")
-                config.write()
+                config.save_config()
             else:
                 spinner.fail("Your Github token key is not valid.")
                 sys.exit(1)
         except KeyboardInterrupt:
             sys.exit(0)
 
     def upload(self):
-        """Upload current history"""
+        """Upload history and config file to Gist"""
         spinner = Spinner.NewTask("Uploading ...")
 
         # Exit process if not logged in
         if not config.is_logged_in():
             spinner.fail("Your Github token key is not valid. Authenticate first.")
             sys.exit(1)
 
         try:
             if config.parser["Auth"]["gist_id"]:
-                gist = config.gist.get_gist(config.parser["Auth"]["gist_id"])
+                gist = config.github.get_gist(config.parser["Auth"]["gist_id"])
 
                 # Set upload date
                 config.parser["Upload"]["last_date"] = str(int(time.time()))
-                config.write()
+                config.save_config()
 
                 files = self.__prepare_payload()
 
                 gist.edit(files=files)
 
                 spinner.succeed(f"Gist ID ({gist.id}) updated.")
             else:
                 description = "SyncShell Gist"
 
-                user = config.gist.get_user()
+                user = config.github.get_user()
                 files = self.__prepare_payload()
                 gist = user.create_gist(False, files, description)
 
                 # Set upload date
                 config.parser["Upload"]["last_date"] = str(int(time.time()))
                 config.parser["Auth"]["gist_id"] = gist.id
 
-                config.write()
+                config.save_config()
 
                 files = self.__prepare_payload()
                 gist.edit(files=files)
                 spinner.succeed(f"New Gist ID ({gist.id}) created.")
         except FileNotFoundError:
             spinner.fail("Couldn't find history file.")
             sys.exit(1)
@@ -106,53 +106,52 @@
                 spinner.fail(
                     "Gist ID not found. If you manually deleted Gist "
                     "in past then try to execute upload command "
                     "again for new upload and sync."
                 )
 
                 config.parser["Auth"]["gist_id"] = ""
-                config.write()
+                config.save_config()
             sys.exit(1)
 
     def download(self):
-        """Download Gist and save it to history file"""
+        """Download history and config file from Gist"""
 
         try:
             token = str(input("Enter your Github token key: "))
             gist_id = str(input("Enter your Gist ID: "))
 
             spinner = Spinner.NewTask("Downloading ...")
 
             # Redefine Github instance with new token
-            config.gist = Github(token)
+            config.github = Github(token)
 
             # Exit process if not logged in
             if not config.is_logged_in():
                 sys.exit(1)
 
             # Download Gist object
-            gist = config.gist.get_gist(gist_id)
+            gist = config.github.get_gist(gist_id)
 
             if len(gist.files) != 2:
                 spinner.fail("Gist content corrupted, Please use another Gist.")
                 sys.exit(1)
 
             # Read new configuration
             temp_config = ConfigParser()
             temp_config.read_string(gist.files[constants.CONFIG_FILENAME].content)
 
             # Check shell names
             if temp_config["Shell"]["name"] != config.parser["Shell"]["name"]:
                 spinner.fail("Unable to convert different shells")
                 sys.exit(1)
 
-            # Write configuration
             config.parser["Auth"]["token"] = token
             config.parser["Auth"]["gist_id"] = gist_id
-            config.write()
+            config.save_config()
 
             history_file = config.get_shell_history()
             history_content = history_file["content"]
 
             new_changes = gist.files[
                 constants.SUPPORTED_SHELLS[config.parser["Shell"]["name"]]
             ]
```

### Comparing `syncshell-1.0.7/syncshell/utils/config.py` & `syncshell-1.0.8/syncshell/utils/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from configparser import ConfigParser, Error as ConfigParserError
 from github import Github, GithubException
 from github import Auth
 from syncshell.utils import constants
 
 
 class SyncShellConfig:
-    """Config class consits of fundamental methods to read, save and validate
+    """Config class consists of fundamental methods to read, save and validate
     config file for different scenarios of syncshell.
     """
 
     def __init__(self, path=constants.CONFIG_PATH):
         """Constructor
 
         Return configuration placed in config default path
@@ -23,16 +23,15 @@
         Keyword arguments:
         path -- the config file path
         """
         self.path = path
         self.parser = ConfigParser()
         self.github = None
 
-        # Copy template config file to home directory
-        if os.path.exists(constants.CONFIG_PATH) is False:
+        if os.path.exists(path) is False or os.path.getsize(path) == 0:
             copy(constants.CONFIG_PATH_TEMPLATE, constants.CONFIG_PATH)
 
     def __deepcopy__(self, memo):
         return self
 
     def read_config(self):
         """Read and parse config file and config object"""
@@ -109,23 +108,23 @@
 
     def write_shell_history(self, content):
         """Write shell history content"""
         try:
             with open(self.parser["Shell"]["path"], "w") as history_file:
                 history_file.write(content)
                 return True
-        except:
+        except IOError:
             return False
 
     def get_config(self):
         """Return config file path and content"""
         with open(self.path, "r") as config_file:
             config_file_path = os.path.basename(config_file.name)
 
-            # Remove token key on uplaod
+            # Remove token key on upload
             lines = config_file.readlines()
             lines.pop(1)
 
             return {
                 "path": config_file_path,
                 "content": "".join(map(str, lines)),
             }
```

### Comparing `syncshell-1.0.7/syncshell/utils/constants.py` & `syncshell-1.0.8/syncshell/utils/constants.py`

 * *Files identical despite different names*

### Comparing `syncshell-1.0.7/syncshell/utils/spinner.py` & `syncshell-1.0.8/syncshell/utils/spinner.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     __spinner = None
 
     def __init__(self, text, spinner="dots"):
         self.__spinner = Halo(text=text, spinner=spinner)
         self.__spinner.start()
 
     def succeed(self, text):
-        """Overide Halo succeed method"""
+        """Override Halo succeed method"""
         self.__spinner.succeed(text)
         self.__spinner.stop()
 
     def fail(self, text):
-        """Overide Halo fail method"""
+        """Override Halo fail method"""
         self.__spinner.fail(text)
         self.__spinner.stop()
```

### Comparing `syncshell-1.0.7/PKG-INFO` & `syncshell-1.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: syncshell
-Version: 1.0.7
+Version: 1.0.8
 Summary: Keep your machine's shell history synchronized
 Home-page: https://github.com/msudgh/syncshell
 License: MIT
 Keywords: sync,shell,history,bash,zsh
 Author: Masoud Ghorbani
 Author-email: masoudghorbani@pm.me
-Requires-Python: >=3.8.16,<4.0.0
+Requires-Python: >=3.8.18,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: Utilities
-Requires-Dist: PyGithub (==1.59.0)
-Requires-Dist: fire (==0.5.0)
+Requires-Dist: PyGithub (==2.3.0)
+Requires-Dist: fire (==0.6.0)
 Requires-Dist: halo (==0.0.31)
 Project-URL: Repository, https://github.com/msudgh/syncshell
 Description-Content-Type: text/markdown
 
 # SyncShell
 <!-- License -->
 <a href="https://mit-license.org/msudgh">
@@ -87,35 +88,43 @@
 
 ```bash
 $ syncshell
 Type:        Application
 String form: <syncshell.cli.Application object at 0x101b1ff10>
 Docstring:   SyncShell CLI Application
 
-Usage:       syncshell 
+Usage:       syncshell
              syncshell auth
              syncshell download
              syncshell upload
 ```
 
 ## How it Works
 
 SyncShell is a tool that synchronizes shell history across all devices by securely storing the history file on Github Gist. Github Gist provides two types of Gists, `public` and `secret`. When the `syncshell upload` command is executed, the shell history file is uploaded and stored securely on Github Gist as a secret Gist. To download the uploaded shell history on other devices, the `syncshell download` command is used. This command retrieves the previously uploaded Gist, allowing the user to access their shell history on any device.
 
 **Security:** A Gist will be secret until it's not shared and will be secret and safe until you only have the Github Token and Gist ID.
 
 **Privacy:** In case of having password or secret in a history file, Its suggested to first have a alignment with privacy policies for any usecase.
 
 ## Contributing
-Appreciate the contribution to this repository.
 
-To contribute, you need to follow the below steps for suggesting a change or a new feature:
+I would love to have your help in making SyncShell idea better and expand it capabilities.
+
+### Branching
+
+- `main` is being used for the latest development version.
+- `release` is being used for the latest stable version.
+
+
+### Pull Requests
+To contribute follow the below steps:
 
 1. Install [poetry](https://python-poetry.org/docs/#installation) as a dependency manager
-2. Install dependencies by running ```poetry install```
+2. Install dependencies by running ```poetry shell && poetry install```
 3. Make your changes
 4. Run and debug your changes by running ```poetry run python syncshell```
 5. Run tests by running ```poetry run pytest -c pytest.ini -s```
 6. Submit a pull request
 
 ## License
 The code is licensed under the MIT License. See the data's [LICENSE](https://github.com/msudgh/syncshell/blob/main/LICENSE) file for more information.
```

#### html2text {}

```diff
@@ -1,52 +1,55 @@
-Metadata-Version: 2.1 Name: syncshell Version: 1.0.7 Summary: Keep your
+Metadata-Version: 2.1 Name: syncshell Version: 1.0.8 Summary: Keep your
 machine's shell history synchronized Home-page: https://github.com/msudgh/
 syncshell License: MIT Keywords: sync,shell,history,bash,zsh Author: Masoud
-Ghorbani Author-email: masoudghorbani@pm.me Requires-Python: >=3.8.16,<4.0.0
+Ghorbani Author-email: masoudghorbani@pm.me Requires-Python: >=3.8.18,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Topic :: Software Development Classifier: Topic :: System :: Shells Classifier:
-Topic :: Utilities Requires-Dist: PyGithub (==1.59.0) Requires-Dist: fire
-(==0.5.0) Requires-Dist: halo (==0.0.31) Project-URL: Repository, https://
-github.com/msudgh/syncshell Description-Content-Type: text/markdown # SyncShell
-_[_M_I_T_ _L_i_c_e_n_s_e_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_P_y_P_i_]_[_P_y_P_i_]SyncShell as a simple and secure tool
-allows to synchronize machine's shell history across devices. It's built on top
-of Github Gist and written in Python (CLI). With SyncShell, you no longer have
-to worry about manually syncing your office and home machine's shell history
-and let continue where the terminal session left. ## Features - Sync your shell
-history across all your devices - Securely store your shell history on Github
-Gist - Support for `zsh` and `bash` shells - Easy to install and use ##
-Installation To install SyncShell, simply run the following command: ```bash $
-pip install syncshell ``` ## Usage To use SyncShell, It first needs to set up a
-Github token key by following these steps: 1. Open [**Github personal access
-tokens**](https://github.com/settings/tokens) page, [**Generate a new token**]
-(https://github.com/settings/tokens/new) with `gist` scope feature. 2. Execute
-the **`syncshell auth`** command, Enter the token key to validate and confirm
-it. Once finished, try to upload shell history by the following command:
-```bash $ syncshell upload ``` After uploading, the download command lets to
-sync and pull changes on the other machines: ```bash $ syncshell download ```
-### Synopsis ```bash $ syncshell Type: Application String form:
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Topic :: Software Development
+Classifier: Topic :: System :: Shells Classifier: Topic :: Utilities Requires-
+Dist: PyGithub (==2.3.0) Requires-Dist: fire (==0.6.0) Requires-Dist: halo
+(==0.0.31) Project-URL: Repository, https://github.com/msudgh/syncshell
+Description-Content-Type: text/markdown # SyncShell _[_M_I_T_ _L_i_c_e_n_s_e_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]
+_[_P_y_P_i_]_[_P_y_P_i_]SyncShell as a simple and secure tool allows to synchronize
+machine's shell history across devices. It's built on top of Github Gist and
+written in Python (CLI). With SyncShell, you no longer have to worry about
+manually syncing your office and home machine's shell history and let continue
+where the terminal session left. ## Features - Sync your shell history across
+all your devices - Securely store your shell history on Github Gist - Support
+for `zsh` and `bash` shells - Easy to install and use ## Installation To
+install SyncShell, simply run the following command: ```bash $ pip install
+syncshell ``` ## Usage To use SyncShell, It first needs to set up a Github
+token key by following these steps: 1. Open [**Github personal access tokens**]
+(https://github.com/settings/tokens) page, [**Generate a new token**](https://
+github.com/settings/tokens/new) with `gist` scope feature. 2. Execute the
+**`syncshell auth`** command, Enter the token key to validate and confirm it.
+Once finished, try to upload shell history by the following command: ```bash $
+syncshell upload ``` After uploading, the download command lets to sync and
+pull changes on the other machines: ```bash $ syncshell download ``` ###
+Synopsis ```bash $ syncshell Type: Application String form:
 x101b1ff10> Docstring: SyncShell CLI Application Usage: syncshell syncshell
 auth syncshell download syncshell upload ``` ## How it Works SyncShell is a
 tool that synchronizes shell history across all devices by securely storing the
 history file on Github Gist. Github Gist provides two types of Gists, `public`
 and `secret`. When the `syncshell upload` command is executed, the shell
 history file is uploaded and stored securely on Github Gist as a secret Gist.
 To download the uploaded shell history on other devices, the `syncshell
 download` command is used. This command retrieves the previously uploaded Gist,
 allowing the user to access their shell history on any device. **Security:** A
 Gist will be secret until it's not shared and will be secret and safe until you
 only have the Github Token and Gist ID. **Privacy:** In case of having password
 or secret in a history file, Its suggested to first have a alignment with
-privacy policies for any usecase. ## Contributing Appreciate the contribution
-to this repository. To contribute, you need to follow the below steps for
-suggesting a change or a new feature: 1. Install [poetry](https://python-
-poetry.org/docs/#installation) as a dependency manager 2. Install dependencies
-by running ```poetry install``` 3. Make your changes 4. Run and debug your
-changes by running ```poetry run python syncshell``` 5. Run tests by running
-```poetry run pytest -c pytest.ini -s``` 6. Submit a pull request ## License
-The code is licensed under the MIT License. See the data's [LICENSE](https://
-github.com/msudgh/syncshell/blob/main/LICENSE) file for more information.
+privacy policies for any usecase. ## Contributing I would love to have your
+help in making SyncShell idea better and expand it capabilities. ### Branching
+- `main` is being used for the latest development version. - `release` is being
+used for the latest stable version. ### Pull Requests To contribute follow the
+below steps: 1. Install [poetry](https://python-poetry.org/docs/#installation)
+as a dependency manager 2. Install dependencies by running ```poetry shell &&
+poetry install``` 3. Make your changes 4. Run and debug your changes by running
+```poetry run python syncshell``` 5. Run tests by running ```poetry run pytest
+-c pytest.ini -s``` 6. Submit a pull request ## License The code is licensed
+under the MIT License. See the data's [LICENSE](https://github.com/msudgh/
+syncshell/blob/main/LICENSE) file for more information.
```

