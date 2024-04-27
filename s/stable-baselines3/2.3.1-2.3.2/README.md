# Comparing `tmp/stable_baselines3-2.3.1.tar.gz` & `tmp/stable_baselines3-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable_baselines3-2.3.1.tar", last modified: Mon Apr 22 08:04:39 2024, max compression
+gzip compressed data, was "stable_baselines3-2.3.2.tar", last modified: Sat Apr 27 13:09:01 2024, max compression
```

## Comparing `stable_baselines3-2.3.1.tar` & `stable_baselines3-2.3.2.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-22 08:04:39.454496 stable_baselines3-2.3.1/
--rw-r--r--   0 antonin   (1000) antonin   (1000)     1075 2020-03-18 13:32:59.000000 stable_baselines3-2.3.1/LICENSE
--rw-r--r--   0 antonin   (1000) antonin   (1000)     1338 2020-07-16 10:57:35.000000 stable_baselines3-2.3.1/NOTICE
--rw-r--r--   0 antonin   (1000) antonin   (1000)     5012 2024-04-22 08:04:39.450497 stable_baselines3-2.3.1/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14533 2024-04-22 08:04:27.000000 stable_baselines3-2.3.1/README.md
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1662 2024-04-22 07:37:26.000000 stable_baselines3-2.3.1/pyproject.toml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2024-04-22 08:04:39.454496 stable_baselines3-2.3.1/setup.cfg
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5608 2024-03-11 12:53:17.000000 stable_baselines3-2.3.1/setup.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-22 08:04:39.430496 stable_baselines3-2.3.1/stable_baselines3/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      939 2024-02-18 14:46:23.000000 stable_baselines3-2.3.1/stable_baselines3/__init__.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-22 08:04:39.434496 stable_baselines3-2.3.1/stable_baselines3/a2c/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.1/stable_baselines3/a2c/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9207 2023-12-07 09:45:38.000000 stable_baselines3-2.3.1/stable_baselines3/a2c/a2c.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.3.1/stable_baselines3/a2c/policies.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-22 08:04:39.438496 stable_baselines3-2.3.1/stable_baselines3/common/
--rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-10-07 09:00:57.000000 stable_baselines3-2.3.1/stable_baselines3/common/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11290 2023-11-08 08:47:59.000000 stable_baselines3-2.3.1/stable_baselines3/common/atari_wrappers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    37032 2024-03-04 19:02:06.000000 stable_baselines3-2.3.1/stable_baselines3/common/base_class.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    34544 2023-11-08 16:24:09.000000 stable_baselines3-2.3.1/stable_baselines3/common/buffers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    26933 2023-11-08 08:47:59.000000 stable_baselines3-2.3.1/stable_baselines3/common/callbacks.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    27792 2024-03-04 19:02:06.000000 stable_baselines3-2.3.1/stable_baselines3/common/distributions.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    22098 2024-03-04 19:02:06.000000 stable_baselines3-2.3.1/stable_baselines3/common/env_checker.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7630 2023-10-23 10:24:06.000000 stable_baselines3-2.3.1/stable_baselines3/common/env_util.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-22 08:04:39.438496 stable_baselines3-2.3.1/stable_baselines3/common/envs/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      533 2023-01-25 14:44:15.000000 stable_baselines3-2.3.1/stable_baselines3/common/envs/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9212 2023-10-23 10:19:05.000000 stable_baselines3-2.3.1/stable_baselines3/common/envs/bit_flipping_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6029 2023-05-08 12:31:56.000000 stable_baselines3-2.3.1/stable_baselines3/common/envs/identity_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6499 2023-10-23 10:19:05.000000 stable_baselines3-2.3.1/stable_baselines3/common/envs/multi_input_envs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6451 2023-04-14 11:14:22.000000 stable_baselines3-2.3.1/stable_baselines3/common/evaluation.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    24237 2023-10-23 10:19:05.000000 stable_baselines3-2.3.1/stable_baselines3/common/logger.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9088 2023-11-08 08:47:59.000000 stable_baselines3-2.3.1/stable_baselines3/common/monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5541 2023-05-20 08:31:13.000000 stable_baselines3-2.3.1/stable_baselines3/common/noise.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    26840 2023-12-07 09:45:38.000000 stable_baselines3-2.3.1/stable_baselines3/common/off_policy_algorithm.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13417 2024-03-22 11:17:06.000000 stable_baselines3-2.3.1/stable_baselines3/common/on_policy_algorithm.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    42975 2024-03-11 12:53:17.000000 stable_baselines3-2.3.1/stable_baselines3/common/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8901 2023-11-08 08:47:59.000000 stable_baselines3-2.3.1/stable_baselines3/common/preprocessing.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4326 2023-03-12 17:58:51.000000 stable_baselines3-2.3.1/stable_baselines3/common/results_plotter.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2012 2023-01-25 14:44:15.000000 stable_baselines3-2.3.1/stable_baselines3/common/running_mean_std.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    21304 2024-04-18 16:04:01.000000 stable_baselines3-2.3.1/stable_baselines3/common/save_util.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-22 08:04:39.438496 stable_baselines3-2.3.1/stable_baselines3/common/sb2_compat/
--rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-08-06 19:36:01.000000 stable_baselines3-2.3.1/stable_baselines3/common/sb2_compat/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5651 2023-10-23 10:19:05.000000 stable_baselines3-2.3.1/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13722 2023-05-22 09:05:45.000000 stable_baselines3-2.3.1/stable_baselines3/common/torch_layers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3189 2024-02-13 10:36:31.000000 stable_baselines3-2.3.1/stable_baselines3/common/type_aliases.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    21072 2024-04-22 08:04:27.000000 stable_baselines3-2.3.1/stable_baselines3/common/utils.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-22 08:04:39.442496 stable_baselines3-2.3.1/stable_baselines3/common/vec_env/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4382 2023-11-08 08:47:59.000000 stable_baselines3-2.3.1/stable_baselines3/common/vec_env/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    18460 2023-11-08 08:47:59.000000 stable_baselines3-2.3.1/stable_baselines3/common/vec_env/base_vec_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6966 2023-11-08 08:47:59.000000 stable_baselines3-2.3.1/stable_baselines3/common/vec_env/dummy_vec_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3432 2023-10-23 10:19:05.000000 stable_baselines3-2.3.1/stable_baselines3/common/vec_env/patch_gym.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8063 2023-10-23 10:19:05.000000 stable_baselines3-2.3.1/stable_baselines3/common/vec_env/stacked_observations.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10514 2023-11-16 16:18:52.000000 stable_baselines3-2.3.1/stable_baselines3/common/vec_env/subproc_vec_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3043 2024-02-13 10:36:31.000000 stable_baselines3-2.3.1/stable_baselines3/common/vec_env/util.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4239 2023-04-14 11:14:22.000000 stable_baselines3-2.3.1/stable_baselines3/common/vec_env/vec_check_nan.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1194 2023-05-05 11:41:26.000000 stable_baselines3-2.3.1/stable_baselines3/common/vec_env/vec_extract_dict_obs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2109 2024-03-20 11:34:49.000000 stable_baselines3-2.3.1/stable_baselines3/common/vec_env/vec_frame_stack.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3892 2023-05-05 11:41:26.000000 stable_baselines3-2.3.1/stable_baselines3/common/vec_env/vec_monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13429 2023-11-08 08:47:59.000000 stable_baselines3-2.3.1/stable_baselines3/common/vec_env/vec_normalize.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4552 2023-09-03 09:35:50.000000 stable_baselines3-2.3.1/stable_baselines3/common/vec_env/vec_transpose.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3887 2023-09-03 09:35:50.000000 stable_baselines3-2.3.1/stable_baselines3/common/vec_env/vec_video_recorder.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-22 08:04:39.442496 stable_baselines3-2.3.1/stable_baselines3/ddpg/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      194 2023-01-25 14:44:15.000000 stable_baselines3-2.3.1/stable_baselines3/ddpg/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5718 2024-01-22 10:13:26.000000 stable_baselines3-2.3.1/stable_baselines3/ddpg/ddpg.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      139 2022-03-31 10:10:15.000000 stable_baselines3-2.3.1/stable_baselines3/ddpg/policies.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-22 08:04:39.442496 stable_baselines3-2.3.1/stable_baselines3/dqn/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.1/stable_baselines3/dqn/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    12859 2024-01-22 10:13:26.000000 stable_baselines3-2.3.1/stable_baselines3/dqn/dqn.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10689 2023-11-08 08:47:59.000000 stable_baselines3-2.3.1/stable_baselines3/dqn/policies.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-22 08:04:39.442496 stable_baselines3-2.3.1/stable_baselines3/her/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      204 2023-01-25 14:44:15.000000 stable_baselines3-2.3.1/stable_baselines3/her/__init__.py
--rw-r--r--   0 antonin   (1000) antonin   (1000)      649 2020-10-24 10:56:51.000000 stable_baselines3-2.3.1/stable_baselines3/her/goal_selection_strategy.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    18963 2023-10-23 10:19:05.000000 stable_baselines3-2.3.1/stable_baselines3/her/her_replay_buffer.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-22 08:04:39.442496 stable_baselines3-2.3.1/stable_baselines3/ppo/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.1/stable_baselines3/ppo/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.3.1/stable_baselines3/ppo/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    15455 2024-03-31 11:40:54.000000 stable_baselines3-2.3.1/stable_baselines3/ppo/ppo.py
--rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-07-16 10:57:35.000000 stable_baselines3-2.3.1/stable_baselines3/py.typed
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-22 08:04:39.442496 stable_baselines3-2.3.1/stable_baselines3/sac/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.1/stable_baselines3/sac/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20687 2023-11-08 08:47:59.000000 stable_baselines3-2.3.1/stable_baselines3/sac/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    15940 2023-12-07 09:45:38.000000 stable_baselines3-2.3.1/stable_baselines3/sac/sac.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-22 08:04:39.446496 stable_baselines3-2.3.1/stable_baselines3/td3/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.1/stable_baselines3/td3/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14486 2023-12-13 10:36:46.000000 stable_baselines3-2.3.1/stable_baselines3/td3/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11199 2024-01-22 10:13:26.000000 stable_baselines3-2.3.1/stable_baselines3/td3/td3.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        6 2024-04-22 08:04:27.000000 stable_baselines3-2.3.1/stable_baselines3/version.txt
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-22 08:04:39.450497 stable_baselines3-2.3.1/stable_baselines3.egg-info/
--rw-r--r--   0 antonin   (1000) antonin   (1000)     5012 2024-04-22 08:04:39.000000 stable_baselines3-2.3.1/stable_baselines3.egg-info/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3614 2024-04-22 08:04:39.000000 stable_baselines3-2.3.1/stable_baselines3.egg-info/SOURCES.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2024-04-22 08:04:39.000000 stable_baselines3-2.3.1/stable_baselines3.egg-info/dependency_links.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      498 2024-04-22 08:04:39.000000 stable_baselines3-2.3.1/stable_baselines3.egg-info/requires.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       18 2024-04-22 08:04:39.000000 stable_baselines3-2.3.1/stable_baselines3.egg-info/top_level.txt
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-22 08:04:39.450497 stable_baselines3-2.3.1/tests/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6515 2023-11-08 16:24:09.000000 stable_baselines3-2.3.1/tests/test_buffers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9523 2023-11-08 08:47:59.000000 stable_baselines3-2.3.1/tests/test_callbacks.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13692 2023-04-14 11:14:22.000000 stable_baselines3-2.3.1/tests/test_cnn.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2360 2023-01-25 14:44:15.000000 stable_baselines3-2.3.1/tests/test_custom_policy.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1362 2023-05-14 15:40:24.000000 stable_baselines3-2.3.1/tests/test_deterministic.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11765 2023-06-22 12:07:17.000000 stable_baselines3-2.3.1/tests/test_dict_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9900 2023-04-14 11:14:22.000000 stable_baselines3-2.3.1/tests/test_distributions.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6309 2023-10-23 10:32:57.000000 stable_baselines3-2.3.1/tests/test_env_checker.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10404 2024-03-04 19:02:06.000000 stable_baselines3-2.3.1/tests/test_envs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6776 2024-02-04 22:19:06.000000 stable_baselines3-2.3.1/tests/test_gae.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    16880 2023-12-07 09:40:18.000000 stable_baselines3-2.3.1/tests/test_her.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1989 2023-04-14 11:14:22.000000 stable_baselines3-2.3.1/tests/test_identity.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    19287 2024-03-22 11:17:06.000000 stable_baselines3-2.3.1/tests/test_logger.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3957 2023-04-14 11:14:22.000000 stable_baselines3-2.3.1/tests/test_monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4031 2023-10-23 10:34:51.000000 stable_baselines3-2.3.1/tests/test_predict.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2429 2023-04-14 11:14:22.000000 stable_baselines3-2.3.1/tests/test_preprocessing.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7403 2023-11-08 16:24:09.000000 stable_baselines3-2.3.1/tests/test_run.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    29554 2024-04-22 08:04:27.000000 stable_baselines3-2.3.1/tests/test_save_load.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4271 2023-10-23 10:19:05.000000 stable_baselines3-2.3.1/tests/test_sde.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5480 2023-11-08 08:47:59.000000 stable_baselines3-2.3.1/tests/test_spaces.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2978 2023-01-25 14:44:15.000000 stable_baselines3-2.3.1/tests/test_tensorboard.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13175 2023-04-14 11:14:22.000000 stable_baselines3-2.3.1/tests/test_train_eval_mode.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    22783 2024-04-22 07:09:23.000000 stable_baselines3-2.3.1/tests/test_utils.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1398 2023-10-23 10:35:07.000000 stable_baselines3-2.3.1/tests/test_vec_check_nan.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    21829 2023-11-08 08:47:59.000000 stable_baselines3-2.3.1/tests/test_vec_envs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2941 2023-06-07 14:35:29.000000 stable_baselines3-2.3.1/tests/test_vec_extract_dict_obs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5276 2023-04-14 11:14:22.000000 stable_baselines3-2.3.1/tests/test_vec_monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    17740 2023-10-23 10:19:05.000000 stable_baselines3-2.3.1/tests/test_vec_normalize.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14821 2023-04-14 11:14:22.000000 stable_baselines3-2.3.1/tests/test_vec_stacked_obs.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-27 13:09:01.190329 stable_baselines3-2.3.2/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1075 2020-03-18 13:32:59.000000 stable_baselines3-2.3.2/LICENSE
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1338 2020-07-16 10:57:35.000000 stable_baselines3-2.3.2/NOTICE
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     5012 2024-04-27 13:09:01.190329 stable_baselines3-2.3.2/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14533 2024-04-22 08:04:27.000000 stable_baselines3-2.3.2/README.md
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1662 2024-04-22 07:37:26.000000 stable_baselines3-2.3.2/pyproject.toml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2024-04-27 13:09:01.190329 stable_baselines3-2.3.2/setup.cfg
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5608 2024-03-11 12:53:17.000000 stable_baselines3-2.3.2/setup.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-27 13:09:01.162329 stable_baselines3-2.3.2/stable_baselines3/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      939 2024-02-18 14:46:23.000000 stable_baselines3-2.3.2/stable_baselines3/__init__.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-27 13:09:01.162329 stable_baselines3-2.3.2/stable_baselines3/a2c/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.2/stable_baselines3/a2c/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9207 2023-12-07 09:45:38.000000 stable_baselines3-2.3.2/stable_baselines3/a2c/a2c.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.3.2/stable_baselines3/a2c/policies.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-27 13:09:01.170329 stable_baselines3-2.3.2/stable_baselines3/common/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-10-07 09:00:57.000000 stable_baselines3-2.3.2/stable_baselines3/common/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11290 2023-11-08 08:47:59.000000 stable_baselines3-2.3.2/stable_baselines3/common/atari_wrappers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    37032 2024-03-04 19:02:06.000000 stable_baselines3-2.3.2/stable_baselines3/common/base_class.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    34544 2023-11-08 16:24:09.000000 stable_baselines3-2.3.2/stable_baselines3/common/buffers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    26933 2023-11-08 08:47:59.000000 stable_baselines3-2.3.2/stable_baselines3/common/callbacks.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    27792 2024-03-04 19:02:06.000000 stable_baselines3-2.3.2/stable_baselines3/common/distributions.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    22098 2024-03-04 19:02:06.000000 stable_baselines3-2.3.2/stable_baselines3/common/env_checker.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7630 2023-10-23 10:24:06.000000 stable_baselines3-2.3.2/stable_baselines3/common/env_util.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-27 13:09:01.170329 stable_baselines3-2.3.2/stable_baselines3/common/envs/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      533 2023-01-25 14:44:15.000000 stable_baselines3-2.3.2/stable_baselines3/common/envs/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9212 2023-10-23 10:19:05.000000 stable_baselines3-2.3.2/stable_baselines3/common/envs/bit_flipping_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6029 2023-05-08 12:31:56.000000 stable_baselines3-2.3.2/stable_baselines3/common/envs/identity_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6499 2023-10-23 10:19:05.000000 stable_baselines3-2.3.2/stable_baselines3/common/envs/multi_input_envs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6451 2023-04-14 11:14:22.000000 stable_baselines3-2.3.2/stable_baselines3/common/evaluation.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    24237 2023-10-23 10:19:05.000000 stable_baselines3-2.3.2/stable_baselines3/common/logger.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9088 2023-11-08 08:47:59.000000 stable_baselines3-2.3.2/stable_baselines3/common/monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5541 2023-05-20 08:31:13.000000 stable_baselines3-2.3.2/stable_baselines3/common/noise.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    26840 2023-12-07 09:45:38.000000 stable_baselines3-2.3.2/stable_baselines3/common/off_policy_algorithm.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    13417 2024-03-22 11:17:06.000000 stable_baselines3-2.3.2/stable_baselines3/common/on_policy_algorithm.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    42975 2024-03-11 12:53:17.000000 stable_baselines3-2.3.2/stable_baselines3/common/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8901 2023-11-08 08:47:59.000000 stable_baselines3-2.3.2/stable_baselines3/common/preprocessing.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4326 2023-03-12 17:58:51.000000 stable_baselines3-2.3.2/stable_baselines3/common/results_plotter.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2012 2023-01-25 14:44:15.000000 stable_baselines3-2.3.2/stable_baselines3/common/running_mean_std.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    21419 2024-04-27 13:08:50.000000 stable_baselines3-2.3.2/stable_baselines3/common/save_util.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-27 13:09:01.170329 stable_baselines3-2.3.2/stable_baselines3/common/sb2_compat/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-08-06 19:36:01.000000 stable_baselines3-2.3.2/stable_baselines3/common/sb2_compat/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5651 2023-10-23 10:19:05.000000 stable_baselines3-2.3.2/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    13722 2023-05-22 09:05:45.000000 stable_baselines3-2.3.2/stable_baselines3/common/torch_layers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3189 2024-02-13 10:36:31.000000 stable_baselines3-2.3.2/stable_baselines3/common/type_aliases.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    21072 2024-04-22 08:04:27.000000 stable_baselines3-2.3.2/stable_baselines3/common/utils.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-27 13:09:01.174329 stable_baselines3-2.3.2/stable_baselines3/common/vec_env/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4382 2023-11-08 08:47:59.000000 stable_baselines3-2.3.2/stable_baselines3/common/vec_env/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    18460 2023-11-08 08:47:59.000000 stable_baselines3-2.3.2/stable_baselines3/common/vec_env/base_vec_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6966 2023-11-08 08:47:59.000000 stable_baselines3-2.3.2/stable_baselines3/common/vec_env/dummy_vec_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3432 2023-10-23 10:19:05.000000 stable_baselines3-2.3.2/stable_baselines3/common/vec_env/patch_gym.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8063 2023-10-23 10:19:05.000000 stable_baselines3-2.3.2/stable_baselines3/common/vec_env/stacked_observations.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    10514 2023-11-16 16:18:52.000000 stable_baselines3-2.3.2/stable_baselines3/common/vec_env/subproc_vec_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3043 2024-02-13 10:36:31.000000 stable_baselines3-2.3.2/stable_baselines3/common/vec_env/util.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4239 2023-04-14 11:14:22.000000 stable_baselines3-2.3.2/stable_baselines3/common/vec_env/vec_check_nan.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1194 2023-05-05 11:41:26.000000 stable_baselines3-2.3.2/stable_baselines3/common/vec_env/vec_extract_dict_obs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2109 2024-03-20 11:34:49.000000 stable_baselines3-2.3.2/stable_baselines3/common/vec_env/vec_frame_stack.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3892 2023-05-05 11:41:26.000000 stable_baselines3-2.3.2/stable_baselines3/common/vec_env/vec_monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    13429 2023-11-08 08:47:59.000000 stable_baselines3-2.3.2/stable_baselines3/common/vec_env/vec_normalize.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4552 2023-09-03 09:35:50.000000 stable_baselines3-2.3.2/stable_baselines3/common/vec_env/vec_transpose.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3887 2023-09-03 09:35:50.000000 stable_baselines3-2.3.2/stable_baselines3/common/vec_env/vec_video_recorder.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-27 13:09:01.174329 stable_baselines3-2.3.2/stable_baselines3/ddpg/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      194 2023-01-25 14:44:15.000000 stable_baselines3-2.3.2/stable_baselines3/ddpg/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5718 2024-01-22 10:13:26.000000 stable_baselines3-2.3.2/stable_baselines3/ddpg/ddpg.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      139 2022-03-31 10:10:15.000000 stable_baselines3-2.3.2/stable_baselines3/ddpg/policies.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-27 13:09:01.174329 stable_baselines3-2.3.2/stable_baselines3/dqn/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.2/stable_baselines3/dqn/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    12859 2024-01-22 10:13:26.000000 stable_baselines3-2.3.2/stable_baselines3/dqn/dqn.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    10689 2023-11-08 08:47:59.000000 stable_baselines3-2.3.2/stable_baselines3/dqn/policies.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-27 13:09:01.174329 stable_baselines3-2.3.2/stable_baselines3/her/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      204 2023-01-25 14:44:15.000000 stable_baselines3-2.3.2/stable_baselines3/her/__init__.py
+-rw-r--r--   0 antonin   (1000) antonin   (1000)      649 2020-10-24 10:56:51.000000 stable_baselines3-2.3.2/stable_baselines3/her/goal_selection_strategy.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    18963 2023-10-23 10:19:05.000000 stable_baselines3-2.3.2/stable_baselines3/her/her_replay_buffer.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-27 13:09:01.178329 stable_baselines3-2.3.2/stable_baselines3/ppo/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.2/stable_baselines3/ppo/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.3.2/stable_baselines3/ppo/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    15455 2024-03-31 11:40:54.000000 stable_baselines3-2.3.2/stable_baselines3/ppo/ppo.py
+-rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-07-16 10:57:35.000000 stable_baselines3-2.3.2/stable_baselines3/py.typed
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-27 13:09:01.178329 stable_baselines3-2.3.2/stable_baselines3/sac/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.2/stable_baselines3/sac/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20687 2023-11-08 08:47:59.000000 stable_baselines3-2.3.2/stable_baselines3/sac/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    15940 2023-12-07 09:45:38.000000 stable_baselines3-2.3.2/stable_baselines3/sac/sac.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-27 13:09:01.178329 stable_baselines3-2.3.2/stable_baselines3/td3/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.3.2/stable_baselines3/td3/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14486 2023-12-13 10:36:46.000000 stable_baselines3-2.3.2/stable_baselines3/td3/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11199 2024-01-22 10:13:26.000000 stable_baselines3-2.3.2/stable_baselines3/td3/td3.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        6 2024-04-27 13:08:50.000000 stable_baselines3-2.3.2/stable_baselines3/version.txt
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-27 13:09:01.186329 stable_baselines3-2.3.2/stable_baselines3.egg-info/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     5012 2024-04-27 13:09:01.000000 stable_baselines3-2.3.2/stable_baselines3.egg-info/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3614 2024-04-27 13:09:01.000000 stable_baselines3-2.3.2/stable_baselines3.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2024-04-27 13:09:01.000000 stable_baselines3-2.3.2/stable_baselines3.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      498 2024-04-27 13:09:01.000000 stable_baselines3-2.3.2/stable_baselines3.egg-info/requires.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       18 2024-04-27 13:09:01.000000 stable_baselines3-2.3.2/stable_baselines3.egg-info/top_level.txt
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2024-04-27 13:09:01.186329 stable_baselines3-2.3.2/tests/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6515 2023-11-08 16:24:09.000000 stable_baselines3-2.3.2/tests/test_buffers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9523 2023-11-08 08:47:59.000000 stable_baselines3-2.3.2/tests/test_callbacks.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    13692 2023-04-14 11:14:22.000000 stable_baselines3-2.3.2/tests/test_cnn.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2360 2023-01-25 14:44:15.000000 stable_baselines3-2.3.2/tests/test_custom_policy.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1362 2023-05-14 15:40:24.000000 stable_baselines3-2.3.2/tests/test_deterministic.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11765 2023-06-22 12:07:17.000000 stable_baselines3-2.3.2/tests/test_dict_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9900 2023-04-14 11:14:22.000000 stable_baselines3-2.3.2/tests/test_distributions.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6309 2023-10-23 10:32:57.000000 stable_baselines3-2.3.2/tests/test_env_checker.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    10404 2024-03-04 19:02:06.000000 stable_baselines3-2.3.2/tests/test_envs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6776 2024-02-04 22:19:06.000000 stable_baselines3-2.3.2/tests/test_gae.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    16880 2023-12-07 09:40:18.000000 stable_baselines3-2.3.2/tests/test_her.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1989 2023-04-14 11:14:22.000000 stable_baselines3-2.3.2/tests/test_identity.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    19287 2024-03-22 11:17:06.000000 stable_baselines3-2.3.2/tests/test_logger.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3957 2023-04-14 11:14:22.000000 stable_baselines3-2.3.2/tests/test_monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4031 2023-10-23 10:34:51.000000 stable_baselines3-2.3.2/tests/test_predict.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2429 2023-04-14 11:14:22.000000 stable_baselines3-2.3.2/tests/test_preprocessing.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7403 2023-11-08 16:24:09.000000 stable_baselines3-2.3.2/tests/test_run.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    29554 2024-04-22 08:04:27.000000 stable_baselines3-2.3.2/tests/test_save_load.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4271 2023-10-23 10:19:05.000000 stable_baselines3-2.3.2/tests/test_sde.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5480 2023-11-08 08:47:59.000000 stable_baselines3-2.3.2/tests/test_spaces.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2978 2023-01-25 14:44:15.000000 stable_baselines3-2.3.2/tests/test_tensorboard.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    13175 2023-04-14 11:14:22.000000 stable_baselines3-2.3.2/tests/test_train_eval_mode.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    22783 2024-04-22 07:09:23.000000 stable_baselines3-2.3.2/tests/test_utils.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1398 2023-10-23 10:35:07.000000 stable_baselines3-2.3.2/tests/test_vec_check_nan.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    21829 2023-11-08 08:47:59.000000 stable_baselines3-2.3.2/tests/test_vec_envs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2941 2023-06-07 14:35:29.000000 stable_baselines3-2.3.2/tests/test_vec_extract_dict_obs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5276 2023-04-14 11:14:22.000000 stable_baselines3-2.3.2/tests/test_vec_monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    17740 2023-10-23 10:19:05.000000 stable_baselines3-2.3.2/tests/test_vec_normalize.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14821 2023-04-14 11:14:22.000000 stable_baselines3-2.3.2/tests/test_vec_stacked_obs.py
```

### Comparing `stable_baselines3-2.3.1/LICENSE` & `stable_baselines3-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/NOTICE` & `stable_baselines3-2.3.2/NOTICE`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/PKG-INFO` & `stable_baselines3-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable_baselines3
-Version: 2.3.1
+Version: 2.3.2
 Summary: Pytorch version of Stable Baselines, implementations of reinforcement learning algorithms.
 Home-page: https://github.com/DLR-RM/stable-baselines3
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Project-URL: Code, https://github.com/DLR-RM/stable-baselines3
 Project-URL: Documentation, https://stable-baselines3.readthedocs.io/
```

