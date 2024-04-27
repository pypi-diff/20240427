# Comparing `tmp/hydrobricks-0.7.0.tar.gz` & `tmp/hydrobricks-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrobricks-0.7.0.tar", last modified: Mon Feb 19 08:12:01 2024, max compression
+gzip compressed data, was "hydrobricks-0.7.1.tar", last modified: Sat Apr 27 16:07:24 2024, max compression
```

## Comparing `hydrobricks-0.7.0.tar` & `hydrobricks-0.7.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:12:01.619288 hydrobricks-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-02-19 08:12:01.615288 hydrobricks-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:12:01.615288 hydrobricks-0.7.0/hydrobricks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-02-19 08:12:01.000000 hydrobricks-0.7.0/hydrobricks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-02-19 08:12:01.000000 hydrobricks-0.7.0/hydrobricks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 08:12:01.000000 hydrobricks-0.7.0/hydrobricks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 08:12:01.000000 hydrobricks-0.7.0/hydrobricks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-19 08:12:01.000000 hydrobricks-0.7.0/hydrobricks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-19 08:12:01.000000 hydrobricks-0.7.0/hydrobricks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:12:01.611288 hydrobricks-0.7.0/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:12:01.611288 hydrobricks-0.7.0/python/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:12:01.615288 hydrobricks-0.7.0/python/src/hydrobricks/
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:12:01.615288 hydrobricks-0.7.0/python/src/hydrobricks/behaviours/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/behaviours/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/behaviours/behaviour.py
--rw-r--r--   0 runner    (1001) docker     (127)    22097 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/behaviours/behaviour_land_cover_change.py
--rw-r--r--   0 runner    (1001) docker     (127)    46041 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/catchment.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    29689 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/forcing.py
--rw-r--r--   0 runner    (1001) docker     (127)    14242 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/hydro_units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:12:01.615288 hydrobricks-0.7.0/python/src/hydrobricks/models/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15455 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/models/model_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/models/socont.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/observations.py
--rw-r--r--   0 runner    (1001) docker     (127)    31056 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    14463 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/time_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/python/src/hydrobricks/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 08:12:01.619288 hydrobricks-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-02-19 08:11:42.000000 hydrobricks-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:07:24.785595 hydrobricks-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-27 16:07:24.785595 hydrobricks-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:07:24.785595 hydrobricks-0.7.1/hydrobricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-27 16:07:24.000000 hydrobricks-0.7.1/hydrobricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-27 16:07:24.000000 hydrobricks-0.7.1/hydrobricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:07:24.000000 hydrobricks-0.7.1/hydrobricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:07:24.000000 hydrobricks-0.7.1/hydrobricks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-27 16:07:24.000000 hydrobricks-0.7.1/hydrobricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-27 16:07:24.000000 hydrobricks-0.7.1/hydrobricks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:07:24.777595 hydrobricks-0.7.1/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:07:24.781595 hydrobricks-0.7.1/python/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:07:24.785595 hydrobricks-0.7.1/python/src/hydrobricks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:07:24.785595 hydrobricks-0.7.1/python/src/hydrobricks/behaviours/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/behaviours/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/behaviours/behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22097 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/behaviours/behaviour_land_cover_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57573 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/catchment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29697 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/forcing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14254 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/hydro_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:07:24.785595 hydrobricks-0.7.1/python/src/hydrobricks/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15509 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/models/model_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/models/socont.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/observations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31056 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14463 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/python/src/hydrobricks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 16:07:24.785595 hydrobricks-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-27 16:07:12.000000 hydrobricks-0.7.1/setup.py
```

### Comparing `hydrobricks-0.7.0/LICENSE` & `hydrobricks-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.0/PKG-INFO` & `hydrobricks-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrobricks
-Version: 0.7.0
+Version: 0.7.1
 Summary: A modular hydrological modelling framework
 Author: Pascal Horton
 Author-email: pascal.horton@unibe.ch
 License: MIT
 Project-URL: Source Code, https://github.com/hydrobricks/hydrobricks
 Project-URL: Bug Tracker, https://github.com/hydrobricks/hydrobricks/issues
 Classifier: Programming Language :: C++
```

### Comparing `hydrobricks-0.7.0/README.md` & `hydrobricks-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.0/hydrobricks.egg-info/PKG-INFO` & `hydrobricks-0.7.1/hydrobricks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrobricks
-Version: 0.7.0
+Version: 0.7.1
 Summary: A modular hydrological modelling framework
 Author: Pascal Horton
 Author-email: pascal.horton@unibe.ch
 License: MIT
 Project-URL: Source Code, https://github.com/hydrobricks/hydrobricks
 Project-URL: Bug Tracker, https://github.com/hydrobricks/hydrobricks/issues
 Classifier: Programming Language :: C++
