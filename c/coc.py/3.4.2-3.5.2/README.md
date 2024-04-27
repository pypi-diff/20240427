# Comparing `tmp/coc_py-3.4.2.tar.gz` & `tmp/coc_py-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coc_py-3.4.2.tar", last modified: Sat Apr 20 11:00:26 2024, max compression
+gzip compressed data, was "coc_py-3.5.2.tar", last modified: Sat Apr 27 17:31:55 2024, max compression
```

## Comparing `coc_py-3.4.2.tar` & `coc_py-3.5.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:26.560305 coc_py-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-20 11:00:22.000000 coc_py-3.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-20 11:00:22.000000 coc_py-3.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-20 11:00:26.560305 coc_py-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-20 11:00:22.000000 coc_py-3.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:26.544305 coc_py-3.4.2/coc/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15861 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/clans.py
--rw-r--r--   0 runner    (1001) docker     (127)    83280 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/entry_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    39787 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    11319 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/events.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:26.536305 coc_py-3.4.2/coc/ext/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:26.544305 coc_py-3.4.2/coc/ext/discordlinks/
--rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/ext/discordlinks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:26.544305 coc_py-3.4.2/coc/ext/fullwarapi/
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/ext/fullwarapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:26.548305 coc_py-3.4.2/coc/ext/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/ext/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/ext/triggers/cron.py
--rw-r--r--   0 runner    (1001) docker     (127)    21909 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/ext/triggers/triggers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/hero.py
--rw-r--r--   0 runner    (1001) docker     (127)    23363 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)    21407 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/miscmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/player_clan.py
--rw-r--r--   0 runner    (1001) docker     (127)    30035 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/players.py
--rw-r--r--   0 runner    (1001) docker     (127)    19577 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/raid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/spell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:26.556305 coc_py-3.4.2/coc/static/
--rw-r--r--   0 runner    (1001) docker     (127)  1291668 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/buildings.json
--rw-r--r--   0 runner    (1001) docker     (127)  1965460 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/characters.json
--rw-r--r--   0 runner    (1001) docker     (127)   220960 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/equipment.json
--rw-r--r--   0 runner    (1001) docker     (127)   648975 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/heroes.json
--rw-r--r--   0 runner    (1001) docker     (127)   255626 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/pets.json
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/spell_ids.json
--rw-r--r--   0 runner    (1001) docker     (127)   566845 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/spells.json
--rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/supers.json
--rw-r--r--   0 runner    (1001) docker     (127)  1025147 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/texts_EN.json
--rw-r--r--   0 runner    (1001) docker     (127)    92590 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/townhall_levels.json
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/troop_ids.json
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/update_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/troop.py
--rw-r--r--   0 runner    (1001) docker     (127)    19780 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/war_attack.py
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/war_clans.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/war_members.py
--rw-r--r--   0 runner    (1001) docker     (127)    19658 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/wars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:26.560305 coc_py-3.4.2/coc.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-20 11:00:26.000000 coc_py-3.4.2/coc.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-20 11:00:26.000000 coc_py-3.4.2/coc.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 11:00:26.000000 coc_py-3.4.2/coc.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-20 11:00:26.000000 coc_py-3.4.2/coc.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-20 11:00:26.000000 coc_py-3.4.2/coc.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-20 11:00:22.000000 coc_py-3.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-20 11:00:22.000000 coc_py-3.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 11:00:26.560305 coc_py-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-20 11:00:22.000000 coc_py-3.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:26.560305 coc_py-3.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_capitalraidseasons.py
--rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_clans.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_clash_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_miscmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_players.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_troop_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_wars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:55.009181 coc_py-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-27 17:31:50.000000 coc_py-3.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-27 17:31:50.000000 coc_py-3.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-27 17:31:55.009181 coc_py-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-27 17:31:50.000000 coc_py-3.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:54.997182 coc_py-3.5.2/coc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15861 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/clans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83547 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/entry_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41186 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12992 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/events.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:54.993182 coc_py-3.5.2/coc/ext/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:54.997182 coc_py-3.5.2/coc/ext/discordlinks/
+-rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/ext/discordlinks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:54.997182 coc_py-3.5.2/coc/ext/fullwarapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/ext/fullwarapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:54.997182 coc_py-3.5.2/coc/ext/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/ext/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/ext/triggers/cron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21909 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/ext/triggers/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/hero.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24212 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21407 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/miscmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/player_clan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30024 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/players.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19577 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/raid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/spell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:55.009181 coc_py-3.5.2/coc/static/
+-rw-r--r--   0 runner    (1001) docker     (127)  1291668 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/buildings.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1965460 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/characters.json
+-rw-r--r--   0 runner    (1001) docker     (127)   220960 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/equipment.json
+-rw-r--r--   0 runner    (1001) docker     (127)   648975 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/heroes.json
+-rw-r--r--   0 runner    (1001) docker     (127)   255626 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/pets.json
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/spell_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)   566845 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/spells.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/supers.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1025147 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/texts_EN.json
+-rw-r--r--   0 runner    (1001) docker     (127)    92590 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/townhall_levels.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/troop_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/static/update_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/troop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19780 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/war_attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/war_clans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/war_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19658 2024-04-27 17:31:50.000000 coc_py-3.5.2/coc/wars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:55.009181 coc_py-3.5.2/coc.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-27 17:31:54.000000 coc_py-3.5.2/coc.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-27 17:31:54.000000 coc_py-3.5.2/coc.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:31:54.000000 coc_py-3.5.2/coc.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-27 17:31:54.000000 coc_py-3.5.2/coc.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-27 17:31:54.000000 coc_py-3.5.2/coc.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-27 17:31:50.000000 coc_py-3.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-27 17:31:50.000000 coc_py-3.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 17:31:55.013182 coc_py-3.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-27 17:31:50.000000 coc_py-3.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:55.009181 coc_py-3.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_capitalraidseasons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_clans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_clash_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_miscmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_players.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_troop_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-27 17:31:50.000000 coc_py-3.5.2/tests/test_wars.py
```

### Comparing `coc_py-3.4.2/LICENSE` & `coc_py-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/PKG-INFO` & `coc_py-3.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coc.py
-Version: 3.4.2
+Version: 3.5.2
 Summary: A python wrapper for the Clash of Clans API
 Author: mathsman5133
 Maintainer: majordoobie, MagicTheDev, Kuchenmampfer, lukasthaler, doluk
 License: MIT
 Project-URL: documentation, https://cocpy.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/mathsman5133/coc.py
 Project-URL: changelog, https://cocpy.readthedocs.io/en/latest/miscellaneous/changelog.html