### Comparing `stable_baselines3-2.3.1/README.md` & `stable_baselines3-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/pyproject.toml` & `stable_baselines3-2.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/setup.py` & `stable_baselines3-2.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/__init__.py` & `stable_baselines3-2.3.2/stable_baselines3/__init__.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/a2c/a2c.py` & `stable_baselines3-2.3.2/stable_baselines3/a2c/a2c.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/atari_wrappers.py` & `stable_baselines3-2.3.2/stable_baselines3/common/atari_wrappers.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/base_class.py` & `stable_baselines3-2.3.2/stable_baselines3/common/base_class.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/buffers.py` & `stable_baselines3-2.3.2/stable_baselines3/common/buffers.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/callbacks.py` & `stable_baselines3-2.3.2/stable_baselines3/common/callbacks.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/distributions.py` & `stable_baselines3-2.3.2/stable_baselines3/common/distributions.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/env_checker.py` & `stable_baselines3-2.3.2/stable_baselines3/common/env_checker.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/env_util.py` & `stable_baselines3-2.3.2/stable_baselines3/common/env_util.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/envs/__init__.py` & `stable_baselines3-2.3.2/stable_baselines3/common/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/envs/bit_flipping_env.py` & `stable_baselines3-2.3.2/stable_baselines3/common/envs/bit_flipping_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/envs/identity_env.py` & `stable_baselines3-2.3.2/stable_baselines3/common/envs/identity_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/envs/multi_input_envs.py` & `stable_baselines3-2.3.2/stable_baselines3/common/envs/multi_input_envs.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/evaluation.py` & `stable_baselines3-2.3.2/stable_baselines3/common/evaluation.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/logger.py` & `stable_baselines3-2.3.2/stable_baselines3/common/logger.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/monitor.py` & `stable_baselines3-2.3.2/stable_baselines3/common/monitor.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/noise.py` & `stable_baselines3-2.3.2/stable_baselines3/common/noise.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/off_policy_algorithm.py` & `stable_baselines3-2.3.2/stable_baselines3/common/off_policy_algorithm.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/on_policy_algorithm.py` & `stable_baselines3-2.3.2/stable_baselines3/common/on_policy_algorithm.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/policies.py` & `stable_baselines3-2.3.2/stable_baselines3/common/policies.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/preprocessing.py` & `stable_baselines3-2.3.2/stable_baselines3/common/preprocessing.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/results_plotter.py` & `stable_baselines3-2.3.2/stable_baselines3/common/results_plotter.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/running_mean_std.py` & `stable_baselines3-2.3.2/stable_baselines3/common/running_mean_std.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/save_util.py` & `stable_baselines3-2.3.2/stable_baselines3/common/save_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -443,15 +443,16 @@
                     # fixed in python >= 3.7
                     file_content = io.BytesIO()
                     file_content.write(param_file.read())
                     # go to start of file
                     file_content.seek(0)
                     # Load the parameters with the right ``map_location``.
                     # Remove ".pth" ending with splitext
