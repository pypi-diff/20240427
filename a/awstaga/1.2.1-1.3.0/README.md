# Comparing `tmp/awstaga-1.2.1.tar.gz` & `tmp/awstaga-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awstaga-1.2.1.tar", max compression
+gzip compressed data, was "awstaga-1.3.0.tar", max compression
```

## Comparing `awstaga-1.2.1.tar` & `awstaga-1.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11345 2023-12-12 20:00:52.202959 awstaga-1.2.1/LICENSE
--rw-r--r--   0        0        0     8656 2023-12-12 20:00:52.202959 awstaga-1.2.1/README.md
--rw-r--r--   0        0        0     3845 2023-12-12 20:00:52.202959 awstaga-1.2.1/awstaga/__init__.py
--rw-r--r--   0        0        0     2785 2023-12-12 20:00:52.202959 awstaga-1.2.1/awstaga/config.py
--rw-r--r--   0        0        0      368 2023-12-12 20:00:52.202959 awstaga-1.2.1/awstaga/logger.py
--rw-r--r--   0        0        0       62 2023-12-12 20:00:52.202959 awstaga-1.2.1/awstaga/models/__init__.py
--rw-r--r--   0        0        0      906 2023-12-12 20:00:52.202959 awstaga-1.2.1/awstaga/models/resource.py
--rw-r--r--   0        0        0      774 2023-12-12 20:00:52.202959 awstaga-1.2.1/awstaga/models/tag.py
--rw-r--r--   0        0        0      536 2023-12-12 20:00:52.202959 awstaga-1.2.1/awstaga/models/tagset.py
--rw-r--r--   0        0        0     1265 2023-12-12 20:00:52.202959 awstaga-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     9753 1970-01-01 00:00:00.000000 awstaga-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-04-27 05:40:37.043499 awstaga-1.3.0/LICENSE
+-rw-r--r--   0        0        0     8786 2024-04-27 05:40:37.043499 awstaga-1.3.0/README.md
+-rw-r--r--   0        0        0     3886 2024-04-27 05:40:37.043499 awstaga-1.3.0/awstaga/__init__.py
+-rw-r--r--   0        0        0     2785 2024-04-27 05:40:37.043499 awstaga-1.3.0/awstaga/config.py
+-rw-r--r--   0        0        0      368 2024-04-27 05:40:37.043499 awstaga-1.3.0/awstaga/logger.py
+-rw-r--r--   0        0        0       76 2024-04-27 05:40:37.043499 awstaga-1.3.0/awstaga/models/__init__.py
+-rw-r--r--   0        0        0      906 2024-04-27 05:40:37.043499 awstaga-1.3.0/awstaga/models/resource.py
+-rw-r--r--   0        0        0      774 2024-04-27 05:40:37.043499 awstaga-1.3.0/awstaga/models/tag.py
+-rw-r--r--   0        0        0      536 2024-04-27 05:40:37.043499 awstaga-1.3.0/awstaga/models/tagset.py
+-rw-r--r--   0        0        0     1248 2024-04-27 05:40:37.043499 awstaga-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9855 1970-01-01 00:00:00.000000 awstaga-1.3.0/PKG-INFO
```

### Comparing `awstaga-1.2.1/LICENSE` & `awstaga-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `awstaga-1.2.1/README.md` & `awstaga-1.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 <img align="right" src="https://raw.github.com/cliffano/awstaga/main/avatar.jpg" alt="Avatar"/>
 
 [![Build Status](https://github.com/cliffano/awstaga/workflows/CI/badge.svg)](https://github.com/cliffano/awstaga/actions?query=workflow%3ACI)
 [![Security Status](https://snyk.io/test/github/cliffano/awstaga/badge.svg)](https://snyk.io/test/github/cliffano/awstaga)
+[![Dependencies Status](https://img.shields.io/librariesio/release/pypi/awstaga)](https://libraries.io/github/cliffano/awstaga)
 [![Published Version](https://img.shields.io/pypi/v/awstaga.svg)](https://pypi.python.org/pypi/awstaga)
 <br/>
 
 Awstaga
 -------
 
-Awstaga is a Python CLI for tagging AWS resources based on a YAML configuration.
+Awstaga is a Python CLI for tagging AWS resources defined in a YAML configuration.
 
 This package is intended as a companion for [AWS Tag Editor](https://docs.aws.amazon.com/tag-editor/latest/userguide/tagging-resources.html). While AWS Tag Editor is useful for tagging multiple resources in one go, it has no easy way to re-run the tagging since you have to use the AWS console UI, and its resource filtering capability is quite limited, making it hard to select resources with-more-than basic logic.
 
 Using Awstaga, you can easily re-run the tagging by running the CLI again. And with its support of YAML configuration, it allows you to define multiple tagsets which you can reuse and mix and match with the resources, you can construct your own mapping between the resources and the relevant tags and tagsets. You can generate your own YAML configuration using Python scripts, or any other programming language, allowing you to construct a more complex filtering logic.
 
 Installation
 ------------
```

