# Comparing `tmp/pyastroweatherio-0.50.0.dev3.tar.gz` & `tmp/pyastroweatherio-0.50.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.50.0.dev3.tar", last modified: Sat Apr 27 10:38:42 2024, max compression
+gzip compressed data, was "pyastroweatherio-0.50.0.dev4.tar", last modified: Sat Apr 27 11:42:08 2024, max compression
```

## Comparing `pyastroweatherio-0.50.0.dev3.tar` & `pyastroweatherio-0.50.0.dev4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-27 10:38:42.974777 pyastroweatherio-0.50.0.dev3/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.50.0.dev3/LICENSE
--rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-04-27 10:38:42.974777 pyastroweatherio-0.50.0.dev3/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.50.0.dev3/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-27 10:38:42.962777 pyastroweatherio-0.50.0.dev3/pyastroweatherio/
--rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.50.0.dev3/pyastroweatherio/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    36515 2024-04-27 10:38:39.000000 pyastroweatherio-0.50.0.dev3/pyastroweatherio/client.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     4002 2024-04-27 09:34:38.000000 pyastroweatherio-0.50.0.dev3/pyastroweatherio/const.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    20099 2024-04-27 09:24:39.000000 pyastroweatherio-0.50.0.dev3/pyastroweatherio/dataclasses.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.50.0.dev3/pyastroweatherio/errors.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    41918 2024-04-26 06:34:43.000000 pyastroweatherio-0.50.0.dev3/pyastroweatherio/helper_functions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-27 10:38:42.970777 pyastroweatherio-0.50.0.dev3/pyastroweatherio.egg-info/
--rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-04-27 10:38:42.000000 pyastroweatherio-0.50.0.dev3/pyastroweatherio.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-04-27 10:38:42.000000 pyastroweatherio-0.50.0.dev3/pyastroweatherio.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-27 10:38:42.000000 pyastroweatherio-0.50.0.dev3/pyastroweatherio.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-04-27 10:38:42.000000 pyastroweatherio-0.50.0.dev3/pyastroweatherio.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-04-27 10:38:42.000000 pyastroweatherio-0.50.0.dev3/pyastroweatherio.egg-info/top_level.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-04-27 10:38:42.974777 pyastroweatherio-0.50.0.dev3/setup.cfg
--rw-rw-r--   0 markus    (1000) markus    (1000)     1390 2024-04-27 10:38:18.000000 pyastroweatherio-0.50.0.dev3/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-27 11:42:08.103517 pyastroweatherio-0.50.0.dev4/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.50.0.dev4/LICENSE
+-rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-04-27 11:42:08.103517 pyastroweatherio-0.50.0.dev4/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.50.0.dev4/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-27 11:42:08.099517 pyastroweatherio-0.50.0.dev4/pyastroweatherio/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      286 2024-04-27 10:55:14.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    37537 2024-04-27 11:42:03.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio/client.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3968 2024-04-27 10:55:14.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio/const.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    20099 2024-04-27 09:24:39.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio/dataclasses.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio/errors.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    42008 2024-04-27 10:59:55.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio/helper_functions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-27 11:42:08.103517 pyastroweatherio-0.50.0.dev4/pyastroweatherio.egg-info/
+-rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-04-27 11:42:08.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-04-27 11:42:08.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-27 11:42:08.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-04-27 11:42:08.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-04-27 11:42:08.000000 pyastroweatherio-0.50.0.dev4/pyastroweatherio.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-04-27 11:42:08.103517 pyastroweatherio-0.50.0.dev4/setup.cfg
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1390 2024-04-27 11:41:15.000000 pyastroweatherio-0.50.0.dev4/setup.py
```

### Comparing `pyastroweatherio-0.50.0.dev3/LICENSE` & `pyastroweatherio-0.50.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.0.dev3/PKG-INFO` & `pyastroweatherio-0.50.0.dev4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.50.0.dev3
+Version: 0.50.0.dev4
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.50.0.dev3/README.md` & `pyastroweatherio-0.50.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.0.dev3/pyastroweatherio/client.py` & `pyastroweatherio-0.50.0.dev4/pyastroweatherio/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,18 +236,30 @@
             "cloud_area_fraction_medium": details_metno.get("cloud_area_fraction_medium", -1),
             "fog_area_fraction": details_metno.get("fog_area_fraction", -1),
             "rh2m": details_metno.get("relative_humidity", -1),
             "wind_speed": details_metno.get("wind_speed", -1),
             "wind_from_direction": details_metno.get("wind_from_direction", -1),
             "temp2m": details_metno.get("air_temperature", -1),
             "dewpoint2m": details_metno.get("dew_point_temperature", -1),