```

### Comparing `hydrobricks-0.7.0/hydrobricks.egg-info/SOURCES.txt` & `hydrobricks-0.7.1/hydrobricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.0/pyproject.toml` & `hydrobricks-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.0/python/src/hydrobricks/__init__.py` & `hydrobricks-0.7.1/python/src/hydrobricks/__init__.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.0/python/src/hydrobricks/behaviours/behaviour_land_cover_change.py` & `hydrobricks-0.7.1/python/src/hydrobricks/behaviours/behaviour_land_cover_change.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.0/python/src/hydrobricks/catchment.py` & `hydrobricks-0.7.1/python/src/hydrobricks/catchment.py`

 * *Files 11% similar despite different names*

```diff
@@ -479,17 +479,17 @@
 
     def resample_dem_and_calculate_slope_aspect(self, resolution, output_path):
         """
         Resample the DEM and calculate the slope and aspect of the whole DEM.
 
         Parameters
         ----------
-        resolution : float
+        resolution : ?float
             Desired pixel resolution.
-        output_path : str
+        output_path : str|Path
             Path of the directory to save the downsampled DEM to.
 
         Returns
         -------
         The downsampled DEM, the masked downsampled DEM data, the slope and the aspect.
         """
         if not hb.has_rasterio:
@@ -518,15 +518,17 @@
             xr_dem_downsampled = xr_dem.rio.reproject(
                 xr_dem.rio.crs,
                 shape=(new_height, new_width),
                 resampling=Resampling.bilinear,
             )
 
         # Save the downsampled DEM to a file
-        filepath = output_path + '/downsampled_dem.tif'
+        if isinstance(output_path, str):
+            output_path = Path(output_path)
+        filepath = output_path / 'downsampled_dem.tif'
         xr_dem_downsampled.rio.to_raster(filepath)
 
         # Reopen the downsampled DEM as a rasterio dataset
         new_dem = hb.rasterio.open(filepath)
         if self.outline is not None:
             geoms = [mapping(polygon) for polygon in self.outline]
             new_masked_dem_data, _ = mask(new_dem, geoms, crop=False)
@@ -550,14 +552,214 @@
 
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=UserWarning)  # pyproj
             xr_dem = hb.rxr.open_rasterio(self.dem.files[0]).drop_vars('band')[0]
             self.slope = hb.xrs.slope(xr_dem, name='slope').to_numpy()
             self.aspect = hb.xrs.aspect(xr_dem, name='aspect').to_numpy()
 
