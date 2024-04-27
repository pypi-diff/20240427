# Comparing `tmp/pyastroweatherio-0.43.1.dev9.tar.gz` & `tmp/pyastroweatherio-0.50.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.43.1.dev9.tar", last modified: Tue Apr 23 10:48:06 2024, max compression
+gzip compressed data, was "pyastroweatherio-0.50.0.dev1.tar", last modified: Sat Apr 27 09:37:36 2024, max compression
```

## Comparing `pyastroweatherio-0.43.1.dev9.tar` & `pyastroweatherio-0.50.0.dev1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-23 10:48:06.903584 pyastroweatherio-0.43.1.dev9/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev9/LICENSE
--rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-23 10:48:06.903584 pyastroweatherio-0.43.1.dev9/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.43.1.dev9/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-23 10:48:06.899584 pyastroweatherio-0.43.1.dev9/pyastroweatherio/
--rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    33774 2024-04-23 10:16:21.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio/client.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     3639 2024-04-22 11:00:22.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio/const.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    20074 2024-04-22 11:00:22.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio/dataclasses.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio/errors.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    37621 2024-04-23 10:29:18.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio/helper_functions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-23 10:48:06.903584 pyastroweatherio-0.43.1.dev9/pyastroweatherio.egg-info/
--rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-23 10:48:06.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-04-23 10:48:06.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-23 10:48:06.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-04-23 10:48:06.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-04-23 10:48:06.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio.egg-info/top_level.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-04-23 10:48:06.907584 pyastroweatherio-0.43.1.dev9/setup.cfg
--rw-rw-r--   0 markus    (1000) markus    (1000)     1340 2024-04-23 10:47:56.000000 pyastroweatherio-0.43.1.dev9/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-27 09:37:36.557600 pyastroweatherio-0.50.0.dev1/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.50.0.dev1/LICENSE
+-rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-04-27 09:37:36.557600 pyastroweatherio-0.50.0.dev1/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.50.0.dev1/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-27 09:37:36.553600 pyastroweatherio-0.50.0.dev1/pyastroweatherio/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.50.0.dev1/pyastroweatherio/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    35558 2024-04-27 09:35:16.000000 pyastroweatherio-0.50.0.dev1/pyastroweatherio/client.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     4002 2024-04-27 09:34:38.000000 pyastroweatherio-0.50.0.dev1/pyastroweatherio/const.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    20099 2024-04-27 09:24:39.000000 pyastroweatherio-0.50.0.dev1/pyastroweatherio/dataclasses.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.50.0.dev1/pyastroweatherio/errors.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    41918 2024-04-26 06:34:43.000000 pyastroweatherio-0.50.0.dev1/pyastroweatherio/helper_functions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-27 09:37:36.557600 pyastroweatherio-0.50.0.dev1/pyastroweatherio.egg-info/
+-rw-r--r--   0 markus    (1000) markus    (1000)     1093 2024-04-27 09:37:36.000000 pyastroweatherio-0.50.0.dev1/pyastroweatherio.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-04-27 09:37:36.000000 pyastroweatherio-0.50.0.dev1/pyastroweatherio.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-27 09:37:36.000000 pyastroweatherio-0.50.0.dev1/pyastroweatherio.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-04-27 09:37:36.000000 pyastroweatherio-0.50.0.dev1/pyastroweatherio.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-04-27 09:37:36.000000 pyastroweatherio-0.50.0.dev1/pyastroweatherio.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-04-27 09:37:36.557600 pyastroweatherio-0.50.0.dev1/setup.cfg
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1390 2024-04-27 09:37:18.000000 pyastroweatherio-0.50.0.dev1/setup.py
```

### Comparing `pyastroweatherio-0.43.1.dev9/LICENSE` & `pyastroweatherio-0.50.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev9/PKG-INFO` & `pyastroweatherio-0.50.0.dev1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.43.1.dev9
+Version: 0.50.0.dev1
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
@@ -15,12 +15,13 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: pyephem
 
 Lightweight Python 3 module to receive data via REST API from 7Timer and Met.no.
```

### Comparing `pyastroweatherio-0.43.1.dev9/README.md` & `pyastroweatherio-0.50.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev9/pyastroweatherio/client.py` & `pyastroweatherio-0.50.0.dev1/pyastroweatherio/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 """Define a client to interact with 7Timer."""
 
 import asyncio
 import json
+from json.decoder import JSONDecodeError
 import logging
 import os.path
 import math
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from typing import Optional
 from decimal import Decimal
 from aiohttp import ClientSession, ClientTimeout
 from aiohttp.client_exceptions import ClientError
 
 import pprint
+
 pp = pprint.PrettyPrinter()
-     
+
 from pyastroweatherio.const import (
     BASE_URL_SEVENTIMER,
     BASE_URL_MET,
     HEADERS,
     DEFAULT_TIMEOUT,
     DEFAULT_CACHE_TIMEOUT,
     DEFAULT_ELEVATION,
     DEFAULT_TIMEZONE,
     DEFAULT_CONDITION_CLOUDCOVER_WEIGHT,
+    DEFAULT_CONDITION_CLOUDCOVER_HIGH_WEAKENING,
+    DEFAULT_CONDITION_CLOUDCOVER_MEDIUM_WEAKENING,
+    DEFAULT_CONDITION_CLOUDCOVER_LOW_WEAKENING,
     DEFAULT_CONDITION_SEEING_WEIGHT,
     DEFAULT_CONDITION_TRANSPARENCY_WEIGHT,
     DEFAULT_CONDITION_CALM_WEIGHT,
     WIND10M_VALUE,
     WIND10M_RANGE,
     HOME_LATITUDE,
     HOME_LONGITUDE,
     STIMER_OUTPUT,
-    # FORECAST_TYPE_DAILY,
     FORECAST_TYPE_HOURLY,
-    MAGNUS_COEFFICIENT_A,
-    MAGNUS_COEFFICIENT_B,
+    SEEING,
 )
 from pyastroweatherio.dataclasses import (
     ForecastData,
     LocationData,
     NightlyConditionsData,
     DSOUpTonight,
 )
@@ -55,14 +58,17 @@
         self,
         session: Optional[ClientSession] = None,
         latitude=HOME_LATITUDE,
         longitude=HOME_LONGITUDE,
         elevation=DEFAULT_ELEVATION,
         timezone_info=DEFAULT_TIMEZONE,
         cloudcover_weight=DEFAULT_CONDITION_CLOUDCOVER_WEIGHT,
+        cloudcover_high_weakening=DEFAULT_CONDITION_CLOUDCOVER_HIGH_WEAKENING,
+        cloudcover_medium_weakening=DEFAULT_CONDITION_CLOUDCOVER_MEDIUM_WEAKENING,
+        cloudcover_low_weakening=DEFAULT_CONDITION_CLOUDCOVER_LOW_WEAKENING,
         seeing_weight=DEFAULT_CONDITION_SEEING_WEIGHT,
         transparency_weight=DEFAULT_CONDITION_TRANSPARENCY_WEIGHT,
         calm_weight=DEFAULT_CONDITION_CALM_WEIGHT,
         uptonight_path="/conf/www",
         test_datetime=None,
     ):
         self._session: ClientSession = session
@@ -75,14 +81,17 @@
         self._weather_data_metno = []
         self._weather_data_metno_init = ""
         self._weather_data_uptonight = {}
         self._weather_data_seventimer_timestamp = datetime.now() - timedelta(seconds=(DEFAULT_CACHE_TIMEOUT + 1))
         self._weather_data_metno_timestamp = datetime.now() - timedelta(seconds=(DEFAULT_CACHE_TIMEOUT + 1))
         self._data_uptonight_timestamp = datetime.now() - timedelta(seconds=(DEFAULT_CACHE_TIMEOUT + 1))
         self._cloudcover_weight = cloudcover_weight
+        self._cloudcover_high_weakening = cloudcover_high_weakening
+        self._cloudcover_medium_weakening = cloudcover_medium_weakening
+        self._cloudcover_low_weakening = cloudcover_low_weakening
         self._seeing_weight = seeing_weight
         self._transparency_weight = transparency_weight
         self._calm_weight = calm_weight
         self._uptonight_path = uptonight_path
         self._test_datetime = test_datetime
 
         self._forecast_data = None
@@ -95,36 +104,27 @@
             self._longitude,
             self._elevation,
             self._timezone_info,
             self._test_datetime,
         )
 
         self._astro_seeing = AstronomicalSeeing()
-        
+
         # Testing
         self._test_mode = False
         if self._test_datetime is not None:
             self._test_mode = True
 
     # Public functions
     async def get_location_data(
         self,
     ) -> None:
         """Returns station Weather Forecast."""
         return await self._get_location_data()
 
-    # async def get_forecast(self, forecast_type=FORECAST_TYPE_DAILY, hours_to_show=24) -> None:
-    #     """Returns station Weather Forecast."""
-    #     _LOGGER.debug("get_forecast called")
-    #     return await self._get_forecast_data(forecast_type, hours_to_show)
-
-    # async def get_daily_forecast(self) -> None:
-    #     """Returns daily Weather Forecast."""
-    #     return await self._get_forecast_data(FORECAST_TYPE_DAILY, 72)
-
     async def get_hourly_forecast(self) -> None:
         """Returns hourly Weather Forecast."""
         return await self._get_forecast_data(FORECAST_TYPE_HOURLY, 72)
 
     async def get_deepsky_forecast(self) -> None:
         """Returns Deep Sky Forecast."""
         return await self._get_deepsky_forecast()
@@ -132,274 +132,279 @@
     # Private functions
     async def _get_location_data(self) -> None:
         """Return Forecast data"""
 
         cnv = ConversionFunctions()
         items = []
 
