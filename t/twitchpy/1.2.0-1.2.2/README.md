# Comparing `tmp/TwitchPy-1.2.0.tar.gz` & `tmp/twitchpy-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TwitchPy-1.2.0.tar", last modified: Sat Apr 27 12:23:43 2024, max compression
+gzip compressed data, was "twitchpy-1.2.2.tar", last modified: Sat Apr 27 14:15:07 2024, max compression
```

## Comparing `TwitchPy-1.2.0.tar` & `twitchpy-1.2.2.tar`

### file list

```diff
@@ -1,9 +1,105 @@
-drwxr-xr-x   0 dacasbe   (1000) dacasbe   (1000)        0 2024-04-27 12:23:43.695703 TwitchPy-1.2.0/
--rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      397 2024-04-27 12:23:43.695703 TwitchPy-1.2.0/PKG-INFO
--rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)       39 2024-04-27 12:21:50.001596 TwitchPy-1.2.0/setup.cfg
--rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      487 2024-04-27 12:22:42.411949 TwitchPy-1.2.0/setup.py
-drwxr-xr-x   0 dacasbe   (1000) dacasbe   (1000)        0 2024-04-27 12:23:43.695703 TwitchPy-1.2.0/twitchpy/
--rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)       48 2024-04-27 12:22:01.758342 TwitchPy-1.2.0/twitchpy/__init__.py
--rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)    43477 2024-04-27 12:22:01.791675 TwitchPy-1.2.0/twitchpy/bot.py
--rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)   144401 2024-04-27 12:22:01.798342 TwitchPy-1.2.0/twitchpy/client.py
--rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      562 2024-04-27 12:22:01.821675 TwitchPy-1.2.0/twitchpy/errors.py
+drwxr-xr-x   0 dacasbe   (1000) dacasbe   (1000)        0 2024-04-27 14:15:07.796839 twitchpy-1.2.2/
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      397 2024-04-27 14:15:07.796839 twitchpy-1.2.2/PKG-INFO
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)       39 2024-04-27 12:21:50.001596 twitchpy-1.2.2/setup.cfg
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      547 2024-04-27 14:14:45.286705 twitchpy-1.2.2/setup.py
+drwxr-xr-x   0 dacasbe   (1000) dacasbe   (1000)        0 2024-04-27 14:15:07.790172 twitchpy-1.2.2/twitchpy/
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)       48 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/__init__.py
+drwxr-xr-x   0 dacasbe   (1000) dacasbe   (1000)        0 2024-04-27 14:15:07.793505 twitchpy-1.2.2/twitchpy/_api/
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)        0 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/__init__.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1979 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/ads.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     2452 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/analytics.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     2020 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/bits.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     6022 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/channels.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     2310 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/charity_campaigns.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)    10903 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/chats.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     2379 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/clips.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      781 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/content_classification_labels.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     2097 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/drops.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     7115 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/eventsubs.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)    11934 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/extensions.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1294 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/games.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      974 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/goals.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     9566 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/guest_stars.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     2027 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/hype_trains.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)    15596 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/moderation.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     4310 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/polls.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     6392 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/predictions.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      943 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/raids.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)    12726 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/rewards.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     7634 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/schedules.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1268 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/searchs.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     4012 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/streams.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     2320 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/subscriptions.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1251 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/tags.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     2010 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/teams.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     4341 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/users.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     2098 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/videos.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      494 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_api/whispers.py
+drwxr-xr-x   0 dacasbe   (1000) dacasbe   (1000)        0 2024-04-27 14:15:07.793505 twitchpy-1.2.2/twitchpy/_utils/
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)        0 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_utils/__init__.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)       44 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_utils/date.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     4104 2024-04-27 12:22:01.758342 twitchpy-1.2.2/twitchpy/_utils/http.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)    43477 2024-04-27 12:22:01.791675 twitchpy-1.2.2/twitchpy/bot.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)   144401 2024-04-27 12:22:01.798342 twitchpy-1.2.2/twitchpy/client.py
+drwxr-xr-x   0 dacasbe   (1000) dacasbe   (1000)        0 2024-04-27 14:15:07.793505 twitchpy-1.2.2/twitchpy/dataclasses/
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     2393 2024-04-27 12:22:01.798342 twitchpy-1.2.2/twitchpy/dataclasses/__init__.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      955 2024-04-27 12:22:01.798342 twitchpy-1.2.2/twitchpy/dataclasses/ad_schedule.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1221 2024-04-27 12:22:01.798342 twitchpy-1.2.2/twitchpy/dataclasses/automod_settings.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      330 2024-04-27 12:22:01.798342 twitchpy-1.2.2/twitchpy/dataclasses/badge.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      875 2024-04-27 12:22:01.798342 twitchpy-1.2.2/twitchpy/dataclasses/badge_version.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      803 2024-04-27 12:22:01.798342 twitchpy-1.2.2/twitchpy/dataclasses/banned_user.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      401 2024-04-27 12:22:01.798342 twitchpy-1.2.2/twitchpy/dataclasses/bits_leaderboard_leader.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      937 2024-04-27 12:22:01.798342 twitchpy-1.2.2/twitchpy/dataclasses/blocked_term.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1128 2024-04-27 12:22:01.798342 twitchpy-1.2.2/twitchpy/dataclasses/channel.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      995 2024-04-27 12:22:01.801675 twitchpy-1.2.2/twitchpy/dataclasses/charity_campaign.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      527 2024-04-27 12:22:01.801675 twitchpy-1.2.2/twitchpy/dataclasses/charity_campaign_amount.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      619 2024-04-27 12:22:01.801675 twitchpy-1.2.2/twitchpy/dataclasses/charity_campaign_donation.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1822 2024-04-27 12:22:01.801675 twitchpy-1.2.2/twitchpy/dataclasses/chat_settings.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1230 2024-04-27 12:22:01.801675 twitchpy-1.2.2/twitchpy/dataclasses/cheermote.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1431 2024-04-27 12:22:01.801675 twitchpy-1.2.2/twitchpy/dataclasses/cheermote_tier.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1550 2024-04-27 12:22:01.801675 twitchpy-1.2.2/twitchpy/dataclasses/clip.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      441 2024-04-27 12:22:01.801675 twitchpy-1.2.2/twitchpy/dataclasses/commercial.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      272 2024-04-27 12:22:01.801675 twitchpy-1.2.2/twitchpy/dataclasses/conduit.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      729 2024-04-27 12:22:01.801675 twitchpy-1.2.2/twitchpy/dataclasses/conduit_shard.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      380 2024-04-27 12:22:01.801675 twitchpy-1.2.2/twitchpy/dataclasses/content_classification_label.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      890 2024-04-27 12:22:01.801675 twitchpy-1.2.2/twitchpy/dataclasses/creator_goal.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1002 2024-04-27 12:22:01.801675 twitchpy-1.2.2/twitchpy/dataclasses/drop_entitlement.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1640 2024-04-27 12:22:01.805009 twitchpy-1.2.2/twitchpy/dataclasses/emote.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1106 2024-04-27 12:22:01.805009 twitchpy-1.2.2/twitchpy/dataclasses/eventsub_subscription.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     2974 2024-04-27 12:22:01.805009 twitchpy-1.2.2/twitchpy/dataclasses/extension.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      622 2024-04-27 12:22:01.805009 twitchpy-1.2.2/twitchpy/dataclasses/extension_analytics_report.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      585 2024-04-27 12:22:01.805009 twitchpy-1.2.2/twitchpy/dataclasses/extension_configuration_segment.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      555 2024-04-27 12:22:01.805009 twitchpy-1.2.2/twitchpy/dataclasses/extension_secret.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      821 2024-04-27 12:22:01.805009 twitchpy-1.2.2/twitchpy/dataclasses/extension_transaction.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      497 2024-04-27 12:22:01.805009 twitchpy-1.2.2/twitchpy/dataclasses/game.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      596 2024-04-27 12:22:01.805009 twitchpy-1.2.2/twitchpy/dataclasses/game_analytics_report.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      948 2024-04-27 12:22:01.805009 twitchpy-1.2.2/twitchpy/dataclasses/guest.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1086 2024-04-27 12:22:01.805009 twitchpy-1.2.2/twitchpy/dataclasses/guest_star_invite.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      409 2024-04-27 12:22:01.805009 twitchpy-1.2.2/twitchpy/dataclasses/guest_star_session.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      995 2024-04-27 12:22:01.805009 twitchpy-1.2.2/twitchpy/dataclasses/guest_star_settings.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      416 2024-04-27 12:22:01.805009 twitchpy-1.2.2/twitchpy/dataclasses/hype_train_contribution.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1399 2024-04-27 12:22:01.805009 twitchpy-1.2.2/twitchpy/dataclasses/hype_train_event_data.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      656 2024-04-27 12:22:01.805009 twitchpy-1.2.2/twitchpy/dataclasses/hypetrain_event.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      853 2024-04-27 12:22:01.808342 twitchpy-1.2.2/twitchpy/dataclasses/message.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1260 2024-04-27 12:22:01.808342 twitchpy-1.2.2/twitchpy/dataclasses/poll.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      522 2024-04-27 12:22:01.808342 twitchpy-1.2.2/twitchpy/dataclasses/poll_choice.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1352 2024-04-27 12:22:01.808342 twitchpy-1.2.2/twitchpy/dataclasses/prediction.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      787 2024-04-27 12:22:01.808342 twitchpy-1.2.2/twitchpy/dataclasses/prediction_outcome.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      447 2024-04-27 12:22:01.808342 twitchpy-1.2.2/twitchpy/dataclasses/predictor.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      872 2024-04-27 12:22:01.808342 twitchpy-1.2.2/twitchpy/dataclasses/product.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      322 2024-04-27 12:22:01.808342 twitchpy-1.2.2/twitchpy/dataclasses/product_cost.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      799 2024-04-27 12:22:01.808342 twitchpy-1.2.2/twitchpy/dataclasses/redemption.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     2406 2024-04-27 12:22:01.808342 twitchpy-1.2.2/twitchpy/dataclasses/reward.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      553 2024-04-27 12:22:01.808342 twitchpy-1.2.2/twitchpy/dataclasses/shield_mode_status.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1162 2024-04-27 12:22:01.808342 twitchpy-1.2.2/twitchpy/dataclasses/stream.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      660 2024-04-27 12:22:01.808342 twitchpy-1.2.2/twitchpy/dataclasses/stream_marker.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      682 2024-04-27 12:22:01.808342 twitchpy-1.2.2/twitchpy/dataclasses/stream_schedule.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1099 2024-04-27 12:22:01.808342 twitchpy-1.2.2/twitchpy/dataclasses/stream_schedule_segment.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      721 2024-04-27 12:22:01.808342 twitchpy-1.2.2/twitchpy/dataclasses/subscription.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      640 2024-04-27 12:22:01.808342 twitchpy-1.2.2/twitchpy/dataclasses/tag.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      904 2024-04-27 12:22:01.808342 twitchpy-1.2.2/twitchpy/dataclasses/team.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      908 2024-04-27 12:22:01.808342 twitchpy-1.2.2/twitchpy/dataclasses/transport.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1082 2024-04-27 12:22:01.811675 twitchpy-1.2.2/twitchpy/dataclasses/unban_request.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1189 2024-04-27 12:22:01.811675 twitchpy-1.2.2/twitchpy/dataclasses/user.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)     1366 2024-04-27 12:22:01.811675 twitchpy-1.2.2/twitchpy/dataclasses/video.py
+-rw-r--r--   0 dacasbe   (1000) dacasbe   (1000)      562 2024-04-27 12:22:01.821675 twitchpy-1.2.2/twitchpy/errors.py
```

### Comparing `TwitchPy-1.2.0/twitchpy/bot.py` & `twitchpy-1.2.2/twitchpy/bot.py`

 * *Files identical despite different names*

### Comparing `TwitchPy-1.2.0/twitchpy/client.py` & `twitchpy-1.2.2/twitchpy/client.py`

 * *Files identical despite different names*

### Comparing `TwitchPy-1.2.0/twitchpy/errors.py` & `twitchpy-1.2.2/twitchpy/errors.py`

 * *Files identical despite different names*

