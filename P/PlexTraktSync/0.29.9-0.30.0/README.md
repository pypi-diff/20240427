# Comparing `tmp/PlexTraktSync-0.29.9.tar.gz` & `tmp/plextraktsync-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlexTraktSync-0.29.9.tar", last modified: Tue Mar 26 22:39:34 2024, max compression
+gzip compressed data, was "plextraktsync-0.30.0.tar", last modified: Sat Apr 27 18:24:03 2024, max compression
```

## Comparing `PlexTraktSync-0.29.9.tar` & `plextraktsync-0.30.0.tar`

### file list

```diff
@@ -1,154 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.567499 PlexTraktSync-0.29.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    29730 2024-03-26 22:39:34.567499 PlexTraktSync-0.29.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.567499 PlexTraktSync-0.29.9/PlexTraktSync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29730 2024-03-26 22:39:34.000000 PlexTraktSync-0.29.9/PlexTraktSync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-03-26 22:39:34.000000 PlexTraktSync-0.29.9/PlexTraktSync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 22:39:34.000000 PlexTraktSync-0.29.9/PlexTraktSync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-26 22:39:34.000000 PlexTraktSync-0.29.9/PlexTraktSync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-26 22:39:34.000000 PlexTraktSync-0.29.9/PlexTraktSync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-26 22:39:34.000000 PlexTraktSync-0.29.9/PlexTraktSync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26700 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.547499 PlexTraktSync-0.29.9/plextraktsync/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.551499 PlexTraktSync-0.29.9/plextraktsync/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/bug_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/clear_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/imdb_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/plex_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/self_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/trakt_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/unmatched.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/watch.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/commands/watched_shows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.551499 PlexTraktSync-0.29.9/plextraktsync/config/
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config/ConfigLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config/ConfigMergeMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config/HttpCacheConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config/PlexServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config/RunConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config/ServerConfigFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config/SyncConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/config.default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.551499 PlexTraktSync-0.29.9/plextraktsync/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/decorators/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/decorators/measure_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/decorators/memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/decorators/nocache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/decorators/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/decorators/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/decorators/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.551499 PlexTraktSync-0.29.9/plextraktsync/logger/
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/logger/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/logger/init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.551499 PlexTraktSync-0.29.9/plextraktsync/media/
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/media/Media.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/media/MediaFactory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.551499 PlexTraktSync-0.29.9/plextraktsync/mixin/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/mixin/ChangeNotifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/mixin/RichMarkup.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/mixin/SetWindowTitle.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.555499 PlexTraktSync-0.29.9/plextraktsync/plan/
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plan/WalkConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plan/WalkPlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plan/WalkPlanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plan/Walker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.555499 PlexTraktSync-0.29.9/plextraktsync/plex/
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexAudioCodec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuidProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuidProviderIMDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuidProviderLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuidProviderMbid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuidProviderTMDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuidProviderTVDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexId.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexIdFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexLibraryItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexLibrarySection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexPlaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexPlaylistCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexRatings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexSectionPager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexServerConnection.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/PlexWatchList.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/SessionCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/plex/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/pytrakt_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.559499 PlexTraktSync-0.29.9/plextraktsync/queue/
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/queue/BackgroundTask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/queue/Queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/queue/TraktBatchWorker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/queue/TraktMarkWatchedWorker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/queue/TraktScrobbleWorker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.559499 PlexTraktSync-0.29.9/plextraktsync/rich/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/rich/RichHighlighter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/rich/RichProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/style.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.559499 PlexTraktSync-0.29.9/plextraktsync/sync/
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/sync/Sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.559499 PlexTraktSync-0.29.9/plextraktsync/trakt/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/PartialTraktMedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/ScrobblerCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/ScrobblerProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10006 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/TraktApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/TraktItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/TraktLookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/TraktRatingCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/TraktUserList.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/TraktUserListCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/TraktWatchlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/trakt_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/trakt/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.563499 PlexTraktSync-0.29.9/plextraktsync/util/
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/Factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/Path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/Rating.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/Timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/Version.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/execp.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/execx.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/expand_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/git_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/local_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/openurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/parse_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/util/remove_empty_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.563499 PlexTraktSync-0.29.9/plextraktsync/watch/
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/watch/EventDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/watch/EventFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/watch/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/watch/WatchStateUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/watch/WebSocketListener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/plextraktsync/watch/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-26 22:39:32.000000 PlexTraktSync-0.29.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-26 22:39:34.567499 PlexTraktSync-0.29.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:39:34.563499 PlexTraktSync-0.29.9/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1923 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_collection_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1443 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2703 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_events.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_logger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      977 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_new_agent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2104 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_plex_id.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_rating.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      503 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_threading.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1174 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_timer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      572 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_trakt_progress.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3584 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_tv_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-03-26 22:39:30.000000 PlexTraktSync-0.29.9/tests/test_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.533368 plextraktsync-0.30.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    30033 2024-04-27 18:24:03.533368 plextraktsync-0.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.533368 plextraktsync-0.30.0/PlexTraktSync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    30033 2024-04-27 18:24:03.000000 plextraktsync-0.30.0/PlexTraktSync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-27 18:24:03.000000 plextraktsync-0.30.0/PlexTraktSync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 18:24:03.000000 plextraktsync-0.30.0/PlexTraktSync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-27 18:24:03.000000 plextraktsync-0.30.0/PlexTraktSync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-27 18:24:03.000000 plextraktsync-0.30.0/PlexTraktSync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-27 18:24:03.000000 plextraktsync-0.30.0/PlexTraktSync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26812 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.513368 plextraktsync-0.30.0/plextraktsync/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.517368 plextraktsync-0.30.0/plextraktsync/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/clear_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/imdb_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/plex_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/self_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/trakt_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/unmatched.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/commands/watched_shows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.517368 plextraktsync-0.30.0/plextraktsync/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config/ConfigLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config/ConfigMergeMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config/HttpCacheConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config/PlexServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config/RunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config/ServerConfigFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config/SyncConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/config.default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.517368 plextraktsync-0.30.0/plextraktsync/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/decorators/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/decorators/measure_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/decorators/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/decorators/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/decorators/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/decorators/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/decorators/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.517368 plextraktsync-0.30.0/plextraktsync/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/logger/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/logger/init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.517368 plextraktsync-0.30.0/plextraktsync/media/
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/media/Media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/media/MediaFactory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.521368 plextraktsync-0.30.0/plextraktsync/mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/mixin/ChangeNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/mixin/RichMarkup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/mixin/SetWindowTitle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.521368 plextraktsync-0.30.0/plextraktsync/plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plan/WalkConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plan/WalkPlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plan/WalkPlanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plan/Walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.525368 plextraktsync-0.30.0/plextraktsync/plex/
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexAudioCodec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexGuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexGuidProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexGuidProviderIMDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexGuidProviderLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexGuidProviderMbid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexGuidProviderTMDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexGuidProviderTVDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexId.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexIdFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexLibraryItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexLibrarySection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexPlaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexPlaylistCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexRatings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexSectionPager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexServerConnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/PlexWatchList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/SessionCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plex/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.525368 plextraktsync-0.30.0/plextraktsync/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/pytrakt_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.525368 plextraktsync-0.30.0/plextraktsync/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/queue/BackgroundTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/queue/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/queue/TraktBatchWorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/queue/TraktMarkWatchedWorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/queue/TraktScrobbleWorker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.525368 plextraktsync-0.30.0/plextraktsync/rich/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/rich/RichHighlighter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/rich/RichProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/style.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.525368 plextraktsync-0.30.0/plextraktsync/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/AddCollectionPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/ClearCollectedPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/LikedListsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/Sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/SyncRatingsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/SyncWatchedPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/WatchListPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/WatchProgressPlugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.525368 plextraktsync-0.30.0/plextraktsync/sync/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/plugin/SyncPluginInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/plugin/SyncPluginManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/sync/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.529368 plextraktsync-0.30.0/plextraktsync/trakt/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/PartialTraktMedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/ScrobblerCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/ScrobblerProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/TraktApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/TraktItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/TraktLookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/TraktRatingCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/TraktUserList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/TraktUserListCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/TraktWatchlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/WatchProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/trakt_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/trakt/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.529368 plextraktsync-0.30.0/plextraktsync/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/Factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/Path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/Rating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/Timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/Version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/execp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/execx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/expand_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/git_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/local_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/openurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/parse_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/util/remove_empty_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.533368 plextraktsync-0.30.0/plextraktsync/watch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/watch/EventDispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/watch/EventFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/watch/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/watch/WatchStateUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/watch/WebSocketListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/plextraktsync/watch/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-27 18:24:01.000000 plextraktsync-0.30.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-27 18:24:03.533368 plextraktsync-0.30.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:03.533368 plextraktsync-0.30.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1923 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_collection_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1443 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2703 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      977 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_new_agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2104 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_plex_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_rating.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      503 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_threading.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1174 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_timer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      572 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_trakt_progress.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3584 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_tv_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-04-27 18:23:59.000000 plextraktsync-0.30.0/tests/test_walker.py
```

### Comparing `PlexTraktSync-0.29.9/LICENSE` & `plextraktsync-0.30.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/PKG-INFO` & `plextraktsync-0.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.29.9
+Version: 0.30.0
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,35 +20,39 @@
 License-File: LICENSE
 Requires-Dist: attrs==23.2.0; python_version >= "3.7"
 Requires-Dist: cattrs==23.2.3; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: certifi==2024.2.2; python_version >= "3.6"
 Requires-Dist: charset-normalizer==3.3.2; python_full_version >= "3.7.0"
 Requires-Dist: click==8.1.7; python_version >= "3.7"
 Requires-Dist: deprecated==1.2.14; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
