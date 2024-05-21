# Comparing `tmp/plextraktsync-0.30.8.tar.gz` & `tmp/plextraktsync-0.30.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plextraktsync-0.30.8.tar", last modified: Thu May 16 15:41:21 2024, max compression
+gzip compressed data, was "plextraktsync-0.30.9.tar", last modified: Tue May 21 19:04:55 2024, max compression
```

## Comparing `plextraktsync-0.30.8.tar` & `plextraktsync-0.30.9.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.065047 plextraktsync-0.30.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    30195 2024-05-16 15:41:21.065047 plextraktsync-0.30.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.065047 plextraktsync-0.30.8/PlexTraktSync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    30195 2024-05-16 15:41:21.000000 plextraktsync-0.30.8/PlexTraktSync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-16 15:41:21.000000 plextraktsync-0.30.8/PlexTraktSync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:41:21.000000 plextraktsync-0.30.8/PlexTraktSync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-16 15:41:21.000000 plextraktsync-0.30.8/PlexTraktSync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-16 15:41:21.000000 plextraktsync-0.30.8/PlexTraktSync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 15:41:21.000000 plextraktsync-0.30.8/PlexTraktSync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26819 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.037047 plextraktsync-0.30.8/plextraktsync/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.041047 plextraktsync-0.30.8/plextraktsync/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/commands/bug_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/commands/clear_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/commands/imdb_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/commands/plex_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/commands/self_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/commands/trakt_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/commands/unmatched.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/commands/watch.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/commands/watched_shows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.041047 plextraktsync-0.30.8/plextraktsync/config/
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/config/ConfigLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/config/ConfigMergeMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/config/HttpCacheConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/config/PlexServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/config/RunConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/config/ServerConfigFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/config/SyncConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/config.default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.045047 plextraktsync-0.30.8/plextraktsync/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/decorators/coro.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/decorators/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/decorators/measure_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/decorators/memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/decorators/nocache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/decorators/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/decorators/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/decorators/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.045047 plextraktsync-0.30.8/plextraktsync/logger/
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/logger/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/logger/init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.045047 plextraktsync-0.30.8/plextraktsync/media/
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/media/Media.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/media/MediaFactory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.045047 plextraktsync-0.30.8/plextraktsync/mixin/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/mixin/ChangeNotifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/mixin/RichMarkup.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/mixin/SetWindowTitle.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.045047 plextraktsync-0.30.8/plextraktsync/plan/
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plan/WalkConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plan/WalkPlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plan/WalkPlanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plan/Walker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.049047 plextraktsync-0.30.8/plextraktsync/plex/
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/PlexApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/PlexAudioCodec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/PlexGuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/PlexGuidProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/PlexGuidProviderIMDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/PlexGuidProviderLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/PlexGuidProviderMbid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/PlexGuidProviderTMDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/PlexGuidProviderTVDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/PlexId.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/PlexIdFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/PlexLibraryItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/PlexLibrarySection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/PlexPlaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/PlexPlaylistCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/PlexRatings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/PlexSectionPager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/PlexServerConnection.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/PlexWatchList.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/SessionCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plex/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.049047 plextraktsync-0.30.8/plextraktsync/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/pytrakt_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.053047 plextraktsync-0.30.8/plextraktsync/queue/
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/queue/BackgroundTask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/queue/Queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/queue/TraktBatchWorker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/queue/TraktMarkWatchedWorker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/queue/TraktScrobbleWorker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.053047 plextraktsync-0.30.8/plextraktsync/rich/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/rich/RichHighlighter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/rich/RichProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/style.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.053047 plextraktsync-0.30.8/plextraktsync/sync/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/sync/AddCollectionPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/sync/ClearCollectedPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/sync/LikedListsPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/sync/Sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/sync/SyncRatingsPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/sync/SyncWatchedPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/sync/TraktListsPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/sync/WatchListPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/sync/WatchProgressPlugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.053047 plextraktsync-0.30.8/plextraktsync/sync/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/sync/plugin/SyncPluginInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/sync/plugin/SyncPluginManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/sync/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.057047 plextraktsync-0.30.8/plextraktsync/trakt/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/trakt/PartialTraktMedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/trakt/ScrobblerCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/trakt/ScrobblerProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/trakt/TraktApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/trakt/TraktItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/trakt/TraktLookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/trakt/TraktRatingCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/trakt/TraktUserList.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/trakt/TraktUserListCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/trakt/TraktWatchlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/trakt/WatchProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/trakt/trakt_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/trakt/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.061047 plextraktsync-0.30.8/plextraktsync/util/
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/util/Factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/util/Path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/util/Rating.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/util/Timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/util/Version.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/util/execp.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/util/execx.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/util/expand_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/util/git_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/util/local_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/util/openurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/util/packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/util/parse_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/util/remove_empty_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.061047 plextraktsync-0.30.8/plextraktsync/watch/
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/watch/EventDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/watch/EventFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/watch/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/watch/WatchStateUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/watch/WebSocketListener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/plextraktsync/watch/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-16 15:41:18.000000 plextraktsync-0.30.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-16 15:41:21.065047 plextraktsync-0.30.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:21.061047 plextraktsync-0.30.8/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1964 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/tests/test_collection_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1499 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2703 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/tests/test_events.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/tests/test_logger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      977 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/tests/test_new_agent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2104 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/tests/test_plex_id.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      224 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/tests/test_plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/tests/test_rating.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      503 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/tests/test_threading.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1174 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/tests/test_timer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      627 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/tests/test_trakt_progress.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3762 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/tests/test_tv_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-05-16 15:41:17.000000 plextraktsync-0.30.8/tests/test_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.995172 plextraktsync-0.30.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    30195 2024-05-21 19:04:54.995172 plextraktsync-0.30.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.995172 plextraktsync-0.30.9/PlexTraktSync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    30195 2024-05-21 19:04:54.000000 plextraktsync-0.30.9/PlexTraktSync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-21 19:04:54.000000 plextraktsync-0.30.9/PlexTraktSync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:04:54.000000 plextraktsync-0.30.9/PlexTraktSync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-21 19:04:54.000000 plextraktsync-0.30.9/PlexTraktSync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-21 19:04:54.000000 plextraktsync-0.30.9/PlexTraktSync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 19:04:54.000000 plextraktsync-0.30.9/PlexTraktSync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26819 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.971171 plextraktsync-0.30.9/plextraktsync/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 19:04:51.000000 plextraktsync-0.30.9/plextraktsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.975171 plextraktsync-0.30.9/plextraktsync/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/commands/bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/commands/clear_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/commands/imdb_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/commands/plex_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/commands/self_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/commands/trakt_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/commands/unmatched.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/commands/watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/commands/watched_shows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.975171 plextraktsync-0.30.9/plextraktsync/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/config/ConfigLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/config/ConfigMergeMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/config/HttpCacheConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/config/PlexServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/config/RunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/config/ServerConfigFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/config/SyncConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/config.default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.975171 plextraktsync-0.30.9/plextraktsync/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/decorators/coro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/decorators/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/decorators/measure_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/decorators/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/decorators/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/decorators/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/decorators/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/decorators/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.979172 plextraktsync-0.30.9/plextraktsync/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/logger/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/logger/init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.979172 plextraktsync-0.30.9/plextraktsync/media/
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/media/Media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/media/MediaFactory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.979172 plextraktsync-0.30.9/plextraktsync/mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/mixin/ChangeNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/mixin/RichMarkup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/mixin/SetWindowTitle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.979172 plextraktsync-0.30.9/plextraktsync/plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plan/WalkConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plan/WalkPlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plan/WalkPlanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plan/Walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.983172 plextraktsync-0.30.9/plextraktsync/plex/
+-rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/PlexApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/PlexAudioCodec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/PlexGuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/PlexGuidProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/PlexGuidProviderIMDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/PlexGuidProviderLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/PlexGuidProviderMbid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/PlexGuidProviderTMDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/PlexGuidProviderTVDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/PlexId.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/PlexIdFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/PlexLibraryItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/PlexLibrarySection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/PlexPlaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/PlexPlaylistCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/PlexRatings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/PlexSectionPager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/PlexServerConnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/PlexWatchList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/SessionCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plex/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.983172 plextraktsync-0.30.9/plextraktsync/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/pytrakt_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.983172 plextraktsync-0.30.9/plextraktsync/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/queue/BackgroundTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/queue/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/queue/TraktBatchWorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/queue/TraktMarkWatchedWorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/queue/TraktScrobbleWorker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.983172 plextraktsync-0.30.9/plextraktsync/rich/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/rich/RichHighlighter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/rich/RichProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/style.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.987172 plextraktsync-0.30.9/plextraktsync/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/sync/AddCollectionPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/sync/ClearCollectedPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/sync/LikedListsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/sync/Sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/sync/SyncRatingsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/sync/SyncWatchedPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/sync/TraktListsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/sync/WatchListPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/sync/WatchProgressPlugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.987172 plextraktsync-0.30.9/plextraktsync/sync/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/sync/plugin/SyncPluginInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/sync/plugin/SyncPluginManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/sync/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.987172 plextraktsync-0.30.9/plextraktsync/trakt/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/trakt/PartialTraktMedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/trakt/ScrobblerCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/trakt/ScrobblerProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10978 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/trakt/TraktApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/trakt/TraktItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/trakt/TraktLookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/trakt/TraktRatingCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/trakt/TraktUserList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/trakt/TraktUserListCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/trakt/TraktWatchlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/trakt/WatchProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/trakt/trakt_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/trakt/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.991172 plextraktsync-0.30.9/plextraktsync/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/util/Factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/util/Path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/util/Rating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/util/Timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/util/Version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/util/execp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/util/execx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/util/expand_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/util/git_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/util/local_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/util/openurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/util/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/util/parse_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/util/remove_empty_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.991172 plextraktsync-0.30.9/plextraktsync/watch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/watch/EventDispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/watch/EventFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/watch/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/watch/WatchStateUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/watch/WebSocketListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/plextraktsync/watch/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-21 19:04:52.000000 plextraktsync-0.30.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-21 19:04:54.995172 plextraktsync-0.30.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:04:54.991172 plextraktsync-0.30.9/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1964 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/tests/test_collection_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1499 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2703 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/tests/test_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/tests/test_logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      977 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/tests/test_new_agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2104 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/tests/test_plex_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      224 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/tests/test_plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/tests/test_rating.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      503 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/tests/test_threading.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1174 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/tests/test_timer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      627 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/tests/test_trakt_progress.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3762 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/tests/test_tv_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-05-21 19:04:50.000000 plextraktsync-0.30.9/tests/test_walker.py
```

### Comparing `plextraktsync-0.30.8/LICENSE` & `plextraktsync-0.30.9/LICENSE`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/PKG-INFO` & `plextraktsync-0.30.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.30.8
+Version: 0.30.9
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,24 +31,24 @@
 Requires-Dist: idna==3.7; python_version >= "3.5"
 Requires-Dist: inquirerpy==0.3.4; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: mdurl==0.1.2; python_version >= "3.7"
 Requires-Dist: oauthlib==3.2.2; python_version >= "3.6"
 Requires-Dist: pfzy==0.3.4; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: platformdirs==4.2.2; python_version >= "3.8"
-Requires-Dist: plexapi==4.15.12; python_version >= "3.8"
+Requires-Dist: plexapi==4.15.13; python_version >= "3.8"
 Requires-Dist: pluggy==1.5.0; python_version >= "3.8"
 Requires-Dist: prompt-toolkit==3.0.43; python_full_version >= "3.7.0"
 Requires-Dist: pygments==2.18.0; python_version >= "3.8"
 Requires-Dist: python-dotenv==1.0.1; python_version >= "3.8"
 Requires-Dist: python-git-info==0.8.3
 Requires-Dist: pytimeparse==1.1.8
 Requires-Dist: pytrakt==3.4.32
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6"
-Requires-Dist: requests==2.31.0; python_version >= "3.7"
+Requires-Dist: requests==2.32.0; python_version >= "3.8"
 Requires-Dist: requests-cache==1.2.0; python_version >= "3.8"
 Requires-Dist: requests-oauthlib==2.0.0; python_version >= "3.4"
 Requires-Dist: rich==13.7.1; python_full_version >= "3.7.0"
 Requires-Dist: six==1.16.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3" and python_version >= "3.4"
 Requires-Dist: tqdm==4.66.4; python_version >= "3.7"
 Requires-Dist: types-decorator==5.1.8.20240310; python_version >= "3.8"
 Requires-Dist: typing-extensions==4.11.0; python_version < "3.9"
```

