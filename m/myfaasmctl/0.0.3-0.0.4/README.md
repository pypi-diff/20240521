# Comparing `tmp/myfaasmctl-0.0.3.tar.gz` & `tmp/myfaasmctl-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myfaasmctl-0.0.3.tar", last modified: Tue May 14 12:39:58 2024, max compression
+gzip compressed data, was "myfaasmctl-0.0.4.tar", last modified: Tue May 21 14:32:09 2024, max compression
```

## Comparing `myfaasmctl-0.0.3.tar` & `myfaasmctl-0.0.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:39:58.788933 myfaasmctl-0.0.3/
--rw-r--r--   0 root         (0) root         (0)    11343 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1341 2024-05-14 12:39:58.788933 myfaasmctl-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      777 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:39:58.780933 myfaasmctl-0.0.3/faasmctl/
--rw-r--r--   0 root         (0) root         (0)       55 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:39:58.780933 myfaasmctl-0.0.3/faasmctl/bin/
--rwxr-xr-x   0 root         (0) root         (0)     3438 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/bin/gen_proto_files.py
--rw-r--r--   0 root         (0) root         (0)      314 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:39:58.784933 myfaasmctl-0.0.3/faasmctl/tasks/
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5688 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/tasks/cli.py
--rw-r--r--   0 root         (0) root         (0)      823 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/tasks/delete.py
--rw-r--r--   0 root         (0) root         (0)     3524 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/tasks/deploy.py
--rw-r--r--   0 root         (0) root         (0)      656 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/tasks/flush.py
--rw-r--r--   0 root         (0) root         (0)      395 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/tasks/generate.py
--rw-r--r--   0 root         (0) root         (0)     3454 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/tasks/invoke.py
--rw-r--r--   0 root         (0) root         (0)     2192 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/tasks/logs.py
--rw-r--r--   0 root         (0) root         (0)    10483 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/tasks/monitor.py
--rw-r--r--   0 root         (0) root         (0)     1373 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/tasks/restart.py
--rw-r--r--   0 root         (0) root         (0)     1577 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/tasks/scale.py
--rw-r--r--   0 root         (0) root         (0)      808 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/tasks/status.py
--rw-r--r--   0 root         (0) root         (0)     1346 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/tasks/upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:39:58.784933 myfaasmctl-0.0.3/faasmctl/util/
--rw-r--r--   0 root         (0) root         (0)       48 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/util/backend.py
--rw-r--r--   0 root         (0) root         (0)      475 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/util/batch.py
--rw-r--r--   0 root         (0) root         (0)    14750 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/util/compose.py
--rw-r--r--   0 root         (0) root         (0)     2464 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/util/config.py
--rw-r--r--   0 root         (0) root         (0)     5855 2024-05-14 11:39:12.000000 myfaasmctl-0.0.3/faasmctl/util/deploy.py
--rw-r--r--   0 root         (0) root         (0)     1698 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/util/docker.py
--rw-r--r--   0 root         (0) root         (0)      471 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/util/env.py
--rw-r--r--   0 root         (0) root         (0)      670 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/util/faasm.py
--rw-r--r--   0 root         (0) root         (0)     1069 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/util/flush.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:39:58.788933 myfaasmctl-0.0.3/faasmctl/util/gen_proto/
--rw-r--r--   0 root         (0) root         (0)     8690 2024-05-10 02:54:00.000000 myfaasmctl-0.0.3/faasmctl/util/gen_proto/faabric_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5799 2024-05-10 02:54:00.000000 myfaasmctl-0.0.3/faasmctl/util/gen_proto/planner_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5795 2024-05-10 02:57:43.000000 myfaasmctl-0.0.3/faasmctl/util/invoke.py
--rw-r--r--   0 root         (0) root         (0)    11303 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/util/k8s.py
--rw-r--r--   0 root         (0) root         (0)      358 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/util/message.py
--rw-r--r--   0 root         (0) root         (0)     1094 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/util/network.py
--rw-r--r--   0 root         (0) root         (0)     6569 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/util/planner.py
--rw-r--r--   0 root         (0) root         (0)      138 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/util/random.py
--rw-r--r--   0 root         (0) root         (0)      688 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/util/restart.py
--rw-r--r--   0 root         (0) root         (0)     1371 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/util/results.py
--rw-r--r--   0 root         (0) root         (0)      137 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/util/time.py
--rw-r--r--   0 root         (0) root         (0)     2017 2024-05-10 02:02:06.000000 myfaasmctl-0.0.3/faasmctl/util/upload.py
--rw-r--r--   0 root         (0) root         (0)       76 2024-05-10 02:58:15.000000 myfaasmctl-0.0.3/faasmctl/util/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 12:39:58.788933 myfaasmctl-0.0.3/myfaasmctl.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1341 2024-05-14 12:39:58.000000 myfaasmctl-0.0.3/myfaasmctl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1200 2024-05-14 12:39:58.000000 myfaasmctl-0.0.3/myfaasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 12:39:58.000000 myfaasmctl-0.0.3/myfaasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-05-14 12:39:58.000000 myfaasmctl-0.0.3/myfaasmctl.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-05-14 12:39:58.000000 myfaasmctl-0.0.3/myfaasmctl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-14 12:39:58.000000 myfaasmctl-0.0.3/myfaasmctl.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      692 2024-05-14 11:39:44.000000 myfaasmctl-0.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       90 2024-05-14 12:39:58.788933 myfaasmctl-0.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:32:09.022449 myfaasmctl-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)    11343 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1341 2024-05-21 14:32:09.022449 myfaasmctl-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      777 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:32:09.014449 myfaasmctl-0.0.4/faasmctl/
+-rw-r--r--   0 root         (0) root         (0)       55 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:32:09.014449 myfaasmctl-0.0.4/faasmctl/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     3438 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/bin/gen_proto_files.py
+-rw-r--r--   0 root         (0) root         (0)      314 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:32:09.018449 myfaasmctl-0.0.4/faasmctl/tasks/
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5688 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/cli.py
+-rw-r--r--   0 root         (0) root         (0)      823 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/delete.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/deploy.py
+-rw-r--r--   0 root         (0) root         (0)      656 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/flush.py
+-rw-r--r--   0 root         (0) root         (0)      395 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/generate.py
+-rw-r--r--   0 root         (0) root         (0)     3454 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/invoke.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/logs.py
+-rw-r--r--   0 root         (0) root         (0)    10483 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/monitor.py
+-rw-r--r--   0 root         (0) root         (0)     1373 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/restart.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/scale.py
+-rw-r--r--   0 root         (0) root         (0)      808 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/status.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:32:09.018449 myfaasmctl-0.0.4/faasmctl/util/
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/backend.py
+-rw-r--r--   0 root         (0) root         (0)      475 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/batch.py
+-rw-r--r--   0 root         (0) root         (0)    14750 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/compose.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/config.py
+-rw-r--r--   0 root         (0) root         (0)     5829 2024-05-21 14:28:54.000000 myfaasmctl-0.0.4/faasmctl/util/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/docker.py
+-rw-r--r--   0 root         (0) root         (0)      471 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/env.py
+-rw-r--r--   0 root         (0) root         (0)      670 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/faasm.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/flush.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:32:09.018449 myfaasmctl-0.0.4/faasmctl/util/gen_proto/
+-rw-r--r--   0 root         (0) root         (0)     8690 2024-05-10 02:54:00.000000 myfaasmctl-0.0.4/faasmctl/util/gen_proto/faabric_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5799 2024-05-10 02:54:00.000000 myfaasmctl-0.0.4/faasmctl/util/gen_proto/planner_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5795 2024-05-10 02:57:43.000000 myfaasmctl-0.0.4/faasmctl/util/invoke.py
+-rw-r--r--   0 root         (0) root         (0)    11303 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/k8s.py
+-rw-r--r--   0 root         (0) root         (0)      358 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/message.py
+-rw-r--r--   0 root         (0) root         (0)     1094 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/network.py
+-rw-r--r--   0 root         (0) root         (0)     6569 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/planner.py
+-rw-r--r--   0 root         (0) root         (0)      138 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/random.py
+-rw-r--r--   0 root         (0) root         (0)      688 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/restart.py
+-rw-r--r--   0 root         (0) root         (0)     1371 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/results.py
+-rw-r--r--   0 root         (0) root         (0)      137 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/time.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/upload.py
+-rw-r--r--   0 root         (0) root         (0)       76 2024-05-10 02:58:15.000000 myfaasmctl-0.0.4/faasmctl/util/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:32:09.022449 myfaasmctl-0.0.4/myfaasmctl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1341 2024-05-21 14:32:09.000000 myfaasmctl-0.0.4/myfaasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-05-21 14:32:09.000000 myfaasmctl-0.0.4/myfaasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 14:32:09.000000 myfaasmctl-0.0.4/myfaasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-21 14:32:09.000000 myfaasmctl-0.0.4/myfaasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-21 14:32:09.000000 myfaasmctl-0.0.4/myfaasmctl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-21 14:32:09.000000 myfaasmctl-0.0.4/myfaasmctl.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      692 2024-05-21 14:31:40.000000 myfaasmctl-0.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       90 2024-05-21 14:32:09.022449 myfaasmctl-0.0.4/setup.cfg
```

### Comparing `myfaasmctl-0.0.3/LICENSE.md` & `myfaasmctl-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/PKG-INFO` & `myfaasmctl-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfaasmctl
-Version: 0.0.3
+Version: 0.0.4
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `myfaasmctl-0.0.3/README.md` & `myfaasmctl-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/bin/gen_proto_files.py` & `myfaasmctl-0.0.4/faasmctl/bin/gen_proto_files.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/tasks/cli.py` & `myfaasmctl-0.0.4/faasmctl/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/tasks/delete.py` & `myfaasmctl-0.0.4/faasmctl/tasks/delete.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/tasks/deploy.py` & `myfaasmctl-0.0.4/faasmctl/tasks/deploy.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/tasks/flush.py` & `myfaasmctl-0.0.4/faasmctl/tasks/flush.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/tasks/invoke.py` & `myfaasmctl-0.0.4/faasmctl/tasks/invoke.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/tasks/logs.py` & `myfaasmctl-0.0.4/faasmctl/tasks/logs.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/tasks/monitor.py` & `myfaasmctl-0.0.4/faasmctl/tasks/monitor.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/tasks/restart.py` & `myfaasmctl-0.0.4/faasmctl/tasks/restart.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/tasks/scale.py` & `myfaasmctl-0.0.4/faasmctl/tasks/scale.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/tasks/status.py` & `myfaasmctl-0.0.4/faasmctl/tasks/status.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/tasks/upload.py` & `myfaasmctl-0.0.4/faasmctl/tasks/upload.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/util/compose.py` & `myfaasmctl-0.0.4/faasmctl/util/compose.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/util/config.py` & `myfaasmctl-0.0.4/faasmctl/util/config.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/util/deploy.py` & `myfaasmctl-0.0.4/faasmctl/util/deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     # Ensure a clean clone directory
     rmtree(checkout_path, ignore_errors=True)
     makedirs(checkout_path, exist_ok=True)
 
     print("Checking out Faasm v{} to {}".format(get_faasm_version(), checkout_path))
     git_cmd = [
         "git clone",
-        "--branch v{}".format(get_faasm_version()),
+        "--branch state",
         "https://github.com/PancakeTY/faasm",
         checkout_path,
     ]
     git_cmd = " ".join(git_cmd)
     try:
         run(git_cmd, shell=True, check=True)
     except CalledProcessError as e:
```

