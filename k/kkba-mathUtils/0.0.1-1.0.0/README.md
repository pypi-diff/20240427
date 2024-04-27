# Comparing `tmp/kkba_mathutils-0.0.1.tar.gz` & `tmp/kkba_mathutils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkba_mathutils-0.0.1.tar", last modified: Fri Apr 19 16:51:55 2024, max compression
+gzip compressed data, was "kkba_mathutils-1.0.0.tar", last modified: Sat Apr 27 17:01:46 2024, max compression
```

## Comparing `kkba_mathutils-0.0.1.tar` & `kkba_mathutils-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxr-x   0 brayanarmel  (1000) brayanarmel  (1000)        0 2024-04-19 16:51:55.518507 kkba_mathutils-0.0.1/
--rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)     1073 2024-04-19 16:18:16.000000 kkba_mathutils-0.0.1/LICENCE
--rw-r--r--   0 brayanarmel  (1000) brayanarmel  (1000)      560 2024-04-19 16:51:55.518507 kkba_mathutils-0.0.1/PKG-INFO
--rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)      431 2024-04-19 16:32:38.000000 kkba_mathutils-0.0.1/README.md
-drwxrwxr-x   0 brayanarmel  (1000) brayanarmel  (1000)        0 2024-04-19 16:51:55.518507 kkba_mathutils-0.0.1/kkba_mathUtils/
--rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)        0 2024-04-19 14:27:48.000000 kkba_mathutils-0.0.1/kkba_mathUtils/__init__.py
--rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)     6384 2024-04-19 16:20:42.000000 kkba_mathutils-0.0.1/kkba_mathUtils/kkba_mathUtils.py
-drwxrwxr-x   0 brayanarmel  (1000) brayanarmel  (1000)        0 2024-04-19 16:51:55.518507 kkba_mathutils-0.0.1/kkba_mathUtils.egg-info/
--rw-r--r--   0 brayanarmel  (1000) brayanarmel  (1000)      560 2024-04-19 16:51:55.000000 kkba_mathutils-0.0.1/kkba_mathUtils.egg-info/PKG-INFO
--rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)      279 2024-04-19 16:51:55.000000 kkba_mathutils-0.0.1/kkba_mathUtils.egg-info/SOURCES.txt
--rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)        1 2024-04-19 16:51:55.000000 kkba_mathutils-0.0.1/kkba_mathUtils.egg-info/dependency_links.txt
--rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)       15 2024-04-19 16:51:55.000000 kkba_mathutils-0.0.1/kkba_mathUtils.egg-info/top_level.txt
--rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)      685 2024-04-19 16:48:21.000000 kkba_mathutils-0.0.1/pyproject.toml
--rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)       38 2024-04-19 16:51:55.518507 kkba_mathutils-0.0.1/setup.cfg
--rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)      363 2024-04-19 15:50:14.000000 kkba_mathutils-0.0.1/setup.py
-drwxrwxr-x   0 brayanarmel  (1000) brayanarmel  (1000)        0 2024-04-19 16:51:55.518507 kkba_mathutils-0.0.1/tests/
--rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)        0 2024-04-19 16:15:32.000000 kkba_mathutils-0.0.1/tests/test_myfunctions.py
+drwxrwxr-x   0 brayanarmel  (1000) brayanarmel  (1000)        0 2024-04-27 17:01:46.951839 kkba_mathutils-1.0.0/
+-rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)     1073 2024-04-19 16:18:16.000000 kkba_mathutils-1.0.0/LICENCE
+-rw-r--r--   0 brayanarmel  (1000) brayanarmel  (1000)      586 2024-04-27 17:01:46.951839 kkba_mathutils-1.0.0/PKG-INFO
+-rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)    11612 2024-04-27 16:50:05.000000 kkba_mathutils-1.0.0/README.md
+drwxrwxr-x   0 brayanarmel  (1000) brayanarmel  (1000)        0 2024-04-27 17:01:46.947839 kkba_mathutils-1.0.0/kkba_mathUtils/
+-rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)        0 2024-04-19 14:27:48.000000 kkba_mathutils-1.0.0/kkba_mathUtils/__init__.py
+-rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)     1529 2024-04-27 16:56:12.000000 kkba_mathutils-1.0.0/kkba_mathUtils/area.py
+-rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)       11 2024-04-27 16:56:12.000000 kkba_mathutils-1.0.0/kkba_mathUtils/converter.py
+-rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)     8932 2024-04-27 16:56:12.000000 kkba_mathutils-1.0.0/kkba_mathUtils/mathUtils.py
+-rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)      615 2024-04-27 15:23:45.000000 kkba_mathutils-1.0.0/kkba_mathUtils/mean.py
+-rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)      987 2024-04-27 16:56:12.000000 kkba_mathutils-1.0.0/kkba_mathUtils/perimeter.py
+drwxrwxr-x   0 brayanarmel  (1000) brayanarmel  (1000)        0 2024-04-27 17:01:46.951839 kkba_mathutils-1.0.0/kkba_mathUtils.egg-info/
+-rw-r--r--   0 brayanarmel  (1000) brayanarmel  (1000)      586 2024-04-27 17:01:46.000000 kkba_mathutils-1.0.0/kkba_mathUtils.egg-info/PKG-INFO
+-rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)      376 2024-04-27 17:01:46.000000 kkba_mathutils-1.0.0/kkba_mathUtils.egg-info/SOURCES.txt
+-rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)        1 2024-04-27 17:01:46.000000 kkba_mathutils-1.0.0/kkba_mathUtils.egg-info/dependency_links.txt
+-rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)       15 2024-04-27 17:01:46.000000 kkba_mathutils-1.0.0/kkba_mathUtils.egg-info/top_level.txt
+-rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)      714 2024-04-27 17:00:08.000000 kkba_mathutils-1.0.0/pyproject.toml
+-rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)       38 2024-04-27 17:01:46.951839 kkba_mathutils-1.0.0/setup.cfg
+-rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)      363 2024-04-27 16:56:12.000000 kkba_mathutils-1.0.0/setup.py
+drwxrwxr-x   0 brayanarmel  (1000) brayanarmel  (1000)        0 2024-04-27 17:01:46.951839 kkba_mathutils-1.0.0/tests/
+-rw-rw-r--   0 brayanarmel  (1000) brayanarmel  (1000)        0 2024-04-19 16:15:32.000000 kkba_mathutils-1.0.0/tests/test_myfunctions.py
```

### Comparing `kkba_mathutils-0.0.1/LICENCE` & `kkba_mathutils-1.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `kkba_mathutils-0.0.1/PKG-INFO` & `kkba_mathutils-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: kkba_mathUtils
-Version: 0.0.1
+Version: 1.0.0
 Summary: My basic mathematics Python library
 Author: Kuate Brayan
 Author-email: Kuate Brayan <brayanarmel@gmail.com>
-Project-URL: Homepage, https://github.com/KamgaBrayan/KKBA_BASIC_MATH_PYTHON_LIBRARY
-Keywords: mathematics,maths,mean,operations,gcd,arithmetic,quadratic
+Project-URL: Homepage, https://github.com/KamgaBrayan/KKBA_BASIC_MATH_PYTHON_LIBRARY/tree/main_pypi
+Keywords: mathematics,maths,mean,operations,area,perimeter,arithmetic,quadratic
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `kkba_mathutils-0.0.1/kkba_mathUtils/kkba_mathUtils.py` & `kkba_mathutils-1.0.0/kkba_mathUtils/mathUtils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,9 @@
 import math
