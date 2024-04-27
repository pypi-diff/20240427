# Comparing `tmp/pyDecision-4.4.7.tar.gz` & `tmp/pyDecision-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyDecision-4.4.7.tar", last modified: Thu Apr 25 19:14:28 2024, max compression
+gzip compressed data, was "dist\pyDecision-4.5.1.tar", last modified: Sat Apr 27 02:01:25 2024, max compression
```

## Comparing `pyDecision-4.4.7.tar` & `pyDecision-4.5.1.tar`

### file list

```diff
@@ -1,93 +1,99 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 19:14:28.000000 pyDecision-4.4.7/
--rw-rw-rw-   0        0        0      656 2023-10-24 20:28:27.000000 pyDecision-4.4.7/LICENSE
--rw-rw-rw-   0        0        0    18765 2024-04-25 19:14:28.000000 pyDecision-4.4.7/PKG-INFO
--rw-rw-rw-   0        0        0    18270 2024-04-25 15:42:00.000000 pyDecision-4.4.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 19:14:28.000000 pyDecision-4.4.7/pyDecision/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-4.4.7/pyDecision/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 19:14:28.000000 pyDecision-4.4.7/pyDecision/algorithm/
--rw-rw-rw-   0        0        0     2934 2024-04-25 15:49:24.000000 pyDecision-4.4.7/pyDecision/algorithm/__init__.py
--rw-rw-rw-   0        0        0     1638 2023-08-15 11:11:40.000000 pyDecision-4.4.7/pyDecision/algorithm/ahp.py
--rw-rw-rw-   0        0        0     2591 2023-07-21 17:32:54.000000 pyDecision-4.4.7/pyDecision/algorithm/aras.py
--rw-rw-rw-   0        0        0     2147 2023-07-21 20:21:53.000000 pyDecision-4.4.7/pyDecision/algorithm/borda.py
--rw-rw-rw-   0        0        0     2553 2023-11-10 15:52:16.000000 pyDecision-4.4.7/pyDecision/algorithm/bwm.py
--rw-rw-rw-   0        0        0     1006 2023-11-12 15:54:44.000000 pyDecision-4.4.7/pyDecision/algorithm/bwm_s.py
--rw-rw-rw-   0        0        0     1221 2024-04-24 14:49:40.000000 pyDecision-4.4.7/pyDecision/algorithm/cilos.py
--rw-rw-rw-   0        0        0     2762 2023-07-22 02:44:56.000000 pyDecision-4.4.7/pyDecision/algorithm/cocoso.py
--rw-rw-rw-   0        0        0     2754 2023-07-21 17:33:49.000000 pyDecision-4.4.7/pyDecision/algorithm/codas.py
--rw-rw-rw-   0        0        0     2870 2023-07-23 17:00:58.000000 pyDecision-4.4.7/pyDecision/algorithm/copeland.py
--rw-rw-rw-   0        0        0     2471 2023-07-21 17:34:03.000000 pyDecision-4.4.7/pyDecision/algorithm/copras.py
--rw-rw-rw-   0        0        0     2347 2023-07-23 16:38:01.000000 pyDecision-4.4.7/pyDecision/algorithm/cradis.py
--rw-rw-rw-   0        0        0     1125 2023-10-24 20:07:49.000000 pyDecision-4.4.7/pyDecision/algorithm/critic.py
--rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-4.4.7/pyDecision/algorithm/dematel.py
--rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-4.4.7/pyDecision/algorithm/e_i.py
--rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-4.4.7/pyDecision/algorithm/e_i_s.py
--rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-4.4.7/pyDecision/algorithm/e_i_v.py
--rw-rw-rw-   0        0        0    16907 2023-07-21 20:38:15.000000 pyDecision-4.4.7/pyDecision/algorithm/e_ii.py
--rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-4.4.7/pyDecision/algorithm/e_iii.py
--rw-rw-rw-   0        0        0    14298 2023-07-21 19:41:40.000000 pyDecision-4.4.7/pyDecision/algorithm/e_iv.py
--rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-4.4.7/pyDecision/algorithm/e_tri_b.py
--rw-rw-rw-   0        0        0     2711 2023-07-21 20:33:16.000000 pyDecision-4.4.7/pyDecision/algorithm/edas.py
--rw-rw-rw-   0        0        0      925 2023-07-19 01:09:53.000000 pyDecision-4.4.7/pyDecision/algorithm/entropy.py
--rw-rw-rw-   0        0        0     2289 2024-04-24 15:29:47.000000 pyDecision-4.4.7/pyDecision/algorithm/fucom.py
--rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-4.4.7/pyDecision/algorithm/fuzzy_ahp.py
--rw-rw-rw-   0        0        0     3321 2023-07-25 15:17:23.000000 pyDecision-4.4.7/pyDecision/algorithm/fuzzy_aras.py
--rw-rw-rw-   0        0        0     4635 2023-11-12 11:24:00.000000 pyDecision-4.4.7/pyDecision/algorithm/fuzzy_bwm.py
--rw-rw-rw-   0        0        0     4545 2023-07-21 17:31:44.000000 pyDecision-4.4.7/pyDecision/algorithm/fuzzy_copras.py
--rw-rw-rw-   0        0        0     4100 2023-08-01 01:06:41.000000 pyDecision-4.4.7/pyDecision/algorithm/fuzzy_dematel.py
--rw-rw-rw-   0        0        0     5042 2023-07-21 18:03:22.000000 pyDecision-4.4.7/pyDecision/algorithm/fuzzy_edas.py
--rw-rw-rw-   0        0        0     3706 2023-07-21 18:11:21.000000 pyDecision-4.4.7/pyDecision/algorithm/fuzzy_moora.py
--rw-rw-rw-   0        0        0     4098 2023-07-21 18:13:14.000000 pyDecision-4.4.7/pyDecision/algorithm/fuzzy_ocra.py
--rw-rw-rw-   0        0        0     4086 2023-07-21 18:17:14.000000 pyDecision-4.4.7/pyDecision/algorithm/fuzzy_topsis.py
--rw-rw-rw-   0        0        0     5994 2023-07-21 18:18:25.000000 pyDecision-4.4.7/pyDecision/algorithm/fuzzy_vikor.py
--rw-rw-rw-   0        0        0     5399 2023-09-09 01:09:43.000000 pyDecision-4.4.7/pyDecision/algorithm/fuzzy_waspas.py
--rw-rw-rw-   0        0        0     2553 2023-07-22 02:46:58.000000 pyDecision-4.4.7/pyDecision/algorithm/gra.py
--rw-rw-rw-   0        0        0     2300 2023-10-26 23:42:55.000000 pyDecision-4.4.7/pyDecision/algorithm/idocriw.py
--rw-rw-rw-   0        0        0     2585 2023-07-21 18:06:06.000000 pyDecision-4.4.7/pyDecision/algorithm/mabac.py
--rw-rw-rw-   0        0        0     2388 2023-07-28 22:31:36.000000 pyDecision-4.4.7/pyDecision/algorithm/macbeth.py
--rw-rw-rw-   0        0        0     2575 2023-07-23 16:39:11.000000 pyDecision-4.4.7/pyDecision/algorithm/mairca.py
--rw-rw-rw-   0        0        0     2598 2024-04-25 15:20:07.000000 pyDecision-4.4.7/pyDecision/algorithm/mara.py
--rw-rw-rw-   0        0        0     3048 2023-07-21 18:09:18.000000 pyDecision-4.4.7/pyDecision/algorithm/marcos.py
--rw-rw-rw-   0        0        0     3766 2023-07-22 02:46:58.000000 pyDecision-4.4.7/pyDecision/algorithm/maut.py
--rw-rw-rw-   0        0        0     1175 2023-10-26 23:47:00.000000 pyDecision-4.4.7/pyDecision/algorithm/merec.py
--rw-rw-rw-   0        0        0     2541 2023-07-21 18:10:51.000000 pyDecision-4.4.7/pyDecision/algorithm/moora.py
--rw-rw-rw-   0        0        0     2549 2023-07-21 18:12:07.000000 pyDecision-4.4.7/pyDecision/algorithm/moosra.py
--rw-rw-rw-   0        0        0     4968 2023-07-22 01:50:19.000000 pyDecision-4.4.7/pyDecision/algorithm/multimoora.py
--rw-rw-rw-   0        0        0     2477 2023-07-21 23:26:24.000000 pyDecision-4.4.7/pyDecision/algorithm/ocra.py
--rw-rw-rw-   0        0        0     2563 2023-09-09 00:46:31.000000 pyDecision-4.4.7/pyDecision/algorithm/oreste.py
--rw-rw-rw-   0        0        0    13836 2023-10-30 12:17:12.000000 pyDecision-4.4.7/pyDecision/algorithm/p_ec.py
--rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-4.4.7/pyDecision/algorithm/p_i.py
--rw-rw-rw-   0        0        0     5891 2023-07-21 19:40:41.000000 pyDecision-4.4.7/pyDecision/algorithm/p_ii.py
--rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-4.4.7/pyDecision/algorithm/p_iii.py
--rw-rw-rw-   0        0        0     8547 2023-07-21 19:39:42.000000 pyDecision-4.4.7/pyDecision/algorithm/p_iv.py
--rw-rw-rw-   0        0        0     6622 2023-08-02 21:49:15.000000 pyDecision-4.4.7/pyDecision/algorithm/p_v.py
--rw-rw-rw-   0        0        0     9380 2023-07-21 19:37:53.000000 pyDecision-4.4.7/pyDecision/algorithm/p_vi.py
--rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-4.4.7/pyDecision/algorithm/p_xgaia.py
--rw-rw-rw-   0        0        0     2139 2023-07-23 16:40:26.000000 pyDecision-4.4.7/pyDecision/algorithm/piv.py
--rw-rw-rw-   0        0        0     2184 2023-07-21 18:14:04.000000 pyDecision-4.4.7/pyDecision/algorithm/psi.py
--rw-rw-rw-   0        0        0      688 2024-04-25 15:23:46.000000 pyDecision-4.4.7/pyDecision/algorithm/psi_m.py
--rw-rw-rw-   0        0        0     5265 2024-04-25 14:52:15.000000 pyDecision-4.4.7/pyDecision/algorithm/regime.py
--rw-rw-rw-   0        0        0     2434 2023-07-22 02:08:59.000000 pyDecision-4.4.7/pyDecision/algorithm/rov.py
--rw-rw-rw-   0        0        0     2130 2023-07-21 18:14:55.000000 pyDecision-4.4.7/pyDecision/algorithm/saw.py
--rw-rw-rw-   0        0        0     2344 2023-07-21 18:15:17.000000 pyDecision-4.4.7/pyDecision/algorithm/smart.py
--rw-rw-rw-   0        0        0     2185 2023-08-02 00:35:27.000000 pyDecision-4.4.7/pyDecision/algorithm/spotis.py
--rw-rw-rw-   0        0        0     2867 2023-07-21 18:15:39.000000 pyDecision-4.4.7/pyDecision/algorithm/todim.py
--rw-rw-rw-   0        0        0     2600 2023-07-21 18:16:04.000000 pyDecision-4.4.7/pyDecision/algorithm/topsis.py
--rw-rw-rw-   0        0        0     3703 2023-07-22 03:11:26.000000 pyDecision-4.4.7/pyDecision/algorithm/vikor.py
--rw-rw-rw-   0        0        0     4278 2023-09-08 23:55:42.000000 pyDecision-4.4.7/pyDecision/algorithm/waspas.py
--rw-rw-rw-   0        0        0     2643 2023-07-21 18:23:36.000000 pyDecision-4.4.7/pyDecision/algorithm/wings.py
--rw-rw-rw-   0        0        0     3188 2024-04-24 01:11:01.000000 pyDecision-4.4.7/pyDecision/algorithm/wisp.py
-drwxrwxrwx   0        0        0        0 2024-04-25 19:14:28.000000 pyDecision-4.4.7/pyDecision/compare/
--rw-rw-rw-   0        0        0      104 2024-04-25 14:56:00.000000 pyDecision-4.4.7/pyDecision/compare/__init__.py
--rw-rw-rw-   0        0        0    24196 2024-04-25 19:09:15.000000 pyDecision-4.4.7/pyDecision/compare/compare.py
-drwxrwxrwx   0        0        0        0 2024-04-25 19:14:28.000000 pyDecision-4.4.7/pyDecision/util/
--rw-rw-rw-   0        0        0     8733 2023-12-03 18:26:24.000000 pyDecision-4.4.7/pyDecision/util/LLM.py
--rw-rw-rw-   0        0        0      109 2023-08-02 19:44:51.000000 pyDecision-4.4.7/pyDecision/util/__init__.py
--rw-rw-rw-   0        0        0     6266 2023-08-02 19:44:27.000000 pyDecision-4.4.7/pyDecision/util/ga.py
-drwxrwxrwx   0        0        0        0 2024-04-25 19:14:28.000000 pyDecision-4.4.7/pyDecision.egg-info/
--rw-rw-rw-   0        0        0    18765 2024-04-25 19:14:27.000000 pyDecision-4.4.7/pyDecision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2549 2024-04-25 19:14:27.000000 pyDecision-4.4.7/pyDecision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 19:14:27.000000 pyDecision-4.4.7/pyDecision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-25 19:14:27.000000 pyDecision-4.4.7/pyDecision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-25 19:14:27.000000 pyDecision-4.4.7/pyDecision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 19:14:28.000000 pyDecision-4.4.7/setup.cfg
--rw-rw-rw-   0        0        0      744 2024-04-25 19:13:18.000000 pyDecision-4.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 02:01:25.000000 pyDecision-4.5.1/
+-rw-rw-rw-   0        0        0      656 2023-10-24 20:28:27.000000 pyDecision-4.5.1/LICENSE
+-rw-rw-rw-   0        0        0    20106 2024-04-27 02:01:25.000000 pyDecision-4.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0    19604 2024-04-27 01:58:37.000000 pyDecision-4.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 02:01:24.000000 pyDecision-4.5.1/pyDecision/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-4.5.1/pyDecision/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 02:01:25.000000 pyDecision-4.5.1/pyDecision/algorithm/
+-rw-rw-rw-   0        0        0     3187 2024-04-26 23:34:28.000000 pyDecision-4.5.1/pyDecision/algorithm/__init__.py
+-rw-rw-rw-   0        0        0     1638 2023-08-15 11:11:40.000000 pyDecision-4.5.1/pyDecision/algorithm/ahp.py
+-rw-rw-rw-   0        0        0     2591 2023-07-21 17:32:54.000000 pyDecision-4.5.1/pyDecision/algorithm/aras.py
+-rw-rw-rw-   0        0        0     2147 2023-07-21 20:21:53.000000 pyDecision-4.5.1/pyDecision/algorithm/borda.py
+-rw-rw-rw-   0        0        0     2553 2023-11-10 15:52:16.000000 pyDecision-4.5.1/pyDecision/algorithm/bwm.py
+-rw-rw-rw-   0        0        0     1006 2023-11-12 15:54:44.000000 pyDecision-4.5.1/pyDecision/algorithm/bwm_s.py
+-rw-rw-rw-   0        0        0     1221 2024-04-24 14:49:40.000000 pyDecision-4.5.1/pyDecision/algorithm/cilos.py
+-rw-rw-rw-   0        0        0     2762 2023-07-22 02:44:56.000000 pyDecision-4.5.1/pyDecision/algorithm/cocoso.py
+-rw-rw-rw-   0        0        0     2754 2023-07-21 17:33:49.000000 pyDecision-4.5.1/pyDecision/algorithm/codas.py
+-rw-rw-rw-   0        0        0     2870 2023-07-23 17:00:58.000000 pyDecision-4.5.1/pyDecision/algorithm/copeland.py
+-rw-rw-rw-   0        0        0     2471 2023-07-21 17:34:03.000000 pyDecision-4.5.1/pyDecision/algorithm/copras.py
+-rw-rw-rw-   0        0        0     2347 2023-07-23 16:38:01.000000 pyDecision-4.5.1/pyDecision/algorithm/cradis.py
+-rw-rw-rw-   0        0        0     1125 2023-10-24 20:07:49.000000 pyDecision-4.5.1/pyDecision/algorithm/critic.py
+-rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-4.5.1/pyDecision/algorithm/dematel.py
+-rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-4.5.1/pyDecision/algorithm/e_i.py
+-rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-4.5.1/pyDecision/algorithm/e_i_s.py
+-rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-4.5.1/pyDecision/algorithm/e_i_v.py
+-rw-rw-rw-   0        0        0    16907 2023-07-21 20:38:15.000000 pyDecision-4.5.1/pyDecision/algorithm/e_ii.py
+-rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-4.5.1/pyDecision/algorithm/e_iii.py
+-rw-rw-rw-   0        0        0    14298 2023-07-21 19:41:40.000000 pyDecision-4.5.1/pyDecision/algorithm/e_iv.py
+-rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-4.5.1/pyDecision/algorithm/e_tri_b.py
+-rw-rw-rw-   0        0        0     2711 2023-07-21 20:33:16.000000 pyDecision-4.5.1/pyDecision/algorithm/edas.py
+-rw-rw-rw-   0        0        0      925 2023-07-19 01:09:53.000000 pyDecision-4.5.1/pyDecision/algorithm/entropy.py
+-rw-rw-rw-   0        0        0     2289 2024-04-24 15:29:47.000000 pyDecision-4.5.1/pyDecision/algorithm/fucom.py
+-rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_ahp.py
+-rw-rw-rw-   0        0        0     3321 2023-07-25 15:17:23.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_aras.py
+-rw-rw-rw-   0        0        0     4635 2023-11-12 11:24:00.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_bwm.py
+-rw-rw-rw-   0        0        0     4545 2023-07-21 17:31:44.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_copras.py
+-rw-rw-rw-   0        0        0     2500 2024-04-26 21:40:48.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_critic.py
+-rw-rw-rw-   0        0        0     4100 2023-08-01 01:06:41.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_dematel.py
+-rw-rw-rw-   0        0        0     5042 2023-07-21 18:03:22.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_edas.py
+-rw-rw-rw-   0        0        0     5402 2024-04-27 00:21:30.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_fucom.py
+-rw-rw-rw-   0        0        0     1786 2024-04-26 21:41:04.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_merec.py
+-rw-rw-rw-   0        0        0     3706 2023-07-21 18:11:21.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_moora.py
+-rw-rw-rw-   0        0        0     4098 2023-07-21 18:13:14.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_ocra.py
+-rw-rw-rw-   0        0        0     4086 2023-07-21 18:17:14.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_topsis.py
+-rw-rw-rw-   0        0        0     5994 2023-07-21 18:18:25.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_vikor.py
+-rw-rw-rw-   0        0        0     5399 2023-09-09 01:09:43.000000 pyDecision-4.5.1/pyDecision/algorithm/fuzzy_waspas.py
+-rw-rw-rw-   0        0        0     2553 2023-07-22 02:46:58.000000 pyDecision-4.5.1/pyDecision/algorithm/gra.py
+-rw-rw-rw-   0        0        0     2300 2023-10-26 23:42:55.000000 pyDecision-4.5.1/pyDecision/algorithm/idocriw.py
+-rw-rw-rw-   0        0        0     2585 2023-07-21 18:06:06.000000 pyDecision-4.5.1/pyDecision/algorithm/mabac.py
+-rw-rw-rw-   0        0        0     2388 2023-07-28 22:31:36.000000 pyDecision-4.5.1/pyDecision/algorithm/macbeth.py
+-rw-rw-rw-   0        0        0     2575 2023-07-23 16:39:11.000000 pyDecision-4.5.1/pyDecision/algorithm/mairca.py
+-rw-rw-rw-   0        0        0     2598 2024-04-25 15:20:07.000000 pyDecision-4.5.1/pyDecision/algorithm/mara.py
+-rw-rw-rw-   0        0        0     3048 2023-07-21 18:09:18.000000 pyDecision-4.5.1/pyDecision/algorithm/marcos.py
+-rw-rw-rw-   0        0        0     3766 2023-07-22 02:46:58.000000 pyDecision-4.5.1/pyDecision/algorithm/maut.py
+-rw-rw-rw-   0        0        0     1175 2023-10-26 23:47:00.000000 pyDecision-4.5.1/pyDecision/algorithm/merec.py
+-rw-rw-rw-   0        0        0     2541 2023-07-21 18:10:51.000000 pyDecision-4.5.1/pyDecision/algorithm/moora.py
+-rw-rw-rw-   0        0        0     2549 2023-07-21 18:12:07.000000 pyDecision-4.5.1/pyDecision/algorithm/moosra.py
+-rw-rw-rw-   0        0        0     4968 2023-07-22 01:50:19.000000 pyDecision-4.5.1/pyDecision/algorithm/multimoora.py
+-rw-rw-rw-   0        0        0     2477 2023-07-21 23:26:24.000000 pyDecision-4.5.1/pyDecision/algorithm/ocra.py
+-rw-rw-rw-   0        0        0     2563 2023-09-09 00:46:31.000000 pyDecision-4.5.1/pyDecision/algorithm/oreste.py
+-rw-rw-rw-   0        0        0    13836 2023-10-30 12:17:12.000000 pyDecision-4.5.1/pyDecision/algorithm/p_ec.py
+-rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-4.5.1/pyDecision/algorithm/p_i.py
+-rw-rw-rw-   0        0        0     5891 2023-07-21 19:40:41.000000 pyDecision-4.5.1/pyDecision/algorithm/p_ii.py
+-rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-4.5.1/pyDecision/algorithm/p_iii.py
+-rw-rw-rw-   0        0        0     8547 2023-07-21 19:39:42.000000 pyDecision-4.5.1/pyDecision/algorithm/p_iv.py
+-rw-rw-rw-   0        0        0     6622 2023-08-02 21:49:15.000000 pyDecision-4.5.1/pyDecision/algorithm/p_v.py
+-rw-rw-rw-   0        0        0     9380 2023-07-21 19:37:53.000000 pyDecision-4.5.1/pyDecision/algorithm/p_vi.py
+-rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-4.5.1/pyDecision/algorithm/p_xgaia.py
+-rw-rw-rw-   0        0        0     2139 2023-07-23 16:40:26.000000 pyDecision-4.5.1/pyDecision/algorithm/piv.py
+-rw-rw-rw-   0        0        0     2184 2023-07-21 18:14:04.000000 pyDecision-4.5.1/pyDecision/algorithm/psi.py
+-rw-rw-rw-   0        0        0      688 2024-04-25 15:23:46.000000 pyDecision-4.5.1/pyDecision/algorithm/psi_m.py
+-rw-rw-rw-   0        0        0     5265 2024-04-25 14:52:15.000000 pyDecision-4.5.1/pyDecision/algorithm/regime.py
+-rw-rw-rw-   0        0        0      969 2024-04-26 21:38:23.000000 pyDecision-4.5.1/pyDecision/algorithm/roc.py
+-rw-rw-rw-   0        0        0     2434 2023-07-22 02:08:59.000000 pyDecision-4.5.1/pyDecision/algorithm/rov.py
+-rw-rw-rw-   0        0        0      970 2024-04-26 21:39:12.000000 pyDecision-4.5.1/pyDecision/algorithm/rrw.py
+-rw-rw-rw-   0        0        0      929 2024-04-26 21:38:49.000000 pyDecision-4.5.1/pyDecision/algorithm/rsw.py
+-rw-rw-rw-   0        0        0     2130 2023-07-21 18:14:55.000000 pyDecision-4.5.1/pyDecision/algorithm/saw.py
+-rw-rw-rw-   0        0        0     2344 2023-07-21 18:15:17.000000 pyDecision-4.5.1/pyDecision/algorithm/smart.py
+-rw-rw-rw-   0        0        0     2185 2023-08-02 00:35:27.000000 pyDecision-4.5.1/pyDecision/algorithm/spotis.py
+-rw-rw-rw-   0        0        0     2867 2023-07-21 18:15:39.000000 pyDecision-4.5.1/pyDecision/algorithm/todim.py
+-rw-rw-rw-   0        0        0     2600 2023-07-21 18:16:04.000000 pyDecision-4.5.1/pyDecision/algorithm/topsis.py
+-rw-rw-rw-   0        0        0     3703 2023-07-22 03:11:26.000000 pyDecision-4.5.1/pyDecision/algorithm/vikor.py
+-rw-rw-rw-   0        0        0     4278 2023-09-08 23:55:42.000000 pyDecision-4.5.1/pyDecision/algorithm/waspas.py
+-rw-rw-rw-   0        0        0     2643 2023-07-21 18:23:36.000000 pyDecision-4.5.1/pyDecision/algorithm/wings.py
+-rw-rw-rw-   0        0        0     3188 2024-04-24 01:11:01.000000 pyDecision-4.5.1/pyDecision/algorithm/wisp.py
+drwxrwxrwx   0        0        0        0 2024-04-27 02:01:25.000000 pyDecision-4.5.1/pyDecision/compare/
+-rw-rw-rw-   0        0        0      127 2024-04-27 00:17:39.000000 pyDecision-4.5.1/pyDecision/compare/__init__.py
+-rw-rw-rw-   0        0        0    26165 2024-04-27 01:59:48.000000 pyDecision-4.5.1/pyDecision/compare/compare.py
+drwxrwxrwx   0        0        0        0 2024-04-27 02:01:25.000000 pyDecision-4.5.1/pyDecision/util/
+-rw-rw-rw-   0        0        0     8733 2023-12-03 18:26:24.000000 pyDecision-4.5.1/pyDecision/util/LLM.py
+-rw-rw-rw-   0        0        0      109 2023-08-02 19:44:51.000000 pyDecision-4.5.1/pyDecision/util/__init__.py
+-rw-rw-rw-   0        0        0     6266 2023-08-02 19:44:27.000000 pyDecision-4.5.1/pyDecision/util/ga.py
+drwxrwxrwx   0        0        0        0 2024-04-27 02:01:24.000000 pyDecision-4.5.1/pyDecision.egg-info/
+-rw-rw-rw-   0        0        0    20106 2024-04-27 02:01:23.000000 pyDecision-4.5.1/pyDecision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2742 2024-04-27 02:01:23.000000 pyDecision-4.5.1/pyDecision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 02:01:23.000000 pyDecision-4.5.1/pyDecision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-27 02:01:23.000000 pyDecision-4.5.1/pyDecision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-27 02:01:23.000000 pyDecision-4.5.1/pyDecision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 02:01:25.000000 pyDecision-4.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      744 2024-04-26 21:35:52.000000 pyDecision-4.5.1/setup.py
```

### Comparing `pyDecision-4.4.7/LICENSE` & `pyDecision-4.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/PKG-INFO` & `pyDecision-4.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 4.4.7
+Version: 4.5.1
 Summary: A MCDA Library Incorporating a Large Language Model to Enhance Decision Analysis
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **Regime** (REGIonal Multicriteria Elimination); **ROV** (Range Of Value); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **Fuzzy WASPAS**. 
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **Fuzzy CRITIC**; **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **Fuzzy FUCOM**; **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **Regime** (REGIonal Multicriteria Elimination); **ROC** (Rank Ordered Centroid); **ROV** (Range Of Value); **RRW** (Rank Reciprocal Weighting); **RSW** (Rank Summed Weight); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **Fuzzy WASPAS**. 
 
 pyDecision offers an array of features, including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
 
 ## Citation
 
 PEREIRA, V.; BASILIO, M.P.; SANTOS, C.H.T (2024). Enhancing Decision Analysis with a Large Language Model: pyDecision a Comprehensive Library of MCDA Methods in Python. arXiv. https://arxiv.org/abs/2404.06370
 
