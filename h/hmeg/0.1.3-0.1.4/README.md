# Comparing `tmp/hmeg-0.1.3.tar.gz` & `tmp/hmeg-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmeg-0.1.3.tar", max compression
+gzip compressed data, was "hmeg-0.1.4.tar", max compression
```

## Comparing `hmeg-0.1.3.tar` & `hmeg-0.1.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     1066 2024-03-01 07:41:02.775209 hmeg-0.1.3/LICENSE
--rw-r--r--   0        0        0     4437 2024-04-06 02:58:35.143708 hmeg-0.1.3/README.md
--rw-r--r--   0        0        0      137 2024-03-31 04:16:50.659172 hmeg-0.1.3/hmeg/__init__.py
--rw-r--r--   0        0        0     2782 2024-04-17 14:36:24.427936 hmeg-0.1.3/hmeg/entities.py
--rw-r--r--   0        0        0     1652 2024-04-17 14:36:24.427936 hmeg-0.1.3/hmeg/exercise_generator.py
--rw-r--r--   0        0        0     1500 2024-03-30 08:41:48.508255 hmeg-0.1.3/hmeg/miniphrase/ab.toml
--rw-r--r--   0        0        0     1782 2024-03-30 08:41:48.508255 hmeg-0.1.3/hmeg/miniphrase/cd.toml
--rw-r--r--   0        0        0     1897 2024-03-30 08:41:48.508255 hmeg-0.1.3/hmeg/miniphrase/efg.toml
--rw-r--r--   0        0        0     1384 2024-03-30 08:41:48.508255 hmeg-0.1.3/hmeg/miniphrase/h.toml
--rw-r--r--   0        0        0     1631 2024-03-30 08:41:48.508255 hmeg-0.1.3/hmeg/miniphrase/ikl.toml
--rw-r--r--   0        0        0     1809 2024-03-30 08:41:48.508255 hmeg-0.1.3/hmeg/miniphrase/mn.toml
--rw-r--r--   0        0        0     1216 2024-03-30 08:41:48.508255 hmeg-0.1.3/hmeg/miniphrase/opr.toml
--rw-r--r--   0        0        0     3075 2024-03-30 08:41:48.508255 hmeg-0.1.3/hmeg/miniphrase/stu.toml
--rw-r--r--   0        0        0     2146 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/miniphrase/wy.toml
--rw-r--r--   0        0        0     2327 2024-04-17 14:36:24.427936 hmeg-0.1.3/hmeg/registry.py
--rw-r--r--   0        0        0      290 2024-03-10 07:44:10.147484 hmeg-0.1.3/hmeg/topics/1_basic_present_tense.toml
--rw-r--r--   0        0        0      296 2024-03-10 07:44:10.147484 hmeg-0.1.3/hmeg/topics/1_from_a_to_b_from_c_until_d.toml
--rw-r--r--   0        0        0      325 2024-03-24 12:49:15.051567 hmeg-0.1.3/hmeg/topics/1_have_dont_have_there_is_there_isnt.toml
--rw-r--r--   0        0        0      290 2024-03-10 07:44:10.147484 hmeg-0.1.3/hmeg/topics/1_i_want_to.toml
--rw-r--r--   0        0        0      415 2024-03-10 07:44:10.147484 hmeg-0.1.3/hmeg/topics/1_negative_sentenses.toml
--rw-r--r--   0        0        0      233 2024-03-10 07:44:10.151485 hmeg-0.1.3/hmeg/topics/1_past_tense.toml
--rw-r--r--   0        0        0      161 2024-03-10 07:44:10.151485 hmeg-0.1.3/hmeg/topics/1_please_give_me.toml
--rw-r--r--   0        0        0      224 2024-03-24 12:49:15.051567 hmeg-0.1.3/hmeg/topics/1_this_is.toml
--rw-r--r--   0        0        0      165 2024-03-10 07:44:10.151485 hmeg-0.1.3/hmeg/topics/1_topic_subject_particle.toml
--rw-r--r--   0        0        0      327 2024-03-10 07:44:10.151485 hmeg-0.1.3/hmeg/topics/1_what_do_you_want_to_do.toml
--rw-r--r--   0        0        0      230 2024-03-14 13:30:47.048412 hmeg-0.1.3/hmeg/topics/2_and_and_then_therefore_so.toml
--rw-r--r--   0        0        0      154 2024-03-14 13:33:59.925728 hmeg-0.1.3/hmeg/topics/2_and_with.toml
--rw-r--r--   0        0        0      288 2024-03-14 13:39:48.992097 hmeg-0.1.3/hmeg/topics/2_but_however.toml
--rw-r--r--   0        0        0      250 2024-03-14 13:49:14.375934 hmeg-0.1.3/hmeg/topics/2_can_cannot.toml
--rw-r--r--   0        0        0      152 2024-03-15 14:01:09.329766 hmeg-0.1.3/hmeg/topics/2_dont_do_it.toml
--rw-r--r--   0        0        0      242 2024-03-14 13:27:05.334892 hmeg-0.1.3/hmeg/topics/2_future_tense.toml
--rw-r--r--   0        0        0      281 2024-03-21 21:46:08.368116 hmeg-0.1.3/hmeg/topics/2_have_to_should_must.toml
--rw-r--r--   0        0        0      185 2024-03-15 13:48:12.447505 hmeg-0.1.3/hmeg/topics/2_if_in_case.toml
--rw-r--r--   0        0        0      138 2024-03-15 13:50:12.715855 hmeg-0.1.3/hmeg/topics/2_imperative.toml
--rw-r--r--   0        0        0      183 2024-03-15 13:59:28.597472 hmeg-0.1.3/hmeg/topics/2_particles_for_method_way.toml
--rw-r--r--   0        0        0      173 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/2_please_do_it_for_me.toml
--rw-r--r--   0        0        0      251 2024-03-14 13:46:29.870818 hmeg-0.1.3/hmeg/topics/2_present_progressive.toml
--rw-r--r--   0        0        0      294 2024-03-14 13:51:21.940821 hmeg-0.1.3/hmeg/topics/2_to_be_good_poor_at.toml
--rw-r--r--   0        0        0      288 2024-03-14 13:56:35.319010 hmeg-0.1.3/hmeg/topics/2_to_like.toml
--rw-r--r--   0        0        0      152 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_after_ing.toml
--rw-r--r--   0        0        0      209 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_approximately_about.toml
--rw-r--r--   0        0        0      156 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_before_ing.toml
--rw-r--r--   0        0        0      167 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_but_still_nevertheless.toml
--rw-r--r--   0        0        0      166 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_even_if_even_though.toml
--rw-r--r--   0        0        0      284 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_in_front_of_behind.toml
--rw-r--r--   0        0        0      215 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_in_order_to_for_the_sake_of.toml
--rw-r--r--   0        0        0      204 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_linking_verbs_고.toml
--rw-r--r--   0        0        0      165 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_linking_verbs_여서.toml
--rw-r--r--   0        0        0      256 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_linking_words_는데.toml
--rw-r--r--   0        0        0      339 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_maybe_i_might.toml
--rw-r--r--   0        0        0      289 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_nothing_but_only.toml
--rw-r--r--   0        0        0      241 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_shall_we_i_wonder.toml
--rw-r--r--   0        0        0      198 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_to_look_like_seem_like.toml
--rw-r--r--   0        0        0      166 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_too_much_very.toml
--rw-r--r--   0        0        0      159 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_verb_ending_네요.toml
--rw-r--r--   0        0        0      371 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/3_well_then_in_that_case.toml
--rw-r--r--   0        0        0      284 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/4_among_between.toml
--rw-r--r--   0        0        0      168 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/4_do_you_want_to.toml
--rw-r--r--   0        0        0      511 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/4_i_think_past_future.toml
--rw-r--r--   0        0        0      293 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/4_it_cant_be.toml
--rw-r--r--   0        0        0      439 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/4_it_is_ok_to.toml
--rw-r--r--   0        0        0      281 2024-04-06 02:58:35.143708 hmeg-0.1.3/hmeg/topics/4_less_not_completely.toml
--rw-r--r--   0        0        0      314 2024-04-06 02:58:35.147708 hmeg-0.1.3/hmeg/topics/4_most_best.toml
--rw-r--r--   0        0        0      190 2024-04-06 02:58:35.147708 hmeg-0.1.3/hmeg/topics/4_much_more_much_less.toml
--rw-r--r--   0        0        0      343 2024-04-06 02:58:35.147708 hmeg-0.1.3/hmeg/topics/4_the_more_the_more.toml
--rw-r--r--   0        0        0      224 2024-04-06 02:58:35.147708 hmeg-0.1.3/hmeg/topics/4_to_become_adj.toml
--rw-r--r--   0        0        0      371 2024-04-06 02:58:35.147708 hmeg-0.1.3/hmeg/topics/4_to_gradually_get_to_do.toml
--rw-r--r--   0        0        0      339 2024-04-06 02:58:35.147708 hmeg-0.1.3/hmeg/topics/4_to_try_doing_something.toml
--rw-r--r--   0        0        0      247 2024-04-06 02:58:35.147708 hmeg-0.1.3/hmeg/topics/4_verb_ending_지_죠.toml
--rw-r--r--   0        0        0      413 2024-04-06 02:58:35.147708 hmeg-0.1.3/hmeg/topics/4_you_should_not.toml
--rw-r--r--   0        0        0      354 2024-03-10 07:43:30.163214 hmeg-0.1.3/hmeg/topics/9_while.toml
--rw-r--r--   0        0        0     5504 2024-04-17 14:36:24.427936 hmeg-0.1.3/hmeg/usecases.py
--rw-r--r--   0        0        0     2673 2024-04-17 14:36:24.427936 hmeg-0.1.3/hmeg/vocabs/minilex.toml
--rw-r--r--   0        0        0     1037 2024-04-17 14:36:24.427936 hmeg-0.1.3/hmeg/vocabs/nanolex.toml
--rw-r--r--   0        0        0     5598 2024-04-17 14:36:24.427936 hmeg-0.1.3/hmeg/vocabulary.py
--rw-r--r--   0        0        0      500 2024-04-17 14:36:28.371952 hmeg-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5286 1970-01-01 00:00:00.000000 hmeg-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-01 07:41:02.775209 hmeg-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4437 2024-04-06 02:58:35.143708 hmeg-0.1.4/README.md
+-rw-r--r--   0        0        0      137 2024-03-31 04:16:50.659172 hmeg-0.1.4/hmeg/__init__.py
+-rw-r--r--   0        0        0     2782 2024-04-17 14:37:13.372136 hmeg-0.1.4/hmeg/entities.py
+-rw-r--r--   0        0        0     1652 2024-04-17 14:37:13.372136 hmeg-0.1.4/hmeg/exercise_generator.py
+-rw-r--r--   0        0        0     1500 2024-03-30 08:41:48.508255 hmeg-0.1.4/hmeg/miniphrase/ab.toml
+-rw-r--r--   0        0        0     1782 2024-03-30 08:41:48.508255 hmeg-0.1.4/hmeg/miniphrase/cd.toml
+-rw-r--r--   0        0        0     1897 2024-03-30 08:41:48.508255 hmeg-0.1.4/hmeg/miniphrase/efg.toml
+-rw-r--r--   0        0        0     1384 2024-03-30 08:41:48.508255 hmeg-0.1.4/hmeg/miniphrase/h.toml
+-rw-r--r--   0        0        0     1631 2024-03-30 08:41:48.508255 hmeg-0.1.4/hmeg/miniphrase/ikl.toml
+-rw-r--r--   0        0        0     1809 2024-03-30 08:41:48.508255 hmeg-0.1.4/hmeg/miniphrase/mn.toml
+-rw-r--r--   0        0        0     1216 2024-03-30 08:41:48.508255 hmeg-0.1.4/hmeg/miniphrase/opr.toml
+-rw-r--r--   0        0        0     3075 2024-03-30 08:41:48.508255 hmeg-0.1.4/hmeg/miniphrase/stu.toml
+-rw-r--r--   0        0        0     2146 2024-04-06 02:58:35.143708 hmeg-0.1.4/hmeg/miniphrase/wy.toml
+-rw-r--r--   0        0        0     2327 2024-04-17 14:37:13.372136 hmeg-0.1.4/hmeg/registry.py
+-rw-r--r--   0        0        0      423 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/1_basic_present_tense.toml
+-rw-r--r--   0        0        0      793 2024-04-24 14:03:25.414198 hmeg-0.1.4/hmeg/topics/1_from_a_to_b_from_c_until_d.toml
+-rw-r--r--   0        0        0      370 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/1_have_dont_have_there_is_there_isnt.toml
+-rw-r--r--   0        0        0      419 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/1_i_want_to.toml
+-rw-r--r--   0        0        0      550 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/1_negative_sentenses.toml
+-rw-r--r--   0        0        0      366 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/1_past_tense.toml
+-rw-r--r--   0        0        0      323 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/1_please_give_me.toml
+-rw-r--r--   0        0        0      356 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/1_this_is.toml
+-rw-r--r--   0        0        0      388 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/1_topic_subject_particle.toml
+-rw-r--r--   0        0        0      456 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/1_what_do_you_want_to_do.toml
+-rw-r--r--   0        0        0      392 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/2_and_and_then_therefore_so.toml
+-rw-r--r--   0        0        0      566 2024-04-24 14:08:53.431398 hmeg-0.1.4/hmeg/topics/2_and_with.toml
+-rw-r--r--   0        0        0      600 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/2_but_however.toml
+-rw-r--r--   0        0        0      412 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/2_can_cannot.toml
+-rw-r--r--   0        0        0      364 2024-04-24 14:15:05.256760 hmeg-0.1.4/hmeg/topics/2_dont_do_it.toml
+-rw-r--r--   0        0        0      375 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/2_future_tense.toml
+-rw-r--r--   0        0        0      443 2024-04-24 13:48:02.146818 hmeg-0.1.4/hmeg/topics/2_have_to_should_must.toml
+-rw-r--r--   0        0        0      347 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/2_if_in_case.toml
+-rw-r--r--   0        0        0      300 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/2_imperative.toml
+-rw-r--r--   0        0        0      310 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/2_particles_for_method_way.toml
+-rw-r--r--   0        0        0      389 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/2_please_do_it_for_me.toml
+-rw-r--r--   0        0        0      380 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/2_present_progressive.toml
+-rw-r--r--   0        0        0      419 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/2_to_be_good_poor_at.toml
+-rw-r--r--   0        0        0      420 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/2_to_like.toml
+-rw-r--r--   0        0        0      396 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_after_ing.toml
+-rw-r--r--   0        0        0      612 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_approximately_about.toml
+-rw-r--r--   0        0        0      442 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_before_ing.toml
+-rw-r--r--   0        0        0      330 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_but_still_nevertheless.toml
+-rw-r--r--   0        0        0      400 2024-04-27 08:55:56.656265 hmeg-0.1.4/hmeg/topics/3_even_if_even_though.toml
+-rw-r--r--   0        0        0      417 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_in_front_of_behind.toml
+-rw-r--r--   0        0        0      529 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_in_order_to_for_the_sake_of.toml
+-rw-r--r--   0        0        0      332 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_linking_verbs_고.toml
+-rw-r--r--   0        0        0      294 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_linking_verbs_여서.toml
+-rw-r--r--   0        0        0      411 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_linking_words_는데.toml
+-rw-r--r--   0        0        0      556 2024-04-24 14:11:33.291983 hmeg-0.1.4/hmeg/topics/3_maybe_i_might.toml
+-rw-r--r--   0        0        0      438 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_nothing_but_only.toml
+-rw-r--r--   0        0        0      468 2024-04-27 08:55:56.656265 hmeg-0.1.4/hmeg/topics/3_shall_we_i_wonder.toml
+-rw-r--r--   0        0        0      360 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_to_look_like_seem_like.toml
+-rw-r--r--   0        0        0      293 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_too_much_very.toml
+-rw-r--r--   0        0        0      314 2024-04-24 13:48:02.150818 hmeg-0.1.4/hmeg/topics/3_verb_ending_네요.toml
+-rw-r--r--   0        0        0      670 2024-04-24 14:18:15.221455 hmeg-0.1.4/hmeg/topics/3_well_then_in_that_case.toml
+-rw-r--r--   0        0        0      446 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_among_between.toml
+-rw-r--r--   0        0        0      330 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_do_you_want_to.toml
+-rw-r--r--   0        0        0      673 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_i_think_past_future.toml
+-rw-r--r--   0        0        0      418 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_it_cant_be.toml
+-rw-r--r--   0        0        0      668 2024-04-27 08:55:56.656265 hmeg-0.1.4/hmeg/topics/4_it_is_ok_to.toml
+-rw-r--r--   0        0        0      413 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_less_not_completely.toml
+-rw-r--r--   0        0        0      445 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_most_best.toml
+-rw-r--r--   0        0        0      352 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_much_more_much_less.toml
+-rw-r--r--   0        0        0      468 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_the_more_the_more.toml
+-rw-r--r--   0        0        0      351 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_to_become_adj.toml
+-rw-r--r--   0        0        0      527 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_to_gradually_get_to_do.toml
+-rw-r--r--   0        0        0      608 2024-04-24 14:07:24.823074 hmeg-0.1.4/hmeg/topics/4_to_try_doing_something.toml
+-rw-r--r--   0        0        0      403 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_verb_ending_지_죠.toml
+-rw-r--r--   0        0        0      568 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/4_you_should_not.toml
+-rw-r--r--   0        0        0      510 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/topics/9_while.toml
+-rw-r--r--   0        0        0     5902 2024-04-27 08:55:56.656265 hmeg-0.1.4/hmeg/usecases.py
+-rw-r--r--   0        0        0     2654 2024-04-24 13:53:05.935930 hmeg-0.1.4/hmeg/vocabs/minilex.toml
+-rw-r--r--   0        0        0      989 2024-04-24 13:48:02.154818 hmeg-0.1.4/hmeg/vocabs/nanolex.toml
+-rw-r--r--   0        0        0     5598 2024-04-17 14:37:13.372136 hmeg-0.1.4/hmeg/vocabulary.py
+-rw-r--r--   0        0        0      500 2024-04-27 08:56:20.804362 hmeg-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5286 1970-01-01 00:00:00.000000 hmeg-0.1.4/PKG-INFO
```

### Comparing `hmeg-0.1.3/LICENSE` & `hmeg-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.3/README.md` & `hmeg-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.3/hmeg/entities.py` & `hmeg-0.1.4/hmeg/entities.py`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.3/hmeg/exercise_generator.py` & `hmeg-0.1.4/hmeg/exercise_generator.py`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.3/hmeg/miniphrase/ab.toml` & `hmeg-0.1.4/hmeg/miniphrase/ab.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.3/hmeg/miniphrase/cd.toml` & `hmeg-0.1.4/hmeg/miniphrase/cd.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.3/hmeg/miniphrase/efg.toml` & `hmeg-0.1.4/hmeg/miniphrase/efg.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.3/hmeg/miniphrase/h.toml` & `hmeg-0.1.4/hmeg/miniphrase/h.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.3/hmeg/miniphrase/ikl.toml` & `hmeg-0.1.4/hmeg/miniphrase/ikl.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.3/hmeg/miniphrase/mn.toml` & `hmeg-0.1.4/hmeg/miniphrase/mn.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.3/hmeg/miniphrase/opr.toml` & `hmeg-0.1.4/hmeg/miniphrase/opr.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.3/hmeg/miniphrase/stu.toml` & `hmeg-0.1.4/hmeg/miniphrase/stu.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.3/hmeg/miniphrase/wy.toml` & `hmeg-0.1.4/hmeg/miniphrase/wy.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.3/hmeg/registry.py` & `hmeg-0.1.4/hmeg/registry.py`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.3/hmeg/usecases.py` & `hmeg-0.1.4/hmeg/usecases.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,27 @@
             continue
         with open(os.path.join(grammar_dir, file), "r") as f:
             grammar_descr_dict = toml.loads(f.read())
             grammar_descr = GrammarDescription.from_dict(grammar_descr_dict)
             GrammarRegistry.register_grammar_topic(grammar_descr)
 
 
+def get_vocabulary_names() -> list[str]:
+    """
+    Returns list with names of the built-in vocabularies.
+    """
+    vocabs_dir = os.path.join(os.path.dirname(__file__), "vocabs")
+    res = []
+    for file in os.listdir(vocabs_dir):
+        with open(os.path.join(vocabs_dir, file), "r") as f:
+            vocab_info = toml.loads(f.read())
+        res.append(vocab_info["name"])
+    return res
+
+
 def apply_vocabulary(s: str, vocab: Vocabulary) -> str:
     """
     Takes input string and replaces placeholders with respective minilex entities.
     """
 
     vocab_function = {
         VocabularyPlaceholders.Verb: vocab.random_verb,
```

