# Comparing `tmp/nokey-0.2.0.tar.gz` & `tmp/nokey-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nokey-0.2.0.tar", last modified: Sat Apr 20 15:25:31 2024, max compression
+gzip compressed data, was "nokey-0.3.0.tar", last modified: Sat Apr 27 13:50:43 2024, max compression
```

## Comparing `nokey-0.2.0.tar` & `nokey-0.3.0.tar`

### file list

```diff
@@ -1,76 +1,88 @@
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.120087 nokey-0.2.0/
--rw-------   0 root         (0) root         (0)     1068 2024-04-10 23:28:41.000000 nokey-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3516 2024-04-20 15:25:31.116087 nokey-0.2.0/PKG-INFO
--rw-------   0 root         (0) root         (0)     2995 2024-04-20 15:20:37.000000 nokey-0.2.0/README.md
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.872087 nokey-0.2.0/nokey/
--rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/__init__.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.892087 nokey-0.2.0/nokey/activities/
--rw-------   0 root         (0) root         (0)     5116 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/activities/bored_api.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.900087 nokey-0.2.0/nokey/animals/
--rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/animals/__init__.py
--rw-------   0 root         (0) root         (0)     2754 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/animals/dog_api.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.912087 nokey-0.2.0/nokey/calendar/
--rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/calendar/__init__.py
--rw-------   0 root         (0) root         (0)     4848 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/calendar/nager_date.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.920087 nokey-0.2.0/nokey/country_info/
--rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/country_info/__init__.py
--rw-------   0 root         (0) root         (0)     4824 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/country_info/rest_country.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.948087 nokey-0.2.0/nokey/developer_tools/
--rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/developer_tools/__init__.py
--rw-------   0 root         (0) root         (0)     3945 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/developer_tools/apis_guru.py
--rw-------   0 root         (0) root         (0)     2578 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/developer_tools/microlink.py
--rw-------   0 root         (0) root         (0)     7314 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/developer_tools/url_haus.py
--rw-------   0 root         (0) root         (0)     1621 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/developer_tools/url_shortener.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.960087 nokey-0.2.0/nokey/education/
--rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/education/__init__.py
--rw-------   0 root         (0) root         (0)     2348 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/education/university_domains_and_names.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.968087 nokey-0.2.0/nokey/finance/
--rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/finance/__init__.py
--rw-------   0 root         (0) root         (0)     1127 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/finance/wall_street_bets.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.980087 nokey-0.2.0/nokey/food/
--rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/food/__init__.py
--rw-------   0 root         (0) root         (0)     3198 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/food/fruityvice.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:30.996087 nokey-0.2.0/nokey/games/
--rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/games/__init__.py
--rw-------   0 root         (0) root         (0)     6542 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/games/free_to_game.py
--rw-------   0 root         (0) root         (0)     5382 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/games/open_trivia_db.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.008087 nokey-0.2.0/nokey/geolocation/
--rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/geolocation/__init__.py
--rw-------   0 root         (0) root         (0)     1045 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/geolocation/ip_api.py
--rw-------   0 root         (0) root         (0)     1874 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/geolocation/zippopotamus.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.020087 nokey-0.2.0/nokey/government/
--rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/government/__init__.py
--rw-------   0 root         (0) root         (0)    10654 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/government/federal_register.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.040087 nokey-0.2.0/nokey/helperFuncs/
--rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/helperFuncs/__init__.py
--rw-------   0 root         (0) root         (0)      822 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/helperFuncs/get_api_list.py
--rw-------   0 root         (0) root         (0)     2337 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/helperFuncs/make_request.py
--rw-------   0 root         (0) root         (0)      741 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/helperFuncs/nokey_apis.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.048087 nokey-0.2.0/nokey/inspiration/
--rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/inspiration/__init__.py
--rw-------   0 root         (0) root         (0)     5925 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/inspiration/dictum.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.060087 nokey-0.2.0/nokey/jokes/
--rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/jokes/__init__.py
--rw-------   0 root         (0) root         (0)     3004 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/jokes/joke_api.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.068087 nokey-0.2.0/nokey/language/
--rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/language/__init__.py
--rw-------   0 root         (0) root         (0)     1185 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/language/free_dictionary.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.080087 nokey-0.2.0/nokey/random/
--rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/random/__init__.py
--rw-------   0 root         (0) root         (0)     1119 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/random/random_user.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.088087 nokey-0.2.0/nokey/science/
--rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/science/__init__.py
--rw-------   0 root         (0) root         (0)     2948 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/science/nobel_prize.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.096087 nokey-0.2.0/nokey/spaceflight/
--rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/spaceflight/__init__.py
--rw-------   0 root         (0) root         (0)     8784 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/spaceflight/spaceflight_news.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.108087 nokey-0.2.0/nokey/weather/
--rw-------   0 root         (0) root         (0)        0 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/weather/__init__.py
--rw-------   0 root         (0) root         (0)    26115 2024-04-20 15:22:18.000000 nokey-0.2.0/nokey/weather/national_weather_service.py
-drwx------   0 root         (0) root         (0)        0 2024-04-20 15:25:31.112087 nokey-0.2.0/nokey.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3516 2024-04-20 15:25:30.000000 nokey-0.2.0/nokey.egg-info/PKG-INFO
--rw-------   0 root         (0) root         (0)     1511 2024-04-20 15:25:30.000000 nokey-0.2.0/nokey.egg-info/SOURCES.txt
--rw-------   0 root         (0) root         (0)        1 2024-04-20 15:25:30.000000 nokey-0.2.0/nokey.egg-info/dependency_links.txt
--rw-------   0 root         (0) root         (0)        6 2024-04-20 15:25:30.000000 nokey-0.2.0/nokey.egg-info/top_level.txt
--rw-------   0 root         (0) root         (0)      503 2024-04-20 15:23:04.000000 nokey-0.2.0/pyproject.toml
--rw-------   0 root         (0) root         (0)       38 2024-04-20 15:25:31.120087 nokey-0.2.0/setup.cfg
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.813063 nokey-0.3.0/
+-rw-------   0 root         (0) root         (0)     1068 2024-04-10 23:28:41.000000 nokey-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3685 2024-04-27 13:50:43.809063 nokey-0.3.0/PKG-INFO
+-rw-------   0 root         (0) root         (0)     3164 2024-04-27 13:46:03.000000 nokey-0.3.0/README.md
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.341063 nokey-0.3.0/nokey/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/__init__.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.373063 nokey-0.3.0/nokey/activities/
+-rw-------   0 root         (0) root         (0)     5116 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/activities/bored_api.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.389063 nokey-0.3.0/nokey/animals/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/animals/__init__.py
+-rw-------   0 root         (0) root         (0)     2754 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/animals/dog_api.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.401063 nokey-0.3.0/nokey/art_and_images/
+-rw-------   0 root         (0) root         (0)     7770 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/art_and_images/lorem_picsum.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.413063 nokey-0.3.0/nokey/books_and_literature/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/books_and_literature/__init__.py
+-rw-------   0 root         (0) root         (0)     6079 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/books_and_literature/gutendex.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.429063 nokey-0.3.0/nokey/calendar/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/calendar/__init__.py
+-rw-------   0 root         (0) root         (0)     4848 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/calendar/nager_date.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.445063 nokey-0.3.0/nokey/country_info/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/country_info/__init__.py
+-rw-------   0 root         (0) root         (0)     4740 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/country_info/rest_country.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.489063 nokey-0.3.0/nokey/developer_tools/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/developer_tools/__init__.py
+-rw-------   0 root         (0) root         (0)     3945 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/developer_tools/apis_guru.py
+-rw-------   0 root         (0) root         (0)     3564 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/developer_tools/filter_lists.py
+-rw-------   0 root         (0) root         (0)     2578 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/developer_tools/microlink.py
+-rw-------   0 root         (0) root         (0)     7314 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/developer_tools/url_haus.py
+-rw-------   0 root         (0) root         (0)     1621 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/developer_tools/url_shortener.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.505063 nokey-0.3.0/nokey/education/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/education/__init__.py
+-rw-------   0 root         (0) root         (0)     2348 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/education/university_domains_and_names.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.541063 nokey-0.3.0/nokey/finance_and_crypto/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/finance_and_crypto/__init__.py
+-rw-------   0 root         (0) root         (0)     5877 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/finance_and_crypto/coinmap.py
+-rw-------   0 root         (0) root         (0)     2513 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/finance_and_crypto/exchange_api.py
+-rw-------   0 root         (0) root         (0)     1127 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/finance_and_crypto/wall_street_bets.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.557063 nokey-0.3.0/nokey/food/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/food/__init__.py
+-rw-------   0 root         (0) root         (0)     3198 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/food/fruityvice.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.581063 nokey-0.3.0/nokey/games/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/games/__init__.py
+-rw-------   0 root         (0) root         (0)     6542 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/games/free_to_game.py
+-rw-------   0 root         (0) root         (0)     5382 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/games/open_trivia_db.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.605063 nokey-0.3.0/nokey/geolocation/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/geolocation/__init__.py
+-rw-------   0 root         (0) root         (0)     1045 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/geolocation/ip_api.py
+-rw-------   0 root         (0) root         (0)     1874 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/geolocation/zippopotamus.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.621063 nokey-0.3.0/nokey/government/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/government/__init__.py
+-rw-------   0 root         (0) root         (0)    10654 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/government/federal_register.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.657063 nokey-0.3.0/nokey/helperFuncs/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/helperFuncs/__init__.py
+-rw-------   0 root         (0) root         (0)      822 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/helperFuncs/get_api_list.py
+-rw-------   0 root         (0) root         (0)     3234 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/helperFuncs/make_request.py
+-rw-------   0 root         (0) root         (0)      953 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/helperFuncs/nokey_apis.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.669063 nokey-0.3.0/nokey/inspiration/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/inspiration/__init__.py
+-rw-------   0 root         (0) root         (0)     5925 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/inspiration/dictum.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.685063 nokey-0.3.0/nokey/jokes/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/jokes/__init__.py
+-rw-------   0 root         (0) root         (0)     3004 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/jokes/joke_api.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.701063 nokey-0.3.0/nokey/language/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/language/__init__.py
+-rw-------   0 root         (0) root         (0)     1185 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/language/free_dictionary.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.713063 nokey-0.3.0/nokey/random/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/random/__init__.py
+-rw-------   0 root         (0) root         (0)     1119 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/random/random_user.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.741063 nokey-0.3.0/nokey/science_and_nature/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/science_and_nature/__init__.py
+-rw-------   0 root         (0) root         (0)    50596 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/science_and_nature/integrated_taxonomic_information_system.py
+-rw-------   0 root         (0) root         (0)     2948 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/science_and_nature/nobel_prize.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.761063 nokey-0.3.0/nokey/spaceflight/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/spaceflight/__init__.py
+-rw-------   0 root         (0) root         (0)     8784 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/spaceflight/spaceflight_news.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.773063 nokey-0.3.0/nokey/tv_and_film/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/tv_and_film/__init__.py
+-rw-------   0 root         (0) root         (0)    43523 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/tv_and_film/star_trek_api.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.793063 nokey-0.3.0/nokey/weather/
+-rw-------   0 root         (0) root         (0)        0 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/weather/__init__.py
+-rw-------   0 root         (0) root         (0)    26115 2024-04-27 13:48:18.000000 nokey-0.3.0/nokey/weather/national_weather_service.py
+drwx------   0 root         (0) root         (0)        0 2024-04-27 13:50:43.801063 nokey-0.3.0/nokey.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3685 2024-04-27 13:50:42.000000 nokey-0.3.0/nokey.egg-info/PKG-INFO
+-rw-------   0 root         (0) root         (0)     1918 2024-04-27 13:50:43.000000 nokey-0.3.0/nokey.egg-info/SOURCES.txt
+-rw-------   0 root         (0) root         (0)        1 2024-04-27 13:50:42.000000 nokey-0.3.0/nokey.egg-info/dependency_links.txt
+-rw-------   0 root         (0) root         (0)        6 2024-04-27 13:50:42.000000 nokey-0.3.0/nokey.egg-info/top_level.txt
+-rw-------   0 root         (0) root         (0)      503 2024-04-27 13:39:55.000000 nokey-0.3.0/pyproject.toml
+-rw-------   0 root         (0) root         (0)       38 2024-04-27 13:50:43.817063 nokey-0.3.0/setup.cfg
```

### Comparing `nokey-0.2.0/LICENSE` & `nokey-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/PKG-INFO` & `nokey-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nokey
-Version: 0.2.0
+Version: 0.3.0
 Summary: A python package for accessing APIs that require no key.
 Author-email: Spyder Rex <billyjohnsonauthor@gmail.com>
 Project-URL: Homepage, https://github.com/SpyderRex/nokey
 Project-URL: Issues, https://github.com/Spyder/nokey/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -62,70 +62,89 @@
 ## Contributing
 We welcome contributions to expand the range of APIs available in nokey. Whether you want to add a new submodule or enhance an existing one, your contributions are valuable. To contribute, please fork the repository, make your changes, and submit a pull request.
 
 # Supported APIs
 ## country_info
 RestCountries
 