-        await self.retrieve_data_seventimer()
         await self.retrieve_data_metno()
-        now = datetime.utcnow()
-
-        # Anchor timestamp
-        init_ts = await cnv.anchor_timestamp(self._weather_data_seventimer_init)
+        await self.retrieve_data_seventimer()
+        now = datetime.now(timezone.utc).replace(tzinfo=None)
 
         if self._test_datetime is not None:
             await self._astro_routines.need_update()
         else:
             await self._astro_routines.need_update(forecast_time=now)
 
-        # Met.no
-        metno_index = -1
-        # 7Timer
-        forecast_skipped = 0
-
-        for row in self._weather_data_seventimer:
-            # 7Timer: Skip over past forecasts
-            forecast_time = init_ts + timedelta(hours=row["timepoint"])
-            if now > forecast_time:
-                forecast_skipped += 1
-                continue
-
-            _LOGGER.debug("Forecast time: %s", str(forecast_time))
+        forecast_time = now.replace(minute=0, second=0, microsecond=0)
+        _LOGGER.debug("Forecast time: %s", str(forecast_time))
 
-            # Met.no: Search for 7Timer forecast time
-            for datapoint in self._weather_data_metno:
-                metno_index += 1
-                if forecast_time == datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"):
-                    break
-            _LOGGER.debug("Met.no start index: %s", str(metno_index))
+        # Met.no
+        metno_index = 0
+        seventimer_index = 0
 
-            details = None
-            # Verify that Met.no start index is correct and get details
-            if (
-                datetime.strptime(
-                    self._weather_data_metno[metno_index].get("time"),
-                    "%Y-%m-%dT%H:%M:%SZ",
-                )
-                == forecast_time
-            ):
-                details = self._weather_data_metno[metno_index].get("data", {}).get("instant", {}).get("details", {})
-            else:
+        # Met.no: Search for start index
+        for datapoint in self._weather_data_metno:
+            if forecast_time == datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"):
+                break
+            metno_index += 1
+        _LOGGER.debug("Met.no start index: %s", str(metno_index))
+        details_metno = self._weather_data_metno[metno_index].get("data", {}).get("instant", {}).get("details", {})
+
+        # 7Timer: Search for start index
+        seventimer_init = await cnv.anchor_timestamp(self._weather_data_seventimer_init)
+        for row7 in self._weather_data_seventimer:
+            if seventimer_init + timedelta(hours=row7["timepoint"]) > now:
                 break
+            seventimer_index += 1
+        if seventimer_index < len(self._weather_data_seventimer):
+            _LOGGER.debug("7Timer start index: %s", str(seventimer_index))
+            details_seventimer = self._weather_data_seventimer[seventimer_index]
+        else:
+            details_seventimer = {"timepoint": 0, "seeing": -1, "transparency": -1, "lifted_index": -1}
 
-            item = {
-                # seventimer_init is "init" of 7timer astro data
-                "seventimer_init": init_ts,  # init
-                # seventimer_timepoint is "timepoint" of 7timer astro data and defines the data for init + timepoint
-                "seventimer_timepoint": row["timepoint"],  # timepoint
-                # Forecast_time is the actual datetime for the forecast data onwards in UTC
-                # Corresponds to "time" in met data
-                "forecast_time": forecast_time,  # timestamp
-                # Time shift to UTC
-                "time_shift": await self._astro_routines.time_shift(),
-                # Remaining forecast data point in 7timer data
-                "forecast_length": (len(self._weather_data_seventimer) - forecast_skipped) * 3,
-                # Location
-                "latitude": self._latitude,
-                "longitude": self._longitude,
-                "elevation": self._elevation,
-                # 7timer
-                "seeing": await self._astro_seeing.calculate_seeing_model4(details.get("air_temperature", -1), details.get("wind_speed", -1), details.get("relative_humidity", -1), self._elevation), #row["seeing"],
-                "transparency": row["transparency"],
-                "lifted_index": row["lifted_index"],
-                # Calculate
-                "sun_next_rising": await self._astro_routines.sun_next_rising_civil(),
-                "sun_next_rising_nautical": await self._astro_routines.sun_next_rising_nautical(),
-                "sun_next_rising_astro": await self._astro_routines.sun_next_rising_astro(),
-                "sun_next_setting": await self._astro_routines.sun_next_setting_civil(),
-                "sun_next_setting_nautical": await self._astro_routines.sun_next_setting_nautical(),
-                "sun_next_setting_astro": await self._astro_routines.sun_next_setting_astro(),
-                "sun_altitude": await self._astro_routines.sun_altitude(),
-                "sun_azimuth": await self._astro_routines.sun_azimuth(),
-                "moon_next_rising": await self._astro_routines.moon_next_rising(),
-                "moon_next_setting": await self._astro_routines.moon_next_setting(),
-                "moon_phase": await self._astro_routines.moon_phase(),
-                "moon_next_new_moon": await self._astro_routines.moon_next_new_moon(),
-                "moon_next_full_moon": await self._astro_routines.moon_next_full_moon(),
-                "moon_altitude": await self._astro_routines.moon_altitude(),
-                "moon_azimuth": await self._astro_routines.moon_azimuth(),
-                "night_duration_astronomical": await self._astro_routines.night_duration_astronomical(),
-                "deep_sky_darkness_moon_rises": await self._astro_routines.deep_sky_darkness_moon_rises(),
-                "deep_sky_darkness_moon_sets": await self._astro_routines.deep_sky_darkness_moon_sets(),
-                "deep_sky_darkness_moon_always_up": await self._astro_routines.deep_sky_darkness_moon_always_up(),
-                "deep_sky_darkness_moon_always_down": await self._astro_routines.deep_sky_darkness_moon_always_down(),
-                "deep_sky_darkness": await self._astro_routines.deep_sky_darkness(),
-                "deepsky_forecast": await self._get_deepsky_forecast(),
-                # Met.no
-                "cloudcover": int(details.get("cloud_area_fraction", -1) / 12.5 + 1),
-                "cloud_area_fraction": details.get("cloud_area_fraction", -1),
-                "cloud_area_fraction_high": details.get("cloud_area_fraction_high", -1),
-                "cloud_area_fraction_low": details.get("cloud_area_fraction_low", -1),
-                "cloud_area_fraction_medium": details.get("cloud_area_fraction_medium", -1),
-                "fog_area_fraction": details.get("fog_area_fraction", -1),
-                "rh2m": details.get("relative_humidity", -1),
-                "wind_speed": details.get("wind_speed", -1),
-                "wind_from_direction": details.get("wind_from_direction", -1),
-                "temp2m": details.get("air_temperature", -1),
-                "dewpoint2m": details.get("dew_point_temperature", -1),
-                "weather": self._weather_data_metno[metno_index]
-                .get("data", {})
-                .get("next_1_hours", {})
-                .get("summary", {})
-                .get("symbol_code", ""),
-                "weather6": self._weather_data_metno[metno_index]
-                .get("data", {})
-                .get("next_6_hours", {})
-                .get("summary", {})
-                .get("symbol_code", ""),
-                "precipitation_amount": (
-                    self._weather_data_metno[metno_index]
-                    .get("data", {})
-                    .get("next_1_hours", {})
-                    .get("details", {})
-                    .get("precipitation_amount", "")
-                ),
-                # Condition
-                "condition_percentage": await self.calc_condition_percentage(
-                    details.get("cloud_area_fraction", -1) / 12.5 + 1,
-                    await self._astro_seeing.calculate_seeing_model4(details.get("air_temperature", -1), details.get("wind_speed", -1), details.get("relative_humidity", -1), self._elevation), #row["seeing"],
-                    row["transparency"],
-                    details.get("wind_speed", -1),
-                ),
-                # Uptonight objects
-                "uptonight": await self._get_deepsky_objects(),
-            }
+        seeing = 0
+        if details_seventimer["seeing"] == -1:
+            seeing = await self._astro_seeing.calculate_seeing_model6(
+                temperature=details_metno.get("air_temperature", -1),
+                humidity=details_metno.get("relative_humidity", -1),
+                dew_point_temperature=details_metno.get("dew_point_temperature", -1),
+                wind_speed=details_metno.get("wind_speed", -1),
+                cloud_cover=details_metno.get("cloud_area_fraction", -1),
+                altitude=self._elevation,
+                air_pressure_at_sea_level=details_metno.get("air_pressure_at_sea_level", -1),
+            )
+        else:
+            seeing = SEEING[details_seventimer["seeing"] - 1]
+
+        item = {
+            # seventimer_init is "init" of 7timer astro data
+            "seventimer_init": seventimer_init,  # init
+            # seventimer_timepoint is "timepoint" of 7timer astro data and defines the data for init + timepoint
+            "seventimer_timepoint": details_seventimer["timepoint"],  # timepoint
+            # Forecast_time is the actual datetime for the forecast data onwards in UTC
+            # Corresponds to "time" in met data
+            "forecast_time": forecast_time,  # timestamp
+            # Time shift to UTC
+            "time_shift": await self._astro_routines.time_shift(),
+            # Remaining forecast data point in met.no data
+            "forecast_length": (len(self._weather_data_metno) - metno_index),
+            # Location
+            "latitude": self._latitude,
+            "longitude": self._longitude,
+            "elevation": self._elevation,
+            "seeing": seeing,
+            "transparency": details_seventimer["transparency"],
+            "lifted_index": details_seventimer["lifted_index"],
+            # Calculate
+            "sun_next_rising": await self._astro_routines.sun_next_rising_civil(),
+            "sun_next_rising_nautical": await self._astro_routines.sun_next_rising_nautical(),
+            "sun_next_rising_astro": await self._astro_routines.sun_next_rising_astro(),
+            "sun_next_setting": await self._astro_routines.sun_next_setting_civil(),
+            "sun_next_setting_nautical": await self._astro_routines.sun_next_setting_nautical(),
+            "sun_next_setting_astro": await self._astro_routines.sun_next_setting_astro(),
+            "sun_altitude": await self._astro_routines.sun_altitude(),
+            "sun_azimuth": await self._astro_routines.sun_azimuth(),
+            "moon_next_rising": await self._astro_routines.moon_next_rising(),
+            "moon_next_setting": await self._astro_routines.moon_next_setting(),
+            "moon_phase": await self._astro_routines.moon_phase(),
+            "moon_next_new_moon": await self._astro_routines.moon_next_new_moon(),
+            "moon_next_full_moon": await self._astro_routines.moon_next_full_moon(),
+            "moon_altitude": await self._astro_routines.moon_altitude(),
+            "moon_azimuth": await self._astro_routines.moon_azimuth(),
+            "night_duration_astronomical": await self._astro_routines.night_duration_astronomical(),
+            "deep_sky_darkness_moon_rises": await self._astro_routines.deep_sky_darkness_moon_rises(),
+            "deep_sky_darkness_moon_sets": await self._astro_routines.deep_sky_darkness_moon_sets(),
+            "deep_sky_darkness_moon_always_up": await self._astro_routines.deep_sky_darkness_moon_always_up(),
+            "deep_sky_darkness_moon_always_down": await self._astro_routines.deep_sky_darkness_moon_always_down(),
+            "deep_sky_darkness": await self._astro_routines.deep_sky_darkness(),
+            "deepsky_forecast": await self._get_deepsky_forecast(),
+            # Met.no
+            "cloudcover": details_metno.get("cloud_area_fraction", -1),
+            "cloud_area_fraction": details_metno.get("cloud_area_fraction", -1),
+            "cloud_area_fraction_high": details_metno.get("cloud_area_fraction_high", -1),
+            "cloud_area_fraction_low": details_metno.get("cloud_area_fraction_low", -1),
+            "cloud_area_fraction_medium": details_metno.get("cloud_area_fraction_medium", -1),
+            "fog_area_fraction": details_metno.get("fog_area_fraction", -1),
+            "rh2m": details_metno.get("relative_humidity", -1),
+            "wind_speed": details_metno.get("wind_speed", -1),
+            "wind_from_direction": details_metno.get("wind_from_direction", -1),
+            "temp2m": details_metno.get("air_temperature", -1),
+            "dewpoint2m": details_metno.get("dew_point_temperature", -1),
+            "weather": self._weather_data_metno[metno_index].get("data", {}).get("next_1_hours", {}).get("summary", {}).get("symbol_code", ""),
+            "weather6": self._weather_data_metno[metno_index].get("data", {}).get("next_6_hours", {}).get("summary", {}).get("symbol_code", ""),
+            "precipitation_amount": (
+                self._weather_data_metno[metno_index].get("data", {}).get("next_1_hours", {}).get("details", {}).get("precipitation_amount", "")
+            ),
+            # Condition
+            "condition_percentage": await self.calc_condition_percentage(
+                details_metno.get("cloud_area_fraction_high", -1),
+                details_metno.get("cloud_area_fraction_medium", -1),
+                details_metno.get("cloud_area_fraction_low", -1),
+                seeing,
+                details_seventimer["transparency"],
+                details_metno.get("wind_speed", -1),
+            ),
+            # Uptonight objects
+            "uptonight": await self._get_deepsky_objects(),
+        }
 
