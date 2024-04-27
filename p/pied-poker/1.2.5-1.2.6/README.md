# Comparing `tmp/pied_poker-1.2.5.tar.gz` & `tmp/pied_poker-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pied_poker-1.2.5.tar", last modified: Fri Apr 26 23:49:18 2024, max compression
+gzip compressed data, was "pied_poker-1.2.6.tar", last modified: Fri Apr 26 23:52:55 2024, max compression
```

## Comparing `pied_poker-1.2.5.tar` & `pied_poker-1.2.6.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:49:18.543409 pied_poker-1.2.5/
--rw-r--r--   0 ellek      (501) staff       (20)      737 2024-04-26 23:49:18.543151 pied_poker-1.2.5/PKG-INFO
--rw-r--r--   0 ellek      (501) staff       (20)    31804 2024-01-10 19:08:36.000000 pied_poker-1.2.5/README.md
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:49:18.525592 pied_poker-1.2.5/pied_poker/
--rw-r--r--   0 ellek      (501) staff       (20)     2698 2024-04-26 23:49:00.000000 pied_poker-1.2.5/pied_poker/__init__.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:49:18.528732 pied_poker-1.2.5/pied_poker/card/
--rw-r--r--   0 ellek      (501) staff       (20)      164 2022-03-21 04:52:37.000000 pied_poker-1.2.5/pied_poker/card/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)     1791 2024-04-09 07:53:12.000000 pied_poker-1.2.5/pied_poker/card/card.py
--rw-r--r--   0 ellek      (501) staff       (20)      379 2022-03-21 04:52:37.000000 pied_poker-1.2.5/pied_poker/card/comparable.py
--rw-r--r--   0 ellek      (501) staff       (20)     2157 2023-01-15 06:59:01.000000 pied_poker-1.2.5/pied_poker/card/rank.py
--rw-r--r--   0 ellek      (501) staff       (20)      824 2023-01-08 20:45:48.000000 pied_poker-1.2.5/pied_poker/card/suit.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:49:18.529445 pied_poker-1.2.5/pied_poker/deck/
--rw-r--r--   0 ellek      (501) staff       (20)       38 2022-03-21 04:52:37.000000 pied_poker-1.2.5/pied_poker/deck/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)     2450 2023-08-19 21:24:44.000000 pied_poker-1.2.5/pied_poker/deck/deck.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:49:18.534168 pied_poker-1.2.5/pied_poker/hand/
--rw-r--r--   0 ellek      (501) staff       (20)      724 2023-08-21 04:17:06.000000 pied_poker-1.2.5/pied_poker/hand/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)    10894 2023-12-23 23:23:25.000000 pied_poker-1.2.5/pied_poker/hand/base_hand.py
--rw-r--r--   0 ellek      (501) staff       (20)     1061 2023-01-25 00:26:09.000000 pied_poker-1.2.5/pied_poker/hand/empty_hand.py
--rw-r--r--   0 ellek      (501) staff       (20)     3215 2023-01-30 23:07:57.000000 pied_poker-1.2.5/pied_poker/hand/flush.py
--rw-r--r--   0 ellek      (501) staff       (20)     2567 2023-01-10 07:31:28.000000 pied_poker-1.2.5/pied_poker/hand/four_of_a_kind.py
--rw-r--r--   0 ellek      (501) staff       (20)     3511 2023-06-08 21:06:49.000000 pied_poker-1.2.5/pied_poker/hand/full_house.py
--rw-r--r--   0 ellek      (501) staff       (20)     3375 2023-06-08 21:28:48.000000 pied_poker-1.2.5/pied_poker/hand/high_card.py
--rw-r--r--   0 ellek      (501) staff       (20)      853 2023-08-21 04:23:37.000000 pied_poker-1.2.5/pied_poker/hand/killer_card.py
--rw-r--r--   0 ellek      (501) staff       (20)     2913 2023-01-10 07:31:44.000000 pied_poker-1.2.5/pied_poker/hand/one_pair.py
--rw-r--r--   0 ellek      (501) staff       (20)      858 2023-12-23 23:24:38.000000 pied_poker-1.2.5/pied_poker/hand/out.py
--rw-r--r--   0 ellek      (501) staff       (20)     3318 2023-01-10 06:50:18.000000 pied_poker-1.2.5/pied_poker/hand/poker_hand.py
--rw-r--r--   0 ellek      (501) staff       (20)     1953 2023-01-10 08:17:04.000000 pied_poker-1.2.5/pied_poker/hand/royal_flush.py
--rw-r--r--   0 ellek      (501) staff       (20)     2099 2023-01-10 07:31:59.000000 pied_poker-1.2.5/pied_poker/hand/straight.py
--rw-r--r--   0 ellek      (501) staff       (20)     2012 2023-01-10 08:11:25.000000 pied_poker-1.2.5/pied_poker/hand/straight_flush.py
--rw-r--r--   0 ellek      (501) staff       (20)     2853 2023-01-10 07:32:10.000000 pied_poker-1.2.5/pied_poker/hand/three_of_a_kind.py
--rw-r--r--   0 ellek      (501) staff       (20)     3493 2023-01-10 07:32:15.000000 pied_poker-1.2.5/pied_poker/hand/two_pair.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:49:18.534825 pied_poker-1.2.5/pied_poker/player/
--rw-r--r--   0 ellek      (501) staff       (20)       44 2022-03-21 04:52:37.000000 pied_poker-1.2.5/pied_poker/player/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)      840 2023-07-21 23:13:34.000000 pied_poker-1.2.5/pied_poker/player/player.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:49:18.536420 pied_poker-1.2.5/pied_poker/poker_round/
--rw-r--r--   0 ellek      (501) staff       (20)      297 2022-03-21 04:52:37.000000 pied_poker-1.2.5/pied_poker/poker_round/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)     3735 2022-03-21 04:52:37.000000 pied_poker-1.2.5/pied_poker/poker_round/poker_round.py
--rw-r--r--   0 ellek      (501) staff       (20)     4728 2023-08-21 05:02:53.000000 pied_poker-1.2.5/pied_poker/poker_round/poker_round_result.py
--rw-r--r--   0 ellek      (501) staff       (20)     6794 2022-03-21 04:52:37.000000 pied_poker-1.2.5/pied_poker/poker_round/poker_round_simulation_result.py
--rw-r--r--   0 ellek      (501) staff       (20)     4671 2023-01-11 02:01:55.000000 pied_poker-1.2.5/pied_poker/poker_round/poker_round_simulator.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:49:18.537325 pied_poker-1.2.5/pied_poker/probability/
--rw-r--r--   0 ellek      (501) staff       (20)      912 2024-04-26 23:47:42.000000 pied_poker-1.2.5/pied_poker/probability/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)     1053 2022-03-21 04:52:37.000000 pied_poker-1.2.5/pied_poker/probability/base_poker_event.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:49:18.541480 pied_poker-1.2.5/pied_poker/probability/events/
--rw-r--r--   0 ellek      (501) staff       (20)      980 2023-01-01 00:47:51.000000 pied_poker-1.2.5/pied_poker/probability/events/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)      861 2022-03-21 04:52:37.000000 pied_poker-1.2.5/pied_poker/probability/events/community_cards_include.py
--rw-r--r--   0 ellek      (501) staff       (20)      770 2022-03-21 04:52:37.000000 pied_poker-1.2.5/pied_poker/probability/events/no_tie.py
--rw-r--r--   0 ellek      (501) staff       (20)     1211 2022-03-21 04:52:37.000000 pied_poker-1.2.5/pied_poker/probability/events/player_has_card_ranks.py
--rw-r--r--   0 ellek      (501) staff       (20)     1211 2022-03-21 04:52:37.000000 pied_poker-1.2.5/pied_poker/probability/events/player_has_card_suits.py
--rw-r--r--   0 ellek      (501) staff       (20)     1181 2022-03-21 04:52:37.000000 pied_poker-1.2.5/pied_poker/probability/events/player_has_cards.py
--rw-r--r--   0 ellek      (501) staff       (20)     1611 2022-03-21 04:52:37.000000 pied_poker-1.2.5/pied_poker/probability/events/player_has_hand.py
--rw-r--r--   0 ellek      (501) staff       (20)     1224 2022-03-21 04:52:37.000000 pied_poker-1.2.5/pied_poker/probability/events/player_has_hand_or_higher.py
--rw-r--r--   0 ellek      (501) staff       (20)     2218 2022-03-21 04:52:37.000000 pied_poker-1.2.5/pied_poker/probability/events/player_has_pocket_pair.py
--rw-r--r--   0 ellek      (501) staff       (20)     1520 2022-03-21 04:52:37.000000 pied_poker-1.2.5/pied_poker/probability/events/player_has_suited_cards.py
--rw-r--r--   0 ellek      (501) staff       (20)      792 2022-03-21 04:52:37.000000 pied_poker-1.2.5/pied_poker/probability/events/player_loses.py
--rw-r--r--   0 ellek      (501) staff       (20)     1275 2022-03-21 04:52:37.000000 pied_poker-1.2.5/pied_poker/probability/events/player_wins.py
--rw-r--r--   0 ellek      (501) staff       (20)      959 2023-01-01 00:52:22.000000 pied_poker-1.2.5/pied_poker/probability/events/player_wins_with_tie.py
--rw-r--r--   0 ellek      (501) staff       (20)      767 2023-01-01 00:43:13.000000 pied_poker-1.2.5/pied_poker/probability/events/tie.py
--rw-r--r--   0 ellek      (501) staff       (20)     1184 2023-08-19 21:40:15.000000 pied_poker-1.2.5/pied_poker/probability/probability_value.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:49:18.542737 pied_poker-1.2.5/pied_poker/visualization/
--rw-r--r--   0 ellek      (501) staff       (20)      245 2023-12-23 23:33:26.000000 pied_poker-1.2.5/pied_poker/visualization/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)     8326 2023-12-28 22:01:51.000000 pied_poker-1.2.5/pied_poker/visualization/data_generator.py
--rw-r--r--   0 ellek      (501) staff       (20)     5061 2023-12-23 23:33:26.000000 pied_poker-1.2.5/pied_poker/visualization/pocket_pairs_vs_num_players.py
--rw-r--r--   0 ellek      (501) staff       (20)     6366 2023-12-23 23:33:26.000000 pied_poker-1.2.5/pied_poker/visualization/starting_card_probabilities.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:49:18.527047 pied_poker-1.2.5/pied_poker.egg-info/
--rw-r--r--   0 ellek      (501) staff       (20)      737 2024-04-26 23:49:18.000000 pied_poker-1.2.5/pied_poker.egg-info/PKG-INFO
--rw-r--r--   0 ellek      (501) staff       (20)     2161 2024-04-26 23:49:18.000000 pied_poker-1.2.5/pied_poker.egg-info/SOURCES.txt
--rw-r--r--   0 ellek      (501) staff       (20)        1 2024-04-26 23:49:18.000000 pied_poker-1.2.5/pied_poker.egg-info/dependency_links.txt
--rw-r--r--   0 ellek      (501) staff       (20)       44 2024-04-26 23:49:18.000000 pied_poker-1.2.5/pied_poker.egg-info/requires.txt
--rw-r--r--   0 ellek      (501) staff       (20)       11 2024-04-26 23:49:18.000000 pied_poker-1.2.5/pied_poker.egg-info/top_level.txt
--rw-r--r--   0 ellek      (501) staff       (20)       38 2024-04-26 23:49:18.543530 pied_poker-1.2.5/setup.cfg
--rw-r--r--   0 ellek      (501) staff       (20)     1266 2024-04-26 23:49:17.000000 pied_poker-1.2.5/setup.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:52:55.399167 pied_poker-1.2.6/
+-rw-r--r--   0 ellek      (501) staff       (20)      737 2024-04-26 23:52:55.398908 pied_poker-1.2.6/PKG-INFO
+-rw-r--r--   0 ellek      (501) staff       (20)    31804 2024-01-10 19:08:36.000000 pied_poker-1.2.6/README.md
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:52:55.381713 pied_poker-1.2.6/pied_poker/
+-rw-r--r--   0 ellek      (501) staff       (20)      217 2024-04-26 23:52:39.000000 pied_poker-1.2.6/pied_poker/__init__.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:52:55.384842 pied_poker-1.2.6/pied_poker/card/
+-rw-r--r--   0 ellek      (501) staff       (20)      164 2022-03-21 04:52:37.000000 pied_poker-1.2.6/pied_poker/card/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1791 2024-04-09 07:53:12.000000 pied_poker-1.2.6/pied_poker/card/card.py
+-rw-r--r--   0 ellek      (501) staff       (20)      379 2022-03-21 04:52:37.000000 pied_poker-1.2.6/pied_poker/card/comparable.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2157 2023-01-15 06:59:01.000000 pied_poker-1.2.6/pied_poker/card/rank.py
+-rw-r--r--   0 ellek      (501) staff       (20)      824 2023-01-08 20:45:48.000000 pied_poker-1.2.6/pied_poker/card/suit.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:52:55.385422 pied_poker-1.2.6/pied_poker/deck/
+-rw-r--r--   0 ellek      (501) staff       (20)       38 2022-03-21 04:52:37.000000 pied_poker-1.2.6/pied_poker/deck/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2450 2023-08-19 21:24:44.000000 pied_poker-1.2.6/pied_poker/deck/deck.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:52:55.390177 pied_poker-1.2.6/pied_poker/hand/
+-rw-r--r--   0 ellek      (501) staff       (20)      724 2023-08-21 04:17:06.000000 pied_poker-1.2.6/pied_poker/hand/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)    10894 2023-12-23 23:23:25.000000 pied_poker-1.2.6/pied_poker/hand/base_hand.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1061 2023-01-25 00:26:09.000000 pied_poker-1.2.6/pied_poker/hand/empty_hand.py
+-rw-r--r--   0 ellek      (501) staff       (20)     3215 2023-01-30 23:07:57.000000 pied_poker-1.2.6/pied_poker/hand/flush.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2567 2023-01-10 07:31:28.000000 pied_poker-1.2.6/pied_poker/hand/four_of_a_kind.py
+-rw-r--r--   0 ellek      (501) staff       (20)     3511 2023-06-08 21:06:49.000000 pied_poker-1.2.6/pied_poker/hand/full_house.py
+-rw-r--r--   0 ellek      (501) staff       (20)     3375 2023-06-08 21:28:48.000000 pied_poker-1.2.6/pied_poker/hand/high_card.py
+-rw-r--r--   0 ellek      (501) staff       (20)      853 2023-08-21 04:23:37.000000 pied_poker-1.2.6/pied_poker/hand/killer_card.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2913 2023-01-10 07:31:44.000000 pied_poker-1.2.6/pied_poker/hand/one_pair.py
+-rw-r--r--   0 ellek      (501) staff       (20)      858 2023-12-23 23:24:38.000000 pied_poker-1.2.6/pied_poker/hand/out.py
+-rw-r--r--   0 ellek      (501) staff       (20)     3318 2023-01-10 06:50:18.000000 pied_poker-1.2.6/pied_poker/hand/poker_hand.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1953 2023-01-10 08:17:04.000000 pied_poker-1.2.6/pied_poker/hand/royal_flush.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2099 2023-01-10 07:31:59.000000 pied_poker-1.2.6/pied_poker/hand/straight.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2012 2023-01-10 08:11:25.000000 pied_poker-1.2.6/pied_poker/hand/straight_flush.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2853 2023-01-10 07:32:10.000000 pied_poker-1.2.6/pied_poker/hand/three_of_a_kind.py
+-rw-r--r--   0 ellek      (501) staff       (20)     3493 2023-01-10 07:32:15.000000 pied_poker-1.2.6/pied_poker/hand/two_pair.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:52:55.390776 pied_poker-1.2.6/pied_poker/player/
+-rw-r--r--   0 ellek      (501) staff       (20)       44 2022-03-21 04:52:37.000000 pied_poker-1.2.6/pied_poker/player/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)      840 2023-07-21 23:13:34.000000 pied_poker-1.2.6/pied_poker/player/player.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:52:55.392307 pied_poker-1.2.6/pied_poker/poker_round/
+-rw-r--r--   0 ellek      (501) staff       (20)      297 2022-03-21 04:52:37.000000 pied_poker-1.2.6/pied_poker/poker_round/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)     3735 2022-03-21 04:52:37.000000 pied_poker-1.2.6/pied_poker/poker_round/poker_round.py
+-rw-r--r--   0 ellek      (501) staff       (20)     4728 2023-08-21 05:02:53.000000 pied_poker-1.2.6/pied_poker/poker_round/poker_round_result.py
+-rw-r--r--   0 ellek      (501) staff       (20)     6794 2022-03-21 04:52:37.000000 pied_poker-1.2.6/pied_poker/poker_round/poker_round_simulation_result.py
+-rw-r--r--   0 ellek      (501) staff       (20)     4671 2023-01-11 02:01:55.000000 pied_poker-1.2.6/pied_poker/poker_round/poker_round_simulator.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:52:55.393205 pied_poker-1.2.6/pied_poker/probability/
+-rw-r--r--   0 ellek      (501) staff       (20)      912 2024-04-26 23:47:42.000000 pied_poker-1.2.6/pied_poker/probability/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1053 2022-03-21 04:52:37.000000 pied_poker-1.2.6/pied_poker/probability/base_poker_event.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:52:55.397275 pied_poker-1.2.6/pied_poker/probability/events/
+-rw-r--r--   0 ellek      (501) staff       (20)      980 2023-01-01 00:47:51.000000 pied_poker-1.2.6/pied_poker/probability/events/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)      861 2022-03-21 04:52:37.000000 pied_poker-1.2.6/pied_poker/probability/events/community_cards_include.py
+-rw-r--r--   0 ellek      (501) staff       (20)      770 2022-03-21 04:52:37.000000 pied_poker-1.2.6/pied_poker/probability/events/no_tie.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1211 2022-03-21 04:52:37.000000 pied_poker-1.2.6/pied_poker/probability/events/player_has_card_ranks.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1211 2022-03-21 04:52:37.000000 pied_poker-1.2.6/pied_poker/probability/events/player_has_card_suits.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1181 2022-03-21 04:52:37.000000 pied_poker-1.2.6/pied_poker/probability/events/player_has_cards.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1611 2022-03-21 04:52:37.000000 pied_poker-1.2.6/pied_poker/probability/events/player_has_hand.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1224 2022-03-21 04:52:37.000000 pied_poker-1.2.6/pied_poker/probability/events/player_has_hand_or_higher.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2218 2022-03-21 04:52:37.000000 pied_poker-1.2.6/pied_poker/probability/events/player_has_pocket_pair.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1520 2022-03-21 04:52:37.000000 pied_poker-1.2.6/pied_poker/probability/events/player_has_suited_cards.py
+-rw-r--r--   0 ellek      (501) staff       (20)      792 2022-03-21 04:52:37.000000 pied_poker-1.2.6/pied_poker/probability/events/player_loses.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1275 2022-03-21 04:52:37.000000 pied_poker-1.2.6/pied_poker/probability/events/player_wins.py
+-rw-r--r--   0 ellek      (501) staff       (20)      959 2023-01-01 00:52:22.000000 pied_poker-1.2.6/pied_poker/probability/events/player_wins_with_tie.py
+-rw-r--r--   0 ellek      (501) staff       (20)      767 2023-01-01 00:43:13.000000 pied_poker-1.2.6/pied_poker/probability/events/tie.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1184 2023-08-19 21:40:15.000000 pied_poker-1.2.6/pied_poker/probability/probability_value.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:52:55.398502 pied_poker-1.2.6/pied_poker/visualization/
+-rw-r--r--   0 ellek      (501) staff       (20)      245 2023-12-23 23:33:26.000000 pied_poker-1.2.6/pied_poker/visualization/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)     8326 2023-12-28 22:01:51.000000 pied_poker-1.2.6/pied_poker/visualization/data_generator.py
+-rw-r--r--   0 ellek      (501) staff       (20)     5061 2023-12-23 23:33:26.000000 pied_poker-1.2.6/pied_poker/visualization/pocket_pairs_vs_num_players.py
+-rw-r--r--   0 ellek      (501) staff       (20)     6366 2023-12-23 23:33:26.000000 pied_poker-1.2.6/pied_poker/visualization/starting_card_probabilities.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-26 23:52:55.383075 pied_poker-1.2.6/pied_poker.egg-info/
+-rw-r--r--   0 ellek      (501) staff       (20)      737 2024-04-26 23:52:55.000000 pied_poker-1.2.6/pied_poker.egg-info/PKG-INFO
+-rw-r--r--   0 ellek      (501) staff       (20)     2161 2024-04-26 23:52:55.000000 pied_poker-1.2.6/pied_poker.egg-info/SOURCES.txt
+-rw-r--r--   0 ellek      (501) staff       (20)        1 2024-04-26 23:52:55.000000 pied_poker-1.2.6/pied_poker.egg-info/dependency_links.txt
+-rw-r--r--   0 ellek      (501) staff       (20)       44 2024-04-26 23:52:55.000000 pied_poker-1.2.6/pied_poker.egg-info/requires.txt
+-rw-r--r--   0 ellek      (501) staff       (20)       11 2024-04-26 23:52:55.000000 pied_poker-1.2.6/pied_poker.egg-info/top_level.txt
+-rw-r--r--   0 ellek      (501) staff       (20)       38 2024-04-26 23:52:55.399276 pied_poker-1.2.6/setup.cfg
+-rw-r--r--   0 ellek      (501) staff       (20)     1266 2024-04-26 23:52:52.000000 pied_poker-1.2.6/setup.py
```

### Comparing `pied_poker-1.2.5/PKG-INFO` & `pied_poker-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pied_poker
-Version: 1.2.5
+Version: 1.2.6
 Summary: A Python package to run flexible and fast poker simulations using a monte carlo style simulator.
 Home-page: https://github.com/elleklinton/PiedPoker
 Author: Ellek Linton
 Author-email: ellek@elleklinton.com
 License: GNU LGPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pied_poker-1.2.5/README.md` & `pied_poker-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/card/card.py` & `pied_poker-1.2.6/pied_poker/card/card.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/card/rank.py` & `pied_poker-1.2.6/pied_poker/card/rank.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/card/suit.py` & `pied_poker-1.2.6/pied_poker/card/suit.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/deck/deck.py` & `pied_poker-1.2.6/pied_poker/deck/deck.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/hand/__init__.py` & `pied_poker-1.2.6/pied_poker/hand/__init__.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/hand/base_hand.py` & `pied_poker-1.2.6/pied_poker/hand/base_hand.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/hand/empty_hand.py` & `pied_poker-1.2.6/pied_poker/hand/empty_hand.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/hand/flush.py` & `pied_poker-1.2.6/pied_poker/hand/flush.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/hand/four_of_a_kind.py` & `pied_poker-1.2.6/pied_poker/hand/four_of_a_kind.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/hand/full_house.py` & `pied_poker-1.2.6/pied_poker/hand/full_house.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/hand/high_card.py` & `pied_poker-1.2.6/pied_poker/hand/high_card.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/hand/killer_card.py` & `pied_poker-1.2.6/pied_poker/hand/killer_card.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/hand/one_pair.py` & `pied_poker-1.2.6/pied_poker/hand/one_pair.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/hand/out.py` & `pied_poker-1.2.6/pied_poker/hand/out.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/hand/poker_hand.py` & `pied_poker-1.2.6/pied_poker/hand/poker_hand.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/hand/royal_flush.py` & `pied_poker-1.2.6/pied_poker/hand/royal_flush.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/hand/straight.py` & `pied_poker-1.2.6/pied_poker/hand/straight.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/hand/straight_flush.py` & `pied_poker-1.2.6/pied_poker/hand/straight_flush.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/hand/three_of_a_kind.py` & `pied_poker-1.2.6/pied_poker/hand/three_of_a_kind.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/hand/two_pair.py` & `pied_poker-1.2.6/pied_poker/hand/two_pair.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/player/player.py` & `pied_poker-1.2.6/pied_poker/player/player.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/poker_round/poker_round.py` & `pied_poker-1.2.6/pied_poker/poker_round/poker_round.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/poker_round/poker_round_result.py` & `pied_poker-1.2.6/pied_poker/poker_round/poker_round_result.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/poker_round/poker_round_simulation_result.py` & `pied_poker-1.2.6/pied_poker/poker_round/poker_round_simulation_result.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/poker_round/poker_round_simulator.py` & `pied_poker-1.2.6/pied_poker/poker_round/poker_round_simulator.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/probability/__init__.py` & `pied_poker-1.2.6/pied_poker/probability/__init__.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/probability/base_poker_event.py` & `pied_poker-1.2.6/pied_poker/probability/base_poker_event.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/probability/events/__init__.py` & `pied_poker-1.2.6/pied_poker/probability/events/__init__.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/probability/events/community_cards_include.py` & `pied_poker-1.2.6/pied_poker/probability/events/community_cards_include.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/probability/events/no_tie.py` & `pied_poker-1.2.6/pied_poker/probability/events/no_tie.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/probability/events/player_has_card_ranks.py` & `pied_poker-1.2.6/pied_poker/probability/events/player_has_card_ranks.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/probability/events/player_has_card_suits.py` & `pied_poker-1.2.6/pied_poker/probability/events/player_has_card_suits.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/probability/events/player_has_cards.py` & `pied_poker-1.2.6/pied_poker/probability/events/player_has_cards.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/probability/events/player_has_hand.py` & `pied_poker-1.2.6/pied_poker/probability/events/player_has_hand.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/probability/events/player_has_hand_or_higher.py` & `pied_poker-1.2.6/pied_poker/probability/events/player_has_hand_or_higher.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/probability/events/player_has_pocket_pair.py` & `pied_poker-1.2.6/pied_poker/probability/events/player_has_pocket_pair.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/probability/events/player_has_suited_cards.py` & `pied_poker-1.2.6/pied_poker/probability/events/player_has_suited_cards.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/probability/events/player_loses.py` & `pied_poker-1.2.6/pied_poker/probability/events/player_loses.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/probability/events/player_wins.py` & `pied_poker-1.2.6/pied_poker/probability/events/player_wins.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/probability/events/player_wins_with_tie.py` & `pied_poker-1.2.6/pied_poker/probability/events/player_wins_with_tie.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/probability/events/tie.py` & `pied_poker-1.2.6/pied_poker/probability/events/tie.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/probability/probability_value.py` & `pied_poker-1.2.6/pied_poker/probability/probability_value.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/visualization/data_generator.py` & `pied_poker-1.2.6/pied_poker/visualization/data_generator.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/visualization/pocket_pairs_vs_num_players.py` & `pied_poker-1.2.6/pied_poker/visualization/pocket_pairs_vs_num_players.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker/visualization/starting_card_probabilities.py` & `pied_poker-1.2.6/pied_poker/visualization/starting_card_probabilities.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/pied_poker.egg-info/PKG-INFO` & `pied_poker-1.2.6/pied_poker.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pied-poker
-Version: 1.2.5
+Version: 1.2.6
 Summary: A Python package to run flexible and fast poker simulations using a monte carlo style simulator.
 Home-page: https://github.com/elleklinton/PiedPoker
 Author: Ellek Linton
 Author-email: ellek@elleklinton.com
 License: GNU LGPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pied_poker-1.2.5/pied_poker.egg-info/SOURCES.txt` & `pied_poker-1.2.6/pied_poker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pied_poker-1.2.5/setup.py` & `pied_poker-1.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name='pied_poker',
-    version='1.2.5',
+    version='1.2.6',
     description='A Python package to run flexible and fast poker simulations using a monte carlo style simulator.',
     long_description='A Python package to run flexible and fast poker simulations using a monte carlo style simulator.',
     url='https://github.com/elleklinton/PiedPoker',
     author='Ellek Linton',
     author_email='ellek@elleklinton.com',
     license='GNU LGPLv3',
     packages=['pied_poker',
```