-## finance
+## finance_and_crypto
 Wallstreet Bets
 
+Exchange API
+
+Coinmap
+
 ## geolocation
 IP API
+
 Zippopotomus
 
 ## spaceflight
 Spaceflight News
 
 ## education
 University Domains and Names
 
 ## food
 Fruityvice
 
 ## random
 RandomUserGenerator
 
-##jokes
+## jokes
 JokeAPI
 
 ## animals
 DogAPI
 
-## science
+## science_and_nature
 Nobel Prize API
 
+Integrated Taxonomic Information System
+
 ## weather
 National Weather Service API
 
 ## developer_tools
 URL Shortener
+
 URLHaus
+
 APIsGuru
+
 Microlink
 
+FilterLists
+
 ## inspiration
 Dictum
 
 ## language
 Free Dictionary
 
 ## games
 Free To Game
+
 Open Trivia Database
 
 ## activities
 Bored API
 
 ## calendar
 Nager.Date
 
 ## government
 Federal Register
 
+## tv_and_film
+Star Trek API
+
+## books_and_literature
+Gutendex
+
 # Future Roadmap
 As the project grows, we envision expanding the collection of keyless APIs to cover a wide range of categories. Your feedback and contributions will play a crucial role in shaping the future of nokey.
 
 # License
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 # Documentation
```

### Comparing `nokey-0.2.0/README.md` & `nokey-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -48,70 +48,89 @@
 ## Contributing
 We welcome contributions to expand the range of APIs available in nokey. Whether you want to add a new submodule or enhance an existing one, your contributions are valuable. To contribute, please fork the repository, make your changes, and submit a pull request.
 
 # Supported APIs
 ## country_info
 RestCountries
 
