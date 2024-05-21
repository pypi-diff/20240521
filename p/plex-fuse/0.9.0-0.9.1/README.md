# Comparing `tmp/plex_fuse-0.9.0.tar.gz` & `tmp/plex_fuse-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex_fuse-0.9.0.tar", last modified: Sun May 12 09:52:58 2024, max compression
+gzip compressed data, was "plex_fuse-0.9.1.tar", last modified: Tue May 21 17:41:23 2024, max compression
```

## Comparing `plex_fuse-0.9.0.tar` & `plex_fuse-0.9.1.tar`

### file list

```diff
@@ -1,69 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:52:58.125071 plex_fuse-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-12 09:52:58.125071 plex_fuse-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:52:58.125071 plex_fuse-0.9.0/plex_fuse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-12 09:52:58.000000 plex_fuse-0.9.0/plex_fuse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-12 09:52:58.000000 plex_fuse-0.9.0/plex_fuse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 09:52:58.000000 plex_fuse-0.9.0/plex_fuse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-12 09:52:58.000000 plex_fuse-0.9.0/plex_fuse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-12 09:52:58.000000 plex_fuse-0.9.0/plex_fuse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-12 09:52:58.000000 plex_fuse-0.9.0/plex_fuse.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:52:58.117071 plex_fuse-0.9.0/plexfuse/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/TimeoutLock.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-12 09:52:53.000000 plex_fuse-0.9.0/plexfuse/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:52:58.117071 plex_fuse-0.9.0/plexfuse/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/cache/CacheControl.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/cache/CachedPropertyCacheControl.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/cache/DelayedPropertyCacheControl.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/cache/FileCache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/cache/HttpCache.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/cache/UserDictCacheControl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:52:58.117071 plex_fuse-0.9.0/plexfuse/control/
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/control/Control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/control/ControlListener.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/control/ControlVFS.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:52:58.121071 plex_fuse-0.9.0/plexfuse/fs/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/fs/FsOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/fs/PlexDirectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/fs/PlexFS.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/fs/PlexFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/fs/RefCountedDict.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/fs/Timestampable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/fs/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/fs/plex_errno.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/measure_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:52:58.121071 plex_fuse-0.9.0/plexfuse/plex/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/plex/Monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/plex/PlexApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/plex/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:52:58.121071 plex_fuse-0.9.0/plexfuse/vfs/
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/vfs/ChunkedFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/vfs/Playable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/vfs/PlexVFS.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:52:58.121071 plex_fuse-0.9.0/plexfuse/vfs/entry/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/vfs/entry/AttrEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/vfs/entry/ControlSockEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/vfs/entry/DirEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/vfs/entry/EpisodeEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/vfs/entry/FileEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/vfs/entry/LibraryEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/vfs/entry/MovieEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/vfs/entry/PathEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/vfs/entry/PlexMatchEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/vfs/entry/SeasonEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/vfs/entry/SectionEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/vfs/entry/SubtitleEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/plexfuse/vfs/entry/SymlinkEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 09:52:58.125071 plex_fuse-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:52:58.125071 plex_fuse-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/tests/test_RefCountedDict.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/tests/test_chunk_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/tests/test_chunk_read.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/tests/test_file_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/tests/test_file_copy_partial.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/tests/test_socket_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-12 09:52:52.000000 plex_fuse-0.9.0/tests/test_timeout_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:41:23.894209 plex_fuse-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-21 17:41:23.894209 plex_fuse-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:41:23.894209 plex_fuse-0.9.1/plex_fuse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-21 17:41:23.000000 plex_fuse-0.9.1/plex_fuse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-21 17:41:23.000000 plex_fuse-0.9.1/plex_fuse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 17:41:23.000000 plex_fuse-0.9.1/plex_fuse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-21 17:41:23.000000 plex_fuse-0.9.1/plex_fuse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-21 17:41:23.000000 plex_fuse-0.9.1/plex_fuse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 17:41:23.000000 plex_fuse-0.9.1/plex_fuse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:41:23.886209 plex_fuse-0.9.1/plexfuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/TimeoutLock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:41:23.886209 plex_fuse-0.9.1/plexfuse/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/cache/CacheControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/cache/CachedPropertyCacheControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/cache/DelayedPropertyCacheControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/cache/FileCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/cache/HttpCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/cache/UserDictCacheControl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:41:23.890209 plex_fuse-0.9.1/plexfuse/control/
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/control/Control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/control/ControlListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/control/ControlVFS.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:41:23.890209 plex_fuse-0.9.1/plexfuse/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/fs/FsOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/fs/PlexDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/fs/PlexFS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/fs/PlexFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/fs/RefCountedDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/fs/Timestampable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/fs/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/fs/plex_errno.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/fs/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/measure_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:41:23.890209 plex_fuse-0.9.1/plexfuse/plex/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/plex/Monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/plex/PlexApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/plex/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:41:23.890209 plex_fuse-0.9.1/plexfuse/sentry/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/sentry/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:41:23.890209 plex_fuse-0.9.1/plexfuse/vfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/vfs/ChunkedFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/vfs/Playable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/vfs/PlexVFS.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:41:23.894209 plex_fuse-0.9.1/plexfuse/vfs/entry/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/vfs/entry/AttrEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/vfs/entry/ControlSockEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/vfs/entry/DirEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/vfs/entry/EpisodeEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/vfs/entry/FileEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/vfs/entry/LibraryEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/vfs/entry/MovieEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/vfs/entry/PathEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/vfs/entry/PlexMatchEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/vfs/entry/SeasonEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/vfs/entry/SectionEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/vfs/entry/SubtitleEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/plexfuse/vfs/entry/SymlinkEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 17:41:23.894209 plex_fuse-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:41:23.894209 plex_fuse-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/tests/test_RefCountedDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/tests/test_chunk_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/tests/test_chunk_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/tests/test_file_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/tests/test_file_copy_partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/tests/test_socket_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-21 17:41:20.000000 plex_fuse-0.9.1/tests/test_timeout_lock.py
```

### Comparing `plex_fuse-0.9.0/LICENSE` & `plex_fuse-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/PKG-INFO` & `plex_fuse-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-fuse
-Version: 0.9.0
+Version: 0.9.1
 Summary: Plex FUSE Filesystem - Mount Remote Plex Media Server contents as local filesystem
 Author-email: Elan Ruusamäe <glen@pld-linux.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Elan Ruusamäe
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `plex_fuse-0.9.0/README.md` & `plex_fuse-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plex_fuse.egg-info/PKG-INFO` & `plex_fuse-0.9.1/plex_fuse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-fuse
-Version: 0.9.0
+Version: 0.9.1
 Summary: Plex FUSE Filesystem - Mount Remote Plex Media Server contents as local filesystem
 Author-email: Elan Ruusamäe <glen@pld-linux.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Elan Ruusamäe
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `plex_fuse-0.9.0/plex_fuse.egg-info/SOURCES.txt` & `plex_fuse-0.9.1/plex_fuse.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -25,17 +25,20 @@
 plexfuse/fs/PlexDirectory.py
 plexfuse/fs/PlexFS.py
 plexfuse/fs/PlexFile.py
 plexfuse/fs/RefCountedDict.py
 plexfuse/fs/Timestampable.py
 plexfuse/fs/main.py
 plexfuse/fs/plex_errno.py
