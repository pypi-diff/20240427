# Comparing `tmp/arcade_accelerate-1.0.1.tar.gz` & `tmp/arcade_accelerate-1.0.2.tar.gz`

## Comparing `arcade_accelerate-1.0.1.tar` & `arcade_accelerate-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 arcade_accelerate-1.0.1/Cargo.toml
--rw-r--r--   0     1001      127     1458 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     4138 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/.github/workflows/release.yml
--rw-r--r--   0     1001      127      713 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/.gitignore
--rw-r--r--   0     1001      127     2042 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/CONTRIBUTING.md
--rw-r--r--   0     1001      127     1089 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/LICENSE
--rw-r--r--   0     1001      127      448 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/Makefile
--rw-r--r--   0     1001      127     1716 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/README.md
--rw-r--r--   0     1001      127      147 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/benchmark/__init__.py
--rw-r--r--   0     1001      127     1116 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/benchmark/__main__.py
--rw-r--r--   0     1001      127     2605 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/benchmark/graph.py
--rw-r--r--   0     1001      127     5387 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/benchmark/manager.py
--rw-r--r--   0     1001      127        0 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/benchmark/tests/__init__.py
--rw-r--r--   0     1001      127       25 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/benchmark/tests/arcade/__init__.py
--rw-r--r--   0     1001      127     3638 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/benchmark/tests/arcade/collision.py
--rw-r--r--   0     1001      127       25 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/benchmark/tests/arcade_accelerate/__init__.py
--rw-r--r--   0     1001      127     3717 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/benchmark/tests/arcade_accelerate/collision.py
--rw-r--r--   0     1001      127     3875 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/benchmark/tests/base.py
--rw-r--r--   0     1001      127     2507 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/benchmark/timing.py
--rw-r--r--   0     1001      127     2836 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/python/arcade_accelerate/__init__.py
--rw-r--r--   0     1001      127     1759 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/python/arcade_accelerate/module_patcher.py
--rw-r--r--   0     1001      127     9949 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/src/geometry.rs
--rw-r--r--   0     1001      127    11257 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/src/hitbox.rs
--rw-r--r--   0     1001      127     2010 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/src/lib.rs
--rw-r--r--   0     1001      127    11715 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/src/math.rs
--rw-r--r--   0     1001      127     4495 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/src/sprite_list.rs
--rw-r--r--   0     1001      127     1402 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/tests/perf_compare.py
--rw-r--r--   0     1001      127       11 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/tests/requirements-linting.txt
--rw-r--r--   0     1001      127     9674 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/Cargo.lock
--rw-r--r--   0     1001      127      886 2024-03-03 06:48:04.000000 arcade_accelerate-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2513 1970-01-01 00:00:00.000000 arcade_accelerate-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 arcade_accelerate-1.0.2/Cargo.toml
+-rw-r--r--   0     1001      127     1458 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     4138 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/.github/workflows/release.yml
+-rw-r--r--   0     1001      127      713 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/.gitignore
+-rw-r--r--   0     1001      127     2042 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0     1001      127     1089 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/LICENSE
+-rw-r--r--   0     1001      127      448 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/Makefile
+-rw-r--r--   0     1001      127     1716 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/README.md
+-rw-r--r--   0     1001      127      147 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/benchmark/__init__.py
+-rw-r--r--   0     1001      127     1116 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/benchmark/__main__.py
+-rw-r--r--   0     1001      127     2605 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/benchmark/graph.py
+-rw-r--r--   0     1001      127     5387 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/benchmark/manager.py
+-rw-r--r--   0     1001      127        0 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/benchmark/tests/__init__.py
+-rw-r--r--   0     1001      127       25 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/benchmark/tests/arcade/__init__.py
+-rw-r--r--   0     1001      127     3638 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/benchmark/tests/arcade/collision.py
+-rw-r--r--   0     1001      127       25 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/benchmark/tests/arcade_accelerate/__init__.py
+-rw-r--r--   0     1001      127     3717 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/benchmark/tests/arcade_accelerate/collision.py
+-rw-r--r--   0     1001      127     3875 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/benchmark/tests/base.py
+-rw-r--r--   0     1001      127     2507 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/benchmark/timing.py
+-rw-r--r--   0     1001      127     2984 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/python/arcade_accelerate/__init__.py
+-rw-r--r--   0     1001      127     1759 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/python/arcade_accelerate/module_patcher.py
+-rw-r--r--   0     1001      127     9949 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/src/geometry.rs
+-rw-r--r--   0     1001      127    11257 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/src/hitbox.rs
+-rw-r--r--   0     1001      127     2137 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/src/lib.rs
+-rw-r--r--   0     1001      127    13072 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/src/math.rs
+-rw-r--r--   0     1001      127     4495 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/src/sprite_list.rs
+-rw-r--r--   0     1001      127     1402 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/tests/perf_compare.py
+-rw-r--r--   0     1001      127       11 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/tests/requirements-linting.txt
+-rw-r--r--   0     1001      127     9674 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/Cargo.lock
+-rw-r--r--   0     1001      127      886 2024-04-27 06:53:28.000000 arcade_accelerate-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2513 1970-01-01 00:00:00.000000 arcade_accelerate-1.0.2/PKG-INFO
```

### Comparing `arcade_accelerate-1.0.1/.github/workflows/CI.yml` & `arcade_accelerate-1.0.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `arcade_accelerate-1.0.1/.github/workflows/release.yml` & `arcade_accelerate-1.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `arcade_accelerate-1.0.1/.gitignore` & `arcade_accelerate-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `arcade_accelerate-1.0.1/CONTRIBUTING.md` & `arcade_accelerate-1.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `arcade_accelerate-1.0.1/LICENSE` & `arcade_accelerate-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arcade_accelerate-1.0.1/README.md` & `arcade_accelerate-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `arcade_accelerate-1.0.1/benchmark/__main__.py` & `arcade_accelerate-1.0.2/benchmark/__main__.py`

 * *Files identical despite different names*