-Requires-Dist: idna==3.6; python_version >= "3.5"
+Requires-Dist: exceptiongroup==1.2.0; python_version < "3.11"
+Requires-Dist: humanize==4.9.0; python_version >= "3.8"
+Requires-Dist: idna==3.7; python_version >= "3.5"
 Requires-Dist: inquirerpy==0.3.4; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: mdurl==0.1.2; python_version >= "3.7"
 Requires-Dist: oauthlib==3.2.2; python_version >= "3.6"
 Requires-Dist: pfzy==0.3.4; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: platformdirs==4.2.0; python_version >= "3.7" and python_version >= "3.8"
-Requires-Dist: plexapi==4.15.10; python_version >= "3.8"
+Requires-Dist: plexapi==4.15.11; python_version >= "3.8"
+Requires-Dist: pluggy==1.4.0; python_version >= "3.8"
 Requires-Dist: prompt-toolkit==3.0.43; python_full_version >= "3.7.0"
 Requires-Dist: pygments==2.17.2; python_version >= "3.7"
 Requires-Dist: python-dotenv==1.0.1; python_version >= "3.8"
 Requires-Dist: python-git-info==0.8.3
 Requires-Dist: pytimeparse==1.1.8
-Requires-Dist: pytrakt==3.4.31
+Requires-Dist: pytrakt==3.4.32
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6"
 Requires-Dist: requests==2.31.0; python_version >= "3.7"
 Requires-Dist: requests-cache==1.2.0; python_version >= "3.8"
-Requires-Dist: requests-oauthlib==1.4.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
+Requires-Dist: requests-oauthlib==2.0.0; python_version >= "3.4"
 Requires-Dist: rich==13.7.1; python_full_version >= "3.7.0"
 Requires-Dist: six==1.16.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3" and python_version >= "3.4"
 Requires-Dist: tqdm==4.66.2; python_version >= "3.7"
+Requires-Dist: typing-extensions==4.11.0; python_version < "3.11"
 Requires-Dist: url-normalize==1.4.3; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5" and python_version >= "3.6"
 Requires-Dist: urllib3==2.2.1; python_version >= "3.8"
 Requires-Dist: wcwidth==0.2.13
 Requires-Dist: websocket-client==1.7.0; python_version >= "3.8"
 Requires-Dist: wrapt==1.16.0; python_version >= "3.5" and python_version >= "3.6"
 
 # Plex-Trakt-Sync
@@ -361,14 +365,17 @@
 Academy Award Nominees" but might not be ideal for lists that are updated
 often). Here are the execution times on my Plex server: First run - 1228
 seconds, second run - 111 seconds
 
 You can view sync progress in the `plextraktsync.log` file which will be
 created.
 