```

### Comparing `coc_py-3.4.2/README.rst` & `coc_py-3.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/__init__.py` & `coc_py-3.5.2/coc/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-__version__ = "3.4.2"
+__version__ = "3.5.2"
 
 from .abc import BasePlayer, BaseClan
 from .clans import RankedClan, Clan
 from .client import Client
 from .events import PlayerEvents, ClanEvents, WarEvents, EventsClient, ClientEvents
 from .enums import (
     PlayerHouseElementType,
```

### Comparing `coc_py-3.4.2/coc/abc.py` & `coc_py-3.5.2/coc/abc.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/clans.py` & `coc_py-3.5.2/coc/clans.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/client.py` & `coc_py-3.5.2/coc/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,21 +138,25 @@
 
     raw_attribute: :class:`bool`
         The option to enable the _raw_data attribute for most objects in the library. This attribute will contain
         the original json data as returned by the API. This can be useful if you want to store a response in a database
         for later use or are interested in new things that coc.py does not support otherwise yet. But because this
         increases the memory footprint and is not needed for most use cases, this defaults to ``False``.
 
+    base_url: :class:`str`
+        The base URL to use for API requests. Defaults to "https://api.clashofclans.com/v1"
+
     Attributes
     ----------
     loop : :class:`asyncio.AbstractEventLoop`
         The loop that is used for HTTP requests
     """
 
     __slots__ = (
+        "base_url",
         "loop",
         "correct_key_count",
         "key_names",
         "key_scopes",
         "throttle_limit",
         "throttler",
         "timeout",
@@ -188,14 +192,15 @@
         connector=None,
         timeout: float = 30.0,
         cache_max_size: int = 10000,
         stats_max_size: int = 1000,
         load_game_data: LoadGameData = LoadGameData(default=True),
         realtime=False,
         raw_attribute=False,
+        base_url: str = "https://api.clashofclans.com/v1",
         **kwargs,
     ):
 
         self.loop = loop or asyncio.get_event_loop()
 
         self.correct_key_count = max(min(KEY_MAXIMUM, key_count), KEY_MINIMUM)
 
@@ -212,15 +217,15 @@
         self.stats_max_size = stats_max_size
 
         self.http = None  # set in method login()
         self.realtime = realtime
         self.raw_attribute = raw_attribute
         self.correct_tags = correct_tags
         self.load_game_data = load_game_data
-
+        self.base_url = base_url
         # cache
         self._players = {}
         self._clans = {}
         self._wars = {}
 
     async def __aenter__(self):
         return self
@@ -237,14 +242,15 @@
             key_scopes=self.key_scopes,
             loop=self.loop,
             key_count=self.correct_key_count,
             throttle_limit=self.throttle_limit,
             throttler=self.throttler,
             cache_max_size=self.cache_max_size,
             stats_max_size=self.stats_max_size,
+            base_url=self.base_url,
         )
 
     def _load_holders(self):
         with open(ENGLISH_ALIAS_PATH) as fp:
             english_aliases = ujson.load(fp)
 
         with open(BUILDING_FILE_PATH) as fp:
```

### Comparing `coc_py-3.4.2/coc/entry_logs.py` & `coc_py-3.5.2/coc/entry_logs.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/enums.py` & `coc_py-3.5.2/coc/enums.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/errors.py` & `coc_py-3.5.2/coc/errors.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/events.py` & `coc_py-3.5.2/coc/events.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,14 +78,17 @@
             return getattr(self.cls, item)
         except AttributeError:
             pass
 
         if self.cls.event_type == "client":
             return self.cls.__getattr__(self.cls, item)
 
+        if "versus" in item:
+            item = item.replace("versus", "builder_base")
+
         # handle member_x events:
         if "member_" in item and item != "member_count":
             item = item.replace("member_", "")
             nested = True
         else:
             nested = False
 
@@ -271,14 +274,40 @@
             hero_upgrades = (n for n in player.heroes if n not in set(cached_player.heroes))
             for hero in hero_upgrades:
                 await callback(cached_player, player, hero)
 
         return _ValidateEvent.shortcut_register(wrapped, tags, custom_class, retry_interval, PlayerEvents.event_type)
 
     @classmethod
+    def equipment_change(cls, tags=None, custom_class=None, retry_interval=None):
+        """Event for when a player has upgraded or unlocked an equipment."""
+
+        async def wrapped(cached_player, player, callback):
+            equipment_upgrades = (n for n in player.equipment if n not in set(cached_player.equipment))
+            for equipment in equipment_upgrades:
+                await callback(cached_player, player, equipment)
+
+        return _ValidateEvent.shortcut_register(wrapped, tags, custom_class, retry_interval, PlayerEvents.event_type)
+
+    @classmethod
+    def active_equipment_change(cls, tags=None, custom_class=None, retry_interval=None):
+        """Event for when a player has changed their active equipment."""
+
+        async def wrapped(cached_player, player, callback):
+            for hero in player.heroes:
+                cached_hero = cached_player.get_hero(hero.name)
+                if not cached_hero:
+                    continue
+                for equipment in hero.equipment:
+                    if cached_hero and equipment not in cached_hero.equipment:
+                        await callback(cached_player, player, hero, equipment)
+
+        return _ValidateEvent.shortcut_register(wrapped, tags, custom_class, retry_interval, PlayerEvents.event_type)
+
+    @classmethod
     def joined_clan(cls, tags=None, custom_class=None, retry_interval=None):
         """Event for when a player has joined a new clan."""
 
         async def wrapped(cached_player, player, callback):
             if cached_player.clan is None and player.clan is not None:
                 await callback(cached_player, player)
             elif cached_player.clan is not None and player.clan is not None and cached_player.clan != player.clan:
```

### Comparing `coc_py-3.4.2/coc/events.pyi` & `coc_py-3.5.2/coc/events.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,20 @@
     def badge(cls, tags: Iterable = None, custom_class: _ClanType = Clan, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def level(cls, tags: Iterable = None, custom_class: _ClanType = Clan, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def points(cls, tags: Iterable = None, custom_class: _ClanType = Clan, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def versus_points(cls, tags: Iterable = None, custom_class: _ClanType = Clan, retry_interval: int = None) -> _EventDecoratorReturn: ...
+
+    @classmethod
+    def builder_base_points(cls,
+                            tags: Iterable = None,
+                            custom_class: _ClanType = Clan,
+                            retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def member_count(cls, tags: Iterable = None, custom_class: _ClanType = Clan, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def location(cls, tags: Iterable = None, custom_class: _ClanType = Clan, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def type(cls, tags: Iterable = None, custom_class: _ClanType = Clan, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
@@ -73,15 +79,26 @@
     @classmethod
     def member_clan_rank(cls, tags: Iterable = None, custom_class: _ClanType = Clan, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def member_clan_previous_rank(cls, tags: Iterable = None, custom_class: _ClanType = Clan, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def member_versus_trophies(cls, tags: Iterable = None, custom_class: _ClanType = Clan, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
+    def member_builder_base_trophies(cls,
+                                     tags: Iterable = None,
+                                     custom_class: _ClanType = Clan,
+                                     retry_interval: int = None) -> _EventDecoratorReturn: ...
+    @classmethod
     def member_versus_rank(cls, tags: Iterable = None, custom_class: _ClanType = Clan, retry_interval: int = None) -> _EventDecoratorReturn: ...
+
+    @classmethod
+    def member_builder_base_rank(cls,
+                                 tags: Iterable = None,
+                                 custom_class: _ClanType = Clan,
+                                 retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def member_donations(cls, tags: Iterable = None, custom_class: _ClanType = Clan, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def member_received(cls, tags: Iterable = None, custom_class: _ClanType = Clan, retry_interval: int = None) -> _EventDecoratorReturn: ...
 
 class PlayerEvents:
     event_type: str
@@ -91,14 +108,20 @@
     def name(cls, tags: Iterable = None, custom_class: _PlayerType = Player, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def exp_level(cls, tags: Iterable = None, custom_class: _PlayerType = Player, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def trophies(cls, tags: Iterable = None, custom_class: _PlayerType = Player, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def versus_trophies(cls, tags: Iterable = None, custom_class: _PlayerType = Player, retry_interval: int = None) -> _EventDecoratorReturn: ...
+
+    @classmethod
+    def builder_base_trophies(cls,
+                              tags: Iterable = None,
+                              custom_class: _PlayerType = Player,
+                              retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def clan_rank(cls, tags: Iterable = None, custom_class: _PlayerType = Player, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def clan_previous_rank(cls, tags: Iterable = None, custom_class: _PlayerType = Player, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def donations(cls, tags: Iterable = None, custom_class: _PlayerType = Player, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
@@ -118,17 +141,26 @@
     @classmethod
     def builder_hall(cls, tags: Iterable = None, custom_class: _PlayerType = Player, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def best_versus_trophies(cls, tags: Iterable = None, custom_class: _PlayerType = Player, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def versus_attack_wins(cls, tags: Iterable = None, custom_class: _PlayerType = Player, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
+    def best_builder_base_trophies(cls,
+                                   tags: Iterable = None,
+                                   custom_class: _PlayerType = Player,
+                                   retry_interval: int = None) -> _EventDecoratorReturn: ...
+    @classmethod
     def legend_statistics(cls, tags: Iterable = None, custom_class: _PlayerType = Player, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def labels(cls, tags: Iterable = None, custom_class: _PlayerType = Player, retry_interval: int = None) -> _EventDecoratorReturn: ...
+    @classmethod
+    def equipment_change(cls, tags: Iterable = None, custom_class: _PlayerType = Player, retry_interval: int = None) -> _EventDecoratorReturn: ...
+    @classmethod
+    def active_equipment_change(cls, tags: Iterable = None, custom_class: _PlayerType = Player, retry_interval: int = None) -> _EventDecoratorReturn: ...
 
 class WarEvents:
     event_type: str
     @classmethod
     def war_attack(cls, tags: Iterable = None, custom_class: Type[ClanWar] = ClanWar, retry_interval: int = None) -> _EventDecoratorReturn: ...
     @classmethod
     def state(cls, tags: Iterable = None, custom_class: Type[ClanWar] = ClanWar, retry_interval: int = None) -> _EventDecoratorReturn: ...
```

### Comparing `coc_py-3.4.2/coc/ext/discordlinks/__init__.py` & `coc_py-3.5.2/coc/ext/discordlinks/__init__.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/ext/fullwarapi/__init__.py` & `coc_py-3.5.2/coc/ext/fullwarapi/__init__.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/ext/triggers/cron.py` & `coc_py-3.5.2/coc/ext/triggers/cron.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/ext/triggers/triggers.py` & `coc_py-3.5.2/coc/ext/triggers/triggers.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/hero.py` & `coc_py-3.5.2/coc/hero.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/http.py` & `coc_py-3.5.2/coc/http.py`

 * *Files 7% similar despite different names*

```diff
@@ -140,39 +140,41 @@
     async def __aexit__(self, exception_type, exception, traceback):
         pass
 
 
 class Route:
     """Helper class to create endpoint URLs."""
 
-    BASE = "https://api.clashofclans.com/v1"
-
-    def __init__(self, method: str, path: str, **kwargs: dict):
+    def __init__(self, method: str, base: str, path: str, **kwargs: dict):
         """
         The class is used to create the final URL used to fetch the data
         from the API. The parameters that are passed to the API are all in
         the GET request packet. This class will parse the `kwargs` dictionary
         and concatenate any parameters passed in.
 
         Parameters
         ----------
         method:
             :class:`str`: HTTP method used for the HTTP request
+        base:
+            :class:`str`: Base URL used for the HTTP request
         path:
             :class:`str`: URL path used for the HTTP request
         kwargs:
             :class:`dict`: Optional options used to concatenate into the final
             URL
         """
         if "#" in path:
             path = path.replace("#", "%23")
 
         self.method = method
         self.path = path
-        url = self.BASE + self.path
+        self.base = base
+
+        url = self.base + self.path
 
         if kwargs:
             self.url = "{}?{}".format(url, urlencode({k: v for k, v in kwargs.items() if v is not None}))
         else:
             self.url = url
 
     @property
@@ -192,15 +194,16 @@
             password,
             key_names,
             key_count,
             key_scopes,
             throttle_limit,
             throttler=BasicThrottler,
             cache_max_size=10000,
-            stats_max_size=1000
+            stats_max_size=1000,
+            base_url="https://api.clashofclans.com/v1",
     ):
         self.client = client
         self.loop = loop
         self.email = email
         self.password = password
         self.key_names = key_names
         self.key_count = key_count
@@ -209,15 +212,20 @@
         per_second = key_count * throttle_limit
 
         self.__session = None
         self.__lock = asyncio.Semaphore(per_second)
         self.cache = cache_max_size and FIFO(cache_max_size)
         self._cache_remove_count = 0
         self.stats = stats_max_size and HTTPStats(max_size=stats_max_size)
-
+        if base_url and isinstance(base_url, str) and len(base_url) > 0:
+            if base_url.endswith("/"):
+                base_url = base_url[:-1]
+            self.base_url = base_url
+        else:
+            raise ValueError("base_url must be a string and not empty.")
         if issubclass(throttler, BasicThrottler):
             self.__throttle = throttler(1 / per_second)
         elif issubclass(throttler, BatchThrottler):
             self.__throttle = throttler(per_second)
         else:
             raise TypeError("throttler must be either BasicThrottler or BatchThrottler.")
 
@@ -374,116 +382,116 @@
                 raise GatewayError(response, data)
 
             raise HTTPException(response, data)
 
     # clans
 
     def search_clans(self, **kwargs):
-        return self.request(Route("GET", "/clans", **kwargs))
+        return self.request(Route("GET", self.base_url, "/clans", **kwargs))
 
     def get_clan(self, tag):
-        return self.request(Route("GET", "/clans/{}".format(tag)))
+        return self.request(Route("GET", self.base_url, "/clans/{}".format(tag)))
 
     def get_clan_members(self, tag, **kwargs):
-        return self.request(Route("GET", "/clans/{}/members".format(tag), **kwargs))
+        return self.request(Route("GET", self.base_url, "/clans/{}/members".format(tag), **kwargs))
 
     def get_clan_war_log(self, tag, **kwargs):
-        return self.request(Route("GET", "/clans/{}/warlog".format(tag), **kwargs))
+        return self.request(Route("GET", self.base_url, "/clans/{}/warlog".format(tag), **kwargs))
 
     def get_clan_current_war(self, tag, realtime=None):
-        return self.request(Route("GET", "/clans/{}/currentwar".format(tag) + (
+        return self.request(Route("GET", self.base_url, "/clans/{}/currentwar".format(tag) + (
                                          '?realtime=true' if realtime or (realtime is None and self.client.realtime)
                                          else '')))
 
     def get_clan_war_league_group(self, tag, realtime=None):
-        return self.request(Route("GET", "/clans/{}/currentwar/leaguegroup".format(tag) + (
+        return self.request(Route("GET", self.base_url, "/clans/{}/currentwar/leaguegroup".format(tag) + (
                                          '?realtime=true' if realtime or (realtime is None and self.client.realtime)
                                          else '')))
 
     def get_cwl_wars(self, war_tag, realtime = None):
-        return self.request(Route("GET", "/clanwarleagues/wars/{}".format(war_tag) + (
+        return self.request(Route("GET", self.base_url, "/clanwarleagues/wars/{}".format(war_tag) + (
                                          '?realtime=true' if realtime or (realtime is None and self.client.realtime)
                                          else '')))
 
     def get_clan_raid_log(self, tag, **kwargs):
-        return self.request(Route("GET", "/clans/{}/capitalraidseasons".format(tag), **kwargs))
+        return self.request(Route("GET", self.base_url, "/clans/{}/capitalraidseasons".format(tag), **kwargs))
 
     # locations
 
     def search_locations(self, **kwargs):
-        return self.request(Route("GET", "/locations", **kwargs))
+        return self.request(Route("GET", self.base_url, "/locations", **kwargs))
 
     def get_location(self, location_id):
-        return self.request(Route("GET", "/locations/{}".format(location_id)))
+        return self.request(Route("GET", self.base_url, "/locations/{}".format(location_id)))
 
     def get_location_clans(self, location_id, **kwargs):
-        return self.request(Route("GET", "/locations/{}/rankings/clans".format(location_id), **kwargs))
+        return self.request(Route("GET", self.base_url, "/locations/{}/rankings/clans".format(location_id), **kwargs))
 
     def get_location_players(self, location_id, **kwargs):
-        return self.request(Route("GET", "/locations/{}/rankings/players".format(location_id), **kwargs))
+        return self.request(Route("GET", self.base_url, "/locations/{}/rankings/players".format(location_id), **kwargs))
 
     def get_location_clans_builder_base(self, location_id, **kwargs):
-        return self.request(Route("GET", "/locations/{}/rankings/clans-builder-base".format(location_id), **kwargs))
+        return self.request(Route("GET", self.base_url, "/locations/{}/rankings/clans-builder-base".format(location_id), **kwargs))
 
     def get_location_clans_capital(self, location_id, **kwargs):
-        return self.request(Route("GET", "/locations/{}/rankings/capitals".format(location_id), **kwargs))
+        return self.request(Route("GET", self.base_url, "/locations/{}/rankings/capitals".format(location_id), **kwargs))
 
     def get_location_players_builder_base(self, location_id, **kwargs):
-        return self.request(Route("GET", "/locations/{}/rankings/players-builder-base".format(location_id), **kwargs))
+        return self.request(Route("GET", self.base_url, "/locations/{}/rankings/players-builder-base".format(location_id), **kwargs))
 
     # leagues
 
     def search_leagues(self, **kwargs):
-        return self.request(Route("GET", "/leagues", **kwargs))
+        return self.request(Route("GET", self.base_url, "/leagues", **kwargs))
 
     def search_capital_leagues(self, **kwargs):
-        return self.request(Route("GET", "/capitalleagues", **kwargs))
+        return self.request(Route("GET", self.base_url, "/capitalleagues", **kwargs))
 
     def search_war_leagues(self, **kwargs):
-        return self.request(Route("GET", "/warleagues", **kwargs))
+        return self.request(Route("GET", self.base_url, "/warleagues", **kwargs))
 
     def search_builder_base_leagues(self, **kwargs):
-        return self.request(Route("GET", "/builderbaseleagues", **kwargs))
+        return self.request(Route("GET", self.base_url, "/builderbaseleagues", **kwargs))
 
     def get_league(self, league_id):
-        return self.request(Route("GET", "/leagues/{}".format(league_id)))
+        return self.request(Route("GET", self.base_url, "/leagues/{}".format(league_id)))
 
     def get_capital_league(self, league_id):
-        return self.request(Route("GET", "/capitalleagues/{}".format(league_id)))
+        return self.request(Route("GET", self.base_url, "/capitalleagues/{}".format(league_id)))
 
     def get_war_league(self, league_id):
-        return self.request(Route("GET", "/warleagues/{}".format(league_id)))
+        return self.request(Route("GET", self.base_url, "/warleagues/{}".format(league_id)))
 
     def get_builder_base_league(self, league_id):
-        return self.request(Route("GET", "/builderbaseleagues/{}".format(league_id)))
+        return self.request(Route("GET", self.base_url, "/builderbaseleagues/{}".format(league_id)))
 
     def get_league_seasons(self, league_id, **kwargs):
-        return self.request(Route("GET", "/leagues/{}/seasons".format(league_id), **kwargs))
+        return self.request(Route("GET", self.base_url, "/leagues/{}/seasons".format(league_id), **kwargs))
 
     def get_league_season_info(self, league_id, season_id, **kwargs):
-        return self.request(Route("GET", "/leagues/{}/seasons/{}".format(league_id, season_id), **kwargs))
+        return self.request(Route("GET", self.base_url, "/leagues/{}/seasons/{}".format(league_id, season_id), **kwargs))
 
     # players
 
     def get_player(self, player_tag):
-        return self.request(Route("GET", "/players/{}".format(player_tag)))
+        return self.request(Route("GET", self.base_url, "/players/{}".format(player_tag)))
 
     def verify_player_token(self, player_tag, token):
-        return self.request(Route("POST", "/players/{}/verifytoken".format(player_tag)), json={"token": token})
+        return self.request(Route("POST", self.base_url, "/players/{}/verifytoken".format(player_tag)), json={"token": token})
 
     # labels
 
     def get_clan_labels(self, **kwargs):
-        return self.request(Route("GET", "/labels/clan", **kwargs))
+        return self.request(Route("GET", self.base_url, "/labels/clan", **kwargs))
 
     def get_player_labels(self, **kwargs):
-        return self.request(Route("GET", "/labels/players", **kwargs))
+        return self.request(Route("GET", self.base_url, "/labels/players", **kwargs))
 
     def get_current_goldpass_season(self):
-        return self.request(Route("GET", "/goldpass/seasons/current"))
+        return self.request(Route("GET", self.base_url, "/goldpass/seasons/current"))
 
     # key updating management
 
     async def initialise_keys(self):
         LOG.debug("Initialising keys from the developer site.")
         self.initialising_keys.clear()
```

### Comparing `coc_py-3.4.2/coc/iterators.py` & `coc_py-3.5.2/coc/iterators.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/miscmodels.py` & `coc_py-3.5.2/coc/miscmodels.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/player_clan.py` & `coc_py-3.5.2/coc/player_clan.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/players.py` & `coc_py-3.5.2/coc/players.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,16 @@
         The member's current league.
     builder_base_league: :class:`BaseLeague`
         The member's current builder base league.
     trophies: :class:`int`
         The member's trophy count.
     builder_base_trophies: :class:`int`
         The member's builder base trophy count.
+    town_hall: :class:`int`
+        The player's town hall level. In case the player hasn't logged in since 2019, this will be `0`.
     clan_rank: :class:`int`
         The member's rank in the clan.
     clan_previous_rank: :class:`int`
         The member's rank before the last leaderboard change
         (ie if Bob overtakes Jim in trophies, and they switch ranks on the leaderboard,
         and you want to find out their previous rankings, this will help.).
     builder_base_rank: :class:`int`
@@ -228,16 +230,14 @@
         The number of attacks the player has won this season.
     defense_wins: :class:`int`
         The number of defenses the player has won this season.
     best_trophies: :class:`int`
         The player's best recorded trophies for the home base.
     war_stars: :class:`int`
         The player's total war stars.
-    town_hall: :class:`int`
-        The player's town hall level.
     town_hall_weapon: Optional[:class:`int`]
         The player's town hall weapon level, or ``None`` if it doesn't exist.
     builder_hall: :class:`int`
         The player's builder hall level, or 0 if it hasn't been unlocked.
     best_builder_base_trophies: :class:`int`
         The player's best builder base trophy count.
     clan_capital_contributions: :class:`int`
@@ -253,15 +253,14 @@
 
     __slots__ = (
         "clan",
         "attack_wins",
         "defense_wins",
         "best_trophies",
         "war_stars",
-        "town_hall",
         "town_hall_weapon",
         "builder_hall",
         "best_builder_base_trophies",
         "clan_capital_contributions",
         "legend_statistics",
         "war_opted_in",
         "_achievements",
@@ -344,15 +343,14 @@
         super()._from_data(data)
         data_get = data.get
 
         self.attack_wins: int = data_get("attackWins")
         self.defense_wins: int = data_get("defenseWins")
         self.best_trophies: int = data_get("bestTrophies")
         self.war_stars: int = data_get("warStars")
-        self.town_hall: int = data_get("townHallLevel")
         self.town_hall_weapon: int = data_get("townHallWeaponLevel")
         self.builder_hall: int = data_get("builderHallLevel", 0)
         self.best_builder_base_trophies: int = data_get("bestBuilderBaseTrophies")
         self.clan_capital_contributions: int = data_get("clanCapitalContributions")
         self.legend_statistics = try_enum(LegendStatistics, data=data_get("legendStatistics"))
 
         try:
```

### Comparing `coc_py-3.4.2/coc/raid.py` & `coc_py-3.5.2/coc/raid.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/spell.py` & `coc_py-3.5.2/coc/spell.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/static/buildings.json` & `coc_py-3.5.2/coc/static/buildings.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/static/characters.json` & `coc_py-3.5.2/coc/static/characters.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/static/equipment.json` & `coc_py-3.5.2/coc/static/equipment.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/static/heroes.json` & `coc_py-3.5.2/coc/static/heroes.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/static/pets.json` & `coc_py-3.5.2/coc/static/pets.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/static/spells.json` & `coc_py-3.5.2/coc/static/spells.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/static/supers.json` & `coc_py-3.5.2/coc/static/supers.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/static/texts_EN.json` & `coc_py-3.5.2/coc/static/texts_EN.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/static/townhall_levels.json` & `coc_py-3.5.2/coc/static/townhall_levels.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/static/troop_ids.json` & `coc_py-3.5.2/coc/static/troop_ids.json`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/static/update_static.py` & `coc_py-3.5.2/coc/static/update_static.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/troop.py` & `coc_py-3.5.2/coc/troop.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/utils.py` & `coc_py-3.5.2/coc/utils.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/war_attack.py` & `coc_py-3.5.2/coc/war_attack.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/war_clans.py` & `coc_py-3.5.2/coc/war_clans.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/war_members.py` & `coc_py-3.5.2/coc/war_members.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc/wars.py` & `coc_py-3.5.2/coc/wars.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/coc.py.egg-info/PKG-INFO` & `coc_py-3.5.2/coc.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coc.py
-Version: 3.4.2
+Version: 3.5.2
 Summary: A python wrapper for the Clash of Clans API
 Author: mathsman5133
 Maintainer: majordoobie, MagicTheDev, Kuchenmampfer, lukasthaler, doluk
 License: MIT
 Project-URL: documentation, https://cocpy.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/mathsman5133/coc.py
 Project-URL: changelog, https://cocpy.readthedocs.io/en/latest/miscellaneous/changelog.html
```

### Comparing `coc_py-3.4.2/coc.py.egg-info/SOURCES.txt` & `coc_py-3.5.2/coc.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/pyproject.toml` & `coc_py-3.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coc.py"
 authors = [{ name = "mathsman5133" }]
 maintainers = [{ name = "majordoobie" }, { name = "MagicTheDev" }, { name = "Kuchenmampfer" },
     { name = "lukasthaler"}, { name = "doluk"}]
-version = "3.4.2"
+version = "3.5.2"
 description = "A python wrapper for the Clash of Clans API"
 requires-python = ">=3.7.3"
 readme = "README.rst"
 license = { text = "MIT" }
 keywords = ["coc", "clash of clans", "coc.py", "clash api"]
 classifiers = ["Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
```

### Comparing `coc_py-3.4.2/tests/test_capitalraidseasons.py` & `coc_py-3.5.2/tests/test_capitalraidseasons.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/tests/test_clans.py` & `coc_py-3.5.2/tests/test_clans.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/tests/test_clash_meta.py` & `coc_py-3.5.2/tests/test_clash_meta.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/tests/test_players.py` & `coc_py-3.5.2/tests/test_players.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/tests/test_troop_levels.py` & `coc_py-3.5.2/tests/test_troop_levels.py`

 * *Files identical despite different names*

### Comparing `coc_py-3.4.2/tests/test_wars.py` & `coc_py-3.5.2/tests/test_wars.py`

 * *Files identical despite different names*