-
-def mean_of_list(list):
-    return (1/len(list)) * sum(list)
-
-def harmonic_mean(list):
-    sum_liste = 0
-    for num in list:
-        sum_liste += (1/num)
-        
-    return len(list) / sum_liste
+from mean import mean_of_list
 
 def isbigprime(n):
     if n == 2 or n == 3:
         return True
     if n < 2 or n % 2 == 0:
         return False
     for i in range(3, int(math.sqrt(n)) + 1, 2):
@@ -188,31 +179,14 @@
         line = []
         for j in range(N):
             line.append(math.randint(inf, sup))
         matrix.append(line)
 
     return matrix
 
-def area_circle(rayon):
-    return 2*math.pi*rayon**2
-
-def circumference_circle(rayon):
-    return 2*math.pi*rayon
-
-def perimeter_triangle(ab,bc,ca):
-    return ab+bc+ca
-
-def area_triangle(b, h):
-    return (b+h)/2
-
-def perimeter_rectangle(length, width):
-    return 2*length + 2*width
-
-def area_rectangle(lenght, width):
-    return lenght*width
 
 def unique_elements(liste):
     if len(liste) == len(list(set(liste))):
         return True
 
     else:
         return False
@@ -271,22 +245,116 @@
     if x % y == 0:
         return y
 
     for k in range(y//2, 0, -1):
         if x % k == 0 and y % k == 0:
             return k
 
-def geometric(liste):
-    """Renvoie la moyenne géométrique des éléments d'une liste"""
-    product_list = 1
-    for nb in liste:
-        product_list *= nb
 
-    return product_list**(1/len(liste))
+# Function to calculate the area of a triangle using Heron's formula
+def herons_formula(a, b, c):
+    s = (a + b + c) / 2
+    area = math.sqrt(s * (s - a) * (s - b) * (s - c))
+    return area
+
+
+def hours_to_minutes(hours):
+    return hours * 60
+
+def hours_to_seconds(hours):
+    return hours * 3600
+
+# Function to convert minutes to hours
+def minutes_to_hours(minutes):
+    return minutes / 60
+
+# Function to convert minutes to seconds
+def minutes_to_seconds(minutes):
+    return minutes * 60
+
+def seconds_to_minutes(seconds):
+    return seconds / 60
+
+def seconds_to_hours(seconds):
+    return seconds / 3600
+
+# Function to find the equation of a line passing through two points
+def line_equation(point1, point2):
+    (x1, y1), (x2, y2) = point1, point2
+    m = (y2 - y1) / (x2 - x1)  # slope of the line
+    b = y1 - m * x1  # y-intercept
+    return f"y = {m}x + {b}"
+
+# Function to calculate the nth term of an arithmetic sequence
+def arithmetic_sequence_nth_term(a, d, n):
+    return a + (n - 1) * d
+
+# Function to calculate the sum of the first n terms of an arithmetic sequence
+def arithmetic_sequence_sum(a, d, n):
+    return n / 2 * (2 * a + (n - 1) * d)
+
+# Function to calculate the nth term of a geometric sequence
+def geometric_sequence_nth_term(a, r, n):
+    return a * r ** (n - 1)
+
+# Function to calculate the sum of the first n terms of a geometric sequence
+def geometric_sequence_sum(a, r, n):
+    if r == 1:
+        return a * n
+    else:
+        return a * (1 - r ** n) / (1 - r)
 
-def quadratic(liste):
-    """Renvoie la moyenne quadratique des éléments d'une liste"""
-    sum_liste = 0
-    for nb in liste:
-        sum_liste += nb**2
-    return math.sqrt(sum_liste/len(liste))
+# Function to calculate the nth Fibonacci number using Binet's formula
+def fibonacci_binet(n):
+    phi = (1 + math.sqrt(5)) / 2
+    return round((phi ** n - (-1 / phi) ** n) / math.sqrt(5))
+
+# Function to calculate the least common multiple (LCM)
+def lcm(x, y):
+    return abs(x * y) // gcd_euclid(x, y)
+
+# Function to check if a number is a palindrome
+def is_palindrome(n):
+    return str(n) == str(n)[::-1]
+
+# Function to calculate the distance between two points in 2D space
+def distance_between_points(point1, point2):
+    (x1, y1), (x2, y2) = point1, point2
+    return math.sqrt((x2 - x1) ** 2 + (y2 - y1) ** 2)
+
+# Function to calculate the factorial of a number
+def factorial(n):
+    if n == 0:
+        return 1
+    else:
+        return n * factorial(n - 1)
 
+# Function to calculate the n-th root of a number
+def nth_root(number, root):
+    return number ** (1 / root)
+
+# Function to calculate the angle between two vectors
+def angle_between_vectors(vector1, vector2):
+    dot_product = sum(a * b for a, b in zip(vector1, vector2))
+    magnitude1 = math.sqrt(sum(a ** 2 for a in vector1))
+    magnitude2 = math.sqrt(sum(b ** 2 for b in vector2))
+    return math.acos(dot_product / (magnitude1 * magnitude2))
+
+# Function to calculate the area of a regular polygon with n sides and side length s
+def regular_polygon_area(n, s):
+    return (n * s ** 2) / (4 * math.tan(math.pi / n))
+
+# Function to convert degrees to radians
+def degrees_to_radians(degrees):
+    return degrees * (math.pi / 180)
+
+# Function to convert radians to degrees
+def radians_to_degrees(radians):
+    return radians * (180 / math.pi)
+
+# Function to calculate the compound interest
+def compound_interest(principal, rate, times_compounded, years):
+    return principal * (1 + rate / times_compounded) ** (times_compounded * years)
+
+# Function to calculate the continuous compound interest
+def continuous_compound_interest(principal, rate, years):
+    return principal * math.exp(rate * years)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kkba_mathutils-0.0.1/kkba_mathUtils.egg-info/PKG-INFO` & `kkba_mathutils-1.0.0/kkba_mathUtils.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: kkba_mathUtils
-Version: 0.0.1
+Version: 1.0.0
 Summary: My basic mathematics Python library
 Author: Kuate Brayan
 Author-email: Kuate Brayan <brayanarmel@gmail.com>
-Project-URL: Homepage, https://github.com/KamgaBrayan/KKBA_BASIC_MATH_PYTHON_LIBRARY
-Keywords: mathematics,maths,mean,operations,gcd,arithmetic,quadratic
+Project-URL: Homepage, https://github.com/KamgaBrayan/KKBA_BASIC_MATH_PYTHON_LIBRARY/tree/main_pypi
+Keywords: mathematics,maths,mean,operations,area,perimeter,arithmetic,quadratic
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `kkba_mathutils-0.0.1/pyproject.toml` & `kkba_mathutils-1.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kkba_mathUtils"
-version = "0.0.1"
+version = "1.0.0"
 authors = [
   { name="Kuate Brayan", email="brayanarmel@gmail.com" },
 ]
 description = "My basic mathematics Python library"
 readme = {file = "README.txt", content-type = "text/markdown"}
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-keywords = ["mathematics", "maths", "mean", "operations", "gcd", "arithmetic", "quadratic"]
+keywords = ["mathematics", "maths", "mean", "operations", "area", "perimeter", "arithmetic", "quadratic"]
 
 [project.urls]
-Homepage = "https://github.com/KamgaBrayan/KKBA_BASIC_MATH_PYTHON_LIBRARY"
+Homepage = "https://github.com/KamgaBrayan/KKBA_BASIC_MATH_PYTHON_LIBRARY/tree/main_pypi"
```