+    def get_hillshade(self, azimuth=315, altitude=45, z_factor=1):
+        """
+        Create a hillshade from the DEM.
+
+        Adapted from https://github.com/royalosyin/Work-with-DEM-data-using-Python-
+        from-Simple-to-Complicated/blob/master/ex07-Hillshade%20from%20a%20Digital
+        %20Elevation%20Model%20(DEM).ipynb
+
+        Parameters
+        ----------
+        azimuth : float
+            The desired azimuth for the hillshade.
+        altitude : float
+            The desired sun angle altitude for the hillshade.
+        z_factor : float
+            The z factor to amplify the relief.
+
+        Returns
+        -------
+        A numpy array containing hillshade values.
+        """
+        x, y = np.gradient(self.dem.read(1))
+        x_pixel_size = self.get_dem_x_resolution()
+        y_pixel_size = self.get_dem_y_resolution()
+
+        if azimuth > 360.0:
+            raise ValueError(
+                "Azimuth value should be less than or equal to 360 degrees")
+
+        if altitude > 90.0:
+            raise ValueError(
+                "Altitude value should be less than or equal to 90 degrees")
+
+        # Account for the pixel size
+        x = z_factor * x / x_pixel_size
+        y = z_factor * y / y_pixel_size
+
+        azimuth = 360.0 - azimuth
+        azimuth_rad = azimuth * np.pi / 180.0
+        altitude_rad = altitude * np.pi / 180.0
+
+        slope = np.pi / 2.0 - np.arctan(np.sqrt(x * x + y * y))
+        aspect = np.arctan2(-x, y)
+
+        shaded = (np.sin(altitude_rad) * np.sin(slope) +
+                  np.cos(altitude_rad) * np.cos(slope) *
+                  np.cos((azimuth_rad - np.pi / 2.0) - aspect))
+
+        return 255 * (shaded + 1) / 2
+
+    @staticmethod
+    def get_solar_declination_rad(day_of_year):
+        """
+        Compute the solar declination.
+
+        The solar declination is the angle between the rays of the Sun and the
+        plane of the Earth's equator. It represents how much the sun is
+        tilted towards or away from the observer's latitude. The calculation
+        involves trigonometric functions to account for the observer's latitude
+        and the position of the sun in the sky.
+
+        Parameters
+        ----------
+        day_of_year : int|np.array
+            Day of the year (1-366).
+
+        Returns
+        -------
+        The solar declination in radians
+        """
+
+        # Normalized day of the year
+        # '(jd-172)' calculates the number of days that have passed since the summer
+        # solstice (around June 21st), which is day 172 in a non-leap year.
+        # '(360*(jd-172))/365' normalizes this count to a value representing the
+        # position in the orbit of the Earth around the Sun (in degrees).
+        ndy = ((360 * (day_of_year - 172)) / 365)
+
+        # The cos(...) function is applied to the normalized day of the year. It
+        # produces values between -1 and 1, representing the variation in solar
+        # declination throughout the year. The constant factor 23.45 represents the
+        # tilt of the Earth's axis relative to its orbital plane. This tilt causes the
+        # variation in the angle of the sun's rays reaching different latitudes
+        # on Earth.
+        solar_declin = 23.45 * np.cos(ndy * TO_RAD) * TO_RAD
+
+        return solar_declin
+
+    @staticmethod
+    def get_solar_hour_angle_limit(solar_declination, lat_rad):
+        """
+        Compute the hour angle limit value (min/max).
+
+        The hour angle is the angular distance between the sun and the observer's
+        meridian. It is typically measured in degrees. The tangent of
+        solar_declin/lat_rad represents the ratio of the opposite side
+        (vertical component of the sun's rays) to the adjacent side (horizontal
+        component). It helps capture how much the sun/the observer's location is
+        tilted north or south relative to the equator.
+
+        Parameters
+        ----------
+        solar_declination : float|np.array
+            Solar declination in radians.
+        lat_rad : float
+            Latitude in radians.
+
+        Returns
+        -------
+        The limit value of the hour angle in radians.
+        """
+
+        # The negative sign is applied because the Hour Angle is negative in the
+        # morning and positive in the afternoon.
+        hour_angle = np.arccos(-np.tan(solar_declination) * np.tan(lat_rad))
+
+        return hour_angle
+
+    @staticmethod
+    def get_solar_zenith(hour_angles, lat_rad, solar_declination):
+        """
+        Compute the solar zenith.
+
+        The Solar zenith (IQBAL 2012) is the angle between the sun and the
+        vertical (zenith) position directly above the observer. The result is
+        expressed in degrees. The calculation involves trigonometric functions
+        to account for the observer's latitude, the solar declination, and the
+        position of the sun in the sky (represented by the Hour Angles).
+
+        Parameters
+        ----------
+        hour_angles : float|np.ndarray
+            Hour angle(s).
+        lat_rad : float
+            Latitude in radians.
+        solar_declination : float
+            Solar declination in radians.
+
+        Returns
+        -------
+        The solar zenith in degrees.
+        """
+        zenith = np.arccos((np.sin(lat_rad) * np.sin(solar_declination)) +
+                           (np.cos(lat_rad) * np.cos(solar_declination) *
+                            np.cos(hour_angles))) * TO_DEG
+        return zenith
+
+    @staticmethod
+    def get_solar_azimuth_to_south(hour_angles, lat_rad, solar_declination):
+        """
+        Compute the solar azimuth relative to the south.
+
+        The solar azimuth is the angle between the sun and the observer's meridian.
+        It is typically measured in degrees.
+        Azimuth with negative values before solar noon and positive values with
+        positive values after solar noon. Solar noon is defined by the change in sign
+        of the hour angle (negative in the morning, positive in the afternoon).
+        From https://www.astrolabe-science.fr/diagramme-solaire-azimut-hauteur
+
+        Parameters
+        ----------
+        hour_angles : float|np.ndarray
+            Array with the hour angles.
+        lat_rad : float
+            Latitude in radians.
+        solar_declination : float
+            Solar declination.
+
+        Returns
+        -------
+        The solar azimuth in degrees.
+        """
+        convert_to_float = False
+        if isinstance(hour_angles, (int, float)):
+            hour_angles = np.array([hour_angles])
+            convert_to_float = True
+
+        azimuth = np.degrees(np.arctan(np.sin(hour_angles) / (
+                np.sin(lat_rad) * np.cos(hour_angles) -
+                np.cos(lat_rad) * np.tan(solar_declination))))
+        azimuth[np.where((azimuth < 0) & (hour_angles > 0))] += 180
+        azimuth[np.where((azimuth > 0) & (hour_angles < 0))] -= 180
+
+        if convert_to_float:
+            azimuth = azimuth[0]
+
+        return azimuth
+
+    @staticmethod
+    def get_solar_azimuth_to_north(hour_angles, lat_rad, solar_declination):
+        """
+        Compute the solar azimuth relative to the north.
+        See get_solar_azimuth_to_south() for more details.
+        """
+        azimuth = Catchment.get_solar_azimuth_to_south(
+            hour_angles, lat_rad, solar_declination)
+        azimuth += 180
+
+        return azimuth
+
     @staticmethod
     def _calculate_radiation_hock_equation(elevation, atmos_transmissivity, day_of_year,
                                            zenith, incidence_angle):
         """
         Hock (2005) equation to compute the potential clear-sky direct solar
         radiation at the ice or snow surface [W/m²].
 
@@ -575,14 +777,22 @@
             Angle of incidence between the normal to the grid slope and the
             solar beam
 
         Returns
         -------
         The potential clear-sky direct solar radiation at the ice or snow
         surface [W/m²]
+
+        Notes
+        -----
+        This function is based on the R package TopoSol, authored by Matthew Olson.
+
+        References
+        ----------
+        - Original R package: https://github.com/mattols/TopoSol
         """
 
         # True anomaly (the angle subtended at the Sun between the semi major
         # axis line and the current position)
         # Different definition here:
         # https://physics.stackexchange.com/questions/177949/earth-sun-distance-on-a-given-day-of-the-year
         theta = (365.5 / 360) * day_of_year