-            items.append(LocationData(item))
-            break
+        items.append(LocationData(item))
 
         return items
 
+    def _get_data_seventimer_timer(self, anchor_timestamp, datetime):
+        """Return 7Timer datapoint of interest"""
+
+        seventimer_index = 0
+        for index, row7 in enumerate(self._weather_data_seventimer):
+            if anchor_timestamp + timedelta(hours=row7["timepoint"]) > datetime:
+                seventimer_index = index - 1
+                break
+            # index += 1
+        if seventimer_index >= len(self._weather_data_seventimer):
+            return {"timepoint": row7["timepoint"], "seeing": -1, "transparency": -1, "lifted_index": -1}
+        else:
+            return self._weather_data_seventimer[seventimer_index]
+
     async def _get_forecast_data(self, forecast_type, hours_to_show) -> None:
         """Return Forecast data for the Station."""
 
         cnv = ConversionFunctions()
         items = []
 
-        await self.retrieve_data_seventimer()
         await self.retrieve_data_metno()
-        now = datetime.utcnow()
-        # now = datetime.utcnow() + timedelta(hours=12)
+        await self.retrieve_data_seventimer()
+        now = datetime.now(timezone.utc).replace(tzinfo=None)
 
         # Create items
         cnt = 0
 
+        forecast_time = now.replace(minute=0, second=0, microsecond=0)
+        _LOGGER.debug("Forecast time: %s", str(forecast_time))
+
+        # Met.no
+        # metno_index = 0
+        # seventimer_index = 0
+
+        # Met.no: Search for start index
+        # for datapoint in self._weather_data_metno:
+        #     if forecast_time == datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"):
+        #         break
+        #     metno_index += 1
+        # _LOGGER.debug("Met.no start index: %s", str(metno_index))
+        # details_metno = self._weather_data_metno[metno_index].get("data", {}).get("instant", {}).get("details", {})
+
+        # 7Timer: Search for start index
+        seventimer_init = await cnv.anchor_timestamp(self._weather_data_seventimer_init)
+        # for row7 in self._weather_data_seventimer:
+        #     if seventimer_init + timedelta(hours=row7["timepoint"]) > now:
+        #         break
+        #     seventimer_index += 1
+        # if seventimer_index < len(self._weather_data_seventimer):
+        #     _LOGGER.debug("7Timer start index: %s", str(seventimer_index))
+        #     details_seventimer = self._weather_data_seventimer[seventimer_index]
+        # else:
+        #     details_seventimer = {"timepoint": 0, "seeing": -1, "transparency": -1, "lifted_index": -1}
+
         # Anchor timestamp
         init_ts = await cnv.anchor_timestamp(self._weather_data_seventimer_init)
 
         utc_to_local_diff = self._astro_routines.utc_to_local_diff()
         _LOGGER.debug("UTC to local diff: %s", str(utc_to_local_diff))
         _LOGGER.debug("Forecast length 7timer: %s", str(len(self._weather_data_seventimer)))
 
-        # Met.no
-        metno_index = -1
-        for row in self._weather_data_seventimer:
-            # 7Timer: Skip over past forecasts
-            forecast_time = init_ts + timedelta(hours=row["timepoint"])
-            if now > forecast_time:
+        for metno_index, datapoint in enumerate(self._weather_data_metno):
+            if forecast_time > datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"):
                 continue
 
-            # Met.no: Search for 7Timer forecast time
-            if metno_index == -1:
-                for datapoint in self._weather_data_metno:
-                    metno_index += 1
-                    if forecast_time == datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"):
-                        break
-                _LOGGER.debug("Met.no start index: %s", str(metno_index))
+            details_metno = datapoint.get("data", {}).get("instant", {}).get("details", {})
+
+            if details_metno.get("cloud_area_fraction") is None:
+                _LOGGER.error("Missing Met.no data")
+                break
 