+You can use `--edit` or `--locate` flags to `config` command to open config
+file in editor or in file browser.
+
 ### Libraries
 
 By default, all libraries are processed. You can disable libraries by name by
 changing `excluded-libraries` in `config.yml`.
 
 You can also set `excluded-libraries` per server in `servers.yml`:
```

### Comparing `PlexTraktSync-0.29.9/PlexTraktSync.egg-info/PKG-INFO` & `plextraktsync-0.30.0/PlexTraktSync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.29.9
+Version: 0.30.0
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,35 +20,39 @@
 License-File: LICENSE
 Requires-Dist: attrs==23.2.0; python_version >= "3.7"
 Requires-Dist: cattrs==23.2.3; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: certifi==2024.2.2; python_version >= "3.6"
 Requires-Dist: charset-normalizer==3.3.2; python_full_version >= "3.7.0"
 Requires-Dist: click==8.1.7; python_version >= "3.7"
 Requires-Dist: deprecated==1.2.14; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
-Requires-Dist: idna==3.6; python_version >= "3.5"
+Requires-Dist: exceptiongroup==1.2.0; python_version < "3.11"
+Requires-Dist: humanize==4.9.0; python_version >= "3.8"
+Requires-Dist: idna==3.7; python_version >= "3.5"
 Requires-Dist: inquirerpy==0.3.4; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: mdurl==0.1.2; python_version >= "3.7"
 Requires-Dist: oauthlib==3.2.2; python_version >= "3.6"
 Requires-Dist: pfzy==0.3.4; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: platformdirs==4.2.0; python_version >= "3.7" and python_version >= "3.8"
-Requires-Dist: plexapi==4.15.10; python_version >= "3.8"
+Requires-Dist: plexapi==4.15.11; python_version >= "3.8"
+Requires-Dist: pluggy==1.4.0; python_version >= "3.8"
 Requires-Dist: prompt-toolkit==3.0.43; python_full_version >= "3.7.0"
 Requires-Dist: pygments==2.17.2; python_version >= "3.7"
 Requires-Dist: python-dotenv==1.0.1; python_version >= "3.8"
 Requires-Dist: python-git-info==0.8.3
 Requires-Dist: pytimeparse==1.1.8
-Requires-Dist: pytrakt==3.4.31
+Requires-Dist: pytrakt==3.4.32
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6"
 Requires-Dist: requests==2.31.0; python_version >= "3.7"
 Requires-Dist: requests-cache==1.2.0; python_version >= "3.8"
-Requires-Dist: requests-oauthlib==1.4.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
+Requires-Dist: requests-oauthlib==2.0.0; python_version >= "3.4"
 Requires-Dist: rich==13.7.1; python_full_version >= "3.7.0"
 Requires-Dist: six==1.16.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3" and python_version >= "3.4"
 Requires-Dist: tqdm==4.66.2; python_version >= "3.7"
+Requires-Dist: typing-extensions==4.11.0; python_version < "3.11"
 Requires-Dist: url-normalize==1.4.3; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5" and python_version >= "3.6"
 Requires-Dist: urllib3==2.2.1; python_version >= "3.8"
 Requires-Dist: wcwidth==0.2.13
 Requires-Dist: websocket-client==1.7.0; python_version >= "3.8"
 Requires-Dist: wrapt==1.16.0; python_version >= "3.5" and python_version >= "3.6"
 
 # Plex-Trakt-Sync
@@ -361,14 +365,17 @@
 Academy Award Nominees" but might not be ideal for lists that are updated
 often). Here are the execution times on my Plex server: First run - 1228
 seconds, second run - 111 seconds
 
 You can view sync progress in the `plextraktsync.log` file which will be
 created.
 
+You can use `--edit` or `--locate` flags to `config` command to open config
+file in editor or in file browser.
+
 ### Libraries
 
 By default, all libraries are processed. You can disable libraries by name by
 changing `excluded-libraries` in `config.yml`.
 
 You can also set `excluded-libraries` per server in `servers.yml`:
```

### Comparing `PlexTraktSync-0.29.9/PlexTraktSync.egg-info/SOURCES.txt` & `plextraktsync-0.30.0/PlexTraktSync.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -77,32 +77,45 @@
 plextraktsync/plex/PlexPlaylistCollection.py
 plextraktsync/plex/PlexRatings.py
 plextraktsync/plex/PlexSectionPager.py
 plextraktsync/plex/PlexServerConnection.py
 plextraktsync/plex/PlexWatchList.py
 plextraktsync/plex/SessionCollection.py
 plextraktsync/plex/types.py
+plextraktsync/plugin/__init__.py
+plextraktsync/plugin/plugin.py
 plextraktsync/queue/BackgroundTask.py
 plextraktsync/queue/Queue.py
 plextraktsync/queue/TraktBatchWorker.py
 plextraktsync/queue/TraktMarkWatchedWorker.py
 plextraktsync/queue/TraktScrobbleWorker.py
 plextraktsync/rich/RichHighlighter.py
 plextraktsync/rich/RichProgressBar.py
+plextraktsync/sync/AddCollectionPlugin.py
+plextraktsync/sync/ClearCollectedPlugin.py
+plextraktsync/sync/LikedListsPlugin.py
 plextraktsync/sync/Sync.py
+plextraktsync/sync/SyncRatingsPlugin.py
+plextraktsync/sync/SyncWatchedPlugin.py
+plextraktsync/sync/WatchListPlugin.py
+plextraktsync/sync/WatchProgressPlugin.py
+plextraktsync/sync/plugin/SyncPluginInterface.py
+plextraktsync/sync/plugin/SyncPluginManager.py
+plextraktsync/sync/plugin/__init__.py
 plextraktsync/trakt/PartialTraktMedia.py
 plextraktsync/trakt/ScrobblerCollection.py
 plextraktsync/trakt/ScrobblerProxy.py
 plextraktsync/trakt/TraktApi.py
 plextraktsync/trakt/TraktItem.py
 plextraktsync/trakt/TraktLookup.py
 plextraktsync/trakt/TraktRatingCollection.py
 plextraktsync/trakt/TraktUserList.py
 plextraktsync/trakt/TraktUserListCollection.py
 plextraktsync/trakt/TraktWatchlist.py
