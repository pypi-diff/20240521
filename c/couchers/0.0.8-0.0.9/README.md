# Comparing `tmp/couchers-0.0.8.tar.gz` & `tmp/couchers-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "couchers-0.0.8.tar", last modified: Tue Jul  6 17:20:34 2021, max compression
+gzip compressed data, was "couchers-0.0.9.tar", last modified: Tue Jul  6 17:23:56 2021, max compression
```

## Comparing `couchers-0.0.8.tar` & `couchers-0.0.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 aapeli     (501) staff       (20)        0 2021-07-06 17:20:34.851996 couchers-0.0.8/
--rw-r--r--   0 aapeli     (501) staff       (20)     1189 2021-07-06 17:20:34.852275 couchers-0.0.8/PKG-INFO
--rw-r--r--   0 aapeli     (501) staff       (20)     1105 2021-06-16 16:50:45.000000 couchers-0.0.8/license.md
--rw-r--r--   0 aapeli     (501) staff       (20)      242 2021-07-06 15:14:19.000000 couchers-0.0.8/pyproject.toml
--rw-r--r--   0 aapeli     (501) staff       (20)       77 2021-07-06 17:20:34.853663 couchers-0.0.8/setup.cfg
--rw-r--r--   0 aapeli     (501) staff       (20)     1434 2021-07-06 17:20:27.000000 couchers-0.0.8/setup.py
-drwxr-xr-x   0 aapeli     (501) staff       (20)        0 2021-07-06 17:20:34.817065 couchers-0.0.8/src/
-drwxr-xr-x   0 aapeli     (501) staff       (20)        0 2021-07-06 17:20:34.819213 couchers-0.0.8/src/couchers/
--rw-r--r--   0 aapeli     (501) staff       (20)        0 2021-07-06 17:20:15.000000 couchers-0.0.8/src/couchers/__init__.py
--rw-r--r--   0 aapeli     (501) staff       (20)     2017 2021-07-06 17:20:17.000000 couchers-0.0.8/src/couchers/client.py
-drwxr-xr-x   0 aapeli     (501) staff       (20)        0 2021-07-06 17:20:34.851300 couchers-0.0.8/src/couchers/proto/
--rw-r--r--   0 aapeli     (501) staff       (20)        0 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/__init__.py
--rw-r--r--   0 aapeli     (501) staff       (20)    22921 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/account_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)    13163 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/account_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)    14761 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/admin_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)     8787 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/admin_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)     3936 2021-07-06 17:03:57.000000 couchers-0.0.8/src/couchers/proto/annotations_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)      147 2021-07-06 17:03:56.000000 couchers-0.0.8/src/couchers/proto/annotations_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)   114430 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/api_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)    18235 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/api_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)    38640 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/auth_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)    19759 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/auth_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)     6829 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/blocking_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)     5735 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/blocking_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)     9431 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/bugs_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)     3896 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/bugs_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)    62618 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/communities_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)    22122 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/communities_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)    81369 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/conversations_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)    25778 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/conversations_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)    14091 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/discussions_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)     4101 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/discussions_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)    89792 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/events_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)    24418 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/events_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)     3786 2021-07-06 17:03:58.000000 couchers-0.0.8/src/couchers/proto/gis_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)     7343 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/gis_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)    53787 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/groups_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)    16347 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/groups_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)     8873 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/jail_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)     5880 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/jail_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)     8512 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/media_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)     2683 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/media_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)    42823 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/pages_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)    11236 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/pages_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)    29684 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/references_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)     9842 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/references_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)    41712 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/requests_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)    14609 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/requests_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)    10509 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/resources_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)     5969 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/resources_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)    37760 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/search_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)     3872 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/search_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)    14469 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/threads_pb2.py
--rw-r--r--   0 aapeli     (501) staff       (20)     4567 2021-07-06 17:03:53.000000 couchers-0.0.8/src/couchers/proto/threads_pb2_grpc.py
--rw-r--r--   0 aapeli     (501) staff       (20)     1572 2021-07-06 17:03:10.000000 couchers-0.0.8/src/couchers/services.py
-drwxr-xr-x   0 aapeli     (501) staff       (20)        0 2021-07-06 17:20:34.820770 couchers-0.0.8/src/couchers.egg-info/
--rw-r--r--   0 aapeli     (501) staff       (20)     1189 2021-07-06 17:20:34.000000 couchers-0.0.8/src/couchers.egg-info/PKG-INFO
--rw-r--r--   0 aapeli     (501) staff       (20)     1858 2021-07-06 17:20:34.000000 couchers-0.0.8/src/couchers.egg-info/SOURCES.txt
--rw-r--r--   0 aapeli     (501) staff       (20)        1 2021-07-06 17:20:34.000000 couchers-0.0.8/src/couchers.egg-info/dependency_links.txt
--rw-r--r--   0 aapeli     (501) staff       (20)       16 2021-07-06 17:20:34.000000 couchers-0.0.8/src/couchers.egg-info/requires.txt
--rw-r--r--   0 aapeli     (501) staff       (20)        9 2021-07-06 17:20:34.000000 couchers-0.0.8/src/couchers.egg-info/top_level.txt
+drwxr-xr-x   0 aapeli     (501) staff       (20)        0 2021-07-06 17:23:56.753417 couchers-0.0.9/
+-rw-r--r--   0 aapeli     (501) staff       (20)     1189 2021-07-06 17:23:56.753755 couchers-0.0.9/PKG-INFO
+-rw-r--r--   0 aapeli     (501) staff       (20)     1105 2021-06-16 16:50:45.000000 couchers-0.0.9/license.md
+-rw-r--r--   0 aapeli     (501) staff       (20)      242 2021-07-06 15:14:19.000000 couchers-0.0.9/pyproject.toml
+-rw-r--r--   0 aapeli     (501) staff       (20)       77 2021-07-06 17:23:56.755188 couchers-0.0.9/setup.cfg
+-rw-r--r--   0 aapeli     (501) staff       (20)     1434 2021-07-06 17:23:44.000000 couchers-0.0.9/setup.py
+drwxr-xr-x   0 aapeli     (501) staff       (20)        0 2021-07-06 17:23:56.726736 couchers-0.0.9/src/
+drwxr-xr-x   0 aapeli     (501) staff       (20)        0 2021-07-06 17:23:56.728516 couchers-0.0.9/src/couchers/
+-rw-r--r--   0 aapeli     (501) staff       (20)       31 2021-07-06 17:21:55.000000 couchers-0.0.9/src/couchers/__init__.py
+-rw-r--r--   0 aapeli     (501) staff       (20)     2017 2021-07-06 17:20:17.000000 couchers-0.0.9/src/couchers/client.py
+drwxr-xr-x   0 aapeli     (501) staff       (20)        0 2021-07-06 17:23:56.752729 couchers-0.0.9/src/couchers/proto/
+-rw-r--r--   0 aapeli     (501) staff       (20)        0 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/__init__.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    22921 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/account_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    13163 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/account_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    14761 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/admin_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)     8787 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/admin_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)     3936 2021-07-06 17:03:57.000000 couchers-0.0.9/src/couchers/proto/annotations_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)      147 2021-07-06 17:03:56.000000 couchers-0.0.9/src/couchers/proto/annotations_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)   114430 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/api_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    18235 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/api_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    38640 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/auth_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    19759 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/auth_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)     6829 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/blocking_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)     5735 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/blocking_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)     9431 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/bugs_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)     3896 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/bugs_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    62618 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/communities_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    22122 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/communities_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    81369 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/conversations_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    25778 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/conversations_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    14091 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/discussions_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)     4101 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/discussions_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    89792 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/events_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    24418 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/events_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)     3786 2021-07-06 17:03:58.000000 couchers-0.0.9/src/couchers/proto/gis_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)     7343 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/gis_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    53787 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/groups_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    16347 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/groups_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)     8873 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/jail_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)     5880 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/jail_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)     8512 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/media_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)     2683 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/media_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    42823 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/pages_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    11236 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/pages_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    29684 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/references_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)     9842 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/references_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    41712 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/requests_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    14609 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/requests_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    10509 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/resources_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)     5969 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/resources_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    37760 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/search_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)     3872 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/search_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)    14469 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/threads_pb2.py
+-rw-r--r--   0 aapeli     (501) staff       (20)     4567 2021-07-06 17:03:53.000000 couchers-0.0.9/src/couchers/proto/threads_pb2_grpc.py
+-rw-r--r--   0 aapeli     (501) staff       (20)     1572 2021-07-06 17:03:10.000000 couchers-0.0.9/src/couchers/services.py
+drwxr-xr-x   0 aapeli     (501) staff       (20)        0 2021-07-06 17:23:56.730045 couchers-0.0.9/src/couchers.egg-info/
+-rw-r--r--   0 aapeli     (501) staff       (20)     1189 2021-07-06 17:23:56.000000 couchers-0.0.9/src/couchers.egg-info/PKG-INFO
+-rw-r--r--   0 aapeli     (501) staff       (20)     1858 2021-07-06 17:23:56.000000 couchers-0.0.9/src/couchers.egg-info/SOURCES.txt
+-rw-r--r--   0 aapeli     (501) staff       (20)        1 2021-07-06 17:23:56.000000 couchers-0.0.9/src/couchers.egg-info/dependency_links.txt
+-rw-r--r--   0 aapeli     (501) staff       (20)       16 2021-07-06 17:23:56.000000 couchers-0.0.9/src/couchers.egg-info/requires.txt
+-rw-r--r--   0 aapeli     (501) staff       (20)        9 2021-07-06 17:23:56.000000 couchers-0.0.9/src/couchers.egg-info/top_level.txt
```

### Comparing `couchers-0.0.8/PKG-INFO` & `couchers-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: couchers
-Version: 0.0.8
+Version: 0.0.9
 Summary: Couchers.org: The next-generation couch surfing platform. Free forever. Community‑led. Non‑profit. Modern.
 Home-page: https://couchers.org
 Author: Couchers.org Foundation and Contributors
 Author-email: support@couchers.org
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/Couchers-org/couchers
 Project-URL: Bug Tracker, https://github.com/Couchers-org/couchers/issues