-            seeing = 0  #row["seeing"]
-            transparency = row["transparency"]
+            details_seventimer = self._get_data_seventimer_timer(seventimer_init, datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"))
+
+            transparency = details_seventimer["transparency"]
             item = {
                 "seventimer_init": init_ts,
-                "seventimer_timepoint": row["timepoint"],
-                "forecast_time": forecast_time,
-                "hour": forecast_time.hour % 24,
-                "seeing": seeing,
+                "seventimer_timepoint": details_seventimer["timepoint"],
+                "forecast_time": datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"),
+                "hour": datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ").hour,  # forecast_time.hour % 24,
+                "seeing": details_seventimer["seeing"],
                 "transparency": transparency,
-                "lifted_index": row["lifted_index"],
+                "lifted_index": details_seventimer["lifted_index"],
             }
-            # Met.no
-            if (
-                datetime.strptime(
-                    self._weather_data_metno[metno_index + cnt].get("time"),
-                    "%Y-%m-%dT%H:%M:%SZ",
-                )
-                == forecast_time
-            ):
-                # Continue hourly
-                for i in range(0, 3):
-                    details = (
-                        self._weather_data_metno[metno_index + cnt + i]
-                        .get("data", {})
-                        .get("instant", {})
-                        .get("details", {})
-                    )
-                    if details.get("cloud_area_fraction") is None:
-                        _LOGGER.error("Missing Met.no data")
-                        break
-                    item["cloudcover"] = int(details.get("cloud_area_fraction", -1) / 12.5 + 1)
 
-                    item["cloud_area_fraction"] = details.get("cloud_area_fraction", -1)
-                    item["cloud_area_fraction_high"] = details.get("cloud_area_fraction_high", -1)
-                    item["cloud_area_fraction_low"] = details.get("cloud_area_fraction_low", -1)
-                    item["cloud_area_fraction_medium"] = details.get("cloud_area_fraction_medium", -1)
-                    item["fog_area_fraction"] = details.get("fog_area_fraction", -1)
-                    item["rh2m"] = details.get("relative_humidity", -1)
-                    item["wind_speed"] = details.get("wind_speed", -1)
-                    item["seeing"] = await self._astro_seeing.calculate_seeing_model4(details.get("air_temperature", -1), details.get("wind_speed", -1), details.get("relative_humidity", -1), self._elevation)
-
-                    item["condition_percentage"] = await self.calc_condition_percentage(
-                        item["cloud_area_fraction"] / 12.5 + 1,
-                        await self._astro_seeing.calculate_seeing_model4(details.get("air_temperature", -1), details.get("wind_speed", -1), details.get("relative_humidity", -1), self._elevation), #row["seeing"],
-                        row["transparency"],
-                        item["wind_speed"],
-                    )
+            seeing = 0
+            if details_seventimer["seeing"] == -1 or details_seventimer["seeing"] == -9999:
+                seeing = await self._astro_seeing.calculate_seeing_model6(
+                    temperature=details_metno.get("air_temperature", -1),
+                    humidity=details_metno.get("relative_humidity", -1),
+                    dew_point_temperature=details_metno.get("dew_point_temperature", -1),
+                    wind_speed=details_metno.get("wind_speed", -1),
+                    cloud_cover=details_metno.get("cloud_area_fraction", -1),
+                    altitude=self._elevation,
+                    air_pressure_at_sea_level=details_metno.get("air_pressure_at_sea_level", -1),
+                )
+            else:
+                seeing = SEEING[details_seventimer["seeing"] - 1]
 
-                    item["wind_from_direction"] = details.get("wind_from_direction", -1)
-                    item["temp2m"] = details.get("air_temperature", -1)
-                    item["dewpoint2m"] = details.get("dew_point_temperature", -1)
-                    if self._weather_data_metno[metno_index + cnt + i].get("data", {}).get("next_1_hours", {}) == {}:
-                        # No more hourly data
-                        break
-                    if self._weather_data_metno[metno_index + cnt + i].get("data", {}).get("next_6_hours", {}) == {}:
-                        # No more 6-hourly data
-                        break
-                    item["weather"] = (
-                        self._weather_data_metno[metno_index + cnt + i]
-                        .get("data", {})
-                        .get("next_1_hours", {})
-                        .get("summary", {})
-                        .get("symbol_code", "")
-                    )
-                    item["weather6"] = (
-                        self._weather_data_metno[metno_index + cnt + i]
-                        .get("data", {})
-                        .get("next_6_hours", {})
-                        .get("summary", {})
-                        .get("symbol_code", "")
-                    )
-                    item["precipitation_amount"] = (
-                        self._weather_data_metno[metno_index + cnt + i]
-                        .get("data", {})
-                        .get("next_1_hours", {})
-                        .get("details", {})
-                        .get("precipitation_amount", "")
-                    )
+            item["cloudcover"] = details_metno.get("cloud_area_fraction", -1)
 
-                    items.append(ForecastData(item))
+            item["cloud_area_fraction"] = details_metno.get("cloud_area_fraction", -1)
+            item["cloud_area_fraction_high"] = details_metno.get("cloud_area_fraction_high", -1)
+            item["cloud_area_fraction_medium"] = details_metno.get("cloud_area_fraction_medium", -1)
+            item["cloud_area_fraction_low"] = details_metno.get("cloud_area_fraction_low", -1)
+            item["fog_area_fraction"] = details_metno.get("fog_area_fraction", -1)
+            item["rh2m"] = details_metno.get("relative_humidity", -1)
+            item["wind_speed"] = details_metno.get("wind_speed", -1)
+            item["seeing"] = seeing
+            item["condition_percentage"] = await self.calc_condition_percentage(
+                item["cloud_area_fraction_high"],
+                item["cloud_area_fraction_medium"],
+                item["cloud_area_fraction_low"],
+                seeing,
+                details_seventimer["transparency"],
+                item["wind_speed"],
+            )
 
-                    item["seventimer_timepoint"] = item["seventimer_timepoint"] + 1
-                    item["forecast_time"] = item["forecast_time"] + timedelta(hours=1)
-                    item["hour"] = item["hour"] + 1
-            else:
+            item["wind_from_direction"] = details_metno.get("wind_from_direction", -1)
+            item["temp2m"] = details_metno.get("air_temperature", -1)
+            item["dewpoint2m"] = details_metno.get("dew_point_temperature", -1)
+            if self._weather_data_metno[metno_index + cnt].get("data", {}).get("next_1_hours", {}) == {}:
+                # No more hourly data
+                break
+            if self._weather_data_metno[metno_index + cnt].get("data", {}).get("next_6_hours", {}) == {}:
+                # No more 6-hourly data
                 break
+            item["weather"] = self._weather_data_metno[metno_index + cnt].get("data", {}).get("next_1_hours", {}).get("summary", {}).get("symbol_code", "")
+            item["weather6"] = self._weather_data_metno[metno_index + cnt].get("data", {}).get("next_6_hours", {}).get("summary", {}).get("symbol_code", "")
+            item["precipitation_amount"] = (
+                self._weather_data_metno[metno_index + cnt].get("data", {}).get("next_1_hours", {}).get("details", {}).get("precipitation_amount", "")
+            )
+
+            items.append(ForecastData(item))
+
+            item["seventimer_timepoint"] = item["seventimer_timepoint"] + 1
+            item["forecast_time"] = item["forecast_time"] + timedelta(hours=1)
+            item["hour"] = item["hour"] + 1
 
-            # Limit number of Hours
-            cnt += 3
+            cnt += 1
             if cnt >= hours_to_show:
                 break
 
         self._forecast_data = items
 
         _LOGGER.debug("Forceast Length: %s", str(len(items)))
         return items
@@ -408,15 +413,14 @@
         """Return Deepsky Forecast data"""
 
         cnv = ConversionFunctions()
         items = []
 
         if self._forecast_data == None:
             await self._get_forecast_data(FORECAST_TYPE_HOURLY, 72)
-        now = datetime.utcnow()
 
         # Anchor timestamp
         init_ts = await cnv.anchor_timestamp(self._weather_data_seventimer_init)
 
         utc_to_local_diff = self._astro_routines.utc_to_local_diff()
         _LOGGER.debug("UTC to local diff: %s", str(utc_to_local_diff))
 
@@ -429,63 +433,74 @@
         sun_next_setting = await self._astro_routines.sun_next_setting()
         sun_next_rising = await self._astro_routines.sun_next_rising()
         night_duration_astronomical = await self._astro_routines.night_duration_astronomical()
 
         start_indexes = []
         # Find start index for two nights and store the indexes
         _LOGGER.debug("Forecast data length: %s", str(len(self._forecast_data)))
-        for idx, row in enumerate(self._forecast_data):
-            if row.forecast_time.hour % 24 == sun_next_rising.hour and len(start_indexes) == 0:
+        for index, details_forecast in enumerate(self._forecast_data):
+            if details_forecast.forecast_time.hour % 24 == sun_next_rising.hour and len(start_indexes) == 0:
                 start_indexes.append(0)
-            if row.forecast_time.hour % 24 == sun_next_setting.hour:
-                start_indexes.append(idx)
+            if details_forecast.forecast_time.hour % 24 == sun_next_setting.hour:
+                start_indexes.append(index)
 
         forecast_data_len = len(self._forecast_data)
         for day in range(0, len(start_indexes)):
             start_forecast_hour = 0
             start_weather = ""
             interval_points = []
             start_index = start_indexes[day]
-            for idx in range(
+            for index in range(
                 start_index,
                 start_index + int(math.floor(night_duration_astronomical / 3600) + 2),
             ):
-                if idx >= forecast_data_len:
+                if index >= forecast_data_len:
                     _LOGGER.debug("No more forecast data")
                     break
-                row = self._forecast_data[idx]
-
-                seeing = row.seeing
-                transparency = row.transparency
-                cloud_area_fraction = row.cloud_area_fraction_percentage / 12.5 + 1
-                wind_speed = row.wind10m_speed
+                details_forecast = self._forecast_data[index]
 
                 if len(interval_points) == 0:
-                    forecast_dayname = row.forecast_time.strftime("%A")
-                    start_forecast_hour = row.forecast_time.hour
-                    start_weather = row.weather6
+                    forecast_dayname = details_forecast.forecast_time.strftime("%A")
+                    start_forecast_hour = details_forecast.forecast_time.hour
+                    start_weather = details_forecast.weather6
 
                 _LOGGER.debug(
-                    "Idex: %d, Hour of day: %d, cloud_area_fraction: %s, seeing: %s, transparency: %s, wind_speed: %s, condition: %s",
-                    idx,
-                    row.forecast_time.hour,
-                    str(cloud_area_fraction),
-                    str(seeing),
-                    str(transparency),
-                    str(wind_speed),
-                    await self.calc_condition_percentage(cloud_area_fraction, seeing, transparency, wind_speed),
+                    "Idex: %d, Hour of day: %d, cloud_area_fraction: %s %s %s, seeing: %s, transparency: %s, wind_speed: %s, condition: %s",
+                    index,
+                    details_forecast.forecast_time.hour,
+                    str(details_forecast.cloud_area_fraction_high_percentage),
+                    str(details_forecast.cloud_area_fraction_medium_percentage),
+                    str(details_forecast.cloud_area_fraction_low_percentage),
+                    str(details_forecast.seeing),
+                    str(details_forecast.transparency),
+                    str(details_forecast.wind10m_speed),
+                    await self.calc_condition_percentage(
+                        details_forecast.cloud_area_fraction_high_percentage,
+                        details_forecast.cloud_area_fraction_medium_percentage,
+                        details_forecast.cloud_area_fraction_low_percentage,
+                        details_forecast.seeing,
+                        details_forecast.transparency,
+                        details_forecast.wind10m_speed,
+                    ),
                 )
 
                 # Calculate Condition
                 if len(interval_points) <= int(math.floor(night_duration_astronomical / 3600)):
                     interval_points.append(
-                        await self.calc_condition_percentage(cloud_area_fraction, seeing, transparency, wind_speed)
+                        await self.calc_condition_percentage(
+                            details_forecast.cloud_area_fraction_high_percentage,
+                            details_forecast.cloud_area_fraction_medium_percentage,
+                            details_forecast.cloud_area_fraction_low_percentage,
+                            details_forecast.seeing,
+                            details_forecast.transparency,
+                            details_forecast.wind10m_speed,
+                        )
                     )
 
-                if row.forecast_time.hour == sun_next_rising.hour or idx >= (forecast_data_len - 1):
+                if details_forecast.forecast_time.hour == sun_next_rising.hour or index >= (forecast_data_len - 1):
                     item = {
                         "seventimer_init": init_ts,
                         "dayname": forecast_dayname,
                         "hour": start_forecast_hour,
                         "nightly_conditions": interval_points,
                         "weather": start_weather,
                     }
@@ -500,69 +515,49 @@
                         str(start_forecast_hour),
                         str(len(interval_points)),
                         str(start_weather),
                         conditions_numeric,
                     )
 
                     # Test for end of astronomical night. Will get true if we're already at night.
-                    if row.forecast_time.hour % 24 == sun_next_rising.hour:
+                    if details_forecast.forecast_time.hour % 24 == sun_next_rising.hour:
                         break
             start_index += 24
 
         return items
 
-    async def calc_condition_percentage(self, cloudcover, seeing, transparency, wind_speed):
+    async def calc_condition_percentage(self, cloudcover_high, cloudcover_medium, cloudcover_low, seeing, transparency, wind_speed):
         """Return condition based on cloud cover, seeing, transparency, and wind speed"""
-        # Possible Values:
-        #   Clouds: 1-9
-        #   Seeing: 1-8
-        #   Transparency: 1-8
-        #   Wind: 1-8
-
-        wind_speed_value = 0
-        for (start, end), derate in zip(WIND10M_RANGE, WIND10M_VALUE):
-            if start <= wind_speed <= end:
-                wind_speed_value = derate
+
+        # Seeing is something in between 0 and 2.5 arcsecs
+        seeing = int(100 - seeing * 40)
+        transparency = int((transparency - 1) * (100 / 7))
+        # Wind speed is something in between 0 and 16.5 m/s
+        if wind_speed > 16.5:
+            wind_speed = 16.5
+        wind_speed_value = int(100 - wind_speed * (100 / 16.5))
+
+        cloudcover = []
+        cloudcover.append(cloudcover_high * self._cloudcover_high_weakening)
+        cloudcover.append(cloudcover_medium * self._cloudcover_medium_weakening)
+        cloudcover.append(cloudcover_low * self._cloudcover_low_weakening)
 
         condition = int(
             100
             - (
-                self._cloudcover_weight * cloudcover
+                self._cloudcover_weight * max(cloudcover)
                 + self._seeing_weight * seeing
                 + self._transparency_weight * transparency
                 + self._calm_weight * wind_speed_value
-                - self._cloudcover_weight
-                - self._seeing_weight
-                - self._transparency_weight
-                - self._calm_weight
-            )
-            * 100
-            / (
-                self._cloudcover_weight * 9
-                + self._seeing_weight * 8
-                + self._transparency_weight * 8
-                + self._calm_weight * 8
-                - self._cloudcover_weight
-                - self._seeing_weight
-                - self._transparency_weight
-                - self._calm_weight
             )
+            / (self._cloudcover_weight + self._seeing_weight + self._transparency_weight + self._calm_weight)
         )
 
         return condition
 
-    async def calc_dewpoint2m(self, rh2m, temp2m):
-        """Calculate 2m Dew Point."""
-        # α(T,RH) = ln(RH/100) + aT/(b+T)
-        # Ts = (b × α(T,RH)) / (a - α(T,RH))
-        alpha = float(Decimal(str(rh2m / 100)).ln()) + MAGNUS_COEFFICIENT_A * temp2m / (MAGNUS_COEFFICIENT_B + temp2m)
-        dewpoint = (MAGNUS_COEFFICIENT_B * alpha) / (MAGNUS_COEFFICIENT_A - alpha)
-
-        return dewpoint
-
     async def _get_deepsky_objects(self):
         """Return Deepsky Objects for today"""
 
         items = []
 
         await self.retrieve_data_uptonight()
 
@@ -580,22 +575,22 @@
                     "type": dso_type.get(str(row), ""),
                     "constellation": dso_constellation.get(str(row), ""),
                     "size": dso_size.get(str(row), ""),
                     "foto": dso_foto.get(str(row), ""),
                 }
                 items.append(DSOUpTonight(item))
 
