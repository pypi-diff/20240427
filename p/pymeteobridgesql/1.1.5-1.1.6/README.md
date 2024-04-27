# Comparing `tmp/pymeteobridgesql-1.1.5.tar.gz` & `tmp/pymeteobridgesql-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeteobridgesql-1.1.5.tar", last modified: Fri Apr 26 17:08:28 2024, max compression
+gzip compressed data, was "pymeteobridgesql-1.1.6.tar", last modified: Fri Apr 26 18:15:10 2024, max compression
```

## Comparing `pymeteobridgesql-1.1.5.tar` & `pymeteobridgesql-1.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:08:28.287230 pymeteobridgesql-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 17:08:22.000000 pymeteobridgesql-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-26 17:08:28.287230 pymeteobridgesql-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-26 17:08:22.000000 pymeteobridgesql-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:08:28.283230 pymeteobridgesql-1.1.5/pymeteobridgesql/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-26 17:08:22.000000 pymeteobridgesql-1.1.5/pymeteobridgesql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-26 17:08:22.000000 pymeteobridgesql-1.1.5/pymeteobridgesql/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-04-26 17:08:22.000000 pymeteobridgesql-1.1.5/pymeteobridgesql/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:08:28.283230 pymeteobridgesql-1.1.5/pymeteobridgesql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-26 17:08:28.000000 pymeteobridgesql-1.1.5/pymeteobridgesql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-26 17:08:28.000000 pymeteobridgesql-1.1.5/pymeteobridgesql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 17:08:28.000000 pymeteobridgesql-1.1.5/pymeteobridgesql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-26 17:08:28.000000 pymeteobridgesql-1.1.5/pymeteobridgesql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 17:08:28.287230 pymeteobridgesql-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-26 17:08:22.000000 pymeteobridgesql-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:15:10.498749 pymeteobridgesql-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-26 18:15:06.000000 pymeteobridgesql-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-26 18:15:10.498749 pymeteobridgesql-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-26 18:15:06.000000 pymeteobridgesql-1.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:15:10.498749 pymeteobridgesql-1.1.6/pymeteobridgesql/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-26 18:15:06.000000 pymeteobridgesql-1.1.6/pymeteobridgesql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-26 18:15:06.000000 pymeteobridgesql-1.1.6/pymeteobridgesql/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-04-26 18:15:06.000000 pymeteobridgesql-1.1.6/pymeteobridgesql/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:15:10.498749 pymeteobridgesql-1.1.6/pymeteobridgesql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-26 18:15:10.000000 pymeteobridgesql-1.1.6/pymeteobridgesql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-26 18:15:10.000000 pymeteobridgesql-1.1.6/pymeteobridgesql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 18:15:10.000000 pymeteobridgesql-1.1.6/pymeteobridgesql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-26 18:15:10.000000 pymeteobridgesql-1.1.6/pymeteobridgesql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 18:15:10.498749 pymeteobridgesql-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-26 18:15:06.000000 pymeteobridgesql-1.1.6/setup.py
```

### Comparing `pymeteobridgesql-1.1.5/LICENSE` & `pymeteobridgesql-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymeteobridgesql-1.1.5/PKG-INFO` & `pymeteobridgesql-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeteobridgesql
-Version: 1.1.5
+Version: 1.1.6
 Summary: Gets weather data from a MySQL table
 Home-page: https://github.com/briis/pymeteobridgesql
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymeteobridgesql-1.1.5/pymeteobridgesql/api.py` & `pymeteobridgesql-1.1.6/pymeteobridgesql/api.py`

 * *Files identical despite different names*

### Comparing `pymeteobridgesql-1.1.5/pymeteobridgesql/data.py` & `pymeteobridgesql-1.1.6/pymeteobridgesql/data.py`

 * *Files 26% similar despite different names*

```diff
@@ -173,14 +173,63 @@
         if self.windbearing is None:
             return None
 
         directions = ['N', 'NNE', 'NE', 'ENE', 'E', 'ESE', 'SE', 'SSE', 'S', 'SSW', 'SW', 'WSW', 'W', 'WNW', 'NW', 'NNW']
         index = round(self.windbearing / 22.5) % 16
         return directions[index].lower()
 
+    def to_dict(self):
+        return {
+            "ID": self.ID,
+            "temperature": self.temperature,
+            "tempmax": self.tempmax,
+            "tempmin": self.tempmin,
+            "windchill": self.windchill,
+            "pm1": self.pm1,
+            "pm25": self.pm25,
+            "pm10": self.pm10,
+            "heatindex": self.heatindex,
+            "temp15min": self.temp15min,
+            "humidity": self.humidity,
+            "windspeedavg": self.windspeedavg,
+            "windgust": self.windgust,
+            "dewpoint": self.dewpoint,
+            "rainrate": self.rainrate,
+            "raintoday": self.raintoday,
+            "rainyesterday": self.rainyesterday,
+            "windbearing": self.windbearing,
+            "beaufort": self.beaufort,
+            "sealevelpressure": self.sealevelpressure,
+            "uv": self.uv,
+            "uvdaymax": self.uvdaymax,
+            "solarrad": self.solarrad,
+            "solarraddaymax": self.solarraddaymax,
+            "pressuretrend": self.pressuretrend,
+            "mb_ip": self.mb_ip,
+            "mb_swversion": self.mb_swversion,
+            "mb_buildnum": self.mb_buildnum,
+            "mb_platform": self.mb_platform,
+            "mb_station": self.mb_station,
+            "mb_stationname": self.mb_stationname,
+            "elevation": self.elevation,
+            "description": self.description,
+            "icon": self.icon,
+            "conditions": self.conditions,
+            "absolute_humidity": self.absolute_humidity,
+            "aqi": self.aqi,
+            "beaufort_description": self.beaufort_description,
+            "cloud_base": self.cloud_base,
+            "feels_like_temperature": self.feels_like_temperature,
+            "freezing_altitude": self.freezing_altitude,
+            "pressuretrend_text": self.pressuretrend_text,
+            "uv_description": self.uv_description,
+            "visibility": self.visibility,
+            "wind_direction": self.wind_direction,
+        }
+
 @dataclass(frozen=True)
 class ForecastHourly:
     hour_num: int
     datetime: datetime.datetime
     temperature: float
     apparent_temperature: float
     humidity: int
```

### Comparing `pymeteobridgesql-1.1.5/pymeteobridgesql.egg-info/PKG-INFO` & `pymeteobridgesql-1.1.6/pymeteobridgesql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeteobridgesql
-Version: 1.1.5
+Version: 1.1.6
 Summary: Gets weather data from a MySQL table
 Home-page: https://github.com/briis/pymeteobridgesql
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymeteobridgesql-1.1.5/setup.py` & `pymeteobridgesql-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pymeteobridgesql",
-    version="1.1.5",
+    version="1.1.6",
     author="briis",
     author_email="bjarne@briis.com",
     description="Gets weather data from a MySQL table",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/briis/pymeteobridgesql",
```