@@ -636,14 +846,22 @@
             Aspect of the DEM, in degrees
         tolerance : float
             Error tolerance in the trigonometric computations.
 
         Returns
         -------
         The angle of incidence.
+
+        Notes
+        -----
+        This function is based on the R package TopoSol, authored by Matthew Olson.
+
+        References
+        ----------
+        - Original R package: https://github.com/mattols/TopoSol
         """
 
         # Solar zenith and azimuth on a slope
         zenith_rad = zenith * TO_RAD
         slope_rad = slope * TO_RAD
         azimuth_rad = azimuth * TO_RAD
         aspect_rad = (aspect - 180) * TO_RAD
@@ -658,17 +876,126 @@
             raise ValueError("Argument of arccos is above or below 1.")
 
         # Angle of incidence matrix
         incidence_angle[incidence_angle > 90 * TO_RAD] = 90 * TO_RAD
 
         return incidence_angle
 
+    def calculate_cast_shadows(self, dem_dataset, masked_dem,
+                               zenith, azimuth, lat):
+        """
+        Calculate the cast shadows.
+
+        The approach relies on tilting the DEM to obtain a horizon matching the sun
+        rays and filling the DEM. The algorithm is applied to the whole topography
+        before masking the areas outside the catchment.
+
+        Parameters
+        ----------
+        dem_dataset :
+            DEM as read by rasterio, containing the DEM topography
+        masked_dem : float
+            DEM topography, masked with np.nan for the areas outside the study catchment
+        zenith : float
+            Solar zenith (IQBAL 2012), in degrees
+        azimuth : float
+            Azimuth relative to the south for ZSLOPE CALC, in degrees
+        lat : float
+            Mean latitude of the catchment, in degrees
+
+        Returns
+        -------
+        A np.array with the cast shadows (1), the in sun areas (0),
+        and the masked area (np.nan).
+
+        Notes
+        -----
+        The algorithm is applied to the whole topography before masking the
+        areas outside the catchment.
+        """
+        dem = dem_dataset.read(1)
+        x_size = abs(dem_dataset.res[0])
+        y_size = abs(dem_dataset.res[1])
+
+        if x_size != y_size:
+            raise ValueError("The DEM x and y resolutions must be equal "
+                             "for computing the cast shadows.")
+
+        if zenith >= 90:
+            cast_shadows = np.ones(dem.shape)
+            cast_shadows[np.isnan(masked_dem)] = np.nan
+            return cast_shadows
+
+        # Get mean pixel size
+        pixel_size = (x_size + y_size) / 2
+
+        # Get the x and y grids for the DEM
+        xv, yv = np.indices(dem.shape)
+
+        # Get the base arrays for the solar ray IDs and the offset distances
+        if azimuth < -135:  # NNE
+            ref_grid = xv
+            base_ray_ids = yv[:, ::-1]
+            angle = np.tan(-(azimuth + 90) * TO_RAD)
+        elif azimuth < -90:  # ENE
+            ref_grid = yv[:, ::-1]
+            base_ray_ids = xv
+            angle = np.tan((azimuth + 180) * TO_RAD)
+        elif azimuth < -45:  # ESE
+            ref_grid = yv[:, ::-1]
+            base_ray_ids = xv[::-1, :]
+            angle = np.tan(-azimuth * TO_RAD)
+        elif azimuth < 0:  # SSE
+            ref_grid = xv[::-1, :]
+            base_ray_ids = yv[:, ::-1]
+            angle = np.tan((90 + azimuth) * TO_RAD)
+        elif azimuth < 45:  # SSW
+            ref_grid = xv[::-1, :]
+            base_ray_ids = yv
+            angle = np.tan((90 - azimuth) * TO_RAD)
+        elif azimuth < 90:  # WSW
+            ref_grid = yv
+            base_ray_ids = xv[::-1, :]
+            angle = np.tan(azimuth * TO_RAD)
+        elif azimuth < 135:  # WNW
+            ref_grid = yv
+            base_ray_ids = xv
+            angle = np.tan((180 - azimuth) * TO_RAD)
+        else:  # NNW
+            ref_grid = xv
+            base_ray_ids = yv
+            angle = np.tan((azimuth - 90) * TO_RAD)
+
+        # Computation of the solar ray paths for each pixel (rays with different IDs).
+        ray_ids = base_ray_ids - ref_grid / angle  # Adding the offset (from azimuth)
+        ray_ids = ray_ids - np.nanmin(ray_ids)  # Set all IDs to positive values
+        ray_ids = ray_ids.astype(int) + 1  # Convert to int
+
+        # Compute the tilted DEM
+        orthogonal_distance = ref_grid + base_ray_ids / angle  # Projected distance
+        tilt_heights = orthogonal_distance * pixel_size / np.tan(zenith * TO_RAD)
+        tilted_dem = dem + tilt_heights  # DEM after tilt of zenith °, azimuthal dir.
+
+        # Remapping of the solar rays on another matrix to process them.
+        mapped = np.ones((np.nanmax(ray_ids) + 1, np.max(ref_grid) + 1))
+        mapped = mapped * np.nan  # Mapping of the tilted DEM from solar rays ...
+        mapped[ray_ids, ref_grid] = tilted_dem  # ... to row/columns.
+        accumulated = np.fmax.accumulate(mapped, axis=1)
+        cast_sh = (accumulated > mapped).astype(float)
+        cast_shadows = cast_sh[ray_ids, ref_grid]
+
+        # Put the mask back on (we previously needed the surrounding topography).
+        cast_shadows[np.isnan(masked_dem)] = np.nan
+
+        return cast_shadows
+
     def calculate_daily_potential_radiation(self, output_path, resolution=None,
                                             atmos_transmissivity=0.75,
-                                            steps_per_hour=4):
+                                            steps_per_hour=4,
+                                            with_cast_shadows=True):
         """
         Compute the daily mean potential clear-sky direct solar radiation
         at the DEM surface [W/m²] using Hock (1999)'s equation.
         It is computed for each day of the year and saved in a netcdf file.
 
         Parameters
         ----------