-                _LOGGER.debug(
-                    "DSO: %s, type: %s, constellation: %s, size: %s, foto: %s",
-                    str(item["target_name"]),
-                    str(item["type"]),
-                    str(item["constellation"]),
-                    str(item["size"]),
-                    str(item["foto"]),
-                )
+                # _LOGGER.debug(
+                #     "DSO: %s, type: %s, constellation: %s, size: %s, foto: %s",
+                #     str(item["target_name"]),
+                #     str(item["type"]),
+                #     str(item["constellation"]),
+                #     str(item["size"]),
+                #     str(item["foto"]),
+                # )
 
             return items
         return None
 
     async def retrieve_data_seventimer(self):
         """Retrieves current data from 7timer"""
 
@@ -604,14 +599,15 @@
             _LOGGER.debug("Updating data from 7Timer")
 
             astro_dataseries = None
 
             # Testing
             if self._test_mode:
                 if os.path.isfile("debug/astro.json"):
+                    _LOGGER.debug("Reading 7Timer from file")
                     with open("debug/astro.json") as json_file:
                         astro_dataseries_json = json.load(json_file)
                         astro_dataseries = astro_dataseries_json.get("dataseries", {})
                         json_data_astro = {"init": astro_dataseries_json.get("init")}
                 else:
                     json_data_astro = await self.async_request_seventimer("astro", "get")
                     astro_dataseries = json_data_astro.get("dataseries", {})
@@ -623,35 +619,31 @@
                 self._weather_data_seventimer = astro_dataseries
                 self._weather_data_seventimer_init = json_data_astro.get("init")
             else:
                 # Fake 7timer weather data if service is broken
                 # This eliminates consideration of seeing, transparency, and lifted_index
                 # TODO: Think about a complete redesign of the calculations and potentially
                 #       make met.no the leading source instead of 7timer
-                # TODO: Find another source for seeing and transparency
-                # self._seeing_weight = 0
-                # self._transparency_weight = 0
+                # TODO: Eventually calculate seeing?
                 self._weather_data_seventimer = []
                 for index in range(0, 20):
-                    self._weather_data_seventimer.append({"timepoint": index * 3, "seeing": 0, "transparency": 0, "lifted_index": 0})
+                    self._weather_data_seventimer.append({"timepoint": index * 3, "seeing": -1, "transparency": -1, "lifted_index": -1})
                 self._weather_data_seventimer_init = datetime.now().strftime("%Y%m%d%H")
         else:
             _LOGGER.debug("Using cached data for 7Timer")
 
     async def async_request_seventimer(self, product="astro", method="get") -> dict:
         """Make a request against the 7timer API."""
 
         use_running_session = self._session and not self._session.closed
 
         if use_running_session:
             session = self._session
         else:
-            session = ClientSession(
-                timeout=ClientTimeout(total=DEFAULT_TIMEOUT),
-            )
+            session = ClientSession(timeout=ClientTimeout(total=DEFAULT_TIMEOUT))
 
         # BASE_URL_SEVENTIMER = "https://www.7timer.info/bin/api.pl?lon=XX.XX&lat=YY.YY&product=astro&output=json"
         # STIMER_OUTPUT = "json"
         url = (
             str(f"{BASE_URL_SEVENTIMER}")
             + "?lon="
             + str("%.1f" % round(self._longitude, 2))
@@ -660,33 +652,34 @@
             + "&product="
             + str(product)
             + "&output="
             + STIMER_OUTPUT
         )
         try:
             _LOGGER.debug(f"Query url: {url}")
-            async with session.request(method, url, headers=HEADERS) as resp:
+            async with session.request(method, url, headers=HEADERS, ssl=False) as resp:
                 resp.raise_for_status()
                 plain = str(await resp.text()).replace("\n", " ")
                 data = json.loads(plain)
 
                 if self._test_mode:
                     json_string = json.dumps(data)
                     with open("debug/" + product + ".json", "w") as outfile:
                         outfile.write(json_string)
 
                 return data
+        except JSONDecodeError as jsonerr:
+            _LOGGER.error(f"JSON decode error, expecting value: {jsonerr}")
+            return {}
         except asyncio.TimeoutError as tex:
             _LOGGER.error(f"Request to endpoint timed out: {tex}")
             return {}
-            # raise RequestError(f"Request to endpoint timed out: {tex}") from None
         except ClientError as err:
             _LOGGER.error(f"Error requesting data: {err}")
             return {}
-            # raise RequestError(f"Error requesting data: {err}") from None
 
         finally:
             if not use_running_session:
                 await session.close()
 
     async def retrieve_data_metno(self):
         """Retrieves current data from met"""
@@ -696,14 +689,15 @@
             _LOGGER.debug("Updating data from Met.no")
 
             dataseries = None
 
             # Testing
             if self._test_mode:
                 if os.path.isfile("debug/met.json"):
+                    _LOGGER.debug("Reading Met.no data from file")
                     with open("debug/met.json") as json_file:
                         dataseries = json.load(json_file).get("properties", {}).get("timeseries", [])
                 else:
                     json_data_metno = await self.async_request_met("met", "get")
                     dataseries = json_data_metno.get("properties", {}).get("timeseries", [])
             else:
                 json_data_metno = await self.async_request_met("met", "get")
@@ -746,18 +740,23 @@
 
                 if self._test_mode:
                     json_string = json.dumps(data)
                     with open("debug/" + product + ".json", "w") as outfile:
                         outfile.write(json_string)
 
                 return data