-## finance
+## finance_and_crypto
 Wallstreet Bets
 
+Exchange API
+
+Coinmap
+
 ## geolocation
 IP API
+
 Zippopotomus
 
 ## spaceflight
 Spaceflight News
 
 ## education
 University Domains and Names
 
 ## food
 Fruityvice
 
 ## random
 RandomUserGenerator
 
-##jokes
+## jokes
 JokeAPI
 
 ## animals
 DogAPI
 
-## science
+## science_and_nature
 Nobel Prize API
 
+Integrated Taxonomic Information System
+
 ## weather
 National Weather Service API
 
 ## developer_tools
 URL Shortener
+
 URLHaus
+
 APIsGuru
+
 Microlink
 
+FilterLists
+
 ## inspiration
 Dictum
 
 ## language
 Free Dictionary
 
 ## games
 Free To Game
+
 Open Trivia Database
 
 ## activities
 Bored API
 
 ## calendar
 Nager.Date
 
 ## government
 Federal Register
 
+## tv_and_film
+Star Trek API
+
+## books_and_literature
+Gutendex
+
 # Future Roadmap
 As the project grows, we envision expanding the collection of keyless APIs to cover a wide range of categories. Your feedback and contributions will play a crucial role in shaping the future of nokey.
 
 # License
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 # Documentation
```

### Comparing `nokey-0.2.0/nokey/activities/bored_api.py` & `nokey-0.3.0/nokey/activities/bored_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/animals/dog_api.py` & `nokey-0.3.0/nokey/animals/dog_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/calendar/nager_date.py` & `nokey-0.3.0/nokey/calendar/nager_date.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/country_info/rest_country.py` & `nokey-0.3.0/nokey/country_info/rest_country.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,98 +55,91 @@
         """
         Returns information about countries that use a specific currency.
 
         Args:
         - currency (str): The currency code or name.
 
         Returns:
-        - list: A list of dictionaries containing information about countries using the currency,
-            or an error if no countries found.
+        - list: A list of dictionaries containing information about countries using the currency, or an error if no countries found.
         """
         endpoint = f"currency/{currency}"
         return mr.make_request(self.base_url+endpoint)
 
     def get_country_by_language(self, language):
         """
         Returns information about countries speaking a given language.
 
         Args:
         - language (str): The name of the spoken language of the country.
 
         Returns:
-        - list: A list of dictionaries containing information about countries using the language,
-            or an error if no countries found.
+        - list: A list of dictionaries containing information about countries using the language, or an error if no countries found.
         """
         endpoint = f"lang/{language}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_country_by_capital(self, capital):
         """
         Returns information about a country with the given capital
 
         Args:
         - capital (str): The name of the capital city.
 
         Returns:
-        - list: A list of dictionaries containing information about countries using the capital,
-            or an error if no countries found.
+        - list: A list of dictionaries containing information about countries using the capital, or an error if no countries found.
         """
         endpoint = f"capital/{capital}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_country_by_region(self, region):
         """
         Returns information about countries based on a given region.
 
         Args:
         - region (str): The name of the region.
 
         Returns:
-        - list: A list of dictionaries containing information about countries using the region,
-            or an error if no country is found.
+        - list: A list of dictionaries containing information about countries using the region, or an error if no country is found.
         """
         endpoint = f"region/{region}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_country_by_subregion(self, subregion):
         """
         Returns information about countries based on a given subregion.
 
         Args:
         - subregion (str): The name of the subregion.
 
         Returns:
-        - list: A list of dictionaries containing information about countries using the region,
-            or an error if no country is found.
+        - list: A list of dictionaries containing information about countries using the region, or an error if no country is found.
         """
         endpoint = f"subregion/{subregion}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_country_by_translation(self, translation):
         """
         Returns information about countries based on a translation of the name.
 
         Args:
         - translation (str): The name in a given translation.
 
         Returns:
-        - list: A list of dictionaries containing information about countries using the region,
-            or an error if no country is found.
+        - list: A list of dictionaries containing information about countries using the region, or an error if no country is found.
         """
         endpoint = f"translation/{translation}"
         return mr.make_request(self.base_url+endpoint)
         
     def get_all_countries(self):
         """
         Returns information about all countries listed in the API.
 
         Args:
         - None
 
         Returns:
-        - list: A list of dictionaries containing information about all the countries,
-            or an error if no data is found.
+        - list: A list of dictionaries containing information about all the countries, or an error if no data is found.
         """
         endpoint = "all"
         return mr.make_request(self.base_url+endpoint)