```

### Comparing `couchers-0.0.8/license.md` & `couchers-0.0.9/license.md`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/setup.py` & `couchers-0.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 This is the Couchers.org Python Client, mainly used for administrative purposes and the like.
 
 Usage of the Couchers.org service provided by the Couchers.org Foundation is governed under our [Terms of Service](https://app.couchers.org/terms).
 """
 
 setuptools.setup(
     name="couchers",
-    version="0.0.8",
+    version="0.0.9",
     author="Couchers.org Foundation and Contributors",
     author_email="support@couchers.org",
     description="Couchers.org: The next-generation couch surfing platform. Free forever. Community‑led. Non‑profit. Modern.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://couchers.org",
     project_urls={
```

### Comparing `couchers-0.0.8/src/couchers/client.py` & `couchers-0.0.9/src/couchers/client.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/account_pb2.py` & `couchers-0.0.9/src/couchers/proto/account_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/account_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/account_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/admin_pb2.py` & `couchers-0.0.9/src/couchers/proto/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/admin_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/admin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/annotations_pb2.py` & `couchers-0.0.9/src/couchers/proto/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/api_pb2.py` & `couchers-0.0.9/src/couchers/proto/api_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/api_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/auth_pb2.py` & `couchers-0.0.9/src/couchers/proto/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/auth_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/blocking_pb2.py` & `couchers-0.0.9/src/couchers/proto/blocking_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/blocking_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/blocking_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/bugs_pb2.py` & `couchers-0.0.9/src/couchers/proto/bugs_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/bugs_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/bugs_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/communities_pb2.py` & `couchers-0.0.9/src/couchers/proto/communities_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/communities_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/communities_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/conversations_pb2.py` & `couchers-0.0.9/src/couchers/proto/conversations_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/conversations_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/conversations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/discussions_pb2.py` & `couchers-0.0.9/src/couchers/proto/discussions_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/discussions_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/discussions_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/events_pb2.py` & `couchers-0.0.9/src/couchers/proto/events_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/events_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/events_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/gis_pb2.py` & `couchers-0.0.9/src/couchers/proto/gis_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/gis_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/gis_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/groups_pb2.py` & `couchers-0.0.9/src/couchers/proto/groups_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/groups_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/groups_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/jail_pb2.py` & `couchers-0.0.9/src/couchers/proto/jail_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/jail_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/jail_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/media_pb2.py` & `couchers-0.0.9/src/couchers/proto/media_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/media_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/media_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/pages_pb2.py` & `couchers-0.0.9/src/couchers/proto/pages_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/pages_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/pages_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/references_pb2.py` & `couchers-0.0.9/src/couchers/proto/references_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/references_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/references_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/requests_pb2.py` & `couchers-0.0.9/src/couchers/proto/requests_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/requests_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/requests_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/resources_pb2.py` & `couchers-0.0.9/src/couchers/proto/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/resources_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/resources_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/search_pb2.py` & `couchers-0.0.9/src/couchers/proto/search_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/search_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/search_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/threads_pb2.py` & `couchers-0.0.9/src/couchers/proto/threads_pb2.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/proto/threads_pb2_grpc.py` & `couchers-0.0.9/src/couchers/proto/threads_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers/services.py` & `couchers-0.0.9/src/couchers/services.py`

 * *Files identical despite different names*

### Comparing `couchers-0.0.8/src/couchers.egg-info/PKG-INFO` & `couchers-0.0.9/src/couchers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: couchers
-Version: 0.0.8
+Version: 0.0.9
 Summary: Couchers.org: The next-generation couch surfing platform. Free forever. Community‑led. Non‑profit. Modern.
 Home-page: https://couchers.org
 Author: Couchers.org Foundation and Contributors
 Author-email: support@couchers.org
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/Couchers-org/couchers
 Project-URL: Bug Tracker, https://github.com/Couchers-org/couchers/issues
```

### Comparing `couchers-0.0.8/src/couchers.egg-info/SOURCES.txt` & `couchers-0.0.9/src/couchers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