### Comparing `awstaga-1.2.1/awstaga/__init__.py` & `awstaga-1.3.0/awstaga/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,19 +76,19 @@
                 logger.error(f'{resource_arn}: '\
                              f'{error.get("StatusCode")} - '\
                              f'{error.get("ErrorCode")} - '\
                              f'{error.get("ErrorMessage")}')
         time.sleep(delay)
 
 @click.command()
-@click.option('--conf-file', default='awstaga.yaml', show_default=True,
+@click.option('--conf-file', default='awstaga.yaml', show_default=True, type=str,
               help='Configuration file path')
-@click.option('--dry-run', is_flag=True, default=False, show_default=True,
+@click.option('--dry-run', is_flag=True, default=False, show_default=True, type=bool,
               help='When dry run is enabled, no tags are applied')
-@click.option('--batch-size', default=5, show_default=True,
+@click.option('--batch-size', default=5, show_default=True, type=int,
               help='Number of resources to tag in one go per batch')
-@click.option('--delay', default=2, show_default=True,
+@click.option('--delay', default=2, show_default=True, type=int,
               help='Delay in seconds after tagging each batch')
 def cli(conf_file: str, dry_run: bool, batch_size: int, delay: int) -> None:
     """Python CLI for tagging AWS resources based on a YAML configuration.
     """
     apply(conf_file, dry_run, batch_size, delay)
```

### Comparing `awstaga-1.2.1/awstaga/config.py` & `awstaga-1.3.0/awstaga/config.py`

 * *Files identical despite different names*

### Comparing `awstaga-1.2.1/awstaga/models/resource.py` & `awstaga-1.3.0/awstaga/models/resource.py`

 * *Files identical despite different names*

### Comparing `awstaga-1.2.1/awstaga/models/tag.py` & `awstaga-1.3.0/awstaga/models/tag.py`

 * *Files identical despite different names*

### Comparing `awstaga-1.2.1/awstaga/models/tagset.py` & `awstaga-1.3.0/awstaga/models/tagset.py`

 * *Files identical despite different names*

### Comparing `awstaga-1.2.1/pyproject.toml` & `awstaga-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [installer]
 no-binary = [ ":none:" ]
 
 [tool.poetry]
 name = "awstaga"
-version = "1.2.1"
+version = "1.3.0"
 description = "Python CLI for tagging AWS resources based on a YAML configuration"
 license = "Apache-2.0"
 authors = [ "Cliffano Subagio <cliffano@gmail.com>" ]
 readme = "README.md"
 homepage = "https://github.com/cliffano/awstaga"
 repository = "https://github.com/cliffano/awstaga"
 documentation = "https://github.com/cliffano/awstaga"
@@ -26,27 +26,26 @@
   include = "awstaga"
 
   [tool.poetry.scripts]
   awstaga = "awstaga:cli"
 
   [tool.poetry.dependencies]
   python = "^3.8"
-  boto3 = "^1.26.155"
-  click = "^8.1.3"
-  conflog = "^1.5.1"
-  PyYAML = "^6.0.1"
-  pyyaml-include = "^1.3.1"
+  boto3 = "1.26.155"
+  click = "8.1.3"
+  conflog = "1.5.1"
+  PyYAML = "6.0.1"
+  pyyaml-include = "^1.3.2"
 
 [tool.poetry.group.dev.dependencies]
-twine = "4.0.2"
+twine = "4.0.0"
 wheel = "0.40.0"
-yq = "3.2.2"
 
 [tool.poetry.group.test.dependencies]
-coverage = "7.2.4"
+coverage = "7.2.3"
 pylint = "3.0.1"
 pytest = "7.3.1"
 wily = "1.24.0"
 
 [tool.poetry.group.doc.dependencies]
 pylint-report = "2.4.0"
 pytest-html = "3.2.0"
```

### Comparing `awstaga-1.2.1/PKG-INFO` & `awstaga-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awstaga
-Version: 1.2.1
+Version: 1.3.0
 Summary: Python CLI for tagging AWS resources based on a YAML configuration
 Home-page: https://github.com/cliffano/awstaga
 License: Apache-2.0
 Keywords: awstaga,aws,tag,tagging
 Author: Cliffano Subagio
 Author-email: cliffano@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -12,34 +12,35 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
-Requires-Dist: boto3 (>=1.26.155,<2.0.0)
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: conflog (>=1.5.1,<2.0.0)
-Requires-Dist: pyyaml-include (>=1.3.1,<2.0.0)
+Requires-Dist: PyYAML (==6.0.1)
+Requires-Dist: boto3 (==1.26.155)
+Requires-Dist: click (==8.1.3)
+Requires-Dist: conflog (==1.5.1)
+Requires-Dist: pyyaml-include (>=1.3.2,<2.0.0)
 Project-URL: Documentation, https://github.com/cliffano/awstaga
 Project-URL: Repository, https://github.com/cliffano/awstaga
 Description-Content-Type: text/markdown
 
 <img align="right" src="https://raw.github.com/cliffano/awstaga/main/avatar.jpg" alt="Avatar"/>
 
 [![Build Status](https://github.com/cliffano/awstaga/workflows/CI/badge.svg)](https://github.com/cliffano/awstaga/actions?query=workflow%3ACI)
 [![Security Status](https://snyk.io/test/github/cliffano/awstaga/badge.svg)](https://snyk.io/test/github/cliffano/awstaga)
+[![Dependencies Status](https://img.shields.io/librariesio/release/pypi/awstaga)](https://libraries.io/github/cliffano/awstaga)
 [![Published Version](https://img.shields.io/pypi/v/awstaga.svg)](https://pypi.python.org/pypi/awstaga)
 <br/>
 
 Awstaga
 -------
 
-Awstaga is a Python CLI for tagging AWS resources based on a YAML configuration.
+Awstaga is a Python CLI for tagging AWS resources defined in a YAML configuration.
 
 This package is intended as a companion for [AWS Tag Editor](https://docs.aws.amazon.com/tag-editor/latest/userguide/tagging-resources.html). While AWS Tag Editor is useful for tagging multiple resources in one go, it has no easy way to re-run the tagging since you have to use the AWS console UI, and its resource filtering capability is quite limited, making it hard to select resources with-more-than basic logic.
 
 Using Awstaga, you can easily re-run the tagging by running the CLI again. And with its support of YAML configuration, it allows you to define multiple tagsets which you can reuse and mix and match with the resources, you can construct your own mapping between the resources and the relevant tags and tagsets. You can generate your own YAML configuration using Python scripts, or any other programming language, allowing you to construct a more complex filtering logic.
 
 Installation
 ------------
```