### Comparing `arcade_accelerate-1.0.1/benchmark/graph.py` & `arcade_accelerate-1.0.2/benchmark/graph.py`

 * *Files identical despite different names*

### Comparing `arcade_accelerate-1.0.1/benchmark/manager.py` & `arcade_accelerate-1.0.2/benchmark/manager.py`

 * *Files identical despite different names*

### Comparing `arcade_accelerate-1.0.1/benchmark/tests/arcade/collision.py` & `arcade_accelerate-1.0.2/benchmark/tests/arcade/collision.py`

 * *Files identical despite different names*

### Comparing `arcade_accelerate-1.0.1/benchmark/tests/arcade_accelerate/collision.py` & `arcade_accelerate-1.0.2/benchmark/tests/arcade_accelerate/collision.py`

 * *Files identical despite different names*

### Comparing `arcade_accelerate-1.0.1/benchmark/tests/base.py` & `arcade_accelerate-1.0.2/benchmark/tests/base.py`

 * *Files identical despite different names*

### Comparing `arcade_accelerate-1.0.1/benchmark/timing.py` & `arcade_accelerate-1.0.2/benchmark/timing.py`

 * *Files identical despite different names*

### Comparing `arcade_accelerate-1.0.1/python/arcade_accelerate/__init__.py` & `arcade_accelerate-1.0.2/python/arcade_accelerate/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,16 @@
     )
 
 
 def patch_math(patches):
     patches["arcade.math"].rotate_point = arcade_accelerate.rotate_point
     patches["arcade.math"].clamp = arcade_accelerate.clamp
     patches["arcade.math"].lerp = arcade_accelerate.lerp
