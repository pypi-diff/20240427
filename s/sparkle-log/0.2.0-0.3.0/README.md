# Comparing `tmp/sparkle_log-0.2.0.tar.gz` & `tmp/sparkle_log-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkle_log-0.2.0.tar", max compression
+gzip compressed data, was "sparkle_log-0.3.0.tar", max compression
```

## Comparing `sparkle_log-0.2.0.tar` & `sparkle_log-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       55 2024-04-24 16:13:07.409587 sparkle_log-0.2.0/AUTHORS.md
--rw-r--r--   0        0        0     1071 2024-04-24 16:13:07.409587 sparkle_log-0.2.0/LICENSE
--rw-r--r--   0        0        0     1947 2024-04-24 16:13:07.409587 sparkle_log-0.2.0/README.md
--rw-r--r--   0        0        0     5332 2024-04-24 16:13:07.409587 sparkle_log-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      718 2024-04-24 16:13:07.409587 sparkle_log-0.2.0/sparkle_log/__about__.py
--rw-r--r--   0        0        0      397 2024-04-24 16:13:07.409587 sparkle_log-0.2.0/sparkle_log/__init__.py
--rw-r--r--   0        0        0     2980 2024-04-24 16:13:07.409587 sparkle_log-0.2.0/sparkle_log/__main__.py
--rw-r--r--   0        0        0     1940 2024-04-24 16:13:07.409587 sparkle_log-0.2.0/sparkle_log/as_context_manager.py
--rw-r--r--   0        0        0     1179 2024-04-24 16:13:07.409587 sparkle_log-0.2.0/sparkle_log/as_decorator.py
--rw-r--r--   0        0        0     1990 2024-04-24 16:13:07.409587 sparkle_log-0.2.0/sparkle_log/drive_space.py
--rw-r--r--   0        0        0       84 2024-04-24 16:13:07.409587 sparkle_log-0.2.0/sparkle_log/graphs.py
--rw-r--r--   0        0        0     1924 2024-04-24 16:13:07.409587 sparkle_log-0.2.0/sparkle_log/log_writer.py
--rw-r--r--   0        0        0        0 2024-04-24 16:13:07.409587 sparkle_log-0.2.0/sparkle_log/py.typed
--rw-r--r--   0        0        0      454 2024-04-24 16:13:07.413587 sparkle_log-0.2.0/sparkle_log/scheduler.py
--rw-r--r--   0        0        0      254 2024-04-24 16:13:07.413587 sparkle_log-0.2.0/sparkle_log/ui.py
--rw-r--r--   0        0        0     3241 1970-01-01 00:00:00.000000 sparkle_log-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       55 2024-04-27 18:40:34.684340 sparkle_log-0.3.0/AUTHORS.md
+-rw-r--r--   0        0        0     1071 2024-04-27 18:40:34.684340 sparkle_log-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1947 2024-04-27 18:40:34.684340 sparkle_log-0.3.0/README.md
+-rw-r--r--   0        0        0     5338 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      836 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/__about__.py
+-rw-r--r--   0        0        0      397 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/__init__.py
+-rw-r--r--   0        0        0     3542 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/__main__.py
+-rw-r--r--   0        0        0     2085 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/as_context_manager.py
+-rw-r--r--   0        0        0     1251 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/as_decorator.py
+-rw-r--r--   0        0        0     2464 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/drive_space.py
+-rw-r--r--   0        0        0      109 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/graphs.py
+-rw-r--r--   0        0        0     2722 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/log_writer.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/py.typed
+-rw-r--r--   0        0        0      526 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/scheduler.py
+-rw-r--r--   0        0        0     2464 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/ui.py
+-rw-r--r--   0        0        0     3251 1970-01-01 00:00:00.000000 sparkle_log-0.3.0/PKG-INFO
```

### Comparing `sparkle_log-0.2.0/LICENSE` & `sparkle_log-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkle_log-0.2.0/README.md` & `sparkle_log-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sparkle_log-0.2.0/pyproject.toml` & `sparkle_log-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sparkle-log"
-version = "0.2.0"
+version = "0.3.0"
 description = "Write sparkline graphs of CPU and memory usage to your logs."
 authors = ["Matthew Martin <matthewdeanmartin@gmail.com>"]
 keywords = ["monitoring", "logging" ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -35,15 +35,15 @@
 sparkle_log = 'sparkle_log.__main__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 
 psutil = "*"
 schedule = "*"
-sparklines = "*"
+sparklines = ">=0.5.0"
 colorlog = ">=6.8.0"
 
 # TODO: 3rd party sparkline graphs
 
 [tool.poetry.dev-dependencies]
 # ui for verbose loggging
```

### Comparing `sparkle_log-0.2.0/sparkle_log/__about__.py` & `sparkle_log-0.3.0/sparkle_log/__about__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,20 +8,22 @@
     "__author_email__",
     "__keywords__",
     "__status__",
     "__license__",
     "__readme__",
     "__repository__",
     "__homepage__",
+    "__documentation__",
 ]
 
 __title__ = "sparkle-log"
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 __description__ = "Write sparkline graphs of CPU and memory usage to your logs."
 __author__ = "Matthew Martin"
 __author_email__ = "matthewdeanmartin@gmail.com"
 __keywords__ = ["monitoring", "logging"]
 __status__ = "4 - Beta"
 __license__ = "MIT"
 __readme__ = "README.md"
 __repository__ = "https://github.com/matthewdeanmartin/sparkle_log"
 __homepage__ = "https://github.com/matthewdeanmartin/sparkle_log"
