# Comparing `tmp/compose_viz-0.3.1.tar.gz` & `tmp/compose_viz-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compose_viz-0.3.1.tar", max compression
+gzip compressed data, was "compose_viz-0.3.2.tar", max compression
```

## Comparing `compose_viz-0.3.1.tar` & `compose_viz-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     1067 2023-05-06 14:48:50.439527 compose_viz-0.3.1/LICENSE
--rw-r--r--   0        0        0     7706 2023-05-06 14:48:50.439527 compose_viz-0.3.1/README.md
--rw-r--r--   0        0        0       51 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/__init__.py
--rw-r--r--   0        0        0       82 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/__main__.py
--rw-r--r--   0        0        0     1576 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/cli.py
--rw-r--r--   0        0        0     4943 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/graph.py
--rw-r--r--   0        0        0        0 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/models/__init__.py
--rw-r--r--   0        0        0      249 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/models/compose.py
--rw-r--r--   0        0        0      524 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/models/device.py
--rw-r--r--   0        0        0      347 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/models/extends.py
--rw-r--r--   0        0        0      546 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/models/port.py
--rw-r--r--   0        0        0     2194 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/models/service.py
--rw-r--r--   0        0        0      804 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/models/viz_formats.py
--rw-r--r--   0        0        0      654 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/models/volume.py
--rw-r--r--   0        0        0    12260 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/parser.py
--rw-r--r--   0        0        0        0 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/spec/__init__.py
--rw-r--r--   0        0        0    26517 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/spec/compose-spec.json
--rw-r--r--   0        0        0    16662 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/spec/compose_spec.py
--rw-r--r--   0        0        0      897 2023-05-06 14:48:50.443527 compose_viz-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     8597 1970-01-01 00:00:00.000000 compose_viz-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-27 19:53:32.131202 compose_viz-0.3.2/LICENSE
+-rw-r--r--   0        0        0     7926 2024-04-27 19:53:32.131202 compose_viz-0.3.2/README.md
+-rw-r--r--   0        0        0       53 2024-04-27 19:53:32.131202 compose_viz-0.3.2/compose_viz/__init__.py
+-rw-r--r--   0        0        0       82 2024-04-27 19:53:32.131202 compose_viz-0.3.2/compose_viz/__main__.py
+-rw-r--r--   0        0        0     1744 2024-04-27 19:53:32.131202 compose_viz-0.3.2/compose_viz/cli.py
+-rw-r--r--   0        0        0     7671 2024-04-27 19:53:32.131202 compose_viz-0.3.2/compose_viz/graph.py
+-rw-r--r--   0        0        0        0 2024-04-27 19:53:32.131202 compose_viz-0.3.2/compose_viz/models/__init__.py
+-rw-r--r--   0        0        0      249 2024-04-27 19:53:32.131202 compose_viz-0.3.2/compose_viz/models/compose.py
+-rw-r--r--   0        0        0      524 2024-04-27 19:53:32.131202 compose_viz-0.3.2/compose_viz/models/device.py
+-rw-r--r--   0        0        0      347 2024-04-27 19:53:32.131202 compose_viz-0.3.2/compose_viz/models/extends.py
+-rw-r--r--   0        0        0      901 2024-04-27 19:53:32.131202 compose_viz-0.3.2/compose_viz/models/port.py
+-rw-r--r--   0        0        0     2194 2024-04-27 19:53:32.131202 compose_viz-0.3.2/compose_viz/models/service.py
+-rw-r--r--   0        0        0      804 2024-04-27 19:53:32.131202 compose_viz-0.3.2/compose_viz/models/viz_formats.py
+-rw-r--r--   0        0        0      654 2024-04-27 19:53:32.131202 compose_viz-0.3.2/compose_viz/models/volume.py
+-rw-r--r--   0        0        0    12790 2024-04-27 19:53:32.131202 compose_viz-0.3.2/compose_viz/parser.py
+-rw-r--r--   0        0        0        0 2024-04-27 19:53:32.131202 compose_viz-0.3.2/compose_viz/spec/__init__.py
+-rw-r--r--   0        0        0    17727 2024-04-27 19:53:32.131202 compose_viz-0.3.2/compose_viz/spec/compose_spec.py
+-rw-r--r--   0        0        0      932 2024-04-27 19:53:32.135202 compose_viz-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     8786 1970-01-01 00:00:00.000000 compose_viz-0.3.2/PKG-INFO
```

### Comparing `compose_viz-0.3.1/LICENSE` & `compose_viz-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `compose_viz-0.3.1/README.md` & `compose_viz-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,15 @@
 ### Options
 
 | Option                            | Description                                                                                                                                                                         |
 | --------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `-o, --output-filename FILENAME`  | Output filename for the generated visualization file. [default: compose-viz]                                                                                                        |
 | `-m, --format FORMAT`             | Output format for the generated visualization file. See [supported formats](https://github.com/compose-viz/compose-viz/blob/main/compose_viz/models/viz_formats.py). [default: png] |
 | `-r, --root-service SERVICE_NAME` | Root of the service tree (convenient for large compose yamls)                                                                                                                       |
+| `-l, --legend`                    | Include a legend in the visualization.                                                                                                                                              |
 | `-v, --version`                   | Show the version of compose-viz.                                                                                                                                                    |
 | `--help`                          | Show help and exit.                                                                                                                                                                 |
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- ROADMAP -->
```

#### html2text {}

```diff
@@ -50,16 +50,16 @@
 -------------------------------------------------------------------------------
 ----------------------------- | | `-o, --output-filename FILENAME` | Output
 filename for the generated visualization file. [default: compose-viz] | | `-m,
 --format FORMAT` | Output format for the generated visualization file. See
 [supported formats](https://github.com/compose-viz/compose-viz/blob/main/
 compose_viz/models/viz_formats.py). [default: png] | | `-r, --root-service
 SERVICE_NAME` | Root of the service tree (convenient for large compose yamls) |
-| `-v, --version` | Show the version of compose-viz. | | `--help` | Show help
-and exit. |
+| `-l, --legend` | Include a legend in the visualization. | | `-v, --version` |
+Show the version of compose-viz. | | `--help` | Show help and exit. |
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Roadmap - [ ] Support more vizualization components. See the [open issues]
 (https://github.com/compose-viz/compose-viz/issues) for a full list of proposed
 features (and known issues).
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
```

### Comparing `compose_viz-0.3.1/compose_viz/cli.py` & `compose_viz-0.3.2/compose_viz/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,14 +38,20 @@
     ),
     root_service: str = typer.Option(
         None,
         "--root-service",
         "-r",
         help="Root of the service tree (convenient for large compose yamls)",
     ),