@@ -678,19 +1005,29 @@
         resolution : float, optional
             Desired pixel resolution, default is the DEM resolution.
         atmos_transmissivity : float, optional
             Mean clear-sky atmospheric transmissivity, default is 0.75
             (value taken in Hock 1999)
         steps_per_hour : int, optional
             Number of steps per hour to compute the potential radiation, default is 4.
+        with_cast_shadows : bool, optional
+            If True, the cast shadows are taken into account. Default is True.
 
         Returns
         -------
         The daily mean potential clear-sky direct solar radiation
         at the DEM surface [W/m²]
+
+        Notes
+        -----
+        This function is based on the R package TopoSol, authored by Matthew Olson.
+
+        References
+        ----------
+        - Original R package: https://github.com/mattols/TopoSol
         """
         # Resample the DEM and calculate the slope and aspect
         dem, masked_dem_data, slope, aspect = (
             self.resample_dem_and_calculate_slope_aspect(resolution, output_path))
         n_rows = slope.shape[0]
         n_cols = slope.shape[1]
 
@@ -698,86 +1035,60 @@
         day_of_year = np.arange(1, 367)
 
         # Get some catchment attributes
         mean_elevation = self.get_mean_elevation()
         mean_lat, _ = self._extract_unit_mean_lat_lon(self.masked_dem_data)
         lat_rad = mean_lat * TO_RAD
 
-        # Normalized day of the year
-        # '(jd-172)' calculates the number of days that have passed since the summer
-        # solstice (around June 21st), which is day 172 in a non-leap year.
-        # '(360*(jd-172))/365' normalizes this count to a value representing the
-        # position in the orbit of the Earth around the Sun (in degrees).
-        ndy = ((360 * (day_of_year - 172)) / 365)
+        # Compute the solar declination
+        solar_declin = self.get_solar_declination_rad(day_of_year)
 
-        # The solar Declination is the angle between the rays of the Sun and the
-        # plane of the Earth's equator. It represents how much the sun is
-        # tilted towards or away from the observer's latitude.
-        # The cos(...) function is applied to the normalized day of the year. It
-        # produces values between -1 and 1, representing the variation in solar
-        # declination throughout the year. The constant factor 23.45 represents the
-        # tilt of the Earth's axis relative to its orbital plane. This tilt causes the
-        # variation in the angle of the sun's rays reaching different latitudes
-        # on Earth.
-        solar_declin = 23.45 * np.cos(ndy * TO_RAD) * TO_RAD
+        # Compute the hour angle starting value
+        ha_limit = self.get_solar_hour_angle_limit(solar_declin, lat_rad)
 
-        # The hour angle is the angular distance between the sun and the observer's
-        # meridian. It is typically measured in degrees. The tangent of
-        # solar_declin/lat_rad represents the ratio of the opposite side
-        # (vertical component of the sun's rays) to the adjacent side (horizontal
-        # component). It helps capture how much the sun/the observer's location is
-        # tilted north or south relative to the equator. The negative sign is applied
-        # because the Hour Angle is negative in the morning and positive in the
-        # afternoon.
-        hour_angle = np.arccos(-np.tan(solar_declin) * np.tan(lat_rad))
-
-        # Time intervals (360°/24h = 15° per hour, then divided by the number of steps
-        # per hour)
-        time_interval = (15/steps_per_hour) * TO_RAD
+        # Time intervals (360°/24h = 15° per hour, divided by the # of steps / hour)
+        time_interval = (15 / steps_per_hour) * TO_RAD
 
         # Create array for the daily potential radiation
         daily_radiation = np.full((len(day_of_year), n_rows, n_cols), np.nan)
 
         # Loop over the days of the year
         for i in range(len(day_of_year)):
             # Print every 10 days
             if day_of_year[i] % 10 == 0:
                 print('Computing radiation for day', day_of_year[i])
 
             # List of hour angles throughout the day.
-            ha_list = np.arange(-hour_angle[i], hour_angle[i] + time_interval,
+            ha_list = np.arange(-ha_limit[i], ha_limit[i] + time_interval,
                                 time_interval)
 
-            # The Solar zenith (IQBAL 2012) is the angle between the sun and the
-            # vertical (zenith) position directly above the observer. The result is
-            # expressed in degrees. The calculation involves trigonometric functions
-            # to account for the observer's latitude, the solar declination, and the
-            # position of the sun in the sky (represented by the Hour Angles).
-            zenith = np.arccos((np.sin(lat_rad) * np.sin(solar_declin[i])) +
-                               (np.cos(lat_rad) * np.cos(solar_declin[i]) *
-                                np.cos(ha_list))) * TO_DEG
-
-            # Azimuth with negative values before solar noon and positive
-            # ones after solar noon. Solar noon is defined by the change in sign of
-            # the hour angle (negative in the morning, positive in the afternoon).
-            # From https://www.astrolabe-science.fr/diagramme-solaire-azimut-hauteur
-            azimuth = np.degrees(np.arctan(np.sin(ha_list) / (
-                    np.sin(lat_rad) * np.cos(ha_list) -
-                    np.cos(lat_rad) * np.tan(solar_declin[i]))))
-            azimuth[np.where((azimuth < 0) & (ha_list > 0))] += 180
-            azimuth[np.where((azimuth > 0) & (ha_list < 0))] -= 180
+            # Compute the zenith and azimuth
+            zenith = self.get_solar_zenith(ha_list, lat_rad, solar_declin[i])
+            azimuth = self.get_solar_azimuth_to_south(ha_list, lat_rad, solar_declin[i])
 
             # Potential radiation over the time intervals
             inter_pot_radiation = np.full((len(ha_list), n_rows, n_cols), np.nan)
             for j in range(len(zenith)):
+                # Shorten computation time, because if zenith >= 90 : no irradiation.
+                if zenith[j] >= 90:
+                    inter_pot_radiation[j, :, :] = np.zeros_like(zenith[j])
+                    continue
+
                 incidence_angle = self._calculate_angle_of_incidence(
                     zenith[j], slope, azimuth[j], aspect)
                 potential_radiation = self._calculate_radiation_hock_equation(
                     mean_elevation, atmos_transmissivity, day_of_year[i],
                     zenith[j], incidence_angle)
+
+                # Account for cast shadows
+                if with_cast_shadows:
+                    cast_shadows = self.calculate_cast_shadows(
+                        dem, masked_dem_data, zenith[j], azimuth[j], mean_lat)
+                    potential_radiation = potential_radiation * cast_shadows
+
                 inter_pot_radiation[j, :, :] = potential_radiation.copy()
 
             with warnings.catch_warnings():
                 # This function throws a warning for the first slides of nanmean,
                 # it is normal and due to the NaN bands at the sides of the
                 # slope rasters, etc.
                 warnings.filterwarnings(action='ignore', message='Mean of empty slice')
@@ -786,14 +1097,22 @@
 
         # Mean annual potential radiation
         mean_annual_radiation = np.full((n_rows, n_cols), np.nan)
         mean_annual_radiation[:, :] = np.nanmean(daily_radiation, axis=0)
         self.upscale_and_save_mean_annual_radiation_rasters(
             mean_annual_radiation, dem, output_path)
 
+        # Put the mask back on (we need the surrounding topography in the steps before)
+        # And make sure the padding lines are also set to nans and not 0
+        mean_annual_radiation[np.isnan(masked_dem_data)] = np.nan
+        mean_annual_radiation[0, :] = np.nan
+        mean_annual_radiation[-1, :] = np.nan
+        mean_annual_radiation[:, 0] = np.nan
+        mean_annual_radiation[:, -1] = np.nan
+
         # Save the daily potential radiation to a netcdf file
         self._save_potential_radiation_netcdf(
             daily_radiation, dem, masked_dem_data, day_of_year, output_path)
 
         # If DEM is the downsampled one, close it
         if dem.res[0] != self.get_dem_x_resolution():
             dem.close()
@@ -1021,14 +1340,28 @@
 
         Returns
         -------
         The DEM pixel area.
         """
         return self.get_dem_x_resolution() * self.get_dem_y_resolution()
 