+__documentation__ = "https://matthewdeanmartin.github.io/sparkle_log/sparkle_log/index.html"
```

### Comparing `sparkle_log-0.2.0/sparkle_log/__main__.py` & `sparkle_log-0.3.0/sparkle_log/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,43 +4,49 @@
 """
 
 import argparse
 import logging
 import logging.config
 import sys
 import time
-from typing import Optional, Sequence
+from typing import Optional, Sequence, cast
 
+from sparkle_log.__about__ import __version__
 from sparkle_log.as_context_manager import MetricsLoggingContext
 from sparkle_log.as_decorator import monitor_metrics_on_call
+from sparkle_log.ui import GraphStyle
 
 
 @monitor_metrics_on_call(("cpu",), 1)
 def log_memory_and_cpu():
+    """Example with decorator"""
     while True:
         time.sleep(4)
         print("Executing demo...")
 
 
-def log_memory_and_cpu_cli(metrics=("cpu", "memory"), interval: int = 1, duration: int = 10):
+def log_memory_and_cpu_cli(
+    metrics=("cpu", "memory", "drive"), interval: int = 1, duration: int = 10, style: GraphStyle = "bar"
+):
     """
     Log memory and CPU metrics using the Sparkle Log system.
     """
     configure_logging()
-    with MetricsLoggingContext(metrics=metrics, interval=interval):
+    with MetricsLoggingContext(metrics=metrics, interval=interval, style=style):
         # Execute some operations
         print("Demo of Sparkle Monitoring system metrics during operations...")
         time.sleep(int(duration / 3))
         print("Maybe CPU intensive work done here...")
         time.sleep(int(duration / 3))
         print("Maybe Memory intensive work done here...")
         time.sleep(int(duration / 3))
 
 
 def configure_logging() -> None:
+    """Turn on color logging"""
     logging.config.dictConfig(
         {
             "version": 1,
             "formatters": {
                 "colored": {
                     "()": "colorlog.ColoredFormatter",
                     "format": "%(log_color)s%(levelname)-8s%(reset)s %(blue)s%(message)s",
@@ -62,30 +68,41 @@
                 }
             },
         }
     )
 
 
 def main(argv: Optional[Sequence[str]] = None) -> int:
+    """Arg parse code"""
     parser = argparse.ArgumentParser(description="Monitor system metrics using Sparkle Log.")
     parser.add_argument(
         "--metrics",
         type=str,
-        default="cpu,memory",
-        help="Comma-separated list of metrics to monitor (e.g., 'cpu,memory')",
+        default="cpu,memory,drive",
+        help="Comma-separated list of metrics to monitor (e.g., 'cpu,memory,drive')",
     )
     parser.add_argument("--interval", type=int, default=1, help="Interval in seconds between metric logs")
     parser.add_argument("--duration", type=int, default=10, help="Duration in sections to gather metrics")
-    parser.add_argument("--version", action="version", version="Sparkle Log 1.0")
+    # An add_argument call with a choice of bar, faces
+    parser.add_argument(
+        "--style",
+        choices=["bar", "faces", "jagged", "linear", "vertical", "ascii_art", "pie_chart"],
+        default="bar",
+        help="Graph Style",
+    )
+
+    parser.add_argument("--version", action="version", version=f"Sparkle Log {__version__}")
 
     args = parser.parse_args(argv)
 
     # Convert comma-separated string to tuple of metrics
     metrics_tuple = tuple(args.metrics.split(","))
 
     # Call the function with parsed arguments
-    log_memory_and_cpu_cli(metrics=metrics_tuple, interval=args.interval, duration=args.duration)
+    log_memory_and_cpu_cli(
+        metrics=metrics_tuple, interval=args.interval, duration=args.duration, style=cast(GraphStyle, str(args.style))
+    )
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(main(sys.argv[1:]))
```

### Comparing `sparkle_log-0.2.0/sparkle_log/as_context_manager.py` & `sparkle_log-0.3.0/sparkle_log/as_context_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,39 +5,43 @@
 import logging
 import time
 from threading import Event, Thread
 from typing import Any, Optional
 
 from sparkle_log.graphs import GLOBAL_LOGGER
 from sparkle_log.scheduler import run_scheduler
+from sparkle_log.ui import GraphStyle
 
 
 class MetricsLoggingContext:
     """
     Context manager to log system metrics.
     """
 
-    def __init__(self, metrics=("cpu", "memory"), interval: int = 10) -> None:
+    def __init__(self, metrics=("cpu", "memory"), interval: int = 10, style: GraphStyle = "faces") -> None:
         """Initialize the context manager."""
         if not metrics:
             metrics = ("cpu", "memory")
         else:
             for metric in metrics:
-                if metric not in ("cpu", "memory"):
+                if metric not in ("cpu", "memory", "drive"):
                     raise TypeError("Unexpected metric")
         self.metrics = metrics
         self.interval = interval
+        self.style = style
         self.stop_event: Optional[Event] = None
         self.scheduler_thread: Optional[Thread] = None
 
     def __enter__(self) -> "MetricsLoggingContext":
         """Start the context manager, if logging enabled."""
         if GLOBAL_LOGGER.isEnabledFor(logging.INFO):
             self.stop_event = Event()
-            self.scheduler_thread = Thread(target=run_scheduler, args=(self.stop_event, self.metrics, self.interval))
+            self.scheduler_thread = Thread(
+                target=run_scheduler, args=(self.stop_event, self.metrics, self.interval, self.style)
+            )
             self.scheduler_thread.start()
         return self
 
     def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
         """Stop the context manager."""
         if self.scheduler_thread and self.scheduler_thread.is_alive():
             self.stop_event.set()
```

### Comparing `sparkle_log-0.2.0/sparkle_log/as_decorator.py` & `sparkle_log-0.3.0/sparkle_log/as_decorator.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,33 +4,34 @@
 
 import logging
 from functools import wraps
 from threading import Event, Thread
 
 from sparkle_log.graphs import GLOBAL_LOGGER
 from sparkle_log.scheduler import run_scheduler
+from sparkle_log.ui import GraphStyle
 
 INITIALIZED = False
 
 
-def monitor_metrics_on_call(metrics=("cpu", "memory"), interval=10):
+def monitor_metrics_on_call(metrics=("cpu", "memory"), interval=10, style: GraphStyle = "bar"):
     """
     Decorator to monitor the system metrics while the function is being executed.
     """
 
     def decorator(func):
         """Wrapper function"""
 
         @wraps(func)
         def wrapper(*args, **kwargs):
             """Wrapper function"""
             if not GLOBAL_LOGGER.isEnabledFor(logging.INFO):
                 return func(*args, **kwargs)
             stop_event = Event()
-            scheduler_thread = Thread(target=run_scheduler, args=(stop_event, metrics, interval))
+            scheduler_thread = Thread(target=run_scheduler, args=(stop_event, metrics, interval, style))
             scheduler_thread.start()
 
             try:
                 return func(*args, **kwargs)
             finally:
                 # Stop the scheduler and wait for thread to finish
                 stop_event.set()
```

### Comparing `sparkle_log-0.2.0/sparkle_log/drive_space.py` & `sparkle_log-0.3.0/sparkle_log/drive_space.py`

 * *Files 23% similar despite different names*

```diff
@@ -50,30 +50,51 @@
     "fusectl",
     "pstore",
     "sys_kernel_debug",
     "sys_kernel_config",
 }
 
 
-def get_drive_info() -> list[dict[str, Any]]:
+def get_free_percent_for_all_drives() -> float:
+    """
+    Get the percent of free space for all physical drives on the system.
+
+    Returns:
+        float: The percent of free space.
+    """
+    free = 0.0
+    total = 0.0
+    for data in get_drive_info(use_numbers=True):
+        # get percent free
+        free += data["Free Space"]
+        total += data["Total Space"]
+    if total > 0.0:
+        return (free / total) * 100
+    return 0.0
+
+
+def get_drive_info(use_numbers: bool = False) -> list[dict[str, Any]]:
     """
     Get a list of all physical mounted drives with their total and free space, excluding virtual or system mounts.
 
     Returns:
         list[dict[str, Any]]: A list of dictionaries each containing the mount point, total space, and free space.
     """
     drives = []
     for partition in psutil.disk_partitions():
         if partition.fstype not in ignore_fs_types:
             try:
                 usage = psutil.disk_usage(partition.mountpoint)
                 drive = {
                     "Mount Point": partition.mountpoint,
-                    "Total Space": convert_bytes_to_gb(usage.total),
-                    "Free Space": convert_bytes_to_gb(usage.free),
+                    "Total Space": convert_bytes_to_gb(usage.total) if not use_numbers else usage.total,
+                    "Free Space": convert_bytes_to_gb(usage.free) if not use_numbers else usage.free,
                 }
                 drives.append(drive)
-            except PermissionError:
-                LOGGER.debug(f"Access denied to {partition.mountpoint}")
-            except Exception as e:
-                LOGGER.debug(f"Could not access {partition.mountpoint}: {e}")
+            except Exception:
+                # Too noisy.
+                pass
     return drives
+
+
+if __name__ == "__main__":
+    print(get_free_percent_for_all_drives())
```

### Comparing `sparkle_log-0.2.0/sparkle_log/log_writer.py` & `sparkle_log-0.3.0/sparkle_log/log_writer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """
 Log writer module, stateful and does not require a decorator or context manager.
 """
 
 import logging
 import statistics
-from typing import Optional
+from typing import Literal, Optional
 
 import psutil
 
+from sparkle_log.drive_space import get_free_percent_for_all_drives
 from sparkle_log.graphs import GLOBAL_LOGGER
-from sparkle_log.ui import sparkline
+from sparkle_log.ui import GraphStyle, sparkline
 
-READINGS: dict[str, list[Optional[int]]] = {"cpu": [None] * 29, "memory": [None] * 29}
+READINGS: dict[str, list[Optional[int]]] = {"cpu": [None] * 29, "memory": [None] * 29, "drive": [None] * 29}
 
+Metrics = Literal["cpu", "memory", "drive"]
 
-def log_system_metrics(metrics: tuple[str, ...]) -> None:
+
+def log_system_metrics(metrics: tuple[Metrics, ...], style: GraphStyle = "bar") -> None:
     """
     Log system metrics.
 
     Args:
         metrics: A tuple of metrics to log.