+plextraktsync/trakt/WatchProgress.py
 plextraktsync/trakt/trakt_set.py
 plextraktsync/trakt/types.py
 plextraktsync/util/Factory.py
 plextraktsync/util/Path.py
 plextraktsync/util/Rating.py
 plextraktsync/util/Timer.py
 plextraktsync/util/Version.py
```

### Comparing `PlexTraktSync-0.29.9/PlexTraktSync.egg-info/requires.txt` & `plextraktsync-0.30.0/PlexTraktSync.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 python-git-info==0.8.3
 pytimeparse==1.1.8
-pytrakt==3.4.31
+pytrakt==3.4.32
 wcwidth==0.2.13
 
 [:python_full_version >= "3.7.0"]
 charset-normalizer==3.3.2
 prompt-toolkit==3.0.43
 rich==13.7.1
 
+[:python_version < "3.11"]
+exceptiongroup==1.2.0
+typing-extensions==4.11.0
+
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"]
 deprecated==1.2.14
-requests-oauthlib==1.4.0
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3" and python_version >= "3.4"]
 six==1.16.0
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5" and python_version >= "3.6"]
 url-normalize==1.4.3
 
+[:python_version >= "3.4"]
+requests-oauthlib==2.0.0
+
 [:python_version >= "3.5"]
-idna==3.6
+idna==3.7
 
 [:python_version >= "3.5" and python_version >= "3.6"]
 wrapt==1.16.0
 
 [:python_version >= "3.6"]
 certifi==2024.2.2
 oauthlib==3.2.2
@@ -43,12 +49,14 @@
 
 [:python_version >= "3.7" and python_version >= "3.8"]
 cattrs==23.2.3
 markdown-it-py==3.0.0
 platformdirs==4.2.0
 
 [:python_version >= "3.8"]
-plexapi==4.15.10
+humanize==4.9.0
+plexapi==4.15.11
+pluggy==1.4.0
 python-dotenv==1.0.1
 requests-cache==1.2.0
 urllib3==2.2.1
 websocket-client==1.7.0
```

### Comparing `PlexTraktSync-0.29.9/README.md` & `plextraktsync-0.30.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -308,14 +308,17 @@
 Academy Award Nominees" but might not be ideal for lists that are updated
 often). Here are the execution times on my Plex server: First run - 1228
 seconds, second run - 111 seconds
 
 You can view sync progress in the `plextraktsync.log` file which will be
 created.
 
+You can use `--edit` or `--locate` flags to `config` command to open config
+file in editor or in file browser.
+
 ### Libraries
 
 By default, all libraries are processed. You can disable libraries by name by
 changing `excluded-libraries` in `config.yml`.
 
 You can also set `excluded-libraries` per server in `servers.yml`:
```

### Comparing `PlexTraktSync-0.29.9/plextraktsync/cli.py` & `plextraktsync-0.30.0/plextraktsync/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,14 +328,16 @@
     """
     Print a table of watched shows
     """
 
 
 @command()
 @click.option("--urls-expire-after", is_flag=True, help="Print urls_expire_after configuration")
+@click.option("--edit", is_flag=True, help="Open config file in editor")
+@click.option("--locate", is_flag=True, help="Locate config file in file browser")
 def config():
     """
     Print user config for debugging and bug reports.
     """
 
 
 cli.add_command(bug_report)
```

### Comparing `PlexTraktSync-0.29.9/plextraktsync/commands/bug_report.py` & `plextraktsync-0.30.0/plextraktsync/commands/bug_report.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/commands/cache.py` & `plextraktsync-0.30.0/plextraktsync/commands/cache.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/commands/clear_collections.py` & `plextraktsync-0.30.0/plextraktsync/commands/clear_collections.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/commands/download.py` & `plextraktsync-0.30.0/plextraktsync/commands/download.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/commands/imdb_import.py` & `plextraktsync-0.30.0/plextraktsync/commands/imdb_import.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/commands/info.py` & `plextraktsync-0.30.0/plextraktsync/commands/info.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/commands/inspect.py` & `plextraktsync-0.30.0/plextraktsync/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/commands/login.py` & `plextraktsync-0.30.0/plextraktsync/commands/login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/commands/plex_login.py` & `plextraktsync-0.30.0/plextraktsync/commands/plex_login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/commands/self_update.py` & `plextraktsync-0.30.0/plextraktsync/commands/self_update.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/commands/sync.py` & `plextraktsync-0.30.0/plextraktsync/commands/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     if library:
         wc.add_library(library)
     if show:
         wc.add_show(show)
     if movie:
         wc.add_movie(movie)
 
-    if not wc.is_valid():
+    if not wc.is_valid:
         print("Nothing to sync, this is likely due conflicting options given.")
         return
 
     with measure_time("Completed full sync"):
         runner = factory.sync
         if runner.config.need_library_walk:
             w.print_plan(print=logger.info)
```

### Comparing `PlexTraktSync-0.29.9/plextraktsync/commands/trakt_login.py` & `plextraktsync-0.30.0/plextraktsync/commands/trakt_login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/commands/unmatched.py` & `plextraktsync-0.30.0/plextraktsync/commands/unmatched.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     factory.run_config.update(progressbar=not no_progress_bar)
     ensure_login()
     plex = factory.plex_api
     mf = factory.media_factory
     wc = factory.walk_config
     walker = factory.walker
 
-    if not wc.is_valid():
+    if not wc.is_valid:
         print("Nothing to scan, this is likely due conflicting options given.")
         return
 
     failed = []
     if local:
         for pm in walker.get_plex_movies():
             if all(guid.local for guid in pm.guids):
```

### Comparing `PlexTraktSync-0.29.9/plextraktsync/commands/watch.py` & `plextraktsync-0.30.0/plextraktsync/commands/watch.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/commands/watched_shows.py` & `plextraktsync-0.30.0/plextraktsync/commands/watched_shows.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/config/Config.py` & `plextraktsync-0.30.0/plextraktsync/config/Config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/config/ConfigLoader.py` & `plextraktsync-0.30.0/plextraktsync/config/ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/config/HttpCacheConfig.py` & `plextraktsync-0.30.0/plextraktsync/config/HttpCacheConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         "metadata.provider.plex.tv/": 86400,
         # Plex account
         # Cache for some time, this activates 304 responses
         "plex.tv/users/account": "1m",
         "plex.tv/api/v2/user": "1m",
         # Plex patterns
         # Ratings search