+        except JSONDecodeError as jsonerr:
+            _LOGGER.error(f"JSON decode error, expecting value: {jsonerr}")
+            return {}
         except asyncio.TimeoutError as tex:
-            raise RequestError(f"Request to endpoint timed out: {tex}") from None
+            _LOGGER.error(f"Request to endpoint timed out: {tex}")
+            return {}
         except ClientError as err:
-            raise RequestError(f"Error requesting data: {err}") from None
+            _LOGGER.error(f"Error requesting data: {err}")
+            return {}
 
         finally:
             if not use_running_session:
                 await session.close()
 
     async def retrieve_data_uptonight(self):
         """Retrieves current data from uptonight"""
@@ -770,14 +769,12 @@
 
             if os.path.isfile(self._uptonight_path + "/uptonight-report.json"):
                 _LOGGER.debug(f"Uptonight report found")
                 with open(self._uptonight_path + "/uptonight-report.json") as json_file:
                     dataseries = json.load(json_file)
                     _LOGGER.debug(f"Uptonight imported")
             else:
-                _LOGGER.debug(
-                    f"uptonight-report.json not found. Current path: {self._uptonight_path}/uptonight-report.json"
-                )
+                _LOGGER.debug(f"uptonight-report.json not found. Current path: {self._uptonight_path}/uptonight-report.json")
 
             self._weather_data_uptonight = dataseries
         else:
             _LOGGER.debug("Using cached data for uptonight")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyastroweatherio-0.43.1.dev9/pyastroweatherio/const.py` & `pyastroweatherio-0.50.0.dev1/pyastroweatherio/const.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,74 @@
 """Constant Definitions for AstroWeather."""
 
-BASE_URL_SEVENTIMER = "https://www.7timer.info2/bin/api.pl"
+BASE_URL_SEVENTIMER = "https://www.7timer.info/bin/api.pl"
+# BASE_URL_SEVENTIMER = "https://167.99.8.254/bin/xasteria.php"
 BASE_URL_MET = "https://api.met.no/weatherapi/locationforecast/2.0/complete"
 HEADERS = {"User-Agent": "AstroWeather github.com/mawinkler/astroweather"}
 STIMER_OUTPUT = "json"
 
 DEFAULT_TIMEOUT = 10
 DEFAULT_CACHE_TIMEOUT = 1770
 DEFAULT_ELEVATION = 0
 DEFAULT_TIMEZONE = "Etc/UTC"
 DEFAULT_CONDITION_CLOUDCOVER_WEIGHT = 3
+DEFAULT_CONDITION_CLOUDCOVER_HIGH_WEAKENING = 1
+DEFAULT_CONDITION_CLOUDCOVER_MEDIUM_WEAKENING = 1
+DEFAULT_CONDITION_CLOUDCOVER_LOW_WEAKENING = 1
 DEFAULT_CONDITION_SEEING_WEIGHT = 2
 DEFAULT_CONDITION_TRANSPARENCY_WEIGHT = 1
 DEFAULT_CONDITION_CALM_WEIGHT = 2
 
 CIVIL_TWILIGHT = 0
 CIVIL_DUSK_DAWN = -6
 NAUTICAL_TWILIGHT = -6
 NAUTICAL_DUSK_DAWN = -12
 ASTRONOMICAL_TWILIGHT = -12
 ASTRONOMICAL_DUSK_DAWN = -18
 
 MAGNUS_COEFFICIENT_A = 17.625
 MAGNUS_COEFFICIENT_B = 243.04
+CONSTANT_C = 1.7
 
 DEEP_SKY_THRESHOLD = 75
 HOME_LATITUDE = 0.0
 HOME_LONGITUDE = 0.0
 