```

### Comparing `nokey-0.2.0/nokey/developer_tools/apis_guru.py` & `nokey-0.3.0/nokey/developer_tools/apis_guru.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/developer_tools/microlink.py` & `nokey-0.3.0/nokey/developer_tools/microlink.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/developer_tools/url_haus.py` & `nokey-0.3.0/nokey/developer_tools/url_haus.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/developer_tools/url_shortener.py` & `nokey-0.3.0/nokey/developer_tools/url_shortener.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/education/university_domains_and_names.py` & `nokey-0.3.0/nokey/education/university_domains_and_names.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/finance/wall_street_bets.py` & `nokey-0.3.0/nokey/finance_and_crypto/wall_street_bets.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/food/fruityvice.py` & `nokey-0.3.0/nokey/food/fruityvice.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/games/free_to_game.py` & `nokey-0.3.0/nokey/games/free_to_game.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/games/open_trivia_db.py` & `nokey-0.3.0/nokey/games/open_trivia_db.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/geolocation/ip_api.py` & `nokey-0.3.0/nokey/geolocation/ip_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/geolocation/zippopotamus.py` & `nokey-0.3.0/nokey/geolocation/zippopotamus.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/government/federal_register.py` & `nokey-0.3.0/nokey/government/federal_register.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/helperFuncs/get_api_list.py` & `nokey-0.3.0/nokey/helperFuncs/get_api_list.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/helperFuncs/make_request.py` & `nokey-0.3.0/nokey/helperFuncs/make_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         return {"error": f"An unexpected error occurred: {err}"}
 
 def make_request_with_params(url, params):
     """
     Make a request to an API if the API call requires params.
     
     Args:
-    - url (str): The base url of the API.
+    - url (str): The url of the API.
     - params (dict): The params to be included in the request.
     
     Returns:
     - dict: A dictionary containing either the response data or an error message.
     """
     try:
         response = requests.get(url, params)
