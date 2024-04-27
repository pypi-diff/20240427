# Comparing `tmp/ovp_docker_utils-1.0.7.tar.gz` & `tmp/ovp_docker_utils-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovp_docker_utils-1.0.7.tar", last modified: Tue Apr 23 06:23:58 2024, max compression
+gzip compressed data, was "ovp_docker_utils-1.0.8.tar", last modified: Sat Apr 27 21:07:12 2024, max compression
```

## Comparing `ovp_docker_utils-1.0.7.tar` & `ovp_docker_utils-1.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 06:23:58.501605 ovp_docker_utils-1.0.7/
--rw-rw-rw-   0        0        0    11527 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.7/LICENSE
--rw-rw-rw-   0        0        0      380 2024-04-23 06:23:58.500604 ovp_docker_utils-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1409 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 06:23:58.471052 ovp_docker_utils-1.0.7/ovp_docker_utils/
--rw-rw-rw-   0        0        0      354 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.7/ovp_docker_utils/__init__.py
--rw-rw-rw-   0        0        0       21 2024-04-23 03:55:20.000000 ovp_docker_utils-1.0.7/ovp_docker_utils/__version__.py
--rw-rw-rw-   0        0        0       27 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.7/ovp_docker_utils/defaults.py
--rw-rw-rw-   0        0        0     2441 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.7/ovp_docker_utils/docker_compose_instance.py
--rw-rw-rw-   0        0        0     5084 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.7/ovp_docker_utils/oem_logging.py
--rw-rw-rw-   0        0        0    33907 2024-04-23 05:12:46.000000 ovp_docker_utils-1.0.7/ovp_docker_utils/ovp_docker_utils.py
--rw-rw-rw-   0        0        0     6556 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.7/ovp_docker_utils/ssh_file_utils.py
--rw-rw-rw-   0        0        0     3948 2024-04-03 15:53:12.000000 ovp_docker_utils-1.0.7/ovp_docker_utils/ssh_key_gen.py
-drwxrwxrwx   0        0        0        0 2024-04-23 06:23:58.499605 ovp_docker_utils-1.0.7/ovp_docker_utils.egg-info/
--rw-rw-rw-   0        0        0      380 2024-04-23 06:23:58.000000 ovp_docker_utils-1.0.7/ovp_docker_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2024-04-23 06:23:58.000000 ovp_docker_utils-1.0.7/ovp_docker_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 06:23:58.000000 ovp_docker_utils-1.0.7/ovp_docker_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-04-23 06:23:58.000000 ovp_docker_utils-1.0.7/ovp_docker_utils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       35 2024-04-23 06:23:58.000000 ovp_docker_utils-1.0.7/ovp_docker_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-23 06:23:58.000000 ovp_docker_utils-1.0.7/ovp_docker_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-23 06:23:58.501605 ovp_docker_utils-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      878 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 21:07:12.765952 ovp_docker_utils-1.0.8/
+-rw-rw-rw-   0        0        0    11527 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0      380 2024-04-27 21:07:12.764359 ovp_docker_utils-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1409 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 21:07:12.725133 ovp_docker_utils-1.0.8/ovp_docker_utils/
+-rw-rw-rw-   0        0        0      354 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.8/ovp_docker_utils/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-04-27 21:05:02.000000 ovp_docker_utils-1.0.8/ovp_docker_utils/__version__.py
+-rw-rw-rw-   0        0        0       27 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.8/ovp_docker_utils/defaults.py
+-rw-rw-rw-   0        0        0     2427 2024-04-27 06:28:50.000000 ovp_docker_utils-1.0.8/ovp_docker_utils/docker_compose_instance.py
+-rw-rw-rw-   0        0        0     5084 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.8/ovp_docker_utils/oem_logging.py
+-rw-rw-rw-   0        0        0    33916 2024-04-27 06:44:01.000000 ovp_docker_utils-1.0.8/ovp_docker_utils/ovp_docker_utils.py
+-rw-rw-rw-   0        0        0     6556 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.8/ovp_docker_utils/ssh_file_utils.py
+-rw-rw-rw-   0        0        0     3948 2024-04-03 15:53:12.000000 ovp_docker_utils-1.0.8/ovp_docker_utils/ssh_key_gen.py
+drwxrwxrwx   0        0        0        0 2024-04-27 21:07:12.763278 ovp_docker_utils-1.0.8/ovp_docker_utils.egg-info/
+-rw-rw-rw-   0        0        0      380 2024-04-27 21:07:12.000000 ovp_docker_utils-1.0.8/ovp_docker_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2024-04-27 21:07:12.000000 ovp_docker_utils-1.0.8/ovp_docker_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 21:07:12.000000 ovp_docker_utils-1.0.8/ovp_docker_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-04-27 21:07:12.000000 ovp_docker_utils-1.0.8/ovp_docker_utils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       35 2024-04-27 21:07:12.000000 ovp_docker_utils-1.0.8/ovp_docker_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-27 21:07:12.000000 ovp_docker_utils-1.0.8/ovp_docker_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-27 21:07:12.766480 ovp_docker_utils-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      878 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.8/setup.py
```

### Comparing `ovp_docker_utils-1.0.7/LICENSE` & `ovp_docker_utils-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.7/README.md` & `ovp_docker_utils-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.7/ovp_docker_utils/docker_compose_instance.py` & `ovp_docker_utils-1.0.8/ovp_docker_utils/docker_compose_instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     @property
     def service_name(self):
         return list(self.docker_compose["services"].keys())[0]
 
     @property
     def docker_repository_name(self):