+plexfuse/fs/retry.py
 plexfuse/plex/Monitor.py
 plexfuse/plex/PlexApi.py
 plexfuse/plex/types.py
+plexfuse/sentry/__init__.py
+plexfuse/sentry/sentry.py
 plexfuse/vfs/ChunkedFile.py
 plexfuse/vfs/Playable.py
 plexfuse/vfs/PlexVFS.py
 plexfuse/vfs/entry/AttrEntry.py
 plexfuse/vfs/entry/ControlSockEntry.py
 plexfuse/vfs/entry/DirEntry.py
 plexfuse/vfs/entry/EpisodeEntry.py
```

### Comparing `plex_fuse-0.9.0/plexfuse/TimeoutLock.py` & `plex_fuse-0.9.1/plexfuse/TimeoutLock.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/cache/CacheControl.py` & `plex_fuse-0.9.1/plexfuse/cache/CacheControl.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/cache/CachedPropertyCacheControl.py` & `plex_fuse-0.9.1/plexfuse/cache/CachedPropertyCacheControl.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/cache/DelayedPropertyCacheControl.py` & `plex_fuse-0.9.1/plexfuse/cache/DelayedPropertyCacheControl.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/cache/FileCache.py` & `plex_fuse-0.9.1/plexfuse/cache/FileCache.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/cache/HttpCache.py` & `plex_fuse-0.9.1/plexfuse/cache/HttpCache.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/cache/UserDictCacheControl.py` & `plex_fuse-0.9.1/plexfuse/cache/UserDictCacheControl.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/control/Control.py` & `plex_fuse-0.9.1/plexfuse/control/Control.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/control/ControlListener.py` & `plex_fuse-0.9.1/plexfuse/control/ControlListener.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/control/ControlVFS.py` & `plex_fuse-0.9.1/plexfuse/control/ControlVFS.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/fs/PlexFS.py` & `plex_fuse-0.9.1/plexfuse/fs/PlexFS.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from plexfuse.control.Control import Control
 from plexfuse.control.ControlListener import ControlListener
 from plexfuse.fs.FsOptions import FsOptions
 from plexfuse.fs.plex_errno import plex_errno
 from plexfuse.fs.PlexDirectory import PlexDirectory
 from plexfuse.fs.PlexFile import PlexFile
 from plexfuse.fs.RefCountedDict import RefCountedDict