+    include_legend: bool = typer.Option(
+        False,
+        "--legend",
+        "-l",
+        help="Include a legend in the visualization.",
+    ),
     _: Optional[bool] = typer.Option(
         None,
         "--version",
         "-v",
         help="Show the version of compose-viz.",
         callback=_version_callback,
         is_eager=True,
@@ -53,14 +59,14 @@
 ) -> None:
     parser = Parser()
     compose = parser.parse(input_path, root_service=root_service)
 
     if compose:
         typer.echo(f"Successfully parsed {input_path}")
 
-    Graph(compose, output_filename).render(format)
+    Graph(compose, output_filename, include_legend).render(format)
 
     raise typer.Exit()
 
 
 def start_cli() -> None:
     app(prog_name="cpv")
```

### Comparing `compose_viz-0.3.1/compose_viz/models/device.py` & `compose_viz-0.3.2/compose_viz/models/device.py`

 * *Files identical despite different names*

### Comparing `compose_viz-0.3.1/compose_viz/models/service.py` & `compose_viz-0.3.2/compose_viz/models/service.py`

 * *Files identical despite different names*

### Comparing `compose_viz-0.3.1/compose_viz/models/viz_formats.py` & `compose_viz-0.3.2/compose_viz/models/viz_formats.py`

 * *Files identical despite different names*

### Comparing `compose_viz-0.3.1/compose_viz/models/volume.py` & `compose_viz-0.3.2/compose_viz/models/volume.py`

 * *Files identical despite different names*

### Comparing `compose_viz-0.3.1/compose_viz/parser.py` & `compose_viz-0.3.2/compose_viz/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import re
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import ValidationError
+from pydantic_yaml import parse_yaml_raw_as
 
 import compose_viz.spec.compose_spec as spec
 from compose_viz.models.compose import Compose, Service
 from compose_viz.models.device import Device
 from compose_viz.models.extends import Extends
-from compose_viz.models.port import Port, Protocol
+from compose_viz.models.port import AppProtocol, Port, Protocol
 from compose_viz.models.volume import Volume, VolumeType
 
 
 class Parser:
     def __init__(self):
         pass
 
     @staticmethod
     def _unwrap_depends_on(data_depends_on: Union[spec.ListOfStrings, Dict[Any, spec.DependsOn], None]) -> List[str]:
         service_depends_on = []
         if type(data_depends_on) is spec.ListOfStrings:
-            service_depends_on = data_depends_on.__root__
+            service_depends_on = data_depends_on.root
         elif type(data_depends_on) is dict:
             for depends_on in data_depends_on.keys():
                 service_depends_on.append(str(depends_on))
         return service_depends_on
 
     @staticmethod
     def compile_dependencies(service_name: str, services: Dict[Any, spec.Service], file_path: str) -> List[str]:
@@ -36,16 +36,18 @@
                 dependencies.extend(Parser.compile_dependencies(dependency, services, file_path))
         return dependencies
 
     def parse(self, file_path: str, root_service: Optional[str] = None) -> Compose:
         compose_data: spec.ComposeSpecification
 
         try:
-            compose_data = spec.ComposeSpecification.parse_file(file_path)
-        except ValidationError as e:
+            with open(file_path, "r") as file:
+                file_content = file.read()
+            compose_data = parse_yaml_raw_as(spec.ComposeSpecification, file_content)
+        except Exception as e:
             raise RuntimeError(f"Error parsing file '{file_path}': {e}")
 
         services: List[Service] = []
 
         assert compose_data.services is not None, "No services found, aborting."
 
         root_dependencies: List[str] = []
@@ -59,15 +61,15 @@
             if root_service and service_name not in root_dependencies:
                 continue
 
             service_image: Optional[str] = None
             if service_data.build is not None:
                 if type(service_data.build) is str:
                     service_image = f"build from '{service_data.build}'"
-                elif type(service_data.build) is spec.BuildItem:
+                elif type(service_data.build) is spec.Build:
                     if service_data.build.context is not None and service_data.build.dockerfile is not None:
                         service_image = (
                             f"build from '{service_data.build.context}' using '{service_data.build.dockerfile}'"
                         )
                     elif service_data.build.context is not None:
                         service_image = f"build from '{service_data.build.context}'"
             if service_data.image is not None:
@@ -75,40 +77,41 @@
                     service_image += ", image: " + service_data.image
                 else:
                     service_image = service_data.image
 
             service_networks: List[str] = []
             if service_data.networks is not None:
                 if type(service_data.networks) is spec.ListOfStrings:
-                    service_networks = service_data.networks.__root__
+                    service_networks = service_data.networks.root
                 elif type(service_data.networks) is dict:
                     service_networks = list(service_data.networks.keys())
 
             service_extends: Optional[Extends] = None
             if service_data.extends is not None:
                 # https://github.com/compose-spec/compose-spec/blob/master/spec.md#extends
                 # The value of the extends key MUST be a dictionary.
-                assert type(service_data.extends) is spec.Extend
+                assert type(service_data.extends) is spec.Extends
                 service_extends = Extends(
                     service_name=service_data.extends.service, from_file=service_data.extends.file
                 )
 
             service_ports: List[Port] = []
             if service_data.ports is not None:
                 for port_data in service_data.ports:
                     host_ip: Optional[str] = None
                     host_port: Optional[str] = None
                     container_port: Optional[str] = None
                     protocol: Optional[str] = None
+                    app_protocol: Optional[str] = None
 
                     if type(port_data) is float:
                         container_port = str(int(port_data))
                         host_port = f"0.0.0.0:{container_port}"
                     elif type(port_data) is str:
-                        regex = r"((?P<host_ip>\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}:)|:)?((?P<host_port>\d+(\-\d+)?):)?((?P<container_port>\d+(\-\d+)?))?(/(?P<protocol>\w+))?"  # noqa: E501
+                        regex = r"((?P<host_ip>\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}:|(\$\{([^}]+)\}):)|:|)?((?P<host_port>\d+(\-\d+)?):)?((?P<container_port>\d+(\-\d+)?))?(/(?P<protocol>\w+))?"  # noqa: E501
                         match = re.match(regex, port_data)
 
                         if match:
                             host_ip = match.group("host_ip")
                             host_port = match.group("host_port")
                             container_port = match.group("container_port")
                             protocol = match.group("protocol")
@@ -118,28 +121,26 @@
                             if container_port is not None and host_port is None:
                                 host_port = container_port
 
                             if host_ip is not None:
                                 host_port = f"{host_ip}{host_port}"
                             else:
                                 host_port = f"0.0.0.0:{host_port}"
-                    elif type(port_data) is spec.Port:
+                    elif type(port_data) is spec.Ports:
                         assert port_data.target is not None, "Invalid port format, aborting."
 
