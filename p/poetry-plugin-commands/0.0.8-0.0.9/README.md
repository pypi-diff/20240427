# Comparing `tmp/poetry_plugin_commands-0.0.8.tar.gz` & `tmp/poetry_plugin_commands-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_commands-0.0.8.tar", max compression
+gzip compressed data, was "poetry_plugin_commands-0.0.9.tar", max compression
```

## Comparing `poetry_plugin_commands-0.0.8.tar` & `poetry_plugin_commands-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11324 2024-04-07 18:26:56.337907 poetry_plugin_commands-0.0.8/LICENSE
--rw-r--r--   0        0        0     1926 2024-04-09 00:19:07.509029 poetry_plugin_commands-0.0.8/README.md
--rw-r--r--   0        0        0     3231 2024-04-09 01:02:11.504884 poetry_plugin_commands-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      170 2024-04-07 16:47:18.853243 poetry_plugin_commands-0.0.8/src/poetry_plugin_commands/__init__.py
--rw-r--r--   0        0        0     1112 2024-04-09 01:03:12.116881 poetry_plugin_commands-0.0.8/src/poetry_plugin_commands/command.py
--rw-r--r--   0        0        0     1637 2024-04-09 01:03:26.193880 poetry_plugin_commands-0.0.8/src/poetry_plugin_commands/plugins.py
--rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 poetry_plugin_commands-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11324 2024-04-07 18:26:56.337907 poetry_plugin_commands-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1926 2024-04-09 00:19:07.509029 poetry_plugin_commands-0.0.9/README.md
+-rw-r--r--   0        0        0     3214 2024-04-28 11:48:56.075545 poetry_plugin_commands-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      170 2024-04-07 16:47:18.853243 poetry_plugin_commands-0.0.9/src/poetry_plugin_commands/__init__.py
+-rw-r--r--   0        0        0     1112 2024-04-09 01:03:12.116881 poetry_plugin_commands-0.0.9/src/poetry_plugin_commands/command.py
+-rw-r--r--   0        0        0     1756 2024-04-28 11:48:02.525548 poetry_plugin_commands-0.0.9/src/poetry_plugin_commands/plugins.py
+-rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 poetry_plugin_commands-0.0.9/PKG-INFO
```

### Comparing `poetry_plugin_commands-0.0.8/LICENSE` & `poetry_plugin_commands-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_commands-0.0.8/README.md` & `poetry_plugin_commands-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `poetry_plugin_commands-0.0.8/pyproject.toml` & `poetry_plugin_commands-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-commands"
-version = "0.0.8"
+version = "0.0.9"
 description = "Poetry plugin for simple custom user commands execution."
 readme = "README.md"
 authors = ["BlackCatDevel0per <bcdev@mail.ru>"]
 license = "Apache 2.0"
 
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
@@ -139,15 +139,14 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 poetry = "^1.8.0"
 poetry-core = "^1.7.0"
 
 [tool.poetry.group.fancy]
-optional = false
 
 [tool.poetry.group.fancy.dependencies]
 rich = "^13.7.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.2"
 pytest-dependency = "^0.5.1"
```

### Comparing `poetry_plugin_commands-0.0.8/src/poetry_plugin_commands/command.py` & `poetry_plugin_commands-0.0.9/src/poetry_plugin_commands/command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_commands-0.0.8/src/poetry_plugin_commands/plugins.py` & `poetry_plugin_commands-0.0.9/src/poetry_plugin_commands/plugins.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 
 		User's commands are auto-generated from toml plugin's section shell commands.
 		"""
 		toml_content: dict[str, Any] = self.poetry.pyproject.data
 
 		# TODO: Exec field or catch options of poetry's run command (mb better make something like crun?)
 		# TODO: Make profiles for ux..
-		user_commands = toml_content['tool'][self.plugin_section]
+		user_commands = toml_content.get('tool', {}).get(self.plugin_section)
+		if not user_commands:
+			return [UserCommand._new_cls('help', 'echo not implemented..')]  # noqa: SLF001
 
 		# TODO: Support python commands using toml's optioned values..
 		commands = [
 			UserCommand._new_cls(alias, command)  # noqa: SLF001
 			for alias, command in user_commands.items()
 		]
```

### Comparing `poetry_plugin_commands-0.0.8/PKG-INFO` & `poetry_plugin_commands-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-commands
-Version: 0.0.8
+Version: 0.0.9
 Summary: Poetry plugin for simple custom user commands execution.
 License: Apache 2.0
 Author: BlackCatDevel0per
 Author-email: bcdev@mail.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