@@ -56,8 +56,35 @@
         return {"error": "Request timed out."}
     except RequestException as req_err:
         # Handle other request exceptions
         return {"error": f"Request exception occurred: {req_err}"}
     except Exception as err:
         # Handle any other unexpected errors
         return {"error": f"An unexpected error occurred: {err}"}
+        
+def make_request_for_content(url):
+    """
+    Make a request to an API if the API call returns content other than in JSON format.
+    
+    Args:
+    - url (str): The url of the API.
+    
+    Returns:
+    - string: Text in any format containing either the response data or an error message.
+    """
+    try:
+        response = requests.get(url)
+        return response.content
+    except HTTPError as http_err:
+        # Handle HTTP error
+        return {"error": f"HTTP error occurred: {http_err}"}
+    except Timeout:
+        # Handle timeout error
+        return {"error": "Request timed out."}
+    except RequestException as req_err:
+        # Handle other request exceptions
+        return {"error": f"Request exception occurred: {req_err}"}
+    except Exception as err:
+        # Handle any other unexpected errors
+        return {"error": f"An unexpected error occurred: {err}"}
+
```

### Comparing `nokey-0.2.0/nokey/inspiration/dictum.py` & `nokey-0.3.0/nokey/inspiration/dictum.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/jokes/joke_api.py` & `nokey-0.3.0/nokey/jokes/joke_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/language/free_dictionary.py` & `nokey-0.3.0/nokey/language/free_dictionary.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/random/random_user.py` & `nokey-0.3.0/nokey/random/random_user.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/science/nobel_prize.py` & `nokey-0.3.0/nokey/science_and_nature/nobel_prize.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/spaceflight/spaceflight_news.py` & `nokey-0.3.0/nokey/spaceflight/spaceflight_news.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey/weather/national_weather_service.py` & `nokey-0.3.0/nokey/weather/national_weather_service.py`

 * *Files identical despite different names*

### Comparing `nokey-0.2.0/nokey.egg-info/PKG-INFO` & `nokey-0.3.0/nokey.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nokey
-Version: 0.2.0
+Version: 0.3.0
 Summary: A python package for accessing APIs that require no key.
 Author-email: Spyder Rex <billyjohnsonauthor@gmail.com>
 Project-URL: Homepage, https://github.com/SpyderRex/nokey
 Project-URL: Issues, https://github.com/Spyder/nokey/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -62,70 +62,89 @@
 ## Contributing
 We welcome contributions to expand the range of APIs available in nokey. Whether you want to add a new submodule or enhance an existing one, your contributions are valuable. To contribute, please fork the repository, make your changes, and submit a pull request.
 
 # Supported APIs
 ## country_info
 RestCountries
 