### Comparing `plextraktsync-0.30.8/PlexTraktSync.egg-info/PKG-INFO` & `plextraktsync-0.30.9/PlexTraktSync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.30.8
+Version: 0.30.9
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,24 +31,24 @@
 Requires-Dist: idna==3.7; python_version >= "3.5"
 Requires-Dist: inquirerpy==0.3.4; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: mdurl==0.1.2; python_version >= "3.7"
 Requires-Dist: oauthlib==3.2.2; python_version >= "3.6"
 Requires-Dist: pfzy==0.3.4; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: platformdirs==4.2.2; python_version >= "3.8"
-Requires-Dist: plexapi==4.15.12; python_version >= "3.8"
+Requires-Dist: plexapi==4.15.13; python_version >= "3.8"
 Requires-Dist: pluggy==1.5.0; python_version >= "3.8"
 Requires-Dist: prompt-toolkit==3.0.43; python_full_version >= "3.7.0"
 Requires-Dist: pygments==2.18.0; python_version >= "3.8"
 Requires-Dist: python-dotenv==1.0.1; python_version >= "3.8"
 Requires-Dist: python-git-info==0.8.3
 Requires-Dist: pytimeparse==1.1.8
 Requires-Dist: pytrakt==3.4.32
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6"
-Requires-Dist: requests==2.31.0; python_version >= "3.7"
+Requires-Dist: requests==2.32.0; python_version >= "3.8"
 Requires-Dist: requests-cache==1.2.0; python_version >= "3.8"
 Requires-Dist: requests-oauthlib==2.0.0; python_version >= "3.4"
 Requires-Dist: rich==13.7.1; python_full_version >= "3.7.0"
 Requires-Dist: six==1.16.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3" and python_version >= "3.4"
 Requires-Dist: tqdm==4.66.4; python_version >= "3.7"
 Requires-Dist: types-decorator==5.1.8.20240310; python_version >= "3.8"
 Requires-Dist: typing-extensions==4.11.0; python_version < "3.9"