-        "*/library/sections/*/all?*userRating%3E%3E=-1*": DO_NOT_CACHE,
+        "*/library/sections/*/all?*userRating%3E%3E=-1*": "1m",
         # len(PlexLibrarySection)
         "*/library/sections/*/all?includeCollections=0&X-Plex-Container-Size=0&X-Plex-Container-Start=0": DO_NOT_CACHE,
         # __iter__(PlexLibrarySection)
         "*/library/sections/*/all?includeGuids=1": DO_NOT_CACHE,
         # find_by_title
         "*/library/sections/*/all?includeGuids=1&title=*": DO_NOT_CACHE,
         # fetch_item, fetch_items
```

### Comparing `PlexTraktSync-0.29.9/plextraktsync/config/PlexServerConfig.py` & `plextraktsync-0.30.0/plextraktsync/config/PlexServerConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/config/ServerConfigFactory.py` & `plextraktsync-0.30.0/plextraktsync/config/ServerConfigFactory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/config/SyncConfig.py` & `plextraktsync-0.30.0/plextraktsync/config/SyncConfig.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,14 +53,18 @@
         return self.plex_to_trakt["collection"] and self["plex_to_trakt"]["clear_collected"]
 
     @cached_property
     def sync_watched_status(self):
         return self.trakt_to_plex["watched_status"] or self.plex_to_trakt["watched_status"]
 
     @cached_property
+    def sync_playback_status(self):
+        return self["trakt_to_plex"]["playback_status"]
+
+    @cached_property
     def update_plex_wl(self):
         return self.trakt_to_plex["watchlist"] and not self.trakt_to_plex["watchlist_as_playlist"]
 
     @cached_property
     def update_plex_wl_as_pl(self):
         return self.trakt_to_plex["watchlist"] and self.trakt_to_plex["watchlist_as_playlist"]
 
@@ -80,8 +84,9 @@
     def need_library_walk(self):
         return any([
             self.update_plex_wl_as_pl,
             self.sync_watched_status,
             self.sync_ratings,
             self.plex_to_trakt["collection"],
             self.sync_liked_lists,
+            self.sync_playback_status,
         ])
```

### Comparing `PlexTraktSync-0.29.9/plextraktsync/config.default.yml` & `plextraktsync-0.30.0/plextraktsync/config.default.yml`

 * *Files 7% similar despite different names*

```diff
@@ -17,22 +17,22 @@
   append: true
   # Whether to show timestamps in console messages
   console_time: false
   debug: false
   filename: plextraktsync.log
   # Additional logger names to apply filtering
   filter_loggers:
-#    - plexapi
-#    - requests_cache.backends
-#    - requests_cache.backends.base
-#    - requests_cache.backends.sqlite
-#    - requests_cache.policy.actions
-#    - requests_cache.session
-#    - trakt.core
-#    - urllib3.connectionpool
+  #    - plexapi
+  #    - requests_cache.backends
+  #    - requests_cache.backends.base
+  #    - requests_cache.backends.sqlite
+  #    - requests_cache.policy.actions
+  #    - requests_cache.session
+  #    - trakt.core
+  #    - urllib3.connectionpool
   filter:
 #    # Filter out all messages with level WARNING
 #    - level: WARNING
 #    # Filter out message with level WARNING and containing a text
 #    - level: WARNING
 #      message: "not found on Trakt"
 #    - message: "because provider local has no external Id"
@@ -69,14 +69,16 @@
     watched_status: true
     # If trakt_to_plex watchlist=false and plex_to_trakt watchlist=true
     # the Trakt watchlist will be overwritten by Plex watchlist
     watchlist: true
     # If you prefer to fetch trakt watchlist as a playlist instead of
     # plex watchlist, toggle this to true (is read only if watchlist=true)
     watchlist_as_playlist: false
+    # Sync Play Progress from Trakt to Plex
+    playback_status: false
 
 # settings for 'watch' command
 watch:
   add_collection: false
   remove_collection: false
   # what video watched percentage (0 to 100) triggers the watched status
   scrobble_threshold: 80
@@ -86,30 +88,29 @@
   media_progressbar: true
   # Clients to ignore when listening Play events
   ignore_clients: ~
 
 xbmc-providers:
   movies: imdb
   shows: tvdb
-
 ##### Advanced settings below this line, don't edit unless you know what you're doing #####
 #http_cache:
-  # https://requests-cache.readthedocs.io/en/main/user_guide/expiration.html#url-patterns
-  # https://requests-cache.readthedocs.io/en/main/user_guide/expiration.html#expiration-values
-  #
-  # The value is seconds to cache.
-  # Or one of the following special values:
-  # - DO_NOT_CACHE: Skip both reading from and writing to the cache
-  # - EXPIRE_IMMEDIATELY: Consider the response already expired, but potentially usable
-  # - NEVER_EXPIRE: Store responses indefinitely
-  #
-  # The value can be also suffixed with a time unit:
-  # - 5m, 1h, 3d
-  # See full documentation at:
-  # - https://github.com/wroberts/pytimeparse#pytimeparse-time-expression-parser
-  #
-  # NOTE: If there is more than one match, the first match will be used in the order they are defined
+# https://requests-cache.readthedocs.io/en/main/user_guide/expiration.html#url-patterns
+# https://requests-cache.readthedocs.io/en/main/user_guide/expiration.html#expiration-values
+#
+# The value is seconds to cache.
+# Or one of the following special values:
+# - DO_NOT_CACHE: Skip both reading from and writing to the cache
+# - EXPIRE_IMMEDIATELY: Consider the response already expired, but potentially usable
+# - NEVER_EXPIRE: Store responses indefinitely
+#
+# The value can be also suffixed with a time unit:
+# - 5m, 1h, 3d
+# See full documentation at:
+# - https://github.com/wroberts/pytimeparse#pytimeparse-time-expression-parser
+#
+# NOTE: If there is more than one match, the first match will be used in the order they are defined
 #  policy:
 #    "*.trakt.tv/users/me": 1d
 #    "*.trakt.tv/users/likes/lists": DO_NOT_CACHE
 
 # vim:ts=2:sw=2:et