-## finance
+## finance_and_crypto
 Wallstreet Bets
 
+Exchange API
+
+Coinmap
+
 ## geolocation
 IP API
+
 Zippopotomus
 
 ## spaceflight
 Spaceflight News
 
 ## education
 University Domains and Names
 
 ## food
 Fruityvice
 
 ## random
 RandomUserGenerator
 
-##jokes
+## jokes
 JokeAPI
 
 ## animals
 DogAPI
 
-## science
+## science_and_nature
 Nobel Prize API
 
+Integrated Taxonomic Information System
+
 ## weather
 National Weather Service API
 
 ## developer_tools
 URL Shortener
+
 URLHaus
+
 APIsGuru
+
 Microlink
 
+FilterLists
+
 ## inspiration
 Dictum
 
 ## language
 Free Dictionary
 
 ## games
 Free To Game
+
 Open Trivia Database
 
 ## activities
 Bored API
 
 ## calendar
 Nager.Date
 
 ## government
 Federal Register
 
+## tv_and_film
+Star Trek API
+
+## books_and_literature
+Gutendex
+
 # Future Roadmap
 As the project grows, we envision expanding the collection of keyless APIs to cover a wide range of categories. Your feedback and contributions will play a crucial role in shaping the future of nokey.
 
 # License
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 # Documentation
```

### Comparing `nokey-0.2.0/nokey.egg-info/SOURCES.txt` & `nokey-0.3.0/nokey.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -5,27 +5,33 @@
 nokey.egg-info/PKG-INFO
 nokey.egg-info/SOURCES.txt
 nokey.egg-info/dependency_links.txt
 nokey.egg-info/top_level.txt
 nokey/activities/bored_api.py
 nokey/animals/__init__.py
 nokey/animals/dog_api.py