```

### Comparing `plextraktsync-0.30.8/PlexTraktSync.egg-info/SOURCES.txt` & `plextraktsync-0.30.9/PlexTraktSync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/PlexTraktSync.egg-info/requires.txt` & `plextraktsync-0.30.9/PlexTraktSync.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -38,30 +38,30 @@
 oauthlib==3.2.2
 pyyaml==6.0.1
 
 [:python_version >= "3.7"]
 attrs==23.2.0
 click==8.1.7
 mdurl==0.1.2
-requests==2.31.0
 tqdm==4.66.4
 
 [:python_version >= "3.7" and python_version < "4.0"]
 inquirerpy==0.3.4
 pfzy==0.3.4
 
 [:python_version >= "3.7" and python_version >= "3.8"]
 cattrs==23.2.3
 markdown-it-py==3.0.0
 
 [:python_version >= "3.8"]
 apluggy==0.9.4
 humanize==4.9.0
 platformdirs==4.2.2
-plexapi==4.15.12
+plexapi==4.15.13
 pluggy==1.5.0
 pygments==2.18.0
 python-dotenv==1.0.1
+requests==2.32.0
 requests-cache==1.2.0
 types-decorator==5.1.8.20240310
 urllib3==2.2.1
 websocket-client==1.8.0
```

### Comparing `plextraktsync-0.30.8/README.md` & `plextraktsync-0.30.9/README.md`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/cli.py` & `plextraktsync-0.30.9/plextraktsync/cli.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/commands/bug_report.py` & `plextraktsync-0.30.9/plextraktsync/commands/bug_report.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/commands/cache.py` & `plextraktsync-0.30.9/plextraktsync/commands/cache.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/commands/clear_collections.py` & `plextraktsync-0.30.9/plextraktsync/commands/clear_collections.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/commands/config.py` & `plextraktsync-0.30.9/plextraktsync/commands/config.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/commands/download.py` & `plextraktsync-0.30.9/plextraktsync/commands/download.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/commands/imdb_import.py` & `plextraktsync-0.30.9/plextraktsync/commands/imdb_import.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/commands/info.py` & `plextraktsync-0.30.9/plextraktsync/commands/info.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/commands/inspect.py` & `plextraktsync-0.30.9/plextraktsync/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/commands/login.py` & `plextraktsync-0.30.9/plextraktsync/commands/login.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/commands/plex_login.py` & `plextraktsync-0.30.9/plextraktsync/commands/plex_login.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/commands/self_update.py` & `plextraktsync-0.30.9/plextraktsync/commands/self_update.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/commands/sync.py` & `plextraktsync-0.30.9/plextraktsync/commands/sync.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/commands/trakt_login.py` & `plextraktsync-0.30.9/plextraktsync/commands/trakt_login.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/commands/unmatched.py` & `plextraktsync-0.30.9/plextraktsync/commands/unmatched.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/commands/watch.py` & `plextraktsync-0.30.9/plextraktsync/commands/watch.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/commands/watched_shows.py` & `plextraktsync-0.30.9/plextraktsync/commands/watched_shows.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/config/Config.py` & `plextraktsync-0.30.9/plextraktsync/config/Config.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/config/ConfigLoader.py` & `plextraktsync-0.30.9/plextraktsync/config/ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/config/HttpCacheConfig.py` & `plextraktsync-0.30.9/plextraktsync/config/HttpCacheConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/config/PlexServerConfig.py` & `plextraktsync-0.30.9/plextraktsync/config/PlexServerConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/config/ServerConfigFactory.py` & `plextraktsync-0.30.9/plextraktsync/config/ServerConfigFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/config/SyncConfig.py` & `plextraktsync-0.30.9/plextraktsync/config/SyncConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/config.default.yml` & `plextraktsync-0.30.9/plextraktsync/config.default.yml`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/decorators/measure_time.py` & `plextraktsync-0.30.9/plextraktsync/decorators/measure_time.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/decorators/rate_limit.py` & `plextraktsync-0.30.9/plextraktsync/decorators/rate_limit.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/decorators/retry.py` & `plextraktsync-0.30.9/plextraktsync/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/logger/filter.py` & `plextraktsync-0.30.9/plextraktsync/logger/filter.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/logger/init.py` & `plextraktsync-0.30.9/plextraktsync/logger/init.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/media/Media.py` & `plextraktsync-0.30.9/plextraktsync/media/Media.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/media/MediaFactory.py` & `plextraktsync-0.30.9/plextraktsync/media/MediaFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/mixin/ChangeNotifier.py` & `plextraktsync-0.30.9/plextraktsync/mixin/ChangeNotifier.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/plan/WalkConfig.py` & `plextraktsync-0.30.9/plextraktsync/plan/WalkConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/plan/WalkPlanner.py` & `plextraktsync-0.30.9/plextraktsync/plan/WalkPlanner.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/plan/Walker.py` & `plextraktsync-0.30.9/plextraktsync/plan/Walker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/plex/PlexApi.py` & `plextraktsync-0.30.9/plextraktsync/plex/PlexApi.py`

 * *Files 14% similar despite different names*

```diff
@@ -95,14 +95,46 @@
 
     def download(self, m: SubtitleStream | MediaPart, **kwargs):
         url = self.server.url(m.key)
         token = self.server._token
 
         return plexapi.utils.download(url, token, **kwargs)
 