-    patches["arcade.math"].lerp_vec = arcade_accelerate.lerp_vec
+    patches["arcade.math"].lerp_2d = arcade_accelerate.lerp_2d
+    patches["arcade.math"].lerp_3d = arcade_accelerate.lerp_3d
     patches["arcade.math"].lerp_angle = arcade_accelerate.lerp_angle
     patches["arcade.math"].get_distance = arcade_accelerate.get_distance
     patches["arcade.math"].get_angle_degrees = arcade_accelerate.get_angle_degrees
     patches["arcade.math"].get_angle_radians = arcade_accelerate.get_angle_radians
     patches["arcade.math"].rand_in_rect = arcade_accelerate.rand_in_rect
     patches["arcade.math"].rand_in_circle = arcade_accelerate.rand_in_circle
     patches["arcade.math"].rand_on_circle = arcade_accelerate.rand_on_circle
@@ -49,14 +50,15 @@
     patches["arcade.math"].rand_angle_spread_deg = (
         arcade_accelerate.rand_angle_spread_deg
     )
     patches["arcade.math"].rand_vec_degree_spread = (
         arcade_accelerate.rand_vec_degree_spread
     )
     patches["arcade.math"].rand_vec_magnitude = arcade_accelerate.rand_vec_magnitude
+    patches["arcade.math"].quaternion_rotation = arcade_accelerate.quaternion_rotation
 
 
 def patch_geometry(patches):
     patches["arcade.geometry"].are_polygons_intersecting = (
         arcade_accelerate.are_polygons_intersecting
     )
     patches["arcade.geometry"].is_point_in_box = arcade_accelerate.is_point_in_box