+nokey/art_and_images/lorem_picsum.py
+nokey/books_and_literature/__init__.py
+nokey/books_and_literature/gutendex.py
 nokey/calendar/__init__.py
 nokey/calendar/nager_date.py
 nokey/country_info/__init__.py
 nokey/country_info/rest_country.py
 nokey/developer_tools/__init__.py
 nokey/developer_tools/apis_guru.py
+nokey/developer_tools/filter_lists.py
 nokey/developer_tools/microlink.py
 nokey/developer_tools/url_haus.py
 nokey/developer_tools/url_shortener.py
 nokey/education/__init__.py
 nokey/education/university_domains_and_names.py
-nokey/finance/__init__.py
-nokey/finance/wall_street_bets.py
+nokey/finance_and_crypto/__init__.py
+nokey/finance_and_crypto/coinmap.py
+nokey/finance_and_crypto/exchange_api.py
+nokey/finance_and_crypto/wall_street_bets.py
 nokey/food/__init__.py
 nokey/food/fruityvice.py
 nokey/games/__init__.py
 nokey/games/free_to_game.py
 nokey/games/open_trivia_db.py
 nokey/geolocation/__init__.py
 nokey/geolocation/ip_api.py
@@ -40,13 +46,16 @@
 nokey/inspiration/dictum.py
 nokey/jokes/__init__.py
 nokey/jokes/joke_api.py
 nokey/language/__init__.py
 nokey/language/free_dictionary.py
 nokey/random/__init__.py
 nokey/random/random_user.py
-nokey/science/__init__.py
-nokey/science/nobel_prize.py
+nokey/science_and_nature/__init__.py
+nokey/science_and_nature/integrated_taxonomic_information_system.py
+nokey/science_and_nature/nobel_prize.py
 nokey/spaceflight/__init__.py
 nokey/spaceflight/spaceflight_news.py
+nokey/tv_and_film/__init__.py
+nokey/tv_and_film/star_trek_api.py
 nokey/weather/__init__.py
 nokey/weather/national_weather_service.py
```