+        style: The style of the sparkline.
     """
     if not GLOBAL_LOGGER.isEnabledFor(logging.INFO):
         return
     if "cpu" in metrics:
         # Interval non to prevent blocking.
         # https://psutil.readthedocs.io/en/latest/#psutil.cpu_percent
         interval = None
@@ -32,27 +36,45 @@
         if reading == 0 and interval is None:
             # First reading on interval None is trash, bail.
             return
         READINGS["cpu"].append(int(reading))
     if "memory" in metrics:
         READINGS["memory"].append(int(psutil.virtual_memory().percent))
 
+    if "drive" in metrics:
+        READINGS["drive"].append(int(get_free_percent_for_all_drives()))
+
     for _key, value in READINGS.items():
         if len(value) > 30:  # Keep the last 30 readings
             value.pop(0)
 
     for metric, value in READINGS.items():
         if metric not in metrics:
             continue
         values_for_stats = [_ for _ in value if _ is not None]
-        average = round(statistics.mean(values_for_stats), 1)
-        minimum = min(values_for_stats)
-        maximum = max(values_for_stats)
-        metric_formatted = "  " + str(value[-1])[-2:]
+        average = int(round(statistics.mean(values_for_stats), 0))
+
+        def pad(value: int) -> str:
+            """Pad the value with spaces."""
+            return str(value).rjust(2)
+
+        minimum = pad(min(values_for_stats))
+        maximum = pad(max(values_for_stats))
+        metric_formatted = pad(value[-1])[-2:]
         if metric == "cpu":
             GLOBAL_LOGGER.info(
-                f"CPU   : {metric_formatted}% | {sparkline(value)} | min, mean, max ({minimum}, {average}, {maximum})"
+                f"CPU   : {metric_formatted}% "
+                f"| min, mean, max ({minimum}, {average}, {maximum}) "
+                f"| {sparkline(value, style)}"
             )
         elif metric == "memory":
             GLOBAL_LOGGER.info(
-                f"Memory: {metric_formatted}% | {sparkline(value)} | min, mean, max ({minimum}, {average}, {maximum})"
+                f"Memory: {metric_formatted}% "
+                f"| min, mean, max ({minimum}, {average}, {maximum}) "
+                f"| {sparkline(value, style)}"
+            )
+        elif metric == "drive":
+            GLOBAL_LOGGER.info(
+                f"Drive: {metric_formatted}% "
+                f"| min, mean, max ({minimum}, {average}, {maximum}) "
+                f"| {sparkline(value, style)}"
             )
```

### Comparing `sparkle_log-0.2.0/PKG-INFO` & `sparkle_log-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkle-log
-Version: 0.2.0
+Version: 0.3.0
 Summary: Write sparkline graphs of CPU and memory usage to your logs.
 Home-page: https://github.com/matthewdeanmartin/sparkle_log
 License: MIT
 Keywords: monitoring,logging
 Author: Matthew Martin
 Author-email: matthewdeanmartin@gmail.com
 Requires-Python: >=3.9
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorlog (>=6.8.0)
 Requires-Dist: psutil
 Requires-Dist: schedule
-Requires-Dist: sparklines
+Requires-Dist: sparklines (>=0.5.0)
 Project-URL: Bug Tracker, https://github.com/matthewdeanmartin/sparkle_log/issues
 Project-URL: Change Log, https://github.com/matthewdeanmartin/sparkle_log/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://matthewdeanmartin.github.io/sparkle_log/sparkle_log/index.html
 Project-URL: Repository, https://github.com/matthewdeanmartin/sparkle_log
 Description-Content-Type: text/markdown
 
 # sparkle_log
```