-            "weather": self._weather_data_metno[metno_index].get("data", {}).get("next_1_hours", {}).get("summary", {}).get("symbol_code", ""),
-            "weather6": self._weather_data_metno[metno_index].get("data", {}).get("next_6_hours", {}).get("summary", {}).get("symbol_code", ""),
+            "weather": self._weather_data_metno[metno_index]
+            .get("data", {})
+            .get("next_1_hours", {})
+            .get("summary", {})
+            .get("symbol_code", ""),
+            "weather6": self._weather_data_metno[metno_index]
+            .get("data", {})
+            .get("next_6_hours", {})
+            .get("summary", {})
+            .get("symbol_code", ""),
             "precipitation_amount": (
-                self._weather_data_metno[metno_index].get("data", {}).get("next_1_hours", {}).get("details", {}).get("precipitation_amount", "")
+                self._weather_data_metno[metno_index]
+                .get("data", {})
+                .get("next_1_hours", {})
+                .get("details", {})
+                .get("precipitation_amount", "")
             ),
             # Condition
             "condition_percentage": await self.calc_condition_percentage(
                 details_metno.get("cloud_area_fraction_high", -1),
                 details_metno.get("cloud_area_fraction_medium", -1),
                 details_metno.get("cloud_area_fraction_low", -1),
                 seeing,
@@ -319,25 +331,31 @@
         # Anchor timestamp
         init_ts = await cnv.anchor_timestamp(self._weather_data_seventimer_init)
 
         utc_to_local_diff = self._astro_routines.utc_to_local_diff()
         _LOGGER.debug("UTC to local diff: %s", str(utc_to_local_diff))
         _LOGGER.debug("Forecast length 7timer: %s", str(len(self._weather_data_seventimer)))
 
+        last_forecast_time = forecast_time
         for metno_index, datapoint in enumerate(self._weather_data_metno):
             if forecast_time > datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"):
                 continue
 
+            if (datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ") - last_forecast_time > timedelta(hours=1)):
+                break
+            last_forecast_time = datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ")
             details_metno = datapoint.get("data", {}).get("instant", {}).get("details", {})
 
             if details_metno.get("cloud_area_fraction") is None:
                 _LOGGER.error("Missing Met.no data")
                 break
 
-            details_seventimer = self._get_data_seventimer_timer(seventimer_init, datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"))
+            details_seventimer = self._get_data_seventimer_timer(
+                seventimer_init, datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ")
+            )
 
             transparency = details_seventimer["transparency"]
             item = {
                 "seventimer_init": init_ts,
                 "seventimer_timepoint": details_seventimer["timepoint"],
                 "forecast_time": datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"),
                 "hour": datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ").hour,  # forecast_time.hour % 24,
@@ -378,24 +396,42 @@
                 details_seventimer["transparency"],
                 item["wind_speed"],
             )
 
             item["wind_from_direction"] = details_metno.get("wind_from_direction", -1)
             item["temp2m"] = details_metno.get("air_temperature", -1)
             item["dewpoint2m"] = details_metno.get("dew_point_temperature", -1)
-            if self._weather_data_metno[metno_index + cnt].get("data", {}).get("next_1_hours", {}) == {}:
+            if self._weather_data_metno[metno_index].get("data", {}).get("next_1_hours", {}) == {}:
                 # No more hourly data
+                _LOGGER.debug("No more hourly data at %s", self._weather_data_metno[metno_index].get("time", {}))
                 break
-            if self._weather_data_metno[metno_index + cnt].get("data", {}).get("next_6_hours", {}) == {}:
+            if self._weather_data_metno[metno_index].get("data", {}).get("next_6_hours", {}) == {}:
                 # No more 6-hourly data
-                break
-            item["weather"] = self._weather_data_metno[metno_index + cnt].get("data", {}).get("next_1_hours", {}).get("summary", {}).get("symbol_code", "")
-            item["weather6"] = self._weather_data_metno[metno_index + cnt].get("data", {}).get("next_6_hours", {}).get("summary", {}).get("symbol_code", "")
+                _LOGGER.debug("No more 6-hourly data at %s", self._weather_data_metno[metno_index].get("time", {}))
+                # break
+            item["weather"] = (
+                self._weather_data_metno[metno_index]
+                .get("data", {})
+                .get("next_1_hours", {})
+                .get("summary", {})
+                .get("symbol_code", "")
+            )
+            item["weather6"] = (
+                self._weather_data_metno[metno_index]
+                .get("data", {})
+                .get("next_6_hours", {})
+                .get("summary", {})
+                .get("symbol_code", "")
+            )
             item["precipitation_amount"] = (
-                self._weather_data_metno[metno_index + cnt].get("data", {}).get("next_1_hours", {}).get("details", {}).get("precipitation_amount", "")
+                self._weather_data_metno[metno_index]
+                .get("data", {})
+                .get("next_1_hours", {})
+                .get("details", {})
+                .get("precipitation_amount", "")
             )
 
             items.append(ForecastData(item))
 
             item["seventimer_timepoint"] = item["seventimer_timepoint"] + 1
             item["forecast_time"] = item["forecast_time"] + timedelta(hours=1)
             item["hour"] = item["hour"] + 1
@@ -521,33 +557,35 @@
                     # Test for end of astronomical night. Will get true if we're already at night.
                     if details_forecast.forecast_time.hour % 24 == sun_next_rising.hour:
                         break
             start_index += 24
 
         return items
 
-    async def calc_condition_percentage(self, cloudcover_high, cloudcover_medium, cloudcover_low, seeing, transparency, wind_speed):
+    async def calc_condition_percentage(
+        self, cloudcover_high, cloudcover_medium, cloudcover_low, seeing, transparency, wind_speed
+    ):
         """Return condition based on cloud cover, seeing, transparency, and wind speed"""
 
         # Seeing is something in between 0 and 2.5 arcsecs
-        seeing = int(seeing * 40)                             # arcsecs up to 2.5
-        transparency = int((transparency - 1) * (100 / 7))    # 1-8, 8 is bad
+        seeing = int(seeing * 40)  # arcsecs up to 2.5
+        transparency = int((transparency - 1) * (100 / 7))  # 1-8, 8 is bad
         # Wind speed is something in between 0 and 16.5 m/s
         if wind_speed > 16.5:
             wind_speed = 16.5
-        wind_speed_value = int(wind_speed * (100 / 16.5))     # m/s up to 16.5
+        wind_speed_value = int(wind_speed * (100 / 16.5))  # m/s up to 16.5
 
         cloudcover = []
         cloudcover.append(cloudcover_high * self._cloudcover_high_weakening)
         cloudcover.append(cloudcover_medium * self._cloudcover_medium_weakening)
         cloudcover.append(cloudcover_low * self._cloudcover_low_weakening)
 
         condition = int(
-            100 -
-            (
+            100
+            - (
                 self._cloudcover_weight * max(cloudcover)
                 + self._seeing_weight * seeing
                 + self._transparency_weight * transparency
                 + self._calm_weight * wind_speed_value
             )
             / (self._cloudcover_weight + self._seeing_weight + self._transparency_weight + self._calm_weight)
         )
@@ -644,15 +682,17 @@
                 # Fake 7timer weather data if service is broken
                 # This eliminates consideration of seeing, transparency, and lifted_index
                 # TODO: Think about a complete redesign of the calculations and potentially
                 #       make met.no the leading source instead of 7timer
                 # TODO: Eventually calculate seeing?
                 self._weather_data_seventimer = []
                 for index in range(0, 20):
-                    self._weather_data_seventimer.append({"timepoint": index * 3, "seeing": -1, "transparency": -1, "lifted_index": -1})
+                    self._weather_data_seventimer.append(
+                        {"timepoint": index * 3, "seeing": -1, "transparency": -1, "lifted_index": -1}
+                    )
                 self._weather_data_seventimer_init = datetime.now().strftime("%Y%m%d%H")
         else:
             _LOGGER.debug("Using cached data for 7Timer")
 
     async def async_request_seventimer(self, product="astro", method="get") -> dict:
         """Make a request against the 7timer API."""
 
@@ -791,12 +831,14 @@
 
             if os.path.isfile(self._uptonight_path + "/uptonight-report.json"):
                 _LOGGER.debug(f"Uptonight report found")
                 with open(self._uptonight_path + "/uptonight-report.json") as json_file:
                     dataseries = json.load(json_file)
                     _LOGGER.debug(f"Uptonight imported")
             else:
-                _LOGGER.debug(f"uptonight-report.json not found. Current path: {self._uptonight_path}/uptonight-report.json")
+                _LOGGER.debug(
+                    f"uptonight-report.json not found. Current path: {self._uptonight_path}/uptonight-report.json"
+                )
 
             self._weather_data_uptonight = dataseries
         else:
             _LOGGER.debug("Using cached data for uptonight")
```

### Comparing `pyastroweatherio-0.50.0.dev3/pyastroweatherio/const.py` & `pyastroweatherio-0.50.0.dev4/pyastroweatherio/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,24 +52,15 @@
 #     '1 to 1.25"',
 #     '1.25 to 1.5"',
 #     '1.5 to 2"',
 #     '2 to 2.5"',
 #     'Over 2.5"',
 # ]
 
-SEEING = [
-    0.25,
-    0.625,
-    0.875,
-    1.125,
-    1.375,
-    1.75,
-    2.25,
-    2.5
-]
+SEEING = [0.25, 0.625, 0.875, 1.125, 1.375, 1.75, 2.25, 2.5]
 
 TRANSPARENCY_PLAIN = [
     "Below 0.3 mag",
     "0.3 to 0.4 mag",
     "0.4 to 0.5 mag",
     "0.5 to 0.6 mag",
     "0.6 to 0.7 mag",
```

### Comparing `pyastroweatherio-0.50.0.dev3/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.50.0.dev4/pyastroweatherio/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.0.dev3/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.50.0.dev4/pyastroweatherio/helper_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,20 +215,22 @@
 
     def calculate_water_vapor_pressure6(self, dew_point_temperature, humidity):
         dew_point = dew_point_temperature
         es = self.calculate_saturation_vapor_pressure(dew_point)
         water_vapor_pressure = (humidity / 100) * es
 
         return water_vapor_pressure
-    
+
     # Modell 6:
     # This algorithm first calculates the seeing factor based on temperature, humidity, wind speed
     # and altitude above sea level. It is similar to Model 4 and 5 but uses the air pressure at sea level
     # and dew point provided by Met.no.
-    async def calculate_seeing_model6(self, temperature, humidity, dew_point_temperature, wind_speed, cloud_cover, altitude, air_pressure_at_sea_level):
+    async def calculate_seeing_model6(
+        self, temperature, humidity, dew_point_temperature, wind_speed, cloud_cover, altitude, air_pressure_at_sea_level
+    ):
         water_vapor_pressure = self.calculate_water_vapor_pressure6(dew_point_temperature, humidity)
 
         adjusted_pressure = air_pressure_at_sea_level * math.exp(-0.00012 * altitude)
         relative_pressure = adjusted_pressure / air_pressure_at_sea_level
 
         seeing_factor = CONSTANT_C * (water_vapor_pressure / 10) ** 0.35 * (wind_speed / 10) ** 0.65 * relative_pressure
         seeing = 0.98 / seeing_factor
@@ -251,29 +253,37 @@
 
     def calculate_water_vapor_pressure7(self, dew_point_temperature, humidity):
         dew_point = dew_point_temperature
         es = self.calculate_saturation_vapor_pressure(dew_point)
         water_vapor_pressure = (humidity / 100) * es
 
         return water_vapor_pressure
-    
+
     # Modell 7:
     # This algorithm first calculates the seeing factor based on temperature, humidity, wind speed
     # and altitude above sea level. It is similar to Model 6 but takes the cloud coverage into account.
     # This somehow doesn't seem to be correct, since seeing can be good even with clouds.
-    async def calculate_seeing_model7(self, temperature, humidity, dew_point_temperature, wind_speed, cloud_cover, altitude, air_pressure_at_sea_level):
+    async def calculate_seeing_model7(
+        self, temperature, humidity, dew_point_temperature, wind_speed, cloud_cover, altitude, air_pressure_at_sea_level
+    ):
         water_vapor_pressure = self.calculate_water_vapor_pressure7(dew_point_temperature, humidity)
 
         adjusted_pressure = air_pressure_at_sea_level * math.exp(-0.00012 * altitude)
         relative_pressure = adjusted_pressure / air_pressure_at_sea_level
 
         # Take care on the clouds
         cloud_factor = 1 - (cloud_cover / 100)
 
-        seeing_factor = CONSTANT_C * (water_vapor_pressure / 10) ** 0.2 * (wind_speed / 10) ** 0.6 * relative_pressure ** 0.3 * cloud_factor
+        seeing_factor = (
+            CONSTANT_C
+            * (water_vapor_pressure / 10) ** 0.2
+            * (wind_speed / 10) ** 0.6
+            * relative_pressure**0.3
+            * cloud_factor
+        )
         if seeing_factor == 0:
             seeing = 2.5  # max out seeing
         else:
             seeing = 0.98 / seeing_factor
 
         _LOGGER.debug(
             "AstronomicalSeeing calculation model7: T %s, H %s, DP %s, W %s, C %s, E %s, P %s - S %s",
```

### Comparing `pyastroweatherio-0.50.0.dev3/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.50.0.dev4/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.50.0.dev3
+Version: 0.50.0.dev4
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.50.0.dev3/setup.py` & `pyastroweatherio-0.50.0.dev4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.50.0.dev3",
+    version="0.50.0.dev4",
     license="MIT",
     description="Python Wrapper for 7Timer and Met.no REST API",
     long_description=" ".join(
         [
             "Lightweight Python 3 module to receive data via",
             "REST API from 7Timer and Met.no.",
         ],
```

