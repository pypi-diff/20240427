# Comparing `tmp/placo-0.4.9.tar.gz` & `tmp/placo-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "placo-0.4.9.tar", last modified: Mon Mar  4 19:48:00 2024, from Unix
+gzip compressed data, was "placo-0.5.0.tar", last modified: Sat Apr 27 20:42:25 2024, from Unix
```

## Comparing `placo-0.4.9.tar` & `placo-0.5.0.tar`

### file list

```diff
@@ -1,164 +1,164 @@
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1887 2023-01-02 16:33:18.782324 placo-0.4.9/.clang-format
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       76 2023-11-13 21:37:54.672208 placo-0.4.9/.gitattributes
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       56 2023-11-14 01:16:50.300368 placo-0.4.9/.gitignore
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2023-11-13 21:37:54.672208 placo-0.4.9/.readthedocs.yaml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5913 2024-01-22 20:05:35.788006 placo-0.4.9/CMakeLists.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   116595 2023-12-06 10:18:00.208958 placo-0.4.9/Doxyfile
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1061 2023-11-13 21:37:51.528208 placo-0.4.9/LICENSE
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      181 2023-11-13 21:37:54.676208 placo-0.4.9/Makefile
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       97 2023-12-13 23:01:07.520446 placo-0.4.9/README.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    14378 2024-02-02 22:01:55.732103 placo-0.4.9/bindings/expose-dynamics.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1499 2024-03-04 19:44:36.884043 placo-0.4.9/bindings/expose-eigen.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3424 2023-12-06 10:05:50.664949 placo-0.4.9/bindings/expose-footsteps.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    12784 2024-02-01 08:53:47.380011 placo-0.4.9/bindings/expose-kinematics.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4195 2023-12-06 10:05:50.664949 placo-0.4.9/bindings/expose-parameters.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     7244 2024-03-04 19:44:36.884043 placo-0.4.9/bindings/expose-problem.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9975 2024-02-05 18:49:52.412001 placo-0.4.9/bindings/expose-robot-wrapper.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5504 2024-01-17 12:43:18.400045 placo-0.4.9/bindings/expose-tools.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2779 2023-01-02 16:33:18.782324 placo-0.4.9/bindings/expose-utils.hpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6689 2023-12-06 10:05:50.664949 placo-0.4.9/bindings/expose-walk-pattern-generator.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      453 2023-12-06 10:05:50.664949 placo-0.4.9/bindings/module.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      257 2023-12-06 10:05:50.664949 placo-0.4.9/bindings/module.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      494 2023-11-13 21:37:54.676208 placo-0.4.9/bindings/registry.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2635 2023-11-13 21:37:54.676208 placo-0.4.9/bindings/registry.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6488 2023-11-20 19:37:44.876099 placo-0.4.9/doxygen_parse.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      859 2024-03-04 19:45:08.164043 placo-0.4.9/pyproject.toml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      214 2023-11-11 14:16:55.940833 placo-0.4.9/python/.vscode/settings.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       59 2023-04-20 22:28:38.524108 placo-0.4.9/python/Makefile
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       80 2023-11-13 23:31:34.448291 placo-0.4.9/python/placo_utils/__init__.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       36 2023-04-20 22:28:38.540108 placo-0.4.9/python/placo_utils/tf.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     7440 2024-01-31 21:20:50.320566 placo-0.4.9/python/placo_utils/visualization.py
--rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)       59 2023-03-08 21:48:21.783277 placo-0.4.9/python/run_tests.sh
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3426 2024-01-31 20:57:39.144549 placo-0.4.9/src/placo/dynamics/avoid_self_collisions_constraint.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      537 2023-11-13 21:37:54.676208 placo-0.4.9/src/placo/dynamics/avoid_self_collisions_constraint.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1129 2023-11-13 21:37:54.676208 placo-0.4.9/src/placo/dynamics/com_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      837 2023-11-13 21:37:54.676208 placo-0.4.9/src/placo/dynamics/com_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      116 2023-11-13 21:37:54.676208 placo-0.4.9/src/placo/dynamics/constraint.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      702 2023-11-13 21:37:54.676208 placo-0.4.9/src/placo/dynamics/constraint.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5276 2024-01-31 20:19:14.692520 placo-0.4.9/src/placo/dynamics/contacts.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4748 2024-01-31 21:03:00.572553 placo-0.4.9/src/placo/dynamics/contacts.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    18034 2024-02-02 22:02:25.556103 placo-0.4.9/src/placo/dynamics/dynamics_solver.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    14826 2024-02-02 21:58:29.472100 placo-0.4.9/src/placo/dynamics/dynamics_solver.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      927 2023-11-13 21:37:54.676208 placo-0.4.9/src/placo/dynamics/frame_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      970 2023-11-13 21:37:54.676208 placo-0.4.9/src/placo/dynamics/frame_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1645 2023-12-20 19:17:11.004007 placo-0.4.9/src/placo/dynamics/gear_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1026 2023-12-20 16:00:30.500309 placo-0.4.9/src/placo/dynamics/gear_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1328 2023-12-20 19:17:13.532007 placo-0.4.9/src/placo/dynamics/joints_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1058 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/dynamics/joints_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1579 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/dynamics/orientation_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      941 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/dynamics/orientation_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1588 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/dynamics/position_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      837 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/dynamics/position_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      992 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/dynamics/reaction_ratio_constraint.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      565 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/dynamics/reaction_ratio_constraint.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      974 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/dynamics/relative_frame_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1361 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/dynamics/relative_frame_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2541 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/dynamics/relative_orientation_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1035 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/dynamics/relative_orientation_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2950 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/dynamics/relative_position_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1011 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/dynamics/relative_position_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      208 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/dynamics/task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1753 2023-12-21 21:15:07.840042 placo-0.4.9/src/placo/dynamics/task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      838 2023-12-21 21:24:15.772049 placo-0.4.9/src/placo/dynamics/torque_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      710 2023-12-21 21:19:31.836046 placo-0.4.9/src/placo/dynamics/torque_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      144 2023-12-06 10:05:50.664949 placo-0.4.9/src/placo/humanoid/foot_trajectory.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      325 2023-12-06 10:05:50.664949 placo-0.4.9/src/placo/humanoid/foot_trajectory.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     8900 2023-12-06 10:05:50.664949 placo-0.4.9/src/placo/humanoid/footsteps_planner.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4303 2023-12-06 10:05:50.664949 placo-0.4.9/src/placo/humanoid/footsteps_planner.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     7838 2023-12-06 10:05:50.664949 placo-0.4.9/src/placo/humanoid/footsteps_planner_naive.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1507 2023-12-06 10:05:50.664949 placo-0.4.9/src/placo/humanoid/footsteps_planner_naive.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1136 2023-12-06 10:05:50.664949 placo-0.4.9/src/placo/humanoid/footsteps_planner_repetitive.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1231 2023-12-06 10:05:50.664949 placo-0.4.9/src/placo/humanoid/footsteps_planner_repetitive.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3303 2023-12-06 10:05:50.664949 placo-0.4.9/src/placo/humanoid/humanoid_parameters.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4882 2023-12-06 10:05:50.664949 placo-0.4.9/src/placo/humanoid/humanoid_parameters.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     8975 2024-03-04 19:44:43.216043 placo-0.4.9/src/placo/humanoid/humanoid_robot.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4348 2024-01-31 20:59:40.308550 placo-0.4.9/src/placo/humanoid/humanoid_robot.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1845 2023-12-06 10:05:50.664949 placo-0.4.9/src/placo/humanoid/kick.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      807 2023-12-06 10:05:50.664949 placo-0.4.9/src/placo/humanoid/kick.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2717 2024-03-04 19:44:36.884043 placo-0.4.9/src/placo/humanoid/lipm.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1684 2023-12-06 10:05:50.668949 placo-0.4.9/src/placo/humanoid/lipm.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3721 2023-12-06 10:05:50.668949 placo-0.4.9/src/placo/humanoid/swing_foot.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      834 2023-12-06 10:05:50.668949 placo-0.4.9/src/placo/humanoid/swing_foot.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1384 2023-12-06 10:05:50.668949 placo-0.4.9/src/placo/humanoid/swing_foot_cubic.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      741 2023-12-06 10:05:50.668949 placo-0.4.9/src/placo/humanoid/swing_foot_cubic.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3422 2023-12-06 10:05:50.668949 placo-0.4.9/src/placo/humanoid/swing_foot_quintic.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      628 2023-12-06 10:05:50.668949 placo-0.4.9/src/placo/humanoid/swing_foot_quintic.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    21004 2023-12-06 10:05:50.668949 placo-0.4.9/src/placo/humanoid/walk_pattern_generator.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6423 2023-12-06 10:05:50.668949 placo-0.4.9/src/placo/humanoid/walk_pattern_generator.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4436 2023-12-06 10:05:50.668949 placo-0.4.9/src/placo/humanoid/walk_tasks.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1279 2023-12-06 10:05:50.668949 placo-0.4.9/src/placo/humanoid/walk_tasks.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1964 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/avoid_self_collisions_constraint.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      526 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/avoid_self_collisions_constraint.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1965 2023-12-11 22:05:57.864076 placo-0.4.9/src/placo/kinematics/axis_align_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      658 2023-12-11 22:12:10.512081 placo-0.4.9/src/placo/kinematics/axis_align_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      600 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/centroidal_momentum_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      646 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/centroidal_momentum_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1421 2024-02-01 09:05:27.836020 placo-0.4.9/src/placo/kinematics/com_polygon_constraint.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1024 2024-02-01 09:00:05.596016 placo-0.4.9/src/placo/kinematics/com_polygon_constraint.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      474 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/com_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      555 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/com_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2114 2023-12-06 09:46:59.260936 placo-0.4.9/src/placo/kinematics/cone_constraint.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1322 2023-12-06 10:41:00.464975 placo-0.4.9/src/placo/kinematics/cone_constraint.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      122 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/constraint.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      533 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/constraint.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1137 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/distance_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      685 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/distance_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      933 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/frame_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1232 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/frame_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1369 2023-12-20 13:18:04.168190 placo-0.4.9/src/placo/kinematics/gear_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      955 2023-12-20 13:17:19.496189 placo-0.4.9/src/placo/kinematics/gear_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      714 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/joints_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      609 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/joints_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13958 2024-01-22 20:19:15.236016 placo-0.4.9/src/placo/kinematics/kinematics_solver.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    14474 2024-01-22 20:19:11.352016 placo-0.4.9/src/placo/kinematics/kinematics_solver.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      991 2024-01-22 20:30:44.588025 placo-0.4.9/src/placo/kinematics/kinetic_energy_regularization_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      291 2024-01-22 20:05:19.112006 placo-0.4.9/src/placo/kinematics/kinetic_energy_regularization_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      943 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/orientation_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      710 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/orientation_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      842 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/position_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      690 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/position_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      761 2024-02-02 22:15:00.524113 placo-0.4.9/src/placo/kinematics/regularization_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      278 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/regularization_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      937 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/relative_frame_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1258 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/relative_frame_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1283 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/relative_orientation_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      857 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/relative_orientation_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      935 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/relative_position_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      834 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/relative_position_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      195 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1719 2023-11-13 21:37:54.680208 placo-0.4.9/src/placo/kinematics/task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2059 2023-11-18 21:17:54.440643 placo-0.4.9/src/placo/kinematics/wheel_task.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      715 2023-11-18 21:17:08.432642 placo-0.4.9/src/placo/kinematics/wheel_task.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    20315 2024-01-17 12:43:18.400045 placo-0.4.9/src/placo/model/robot_wrapper.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    19546 2023-12-21 20:27:13.964007 placo-0.4.9/src/placo/model/robot_wrapper.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      629 2023-11-13 21:37:54.684208 placo-0.4.9/src/placo/problem/constraint.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1709 2023-11-13 21:37:54.684208 placo-0.4.9/src/placo/problem/constraint.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6397 2024-03-04 19:44:36.884043 placo-0.4.9/src/placo/problem/expression.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4658 2024-03-04 19:44:36.884043 placo-0.4.9/src/placo/problem/expression.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5519 2024-03-04 19:44:36.884043 placo-0.4.9/src/placo/problem/integrator.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5414 2024-03-04 19:44:36.888043 placo-0.4.9/src/placo/problem/integrator.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1576 2023-11-13 21:37:54.684208 placo-0.4.9/src/placo/problem/polygon_constraint.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1060 2023-11-13 21:37:54.684208 placo-0.4.9/src/placo/problem/polygon_constraint.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    12066 2024-03-04 19:44:36.888043 placo-0.4.9/src/placo/problem/problem.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3521 2023-11-13 21:37:54.684208 placo-0.4.9/src/placo/problem/problem.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      181 2023-11-13 21:37:54.684208 placo-0.4.9/src/placo/problem/qp_error.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      255 2023-11-13 21:37:54.684208 placo-0.4.9/src/placo/problem/qp_error.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2683 2023-11-13 21:37:54.684208 placo-0.4.9/src/placo/problem/sparsity.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1405 2023-11-13 21:37:54.684208 placo-0.4.9/src/placo/problem/sparsity.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      505 2023-11-13 21:37:54.684208 placo-0.4.9/src/placo/problem/variable.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      960 2024-03-04 19:44:36.888043 placo-0.4.9/src/placo/problem/variable.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1528 2023-11-13 21:37:54.684208 placo-0.4.9/src/placo/tools/axises_mask.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2201 2023-11-13 21:37:54.684208 placo-0.4.9/src/placo/tools/axises_mask.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3726 2023-12-06 10:05:50.668949 placo-0.4.9/src/placo/tools/cubic_spline.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1993 2023-12-06 10:05:50.668949 placo-0.4.9/src/placo/tools/cubic_spline.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      842 2023-12-06 10:05:50.668949 placo-0.4.9/src/placo/tools/cubic_spline_3d.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      987 2023-12-06 10:05:50.668949 placo-0.4.9/src/placo/tools/cubic_spline_3d.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1205 2023-12-06 10:45:01.876978 placo-0.4.9/src/placo/tools/prioritized.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1658 2023-12-06 10:44:54.672978 placo-0.4.9/src/placo/tools/prioritized.h
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2516 2023-11-20 22:28:31.128224 placo-0.4.9/src/placo/tools/utils.cpp
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1737 2023-11-20 22:28:33.660224 placo-0.4.9/src/placo/tools/utils.h
--rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)     7977 2023-12-06 10:18:27.344959 placo-0.4.9/stubs.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      467 2023-11-13 21:37:54.684208 placo-0.4.9/tweak_sdist.sh
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       27 2023-11-13 21:37:54.684208 placo-0.4.9/wks.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      851 2024-03-04 19:45:45.656043 placo-0.4.9/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   152214 2024-03-04 19:48:00.212045 placo-0.4.9/placo.pyi
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1887 2023-01-02 16:33:18.782324 placo-0.5.0/.clang-format
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       76 2023-11-13 21:37:54.672208 placo-0.5.0/.gitattributes
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       56 2023-11-14 01:16:50.300368 placo-0.5.0/.gitignore
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2023-11-13 21:37:54.672208 placo-0.5.0/.readthedocs.yaml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5913 2024-01-22 20:05:35.788006 placo-0.5.0/CMakeLists.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   116595 2023-12-06 10:18:00.208958 placo-0.5.0/Doxyfile
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1061 2023-11-13 21:37:51.528208 placo-0.5.0/LICENSE
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      181 2023-11-13 21:37:54.676208 placo-0.5.0/Makefile
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       97 2023-12-13 23:01:07.520446 placo-0.5.0/README.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    14378 2024-02-02 22:01:55.732103 placo-0.5.0/bindings/expose-dynamics.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1499 2024-03-04 19:44:36.884043 placo-0.5.0/bindings/expose-eigen.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3424 2023-12-06 10:05:50.664949 placo-0.5.0/bindings/expose-footsteps.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    12761 2024-04-27 20:34:17.680028 placo-0.5.0/bindings/expose-kinematics.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4195 2023-12-06 10:05:50.664949 placo-0.5.0/bindings/expose-parameters.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     7352 2024-03-05 20:27:35.076089 placo-0.5.0/bindings/expose-problem.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9975 2024-02-05 18:49:52.412001 placo-0.5.0/bindings/expose-robot-wrapper.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5504 2024-04-09 13:55:29.520274 placo-0.5.0/bindings/expose-tools.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2779 2023-01-02 16:33:18.782324 placo-0.5.0/bindings/expose-utils.hpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6689 2023-12-06 10:05:50.664949 placo-0.5.0/bindings/expose-walk-pattern-generator.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      453 2023-12-06 10:05:50.664949 placo-0.5.0/bindings/module.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      257 2023-12-06 10:05:50.664949 placo-0.5.0/bindings/module.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      494 2023-11-13 21:37:54.676208 placo-0.5.0/bindings/registry.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2635 2023-11-13 21:37:54.676208 placo-0.5.0/bindings/registry.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6488 2023-11-20 19:37:44.876099 placo-0.5.0/doxygen_parse.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      859 2024-04-27 20:37:12.384030 placo-0.5.0/pyproject.toml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      214 2023-11-11 14:16:55.940833 placo-0.5.0/python/.vscode/settings.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       59 2023-04-20 22:28:38.524108 placo-0.5.0/python/Makefile
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       80 2023-11-13 23:31:34.448291 placo-0.5.0/python/placo_utils/__init__.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       36 2023-04-20 22:28:38.540108 placo-0.5.0/python/placo_utils/tf.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     7440 2024-01-31 21:20:50.320566 placo-0.5.0/python/placo_utils/visualization.py
+-rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)       59 2023-03-08 21:48:21.783277 placo-0.5.0/python/run_tests.sh
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3426 2024-01-31 20:57:39.144549 placo-0.5.0/src/placo/dynamics/avoid_self_collisions_constraint.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      537 2023-11-13 21:37:54.676208 placo-0.5.0/src/placo/dynamics/avoid_self_collisions_constraint.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1129 2023-11-13 21:37:54.676208 placo-0.5.0/src/placo/dynamics/com_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      837 2023-11-13 21:37:54.676208 placo-0.5.0/src/placo/dynamics/com_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      116 2023-11-13 21:37:54.676208 placo-0.5.0/src/placo/dynamics/constraint.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      702 2023-11-13 21:37:54.676208 placo-0.5.0/src/placo/dynamics/constraint.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5276 2024-01-31 20:19:14.692520 placo-0.5.0/src/placo/dynamics/contacts.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4748 2024-01-31 21:03:00.572553 placo-0.5.0/src/placo/dynamics/contacts.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    18034 2024-02-02 22:02:25.556103 placo-0.5.0/src/placo/dynamics/dynamics_solver.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    14826 2024-02-02 21:58:29.472100 placo-0.5.0/src/placo/dynamics/dynamics_solver.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      927 2023-11-13 21:37:54.676208 placo-0.5.0/src/placo/dynamics/frame_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      970 2023-11-13 21:37:54.676208 placo-0.5.0/src/placo/dynamics/frame_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1645 2023-12-20 19:17:11.004007 placo-0.5.0/src/placo/dynamics/gear_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1026 2023-12-20 16:00:30.500309 placo-0.5.0/src/placo/dynamics/gear_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1328 2023-12-20 19:17:13.532007 placo-0.5.0/src/placo/dynamics/joints_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1058 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/dynamics/joints_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1579 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/dynamics/orientation_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      941 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/dynamics/orientation_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1588 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/dynamics/position_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      837 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/dynamics/position_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      992 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/dynamics/reaction_ratio_constraint.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      565 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/dynamics/reaction_ratio_constraint.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      974 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/dynamics/relative_frame_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1361 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/dynamics/relative_frame_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2541 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/dynamics/relative_orientation_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1035 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/dynamics/relative_orientation_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2950 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/dynamics/relative_position_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1011 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/dynamics/relative_position_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      208 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/dynamics/task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1753 2023-12-21 21:15:07.840042 placo-0.5.0/src/placo/dynamics/task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      838 2023-12-21 21:24:15.772049 placo-0.5.0/src/placo/dynamics/torque_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      710 2023-12-21 21:19:31.836046 placo-0.5.0/src/placo/dynamics/torque_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      144 2023-12-06 10:05:50.664949 placo-0.5.0/src/placo/humanoid/foot_trajectory.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      325 2023-12-06 10:05:50.664949 placo-0.5.0/src/placo/humanoid/foot_trajectory.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     8900 2023-12-06 10:05:50.664949 placo-0.5.0/src/placo/humanoid/footsteps_planner.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4303 2023-12-06 10:05:50.664949 placo-0.5.0/src/placo/humanoid/footsteps_planner.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     7838 2023-12-06 10:05:50.664949 placo-0.5.0/src/placo/humanoid/footsteps_planner_naive.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1507 2023-12-06 10:05:50.664949 placo-0.5.0/src/placo/humanoid/footsteps_planner_naive.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1136 2023-12-06 10:05:50.664949 placo-0.5.0/src/placo/humanoid/footsteps_planner_repetitive.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1231 2023-12-06 10:05:50.664949 placo-0.5.0/src/placo/humanoid/footsteps_planner_repetitive.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3303 2023-12-06 10:05:50.664949 placo-0.5.0/src/placo/humanoid/humanoid_parameters.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4882 2023-12-06 10:05:50.664949 placo-0.5.0/src/placo/humanoid/humanoid_parameters.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     8975 2024-03-04 19:44:43.216043 placo-0.5.0/src/placo/humanoid/humanoid_robot.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4348 2024-01-31 20:59:40.308550 placo-0.5.0/src/placo/humanoid/humanoid_robot.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1845 2023-12-06 10:05:50.664949 placo-0.5.0/src/placo/humanoid/kick.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      807 2023-12-06 10:05:50.664949 placo-0.5.0/src/placo/humanoid/kick.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2717 2024-03-04 19:44:36.884043 placo-0.5.0/src/placo/humanoid/lipm.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1684 2023-12-06 10:05:50.668949 placo-0.5.0/src/placo/humanoid/lipm.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3721 2023-12-06 10:05:50.668949 placo-0.5.0/src/placo/humanoid/swing_foot.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      834 2023-12-06 10:05:50.668949 placo-0.5.0/src/placo/humanoid/swing_foot.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1384 2023-12-06 10:05:50.668949 placo-0.5.0/src/placo/humanoid/swing_foot_cubic.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      741 2023-12-06 10:05:50.668949 placo-0.5.0/src/placo/humanoid/swing_foot_cubic.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3422 2023-12-06 10:05:50.668949 placo-0.5.0/src/placo/humanoid/swing_foot_quintic.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      628 2023-12-06 10:05:50.668949 placo-0.5.0/src/placo/humanoid/swing_foot_quintic.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    21004 2023-12-06 10:05:50.668949 placo-0.5.0/src/placo/humanoid/walk_pattern_generator.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6423 2023-12-06 10:05:50.668949 placo-0.5.0/src/placo/humanoid/walk_pattern_generator.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4440 2024-04-27 20:32:38.912027 placo-0.5.0/src/placo/humanoid/walk_tasks.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1279 2023-12-06 10:05:50.668949 placo-0.5.0/src/placo/humanoid/walk_tasks.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1964 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/avoid_self_collisions_constraint.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      526 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/avoid_self_collisions_constraint.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1965 2023-12-11 22:05:57.864076 placo-0.5.0/src/placo/kinematics/axis_align_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      658 2023-12-11 22:12:10.512081 placo-0.5.0/src/placo/kinematics/axis_align_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      600 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/centroidal_momentum_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      646 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/centroidal_momentum_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1345 2024-03-29 18:51:56.324001 placo-0.5.0/src/placo/kinematics/com_polygon_constraint.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1024 2024-02-01 09:00:05.596016 placo-0.5.0/src/placo/kinematics/com_polygon_constraint.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      474 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/com_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      555 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/com_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2114 2023-12-06 09:46:59.260936 placo-0.5.0/src/placo/kinematics/cone_constraint.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1322 2023-12-06 10:41:00.464975 placo-0.5.0/src/placo/kinematics/cone_constraint.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      122 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/constraint.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      533 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/constraint.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1137 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/distance_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      685 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/distance_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      933 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/frame_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1232 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/frame_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1336 2024-04-27 20:33:41.388028 placo-0.5.0/src/placo/kinematics/gear_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      955 2023-12-20 13:17:19.496189 placo-0.5.0/src/placo/kinematics/gear_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      714 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/joints_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      609 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/joints_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13928 2024-04-27 20:30:41.484026 placo-0.5.0/src/placo/kinematics/kinematics_solver.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    14570 2024-04-27 20:29:21.760025 placo-0.5.0/src/placo/kinematics/kinematics_solver.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      991 2024-01-22 20:30:44.588025 placo-0.5.0/src/placo/kinematics/kinetic_energy_regularization_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      291 2024-01-22 20:05:19.112006 placo-0.5.0/src/placo/kinematics/kinetic_energy_regularization_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      943 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/orientation_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      710 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/orientation_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      842 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/position_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      690 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/position_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      761 2024-02-02 22:15:00.524113 placo-0.5.0/src/placo/kinematics/regularization_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      278 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/regularization_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      937 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/relative_frame_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1258 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/relative_frame_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1283 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/relative_orientation_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      857 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/relative_orientation_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      935 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/relative_position_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      834 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/relative_position_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      195 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1719 2023-11-13 21:37:54.680208 placo-0.5.0/src/placo/kinematics/task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2059 2023-11-18 21:17:54.440643 placo-0.5.0/src/placo/kinematics/wheel_task.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      715 2023-11-18 21:17:08.432642 placo-0.5.0/src/placo/kinematics/wheel_task.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    20315 2024-01-17 12:43:18.400045 placo-0.5.0/src/placo/model/robot_wrapper.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    19546 2023-12-21 20:27:13.964007 placo-0.5.0/src/placo/model/robot_wrapper.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      629 2023-11-13 21:37:54.684208 placo-0.5.0/src/placo/problem/constraint.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1709 2023-11-13 21:37:54.684208 placo-0.5.0/src/placo/problem/constraint.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6397 2024-03-04 19:44:36.884043 placo-0.5.0/src/placo/problem/expression.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4658 2024-03-04 19:44:36.884043 placo-0.5.0/src/placo/problem/expression.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5519 2024-03-05 20:26:35.908088 placo-0.5.0/src/placo/problem/integrator.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5414 2024-03-04 19:44:36.888043 placo-0.5.0/src/placo/problem/integrator.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1576 2023-11-13 21:37:54.684208 placo-0.5.0/src/placo/problem/polygon_constraint.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1060 2023-11-13 21:37:54.684208 placo-0.5.0/src/placo/problem/polygon_constraint.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    12066 2024-03-04 19:44:36.888043 placo-0.5.0/src/placo/problem/problem.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3521 2023-11-13 21:37:54.684208 placo-0.5.0/src/placo/problem/problem.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      181 2023-11-13 21:37:54.684208 placo-0.5.0/src/placo/problem/qp_error.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      255 2023-11-13 21:37:54.684208 placo-0.5.0/src/placo/problem/qp_error.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2683 2023-11-13 21:37:54.684208 placo-0.5.0/src/placo/problem/sparsity.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1405 2023-11-13 21:37:54.684208 placo-0.5.0/src/placo/problem/sparsity.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      505 2023-11-13 21:37:54.684208 placo-0.5.0/src/placo/problem/variable.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      960 2024-03-04 19:44:36.888043 placo-0.5.0/src/placo/problem/variable.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1528 2023-11-13 21:37:54.684208 placo-0.5.0/src/placo/tools/axises_mask.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2201 2023-11-13 21:37:54.684208 placo-0.5.0/src/placo/tools/axises_mask.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3726 2023-12-06 10:05:50.668949 placo-0.5.0/src/placo/tools/cubic_spline.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1993 2023-12-06 10:05:50.668949 placo-0.5.0/src/placo/tools/cubic_spline.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      842 2023-12-06 10:05:50.668949 placo-0.5.0/src/placo/tools/cubic_spline_3d.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      987 2023-12-06 10:05:50.668949 placo-0.5.0/src/placo/tools/cubic_spline_3d.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1205 2023-12-06 10:45:01.876978 placo-0.5.0/src/placo/tools/prioritized.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1658 2023-12-06 10:44:54.672978 placo-0.5.0/src/placo/tools/prioritized.h
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2516 2023-11-20 22:28:31.128224 placo-0.5.0/src/placo/tools/utils.cpp
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1737 2023-11-20 22:28:33.660224 placo-0.5.0/src/placo/tools/utils.h
+-rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)     7977 2023-12-06 10:18:27.344959 placo-0.5.0/stubs.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      467 2023-11-13 21:37:54.684208 placo-0.5.0/tweak_sdist.sh
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       27 2023-11-13 21:37:54.684208 placo-0.5.0/wks.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      851 2024-04-27 20:40:57.380033 placo-0.5.0/PKG-INFO
+-rw-r--r--   0 gregwar   (1000) gregwar   (1000)   152373 2024-04-27 20:42:25.252034 placo-0.5.0/placo.pyi
```

### Comparing `placo-0.4.9/.clang-format` & `placo-0.5.0/.clang-format`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/.readthedocs.yaml` & `placo-0.5.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/CMakeLists.txt` & `placo-0.5.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/Doxyfile` & `placo-0.5.0/Doxyfile`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/LICENSE` & `placo-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/bindings/expose-dynamics.cpp` & `placo-0.5.0/bindings/expose-dynamics.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/bindings/expose-eigen.cpp` & `placo-0.5.0/bindings/expose-eigen.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/bindings/expose-footsteps.cpp` & `placo-0.5.0/bindings/expose-footsteps.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/bindings/expose-kinematics.cpp` & `placo-0.5.0/bindings/expose-kinematics.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 BOOST_PYTHON_MEMBER_FUNCTION_OVERLOADS(frametask_configure_overloads, configure, 2, 4);
 
 void exposeKinematics()
 {
   class_<KinematicsSolver> solver_class =
       class__<KinematicsSolver>("KinematicsSolver", init<RobotWrapper&>())
           .add_property("problem", &KinematicsSolver::problem)
-          .add_property("noise", &KinematicsSolver::noise, &KinematicsSolver::noise)
           .add_property("dt", &KinematicsSolver::dt, &KinematicsSolver::dt)
           .add_property("N", &KinematicsSolver::N)
           .add_property("scale", &KinematicsSolver::scale)
           .add_property(
               "robot", +[](const KinematicsSolver& solver) { return solver.robot; })
 
           // Position and CoM task
@@ -107,15 +106,16 @@
           .def("enable_joint_limits", &KinematicsSolver::enable_joint_limits)
           .def("enable_velocity_limits", &KinematicsSolver::enable_velocity_limits)
           .def<void (KinematicsSolver::*)(Task&)>("add_task", &KinematicsSolver::add_task)
           .def<void (KinematicsSolver::*)(Constraint&)>("add_constraint", &KinematicsSolver::add_constraint)
           .def<void (KinematicsSolver::*)(Task&)>("remove_task", &KinematicsSolver::remove_task)
           .def<void (KinematicsSolver::*)(FrameTask&)>("remove_task", &KinematicsSolver::remove_task)
           .def("remove_constraint", &KinematicsSolver::remove_constraint)
-          .def("solve", &KinematicsSolver::solve);
+          .def("solve", &KinematicsSolver::solve)
+          .def("add_q_noise", &KinematicsSolver::add_q_noise);
 
   class__<Task, bases<tools::Prioritized>, boost::noncopyable>("Task", no_init)
       .add_property(
           "A", +[](const Task& task) { return task.A; })
       .add_property(
           "b", +[](const Task& task) { return task.b; })
       .def("error", &Task::error)
```

### Comparing `placo-0.4.9/bindings/expose-parameters.cpp` & `placo-0.5.0/bindings/expose-parameters.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/bindings/expose-problem.cpp` & `placo-0.5.0/bindings/expose-problem.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 #include <boost/python.hpp>
 
 using namespace boost::python;
 using namespace placo;
 using namespace placo::problem;
 
 BOOST_PYTHON_MEMBER_FUNCTION_OVERLOADS(expr_overloads, expr, 0, 2);
+BOOST_PYTHON_MEMBER_FUNCTION_OVERLOADS(integrator_expr_overloads, expr, 1, 2);
 BOOST_PYTHON_MEMBER_FUNCTION_OVERLOADS(configure_overloads, configure, 1, 2);
 
 void exposeProblem()
 {
   class__<QPError>("QPError", init<std::string>()).def("what", &QPError::what);
 
   class__<Sparsity::Interval>("SparsityInterval")
@@ -87,15 +88,15 @@
           "M", +[](const Integrator& i) { return i.M; })
       .add_property(
           "A", +[](const Integrator& i) { return i.A; })
       .add_property(
           "B", +[](const Integrator& i) { return i.B; })
       .add_property(
           "final_transition_matrix", +[](const Integrator& i) { return i.final_transition_matrix; })
-      .def("expr", &Integrator::expr)
+      .def("expr", &Integrator::expr, integrator_expr_overloads())
       .def("expr_t", &Integrator::expr_t)
       .def("value", &Integrator::value)
       .def("get_trajectory", &Integrator::get_trajectory);
 
   class__<Integrator::Trajectory>("IntegratorTrajectory")
       .def("value", &Integrator::Trajectory::value)
       .def("duration", &Integrator::Trajectory::duration);
```

### Comparing `placo-0.4.9/bindings/expose-robot-wrapper.cpp` & `placo-0.5.0/bindings/expose-robot-wrapper.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/bindings/expose-tools.cpp` & `placo-0.5.0/bindings/expose-tools.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/bindings/expose-utils.hpp` & `placo-0.5.0/bindings/expose-utils.hpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/bindings/expose-walk-pattern-generator.cpp` & `placo-0.5.0/bindings/expose-walk-pattern-generator.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/bindings/registry.h` & `placo-0.5.0/bindings/registry.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/doxygen_parse.py` & `placo-0.5.0/doxygen_parse.py`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/pyproject.toml` & `placo-0.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   "numpy",
   "ischedule"
 ]
 description = "PlaCo: Rhoban Planning and Control"
 license = "MIT"
 name = "placo"
 requires-python = ">= 3.8"
-version = "0.4.9"
+version = "0.5.0"
 
 [project.urls]
 changelog = "https://github.com/rhoban/placo/blob/main/CHANGELOG.md"
 homepage = "https://placo.readthedocs.io/en/latest/"
 repository = "https://github.com/rhoban/placo.git"
 
 [tool.isort]
```

### Comparing `placo-0.4.9/python/placo_utils/visualization.py` & `placo-0.5.0/python/placo_utils/visualization.py`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/avoid_self_collisions_constraint.cpp` & `placo-0.5.0/src/placo/dynamics/avoid_self_collisions_constraint.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/avoid_self_collisions_constraint.h` & `placo-0.5.0/src/placo/dynamics/avoid_self_collisions_constraint.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/com_task.cpp` & `placo-0.5.0/src/placo/dynamics/com_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/com_task.h` & `placo-0.5.0/src/placo/dynamics/com_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/constraint.h` & `placo-0.5.0/src/placo/dynamics/constraint.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/contacts.cpp` & `placo-0.5.0/src/placo/dynamics/contacts.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/contacts.h` & `placo-0.5.0/src/placo/dynamics/contacts.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/dynamics_solver.cpp` & `placo-0.5.0/src/placo/dynamics/dynamics_solver.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/dynamics_solver.h` & `placo-0.5.0/src/placo/dynamics/dynamics_solver.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/frame_task.cpp` & `placo-0.5.0/src/placo/dynamics/frame_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/frame_task.h` & `placo-0.5.0/src/placo/dynamics/frame_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/gear_task.cpp` & `placo-0.5.0/src/placo/dynamics/gear_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/gear_task.h` & `placo-0.5.0/src/placo/dynamics/gear_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/joints_task.cpp` & `placo-0.5.0/src/placo/dynamics/joints_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/joints_task.h` & `placo-0.5.0/src/placo/dynamics/joints_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/orientation_task.cpp` & `placo-0.5.0/src/placo/dynamics/orientation_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/orientation_task.h` & `placo-0.5.0/src/placo/dynamics/orientation_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/position_task.cpp` & `placo-0.5.0/src/placo/dynamics/position_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/position_task.h` & `placo-0.5.0/src/placo/dynamics/position_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/reaction_ratio_constraint.cpp` & `placo-0.5.0/src/placo/dynamics/reaction_ratio_constraint.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/reaction_ratio_constraint.h` & `placo-0.5.0/src/placo/dynamics/reaction_ratio_constraint.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/relative_frame_task.cpp` & `placo-0.5.0/src/placo/dynamics/relative_frame_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/relative_frame_task.h` & `placo-0.5.0/src/placo/dynamics/relative_frame_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/relative_orientation_task.cpp` & `placo-0.5.0/src/placo/dynamics/relative_orientation_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/relative_orientation_task.h` & `placo-0.5.0/src/placo/dynamics/relative_orientation_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/relative_position_task.cpp` & `placo-0.5.0/src/placo/dynamics/relative_position_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/relative_position_task.h` & `placo-0.5.0/src/placo/dynamics/relative_position_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/task.h` & `placo-0.5.0/src/placo/dynamics/task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/torque_task.cpp` & `placo-0.5.0/src/placo/dynamics/torque_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/dynamics/torque_task.h` & `placo-0.5.0/src/placo/dynamics/torque_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/footsteps_planner.cpp` & `placo-0.5.0/src/placo/humanoid/footsteps_planner.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/footsteps_planner.h` & `placo-0.5.0/src/placo/humanoid/footsteps_planner.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/footsteps_planner_naive.cpp` & `placo-0.5.0/src/placo/humanoid/footsteps_planner_naive.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/footsteps_planner_naive.h` & `placo-0.5.0/src/placo/humanoid/footsteps_planner_naive.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/footsteps_planner_repetitive.cpp` & `placo-0.5.0/src/placo/humanoid/footsteps_planner_repetitive.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/footsteps_planner_repetitive.h` & `placo-0.5.0/src/placo/humanoid/footsteps_planner_repetitive.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/humanoid_parameters.cpp` & `placo-0.5.0/src/placo/humanoid/humanoid_parameters.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/humanoid_parameters.h` & `placo-0.5.0/src/placo/humanoid/humanoid_parameters.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/humanoid_robot.cpp` & `placo-0.5.0/src/placo/humanoid/humanoid_robot.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/humanoid_robot.h` & `placo-0.5.0/src/placo/humanoid/humanoid_robot.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/kick.cpp` & `placo-0.5.0/src/placo/humanoid/kick.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/kick.h` & `placo-0.5.0/src/placo/humanoid/kick.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/lipm.cpp` & `placo-0.5.0/src/placo/humanoid/lipm.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/lipm.h` & `placo-0.5.0/src/placo/humanoid/lipm.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/swing_foot.cpp` & `placo-0.5.0/src/placo/humanoid/swing_foot.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/swing_foot.h` & `placo-0.5.0/src/placo/humanoid/swing_foot.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/swing_foot_cubic.cpp` & `placo-0.5.0/src/placo/humanoid/swing_foot_cubic.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/swing_foot_cubic.h` & `placo-0.5.0/src/placo/humanoid/swing_foot_cubic.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/swing_foot_quintic.cpp` & `placo-0.5.0/src/placo/humanoid/swing_foot_quintic.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/swing_foot_quintic.h` & `placo-0.5.0/src/placo/humanoid/swing_foot_quintic.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/walk_pattern_generator.cpp` & `placo-0.5.0/src/placo/humanoid/walk_pattern_generator.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/walk_pattern_generator.h` & `placo-0.5.0/src/placo/humanoid/walk_pattern_generator.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/humanoid/walk_tasks.cpp` & `placo-0.5.0/src/placo/humanoid/walk_tasks.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 #include "placo/humanoid/humanoid_robot.h"
 
 namespace placo::humanoid
 {
 using namespace placo::kinematics;
 using namespace placo::tools;
 
-
 void WalkTasks::initialize_tasks(KinematicsSolver* solver_, HumanoidRobot* robot_)
 {
   robot = robot_;
   solver = solver_;
 
   left_foot_task = solver->add_frame_task("left_foot", robot->get_T_world_left());
-  left_foot_task.configure("left_foot", scaled?"scaled":"soft", 1., 1.);
+  left_foot_task.configure("left_foot", scaled ? "scaled" : "soft", 1., 1.);
 
   right_foot_task = solver->add_frame_task("right_foot", robot->get_T_world_right());
-  right_foot_task.configure("right_foot", scaled?"scaled":"soft", 1., 1.);
+  right_foot_task.configure("right_foot", scaled ? "scaled" : "soft", 1., 1.);
 
   trunk_orientation_task = &solver->add_orientation_task("trunk", robot->get_T_world_trunk().rotation());
-  trunk_orientation_task->configure("trunk", scaled?"scaled":"soft", 1.);
+  trunk_orientation_task->configure("trunk", scaled ? "scaled" : "soft", 1.);
 
   update_com_task();
 }
 
 void WalkTasks::update_com_task()
 {
   if (trunk_mode)
@@ -32,28 +31,28 @@
     {
       solver->remove_task(*com_task);
       com_task = nullptr;
     }
     if (trunk_task == nullptr)
     {
       trunk_task = &solver->add_position_task("trunk", robot->get_T_world_frame("trunk").translation());
-      trunk_task->configure("trunk", scaled?"scaled":"soft", 1.);
+      trunk_task->configure("trunk", scaled ? "scaled" : "soft", 1.);
     }
   }
   else
   {
     if (trunk_task != nullptr)
     {
       solver->remove_task(*trunk_task);
       trunk_task = nullptr;
     }
     if (com_task == nullptr)
     {
       com_task = &solver->add_com_task(robot->com_world());
-      com_task->configure("com", scaled?"scaled":"soft", 1.);
+      com_task->configure("com", scaled ? "scaled" : "soft", 1.);
     }
   }
 }
 
 void WalkTasks::reach_initial_pose(Eigen::Affine3d T_world_left, double feet_spacing, double com_height,
                                    double trunk_pitch)
 {
@@ -65,21 +64,20 @@
 
   Eigen::MatrixXd R_world_trunk = interpolate_frames(T_world_left, T_world_right, .5) *
                                   Eigen::AngleAxisd(trunk_pitch, Eigen::Vector3d::UnitY()).matrix();
   trunk_orientation_task->R_world_frame = R_world_trunk;
 
   update_tasks(T_world_left, T_world_right, com_world, R_world_trunk);
 
-  // Adding strong noise to avoid singularities
-  solver->noise = 0.1;
   for (int i = 0; i < 100; i++)
   {
-    if (i == 10)
+    if (i <= 10)
     {
-      solver->noise = 1e-4;
+      // Adding strong noise to avoid singularities
+      solver->add_q_noise(0.1);
     }
 
     robot->update_kinematics();
     solver->solve(true);
   }
 }
```

### Comparing `placo-0.4.9/src/placo/humanoid/walk_tasks.h` & `placo-0.5.0/src/placo/humanoid/walk_tasks.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/avoid_self_collisions_constraint.cpp` & `placo-0.5.0/src/placo/kinematics/avoid_self_collisions_constraint.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/avoid_self_collisions_constraint.h` & `placo-0.5.0/src/placo/kinematics/avoid_self_collisions_constraint.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/axis_align_task.cpp` & `placo-0.5.0/src/placo/kinematics/axis_align_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/axis_align_task.h` & `placo-0.5.0/src/placo/kinematics/axis_align_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/centroidal_momentum_task.cpp` & `placo-0.5.0/src/placo/kinematics/centroidal_momentum_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/centroidal_momentum_task.h` & `placo-0.5.0/src/placo/kinematics/centroidal_momentum_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/com_polygon_constraint.cpp` & `placo-0.5.0/src/placo/kinematics/com_polygon_constraint.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,14 @@
       throw std::runtime_error("DCM mode requires a non-zero solver.dt and omega");
     }
 
     // DCM is d = c + dc / w with x = sqrt(g / h)
     // Future DCM is c + J dq + J dq / (dt * w)
     //             = c + J dq (1 + 1 / (dt * w))
     com_xy.A *= (1. + 1. / (solver->dt * omega));