```

### Comparing `arcade_accelerate-1.0.1/python/arcade_accelerate/module_patcher.py` & `arcade_accelerate-1.0.2/python/arcade_accelerate/module_patcher.py`

 * *Files identical despite different names*

### Comparing `arcade_accelerate-1.0.1/src/geometry.rs` & `arcade_accelerate-1.0.2/src/geometry.rs`

 * *Files identical despite different names*

### Comparing `arcade_accelerate-1.0.1/src/hitbox.rs` & `arcade_accelerate-1.0.2/src/hitbox.rs`

 * *Files identical despite different names*

### Comparing `arcade_accelerate-1.0.1/src/lib.rs` & `arcade_accelerate-1.0.2/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -16,27 +16,29 @@
 #[pymodule]
 fn arcade_accelerate(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<hitbox::HitBox>()?;
     m.add_class::<hitbox::RotatableHitBox>()?;
     m.add_function(wrap_pyfunction!(math::rotate_point, m)?)?;
     m.add_function(wrap_pyfunction!(math::clamp, m)?)?;
     m.add_function(wrap_pyfunction!(math::lerp, m)?)?;
-    m.add_function(wrap_pyfunction!(math::lerp_vec, m)?)?;
+    m.add_function(wrap_pyfunction!(math::lerp_2d, m)?)?;
+    m.add_function(wrap_pyfunction!(math::lerp_3d, m)?)?;
     m.add_function(wrap_pyfunction!(math::lerp_angle, m)?)?;
     m.add_function(wrap_pyfunction!(math::get_distance, m)?)?;
     m.add_function(wrap_pyfunction!(math::get_angle_degrees, m)?)?;
     m.add_function(wrap_pyfunction!(math::get_angle_radians, m)?)?;
     m.add_function(wrap_pyfunction!(math::rand_in_rect, m)?)?;
     m.add_function(wrap_pyfunction!(math::rand_in_circle, m)?)?;
     m.add_function(wrap_pyfunction!(math::rand_on_circle, m)?)?;
     m.add_function(wrap_pyfunction!(math::rand_on_line, m)?)?;
     m.add_function(wrap_pyfunction!(math::rand_angle_360_deg, m)?)?;
     m.add_function(wrap_pyfunction!(math::rand_angle_spread_deg, m)?)?;
     m.add_function(wrap_pyfunction!(math::rand_vec_degree_spread, m)?)?;
     m.add_function(wrap_pyfunction!(math::rand_vec_magnitude, m)?)?;
+    m.add_function(wrap_pyfunction!(math::quaternion_rotation, m)?)?;
     m.add_function(wrap_pyfunction!(geometry::are_polygons_intersecting, m)?)?;
     m.add_function(wrap_pyfunction!(geometry::is_point_in_polygon, m)?)?;
     m.add_function(wrap_pyfunction!(geometry::is_point_in_box, m)?)?;
     m.add_function(wrap_pyfunction!(geometry::get_triangle_orientation, m)?)?;
     m.add_function(wrap_pyfunction!(geometry::are_lines_intersecting, m)?)?;
     m.add_function(wrap_pyfunction!(
         sprite_list::check_for_collision_with_list,
```

### Comparing `arcade_accelerate-1.0.1/src/math.rs` & `arcade_accelerate-1.0.2/src/math.rs`

 * *Files 8% similar despite different names*

```diff
@@ -37,19 +37,28 @@
 
 #[pyfunction]
 pub fn lerp(v1: f32, v2: f32, u: f32) -> f32 {
     v1 + ((v2 - v1) * u)
 }
 
 #[pyfunction]
-pub fn lerp_vec(v1: (f32, f32), v2: (f32, f32), u: f32) -> (f32, f32) {
+pub fn lerp_2d(v1: (f32, f32), v2: (f32, f32), u: f32) -> (f32, f32) {
     (lerp(v1.0, v2.0, u), lerp(v1.1, v2.1, u))
 }
 
 #[pyfunction]
+pub fn lerp_3d(v1: (f32, f32, f32), v2: (f32, f32, f32), u: f32) -> (f32, f32, f32) {
+    (
+        lerp(v1.0, v2.0, u),
+        lerp(v1.1, v2.1, u),
+        lerp(v1.2, v2.2, u),
+    )
+}
+
+#[pyfunction]
 pub fn lerp_angle(start_angle: f32, end_angle: f32, u: f32) -> f32 {
     let temp_start = start_angle % 360.0;
     let mut temp_end = end_angle % 360.0;
 
     while temp_start - temp_end > 180.0 {
         temp_end += 360.0;
     }
@@ -126,15 +135,15 @@
 }
 
 #[pyfunction]
 pub fn rand_on_line(pos1: (f32, f32), pos2: (f32, f32)) -> (f32, f32) {
     let mut rng = thread_rng();
     let u: f32 = rng.gen_range(0.0..1.0);
 
-    lerp_vec(pos1, pos2, u)
+    lerp_2d(pos1, pos2, u)
 }
 
 #[pyfunction]
 pub fn rand_angle_360_deg() -> f32 {
     let mut rng = thread_rng();
     let random_angle: f32 = rng.gen_range(0.0..360.0);
 
@@ -160,14 +169,37 @@
 pub fn rand_vec_magnitude(angle: f32, lo_magnitude: f32, hi_magnitude: f32) -> (f32, f32) {
     let mut rng = thread_rng();
     let mag = rng.gen_range(lo_magnitude..hi_magnitude);
     let vel = _Vec2::from_polar(angle, mag);
     vel.as_tuple()
 }
 
+#[pyfunction]
+pub fn quaternion_rotation(
+    axis: (f32, f32, f32),
+    vector: (f32, f32, f32),
+    angle: f32,
+) -> (f32, f32, f32) {
+    let angle_rads = -angle.to_radians();
+    let (c2, s2) = (f32::cos(angle_rads / 2.0), f32::sin(angle_rads / 2.0));
+
+    let (q0, q1, q2, q3) = (c2, s2 * axis.0, s2 * axis.1, s2 * axis.2);
+    let (q0_2, q1_2, q2_2, q3_2) = (q0.powi(2), q1.powi(2), q2.powi(2), q3.powi(2));
+    let (q01, q02, q03, q12, q13, q23) = (q0 * q1, q0 * q2, q0 * q3, q1 * q2, q1 * q3, q2 * q3);
+
+    let x = vector.0 * (q0_2 + q1_2 - q2_2 - q3_2)
+        + 2.0 * (vector.1 * (q12 - q03) + vector.2 * (q02 + q13));
+    let y = vector.1 * (q0_2 - q1_2 + q2_2 - q3_2)
+        + 2.0 * (vector.0 * (q03 + q12) + vector.2 * (q23 - q01));
+    let z = vector.2 * (q0_2 - q1_2 - q2_2 + q3_2)
+        + 2.0 * (vector.0 * (q13 + q02) + vector.1 * (q01 + q23));
+
+    (x, y, z)
+}
+
 // This is only a subset of _Vec2 methods defined in arcade.math.py
 struct _Vec2 {
     x: f32,
     y: f32,
 }
 #[allow(dead_code)]
 impl _Vec2 {
@@ -258,23 +290,32 @@
         assert_eq!(result, 0.8);
 
         result = lerp(2.0, 4.0, 0.5);
         assert_eq!(result, 3.0);
     }
 
     #[test]
-    fn test_lerp_vec() {
-        let mut result = lerp_vec((0.0, 2.0), (8.0, 4.0), 0.25);
+    fn test_lerp_2d() {
+        let mut result = lerp_2d((0.0, 2.0), (8.0, 4.0), 0.25);
         assert_eq!(result, (2.0, 2.5));
 
-        result = lerp_vec((0.0, 2.0), (8.0, 4.0), -0.25);
+        result = lerp_2d((0.0, 2.0), (8.0, 4.0), -0.25);
         assert_eq!(result, (-2.0, 1.5));
     }
 
     #[test]
+    fn test_lerp_3d() {
+        let mut result = lerp_3d((0.0, 2.0, 4.0), (8.0, 4.0, 8.0), 0.25);
+        assert_eq!(result, (2.0, 2.5, 5.0));
+
+        result = lerp_3d((0.0, 2.0, 4.0), (8.0, 4.0, 8.0), -0.25);
+        assert_eq!(result, (-2.0, 1.5, 3.0));
+    }
+
+    #[test]
     fn test_lerp_angle_normal() {
         //normal
         let mut result = lerp_angle(0.0, 90.0, 0.5);
         assert_eq!(result, 45.0);
 
         //backwards
         result = lerp_angle(90.0, 0.0, 0.5);
```

### Comparing `arcade_accelerate-1.0.1/src/sprite_list.rs` & `arcade_accelerate-1.0.2/src/sprite_list.rs`

 * *Files identical despite different names*

### Comparing `arcade_accelerate-1.0.1/tests/perf_compare.py` & `arcade_accelerate-1.0.2/tests/perf_compare.py`

 * *Files identical despite different names*

### Comparing `arcade_accelerate-1.0.1/Cargo.lock` & `arcade_accelerate-1.0.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "arcade-accelerate"
-version = "1.0.1"
+version = "1.0.2"
 dependencies = [
  "float_eq",
  "pyo3",
  "rand",
 ]
 
 [[package]]
```

### Comparing `arcade_accelerate-1.0.1/pyproject.toml` & `arcade_accelerate-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.4.0,<1.5.0"]
 build-backend = "maturin"
 
 [project]
 name = "arcade-accelerate"
-version = "1.0.1"
+version = "1.0.2"
 description = "A companion library for Arcade providing accelerated Rust functions"
 readme = "README.md"
 authors = [
     {name="Darren Eberly", email="Daren.Eberly@gmail.com"}
 ]
 maintainers = [
     {name="Darren Eberly", email="Darren.Eberly@gmail.com"}
```

### Comparing `arcade_accelerate-1.0.1/PKG-INFO` & `arcade_accelerate-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcade-accelerate
-Version: 1.0.1
+Version: 1.0.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: ruff ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: matplotlib ; extra == 'dev'
 Requires-Dist: seaborn ; extra == 'dev'
```