-                    th_object = th.load(file_content, map_location=device, weights_only=True)
+                    # Note(antonin): we cannot use weights_only=True, as it breaks with PyTorch 1.13, see GH#1911
+                    th_object = th.load(file_content, map_location=device, weights_only=False)
                     # "tensors.pth" was renamed "pytorch_variables.pth" in v0.9.0, see PR #138
                     if file_path == "pytorch_variables.pth" or file_path == "tensors.pth":
                         # PyTorch variables (not state_dicts)
                         pytorch_variables = th_object
                     else:
                         # State dicts. Store into params dictionary
                         # with same name as in .zip file (without .pth)
```

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py` & `stable_baselines3-2.3.2/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/torch_layers.py` & `stable_baselines3-2.3.2/stable_baselines3/common/torch_layers.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/type_aliases.py` & `stable_baselines3-2.3.2/stable_baselines3/common/type_aliases.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/utils.py` & `stable_baselines3-2.3.2/stable_baselines3/common/utils.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/vec_env/__init__.py` & `stable_baselines3-2.3.2/stable_baselines3/common/vec_env/__init__.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/vec_env/base_vec_env.py` & `stable_baselines3-2.3.2/stable_baselines3/common/vec_env/base_vec_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/vec_env/dummy_vec_env.py` & `stable_baselines3-2.3.2/stable_baselines3/common/vec_env/dummy_vec_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/vec_env/patch_gym.py` & `stable_baselines3-2.3.2/stable_baselines3/common/vec_env/patch_gym.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/vec_env/stacked_observations.py` & `stable_baselines3-2.3.2/stable_baselines3/common/vec_env/stacked_observations.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/vec_env/subproc_vec_env.py` & `stable_baselines3-2.3.2/stable_baselines3/common/vec_env/subproc_vec_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/vec_env/util.py` & `stable_baselines3-2.3.2/stable_baselines3/common/vec_env/util.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/vec_env/vec_check_nan.py` & `stable_baselines3-2.3.2/stable_baselines3/common/vec_env/vec_check_nan.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/vec_env/vec_extract_dict_obs.py` & `stable_baselines3-2.3.2/stable_baselines3/common/vec_env/vec_extract_dict_obs.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/vec_env/vec_frame_stack.py` & `stable_baselines3-2.3.2/stable_baselines3/common/vec_env/vec_frame_stack.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/vec_env/vec_monitor.py` & `stable_baselines3-2.3.2/stable_baselines3/common/vec_env/vec_monitor.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/vec_env/vec_normalize.py` & `stable_baselines3-2.3.2/stable_baselines3/common/vec_env/vec_normalize.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/vec_env/vec_transpose.py` & `stable_baselines3-2.3.2/stable_baselines3/common/vec_env/vec_transpose.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/common/vec_env/vec_video_recorder.py` & `stable_baselines3-2.3.2/stable_baselines3/common/vec_env/vec_video_recorder.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/ddpg/ddpg.py` & `stable_baselines3-2.3.2/stable_baselines3/ddpg/ddpg.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/dqn/dqn.py` & `stable_baselines3-2.3.2/stable_baselines3/dqn/dqn.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/dqn/policies.py` & `stable_baselines3-2.3.2/stable_baselines3/dqn/policies.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/her/goal_selection_strategy.py` & `stable_baselines3-2.3.2/stable_baselines3/her/goal_selection_strategy.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/her/her_replay_buffer.py` & `stable_baselines3-2.3.2/stable_baselines3/her/her_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/ppo/ppo.py` & `stable_baselines3-2.3.2/stable_baselines3/ppo/ppo.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/sac/policies.py` & `stable_baselines3-2.3.2/stable_baselines3/sac/policies.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/sac/sac.py` & `stable_baselines3-2.3.2/stable_baselines3/sac/sac.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/td3/policies.py` & `stable_baselines3-2.3.2/stable_baselines3/td3/policies.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3/td3/td3.py` & `stable_baselines3-2.3.2/stable_baselines3/td3/td3.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/stable_baselines3.egg-info/PKG-INFO` & `stable_baselines3-2.3.2/stable_baselines3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable_baselines3
-Version: 2.3.1
+Version: 2.3.2
 Summary: Pytorch version of Stable Baselines, implementations of reinforcement learning algorithms.
 Home-page: https://github.com/DLR-RM/stable-baselines3
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Project-URL: Code, https://github.com/DLR-RM/stable-baselines3
 Project-URL: Documentation, https://stable-baselines3.readthedocs.io/
```