+    def search_by_guid(self, guids: dict, libtype: str):
+        r"""
+                    fetchItem(ekey, guid__regex=r"com\.plexapp\.agents\.(imdb|themoviedb)://|tt\d+")
+                    fetchItem(ekey, guid__id__regex=r"(imdb|tmdb|tvdb)://")
+        """
+
+        from plextraktsync.plex.PlexGuid import PlexGuid
+
+        # Build regex of possible matches
+        keys = "|".join(guids.keys())
+        values = "|".join(map(str, guids.values()))
+        regex = f"({keys})://({values})"
+
+        plexguids = [PlexGuid(f"{k}://{v}", type=libtype) for k, v in guids.items()]
+        sections = self.movie_sections() if libtype == "movie" else None
+        if not sections:
+            raise RuntimeError(f"Not supported search type: {libtype}")
+        results = []
+        for section in sections:
+            result = section.search(libtype=libtype, guid__id__regex=regex)
+            for m in result:
+                pm = PlexLibraryItem(m, self)
+                # Do proper matching with provider type and provider id
+                matched = len([[True for g1 in pm.guids if g1 == g2] for g2 in plexguids])
+                if matched:
+                    results.append(pm)
+
+        if not len(results):
+            return None
+
+        return results
+
     @property
     def version(self):
         return self.server.version
 
     @property
     def updated_at(self):
         return self.server.updatedAt