-        return self.docker_compose["services"][self.service_name]["image"].split(":")[0]
+        return self.docker_compose["services"][self.service_name]["image"]
 
     @property
     def container_name(self):
         return self.docker_compose["services"][self.service_name]["container_name"]
 
     @property
     def log_driver(self):
```

### Comparing `ovp_docker_utils-1.0.7/ovp_docker_utils/oem_logging.py` & `ovp_docker_utils-1.0.8/ovp_docker_utils/oem_logging.py`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.7/ovp_docker_utils/ovp_docker_utils.py` & `ovp_docker_utils-1.0.8/ovp_docker_utils/ovp_docker_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,17 @@
 else:
     logger = logging.getLogger("deploy")
 
 TESTED_COMPATIBLE_FIRMWARE_RANGES = [
     ["1.0.14", "1.4.30"],
 ]
 
+DEFAULT_LOG_CACHE = "~/ovp_logs"
 
-def configure_manager_logging(logger: logging.Logger, log_level: str = "", log_dir: str = "~/ovp_logs") -> str:
+def configure_manager_logging(logger: logging.Logger, log_level: str = "", log_dir: str = DEFAULT_LOG_CACHE) -> str:
     """
     Configures logging to console and file
 
     If log level is not specified, only console logging is configured and defaults to INFO level
 
     Parameters
     ----------
@@ -244,18 +245,18 @@
     return output_buffer
 
 
 class ManagerConfig(BaseModel):
     IP: str = os.environ.get("IFM3D_IP", DEFAULT_IP)
     possible_initial_ip_addresses_to_try: List[str] = []
     log_level: str = "INFO"
-    log_dir: str = "~/ovp_logs"
+    log_dir: str = DEFAULT_LOG_CACHE
     ssh_key_dir: str = "~/.ssh/"
     oem_user_password: str = "oem"
-    ssh_key_file_name: str = "id_rsa_ovp8xx"
+    ssh_key_file_name: str = "id_rsa"
 
 
 class Manager:
     def __init__(
         self,
         config: ManagerConfig = ManagerConfig(),
     ):
@@ -501,15 +502,15 @@
     def remove_registered_docker_volumes(self, registered_volumes_to_remove: list = []) -> None:
         for volume in registered_volumes_to_remove:
             cmd = f"docker volume rm {volume['VOLUME NAME']}"
             logger.info(cmd)
             _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
             logger.info(f">>>{_stdout.read().decode().strip()}")
 
-    def get_logs(self, vpu_log_dir: str = "/home/oem/share/logs", local_log_cache: str = "~/ovp_logs/From_VPUs") -> None:
+    def get_logs(self, vpu_log_dir: str = "/home/oem/share/logs", local_log_cache: str = DEFAULT_LOG_CACHE + "/From_VPUs") -> None:
         get_logs(
             vpu_log_dir=vpu_log_dir,
             local_log_cache=local_log_cache,
             vpu_sn=self.vpu_sn,
             scp=self._scp,
             ssh=self._ssh,
             vpu_name = self.vpu_name
@@ -574,25 +575,28 @@
             tag_of_loaded_image = stdout.strip().split(" ")[-1]
             cmd = f"docker tag {tag_of_loaded_image} {update_tag_on_VPU_to}"
             logger.info(cmd)
             _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
             logger.info(">>>"+_stdout.read().decode().strip() +
                         _stderr.read().decode().strip())
 
-    def pull_docker_image_from_registry(self, docker_registry_host: str, docker_registry_port: int, docker_repository_name: str, docker_image_tag: str = "latest", update_tag_on_VPU_to: str = "") -> None:
+    def pull_docker_image_from_registry(self, docker_registry_host: str, docker_registry_port: int, docker_tag: str, update_tag_on_VPU_to: str = "") -> None:
+        if ":" not in docker_tag:
+            docker_tag += ":latest"
+
         # pull image
         logger.info("pulling image from local registry (this may take a while)")
-        cmd = f"docker pull {docker_registry_host}:{docker_registry_port}/{docker_repository_name}:{docker_image_tag}"
+        cmd = f"docker pull {docker_registry_host}:{docker_registry_port}/{docker_tag}"
         logger.info(cmd)
         _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
         logger.info(">>>"+_stdout.read().decode().strip() +
                     _stderr.read().decode().strip())
 
         if update_tag_on_VPU_to:
-            cmd = f"docker tag {docker_registry_host}:{docker_registry_port}/{docker_repository_name}:{docker_image_tag} {update_tag_on_VPU_to}"
+            cmd = f"docker tag {docker_registry_host}:{docker_registry_port}/{docker_tag} {update_tag_on_VPU_to}"
             logger.info(cmd)
             _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
             logger.info(">>>"+_stdout.read().decode().strip() +
                         _stderr.read().decode().strip())
 
     def rm_item(self, item_to_rm: str) -> None:
         if SSH_path_exists(self._ssh, item_to_rm):
```

### Comparing `ovp_docker_utils-1.0.7/ovp_docker_utils/ssh_file_utils.py` & `ovp_docker_utils-1.0.8/ovp_docker_utils/ssh_file_utils.py`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.7/ovp_docker_utils/ssh_key_gen.py` & `ovp_docker_utils-1.0.8/ovp_docker_utils/ssh_key_gen.py`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.7/ovp_docker_utils.egg-info/SOURCES.txt` & `ovp_docker_utils-1.0.8/ovp_docker_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.7/setup.py` & `ovp_docker_utils-1.0.8/setup.py`

 * *Files identical despite different names*