### Comparing `stable_baselines3-2.3.1/stable_baselines3.egg-info/SOURCES.txt` & `stable_baselines3-2.3.2/stable_baselines3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_buffers.py` & `stable_baselines3-2.3.2/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_callbacks.py` & `stable_baselines3-2.3.2/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_cnn.py` & `stable_baselines3-2.3.2/tests/test_cnn.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_custom_policy.py` & `stable_baselines3-2.3.2/tests/test_custom_policy.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_deterministic.py` & `stable_baselines3-2.3.2/tests/test_deterministic.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_dict_env.py` & `stable_baselines3-2.3.2/tests/test_dict_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_distributions.py` & `stable_baselines3-2.3.2/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_env_checker.py` & `stable_baselines3-2.3.2/tests/test_env_checker.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_envs.py` & `stable_baselines3-2.3.2/tests/test_envs.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_gae.py` & `stable_baselines3-2.3.2/tests/test_gae.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_her.py` & `stable_baselines3-2.3.2/tests/test_her.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_identity.py` & `stable_baselines3-2.3.2/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_logger.py` & `stable_baselines3-2.3.2/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_monitor.py` & `stable_baselines3-2.3.2/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_predict.py` & `stable_baselines3-2.3.2/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_preprocessing.py` & `stable_baselines3-2.3.2/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_run.py` & `stable_baselines3-2.3.2/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_save_load.py` & `stable_baselines3-2.3.2/tests/test_save_load.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_sde.py` & `stable_baselines3-2.3.2/tests/test_sde.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_spaces.py` & `stable_baselines3-2.3.2/tests/test_spaces.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_tensorboard.py` & `stable_baselines3-2.3.2/tests/test_tensorboard.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_train_eval_mode.py` & `stable_baselines3-2.3.2/tests/test_train_eval_mode.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_utils.py` & `stable_baselines3-2.3.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_vec_check_nan.py` & `stable_baselines3-2.3.2/tests/test_vec_check_nan.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_vec_envs.py` & `stable_baselines3-2.3.2/tests/test_vec_envs.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_vec_extract_dict_obs.py` & `stable_baselines3-2.3.2/tests/test_vec_extract_dict_obs.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_vec_monitor.py` & `stable_baselines3-2.3.2/tests/test_vec_monitor.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_vec_normalize.py` & `stable_baselines3-2.3.2/tests/test_vec_normalize.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.3.1/tests/test_vec_stacked_obs.py` & `stable_baselines3-2.3.2/tests/test_vec_stacked_obs.py`

 * *Files identical despite different names*