### Comparing `myfaasmctl-0.0.3/faasmctl/util/docker.py` & `myfaasmctl-0.0.4/faasmctl/util/docker.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/util/faasm.py` & `myfaasmctl-0.0.4/faasmctl/util/faasm.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/util/flush.py` & `myfaasmctl-0.0.4/faasmctl/util/flush.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/util/gen_proto/faabric_pb2.py` & `myfaasmctl-0.0.4/faasmctl/util/gen_proto/faabric_pb2.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/util/gen_proto/planner_pb2.py` & `myfaasmctl-0.0.4/faasmctl/util/gen_proto/planner_pb2.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/util/invoke.py` & `myfaasmctl-0.0.4/faasmctl/util/invoke.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/util/k8s.py` & `myfaasmctl-0.0.4/faasmctl/util/k8s.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/util/network.py` & `myfaasmctl-0.0.4/faasmctl/util/network.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/util/planner.py` & `myfaasmctl-0.0.4/faasmctl/util/planner.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/util/restart.py` & `myfaasmctl-0.0.4/faasmctl/util/restart.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/util/results.py` & `myfaasmctl-0.0.4/faasmctl/util/results.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/faasmctl/util/upload.py` & `myfaasmctl-0.0.4/faasmctl/util/upload.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/myfaasmctl.egg-info/PKG-INFO` & `myfaasmctl-0.0.4/myfaasmctl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfaasmctl
-Version: 0.0.3
+Version: 0.0.4
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `myfaasmctl-0.0.3/myfaasmctl.egg-info/SOURCES.txt` & `myfaasmctl-0.0.4/myfaasmctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.3/pyproject.toml` & `myfaasmctl-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "myfaasmctl"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
 description = "Command line tool to deploy, manage, and interact with Faasm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