### Comparing `hmeg-0.1.3/hmeg/vocabs/minilex.toml` & `hmeg-0.1.4/hmeg/vocabs/minilex.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 import = "nanolex.toml"
 name = "Minilex"
-nouns = [ "accident", "anybody", "anything", "apartment", "bag", "beginning", "bottom", "boy", "bread", "brother", "child", "clothes", "cold", "colour", "cry", "damage", "daughter", "earth", "evening", "everybody", "everything", "eye", "fall", "father", "flat", "foot", "front", "fun", "girl", "ground", "half", "hand", "head", "hope", "hour", "husband", "joke", "journey", "lady", "laugh", "lie", "light", "mistake", "moment", "month", "morning", "mother", "mouth", "newspaper", "night", "nobody", "nothing", "pain", "pen", "pencil", "picture", "reason", "relative", "sister", "sleep", "somebody", "son", "sound", "stand", "stop", "suitcase", "sun", "surprise", "talk", "teacher", "thing", "ticket", "tomorrow", "town", "true", "voice", "walk", "watch", "weather", "wife", "woman", "word", "worry", "yesterday",]
-adverbs = [ "angrily", "badly", "beautifully", "boringly", "calmly", "certainly", "cheaply", "cheerfully", "cleanly", "clearly", "coldly", "commonly", "dangerously", "deadly", "dearly", "differently", "difficultly", "dirtily", "dryly", "easily", "expensively", "famously", "fastly", "firstly", "freely", "fully", "funnily", "gladly", "greatly", "happily", "heavily", "highly", "hotly", "importantly", "impossibly", "interestingly", "kindly", "lastly", "lately", "lightly", "nearly", "necessarily", "newly", "nicely", "openly", "possibly", "prettily", "quietly", "relatively", "rightly", "safely", "shortly", "slowly", "sorrily", "strangely", "strongly", "stupidly", "surprisingly", "terribly", "tiredly", "urgently", "usually", "warmly", "wonderfully", "wrongly",]
+nouns = [ "accident", "anybody", "anything", "apartment", "bag", "beginning", "bottom", "boy", "bread", "brother", "child", "clothes", "cold", "colour", "cry", "damage", "daughter", "earth", "evening", "everybody", "everything", "eye", "fall", "father", "flat", "foot", "front", "fun", "girl", "ground", "half", "hand", "head", "hope", "hour", "husband", "joke", "journey", "lady", "laugh", "lie", "light", "mistake", "moment", "month", "morning", "mother", "mouth", "newspaper", "night", "nobody", "nothing", "pain", "pen", "pencil", "picture", "reason", "relative", "sister", "sleep", "somebody", "son", "sound", "stand", "stop", "suitcase", "sun", "surprise", "talk", "teacher", "thing", "ticket", "tomorrow", "town", "true", "voice", "walk", "weather", "wife", "woman", "word", "worry", "yesterday",]
+adverbs = [ "angrily", "badly", "beautifully", "boringly", "calmly", "certainly", "cheaply", "cheerfully", "cleanly", "clearly", "coldly", "commonly", "dangerously", "deadly", "dearly", "differently", "difficultly", "dirtily", "dryly", "easily", "expensively", "famously", "fast", "firstly", "freely", "fully", "funnily", "gladly", "greatly", "happily", "heavily", "highly", "hotly", "importantly", "impossibly", "interestingly", "kindly", "lastly", "lately", "lightly", "nearly", "necessarily", "newly", "nicely", "openly", "possibly", "prettily", "quietly", "relatively", "rightly", "safely", "shortly", "slowly", "sorrily", "strangely", "strongly", "stupidly", "surprisingly", "terribly", "tiredly", "urgently", "usually", "warmly", "wonderfully", "wrongly",]
 adjectives = [ "angry", "bad", "beautiful", "boring", "calm", "certain", "cheap", "cheerful", "clean", "clear", "cold", "common", "dangerous", "dead", "dear", "difficult", "dirty", "dry", "easy", "expensive", "famous", "fast", "finished", "fun", "funny", "glad", "happy", "heavy", "ill", "impossible", "interesting", "kind", "late", "light", "mean", "near", "necessary", "nice", "possible", "pretty", "quiet", "relative", "safe", "several", "short", "shut", "slow", "sorry", "strange", "strong", "stupid", "surprised", "tall", "terrible", "tired", "urgent", "usual", "warm", "whole", "wonderful", "worst", "wrong",]