```

### Comparing `plextraktsync-0.30.8/plextraktsync/plex/PlexAudioCodec.py` & `plextraktsync-0.30.9/plextraktsync/plex/PlexAudioCodec.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/plex/PlexGuid.py` & `plextraktsync-0.30.9/plextraktsync/plex/PlexGuid.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/plex/PlexGuidProvider.py` & `plextraktsync-0.30.9/plextraktsync/plex/PlexGuidProvider.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/plex/PlexGuidProviderMbid.py` & `plextraktsync-0.30.9/plextraktsync/plex/PlexGuidProviderMbid.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/plex/PlexGuidProviderTMDB.py` & `plextraktsync-0.30.9/plextraktsync/plex/PlexGuidProviderTMDB.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/plex/PlexId.py` & `plextraktsync-0.30.9/plextraktsync/plex/PlexId.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/plex/PlexIdFactory.py` & `plextraktsync-0.30.9/plextraktsync/plex/PlexIdFactory.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 
 class PlexIdFactory:
     @classmethod
     def create(cls, key: str | int):
         if isinstance(key, int) or key.isnumeric():
             return PlexId(int(key))
+        elif key.startswith("https://trakt.tv/"):
+            return cls.from_trakt_url(key)
         elif key.startswith("https:") or key.startswith("http:"):
             return cls.from_url(key)
         elif key.startswith("plex://"):
             return cls.from_plex_guid(key)
 
         raise RuntimeError(f"Unable to create PlexId: {key}")
 