+    def get_dem_mean_lat_lon(self):
+        # Central coordinates of the catchment
+        mean_x = self.dem.bounds[0] + (self.dem.bounds[2] - self.dem.bounds[0]) / 2
+        if self.dem.bounds[3] > self.dem.bounds[1]:
+            mean_y = self.dem.bounds[1] + (self.dem.bounds[3] - self.dem.bounds[1]) / 2
+        else:
+            mean_y = self.dem.bounds[3] + (self.dem.bounds[1] - self.dem.bounds[3]) / 2
+
+        # Get the mean coordinates of the unit in lat/lon
+        transformer = hb.pyproj.Transformer.from_crs(self.crs, 4326, always_xy=True)
+        mean_lon, mean_lat = transformer.transform(mean_x, mean_y)
+
+        return mean_lat, mean_lon
+
     def create_dem_pixel_geometry(self, i, j):
         """
         Create a shapely geometry of the DEM pixel.
 
         Parameters
         ----------
         i : int
```

### Comparing `hydrobricks-0.7.0/python/src/hydrobricks/constants.py` & `hydrobricks-0.7.1/python/src/hydrobricks/constants.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.0/python/src/hydrobricks/forcing.py` & `hydrobricks-0.7.1/python/src/hydrobricks/forcing.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from enum import auto
 
 import numpy as np
 import pandas as pd
 from cftime import num2date
 
 import hydrobricks as hb
+from hydrobricks.constants import TO_RAD
 
 from .time_series import TimeSeries1D, TimeSeries2D
 
 
 class Forcing:
     """Class for forcing data"""
 
@@ -589,31 +590,31 @@
         use_unit_elevation = False
         use_unit_latitude = False
         if 'elevation' in use:
             use_unit_elevation = True
         if 'latitude' in use or 'lat' in use:
             # If latitude provided in the arguments
             if 'latitude' in kwargs:
-                pyet_args['lat'] = hb.pyet.deg_to_rad(kwargs['latitude'])
+                pyet_args['lat'] = kwargs['latitude'] * TO_RAD
             elif 'lat' in kwargs:
-                pyet_args['lat'] = hb.pyet.deg_to_rad(kwargs['lat'])
+                pyet_args['lat'] = kwargs['lat'] * TO_RAD
             else:
                 use_unit_latitude = True
 
         use = self._remove_lat_elevation_options(use)
         self._check_variables_available(use)
 
         # Loop over the hydro units to compute the PET (pyet xarray implementation is
         # not working as expected in multiplicative operations)
         pet = np.zeros((len(self.data2D.time), len(self.hydro_units)))
         for i_unit, unit in self.hydro_units.iterrows():
             if use_unit_elevation:
                 pyet_args['elevation'] = unit['elevation'].values
             if use_unit_latitude:
-                pyet_args['lat'] = hb.pyet.deg_to_rad(unit['latitude'].values)
+                pyet_args['lat'] = unit['latitude'].values * TO_RAD
             pyet_args = self._set_pyet_variables_data(pyet_args, use, i_unit)
             pet[:, i_unit] = self._compute_pet(method, pyet_args)
 
         # Store outputs
         if self.Variable.PET not in self.data2D.data_name:
             self.data2D.data.append(pet)
             self.data2D.data_name.append(self.Variable.PET)
```

### Comparing `hydrobricks-0.7.0/python/src/hydrobricks/hydro_units.py` & `hydrobricks-0.7.1/python/src/hydrobricks/hydro_units.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,26 +274,26 @@
             if prop[0] in ['id', 'area']:
                 continue
             if 'fraction-' in prop[0]:
                 continue
             properties.append(prop[0])
 
         for _, row in self.hydro_units.iterrows():
-            self.settings.add_hydro_unit(int(row['id'].values),
-                                         float(row['area'].values))
+            self.settings.add_hydro_unit(int(row['id'].values[0]),
+                                         float(row['area'].values[0]))
             for prop in properties:
                 if isinstance(row[prop].values[0], str):
                     self.settings.add_hydro_unit_property_str(prop, row[prop].values[0])
                 else:
                     unit = self._get_unit(row[prop])
                     self.settings.add_hydro_unit_property_double(
-                        prop, float(row[prop].values), unit)
+                        prop, float(row[prop].values[0]), unit)
             for cover_type, cover_name in zip(self.land_cover_types,
                                               self.land_cover_names):
-                fraction = float(row[self.prefix_fraction + cover_name].values)
+                fraction = float(row[self.prefix_fraction + cover_name].values[0])
                 self.settings.add_land_cover(cover_name, cover_type, fraction)
 
     @staticmethod
     def _check_column_names(file_content):
         # Rename unnamed columns to 'No Unit'
         new_column_names = []
         for i, col in enumerate(file_content.columns):
```

### Comparing `hydrobricks-0.7.0/python/src/hydrobricks/models/model.py` & `hydrobricks-0.7.1/python/src/hydrobricks/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,15 +308,17 @@
             from the specified warmup period (as is done automatically during
             calibration).
 
         Returns
         -------
         The value of the selected metric.
         """
