# Comparing `tmp/bucketed_scene_flow_eval-2.0.6.tar.gz` & `tmp/bucketed_scene_flow_eval-2.0.7.tar.gz`

## Comparing `bucketed_scene_flow_eval-2.0.6.tar` & `bucketed_scene_flow_eval-2.0.7.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/build_pypi.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/__init__.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/argoverse2/__init__.py
--rw-r--r--   0        0        0    22729 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_raw_data.py
--rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_scene_flow.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/argoverse2/av2_metacategories.py
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/argoverse2/dataset.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/argoverse2/symlink_camera_data.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/nuscenes/__init__.py
--rw-r--r--   0        0        0    10524 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_loader.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/waymoopen/__init__.py
--rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/waymoopen/dataset.py
--rw-r--r--   0        0        0     7237 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/waymoopen/waymo_supervised_flow.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datastructures/__init__.py
--rw-r--r--   0        0        0    10747 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datastructures/camera_projection.py
--rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datastructures/dataclasses.py
--rw-r--r--   0        0        0     7803 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datastructures/o3d_visualizer.py
--rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datastructures/pointcloud.py
--rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datastructures/rgb_image.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datastructures/se2.py
--rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datastructures/se3.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/eval/__init__.py
--rw-r--r--   0        0        0    13224 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/eval/base_per_frame_sceneflow_eval.py
--rw-r--r--   0        0        0    13693 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/eval/bucketed_epe.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/eval/eval.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/eval/threeway_epe.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/interfaces/__init__.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/interfaces/abstract_dataset.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/interfaces/abstract_sequence_loader.py
--rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/interfaces/base_dataset_abstract_seq_loader.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/utils/__init__.py
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/utils/loaders.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/tests/integration_tests.py
--rwxr-xr-x   0        0        0      144 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/tests/integration_tests.sh
--rwxr-xr-x   0        0        0     4217 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/tests/setup.sh
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/tests/datasets/argoverse2/av2_small_tests.py
--rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/tests/datasets/argoverse2/av2_tiny_tests.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/tests/datasets/nuscenes/nuscenes_tests.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/tests/datastructures/rgb.py
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/tests/eval/bucketed_epe.py
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/tests/eval/threeway_epe.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/.gitignore
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/LICENSE
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/README.md
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/pyproject.toml
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/build_pypi.sh
+-rw-r--r--   0        0        0    49683 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/deflowpp_differences.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/__init__.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/argoverse2/__init__.py
+-rw-r--r--   0        0        0    22729 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_raw_data.py
+-rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_scene_flow.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/argoverse2/av2_metacategories.py
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/argoverse2/dataset.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/argoverse2/symlink_camera_data.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/nuscenes/__init__.py
+-rw-r--r--   0        0        0    10524 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_loader.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/waymoopen/__init__.py
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/waymoopen/dataset.py
+-rw-r--r--   0        0        0     7237 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/waymoopen/waymo_supervised_flow.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datastructures/__init__.py
+-rw-r--r--   0        0        0    10747 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datastructures/camera_projection.py
+-rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datastructures/dataclasses.py
+-rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datastructures/o3d_visualizer.py
+-rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datastructures/pointcloud.py
+-rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datastructures/rgb_image.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datastructures/se2.py
+-rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datastructures/se3.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/eval/__init__.py
+-rw-r--r--   0        0        0    13346 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/eval/base_per_frame_sceneflow_eval.py
+-rw-r--r--   0        0        0    13693 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/eval/bucketed_epe.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/eval/eval.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/eval/threeway_epe.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/interfaces/__init__.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/interfaces/abstract_dataset.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/interfaces/abstract_sequence_loader.py
+-rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/interfaces/base_dataset_abstract_seq_loader.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/utils/__init__.py
+-rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/utils/loaders.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/tests/integration_tests.py
+-rwxr-xr-x   0        0        0      144 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/tests/integration_tests.sh
+-rwxr-xr-x   0        0        0     4217 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/tests/setup.sh
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/tests/datasets/argoverse2/av2_small_tests.py
+-rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/tests/datasets/argoverse2/av2_tiny_tests.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/tests/datasets/nuscenes/nuscenes_tests.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/tests/datastructures/rgb.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/tests/eval/bucketed_epe.py
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/tests/eval/threeway_epe.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/.gitignore
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/LICENSE
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/README.md
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 bucketed_scene_flow_eval-2.0.7/PKG-INFO
```

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/__init__.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/argoverse2/__init__.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/argoverse2/__init__.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_raw_data.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_raw_data.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_scene_flow.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/argoverse2/argoverse_scene_flow.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/argoverse2/av2_metacategories.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/argoverse2/av2_metacategories.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/argoverse2/dataset.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/argoverse2/dataset.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/argoverse2/symlink_camera_data.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/argoverse2/symlink_camera_data.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_loader.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/nuscenes/nuscenes_loader.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/waymoopen/dataset.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/waymoopen/dataset.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datasets/waymoopen/waymo_supervised_flow.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datasets/waymoopen/waymo_supervised_flow.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datastructures/__init__.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datastructures/camera_projection.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datastructures/camera_projection.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datastructures/dataclasses.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datastructures/dataclasses.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datastructures/o3d_visualizer.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datastructures/o3d_visualizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                 self.add_geometry(g)
         else:
             self.geometry_list.append(geometry)
 
     def add_global_pc_frame(
         self,
         pc_frame: PointCloudFrame,
-        color: Union[tuple[float, float, float], None] = None,
+        color: Optional[ColorType] = None,
     ):
         self.add_pointcloud(pc_frame.global_pc, color=color)
 
     def _paint_o3d_color(self, o3d_geom, color: ColorType):
         assert color is not None, "Expected color to be not None"
         color = np.array(color)
         if color.ndim == 1:
@@ -78,23 +78,25 @@
             p1s_o3d, p2s_o3d, corrispondences
         )
         if color is not None:
             self._paint_o3d_color(lineset, color)
 
         self.add_geometry(lineset)
 
-    def add_global_flow(self, pc_frame: PointCloudFrame, ego_flow: EgoLidarFlow):
+    def add_global_flow(
+        self, pc_frame: PointCloudFrame, ego_flow: EgoLidarFlow, color: Optional[ColorType] = None
+    ):
         # Add lineset for flow vectors
         ego_pc1 = pc_frame.full_pc.mask_points(ego_flow.mask)
         ego_p2 = ego_pc1.flow(ego_flow.valid_flow)
         global_pc1 = ego_pc1.transform(pc_frame.global_pose)
         global_pc2 = ego_p2.transform(pc_frame.global_pose)
         # self.add_pointcloud(global_pc1, color=(0, 1, 0))
         # self.add_pointcloud(global_pc2, color=(0, 0, 1))
-        self.add_lineset(global_pc1, global_pc2)
+        self.add_lineset(global_pc1, global_pc2, color=color)
 
     def add_global_rgb_frame(self, rgb_frame: RGBFrame):
         image_plane_pc, colors = rgb_frame.camera_projection.image_to_image_plane_pc(
             rgb_frame.rgb, depth=20
         )
         image_plane_pc = image_plane_pc.transform(rgb_frame.pose.sensor_to_global)
         self.add_pointcloud(image_plane_pc, color=colors)
@@ -200,10 +202,10 @@
             vis.add_geometry(geometry, reset_bounding_box=reset_view)
 
     def run(self, vis=o3d.visualization.Visualizer()):
         print("Running visualizer on geometry list of length", len(self.geometry_list))
         vis.create_window(window_name="Benchmark Visualizer")
         vis.get_render_option().point_size = self.point_size
 
-        self.render()
+        self.render(vis)
 
         vis.run()
```

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datastructures/pointcloud.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datastructures/pointcloud.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datastructures/rgb_image.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datastructures/rgb_image.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datastructures/se2.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datastructures/se2.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/datastructures/se3.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/datastructures/se3.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/eval/base_per_frame_sceneflow_eval.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/eval/base_per_frame_sceneflow_eval.py`

 * *Files 5% similar despite different names*

```diff
@@ -189,17 +189,18 @@
 
         # Ensure that the predictions underlying array is the same shape as the gt
         assert len(predicted_flow.full_flow) == len(
             gt_frame.flow.full_flow
         ), f"predictions and ground_truth must have the same length, got {len(predicted_flow.full_flow)} and {len(gt_frame.flow.full_flow)}"
 
         # Validate that all valid gt flow vectors are considered valid in the predictions.