-                        # ruamel.yaml does not parse port as int
-                        assert type(port_data.published) is not int
-
-                        if type(port_data.published) is str:
-                            host_port = port_data.published
+                        if type(port_data.published) is str or type(port_data.published) is int:
+                            host_port = str(port_data.published)
 
                         if type(port_data.target) is int:
                             container_port = str(port_data.target)
 
                         host_ip = port_data.host_ip
                         protocol = port_data.protocol
+                        app_protocol = port_data.app_protocol
 
                         if container_port is not None and host_port is None:
                             host_port = container_port
 
                         if host_ip is not None:
                             host_port = f"{host_ip}:{host_port}"
                         else:
@@ -147,19 +148,23 @@
 
                     assert host_port is not None, "Error while parsing port, aborting."
                     assert container_port is not None, "Error while parsing port, aborting."
 
                     if protocol is None:
                         protocol = "any"
 
+                    if app_protocol is None:
+                        app_protocol = "na"
+
                     service_ports.append(
                         Port(
                             host_port=host_port,
                             container_port=container_port,
                             protocol=Protocol[protocol],
+                            app_protocol=AppProtocol[app_protocol],
                         )
                     )
 
             service_depends_on: List[str] = []
             if service_data.depends_on is not None:
                 service_depends_on = Parser._unwrap_depends_on(service_data.depends_on)
 
@@ -176,15 +181,15 @@
                             service_volumes.append(
                                 Volume(
                                     source=spilt_data[0],
                                     target=spilt_data[1],
                                     access_mode=spilt_data[2],
                                 )
                             )
-                    elif type(volume_data) is spec.ServiceVolume:
+                    elif type(volume_data) is spec.Volumes:
                         assert volume_data.target is not None, "Invalid volume input, aborting."
 
                         # https://github.com/compose-spec/compose-spec/blob/master/spec.md#long-syntax-4
                         # `volume_data.source` is not applicable for a tmpfs mount.
                         if volume_data.source is None:
                             volume_data.source = volume_data.target
 
@@ -208,29 +213,34 @@
 
             container_name: Optional[str] = None
             if service_data.container_name is not None:
                 container_name = service_data.container_name
 
             env_file: List[str] = []
             if service_data.env_file is not None:
-                if type(service_data.env_file) is spec.StringOrList:
-                    if type(service_data.env_file.__root__) is spec.ListOfStrings:
-                        env_file = service_data.env_file.__root__.__root__
-                    elif type(service_data.env_file.__root__) is str:
-                        env_file.append(service_data.env_file.__root__)
+                if type(service_data.env_file.root) is str:
+                    env_file = [service_data.env_file.root]
+                elif type(service_data.env_file.root) is list:
+                    for env_file_data in service_data.env_file.root:
+                        if type(env_file_data) is str:
+                            env_file.append(env_file_data)
+                        elif type(env_file_data) is spec.EnvFilePath:
+                            env_file.append(env_file_data.path)
+                else:
+                    print(f"Invalid env_file data: {service_data.env_file.root}")
 
             expose: List[str] = []
             if service_data.expose is not None:
                 for port in service_data.expose:
                     expose.append(str(port))
 
             profiles: List[str] = []
             if service_data.profiles is not None:
                 if type(service_data.profiles) is spec.ListOfStrings:
-                    profiles = service_data.profiles.__root__
+                    profiles = service_data.profiles.root
 
             devices: List[Device] = []
             if service_data.devices is not None:
                 for device_data in service_data.devices:
                     if type(device_data) is str:
                         assert ":" in device_data, "Invalid volume input, aborting."