-    std::cout << "Coef: " << (1. + 1. / (solver->dt * omega)) << std::endl;
   }
   com_xy.b = com;
 
   // Adding constraints
   problem.add_constraint(problem::PolygonConstraint::in_polygon_xy(com_xy, polygon, margin))
       .configure(priority == Prioritized::Priority::Hard ? problem::ProblemConstraint::Hard :
                                                            problem::ProblemConstraint::Soft,
```

### Comparing `placo-0.4.9/src/placo/kinematics/com_polygon_constraint.h` & `placo-0.5.0/src/placo/kinematics/com_polygon_constraint.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/com_task.h` & `placo-0.5.0/src/placo/kinematics/com_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/cone_constraint.cpp` & `placo-0.5.0/src/placo/kinematics/cone_constraint.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/cone_constraint.h` & `placo-0.5.0/src/placo/kinematics/cone_constraint.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/constraint.h` & `placo-0.5.0/src/placo/kinematics/constraint.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/distance_task.cpp` & `placo-0.5.0/src/placo/kinematics/distance_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/distance_task.h` & `placo-0.5.0/src/placo/kinematics/distance_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/frame_task.cpp` & `placo-0.5.0/src/placo/kinematics/frame_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/frame_task.h` & `placo-0.5.0/src/placo/kinematics/frame_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/gear_task.cpp` & `placo-0.5.0/src/placo/kinematics/gear_task.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     double q_target = solver->robot.state.q[target + 1];
     b(k, 0) = q_target;
 
     for (auto& gear_source : entry.second)
     {
       int source = gear_source.first;
       double ratio = gear_source.second;
-      auto& gear = entry.second;
       double q_source = solver->robot.state.q[source + 1];
 
       A(k, source) = ratio;
       b(k, 0) -= q_source * ratio;
     }
 
     k += 1;
```

### Comparing `placo-0.4.9/src/placo/kinematics/gear_task.h` & `placo-0.5.0/src/placo/kinematics/gear_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/joints_task.cpp` & `placo-0.5.0/src/placo/kinematics/joints_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/joints_task.h` & `placo-0.5.0/src/placo/kinematics/joints_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/kinematics_solver.cpp` & `placo-0.5.0/src/placo/kinematics/kinematics_solver.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -240,45 +240,42 @@
   if (velocity_limits)
   {
     problem.add_constraint(qd->expr(6) <= dt * robot.model.velocityLimit.bottomRows(N - 6));
     problem.add_constraint(-dt * robot.model.velocityLimit.bottomRows(N - 6) <= qd->expr(6));
   }
 }
 