```

### Comparing `PlexTraktSync-0.29.9/plextraktsync/decorators/rate_limit.py` & `plextraktsync-0.30.0/plextraktsync/decorators/rate_limit.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/decorators/retry.py` & `plextraktsync-0.30.0/plextraktsync/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/logger/filter.py` & `plextraktsync-0.30.0/plextraktsync/logger/filter.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/logger/init.py` & `plextraktsync-0.30.0/plextraktsync/logger/init.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/media/Media.py` & `plextraktsync-0.30.0/plextraktsync/media/Media.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from functools import cached_property
 from typing import TYPE_CHECKING
 
+from trakt.sync import PlaybackEntry
 from trakt.tv import TVShow
 
 from plextraktsync.mixin.RichMarkup import RichMarkup
 from plextraktsync.trakt.TraktLookup import TraktLookup
 
 if TYPE_CHECKING:
     from plextraktsync.media.MediaFactory import MediaFactory
@@ -35,14 +36,23 @@
         self.plex_api = plex_api
         self.trakt_api = trakt_api
         self.mf = mf
         self.plex = plex
         self.trakt = trakt
         self._show = None
 
+    def __eq__(self, other):
+        if isinstance(other, PlaybackEntry):
+            return self.type == other.type and self.trakt_id == other.trakt
+
+        return False
+
+    def __hash__(self):
+        return hash((self.type, self.plex, self.trakt))
+
     @property
     def title(self):
         if self.plex:
             return self.plex.title
 
         return f"{self.trakt.title} ({self.trakt.year})"
 
@@ -211,19 +221,15 @@
 
     @cached_property
     def trakt_rating(self):
         return self.trakt_api.rating(self.trakt)
 
     @cached_property
     def plex_rating(self):
-        if self.media_type == "episodes" and not self.plex.is_discover and self.show:
-            show_id = self.show.plex.item.ratingKey
-        else:
-            show_id = None
-        return self.plex.rating(show_id)
+        return self.plex.rating()
 
     def trakt_rate(self):
         rating = self.plex_rating
         if rating is None:
             return
         self.trakt_api.rate(self.trakt, rating.rating, rating.rated_at)
```

### Comparing `PlexTraktSync-0.29.9/plextraktsync/media/MediaFactory.py` & `plextraktsync-0.30.0/plextraktsync/media/MediaFactory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/mixin/ChangeNotifier.py` & `plextraktsync-0.30.0/plextraktsync/mixin/ChangeNotifier.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/plan/WalkConfig.py` & `plextraktsync-0.30.0/plextraktsync/plan/WalkConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         # Single item provided
         if self.library or self.movie or self.show or self.id:
             return True
 
         # Must sync both movies and shows to be full sync
         return not self.walk_movies or not self.walk_shows
 
+    @property
     def is_valid(self):
         # Single item provided
         if self.library or self.movie or self.show or self.id:
             return True
 
         # Full sync of movies or shows
         if self.walk_movies or self.walk_shows:
```

### Comparing `PlexTraktSync-0.29.9/plextraktsync/plan/WalkPlanner.py` & `plextraktsync-0.30.0/plextraktsync/plan/WalkPlanner.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/plan/Walker.py` & `plextraktsync-0.30.0/plextraktsync/plan/Walker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/plex/PlexApi.py` & `plextraktsync-0.30.0/plextraktsync/plex/PlexApi.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/plex/PlexAudioCodec.py` & `plextraktsync-0.30.0/plextraktsync/plex/PlexAudioCodec.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuid.py` & `plextraktsync-0.30.0/plextraktsync/plex/PlexGuid.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuidProvider.py` & `plextraktsync-0.30.0/plextraktsync/plex/PlexGuidProvider.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuidProviderMbid.py` & `plextraktsync-0.30.0/plextraktsync/plex/PlexGuidProviderMbid.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/plex/PlexGuidProviderTMDB.py` & `plextraktsync-0.30.0/plextraktsync/plex/PlexGuidProviderTMDB.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/plex/PlexId.py` & `plextraktsync-0.30.0/plextraktsync/plex/PlexId.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/plex/PlexIdFactory.py` & `plextraktsync-0.30.0/plextraktsync/plex/PlexIdFactory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/plex/PlexLibraryItem.py` & `plextraktsync-0.30.0/plextraktsync/plex/PlexLibraryItem.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,30 +131,37 @@
     def edition_title(self):
         if self.type == "movie":
             # Use __dict__ access to prevent reloads
             return self.item.__dict__.get("editionTitle")
         return None
 
     @cached_property
+    def year(self):
+        if self.type == "artist":
+            return None
+
+        return self.item.__dict__.get("year")
+
+    @cached_property
     def title(self):
         value = self.item.title
         if self.type == "movie" and self.edition_title:
             value = f"{value} ({self.edition_title})"
 
         if self.type == "episode":
             value = f"{self.item.grandparentTitle}/{self.item.seasonEpisode}/{value}"
 
-        if self.type != "artist" and self.item.year:
-            value = f"{value} ({self.item.year})"
+        if self.year:
+            value = f"{value} ({self.year})"
 
         return value
 
-    def rating(self, show_id: int = None):
+    def rating(self):
         if not self.is_discover and self.plex is not None:
-            return self.plex.ratings.get(self, show_id)
+            return self.plex.ratings.get(self)
 
         return Rating.create(self.item.userRating, self.item.lastRatedAt)
 
     @property
     def seen_date(self):
         return self.date_value(self.item.lastViewedAt)
 
@@ -303,14 +310,20 @@
 
         return None
 
     def watch_progress(self, view_offset):
         percent = view_offset / self.item.duration * 100
         return percent
 
+    def progress_millis(self, percentage: float):
+        """
+        Get Movie progress from percentage to milliseconds
+        """
+        return int((percentage / 100) * self.item.duration)
+
     def episodes(self):
         for ep in self._get_episodes():
             yield PlexLibraryItem(ep, plex=self.plex)
 
     @retry()
     def _get_episodes(self):
         if self.type == "season":