-CLOUDCOVER_PLAIN = [
-    "0 to 6%",
-    "6 to 19%",
-    "19 to 31%",
-    "31 to 44%",
-    "44 to 56%",
-    "56 to 69%",
-    "69 to 81%",
-    "81 to 94%",
-    "94 to 100%",
-]
-
-SEEING_PLAIN = [
-    'Below 0.5"',
-    '0.5 to 0.75"',
-    '0.75 to 1"',
-    '1 to 1.25"',
-    '1.25 to 1.5"',
-    '1.5 to 2"',
-    '2 to 2.5"',
-    'Over 2.5"',
+# CLOUDCOVER_PLAIN = [
+#     "0 to 6%",
+#     "6 to 19%",
+#     "19 to 31%",
+#     "31 to 44%",
+#     "44 to 56%",
+#     "56 to 69%",
+#     "69 to 81%",
+#     "81 to 94%",
+#     "94 to 100%",
+# ]
+
+# SEEING_PLAIN = [
+#     'Below 0.5"',
+#     '0.5 to 0.75"',
+#     '0.75 to 1"',
+#     '1 to 1.25"',
+#     '1.25 to 1.5"',
+#     '1.5 to 2"',
+#     '2 to 2.5"',
+#     'Over 2.5"',
+# ]
+
+SEEING = [
+    0.25,
+    0.625,
+    0.875,
+    1.125,
+    1.375,
+    1.75,
+    2.25,
+    2.5
 ]
 
 TRANSPARENCY_PLAIN = [
     "Below 0.3 mag",
     "0.3 to 0.4 mag",
     "0.4 to 0.5 mag",
     "0.5 to 0.6 mag",
```

### Comparing `pyastroweatherio-0.43.1.dev9/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.50.0.dev1/pyastroweatherio/dataclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Defines the Data Classes used."""
+
 from datetime import datetime, timezone
 import math
 
 from pyastroweatherio.const import (
-    CLOUDCOVER_PLAIN,
+    # CLOUDCOVER_PLAIN,
     CONDITION,
     CONDITION_PLAIN,
     DEEP_SKY_THRESHOLD,
     LIFTED_INDEX_PLAIN,
-    SEEING_PLAIN,
+    # SEEING_PLAIN,
     TRANSPARENCY_PLAIN,
     WIND10M_PLAIN,
     WIND10M_DIRECTON,
     WIND10M_VALUE,
     WIND10M_RANGE,
 )
 
@@ -63,91 +64,91 @@
     def condition_percentage(self) -> int:
         """Return condition based on cloud cover, seeing and transparency"""
         return self._condition_percentage
 
     @property
     def cloudcover(self) -> int:
         """Return Cloud Coverage."""
-        return self._cloudcover
+        return int(self._cloudcover)
 
     @property
     def cloudcover_percentage(self) -> int:
         """Return Cloud Cover Percentage."""
-        return int(-(100 * (1 - self._cloudcover) / 8))
+        return int(self._cloudcover)
 
     @property
     def cloudless_percentage(self) -> int:
         """Return Cloudless Percentage."""
-        return int(100 + 100 * (1 - self._cloudcover) / 8)
+        return 100 - int(self._cloudcover)
 
     @property
     def cloud_area_fraction_percentage(self) -> int:
         """Return Cloud Cover Percentage."""
-        return self._cloud_area_fraction
+        return int(self._cloud_area_fraction)
 
     @property
     def cloud_area_fraction_high_percentage(self) -> int:
         """Return Cloud Cover Percentage."""
-        return self._cloud_area_fraction_high
+        return int(self._cloud_area_fraction_high)
 
     @property
-    def cloud_area_fraction_low_percentage(self) -> int:
+    def cloud_area_fraction_medium_percentage(self) -> int:
         """Return Cloud Cover Percentage."""
-        return self._cloud_area_fraction_low
+        return int(self._cloud_area_fraction_medium)
 
     @property
-    def cloud_area_fraction_medium_percentage(self) -> int:
+    def cloud_area_fraction_low_percentage(self) -> int:
         """Return Cloud Cover Percentage."""
-        return self._cloud_area_fraction_medium
+        return int(self._cloud_area_fraction_low)
 
     @property
     def fog_area_fraction_percentage(self) -> int:
         """Return Fog Area Percentage."""
-        return self._fog_area_fraction
+        return int(self._fog_area_fraction)
 
     @property
-    def seeing(self) -> int:
+    def seeing(self) -> float:
         """Return Seeing."""
-        return self._seeing
+        return round(self._seeing, 2)
 
     @property
     def seeing_percentage(self) -> int:
         """Return Seeing."""
-        return int((100 + 100 / 7 - self._seeing * 100 / 7))
+        return int(100 - self._seeing * 40)
 
     @property
     def transparency(self) -> int:
         """Return Transparency."""
-        return self._transparency
+        return int(self._transparency)
 
     @property
     def transparency_percentage(self) -> int:
         """Return Transparency."""
         return int((100 + 100 / 7 - self._transparency * 100 / 7))
 
     @property
     def lifted_index(self) -> int:
         """Return Lifted Index."""
-        return self._lifted_index
+        return int(self._lifted_index)
 
     @property
     def rh2m(self) -> int:
         """Return 2m Relative Humidity."""
         return self._rh2m
 
     @property
     def wind10m_speed(self) -> float:
         """Return 10m Wind Speed."""
         return self._wind_speed
 
     @property
     def calm_percentage(self) -> int:
         """Return 10m Wind Speed."""
-        return int((100 + 100 / 7 - self._wind_speed * 100 / 7))
-    
+        return int(100 - self._wind_speed * (100 / 16.5))
+
     @property
     def wind10m_direction(self) -> str:
         """Return 10m Wind Direction."""
         direction = self._wind_from_direction
         direction += 22.5
         direction = direction % 360
         direction = int(direction / 45)  # values 0 to 7
@@ -213,15 +214,15 @@
         self._deepsky_forecast = data["deepsky_forecast"]
         self._uptonight = data["uptonight"]
 
     @property
     def time_shift(self) -> int:
         """Return Forecast Timestamp."""
         return self._time_shift
-    
+
     @property
     def forecast_length(self) -> int:
         """Return Forecast Length in Hours"""
         return self._forecast_length
 
     @property
     def latitude(self) -> float:
@@ -234,25 +235,26 @@
         return self._longitude
 
     @property
     def elevation(self) -> float:
         """Return Elevation."""
         return self._elevation
 
-    @property
-    def cloudcover_plain(self) -> str:
-        """Return Cloud Coverage."""
-        cover = self._cloudcover
-        if cover >= 1 and cover <= 9:
-            return CLOUDCOVER_PLAIN[cover - 1]
-        return None
+    # @property
+    # def cloudcover_plain(self) -> str:
+    #     """Return Cloud Coverage."""
+    #     cover = self._cloudcover
+    #     if cover >= 1 and cover <= 9:
+    #         return CLOUDCOVER_PLAIN[cover - 1]
+    #     return None
 
     @property
     def seeing_plain(self) -> str:
         """Return Seeing."""
+        return "Deprecated. Use seeing instead."
         seeing = self._seeing
         if seeing >= 1 and seeing <= 8:
             return SEEING_PLAIN[seeing - 1]
         return None
 
     @property
     def transparency_plain(self) -> str:
@@ -262,24 +264,24 @@
             return TRANSPARENCY_PLAIN[self._transparency - 1]
         return None
 
     @property
     def wind10m_speed_plain(self) -> str:
         """Return Transparency."""
         wind10m_speed = self._wind_speed
-        
+
         wind_speed_value = 0
         for (start, end), derate in zip(WIND10M_RANGE, WIND10M_VALUE):
             if start <= wind10m_speed <= end:
                 wind_speed_value = derate
-                
+
         if wind_speed_value >= 1 and wind_speed_value <= 8:
             return WIND10M_PLAIN[wind_speed_value - 1]
         return None
-    
+
     @property
     def lifted_index_plain(self) -> str:
         """Return Lifted Index."""
 
         trans = {
             -10: LIFTED_INDEX_PLAIN[0],
             -6: LIFTED_INDEX_PLAIN[1],
```

### Comparing `pyastroweatherio-0.43.1.dev9/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.50.0.dev1/pyastroweatherio/helper_functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """ Contains Helper functions for AstroWeather."""
+
 from datetime import datetime, timedelta
 import logging
 import ephem
 import math
+from decimal import Decimal
 from ephem import degree
 from math import degrees as deg
 import pytz
 
 # The introduction of the module [timezonefinder](https://github.com/jannikmi/timezonefinder)
 # with it's nested dependency to [py-h3](https://github.com/uber/h3-py) failed while compiling
 # the `c`-module h3 on some home assistant deployment variants (e.g. Home Assistant
@@ -19,14 +21,17 @@
     HOME_LONGITUDE,
     CIVIL_TWILIGHT,
     CIVIL_DUSK_DAWN,
     NAUTICAL_TWILIGHT,
     NAUTICAL_DUSK_DAWN,
     ASTRONOMICAL_TWILIGHT,
     ASTRONOMICAL_DUSK_DAWN,
+    MAGNUS_COEFFICIENT_A,
+    MAGNUS_COEFFICIENT_B,
+    CONSTANT_C,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class ConversionFunctions:
     """Convert between different Weather Units."""
@@ -54,103 +59,242 @@
         # aerosol_density = 0.1  # in kg/m^3
         # altitude = 1000  # in Meters
 
     # Modell 0: Simple linear Model
     async def calculate_seeing_model0(self, temperature, wind_speed, humidity, altitude):
         constant_1 = 0.314 * temperature / 273
         constant_2 = 20.8 * (1 - math.exp(-0.0695 * humidity))
-        constant_3 = 0.0017 * wind_speed ** 1.5
+        constant_3 = 0.0017 * wind_speed**1.5
         seeing = constant_1 + constant_2 + constant_3
-        _LOGGER.debug("AstronomicalSeeing calculation model1: T %s, W %s, H %s, E %s - S %s", str(temperature), str(wind_speed), str(humidity), str(altitude), str(seeing))
-        if seeing >= 2.5: return 7
-        if seeing >= 2.0: return 6
-        if seeing >= 1.5: return 5
-        if seeing >= 1.25: return 4
-        if seeing >= 1.0: return 3
-        if seeing >= 0.75: return 2
-        if seeing >= 0.5: return 1
-        return 0
-        # return 0.1 * temperature + 0.2 * wind_speed + 0.05 * humidity + 0.1 * aerosol_density - 0.05 * altitude
+
+        _LOGGER.debug(
+            "AstronomicalSeeing calculation model4: T %s, W %s, H %s, E %s - S %s",
+            str(temperature),
+            str(wind_speed),
+            str(humidity),
+            str(altitude),
+            str(seeing),
+        )
+
+        if seeing > 2.5:
+            _LOGGER.debug('AstronomicalSeeing above 2.5"')
+            seeing = 2.5
+
+        return seeing
 
     # Modell 1: Simple linear Model
     async def calculate_seeing_model1(self, temperature, wind_speed, humidity, altitude):
-        seeing = 0.1 * temperature + 0.2 * wind_speed + 0.05 * humidity # - 0.05 * altitude
-        _LOGGER.debug("AstronomicalSeeing calculation model1: T %s, W %s, H %s, E %s - S %s", str(temperature), str(wind_speed), str(humidity), str(altitude), str(seeing))
-        if seeing >= 2.5: return 7
-        if seeing >= 2.0: return 6
-        if seeing >= 1.5: return 5
-        if seeing >= 1.25: return 4
-        if seeing >= 1.0: return 3
-        if seeing >= 0.75: return 2
-        if seeing >= 0.5: return 1
-        return 0
-        # return 0.1 * temperature + 0.2 * wind_speed + 0.05 * humidity + 0.1 * aerosol_density - 0.05 * altitude
+        seeing = 0.1 * temperature + 0.2 * wind_speed + 0.05 * humidity  # - 0.05 * altitude
+
+        _LOGGER.debug(
+            "AstronomicalSeeing calculation model4: T %s, W %s, H %s, E %s - S %s",
+            str(temperature),
+            str(wind_speed),
+            str(humidity),
+            str(altitude),
+            str(seeing),
+        )
+
+        if seeing > 2.5:
+            _LOGGER.debug('AstronomicalSeeing above 2.5"')
+            seeing = 2.5
+
+        return seeing
 
     # Modell 2: Modell with Exponential functions
     async def calculate_seeing_model2(self, temperature, wind_speed, humidity, altitude):
-        seeing = 0.05 * temperature + 0.1 * wind_speed ** 1.5 + 0.02 * humidity ** 2 - 0.03 * altitude ** 1.5
-        _LOGGER.debug("AstronomicalSeeing calculation model2: T %s, W %s, H %s, E %s - S %s", str(temperature), str(wind_speed), str(humidity), str(altitude), str(seeing))
-        if seeing >= 2.5: return 7
-        if seeing >= 2.0: return 6
-        if seeing >= 1.5: return 5
-        if seeing >= 1.25: return 4
-        if seeing >= 1.0: return 3
-        if seeing >= 0.75: return 2
-        if seeing >= 0.5: return 1
-        return 0
-        # return 0.05 * temperature + 0.1 * wind_speed ** 1.5 + 0.02 * humidity ** 2 + 0.08 * aerosol_density - 0.03 * altitude ** 1.5
+        seeing = 0.05 * temperature + 0.1 * wind_speed**1.5 + 0.02 * humidity**2 - 0.03 * altitude**1.5
+
+        _LOGGER.debug(
+            "AstronomicalSeeing calculation model4: T %s, W %s, H %s, E %s - S %s",
+            str(temperature),
+            str(wind_speed),
+            str(humidity),
+            str(altitude),
+            str(seeing),
+        )
+
+        if seeing > 2.5:
+            _LOGGER.debug('AstronomicalSeeing above 2.5"')
+            seeing = 2.5
 
-    # Modell 3: Modell basierend auf empirischen Daten
+        return seeing
+
+    # Modell 3: Modell based on empirical Data
     async def calculate_seeing_model3(self, temperature, wind_speed, humidity, altitude):
         seeing = 0.08 * temperature + 0.15 * math.log(wind_speed + 1) + 0.03 * humidity - 0.02 * altitude
-        _LOGGER.debug("AstronomicalSeeing calculation model3: T %s, W %s, H %s, E %s - S %s", str(temperature), str(wind_speed), str(humidity), str(altitude), str(seeing))
-        if seeing >= 2.5: return 7
-        if seeing >= 2.0: return 6
-        if seeing >= 1.5: return 5
-        if seeing >= 1.25: return 4
-        if seeing >= 1.0: return 3
-        if seeing >= 0.75: return 2
-        if seeing >= 0.5: return 1
-        return 0
-        # return 0.08 * temperature + 0.15 * math.log(wind_speed + 1) + 0.03 * humidity + 0.1 * aerosol_density - 0.02 * altitude
 
+        _LOGGER.debug(
+            "AstronomicalSeeing calculation model4: T %s, W %s, H %s, E %s - S %s",
+            str(temperature),
+            str(wind_speed),
+            str(humidity),
+            str(altitude),
+            str(seeing),
+        )
+
+        if seeing > 2.5:
+            _LOGGER.debug('AstronomicalSeeing above 2.5"')
+            seeing = 2.5
+
+        return seeing
+
+    # Modell 4:
+    # This algorithm first calculates the seeing factor based on temperature, humidity, wind speed
+    # and altitude above sea level. The seeing factor is then used to calculate the astronomical
+    # seeing in arcseconds. The empirical relationship used here states that the seeing in arcseconds
+    # is approximately equal to the reciprocal of the seeing factor multiplied by a conversion
+    # factor of 0.98.
     def calculate_dew_point(self, temperature, humidity):
-        a = 17.62
-        b = 243.12
-        gamma = math.log(humidity / 100) + (a * temperature) / (b + temperature)
-        dew_point = (b * gamma) / (a - gamma)
+        alpha = math.log(humidity / 100) + (MAGNUS_COEFFICIENT_A * temperature) / (MAGNUS_COEFFICIENT_B + temperature)
+        dew_point = (MAGNUS_COEFFICIENT_B * alpha) / (MAGNUS_COEFFICIENT_A - alpha)
+
         return dew_point
 
     def calculate_saturation_vapor_pressure(self, dew_point):
         es = 6.11 * (10 ** (7.5 * dew_point / (237.7 + dew_point)))
+
         return es
 
     def calculate_water_vapor_pressure(self, temperature, humidity):
         dew_point = self.calculate_dew_point(temperature, humidity)
         es = self.calculate_saturation_vapor_pressure(dew_point)
         water_vapor_pressure = (humidity / 100) * es
+
         return water_vapor_pressure
 
     async def calculate_seeing_model4(self, temperature, humidity, wind_speed, altitude):
         water_vapor_pressure = self.calculate_water_vapor_pressure(temperature, humidity)
+
         adjusted_pressure = 1013.25 * math.exp(-0.00012 * altitude)
         relative_pressure = adjusted_pressure / 1013.25
-        seeing_factor = 0.8 * (water_vapor_pressure / 10) ** 0.25 * (wind_speed / 10) ** 0.75 * relative_pressure
+
+        seeing_factor = CONSTANT_C * (water_vapor_pressure / 10) ** 0.25 * (wind_speed / 10) ** 0.75 * relative_pressure
+        seeing = 0.98 / seeing_factor
+
+        _LOGGER.debug(
+            "AstronomicalSeeing calculation model4: T %s, W %s, H %s, E %s - S %s",
+            str(temperature),
+            str(wind_speed),
+            str(humidity),
+            str(altitude),
+            str(seeing),
+        )
+
+        if seeing > 2.5:
+            seeing = 2.5
+
+        return seeing
+
+    # Modell 5:
+    # This algorithm first calculates the seeing factor based on temperature, humidity, wind speed
+    # and altitude above sea level. It is similar to Model 4 but uses the air pressure at sea level
+    # provided by Met.no.
+    async def calculate_seeing_model5(self, temperature, humidity, wind_speed, altitude, air_pressure_at_sea_level):
+        water_vapor_pressure = self.calculate_water_vapor_pressure(temperature, humidity)
+
+        adjusted_pressure = air_pressure_at_sea_level * math.exp(-0.00012 * altitude)
+        relative_pressure = adjusted_pressure / air_pressure_at_sea_level
+
+        seeing_factor = CONSTANT_C * (water_vapor_pressure / 10) ** 0.25 * (wind_speed / 10) ** 0.75 * relative_pressure
         seeing = 0.98 / seeing_factor
-        _LOGGER.debug("AstronomicalSeeing calculation model3: T %s, W %s, H %s, E %s - S %s", str(temperature), str(wind_speed), str(humidity), str(altitude), str(seeing))
-        if seeing >= 2.5: return 7
-        if seeing >= 2.0: return 6
-        if seeing >= 1.5: return 5
-        if seeing >= 1.25: return 4
-        if seeing >= 1.0: return 3
-        if seeing >= 0.75: return 2
-        if seeing >= 0.5: return 1
-        return 0
-        # return seeing_factor
 
+        _LOGGER.debug(
+            "AstronomicalSeeing calculation model5: T %s, W %s, H %s, E %s, P %s - S %s",
+            str(temperature),
+            str(wind_speed),
+            str(humidity),
+            str(altitude),
+            str(air_pressure_at_sea_level),
+            str(seeing),
+        )
+
+        if seeing > 2.5:
+            seeing = 2.5
+
+        return seeing
+
+    def calculate_water_vapor_pressure6(self, dew_point_temperature, humidity):
+        dew_point = dew_point_temperature
+        es = self.calculate_saturation_vapor_pressure(dew_point)
+        water_vapor_pressure = (humidity / 100) * es
+
+        return water_vapor_pressure
+    
+    # Modell 6:
+    # This algorithm first calculates the seeing factor based on temperature, humidity, wind speed
+    # and altitude above sea level. It is similar to Model 4 and 5 but uses the air pressure at sea level
+    # and dew point provided by Met.no.
+    async def calculate_seeing_model6(self, temperature, humidity, dew_point_temperature, wind_speed, cloud_cover, altitude, air_pressure_at_sea_level):
+        water_vapor_pressure = self.calculate_water_vapor_pressure6(dew_point_temperature, humidity)
+
+        adjusted_pressure = air_pressure_at_sea_level * math.exp(-0.00012 * altitude)
+        relative_pressure = adjusted_pressure / air_pressure_at_sea_level
+
+        seeing_factor = CONSTANT_C * (water_vapor_pressure / 10) ** 0.35 * (wind_speed / 10) ** 0.65 * relative_pressure
+        seeing = 0.98 / seeing_factor
+
+        _LOGGER.debug(
+            "AstronomicalSeeing calculation model6: T %s, H %s, DP %s, W %s, E %s, P %s - S %s",
+            str(temperature),
+            str(humidity),
+            str(dew_point_temperature),
+            str(wind_speed),
+            str(altitude),
+            str(air_pressure_at_sea_level),
+            str(seeing),
+        )
+
+        if seeing > 2.5:
+            seeing = 2.5  # max out seeing
+
+        return seeing
+
+    def calculate_water_vapor_pressure7(self, dew_point_temperature, humidity):
+        dew_point = dew_point_temperature
+        es = self.calculate_saturation_vapor_pressure(dew_point)
+        water_vapor_pressure = (humidity / 100) * es
+
+        return water_vapor_pressure
+    
+    # Modell 7:
+    # This algorithm first calculates the seeing factor based on temperature, humidity, wind speed
+    # and altitude above sea level. It is similar to Model 6 but takes the cloud coverage into account.
+    # This somehow doesn't seem to be correct, since seeing can be good even with clouds.
+    async def calculate_seeing_model7(self, temperature, humidity, dew_point_temperature, wind_speed, cloud_cover, altitude, air_pressure_at_sea_level):
+        water_vapor_pressure = self.calculate_water_vapor_pressure7(dew_point_temperature, humidity)
+
+        adjusted_pressure = air_pressure_at_sea_level * math.exp(-0.00012 * altitude)
+        relative_pressure = adjusted_pressure / air_pressure_at_sea_level
+
+        # Take care on the clouds
+        cloud_factor = 1 - (cloud_cover / 100)
+
+        seeing_factor = CONSTANT_C * (water_vapor_pressure / 10) ** 0.2 * (wind_speed / 10) ** 0.6 * relative_pressure ** 0.3 * cloud_factor
+        if seeing_factor == 0:
+            seeing = 2.5  # max out seeing
+        else:
+            seeing = 0.98 / seeing_factor
+
+        _LOGGER.debug(
+            "AstronomicalSeeing calculation model7: T %s, H %s, DP %s, W %s, C %s, E %s, P %s - S %s",
+            str(temperature),
+            str(humidity),
+            str(dew_point_temperature),
+            str(wind_speed),
+            str(cloud_cover),
+            str(altitude),
+            str(air_pressure_at_sea_level),
+            str(seeing),
+        )
+
+        if seeing > 2.5:
+            seeing = 2.5  # max out seeing
+
+        return seeing
 
 
 class AstronomicalRoutines:
     """Calculate different astronomical objects"""
 
     def __init__(
         self,
@@ -565,16 +709,16 @@
         return False
 
     #
     # Public methods
     #
     async def time_shift(self) -> int:
         """Returns the time_shift to UTC"""
-        return self.utc_to_local_diff() * 3600
-        
+        return int(self.utc_to_local_diff() * 3600)
+
     async def need_update(self, forecast_time=None):
         """Update Sun and Moon"""
         if forecast_time is not None:
             self._forecast_time = forecast_time.replace(tzinfo=pytz.utc)
 
         self.calculate_sun_altaz()
         self.calculate_moon_altaz()
@@ -871,15 +1015,14 @@
 
             if await self.deep_sky_darkness_moon_always_down():
                 dsd = self._sun_next_rising_astro - self._forecast_time
                 _LOGGER.debug(f"DSD - Moon always down {dsd}")
             else:
                 _LOGGER.debug(f"DSD - Moon NOT always down {dsd}")
 
-
         if not self.astronomical_darkness():
             _LOGGER.debug(f"DSD - At sunlight")
             if await self.deep_sky_darkness_moon_rises():
                 dsd = self._moon_next_rising - self._sun_next_setting_astro
                 _LOGGER.debug(f"DSD - Sun up, Moon rises {dsd}")
 
             if await self.deep_sky_darkness_moon_sets():
```

### Comparing `pyastroweatherio-0.43.1.dev9/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.50.0.dev1/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.43.1.dev9
+Version: 0.50.0.dev1
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
@@ -15,12 +15,13 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: pyephem
 
 Lightweight Python 3 module to receive data via REST API from 7Timer and Met.no.
```

### Comparing `pyastroweatherio-0.43.1.dev9/setup.py` & `pyastroweatherio-0.50.0.dev1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.43.1.dev9",
+    version="0.50.0.dev1",
     license="MIT",
     description="Python Wrapper for 7Timer and Met.no REST API",
     long_description=" ".join(
         [
             "Lightweight Python 3 module to receive data via",
             "REST API from 7Timer and Met.no.",
         ],
@@ -27,9 +27,10 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
+        "Programming Language :: Python :: 3.13",
     ],
 )
```