@@ -80,36 +80,39 @@
 - CoCoSo ([ Colab Demo ](https://colab.research.google.com/drive/1U8a3NZzQaxDkJdUT3uKIeeoqFtT_3Mnx?usp=sharing)) ( [ Paper ](https://doi.org/10.1108/MD-05-2017-0458))
 - CODAS ([ Colab Demo ](https://colab.research.google.com/drive/1hm7__urqFeBHM6nVQJcBzGPF72DFuoLr?usp=sharing)) ( [ Paper ](https://ideas.repec.org/a/cys/ecocyb/v50y2016i3p25-44.html))
 - Copeland ([ Colab Demo ](https://colab.research.google.com/drive/1ObP3AkQAzoCxT6et5Qkyk1trlER7mcdH?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/BF01212012))
 - COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1TZJtSjXqwYEwuL7-wfLcPQ8ZBtDq3lth?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/20294913.2012.762953))
 - Fuzzy COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1AIGgxBkmcA6YHKx06VeYcGf2EV8dPffW?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/s00500-021-05762-w))
 - CRADIS ([ Colab Demo ](https://colab.research.google.com/drive/1p7AQmPIOsZFxaypqMsiRIWW8mIvDtoLi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/s10668-021-01902-2))
 - CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1D5SaBHa1-Eo_KYSXHkFjsHYu29M21l_F?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0305-0548(94)00059-H))
+- Fuzzy CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1wofFhWDw6fn-XpLQoQjveKjyaId-AsEw?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.engappai.2022.104942))
 - DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/1T04qEft9uwTyQx--gADN6V_vUrT21Xo6?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2018/3696457))
 - Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0957417405003593))
 - EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1xsMdwH-IH-zvOW-1kv6ztQnKGt7p5JnY?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2015.57))
 - Fuzzy EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1kw2LwztNAU9Asjj6BvBmvk11wvk8R3V6?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-32-9072-3_63))
 - Entropy ([ Colab Demo ](https://colab.research.google.com/drive/1LOCef2KFxoV2qUEQRi4DqfzrgnMgtwT9?usp=sharing)) ( [ Paper ](https://people.math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf))
 - ELECTRE I     ([ Colab Demo ](https://colab.research.google.com/drive/1KFqRPBRyv-fxiu2B1y7VNkP5pCCbILF1?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/blob/master/MCDA/E01.pdf))
 - ELECTRE I_s   ([ Colab Demo ](https://colab.research.google.com/drive/1ngxsQPh2QULjd1_AifFofbukq5zIOePd?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE I_v   ([ Colab Demo ](https://colab.research.google.com/drive/1moonq95gqXqmbRe2KvgqbN2IfowJ12C-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE II    ([ Colab Demo ](https://colab.research.google.com/drive/1UeAjICH6_tjVr3O9H-fC65HHYMVZgTKc?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE III   ([ Colab Demo ](https://colab.research.google.com/drive/1smeD5ZoPgBnAAUyooAXSrkxHgqZPmUC9?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/raw/master/MCDA/E03.pdf))
 - ELECTRE IV    ([ Colab Demo ](https://colab.research.google.com/drive/178x062yC-Es6lstEiFaFprbMsTJZwnC-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE Tri-B ([ Colab Demo ](https://colab.research.google.com/drive/1hu0fJcxdBAiEDrVngmKQfpINpjTF-osE?usp=sharing)) ( [ Paper ](https://drive.google.com/file/d/1oWOI_sX3EEYdRbavoBTT7vUmPII1yPgE/view?usp=sharing))
 - FUCOM ([ Colab Demo ](https://colab.research.google.com/drive/1eWP3xf3-9iLLW_l_9JuAe6BEeoMsqzcL?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/sym10090393))
+- Fuzzy FUCOM ([ Colab Demo ](https://colab.research.google.com/drive/1bkelWth_7TOW_gIz8mBNe_4W5Ox84FUB?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/su14094972 ))
 - GRA ([ Colab Demo ](https://colab.research.google.com/drive/1aMMI0Cuo5kpzTDefqEwJhf0wWpBOP_JL?usp=sharing)) ( [ Paper ](https://uranos.ch/research/references/Julong_1989/10.1.1.678.3477.pdf))
 - IDOCRIW ([ Colab Demo ](https://colab.research.google.com/drive/1zt8uPFZGcHaSnpiT7tDnrDjvs0pK_7vS?usp=sharing)) ( [ Paper ](https://doi.org/10.1142/S0219622016500036))
 - MABAC ([ Colab Demo ](https://colab.research.google.com/drive/1BMqO-HnBXdcOZfZoULpx1H4MLPoUGucJ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2014.11.057))
 - MACBETH ([ Colab Demo ](https://colab.research.google.com/drive/1GqM9uPgbaWCGyj4l-XjkoifY2JJoVyf2?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0969-6016(94)90010-8))
 - MAIRCA ([ Colab Demo ](https://colab.research.google.com/drive/1gfqgrBAFGVygwm1j3lTjfy5wTsLgT_j5?usp=sharing)) ( [ Paper ](https://doi.org/10.1080/1331677X.2018.1506706))
 - MARA ([ Colab Demo ](https://colab.research.google.com/drive/1Ggg5e7TKVF_JN4yZRq9zThJO-PRBSI-N?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/systems10060248))
 - MARCOS ([ Colab Demo ](https://colab.research.google.com/drive/13MI2Qrakm5VzHN3r5O2RqggCzQwRxCs-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.cie.2019.106231))
 - MAUT ([ Colab Demo ](https://colab.research.google.com/drive/1qm3ARgQm68GUK2irGiCB-B49vnVHazB7?usp=sharing)) ( [ Paper ](https://doi.org/10.1017/CBO9781139174084))
 - MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1XE3AIzS84w-gw_1MEtV7xvkU1Gj_tRPd?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/sym13040525))
+- Fuzzy MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1yJ1eOXoGNp3amhoyBtEFCXr5PqwI9S5T?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/math11061544))
 - MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](http://matwbn.icm.edu.pl/ksiazki/cc/cc35/cc35213.pdf))
 - Fuzzy MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1ydHzGeA8WBVY5Gyu8K7Oq6kofQ5XbK3P?usp=sharing)) ( [ Paper ](https://pdfs.semanticscholar.org/6d33/ca3f14c9ed44d23742fd4e9cf94cebcaf148.pdf))
 - MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.15623/ijret.2014.0315105))
 - MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
 - OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1yQ41lOdjhiANtD1SOXoxA7gVim7A4X4P?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.5937/sjm10-6802))
 - Fuzzy OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1SniY4RLsR6jR9SnI3AR9k0wGlBWH6Pm8?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.5755/j01.ee.30.5.20546))
 - ORESTE ([ Colab Demo ](https://colab.research.google.com/drive/1USVCt6KJHJK9NXaknY8wTA4L0d4r2kWw?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0377-2217(82)90131-X))
@@ -122,15 +125,18 @@
 - PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - EC PROMETHEE ([ Colab Demo ](https://colab.research.google.com/drive/1YxXXuc2urj7_sUreZAROFldAhE0o6gio?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/math11214432))
 - PSI ([ Colab Demo ](https://colab.research.google.com/drive/1u9tN8cYl2mx6KK6yLW2oz6fuVoy8xcCI?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.matdes.2009.11.020))
 - MPSI ([ Colab Demo ](https://colab.research.google.com/drive/1zj2AS6W_VWmG5mYgY4b-dnCK0q3AG1-K?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/systems10060248))
 - Regime ([ Colab Demo ](https://colab.research.google.com/drive/1jcAcjAS92rxvE2urhc6HPixvzJ60HqEg?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/BF00221383))
+- ROC ([ Colab Demo ](https://colab.research.google.com/drive/1uUFXlCsZkFnh8HemNJ_hppvDC1eAwu4W?usp=sharing)) ( [ Paper ](https://doi.org/10.1002/(SICI)1099-0771(199806)11:2<85::AID-BDM282>3.0.CO;2-K))
 - ROV ([ Colab Demo ](https://colab.research.google.com/drive/1sQAPCem0pcS29uf6-n4TpncXMXNx9JDh?usp=sharing)) ( [ Paper ](https://doi.org/10.5267/j.dsl.2015.12.001))
+- RRW ([ Colab Demo ](https://colab.research.google.com/drive/1Pd13mNOosg0bxKAhALA3U9ppQYMB6yp_?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0030-5073(81)90015-5))
+- RSW ([ Colab Demo ](https://colab.research.google.com/drive/1IvAmwypsA6J3JRKGQsi0fmwnlGmL3rKM?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0030-5073(81)90015-5))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
 - SPOTIS ([ Colab Demo ](https://colab.research.google.com/drive/1TyjDn-xwut3w6Rf0zMiugdwytwmGY_NE?usp=sharing)) ( [ Paper ](https://doi.org/10.23919/FUSION45008.2020.9190347))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2007.10.046))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0377-2217(03)00020-1))
@@ -140,14 +146,15 @@
 - WISP, Simple WISP ([ Colab Demo ](https://colab.research.google.com/drive/1xyJf3aydLdVPqhWpNyVXXD8T4PsrX0du?usp=sharing)) ( [ Paper ](https://doi.org/10.1109/TEM.2021.3075783))
 - Fuzzy WSM, Fuzzy WPM, Fuzzy WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1PcN_PaXwPHawzCU05UiHE504SkgF6vQ2?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.15837/ijccc.2015.6.2078))
 
 4. Compare Methods:
 - Compare Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1RfLNEJjaHjtn3Lb2cfEDqS-iblaC4GQZ?usp=sharing))
 - Compare Fuzzy Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1pRO-E9xnk6DYEj_0DaEHUrUiCeIjmnXx?usp=sharing))
 - Compare Weights & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/169hTJxP2APHrDA1h0fD1YEeu9s29wu0T?usp=sharing))
+- Compare Fuzzy Weights & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1nWDF8lrTmXlc-TE4_X1-MPhraFjytj1Z?usp=sharing))
 
 5. Advanced MCDA Methods:
 
 - [3MOAHP](https://github.com/Valdecy/Method_3MOAHP) - Inconsistency Reduction Technique for AHP and Fuzzy-AHP Methods
 - [pyMissingAHP](https://github.com/Valdecy/pyMissingAHP) - A Method to Infer AHP Missing Pairwise Comparisons
 - [ELECTRE-Tree](https://github.com/Valdecy/ELECTRE-Tree) - Algorithm to infer the ELECTRE Tri-B method parameters
 - [Ranking-Trees](https://github.com/Valdecy/Ranking-Trees) - Algorithm to infer the ELECTRE II, III, IV, and PROMETHEE I, II, III, IV method parameters
```

### Comparing `pyDecision-4.4.7/README.md` & `pyDecision-4.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **Regime** (REGIonal Multicriteria Elimination); **ROV** (Range Of Value); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **Fuzzy WASPAS**. 
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **Fuzzy CRITIC**; **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **Fuzzy FUCOM**; **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **Regime** (REGIonal Multicriteria Elimination); **ROC** (Rank Ordered Centroid); **ROV** (Range Of Value); **RRW** (Rank Reciprocal Weighting); **RSW** (Rank Summed Weight); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **Fuzzy WASPAS**. 
 
 pyDecision offers an array of features, including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
 
 ## Citation
 
 PEREIRA, V.; BASILIO, M.P.; SANTOS, C.H.T (2024). Enhancing Decision Analysis with a Large Language Model: pyDecision a Comprehensive Library of MCDA Methods in Python. arXiv. https://arxiv.org/abs/2404.06370
 
@@ -69,36 +69,39 @@
 - CoCoSo ([ Colab Demo ](https://colab.research.google.com/drive/1U8a3NZzQaxDkJdUT3uKIeeoqFtT_3Mnx?usp=sharing)) ( [ Paper ](https://doi.org/10.1108/MD-05-2017-0458))
 - CODAS ([ Colab Demo ](https://colab.research.google.com/drive/1hm7__urqFeBHM6nVQJcBzGPF72DFuoLr?usp=sharing)) ( [ Paper ](https://ideas.repec.org/a/cys/ecocyb/v50y2016i3p25-44.html))
 - Copeland ([ Colab Demo ](https://colab.research.google.com/drive/1ObP3AkQAzoCxT6et5Qkyk1trlER7mcdH?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/BF01212012))
 - COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1TZJtSjXqwYEwuL7-wfLcPQ8ZBtDq3lth?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/20294913.2012.762953))
 - Fuzzy COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1AIGgxBkmcA6YHKx06VeYcGf2EV8dPffW?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/s00500-021-05762-w))
 - CRADIS ([ Colab Demo ](https://colab.research.google.com/drive/1p7AQmPIOsZFxaypqMsiRIWW8mIvDtoLi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/s10668-021-01902-2))
 - CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1D5SaBHa1-Eo_KYSXHkFjsHYu29M21l_F?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0305-0548(94)00059-H))
+- Fuzzy CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1wofFhWDw6fn-XpLQoQjveKjyaId-AsEw?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.engappai.2022.104942))
 - DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/1T04qEft9uwTyQx--gADN6V_vUrT21Xo6?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2018/3696457))
 - Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0957417405003593))
 - EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1xsMdwH-IH-zvOW-1kv6ztQnKGt7p5JnY?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2015.57))
 - Fuzzy EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1kw2LwztNAU9Asjj6BvBmvk11wvk8R3V6?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-32-9072-3_63))
 - Entropy ([ Colab Demo ](https://colab.research.google.com/drive/1LOCef2KFxoV2qUEQRi4DqfzrgnMgtwT9?usp=sharing)) ( [ Paper ](https://people.math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf))
 - ELECTRE I     ([ Colab Demo ](https://colab.research.google.com/drive/1KFqRPBRyv-fxiu2B1y7VNkP5pCCbILF1?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/blob/master/MCDA/E01.pdf))
 - ELECTRE I_s   ([ Colab Demo ](https://colab.research.google.com/drive/1ngxsQPh2QULjd1_AifFofbukq5zIOePd?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE I_v   ([ Colab Demo ](https://colab.research.google.com/drive/1moonq95gqXqmbRe2KvgqbN2IfowJ12C-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE II    ([ Colab Demo ](https://colab.research.google.com/drive/1UeAjICH6_tjVr3O9H-fC65HHYMVZgTKc?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE III   ([ Colab Demo ](https://colab.research.google.com/drive/1smeD5ZoPgBnAAUyooAXSrkxHgqZPmUC9?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/raw/master/MCDA/E03.pdf))
 - ELECTRE IV    ([ Colab Demo ](https://colab.research.google.com/drive/178x062yC-Es6lstEiFaFprbMsTJZwnC-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE Tri-B ([ Colab Demo ](https://colab.research.google.com/drive/1hu0fJcxdBAiEDrVngmKQfpINpjTF-osE?usp=sharing)) ( [ Paper ](https://drive.google.com/file/d/1oWOI_sX3EEYdRbavoBTT7vUmPII1yPgE/view?usp=sharing))
 - FUCOM ([ Colab Demo ](https://colab.research.google.com/drive/1eWP3xf3-9iLLW_l_9JuAe6BEeoMsqzcL?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/sym10090393))
+- Fuzzy FUCOM ([ Colab Demo ](https://colab.research.google.com/drive/1bkelWth_7TOW_gIz8mBNe_4W5Ox84FUB?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/su14094972 ))
 - GRA ([ Colab Demo ](https://colab.research.google.com/drive/1aMMI0Cuo5kpzTDefqEwJhf0wWpBOP_JL?usp=sharing)) ( [ Paper ](https://uranos.ch/research/references/Julong_1989/10.1.1.678.3477.pdf))
 - IDOCRIW ([ Colab Demo ](https://colab.research.google.com/drive/1zt8uPFZGcHaSnpiT7tDnrDjvs0pK_7vS?usp=sharing)) ( [ Paper ](https://doi.org/10.1142/S0219622016500036))
 - MABAC ([ Colab Demo ](https://colab.research.google.com/drive/1BMqO-HnBXdcOZfZoULpx1H4MLPoUGucJ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2014.11.057))
 - MACBETH ([ Colab Demo ](https://colab.research.google.com/drive/1GqM9uPgbaWCGyj4l-XjkoifY2JJoVyf2?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0969-6016(94)90010-8))
 - MAIRCA ([ Colab Demo ](https://colab.research.google.com/drive/1gfqgrBAFGVygwm1j3lTjfy5wTsLgT_j5?usp=sharing)) ( [ Paper ](https://doi.org/10.1080/1331677X.2018.1506706))
 - MARA ([ Colab Demo ](https://colab.research.google.com/drive/1Ggg5e7TKVF_JN4yZRq9zThJO-PRBSI-N?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/systems10060248))
 - MARCOS ([ Colab Demo ](https://colab.research.google.com/drive/13MI2Qrakm5VzHN3r5O2RqggCzQwRxCs-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.cie.2019.106231))
 - MAUT ([ Colab Demo ](https://colab.research.google.com/drive/1qm3ARgQm68GUK2irGiCB-B49vnVHazB7?usp=sharing)) ( [ Paper ](https://doi.org/10.1017/CBO9781139174084))
 - MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1XE3AIzS84w-gw_1MEtV7xvkU1Gj_tRPd?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/sym13040525))
+- Fuzzy MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1yJ1eOXoGNp3amhoyBtEFCXr5PqwI9S5T?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/math11061544))
 - MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](http://matwbn.icm.edu.pl/ksiazki/cc/cc35/cc35213.pdf))
 - Fuzzy MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1ydHzGeA8WBVY5Gyu8K7Oq6kofQ5XbK3P?usp=sharing)) ( [ Paper ](https://pdfs.semanticscholar.org/6d33/ca3f14c9ed44d23742fd4e9cf94cebcaf148.pdf))
 - MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.15623/ijret.2014.0315105))
 - MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
 - OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1yQ41lOdjhiANtD1SOXoxA7gVim7A4X4P?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.5937/sjm10-6802))
 - Fuzzy OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1SniY4RLsR6jR9SnI3AR9k0wGlBWH6Pm8?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.5755/j01.ee.30.5.20546))
 - ORESTE ([ Colab Demo ](https://colab.research.google.com/drive/1USVCt6KJHJK9NXaknY8wTA4L0d4r2kWw?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0377-2217(82)90131-X))
@@ -111,15 +114,18 @@
 - PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - EC PROMETHEE ([ Colab Demo ](https://colab.research.google.com/drive/1YxXXuc2urj7_sUreZAROFldAhE0o6gio?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/math11214432))
 - PSI ([ Colab Demo ](https://colab.research.google.com/drive/1u9tN8cYl2mx6KK6yLW2oz6fuVoy8xcCI?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.matdes.2009.11.020))
 - MPSI ([ Colab Demo ](https://colab.research.google.com/drive/1zj2AS6W_VWmG5mYgY4b-dnCK0q3AG1-K?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/systems10060248))
 - Regime ([ Colab Demo ](https://colab.research.google.com/drive/1jcAcjAS92rxvE2urhc6HPixvzJ60HqEg?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/BF00221383))
+- ROC ([ Colab Demo ](https://colab.research.google.com/drive/1uUFXlCsZkFnh8HemNJ_hppvDC1eAwu4W?usp=sharing)) ( [ Paper ](https://doi.org/10.1002/(SICI)1099-0771(199806)11:2<85::AID-BDM282>3.0.CO;2-K))
 - ROV ([ Colab Demo ](https://colab.research.google.com/drive/1sQAPCem0pcS29uf6-n4TpncXMXNx9JDh?usp=sharing)) ( [ Paper ](https://doi.org/10.5267/j.dsl.2015.12.001))
+- RRW ([ Colab Demo ](https://colab.research.google.com/drive/1Pd13mNOosg0bxKAhALA3U9ppQYMB6yp_?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0030-5073(81)90015-5))
+- RSW ([ Colab Demo ](https://colab.research.google.com/drive/1IvAmwypsA6J3JRKGQsi0fmwnlGmL3rKM?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0030-5073(81)90015-5))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
 - SPOTIS ([ Colab Demo ](https://colab.research.google.com/drive/1TyjDn-xwut3w6Rf0zMiugdwytwmGY_NE?usp=sharing)) ( [ Paper ](https://doi.org/10.23919/FUSION45008.2020.9190347))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2007.10.046))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0377-2217(03)00020-1))
@@ -129,14 +135,15 @@
 - WISP, Simple WISP ([ Colab Demo ](https://colab.research.google.com/drive/1xyJf3aydLdVPqhWpNyVXXD8T4PsrX0du?usp=sharing)) ( [ Paper ](https://doi.org/10.1109/TEM.2021.3075783))
 - Fuzzy WSM, Fuzzy WPM, Fuzzy WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1PcN_PaXwPHawzCU05UiHE504SkgF6vQ2?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.15837/ijccc.2015.6.2078))
 
 4. Compare Methods:
 - Compare Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1RfLNEJjaHjtn3Lb2cfEDqS-iblaC4GQZ?usp=sharing))
 - Compare Fuzzy Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1pRO-E9xnk6DYEj_0DaEHUrUiCeIjmnXx?usp=sharing))
 - Compare Weights & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/169hTJxP2APHrDA1h0fD1YEeu9s29wu0T?usp=sharing))
+- Compare Fuzzy Weights & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1nWDF8lrTmXlc-TE4_X1-MPhraFjytj1Z?usp=sharing))
 
 5. Advanced MCDA Methods:
 
 - [3MOAHP](https://github.com/Valdecy/Method_3MOAHP) - Inconsistency Reduction Technique for AHP and Fuzzy-AHP Methods
 - [pyMissingAHP](https://github.com/Valdecy/pyMissingAHP) - A Method to Infer AHP Missing Pairwise Comparisons
 - [ELECTRE-Tree](https://github.com/Valdecy/ELECTRE-Tree) - Algorithm to infer the ELECTRE Tri-B method parameters
 - [Ranking-Trees](https://github.com/Valdecy/Ranking-Trees) - Algorithm to infer the ELECTRE II, III, IV, and PROMETHEE I, II, III, IV method parameters
```

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/__init__.py` & `pyDecision-4.5.1/pyDecision/algorithm/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,19 @@
 from .edas          import edas_method
 from .entropy       import entropy_method
 from .fucom         import fucom_method
 from .fuzzy_ahp     import fuzzy_ahp_method
 from .fuzzy_aras    import fuzzy_aras_method
 from .fuzzy_bwm     import fuzzy_bw_method
 from .fuzzy_copras  import fuzzy_copras_method
+from .fuzzy_critic  import fuzzy_critic_method
 from .fuzzy_dematel import fuzzy_dematel_method
 from .fuzzy_edas    import fuzzy_edas_method
+from .fuzzy_fucom   import fuzzy_fucom_method
+from .fuzzy_merec   import fuzzy_merec_method
 from .fuzzy_moora   import fuzzy_moora_method
 from .fuzzy_ocra    import fuzzy_ocra_method
 from .fuzzy_topsis  import fuzzy_topsis_method
 from .fuzzy_vikor   import fuzzy_vikor_method
 from .fuzzy_waspas  import fuzzy_waspas_method
 from .gra           import gra_method
 from .idocriw       import idocriw_method
@@ -54,15 +57,18 @@
 from .p_v           import promethee_v
 from .p_vi          import promethee_vi
 from .p_xgaia       import promethee_gaia
 from .piv           import piv_method
 from .psi           import psi_method
 from .psi_m         import mpsi_method
 from .regime        import regime_method
+from .roc           import roc_method
 from .rov           import rov_method
+from .rrw           import rrw_method
+from .rsw           import rsw_method
 from .saw           import saw_method
 from .smart         import smart_method
 from .spotis        import spotis_method
 from .todim         import todim_method
 from .topsis        import topsis_method
 from .vikor         import vikor_method, ranking
 from .waspas        import waspas_method
```

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/ahp.py` & `pyDecision-4.5.1/pyDecision/algorithm/ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/aras.py` & `pyDecision-4.5.1/pyDecision/algorithm/aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/borda.py` & `pyDecision-4.5.1/pyDecision/algorithm/borda.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/bwm.py` & `pyDecision-4.5.1/pyDecision/algorithm/bwm.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/bwm_s.py` & `pyDecision-4.5.1/pyDecision/algorithm/bwm_s.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/cilos.py` & `pyDecision-4.5.1/pyDecision/algorithm/cilos.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/cocoso.py` & `pyDecision-4.5.1/pyDecision/algorithm/cocoso.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/codas.py` & `pyDecision-4.5.1/pyDecision/algorithm/codas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/copeland.py` & `pyDecision-4.5.1/pyDecision/algorithm/copeland.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/copras.py` & `pyDecision-4.5.1/pyDecision/algorithm/copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/cradis.py` & `pyDecision-4.5.1/pyDecision/algorithm/cradis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/critic.py` & `pyDecision-4.5.1/pyDecision/algorithm/critic.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/dematel.py` & `pyDecision-4.5.1/pyDecision/algorithm/dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/e_i.py` & `pyDecision-4.5.1/pyDecision/algorithm/e_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/e_i_s.py` & `pyDecision-4.5.1/pyDecision/algorithm/e_i_s.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/e_i_v.py` & `pyDecision-4.5.1/pyDecision/algorithm/e_i_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/e_ii.py` & `pyDecision-4.5.1/pyDecision/algorithm/e_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/e_iii.py` & `pyDecision-4.5.1/pyDecision/algorithm/e_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/e_iv.py` & `pyDecision-4.5.1/pyDecision/algorithm/e_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/e_tri_b.py` & `pyDecision-4.5.1/pyDecision/algorithm/e_tri_b.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/edas.py` & `pyDecision-4.5.1/pyDecision/algorithm/edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/entropy.py` & `pyDecision-4.5.1/pyDecision/algorithm/entropy.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/fucom.py` & `pyDecision-4.5.1/pyDecision/algorithm/fucom.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/fuzzy_ahp.py` & `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/fuzzy_aras.py` & `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/fuzzy_bwm.py` & `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_bwm.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/fuzzy_copras.py` & `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/fuzzy_dematel.py` & `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/fuzzy_edas.py` & `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/fuzzy_moora.py` & `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/fuzzy_ocra.py` & `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_ocra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/fuzzy_topsis.py` & `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/fuzzy_vikor.py` & `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/fuzzy_waspas.py` & `pyDecision-4.5.1/pyDecision/algorithm/fuzzy_waspas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/gra.py` & `pyDecision-4.5.1/pyDecision/algorithm/gra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/idocriw.py` & `pyDecision-4.5.1/pyDecision/algorithm/idocriw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/mabac.py` & `pyDecision-4.5.1/pyDecision/algorithm/mabac.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/macbeth.py` & `pyDecision-4.5.1/pyDecision/algorithm/macbeth.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/mairca.py` & `pyDecision-4.5.1/pyDecision/algorithm/mairca.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/mara.py` & `pyDecision-4.5.1/pyDecision/algorithm/mara.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/marcos.py` & `pyDecision-4.5.1/pyDecision/algorithm/marcos.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/maut.py` & `pyDecision-4.5.1/pyDecision/algorithm/maut.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/merec.py` & `pyDecision-4.5.1/pyDecision/algorithm/merec.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/moora.py` & `pyDecision-4.5.1/pyDecision/algorithm/moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/moosra.py` & `pyDecision-4.5.1/pyDecision/algorithm/moosra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/multimoora.py` & `pyDecision-4.5.1/pyDecision/algorithm/multimoora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/ocra.py` & `pyDecision-4.5.1/pyDecision/algorithm/ocra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/oreste.py` & `pyDecision-4.5.1/pyDecision/algorithm/oreste.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/p_ec.py` & `pyDecision-4.5.1/pyDecision/algorithm/p_ec.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/p_i.py` & `pyDecision-4.5.1/pyDecision/algorithm/p_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/p_ii.py` & `pyDecision-4.5.1/pyDecision/algorithm/p_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/p_iii.py` & `pyDecision-4.5.1/pyDecision/algorithm/p_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/p_iv.py` & `pyDecision-4.5.1/pyDecision/algorithm/p_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/p_v.py` & `pyDecision-4.5.1/pyDecision/algorithm/p_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/p_vi.py` & `pyDecision-4.5.1/pyDecision/algorithm/p_vi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/p_xgaia.py` & `pyDecision-4.5.1/pyDecision/algorithm/p_xgaia.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/piv.py` & `pyDecision-4.5.1/pyDecision/algorithm/piv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/psi.py` & `pyDecision-4.5.1/pyDecision/algorithm/psi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/psi_m.py` & `pyDecision-4.5.1/pyDecision/algorithm/psi_m.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/regime.py` & `pyDecision-4.5.1/pyDecision/algorithm/regime.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/rov.py` & `pyDecision-4.5.1/pyDecision/algorithm/rov.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/saw.py` & `pyDecision-4.5.1/pyDecision/algorithm/saw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/smart.py` & `pyDecision-4.5.1/pyDecision/algorithm/smart.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/spotis.py` & `pyDecision-4.5.1/pyDecision/algorithm/spotis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/todim.py` & `pyDecision-4.5.1/pyDecision/algorithm/todim.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/topsis.py` & `pyDecision-4.5.1/pyDecision/algorithm/topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/vikor.py` & `pyDecision-4.5.1/pyDecision/algorithm/vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/waspas.py` & `pyDecision-4.5.1/pyDecision/algorithm/waspas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/wings.py` & `pyDecision-4.5.1/pyDecision/algorithm/wings.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/algorithm/wisp.py` & `pyDecision-4.5.1/pyDecision/algorithm/wisp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/compare/compare.py` & `pyDecision-4.5.1/pyDecision/compare/compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,22 @@
 from pyDecision.algorithm.cilos        import cilos_method
 from pyDecision.algorithm.critic       import critic_method
 from pyDecision.algorithm.entropy      import entropy_method
 from pyDecision.algorithm.fucom        import fucom_method
 from pyDecision.algorithm.idocriw      import idocriw_method
 from pyDecision.algorithm.merec        import merec_method
 from pyDecision.algorithm.psi_m        import mpsi_method
-
-#from pyDecision.algorithm.fuzzy_bwm    import fuzzy_bw_method
+from pyDecision.algorithm.roc          import roc_method
+from pyDecision.algorithm.rrw          import rrw_method
+from pyDecision.algorithm.rsw          import rsw_method
+
+from pyDecision.algorithm.fuzzy_bwm    import fuzzy_bw_method
+from pyDecision.algorithm.fuzzy_critic import fuzzy_critic_method
+from pyDecision.algorithm.fuzzy_fucom  import fuzzy_fucom_method
+from pyDecision.algorithm.fuzzy_merec  import fuzzy_merec_method
 
 from pyDecision.algorithm.aras         import aras_method
 from pyDecision.algorithm.borda        import borda_method
 from pyDecision.algorithm.cocoso       import cocoso_method
 from pyDecision.algorithm.codas        import codas_method
 from pyDecision.algorithm.copeland     import copeland_method
 from pyDecision.algorithm.copras       import copras_method
@@ -120,15 +126,15 @@
     return corr_df
 
 ###############################################################################
 
 # Function: Compare Weights Crisp
 def compare_weights(dataset, criterion_type, custom_methods = [], custom_weigths = [], methods_list = [], mic = [], lic = [], criteria_priority = [], criteria_rank = [], alpha = 0.5):
     if ('all' in methods_list):
-        methods_list = ['bwm', 'bwm_s', 'cilos', 'critic', 'entropy', 'fucom', 'idocriw', 'merec', 'mpsi']
+        methods_list = ['bwm', 'bwm_s', 'cilos', 'critic', 'entropy', 'fucom', 'idocriw', 'merec', 'mpsi', 'roc', 'rrw', 'rsw']
     if (len(custom_methods) > 0):
         methods_list = custom_methods + methods_list 
     X       = np.zeros((dataset.shape[1], len(methods_list)))
     j       = 0
     for i in range(0, len(custom_weigths)):
         X[:,j] = custom_weigths[i]
         j      = j + 1 
@@ -175,34 +181,67 @@
             j      = j + 1
             print('MEREC: Done!')
         if (method == 'mpsi' or method == 'all'):
             w      = mpsi_method(dataset, criterion_type)
             X[:,j] = w
             j      = j + 1
             print('MPSI: Done!')
+        if (method == 'roc' or method == 'all'):
+            w      = roc_method(criteria_rank)
+            X[:,j] = w
+            j      = j + 1
+            print('ROC: Done!')
+        if (method == 'rrw' or method == 'all'):
+            w      = rrw_method(criteria_rank)
+            X[:,j] = w
+            j      = j + 1
+            print('RRW: Done!')
+        if (method == 'rsw' or method == 'all'):
+            w      = rsw_method(criteria_rank)
+            X[:,j] = w
+            j      = j + 1
+            print('RSW: Done!')
     X = pd.DataFrame(X, index = ['g'+str(i+1) for i in range(0, X.shape[0])], columns = methods_list)    
     return X
 
 # Function: Compare Weights Fuzzy
-#def compare_weights_fuzzy(dataset, criterion_type, custom_methods = [], custom_weigths = [], methods_list = [], mic = [], lic = [], eps_penalty = 1):
-    #if ('all' in methods_list):
-        #methods_list = ['fuzzy_bwm']
-    #if (len(custom_methods) > 0):
-        #methods_list = custom_methods + methods_list 
-    #for i in range(0, len(custom_weigths)):
-        #X[:,j] = custom_weigths[i]
-        #j      = j + 1 
-        #print(custom_methods[i], ': Done!')
-    #for method in methods_list:
-        #if (method == 'fuzzy_bwm' or method == 'all'):
-            #_, _, _, w = fuzzy_bw_method(mic, lic, eps_penalty = eps_penalty, False)
-            #X[:,j]     = w
-            #j          = j + 1
-            #print('Fuzzy BWM: Done!')
-    #return
+def compare_weights_fuzzy(dataset = [], criterion_type = [], custom_methods = [], custom_weigths = [], methods_list = [], criteria_priority = [], criteria_rank = [], mic = [], lic = [], eps_penalty = 1, n_starts = 250):
+    if ('all' in methods_list):
+        methods_list = ['fuzzy_bwm', 'fuzzy_critic', 'fuzzy_fucom', 'fuzzy_merec']
+    if (len(custom_methods) > 0):
+        methods_list = custom_methods + methods_list 
+    X = np.zeros((np.max((len(criterion_type), len(criteria_rank), len(mic))), len(methods_list)))
+    j = 0
+    for i in range(0, len(custom_weigths)):
+        X[:,j] = custom_weigths[i]
+        j      = j + 1 
+        print(custom_methods[i], ': Done!')
+    for method in methods_list:
+        if (method == 'fuzzy_bwm' or method == 'all'):
+            _, _, _, w = fuzzy_bw_method(mic, lic, eps_penalty, False)
+            X[:,j]     = w
+            j          = j + 1
+            print('Fuzzy BWM: Done!')
+        if (method == 'fuzzy_critic' or method == 'all'):
+            w          = fuzzy_critic_method(dataset, criterion_type)
+            X[:,j]     = w
+            j          = j + 1
+            print('Fuzzy CRITIC: Done!')
+        if (method == 'fuzzy_fucom' or method == 'all'):
+            _, w       = fuzzy_fucom_method(criteria_rank, criteria_priority, n_starts, True, False)
+            X[:,j]     = w
+            j          = j + 1
+            print('Fuzzy FUCOM: Done!')
+        if (method == 'fuzzy_merec' or method == 'all'):
+            w          = fuzzy_merec_method(dataset, criterion_type)
+            X[:,j]     = w
+            j          = j + 1
+            print('Fuzzy MEREC: Done!')
+    X = pd.DataFrame(X, index = ['g'+str(i+1) for i in range(0, X.shape[0])], columns = methods_list) 
+    return X
     
 # Function: Compare Ranks Crisp
 def compare_ranks_crisp(dataset, weights, criterion_type, utility_functions = [], custom_methods = [], custom_ranks = [], methods_list = [], L = 0.5, lmbd = 0.02, epsilon = 0.5, step_size = 1, teta = 1, strategy_coefficient = 0.5, Q = [], S = [], P = [], F = [], custom_sets = [], iterations = 1000, lambda_value = 0.5, alpha = 0.4, s_min = [], s_max = []):
     if ('all' in methods_list):
         methods_list = ['aras', 'borda', 'cocoso', 'codas', 'copeland', 'copras', 'cradis', 'edas', 'gra', 'mabac', 'macbeth', 'mairca', 'mara', 'marcos', 'maut', 'moora', 'moosra', 'multimoora', 'ocra', 'oreste', 'piv', 'promethee_ii', 'promethee_iv', 'ec_promethee', 'psi', 'rov', 'saw', 'spotis', 'todim', 'topsis', 'vikor', 'wsm', 'wpm', 'waspas', 'wisp', 'simple wisp']
     if (len(custom_methods) > 0):
         methods_list = custom_methods + methods_list 
@@ -481,8 +520,8 @@
     ranked = np.zeros_like(X)
     for i in range(0, X.shape[1]):
         ranked[:, i] = X.shape[0] + 1 - rankdata(X[:, i], method = 'max')
     X      = pd.DataFrame(X, index = ['a'+str(i+1) for i in range(0, X.shape[0])], columns = methods_list)    
     ranked = pd.DataFrame(ranked, index = ['a'+str(i+1) for i in range(0, X.shape[0])], columns = methods_list)
     return X, ranked
 
-###############################################################################
+###############################################################################
```

### Comparing `pyDecision-4.4.7/pyDecision/util/LLM.py` & `pyDecision-4.5.1/pyDecision/util/LLM.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision/util/ga.py` & `pyDecision-4.5.1/pyDecision/util/ga.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.7/pyDecision.egg-info/PKG-INFO` & `pyDecision-4.5.1/pyDecision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 4.4.7
+Version: 4.5.1
 Summary: A MCDA Library Incorporating a Large Language Model to Enhance Decision Analysis
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **Regime** (REGIonal Multicriteria Elimination); **ROV** (Range Of Value); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **Fuzzy WASPAS**. 
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **Fuzzy CRITIC**; **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **Fuzzy FUCOM**; **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **Regime** (REGIonal Multicriteria Elimination); **ROC** (Rank Ordered Centroid); **ROV** (Range Of Value); **RRW** (Rank Reciprocal Weighting); **RSW** (Rank Summed Weight); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **Fuzzy WASPAS**. 
 
 pyDecision offers an array of features, including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
 
 ## Citation
 
 PEREIRA, V.; BASILIO, M.P.; SANTOS, C.H.T (2024). Enhancing Decision Analysis with a Large Language Model: pyDecision a Comprehensive Library of MCDA Methods in Python. arXiv. https://arxiv.org/abs/2404.06370
 
@@ -80,36 +80,39 @@
 - CoCoSo ([ Colab Demo ](https://colab.research.google.com/drive/1U8a3NZzQaxDkJdUT3uKIeeoqFtT_3Mnx?usp=sharing)) ( [ Paper ](https://doi.org/10.1108/MD-05-2017-0458))
 - CODAS ([ Colab Demo ](https://colab.research.google.com/drive/1hm7__urqFeBHM6nVQJcBzGPF72DFuoLr?usp=sharing)) ( [ Paper ](https://ideas.repec.org/a/cys/ecocyb/v50y2016i3p25-44.html))
 - Copeland ([ Colab Demo ](https://colab.research.google.com/drive/1ObP3AkQAzoCxT6et5Qkyk1trlER7mcdH?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/BF01212012))
 - COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1TZJtSjXqwYEwuL7-wfLcPQ8ZBtDq3lth?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/20294913.2012.762953))
 - Fuzzy COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1AIGgxBkmcA6YHKx06VeYcGf2EV8dPffW?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/s00500-021-05762-w))
 - CRADIS ([ Colab Demo ](https://colab.research.google.com/drive/1p7AQmPIOsZFxaypqMsiRIWW8mIvDtoLi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/s10668-021-01902-2))
 - CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1D5SaBHa1-Eo_KYSXHkFjsHYu29M21l_F?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0305-0548(94)00059-H))
+- Fuzzy CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1wofFhWDw6fn-XpLQoQjveKjyaId-AsEw?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.engappai.2022.104942))
 - DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/1T04qEft9uwTyQx--gADN6V_vUrT21Xo6?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2018/3696457))
 - Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0957417405003593))
 - EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1xsMdwH-IH-zvOW-1kv6ztQnKGt7p5JnY?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2015.57))
 - Fuzzy EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1kw2LwztNAU9Asjj6BvBmvk11wvk8R3V6?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-32-9072-3_63))
 - Entropy ([ Colab Demo ](https://colab.research.google.com/drive/1LOCef2KFxoV2qUEQRi4DqfzrgnMgtwT9?usp=sharing)) ( [ Paper ](https://people.math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf))
 - ELECTRE I     ([ Colab Demo ](https://colab.research.google.com/drive/1KFqRPBRyv-fxiu2B1y7VNkP5pCCbILF1?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/blob/master/MCDA/E01.pdf))
 - ELECTRE I_s   ([ Colab Demo ](https://colab.research.google.com/drive/1ngxsQPh2QULjd1_AifFofbukq5zIOePd?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE I_v   ([ Colab Demo ](https://colab.research.google.com/drive/1moonq95gqXqmbRe2KvgqbN2IfowJ12C-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE II    ([ Colab Demo ](https://colab.research.google.com/drive/1UeAjICH6_tjVr3O9H-fC65HHYMVZgTKc?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE III   ([ Colab Demo ](https://colab.research.google.com/drive/1smeD5ZoPgBnAAUyooAXSrkxHgqZPmUC9?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/raw/master/MCDA/E03.pdf))
 - ELECTRE IV    ([ Colab Demo ](https://colab.research.google.com/drive/178x062yC-Es6lstEiFaFprbMsTJZwnC-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE Tri-B ([ Colab Demo ](https://colab.research.google.com/drive/1hu0fJcxdBAiEDrVngmKQfpINpjTF-osE?usp=sharing)) ( [ Paper ](https://drive.google.com/file/d/1oWOI_sX3EEYdRbavoBTT7vUmPII1yPgE/view?usp=sharing))
 - FUCOM ([ Colab Demo ](https://colab.research.google.com/drive/1eWP3xf3-9iLLW_l_9JuAe6BEeoMsqzcL?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/sym10090393))
+- Fuzzy FUCOM ([ Colab Demo ](https://colab.research.google.com/drive/1bkelWth_7TOW_gIz8mBNe_4W5Ox84FUB?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/su14094972 ))
 - GRA ([ Colab Demo ](https://colab.research.google.com/drive/1aMMI0Cuo5kpzTDefqEwJhf0wWpBOP_JL?usp=sharing)) ( [ Paper ](https://uranos.ch/research/references/Julong_1989/10.1.1.678.3477.pdf))
 - IDOCRIW ([ Colab Demo ](https://colab.research.google.com/drive/1zt8uPFZGcHaSnpiT7tDnrDjvs0pK_7vS?usp=sharing)) ( [ Paper ](https://doi.org/10.1142/S0219622016500036))
 - MABAC ([ Colab Demo ](https://colab.research.google.com/drive/1BMqO-HnBXdcOZfZoULpx1H4MLPoUGucJ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2014.11.057))
 - MACBETH ([ Colab Demo ](https://colab.research.google.com/drive/1GqM9uPgbaWCGyj4l-XjkoifY2JJoVyf2?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0969-6016(94)90010-8))
 - MAIRCA ([ Colab Demo ](https://colab.research.google.com/drive/1gfqgrBAFGVygwm1j3lTjfy5wTsLgT_j5?usp=sharing)) ( [ Paper ](https://doi.org/10.1080/1331677X.2018.1506706))
 - MARA ([ Colab Demo ](https://colab.research.google.com/drive/1Ggg5e7TKVF_JN4yZRq9zThJO-PRBSI-N?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/systems10060248))
 - MARCOS ([ Colab Demo ](https://colab.research.google.com/drive/13MI2Qrakm5VzHN3r5O2RqggCzQwRxCs-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.cie.2019.106231))
 - MAUT ([ Colab Demo ](https://colab.research.google.com/drive/1qm3ARgQm68GUK2irGiCB-B49vnVHazB7?usp=sharing)) ( [ Paper ](https://doi.org/10.1017/CBO9781139174084))
 - MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1XE3AIzS84w-gw_1MEtV7xvkU1Gj_tRPd?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/sym13040525))
+- Fuzzy MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1yJ1eOXoGNp3amhoyBtEFCXr5PqwI9S5T?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/math11061544))
 - MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](http://matwbn.icm.edu.pl/ksiazki/cc/cc35/cc35213.pdf))
 - Fuzzy MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1ydHzGeA8WBVY5Gyu8K7Oq6kofQ5XbK3P?usp=sharing)) ( [ Paper ](https://pdfs.semanticscholar.org/6d33/ca3f14c9ed44d23742fd4e9cf94cebcaf148.pdf))
 - MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.15623/ijret.2014.0315105))
 - MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
 - OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1yQ41lOdjhiANtD1SOXoxA7gVim7A4X4P?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.5937/sjm10-6802))
 - Fuzzy OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1SniY4RLsR6jR9SnI3AR9k0wGlBWH6Pm8?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.5755/j01.ee.30.5.20546))
 - ORESTE ([ Colab Demo ](https://colab.research.google.com/drive/1USVCt6KJHJK9NXaknY8wTA4L0d4r2kWw?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0377-2217(82)90131-X))
@@ -122,15 +125,18 @@
 - PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - EC PROMETHEE ([ Colab Demo ](https://colab.research.google.com/drive/1YxXXuc2urj7_sUreZAROFldAhE0o6gio?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/math11214432))
 - PSI ([ Colab Demo ](https://colab.research.google.com/drive/1u9tN8cYl2mx6KK6yLW2oz6fuVoy8xcCI?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.matdes.2009.11.020))
 - MPSI ([ Colab Demo ](https://colab.research.google.com/drive/1zj2AS6W_VWmG5mYgY4b-dnCK0q3AG1-K?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/systems10060248))
 - Regime ([ Colab Demo ](https://colab.research.google.com/drive/1jcAcjAS92rxvE2urhc6HPixvzJ60HqEg?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/BF00221383))
+- ROC ([ Colab Demo ](https://colab.research.google.com/drive/1uUFXlCsZkFnh8HemNJ_hppvDC1eAwu4W?usp=sharing)) ( [ Paper ](https://doi.org/10.1002/(SICI)1099-0771(199806)11:2<85::AID-BDM282>3.0.CO;2-K))
 - ROV ([ Colab Demo ](https://colab.research.google.com/drive/1sQAPCem0pcS29uf6-n4TpncXMXNx9JDh?usp=sharing)) ( [ Paper ](https://doi.org/10.5267/j.dsl.2015.12.001))
+- RRW ([ Colab Demo ](https://colab.research.google.com/drive/1Pd13mNOosg0bxKAhALA3U9ppQYMB6yp_?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0030-5073(81)90015-5))
+- RSW ([ Colab Demo ](https://colab.research.google.com/drive/1IvAmwypsA6J3JRKGQsi0fmwnlGmL3rKM?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0030-5073(81)90015-5))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
 - SPOTIS ([ Colab Demo ](https://colab.research.google.com/drive/1TyjDn-xwut3w6Rf0zMiugdwytwmGY_NE?usp=sharing)) ( [ Paper ](https://doi.org/10.23919/FUSION45008.2020.9190347))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2007.10.046))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0377-2217(03)00020-1))
@@ -140,14 +146,15 @@
 - WISP, Simple WISP ([ Colab Demo ](https://colab.research.google.com/drive/1xyJf3aydLdVPqhWpNyVXXD8T4PsrX0du?usp=sharing)) ( [ Paper ](https://doi.org/10.1109/TEM.2021.3075783))
 - Fuzzy WSM, Fuzzy WPM, Fuzzy WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1PcN_PaXwPHawzCU05UiHE504SkgF6vQ2?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.15837/ijccc.2015.6.2078))
 
 4. Compare Methods:
 - Compare Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1RfLNEJjaHjtn3Lb2cfEDqS-iblaC4GQZ?usp=sharing))
 - Compare Fuzzy Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1pRO-E9xnk6DYEj_0DaEHUrUiCeIjmnXx?usp=sharing))
 - Compare Weights & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/169hTJxP2APHrDA1h0fD1YEeu9s29wu0T?usp=sharing))
+- Compare Fuzzy Weights & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1nWDF8lrTmXlc-TE4_X1-MPhraFjytj1Z?usp=sharing))
 
 5. Advanced MCDA Methods:
 
 - [3MOAHP](https://github.com/Valdecy/Method_3MOAHP) - Inconsistency Reduction Technique for AHP and Fuzzy-AHP Methods
 - [pyMissingAHP](https://github.com/Valdecy/pyMissingAHP) - A Method to Infer AHP Missing Pairwise Comparisons
 - [ELECTRE-Tree](https://github.com/Valdecy/ELECTRE-Tree) - Algorithm to infer the ELECTRE Tri-B method parameters
 - [Ranking-Trees](https://github.com/Valdecy/Ranking-Trees) - Algorithm to infer the ELECTRE II, III, IV, and PROMETHEE I, II, III, IV method parameters
```

### Comparing `pyDecision-4.4.7/pyDecision.egg-info/SOURCES.txt` & `pyDecision-4.5.1/pyDecision.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -31,16 +31,19 @@
 pyDecision/algorithm/edas.py
 pyDecision/algorithm/entropy.py
 pyDecision/algorithm/fucom.py
 pyDecision/algorithm/fuzzy_ahp.py
 pyDecision/algorithm/fuzzy_aras.py
 pyDecision/algorithm/fuzzy_bwm.py
 pyDecision/algorithm/fuzzy_copras.py
+pyDecision/algorithm/fuzzy_critic.py
 pyDecision/algorithm/fuzzy_dematel.py
 pyDecision/algorithm/fuzzy_edas.py
+pyDecision/algorithm/fuzzy_fucom.py
+pyDecision/algorithm/fuzzy_merec.py
 pyDecision/algorithm/fuzzy_moora.py
 pyDecision/algorithm/fuzzy_ocra.py
 pyDecision/algorithm/fuzzy_topsis.py
 pyDecision/algorithm/fuzzy_vikor.py
 pyDecision/algorithm/fuzzy_waspas.py
 pyDecision/algorithm/gra.py
 pyDecision/algorithm/idocriw.py
@@ -64,15 +67,18 @@
 pyDecision/algorithm/p_v.py
 pyDecision/algorithm/p_vi.py
 pyDecision/algorithm/p_xgaia.py
 pyDecision/algorithm/piv.py
 pyDecision/algorithm/psi.py
 pyDecision/algorithm/psi_m.py
 pyDecision/algorithm/regime.py
+pyDecision/algorithm/roc.py
 pyDecision/algorithm/rov.py
+pyDecision/algorithm/rrw.py
+pyDecision/algorithm/rsw.py
 pyDecision/algorithm/saw.py
 pyDecision/algorithm/smart.py
 pyDecision/algorithm/spotis.py
 pyDecision/algorithm/todim.py
 pyDecision/algorithm/topsis.py
 pyDecision/algorithm/vikor.py
 pyDecision/algorithm/waspas.py
```

### Comparing `pyDecision-4.4.7/setup.py` & `pyDecision-4.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyDecision',
-    version='4.4.7',
+    version='4.5.1',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyDecisions',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
```