```

### Comparing `PlexTraktSync-0.29.9/plextraktsync/plex/PlexLibrarySection.py` & `plextraktsync-0.30.0/plextraktsync/plex/PlexLibrarySection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/plex/PlexPlaylist.py` & `plextraktsync-0.30.0/plextraktsync/plex/PlexPlaylist.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/plex/PlexSectionPager.py` & `plextraktsync-0.30.0/plextraktsync/plex/PlexSectionPager.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/plex/PlexServerConnection.py` & `plextraktsync-0.30.0/plextraktsync/plex/PlexServerConnection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/plex/PlexWatchList.py` & `plextraktsync-0.30.0/plextraktsync/plex/PlexWatchList.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/plex/SessionCollection.py` & `plextraktsync-0.30.0/plextraktsync/plex/SessionCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/pytrakt_extensions.py` & `plextraktsync-0.30.0/plextraktsync/pytrakt_extensions.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/queue/BackgroundTask.py` & `plextraktsync-0.30.0/plextraktsync/queue/BackgroundTask.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/queue/Queue.py` & `plextraktsync-0.30.0/plextraktsync/queue/Queue.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/queue/TraktBatchWorker.py` & `plextraktsync-0.30.0/plextraktsync/queue/TraktBatchWorker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/queue/TraktMarkWatchedWorker.py` & `plextraktsync-0.30.0/plextraktsync/queue/TraktMarkWatchedWorker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/queue/TraktScrobbleWorker.py` & `plextraktsync-0.30.0/plextraktsync/queue/TraktScrobbleWorker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
+from trakt.errors import ConflictException
+
 from plextraktsync.decorators.rate_limit import rate_limit
 from plextraktsync.decorators.retry import retry
 from plextraktsync.decorators.time_limit import time_limit
 from plextraktsync.factory import logging
 
 if TYPE_CHECKING:
     from trakt.sync import Scrobbler
@@ -27,40 +29,34 @@
             items = queues[name]
             if not len(items):
                 continue
             self.submit(name, items)
             queues[name].clear()
 
     def submit(self, name, items):
-        method = getattr(self, name)
+        name = name.replace("scrobble_", "")
         results = []
         for scrobbler, progress in self.normalize(items).items():
-            res = method(scrobbler, progress)
+            res = self.scrobble(scrobbler, name, progress)
             results.append(res)
 
         if results:
             self.logger.debug(f"Submitted {name}: {results}")
 
     @rate_limit()
     @time_limit()
     @retry()
-    def scrobble_update(self, scrobbler: Scrobbler, progress: float):
-        return scrobbler.update(progress)
-
-    @rate_limit()
-    @time_limit()
-    @retry()
-    def scrobble_pause(self, scrobbler: Scrobbler, progress: float):
-        return scrobbler.pause(progress)
-
-    @rate_limit()
-    @time_limit()
-    @retry()
-    def scrobble_stop(self, scrobbler: Scrobbler, progress: float):
-        return scrobbler.stop(progress)
+    def scrobble(self, scrobbler: Scrobbler, name: str, progress: float):
+        method = getattr(scrobbler, name)
+        try:
+            return method(progress)
+        except ConflictException as e:
+            self.logger.error(e)
+            self.logger.debug(e.response.headers)
+            self.logger.debug(e.response)
 
     @staticmethod
     def normalize(items: list[TraktPlayable]):
         result = {}
         for scrobbler, progress in items:
             result[scrobbler] = progress
```

### Comparing `PlexTraktSync-0.29.9/plextraktsync/rich/RichHighlighter.py` & `plextraktsync-0.30.0/plextraktsync/rich/RichHighlighter.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/rich/RichProgressBar.py` & `plextraktsync-0.30.0/plextraktsync/rich/RichProgressBar.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/trakt/ScrobblerCollection.py` & `plextraktsync-0.30.0/plextraktsync/trakt/ScrobblerCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/trakt/ScrobblerProxy.py` & `plextraktsync-0.30.0/plextraktsync/trakt/ScrobblerProxy.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/trakt/TraktApi.py` & `plextraktsync-0.30.0/plextraktsync/trakt/TraktApi.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from plextraktsync.decorators.retry import retry
 from plextraktsync.decorators.time_limit import time_limit
 from plextraktsync.factory import factory, logging
 from plextraktsync.path import pytrakt_file
 from plextraktsync.trakt.PartialTraktMedia import PartialTraktMedia
 from plextraktsync.trakt.TraktLookup import TraktLookup
 from plextraktsync.trakt.TraktRatingCollection import TraktRatingCollection
+from plextraktsync.trakt.WatchProgress import WatchProgress
 from plextraktsync.util.Rating import Rating
 
 if TYPE_CHECKING:
     from trakt.movies import Movie
     from trakt.tv import TVEpisode, TVShow
 
     from plextraktsync.plex.PlexGuid import PlexGuid
@@ -63,14 +64,19 @@
 
     @cached_property
     @rate_limit()
     @retry()
     @flatten_list
     def liked_lists(self) -> list[TraktLikedList]:
         for item in self.me.get_liked_lists("lists", limit=1000):
+            # Skip private lists
+            # https://github.com/Taxel/PlexTraktSync/issues/1864#issuecomment-2018171311
+            if item["list"]["privacy"] == "private":
+                self.logger.warning(f"Skipping private list: {item['list']['name']} - {item['list']['share_link']}")
+                continue
             tll: TraktLikedList = {
                 "listname": item["list"]["name"],
                 "listid": item["list"]["ids"]["trakt"],
             }
             yield tll
 
     @cached_property
@@ -78,14 +84,20 @@
     @retry()
     def watched_movies(self):
         return set(map(lambda m: m.trakt, self.me.watched_movies))
 
     @cached_property
     @rate_limit()
     @retry()
+    def watch_progress(self):
+        return WatchProgress(trakt.sync.get_playback())
+
+    @cached_property
+    @rate_limit()
+    @retry()
     def movie_collection(self):
         return self.me.movie_collection
 
     @property
     @rate_limit()
     @retry()
     def show_collection(self):
```

### Comparing `PlexTraktSync-0.29.9/plextraktsync/trakt/TraktLookup.py` & `plextraktsync-0.30.0/plextraktsync/trakt/TraktLookup.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/trakt/TraktRatingCollection.py` & `plextraktsync-0.30.0/plextraktsync/trakt/TraktRatingCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/trakt/TraktUserList.py` & `plextraktsync-0.30.0/plextraktsync/trakt/TraktUserList.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/trakt/TraktUserListCollection.py` & `plextraktsync-0.30.0/plextraktsync/trakt/TraktUserListCollection.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,14 +10,18 @@
     from plextraktsync.media.Media import Media
     from plextraktsync.trakt.types import TraktLikedList, TraktPlayable
 
 
 class TraktUserListCollection(UserList):
     logger = logging.getLogger(__name__)
 