+from plexfuse.fs.retry import retry
 from plexfuse.normalize import normalize
 from plexfuse.plex.Monitor import Monitor
 from plexfuse.plex.PlexApi import PlexApi
 from plexfuse.sentry import sentry
 from plexfuse.TimeoutLock import TimeoutLock
 from plexfuse.vfs.entry.DirEntry import DirEntry
 from plexfuse.vfs.PlexVFS import PlexVFS
@@ -103,14 +104,15 @@
         except KeyError as e:
             print(f"ERROR: readdir({path}): {e}")
             return
 
         for r in it:
             yield fuse.Direntry(r)
 
+    @retry(retries=5, delay=1, fail=errno.EBADF)
     def read(self, path, size, offset):
         with self.iolock:
             entry = self.file_map[path]
 
             return entry.read(offset, size)
 
     def release(self, path, flags):
```

### Comparing `plex_fuse-0.9.0/plexfuse/fs/RefCountedDict.py` & `plex_fuse-0.9.1/plexfuse/fs/RefCountedDict.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/fs/main.py` & `plex_fuse-0.9.1/plexfuse/fs/main.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/fs/plex_errno.py` & `plex_fuse-0.9.1/plexfuse/fs/plex_errno.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/measure_speed.py` & `plex_fuse-0.9.1/plexfuse/measure_speed.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/plex/Monitor.py` & `plex_fuse-0.9.1/plexfuse/plex/Monitor.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/plex/PlexApi.py` & `plex_fuse-0.9.1/plexfuse/plex/PlexApi.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/vfs/ChunkedFile.py` & `plex_fuse-0.9.1/plexfuse/vfs/ChunkedFile.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/vfs/Playable.py` & `plex_fuse-0.9.1/plexfuse/vfs/Playable.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/vfs/PlexVFS.py` & `plex_fuse-0.9.1/plexfuse/vfs/PlexVFS.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/vfs/entry/FileEntry.py` & `plex_fuse-0.9.1/plexfuse/vfs/entry/FileEntry.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/vfs/entry/LibraryEntry.py` & `plex_fuse-0.9.1/plexfuse/vfs/entry/LibraryEntry.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/vfs/entry/PlexMatchEntry.py` & `plex_fuse-0.9.1/plexfuse/vfs/entry/PlexMatchEntry.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/vfs/entry/SectionEntry.py` & `plex_fuse-0.9.1/plexfuse/vfs/entry/SectionEntry.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/plexfuse/vfs/entry/SubtitleEntry.py` & `plex_fuse-0.9.1/plexfuse/vfs/entry/SubtitleEntry.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/pyproject.toml` & `plex_fuse-0.9.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -53,10 +53,11 @@
 [tool.setuptools]
 packages = [
 	"plexfuse",
 	"plexfuse.cache",
 	"plexfuse.control",
 	"plexfuse.fs",
 	"plexfuse.plex",
+	"plexfuse.sentry",
 	"plexfuse.vfs",
 	"plexfuse.vfs.entry"
 ]
```

### Comparing `plex_fuse-0.9.0/tests/test_RefCountedDict.py` & `plex_fuse-0.9.1/tests/test_RefCountedDict.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/tests/test_chunk_calc.py` & `plex_fuse-0.9.1/tests/test_chunk_calc.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/tests/test_chunk_read.py` & `plex_fuse-0.9.1/tests/test_chunk_read.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/tests/test_file_copy_partial.py` & `plex_fuse-0.9.1/tests/test_file_copy_partial.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/tests/test_socket_control.py` & `plex_fuse-0.9.1/tests/test_socket_control.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.9.0/tests/test_timeout_lock.py` & `plex_fuse-0.9.1/tests/test_timeout_lock.py`

 * *Files identical despite different names*