```

### Comparing `compose_viz-0.3.1/compose_viz/spec/compose_spec.py` & `compose_viz-0.3.2/compose_viz/spec/compose_spec.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,592 +1,620 @@
-# generated by datamodel-codegen:
-#   filename:  compose-spec.json
-#   timestamp: 2023-05-03T07:42:00+00:00
-
-from __future__ import annotations
-
-from typing import Any, Dict, List, Optional, Union
-
-from pydantic import Extra, Field, conint, constr
-from pydantic_yaml import YamlModel, YamlStrEnum
-
-
-class Cgroup(YamlStrEnum):
-    host = "host"
-    private = "private"
-
-
-class CredentialSpec(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    config: Optional[str] = None
-    file: Optional[str] = None
-    registry: Optional[str] = None
-
-
-class Condition(YamlStrEnum):
-    service_started = "service_started"
-    service_healthy = "service_healthy"
-    service_completed_successfully = "service_completed_successfully"
-
-
-class DependsOn(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    restart: Optional[bool] = None
-    condition: Condition
-
-
-class Extend(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    service: str
-    file: Optional[str] = None
-
-
-class Logging(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    driver: Optional[str] = None
-    options: Optional[Dict[constr(regex=r"^.+$"), Optional[Union[str, float]]]] = None  # type: ignore  # noqa: F722
-
-
-class Port(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    mode: Optional[str] = None
-    host_ip: Optional[str] = None
-    target: Optional[int] = None
-    published: Optional[Union[str, int]] = None
-    protocol: Optional[str] = None
-
-
-class PullPolicy(YamlStrEnum):
-    always = "always"
-    never = "never"
-    if_not_present = "if_not_present"
-    build = "build"
-    missing = "missing"
-
-
-class Ulimit(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    hard: int
-    soft: int
-
-
-class Selinux(YamlStrEnum):
-    z = "z"
-    Z = "Z"
-
-
-class Bind(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    propagation: Optional[str] = None
-    create_host_path: Optional[bool] = None
-    selinux: Optional[Selinux] = None
-
-
-class AdditionalVolumeOption(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    nocopy: Optional[bool] = None
-
-
-class Tmpfs(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    size: Optional[Union[conint(ge=0), str]] = None  # type: ignore
-    mode: Optional[float] = None
-
-
-class ServiceVolume(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    type: str
-    source: Optional[str] = None
-    target: Optional[str] = None
-    read_only: Optional[bool] = None
-    consistency: Optional[str] = None
-    bind: Optional[Bind] = None
-    volume: Optional[AdditionalVolumeOption] = None
-    tmpfs: Optional[Tmpfs] = None
-
-
-class Healthcheck(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    disable: Optional[bool] = None
-    interval: Optional[str] = None
-    retries: Optional[float] = None
-    test: Optional[Union[str, List[str]]] = None
-    timeout: Optional[str] = None
-    start_period: Optional[str] = None
-
-
-class Order(YamlStrEnum):
-    start_first = "start-first"
-    stop_first = "stop-first"
-
-
-class RollbackConfig(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    parallelism: Optional[int] = None
-    delay: Optional[str] = None
-    failure_action: Optional[str] = None
-    monitor: Optional[str] = None
-    max_failure_ratio: Optional[float] = None
-    order: Optional[Order] = None
-
-
-class ConfigOrder(YamlStrEnum):
-    start_first = "start-first"
-    stop_first = "stop-first"
-
-
-class UpdateConfig(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    parallelism: Optional[int] = None
-    delay: Optional[str] = None
-    failure_action: Optional[str] = None
-    monitor: Optional[str] = None
-    max_failure_ratio: Optional[float] = None
-    order: Optional[ConfigOrder] = None
-
-
-class Limits(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    cpus: Optional[Union[float, str]] = None
-    memory: Optional[str] = None
-    pids: Optional[int] = None
-
-
-class RestartPolicy(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    condition: Optional[str] = None
-    delay: Optional[str] = None
-    max_attempts: Optional[int] = None
-    window: Optional[str] = None
-
-
-class Preference(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    spread: Optional[str] = None
-
-
-class Placement(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    constraints: Optional[List[str]] = None
-    preferences: Optional[List[Preference]] = None
-    max_replicas_per_node: Optional[int] = None
-
-
-class DiscreteResourceSpec(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    kind: Optional[str] = None
-    value: Optional[float] = None
-
-
-class GenericResource(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    discrete_resource_spec: Optional[DiscreteResourceSpec] = None
-
-
-class GenericResources(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    __root__: List[GenericResource]
-
-
-class ConfigItem(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    subnet: Optional[str] = None
-    ip_range: Optional[str] = None
-    gateway: Optional[str] = None
-    aux_addresses: Optional[Dict[constr(regex=r"^.+$"), str]] = None  # type: ignore  # noqa: F722
-
-
-class Ipam(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    driver: Optional[str] = None
-    config: Optional[List[ConfigItem]] = None
-    options: Optional[Dict[constr(regex=r"^.+$"), str]] = None  # type: ignore  # noqa: F722
-
-
-class ExternalNetwork(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    name: Optional[str] = None
-
-
-class ExternalVolume(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    name: Optional[str] = None
-
-
-class ExternalSecret(YamlModel):
-    name: Optional[str] = None
-
-
-class ExternalConfig(YamlModel):
-    name: Optional[str] = None
-
-
-class ListOfStrings(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    __root__: List[str] = Field(..., unique_items=True)
-
-
-class ListOrDict(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    __root__: Union[
-        Dict[constr(regex=r".+"), Optional[Union[str, float, bool]]], List[str]  # type: ignore  # noqa: F722
-    ]
-
-
-class BlkioLimit(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    path: Optional[str] = None
-    rate: Optional[Union[int, str]] = None
-
-
-class BlkioWeight(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    path: Optional[str] = None
-    weight: Optional[int] = None
-
-
-class ServiceConfigOrSecretItem(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    source: Optional[str] = None
-    target: Optional[str] = None
-    uid: Optional[str] = None
-    gid: Optional[str] = None
-    mode: Optional[float] = None
-
-
-class ServiceConfigOrSecret(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    __root__: List[Union[str, ServiceConfigOrSecretItem]]
-
-
-class Constraints(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    __root__: Any
-
-
-class BuildItem(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    context: Optional[str] = None
-    dockerfile: Optional[str] = None
-    dockerfile_inline: Optional[str] = None
-    args: Optional[ListOrDict] = None
-    ssh: Optional[ListOrDict] = None
-    labels: Optional[ListOrDict] = None
-    cache_from: Optional[List[str]] = None
-    cache_to: Optional[List[str]] = None
-    no_cache: Optional[bool] = None
-    additional_contexts: Optional[ListOrDict] = None
-    network: Optional[str] = None
-    pull: Optional[bool] = None
-    target: Optional[str] = None
-    shm_size: Optional[Union[int, str]] = None
-    extra_hosts: Optional[ListOrDict] = None
-    isolation: Optional[str] = None
-    privileged: Optional[bool] = None
-    secrets: Optional[ServiceConfigOrSecret] = None
-    tags: Optional[List[str]] = None
-    platforms: Optional[List[str]] = None
-
-
-class BlkioConfig(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    device_read_bps: Optional[List[BlkioLimit]] = None
-    device_read_iops: Optional[List[BlkioLimit]] = None
-    device_write_bps: Optional[List[BlkioLimit]] = None
-    device_write_iops: Optional[List[BlkioLimit]] = None
-    weight: Optional[int] = None
-    weight_device: Optional[List[BlkioWeight]] = None
-
-
-class ServiceNetwork(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    aliases: Optional[ListOfStrings] = None
-    ipv4_address: Optional[str] = None
-    ipv6_address: Optional[str] = None
-    link_local_ips: Optional[ListOfStrings] = None
-    priority: Optional[float] = None
-
-
-class Device(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    capabilities: Optional[ListOfStrings] = None
-    count: Optional[Union[str, int]] = None
-    device_ids: Optional[ListOfStrings] = None
-    driver: Optional[str] = None
-    options: Optional[ListOrDict] = None
-
-
-class Devices(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    __root__: List[Device]
-
-
-class Network(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    name: Optional[str] = None
-    driver: Optional[str] = None
-    driver_opts: Optional[Dict[constr(regex=r"^.+$"), Union[str, float]]] = None  # type: ignore  # noqa: F722
-    ipam: Optional[Ipam] = None
-    external: Optional[bool | ExternalNetwork] = None
-    internal: Optional[bool] = None
-    enable_ipv6: Optional[bool] = None
-    attachable: Optional[bool] = None
-    labels: Optional[ListOrDict] = None
-
-
-class Volume(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    name: Optional[str] = None
-    driver: Optional[str] = None
-    driver_opts: Optional[Dict[constr(regex=r"^.+$"), Union[str, float]]] = None  # type: ignore  # noqa: F722
-    external: Optional[ExternalVolume] = None
-    labels: Optional[ListOrDict] = None
-
-
-class Secret(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    name: Optional[str] = None
-    environment: Optional[str] = None
-    file: Optional[str] = None
-    external: Optional[ExternalSecret] = None
-    labels: Optional[ListOrDict] = None
-    driver: Optional[str] = None
-    driver_opts: Optional[Dict[constr(regex=r"^.+$"), Union[str, float]]] = None  # type: ignore  # noqa: F722
-    template_driver: Optional[str] = None
-
-
-class Config(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    name: Optional[str] = None
-    file: Optional[str] = None
-    external: Optional[ExternalConfig] = None
-    labels: Optional[ListOrDict] = None
-    template_driver: Optional[str] = None
-
-
-class StringOrList(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    __root__: Union[str, ListOfStrings]
-
-
-class Reservations(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    cpus: Optional[Union[float, str]] = None
-    memory: Optional[str] = None
-    generic_resources: Optional[GenericResources] = None
-    devices: Optional[Devices] = None
-
-
-class Resources(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    limits: Optional[Limits] = None
-    reservations: Optional[Reservations] = None
-
-
-class Deployment(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    mode: Optional[str] = None
-    endpoint_mode: Optional[str] = None
-    replicas: Optional[int] = None
-    labels: Optional[ListOrDict] = None
-    rollback_config: Optional[RollbackConfig] = None
-    update_config: Optional[UpdateConfig] = None
-    resources: Optional[Resources] = None
-    restart_policy: Optional[RestartPolicy] = None
-    placement: Optional[Placement] = None
-
-
-class Service(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    deploy: Optional[Deployment] = None
-    build: Optional[Union[str, BuildItem]] = None
-    blkio_config: Optional[BlkioConfig] = None
-    cap_add: Optional[List[str]] = Field(None, unique_items=True)
-    cap_drop: Optional[List[str]] = Field(None, unique_items=True)
-    cgroup: Optional[Cgroup] = None
-    cgroup_parent: Optional[str] = None
-    command: Optional[Union[str, List[str]]] = None
-    configs: Optional[ServiceConfigOrSecret] = None
-    container_name: Optional[str] = None
-    cpu_count: Optional[conint(ge=0)] = None  # type: ignore
-    cpu_percent: Optional[conint(ge=0, le=100)] = None  # type: ignore
-    cpu_shares: Optional[Union[float, str]] = None
-    cpu_quota: Optional[Union[float, str]] = None
-    cpu_period: Optional[Union[float, str]] = None
-    cpu_rt_period: Optional[Union[float, str]] = None
-    cpu_rt_runtime: Optional[Union[float, str]] = None
-    cpus: Optional[Union[float, str]] = None
-    cpuset: Optional[str] = None
-    credential_spec: Optional[CredentialSpec] = None
-    depends_on: Optional[
-        Union[ListOfStrings, Dict[constr(regex=r"^[a-zA-Z0-9._-]+$"), DependsOn]]  # type: ignore  # noqa: F722, E501
-    ] = None
-    device_cgroup_rules: Optional[ListOfStrings] = None
-    devices: Optional[List[str]] = Field(None, unique_items=True)
-    dns: Optional[StringOrList] = None
-    dns_opt: Optional[List[str]] = Field(None, unique_items=True)
-    dns_search: Optional[StringOrList] = None
-    domainname: Optional[str] = None
-    entrypoint: Optional[Union[str, List[str]]] = None
-    env_file: Optional[StringOrList] = None
-    environment: Optional[ListOrDict] = None
-    expose: Optional[List[Union[str, float]]] = Field(None, unique_items=True)
-    extends: Optional[Union[str, Extend]] = None
-    external_links: Optional[List[str]] = Field(None, unique_items=True)
-    extra_hosts: Optional[ListOrDict] = None
-    group_add: Optional[List[Union[str, float]]] = Field(None, unique_items=True)
-    healthcheck: Optional[Healthcheck] = None
-    hostname: Optional[str] = None
-    image: Optional[str] = None
-    init: Optional[bool] = None
-    ipc: Optional[str] = None
-    isolation: Optional[str] = None
-    labels: Optional[ListOrDict] = None
-    links: Optional[List[str]] = Field(None, unique_items=True)
-    logging: Optional[Logging] = None
-    mac_address: Optional[str] = None
-    mem_limit: Optional[Union[float, str]] = None
-    mem_reservation: Optional[Union[str, int]] = None
-    mem_swappiness: Optional[int] = None
-    memswap_limit: Optional[Union[float, str]] = None
-    network_mode: Optional[str] = None
-    networks: Optional[
-        Union[
-            ListOfStrings, Dict[constr(regex=r"^[a-zA-Z0-9._-]+$"), Optional[ServiceNetwork]]  # type: ignore  # noqa: F722, E501
-        ]
-    ] = None
-    oom_kill_disable: Optional[bool] = None
-    oom_score_adj: Optional[conint(ge=-1000, le=1000)] = None  # type: ignore
-    pid: Optional[str] = None
-    pids_limit: Optional[Union[float, str]] = None
-    platform: Optional[str] = None
-    ports: Optional[List[Union[float, str, Port]]] = Field(None, unique_items=True)
-    privileged: Optional[bool] = None
-    profiles: Optional[ListOfStrings] = None
-    pull_policy: Optional[PullPolicy] = None
-    read_only: Optional[bool] = None
-    restart: Optional[str] = None
-    runtime: Optional[str] = None
-    scale: Optional[int] = None
-    security_opt: Optional[List[str]] = Field(None, unique_items=True)
-    shm_size: Optional[Union[float, str]] = None
-    secrets: Optional[ServiceConfigOrSecret] = None
-    sysctls: Optional[ListOrDict] = None
-    stdin_open: Optional[bool] = None
-    stop_grace_period: Optional[str] = None
-    stop_signal: Optional[str] = None
-    storage_opt: Optional[Dict[str, Any]] = None
-    tmpfs: Optional[StringOrList] = None
-    tty: Optional[bool] = None
-    ulimits: Optional[Dict[constr(regex=r"^[a-z]+$"), Union[int, Ulimit]]] = None  # type: ignore  # noqa: F722
-    user: Optional[str] = None
-    uts: Optional[str] = None
-    userns_mode: Optional[str] = None
-    volumes: Optional[List[Union[str, ServiceVolume]]] = Field(None, unique_items=True)
-    volumes_from: Optional[List[str]] = Field(None, unique_items=True)
-    working_dir: Optional[str] = None
-
-
-class ComposeSpecification(YamlModel):
-    class Config:
-        extra = Extra.allow
-
-    version: Optional[str] = Field(None, description="declared for backward compatibility, ignored.")
-    name: Optional[constr(regex=r"^[a-z0-9][a-z0-9_-]*$")] = Field(  # type: ignore  # noqa: F722
-        None,
-        description="define the Compose project name, until user defines one explicitly.",
-    )
-    services: Optional[Dict[constr(regex=r"^[a-zA-Z0-9._-]+$"), Service]] = None  # type: ignore  # noqa: F722
-    networks: Optional[Dict[constr(regex=r"^[a-zA-Z0-9._-]+$"), Optional[Network]]] = None  # type: ignore  # noqa: F722
-    volumes: Optional[Dict[constr(regex=r"^[a-zA-Z0-9._-]+$"), Optional[Volume]]] = None  # type: ignore  # noqa: F722
-    secrets: Optional[Dict[constr(regex=r"^[a-zA-Z0-9._-]+$"), Secret]] = None  # type: ignore  # noqa: F722
-    configs: Optional[Dict[constr(regex=r"^[a-zA-Z0-9._-]+$"), Config]] = None  # type: ignore  # noqa: F722
+# generated by datamodel-codegen:
+#   filename:  compose-spec.json
+#   timestamp: 2024-04-27T08:31:04+00:00
+
+from __future__ import annotations
+
+from enum import Enum
+from typing import Any, Dict, List, Optional, Union
+
+from pydantic import BaseModel, ConfigDict, Field, RootModel
+
+
+class Cgroup(Enum):
+    host = "host"
+    private = "private"
+
+
+class CredentialSpec(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    config: Optional[str] = None
+    file: Optional[str] = None
+    registry: Optional[str] = None
+
+
+class Condition(Enum):
+    service_started = "service_started"
+    service_healthy = "service_healthy"
+    service_completed_successfully = "service_completed_successfully"
+
+
+class DependsOn(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    restart: Optional[bool] = None
+    required: Optional[bool] = True
+    condition: Condition
+
+
+class Extends(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    service: str
+    file: Optional[str] = None
+
+
+class Logging(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    driver: Optional[str] = None
+    options: Optional[Dict[str, Optional[Union[str, float]]]] = None
+
+
+class Ports(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    name: Optional[str] = None
+    mode: Optional[str] = None
+    host_ip: Optional[str] = None
+    target: Optional[int] = None
+    published: Optional[Union[str, int]] = None
+    protocol: Optional[str] = None
+    app_protocol: Optional[str] = None
+
+
+class PullPolicy(Enum):
+    always = "always"
+    never = "never"
+    if_not_present = "if_not_present"
+    build = "build"
+    missing = "missing"
+
+
+class Selinux(Enum):
+    z = "z"
+    Z = "Z"
+
+
+class Bind(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    propagation: Optional[str] = None
+    create_host_path: Optional[bool] = None
+    selinux: Optional[Selinux] = None
+
+
+class AdditionalVolumeOption(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    nocopy: Optional[bool] = None
+    subpath: Optional[str] = None
+
+
+class Size(RootModel[int]):
+    root: int = Field(..., ge=0)
+
+
+class Tmpfs(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    size: Optional[Union[Size, str]] = None
+    mode: Optional[float] = None
+
+
+class Volumes(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    type: str
+    source: Optional[str] = None
+    target: Optional[str] = None
+    read_only: Optional[bool] = None
+    consistency: Optional[str] = None
+    bind: Optional[Bind] = None
+    volume: Optional[AdditionalVolumeOption] = None
+    tmpfs: Optional[Tmpfs] = None
+
+
+class Healthcheck(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    disable: Optional[bool] = None
+    interval: Optional[str] = None
+    retries: Optional[float] = None
+    test: Optional[Union[str, List[str]]] = None
+    timeout: Optional[str] = None
+    start_period: Optional[str] = None
+    start_interval: Optional[str] = None
+
+
+class Action(Enum):
+    rebuild = "rebuild"
+    sync = "sync"
+    sync_restart = "sync+restart"
+
+
+class WatchItem(BaseModel):
+    ignore: Optional[List[str]] = None
+    path: str
+    action: Action
+    target: Optional[str] = None
+
+
+class Development(BaseModel):
+    watch: Optional[List[WatchItem]] = None
+
+
+class Order(Enum):
+    start_first = "start-first"
+    stop_first = "stop-first"
+
+
+class RollbackConfig(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    parallelism: Optional[int] = None
+    delay: Optional[str] = None
+    failure_action: Optional[str] = None
+    monitor: Optional[str] = None
+    max_failure_ratio: Optional[float] = None
+    order: Optional[Order] = None
+
+
+class UpdateConfig(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    parallelism: Optional[int] = None
+    delay: Optional[str] = None
+    failure_action: Optional[str] = None
+    monitor: Optional[str] = None
+    max_failure_ratio: Optional[float] = None
+    order: Optional[Order] = None
+
+
+class Limits(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    cpus: Optional[Union[float, str]] = None
+    memory: Optional[str] = None
+    pids: Optional[int] = None
+
+
+class RestartPolicy(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    condition: Optional[str] = None
+    delay: Optional[str] = None
+    max_attempts: Optional[int] = None
+    window: Optional[str] = None
+
+
+class Preference(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    spread: Optional[str] = None
+
+
+class Placement(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    constraints: Optional[List[str]] = None
+    preferences: Optional[List[Preference]] = None
+    max_replicas_per_node: Optional[int] = None
+
+
+class DiscreteResourceSpec(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    kind: Optional[str] = None
+    value: Optional[float] = None
+
+
+class GenericResource(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    discrete_resource_spec: Optional[DiscreteResourceSpec] = None
+
+
+class GenericResources(RootModel[List[GenericResource]]):
+    root: List[GenericResource]
+
+
+class ConfigItem(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    subnet: Optional[str] = None
+    ip_range: Optional[str] = None
+    gateway: Optional[str] = None
+    aux_addresses: Optional[Dict[str, str]] = None
+
+
+class Ipam(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    driver: Optional[str] = None
+    config: Optional[List[ConfigItem]] = None
+    options: Optional[Dict[str, str]] = None
+
+
+class ExternalVolumeNetwork(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    name: Optional[str] = None
+
+
+class ExternalConfig(BaseModel):
+    name: Optional[str] = None
+
+
+class Command(RootModel[Optional[Union[str, List[str]]]]):
+    root: Optional[Union[str, List[str]]]
+
+
+class EnvFilePath(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    path: str
+    required: Optional[bool] = True
+
+
+class EnvFile(RootModel[Union[str, List[Union[str, EnvFilePath]]]]):
+    root: Union[str, List[Union[str, EnvFilePath]]]
+
+
+class ListOfStrings(RootModel[List[str]]):
+    root: List[str]
+
+
+class ListOrDict1(RootModel[List[Any]]):
+    root: List[Any]
+
+
+class ListOrDict(RootModel[Union[Dict[str, Optional[Union[str, float, bool]]], ListOrDict1]]):
+    root: Union[Dict[str, Optional[Union[str, float, bool]]], ListOrDict1]
+
+
+class BlkioLimit(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    path: Optional[str] = None
+    rate: Optional[Union[int, str]] = None
+
+
+class BlkioWeight(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    path: Optional[str] = None
+    weight: Optional[int] = None
+
+
+class ServiceConfigOrSecret1(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    source: Optional[str] = None
+    target: Optional[str] = None
+    uid: Optional[str] = None
+    gid: Optional[str] = None
+    mode: Optional[float] = None
+
+
+class ServiceConfigOrSecret(RootModel[List[Union[str, ServiceConfigOrSecret1]]]):
+    root: List[Union[str, ServiceConfigOrSecret1]]
+
+
+class Ulimits1(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    hard: int
+    soft: int
+
+
+class Ulimits(RootModel[Dict[str, Union[int, Ulimits1]]]):
+    root: Dict[str, Union[int, Ulimits1]]
+
+
+class Constraints(RootModel[Any]):
+    root: Any
+
+
+class Build(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    context: Optional[str] = None
+    dockerfile: Optional[str] = None
+    dockerfile_inline: Optional[str] = None
+    entitlements: Optional[List[str]] = None
+    args: Optional[ListOrDict] = None
+    ssh: Optional[ListOrDict] = None
+    labels: Optional[ListOrDict] = None
+    cache_from: Optional[List[str]] = None
+    cache_to: Optional[List[str]] = None
+    no_cache: Optional[bool] = None
+    additional_contexts: Optional[ListOrDict] = None
+    network: Optional[str] = None
+    pull: Optional[bool] = None
+    target: Optional[str] = None
+    shm_size: Optional[Union[int, str]] = None
+    extra_hosts: Optional[ListOrDict] = None
+    isolation: Optional[str] = None
+    privileged: Optional[bool] = None
+    secrets: Optional[ServiceConfigOrSecret] = None
+    tags: Optional[List[str]] = None
+    ulimits: Optional[Ulimits] = None
+    platforms: Optional[List[str]] = None
+
+
+class BlkioConfig(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    device_read_bps: Optional[List[BlkioLimit]] = None
+    device_read_iops: Optional[List[BlkioLimit]] = None
+    device_write_bps: Optional[List[BlkioLimit]] = None
+    device_write_iops: Optional[List[BlkioLimit]] = None
+    weight: Optional[int] = None
+    weight_device: Optional[List[BlkioWeight]] = None
+
+
+class Networks(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    aliases: Optional[ListOfStrings] = None
+    ipv4_address: Optional[str] = None
+    ipv6_address: Optional[str] = None
+    link_local_ips: Optional[ListOfStrings] = None
+    mac_address: Optional[str] = None
+    priority: Optional[float] = None
+
+
+class Device(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    capabilities: Optional[ListOfStrings] = None
+    count: Optional[Union[str, int]] = None
+    device_ids: Optional[ListOfStrings] = None
+    driver: Optional[str] = None
+    options: Optional[ListOrDict] = None
+
+
+class Devices(RootModel[List[Device]]):
+    root: List[Device]
+
+
+class Network(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    name: Optional[str] = None
+    driver: Optional[str] = None
+    driver_opts: Optional[Dict[str, Union[str, float]]] = None
+    ipam: Optional[Ipam] = None
+    external: Optional[ExternalVolumeNetwork] = None
+    internal: Optional[bool] = None
+    enable_ipv6: Optional[bool] = None
+    attachable: Optional[bool] = None
+    labels: Optional[ListOrDict] = None
+
+
+class Volume(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    name: Optional[str] = None
+    driver: Optional[str] = None
+    driver_opts: Optional[Dict[str, Union[str, float]]] = None
+    external: Optional[ExternalVolumeNetwork] = None
+    labels: Optional[ListOrDict] = None
+
+
+class Secret(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    name: Optional[str] = None
+    environment: Optional[str] = None
+    file: Optional[str] = None
+    external: Optional[ExternalConfig] = None
+    labels: Optional[ListOrDict] = None
+    driver: Optional[str] = None
+    driver_opts: Optional[Dict[str, Union[str, float]]] = None
+    template_driver: Optional[str] = None
+
+
+class Config(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    name: Optional[str] = None
+    content: Optional[str] = None
+    environment: Optional[str] = None
+    file: Optional[str] = None
+    external: Optional[ExternalConfig] = None
+    labels: Optional[ListOrDict] = None
+    template_driver: Optional[str] = None
+
+
+class StringOrList(RootModel[Union[str, ListOfStrings]]):
+    root: Union[str, ListOfStrings]
+
+
+class Reservations(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    cpus: Optional[Union[float, str]] = None
+    memory: Optional[str] = None
+    generic_resources: Optional[GenericResources] = None
+    devices: Optional[Devices] = None
+
+
+class Resources(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    limits: Optional[Limits] = None
+    reservations: Optional[Reservations] = None
+
+
+class Deployment(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    mode: Optional[str] = None
+    endpoint_mode: Optional[str] = None
+    replicas: Optional[int] = None
+    labels: Optional[ListOrDict] = None
+    rollback_config: Optional[RollbackConfig] = None
+    update_config: Optional[UpdateConfig] = None
+    resources: Optional[Resources] = None
+    restart_policy: Optional[RestartPolicy] = None
+    placement: Optional[Placement] = None
+
+
+class Include1(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    path: Optional[StringOrList] = None
+    env_file: Optional[StringOrList] = None
+    project_directory: Optional[str] = None
+
+
+class Include(RootModel[Union[str, Include1]]):
+    root: Union[str, Include1]
+
+
+class Service(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    develop: Optional[Development] = None
+    deploy: Optional[Deployment] = None
+    annotations: Optional[ListOrDict] = None
+    attach: Optional[bool] = None
+    build: Optional[Union[str, Build]] = None
+    blkio_config: Optional[BlkioConfig] = None
+    cap_add: Optional[List[str]] = None
+    cap_drop: Optional[List[str]] = None
+    cgroup: Optional[Cgroup] = None
+    cgroup_parent: Optional[str] = None
+    command: Optional[Command] = None
+    configs: Optional[ServiceConfigOrSecret] = None
+    container_name: Optional[str] = None
+    cpu_count: Optional[int] = Field(None, ge=0)
+    cpu_percent: Optional[int] = Field(None, ge=0, le=100)
+    cpu_shares: Optional[Union[float, str]] = None
+    cpu_quota: Optional[Union[float, str]] = None
+    cpu_period: Optional[Union[float, str]] = None
+    cpu_rt_period: Optional[Union[float, str]] = None
+    cpu_rt_runtime: Optional[Union[float, str]] = None
+    cpus: Optional[Union[float, str]] = None
+    cpuset: Optional[str] = None
+    credential_spec: Optional[CredentialSpec] = None
+    depends_on: Optional[Union[ListOfStrings, Dict[str, DependsOn]]] = None
+    device_cgroup_rules: Optional[ListOfStrings] = None
+    devices: Optional[List[str]] = None
+    dns: Optional[StringOrList] = None
+    dns_opt: Optional[List[str]] = None
+    dns_search: Optional[StringOrList] = None
+    domainname: Optional[str] = None
+    entrypoint: Optional[Command] = None
+    env_file: Optional[EnvFile] = None
+    environment: Optional[ListOrDict] = None
+    expose: Optional[List[Union[str, float]]] = None
+    extends: Optional[Union[str, Extends]] = None
+    external_links: Optional[List[str]] = None
+    extra_hosts: Optional[ListOrDict] = None
+    group_add: Optional[List[Union[str, float]]] = None
+    healthcheck: Optional[Healthcheck] = None
+    hostname: Optional[str] = None
+    image: Optional[str] = None
+    init: Optional[bool] = None
+    ipc: Optional[str] = None
+    isolation: Optional[str] = None
+    labels: Optional[ListOrDict] = None
+    links: Optional[List[str]] = None
+    logging: Optional[Logging] = None
+    mac_address: Optional[str] = None
+    mem_limit: Optional[Union[float, str]] = None
+    mem_reservation: Optional[Union[str, int]] = None
+    mem_swappiness: Optional[int] = None
+    memswap_limit: Optional[Union[float, str]] = None
+    network_mode: Optional[str] = None
+    networks: Optional[Union[ListOfStrings, Dict[str, Optional[Networks]]]] = None
+    oom_kill_disable: Optional[bool] = None
+    oom_score_adj: Optional[int] = Field(None, ge=-1000, le=1000)
+    pid: Optional[str] = None
+    pids_limit: Optional[Union[float, str]] = None
+    platform: Optional[str] = None
+    ports: Optional[List[Union[float, str, Ports]]] = None
+    privileged: Optional[bool] = None
+    profiles: Optional[ListOfStrings] = None
+    pull_policy: Optional[PullPolicy] = None
+    read_only: Optional[bool] = None
+    restart: Optional[str] = None
+    runtime: Optional[str] = None
+    scale: Optional[int] = None
+    security_opt: Optional[List[str]] = None
+    shm_size: Optional[Union[float, str]] = None
+    secrets: Optional[ServiceConfigOrSecret] = None
+    sysctls: Optional[ListOrDict] = None
+    stdin_open: Optional[bool] = None
+    stop_grace_period: Optional[str] = None
+    stop_signal: Optional[str] = None
+    storage_opt: Optional[Dict[str, Any]] = None
+    tmpfs: Optional[StringOrList] = None
+    tty: Optional[bool] = None
+    ulimits: Optional[Ulimits] = None
+    user: Optional[str] = None
+    uts: Optional[str] = None
+    userns_mode: Optional[str] = None
+    volumes: Optional[List[Union[str, Volumes]]] = None
+    volumes_from: Optional[List[str]] = None
+    working_dir: Optional[str] = None
+
+
+class ComposeSpecification(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+    )
+    version: Optional[str] = Field(None, description="declared for backward compatibility, ignored.")
+    name: Optional[str] = Field(
+        None,
+        description="define the Compose project name, until user defines one explicitly.",
+        pattern="^[a-z0-9][a-z0-9_-]*$",
+    )
+    include: Optional[List[Include]] = Field(None, description="compose sub-projects to be included.")
+    services: Optional[Dict[str, Service]] = None
+    networks: Optional[Dict[str, Optional[Network]]] = None
+    volumes: Optional[Dict[str, Optional[Volume]]] = None
+    secrets: Optional[Dict[str, Secret]] = None
+    configs: Optional[Dict[str, Config]] = None
```

### Comparing `compose_viz-0.3.1/PKG-INFO` & `compose_viz-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: compose-viz
-Version: 0.3.1
+Version: 0.3.2
 Summary: A compose file visualization tool that supports compose-spec and allows you to gernerate graph in several formats.
 Home-page: https://github.com/compose-viz/compose-viz
 License: MIT
 Author: Xyphuz Wu
 Author-email: xyphuzwu@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyYAML (>=6.0,<7.0)
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: graphviz (>=0.20,<0.21)
-Requires-Dist: pydantic-yaml (>=0.7.0,<0.8.0)
-Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
+Requires-Dist: pydantic-yaml (>=1.3.0,<2.0.0)
 Requires-Dist: typer (>=0.4.1,<0.5.0)
 Project-URL: Repository, https://github.com/compose-viz/compose-viz
 Description-Content-Type: text/markdown
 
 <div id="top"></div>
 
 <!-- PROJECT SHIELDS -->
@@ -140,14 +139,15 @@
 ### Options
 
 | Option                            | Description                                                                                                                                                                         |
 | --------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `-o, --output-filename FILENAME`  | Output filename for the generated visualization file. [default: compose-viz]                                                                                                        |
 | `-m, --format FORMAT`             | Output format for the generated visualization file. See [supported formats](https://github.com/compose-viz/compose-viz/blob/main/compose_viz/models/viz_formats.py). [default: png] |
 | `-r, --root-service SERVICE_NAME` | Root of the service tree (convenient for large compose yamls)                                                                                                                       |
+| `-l, --legend`                    | Include a legend in the visualization.                                                                                                                                              |
 | `-v, --version`                   | Show the version of compose-viz.                                                                                                                                                    |
 | `--help`                          | Show help and exit.                                                                                                                                                                 |
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- ROADMAP -->
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: compose-viz Version: 0.3.1 Summary: A compose file
+Metadata-Version: 2.1 Name: compose-viz Version: 0.3.2 Summary: A compose file
 visualization tool that supports compose-spec and allows you to gernerate graph
 in several formats. Home-page: https://github.com/compose-viz/compose-viz
 License: MIT Author: Xyphuz Wu Author-email: xyphuzwu@gmail.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: PyYAML
-(>=6.0,<7.0) Requires-Dist: graphviz (>=0.20,<0.21) Requires-Dist: pydantic-
-yaml (>=0.7.0,<0.8.0) Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0) Requires-
-Dist: typer (>=0.4.1,<0.5.0) Project-URL: Repository, https://github.com/
-compose-viz/compose-viz Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Requires-Dist: graphviz (>=0.20,<0.21) Requires-
+Dist: pydantic-yaml (>=1.3.0,<2.0.0) Requires-Dist: typer (>=0.4.1,<0.5.0)
+Project-URL: Repository, https://github.com/compose-viz/compose-viz
+Description-Content-Type: text/markdown
 [
    ![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
  shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![MIT License]
 [license-shield]][license-url] [![Issues][issues-shield]][issues-url] [![Issues
                          Closed][issues-closed-shield]
 ][issues-closed-url]
 ![compose-viz](https://socialify.git.ci/compose-viz/compose-viz/
@@ -62,16 +62,16 @@
 -------------------------------------------------------------------------------
 ----------------------------- | | `-o, --output-filename FILENAME` | Output
 filename for the generated visualization file. [default: compose-viz] | | `-m,
 --format FORMAT` | Output format for the generated visualization file. See
 [supported formats](https://github.com/compose-viz/compose-viz/blob/main/
 compose_viz/models/viz_formats.py). [default: png] | | `-r, --root-service
 SERVICE_NAME` | Root of the service tree (convenient for large compose yamls) |
-| `-v, --version` | Show the version of compose-viz. | | `--help` | Show help
-and exit. |
+| `-l, --legend` | Include a legend in the visualization. | | `-v, --version` |
+Show the version of compose-viz. | | `--help` | Show help and exit. |
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Roadmap - [ ] Support more vizualization components. See the [open issues]
 (https://github.com/compose-viz/compose-viz/issues) for a full list of proposed
 features (and known issues).
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
```