+    @property
+    def is_empty(self):
+        return not len(self)
+
     def add_to_lists(self, m: Media):
         # Skip movie editions
         # https://support.plex.tv/articles/multiple-editions/#:~:text=Do%20Multiple%20Editions%20work%20with%20watch%20state%20syncing%3F
         if m.plex.edition_title is not None:
             return
         for tl in self:
             tl.add(m)
```

### Comparing `PlexTraktSync-0.29.9/plextraktsync/trakt/TraktWatchlist.py` & `plextraktsync-0.30.0/plextraktsync/trakt/TraktWatchlist.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/util/Factory.py` & `plextraktsync-0.30.0/plextraktsync/util/Factory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/util/Path.py` & `plextraktsync-0.30.0/plextraktsync/util/Path.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/util/Rating.py` & `plextraktsync-0.30.0/plextraktsync/util/Rating.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/util/Timer.py` & `plextraktsync-0.30.0/plextraktsync/util/Timer.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/util/Version.py` & `plextraktsync-0.30.0/plextraktsync/util/Version.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/util/local_url.py` & `plextraktsync-0.30.0/plextraktsync/util/local_url.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/util/openurl.py` & `plextraktsync-0.30.0/plextraktsync/util/openurl.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/util/packaging.py` & `plextraktsync-0.30.0/plextraktsync/util/packaging.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/util/remove_empty_values.py` & `plextraktsync-0.30.0/plextraktsync/util/remove_empty_values.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/watch/EventDispatcher.py` & `plextraktsync-0.30.0/plextraktsync/watch/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/watch/EventFactory.py` & `plextraktsync-0.30.0/plextraktsync/watch/EventFactory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/watch/ProgressBar.py` & `plextraktsync-0.30.0/plextraktsync/watch/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/watch/WatchStateUpdater.py` & `plextraktsync-0.30.0/plextraktsync/watch/WatchStateUpdater.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/watch/WebSocketListener.py` & `plextraktsync-0.30.0/plextraktsync/watch/WebSocketListener.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/plextraktsync/watch/events.py` & `plextraktsync-0.30.0/plextraktsync/watch/events.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/requirements.txt` & `plextraktsync-0.30.0/requirements.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 attrs==23.2.0; python_version >= '3.7'
 cattrs==23.2.3; python_version >= '3.7' and python_version >= '3.8'
 certifi==2024.2.2; python_version >= '3.6'
 charset-normalizer==3.3.2; python_full_version >= '3.7.0'
 click==8.1.7; python_version >= '3.7'
 deprecated==1.2.14; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
-idna==3.6; python_version >= '3.5'
+exceptiongroup==1.2.0; python_version < '3.11'
+humanize==4.9.0; python_version >= '3.8'
+idna==3.7; python_version >= '3.5'
 inquirerpy==0.3.4; python_version >= '3.7' and python_version < '4.0'
 markdown-it-py==3.0.0; python_version >= '3.7' and python_version >= '3.8'
 mdurl==0.1.2; python_version >= '3.7'
 oauthlib==3.2.2; python_version >= '3.6'
 pfzy==0.3.4; python_version >= '3.7' and python_version < '4.0'
 platformdirs==4.2.0; python_version >= '3.7' and python_version >= '3.8'
-plexapi==4.15.10; python_version >= '3.8'
+plexapi==4.15.11; python_version >= '3.8'
+pluggy==1.4.0; python_version >= '3.8'
 prompt-toolkit==3.0.43; python_full_version >= '3.7.0'
 pygments==2.17.2; python_version >= '3.7'
 python-dotenv==1.0.1; python_version >= '3.8'
 python-git-info==0.8.3
 pytimeparse==1.1.8
-pytrakt==3.4.31
+pytrakt==3.4.32
 pyyaml==6.0.1; python_version >= '3.6'
 requests==2.31.0; python_version >= '3.7'
 requests-cache==1.2.0; python_version >= '3.8'
-requests-oauthlib==1.4.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
+requests-oauthlib==2.0.0; python_version >= '3.4'
 rich==13.7.1; python_full_version >= '3.7.0'
 six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3' and python_version >= '3.4'
 tqdm==4.66.2; python_version >= '3.7'
+typing-extensions==4.11.0; python_version < '3.11'
 url-normalize==1.4.3; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5' and python_version >= '3.6'
 urllib3==2.2.1; python_version >= '3.8'
 wcwidth==0.2.13
 websocket-client==1.7.0; python_version >= '3.8'
 wrapt==1.16.0; python_version >= '3.5' and python_version >= '3.6'
```

### Comparing `PlexTraktSync-0.29.9/setup.cfg` & `plextraktsync-0.30.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -28,17 +28,19 @@
 	plextraktsync.config
 	plextraktsync.decorators
 	plextraktsync.logger
 	plextraktsync.media
 	plextraktsync.mixin
 	plextraktsync.plan
 	plextraktsync.plex
+	plextraktsync.plugin
 	plextraktsync.queue
 	plextraktsync.rich
 	plextraktsync.sync
+	plextraktsync.sync.plugin
 	plextraktsync.trakt
 	plextraktsync.util
 	plextraktsync.watch
 python_requires = >=3.8
 include_package_data = True
 
 [options.packages.find]
```

### Comparing `PlexTraktSync-0.29.9/tests/test_collection_metadata.py` & `plextraktsync-0.30.0/tests/test_collection_metadata.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/tests/test_config.py` & `plextraktsync-0.30.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/tests/test_events.py` & `plextraktsync-0.30.0/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/tests/test_new_agent.py` & `plextraktsync-0.30.0/tests/test_new_agent.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/tests/test_plex_id.py` & `plextraktsync-0.30.0/tests/test_plex_id.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/tests/test_rating.py` & `plextraktsync-0.30.0/tests/test_rating.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/tests/test_timer.py` & `plextraktsync-0.30.0/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/tests/test_trakt_progress.py` & `plextraktsync-0.30.0/tests/test_trakt_progress.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/tests/test_tv_lookup.py` & `plextraktsync-0.30.0/tests/test_tv_lookup.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.29.9/tests/test_walker.py` & `plextraktsync-0.30.0/tests/test_walker.py`

 * *Files identical despite different names*

