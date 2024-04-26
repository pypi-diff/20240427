# Comparing `tmp/google-cloud-jupyter-config-0.0.5.tar.gz` & `tmp/google_cloud_jupyter_config-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-jupyter-config-0.0.5.tar", last modified: Wed Aug 16 23:17:16 2023, max compression
+gzip compressed data, was "google_cloud_jupyter_config-0.0.7.tar", last modified: Fri Apr 26 22:31:49 2024, max compression
```

## Comparing `google-cloud-jupyter-config-0.0.5.tar` & `google_cloud_jupyter_config-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2023-08-16 23:17:16.925120 google-cloud-jupyter-config-0.0.5/
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)    11358 2023-08-11 16:50:41.000000 google-cloud-jupyter-config-0.0.5/LICENSE
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       15 2023-08-11 16:50:41.000000 google-cloud-jupyter-config-0.0.5/MANIFEST.in
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2532 2023-08-16 23:17:16.925120 google-cloud-jupyter-config-0.0.5/PKG-INFO
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     1682 2023-08-11 16:50:41.000000 google-cloud-jupyter-config-0.0.5/README.md
-drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2023-08-16 23:17:16.924120 google-cloud-jupyter-config-0.0.5/google/
-drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2023-08-16 23:17:16.924120 google-cloud-jupyter-config-0.0.5/google/cloud/
-drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2023-08-16 23:17:16.925120 google-cloud-jupyter-config-0.0.5/google/cloud/jupyter_config/
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)      831 2023-08-11 16:50:41.000000 google-cloud-jupyter-config-0.0.5/google/cloud/jupyter_config/__init__.py
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2932 2023-08-16 23:16:35.000000 google-cloud-jupyter-config-0.0.5/google/cloud/jupyter_config/config.py
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     1822 2023-08-11 16:50:41.000000 google-cloud-jupyter-config-0.0.5/google/cloud/jupyter_config/config_test.py
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2691 2023-08-16 23:16:35.000000 google-cloud-jupyter-config-0.0.5/google/cloud/jupyter_config/tokenrenewer.py
-drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2023-08-16 23:17:16.925120 google-cloud-jupyter-config-0.0.5/google_cloud_jupyter_config.egg-info/
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2532 2023-08-16 23:17:16.000000 google-cloud-jupyter-config-0.0.5/google_cloud_jupyter_config.egg-info/PKG-INFO
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)      467 2023-08-16 23:17:16.000000 google-cloud-jupyter-config-0.0.5/google_cloud_jupyter_config.egg-info/SOURCES.txt
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)        1 2023-08-16 23:17:16.000000 google-cloud-jupyter-config-0.0.5/google_cloud_jupyter_config.egg-info/dependency_links.txt
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       32 2023-08-16 23:17:16.000000 google-cloud-jupyter-config-0.0.5/google_cloud_jupyter_config.egg-info/requires.txt
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)        7 2023-08-16 23:17:16.000000 google-cloud-jupyter-config-0.0.5/google_cloud_jupyter_config.egg-info/top_level.txt
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       67 2023-08-16 23:17:16.925120 google-cloud-jupyter-config-0.0.5/setup.cfg
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     1198 2023-08-16 23:16:35.000000 google-cloud-jupyter-config-0.0.5/setup.py
+drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-04-26 22:31:49.429093 google_cloud_jupyter_config-0.0.7/
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)    11358 2024-04-26 22:29:06.000000 google_cloud_jupyter_config-0.0.7/LICENSE
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       15 2024-04-26 22:29:06.000000 google_cloud_jupyter_config-0.0.7/MANIFEST.in
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2139 2024-04-26 22:31:49.429093 google_cloud_jupyter_config-0.0.7/PKG-INFO
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     1682 2024-04-26 22:29:06.000000 google_cloud_jupyter_config-0.0.7/README.md
+drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-04-26 22:31:49.428094 google_cloud_jupyter_config-0.0.7/google/
+drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-04-26 22:31:49.428094 google_cloud_jupyter_config-0.0.7/google/cloud/
+drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-04-26 22:31:49.429093 google_cloud_jupyter_config-0.0.7/google/cloud/jupyter_config/
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)      830 2024-04-26 22:29:06.000000 google_cloud_jupyter_config-0.0.7/google/cloud/jupyter_config/__init__.py
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     6495 2024-04-26 22:29:06.000000 google_cloud_jupyter_config-0.0.7/google/cloud/jupyter_config/config.py
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2588 2024-04-26 22:29:06.000000 google_cloud_jupyter_config-0.0.7/google/cloud/jupyter_config/config_test.py
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2909 2024-04-26 22:29:06.000000 google_cloud_jupyter_config-0.0.7/google/cloud/jupyter_config/tokenrenewer.py
+drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-04-26 22:31:49.429093 google_cloud_jupyter_config-0.0.7/google_cloud_jupyter_config.egg-info/
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2139 2024-04-26 22:31:49.000000 google_cloud_jupyter_config-0.0.7/google_cloud_jupyter_config.egg-info/PKG-INFO
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)      467 2024-04-26 22:31:49.000000 google_cloud_jupyter_config-0.0.7/google_cloud_jupyter_config.egg-info/SOURCES.txt
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)        1 2024-04-26 22:31:49.000000 google_cloud_jupyter_config-0.0.7/google_cloud_jupyter_config.egg-info/dependency_links.txt
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       43 2024-04-26 22:31:49.000000 google_cloud_jupyter_config-0.0.7/google_cloud_jupyter_config.egg-info/requires.txt
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       12 2024-04-26 22:31:49.000000 google_cloud_jupyter_config-0.0.7/google_cloud_jupyter_config.egg-info/top_level.txt
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       67 2024-04-26 22:31:49.429093 google_cloud_jupyter_config-0.0.7/setup.cfg
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     1216 2024-04-26 22:29:06.000000 google_cloud_jupyter_config-0.0.7/setup.py
```

### Comparing `google-cloud-jupyter-config-0.0.5/LICENSE` & `google_cloud_jupyter_config-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-jupyter-config-0.0.5/PKG-INFO` & `google_cloud_jupyter_config-0.0.7/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,59 @@
-Metadata-Version: 2.1
-Name: google-cloud-jupyter-config
-Version: 0.0.5
-Summary: Jupyter configuration utilities using gcloud
-Home-page: https://github.com/GoogleCloudPlatform/jupyter-extensions/tree/master/google-cloud-jupyter-config
-Author: Google, Inc.
-License: Apache License 2.0
-Description: # Notebook server configuration using the Google Cloud SDK
-        
-        This package provides Python classes that can be used in the Jupyter config file
-        (e.g. `~/.jupyter/jupyter_lab_config.py`) in order to fill in some configuration
-        using the Google Cloud SDK's [`gcloud` tool](https://cloud.google.com/sdk/gcloud).
-        
-        ## Included features
-        
-        This package provides utility methods to look up any configuration options stored
-        in the active gcloud config, in particular the project and region.
-        
-        Additionally, this provides a utility method to update a given
-        [`Config`](https://traitlets.readthedocs.io/en/latest/config-api.html#traitlets.config.Config)
-        object to connect to a kernel gateway URL managed by Google.
-        
-        ## Prerequisites
-        
-        Install both Jupyter and [gcloud](https://cloud.google.com/sdk/docs/install).
-        
-        For the kernel gateway feature, you will need an installation of Jupyter that uses the
-        `jupyter_server` project and the version of `jupyter_server` you have installed needs to be
-        at least version `2.4.0`.
-        
-        You will also need to log in to gcloud:
-        
-        ```sh
-        gcloud auth login
-        ```
-        
-        ... and configure your project and region:
-        
-        ```sh
-        gcloud config set core/project ${PROJECT}
-        gcloud config set compute/region ${REGION}
-        ```
-        
-        ## Install
-        
-        Clone this repository, and from this directory run the following:
-        
-        ```sh
-        pip install .
-        ```
-        
-        ## Setup
-        
-        If you do not already have a Jupyter config file (e.g. `~/.jupyter/jupyter_lab_config.py`),
-        the first generate one with the following command:
-        
-        ```sh
-        jupyter lab --generate-config
-        ```
-        
-        The open your config file and add the following two lines to the end:
-        
-        ```py
-        import google.cloud.jupyter_config
-        google.cloud.jupyter_config.configure_gateway_client(c)
-        ```
-        
-Platform: UNKNOWN
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+# Notebook server configuration using the Google Cloud SDK
+
+This package provides Python classes that can be used in the Jupyter config file
+(e.g. `~/.jupyter/jupyter_lab_config.py`) in order to fill in some configuration
+using the Google Cloud SDK's [`gcloud` tool](https://cloud.google.com/sdk/gcloud).
+
+## Included features
+
+This package provides utility methods to look up any configuration options stored
+in the active gcloud config, in particular the project and region.
+
+Additionally, this provides a utility method to update a given
+[`Config`](https://traitlets.readthedocs.io/en/latest/config-api.html#traitlets.config.Config)
+object to connect to a kernel gateway URL managed by Google.
+
+## Prerequisites
+
+Install both Jupyter and [gcloud](https://cloud.google.com/sdk/docs/install).
+
+For the kernel gateway feature, you will need an installation of Jupyter that uses the
+`jupyter_server` project and the version of `jupyter_server` you have installed needs to be
+at least version `2.4.0`.
+
+You will also need to log in to gcloud:
+
+```sh
+gcloud auth login
+```
+
+... and configure your project and region:
+
+```sh
+gcloud config set core/project ${PROJECT}
+gcloud config set compute/region ${REGION}
+```
+
+## Install
+
+Clone this repository, and from this directory run the following:
+
+```sh
+pip install .
+```
+
+## Setup
+
+If you do not already have a Jupyter config file (e.g. `~/.jupyter/jupyter_lab_config.py`),
+the first generate one with the following command:
+
+```sh
+jupyter lab --generate-config
+```
+
+The open your config file and add the following two lines to the end:
+
+```py
+import google.cloud.jupyter_config
+google.cloud.jupyter_config.configure_gateway_client(c)
+```
```

### Comparing `google-cloud-jupyter-config-0.0.5/google/cloud/jupyter_config/__init__.py` & `google_cloud_jupyter_config-0.0.7/google/cloud/jupyter_config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from google.cloud.jupyter_config.config import get_gcloud_config
 from google.cloud.jupyter_config.config import gcp_project
 from google.cloud.jupyter_config.config import gcp_region
-from google.cloud.jupyter_config.config import configure_gateway_client 
+from google.cloud.jupyter_config.config import configure_gateway_client
```

### Comparing `google-cloud-jupyter-config-0.0.5/google/cloud/jupyter_config/tokenrenewer.py` & `google_cloud_jupyter_config-0.0.7/google/cloud/jupyter_config/tokenrenewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,73 +21,74 @@
 
 from abc import abstractmethod
 from traitlets import Int, Unicode
 from jupyter_server.gateway.gateway_client import GatewayTokenRenewerBase
 
 
 class CachedTokenRenewerBase(GatewayTokenRenewerBase):
-  """Token renewer base class that only renews the token after a specified timeout."""
+    """Token renewer base class that only renews the token after a specified timeout."""
 
-  token_lifetime_seconds = Int(
-    default_value=300,
-    config=True,
-    help="""Time (in seconds) to wait between successive token renewals.""",
-  )
-
-  @abstractmethod
-  def force_new_token(
-      self,
-      auth_header_key: str,
-      auth_scheme: typing.Union[str, None],
-      **kwargs: typing.Any,
-  ):
-    pass
-
-  _created = datetime.datetime.min
-
-  def get_token(
-      self,
-      auth_header_key: str,
-      auth_scheme: typing.Union[str, None],
-      auth_token: str,
-      **kwargs: typing.Any,
-  ):
-    current_time = datetime.datetime.now()
-    duration = (current_time - self._created).total_seconds()
-    if (not auth_token) or (duration > self.token_lifetime_seconds):
-      auth_token = self.force_new_token(auth_header_key, auth_scheme, **kwargs)
-      self._created = datetime.datetime.now()
+    token_lifetime_seconds = Int(
+        default_value=300,
+        config=True,
+        help="""Time (in seconds) to wait between successive token renewals.""",
+    )
+
+    @abstractmethod
+    def force_new_token(
+        self,
+        auth_header_key: str,
+        auth_scheme: typing.Union[str, None],
+        **kwargs: typing.Any,
+    ):
+        pass
+
+    _created = datetime.datetime.min
+
+    def get_token(
+        self,
+        auth_header_key: str,
+        auth_scheme: typing.Union[str, None],
+        auth_token: str,
+        **kwargs: typing.Any,
+    ):
+        current_time = datetime.datetime.now()
+        duration = (current_time - self._created).total_seconds()
+        if (not auth_token) or (duration > self.token_lifetime_seconds):
+            auth_token = self.force_new_token(auth_header_key, auth_scheme, **kwargs)
+            self._created = datetime.datetime.now()
 
-    return auth_token
+        return auth_token
 
 
 class CommandTokenRenewer(CachedTokenRenewerBase):
-  """Token renewer that invokes an external command to generate the token."""
+    """Token renewer that invokes an external command to generate the token."""
 
-  token_command = Unicode(
-    default_value="",
-    config=True,
-    help="""External command run to generate auth tokens.""",
-  )
-
-  def force_new_token(
-      self,
-      auth_header_key: str,
-      auth_scheme: typing.Union[str, None],
-      **kwargs: typing.Any,
-  ):
-    """Run the specified command to generate a new token, which is taken from its output.
-
-    We reuse the system stderr for the command so that any prompts from it
-    will be displayed to the user.
-    """
-    with tempfile.TemporaryFile() as t:
-      p = subprocess.run(
-        self.token_command,
-        stdin=subprocess.DEVNULL,
-        stderr=sys.stderr,
-        stdout=t,
-        check=True,
-        shell=True,
-        encoding='UTF-8')
-      t.seek(0)
-      return t.read().decode('UTF-8').strip()
+    token_command = Unicode(
+        default_value="",
+        config=True,
+        help="""External command run to generate auth tokens.""",
+    )
+
+    def force_new_token(
+        self,
+        auth_header_key: str,
+        auth_scheme: typing.Union[str, None],
+        **kwargs: typing.Any,
+    ):
+        """Run the specified command to generate a new token, which is taken from its output.
+
+        We reuse the system stderr for the command so that any prompts from it
+        will be displayed to the user.
+        """
+        with tempfile.TemporaryFile() as t:
+            p = subprocess.run(
+                self.token_command,
+                stdin=subprocess.DEVNULL,
+                stderr=sys.stderr,
+                stdout=t,
+                check=True,
+                shell=True,
+                encoding="UTF-8",
+            )
+            t.seek(0)
+            return t.read().decode("UTF-8").strip()
```

### Comparing `google-cloud-jupyter-config-0.0.5/setup.py` & `google_cloud_jupyter_config-0.0.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,20 +15,21 @@
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="google-cloud-jupyter-config",
   author="Google, Inc.",
-  version="0.0.5",
+  version="0.0.7",
   description="Jupyter configuration utilities using gcloud",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/GoogleCloudPlatform/jupyter-extensions/tree/master/google-cloud-jupyter-config",
   license="Apache License 2.0",
   packages=setuptools.find_namespace_packages(),
   python_requires=">=3.8",
   install_requires=[
+    "cachetools",
     "jupyter_server>=2.4.0",
     "traitlets",
   ],
 )
```