-        assert np.all(
-            (predicted_flow.mask & gt_frame.flow.mask) == gt_frame.flow.mask
-        ), "All valid gt flow vectors must be considered valid in the predictions"
+        if not np.all((predicted_flow.mask & gt_frame.flow.mask) == gt_frame.flow.mask):
+            print(
+                f"{gt_frame.log_id} index {gt_frame.log_idx} with timestamp {gt_frame.log_timestamp} missing {np.sum(gt_frame.flow.mask & ~predicted_flow.mask)} points marked valid."
+            )
 
         # Set the prediction valid flow mask to be the gt flow so everything lines up
         predicted_flow.mask = gt_frame.flow.mask
 
     def eval(self, predicted_flow: EgoLidarFlow, gt_frame: TimeSyncedSceneFlowFrame):
         self._sanitize_and_validate_inputs(predicted_flow, gt_frame)
```

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/eval/bucketed_epe.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/eval/bucketed_epe.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/eval/threeway_epe.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/eval/threeway_epe.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/interfaces/__init__.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/interfaces/abstract_dataset.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/interfaces/abstract_dataset.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/interfaces/abstract_sequence_loader.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/interfaces/abstract_sequence_loader.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/interfaces/base_dataset_abstract_seq_loader.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/interfaces/base_dataset_abstract_seq_loader.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/utils/__init__.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/bucketed_scene_flow_eval/utils/loaders.py` & `bucketed_scene_flow_eval-2.0.7/bucketed_scene_flow_eval/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/tests/integration_tests.py` & `bucketed_scene_flow_eval-2.0.7/tests/integration_tests.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/tests/setup.sh` & `bucketed_scene_flow_eval-2.0.7/tests/setup.sh`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/tests/datasets/argoverse2/av2_small_tests.py` & `bucketed_scene_flow_eval-2.0.7/tests/datasets/argoverse2/av2_small_tests.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/tests/datasets/argoverse2/av2_tiny_tests.py` & `bucketed_scene_flow_eval-2.0.7/tests/datasets/argoverse2/av2_tiny_tests.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/tests/datasets/nuscenes/nuscenes_tests.py` & `bucketed_scene_flow_eval-2.0.7/tests/datasets/nuscenes/nuscenes_tests.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/tests/datastructures/rgb.py` & `bucketed_scene_flow_eval-2.0.7/tests/datastructures/rgb.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/tests/eval/bucketed_epe.py` & `bucketed_scene_flow_eval-2.0.7/tests/eval/bucketed_epe.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/tests/eval/threeway_epe.py` & `bucketed_scene_flow_eval-2.0.7/tests/eval/threeway_epe.py`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/LICENSE` & `bucketed_scene_flow_eval-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/README.md` & `bucketed_scene_flow_eval-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `bucketed_scene_flow_eval-2.0.6/pyproject.toml` & `bucketed_scene_flow_eval-2.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   "/data_prep_scripts",
   "/launch.sh",
   "/README.md",
 ]
 
 [project]
 name = "bucketed_scene_flow_eval"
-version = "2.0.6"
+version = "2.0.7"
 authors = [
   { name="Kyle Vedder", email="kvedder@seas.upenn.edu" },
 ]
 description = "Bucketed Scene Flow Evaluation"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `bucketed_scene_flow_eval-2.0.6/PKG-INFO` & `bucketed_scene_flow_eval-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bucketed_scene_flow_eval
-Version: 2.0.6
+Version: 2.0.7
 Summary: Bucketed Scene Flow Evaluation
 Author-email: Kyle Vedder <kvedder@seas.upenn.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