@@ -57,7 +59,31 @@
 
         if "filters" in parsed:
             filters = parse_qs(parsed["filters"][0])
             if "metadataItemID" in filters:
                 return PlexId(int(filters["metadataItemID"][0]), server=server)
 
         raise RuntimeError(f"Unable to parse: {url}")
+
+    @classmethod
+    def from_trakt_url(cls, url: str):
+        path = urlparse(url).path
+
+        if path.startswith("/movies/"):
+            media_type = "movie"
+            slug = path[len("/movies/"):]
+        else:
+            from click import ClickException
+            raise ClickException(f"Unable to create PlexId: {path}")
+
+        from plextraktsync.factory import factory
+        from plextraktsync.trakt.TraktItem import TraktItem
+
+        tm = TraktItem(factory.trakt_api.find_by_slug(slug, media_type))
+        results = factory.plex_api.search_by_guid(tm.guids, libtype=tm.type)
+        if results is None:
+            raise RuntimeError(f"Unable to find Plex Match: {url}")
+        if len(results) > 1:
+            raise RuntimeError(f"Failed to find unique match: {url}")
+        pm = results[0]
+
+        return PlexId(pm.key, server=pm.plex.server.machineIdentifier)
```

### Comparing `plextraktsync-0.30.8/plextraktsync/plex/PlexLibraryItem.py` & `plextraktsync-0.30.9/plextraktsync/plex/PlexLibraryItem.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/plex/PlexLibrarySection.py` & `plextraktsync-0.30.9/plextraktsync/plex/PlexLibrarySection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/plex/PlexPlaylist.py` & `plextraktsync-0.30.9/plextraktsync/plex/PlexPlaylist.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/plex/PlexRatings.py` & `plextraktsync-0.30.9/plextraktsync/plex/PlexRatings.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/plex/PlexSectionPager.py` & `plextraktsync-0.30.9/plextraktsync/plex/PlexSectionPager.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/plex/PlexServerConnection.py` & `plextraktsync-0.30.9/plextraktsync/plex/PlexServerConnection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/plex/PlexWatchList.py` & `plextraktsync-0.30.9/plextraktsync/plex/PlexWatchList.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/plex/SessionCollection.py` & `plextraktsync-0.30.9/plextraktsync/plex/SessionCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/pytrakt_extensions.py` & `plextraktsync-0.30.9/plextraktsync/pytrakt_extensions.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/queue/BackgroundTask.py` & `plextraktsync-0.30.9/plextraktsync/queue/BackgroundTask.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/queue/Queue.py` & `plextraktsync-0.30.9/plextraktsync/queue/Queue.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/queue/TraktBatchWorker.py` & `plextraktsync-0.30.9/plextraktsync/queue/TraktBatchWorker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/queue/TraktMarkWatchedWorker.py` & `plextraktsync-0.30.9/plextraktsync/queue/TraktMarkWatchedWorker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/queue/TraktScrobbleWorker.py` & `plextraktsync-0.30.9/plextraktsync/queue/TraktScrobbleWorker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/rich/RichHighlighter.py` & `plextraktsync-0.30.9/plextraktsync/rich/RichHighlighter.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/rich/RichProgressBar.py` & `plextraktsync-0.30.9/plextraktsync/rich/RichProgressBar.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/sync/AddCollectionPlugin.py` & `plextraktsync-0.30.9/plextraktsync/sync/AddCollectionPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/sync/ClearCollectedPlugin.py` & `plextraktsync-0.30.9/plextraktsync/sync/ClearCollectedPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/sync/LikedListsPlugin.py` & `plextraktsync-0.30.9/plextraktsync/sync/LikedListsPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/sync/Sync.py` & `plextraktsync-0.30.9/plextraktsync/sync/Sync.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/sync/SyncRatingsPlugin.py` & `plextraktsync-0.30.9/plextraktsync/sync/SyncRatingsPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/sync/SyncWatchedPlugin.py` & `plextraktsync-0.30.9/plextraktsync/sync/SyncWatchedPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/sync/TraktListsPlugin.py` & `plextraktsync-0.30.9/plextraktsync/sync/TraktListsPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/sync/WatchListPlugin.py` & `plextraktsync-0.30.9/plextraktsync/sync/WatchListPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/sync/WatchProgressPlugin.py` & `plextraktsync-0.30.9/plextraktsync/sync/WatchProgressPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/sync/plugin/SyncPluginInterface.py` & `plextraktsync-0.30.9/plextraktsync/sync/plugin/SyncPluginInterface.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/sync/plugin/SyncPluginManager.py` & `plextraktsync-0.30.9/plextraktsync/sync/plugin/SyncPluginManager.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/trakt/ScrobblerCollection.py` & `plextraktsync-0.30.9/plextraktsync/trakt/ScrobblerCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/trakt/ScrobblerProxy.py` & `plextraktsync-0.30.9/plextraktsync/trakt/ScrobblerProxy.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/trakt/TraktApi.py` & `plextraktsync-0.30.9/plextraktsync/trakt/TraktApi.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from typing import TYPE_CHECKING
 
 import trakt
 import trakt.movies
 import trakt.sync
 import trakt.users
 from click import ClickException