+void KinematicsSolver::add_q_noise(double noise)
+{
+  auto q_random = pinocchio::randomConfiguration(robot.model);
+
+  // Adding some noise in direction of a random configuration (except floating base)
+  for (int k = 7; k < robot.model.nq; k++)
+  {
+    if (robot.model.lowerPositionLimit(k) == std::numeric_limits<double>::lowest() ||
+        robot.model.upperPositionLimit(k) == std::numeric_limits<double>::max())
+    {
+      continue;
+    }
+
+    robot.state.q(k) += (q_random(k) - robot.state.q(k)) * noise;
+  }
+}
+
 Eigen::VectorXd KinematicsSolver::solve(bool apply)
 {
   // Ensure variable is created
   if (qd == nullptr)
   {
     qd = &problem.add_variable(N);
   }
 
   // Clear previously created constraints
   problem.clear_constraints();
 
-  // Adding some random noise
-  auto q_save = robot.state.q;
-
-  if (noise > 0)
-  {
-    auto q_random = pinocchio::randomConfiguration(robot.model);
-
-    // Adding some noise in direction of a random configuration (except floating base)
-    for (int k = 7; k < robot.model.nq; k++)
-    {
-      if (robot.model.lowerPositionLimit(k) == std::numeric_limits<double>::lowest() ||
-          robot.model.upperPositionLimit(k) == std::numeric_limits<double>::max())
-      {
-        continue;
-      }
-
-      robot.state.q(k) += (q_random(k) - robot.state.q(k)) * noise;
-    }
-  }
-
   has_scaling = false;
 
   // Updating all the task matrices
   for (auto task : tasks)
   {
     task->update();
 
@@ -355,26 +352,25 @@
   if (has_scaling)
   {
     scale = scale_variable->value(0, 0);
   }
 
   if (apply)
   {
+    // Initial robot configuration
+    auto q_save = robot.state.q;
+
     robot.state.q = pinocchio::integrate(robot.model, robot.state.q, qd_sol);
     if (dt > 0)
     {
       auto qd_save = robot.state.qd;
       robot.state.qd = pinocchio::difference(robot.model, q_save, robot.state.q) / dt;
       robot.state.qdd = (robot.state.qd - qd_save) / dt;
     }
   }
-  else
-  {
-    robot.state.q = q_save;
-  }
 
   return qd_sol;
 }
 
 void KinematicsSolver::clear()
 {
   for (auto& task : tasks)
```

### Comparing `placo-0.4.9/src/placo/kinematics/kinematics_solver.h` & `placo-0.5.0/src/placo/kinematics/kinematics_solver.h`

 * *Files 2% similar despite different names*

```diff
@@ -296,14 +296,20 @@
    * @brief Constructs the QP problem and solves it
    * @param apply apply the solution to the robot model
    * @return the vector containing delta q, which are target variations for the robot degrees of freedom.
    */
   Eigen::VectorXd solve(bool apply = false);
 
   /**
+   * @brief Adds some noise on the configuration of the robot (q)
+   * @param noise noise level, expressed in ratio of the joint limits
+   */
+  void add_q_noise(double noise = 1e-5);
+
+  /**
    * @brief Masks (disables a DoF) from being used by the QP solver (it can't provide speed)
    * @param dof the dof name
    */
   void mask_dof(std::string dof);
 
   /**
    * @brief Unmsks (enables a DoF) from being used by the QP solver (it can provide speed)
@@ -376,19 +382,14 @@
 
   /**
    * @brief Size of the problem (number of variables)
    */
   int N;
 
   /**
-   * @brief Some configuration noise added before solving
-   */
-  double noise = 1e-5;
-
-  /**
    * @brief solver dt (for speeds limiting)
    */
   double dt = 0.;
 
   /**
    * @brief scale obtained when using tasks scaling
    */
```

### Comparing `placo-0.4.9/src/placo/kinematics/kinetic_energy_regularization_task.cpp` & `placo-0.5.0/src/placo/kinematics/kinetic_energy_regularization_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/orientation_task.cpp` & `placo-0.5.0/src/placo/kinematics/orientation_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/orientation_task.h` & `placo-0.5.0/src/placo/kinematics/orientation_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/position_task.cpp` & `placo-0.5.0/src/placo/kinematics/position_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/position_task.h` & `placo-0.5.0/src/placo/kinematics/position_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/regularization_task.cpp` & `placo-0.5.0/src/placo/kinematics/regularization_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/relative_frame_task.cpp` & `placo-0.5.0/src/placo/kinematics/relative_frame_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/relative_frame_task.h` & `placo-0.5.0/src/placo/kinematics/relative_frame_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/relative_orientation_task.cpp` & `placo-0.5.0/src/placo/kinematics/relative_orientation_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/relative_orientation_task.h` & `placo-0.5.0/src/placo/kinematics/relative_orientation_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/relative_position_task.cpp` & `placo-0.5.0/src/placo/kinematics/relative_position_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/relative_position_task.h` & `placo-0.5.0/src/placo/kinematics/relative_position_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/task.h` & `placo-0.5.0/src/placo/kinematics/task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/wheel_task.cpp` & `placo-0.5.0/src/placo/kinematics/wheel_task.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/kinematics/wheel_task.h` & `placo-0.5.0/src/placo/kinematics/wheel_task.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/model/robot_wrapper.cpp` & `placo-0.5.0/src/placo/model/robot_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/model/robot_wrapper.h` & `placo-0.5.0/src/placo/model/robot_wrapper.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/problem/constraint.cpp` & `placo-0.5.0/src/placo/problem/constraint.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/problem/constraint.h` & `placo-0.5.0/src/placo/problem/constraint.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/problem/expression.cpp` & `placo-0.5.0/src/placo/problem/expression.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/problem/expression.h` & `placo-0.5.0/src/placo/problem/expression.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/problem/integrator.cpp` & `placo-0.5.0/src/placo/problem/integrator.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/problem/integrator.h` & `placo-0.5.0/src/placo/problem/integrator.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/problem/polygon_constraint.cpp` & `placo-0.5.0/src/placo/problem/polygon_constraint.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/problem/polygon_constraint.h` & `placo-0.5.0/src/placo/problem/polygon_constraint.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/problem/problem.cpp` & `placo-0.5.0/src/placo/problem/problem.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/problem/problem.h` & `placo-0.5.0/src/placo/problem/problem.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/problem/sparsity.cpp` & `placo-0.5.0/src/placo/problem/sparsity.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/problem/sparsity.h` & `placo-0.5.0/src/placo/problem/sparsity.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/problem/variable.h` & `placo-0.5.0/src/placo/problem/variable.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/tools/axises_mask.cpp` & `placo-0.5.0/src/placo/tools/axises_mask.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/tools/axises_mask.h` & `placo-0.5.0/src/placo/tools/axises_mask.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/tools/cubic_spline.cpp` & `placo-0.5.0/src/placo/tools/cubic_spline.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/tools/cubic_spline.h` & `placo-0.5.0/src/placo/tools/cubic_spline.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/tools/cubic_spline_3d.cpp` & `placo-0.5.0/src/placo/tools/cubic_spline_3d.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/tools/cubic_spline_3d.h` & `placo-0.5.0/src/placo/tools/cubic_spline_3d.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/tools/prioritized.cpp` & `placo-0.5.0/src/placo/tools/prioritized.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/tools/prioritized.h` & `placo-0.5.0/src/placo/tools/prioritized.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/tools/utils.cpp` & `placo-0.5.0/src/placo/tools/utils.cpp`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/src/placo/tools/utils.h` & `placo-0.5.0/src/placo/tools/utils.h`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/stubs.py` & `placo-0.5.0/stubs.py`

 * *Files identical despite different names*

### Comparing `placo-0.4.9/PKG-INFO` & `placo-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: placo
-Version: 0.4.9
+Version: 0.5.0
 Summary: PlaCo: Rhoban Planning and Control
 Requires-Python: >= 3.8
 License-Expression: MIT
 Author-email: Rhoban team <team@rhoban.com>
 Project-URL: Changelog, https://github.com/rhoban/placo/blob/main/CHANGELOG.md
 Home-page: https://placo.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/rhoban/placo.git
```

### Comparing `placo-0.4.9/placo.pyi` & `placo-0.5.0/placo.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4379,14 +4379,25 @@
     :param frame: the robot frame we want to control 
 
     :param target_world: the target position, expressed in the world (as T_world_frame) 
 
     :return: position task"""
     ...
 
+  def add_q_noise(
+    self: KinematicsSolver,
+    noise: float = 1e-5, # double
+
+  ) -> None:
+    """Adds some noise on the configuration of the robot (q) 
+        
+
+    :param noise: noise level, expressed in ratio of the joint limits"""
+    ...
+
   def add_regularization_task(
     self: KinematicsSolver,
     magnitude: float = 1e-6, # double
 
   ) -> RegularizationTask:
     """Adds a regularization task for a given magnitude. 
         
@@ -4528,18 +4539,14 @@
     self: KinematicsSolver,
     masked: bool, # bool
 
   ) -> None:
     """Decides if the floating base should be masked."""
     ...
 
-  noise: float # double
-  """Some configuration noise added before solving. 
-        """
-
   problem: Problem # placo::problem::Problem
   """The underlying QP problem. 
         """
 
   def remove_constraint(
     self: KinematicsSolver,
     constraint: KinematicsConstraint, # placo::kinematics::Constraint
```