-        return hb.evaluate(self.get_outlet_discharge()[warmup:], observations[warmup:], metric)
+        return hb.evaluate(self.get_outlet_discharge()[warmup:],
+                           observations[warmup:],
+                           metric)
 
     def generate_parameters(self):
         ps = hb.ParameterSet()
         ps.generate_parameters(self.land_cover_types, self.land_cover_names,
                                self.options, self.structure)
 
         for alias_key, alias_value in self.parameter_aliases.items():
```

### Comparing `hydrobricks-0.7.0/python/src/hydrobricks/models/model_settings.py` & `hydrobricks-0.7.1/python/src/hydrobricks/models/model_settings.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.0/python/src/hydrobricks/models/socont.py` & `hydrobricks-0.7.1/python/src/hydrobricks/models/socont.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.0/python/src/hydrobricks/observations.py` & `hydrobricks-0.7.1/python/src/hydrobricks/observations.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.0/python/src/hydrobricks/parameters.py` & `hydrobricks-0.7.1/python/src/hydrobricks/parameters.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.0/python/src/hydrobricks/plotting.py` & `hydrobricks-0.7.1/python/src/hydrobricks/plotting.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.0/python/src/hydrobricks/results.py` & `hydrobricks-0.7.1/python/src/hydrobricks/results.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.0/python/src/hydrobricks/time_series.py` & `hydrobricks-0.7.1/python/src/hydrobricks/time_series.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.0/python/src/hydrobricks/trainer.py` & `hydrobricks-0.7.1/python/src/hydrobricks/trainer.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.0/python/src/hydrobricks/units.py` & `hydrobricks-0.7.1/python/src/hydrobricks/units.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.0/python/src/hydrobricks/utils.py` & `hydrobricks-0.7.1/python/src/hydrobricks/utils.py`

 * *Files identical despite different names*

### Comparing `hydrobricks-0.7.0/setup.py` & `hydrobricks-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 # Read the contents of the README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "python" / "README.md").read_text()
 
 # Setup
 setup(
     name="hydrobricks",
-    version="0.7.0",
+    version="0.7.1",
     author="Pascal Horton",
     author_email="pascal.horton@unibe.ch",
     description="A modular hydrological modelling framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     ext_modules=[CMakeExtension("_hydrobricks")],
     cmdclass={"build_ext": CMakeBuild},
```