-verbs = [ "arrive", "ask", "become", "begin", "believe", "borrow", "bring", "clean", "continue", "cry", "damage", "drop", "eat", "fall", "feel", "finish", "forget", "head", "hold", "hope", "hurt", "joke", "keep", "laugh", "leave", "lend", "lie", "listen", "look for", "mean", "meet", "pay", "put", "remember", "shut", "sing", "speak", "stand", "stay", "stop", "suggest", "talk", "teach", "understand", "wait", "walk", "worry", "write",]
+verbs = [ "arrive", "ask", "become", "begin", "believe", "borrow", "bring", "clean", "continue", "cry", "damage", "drop", "eat", "fall", "feel", "finish", "forget", "hold", "hope", "hurt", "joke", "keep", "laugh", "leave", "lend", "lie", "listen", "look for", "mean", "meet", "pay", "put", "remember", "shut", "sing", "speak", "stand", "stay", "stop", "suggest", "talk", "teach", "understand", "wait", "walk", "worry", "write",]
```

### Comparing `hmeg-0.1.3/hmeg/vocabs/nanolex.toml` & `hmeg-0.1.4/hmeg/vocabs/nanolex.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,5 +1,5 @@
 name = "Nanolex"
-nouns = [ "address", "air", "book", "buy", "change", "country", "day", "family", "food", "friend", "help", "home", "house", "key", "language", "left", "life", "love", "man", "money", "name", "need", "news", "now", "other", "page", "paper", "part", "people", "person", "place", "question", "right", "road", "room", "school", "shop", "show", "side", "something", "street", "tax", "time", "today", "top", "travel", "use", "water", "way", "week", "will", "work", "world", "year",]
+nouns = [ "address", "air", "book", "buy", "change", "country", "day", "family", "food", "friend", "help", "home", "house", "key", "language", "life", "love", "man", "money", "name", "need", "news", "now", "other", "page", "paper", "part", "people", "person", "place", "question", "road", "room", "school", "shop", "side", "something", "street", "tax", "time", "today", "top", "travel", "water", "way", "week", "will", "work", "world", "year",]
 adverbs = [ "every", "next", "well",]
 adjectives = [ "another", "any", "different", "each", "every", "first", "free", "full", "good", "great", "high", "hot", "important", "last", "left", "little", "low", "new", "next", "no", "open", "other", "right", "same", "small", "some", "such", "young",]
-verbs = [ "buy", "come", "do", "find", "free", "have", "know", "learn", "let", "like", "live", "look", "love", "make", "name", "need", "place", "play", "read", "say", "see", "sell", "send", "show", "take", "think", "travel", "use", "want", "work",]
+verbs = [ "buy", "come", "do", "find", "have", "know", "learn", "let", "like", "live", "look", "love", "make", "need", "place", "play", "read", "say", "see", "sell", "send", "show", "take", "think", "travel", "use", "want", "work",]
```

### Comparing `hmeg-0.1.3/hmeg/vocabulary.py` & `hmeg-0.1.4/hmeg/vocabulary.py`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.3/PKG-INFO` & `hmeg-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmeg
-Version: 0.1.3
+Version: 0.1.4
 Summary: Generator of exercises for practicing speaking for language learning.
 Home-page: https://github.com/yurytsoy/hmeg
 License: MIT
 Author: Yury Choi
 Author-email: yurytsoy@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