-from trakt.errors import (ForbiddenException, OAuthException,
-                          OAuthRefreshException)
+from trakt.errors import (ForbiddenException, NotFoundException,
+                          OAuthException, OAuthRefreshException)
 
 from plextraktsync import pytrakt_extensions
 from plextraktsync.decorators.flatten import flatten_list
 from plextraktsync.decorators.rate_limit import rate_limit
 from plextraktsync.decorators.retry import retry
 from plextraktsync.decorators.time_limit import time_limit
 from plextraktsync.factory import factory, logging
@@ -253,14 +253,27 @@
             tm = self.search_by_id(guid.id, id_type=guid.provider, media_type=guid.type)
             if tm is None and guid.type == "movie":
                 if self.search_by_id(guid.id, id_type=guid.provider, media_type="show"):
                     self.logger.warning(f"Found match using show search: {guid.title_link}", extra={"markup": True})
 
             return tm
 
+    @staticmethod
+    def find_by_slug(slug: str, media_type: str):
+        if media_type == "movie":
+            from trakt.movies import Movie
+            factory_method = Movie
+        else:
+            raise RuntimeError(f"Unsupported media_type={media_type}")
+
+        try:
+            return factory_method(title=slug, slug=slug)
+        except NotFoundException:
+            raise RuntimeError(f"Unable to find by slug: {slug}")
+
     @rate_limit()
     @retry()
     def search_by_id(self, media_id: str, id_type: str, media_type: str) -> TVShow | Movie | None:
         if id_type == "tvdb" and media_type == "movie":
             # Skip invalid search.
             # The Trakt API states that tvdb is only for shows and episodes:
             # https://trakt.docs.apiary.io/#reference/search/id-lookup/get-id-lookup-results
```

### Comparing `plextraktsync-0.30.8/plextraktsync/trakt/TraktLookup.py` & `plextraktsync-0.30.9/plextraktsync/trakt/TraktLookup.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/trakt/TraktRatingCollection.py` & `plextraktsync-0.30.9/plextraktsync/trakt/TraktRatingCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/trakt/TraktUserList.py` & `plextraktsync-0.30.9/plextraktsync/trakt/TraktUserList.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/trakt/TraktUserListCollection.py` & `plextraktsync-0.30.9/plextraktsync/trakt/TraktUserListCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/trakt/TraktWatchlist.py` & `plextraktsync-0.30.9/plextraktsync/trakt/TraktWatchlist.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/trakt/WatchProgress.py` & `plextraktsync-0.30.9/plextraktsync/trakt/WatchProgress.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/util/Factory.py` & `plextraktsync-0.30.9/plextraktsync/util/Factory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/util/Path.py` & `plextraktsync-0.30.9/plextraktsync/util/Path.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/util/Rating.py` & `plextraktsync-0.30.9/plextraktsync/util/Rating.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/util/Timer.py` & `plextraktsync-0.30.9/plextraktsync/util/Timer.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/util/Version.py` & `plextraktsync-0.30.9/plextraktsync/util/Version.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/util/local_url.py` & `plextraktsync-0.30.9/plextraktsync/util/local_url.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/util/openurl.py` & `plextraktsync-0.30.9/plextraktsync/util/openurl.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/util/packaging.py` & `plextraktsync-0.30.9/plextraktsync/util/packaging.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/util/remove_empty_values.py` & `plextraktsync-0.30.9/plextraktsync/util/remove_empty_values.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/watch/EventDispatcher.py` & `plextraktsync-0.30.9/plextraktsync/watch/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/watch/EventFactory.py` & `plextraktsync-0.30.9/plextraktsync/watch/EventFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/watch/ProgressBar.py` & `plextraktsync-0.30.9/plextraktsync/watch/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/watch/WatchStateUpdater.py` & `plextraktsync-0.30.9/plextraktsync/watch/WatchStateUpdater.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/watch/WebSocketListener.py` & `plextraktsync-0.30.9/plextraktsync/watch/WebSocketListener.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/plextraktsync/watch/events.py` & `plextraktsync-0.30.9/plextraktsync/watch/events.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/requirements.txt` & `plextraktsync-0.30.9/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 idna==3.7; python_version >= '3.5'
 inquirerpy==0.3.4; python_version >= '3.7' and python_version < '4.0'
 markdown-it-py==3.0.0; python_version >= '3.7' and python_version >= '3.8'
 mdurl==0.1.2; python_version >= '3.7'
 oauthlib==3.2.2; python_version >= '3.6'
 pfzy==0.3.4; python_version >= '3.7' and python_version < '4.0'
 platformdirs==4.2.2; python_version >= '3.8'
-plexapi==4.15.12; python_version >= '3.8'
+plexapi==4.15.13; python_version >= '3.8'
 pluggy==1.5.0; python_version >= '3.8'
 prompt-toolkit==3.0.43; python_full_version >= '3.7.0'
 pygments==2.18.0; python_version >= '3.8'
 python-dotenv==1.0.1; python_version >= '3.8'
 python-git-info==0.8.3
 pytimeparse==1.1.8
 pytrakt==3.4.32
 pyyaml==6.0.1; python_version >= '3.6'
-requests==2.31.0; python_version >= '3.7'
+requests==2.32.0; python_version >= '3.8'
 requests-cache==1.2.0; python_version >= '3.8'
 requests-oauthlib==2.0.0; python_version >= '3.4'
 rich==13.7.1; python_full_version >= '3.7.0'
 six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3' and python_version >= '3.4'
 tqdm==4.66.4; python_version >= '3.7'
 types-decorator==5.1.8.20240310; python_version >= '3.8'
 typing-extensions==4.11.0; python_version < '3.9'
```

### Comparing `plextraktsync-0.30.8/setup.cfg` & `plextraktsync-0.30.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/tests/test_collection_metadata.py` & `plextraktsync-0.30.9/tests/test_collection_metadata.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/tests/test_config.py` & `plextraktsync-0.30.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/tests/test_events.py` & `plextraktsync-0.30.9/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/tests/test_new_agent.py` & `plextraktsync-0.30.9/tests/test_new_agent.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/tests/test_plex_id.py` & `plextraktsync-0.30.9/tests/test_plex_id.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/tests/test_rating.py` & `plextraktsync-0.30.9/tests/test_rating.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/tests/test_timer.py` & `plextraktsync-0.30.9/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/tests/test_trakt_progress.py` & `plextraktsync-0.30.9/tests/test_trakt_progress.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/tests/test_tv_lookup.py` & `plextraktsync-0.30.9/tests/test_tv_lookup.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.8/tests/test_walker.py` & `plextraktsync-0.30.9/tests/test_walker.py`

 * *Files identical despite different names*

